# Comparing `tmp/dask-cuda-23.8.0a230719.tar.gz` & `tmp/dask-cuda-23.8.0a230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.8.0a230719.tar", last modified: Wed Jul 19 05:07:23 2023, max compression
+gzip compressed data, was "dask-cuda-23.8.0a230720.tar", last modified: Thu Jul 20 05:07:51 2023, max compression
```

## Comparing `dask-cuda-23.8.0a230719.tar` & `dask-cuda-23.8.0a230720.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.284019 dask-cuda-23.8.0a230719/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1431 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.288019 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15970 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.288019 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.288019 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20056 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17395 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    11150 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15940 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23370 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9452 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29398 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.288019 dask-cuda-23.8.0a230719/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1680 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-19 05:07:23.000000 dask-cuda-23.8.0a230719/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.280019 dask-cuda-23.8.0a230719/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3019 2023-07-19 05:07:17.000000 dask-cuda-23.8.0a230719/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 05:07:23.292019 dask-cuda-23.8.0a230719/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 05:07:15.000000 dask-cuda-23.8.0a230719/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.382872 dask-cuda-23.8.0a230720/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-20 05:07:51.382872 dask-cuda-23.8.0a230720/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.374872 dask-cuda-23.8.0a230720/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.378872 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15970 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8571 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.378872 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.378872 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20056 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17377 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.382872 dask-cuda-23.8.0a230720/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15940 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23370 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.374872 dask-cuda-23.8.0a230720/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-20 05:07:51.000000 dask-cuda-23.8.0a230720/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.366872 dask-cuda-23.8.0a230720/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 05:07:51.382872 dask-cuda-23.8.0a230720/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3019 2023-07-20 05:07:44.000000 dask-cuda-23.8.0a230720/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 05:07:51.382872 dask-cuda-23.8.0a230720/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 05:07:42.000000 dask-cuda-23.8.0a230720/setup.py
```

### Comparing `dask-cuda-23.8.0a230719/LICENSE` & `dask-cuda-23.8.0a230720/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/PKG-INFO` & `dask-cuda-23.8.0a230720/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230719
+Version: 23.8.0a230720
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
-[![RTD](https://readthedocs.org/projects/dask-cuda/badge/?version=latest)](https://dask-cuda.readthedocs.io/en/latest/?badge=latest)
-
 Dask CUDA
 =========
 
 Various utilities to improve deployment and management of Dask workers on
 CUDA-enabled systems.
 
 This library is experimental, and its API is subject to change at any time
@@ -38,20 +36,20 @@
 from dask_cuda import LocalCUDACluster
 from dask.distributed import Client
 
 cluster = LocalCUDACluster()
 client = Client(cluster)
 ```
 
-Documentation is available [here](https://dask-cuda.readthedocs.io/).
+Documentation is available [here](https://docs.rapids.ai/api/dask-cuda/nightly/).
 
 What this is not
 ----------------
 
 This library does not automatically convert your Dask code to run on GPUs.
 
 It only helps with deployment and management of Dask workers in multi-GPU
 systems.  Parallelizing GPU libraries like [RAPIDS](https://rapids.ai) and
 [CuPy](https://cupy.chainer.org) with Dask is an ongoing effort.  You may wish
 to read about this effort at [blog.dask.org](https://blog.dask.org) for more
 information.  Additional information about Dask-CUDA can also be found in the
-[docs]( https://dask-cuda.readthedocs.io ).
+[docs](https://docs.rapids.ai/api/dask-cuda/nightly/).
```

### Comparing `dask-cuda-23.8.0a230719/README.md` & `dask-cuda-23.8.0a230720/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-[![RTD](https://readthedocs.org/projects/dask-cuda/badge/?version=latest)](https://dask-cuda.readthedocs.io/en/latest/?badge=latest)
-
 Dask CUDA
 =========
 
 Various utilities to improve deployment and management of Dask workers on
 CUDA-enabled systems.
 
 This library is experimental, and its API is subject to change at any time
@@ -16,20 +14,20 @@
 from dask_cuda import LocalCUDACluster
 from dask.distributed import Client
 
 cluster = LocalCUDACluster()
 client = Client(cluster)
 ```
 
-Documentation is available [here](https://dask-cuda.readthedocs.io/).
+Documentation is available [here](https://docs.rapids.ai/api/dask-cuda/nightly/).
 
 What this is not
 ----------------
 
 This library does not automatically convert your Dask code to run on GPUs.
 
 It only helps with deployment and management of Dask workers in multi-GPU
 systems.  Parallelizing GPU libraries like [RAPIDS](https://rapids.ai) and
 [CuPy](https://cupy.chainer.org) with Dask is an ongoing effort.  You may wish
 to read about this effort at [blog.dask.org](https://blog.dask.org) for more
 information.  Additional information about Dask-CUDA can also be found in the
-[docs]( https://dask-cuda.readthedocs.io ).
+[docs](https://docs.rapids.ai/api/dask-cuda/nightly/).
```

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/__init__.py` & `dask-cuda-23.8.0a230720/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/common.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.8.0a230720/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/cli.py` & `dask-cuda-23.8.0a230720/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/cuda_worker.py` & `dask-cuda-23.8.0a230720/dask_cuda/cuda_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
                     "https://github.com/rapidsai/rmm"
                 )  # pragma: no cover
         else:
             if enable_nvlink:
                 warnings.warn(
                     "When using NVLink we recommend setting a "
                     "`rmm_pool_size`.  Please see: "
-                    "https://dask-cuda.readthedocs.io/en/latest/ucx.html"
-                    "#important-notes for more details"
+                    "https://docs.rapids.ai/api/dask-cuda/nightly/ucx/ "
+                    "for more details"
                 )
 
         if enable_nvlink and rmm_managed_memory:
             raise ValueError(
                 "RMM managed memory and NVLink are currently incompatible."
             )
```

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/device_host_file.py` & `dask-cuda-23.8.0a230720/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/disk_io.py` & `dask-cuda-23.8.0a230720/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.8.0a230720/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.8.0a230720/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/initialize.py` & `dask-cuda-23.8.0a230720/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/is_device_object.py` & `dask-cuda-23.8.0a230720/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/is_spillable_object.py` & `dask-cuda-23.8.0a230720/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.8.0a230720/dask_cuda/local_cuda_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,16 +272,16 @@
                     "see https://github.com/rapidsai/rmm"
                 )  # pragma: no cover
         else:
             if enable_nvlink:
                 warnings.warn(
                     "When using NVLink we recommend setting a "
                     "`rmm_pool_size`. Please see: "
-                    "https://dask-cuda.readthedocs.io/en/latest/ucx.html"
-                    "#important-notes for more details"
+                    "https://docs.rapids.ai/api/dask-cuda/nightly/ucx/ "
+                    "for more details"
                 )
 
         self.rmm_log_directory = rmm_log_directory
         self.rmm_track_allocations = rmm_track_allocations
 
         if not kwargs.pop("processes", True):
             raise ValueError(
```

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.8.0a230720/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/proxify_host_file.py` & `dask-cuda-23.8.0a230720/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/proxy_object.py` & `dask-cuda-23.8.0a230720/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_gds.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_spill.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_utils.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.8.0a230720/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/utils.py` & `dask-cuda-23.8.0a230720/dask_cuda/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import math
 import operator
 import os
+import pickle
 import time
 import warnings
 from contextlib import suppress
 from functools import singledispatch
 from multiprocessing import cpu_count
 from typing import Optional
 
@@ -712,22 +713,28 @@
 
 def get_worker_config(dask_worker):
     from .proxify_host_file import ProxifyHostFile
 
     # assume homogeneous cluster
     plugin_vals = dask_worker.plugins.values()
     ret = {}
-
     # device and host memory configuration
     for p in plugin_vals:
-        ret[f"[plugin] {type(p).__name__}"] = {
+        config = {
             v: getattr(p, v)
             for v in dir(p)
             if not (v.startswith("_") or v in {"setup", "cores"})
         }
+        # To send this back to the client the data will be serialised
+        # which might fail, so pre-emptively check
+        try:
+            pickle.dumps(config)
+        except TypeError:
+            config = "UNKNOWN CONFIG"
+        ret[f"[plugin] {type(p).__name__}"] = config
 
     for mem in [
         "memory_limit",
         "memory_pause_fraction",
         "memory_spill_fraction",
         "memory_target_fraction",
     ]:
```

### Comparing `dask-cuda-23.8.0a230719/dask_cuda/worker_spec.py` & `dask-cuda-23.8.0a230720/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.8.0a230720/dask_cuda.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230719
+Version: 23.8.0a230720
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
-[![RTD](https://readthedocs.org/projects/dask-cuda/badge/?version=latest)](https://dask-cuda.readthedocs.io/en/latest/?badge=latest)
-
 Dask CUDA
 =========
 
 Various utilities to improve deployment and management of Dask workers on
 CUDA-enabled systems.
 
 This library is experimental, and its API is subject to change at any time
@@ -38,20 +36,20 @@
 from dask_cuda import LocalCUDACluster
 from dask.distributed import Client
 
 cluster = LocalCUDACluster()
 client = Client(cluster)
 ```
 
-Documentation is available [here](https://dask-cuda.readthedocs.io/).
+Documentation is available [here](https://docs.rapids.ai/api/dask-cuda/nightly/).
 
 What this is not
 ----------------
 
 This library does not automatically convert your Dask code to run on GPUs.
 
 It only helps with deployment and management of Dask workers in multi-GPU
 systems.  Parallelizing GPU libraries like [RAPIDS](https://rapids.ai) and
 [CuPy](https://cupy.chainer.org) with Dask is an ongoing effort.  You may wish
 to read about this effort at [blog.dask.org](https://blog.dask.org) for more
 information.  Additional information about Dask-CUDA can also be found in the
-[docs]( https://dask-cuda.readthedocs.io ).
+[docs](https://docs.rapids.ai/api/dask-cuda/nightly/).
```

### Comparing `dask-cuda-23.8.0a230719/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.8.0a230720/dask_cuda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,9 +46,8 @@
 dask_cuda/tests/test_local_cuda_cluster.py
 dask_cuda/tests/test_proxify_host_file.py
 dask_cuda/tests/test_proxy.py
 dask_cuda/tests/test_spill.py
 dask_cuda/tests/test_utils.py
 dask_cuda/tests/test_worker_spec.py
 examples/ucx/client_initialize.py
-examples/ucx/local_cuda_cluster.py
-rtd/conf.py
+examples/ucx/local_cuda_cluster.py
```

### Comparing `dask-cuda-23.8.0a230719/examples/ucx/client_initialize.py` & `dask-cuda-23.8.0a230720/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.8.0a230720/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230719/pyproject.toml` & `dask-cuda-23.8.0a230720/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=64.0.0",
     "tomli  ; python_version < '3.11'",
 ]
 
 [project]
 name = "dask-cuda"
-version = "23.08.00a230719"
+version = "23.08.00a230720"
 description = "Utilities for Dask and CUDA interactions"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "NVIDIA Corporation" },
 ]
 license = { text = "Apache-2.0" }
 requires-python = ">=3.9"
```

