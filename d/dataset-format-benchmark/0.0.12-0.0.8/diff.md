# Comparing `tmp/dataset-format-benchmark-0.0.12.tar.gz` & `tmp/dataset-format-benchmark-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-format-benchmark-0.0.12.tar", last modified: Thu Jul 20 16:36:27 2023, max compression
+gzip compressed data, was "dataset-format-benchmark-0.0.8.tar", last modified: Thu Jan  5 18:02:18 2023, max compression
```

## Comparing `dataset-format-benchmark-0.0.12.tar` & `dataset-format-benchmark-0.0.8.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.238841 dataset-format-benchmark-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.218841 dataset-format-benchmark-0.0.12/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.226841 dataset-format-benchmark-0.0.12/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 16:36:27.238841 dataset-format-benchmark-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.230841 dataset-format-benchmark-0.0.12/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.230841 dataset-format-benchmark-0.0.12/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-20 16:36:27.238841 dataset-format-benchmark-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.222841 dataset-format-benchmark-0.0.12/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/face_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/flicrk_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/wiki_art.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/ffhq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/own/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/own/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/own/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/models/inception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.238841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/storages/
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/storages/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/storages/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.234841 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 16:36:27.000000 dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:36:27.238841 dataset-format-benchmark-0.0.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 16:36:10.000000 dataset-format-benchmark-0.0.12/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.100314 dataset-format-benchmark-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.100314 dataset-format-benchmark-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/face_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/flicrk_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/wiki_art.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/ffhq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/own/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/own/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/own/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/models/inception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/storages/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/storages/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.104314 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-05 18:02:18.000000 dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:02:18.108314 dataset-format-benchmark-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-05 18:02:07.000000 dataset-format-benchmark-0.0.8/tests/conftest.py
```

### Comparing `dataset-format-benchmark-0.0.12/.coveragerc` & `dataset-format-benchmark-0.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/.github/workflows/python-publish.yml` & `dataset-format-benchmark-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/.gitignore` & `dataset-format-benchmark-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/Dockerfile` & `dataset-format-benchmark-0.0.8/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.11-slim as build-image
+FROM python:3.10-slim as build-image
 
 WORKDIR /usr/local/bin/deployment
 
 RUN apt-get update && apt-get upgrade -y
 RUN apt-get install -y curl ca-certificates gnupg
 RUN apt-get install -y gcc g++ make libffi-dev git cargo
 
@@ -18,19 +18,19 @@
 RUN  export APP_HOME=/usr/local/bin/deployment \
      && (cd $APP_HOME \
          && python3 -m venv py3env \
          && . py3env/bin/activate \
          && python3 -m pip install -U pip \
          && python3 -m pip install -U setuptools \
          && python3 -m pip install -U wheel \
-         && python3 -m pip install -U --pre torch\<2.0.0 torchvision --extra-index-url https://download.pytorch.org/whl/nightly/cu118 \
-         && python3 -m pip install -U /tmp/build/dist/*.whl)
+         && python3 -m pip install -U --pre torch torchvision --extra-index-url https://download.pytorch.org/whl/nightly/cu117 \
+         && python3 -m pip install -U dataset_format_benchmark --find-links=/tmp/build/dist)
 
 
-FROM python:3.11-slim
+FROM python:3.10-slim
 
 ENV  PYTHONPATH=/usr/local/bin/deployment
 
 WORKDIR /usr/local/bin/deployment
 
 COPY --from=build-image /usr/local/bin/deployment/ ./
```

### Comparing `dataset-format-benchmark-0.0.12/LICENSE` & `dataset-format-benchmark-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/docs/Makefile` & `dataset-format-benchmark-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/docs/conf.py` & `dataset-format-benchmark-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/docs/index.rst` & `dataset-format-benchmark-0.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/setup.cfg` & `dataset-format-benchmark-0.0.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataset-format-benchmark
-version = 0.0.11
+version = 0.0.1
 description = Image dataset format benchmark
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/dataset-format-benchmark
@@ -19,43 +19,35 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	Cython==3.0.0
-	h5py==3.9.0
-	imageio[freeimage,opencv,pillow,pyav]==2.31.1
-	kaggle==1.5.16
-	matplotlib==3.7.2
-	numpy==1.25.1
-	Pillow==10.0.0
-	pkgconfig==1.5.5
-	pytorch-lightning==1.9.3
-	rawpy==0.18.1
-	scikit-learn==1.3.0
-	scipy==1.11.1
+	cupy-cuda11x==11.4.0
+	h5py==3.7.0
+	kaggle==1.5.12
+	matplotlib==3.6.2
+	numpy==1.24.1
+	Pillow==9.4.0
+	scikit-learn==1.2.0
+	scipy==1.10.0
 	seaborn==0.12.2
 	torch
 	torchvision
-	tqdm==4.65.0
-	zarr==2.15.0
-	requests==2.28.2
-	urllib3<1.27
-python_requires = >=3.11
+	tqdm==4.64.1
+	zarr==2.13.3
+python_requires = >=3.10
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
-cuda = 
-	cupy-cuda12x==11.5.0
 testing = 
 	pytest
 	pytest-cov
 
 [options.entry_points]
 
 [test]
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/__main__.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import argparse
 import logging
 import time
 from pathlib import Path
-from typing import Sequence
 
 import matplotlib.pyplot as plt
 import torch.utils.data
-from rawpy._rawpy import ColorSpace
 
-from dataset_format_benchmark.datasets import PyTorchDataset
+from dataset_format_benchmark.extmod import c_fib
+from dataset_format_benchmark.datasets import BaseDataset, PyTorchDataset
+from dataset_format_benchmark.datasets.kaggle.face_masks import FaceMasksDataset
+from dataset_format_benchmark.datasets.kaggle.wiki_art import WikiArtDataset
+from dataset_format_benchmark.datasets.nvidia.ffhq import NvidiaFFHQDataset
 from dataset_format_benchmark.datasets.own.transport import OwnTransportDataset
 from dataset_format_benchmark.models.inception import InceptionNet
 from dataset_format_benchmark.runner import benchmark_dataset
-from dataset_format_benchmark.storages.containers import NumpyZipImageStorage
+from dataset_format_benchmark.storages import ImageFileStorage
 from dataset_format_benchmark.storages.fs import (
-    JPEGImageStorage, PNGImageStorage, BMPImageStorage, TIFFImageStorage
+    JPEGImageStorage, PNGImageStorage, BMPImageStorage, TIFFImageStorage, WebPImageStorage
 )
 
 logger = logging.getLogger(__name__)
 
 plt.rcParams['figure.figsize'] = (15, 5)
 plt.style.use('dark_background')
 
@@ -46,68 +48,57 @@
     device = torch.device('cuda' if use_cuda else 'cpu')
     worker_count = 4  # multiprocessing.cpu_count() if USE_CUDA else 0
     train_test_split = 0.8
     batch_size = 8
     learning_rate = 1e-8
     epochs = 100
 
-    datasets: Sequence = (
+    datasets: list[BaseDataset] = [
         OwnTransportDataset(root=data_root_path),
         # FaceMasksDataset(root=data_root_path),
         # WikiArtDataset(root=data_root_path),
         # NvidiaFFHQDataset(root=data_root_path),
-    )
-    color_spaces = (
-        ColorSpace.sRGB,
-        # ColorSpace.Adobe,
-        # ColorSpace.ACES,
-        # ColorSpace.ProPhoto,
-        # ColorSpace.XYZ,
-        # ColorSpace.Wide
-    )
-    storages: Sequence = (
-        JPEGImageStorage(quality=100, color_spaces=color_spaces),
-        JPEGImageStorage(quality=75, color_spaces=color_spaces),
-        JPEGImageStorage(quality=50, color_spaces=color_spaces),
-        JPEGImageStorage(quality=25, color_spaces=color_spaces),
-        JPEGImageStorage(quality=10, color_spaces=color_spaces),
-        PNGImageStorage(color_spaces=color_spaces),
-        BMPImageStorage(color_spaces=color_spaces),
-        TIFFImageStorage(color_spaces=color_spaces),
-        # WebPImageStorage(),
-        NumpyZipImageStorage(color_spaces=color_spaces),
+    ]
+    storages: list[ImageFileStorage] = [
+        JPEGImageStorage(quality=100),
+        PNGImageStorage(),
+        BMPImageStorage(),
+        TIFFImageStorage(),
+        WebPImageStorage(),
+        # NumpyZipImageStorage(),
         # NumpyMmapImageStorage(),
         # CupyMmapImageStorage(),
-    )
-    models: Sequence = (
+    ]
+    models = (
         InceptionNet,
         # DenseNet,
     )
 
     # Loading original dataset and storing in storages
     for dataset in datasets:
         dataset_class_name = dataset.__class__.__name__
 
-        for storage in storages:
-            dataset.add_storage(storage)
-
         logger.info(f'Loading dataset: {dataset_class_name}')
         dataset.load()
 
+        for storage in storages:
+            storage.store_dataset(dataset)
+            dataset.add_storage(storage)
+
     # Testing models against all dataset storages and models
     for dataset in datasets:
         for storage in dataset.get_storages():
             for model in models:
                 dataset_class_name = dataset.__class__.__name__
                 model_class_name = model.__name__
 
                 try:
                     start_time = time.perf_counter()
                     logger.info(f'{start_time}: Benchmarking dataset{dataset_class_name} with {model_class_name} model')
-                    pytorch_dataset = PyTorchDataset(dataset, storage)
+                    pytorch_dataset = PyTorchDataset(storage)
                     benchmark_dataset(pytorch_dataset, epochs, train_test_split, batch_size, learning_rate, use_cuda,
                                       worker_count, device)
                     end_time = time.perf_counter()
                     logger.info(f'{end_time}: Benchmark took {end_time - start_time}')
                 except KeyboardInterrupt:
                     logger.info(f'Skipping {dataset_class_name} / {model_class_name}')
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/__init__.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Iterator, Generator, Sequence
+from typing import Iterator, Optional
 
 import torch
 import torch.utils.data
 from torch.utils.data.dataset import T_co
 
 from dataset_format_benchmark.storages import ImageFileStorage
 
@@ -15,34 +15,27 @@
     DATASET_DIR_NAME = None
     METADATA_FILE_NAME = None
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__()
         self.device = torch.device('cuda' if USE_CUDA else 'cpu')
         self.data_length = 0
-        self.dataset_root_path = Path(root, self.DATASET_DIR_NAME)
-        self.metadata_file_path = Path(self.dataset_root_path, 'metadata_fs.json')
-        self.filenames: Sequence[str] = []
+        self.dataset_path = Path(root, self.DATASET_DIR_NAME)
+        self.metadata_file_path = Path(self.dataset_path, 'metadata_fs.json')
         self.storages: list[ImageFileStorage] = []
 
     def add_storage(self, storage: ImageFileStorage):
         self.storages.append(storage)
 
     def get_storages(self) -> list[ImageFileStorage]:
         return self.storages
 
-    def iter_files(self, root: Path, recursive: bool = True) -> Generator[Path, None, None]:
-        for item in root.iterdir():
-            if item.is_file():
-                yield item
-            elif item.is_dir() and recursive and not item.name.startswith('.'):
-                yield from self.iter_files(item)
-
+    @staticmethod
     @abstractmethod
-    def iter_images(self, root: Path) -> Iterator:
+    def iter_images(root: Path, min_size: Optional[int] = None) -> Iterator:
         pass
 
     def _download(self, force: bool = False):
         pass
 
     @abstractmethod
     def _prepare(self, force: bool = False):
@@ -53,18 +46,17 @@
         self._prepare(force_prepare)
 
     def __len__(self):
         return self.data_length
 
 
 class PyTorchDataset(torch.utils.data.Dataset):
-    def __init__(self, dataset: BaseDataset, storage: ImageFileStorage, transform=None, target_transform=None):
+    def __init__(self, storage: ImageFileStorage, transform=None, target_transform=None):
         super().__init__()
         self.device = torch.device('cuda' if USE_CUDA else 'cpu')
-        self.dataset = dataset
         self.storage = storage
 
     def __getitem__(self, index) -> T_co:
-        return self.storage[self.dataset[index]]
+        return self.storage[index]
 
     def __len__(self):
-        return len(self.dataset)
+        return len(self.storage)
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/__init__.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     IMAGE_WIDTH = None
     RESULT_FILE_NAME = None
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
 
         if self.IMAGE_DIR_NAME:
-            self.image_dir_path = Path(self.dataset_root_path, self.IMAGE_DIR_NAME)
+            self.image_dir_path = Path(self.dataset_path, self.IMAGE_DIR_NAME)
         else:
             self.image_dir_path = None
 
         if self.RESULT_FILE_NAME:
-            self.result_file_path = Path(self.dataset_root_path, self.RESULT_FILE_NAME)
+            self.result_file_path = Path(self.dataset_path, self.RESULT_FILE_NAME)
         else:
             self.result_file_path = None
 
         self.transform = transform
         self.target_transform = target_transform
         self.x = None
         self.y = None
@@ -33,12 +33,12 @@
     def _download(self, force: bool = False):
         import kaggle
 
         kaggle.api.authenticate()
 
         if isinstance(self.DATASET_NAME, list):
             for dataset_name in self.DATASET_NAME:
-                kaggle.api.dataset_download_files(dataset_name, path=self.dataset_root_path, quiet=False, unzip=True,
+                kaggle.api.dataset_download_files(dataset_name, path=self.dataset_path, quiet=False, unzip=True,
                                                   force=force)
         else:
-            kaggle.api.dataset_download_files(self.DATASET_NAME, path=self.dataset_root_path, quiet=False, unzip=True,
+            kaggle.api.dataset_download_files(self.DATASET_NAME, path=self.dataset_path, quiet=False, unzip=True,
                                               force=force)
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/face_masks.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/face_masks.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,35 +34,35 @@
         3: 'There is no mask on the face.',
     }
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
 
         if self.DATASET_SUBDIR_NAME:
-            self.dataset_subdir_path = Path(self.dataset_root_path, self.DATASET_SUBDIR_NAME)
+            self.dataset_subdir_path = Path(self.dataset_path, self.DATASET_SUBDIR_NAME)
         else:
-            self.dataset_subdir_path = self.dataset_root_path
+            self.dataset_subdir_path = self.dataset_path
 
         if self.DATASET_FILE_NAME:
             self.dataset_file_path = Path(self.dataset_subdir_path, self.DATASET_FILE_NAME)
         else:
             self.dataset_file_path = None
 
         if self.METADATA_FILE_NAME:
             self.metadata_file_path = Path(self.dataset_subdir_path, self.METADATA_FILE_NAME)
         else:
             self.metadata_file_path = None
 
     def _download(self, force: bool = False):
-        if force or not self.dataset_root_path.exists():
+        if force or not self.dataset_path.exists():
             super()._download(force)
 
-            second_file_path = Path(self.dataset_root_path, 'df_part_2.csv')
+            second_file_path = Path(self.dataset_path, 'df_part_2.csv')
 
-            with open(second_file_path) as fi, open(Path(self.dataset_root_path, 'df.csv'), 'a') as fo:
+            with open(second_file_path) as fi, open(Path(self.dataset_path, 'df.csv'), 'a') as fo:
                 next(fi)
                 fo.writelines(fi)
 
             second_file_path.unlink(missing_ok=True)
 
     @staticmethod
     def iter_images(root: Path, min_size: Optional[int] = None) -> Generator:
@@ -140,15 +140,15 @@
         if force or not self.metadata_file_path.exists():
             min_size = self._get_min_size()
             print(f'Found minimum size: {min_size}px')
 
             image_set = self._resize_images(min_size)
             directories = sorted(
                 file_item.name
-                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_root_path.iterdir())
+                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_path.iterdir())
             )
 
             metadata = {
                 'labels': {idx: dir_name for idx, dir_name in enumerate(directories)},
                 'images': image_set
             }
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/flicrk_image.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/flicrk_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     IMAGE_WIDTH = 256
     RESULT_FILE_NAME = 'results.csv'
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
 
     def _download(self, force: bool = False):
-        if force or not self.dataset_root_path.exists():
+        if force or not self.dataset_path.exists():
             super()._download(force)
             # Removing duplicated data
             rmtree(Path(self.image_dir_path, self.DATASET_DIR_NAME), ignore_errors=True)
             Path(self.image_dir_path, self.RESULT_FILE_NAME).unlink(missing_ok=True)
 
     def _prepare(self, force: bool = False):
         pass
@@ -86,15 +86,15 @@
 
         return x, y
 
 
 class DatasetFlickrImageZarr(DatasetFlickrImage):
     def __init__(self, root: Path, transform=None, target_transform=None, chunks=None):
         super().__init__(root, transform, target_transform)
-        self.dataset_file_path = Path(self.dataset_root_path, 'data.zarr')
+        self.dataset_file_path = Path(self.dataset_path, 'data.zarr')
         self.chunks = chunks
 
     def _prepare(self, force: bool = True):
         if force or not self.dataset_file_path.exists():
             with open(self.result_file_path, mode='r', encoding='utf-8') as f:
                 reader = csv.reader(f, delimiter='|')
                 # Skipping header
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/kaggle/wiki_art.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/kaggle/wiki_art.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     IMAGE_HEIGHT = 256
     IMAGE_WIDTH = 256
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
 
         if self.METADATA_FILE_NAME:
-            self.metadata_file_path = Path(self.dataset_root_path, self.METADATA_FILE_NAME)
+            self.metadata_file_path = Path(self.dataset_path, self.METADATA_FILE_NAME)
         else:
             self.metadata_file_path = None
 
     def _download(self, force: bool = False):
-        if force or not self.dataset_root_path.exists():
+        if force or not self.dataset_path.exists():
             super()._download(force)
 
     @staticmethod
     def iter_images(root: Path, min_size: Optional[int] = None) -> Generator:
         dir_names = sorted(
             file_item.name for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', root.iterdir())
         )
@@ -53,15 +53,15 @@
                             yield idx, image
                     except UnidentifiedImageError:
                         pass
 
     def _get_min_size(self, limit_size: Optional[int] = None):
         min_size = 999999
 
-        for _, image in self.iter_images(self.dataset_root_path, limit_size):
+        for _, image in self.iter_images(self.dataset_path, limit_size):
             width, height = image.size
 
             # Filter out images with any dimension smaller than self.IMAGE_WIDTH px
             min_size = max(limit_size, min(min_size, min(height, width)))
 
         return min_size
 
@@ -76,15 +76,15 @@
 
             raise NotImplementedError
 
             image_set = self._resize_images(min_size)
 
             directories = sorted(
                 file_item.name
-                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_root_path.iterdir())
+                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_path.iterdir())
             )
 
             metadata = {
                 'labels': {idx: dir_name for idx, dir_name in enumerate(directories)},
                 'images': image_set
             }
 
@@ -98,15 +98,15 @@
 
     def _resize_images(self, size: Optional[int] = None) -> Mapping[str, int]:
         image_set = {}
         dir_indexes = set()
 
         self.image_dir_path.mkdir(exist_ok=True)
 
-        for idx, image in self.iter_images(self.dataset_root_path, size):
+        for idx, image in self.iter_images(self.dataset_path, size):
             crop_dir_path = Path(self.image_dir_path, str(idx))
             file_name = Path(image.filename).name
 
             if idx not in dir_indexes:
                 crop_dir_path.mkdir(exist_ok=True)
                 dir_indexes.add(idx)
 
@@ -157,15 +157,15 @@
 
         return x, y
 
 
 class DatasetWikiArtZarr(WikiArtDataset):
     def __init__(self, root: Path, transform=None, target_transform=None, chunks=None):
         super().__init__(root, transform, target_transform)
-        self.dataset_file_path = Path(self.dataset_root_path, 'data.zarr')
+        self.dataset_file_path = Path(self.dataset_path, 'data.zarr')
         self.chunks = chunks
 
     def _prepare(self, force: bool = True):
         if force or not self.dataset_file_path.exists():
             with open(self.result_file_path, mode='r', encoding='utf-8') as f:
                 reader = csv.reader(f, delimiter='|')
                 # Skipping header
@@ -224,35 +224,35 @@
 
 class DatasetWikiArtNumpyMmap(WikiArtDataset):
     DATASET_DTYPE = 'float16'
     METADATA_FILE_NAME = 'metadata_numpy_mmap.json'
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
-        self.dataset_file_path = Path(self.dataset_root_path, 'data.npy')
+        self.dataset_file_path = Path(self.dataset_path, 'data.npy')
 
     def __count_images(self, min_size: Optional[int] = None) -> int:
         cnt = sum(
             int(min(image.width, image.height) >= min_size)
-            for _, image in self.iter_images(self.dataset_root_path)
+            for _, image in self.iter_images(self.dataset_path)
         )
 
         return cnt
 
     def _resize_images(self, size: Optional[int] = None):
         item_count = self.__count_images(size)
         print(f'Item count: {item_count}')
         dataset_shape = (item_count, 3, size, size)
 
         x = open_memmap(
             str(self.dataset_file_path), mode='w+', dtype=self.DATASET_DTYPE, shape=dataset_shape
         )
         y = []
 
-        for idx, (dir_idx, image) in enumerate(self.iter_images(self.dataset_root_path, size)):
+        for idx, (dir_idx, image) in enumerate(self.iter_images(self.dataset_path, size)):
             file_name = Path(image.filename).name
 
             try:
                 image = adjust_image(image, size, size)
             except OSError as e:
                 print(f'Failed reading image file: {dir_idx}/{file_name}, {e}. Deleting original file')
                 Path(image.filename).unlink(missing_ok=True)
@@ -310,35 +310,35 @@
 
 class DatasetWikiArtCuPyMmap(WikiArtDataset):
     DATASET_DTYPE = 'float16'
     METADATA_FILE_NAME = 'metadata_cupy_mmap.json'
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
-        self.dataset_file_path = Path(self.dataset_root_path, 'cupy_data.npz')
+        self.dataset_file_path = Path(self.dataset_path, 'cupy_data.npz')
 
     def __count_images(self, min_size: Optional[int] = None) -> int:
         cnt = sum(
             int(min(image.width, image.height) >= min_size)
-            for _, image in self.iter_images(self.dataset_root_path)
+            for _, image in self.iter_images(self.dataset_path)
         )
 
         return cnt
 
     def _resize_images(self, size: Optional[int] = None):
         item_count = self.__count_images(size)
         print(f'Item count: {item_count}')
         dataset_shape = (item_count, 3, size, size)
 
         x = open_memmap(
             str(self.dataset_file_path), mode='w+', dtype=self.DATASET_DTYPE, shape=dataset_shape
         )
         y = []
 
-        for idx, (dir_idx, image) in enumerate(self.iter_images(self.dataset_root_path, size)):
+        for idx, (dir_idx, image) in enumerate(self.iter_images(self.dataset_path, size)):
             file_name = Path(image.filename).name
 
             try:
                 image = adjust_image(image, size, size)
             except OSError as e:
                 print(f'Failed reading image file: {dir_idx}/{file_name}, {e}. Deleting original file')
                 Path(image.filename).unlink(missing_ok=True)
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/downloader.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/downloader.py`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/nvidia/ffhq.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/nvidia/ffhq.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
     IMAGE_WIDTH = 1024
     RESULT_FILE_NAME = 'df.csv'
 
     def __init__(self, root: Path, transform=None, target_transform=None):
         super().__init__(root, transform, target_transform)
 
         if self.DATASET_SUBDIR_NAME:
-            self.dataset_subdir_path = Path(self.dataset_root_path, self.DATASET_SUBDIR_NAME)
+            self.dataset_subdir_path = Path(self.dataset_path, self.DATASET_SUBDIR_NAME)
         else:
-            self.dataset_subdir_path = self.dataset_root_path
+            self.dataset_subdir_path = self.dataset_path
 
         if self.DATASET_FILE_NAME:
             self.dataset_file_path = Path(self.dataset_subdir_path, self.DATASET_FILE_NAME)
         else:
             self.dataset_file_path = None
 
         if self.METADATA_FILE_NAME:
             self.metadata_file_path = Path(self.dataset_subdir_path, self.METADATA_FILE_NAME)
         else:
             self.metadata_file_path = None
 
     def _download(self, force: bool = False):
-        if force or not self.dataset_root_path.exists():
+        if force or not self.dataset_path.exists():
             tasks = ('json', 'stats', 'images',)
             downloader.run(tasks)
 
     @staticmethod
     def iter_images(root: Path, min_size: Optional[int] = None):
         # ID, TYPE, USER_ID, GENDER, AGE, name, size_mb
 
@@ -121,15 +121,15 @@
         if force or not self.metadata_file_path.exists():
             min_size = self._get_min_size()
             print(f'Found minimum size: {min_size}px')
 
             image_set = self._resize_images(min_size)
             directories = sorted(
                 file_item.name
-                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_root_path.iterdir())
+                for file_item in filter(lambda i: i.is_dir() and i.name[0] != '.', self.dataset_path.iterdir())
             )
 
             metadata = {
                 'labels': {idx: dir_name for idx, dir_name in enumerate(directories)},
                 'images': image_set
             }
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/datasets/utils.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/models/inception.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/models/inception.py`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/runner.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/runner.py`

 * *Files identical despite different names*

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark/storages/containers.py` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark/storages/containers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,185 +1,173 @@
+import json
 from pathlib import Path
-from typing import Sequence
+from typing import Optional
 
-import imageio as iio
 import numpy as np
-
-from dataset_format_benchmark.storages import ImageFileStorage
+import torch
+import torch.utils.data
+from meeting06.datasets.utils import adjust_image
+from meeting06.storages import ImageFileStorage
+from numpy.lib.format import open_memmap
+from torch.nn import functional
 
 
 class NumpyZipImageStorage(ImageFileStorage):
-    IMAGE_FILE_EXTENSION = 'npz'
-    DATASET_SUBDIR_NAME = f'{IMAGE_FILE_EXTENSION}_files'
+    DATASET_DTYPE = 'float16'
+    DATASET_SUBDIR_NAME = 'numpy_zip_files'
+    METADATA_FILE_NAME = 'metadata.json'
+
+    def _resize_images(self, size: Optional[int] = None):
+        item_count = self._count_images(size)
+        print(f'Item count: {item_count}')
+
+        self.dataset_subdir_path.mkdir(exist_ok=True)
+
+        x = []
+        y = []
+
+        for idx, (label, image) in enumerate(self._iter_images(self.image_dir_path, size)):
+            label = int(label) - 1
+            file_name = Path(image.filename).name
+            print(f'{idx}/{item_count}: Processing {file_name}')
+
+            try:
+                image = adjust_image(image, size, size)
+            except OSError as e:
+                print(f'Failed reading image file: {file_name}, {e}. Deleting original file')
+                Path(image.filename).unlink(missing_ok=True)
+            else:
+                image = np.asarray(image) / 255.0
+                # Converting HxWxC to CxHxW
+                image = np.transpose(image, (2, 0, 1))
+                file_name_base = file_name.split('.', maxsplit=1)[0]
+                label_dir_path = Path(self.dataset_subdir_path, str(label))
+                label_dir_path.mkdir(exist_ok=True)
+                out_file_path = Path(label_dir_path, f'{file_name_base}.npz')
+                np.savez_compressed(out_file_path, value=image)
+                x.append(f'{label}/{file_name_base}.npz')
+                y.append(label)
+
+        metadata = {
+            'shape': (3, size, size),
+            'filenames': x,
+            'labels': y
+        }
+
+        return metadata
+
+    def _prepare(self, force: bool = True):
+        if force or not self.metadata_file_path.exists():
+            print('Preparing dataset')
+            min_size = self._get_min_size(self.IMAGE_WIDTH)
+            print(f'Found minimum size: {min_size}px')
+
+            metadata = self._resize_images(min_size)
+
+            with open(self.metadata_file_path, 'w') as fm:
+                json.dump(metadata, fm)
+
+    def load(self, force_download: bool = False, force_prepare: bool = False):
+        super().load(force_download, force_prepare)
+
+        with open(self.metadata_file_path) as f:
+            metadata = json.load(f)
+
+        self.dataset_shape = metadata['shape']
+        self.x = metadata['filenames']
+        self.y = metadata['labels']
+        self.data_length = len(self.y)
+
+        self.y = functional.one_hot(torch.tensor(self.y, dtype=torch.long))
+
+    def __getitem__(self, index):
+        x_path = str(Path(self.dataset_subdir_path, self.x[index]))
+
+        with np.load(x_path) as f:
+            x = torch.from_numpy(f)
+
+        return x, self.y[index]
+
+
+class DatasetMasksNumpyMmap(ImageFileStorage):
+    DATASET_DTYPE = 'float16'
+    DATASET_SUBDIR_NAME = 'numpy_mmap'
+    DATASET_FILE_NAME = 'data.npy'
     METADATA_FILE_NAME = 'metadata.json'
-    SUPPORTED_BPS = (8, 16, )
 
-    def __init__(self, color_spaces: Sequence):
-        super().__init__(color_spaces)
+    def __init__(self, root: Path, transform=None, target_transform=None):
+        super().__init__(root, transform, target_transform)
 
-    def __str__(self):
-        return f'{self.DATASET_SUBDIR_NAME}'
+    def _resize_images(self, size: Optional[int] = None):
+        item_count = self._count_images(size)
+        print(f'Item count: {item_count}')
+
+        dataset_shape = (item_count, 3, size, size)
+
+        self.dataset_file_path.parent.mkdir(exist_ok=True)
+
+        x = open_memmap(
+            str(self.dataset_file_path), mode='w+', dtype=self.DATASET_DTYPE, shape=dataset_shape
+        )
+        y = []
+
+        for idx, (label, image) in enumerate(self._iter_images(self.image_dir_path, size)):
+            file_name = Path(image.filename).name
+            print(f'{idx}/{item_count}: Processing {file_name}')
+
+            try:
+                image = adjust_image(image, size, size)
+            except OSError as e:
+                print(f'Failed reading image file: {file_name}, {e}. Deleting original file')
+                Path(image.filename).unlink(missing_ok=True)
+            else:
+                image = np.asarray(image) / 255.0
+                # Converting HxWxC to CxHxW
+                image = np.transpose(image, (2, 0, 1))
+                x[idx, :, :] = image[:, :]
+                # Decreasing by 1 due to indexes start from 1
+                y.append(int(label) - 1)
+
+        x.flush()
+
+        metadata = {
+            'shape': (len(y), 3, size, size),
+            'labels': y
+        }
+
+        return metadata
+
+    def _prepare(self, force: bool = True):
+        if force or not self.dataset_file_path.exists() or not self.metadata_file_path.exists():
+            print('Preparing dataset')
+            min_size = self._get_min_size(self.IMAGE_WIDTH)
+            print(f'Found minimum size: {min_size}px')
+
+            metadata = self._resize_images(min_size)
+
+            with open(self.metadata_file_path, 'w') as fm:
+                json.dump(metadata, fm)
+
+    def load(self, force_download: bool = False, force_prepare: bool = False):
+        super().load(force_download, force_prepare)
+
+        with open(self.metadata_file_path) as f:
+            metadata = json.load(f)
+
+        self.dataset_shape = metadata['shape']
+        self.data_length = self.dataset_shape[0]
+        self.y = metadata['labels']
+
+        self.x = open_memmap(
+            str(self.dataset_file_path), mode='r', dtype=self.DATASET_DTYPE, shape=self.dataset_shape
+        )
+        self.y = functional.one_hot(torch.tensor(self.y, dtype=torch.long))
+
+#    def __len__(self):
+#        return 10000
+
+    def __getitem__(self, index):
+        x = self.x[index]
+        x = np.array(x)
+        x = torch.from_numpy(x)
 
-    def _save_image(self, dst_path: Path, image: np.ndarray):
-        np.savez_compressed(dst_path, image)
-
-
-# class NumpyZipImageStorage(ImageFileStorage):
-#     DATASET_DTYPE = 'float16'
-#     DATASET_SUBDIR_NAME = 'numpy_zip_files'
-#     METADATA_FILE_NAME = 'metadata.json'
-#
-#     def _resize_images(self, size: Optional[int] = None):
-#         item_count = self._count_images(size)
-#         print(f'Item count: {item_count}')
-#
-#         self.dataset_subdir_path.mkdir(exist_ok=True)
-#
-#         x = []
-#         y = []
-#
-#         for idx, (label, image) in enumerate(self._iter_images(self.image_dir_path, size)):
-#             label = int(label) - 1
-#             file_name = Path(image.filename).name
-#             print(f'{idx}/{item_count}: Processing {file_name}')
-#
-#             try:
-#                 image = adjust_image(image, size, size)
-#             except OSError as e:
-#                 print(f'Failed reading image file: {file_name}, {e}. Deleting original file')
-#                 Path(image.filename).unlink(missing_ok=True)
-#             else:
-#                 image = np.asarray(image) / 255.0
-#                 # Converting HxWxC to CxHxW
-#                 image = np.transpose(image, (2, 0, 1))
-#                 file_name_base = file_name.split('.', maxsplit=1)[0]
-#                 label_dir_path = Path(self.dataset_subdir_path, str(label))
-#                 label_dir_path.mkdir(exist_ok=True)
-#                 out_file_path = Path(label_dir_path, f'{file_name_base}.npz')
-#                 np.savez_compressed(out_file_path, value=image)
-#                 x.append(f'{label}/{file_name_base}.npz')
-#                 y.append(label)
-#
-#         metadata = {
-#             'shape': (3, size, size),
-#             'filenames': x,
-#             'labels': y
-#         }
-#
-#         return metadata
-#
-#     def _prepare(self, force: bool = True):
-#         if force or not self.metadata_file_path.exists():
-#             print('Preparing dataset')
-#             min_size = self._get_min_size(self.IMAGE_WIDTH)
-#             print(f'Found minimum size: {min_size}px')
-#
-#             metadata = self._resize_images(min_size)
-#
-#             with open(self.metadata_file_path, 'w') as fm:
-#                 json.dump(metadata, fm)
-#
-#     def load(self, force_download: bool = False, force_prepare: bool = False):
-#         super().load(force_download, force_prepare)
-#
-#         with open(self.metadata_file_path) as f:
-#             metadata = json.load(f)
-#
-#         self.dataset_shape = metadata['shape']
-#         self.x = metadata['filenames']
-#         self.y = metadata['labels']
-#         self.data_length = len(self.y)
-#
-#         self.y = functional.one_hot(torch.tensor(self.y, dtype=torch.long))
-#
-#     def __getitem__(self, index):
-#         x_path = str(Path(self.dataset_subdir_path, self.x[index]))
-#
-#         with np.load(x_path) as f:
-#             x = torch.from_numpy(f)
-#
-#         return x, self.y[index]
-#
-#
-# class DatasetMasksNumpyMmap(ImageFileStorage):
-#     DATASET_DTYPE = 'float16'
-#     DATASET_SUBDIR_NAME = 'numpy_mmap'
-#     DATASET_FILE_NAME = 'data.npy'
-#     METADATA_FILE_NAME = 'metadata.json'
-#
-#     def __init__(self, root: Path, transform=None, target_transform=None):
-#         super().__init__(root, transform, target_transform)
-#
-#     def _resize_images(self, size: Optional[int] = None):
-#         item_count = self._count_images(size)
-#         print(f'Item count: {item_count}')
-#
-#         dataset_shape = (item_count, 3, size, size)
-#
-#         self.dataset_file_path.parent.mkdir(exist_ok=True)
-#
-#         x = open_memmap(
-#             str(self.dataset_file_path), mode='w+', dtype=self.DATASET_DTYPE, shape=dataset_shape
-#         )
-#         y = []
-#
-#         for idx, (label, image) in enumerate(self._iter_images(self.image_dir_path, size)):
-#             file_name = Path(image.filename).name
-#             print(f'{idx}/{item_count}: Processing {file_name}')
-#
-#             try:
-#                 image = adjust_image(image, size, size)
-#             except OSError as e:
-#                 print(f'Failed reading image file: {file_name}, {e}. Deleting original file')
-#                 Path(image.filename).unlink(missing_ok=True)
-#             else:
-#                 image = np.asarray(image) / 255.0
-#                 # Converting HxWxC to CxHxW
-#                 image = np.transpose(image, (2, 0, 1))
-#                 x[idx, :, :] = image[:, :]
-#                 # Decreasing by 1 due to indexes start from 1
-#                 y.append(int(label) - 1)
-#
-#         x.flush()
-#
-#         metadata = {
-#             'shape': (len(y), 3, size, size),
-#             'labels': y
-#         }
-#
-#         return metadata
-#
-#     def _prepare(self, force: bool = True):
-#         if force or not self.dataset_file_path.exists() or not self.metadata_file_path.exists():
-#             print('Preparing dataset')
-#             min_size = self._get_min_size(self.IMAGE_WIDTH)
-#             print(f'Found minimum size: {min_size}px')
-#
-#             metadata = self._resize_images(min_size)
-#
-#             with open(self.metadata_file_path, 'w') as fm:
-#                 json.dump(metadata, fm)
-#
-#     def load(self, force_download: bool = False, force_prepare: bool = False):
-#         super().load(force_download, force_prepare)
-#
-#         with open(self.metadata_file_path) as f:
-#             metadata = json.load(f)
-#
-#         self.dataset_shape = metadata['shape']
-#         self.data_length = self.dataset_shape[0]
-#         self.y = metadata['labels']
-#
-#         self.x = open_memmap(
-#             str(self.dataset_file_path), mode='r', dtype=self.DATASET_DTYPE, shape=self.dataset_shape
-#         )
-#         self.y = functional.one_hot(torch.tensor(self.y, dtype=torch.long))
-#
-# #    def __len__(self):
-# #        return 10000
-#
-#     def __getitem__(self, index):
-#         x = self.x[index]
-#         x = np.array(x)
-#         x = torch.from_numpy(x)
-#
-#         return x, self.y[index]
+        return x, self.y[index]
```

### Comparing `dataset-format-benchmark-0.0.12/src/dataset_format_benchmark.egg-info/SOURCES.txt` & `dataset-format-benchmark-0.0.8/src/dataset_format_benchmark.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .coveragerc
-.dockerignore
 .gitignore
 AUTHORS.rst
 CHANGELOG.rst
 Dockerfile
 LICENSE
 README.md
 README.rst
@@ -19,15 +18,14 @@
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
 docs/_static/.gitignore
 src/dataset_format_benchmark/__init__.py
 src/dataset_format_benchmark/__main__.py
-src/dataset_format_benchmark/matrices.py
 src/dataset_format_benchmark/runner.py
 src/dataset_format_benchmark.egg-info/PKG-INFO
 src/dataset_format_benchmark.egg-info/SOURCES.txt
 src/dataset_format_benchmark.egg-info/dependency_links.txt
 src/dataset_format_benchmark.egg-info/not-zip-safe
 src/dataset_format_benchmark.egg-info/requires.txt
 src/dataset_format_benchmark.egg-info/top_level.txt
```

