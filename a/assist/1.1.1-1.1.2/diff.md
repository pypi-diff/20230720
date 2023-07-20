# Comparing `tmp/assist-1.1.1.tar.gz` & `tmp/assist-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assist-1.1.1.tar", last modified: Wed Feb 15 01:10:58 2023, max compression
+gzip compressed data, was "assist-1.1.2.tar", last modified: Thu Jul 20 17:49:51 2023, max compression
```

## Comparing `assist-1.1.1.tar` & `assist-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-02-15 01:10:58.635563 assist-1.1.1/
--rw-r--r--   0 mholman    (501) staff       (20)    35147 2022-05-21 12:30:35.000000 assist-1.1.1/LICENSE
--rw-r--r--   0 mholman    (501) staff       (20)      261 2023-02-09 16:44:30.000000 assist-1.1.1/MANIFEST.in
--rw-r--r--   0 mholman    (501) staff       (20)     5978 2023-02-15 01:10:58.635772 assist-1.1.1/PKG-INFO
--rw-r--r--   0 mholman    (501) staff       (20)     5237 2023-02-15 01:10:52.000000 assist-1.1.1/README.md
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-02-15 01:10:58.628692 assist-1.1.1/assist/
--rw-r--r--   0 mholman    (501) staff       (20)     1468 2023-02-09 20:45:34.000000 assist-1.1.1/assist/__init__.py
--rw-r--r--   0 mholman    (501) staff       (20)     2545 2023-02-09 15:41:22.000000 assist-1.1.1/assist/ephem.py
--rw-r--r--   0 mholman    (501) staff       (20)     3179 2023-02-09 18:25:53.000000 assist-1.1.1/assist/extras.py
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-02-15 01:10:58.630925 assist-1.1.1/assist.egg-info/
--rw-r--r--   0 mholman    (501) staff       (20)     5978 2023-02-15 01:10:58.000000 assist-1.1.1/assist.egg-info/PKG-INFO
--rw-r--r--   0 mholman    (501) staff       (20)      432 2023-02-15 01:10:58.000000 assist-1.1.1/assist.egg-info/SOURCES.txt
--rw-r--r--   0 mholman    (501) staff       (20)        1 2023-02-15 01:10:58.000000 assist-1.1.1/assist.egg-info/dependency_links.txt
--rw-r--r--   0 mholman    (501) staff       (20)        1 2022-11-17 19:00:24.000000 assist-1.1.1/assist.egg-info/not-zip-safe
--rw-r--r--   0 mholman    (501) staff       (20)       22 2023-02-15 01:10:58.000000 assist-1.1.1/assist.egg-info/requires.txt
--rw-r--r--   0 mholman    (501) staff       (20)       17 2023-02-15 01:10:58.000000 assist-1.1.1/assist.egg-info/top_level.txt
--rw-r--r--   0 mholman    (501) staff       (20)       81 2023-02-09 16:44:30.000000 assist-1.1.1/pyproject.toml
--rw-r--r--   0 mholman    (501) staff       (20)      104 2023-02-15 01:10:58.636290 assist-1.1.1/setup.cfg
--rw-r--r--   0 mholman    (501) staff       (20)     4813 2023-02-15 01:10:52.000000 assist-1.1.1/setup.py
-drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-02-15 01:10:58.635171 assist-1.1.1/src/
--rw-r--r--   0 mholman    (501) staff       (20)    18472 2023-02-15 01:10:52.000000 assist-1.1.1/src/assist.c
--rw-r--r--   0 mholman    (501) staff       (20)     6272 2023-02-09 15:41:22.000000 assist-1.1.1/src/assist.h
--rw-r--r--   0 mholman    (501) staff       (20)    44930 2022-06-05 18:28:03.000000 assist-1.1.1/src/const.h
--rw-r--r--   0 mholman    (501) staff       (20)    84802 2023-02-09 15:41:22.000000 assist-1.1.1/src/forces.c
--rw-r--r--   0 mholman    (501) staff       (20)     1383 2023-02-02 16:10:38.000000 assist-1.1.1/src/forces.h
--rw-r--r--   0 mholman    (501) staff       (20)      548 2023-02-05 13:48:31.000000 assist-1.1.1/src/get_mass.c
--rw-r--r--   0 mholman    (501) staff       (20)    12496 2023-02-09 15:41:22.000000 assist-1.1.1/src/planets.c
--rw-r--r--   0 mholman    (501) staff       (20)     2914 2023-02-05 13:48:31.000000 assist-1.1.1/src/planets.h
--rw-r--r--   0 mholman    (501) staff       (20)     7185 2023-02-09 15:41:22.000000 assist-1.1.1/src/spk.c
--rw-r--r--   0 mholman    (501) staff       (20)     1972 2023-02-09 15:41:22.000000 assist-1.1.1/src/spk.h
--rw-r--r--   0 mholman    (501) staff       (20)        7 2023-02-15 01:10:48.000000 assist-1.1.1/version.txt
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.152630 assist-1.1.2/
+-rw-r--r--   0 mholman    (501) staff       (20)    35147 2023-03-16 20:41:43.000000 assist-1.1.2/LICENSE
+-rw-r--r--   0 mholman    (501) staff       (20)      264 2023-07-20 17:44:53.000000 assist-1.1.2/MANIFEST.in
+-rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-20 17:49:51.152454 assist-1.1.2/PKG-INFO
+-rw-r--r--   0 mholman    (501) staff       (20)     5345 2023-07-20 17:49:30.000000 assist-1.1.2/README.md
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.149949 assist-1.1.2/assist/
+-rw-r--r--   0 mholman    (501) staff       (20)     1813 2023-07-20 17:44:53.000000 assist-1.1.2/assist/__init__.py
+-rw-r--r--   0 mholman    (501) staff       (20)     2829 2023-07-20 17:44:53.000000 assist-1.1.2/assist/ephem.py
+-rw-r--r--   0 mholman    (501) staff       (20)     3601 2023-07-20 17:44:53.000000 assist-1.1.2/assist/extras.py
+-rw-r--r--   0 mholman    (501) staff       (20)        0 2023-07-20 17:44:53.000000 assist-1.1.2/assist/py.typed
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.150935 assist-1.1.2/assist.egg-info/
+-rw-r--r--   0 mholman    (501) staff       (20)     6086 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/PKG-INFO
+-rw-r--r--   0 mholman    (501) staff       (20)      411 2023-07-20 17:49:51.000000 assist-1.1.2/assist.egg-info/SOURCES.txt
+-rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/dependency_links.txt
+-rw-r--r--   0 mholman    (501) staff       (20)        1 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/not-zip-safe
+-rw-r--r--   0 mholman    (501) staff       (20)       22 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/requires.txt
+-rw-r--r--   0 mholman    (501) staff       (20)       17 2023-07-20 17:49:50.000000 assist-1.1.2/assist.egg-info/top_level.txt
+-rw-r--r--   0 mholman    (501) staff       (20)       81 2023-03-16 20:41:43.000000 assist-1.1.2/pyproject.toml
+-rw-r--r--   0 mholman    (501) staff       (20)       38 2023-07-20 17:49:51.152678 assist-1.1.2/setup.cfg
+-rw-r--r--   0 mholman    (501) staff       (20)     4818 2023-07-20 17:49:30.000000 assist-1.1.2/setup.py
+drwxr-xr-x   0 mholman    (501) staff       (20)        0 2023-07-20 17:49:51.152232 assist-1.1.2/src/
+-rw-r--r--   0 mholman    (501) staff       (20)    21697 2023-07-20 17:49:30.000000 assist-1.1.2/src/assist.c
+-rw-r--r--   0 mholman    (501) staff       (20)     6849 2023-07-20 17:44:53.000000 assist-1.1.2/src/assist.h
+-rw-r--r--   0 mholman    (501) staff       (20)    84761 2023-07-20 17:44:53.000000 assist-1.1.2/src/forces.c
+-rw-r--r--   0 mholman    (501) staff       (20)     1383 2023-03-16 20:41:43.000000 assist-1.1.2/src/forces.h
+-rw-r--r--   0 mholman    (501) staff       (20)    12771 2023-03-16 20:41:43.000000 assist-1.1.2/src/planets.c
+-rw-r--r--   0 mholman    (501) staff       (20)     3161 2023-03-16 20:41:43.000000 assist-1.1.2/src/planets.h
+-rw-r--r--   0 mholman    (501) staff       (20)     8181 2023-03-16 20:41:43.000000 assist-1.1.2/src/spk.c
+-rw-r--r--   0 mholman    (501) staff       (20)     1135 2023-03-16 20:41:43.000000 assist-1.1.2/src/spk.h
+-rw-r--r--   0 mholman    (501) staff       (20)        7 2023-07-20 17:49:02.000000 assist-1.1.2/version.txt
```

### Comparing `assist-1.1.1/LICENSE` & `assist-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `assist-1.1.1/PKG-INFO` & `assist-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assist
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library high accuracy ephemeris in REBOUND
 Home-page: https://github.com/matthewholman/assist
 Author: Matthew Holman
 Author-email: mholman@cfa.harvard.edu
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,21 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Version](https://img.shields.io/badge/assist-v1.1.1-green.svg?style=flat)](https://assist.readthedocs.org)
+[![Version](https://img.shields.io/badge/assist-v1.1.2-green.svg?style=flat)](https://assist.readthedocs.org)
 [![GPL](https://img.shields.io/badge/license-GPL-green.svg?style=flat)](https://github.com/matthewholman/blob/main/LICENSE)
 [![Python unit tests)](https://github.com/matthewholman/assist/actions/workflows/python.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/python.yml)
 [![C unit tests](https://github.com/matthewholman/assist/actions/workflows/c.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/c.yml)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7778016.svg)](https://doi.org/10.5281/zenodo.7778016)
+
+
 
 # ASSIST
 
 ASSIST is a software package for ephemeris-quality integrations of test particles. ASSIST is an extension of the [REBOUND framework](https://github.com/hannorein/rebound) and makes use of its [IAS15 integrator](https://ui.adsabs.harvard.edu/abs/2015MNRAS.446.1424R/abstract) to integrate test particle trajectories in the field of the Sun, Moon, planets, and 16 massive asteroids, with the positions of the masses coming from the JPL DE441 ephemeris and its associated asteroid perturber file. The package incorporates the most significant gravitational harmonics and general relativistic corrections. ASSIST also accounts for position- and velocity-dependent non-gravitational effects according to the [Marsden (1973) model](https://ui.adsabs.harvard.edu/abs/1973AJ.....78..211M/abstract). All components in the equations of motion have been verified to machine precision in a term-by-term comparison with output from JPL's small body integrator. The first order variational equations are included for all terms to support orbit fitting and covariance mapping. This framework is meant to provide an open-source package written in a modern language to enable high-precision orbital analysis and science by the small body community.
```

### Comparing `assist-1.1.1/README.md` & `assist-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b21 5b56 6572 7369 6f6e 5d28 6874 7470  [![Version](http
 00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 00000020: 696f 2f62 6164 6765 2f61 7373 6973 742d  io/badge/assist-
-00000030: 7631 2e31 2e31 2d67 7265 656e 2e73 7667  v1.1.1-green.svg
+00000030: 7631 2e31 2e32 2d67 7265 656e 2e73 7667  v1.1.2-green.svg
 00000040: 3f73 7479 6c65 3d66 6c61 7429 5d28 6874  ?style=flat)](ht
 00000050: 7470 733a 2f2f 6173 7369 7374 2e72 6561  tps://assist.rea
 00000060: 6474 6865 646f 6373 2e6f 7267 290a 5b21  dthedocs.org).[!
 00000070: 5b47 504c 5d28 6874 7470 733a 2f2f 696d  [GPL](https://im
 00000080: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
 00000090: 6765 2f6c 6963 656e 7365 2d47 504c 2d67  ge/license-GPL-g
 000000a0: 7265 656e 2e73 7667 3f73 7479 6c65 3d66  reen.svg?style=f
@@ -29,300 +29,307 @@
 000001c0: 6865 7768 6f6c 6d61 6e2f 6173 7369 7374  hewholman/assist
 000001d0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
 000001e0: 7773 2f63 2e79 6d6c 2f62 6164 6765 2e73  ws/c.yml/badge.s
 000001f0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
 00000200: 6875 622e 636f 6d2f 6d61 7474 6865 7768  hub.com/matthewh
 00000210: 6f6c 6d61 6e2f 6173 7369 7374 2f61 6374  olman/assist/act
 00000220: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
-00000230: 2e79 6d6c 290a 0a23 2041 5353 4953 540a  .yml)..# ASSIST.
-00000240: 0a41 5353 4953 5420 6973 2061 2073 6f66  .ASSIST is a sof
-00000250: 7477 6172 6520 7061 636b 6167 6520 666f  tware package fo
-00000260: 7220 6570 6865 6d65 7269 732d 7175 616c  r ephemeris-qual
-00000270: 6974 7920 696e 7465 6772 6174 696f 6e73  ity integrations
-00000280: 206f 6620 7465 7374 2070 6172 7469 636c   of test particl
-00000290: 6573 2e20 4153 5349 5354 2069 7320 616e  es. ASSIST is an
-000002a0: 2065 7874 656e 7369 6f6e 206f 6620 7468   extension of th
-000002b0: 6520 5b52 4542 4f55 4e44 2066 7261 6d65  e [REBOUND frame
-000002c0: 776f 726b 5d28 6874 7470 733a 2f2f 6769  work](https://gi
-000002d0: 7468 7562 2e63 6f6d 2f68 616e 6e6f 7265  thub.com/hannore
-000002e0: 696e 2f72 6562 6f75 6e64 2920 616e 6420  in/rebound) and 
-000002f0: 6d61 6b65 7320 7573 6520 6f66 2069 7473  makes use of its
-00000300: 205b 4941 5331 3520 696e 7465 6772 6174   [IAS15 integrat
-00000310: 6f72 5d28 6874 7470 733a 2f2f 7569 2e61  or](https://ui.a
-00000320: 6473 6162 732e 6861 7276 6172 642e 6564  dsabs.harvard.ed
-00000330: 752f 6162 732f 3230 3135 4d4e 5241 532e  u/abs/2015MNRAS.
-00000340: 3434 362e 3134 3234 522f 6162 7374 7261  446.1424R/abstra
-00000350: 6374 2920 746f 2069 6e74 6567 7261 7465  ct) to integrate
-00000360: 2074 6573 7420 7061 7274 6963 6c65 2074   test particle t
-00000370: 7261 6a65 6374 6f72 6965 7320 696e 2074  rajectories in t
-00000380: 6865 2066 6965 6c64 206f 6620 7468 6520  he field of the 
-00000390: 5375 6e2c 204d 6f6f 6e2c 2070 6c61 6e65  Sun, Moon, plane
-000003a0: 7473 2c20 616e 6420 3136 206d 6173 7369  ts, and 16 massi
-000003b0: 7665 2061 7374 6572 6f69 6473 2c20 7769  ve asteroids, wi
-000003c0: 7468 2074 6865 2070 6f73 6974 696f 6e73  th the positions
-000003d0: 206f 6620 7468 6520 6d61 7373 6573 2063   of the masses c
-000003e0: 6f6d 696e 6720 6672 6f6d 2074 6865 204a  oming from the J
-000003f0: 504c 2044 4534 3431 2065 7068 656d 6572  PL DE441 ephemer
-00000400: 6973 2061 6e64 2069 7473 2061 7373 6f63  is and its assoc
-00000410: 6961 7465 6420 6173 7465 726f 6964 2070  iated asteroid p
-00000420: 6572 7475 7262 6572 2066 696c 652e 2054  erturber file. T
-00000430: 6865 2070 6163 6b61 6765 2069 6e63 6f72  he package incor
-00000440: 706f 7261 7465 7320 7468 6520 6d6f 7374  porates the most
-00000450: 2073 6967 6e69 6669 6361 6e74 2067 7261   significant gra
-00000460: 7669 7461 7469 6f6e 616c 2068 6172 6d6f  vitational harmo
-00000470: 6e69 6373 2061 6e64 2067 656e 6572 616c  nics and general
-00000480: 2072 656c 6174 6976 6973 7469 6320 636f   relativistic co
-00000490: 7272 6563 7469 6f6e 732e 2041 5353 4953  rrections. ASSIS
-000004a0: 5420 616c 736f 2061 6363 6f75 6e74 7320  T also accounts 
-000004b0: 666f 7220 706f 7369 7469 6f6e 2d20 616e  for position- an
-000004c0: 6420 7665 6c6f 6369 7479 2d64 6570 656e  d velocity-depen
-000004d0: 6465 6e74 206e 6f6e 2d67 7261 7669 7461  dent non-gravita
-000004e0: 7469 6f6e 616c 2065 6666 6563 7473 2061  tional effects a
-000004f0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00000500: 5b4d 6172 7364 656e 2028 3139 3733 2920  [Marsden (1973) 
-00000510: 6d6f 6465 6c5d 2868 7474 7073 3a2f 2f75  model](https://u
-00000520: 692e 6164 7361 6273 2e68 6172 7661 7264  i.adsabs.harvard
-00000530: 2e65 6475 2f61 6273 2f31 3937 3341 4a2e  .edu/abs/1973AJ.
-00000540: 2e2e 2e2e 3738 2e2e 3231 314d 2f61 6273  ....78..211M/abs
-00000550: 7472 6163 7429 2e20 416c 6c20 636f 6d70  tract). All comp
-00000560: 6f6e 656e 7473 2069 6e20 7468 6520 6571  onents in the eq
-00000570: 7561 7469 6f6e 7320 6f66 206d 6f74 696f  uations of motio
-00000580: 6e20 6861 7665 2062 6565 6e20 7665 7269  n have been veri
-00000590: 6669 6564 2074 6f20 6d61 6368 696e 6520  fied to machine 
-000005a0: 7072 6563 6973 696f 6e20 696e 2061 2074  precision in a t
-000005b0: 6572 6d2d 6279 2d74 6572 6d20 636f 6d70  erm-by-term comp
-000005c0: 6172 6973 6f6e 2077 6974 6820 6f75 7470  arison with outp
-000005d0: 7574 2066 726f 6d20 4a50 4c27 7320 736d  ut from JPL's sm
-000005e0: 616c 6c20 626f 6479 2069 6e74 6567 7261  all body integra
-000005f0: 746f 722e 2054 6865 2066 6972 7374 206f  tor. The first o
-00000600: 7264 6572 2076 6172 6961 7469 6f6e 616c  rder variational
-00000610: 2065 7175 6174 696f 6e73 2061 7265 2069   equations are i
-00000620: 6e63 6c75 6465 6420 666f 7220 616c 6c20  ncluded for all 
-00000630: 7465 726d 7320 746f 2073 7570 706f 7274  terms to support
-00000640: 206f 7262 6974 2066 6974 7469 6e67 2061   orbit fitting a
-00000650: 6e64 2063 6f76 6172 6961 6e63 6520 6d61  nd covariance ma
-00000660: 7070 696e 672e 2054 6869 7320 6672 616d  pping. This fram
-00000670: 6577 6f72 6b20 6973 206d 6561 6e74 2074  ework is meant t
-00000680: 6f20 7072 6f76 6964 6520 616e 206f 7065  o provide an ope
-00000690: 6e2d 736f 7572 6365 2070 6163 6b61 6765  n-source package
-000006a0: 2077 7269 7474 656e 2069 6e20 6120 6d6f   written in a mo
-000006b0: 6465 726e 206c 616e 6775 6167 6520 746f  dern language to
-000006c0: 2065 6e61 626c 6520 6869 6768 2d70 7265   enable high-pre
-000006d0: 6369 7369 6f6e 206f 7262 6974 616c 2061  cision orbital a
-000006e0: 6e61 6c79 7369 7320 616e 6420 7363 6965  nalysis and scie
-000006f0: 6e63 6520 6279 2074 6865 2073 6d61 6c6c  nce by the small
-00000700: 2062 6f64 7920 636f 6d6d 756e 6974 792e   body community.
-00000710: 0a0a 0a0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
-00000720: 696f 6e20 2850 7974 686f 6e29 0a0a 4974  ion (Python)..It
-00000730: 2773 2065 6173 6965 7374 2074 6f20 696e  's easiest to in
-00000740: 7374 616c 6c20 4153 5349 5354 2069 6e74  stall ASSIST int
-00000750: 6f20 6120 7079 7468 6f6e 2076 6972 7475  o a python virtu
-00000760: 616c 2065 6e76 6972 6f6e 6d65 6e74 2e20  al environment. 
-00000770: 4966 2079 6f75 2061 6c72 6561 6479 2068  If you already h
-00000780: 6176 6520 6120 7669 7274 7561 6c20 656e  ave a virtual en
-00000790: 7669 726f 6e6d 656e 7420 6f72 2064 6f20  vironment or do 
-000007a0: 6e6f 7420 7761 6e74 2074 6f20 7573 6520  not want to use 
-000007b0: 6f6e 652c 2079 6f75 2063 616e 2073 6b69  one, you can ski
-000007c0: 7020 7468 6973 2073 7465 702e 204f 7468  p this step. Oth
-000007d0: 6572 7769 7365 2c20 7275 6e20 7468 6520  erwise, run the 
-000007e0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-000007f0: 6420 696e 2061 6e20 656d 7074 7920 6469  d in an empty di
-00000800: 7265 6374 6f72 792e 2054 6865 7920 7769  rectory. They wi
-00000810: 6c6c 2073 6574 7570 2061 6e64 2061 6374  ll setup and act
-00000820: 6976 6174 6520 6120 6e65 7720 7669 7274  ivate a new virt
-00000830: 7561 6c20 656e 7669 726f 6e6d 656e 7420  ual environment 
-00000840: 696e 2061 2064 6972 6563 746f 7279 2e20  in a directory. 
-00000850: 0a0a 2020 2020 7079 7468 6f6e 3320 2d6d  ..    python3 -m
-00000860: 2076 656e 7620 7665 6e76 0a20 2020 2073   venv venv.    s
-00000870: 6f75 7263 6520 7665 6e76 2f62 696e 2f61  ource venv/bin/a
-00000880: 6374 6976 6174 650a 0a4e 6f77 2077 6520  ctivate..Now we 
-00000890: 6361 6e20 696e 7374 616c 6c20 6e75 6d70  can install nump
-000008a0: 792c 2052 4542 4f55 4e44 2c20 616e 6420  y, REBOUND, and 
-000008b0: 4153 5349 5354 3a0a 0a20 2020 2070 6970  ASSIST:..    pip
-000008c0: 2069 6e73 7461 6c6c 206e 756d 7079 0a20   install numpy. 
-000008d0: 2020 2070 6970 2069 6e73 7461 6c6c 2072     pip install r
-000008e0: 6562 6f75 6e64 200a 2020 2020 7069 7020  ebound .    pip 
-000008f0: 696e 7374 616c 6c20 6173 7369 7374 0a0a  install assist..
-00000900: 546f 2075 7365 2075 7365 2041 5353 4953  To use use ASSIS
-00000910: 542c 2079 6f75 2061 6c73 6f20 6e65 6564  T, you also need
-00000920: 2074 6f20 646f 776e 6c6f 6164 2065 7068   to download eph
-00000930: 656d 6572 6973 2064 6174 6120 6669 6c65  emeris data file
-00000940: 732e 204f 6e65 2066 696c 6520 666f 7220  s. One file for 
-00000950: 706c 616e 6574 2065 7068 656d 6572 6973  planet ephemeris
-00000960: 2061 6e64 2061 6e6f 7468 6572 2073 7570   and another sup
-00000970: 6c65 6d65 6e74 6172 7920 6669 6c65 2066  lementary file f
-00000980: 6f72 2061 7374 6572 6f69 6420 6570 6865  or asteroid ephe
-00000990: 6d65 7269 732e 2054 6865 2066 6f6c 6c6f  meris. The follo
-000009a0: 7769 6e67 2063 6f6d 6d61 6e64 7320 646f  wing commands do
-000009b0: 776e 6c6f 6164 2074 6865 7365 2066 696c  wnload these fil
-000009c0: 6573 2077 6974 6820 6375 726c 2e20 596f  es with curl. Yo
-000009d0: 7520 6361 6e20 616c 736f 206d 616e 7561  u can also manua
-000009e0: 6c6c 7920 646f 776e 6c6f 6164 2074 6865  lly download the
-000009f0: 6d20 7573 696e 6720 796f 7572 2062 726f  m using your bro
-00000a00: 7773 6572 2e20 4e6f 7465 2074 6861 7420  wser. Note that 
-00000a10: 7468 6573 6520 6172 6520 6c61 7267 6520  these are large 
-00000a20: 6669 6c65 732c 2061 6c6d 6f73 7420 3147  files, almost 1G
-00000a30: 4220 696e 2073 697a 652e 0a0a 2020 2020  B in size...    
-00000a40: 6d6b 6469 7220 6461 7461 0a20 2020 2063  mkdir data.    c
-00000a50: 7572 6c20 6874 7470 733a 2f2f 7373 642e  url https://ssd.
-00000a60: 6a70 6c2e 6e61 7361 2e67 6f76 2f66 7470  jpl.nasa.gov/ftp
-00000a70: 2f65 7068 2f70 6c61 6e65 7473 2f4c 696e  /eph/planets/Lin
-00000a80: 7578 2f64 6534 3430 2f6c 696e 7578 5f70  ux/de440/linux_p
-00000a90: 3135 3530 7032 3635 302e 3434 3020 2d6f  1550p2650.440 -o
-00000aa0: 2064 6174 612f 6c69 6e75 785f 7031 3535   data/linux_p155
-00000ab0: 3070 3236 3530 2e34 3430 0a20 2020 2063  0p2650.440.    c
-00000ac0: 7572 6c20 6874 7470 733a 2f2f 7373 642e  url https://ssd.
-00000ad0: 6a70 6c2e 6e61 7361 2e67 6f76 2f66 7470  jpl.nasa.gov/ftp
-00000ae0: 2f65 7068 2f73 6d61 6c6c 5f62 6f64 6965  /eph/small_bodie
-00000af0: 732f 6173 7465 726f 6964 735f 6465 3434  s/asteroids_de44
-00000b00: 312f 7362 3434 312d 6e31 362e 6273 7020  1/sb441-n16.bsp 
-00000b10: 2d6f 2064 6174 612f 7362 3434 312d 6e31  -o data/sb441-n1
-00000b20: 362e 6273 700a 0a4e 6f77 2079 6f75 2063  6.bsp..Now you c
-00000b30: 616e 2074 7279 206f 7574 2069 6620 6173  an try out if as
-00000b40: 7369 7374 2077 6f72 6b73 2e0a 0a20 2020  sist works...   
-00000b50: 2070 7974 686f 6e33 0a0a 2020 2020 3e3e   python3..    >>
-00000b60: 3e20 696d 706f 7274 2061 7373 6973 740a  > import assist.
-00000b70: 2020 2020 3e3e 3e20 6570 6865 6d20 3d20      >>> ephem = 
-00000b80: 6173 7369 7374 2e45 7068 656d 2822 6461  assist.Ephem("da
-00000b90: 7461 2f6c 696e 7578 5f70 3135 3530 7032  ta/linux_p1550p2
-00000ba0: 3635 302e 3434 3022 2c20 2264 6174 612f  650.440", "data/
-00000bb0: 7362 3434 312d 6e31 362e 6273 7022 290a  sb441-n16.bsp").
-00000bc0: 2020 2020 3e3e 3e20 7072 696e 7428 6570      >>> print(ep
-00000bd0: 6865 6d2e 6a64 5f72 6566 290a 2020 2020  hem.jd_ref).    
-00000be0: 3e3e 3e20 6570 6865 6d2e 6765 745f 7061  >>> ephem.get_pa
-00000bf0: 7274 6963 6c65 2822 4561 7274 6822 2c20  rticle("Earth", 
-00000c00: 3029 0a0a 596f 7520 7368 6f75 6c64 2073  0)..You should s
-00000c10: 6565 2074 6865 2064 6566 6175 6c74 2072  ee the default r
-00000c20: 6566 6572 656e 6365 204a 756c 6961 6e20  eference Julian 
-00000c30: 6461 7465 2028 3234 3531 3534 352e 3029  date (2451545.0)
-00000c40: 2061 6e64 2074 6865 2070 6f73 6974 696f   and the positio
-00000c50: 6e20 6f66 2074 6865 2045 6172 7468 2061  n of the Earth a
-00000c60: 7420 7468 6174 2074 696d 6520 7072 696e  t that time prin
-00000c70: 7465 6420 6f6e 2074 6865 2073 6372 6565  ted on the scree
-00000c80: 6e2e 0a0a 2323 2049 6e73 7461 6c6c 6174  n...## Installat
-00000c90: 696f 6e20 2843 290a 0a54 6f20 696e 7374  ion (C)..To inst
-00000ca0: 616c 6c20 7468 6520 4320 7665 7273 696f  all the C versio
-00000cb0: 6e20 6f66 2041 5353 4953 542c 2066 6972  n of ASSIST, fir
-00000cc0: 7374 2063 6c6f 6e65 2074 6865 2052 4542  st clone the REB
-00000cd0: 4f55 4e44 2061 6e64 2074 6865 6e20 7468  OUND and then th
-00000ce0: 6520 4153 5349 5354 2072 6570 6f73 6974  e ASSIST reposit
-00000cf0: 6f72 6965 732e 2049 6e20 616e 2065 6d70  ories. In an emp
-00000d00: 7479 2064 6972 6563 746f 7279 2c20 7275  ty directory, ru
-00000d10: 6e3a 0a0a 2020 2020 6769 7420 636c 6f6e  n:..    git clon
-00000d20: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00000d30: 2e63 6f6d 2f68 616e 6e6f 7265 696e 2f72  .com/hannorein/r
-00000d40: 6562 6f75 6e64 2e67 6974 0a20 2020 2067  ebound.git.    g
-00000d50: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00000d60: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
-00000d70: 6865 7768 6f6c 6d61 6e2f 6173 7369 7374  hewholman/assist
-00000d80: 2e67 6974 0a0a 546f 2075 7365 2075 7365  .git..To use use
-00000d90: 2041 5353 4953 542c 2079 6f75 2061 6c73   ASSIST, you als
-00000da0: 6f20 6e65 6564 2074 6f20 646f 776e 6c6f  o need to downlo
-00000db0: 6164 2065 7068 656d 6572 6973 2064 6174  ad ephemeris dat
-00000dc0: 6120 6669 6c65 732e 204f 6e65 2066 696c  a files. One fil
-00000dd0: 6520 666f 7220 706c 616e 6574 2065 7068  e for planet eph
-00000de0: 656d 6572 6973 2061 6e64 2061 6e6f 7468  emeris and anoth
-00000df0: 6572 2073 7570 6c65 6d65 6e74 6172 7920  er suplementary 
-00000e00: 6669 6c65 2066 6f72 2061 7374 6572 6f69  file for asteroi
-00000e10: 6420 6570 6865 6d65 7269 732e 2054 6865  d ephemeris. The
-00000e20: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000e30: 6e64 7320 646f 776e 6c6f 6164 2074 6865  nds download the
-00000e40: 7365 2066 696c 6573 2077 6974 6820 6375  se files with cu
-00000e50: 726c 2e20 596f 7520 6361 6e20 616c 736f  rl. You can also
-00000e60: 206d 616e 7561 6c6c 7920 646f 776e 6c6f   manually downlo
-00000e70: 6164 2074 6865 6d20 7573 696e 6720 796f  ad them using yo
-00000e80: 7572 2062 726f 7773 6572 2e20 4e6f 7465  ur browser. Note
-00000e90: 2074 6861 7420 7468 6573 6520 6172 6520   that these are 
-00000ea0: 6c61 7267 6520 6669 6c65 732c 2061 6c6d  large files, alm
-00000eb0: 6f73 7420 3147 4220 696e 2073 697a 652e  ost 1GB in size.
-00000ec0: 0a0a 2020 2020 6375 726c 2068 7474 7073  ..    curl https
-00000ed0: 3a2f 2f73 7364 2e6a 706c 2e6e 6173 612e  ://ssd.jpl.nasa.
-00000ee0: 676f 762f 6674 702f 6570 682f 706c 616e  gov/ftp/eph/plan
-00000ef0: 6574 732f 4c69 6e75 782f 6465 3434 302f  ets/Linux/de440/
-00000f00: 6c69 6e75 785f 7031 3535 3070 3236 3530  linux_p1550p2650
-00000f10: 2e34 3430 202d 6f20 6173 7369 7374 2f64  .440 -o assist/d
-00000f20: 6174 612f 6c69 6e75 785f 7031 3535 3070  ata/linux_p1550p
-00000f30: 3236 3530 2e34 3430 0a20 2020 2063 7572  2650.440.    cur
-00000f40: 6c20 6874 7470 733a 2f2f 7373 642e 6a70  l https://ssd.jp
-00000f50: 6c2e 6e61 7361 2e67 6f76 2f66 7470 2f65  l.nasa.gov/ftp/e
-00000f60: 7068 2f73 6d61 6c6c 5f62 6f64 6965 732f  ph/small_bodies/
-00000f70: 6173 7465 726f 6964 735f 6465 3434 312f  asteroids_de441/
-00000f80: 7362 3434 312d 6e31 362e 6273 7020 2d6f  sb441-n16.bsp -o
-00000f90: 2061 7373 6973 742f 6461 7461 2f73 6234   assist/data/sb4
-00000fa0: 3431 2d6e 3136 2e62 7370 0a0a 466f 7220  41-n16.bsp..For 
-00000fb0: 736f 6d65 206f 6620 7468 6520 6578 616d  some of the exam
-00000fc0: 706c 6573 2c20 796f 7520 7769 6c6c 2061  ples, you will a
-00000fd0: 6c73 6f20 6e65 6564 2074 6865 2070 6c61  lso need the pla
-00000fe0: 6e65 7420 6570 6865 6d65 7269 7320 6669  net ephemeris fi
-00000ff0: 6c65 2077 6974 6820 616e 2065 7874 656e  le with an exten
-00001000: 6465 6420 636f 7665 7261 6765 2e20 4e6f  ded coverage. No
-00001010: 7465 2074 6861 7420 7468 6973 2066 696c  te that this fil
-00001020: 6520 6973 2032 2e36 4742 2069 6e20 7369  e is 2.6GB in si
-00001030: 7a65 2e0a 0a20 2020 2063 7572 6c20 6874  ze...    curl ht
-00001040: 7470 733a 2f2f 7373 642e 6a70 6c2e 6e61  tps://ssd.jpl.na
-00001050: 7361 2e67 6f76 2f66 7470 2f65 7068 2f70  sa.gov/ftp/eph/p
-00001060: 6c61 6e65 7473 2f4c 696e 7578 2f64 6534  lanets/Linux/de4
-00001070: 3431 2f6c 696e 7578 5f6d 3133 3030 3070  41/linux_m13000p
-00001080: 3137 3030 302e 3434 3120 2d6f 2061 7373  17000.441 -o ass
-00001090: 6973 742f 6461 7461 2f6c 696e 7578 5f6d  ist/data/linux_m
-000010a0: 3133 3030 3070 3137 3030 302e 3434 310a  13000p17000.441.
-000010b0: 0a4e 6578 742c 2067 6f20 746f 206f 6e65  .Next, go to one
-000010c0: 206f 6620 7468 6520 6578 616d 706c 6520   of the example 
-000010d0: 6469 7265 6374 6f72 6965 7320 616e 6420  directories and 
-000010e0: 636f 6d70 696c 6520 7468 6520 7072 6f62  compile the prob
-000010f0: 6c65 6d20 6669 6c65 2e20 5468 6973 2077  lem file. This w
-00001100: 696c 6c20 616c 736f 2074 7269 6767 6572  ill also trigger
-00001110: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
-00001120: 6e20 6f66 2074 6865 2052 4542 4f55 4e44  n of the REBOUND
-00001130: 2061 6e64 2041 5353 4953 5420 7368 6172   and ASSIST shar
-00001140: 6564 206c 6962 7261 7269 6573 2e0a 0a20  ed libraries... 
-00001150: 2020 2063 6420 6173 7369 7374 2f65 7861     cd assist/exa
-00001160: 6d70 6c65 732f 706c 6169 6e5f 696e 7465  mples/plain_inte
-00001170: 7266 6163 650a 2020 2020 6d61 6b65 0a0a  rface.    make..
-00001180: 4e6f 772c 2079 6f75 2772 6520 7265 6164  Now, you're read
-00001190: 7920 746f 2072 756e 2074 6865 2065 7861  y to run the exa
-000011a0: 6d70 6c65 2077 6974 683a 0a0a 2020 2020  mple with:..    
-000011b0: 2e2f 7265 626f 756e 640a 0a0a 2323 204c  ./rebound...## L
-000011c0: 6963 656e 7365 0a41 5353 4953 5420 6973  icense.ASSIST is
-000011d0: 206f 7065 6e20 736f 7572 6365 2c20 6672   open source, fr
-000011e0: 6565 6c79 2064 6973 7472 6962 7574 6564  eely distributed
-000011f0: 2075 6e64 6572 2074 6865 205b 474e 5520   under the [GNU 
-00001200: 4765 6e65 7261 6c20 5075 626c 6963 206c  General Public l
-00001210: 6963 656e 7365 2c20 7665 7273 696f 6e20  icense, version 
-00001220: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-00001230: 622e 636f 6d2f 6d61 7474 6865 7768 6f6c  b.com/matthewhol
-00001240: 6d61 6e2f 626c 6f62 2f6d 6169 6e2f 4c49  man/blob/main/LI
-00001250: 4345 4e53 4529 2e0a 0a23 2320 436f 6e74  CENSE)...## Cont
-00001260: 7269 6275 746f 7273 0a0a 2a20 4d61 7474  ributors..* Matt
-00001270: 6865 7720 4a2e 2048 6f6c 6d61 6e2c 2043  hew J. Holman, C
-00001280: 656e 7465 7220 666f 7220 4173 7472 6f70  enter for Astrop
-00001290: 6879 7369 6373 207c 2048 6172 7661 7264  hysics | Harvard
-000012a0: 2026 2053 6d69 7468 736f 6e69 616e 2c20   & Smithsonian, 
-000012b0: 3c6d 686f 6c6d 616e 4063 6661 2e68 6172  <mholman@cfa.har
-000012c0: 7661 7264 2e65 6475 3e0a 2a20 4172 7961  vard.edu>.* Arya
-000012d0: 2041 6b6d 616c 2c20 4d6f 6e74 676f 6d65   Akmal, Montgome
-000012e0: 7279 2043 6f6c 6c65 6765 2c20 526f 636b  ry College, Rock
-000012f0: 7669 6c6c 650a 2a20 4461 7669 6465 2046  ville.* Davide F
-00001300: 6172 6e6f 6363 6869 612c 204a 6574 2050  arnocchia, Jet P
-00001310: 726f 7075 6c73 696f 6e20 4c61 626f 7261  ropulsion Labora
-00001320: 746f 7279 2c20 4361 6c69 666f 726e 6961  tory, California
-00001330: 2049 6e73 7469 7475 7465 206f 6620 5465   Institute of Te
-00001340: 6368 6e6f 6c6f 6779 200a 2a20 4861 6e6e  chnology .* Hann
-00001350: 6f20 5265 696e 2c20 556e 6976 6572 7369  o Rein, Universi
-00001360: 7479 206f 6620 546f 726f 6e74 6f2c 203c  ty of Toronto, <
-00001370: 6861 6e6e 6f40 6861 6e6e 6f2d 7265 696e  hanno@hanno-rein
-00001380: 2e64 653e 0a2a 204d 6174 7468 6577 204a  .de>.* Matthew J
-00001390: 2e20 5061 796e 652c 2043 656e 7465 7220  . Payne, Center 
-000013a0: 666f 7220 4173 7472 6f70 6879 7369 6373  for Astrophysics
-000013b0: 207c 2048 6172 7661 7264 2026 2053 6d69   | Harvard & Smi
-000013c0: 7468 736f 6e69 616e 0a2a 2052 6f62 6572  thsonian.* Rober
-000013d0: 7420 5765 7279 6b2c 2055 6e69 7665 7273  t Weryk, Univers
-000013e0: 6974 7920 6f66 2057 6573 7465 726e 204f  ity of Western O
-000013f0: 6e74 6172 696f 0a2a 2044 616e 2054 616d  ntario.* Dan Tam
-00001400: 6179 6f2c 2048 6172 7665 7920 4d75 6464  ayo, Harvey Mudd
-00001410: 2043 6f6c 6c65 6765 2c20 3c64 7461 6d61   College, <dtama
-00001420: 796f 4068 6d63 2e65 6475 3e0a 2a20 4461  yo@hmc.edu>.* Da
-00001430: 7669 6420 4d2e 2048 6572 6e61 6e64 657a  vid M. Hernandez
-00001440: 2c20 4365 6e74 6572 2066 6f72 2041 7374  , Center for Ast
-00001450: 726f 7068 7973 6963 7320 7c20 4861 7276  rophysics | Harv
-00001460: 6172 6420 2620 536d 6974 6873 6f6e 6961  ard & Smithsonia
-00001470: 6e20 0a0a 0a                             n ...
+00000230: 2e79 6d6c 290a 5b21 5b44 4f49 5d28 6874  .yml).[![DOI](ht
+00000240: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
+00000250: 2f62 6164 6765 2f44 4f49 2f31 302e 3532  /badge/DOI/10.52
+00000260: 3831 2f7a 656e 6f64 6f2e 3737 3738 3031  81/zenodo.777801
+00000270: 362e 7376 6729 5d28 6874 7470 733a 2f2f  6.svg)](https://
+00000280: 646f 692e 6f72 672f 3130 2e35 3238 312f  doi.org/10.5281/
+00000290: 7a65 6e6f 646f 2e37 3737 3830 3136 290a  zenodo.7778016).
+000002a0: 0a0a 0a23 2041 5353 4953 540a 0a41 5353  ...# ASSIST..ASS
+000002b0: 4953 5420 6973 2061 2073 6f66 7477 6172  IST is a softwar
+000002c0: 6520 7061 636b 6167 6520 666f 7220 6570  e package for ep
+000002d0: 6865 6d65 7269 732d 7175 616c 6974 7920  hemeris-quality 
+000002e0: 696e 7465 6772 6174 696f 6e73 206f 6620  integrations of 
+000002f0: 7465 7374 2070 6172 7469 636c 6573 2e20  test particles. 
+00000300: 4153 5349 5354 2069 7320 616e 2065 7874  ASSIST is an ext
+00000310: 656e 7369 6f6e 206f 6620 7468 6520 5b52  ension of the [R
+00000320: 4542 4f55 4e44 2066 7261 6d65 776f 726b  EBOUND framework
+00000330: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000340: 2e63 6f6d 2f68 616e 6e6f 7265 696e 2f72  .com/hannorein/r
+00000350: 6562 6f75 6e64 2920 616e 6420 6d61 6b65  ebound) and make
+00000360: 7320 7573 6520 6f66 2069 7473 205b 4941  s use of its [IA
+00000370: 5331 3520 696e 7465 6772 6174 6f72 5d28  S15 integrator](
+00000380: 6874 7470 733a 2f2f 7569 2e61 6473 6162  https://ui.adsab
+00000390: 732e 6861 7276 6172 642e 6564 752f 6162  s.harvard.edu/ab
+000003a0: 732f 3230 3135 4d4e 5241 532e 3434 362e  s/2015MNRAS.446.
+000003b0: 3134 3234 522f 6162 7374 7261 6374 2920  1424R/abstract) 
+000003c0: 746f 2069 6e74 6567 7261 7465 2074 6573  to integrate tes
+000003d0: 7420 7061 7274 6963 6c65 2074 7261 6a65  t particle traje
+000003e0: 6374 6f72 6965 7320 696e 2074 6865 2066  ctories in the f
+000003f0: 6965 6c64 206f 6620 7468 6520 5375 6e2c  ield of the Sun,
+00000400: 204d 6f6f 6e2c 2070 6c61 6e65 7473 2c20   Moon, planets, 
+00000410: 616e 6420 3136 206d 6173 7369 7665 2061  and 16 massive a
+00000420: 7374 6572 6f69 6473 2c20 7769 7468 2074  steroids, with t
+00000430: 6865 2070 6f73 6974 696f 6e73 206f 6620  he positions of 
+00000440: 7468 6520 6d61 7373 6573 2063 6f6d 696e  the masses comin
+00000450: 6720 6672 6f6d 2074 6865 204a 504c 2044  g from the JPL D
+00000460: 4534 3431 2065 7068 656d 6572 6973 2061  E441 ephemeris a
+00000470: 6e64 2069 7473 2061 7373 6f63 6961 7465  nd its associate
+00000480: 6420 6173 7465 726f 6964 2070 6572 7475  d asteroid pertu
+00000490: 7262 6572 2066 696c 652e 2054 6865 2070  rber file. The p
+000004a0: 6163 6b61 6765 2069 6e63 6f72 706f 7261  ackage incorpora
+000004b0: 7465 7320 7468 6520 6d6f 7374 2073 6967  tes the most sig
+000004c0: 6e69 6669 6361 6e74 2067 7261 7669 7461  nificant gravita
+000004d0: 7469 6f6e 616c 2068 6172 6d6f 6e69 6373  tional harmonics
+000004e0: 2061 6e64 2067 656e 6572 616c 2072 656c   and general rel
+000004f0: 6174 6976 6973 7469 6320 636f 7272 6563  ativistic correc
+00000500: 7469 6f6e 732e 2041 5353 4953 5420 616c  tions. ASSIST al
+00000510: 736f 2061 6363 6f75 6e74 7320 666f 7220  so accounts for 
+00000520: 706f 7369 7469 6f6e 2d20 616e 6420 7665  position- and ve
+00000530: 6c6f 6369 7479 2d64 6570 656e 6465 6e74  locity-dependent
+00000540: 206e 6f6e 2d67 7261 7669 7461 7469 6f6e   non-gravitation
+00000550: 616c 2065 6666 6563 7473 2061 6363 6f72  al effects accor
+00000560: 6469 6e67 2074 6f20 7468 6520 5b4d 6172  ding to the [Mar
+00000570: 7364 656e 2028 3139 3733 2920 6d6f 6465  sden (1973) mode
+00000580: 6c5d 2868 7474 7073 3a2f 2f75 692e 6164  l](https://ui.ad
+00000590: 7361 6273 2e68 6172 7661 7264 2e65 6475  sabs.harvard.edu
+000005a0: 2f61 6273 2f31 3937 3341 4a2e 2e2e 2e2e  /abs/1973AJ.....
+000005b0: 3738 2e2e 3231 314d 2f61 6273 7472 6163  78..211M/abstrac
+000005c0: 7429 2e20 416c 6c20 636f 6d70 6f6e 656e  t). All componen
+000005d0: 7473 2069 6e20 7468 6520 6571 7561 7469  ts in the equati
+000005e0: 6f6e 7320 6f66 206d 6f74 696f 6e20 6861  ons of motion ha
+000005f0: 7665 2062 6565 6e20 7665 7269 6669 6564  ve been verified
+00000600: 2074 6f20 6d61 6368 696e 6520 7072 6563   to machine prec
+00000610: 6973 696f 6e20 696e 2061 2074 6572 6d2d  ision in a term-
+00000620: 6279 2d74 6572 6d20 636f 6d70 6172 6973  by-term comparis
+00000630: 6f6e 2077 6974 6820 6f75 7470 7574 2066  on with output f
+00000640: 726f 6d20 4a50 4c27 7320 736d 616c 6c20  rom JPL's small 
+00000650: 626f 6479 2069 6e74 6567 7261 746f 722e  body integrator.
+00000660: 2054 6865 2066 6972 7374 206f 7264 6572   The first order
+00000670: 2076 6172 6961 7469 6f6e 616c 2065 7175   variational equ
+00000680: 6174 696f 6e73 2061 7265 2069 6e63 6c75  ations are inclu
+00000690: 6465 6420 666f 7220 616c 6c20 7465 726d  ded for all term
+000006a0: 7320 746f 2073 7570 706f 7274 206f 7262  s to support orb
+000006b0: 6974 2066 6974 7469 6e67 2061 6e64 2063  it fitting and c
+000006c0: 6f76 6172 6961 6e63 6520 6d61 7070 696e  ovariance mappin
+000006d0: 672e 2054 6869 7320 6672 616d 6577 6f72  g. This framewor
+000006e0: 6b20 6973 206d 6561 6e74 2074 6f20 7072  k is meant to pr
+000006f0: 6f76 6964 6520 616e 206f 7065 6e2d 736f  ovide an open-so
+00000700: 7572 6365 2070 6163 6b61 6765 2077 7269  urce package wri
+00000710: 7474 656e 2069 6e20 6120 6d6f 6465 726e  tten in a modern
+00000720: 206c 616e 6775 6167 6520 746f 2065 6e61   language to ena
+00000730: 626c 6520 6869 6768 2d70 7265 6369 7369  ble high-precisi
+00000740: 6f6e 206f 7262 6974 616c 2061 6e61 6c79  on orbital analy
+00000750: 7369 7320 616e 6420 7363 6965 6e63 6520  sis and science 
+00000760: 6279 2074 6865 2073 6d61 6c6c 2062 6f64  by the small bod
+00000770: 7920 636f 6d6d 756e 6974 792e 0a0a 0a0a  y community.....
+00000780: 2323 2049 6e73 7461 6c6c 6174 696f 6e20  ## Installation 
+00000790: 2850 7974 686f 6e29 0a0a 4974 2773 2065  (Python)..It's e
+000007a0: 6173 6965 7374 2074 6f20 696e 7374 616c  asiest to instal
+000007b0: 6c20 4153 5349 5354 2069 6e74 6f20 6120  l ASSIST into a 
+000007c0: 7079 7468 6f6e 2076 6972 7475 616c 2065  python virtual e
+000007d0: 6e76 6972 6f6e 6d65 6e74 2e20 4966 2079  nvironment. If y
+000007e0: 6f75 2061 6c72 6561 6479 2068 6176 6520  ou already have 
+000007f0: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
+00000800: 6e6d 656e 7420 6f72 2064 6f20 6e6f 7420  nment or do not 
+00000810: 7761 6e74 2074 6f20 7573 6520 6f6e 652c  want to use one,
+00000820: 2079 6f75 2063 616e 2073 6b69 7020 7468   you can skip th
+00000830: 6973 2073 7465 702e 204f 7468 6572 7769  is step. Otherwi
+00000840: 7365 2c20 7275 6e20 7468 6520 666f 6c6c  se, run the foll
+00000850: 6f77 696e 6720 636f 6d6d 616e 6420 696e  owing command in
+00000860: 2061 6e20 656d 7074 7920 6469 7265 6374   an empty direct
+00000870: 6f72 792e 2054 6865 7920 7769 6c6c 2073  ory. They will s
+00000880: 6574 7570 2061 6e64 2061 6374 6976 6174  etup and activat
+00000890: 6520 6120 6e65 7720 7669 7274 7561 6c20  e a new virtual 
+000008a0: 656e 7669 726f 6e6d 656e 7420 696e 2061  environment in a
+000008b0: 2064 6972 6563 746f 7279 2e20 0a0a 2020   directory. ..  
+000008c0: 2020 7079 7468 6f6e 3320 2d6d 2076 656e    python3 -m ven
+000008d0: 7620 7665 6e76 0a20 2020 2073 6f75 7263  v venv.    sourc
+000008e0: 6520 7665 6e76 2f62 696e 2f61 6374 6976  e venv/bin/activ
+000008f0: 6174 650a 0a4e 6f77 2077 6520 6361 6e20  ate..Now we can 
+00000900: 696e 7374 616c 6c20 6e75 6d70 792c 2052  install numpy, R
+00000910: 4542 4f55 4e44 2c20 616e 6420 4153 5349  EBOUND, and ASSI
+00000920: 5354 3a0a 0a20 2020 2070 6970 2069 6e73  ST:..    pip ins
+00000930: 7461 6c6c 206e 756d 7079 0a20 2020 2070  tall numpy.    p
+00000940: 6970 2069 6e73 7461 6c6c 2072 6562 6f75  ip install rebou
+00000950: 6e64 200a 2020 2020 7069 7020 696e 7374  nd .    pip inst
+00000960: 616c 6c20 6173 7369 7374 0a0a 546f 2075  all assist..To u
+00000970: 7365 2075 7365 2041 5353 4953 542c 2079  se use ASSIST, y
+00000980: 6f75 2061 6c73 6f20 6e65 6564 2074 6f20  ou also need to 
+00000990: 646f 776e 6c6f 6164 2065 7068 656d 6572  download ephemer
+000009a0: 6973 2064 6174 6120 6669 6c65 732e 204f  is data files. O
+000009b0: 6e65 2066 696c 6520 666f 7220 706c 616e  ne file for plan
+000009c0: 6574 2065 7068 656d 6572 6973 2061 6e64  et ephemeris and
+000009d0: 2061 6e6f 7468 6572 2073 7570 6c65 6d65   another supleme
+000009e0: 6e74 6172 7920 6669 6c65 2066 6f72 2061  ntary file for a
+000009f0: 7374 6572 6f69 6420 6570 6865 6d65 7269  steroid ephemeri
+00000a00: 732e 2054 6865 2066 6f6c 6c6f 7769 6e67  s. The following
+00000a10: 2063 6f6d 6d61 6e64 7320 646f 776e 6c6f   commands downlo
+00000a20: 6164 2074 6865 7365 2066 696c 6573 2077  ad these files w
+00000a30: 6974 6820 6375 726c 2e20 596f 7520 6361  ith curl. You ca
+00000a40: 6e20 616c 736f 206d 616e 7561 6c6c 7920  n also manually 
+00000a50: 646f 776e 6c6f 6164 2074 6865 6d20 7573  download them us
+00000a60: 696e 6720 796f 7572 2062 726f 7773 6572  ing your browser
+00000a70: 2e20 4e6f 7465 2074 6861 7420 7468 6573  . Note that thes
+00000a80: 6520 6172 6520 6c61 7267 6520 6669 6c65  e are large file
+00000a90: 732c 2061 6c6d 6f73 7420 3147 4220 696e  s, almost 1GB in
+00000aa0: 2073 697a 652e 0a0a 2020 2020 6d6b 6469   size...    mkdi
+00000ab0: 7220 6461 7461 0a20 2020 2063 7572 6c20  r data.    curl 
+00000ac0: 6874 7470 733a 2f2f 7373 642e 6a70 6c2e  https://ssd.jpl.
+00000ad0: 6e61 7361 2e67 6f76 2f66 7470 2f65 7068  nasa.gov/ftp/eph
+00000ae0: 2f70 6c61 6e65 7473 2f4c 696e 7578 2f64  /planets/Linux/d
+00000af0: 6534 3430 2f6c 696e 7578 5f70 3135 3530  e440/linux_p1550
+00000b00: 7032 3635 302e 3434 3020 2d6f 2064 6174  p2650.440 -o dat
+00000b10: 612f 6c69 6e75 785f 7031 3535 3070 3236  a/linux_p1550p26
+00000b20: 3530 2e34 3430 0a20 2020 2063 7572 6c20  50.440.    curl 
+00000b30: 6874 7470 733a 2f2f 7373 642e 6a70 6c2e  https://ssd.jpl.
+00000b40: 6e61 7361 2e67 6f76 2f66 7470 2f65 7068  nasa.gov/ftp/eph
+00000b50: 2f73 6d61 6c6c 5f62 6f64 6965 732f 6173  /small_bodies/as
+00000b60: 7465 726f 6964 735f 6465 3434 312f 7362  teroids_de441/sb
+00000b70: 3434 312d 6e31 362e 6273 7020 2d6f 2064  441-n16.bsp -o d
+00000b80: 6174 612f 7362 3434 312d 6e31 362e 6273  ata/sb441-n16.bs
+00000b90: 700a 0a4e 6f77 2079 6f75 2063 616e 2074  p..Now you can t
+00000ba0: 7279 206f 7574 2069 6620 6173 7369 7374  ry out if assist
+00000bb0: 2077 6f72 6b73 2e0a 0a20 2020 2070 7974   works...    pyt
+00000bc0: 686f 6e33 0a0a 2020 2020 3e3e 3e20 696d  hon3..    >>> im
+00000bd0: 706f 7274 2061 7373 6973 740a 2020 2020  port assist.    
+00000be0: 3e3e 3e20 6570 6865 6d20 3d20 6173 7369  >>> ephem = assi
+00000bf0: 7374 2e45 7068 656d 2822 6461 7461 2f6c  st.Ephem("data/l
+00000c00: 696e 7578 5f70 3135 3530 7032 3635 302e  inux_p1550p2650.
+00000c10: 3434 3022 2c20 2264 6174 612f 7362 3434  440", "data/sb44
+00000c20: 312d 6e31 362e 6273 7022 290a 2020 2020  1-n16.bsp").    
+00000c30: 3e3e 3e20 7072 696e 7428 6570 6865 6d2e  >>> print(ephem.
+00000c40: 6a64 5f72 6566 290a 2020 2020 3e3e 3e20  jd_ref).    >>> 
+00000c50: 6570 6865 6d2e 6765 745f 7061 7274 6963  ephem.get_partic
+00000c60: 6c65 2822 4561 7274 6822 2c20 3029 0a0a  le("Earth", 0)..
+00000c70: 596f 7520 7368 6f75 6c64 2073 6565 2074  You should see t
+00000c80: 6865 2064 6566 6175 6c74 2072 6566 6572  he default refer
+00000c90: 656e 6365 204a 756c 6961 6e20 6461 7465  ence Julian date
+00000ca0: 2028 3234 3531 3534 352e 3029 2061 6e64   (2451545.0) and
+00000cb0: 2074 6865 2070 6f73 6974 696f 6e20 6f66   the position of
+00000cc0: 2074 6865 2045 6172 7468 2061 7420 7468   the Earth at th
+00000cd0: 6174 2074 696d 6520 7072 696e 7465 6420  at time printed 
+00000ce0: 6f6e 2074 6865 2073 6372 6565 6e2e 0a0a  on the screen...
+00000cf0: 2323 2049 6e73 7461 6c6c 6174 696f 6e20  ## Installation 
+00000d00: 2843 290a 0a54 6f20 696e 7374 616c 6c20  (C)..To install 
+00000d10: 7468 6520 4320 7665 7273 696f 6e20 6f66  the C version of
+00000d20: 2041 5353 4953 542c 2066 6972 7374 2063   ASSIST, first c
+00000d30: 6c6f 6e65 2074 6865 2052 4542 4f55 4e44  lone the REBOUND
+00000d40: 2061 6e64 2074 6865 6e20 7468 6520 4153   and then the AS
+00000d50: 5349 5354 2072 6570 6f73 6974 6f72 6965  SIST repositorie
+00000d60: 732e 2049 6e20 616e 2065 6d70 7479 2064  s. In an empty d
+00000d70: 6972 6563 746f 7279 2c20 7275 6e3a 0a0a  irectory, run:..
+00000d80: 2020 2020 6769 7420 636c 6f6e 6520 6874      git clone ht
+00000d90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000da0: 2f68 616e 6e6f 7265 696e 2f72 6562 6f75  /hannorein/rebou
+00000db0: 6e64 2e67 6974 0a20 2020 2067 6974 2063  nd.git.    git c
+00000dc0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00000dd0: 6875 622e 636f 6d2f 6d61 7474 6865 7768  hub.com/matthewh
+00000de0: 6f6c 6d61 6e2f 6173 7369 7374 2e67 6974  olman/assist.git
+00000df0: 0a0a 546f 2075 7365 2075 7365 2041 5353  ..To use use ASS
+00000e00: 4953 542c 2079 6f75 2061 6c73 6f20 6e65  IST, you also ne
+00000e10: 6564 2074 6f20 646f 776e 6c6f 6164 2065  ed to download e
+00000e20: 7068 656d 6572 6973 2064 6174 6120 6669  phemeris data fi
+00000e30: 6c65 732e 204f 6e65 2066 696c 6520 666f  les. One file fo
+00000e40: 7220 706c 616e 6574 2065 7068 656d 6572  r planet ephemer
+00000e50: 6973 2061 6e64 2061 6e6f 7468 6572 2073  is and another s
+00000e60: 7570 6c65 6d65 6e74 6172 7920 6669 6c65  uplementary file
+00000e70: 2066 6f72 2061 7374 6572 6f69 6420 6570   for asteroid ep
+00000e80: 6865 6d65 7269 732e 2054 6865 2066 6f6c  hemeris. The fol
+00000e90: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 7320  lowing commands 
+00000ea0: 646f 776e 6c6f 6164 2074 6865 7365 2066  download these f
+00000eb0: 696c 6573 2077 6974 6820 6375 726c 2e20  iles with curl. 
+00000ec0: 596f 7520 6361 6e20 616c 736f 206d 616e  You can also man
+00000ed0: 7561 6c6c 7920 646f 776e 6c6f 6164 2074  ually download t
+00000ee0: 6865 6d20 7573 696e 6720 796f 7572 2062  hem using your b
+00000ef0: 726f 7773 6572 2e20 4e6f 7465 2074 6861  rowser. Note tha
+00000f00: 7420 7468 6573 6520 6172 6520 6c61 7267  t these are larg
+00000f10: 6520 6669 6c65 732c 2061 6c6d 6f73 7420  e files, almost 
+00000f20: 3147 4220 696e 2073 697a 652e 0a0a 2020  1GB in size...  
+00000f30: 2020 6375 726c 2068 7474 7073 3a2f 2f73    curl https://s
+00000f40: 7364 2e6a 706c 2e6e 6173 612e 676f 762f  sd.jpl.nasa.gov/
+00000f50: 6674 702f 6570 682f 706c 616e 6574 732f  ftp/eph/planets/
+00000f60: 4c69 6e75 782f 6465 3434 302f 6c69 6e75  Linux/de440/linu
+00000f70: 785f 7031 3535 3070 3236 3530 2e34 3430  x_p1550p2650.440
+00000f80: 202d 6f20 6173 7369 7374 2f64 6174 612f   -o assist/data/
+00000f90: 6c69 6e75 785f 7031 3535 3070 3236 3530  linux_p1550p2650
+00000fa0: 2e34 3430 0a20 2020 2063 7572 6c20 6874  .440.    curl ht
+00000fb0: 7470 733a 2f2f 7373 642e 6a70 6c2e 6e61  tps://ssd.jpl.na
+00000fc0: 7361 2e67 6f76 2f66 7470 2f65 7068 2f73  sa.gov/ftp/eph/s
+00000fd0: 6d61 6c6c 5f62 6f64 6965 732f 6173 7465  mall_bodies/aste
+00000fe0: 726f 6964 735f 6465 3434 312f 7362 3434  roids_de441/sb44
+00000ff0: 312d 6e31 362e 6273 7020 2d6f 2061 7373  1-n16.bsp -o ass
+00001000: 6973 742f 6461 7461 2f73 6234 3431 2d6e  ist/data/sb441-n
+00001010: 3136 2e62 7370 0a0a 466f 7220 736f 6d65  16.bsp..For some
+00001020: 206f 6620 7468 6520 6578 616d 706c 6573   of the examples
+00001030: 2c20 796f 7520 7769 6c6c 2061 6c73 6f20  , you will also 
+00001040: 6e65 6564 2074 6865 2070 6c61 6e65 7420  need the planet 
+00001050: 6570 6865 6d65 7269 7320 6669 6c65 2077  ephemeris file w
+00001060: 6974 6820 616e 2065 7874 656e 6465 6420  ith an extended 
+00001070: 636f 7665 7261 6765 2e20 4e6f 7465 2074  coverage. Note t
+00001080: 6861 7420 7468 6973 2066 696c 6520 6973  hat this file is
+00001090: 2032 2e36 4742 2069 6e20 7369 7a65 2e0a   2.6GB in size..
+000010a0: 0a20 2020 2063 7572 6c20 6874 7470 733a  .    curl https:
+000010b0: 2f2f 7373 642e 6a70 6c2e 6e61 7361 2e67  //ssd.jpl.nasa.g
+000010c0: 6f76 2f66 7470 2f65 7068 2f70 6c61 6e65  ov/ftp/eph/plane
+000010d0: 7473 2f4c 696e 7578 2f64 6534 3431 2f6c  ts/Linux/de441/l
+000010e0: 696e 7578 5f6d 3133 3030 3070 3137 3030  inux_m13000p1700
+000010f0: 302e 3434 3120 2d6f 2061 7373 6973 742f  0.441 -o assist/
+00001100: 6461 7461 2f6c 696e 7578 5f6d 3133 3030  data/linux_m1300
+00001110: 3070 3137 3030 302e 3434 310a 0a4e 6578  0p17000.441..Nex
+00001120: 742c 2067 6f20 746f 206f 6e65 206f 6620  t, go to one of 
+00001130: 7468 6520 6578 616d 706c 6520 6469 7265  the example dire
+00001140: 6374 6f72 6965 7320 616e 6420 636f 6d70  ctories and comp
+00001150: 696c 6520 7468 6520 7072 6f62 6c65 6d20  ile the problem 
+00001160: 6669 6c65 2e20 5468 6973 2077 696c 6c20  file. This will 
+00001170: 616c 736f 2074 7269 6767 6572 2074 6865  also trigger the
+00001180: 2069 6e73 7461 6c6c 6174 696f 6e20 6f66   installation of
+00001190: 2074 6865 2052 4542 4f55 4e44 2061 6e64   the REBOUND and
+000011a0: 2041 5353 4953 5420 7368 6172 6564 206c   ASSIST shared l
+000011b0: 6962 7261 7269 6573 2e0a 0a20 2020 2063  ibraries...    c
+000011c0: 6420 6173 7369 7374 2f65 7861 6d70 6c65  d assist/example
+000011d0: 732f 706c 6169 6e5f 696e 7465 7266 6163  s/plain_interfac
+000011e0: 650a 2020 2020 6d61 6b65 0a0a 4e6f 772c  e.    make..Now,
+000011f0: 2079 6f75 2772 6520 7265 6164 7920 746f   you're ready to
+00001200: 2072 756e 2074 6865 2065 7861 6d70 6c65   run the example
+00001210: 2077 6974 683a 0a0a 2020 2020 2e2f 7265   with:..    ./re
+00001220: 626f 756e 640a 0a0a 2323 204c 6963 656e  bound...## Licen
+00001230: 7365 0a41 5353 4953 5420 6973 206f 7065  se.ASSIST is ope
+00001240: 6e20 736f 7572 6365 2c20 6672 6565 6c79  n source, freely
+00001250: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
+00001260: 6572 2074 6865 205b 474e 5520 4765 6e65  er the [GNU Gene
+00001270: 7261 6c20 5075 626c 6963 206c 6963 656e  ral Public licen
+00001280: 7365 2c20 7665 7273 696f 6e20 335d 2868  se, version 3](h
+00001290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000012a0: 6d2f 6d61 7474 6865 7768 6f6c 6d61 6e2f  m/matthewholman/
+000012b0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+000012c0: 4529 2e0a 0a23 2320 436f 6e74 7269 6275  E)...## Contribu
+000012d0: 746f 7273 0a0a 2a20 4d61 7474 6865 7720  tors..* Matthew 
+000012e0: 4a2e 2048 6f6c 6d61 6e2c 2043 656e 7465  J. Holman, Cente
+000012f0: 7220 666f 7220 4173 7472 6f70 6879 7369  r for Astrophysi
+00001300: 6373 207c 2048 6172 7661 7264 2026 2053  cs | Harvard & S
+00001310: 6d69 7468 736f 6e69 616e 2c20 3c6d 686f  mithsonian, <mho
+00001320: 6c6d 616e 4063 6661 2e68 6172 7661 7264  lman@cfa.harvard
+00001330: 2e65 6475 3e0a 2a20 4172 7961 2041 6b6d  .edu>.* Arya Akm
+00001340: 616c 2c20 4d6f 6e74 676f 6d65 7279 2043  al, Montgomery C
+00001350: 6f6c 6c65 6765 2c20 526f 636b 7669 6c6c  ollege, Rockvill
+00001360: 650a 2a20 4461 7669 6465 2046 6172 6e6f  e.* Davide Farno
+00001370: 6363 6869 612c 204a 6574 2050 726f 7075  cchia, Jet Propu
+00001380: 6c73 696f 6e20 4c61 626f 7261 746f 7279  lsion Laboratory
+00001390: 2c20 4361 6c69 666f 726e 6961 2049 6e73  , California Ins
+000013a0: 7469 7475 7465 206f 6620 5465 6368 6e6f  titute of Techno
+000013b0: 6c6f 6779 200a 2a20 4861 6e6e 6f20 5265  logy .* Hanno Re
+000013c0: 696e 2c20 556e 6976 6572 7369 7479 206f  in, University o
+000013d0: 6620 546f 726f 6e74 6f2c 203c 6861 6e6e  f Toronto, <hann
+000013e0: 6f40 6861 6e6e 6f2d 7265 696e 2e64 653e  o@hanno-rein.de>
+000013f0: 0a2a 204d 6174 7468 6577 204a 2e20 5061  .* Matthew J. Pa
+00001400: 796e 652c 2043 656e 7465 7220 666f 7220  yne, Center for 
+00001410: 4173 7472 6f70 6879 7369 6373 207c 2048  Astrophysics | H
+00001420: 6172 7661 7264 2026 2053 6d69 7468 736f  arvard & Smithso
+00001430: 6e69 616e 0a2a 2052 6f62 6572 7420 5765  nian.* Robert We
+00001440: 7279 6b2c 2055 6e69 7665 7273 6974 7920  ryk, University 
+00001450: 6f66 2057 6573 7465 726e 204f 6e74 6172  of Western Ontar
+00001460: 696f 0a2a 2044 616e 2054 616d 6179 6f2c  io.* Dan Tamayo,
+00001470: 2048 6172 7665 7920 4d75 6464 2043 6f6c   Harvey Mudd Col
+00001480: 6c65 6765 2c20 3c64 7461 6d61 796f 4068  lege, <dtamayo@h
+00001490: 6d63 2e65 6475 3e0a 2a20 4461 7669 6420  mc.edu>.* David 
+000014a0: 4d2e 2048 6572 6e61 6e64 657a 2c20 4365  M. Hernandez, Ce
+000014b0: 6e74 6572 2066 6f72 2041 7374 726f 7068  nter for Astroph
+000014c0: 7973 6963 7320 7c20 4861 7276 6172 6420  ysics | Harvard 
+000014d0: 2620 536d 6974 6873 6f6e 6961 6e20 0a0a  & Smithsonian ..
+000014e0: 0a                                       .
```

### Comparing `assist-1.1.1/assist/__init__.py` & `assist-1.1.2/assist/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,30 +8,40 @@
 
 #Import shared C library
 import os
 pymodulespath = os.path.dirname(__file__)
 from ctypes import *
 clibassist = cdll.LoadLibrary(pymodulespath + '/../libassist' + suffix)
 
-# Version
-__version__ = c_char_p.in_dll(clibassist, "assist_version_str").value.decode('ascii')
 
-# Build
-__build__ = c_char_p.in_dll(clibassist, "assist_build_str").value.decode('ascii')
-# Check for version
+def _libassist_str(name: str) -> str:
+    """Extract a string from libassist, referencing it by symbol
+    name. Raise a RuntimeError if the name is not present.
 
-# Githash
-__githash__ = c_char_p.in_dll(clibassist, "assist_githash_str").value.decode('ascii')
+    """
+    val = c_char_p.in_dll(clibassist, name).value
+    if val is None:
+        raise RuntimeError(f"unable to find symbol {name} in libassist")
+    return val.decode("ascii")
 
-def assist_error_messages(e):
+__version__ = _libassist_str("assist_version_str")
+
+__build__ = _libassist_str("assist_build_str")
+
+__githash__ = _libassist_str("assist_githash_str")
+
+
+def assist_error_messages(e: int) -> str:
     e_N = c_int.in_dll(clibassist, "assist_error_messages_N").value
     if e >= e_N:
-        raise RuntimeError("And error occured while trying to process an ASSIST error message.")
+        raise RuntimeError("An error occured while trying to process an ASSIST error message.")
     ccpp  = c_char_p * e_N
     message = ccpp.in_dll(clibassist, "assist_error_messages")[e]
+    if message is None:
+        raise RuntimeError("assist_error_messages is missing from libassist. Please report this issue on GitHub.")
     return message.decode("ascii")
 
 try:
     import pkg_resources
     moduleversion = pkg_resources.require("assist")[0].version
     libassistversion = __version__
     if moduleversion != libassistversion:
```

### Comparing `assist-1.1.1/assist/ephem.py` & `assist-1.1.2/assist/ephem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional, Union
+
 from . import clibassist, assist_error_messages
 from ctypes import Structure, c_double, POINTER, c_int, c_uint, c_long, c_ulong, c_void_p, c_char_p, CFUNCTYPE, byref, c_uint32, c_uint, cast, c_char
 import rebound
 import assist
 import warnings
 
 ASSIST_BODY_IDS = {
@@ -35,47 +37,53 @@
         }
 
 class Ephem(Structure):
     """
     Main object used for all ASSIST Ephemeris operations.
     Not tied to a particular REBOUND simulation.
     """
-    
-    def __init__(self, planets_path=None, asteroids_path=None):
+
+    def __init__(self, planets_path: Optional[str] = None, asteroids_path: Optional[str] = None):
         if planets_path is not None:
-            planets_path = planets_path.encode("ascii")
+            c_planets_path = c_char_p(str(planets_path).encode("ascii"))
+        else:
+            c_planets_path = c_char_p(None)
+
         if asteroids_path is not None:
-            asteroids_path = asteroids_path.encode("ascii")
+            c_asteroids_path = c_char_p(str(asteroids_path).encode("ascii"))
+        else:
+            c_asteroids_path = c_char_p(None)
+
         clibassist.assist_ephem_init.restype = c_int
-        ret = clibassist.assist_ephem_init(byref(self), c_char_p(planets_path), c_char_p(asteroids_path))
+        ret = clibassist.assist_ephem_init(byref(self), c_planets_path, c_asteroids_path)
         if ret != 0:
             raise RuntimeError(assist_error_messages(ret))
 
-    def get_particle(self, body, t):
+    def get_particle(self, body: Union[int, str], t: float) -> rebound.Particle:
         if isinstance(body, str):
             body_str = body.lower()
             body = -1
             for k in ASSIST_BODY_IDS:
                 if body_str == ASSIST_BODY_IDS[k].lower():
                     body = k
             if body < 0:
-                raise ValueError("Cannot find body '"+body_str+"'. Needs to be one of: "+", ".join([ASSIST_BODY_IDS[k] for k in ASSIST_BODY_IDS])+".")
+                raise ValueError("Cannot find body '" + body_str + "'. Needs to be one of: " + ", ".join([ASSIST_BODY_IDS[k] for k in ASSIST_BODY_IDS]) + ".")
         if not isinstance(body, int):
             raise ValueError("Expecting integer for body id.")
 
         clibassist.assist_get_particle_with_error.restype = rebound.Particle
         e = c_int(0)
-        p = clibassist.assist_get_particle_with_error(byref(self), c_int(body), c_double(t), byref(e))
+        p = clibassist.assist_get_particle_with_error(
+            byref(self), c_int(body), c_double(t), byref(e)
+        )
         if e.value:
             raise RuntimeError(assist_error_messages(e.value))
         return p
 
-
-
-    def __del__(self):
+    def __del__(self) -> None:
         clibassist.assist_ephem_free_pointers(byref(self))
 
     _fields_ =  [("jd_ref", c_double),
                  ("_pl", c_void_p),
                  ("_spl", c_void_p),
             ]
```

### Comparing `assist-1.1.1/assist/extras.py` & `assist-1.1.2/assist/extras.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,80 @@
+from typing import NoReturn, List
+
 from . import clibassist
 from ctypes import Structure, c_double, POINTER, c_int, c_uint, c_long, c_ulong, c_void_p, c_char_p, CFUNCTYPE, byref, c_uint32, c_uint, cast, c_char
 import rebound
 import warnings
 from .ephem import Ephem
+import numpy as np
+import numpy.typing as npt
 
 ASSIST_FORCES = {
     "SUN"                : 0x01,
     "PLANETS"            : 0x02,
     "ASTEROIDS"          : 0x04,
     "NON_GRAVITATIONAL"  : 0x08,
     "EARTH_HARMONICS"    : 0x10,
     "SUN_HARMONICS"      : 0x20,
     "GR_EIH"             : 0x40,
     "GR_SIMPLE"          : 0x80,
     "GR_POTENTIAL"       : 0x100,
-} 
+}
 
 class Extras(Structure):
     """
     Main object used for all ASSIST operations, tied to a particular REBOUND simulation.
     This is an abstraction of the C struct assist_extras.
     """
-    
-    def __init__(self, sim, ephem):
-        sim._extras_ref = self # add a reference to this instance in sim to make sure it's not garbage collected_ 
+    def __init__(self, sim: rebound.Simulation, ephem: Ephem):
+        sim._extras_ref = self  # add a reference to this instance in sim to make sure it's not garbage collected_
         clibassist.assist_init(byref(self), byref(sim), byref(ephem))
+        # set up units and frame to allow direct access to JPL Horizons via REBOUND
+        sim.update_units(("au","day","massist"))
+        sim.default_plane = "frame"
         self.extras_should_free_ephem = 0
 
-    def __del__(self):
+    def __del__(self) -> None:
         clibassist.assist_free_pointers(byref(self))
 
-    def detach(self, sim):
-        sim._extras_ref = None # remove reference to assist so it can be garbage collected 
+    def detach(self, sim: rebound.Simulation) -> None:
+        sim._extras_ref = None # remove reference to assist so it can be garbage collected
         clibassist.assist_detach(byref(sim), byref(self))
 
-    def integrate_or_interpolate(self, t):
+    def integrate_or_interpolate(self, t: float) -> None:
         clibassist.assist_integrate_or_interpolate(byref(self), c_double(t))
-    
+
     @property
-    def forces(self):
+    def forces(self) -> List[str]:
         l = []
         for k in ASSIST_FORCES:
-            if self._forces & ASSIST_FORCES[k]:
+            if self._forces & ASSIST_FORCES[k]:  # type: ignore
                 l.append(k)
         return l
     @forces.setter
-    def forces(self, value):
+    def forces(self, value: List[str]) -> None:
         if not isinstance(value, list):
             raise AttributeError("Forces need to be a list.")
-        for v in value:
-            if not isinstance(v, str):
+        for elem in value:
+            if not isinstance(elem, str):
                 raise AttributeError("Each force needs to be a string.")
-            if v.upper() not in ASSIST_FORCES:
-                raise AttributeError("Force '"+v+"' not recognized. Needs to be one of the following: "+", ".join(ASSIST_FORCES))
+            if elem.upper() not in ASSIST_FORCES:
+                raise AttributeError("Force '"+elem+"' not recognized. Needs to be one of the following: "+", ".join(ASSIST_FORCES))
         v = 0
         for k in ASSIST_FORCES:
             if k in value:
                 v = v | ASSIST_FORCES[k]
         self._forces = c_int(v)
 
     @property
-    def particle_params(self):
+    def particle_params(self) -> NoReturn:
         raise AttributeError("Cannot get particle_params. Only setting is supported.")
 
     @particle_params.setter
-    def particle_params(self, value):
+    def particle_params(self, value: npt.NDArray[np.float64]) -> None:
         self._particle_params_reference = value.copy() # keep copy of array to avoid it beeing freed
         value_p = self._particle_params_reference.ctypes.data_as(POINTER(c_double))
         self._particle_params = value_p
 
 
 
     _fields_ =  [("_sim", POINTER(rebound.Simulation)),
```

### Comparing `assist-1.1.1/assist.egg-info/PKG-INFO` & `assist-1.1.2/assist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assist
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library high accuracy ephemeris in REBOUND
 Home-page: https://github.com/matthewholman/assist
 Author: Matthew Holman
 Author-email: mholman@cfa.harvard.edu
 License: GPL
 Keywords: astronomy astrophysics nbody integrator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,21 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Version](https://img.shields.io/badge/assist-v1.1.1-green.svg?style=flat)](https://assist.readthedocs.org)
+[![Version](https://img.shields.io/badge/assist-v1.1.2-green.svg?style=flat)](https://assist.readthedocs.org)
 [![GPL](https://img.shields.io/badge/license-GPL-green.svg?style=flat)](https://github.com/matthewholman/blob/main/LICENSE)
 [![Python unit tests)](https://github.com/matthewholman/assist/actions/workflows/python.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/python.yml)
 [![C unit tests](https://github.com/matthewholman/assist/actions/workflows/c.yml/badge.svg)](https://github.com/matthewholman/assist/actions/workflows/c.yml)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7778016.svg)](https://doi.org/10.5281/zenodo.7778016)
+
+
 
 # ASSIST
 
 ASSIST is a software package for ephemeris-quality integrations of test particles. ASSIST is an extension of the [REBOUND framework](https://github.com/hannorein/rebound) and makes use of its [IAS15 integrator](https://ui.adsabs.harvard.edu/abs/2015MNRAS.446.1424R/abstract) to integrate test particle trajectories in the field of the Sun, Moon, planets, and 16 massive asteroids, with the positions of the masses coming from the JPL DE441 ephemeris and its associated asteroid perturber file. The package incorporates the most significant gravitational harmonics and general relativistic corrections. ASSIST also accounts for position- and velocity-dependent non-gravitational effects according to the [Marsden (1973) model](https://ui.adsabs.harvard.edu/abs/1973AJ.....78..211M/abstract). All components in the equations of motion have been verified to machine precision in a term-by-term comparison with output from JPL's small body integrator. The first order variational equations are included for all terms to support orbit fitting and covariance mapping. This framework is meant to provide an open-source package written in a modern language to enable high-precision orbital analysis and science by the small body community.
```

### Comparing `assist-1.1.1/setup.py` & `assist-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DASSISTGITHASH="+ghash
 except:
-    ghash_arg = "-DASSISTGITHASH=b9c30cd01aefc5be3786f0d0b50bd0fe2c3c328e" #GITHASHAUTOUPDATE
+    ghash_arg = "-DASSISTGITHASH=14a8eee16015ce67506db3c69a060428d026ffaa" #GITHASHAUTOUPDATE
 
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
 
         try:
             import rebound
@@ -73,15 +73,15 @@
                     )
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='assist',
-    version='1.1.1',
+    version='1.1.2',
     description='A library high accuracy ephemeris in REBOUND',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/matthewholman/assist',
     author='Matthew Holman',
     author_email='mholman@cfa.harvard.edu',
     license='GPL',
@@ -103,15 +103,15 @@
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
     ],
     keywords='astronomy astrophysics nbody integrator',
     packages=['assist'],
-    package_data = {'assist':['assist.h']},      
+    package_data={"assist": ["assist.h", "py.typed"]},
     cmdclass={'build_ext':build_ext},
     setup_requires=['rebound>=3.10.0', 'numpy'],
     install_requires=['rebound>=3.10.0', 'numpy'],
     tests_require=["numpy","matplotlib","rebound"],
     test_suite="assist.test",
     ext_modules = [libassistmodule],
     zip_safe=False)
```

### Comparing `assist-1.1.1/src/assist.c` & `assist-1.1.2/src/assist.c`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,14 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with ASSIST. If not, see <http://www.gnu.org/licenses/>.
  *
  */
 
-#include "const.h"
-
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 #include <stdint.h>
 #include <math.h>
 #include <limits.h>
 #include <float.h>
@@ -42,24 +40,24 @@
 const int reb_max_messages_length = 1024;   // needs to be constant expression for array size
 const int reb_max_messages_N = 10;
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* assist_build_str = __DATE__ " " __TIME__;   // Date and time build string. 
-const char* assist_version_str = "1.1.1";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* assist_version_str = "1.1.2";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* assist_githash_str = STRINGIFY(ASSISTGITHASH);// This line gets updated automatically. Do not edit manually.
 
 
 // These correspond to ASSIST_STATUS enum.
 
 const char* assist_error_messages[] = {
     "No error has occured.", // ASSIST_SUCCESS
     "The JPL planet ephemeris file has not been found.", // ASSIST_ERROR_EPHEM_FILE
-    "The JPL asteroid ephemeris file has not been found.", // ASSIST_ERROR_AST_FILE
+    "The JPL asteroid ephemeris file has not been found. Asteroid forces have been disabled.", // ASSIST_ERROR_AST_FILE
     "The requested asteroid ID has not been found.", // ASSIST_ERROR_NAST
     "The requested planet ID has not been found.", // ASSIST_ERROR_NEPHEM
     "The requested time is outside the coverage provided by the ephemeris file.", // ASSIST_ERROR_COVERAGE
 };
 const int assist_error_messages_N = ASSIST_ERROR_N;
 
     
@@ -119,26 +117,111 @@
         strncpy(planets_path, user_planets_path, FNAMESIZE-1);	
     }
 
     if ((ephem->jpl = assist_jpl_init(planets_path)) == NULL) {
         return ASSIST_ERROR_EPHEM_FILE;	  
     }
 
-    if(user_asteroids_path == NULL && getenv("ASSIST_DIR")==NULL){
-        return ASSIST_ERROR_AST_FILE;	  
-    }
+    int asteroids_path_not_found = 0;
+
 
     if(user_asteroids_path == NULL){
-        sprintf(asteroids_path, "%s%s", getenv("ASSIST_DIR"), default_asteroids_path);
+        if(getenv("ASSIST_DIR")==NULL){
+            asteroids_path_not_found = 1;
+        }else{
+            sprintf(asteroids_path, "%s%s", getenv("ASSIST_DIR"), default_asteroids_path);
+        }
     }else{
         strncpy(asteroids_path, user_asteroids_path, FNAMESIZE-1);	
     }
 
-    if ((ephem->spl = assist_spk_init(asteroids_path)) == NULL) {
-        return ASSIST_ERROR_AST_FILE;	  
+    if (asteroids_path_not_found != 1){
+        if ((ephem->spl = assist_spk_init(asteroids_path)) == NULL) {
+            asteroids_path_not_found = 1;
+        }
+    }
+            
+    if (asteroids_path_not_found != 1){
+        // Try to find masses of bodies in spk file in ephemeris constants
+        for(int n=0; n<ephem->spl->num; n++){ // loop over all asteroids
+            int found = 0;
+            for(int c=0; c<ephem->jpl->num; c++){ // loop over all constants
+                if (strncmp(ephem->jpl->str[c], "MA", 2) == 0) {
+                    int cid = atoi(ephem->jpl->str[c]+2);
+                    int offset = 2000000;
+                    if (cid==ephem->spl->targets[n].code-offset){
+                        ephem->spl->targets[n].mass = ephem->jpl->con[c];
+                        found = 1;
+                        break;
+                    }
+                }
+            }
+            // Use lookup table for new KBO objects in DE440/441
+            // Source: https://ssd.jpl.nasa.gov/ftp/eph/planets/bsp/README.txt
+            int massmap[] = {
+                // ID, SPK_ID
+                8001,  2136199,
+                8002,  2136108,
+                8003,  2090377,
+                8004,  2136472,
+                8005,  2050000,
+                8006,  2084522,
+                8007,  2090482,
+                8008,  2020000,
+                8009,  2055637,
+                8010,  2028978,
+                8011,  2307261,
+                8012,  2174567,
+                8013,  3361580,
+                8014,  3308265,
+                8015,  2055565,
+                8016,  2145452,
+                8017,  2090568,
+                8018,  2208996,
+                8019,  2225088,
+                8020,  2019521,
+                8021,  2120347,
+                8022,  2278361,
+                8023,  3525142,
+                8024,  2230965,
+                8025,  2042301,
+                8026,  2455502,
+                8027,  3545742,
+                8028,  2523639,
+                8029,  2528381,
+                8030,  3515022,
+            };
+            if (found==0){
+                int mapped = -1;
+                for (int m=0; m<sizeof(massmap); m+=2){
+                    if (massmap[m+1]==ephem->spl->targets[n].code){
+                        mapped = massmap[m];
+                        break;
+                    }
+                }
+                if (mapped != -1){
+                    for(int c=0; c<ephem->jpl->num; c++){ // loop over all constants (again)
+                        if (strncmp(ephem->jpl->str[c], "MA", 2) == 0) {
+                            int cid = atoi(ephem->jpl->str[c]+2);
+                            if (cid==mapped){
+                                ephem->spl->targets[n].mass = ephem->jpl->con[c];
+                                found = 1;
+                                break;
+                            }
+                        }
+                    }
+                }
+            }
+            if (found==0){
+                fprintf(stderr,"WARNING: Cannot find mass for asteroid %d (NAIF ID Number %d).\n", n, ephem->spl->targets[n].code );
+            }
+
+        }
+    }else{
+        fprintf(stderr, "(ASSIST) %s\n", assist_error_messages[ASSIST_ERROR_AST_FILE]);
     }
 
     return ASSIST_SUCCESS;
 }
 
 struct assist_ephem* assist_ephem_create(char *user_planets_path, char *user_asteroids_path){
     struct assist_ephem* ephem = calloc(1, sizeof(struct assist_ephem));
@@ -193,15 +276,18 @@
     struct assist_extras* assist = sim->extras;
     assist->sim = NULL;
 }
 
 void assist_init(struct assist_extras* assist, struct reb_simulation* sim, struct assist_ephem* ephem){
     assist->sim = sim;
     assist->ephem_cache = calloc(1, sizeof(struct assist_ephem_cache));
-    const int N_total = ASSIST_BODY_NPLANETS + ASSIST_BODY_NASTEROIDS;
+    int N_total = ASSIST_BODY_NPLANETS;
+    if (ephem->spl){
+        N_total += ephem->spl->num;
+    }
     assist->gr_eih_sources = 1; // Only include Sun by default
     assist->ephem_cache->items = calloc(N_total*7, sizeof(struct assist_cache_item));
     assist->ephem_cache->t = malloc(N_total*7*sizeof(double));
     for (int i=0;i<7*N_total;i++){
         assist->ephem_cache->t[i] = -1e306;
     }
```

### Comparing `assist-1.1.1/src/forces.c` & `assist-1.1.2/src/forces.c`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 #include <string.h>
 #include <stdint.h>
 #include <math.h>
 #include <limits.h>
 #include <float.h>
 #include "assist.h"
 #include "rebound.h"
-#include "const.h"
 #include "spk.h"
 #include "planets.h"
 #include "forces.h"
 
 
 // Forward function declarations
 static void assist_additional_force_direct(struct reb_simulation* sim, double xo, double yo, double zo, FILE *outfile);
@@ -274,47 +273,40 @@
     const double t = sim->t;    
 
     struct reb_particle* const particles = sim->particles;
 
     double GM;
     double x, y, z, vx, vy, vz, ax, ay, az;
 
-    static const int order[ASSIST_BODY_NPLANETS + ASSIST_BODY_NASTEROIDS] = { 
-        ASSIST_BODY_CYBELE,
-        ASSIST_BODY_EUPHROSYNE,
-        ASSIST_BODY_IRIS,
-        ASSIST_BODY_THISBE,
-        ASSIST_BODY_CAMILLA,
-        ASSIST_BODY_PSYCHE,
-        ASSIST_BODY_JUNO,
-        ASSIST_BODY_EUNOMIA,
-        ASSIST_BODY_SYLVIA,
-        ASSIST_BODY_EUROPA,
-        ASSIST_BODY_INTERAMNIA,
-        ASSIST_BODY_DAVIDA,
-        ASSIST_BODY_HYGIEA,
-        ASSIST_BODY_PALLAS,
-        ASSIST_BODY_VESTA,
-        ASSIST_BODY_CERES,
+    static const int order[ASSIST_BODY_NPLANETS] = { 
         ASSIST_BODY_PLUTO,
         ASSIST_BODY_MOON,
         ASSIST_BODY_MARS,
         ASSIST_BODY_MERCURY,
         ASSIST_BODY_NEPTUNE,
         ASSIST_BODY_URANUS,
         ASSIST_BODY_EARTH,
         ASSIST_BODY_VENUS,
         ASSIST_BODY_SATURN,
         ASSIST_BODY_JUPITER,
         ASSIST_BODY_SUN
     };
+    int spl_num = 0;
+    if (ephem->spl){
+        spl_num += ephem->spl->num;
+    }
 
     // Direct forces from massives bodies
-    for (int k=0; k < ASSIST_BODY_NPLANETS + ASSIST_BODY_NASTEROIDS; k++){
-        int i = order[k];
+    for (int k=0; k < ASSIST_BODY_NPLANETS + spl_num; k++){
+        int i; // ordered index
+        if (k>=spl_num){
+            i = order[k-spl_num]; // planets and sun last 
+        }else{
+            i = k + ASSIST_BODY_NPLANETS; // asteroids first
+        }
         if (i==ASSIST_BODY_SUN && !(assist->forces & ASSIST_FORCE_SUN)) continue;
         if (i>ASSIST_BODY_SUN && i<ASSIST_BODY_NPLANETS && !(assist->forces & ASSIST_FORCE_PLANETS)) continue;
         if (i>=ASSIST_BODY_NPLANETS && !(assist->forces & ASSIST_FORCE_ASTEROIDS)) continue;
 
         // Get position and mass of massive body i.
         // TOOD: make a version that returns the positions, velocities,
         // and accelerations for all the bodies at a given time.
@@ -349,17 +341,22 @@
     }
 
     // Acceleration of variational particles due to direct forces from massive bodies 
     // Loop over the perturbers
     // We should put a check at the top to see if there are any variational
     // particles.
 
-    for (int k=0; k < ASSIST_BODY_NPLANETS + ASSIST_BODY_NASTEROIDS; k++){
-	int i = order[k];
-	//int i = k;
+    for (int k=0; k < ASSIST_BODY_NPLANETS + spl_num; k++){
+        int i; // ordered index
+        if (k>=spl_num){
+            i = order[k-spl_num]; // planets and sun last 
+        }else{
+            i = k + ASSIST_BODY_NPLANETS; // asteroids first
+        }
+        // Note need checks for force flags here. TODO!
 
         // Get position and mass of massive body i.	
 	int flag = assist_all_ephem(ephem, assist->ephem_cache, i, t, &GM, &x, &y, &z, &vx, &vy, &vz, &ax, &ay, &az);
 
 	if(flag != ASSIST_SUCCESS){
         reb_error(sim, assist_error_messages[flag]);
 	}
@@ -458,19 +455,18 @@
     double xe, ye, ze, vxe, vye, vze, axe, aye, aze;    
     assist_all_ephem(ephem, assist->ephem_cache, ASSIST_BODY_EARTH, t, &GM, &xe, &ye, &ze, &vxe, &vye, &vze, &axe, &aye, &aze);
     const double GMearth = GM;
 
     double xr, yr, zr; //, vxr, vyr, vzr, axr, ayr, azr;
     xr = xe;  yr = ye;  zr = ze;
 
-    const double J2e = JPL_EPHEM_J2E;
-    const double J3e = JPL_EPHEM_J3E;
-    const double J4e = JPL_EPHEM_J4E;
-    const double au = JPL_EPHEM_CAU;
-    const double Re_eq = JPL_EPHEM_RE/au;
+    const double J2e = ephem->jpl->J2E;
+    const double J3e = ephem->jpl->J3E;
+    const double J4e = ephem->jpl->J4E;
+    const double Re_eq = ephem->jpl->RE/ephem->jpl->AU;
 
     // Unit vector to equatorial pole at the epoch
     // Note also that the pole orientation is not changing during
     // the integration.
 
     double RAe =  359.87123273*M_PI/180.;
     double Dece =  89.88809752*M_PI/180.;
@@ -655,17 +651,17 @@
     // The Sun center is reference for these calculations.
 
     double xr, yr, zr, vxr, vyr, vzr, axr, ayr, azr;
 
     assist_all_ephem(ephem, assist->ephem_cache, ASSIST_BODY_SUN, t, &GM, &xr, &yr, &zr, &vxr, &vyr, &vzr, &axr, &ayr, &azr);
     const double GMsun = GM;    
 
-    const double au = JPL_EPHEM_CAU;
-    const double Rs_eq = JPL_EPHEM_ASUN/au;
-    const double J2s = JPL_EPHEM_J2SUN;
+    const double au = ephem->jpl->AU;
+    const double Rs_eq = ephem->jpl->ASUN/au;
+    const double J2s = ephem->jpl->J2SUN;
 
     // Hard-coded constants.  BEWARE!
     double RAs = 286.13*M_PI/180.;
     double Decs = 63.87*M_PI/180.;
 
     double cosa = cos(RAs);
     double sina = sin(RAs);
@@ -1069,16 +1065,16 @@
     
     struct assist_extras* assist = (struct assist_extras*) sim->extras;
     struct assist_ephem* ephem = assist->ephem;
     const double jd_ref = ephem->jd_ref;
     
     // Nobili and Roxburgh GR treatment
 
-    const double au = JPL_EPHEM_CAU;    
-    const double c = (JPL_EPHEM_CLIGHT/au)*86400;
+    const double au = ephem->jpl->AU;    
+    const double c = (ephem->jpl->CLIGHT/au)*86400;
     const double C2 = c*c;  
     
     const unsigned int N = sim->N;  // N includes real+variational particles
     const unsigned int N_real = N - sim->N_var;
 
     const double t = sim->t;    
 
@@ -1176,16 +1172,16 @@
     
     struct assist_extras* assist = (struct assist_extras*) sim->extras;
     struct assist_ephem* ephem = assist->ephem;
     const double jd_ref = ephem->jd_ref;
     
     // Damour and Deruelle solar GR treatment
 
-    const double au = JPL_EPHEM_CAU;    
-    const double c = (JPL_EPHEM_CLIGHT/au)*86400;
+    const double au = ephem->jpl->AU;    
+    const double c = (ephem->jpl->CLIGHT/au)*86400;
 
     const double C2 = c*c; 
     
     const unsigned int N = sim->N;  // N includes real+variational particles
     const unsigned int N_real = N - sim->N_var;
 
     const double t = sim->t;    
@@ -1310,16 +1306,16 @@
     const double jd_ref = ephem->jd_ref;
     const int gr_eih_sources = assist->gr_eih_sources;
 
     // Einstein-Infeld-Hoffman PPN GR treatment
     // This is one of three options for GR.
     // This version is only rarely needed.
 
-    const double au = JPL_EPHEM_CAU;    
-    const double c = (JPL_EPHEM_CLIGHT/au)*86400;
+    const double au = ephem->jpl->AU;    
+    const double c = (ephem->jpl->CLIGHT/au)*86400;
     const double C2 = c*c;
     const double over_C2 = 1./(c*c);
 
     const unsigned int N = sim->N;  // N includes real+variational particles
     const unsigned int N_real = N - sim->N_var;
 
     const double t = sim->t;    
@@ -2009,16 +2005,16 @@
     struct assist_ephem* ephem = assist->ephem;
     const double jd_ref = ephem->jd_ref;
 
     // Einstein-Infeld-Hoffman PPN GR treatment
     // This is one of three options for GR.
     // This version is only rarely needed.
 
-    const double au = JPL_EPHEM_CAU;    
-    const double c = (JPL_EPHEM_CLIGHT/au)*86400;
+    const double au = ephem->jpl->AU;    
+    const double c = (ephem->jpl->CLIGHT/au)*86400;
     const double C2 = c*c;  // This could be stored as C2.
     const double over_C2 = 1./(c*c);    
 
     const unsigned int N = sim->N;  // N includes real+variational particles
     const unsigned int N_real = N - sim->N_var;
 
     const double t = sim->t;
```

### Comparing `assist-1.1.1/src/forces.h` & `assist-1.1.2/src/forces.h`

 * *Files identical despite different names*

### Comparing `assist-1.1.1/src/planets.c` & `assist-1.1.2/src/planets.c`

 * *Files 19% similar despite different names*

```diff
@@ -7,21 +7,16 @@
 
 #include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
 
 #include "spk.h"
 #include "planets.h"
-#include "const.h"
 #include "assist.h"
 
-#ifndef JPL_EPHEM_FILE
-#define JPL_EPHEM_FILE "../../data/linux_m13000p17000.441"
-#endif
-
 /*
  *  assist_jpl_work
  *
  *  Interpolate the appropriate Chebyshev polynomial coefficients.
  *
  *      ncf - number of coefficients per component
  *      ncm - number of components (ie: 3 for most)
@@ -72,164 +67,185 @@
 /*
  *  assist_jpl_init
  *
  *  Initialise everything needed ... probaly not be compatible with a non-430 file.
  *
  */
 
-struct jpl_s * assist_jpl_init(char *str)
-{
-        struct jpl_s *jpl;
-	struct stat sb;
-	//char *str;
-	ssize_t ret;
-	off_t off;
-        int fd, p;
-
-        /** use or environment-specified file, 
-	 * or the default filename, in that order
-         */
-	//if ((str = getenv("JPL_PLANET_EPHEM")) == NULL)
-	//str = JPL_EPHEM_FILE;
-
-        if ((fd = open(str, O_RDONLY)) < 0)
-                return NULL;
-
-        jpl = malloc(sizeof(struct jpl_s));
-        memset(jpl, 0, sizeof(struct jpl_s));
-
-        if (fstat(fd, &sb) < 0)
-                goto err;
-
-	// FIXME : probably should ensure the file is sized corrrectly
-	// FIXME : also could read 3*84 bytes to see if this is a JPL file
-
-	// skip the header and constant names for now
-        if (lseek(fd, 0x0A5C, SEEK_SET) < 0)
-                goto err;
-
-        // read header
-        ret  = read(fd, &jpl->beg, sizeof(double));
-        ret += read(fd, &jpl->end, sizeof(double));
-        ret += read(fd, &jpl->inc, sizeof(double));
-        ret += read(fd, &jpl->num, sizeof(int32_t));
-        ret += read(fd, &jpl->cau, sizeof(double));
-        ret += read(fd, &jpl->cem, sizeof(double));
-
-	//printf("%lf %lf %lf %d\n", jpl->beg, jpl->end, jpl->inc, jpl->num);
-
-        // number of coefficients for all components
-        for (p = 0; p < JPL_N; p++)
-                jpl->ncm[p] = 3;
-
-        // exceptions:
-        jpl->ncm[JPL_NUT] = 2; // nutations
-        jpl->ncm[JPL_TDB] = 1; // TT-TDB
-
-        for (p = 0; p < 12; p++) {
-                ret += read(fd, &jpl->off[p], sizeof(int32_t));
-                ret += read(fd, &jpl->ncf[p], sizeof(int32_t));
-                ret += read(fd, &jpl->niv[p], sizeof(int32_t));
-        }
-
-        ret += read(fd, &jpl->ver,     sizeof(int32_t));
-        ret += read(fd, &jpl->off[12], sizeof(int32_t));
-        ret += read(fd, &jpl->ncf[12], sizeof(int32_t));
-        ret += read(fd, &jpl->niv[12], sizeof(int32_t));
-
-	// get all the constant names, from two lcoations
-	jpl->str = calloc(jpl->num, sizeof(char *));
-	off = lseek(fd, 0, SEEK_CUR);
-	lseek(fd, 0x00FC, SEEK_SET);
-
-	// retrieve the names of the first 400 constants
-	for (p = 0; p < 400; p++) {
-		jpl->str[p] = calloc(1, 8);
-		read(fd, jpl->str[p], 6);
-	}
-
-	lseek(fd, off, SEEK_SET);
-
-	// read the remaining constant names
-	for (p = 400; p < jpl->num; p++) {
-		jpl->str[p] = calloc(1, 8);
-		read(fd, jpl->str[p], 6);
-	}
-
-        // finishing reading
-        for (p = 13; p < 15; p++) {
-                ret += read(fd, &jpl->off[p], sizeof(int32_t));
-                ret += read(fd, &jpl->ncf[p], sizeof(int32_t));
-                ret += read(fd, &jpl->niv[p], sizeof(int32_t));
+static double getConstant(struct jpl_s* jpl, char* name){
+    for (int p = 0; p < jpl->num; p++) {
+        if (strncmp(name,jpl->str[p],6)==0){
+            return jpl->con[p];
         }
+    }
+    fprintf(stderr,"WARNING: Constant [%s] not found in ephemeris file.\n",name); 
+    return 0;
+}
 
-        // adjust for correct indexing (ie: zero based)
-        for (p = 0; p < JPL_N; p++)
-                jpl->off[p] -= 1;
-
-        // save file size, and determine 'kernel size'
-        jpl->len = sb.st_size;
-        jpl->rec = sizeof(double) * 2;
-
-        for (p = 0; p < JPL_N; p++)
-                jpl->rec += sizeof(double) * jpl->ncf[p] * jpl->niv[p] * jpl->ncm[p];
+struct jpl_s * assist_jpl_init(char *str)
+{
+    struct stat sb;
+    ssize_t ret;
+    int fd;
 
-        // memory map the file, which makes us thread-safe with kernel caching
-        jpl->map = mmap(NULL, jpl->len, PROT_READ, MAP_SHARED, fd, 0);
+    if ((fd = open(str, O_RDONLY)) < 0){
+        return NULL;
+    }
 
-        if (jpl->map == NULL)
-                goto err;
+    if (fstat(fd, &sb) < 0){
+        close(fd);
+        fprintf(stderr, "Error while trying to determine filesize.\n");
+        return NULL;
+    }
+    
 
-	// now read the constant values after seeking to where they are
-	if (lseek(fd, jpl->rec, SEEK_SET) < 0)
-		goto err;
+    // skip the header and constant names for now
+    if (lseek(fd, 0x0A5C, SEEK_SET) < 0){
+        close(fd);
+        fprintf(stderr, "Error while seeking to header.\n");
+        return NULL;
+    }
 
-	jpl->con = calloc(jpl->num, sizeof(double));
+    struct jpl_s* jpl = calloc(1, sizeof(struct jpl_s));
 
-	for (p = 0; p < jpl->num; p++)
-		read(fd, &jpl->con[p], sizeof(double));
+    // read header
+    ret  = read(fd, &jpl->beg, sizeof(double));     // Start JD
+    ret += read(fd, &jpl->end, sizeof(double));     // End JD
+    ret += read(fd, &jpl->inc, sizeof(double));     // Days per block
+    ret += read(fd, &jpl->num, sizeof(int32_t));    // Number of constants
+    ret += read(fd, &jpl->cau, sizeof(double));     // AU to km 
+    ret += read(fd, &jpl->cem, sizeof(double));     // Ratio between Earth/Moon
+
+    // number of coefficients for all components
+    for (int p = 0; p < JPL_N; p++){
+        jpl->ncm[p] = 3;
+    }
+    // exceptions:
+    jpl->ncm[JPL_NUT] = 2; // nutations
+    jpl->ncm[JPL_TDB] = 1; // TT-TDB
+
+    for (int p = 0; p < 12; p++) {                      // Columns 1-12 of Group 1050
+        ret += read(fd, &jpl->off[p], sizeof(int32_t));
+        ret += read(fd, &jpl->ncf[p], sizeof(int32_t));
+        ret += read(fd, &jpl->niv[p], sizeof(int32_t));
+    }
+
+    ret += read(fd, &jpl->ver,     sizeof(int32_t));    // Version. e.g. 440
+    ret += read(fd, &jpl->off[12], sizeof(int32_t));    // Columns 13 of Group 1050
+    ret += read(fd, &jpl->ncf[12], sizeof(int32_t));
+    ret += read(fd, &jpl->niv[12], sizeof(int32_t));
+
+    // Get all the constant names
+    jpl->str = calloc(jpl->num, sizeof(char *));
+
+    // retrieve the names of the first 400 constants
+    lseek(fd, 0x00FC, SEEK_SET);    
+    for (int p = 0; p < 400; p++) {     // Group 1040
+        jpl->str[p] = calloc(8, sizeof(char));
+        read(fd, jpl->str[p], 6);
+    }
+
+    // read the remaining constant names
+    lseek(fd, 0x0B28, SEEK_SET);
+    for (int p = 400; p < jpl->num; p++) {
+        jpl->str[p] = calloc(8, sizeof(char));
+        read(fd, jpl->str[p], 6);
+    }
+
+    for (int p = 13; p < 15; p++) {                     // Columns 14 and 15 of Group 1050
+        ret += read(fd, &jpl->off[p], sizeof(int32_t));
+        ret += read(fd, &jpl->ncf[p], sizeof(int32_t));
+        ret += read(fd, &jpl->niv[p], sizeof(int32_t));
+    }
+
+    // adjust for correct indexing (ie: zero based)
+    for (int p = 0; p < JPL_N; p++){
+        jpl->off[p] -= 1;
+    }
+
+    // save file size, and determine 'kernel size' or 'block size' (=8144 bytes for DE440/441)
+    jpl->len = sb.st_size;
+    jpl->rec = sizeof(double) * 2;
+
+    for (int p = 0; p < JPL_N; p++){
+        jpl->rec += sizeof(double) * jpl->ncf[p] * jpl->niv[p] * jpl->ncm[p];
+    }
+
+    // memory map the file, which makes us thread-safe with kernel caching
+    jpl->map = mmap(NULL, jpl->len, PROT_READ, MAP_SHARED, fd, 0);
+
+    if (jpl->map == NULL){ 
+        close(fd);
+        free(jpl); // note constants leak
+        fprintf(stderr, "Error while calling mmap().\n");
+        return NULL;
+    }
 
-        // this file descriptor is no longer needed since we are memory mapped
-        if (close(fd) < 0)
-                { ; } // perror ...
+    // Read constants
+    jpl->con = calloc(jpl->num, sizeof(double));
+    lseek(fd, jpl->rec, SEEK_SET); // Starts at offset of 1 block size
+    for (int p = 0; p < jpl->num; p++){
+        read(fd, &jpl->con[p], sizeof(double));
+        //printf("%6d  %s   %.5e\n",p,jpl->str[p],jpl->con[p]);
+    }
+
+
+    // Find masses
+    jpl->mass[0] = getConstant(jpl, "GMS   ");  // Sun 
+    jpl->mass[1] = getConstant(jpl, "GM1   ");  // Mercury
+    jpl->mass[2] = getConstant(jpl, "GM2   ");
+	double emrat = getConstant(jpl, "EMRAT  "); // Earth Moon Ratio
+    double gmb = getConstant(jpl, "GMB   ");    // Earth Moon combined
+    jpl->mass[3] = (emrat/(1.+emrat)) * gmb;    // Earth 
+    jpl->mass[4] = 1./(1+emrat) * gmb;          // Moon 
+    jpl->mass[5] = getConstant(jpl, "GM4   ");  // Mars
+    jpl->mass[6] = getConstant(jpl, "GM5   ");  // Jupiter
+    jpl->mass[7] = getConstant(jpl, "GM6   ");
+    jpl->mass[8] = getConstant(jpl, "GM7   ");
+    jpl->mass[9] = getConstant(jpl, "GM8   ");
+    jpl->mass[10] = getConstant(jpl, "GM9   "); // Pluto
+
+
+    // Other constants
+    jpl->J2E = getConstant(jpl, "J2E   ");
+    jpl->J3E = getConstant(jpl, "J3E   ");
+    jpl->J4E = getConstant(jpl, "J4E   ");
+    jpl->J2SUN = getConstant(jpl, "J2SUN ");
+    jpl->AU = getConstant(jpl, "AU    ");
+    jpl->RE = getConstant(jpl, "RE    ");
+    jpl->CLIGHT = getConstant(jpl, "CLIGHT");
+    jpl->ASUN = getConstant(jpl, "ASUN  ");
+
+    // this file descriptor is no longer needed since we are memory mapped
+    if (close(fd) < 0) { 
+        fprintf(stderr, "Error while closing file.\n");
+    }
 #if defined(MADV_RANDOM)
-        if (madvise(jpl->map, jpl->len, MADV_RANDOM) < 0)
-                { ; } // perror ...
+    if (madvise(jpl->map, jpl->len, MADV_RANDOM) < 0){
+        fprintf(stderr, "Error during madvise.\n");
+    }
 #endif
 
-        return jpl;
-
-err:    close(fd);
-        free(jpl);
+    return jpl;
 
-        return NULL;
 }
 
-/*
- *  assist_jpl_free
- *
- */
-int assist_jpl_free(struct jpl_s *jpl)
-{
-	int p;
-
-        if (jpl == NULL)
-                return -1;
-
-        if (munmap(jpl->map, jpl->len) < 0)
-                { ; } // perror...
-
-	for (p = 0; p < jpl->num; p++)
-		free(jpl->str[p]);
-
-	free(jpl->str);
-	free(jpl->con);
-        memset(jpl, 0, sizeof(struct jpl_s));
-        free(jpl);
-        return 0;
+void assist_jpl_free(struct jpl_s *jpl) {
+    if (jpl == NULL){
+        return;
+    }
+    if (munmap(jpl->map, jpl->len) < 0){ 
+        fprintf(stderr, "Error during munmap().\n");
+    }
+    for (int p = 0; p < jpl->num; p++){
+        free(jpl->str[p]);
+    }
+    free(jpl->str);
+    free(jpl->con);
+    free(jpl);
 }
 
 /*
  *  jpl_calc
  *
  *  Caculate the position+velocity in _equatorial_ coordinates.
  *  Assumes pos is initially zero.
@@ -245,36 +261,16 @@
     if (jpl == NULL || jpl->map == NULL)
         return ASSIST_ERROR_EPHEM_FILE;
     if(body<0 || body >= ASSIST_BODY_NPLANETS)
 	    return(ASSIST_ERROR_NEPHEM);
     
     struct mpos_s pos;
 
-    // The values below are G*mass.
-    // Units are solar masses, au, days.
-    // DE440/441 units: au^3 day^-2.
-    const static double JPL_GM[ASSIST_BODY_NPLANETS] =
-	{
-	    JPL_EPHEM_GMS, // 0 sun
-	    JPL_EPHEM_GM1, // 1 mercury
-	    JPL_EPHEM_GM2, // 2 venus
-	    (JPL_EPHEM_EMRAT/(1.+JPL_EPHEM_EMRAT) * JPL_EPHEM_GMB),  // 3 earth    Calculate GM values for Earth and Moon
-	    (1./(1.+JPL_EPHEM_EMRAT) * JPL_EPHEM_GMB),               // 4 moon     from Earth-moon ratio and sum.
-	    JPL_EPHEM_GM4, // 5 mars
-	    JPL_EPHEM_GM5, // 6 jupiter
-	    JPL_EPHEM_GM6, // 7 saturn
-	    JPL_EPHEM_GM7, // 8 uranus
-	    JPL_EPHEM_GM8, // 9 neptune
-	    JPL_EPHEM_GM9, // 10 pluto
-	};
-
-
-    // Get position, velocity, and mass of body i in barycentric coords.
-
-    *GM = JPL_GM[body];
+    // Get mass, position, velocity, and mass of body i in barycentric coords.
+    *GM = jpl->mass[body];
 
         // check if covered by this file
         if (jd_ref + jd_rel < jpl->beg || jd_ref + jd_rel > jpl->end)
             return ASSIST_ERROR_COVERAGE;
 
         // compute record number and 'offset' into record
         blk = (u_int32_t)((jd_ref + jd_rel - jpl->beg) / jpl->inc);
@@ -361,33 +357,7 @@
     *out_ay = pos.w[1];
     *out_az = pos.w[2];
 
     return(ASSIST_SUCCESS);
 
 }
 
-/*
- *  assist_jpl_mass
- *
- */
-double assist_jpl_mass(struct jpl_s *jpl, int tar)
-{
-	char buf[14];
-	int n;
-
-	if (jpl == NULL)
-		return 0.0;
-
-	if (tar >= 10000)
-		return 0.0;
-
-	snprintf(buf, sizeof(buf), "MA%04d", tar);
-
-	for (n = 0; n < jpl->num; n++) {
-		if (strncmp(jpl->str[n], buf, 6) == 0)
-			return jpl->con[n];
-	}
-
-	// not found
-	return 0.0;
-}
-
```

### Comparing `assist-1.1.1/src/planets.h` & `assist-1.1.2/src/planets.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #ifndef _JPL_EPHEM_H
 #define _JPL_EPHEM_H
 #include "assist.h"
 
 struct jpl_s * assist_jpl_init(char *str);
-int assist_jpl_free(struct jpl_s *jpl);
+void assist_jpl_free(struct jpl_s *jpl);
 void assist_jpl_work(double *P, int ncm, int ncf, int niv, double t0, double t1, double *u, double *v, double *w);
 enum ASSIST_STATUS assist_jpl_calc(struct jpl_s *pl, double jd_ref, double jd_rel, int body, 
 		 double* const GM,
 		 double* const x, double* const y, double* const z,
 		 double* const vx, double* const vy, double* const vz,
          double* const ax, double* const ay, double* const az);
-double assist_jpl_mass(struct jpl_s *pl, int tar);
 
 // Order of columns in JPL Ephemeris file
 enum {
          JPL_MER,                        // Mercury
          JPL_VEN,                        // Venus
          JPL_EMB,                        // Earth
          JPL_MAR,                        // Mars
@@ -36,23 +35,31 @@
 struct jpl_s {
         double beg, end;                // begin and end times
         double inc;                     // time step size
         double cau;                     // definition of AU
         double cem;                     // Earth/Moon mass ratio
         int32_t num;                    // number of constants
         int32_t ver;                    // ephemeris version
-        int32_t off[JPL_N];                // indexing offset
-        int32_t ncf[JPL_N];                // number of chebyshev coefficients
-        int32_t niv[JPL_N];                // number of interpolation intervals
-        int32_t ncm[JPL_N];                // number of components / dimension
-///
+        int32_t off[JPL_N];             // indexing offset
+        int32_t ncf[JPL_N];             // number of chebyshev coefficients
+        int32_t niv[JPL_N];             // number of interpolation intervals
+        int32_t ncm[JPL_N];             // number of components / dimension
+        double mass[JPL_N];             // G*mass for all bodies
+        double J2E;                     // Other constant names follow JPL 
+        double J3E;
+        double J4E;
+        double J2SUN;
+        double AU;
+        double RE;
+        double CLIGHT;
+        double ASUN;
         size_t len, rec;                // file and record sizes
         void *map;                      // memory mapped location
-	double *con;			// constant values
-	char **str;			// constant names
+	    double *con;			        // constant values
+	    char **str;			            // constant names
 };
 
 // From Weryk's code
 /////// private interface :
 
 static inline void vecpos_off(double *u, const double *v, const double w)
         { u[0] += v[0] * w; u[1] += v[1] * w; u[2] += v[2] * w; }
```

### Comparing `assist-1.1.1/src/spk.c` & `assist-1.1.2/src/spk.c`

 * *Files 20% similar despite different names*

```diff
@@ -14,44 +14,35 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <unistd.h>
 #include <time.h>
 #include "assist.h"
 #include "spk.h"
-#include "const.h"
 
 
-struct sum_s {
-	double beg;		// begin epoch, seconds since J2000.0
-	double end;		// ending epoch
-	int tar;		// target code
-	int cen;		// centre code (10 = sun)
-	int ref;		// reference frame (1 = J2000.0)
-	int ver;		// type of ephemeris (2 = chebyshev)
-	int one;		// initial array address
-	int two;		// final array address
-};
 
 
 /*
  *  spk_free
  *
  */
 int assist_spk_free(struct spk_s *pl)
 {
-	int m;
 
 	if (pl == NULL)
 		return -1;
 
-	for (m = 0; m < pl->num; m++) {
-		free(pl->one[m]);
-		free(pl->two[m]);
-	}
+    if (pl->targets){
+        for (int m = 0; m < pl->num; m++) {
+            free(pl->targets[m].one);
+            free(pl->targets[m].two);
+        }
+        free(pl->targets);
+    }
 
 	munmap(pl->map, pl->len);
 	memset(pl, 0, sizeof(struct spk_s));
 	free(pl);
 	return 0;
 }
 
@@ -61,243 +52,200 @@
  *
  */
 
 // convert SPK epoch (since J2000.0) to julian day number
 static double inline _jul(double eph)
 	{ return 2451545.0 + eph / 86400.0; }
 
+
+#define record_length 1024
 // check for any non-7bit ascii characters
-static int _com(const char *buf)
-{
-	for (int n = 0; n < 1024; n++)
-		{ if (buf[n] < 0) return 0; }
+static int _com(const char *record) {
+	for (int n = 0; n < record_length; n++)
+		{ if (record[n] < 0) return 0; }
 
 	return 1;
 }
 
-// display output strings to console
-//static void _sho(const char *buf)
-//{
-//	int n;
-//
-//	// this doesn't always handle the newlines correctly
-//	for (n = 0; buf[n+1] != '\0';)
-//		n += fprintf(stdout, "%s\n", &buf[n]) - 1;
-//}
+struct spk_s * assist_spk_init(const char *path) {
+    // For file format information, see https://naif.jpl.nasa.gov/pub/naif/toolkit_docs/FORTRAN/req/daf.html
 
-struct spk_s * assist_spk_init(const char *path)
-{
-	struct spk_s *pl;
-	struct stat sb;
-	char buf[1024];
-	struct sum_s *sum;
-	double *val;
-	int fd, nd, ni, nc;
-	int m, n, c, b, B;
-	off_t off;
+    // Format for one summary
+    struct sum_s {
+        double beg;		// begin epoch, seconds since J2000.0
+        double end;		// ending epoch
+        int tar;		// target code
+        int cen;		// centre code (10 = sun)
+        int ref;		// reference frame (1 = J2000.0)
+        int ver;		// type of ephemeris (2 = chebyshev)
+        int one;		// initial array address
+        int two;		// final array address
+    };
 
-	if ((fd = open(path, O_RDONLY)) < 0)
+    // File is split into records. We read one record at a time.
+    union {
+	    char buf[record_length];
+        struct {
+            double next;    // The record number of the next summary record in the file. Zero if this is the final summary record.
+            double prev;    // The record number of the previous summary record in the file. Zero if this is the initial summary record.
+            double nsum;    // Number of summaries in this record
+            struct sum_s s[25]; // Summaries (25 is the maximum)
+        } summary;          // Summary record
+        struct {
+            char locidw[8]; // An identification word
+            int nd;         // The number of double precision components in each array summary.
+            int ni;         // The number of integer components in each array summary.
+        } file;             // File record
+    } record;
+
+    // Try opening file.
+	int fd = open(path, O_RDONLY);
+	if (fd < 0){
 		return NULL;
+    }
 
-	pl = malloc(sizeof(struct spk_s));
-	memset(pl, 0, sizeof(struct spk_s));
-	val = (double *)buf;
-	sum = (struct sum_s *)buf;
-
-	if (fstat(fd, &sb) < 0)
-		goto err;
-
-	// LOCIDW
-	if (read(fd, buf, 8) != 8)
-		goto err;
-
-	if (strncmp(buf, "DAF/SPK", 7) != 0) {
-		errno = EILSEQ;
-		goto err;
+	// Read the file record. 
+    read(fd, &record, 1024);
+    // Check if the file is a valid Double Precision Array File
+	if (strncmp(record.file.locidw, "DAF/SPK", 7) != 0) {
+        fprintf(stderr,"Error parsing DAF/SPK file. Incorrect header.\n");
+		close(fd);
+		return NULL;
 	}
 
-	// ND, NI
-	read(fd, &nd, sizeof(int));
-	read(fd, &ni, sizeof(int));
-
-	// length of each segment, must match our sum_s struct
-	nc = 8 * ( nd + (ni + 1) / 2 );
-
+    // Check that the size of a summary record is equal to the size of our struct.
+	int nc = 8 * ( record.file.nd + (record.file.ni + 1) / 2 );
 	if (nc != sizeof(struct sum_s)) {
-		errno = EILSEQ;
-		goto err;
+        fprintf(stderr,"Error parsing DAF/SPK file. Wrong size of summary record.\n");
+		close(fd);
+		return NULL;
 	}
-
-	// could check the other headers, but we really don't care
-	// so find the first summary record (after potential comments)
-	off = lseek(fd, 1024, SEEK_SET);
-	read(fd, buf, 1024);
-
-	while (_com(buf) > 0) {
-	//	_sho(buf);
-		off = lseek(fd, 0, SEEK_CUR);
-		read(fd, buf, 1024);
-	}
-
-	// we are at the first summary block, validate
-	if (val[1] != 0.0) {
-		errno = EILSEQ;
-		goto err;
+    
+    // Continue reading file until we find a non-ascii record.
+    do {
+		read(fd, record.buf, 1024);
+    } while (_com(record.buf) > 0);
+
+	// We are at the first summary block, validate
+	if ((int64_t)record.buf[8] != 0) {
+        fprintf(stderr, "Error parsing DAF/SPL file. Cannot find summary block.\n");
+		close(fd);
+        return NULL; 
 	}
 
 	// okay, let's go
-	m = 0;
-next:	n = (int)val[0] - 1;
-	B = (int)val[2];
-
-	for (b = 0; b < B; b++) {
-		sum = (struct sum_s *)&buf[24 + b * sizeof(struct sum_s)];
-
-//		fprintf(stdout, "beg %.1f end %.1f tar %d cen %d ref %d ver %d one %d two %d\n",
-//				_jul(sum->beg), _jul(sum->end), sum->tar, sum->cen,
-//				sum->ref, sum->ver, sum->one, sum->two);
-
-		// pick out new target!
-		if (sum->tar != pl->tar[m]) {
-			m = pl->num++;
-			pl->tar[m] = sum->tar;
-			pl->cen[m] = sum->cen;
-			pl->beg[m] = _jul(sum->beg);
-			pl->res[m] = _jul(sum->end) - pl->beg[m];
-			pl->one[m] = calloc(32768, sizeof(int));
-			pl->two[m] = calloc(32768, sizeof(int));
-		}
-
-		// add index
-		c = pl->ind[m]++;
-		pl->one[m][c] = sum->one;
-		pl->two[m][c] = sum->two;
-		pl->end[m] = _jul(sum->end);
-	}
-
-	if (n >= 0) {
-		// this could probably be more elegant if the mmap happened sooner
-		off = lseek(fd, n * 1024, SEEK_SET);
-		read(fd, buf, 1024);
-		goto next;
-	}
+	struct spk_s* pl = calloc(1, sizeof(struct spk_s));
+    while (1){ // Loop over records 
+        for (int b = 0; b < (int)record.summary.nsum; b++) { // Loop over summaries
+            struct sum_s* sum = &record.summary.s[b]; // get current summary
+            
+            // Index in our arrays for current target
+            int m = pl->num - 1;
+
+            // New target?
+            if (pl->num==0 || sum->tar != pl->targets[m].code) {
+                if (pl->num <= pl->allocated_num){
+                    pl->allocated_num += 32; // increase space in batches of 32
+                    pl->targets = realloc(pl->targets, pl->allocated_num*sizeof(struct spk_target));
+                }
+                m++;
+                pl->targets[m].code = sum->tar;
+                pl->targets[m].cen = sum->cen;
+                pl->targets[m].beg = _jul(sum->beg);
+                pl->targets[m].res = _jul(sum->end) - pl->targets[m].beg;
+                pl->targets[m].one = calloc(32768, sizeof(int));
+                pl->targets[m].two = calloc(32768, sizeof(int));
+                pl->targets[m].ind = 0;
+                pl->num++;
+            }
+
+            // add index for target
+            pl->targets[m].one[pl->targets[m].ind] = sum->one;
+            pl->targets[m].two[pl->targets[m].ind] = sum->two;
+            pl->targets[m].end = _jul(sum->end);
+            pl->targets[m].ind++;
+        }
+
+        // Location of next record
+        long n = (long)record.summary.next - 1;
+        if (n<0){
+            // this is already the last record.
+            break;
+        }else{
+            // Find and read next record
+            lseek(fd, n * 1024, SEEK_SET);
+            read(fd, record.buf, 1024);
+        }
+    }
 
-	// memory map : kernel caching and thread safe
+    // Get file size
+	struct stat sb;
+	if (fstat(fd, &sb) < 0){
+        fprintf(stderr, "Error calculating size for DAF/SPL file.\n");
+        return NULL; 
+    }
 	pl->len = sb.st_size;
-	pl->map = mmap(NULL, pl->len, PROT_READ, MAP_SHARED, fd, 0);
 
-	if (pl->map == NULL)
-		goto err;
+    // Memory map
+	pl->map = mmap(NULL, pl->len, PROT_READ, MAP_SHARED, fd, 0);
+	if (pl->map == NULL){
+        fprintf(stderr, "Error creating memory map.\n");
+        return NULL; // Will leak memory
+    }
 
-	if (close(fd) < 0)
-		{ ; }
 #if defined(MADV_RANDOM)
-	if (madvise(pl->map, pl->len, MADV_RANDOM) < 0)
-		{ ; }
+	if (madvise(pl->map, pl->len, MADV_RANDOM) < 0){
+        fprintf(stderr, "Error while calling madvise().\n");
+        return NULL; // Will leak memory
+    }
 #endif
 
+	close(fd);
 	return pl;
-
-err:	perror(path);
-	free(pl);
-
-	return NULL;
-}
-
-
-/*
- *  assist_spk_find
- *
- *  See if we have the given body.
- *
- */
-int assist_spk_find(struct spk_s *pl, int tar)
-{
-	int n;
-
-	if (pl == NULL)
-		return -1;
-
-	for (n = 0; n < pl->num; n++)
-		if (pl->tar[n] == tar)
-			{ return n; }
-
-	return -1;
 }
 
 
-/*
- *  assist_spk_calc
- *
- *  Compute the position and velocity after fetching the chebyshev polynomials.
- *
- */
-
 enum ASSIST_STATUS assist_spk_calc(struct spk_s *pl, double jde, double rel, int m, double* GM, double* out_x, double* out_y, double* out_z)
 {
-    const static double JPL_GM[16] =    
-    {
-	JPL_EPHEM_MA0107, // 107 camilla
-	JPL_EPHEM_MA0001, // 1 Ceres
-	JPL_EPHEM_MA0065, // 65 cybele
-	JPL_EPHEM_MA0511, // 511 davida
-	JPL_EPHEM_MA0015, // 15 eunomia
-	JPL_EPHEM_MA0031, // 31 euphrosyne	    
-	JPL_EPHEM_MA0052, // 52 europa
-	JPL_EPHEM_MA0010, // 10 hygiea
-	JPL_EPHEM_MA0704, // 704 interamnia
-	JPL_EPHEM_MA0007, // 7 iris
-	JPL_EPHEM_MA0003, // 3 juno
-	JPL_EPHEM_MA0002, // 2 pallas
-	JPL_EPHEM_MA0016, // 16 psyche
-	JPL_EPHEM_MA0087, // 87 sylvia
-	JPL_EPHEM_MA0088, // 88 thisbe
-	JPL_EPHEM_MA0004  // 4 vesta
-    };
-
     if(pl==NULL){
         return(ASSIST_ERROR_AST_FILE);	
     }
 
     if(m<0 || m > pl->num){
         return(ASSIST_ERROR_NAST);
     }
+    struct spk_target* target = &(pl->targets[m]);
         
-    if (jde + rel < pl->beg[m] || jde + rel > pl->end[m]){
+    if (jde + rel < target->beg || jde + rel > target->end){
         return ASSIST_ERROR_COVERAGE;
     }
 
-    // TODO: again, the units might be handled more
-    // generally
-
-    *GM = JPL_GM[m];
+    *GM = target->mass; // Note mass constants defined in DE440/441 ephemeris files. If not found mass of 0 is used.
 
 	int n, b, p, P, R;
 	double T[32];
     // double S[32]; // Not used at the moment
 	double *val, z;
     struct mpos_s pos = {0};
 
 	for (n = 0; n < 3; n++)
 		pos.u[n] = pos.v[n] = 0.0;
 
 	// find location of 'directory' describing the data records
-	n = (int)((jde + rel - pl->beg[m]) / pl->res[m]);
-	//val = (double*)pl->map + sizeof(double) * (pl->two[m][n] - 1);
-	val = (double *)pl->map + pl->two[m][n] - 1;	
+	n = (int)((jde + rel - target->beg) / target->res);
+	val = (double *)pl->map + target->two[n] - 1;	
 
 	// record size and number of coefficients per coordinate
 	R = (int)val[-1];
 	P = (R - 2) / 3; // must be < 32 !!
 
 	// pick out the precise record
 	b = (int)(((jde - _jul(val[-3])) + rel) / (val[-2] / 86400.0));
-	//val = (double*)pl->map + sizeof(double) * (pl->one[m][n] - 1)
 	//+ sizeof(double) * b * R;
-	val = (double *)pl->map + (pl->one[m][n] - 1) + b * R;
+	val = (double *)pl->map + (target->one[n] - 1) + b * R;
 
 	// scale to interpolation units
 	z = ((jde - _jul(val[0])) + rel) / (val[1] / 86400.0);
 
 	// set up Chebyshev polynomials
 	T[0] = 1.0; T[1] = z;   
     // Not used at the moment:
```

