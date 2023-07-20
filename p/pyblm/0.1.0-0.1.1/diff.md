# Comparing `tmp/pyblm-0.1.0.tar.gz` & `tmp/pyblm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblm-0.1.0.tar", last modified: Thu Jul 20 17:34:09 2023, max compression
+gzip compressed data, was "pyblm-0.1.1.tar", last modified: Thu Jul 20 17:42:07 2023, max compression
```

## Comparing `pyblm-0.1.0.tar` & `pyblm-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:34:09.991907 pyblm-0.1.0/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10899 2023-07-20 17:34:09.989587 pyblm-0.1.0/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10464 2023-07-20 15:14:57.000000 pyblm-0.1.0/README.md
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:34:09.832909 pyblm-0.1.0/blm/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.0/blm/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:02:41.000000 pyblm-0.1.0/blm/blm_cluster.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:34:09.898337 pyblm-0.1.0/blm/lib/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.0/blm/lib/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 15:15:34.000000 pyblm-0.1.0/blm/lib/blm_batch.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 15:15:35.000000 pyblm-0.1.0/blm/lib/blm_concat.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 15:15:35.000000 pyblm-0.1.0/blm/lib/blm_results.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 15:15:35.000000 pyblm-0.1.0/blm/lib/blm_setup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    24399 2023-07-20 15:15:35.000000 pyblm-0.1.0/blm/lib/fileio.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:34:09.920614 pyblm-0.1.0/pyblm.egg-info/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10899 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/SOURCES.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/dependency_links.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/entry_points.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/requires.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 17:34:08.000000 pyblm-0.1.0/pyblm.egg-info/top_level.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 17:34:09.993475 pyblm-0.1.0/setup.cfg
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 17:26:38.000000 pyblm-0.1.0/setup.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:34:09.980227 pyblm-0.1.0/test/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:14:57.000000 pyblm-0.1.0/test/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 15:15:35.000000 pyblm-0.1.0/test/blm_cluster_test.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 15:15:35.000000 pyblm-0.1.0/test/cleanup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17906 2023-07-20 15:15:35.000000 pyblm-0.1.0/test/generate_test_data.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.433488 pyblm-0.1.1/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:42:07.428694 pyblm-0.1.1/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10239 2023-07-20 17:40:09.000000 pyblm-0.1.1/README.md
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.198409 pyblm-0.1.1/blm/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:02:41.000000 pyblm-0.1.1/blm/blm_cluster.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.313847 pyblm-0.1.1/blm/lib/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/lib/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/lib/blm_batch.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_concat.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_results.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_setup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    24399 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/fileio.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.339059 pyblm-0.1.1/pyblm.egg-info/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/entry_points.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/requires.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/top_level.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 17:42:07.434017 pyblm-0.1.1/setup.cfg
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 17:40:45.000000 pyblm-0.1.1/setup.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.425153 pyblm-0.1.1/test/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:14:57.000000 pyblm-0.1.1/test/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/blm_cluster_test.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/cleanup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17906 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/generate_test_data.py
```

### Comparing `pyblm-0.1.0/PKG-INFO` & `pyblm-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # BLM-py
-This repository contains the code for Big Linear Models for Neuroimaging cluster and local usage.
+This repository contains the code for Big Linear Models cluster package.
 
 ## Requirements
-To use the BLM-py code, please clone this repository to your cluster. 
+To use the BLM-py code, please pip install like so:
 
 ```
-git clone https://github.com/TomMaullin/BLM.git
+pip install pyblm
 ```
 
-Then pip install the requirements:
-
-```
-pip install -r requirements.txt
-```
-
-Finally, you must set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
+You must then set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
 
 ```
 jobqueue:
   slurm:
     name: dask-worker
 
     # Dask worker options
@@ -58,18 +52,18 @@
 
     # Scheduler options
     scheduler-options: {'dashboard_address': ':46405'}
 ```
 
 
 ## Usage
-To run `BLM-py` first specify your design using `blm_config.yml` and then run the job in parallel by following the below guidelines.
+To run `BLM-py` first specify your design by creating a `blm_config.yml` file and then run the job in parallel by following the below guidelines.
 
 ### Specifying your model
-The regression model for BLM must be specified in `blm_config.yml`. Below is a complete list of possible inputs to this file.
+The regression model for BLM must be specified in a yaml file (e.g. `blm_config.yml` for instance). Below is a complete list of possible inputs to this file.
 
 #### Mandatory fields
 The following fields are mandatory:
 
  - `Y_files`: Text file containing a list of response variable images in NIFTI format.
  - `X`: CSV file of the design matrix (no column header, no ID row).
  - `outdir`: Path to the output directory.
@@ -144,18 +138,18 @@
 analysis_mask: /path/to/data/MNI152_T1_2mm_brain_mask.nii.gz
 clusterType: SLURM
 numNodes: 100
 ```
 
 ### Running the Analysis
 
-On your HPC system, ensure you are in the `BLM-py` directory and once you are happy with the analysis you have specified in `blm_config.yml`, run the following command:
+BLM can be run from the terminal as follows:
 
 ```
-python blm_cluster.py &
+blm <name_of_your_yaml_file>.yml
 ```
 
 You can watch your analysis progress either by using `qstat` or `squeue` (depending on your system), or by using the interactive dask console. To do so, in a seperate terminal, tunnel into your HPC as follows:
 
 ```
 ssh -L <local port>:localhost:<remote port> username@hpc_address
 ```
```

### Comparing `pyblm-0.1.0/README.md` & `pyblm-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 # BLM-py
-This repository contains the code for Big Linear Models for Neuroimaging cluster and local usage.
+This repository contains the code for Big Linear Models cluster package.
 
 ## Requirements
-To use the BLM-py code, please clone this repository to your cluster. 
+To use the BLM-py code, please pip install like so:
 
 ```
-git clone https://github.com/TomMaullin/BLM.git
+pip install pyblm
 ```
 
-Then pip install the requirements:
-
-```
-pip install -r requirements.txt
-```
-
-Finally, you must set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
+You must then set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
 
 ```
 jobqueue:
   slurm:
     name: dask-worker
 
     # Dask worker options
@@ -43,18 +37,18 @@
 
     # Scheduler options
     scheduler-options: {'dashboard_address': ':46405'}
 ```
 
 
 ## Usage
-To run `BLM-py` first specify your design using `blm_config.yml` and then run the job in parallel by following the below guidelines.
+To run `BLM-py` first specify your design by creating a `blm_config.yml` file and then run the job in parallel by following the below guidelines.
 
 ### Specifying your model
-The regression model for BLM must be specified in `blm_config.yml`. Below is a complete list of possible inputs to this file.
+The regression model for BLM must be specified in a yaml file (e.g. `blm_config.yml` for instance). Below is a complete list of possible inputs to this file.
 
 #### Mandatory fields
 The following fields are mandatory:
 
  - `Y_files`: Text file containing a list of response variable images in NIFTI format.
  - `X`: CSV file of the design matrix (no column header, no ID row).
  - `outdir`: Path to the output directory.
@@ -129,18 +123,18 @@
 analysis_mask: /path/to/data/MNI152_T1_2mm_brain_mask.nii.gz
 clusterType: SLURM
 numNodes: 100
 ```
 
 ### Running the Analysis
 
-On your HPC system, ensure you are in the `BLM-py` directory and once you are happy with the analysis you have specified in `blm_config.yml`, run the following command:
+BLM can be run from the terminal as follows:
 
 ```
-python blm_cluster.py &
+blm <name_of_your_yaml_file>.yml
 ```
 
 You can watch your analysis progress either by using `qstat` or `squeue` (depending on your system), or by using the interactive dask console. To do so, in a seperate terminal, tunnel into your HPC as follows:
 
 ```
 ssh -L <local port>:localhost:<remote port> username@hpc_address
 ```
```

### Comparing `pyblm-0.1.0/blm/blm_cluster.py` & `pyblm-0.1.1/blm/blm_cluster.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/blm/lib/blm_batch.py` & `pyblm-0.1.1/blm/lib/blm_batch.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/blm/lib/blm_concat.py` & `pyblm-0.1.1/blm/lib/blm_concat.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/blm/lib/blm_results.py` & `pyblm-0.1.1/blm/lib/blm_results.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/blm/lib/blm_setup.py` & `pyblm-0.1.1/blm/lib/blm_setup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/blm/lib/fileio.py` & `pyblm-0.1.1/blm/lib/fileio.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/pyblm.egg-info/PKG-INFO` & `pyblm-0.1.1/pyblm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # BLM-py
-This repository contains the code for Big Linear Models for Neuroimaging cluster and local usage.
+This repository contains the code for Big Linear Models cluster package.
 
 ## Requirements
-To use the BLM-py code, please clone this repository to your cluster. 
+To use the BLM-py code, please pip install like so:
 
 ```
-git clone https://github.com/TomMaullin/BLM.git
+pip install pyblm
 ```
 
-Then pip install the requirements:
-
-```
-pip install -r requirements.txt
-```
-
-Finally, you must set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
+You must then set up your `dask-jobqueue` configuration file, which is likely located at `~/.config/dask/jobqueue.yaml`. This will require you to provide some details about your HPC system. See [here](https://jobqueue.dask.org/en/latest/configuration-setup.html#managing-configuration-files) for further detail. For instance, if you are using rescomp your `jobqueue.yaml` file may look something like this:
 
 ```
 jobqueue:
   slurm:
     name: dask-worker
 
     # Dask worker options
@@ -58,18 +52,18 @@
 
     # Scheduler options
     scheduler-options: {'dashboard_address': ':46405'}
 ```
 
 
 ## Usage
-To run `BLM-py` first specify your design using `blm_config.yml` and then run the job in parallel by following the below guidelines.
+To run `BLM-py` first specify your design by creating a `blm_config.yml` file and then run the job in parallel by following the below guidelines.
 
 ### Specifying your model
-The regression model for BLM must be specified in `blm_config.yml`. Below is a complete list of possible inputs to this file.
+The regression model for BLM must be specified in a yaml file (e.g. `blm_config.yml` for instance). Below is a complete list of possible inputs to this file.
 
 #### Mandatory fields
 The following fields are mandatory:
 
  - `Y_files`: Text file containing a list of response variable images in NIFTI format.
  - `X`: CSV file of the design matrix (no column header, no ID row).
  - `outdir`: Path to the output directory.
@@ -144,18 +138,18 @@
 analysis_mask: /path/to/data/MNI152_T1_2mm_brain_mask.nii.gz
 clusterType: SLURM
 numNodes: 100
 ```
 
 ### Running the Analysis
 
-On your HPC system, ensure you are in the `BLM-py` directory and once you are happy with the analysis you have specified in `blm_config.yml`, run the following command:
+BLM can be run from the terminal as follows:
 
 ```
-python blm_cluster.py &
+blm <name_of_your_yaml_file>.yml
 ```
 
 You can watch your analysis progress either by using `qstat` or `squeue` (depending on your system), or by using the interactive dask console. To do so, in a seperate terminal, tunnel into your HPC as follows:
 
 ```
 ssh -L <local port>:localhost:<remote port> username@hpc_address
 ```
```

### Comparing `pyblm-0.1.0/setup.py` & `pyblm-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pyblm",
-    version="0.1.0",
+    version="0.1.1",
     author="Tom Maullin",
     author_email="TomMaullin@gmail.com",
     description="The Big Linear Models Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tommaullin/blm",
     packages=find_packages(),
```

### Comparing `pyblm-0.1.0/test/blm_cluster_test.py` & `pyblm-0.1.1/test/blm_cluster_test.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/test/cleanup.py` & `pyblm-0.1.1/test/cleanup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.0/test/generate_test_data.py` & `pyblm-0.1.1/test/generate_test_data.py`

 * *Files identical despite different names*

