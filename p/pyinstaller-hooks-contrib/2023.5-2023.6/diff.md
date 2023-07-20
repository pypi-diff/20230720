# Comparing `tmp/pyinstaller-hooks-contrib-2023.5.tar.gz` & `tmp/pyinstaller-hooks-contrib-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinstaller-hooks-contrib-2023.5.tar", last modified: Tue Jul  4 23:40:39 2023, max compression
+gzip compressed data, was "pyinstaller-hooks-contrib-2023.6.tar", last modified: Thu Jul 20 12:30:00 2023, max compression
```

## Comparing `pyinstaller-hooks-contrib-2023.5.tar` & `pyinstaller-hooks-contrib-2023.6.tar`

### file list

```diff
@@ -1,409 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/LICENSE.APL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/LICENSE.GPL.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-04 23:40:39.468399 pyinstaller-hooks-contrib-2023.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 23:40:39.468399 pyinstaller-hooks-contrib-2023.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-argon2.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cx_Oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-exchangelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gadfly.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinxed.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.etree.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.objectify.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbt.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-patsy.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-raven.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-redmine.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.lib.utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-web3.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.xrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.420399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    44522 2023-07-04 23:40:28.000000 pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/test_libraries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:40:39.464399 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 23:40:39.000000 pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/LICENSE.APL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/LICENSE.GPL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.184052 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-argon2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cx_Oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-exchangelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gadfly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinxed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.etree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.objectify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-patsy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-redmine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.lib.utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-web3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.xrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.184052 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.120051 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45165 2023-07-20 12:29:39.000000 pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/test_libraries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:30:00.188052 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 12:30:00.000000 pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/top_level.txt
```

### Comparing `pyinstaller-hooks-contrib-2023.5/LICENSE` & `pyinstaller-hooks-contrib-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/LICENSE.APL.txt` & `pyinstaller-hooks-contrib-2023.6/LICENSE.APL.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/LICENSE.GPL.txt` & `pyinstaller-hooks-contrib-2023.6/LICENSE.GPL.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/PKG-INFO` & `pyinstaller-hooks-contrib-2023.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller-hooks-contrib
-Version: 2023.5
+Version: 2023.6
 Summary: Community maintained hooks for PyInstaller
 Home-page: https://github.com/pyinstaller/pyinstaller-hooks-contrib
 Download-URL: https://pypi.org/project/pyinstaller-hooks-contrib
 Maintainer: Legorooj
 Maintainer-email: legorooj@protonmail.com
 Keywords: pyinstaller development hooks
 Classifier: Intended Audience :: Developers
```

### Comparing `pyinstaller-hooks-contrib-2023.5/README.md` & `pyinstaller-hooks-contrib-2023.6/README.md`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/pyproject.toml` & `pyinstaller-hooks-contrib-2023.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/setup.cfg` & `pyinstaller-hooks-contrib-2023.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/setup.py` & `pyinstaller-hooks-contrib-2023.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/__init__.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-__version__ = '2023.5'
+__version__ = '2023.6'
 __maintainer__ = 'Legorooj, bwoodsend'
 __uri__ = 'https://github.com/pyinstaller/pyinstaller-hooks-contrib'
```

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/__init__.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-# This is needed to bundle draft3.json and draft4.json files that come
-# with jsonschema module
+# This is needed to bundle draft3.json and draft4.json files that come with jsonschema module.
+# NOTE: with jsonschema >= 4.18.0, the specification files are part of jsonschema_specifications package, and are
+# handled by the corresponding hook-jsonschema.
 
 from PyInstaller.utils.hooks import collect_data_files, copy_metadata
 
 datas = collect_data_files('jsonschema')
 datas += copy_metadata('jsonschema')
```

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.ops.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.ops.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/__init__.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/conftest.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-hooks-contrib-2023.5/src/_pyinstaller_hooks_contrib/tests/test_libraries.py` & `pyinstaller-hooks-contrib-2023.6/src/_pyinstaller_hooks_contrib/tests/test_libraries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1668,7 +1668,30 @@
 
 
 @importorskip('mistune')
 def test_mistune(pyi_builder):
     pyi_builder.test_source("""
         import mistune
     """)
+
+
+@importorskip('jsonschema')
+def test_jsonschema(pyi_builder):
+    pyi_builder.test_source("""
+        import jsonschema
+
+        # Sample schema
+        schema = {
+            "type" : "object",
+            "properties" : {
+                "price" : {"type" : "number"},
+                "name" : {"type" : "string"},
+            },
+        }
+
+        jsonschema.validate(instance={"name" : "Eggs", "price" : 3.38}, schema=schema)
+
+        try:
+            jsonschema.validate(instance={"name" : "Eggs", "price" : "Invalid"}, schema=schema)
+        except jsonschema.ValidationError as e:
+            print(f"Validation error: {e}")
+    """)
```

### Comparing `pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO` & `pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller-hooks-contrib
-Version: 2023.5
+Version: 2023.6
 Summary: Community maintained hooks for PyInstaller
 Home-page: https://github.com/pyinstaller/pyinstaller-hooks-contrib
 Download-URL: https://pypi.org/project/pyinstaller-hooks-contrib
 Maintainer: Legorooj
 Maintainer-email: legorooj@protonmail.com
 Keywords: pyinstaller development hooks
 Classifier: Intended Audience :: Developers
```

### Comparing `pyinstaller-hooks-contrib-2023.5/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt` & `pyinstaller-hooks-contrib-2023.6/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py
+src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-exchangelib.py
@@ -156,14 +157,15 @@
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinja2.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinxed.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py
+src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py
```

