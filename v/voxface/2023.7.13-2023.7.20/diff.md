# Comparing `tmp/voxface-2023.7.13.tar.gz` & `tmp/voxface-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxface-2023.7.13.tar", last modified: Wed Jul 19 22:58:53 2023, max compression
+gzip compressed data, was "voxface-2023.7.20.tar", last modified: Thu Jul 20 20:44:04 2023, max compression
```

## Comparing `voxface-2023.7.13.tar` & `voxface-2023.7.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-19 22:58:53.304415 voxface-2023.7.13/
--rw-r--r--   0 jmt        (501) staff       (20)     1068 2021-07-19 23:23:08.000000 voxface-2023.7.13/LICENSE
--rw-r--r--   0 jmt        (501) staff       (20)     1622 2023-07-19 22:58:53.304119 voxface-2023.7.13/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      802 2023-07-13 16:50:14.000000 voxface-2023.7.13/README.md
--rw-r--r--   0 jmt        (501) staff       (20)       38 2023-07-19 22:58:53.304509 voxface-2023.7.13/setup.cfg
--rw-r--r--   0 jmt        (501) staff       (20)     8584 2023-07-19 22:54:28.000000 voxface-2023.7.13/setup.py
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-19 22:58:53.296901 voxface-2023.7.13/voxface/
--rw-r--r--   0 jmt        (501) staff       (20)        0 2021-07-19 23:23:08.000000 voxface-2023.7.13/voxface/__init__.py
--rwxr-xr-x   0 jmt        (501) staff       (20)     5784 2023-07-19 22:55:20.000000 voxface-2023.7.13/voxface/__main__.py
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-19 22:58:53.298640 voxface-2023.7.13/voxface/templates/
--rw-r--r--   0 jmt        (501) staff       (20)     8489 2021-07-19 23:23:08.000000 voxface-2023.7.13/voxface/templates/ConteCore2_50_2mm_deface_mask.nii.gz
--rw-r--r--   0 jmt        (501) staff       (20)  4435119 2021-07-19 23:23:08.000000 voxface-2023.7.13/voxface/templates/ConteCore2_50_T1w_2mm.nii.gz
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-19 22:58:53.298129 voxface-2023.7.13/voxface.egg-info/
--rw-r--r--   0 jmt        (501) staff       (20)     1622 2023-07-19 22:58:53.000000 voxface-2023.7.13/voxface.egg-info/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      326 2023-07-19 22:58:53.000000 voxface-2023.7.13/voxface.egg-info/SOURCES.txt
--rw-r--r--   0 jmt        (501) staff       (20)        1 2023-07-19 22:58:53.000000 voxface-2023.7.13/voxface.egg-info/dependency_links.txt
--rw-r--r--   0 jmt        (501) staff       (20)       50 2023-07-19 22:58:53.000000 voxface-2023.7.13/voxface.egg-info/entry_points.txt
--rw-r--r--   0 jmt        (501) staff       (20)        8 2023-07-19 22:58:53.000000 voxface-2023.7.13/voxface.egg-info/top_level.txt
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-20 20:44:04.061707 voxface-2023.7.20/
+-rw-r--r--   0 jmt        (501) staff       (20)     1068 2021-07-19 23:23:08.000000 voxface-2023.7.20/LICENSE
+-rw-r--r--   0 jmt        (501) staff       (20)     1622 2023-07-20 20:44:04.061446 voxface-2023.7.20/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      802 2023-07-20 19:37:47.000000 voxface-2023.7.20/README.md
+-rw-r--r--   0 jmt        (501) staff       (20)       38 2023-07-20 20:44:04.061780 voxface-2023.7.20/setup.cfg
+-rw-r--r--   0 jmt        (501) staff       (20)     8584 2023-07-20 19:36:13.000000 voxface-2023.7.20/setup.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-20 20:44:04.048496 voxface-2023.7.20/voxface/
+-rw-r--r--   0 jmt        (501) staff       (20)        0 2021-07-19 23:23:08.000000 voxface-2023.7.20/voxface/__init__.py
+-rwxr-xr-x   0 jmt        (501) staff       (20)     5784 2023-07-19 22:55:20.000000 voxface-2023.7.20/voxface/__main__.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-20 20:44:04.051204 voxface-2023.7.20/voxface/templates/
+-rw-r--r--   0 jmt        (501) staff       (20)     8489 2021-07-19 23:23:08.000000 voxface-2023.7.20/voxface/templates/ConteCore2_50_2mm_deface_mask.nii.gz
+-rw-r--r--   0 jmt        (501) staff       (20)  4435119 2021-07-19 23:23:08.000000 voxface-2023.7.20/voxface/templates/ConteCore2_50_T1w_2mm.nii.gz
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-07-20 20:44:04.050305 voxface-2023.7.20/voxface.egg-info/
+-rw-r--r--   0 jmt        (501) staff       (20)     1622 2023-07-20 20:44:03.000000 voxface-2023.7.20/voxface.egg-info/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      326 2023-07-20 20:44:03.000000 voxface-2023.7.20/voxface.egg-info/SOURCES.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        1 2023-07-20 20:44:03.000000 voxface-2023.7.20/voxface.egg-info/dependency_links.txt
+-rw-r--r--   0 jmt        (501) staff       (20)       50 2023-07-20 20:44:03.000000 voxface-2023.7.20/voxface.egg-info/entry_points.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        8 2023-07-20 20:44:03.000000 voxface-2023.7.20/voxface.egg-info/top_level.txt
```

### Comparing `voxface-2023.7.13/LICENSE` & `voxface-2023.7.20/LICENSE`

 * *Files identical despite different names*

### Comparing `voxface-2023.7.13/PKG-INFO` & `voxface-2023.7.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxface
-Version: 2023.7.13
+Version: 2023.7.20
 Summary: Fast MRI face voxelator
 Home-page: https://github.com/jmtyszka/voxface
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/voxface/issues
 Project-URL: Funding, http://conte.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/voxface/
@@ -23,15 +23,15 @@
 
 Fast voxelation of the face in 3D structural MRI data combining spline downsampling with nearest-neighbor upsampling to
 deidentify the face while retaining some signal intensity to guide whole-head registration.
 
 ## Installation
 
 ### Latest Version
-2021.7.20
+2023.7.20
 
 ### GitHub Installation
 
 1. Clone this branch to your local system
    ```
    % git clone https://github.com/jmtyszka/voxface.git
    ```
```

### Comparing `voxface-2023.7.13/README.md` & `voxface-2023.7.20/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Fast voxelation of the face in 3D structural MRI data combining spline downsampling with nearest-neighbor upsampling to
 deidentify the face while retaining some signal intensity to guide whole-head registration.
 
 ## Installation
 
 ### Latest Version
-2021.7.20
+2023.7.20
 
 ### GitHub Installation
 
 1. Clone this branch to your local system
    ```
    % git clone https://github.com/jmtyszka/voxface.git
    ```
```

### Comparing `voxface-2023.7.13/setup.py` & `voxface-2023.7.20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2023.7.13',  # Required
+    version='2023.7.20',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Fast MRI face voxelator',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `voxface-2023.7.13/voxface/__main__.py` & `voxface-2023.7.20/voxface/__main__.py`

 * *Files identical despite different names*

### Comparing `voxface-2023.7.13/voxface/templates/ConteCore2_50_2mm_deface_mask.nii.gz` & `voxface-2023.7.20/voxface/templates/ConteCore2_50_2mm_deface_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `voxface-2023.7.13/voxface/templates/ConteCore2_50_T1w_2mm.nii.gz` & `voxface-2023.7.20/voxface/templates/ConteCore2_50_T1w_2mm.nii.gz`

 * *Files identical despite different names*

### Comparing `voxface-2023.7.13/voxface.egg-info/PKG-INFO` & `voxface-2023.7.20/voxface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxface
-Version: 2023.7.13
+Version: 2023.7.20
 Summary: Fast MRI face voxelator
 Home-page: https://github.com/jmtyszka/voxface
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/voxface/issues
 Project-URL: Funding, http://conte.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/voxface/
@@ -23,15 +23,15 @@
 
 Fast voxelation of the face in 3D structural MRI data combining spline downsampling with nearest-neighbor upsampling to
 deidentify the face while retaining some signal intensity to guide whole-head registration.
 
 ## Installation
 
 ### Latest Version
-2021.7.20
+2023.7.20
 
 ### GitHub Installation
 
 1. Clone this branch to your local system
    ```
    % git clone https://github.com/jmtyszka/voxface.git
    ```
```

