# Comparing `tmp/figaro-1.1.2.tar.gz` & `tmp/figaro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.1.2.tar", last modified: Sat Jul 15 13:49:39 2023, max compression
+gzip compressed data, was "figaro-1.2.0.tar", last modified: Thu Jul 20 14:26:07 2023, max compression
```

## Comparing `figaro-1.1.2.tar` & `figaro-1.2.0.tar`

### file list

```diff
@@ -1,77 +1,88 @@
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.822779 figaro-1.1.2/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.2/LICENSE
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 09:07:00.000000 figaro-1.1.2/MANIFEST.in
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-15 13:49:39.822307 figaro-1.1.2/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.2/README.md
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.782888 figaro-1.1.2/docs/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      142 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.coordinates.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.cosmology.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      159 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.credible_regions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.cumulative.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.decorators.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.diagnostic.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.exceptions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.likelihood.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.load.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.marginal.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      130 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.mixture.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.montecarlo.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      177 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.create_glade.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      160 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.entropy.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      182 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.gen_mock_data.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      207 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.hierarchical_inference.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      221 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.par_hierarchical_inference.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      212 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.par_probability_density.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      157 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.ppplot.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      198 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.probability_density.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      521 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.plot.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      150 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.plot_settings.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      545 2023-07-14 21:26:56.000000 figaro-1.1.2/docs/figaro.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.threeDvolume.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.transform.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      124 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.utils.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      443 2023-07-15 08:11:09.000000 figaro-1.1.2/docs/index.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       55 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/modules.rst
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.809949 figaro-1.1.2/figaro/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.2/figaro/__init__.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2465 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/coordinates.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000320 2023-07-15 09:07:35.000000 figaro-1.1.2/figaro/cosmology.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-15 09:06:46.000000 figaro-1.1.2/figaro/cosmology.pxd
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.1.2/figaro/cosmology.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7604 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/credible_regions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.2/figaro/cumulative.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.2/figaro/cumulative.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.2/figaro/decorators.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8492 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/diagnostic.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.2/figaro/exceptions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5262 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/likelihood.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26737 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/load.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5953 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/marginal.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41154 2023-07-15 08:11:25.000000 figaro-1.1.2/figaro/mixture.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2604 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/montecarlo.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.821567 figaro-1.1.2/figaro/pipelines/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.2/figaro/pipelines/create_glade.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.2/figaro/pipelines/entropy.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.2/figaro/pipelines/gen_mock_data.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.2/figaro/pipelines/hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.2/figaro/pipelines/par_hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.2/figaro/pipelines/par_probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.2/figaro/pipelines/ppplot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.2/figaro/pipelines/probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31875 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/plot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.2/figaro/plot_settings.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39731 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/threeDvolume.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2230 2023-07-14 19:38:56.000000 figaro-1.1.2/figaro/transform.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15174 2023-07-14 20:20:08.000000 figaro-1.1.2/figaro/utils.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.815727 figaro-1.1.2/figaro.egg-info/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    24290 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/entry_points.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      103 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/requires.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/top_level.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 13:47:26.000000 figaro-1.1.2/pyproject.toml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      102 2023-07-15 13:48:02.000000 figaro-1.1.2/requirements.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-15 13:49:39.822953 figaro-1.1.2/setup.cfg
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4092 2023-07-15 13:48:51.000000 figaro-1.1.2/setup.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.168753 figaro-1.2.0/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.2.0/LICENSE
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 09:07:00.000000 figaro-1.2.0/MANIFEST.in
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-20 14:26:07.168138 figaro-1.2.0/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.2.0/README.md
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.085645 figaro-1.2.0/docs/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       55 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/modules.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.104630 figaro-1.2.0/docs/source/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      429 2023-07-16 06:22:36.000000 figaro-1.2.0/docs/source/api.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      142 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.coordinates.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      159 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.decorators.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.exceptions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.likelihood.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.load.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.marginal.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      130 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.mixture.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.plot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      150 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.plot_settings.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      404 2023-07-16 06:21:48.000000 figaro-1.2.0/docs/source/figaro.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.threeDvolume.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.transform.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      124 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.utils.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.123449 figaro-1.2.0/docs/source/generated/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      306 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.coordinates.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      207 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      363 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      231 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      263 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      397 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      278 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.exceptions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      407 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.likelihood.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      267 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      211 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      225 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      201 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      357 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      140 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.plot_settings.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      332 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.threeDvolume.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      385 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      320 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      996 2023-07-16 06:43:04.000000 figaro-1.2.0/docs/source/index.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.151912 figaro-1.2.0/figaro/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.2.0/figaro/__init__.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2465 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/coordinates.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000320 2023-07-15 09:07:35.000000 figaro-1.2.0/figaro/cosmology.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-15 09:06:46.000000 figaro-1.2.0/figaro/cosmology.pxd
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.2.0/figaro/cosmology.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7604 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/credible_regions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.2.0/figaro/cumulative.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.2.0/figaro/cumulative.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.2.0/figaro/decorators.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8492 2023-07-19 18:35:03.000000 figaro-1.2.0/figaro/diagnostic.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.2.0/figaro/exceptions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5262 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/likelihood.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26408 2023-07-20 13:59:57.000000 figaro-1.2.0/figaro/load.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5953 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/marginal.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    40334 2023-07-20 14:22:33.000000 figaro-1.2.0/figaro/mixture.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2604 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/montecarlo.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.166823 figaro-1.2.0/figaro/pipelines/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.2.0/figaro/pipelines/create_glade.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.2.0/figaro/pipelines/entropy.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.2.0/figaro/pipelines/gen_mock_data.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.2.0/figaro/pipelines/hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.2.0/figaro/pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.2.0/figaro/pipelines/par_probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.2.0/figaro/pipelines/ppplot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.2.0/figaro/pipelines/probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    38113 2023-07-19 13:23:48.000000 figaro-1.2.0/figaro/plot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.2.0/figaro/plot_settings.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39731 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/threeDvolume.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2230 2023-07-14 19:38:56.000000 figaro-1.2.0/figaro/transform.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12606 2023-07-20 14:22:33.000000 figaro-1.2.0/figaro/utils.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.156752 figaro-1.2.0/figaro.egg-info/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    24809 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      115 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/requires.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/top_level.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 13:47:26.000000 figaro-1.2.0/pyproject.toml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      114 2023-07-16 06:52:54.000000 figaro-1.2.0/requirements.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-20 14:26:07.168925 figaro-1.2.0/setup.cfg
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4092 2023-07-20 14:25:34.000000 figaro-1.2.0/setup.py
```

### Comparing `figaro-1.1.2/LICENSE` & `figaro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/PKG-INFO` & `figaro-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.2
+Version: 1.2.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.1.2/README.md` & `figaro-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/coordinates.py` & `figaro-1.2.0/figaro/coordinates.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/cosmology.c` & `figaro-1.2.0/figaro/cosmology.c`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/cosmology.pxd` & `figaro-1.2.0/figaro/cosmology.pxd`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/cosmology.pyx` & `figaro-1.2.0/figaro/cosmology.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/credible_regions.py` & `figaro-1.2.0/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/cumulative.c` & `figaro-1.2.0/figaro/cumulative.c`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/cumulative.pyx` & `figaro-1.2.0/figaro/cumulative.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/decorators.py` & `figaro-1.2.0/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/diagnostic.py` & `figaro-1.2.0/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/exceptions.py` & `figaro-1.2.0/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/likelihood.py` & `figaro-1.2.0/figaro/likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/load.py` & `figaro-1.2.0/figaro/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,14 @@
         # Check that a list of parameters is passed
         if par is None:
             raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
         # Check that all the parametes are loadable
         if not np.all([p in GW_par.keys() for p in par]):
             wrong_pars = [p for p in par if not p in GW_par.keys()]
             raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
-        # Check if lal is installed
-        if not lal_flag:
-            raise FIGAROException("LAL is not installed. GW posterior samples cannot be loaded.")
         # If everything is ok, load the samples
         else:
             out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = (h, om, ol), rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
     
     if out is None:
         return out, name
     
@@ -194,17 +191,14 @@
             # Check that a list of parameters is passed
             if par is None:
                 raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
             # Check that all the parametes are loadable
             if not np.all([p in GW_par.keys() for p in par]):
                 wrong_pars = [p for p in par if not p in GW_par.keys()]
                 raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
-            # Check if lal is installed
-            if not lal_flag:
-                raise FIGAROException("LAL is not installed. GW posterior samples cannot be loaded.")
             # If everything is ok, load the samples
             else:
                 out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = (h, om, ol), rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold)
                 if out is not None:
                     if out.shape[-1] == len(par):
                         events.append(out)
                     elif 'snr' in par:
@@ -506,15 +500,15 @@
     """
     Loads a list of figaro.mixture instances from path.
     If the requested file extension (pkl or json) is not available, it tries loading the other.
 
     Arguments:
         str or Path path: path with draws (file or folder)
 
-    Returns
+    Returns:
         list: figaro.mixture object instances
     """
     path = Path(path)
     if path.is_file():
         return _load_density_file(path)
     else:
         return [_load_density_file(file) for file in path.glob('*.[jp][sk][ol]*') if not file.stem == 'posteriors_single_event']
```

### Comparing `figaro-1.1.2/figaro/marginal.py` & `figaro-1.2.0/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/mixture.py` & `figaro-1.2.0/figaro/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,94 +101,84 @@
             logP_old = _numba_gammaln(a_old) - _numba_gammaln(a_old + n) + K * np.log(a_old) - 1./a_old
             logP_new = _numba_gammaln(a_new) - _numba_gammaln(a_new + n) + K * np.log(a_new) - 1./a_new
             if logP_new - logP_old > np.log(np.random.random()):
                 a_old = a_new
     return a_old
 
 @njit
-def _compute_t_pars(k, mu, nu, L, mean, S, N, dim):
+def _compute_t_pars(nu, L, mean, S, N, dim):
     """
     Compute parameters for student-t distribution.
     
     Arguments:
-        double k:        Normal std parameter (for NIW)
-        np.ndarray mu:   Normal mean parameter (for NIW)
-        int nu:          Inverse-Wishart df parameter (for NIW)
-        np.ndarray L:    Inverse-Wishart scale matrix (for NIW)
+        int nu:          df parameter (for IG/IW)
+        np.ndarray L:    scale matrix (for IG/IW)
         np.ndarray mean: samples mean
         np.ndarray S:    samples covariance
         int N:           number of samples
         int dim:         number of dimensions
     
     Returns:
         int:        degrees of fredom for student-t
         np.ndarray: scale matrix for student-t
         np.ndarray: mean for student-t
     """
     # Update hyperparameters
-    k_n, mu_n, nu_n, L_n = _compute_hyperpars(k, mu, nu, L, mean, S, N)
+    nu_n, L_n = _compute_hyperpars(nu, L, mean, S, N)
     # Update t-parameters
     t_df    = nu_n - dim + 1
-    t_shape = L_n*(k_n+1)/(k_n*t_df)
-    return t_df, t_shape, mu_n
+    t_shape = L_n/t_df
+    return t_df, t_shape, mean
 
 @njit
-def _compute_hyperpars(k, mu, nu, L, mean, S, N):
+def _compute_hyperpars(nu, L, mean, S, N):
     """
     Update hyperparameters for Normal Inverse Gamma/Wishart (NIG/NIW).
     See https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf
     
     Arguments:
-        double k:        Normal std parameter (for NIG/NIW)
-        np.ndarray mu:   Normal mean parameter (for NIG/NIW)
-        int nu:          Gamma df parameter (for NIG/NIW)
-        np.ndarray L:    Gamma scale matrix (for NIG/NIW)
+        int nu:          df parameter (for IG/IW)
+        np.ndarray L:    scale matrix (for IG/IW)
         np.ndarray mean: samples mean
         np.ndarray S:    samples covariance
         int N:           number of samples
     
     Returns:
-        double:     updated Normal std parameter (for NIG/NIW)
-        np.ndarray: updated Normal mean parameter (for NIG/NIW)
-        int:        updated Gamma df parameter (for NIG/NIW)
-        np.ndarray: updated Gamma scale matrix (for NIG/NIW)
+        int:        updated df parameter (for IG/IW)
+        np.ndarray: updated scale matrix (for IG/IW)
     """
-    k_n  = k + N
-    mu_n = (mu*k + N*mean)/k_n
     nu_n = nu + N
-    L_n  = L + S + k*N*((mean - mu).T@(mean - mu))/k_n
-    return k_n, mu_n, nu_n, L_n
+    L_n  = L + S
+    return nu_n, L_n
 
 @njit
-def _compute_component_suffstats(x, mean, S, N, p_mu, p_k, p_nu, p_L):
+def _compute_component_suffstats(x, mean, S, N, p_nu, p_L):
     """
     Update mean, covariance, number of samples and maximum a posteriori for mean and covariance.
     
     Arguments:
         np.ndarray x:    sample to add
         np.ndarray mean: mean of samples already in the cluster
         np.ndarray cov:  covariance of samples already in the cluster
         int N:           number of samples already in the cluster
-        np.ndarray p_mu: NIG Normal mean parameter
-        double p_k:      NIG Normal std parameter
-        int p_nu:        NIG Gamma df parameter
-        np.ndarray p_L:  NIG Gamma scale matrix
+        int p_nu:        IG/IW df parameter
+        np.ndarray p_L:  IG/IW scale matrix
     
     Returns:
         np.ndarray: updated mean
         np.ndarray: updated covariance
         int:        updated number of samples
         np.ndarray: mean (maximum a posteriori)
         np.ndarray: covariance (maximum a posteriori)
     """
     new_mean  = (mean*N+x)/(N+1)
     new_S     = (S + N*mean.T@mean + x.T@x) - new_mean.T@new_mean*(N+1)
     new_N     = N+1
-    new_mu    = ((p_mu*p_k + new_N*new_mean)/(p_k + new_N))[0]
-    new_sigma = (p_L + new_S + p_k*new_N*((new_mean - p_mu).T@(new_mean - p_mu))/(p_k + new_N))/(p_nu + new_N - x.shape[-1] - 1)
+    new_mu    = new_mean
+    new_sigma = (p_L + new_S)/(p_nu + new_N - x.shape[-1] - 1)
     
     return new_mean, new_S, new_N, new_mu, new_sigma
 
 #-------------------#
 # Auxiliary classes #
 #-------------------#
 
@@ -202,19 +192,17 @@
         np.ndarray mu:   Normal mean parameter
         int nu:          Wishart df parameter
         np.ndarray L:    Wishart scale matrix
     
     Returns:
         prior: instance of prior class
     """
-    def __init__(self, k, L, nu, mu):
-        self.k   = k
-        self.nu  = np.max([nu, mu.shape[-1]+2])
-        self.L   = L*(self.nu-mu.shape[-1]-1)
-        self.mu  = mu
+    def __init__(self, L, nu):
+        self.nu  = np.max([nu, L.shape[-1]+2])
+        self.L   = L*(self.nu-L.shape[-1]-1)
 
 class _component:
     """
     Class to store the relevant informations for each component in the mixture.
     
     Arguments:
         np.ndarray x: sample added to the new component
@@ -223,15 +211,15 @@
     Returns:
         component: instance of component class
     """
     def __init__(self, x, prior):
         self.N     = 1
         self.mean  = x
         self.S     = np.identity(x.shape[-1])*0.
-        self.mu    = np.atleast_2d((prior.mu*prior.k + self.N*self.mean)/(prior.k + self.N)).astype(np.float64)[0]
+        self.mu    = np.atleast_2d(self.mean).astype(np.float64)[0]
         self.sigma = np.identity(x.shape[-1]).astype(np.float64)*prior.L/(prior.nu - x.shape[-1] - 1)
 
 class _component_h:
     """
     Class to store the relevant informations for each component in the mixture.
     To be used in hierarchical inference.
     
@@ -741,14 +729,15 @@
     def __init__(self, bounds,
                        prior_pars = None,
                        alpha0     = 1.,
                        probit     = True,
                        ):
         self.probit = probit
         self.bounds = np.atleast_2d(bounds)
+        self.log_V  = np.sum(np.log(np.diff(self.bounds, axis = -1)))
         self.dim    = len(self.bounds)
         if prior_pars is not None:
             self.prior = _prior(*prior_pars)
         else:
             self.prior = _prior(*get_priors(bounds = self.bounds, probit = self.probit))
         self.alpha      = alpha0
         self.alpha_0    = alpha0
@@ -786,15 +775,15 @@
         Arguments:
             np.ndarray x: sample
             component ss: component to update
         
         Returns:
             component: updated component
         """
-        new_mean, new_S, new_N, new_mu, new_sigma = _compute_component_suffstats(x, ss.mean, ss.S, ss.N, self.prior.mu, self.prior.k, self.prior.nu, self.prior.L)
+        new_mean, new_S, new_N, new_mu, new_sigma = _compute_component_suffstats(x, ss.mean, ss.S, ss.N, self.prior.nu, self.prior.L)
         ss.mean  = new_mean
         ss.S     = new_S
         ss.N     = new_N
         ss.mu    = new_mu
         ss.sigma = new_sigma
         return ss
     
@@ -806,17 +795,16 @@
             np.ndarray x: sample
             component ss: component to update
         
         Returns:
             double: log Likelihood
         """
         if ss is None:
-            ss = _component(np.zeros(self.dim), prior = self.prior)
-            ss.N = 0.
-        t_df, t_shape, mu_n = _compute_t_pars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
+            return -self.log_V
+        t_df, t_shape, mu_n = _compute_t_pars(self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
         return _student_t(df = t_df, t = x, mu = mu_n, sigma = t_shape, dim = self.dim)
 
     def _cluster_assignment_distribution(self, x):
         """
         Compute the marginal distribution of cluster assignment for each cluster.
         
         Arguments:
@@ -897,17 +885,20 @@
             mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
         means     = np.zeros((self.n_cl, self.dim))
         variances = np.zeros((self.n_cl, self.dim, self.dim))
         for i, ss in enumerate(self.mixture):
-            k_n, mu_n, nu_n, L_n = _compute_hyperpars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
+            nu_n, L_n = _compute_hyperpars(self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
             variances[i] = invwishart(df = nu_n, scale = L_n).rvs()
-            means[i]     = mn(mean = mu_n[0], cov = variances[i]/k_n, allow_singular = True).rvs()
+            if ss.N == 1:
+                means[i] = mn(mean = ss.mean[0], cov = L_n/(nu_n - self.dim + 1), allow_singular = True).rvs()
+            else:
+                means[i] = mn(mean = ss.mean[0], cov = ss.S/ss.N**2, allow_singular = True).rvs()
         w = dirichlet(self.w*self.n_pts+self.alpha/self.n_cl).rvs()[0]
         return mixture(means, variances, w, self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
 
     # Methods to overwrite density methods
     def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
```

### Comparing `figaro-1.1.2/figaro/montecarlo.py` & `figaro-1.2.0/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/create_glade.py` & `figaro-1.2.0/figaro/pipelines/create_glade.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/entropy.py` & `figaro-1.2.0/figaro/pipelines/entropy.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/gen_mock_data.py` & `figaro-1.2.0/figaro/pipelines/gen_mock_data.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/hierarchical_inference.py` & `figaro-1.2.0/figaro/pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/par_hierarchical_inference.py` & `figaro-1.2.0/figaro/pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/par_probability_density.py` & `figaro-1.2.0/figaro/pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/ppplot.py` & `figaro-1.2.0/figaro/pipelines/ppplot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/pipelines/probability_density.py` & `figaro-1.2.0/figaro/pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/plot.py` & `figaro-1.2.0/figaro/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import warnings
 
 from pathlib import Path
 from scipy.stats import beta
 from corner import corner
 
 import matplotlib.pyplot as plt
-from matplotlib import axes
+from matplotlib import axes, colormaps
 from matplotlib.projections import projection_registry
-import matplotlib.patches as mpatches
 from matplotlib.lines import Line2D
-from matplotlib import rcParams
+from matplotlib.colors import Normalize
+from matplotlib.gridspec import GridSpec
 
 from figaro import plot_settings
 from figaro.marginal import marginalise
 from figaro.credible_regions import ConfidenceArea
 from figaro.utils import recursive_grid
 
 # Telling python to ignore empty legend warning from matplotlib
@@ -314,14 +314,17 @@
         bool show:              whether to show the plot during the run or not
         bool subfolder:         whether to save in a dedicated subfolder
         int n_pts:              number of grid points (same for each dimension)
         iterable true_value:    true value to plot
         iterable levels:        credible levels to plot
         bool scatter_points:    scatter samples on 2d plots
         str median_label:       label to assign to the reconstruction
+    
+    Returns:
+        matplotlib.figure.Figure: figure with the plot
     """
     
     dim = draws[0].dim
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
@@ -739,7 +742,156 @@
     ax.set_xlabel('$P$')
     ax.set_ylabel('$\mathrm{Fraction\ of\ events\ within\ }CR_P$')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, '{0}_ppplot.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
+
+def joyplot(draws, x_values, y_values, credible_regions = False, fill = True, solid = False, overlap = 1., xlabel = None, ylabel = None, xunit = None, yunit = None, colormap = 'coolwarm', out_folder = '.', name = 'joyplot', subfolder = False, show = False, save = True, joy = False):
+    """
+    Make a joyplot (also known as ridgeline plot) of a set of distributions.
+    Heavily inspired by leotac's JoyPy (https://github.com/leotac/joypy).
+    
+    Arguments:
+        np.ndarray draws:       (n_y, n_x) or (n_y, n_draws, n_x) array containing the distributions to plot
+        np.ndarray x_values:    x values at which the distributions are evaluated
+        np.ndarray y_values:    y values corresponding to the different distributions
+        bool credible_regions:  whether to plot credible regions or not
+        bool fill:              whether to fill the space below the distribution or not (ignored if credible_regions is True)
+        bool solid:             wheter to fill with transparent or solid colour
+        float overlap:          space between different plots
+        str xlabel:             x axis label (LaTeX style)
+        str ylabel:             colorbar label (LaTeX style)
+        str xunit:              x axis units (LaTeX style) - default: no units
+        str yunit:              colorbar units (LaTeX style) - default: no units
+        str colormap:           a valid matplotlib colormap name
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        bool subfolder:         whether to save the plots in different subfolders (for multiple events)
+        bool save:              whether to save the plots or not
+        bool show:              whether to show the plots during the run or not
+        bool joy:               format the plot to look like the cover of Joy Division's "Unknown Pleasures"
+        
+    Returns:
+        matplotlib.figure.Figure: figure with the plot
+    """
+    # Labels
+    if xlabel is None:
+        xlabel = '$x$'
+    else:
+        xlabel = '${0}$'.format(xlabel)
+    if xunit is not None:
+        xlabel = xlabel[:-1]+'\ [{0}]$'.format(xunit)
+    if ylabel is None:
+        ylabel = '$y$'
+    else:
+        ylabel = '${0}$'.format(ylabel)
+    if yunit is not None:
+        ylabel = ylabel[:-1]+'\ [{0}]$'.format(yunit)
+    
+    # Check that we have as many y values as different draws evaluations
+    if not len(y_values) == np.shape(draws)[0]:
+        raise ValueError("y_values and draws must have the same length")
+
+    color = iter(colormaps[colormap](np.linspace(1, 0, len(y_values))))
+    cmappable = plt.cm.ScalarMappable(norm=Normalize(np.min(y_values),np.max(y_values)), cmap=colormap)
+    num_axes = len(y_values)
+
+    # Each plot will have its own axis
+    fig = plt.figure()
+    if joy:
+        fig.patch.set_facecolor('k')
+    gs = GridSpec(len(y_values), 17, figure = fig)
+    _axes = []
+    [_axes.append(fig.add_subplot(gs[i, :-1])) for i in range(len(y_values))]
+    if not joy:
+        _axes.append(fig.add_subplot(gs[:, -1]))
+        # Global colorbar
+        cbar    = fig.colorbar(cmappable, cax = _axes[-1])
+        cbar.set_label(ylabel)
+    if joy:
+        [ax.set_facecolor('k') for ax in _axes]
+    for i, dd in enumerate(draws[::-1]):
+        ax = _axes[i]
+        if not joy:
+            c = next(color)
+        else:
+            c = 'w'
+        percentiles = [50, 16, 84]
+        p = {}
+        if len(np.shape(draws)) == 3:
+            for perc in percentiles:
+                p[perc] = np.percentile(dd, perc, axis = 0)
+            if credible_regions and not joy:
+                ax.fill_between(x_values, p[95], p[5], color = c, alpha = 0.25)
+                ax.fill_between(x_values, p[84], p[16], color = c, alpha = 0.25)
+        else:
+            p[50] = dd
+        if fill and not credible_regions:
+            if solid:
+                alpha = 1
+            else:
+                alpha = 0.25
+            if not joy:
+                ax.fill_between(x_values, p[50], np.zeros(len(x_values)), color = c, alpha = alpha)
+            else:
+                ax.fill_between(x_values, p[50], np.zeros(len(x_values)), color = 'k', alpha = 1)
+        ax.plot(x_values, p[50], clip_on = True, c = c)
+
+        # Setup the current axis: transparency, labels, spines.
+        ax.yaxis.grid(False)
+        ax.patch.set_alpha(0)
+        ax.tick_params(axis='both', which='both', length=0, pad=10)
+        ax.xaxis.set_visible(False)
+        ax.yaxis.set_visible(False)
+        ax.set_frame_on(False)
+
+    # Final adjustments
+    # Compute a final axis, used to apply global settings
+    last_axis = fig.add_subplot(gs[:, :-1])
+    if joy:
+        last_axis.set_facecolor('k')
+
+    for side in ['top', 'bottom', 'left', 'right']:
+        last_axis.spines[side].set_visible(False)
+
+    # This looks hacky, but all the axes share the x-axis,
+    # so they have the same lims and ticks
+    last_axis.set_xlim(_axes[0].get_xlim())
+    last_axis.set_xticks(np.array(_axes[0].get_xticks()[1:-1]))
+    for t in last_axis.get_xticklabels():
+        if not joy:
+            t.set_visible(True)
+        else:
+            t.set_visible(False)
+    else:
+        if not joy:
+            last_axis.xaxis.set_visible(True)
+        else:
+            last_axis.xaxis.set_visible(False)
+    last_axis.yaxis.set_visible(False)
+    last_axis.grid(False)
+
+    # Last axis on the back
+    last_axis.zorder = min(a.zorder for a in _axes) - 1
+    _axes = list(_axes) + [last_axis]
+    last_axis.set_xlabel(xlabel)
+
+    # The magic overlap happens here.
+    h_pad = 5 + (-5*(1+overlap))
+    fig.tight_layout(h_pad=h_pad)
+
+    if show:
+        plt.show()
+    if save:
+        if not subfolder:
+            fig.savefig(Path(out_folder, '{0}.pdf'.format(name)), bbox_inches = 'tight')
+        else:
+            if not Path(out_folder, 'density').exists():
+                try:
+                    Path(out_folder, 'density').mkdir()
+                except FileExistsError:
+                    pass
+            fig.savefig(Path(out_folder, 'density', '{0}.pdf'.format(name)), bbox_inches = 'tight')
+    plt.close()
+    return fig
```

### Comparing `figaro-1.1.2/figaro/plot_settings.py` & `figaro-1.2.0/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/threeDvolume.py` & `figaro-1.2.0/figaro/threeDvolume.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/transform.py` & `figaro-1.2.0/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.2/figaro/utils.py` & `figaro-1.2.0/figaro/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -78,37 +78,33 @@
         probs = f(pts)*selfunc(pts)
         h     = np.random.uniform(0, top, size = n_draws)
         samples.extend(pts[np.where(h < probs)])
     return np.array(samples).flatten()[:n_draws]
 
 def get_priors(bounds, samples = None, mean = None, std = None, cov = None, df = None, k = None, a = None, scale = None, probit = True, hierarchical = False):
     """
-    This method takes the prior parameters for the Normal-Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
+    This method takes the prior parameters for the Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
 
-    Four parameters are returned:
+    Two parameters are returned:
         * df, is the number of degrees of freedom for the Inverse Wishart distribution,. It must be greater than D+1. If this parameter is None or does not satisfy the condition df > D+1, the default value D+2 is used;
-        * k is the scale parameter for the multivariate Normal distribution. Suggested values are  k <~ 1e-1. If None, the default value 1e-2 is used.
-        * mu is the mean of the multivariate Normal distribution. It can be either estimated from the available samples or passed directly as a 1D array with length D (the keyword argument mean overrides the samples). If None, the default value 0 (corresponding to the parameter space center) is used.
         * L is the expected value for the Inverse Wishart distribution. This parameter can be either (in descending priority order):
             * passed as 2D array with shape (D,D), the covariance matrix - keyword cov;
             * passed as 1D array with shape (D,) or double: vector of standard deviations (if double, it assumes that the same std has to be used for all dimensions) - keyword std;
             * estimated from samples - keyword samples.
        
-    The order in which they are returned is (k,L,df,mu).
+    The order in which they are returned is (L,df).
     
     Arguments:
         np.ndarray bounds:              boundaries for probit transformation
         np.ndarray samples:             2D [DPGMM] or 3D [(H)DPGMM] array with samples
-        double or np.ndarray mean:      mean [DPGMM]
         double or np.ndarray std:       expected standard deviation (if double, the same std is used for all dimensions, if np.ndarray must match the number of dimensions) [DPGMM and (H)DPGMM]
         np.ndarray cov:                 covariance matrix [DPGMM]
-        int df:                         degrees of freedom for Inverse Wishart distribution [DPGMM]
-        double k:                       scale parameter for Normal distribution [DPGMM]
+        int df:                         degrees of freedom for Inverse Gamma/Inverse Wishart distribution [DPGMM]
         double a:                       shape parameter for the Inverse Gamma distribution [(H)DPGMM]
-        double scale:                   fraction of samples std [DPGMM]
+        double scale:                   fraction of samples std [DPGMM and (H)DPGMM]
         bool probit:                    whether the probit transformation will be applied or not
         bool hierarchical:              returns the prior pars for (H)DPGMM rather than for DPGMM
         
     Returns:
         tuple: prior parameters ordered as in (H)/DPGMM
     """
     bounds = np.atleast_2d(bounds)
@@ -151,76 +147,32 @@
         # DF
         if df is not None and df > dim+2:
             df_out = df
         else:
             df_out = dim+2
             
         draw_flag = False
-        # Mu
-        if mean is not None:
-            mean = np.atleast_1d(mean)
-            if not np.prod(bounds[:,0] < mean) & np.prod(mean < bounds[:,1]):
-                raise ValueError("Mean is outside of the given bounds")
-            if probit:
-                mu_out = transform_to_probit(mean, bounds)
-            else:
-                mu_out = mean
-        elif samples is not None:
-            if probit:
-                mu_out = np.atleast_1d(np.median(probit_samples, axis = 0))
-            else:
-                mu_out = np.atleast_1d(np.median(samples, axis = 0))
-        else:
-            if probit:
-                mu_out = np.zeros(dim)
-            else:
-                mu_out = np.atleast_1d(np.mean(bounds, axis = 1))
         # L
         if cov is not None:
             L_out = cov
-            if probit:
-                draw_flag = True
         elif std is not None:
-            if probit:
-                L_out = np.identity(dim)*np.minimum(np.abs(mu_out - transform_to_probit((transform_from_probit(mu_out, bounds) + std), bounds)), np.abs(mu_out - transform_to_probit((transform_from_probit(mu_out, bounds) - std), bounds)))**2
-            else:
-                L_out = np.identity(dim)*std**2
+            L_out = np.identity(dim)*std**2
         elif samples is not None:
             if probit:
                 cov_samples = np.atleast_2d(np.cov(probit_samples.T))
             else:
                 cov_samples = np.atleast_2d(np.cov(samples.T))
             L_out = np.identity(dim)*np.diag(cov_samples/scale**2)
         else:
             if probit:
                 sigma = transform_to_probit(np.atleast_2d(np.mean(bounds, axis = -1)+np.diff(bounds, axis = -1).flatten()/scale), bounds)[0]
                 L_out = np.identity(dim)*sigma**2
             else:
                 L_out = np.identity(dim)*(np.diff(bounds, axis = -1).flatten()/scale)**2
-        if draw_flag:
-            ss = mn(np.mean(bounds, axis = -1), L_out, allow_singular = True).rvs(3000)
-            if dim == 1:
-                ss = np.atleast_2d(ss).T
-            # Keeping only samples within bounds
-            ss = ss[np.where((np.prod(bounds[:,0] < ss, axis = 1) & np.prod(ss < bounds[:,1], axis = 1)))]
-            probit_ss = transform_to_probit(ss, bounds)
-            L_out = np.identity(dim)*np.diag(np.atleast_2d(np.cov(probit_ss.T)))
-        # k
-        if k is not None:
-            k_out = k
-        else:
-            if samples is not None:
-                if probit:
-                    cov_samples = np.atleast_2d(np.cov(probit_samples.T))
-                else:
-                    cov_samples = np.atleast_2d(np.cov(samples.T))
-                k_out = np.min(np.diag(L_out)/np.diag(cov_samples))
-            else:
-                k_out = 1./(scale)
-        return (k_out, L_out, df_out, mu_out)
+        return (L_out, df_out)
 
 def rvs_median(draws, size = 1):
     """
     Generates samples from median distribution of a set of draws.
     
     Arguments:
         iterable draws: container for mixture instances
```

### Comparing `figaro-1.1.2/figaro.egg-info/PKG-INFO` & `figaro-1.2.0/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.2
+Version: 1.2.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.1.2/figaro.egg-info/SOURCES.txt` & `figaro-1.2.0/figaro.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -543,43 +543,52 @@
 /opt/local/include/lal/ZPGFilter.h
 /opt/local/include/lal/bayestar_distance.h
 /opt/local/include/lal/bayestar_moc.h
 /opt/local/include/lal/bayestar_sky_map.h
 /opt/local/include/lal/cs_cosmo.h
 /opt/local/include/lal/cs_lambda_cosmo.h
 /opt/local/include/lal/cubic_interp.h
-docs/figaro.coordinates.rst
-docs/figaro.cosmology.rst
-docs/figaro.credible_regions.rst
-docs/figaro.cumulative.rst
-docs/figaro.decorators.rst
-docs/figaro.diagnostic.rst
-docs/figaro.exceptions.rst
-docs/figaro.likelihood.rst
-docs/figaro.load.rst
-docs/figaro.marginal.rst
-docs/figaro.mixture.rst
-docs/figaro.montecarlo.rst
-docs/figaro.pipelines.create_glade.rst
-docs/figaro.pipelines.entropy.rst
-docs/figaro.pipelines.gen_mock_data.rst
-docs/figaro.pipelines.hierarchical_inference.rst
-docs/figaro.pipelines.par_hierarchical_inference.rst
-docs/figaro.pipelines.par_probability_density.rst
-docs/figaro.pipelines.ppplot.rst
-docs/figaro.pipelines.probability_density.rst
-docs/figaro.pipelines.rst
-docs/figaro.plot.rst
-docs/figaro.plot_settings.rst
-docs/figaro.rst
-docs/figaro.threeDvolume.rst
-docs/figaro.transform.rst
-docs/figaro.utils.rst
-docs/index.rst
 docs/modules.rst
+docs/source/api.rst
+docs/source/figaro.coordinates.rst
+docs/source/figaro.cosmology.rst
+docs/source/figaro.credible_regions.rst
+docs/source/figaro.cumulative.rst
+docs/source/figaro.decorators.rst
+docs/source/figaro.diagnostic.rst
+docs/source/figaro.exceptions.rst
+docs/source/figaro.likelihood.rst
+docs/source/figaro.load.rst
+docs/source/figaro.marginal.rst
+docs/source/figaro.mixture.rst
+docs/source/figaro.montecarlo.rst
+docs/source/figaro.plot.rst
+docs/source/figaro.plot_settings.rst
+docs/source/figaro.rst
+docs/source/figaro.threeDvolume.rst
+docs/source/figaro.transform.rst
+docs/source/figaro.utils.rst
+docs/source/index.rst
+docs/source/generated/figaro.coordinates.rst
+docs/source/generated/figaro.cosmology.rst
+docs/source/generated/figaro.credible_regions.rst
+docs/source/generated/figaro.cumulative.rst
+docs/source/generated/figaro.decorators.rst
+docs/source/generated/figaro.diagnostic.rst
+docs/source/generated/figaro.exceptions.rst
+docs/source/generated/figaro.likelihood.rst
+docs/source/generated/figaro.load.rst
+docs/source/generated/figaro.marginal.rst
+docs/source/generated/figaro.mixture.rst
+docs/source/generated/figaro.montecarlo.rst
+docs/source/generated/figaro.plot.rst
+docs/source/generated/figaro.plot_settings.rst
+docs/source/generated/figaro.threeDvolume.rst
+docs/source/generated/figaro.transform.rst
+docs/source/generated/figaro.utils.rst
 figaro/__init__.py
 figaro/coordinates.py
 figaro/cosmology.c
 figaro/cosmology.pxd
 figaro/cosmology.pyx
 figaro/credible_regions.py
 figaro/cumulative.c
```

### Comparing `figaro-1.1.2/setup.py` & `figaro-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     include_dirs = ['figaro', numpy.get_include()],
     setup_requires=['numpy', 'cython'],
     package_data={"": ['*.c', '*.pyx', '*.pxd']},
     ext_modules=ext_modules,
     entry_points = {
         'console_scripts': scripts,
         },
-    version='1.1.2',
+    version='1.2.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     cmdclass = {
             "build_ext": build_ext
             }
     )
```

