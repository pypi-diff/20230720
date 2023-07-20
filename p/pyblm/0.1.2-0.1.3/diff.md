# Comparing `tmp/pyblm-0.1.2.tar.gz` & `tmp/pyblm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblm-0.1.2.tar", last modified: Thu Jul 20 17:59:40 2023, max compression
+gzip compressed data, was "pyblm-0.1.3.tar", last modified: Thu Jul 20 18:04:40 2023, max compression
```

## Comparing `pyblm-0.1.2.tar` & `pyblm-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.163139 pyblm-0.1.2/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:59:40.161011 pyblm-0.1.2/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10239 2023-07-20 17:58:15.000000 pyblm-0.1.2/README.md
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.103329 pyblm-0.1.2/blm/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/blm_cluster.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.132415 pyblm-0.1.2/blm/lib/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_batch.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_concat.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_results.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_setup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    24399 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/fileio.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.146939 pyblm-0.1.2/pyblm.egg-info/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/SOURCES.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/dependency_links.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/entry_points.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/requires.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/top_level.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 17:59:40.163414 pyblm-0.1.2/setup.cfg
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 17:59:26.000000 pyblm-0.1.2/setup.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.158242 pyblm-0.1.2/test/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:01.000000 pyblm-0.1.2/test/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/blm_cluster_test.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/cleanup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17906 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/generate_test_data.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 18:04:40.597402 pyblm-0.1.3/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 18:04:40.595033 pyblm-0.1.3/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10239 2023-07-20 17:58:15.000000 pyblm-0.1.3/README.md
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 18:04:40.507432 pyblm-0.1.3/blm/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/blm_cluster.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 18:04:40.537679 pyblm-0.1.3/blm/lib/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/lib/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/lib/blm_batch.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/lib/blm_concat.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/lib/blm_results.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 17:58:15.000000 pyblm-0.1.3/blm/lib/blm_setup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    24400 2023-07-20 18:03:28.000000 pyblm-0.1.3/blm/lib/fileio.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 18:04:40.579059 pyblm-0.1.3/pyblm.egg-info/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 18:04:40.544220 pyblm-0.1.3/pyblm.egg-info/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 18:04:40.549999 pyblm-0.1.3/pyblm.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 18:04:40.567048 pyblm-0.1.3/pyblm.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 18:04:40.569963 pyblm-0.1.3/pyblm.egg-info/entry_points.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 18:04:40.575400 pyblm-0.1.3/pyblm.egg-info/requires.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 18:04:40.579208 pyblm-0.1.3/pyblm.egg-info/top_level.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 18:04:40.597579 pyblm-0.1.3/setup.cfg
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 18:03:29.000000 pyblm-0.1.3/setup.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 18:04:40.591942 pyblm-0.1.3/test/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:01.000000 pyblm-0.1.3/test/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 17:58:15.000000 pyblm-0.1.3/test/blm_cluster_test.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 17:58:15.000000 pyblm-0.1.3/test/cleanup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17908 2023-07-20 18:03:29.000000 pyblm-0.1.3/test/generate_test_data.py
```

### Comparing `pyblm-0.1.2/PKG-INFO` & `pyblm-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyblm-0.1.2/README.md` & `pyblm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/blm_cluster.py` & `pyblm-0.1.3/blm/blm_cluster.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/lib/blm_batch.py` & `pyblm-0.1.3/blm/lib/blm_batch.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/lib/blm_concat.py` & `pyblm-0.1.3/blm/lib/blm_concat.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/lib/blm_results.py` & `pyblm-0.1.3/blm/lib/blm_results.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/lib/blm_setup.py` & `pyblm-0.1.3/blm/lib/blm_setup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/blm/lib/fileio.py` & `pyblm-0.1.3/blm/lib/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,15 +603,15 @@
   # random effects squared/the largest matrix size we would
   # look at).
   vPerBlock = MAXMEM/(10*8*(p**2))
 
   # Read in analysis mask (if present)
   if 'analysis_mask' in inputs:
     am = loadFile(inputs['analysis_mask'])
-    am = am.get_data()
+    am = am.get_fdata()
   else:
 
     # --------------------------------------------------------------
     # Get one Y volume to make full Nifti mask
     # --------------------------------------------------------------
 
     # Y volumes
```

### Comparing `pyblm-0.1.2/pyblm.egg-info/PKG-INFO` & `pyblm-0.1.3/pyblm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyblm-0.1.2/setup.py` & `pyblm-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pyblm",
-    version="0.1.2",
+    version="0.1.3",
     author="Tom Maullin",
     author_email="TomMaullin@gmail.com",
     description="The Big Linear Models Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tommaullin/blm",
     packages=find_packages(),
```

### Comparing `pyblm-0.1.2/test/blm_cluster_test.py` & `pyblm-0.1.3/test/blm_cluster_test.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/test/cleanup.py` & `pyblm-0.1.3/test/cleanup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.2/test/generate_test_data.py` & `pyblm-0.1.3/test/generate_test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     v_current = len(inds_cv)
 
     # Loop through each subject reading in Y and reducing to just the voxels 
     # needed
     for i in np.arange(n):
 
         # Load in the Y volume
-        Yi = nib.load(os.path.join(simDir,"data","Y"+str(i)+".nii")).get_data()
+        Yi = nib.load(os.path.join(simDir,"data","Y"+str(i)+".nii")).get_fdata()
 
         # Flatten Yi
         Yi = Yi.reshape(v)
 
         # Get just the voxels we're interested in
         Yi = Yi[inds_cv].reshape(1, v_current)
 
@@ -264,15 +264,15 @@
 
 def get_random_mask(dim):
 
     # FWHM
     fwhm = 10
 
     # Load analysis mask
-    mu = nib.load(os.path.join(os.path.dirname(__file__),'mask.nii')).get_data()
+    mu = nib.load(os.path.join(os.path.dirname(__file__),'mask.nii')).get_fdata()
 
     # Add some noise and smooth
     mu = smooth_data(mu + 8*np.random.randn(*(mu.shape)), 3, [fwhm]*3)
 
     # Re-threshold (this has induced a bit of randomness in the mask shape)
     mu = 1*(mu > 0.6)
```

