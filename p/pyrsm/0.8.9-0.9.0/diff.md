# Comparing `tmp/pyrsm-0.8.9.tar.gz` & `tmp/pyrsm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.9.tar", last modified: Tue Jul 18 20:36:37 2023, max compression
+gzip compressed data, was "pyrsm-0.9.0.tar", last modified: Thu Jul 20 09:01:14 2023, max compression
```

## Comparing `pyrsm-0.8.9.tar` & `pyrsm-0.9.0.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.211748 pyrsm-0.8.9/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.9/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.8.9/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-18 20:36:37.211828 pyrsm-0.8.9/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.9/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.9/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.183797 pyrsm-0.8.9/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-18 20:35:29.000000 pyrsm-0.8.9/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.185945 pyrsm-0.8.9/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.8.9/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.9/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8603 2023-07-16 18:57:36.000000 pyrsm-0.8.9/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.9/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.9/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.9/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.9/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     3771 2023-07-18 20:34:24.000000 pyrsm-0.8.9/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)    60884 2023-07-18 20:31:46.000000 pyrsm-0.8.9/pyrsm/basics/probability_calculator_functions.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.9/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.9/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.9/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.9/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.186162 pyrsm-0.8.9/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.9/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.188817 pyrsm-0.8.9/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.191452 pyrsm-0.8.9/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.191897 pyrsm-0.8.9/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.199981 pyrsm-0.8.9/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.9/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.9/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ratings_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.8.9/pyrsm/data/model/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.8.9/pyrsm/data/model/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.206963 pyrsm-0.8.9/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.9/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9375 2023-07-16 14:05:24.000000 pyrsm-0.8.9/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-16 14:04:41.000000 pyrsm-0.8.9/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.9/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.9/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.208649 pyrsm-0.8.9/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.9/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9504 2023-07-16 19:29:31.000000 pyrsm-0.8.9/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5566 2023-07-16 19:32:27.000000 pyrsm-0.8.9/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6572 2023-07-16 14:22:47.000000 pyrsm-0.8.9/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5163 2023-07-16 14:13:07.000000 pyrsm-0.8.9/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    11194 2023-07-16 19:20:46.000000 pyrsm-0.8.9/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.9/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.9/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.9/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.209192 pyrsm-0.8.9/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.9/pyrsm/radiant/www/.DS_Store
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.209989 pyrsm-0.8.9/pyrsm/radiant/www/imgs/
--rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-nc-sa.png
--rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-sa.png
--rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/icon.png
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.210807 pyrsm-0.8.9/pyrsm/radiant/www/js/
--rw-r--r--   0 root         (0) staff       (20)      343 2023-07-14 07:45:06.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/radiantUI.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/screenshot.js
--rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.9/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9391 2023-07-16 14:02:08.000000 pyrsm-0.8.9/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.9/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.9/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.9/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.184442 pyrsm-0.8.9/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3982 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      242 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-18 20:36:37.212166 pyrsm-0.8.9/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.211639 pyrsm-0.8.9/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.9/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.9/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.9/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.9/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.9/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.9/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.9/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.150578 pyrsm-0.9.0/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-20 09:01:14.150650 pyrsm-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.9.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.9.0/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.119885 pyrsm-0.9.0/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-20 08:59:54.000000 pyrsm-0.9.0/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.124818 pyrsm-0.9.0/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.9.0/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.9.0/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8835 2023-07-20 06:02:23.000000 pyrsm-0.9.0/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.9.0/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.9.0/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9602 2023-07-20 08:21:43.000000 pyrsm-0.9.0/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6674 2023-07-20 08:58:12.000000 pyrsm-0.9.0/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)    10022 2023-07-20 07:13:44.000000 pyrsm-0.9.0/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)    46422 2023-07-20 05:21:13.000000 pyrsm-0.9.0/pyrsm/basics/probability_calculator_functions.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.9.0/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.9.0/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.9.0/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.9.0/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.125175 pyrsm-0.9.0/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.9.0/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.127656 pyrsm-0.9.0/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.131104 pyrsm-0.9.0/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.131745 pyrsm-0.9.0/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.137967 pyrsm-0.9.0/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.9.0/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.9.0/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/model/ratings_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.9.0/pyrsm/data/model/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.9.0/pyrsm/data/model/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.142105 pyrsm-0.9.0/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.9.0/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9453 2023-07-20 05:17:59.000000 pyrsm-0.9.0/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25723 2023-07-20 05:15:29.000000 pyrsm-0.9.0/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.9.0/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.9.0/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.9.0/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.145338 pyrsm-0.9.0/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      191 2023-07-20 02:17:33.000000 pyrsm-0.9.0/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9915 2023-07-20 06:02:58.000000 pyrsm-0.9.0/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5502 2023-07-20 07:39:34.000000 pyrsm-0.9.0/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     5275 2023-07-20 08:58:55.000000 pyrsm-0.9.0/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5358 2023-07-20 05:05:48.000000 pyrsm-0.9.0/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    10973 2023-07-20 01:36:07.000000 pyrsm-0.9.0/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)    11336 2023-07-20 06:51:33.000000 pyrsm-0.9.0/pyrsm/radiant/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     4885 2023-07-20 04:10:20.000000 pyrsm-0.9.0/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5545 2023-07-20 05:05:48.000000 pyrsm-0.9.0/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    20121 2023-07-20 07:28:01.000000 pyrsm-0.9.0/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.145983 pyrsm-0.9.0/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.9.0/pyrsm/radiant/www/.DS_Store
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.147144 pyrsm-0.9.0/pyrsm/radiant/www/imgs/
+-rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-nc-sa.png
+-rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-sa.png
+-rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.9.0/pyrsm/radiant/www/imgs/icon.png
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.148277 pyrsm-0.9.0/pyrsm/radiant/www/js/
+-rw-r--r--   0 root         (0) staff       (20)      343 2023-07-20 00:49:53.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/radiantUI.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.9.0/pyrsm/radiant/www/js/screenshot.js
+-rw-r--r--   0 root         (0) staff       (20)      609 2023-07-20 01:32:43.000000 pyrsm-0.9.0/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9469 2023-07-20 05:16:59.000000 pyrsm-0.9.0/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.9.0/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.9.0/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.9.0/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.120794 pyrsm-0.9.0/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4022 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      242 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-20 09:01:14.000000 pyrsm-0.9.0/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-20 09:01:14.151005 pyrsm-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-20 09:01:14.150159 pyrsm-0.9.0/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.9.0/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.9.0/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.9.0/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.9.0/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.9.0/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.9.0/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.9.0/tests/test_utils.py
```

### Comparing `pyrsm-0.8.9/LICENSE` & `pyrsm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/MANIFEST.in` & `pyrsm-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/PKG-INFO` & `pyrsm-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.9/README.md` & `pyrsm-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.9.0/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/basics/compare_means.py` & `pyrsm-0.9.0/pyrsm/basics/compare_means.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,33 +207,40 @@
             comp_stats = comp_stats.iloc[:, [0, 1, 2, 3, -1]]
 
         comp_stats["p.value"] = ifelse(
             comp_stats["p.value"] < 0.001, "< .001", comp_stats["p.value"]
         )
         print(comp_stats.round(dec).to_string(index=False))
 
-    def plot(self, plots: str = "scatter") -> None:
+    def plot(self, plots: str = "scatter", nobs: int = -1) -> None:
         if plots == "scatter":
-            sns.swarmplot(data=self.data, x=self.var1, y=self.var2)
+
+            if nobs < self.data.shape[0] and nobs != np.Inf and nobs != -1:
+                data = self.data.copy().sample(nobs)
+            else:
+                data = self.data.copy()
+
+            sns.swarmplot(data=data, x=self.var1, y=self.var2, alpha=0.5)
 
             # Get the unique categories and their indices
-            categories = self.data[self.var1].cat.categories
+            categories = data[self.var1].cat.categories
             category_indices = {category: i for i, category in enumerate(categories)}
 
-            category_means = self.data.groupby(self.var1)[self.var2].mean()
+            category_means = data.groupby(self.var1)[self.var2].mean()
 
             # Add a horizontal line for each category at the mean of the value for that category
             for category, mean in category_means.items():
                 plt.hlines(
                     y=mean,
                     xmin=category_indices[category] - 0.3,
                     xmax=category_indices[category] + 0.3,
-                    color="red",
+                    color="blue",
                     linestyle="--",
-                    linewidth=3,
+                    linewidth=2,
+                    zorder=2,
                 )
 
         elif plots == "box":
             sns.boxplot(data=self.data, x=self.var1, y=self.var2)
         elif plots == "density":
             sns.kdeplot(data=self.data, x=self.var2, hue=self.var1)
         elif plots == "bar":
```

### Comparing `pyrsm-0.8.9/pyrsm/basics/compare_props.py` & `pyrsm-0.9.0/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/basics/correlation.py` & `pyrsm-0.9.0/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/basics/cross_tabs.py` & `pyrsm-0.9.0/pyrsm/basics/cross_tabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,21 +172,21 @@
 {100 * round(self.expected_low[0] / self.expected_low[1], dec)}% of cells have expected values below 5
 """
         print(prn)
 
         pd.reset_option("display.max_columns")
         pd.reset_option("display.max_rows")
 
-    def plot(self, output: list[str] = "perc_col", **kwargs) -> None:
+    def plot(self, plots: list[str] = "perc_col", **kwargs) -> None:
         """
         Plot of correlations between numeric variables in a Pandas dataframe
 
         Parameters
         ----------
-        output : list of tables to show
+        plots : list of tables to show
             Options include "observed" (observed frequencies),
             "expected" (expected frequencies), "chisq" (chi-square values)
             for each cell, "dev_std" (standardized deviations from expected)
             "perc_row" (percentages conditioned by row), "perc_col"
             (percentages conditioned by column), "perc" (percentages by the
             total number of observations). The default value is ["observed", "expected"]
         **kwargs : Named arguments to be passed to pandas plotting functions
@@ -194,62 +194,62 @@
         Examples
         --------
         import pyrsm as rsm
         rsm.load_data(pkg="basics", name="newspaper", dct=globals())
         ct = rsm.cross_tabs(newspaper, "Income", "Newspaper")
         ct.plot()
         """
-        output = ifelse(isinstance(output, str), [output], output)
+        plots = ifelse(isinstance(plots, str), [plots], plots)
 
         args = {"rot": False}
-        if "observed" in output:
+        if "observed" in plots:
             tab = (
                 self.observed.transpose()
                 .drop(columns="Total")
                 .drop("Total", axis=0)
                 .apply(lambda x: x * 100 / sum(x), axis=1)
             )
             args["title"] = "Observed frequencies"
             args.update(**kwargs)
             fig = tab.plot.bar(stacked=True, **args)
-        if "expected" in output:
+        if "expected" in plots:
             tab = (
                 self.expected.transpose()
                 .drop(columns="Total")
                 .drop("Total", axis=0)
                 .apply(lambda x: x * 100 / sum(x), axis=1)
             )
             args["title"] = "Expected frequencies"
             args.update(**kwargs)
             fig = tab.plot.bar(stacked=True, **args)
-        if "chisq" in output:
+        if "chisq" in plots:
             tab = self.chisq.transpose().drop(columns="Total").drop("Total", axis=0)
             args["title"] = "Contribution to chi-squared statistic"
             args.update(**kwargs)
             fig = tab.plot.bar(**args)
-        if "dev_std" in output:
+        if "dev_std" in plots:
             tab = self.dev_std.transpose()
             args["title"] = "Deviation standardized"
             args.update(**kwargs)
             fig, ax = plt.subplots()
             tab.plot.bar(**args, ax=ax)
             ax.axhline(y=1.96, color="black", linestyle="--")
             ax.axhline(y=1.64, color="black", linestyle="--")
             ax.axhline(y=-1.96, color="black", linestyle="--")
             ax.axhline(y=-1.64, color="black", linestyle="--")
             ax.annotate("95%", xy=(0, 2.1), va="bottom", ha="center")
             ax.annotate("90%", xy=(0, 1.4), va="top", ha="center")
-        if "perc_col" in output:
+        if "perc_col" in plots:
             tab = self.perc_col.transpose().drop(columns="Total").drop("Total", axis=0)
             args["title"] = "Column percentages"
             args.update(**kwargs)
             fig = tab.plot.bar(**args)
-        if "perc_row" in output:
+        if "perc_row" in plots:
             tab = self.perc_row.transpose().drop(columns="Total").drop("Total", axis=0)
             args["title"] = "Row percentages"
             args.update(**kwargs)
             fig = tab.plot.bar(**args)
-        if "perc" in output:
+        if "perc" in plots:
             tab = self.perc.transpose().drop(columns="Total").drop("Total", axis=0)
             args["title"] = "Table percentages"
             args.update(**kwargs)
             fig = tab.plot.bar(**args)
```

### Comparing `pyrsm-0.8.9/pyrsm/basics/probability_calculator_functions.py` & `pyrsm-0.9.0/pyrsm/basics/probability_calculator_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,650 +1,49 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy import stats
 from math import floor, ceil
 
 
 def iround(x, dec):
-    if isinstance(x, float):
-        return round(x, dec)
-    else:
-        return x
-
-
-def prob_tdist(df, lb=None, ub=None, plb=None, pub=None):
-    if lb is None:
-        p_lb = None
-    else:
-        p_lb = stats.t.cdf(lb, df)
-
-    if ub is None:
-        p_ub = None
-    else:
-        p_ub = stats.t.cdf(ub, df)
-
-    p_int = None
-    if lb is not None and ub is not None:
-        if lb > ub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound value"
-            )
-        else:
-            p_int = max(p_ub - p_lb, 0)
-
-    if pub is not None:
-        if pub < 0:
-            pub = 0
-        elif pub > 1:
-            pub = 1
-
-    if plb is not None:
-        if plb < 0:
-            plb = 0
-        elif plb > 1:
-            plb = 1
-
-    if plb is not None:
-        v_lb = stats.t.ppf(plb, df)
-    else:
-        v_lb = None
+    return x if not isinstance(x, float) else round(x, dec)
 
-    if pub is not None:
-        v_ub = stats.t.ppf(pub, df)
-    else:
-        v_ub = None
 
-    if plb is not None and pub is not None:
-        if plb > pub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound probability"
-            )
-
-    return {
-        "p_lb": p_lb,
-        "p_ub": p_ub,
-        "p_int": p_int,
-        "v_lb": v_lb,
-        "v_ub": v_ub,
-        "df": df,
-        "lb": lb,
-        "ub": ub,
-        "plb": plb,
-        "pub": pub,
-    }
-
-
-def summary_prob_tdist(dct, type="values", dec=3):
-    dct = {k: iround(v, dec) for k, v in dct.items()}
-    print("Probability calculator")
-    print("Distribution: t")
-
-    df = dct["df"]
-    n = df + 1
-    print("Df          :", df)
-    print("Mean        :", 0)
-    if n > 2:
-        print("St. dev     :", round(n / (n - 2), dec))
-    else:
-        print("St. dev     :", "NA")
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-
-        print("Lower bound :", "-Inf" if lb is None else lb)
-        print("Upper bound :", "Inf" if ub is None else ub)
-
-        if ub is not None or lb is not None:
-            print()
-
-            if lb is not None:
-                print(f"P(X < {lb}) = {p_lb}")
-                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
-
-            if ub is not None:
-                ub = round(ub, dec)
-                print(f"P(X < {ub}) = {p_ub}")
-                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
-
-            if lb is not None and ub is not None:
-                print(f"P({lb} < X < {ub})     = {p_int}")
-                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
-    else:
-        plb, pub = dct["plb"], dct["pub"]
-        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
-
-        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
-        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
-
-        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
-            print()
-
-            if plb is not None and plb >= 0:
-                v_lb = round(v_lb, dec)
-                print(f"P(X < {v_lb}) = {plb}")
-                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
-
-            if pub is not None and pub <= 1:
-                v_ub = round(v_ub, dec)
-                print(f"P(X < {v_ub}) = {pub}")
-                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
-
-            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
-                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
-                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
-
-
-def plot_prob_tdist(dct, type="values"):
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-    else:
-        lb, ub = dct["v_lb"], dct["v_ub"]
-
-    x_range = np.linspace(-3, 3, 1000)
-    y_range = stats.t.pdf(x_range, dct["df"])
-
-    fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
-    elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
-    elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
-    else:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > 0) | (x_range < 0)),
-            color="blue",
-            alpha=0.5,
+def check(lb, ub, plb, pub):
+    if (lb is not None and ub is not None and lb > ub) or (
+        plb is not None and pub is not None and plb > pub
+    ):
+        raise ValueError(
+            "Please ensure the lower bound is smaller than the upper bound"
         )
 
-    if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
-    if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
-
 
-def prob_fdist(df1, df2, lb=None, ub=None, plb=None, pub=None):
-    if lb is not None and lb < 0:
-        lb = 0
-    if ub is not None and ub < 0:
-        ub = 0
-
-    if lb is None:
-        p_lb = None
-    else:
-        p_lb = stats.f.cdf(lb, df1, df2)
-
-    if ub is None:
-        p_ub = None
-    else:
-        p_ub = stats.f.cdf(ub, df1, df2)
-
-    p_int = None
+def make_colors_discrete(ub, lb, x_range):
     if lb is not None and ub is not None:
-        if lb > ub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound value"
-            )
-        else:
-            p_int = max(p_ub - p_lb, 0)
-
-    if pub is not None:
-        if pub < 0:
-            pub = 0
-        elif pub > 1:
-            pub = 1
-
-    if plb is not None:
-        if plb < 0:
-            plb = 0
-        elif plb > 1:
-            plb = 1
-
-    if plb is not None:
-        v_lb = stats.f.ppf(plb, df1, df2)
-    else:
-        v_lb = None
-
-    if pub is not None:
-        v_ub = stats.f.ppf(pub, df1, df2)
-    else:
-        v_ub = None
-
-    if plb is not None and pub is not None:
-        if plb > pub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound probability"
-            )
-
-    return {
-        "p_lb": p_lb,
-        "p_ub": p_ub,
-        "p_int": p_int,
-        "v_lb": v_lb,
-        "v_ub": v_ub,
-        "df1": df1,
-        "df2": df2,
-        "lb": lb,
-        "ub": ub,
-        "plb": plb,
-        "pub": pub,
-    }
-
-
-def summary_prob_fdist(dct, type="values", dec=3):
-    dct = {k: iround(v, dec) for k, v in dct.items()}
-    print("Probability calculator")
-    print("Distribution: F")
-
-    df1, df2 = dct["df1"], dct["df2"]
-    print("Df 1        :", df1)
-    print("Df 2        :", df2)
-    m = round(df2 / (df2 - 2), dec) if df2 > 2 else "NA"
-    variance = (
-        round(
-            (2 * df2**2 * (df1 + df2 - 2)) / (df1 * (df2 - 2) ** 2 * (df2 - 4)), dec
-        )
-        if df2 > 4
-        else np.nan
-    )
-    print("Mean        :", m)
-    print("Variance    :", variance)
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-
-        print("Lower bound :", "0" if lb is None else lb)
-        print("Upper bound :", "Inf" if ub is None else ub)
-
-        if ub is not None or lb is not None:
-            print()
-
-            if lb is not None:
-                lb = round(lb, dec)
-                print(f"P(X < {lb}) = {p_lb}")
-                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
-
-            if ub is not None:
-                ub = round(ub, dec)
-                print(f"P(X < {ub}) = {p_ub}")
-                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
-
-            if lb is not None and ub is not None:
-                print(f"P({lb} < X < {ub})     = {p_int}")
-                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
-    else:
-        plb, pub = dct["plb"], dct["pub"]
-        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
-
-        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
-        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
-
-        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
-            print()
-
-            if plb is not None and plb >= 0:
-                v_lb = round(v_lb, dec)
-                print(f"P(X < {v_lb}) = {plb}")
-                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
-
-            if pub is not None and pub <= 1:
-                v_ub = round(v_ub, dec)
-                print(f"P(X < {v_ub}) = {pub}")
-                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
-
-            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
-                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
-                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
-
-
-def plot_prob_fdist(dct, type="values"):
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-    else:
-        lb, ub = dct["v_lb"], dct["v_ub"]
-
-    df1, df2 = dct["df1"], dct["df2"]
-    x_range = np.linspace(0, stats.f.ppf(0.99, df1, df2), 1000)
-    y_range = stats.f.pdf(x_range, df1, df2)
-
-    fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
-    elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
+        # colors = ["red" if i < lb else "blue" if i <= ub else "red" for i in x_range]
+        colors = [
+            "red"
+            if i < lb
+            else "red"
+            if i > ub
+            else "green"
+            if i == lb or i == ub
+            else "blue"
+            for i in x_range
+        ]
     elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
-    else:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > 0) | (x_range < 0)),
-            color="blue",
-            alpha=0.5,
-        )
-
-    if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
-    if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
-
-
-def prob_norm(mean, stdev, lb=None, ub=None, plb=None, pub=None):
-    if lb is not None:
-        p_lb = stats.norm.cdf(lb, mean, stdev)
-    else:
-        p_lb = None
-
-    if ub is not None:
-        p_ub = stats.norm.cdf(ub, mean, stdev)
-    else:
-        p_ub = None
-
-    if lb is not None and ub is not None:
-        p_int = max(p_ub - p_lb, 0)
-    else:
-        p_int = None
-
-    if plb is not None:
-        v_lb = stats.norm.ppf(plb, mean, stdev)
-    else:
-        v_lb = None
-
-    if pub is not None:
-        v_ub = stats.norm.ppf(pub, mean, stdev)
-    else:
-        v_ub = None
-
-    return {
-        "p_lb": p_lb,
-        "p_ub": p_ub,
-        "p_int": p_int,
-        "v_lb": v_lb,
-        "v_ub": v_ub,
-        "mean": mean,
-        "stdev": stdev,
-        "lb": lb,
-        "ub": ub,
-        "plb": plb,
-        "pub": pub,
-    }
-
-
-def summary_prob_norm(dct, type="values", dec=3):
-    dct = {k: iround(v, dec) for k, v in dct.items()}
-    print("Probability calculator")
-    print("Distribution: Normal")
-
-    mean, stdev = dct["mean"], dct["stdev"]
-    print("Mean        :", round(mean, dec))
-    print("St. dev     :", round(stdev, dec))
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-
-        print("Lower bound :", "-Inf" if lb is None else lb)
-        print("Upper bound :", "Inf" if ub is None else ub)
-
-        if ub is not None or lb is not None:
-            print()
-
-            if lb is not None:
-                lb = round(lb, dec)
-                print(f"P(X < {lb}) = {p_lb}")
-                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
-
-            if ub is not None:
-                ub = round(ub, dec)
-                print(f"P(X < {ub}) = {p_ub}")
-                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
-
-            if lb is not None and ub is not None:
-                print(f"P({lb} < X < {ub})     = {p_int}")
-                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
-    else:
-        plb, pub = dct["plb"], dct["pub"]
-        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
-
-        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
-        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
-
-        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
-            print()
-
-            if plb is not None and plb >= 0:
-                v_lb = round(v_lb, dec)
-                print(f"P(X < {v_lb}) = {plb}")
-                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
-
-            if pub is not None and pub <= 1:
-                v_ub = round(v_ub, dec)
-                print(f"P(X < {v_ub}) = {pub}")
-                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
-
-            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
-                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
-                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
-
-
-def plot_prob_norm(dct, type="values"):
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-    else:
-        lb, ub = dct["v_lb"], dct["v_ub"]
-
-    mean, stdev = dct["mean"], dct["stdev"]
-    x_range = np.linspace(mean - 3 * stdev, mean + 3 * stdev, 1000)
-    y_range = stats.norm.pdf(x_range, mean, stdev)
-
-    fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
+        colors = ["red" if i < lb else "green" if i == lb else "blue" for i in x_range]
     elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
-    elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
-    else:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > 0) | (x_range < 0)),
-            color="blue",
-            alpha=0.5,
-        )
-
-    if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
-    if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
-
-
-def prob_chisq(df, lb=None, ub=None, plb=None, pub=None):
-    if lb is not None:
-        p_lb = stats.chi2.cdf(lb, df)
-    else:
-        p_lb = None
-
-    if ub is not None:
-        p_ub = stats.chi2.cdf(ub, df)
-    else:
-        p_ub = None
-
-    if lb is not None and ub is not None:
-        p_int = max(p_ub - p_lb, 0)
-    else:
-        p_int = None
-
-    if plb is not None:
-        v_lb = stats.chi2.ppf(plb, df)
-    else:
-        v_lb = None
-
-    if pub is not None:
-        v_ub = stats.chi2.ppf(pub, df)
-    else:
-        v_ub = None
-
-    return {
-        "p_lb": p_lb,
-        "p_ub": p_ub,
-        "p_int": p_int,
-        "v_lb": v_lb,
-        "v_ub": v_ub,
-        "df": df,
-        "lb": lb,
-        "ub": ub,
-        "plb": plb,
-        "pub": pub,
-    }
-
-
-def summary_prob_chisq(dct, type="values", dec=3):
-    dct = {k: iround(v, dec) for k, v in dct.items()}
-    print("Probability calculator")
-    print("Distribution: Chi-square")
-
-    df = dct["df"]
-    print("Df          :", df)
-    print("Mean        :", df)
-    print("Variance    :", 2 * df)
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-
-        print("Lower bound :", "0" if lb is None else lb)
-        print("Upper bound :", "Inf" if ub is None else ub)
-
-        if ub is not None or lb is not None:
-            print()
-
-            if lb is not None:
-                print(f"P(X < {lb}) = {p_lb}")
-                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
-
-            if ub is not None:
-                print(f"P(X < {ub}) = {p_ub}")
-                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
-
-            if lb is not None and ub is not None:
-                print(f"P({lb} < X < {ub})     = {p_int}")
-                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
-    else:
-        plb, pub = dct["plb"], dct["pub"]
-        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
-
-        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
-        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
-
-        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
-            print()
-
-            if plb is not None and plb >= 0:
-                print(f"P(X < {v_lb}) = {plb}")
-                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
-
-            if pub is not None and pub <= 1:
-                print(f"P(X < {v_ub}) = {pub}")
-                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
-
-            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
-                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
-                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
-
-
-def plot_prob_chisq(dct, type="values"):
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
+        colors = ["blue" if i < ub else "green" if i == ub else "red" for i in x_range]
     else:
-        lb, ub = dct["v_lb"], dct["v_ub"]
+        colors = "blue"
+    return colors
 
-    df = dct["df"]
-    x_range = np.linspace(
-        floor(stats.chi2.ppf(0.001, df)), ceil(stats.chi2.ppf(1 - 0.001, df)), 1000
-    )
-    y_range = stats.chi2.pdf(x_range, df)
 
+def make_colors_continuous(ub, lb, x_range, y_range):
     fig, ax = plt.subplots()
     ax.plot(x_range, y_range, "k")
     if ub is not None and lb is not None:
         ax.fill_between(
             x_range,
             y_range,
             where=((x_range > lb) & (x_range < ub)),
@@ -682,206 +81,54 @@
         )
 
     if lb is not None:
         ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
     if ub is not None:
         ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
 
+    return ax
 
-def prob_unif(min, max, lb=None, ub=None, plb=None, pub=None):
-    if min > max:
-        raise ValueError("The maximum value must be larger than the minimum value")
-
-    if lb is not None:
-        p_lb = stats.uniform.cdf(lb, min, max - min)
-    else:
-        p_lb = None
-
-    if ub is not None:
-        p_ub = stats.uniform.cdf(ub, min, max - min)
-    else:
-        p_ub = None
-
-    if lb is not None and ub is not None:
-        p_int = np.max(p_ub - p_lb, 0)
-    else:
-        p_int = None
-
-    if plb is not None:
-        v_lb = stats.uniform.ppf(plb, min, max - min)
-    else:
-        v_lb = None
-
-    if pub is not None:
-        v_ub = stats.uniform.ppf(pub, min, max - min)
-    else:
-        v_ub = None
-
-    mean = (max + min) / 2
-    stdev = np.sqrt((max - min) ** 2 / 12)
-
-    return {
-        "p_lb": p_lb,
-        "p_ub": p_ub,
-        "p_int": p_int,
-        "v_lb": v_lb,
-        "v_ub": v_ub,
-        "mean": mean,
-        "stdev": stdev,
-        "min": min,
-        "max": max,
-        "lb": lb,
-        "ub": ub,
-        "plb": plb,
-        "pub": pub,
-    }
-
-
-def summary_prob_unif(dct, type="values", dec=3):
-    dct = {k: iround(v, dec) for k, v in dct.items()}
-    print("Probability calculator")
-    print("Distribution: Uniform")
-
-    min, max = dct["min"], dct["max"]
-    mean, stdev = dct["mean"], dct["stdev"]
-
-    print("Min         :", min)
-    print("Max         :", max)
-    print("Mean        :", round(mean, dec))
-    print("St. dev     :", round(stdev, dec))
-
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-
-        print("Lower bound :", min if lb is None else lb)
-        print("Upper bound :", max if ub is None else ub)
-
-        if ub is not None or lb is not None:
-            print()
-
-            if lb is not None:
-                print(f"P(X < {lb}) = {p_lb}")
-                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
-
-            if ub is not None:
-                print(f"P(X < {ub}) = {p_ub}")
-                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
-
-            if lb is not None and ub is not None:
-                print(f"P({lb} < X < {ub})     = {p_int}")
-                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
-    else:
-        plb, pub = dct["plb"], dct["pub"]
-        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
-
-        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
-        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
-
-        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
-            print()
-
-            if plb is not None and plb >= 0:
-                print(f"P(X < {v_lb}) = {plb}")
-                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
-
-            if pub is not None and pub <= 1:
-                print(f"P(X < {v_ub}) = {pub}")
-                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
-
-            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
-                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
-                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
-
-
-def plot_prob_unif(dct, type="values"):
-    if type == "values":
-        lb, ub = dct["lb"], dct["ub"]
-    else:
-        lb, ub = dct["v_lb"], dct["v_ub"]
-
-    min, max = dct["min"], dct["max"]
-
-    x_range = np.linspace(min, max, 1000)
-    y_range = stats.uniform.pdf(x_range, min, max - min)
 
+def make_barplot(ub, lb, x_range, y_range):
     fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
-    elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
-    elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
-    else:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > 0) | (x_range < 0)),
-            color="blue",
-            alpha=0.5,
-        )
-
-    ax.axvline(min, ymin=0.048, ymax=0.952, color="black", linewidth=1)
-    ax.axvline(max, ymin=0.048, ymax=0.952, color="black", linewidth=1)
-
-    if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
-    if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
+    colors = make_colors_discrete(ub, lb, x_range)
+    ax.bar(x_range, y_range, color=colors, alpha=0.5)
+    if len(x_range) <= 20:
+        ax.set_xticks(x_range)
 
+    return ax
 
-def prob_binom(n, p, lb=None, ub=None, plb=None, pub=None):
 
-    # Helper function to round to specified decimals
-    def round_to(x, decimals):
-        return np.round(x, decimals).tolist()
+def prob_binom(n: int, p: float, lb=None, ub=None, plb=None, pub=None):
 
     # Helper function to convert to int if not None
     def to_int(x):
-        if x is None:
-            return None
-        else:
-            return int(x)
+        return int(max(0, x)) if x is not None else None
 
-    # Convert n, lb, and ub to int
-    n = int(n)
     lb = to_int(lb)
     ub = to_int(ub)
 
-    if lb is not None and lb < 0:
-        lb = 0
-    if ub is not None and ub < 0:
-        ub = 0
-
-    p_elb = p_lelb = p_lb = p_eub = p_leub = p_ub = p_int = None
-    vlb = vp_elb = vp_lelb = vp_lb = vub = vp_eub = vp_leub = vp_ub = vp_int = None
+    (
+        p_elb,
+        p_lelb,
+        p_lb,
+        p_eub,
+        p_leub,
+        p_ub,
+        p_int,
+        vlb,
+        vp_elb,
+        vp_lelb,
+        vp_lb,
+        vub,
+        vp_eub,
+        vp_leub,
+        vp_ub,
+        vp_int,
+    ) = [None] * 16
 
     if lb is not None:
         if lb > n:
             lb = n
         p_elb = stats.binom.pmf(lb, n, p)
         p_lelb = stats.binom.cdf(lb, n, p)
         if lb > 0:
@@ -924,23 +171,15 @@
         vp_eub = stats.binom.pmf(vub, n, p)
         vp_leub = stats.binom.cdf(vub, n, p)
         if vub > 0:
             vp_ub = sum(stats.binom.pmf(range(0, int(vub)), n, p))
         else:
             vp_ub = 0
 
-    if lb is not None and ub is not None and lb > ub:
-        raise ValueError(
-            "Please ensure the lower bound is smaller than the upper bound"
-        )
-
-    if vlb is not None and vub is not None and vlb > vub:
-        raise ValueError(
-            "Please ensure the lower bound is smaller than the upper bound"
-        )
+    check(lb, ub, plb, pub)
 
     if plb is not None and pub is not None:
         vp_int = sum(stats.binom.pmf(range(int(vlb), int(vub) + 1), n, p))
 
     # Return a dictionary of results
     return {
         "n": n,
@@ -982,20 +221,19 @@
     if type == "values":
         lb, ub = dct["lb"], dct["ub"]
         p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
         p_elb, p_eub = dct["p_elb"], dct["p_eub"]
         p_lelb, p_leub = dct["p_lelb"], dct["p_leub"]
 
         print("Lower bound :", "" if lb is None else lb)
-        print("Upper bound :", "" if ub is None else ub)
+        print("Upper bound :", "" if ub is None else ub, "\n")
 
         if ub is not None or lb is not None:
-            print()
-
             if lb is not None:
+                # print(f"P(X  = {lb}) = {p_elb} (green)")
                 print(f"P(X  = {lb}) = {p_elb}")
                 if lb > 0:
                     print(f"P(X  < {lb}) = {p_lb}")
                     print(f"P(X <= {lb}) = {p_lelb}")
                 if lb < n:
                     print(f"P(X  > {lb}) = {round(1 - (p_lb + p_elb), dec)}")
                     print(f"P(X >= {lb}) = {round(1 - p_lb, dec)}")
@@ -1016,18 +254,17 @@
         plb, pub = dct["plb"], dct["pub"]
         v_lb, v_ub = dct["vlb"], dct["vub"]
         vp_lb, vp_ub, vp_int = dct["vp_lb"], dct["vp_ub"], dct["vp_int"]
         vp_elb, vp_eub = dct["vp_elb"], dct["vp_eub"]
         vp_lelb, vp_leub = dct["vp_lelb"], dct["vp_leub"]
 
         print("Lower bound :", "" if plb is None else f"{plb} ({v_lb})")
-        print("Upper bound :", "" if pub is None else f"{pub} ({v_ub})")
+        print("Upper bound :", "" if pub is None else f"{pub} ({v_ub})\n")
 
         if pub is not None or plb is not None:
-            print()
 
             if plb is not None:
                 print(f"P(X  = {v_lb}) = {vp_elb}")
                 if v_lb > 0:
                     print(f"P(X  < {v_lb}) = {vp_lb}")
                     print(f"P(X <= {v_lb}) = {vp_lelb}")
                 if v_lb < n:
@@ -1055,34 +292,140 @@
         lb, ub = dct["vlb"], dct["vub"]
 
     n, p = dct["n"], dct["p"]
 
     x_range = np.arange(0, n)
     y_range = stats.binom.pmf(x_range, n, p)
 
-    fig, ax = plt.subplots()
+    make_barplot(ub, lb, x_range, y_range)
+
+
+def prob_chisq(df, lb=None, ub=None, plb=None, pub=None):
+    if lb is not None:
+        p_lb = stats.chi2.cdf(lb, df)
+    else:
+        p_lb = None
+
+    if ub is not None:
+        p_ub = stats.chi2.cdf(ub, df)
+    else:
+        p_ub = None
+
     if lb is not None and ub is not None:
-        colors = ["red" if i < lb else "blue" if i <= ub else "black" for i in x_range]
-    elif lb is not None:
-        colors = ["red" if i < lb else "blue" if i == lb else "black" for i in x_range]
-    elif ub is not None:
-        colors = ["red" if i < ub else "blue" if i == ub else "black" for i in x_range]
+        p_int = max(p_ub - p_lb, 0)
+    else:
+        p_int = None
 
-    ax.bar(x_range, y_range, color=colors, alpha=0.5)
+    if plb is not None:
+        v_lb = stats.chi2.ppf(plb, df)
+    else:
+        v_lb = None
+
+    if pub is not None:
+        v_ub = stats.chi2.ppf(pub, df)
+    else:
+        v_ub = None
+
+    check(lb, ub, plb, pub)
+
+    return {
+        "p_lb": p_lb,
+        "p_ub": p_ub,
+        "p_int": p_int,
+        "v_lb": v_lb,
+        "v_ub": v_ub,
+        "df": df,
+        "lb": lb,
+        "ub": ub,
+        "plb": plb,
+        "pub": pub,
+    }
+
+
+def summary_prob_chisq(dct, type="values", dec=3):
+    dct = {k: iround(v, dec) for k, v in dct.items()}
+    print("Probability calculator")
+    print("Distribution: Chi-square")
+
+    df = dct["df"]
+    print("Df          :", df)
+    print("Mean        :", df)
+    print("Variance    :", 2 * df)
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
+
+        print("Lower bound :", "0" if lb is None else lb)
+        print("Upper bound :", "Inf" if ub is None else ub)
+
+        if ub is not None or lb is not None:
+            print()
+
+            if lb is not None:
+                print(f"P(X < {lb}) = {p_lb}")
+                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
+
+            if ub is not None:
+                print(f"P(X < {ub}) = {p_ub}")
+                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
+
+            if lb is not None and ub is not None:
+                print(f"P({lb} < X < {ub})     = {p_int}")
+                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
+    else:
+        plb, pub = dct["plb"], dct["pub"]
+        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
+
+        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
+        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
+
+        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
+            print()
+
+            if plb is not None and plb >= 0:
+                print(f"P(X < {v_lb}) = {plb}")
+                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
+
+            if pub is not None and pub <= 1:
+                print(f"P(X < {v_ub}) = {pub}")
+                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
+
+            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
+                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
+                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
+
+
+def plot_prob_chisq(dct, type="values"):
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+    else:
+        lb, ub = dct["v_lb"], dct["v_ub"]
+
+    df = dct["df"]
+    x_range = np.linspace(
+        floor(stats.chi2.ppf(0.001, df)), ceil(stats.chi2.ppf(1 - 0.001, df)), 1000
+    )
+    y_range = stats.chi2.pdf(x_range, df)
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
 
 
 def prob_disc(v, p, lb=None, ub=None, plb=None, pub=None):
     # Check lengths
     if len(v) != len(p):
-        raise ValueError(
-            "The number of values must be the same or a multiple of the number of probabilities"
-        )
+        if len(v) % len(p) == 0:
+            p *= len(v) // len(p)
+        else:
+            raise ValueError(
+                "The number of values must be the same or a multiple of the number of probabilities"
+            )
 
     # Ensure sum of probabilities is approximately 1
-    if not 0.99 <= sum(p) <= 1.01:
+    if not 0.999 <= sum(p) <= 1.001:
         raise ValueError("Probabilities for a discrete variable do not sum to 1")
 
     # Sort values and probabilities in ascending order of values
     vp_sorted = sorted(zip(v, p))
     v, p = zip(*vp_sorted)
 
     # Discrete distribution functions
@@ -1147,14 +490,16 @@
         plb is not None
         and pub is not None
         and result.get("vlb") is not None
         and result.get("vub") is not None
     ):
         result["vp_int"] = result["vp_leub"] - result["vp_lb"]
 
+    check(lb, ub, plb, pub)
+
     return result
 
 
 def summary_prob_disc(dct, type="values", dec=3):
     dct = {k: iround(v, dec) for k, v in dct.items()}
     lb, ub = dct.get("lb", None), dct.get("ub", None)
     v, p = dct["v"], dct["p"]
@@ -1276,54 +621,32 @@
                     f"P({vlb} <= X <= {vub})     =": dct.get("vp_int", 0),
                     f"1 - P({vlb} <= X <= {vub}) =": round(
                         1 - dct.get("vp_int", 0), dec
                     ),
                 }
             )
 
-        for k, v in header.items():
-            if v is not None:
-                print(f"{k} {v}")
-
-        print()
-        for k, v in summary.items():
+    for k, v in header.items():
+        if v is not None:
             print(f"{k} {v}")
 
+    for k, v in summary.items():
+        print(f"{k} {v}")
+
 
 def plot_prob_disc(dct, type="values"):
     if type == "values":
         lb, ub = dct.get("lb", None), dct.get("ub", None)
     else:
         lb, ub = dct.get("vlb", None), dct.get("vub", None)
-    v, p = dct["v"], dct["p"]
+    x_range, y_range = dct["v"], dct["p"]
 
-    # Determine colors for each bar
-    colors = ["black"] * len(v)
-    if lb is not None and ub is not None:
-        for i, vi in enumerate(v):
-            if lb <= vi <= ub:
-                colors[i] = "blue"
-            elif vi < lb:
-                colors[i] = "red"
-    elif lb is not None:
-        for i, vi in enumerate(v):
-            if vi == lb:
-                colors[i] = "blue"
-            elif vi < lb:
-                colors[i] = "red"
-    elif ub is not None:
-        for i, vi in enumerate(v):
-            if vi == ub:
-                colors[i] = "blue"
-            elif vi < ub:
-                colors[i] = "red"
-
-    # Create bar plot
     fig, ax = plt.subplots()
-    ax.bar(v, p, color=colors, alpha=0.5)
+    colors = make_colors_discrete(ub, lb, x_range)
+    ax.bar(range(len(x_range)), y_range, tick_label=x_range, color=colors, alpha=0.5)
 
 
 def prob_expo(rate, lb=None, ub=None, plb=None, pub=None):
     if lb is not None and lb < 0:
         lb = 0
     if ub is not None and ub < 0:
         ub = 0
@@ -1365,19 +688,15 @@
         v_lb = None
 
     if pub is not None:
         v_ub = stats.expon.ppf(pub, scale=1 / rate)
     else:
         v_ub = None
 
-    if plb is not None and pub is not None:
-        if plb > pub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound probability"
-            )
+    check(lb, ub, plb, pub)
 
     return {
         "p_lb": p_lb,
         "p_ub": p_ub,
         "p_int": p_int,
         "v_lb": v_lb,
         "v_ub": v_ub,
@@ -1448,224 +767,153 @@
         lb, ub = dct["lb"], dct["ub"]
     else:
         lb, ub = dct["v_lb"], dct["v_ub"]
 
     rate = dct["rate"]
     x_range = np.linspace(0, stats.expon.ppf(0.99, scale=1 / rate), 1000)
     y_range = stats.expon.pdf(x_range, scale=1 / rate)
-
-    fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
-    elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
-    elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
-    else:
-        ax.fill_between(
-            x_range,
-            y_range,
-        )
-
-    if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
-    if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
 
 
-def prob_pois(lamb, lb=None, ub=None, plb=None, pub=None):
-    if lamb <= 0:
-        raise ValueError("Lambda must be positive")
-
+def prob_fdist(df1, df2, lb=None, ub=None, plb=None, pub=None):
     if lb is not None and lb < 0:
         lb = 0
     if ub is not None and ub < 0:
         ub = 0
 
     if lb is None:
         p_lb = None
-        p_elb = None
     else:
-        p_elb = stats.poisson.pmf(lb, lamb)
-        p_lelb = stats.poisson.cdf(lb, lamb)
-        if lb > 0:
-            p_lb = p_lelb - p_elb
-        else:
-            p_lb = 0
+        p_lb = stats.f.cdf(lb, df1, df2)
 
     if ub is None:
         p_ub = None
-        p_eub = None
     else:
-        p_eub = stats.poisson.pmf(ub, lamb)
-        p_leub = stats.poisson.cdf(ub, lamb)
-        if ub > 0:
-            p_ub = p_leub - p_eub
-        else:
-            p_ub = 0
+        p_ub = stats.f.cdf(ub, df1, df2)
 
     p_int = None
     if lb is not None and ub is not None:
-        if lb > ub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound value"
-            )
-        else:
-            p_int = max(
-                np.sum([stats.poisson.pmf(k, lamb) for k in range(lb, ub + 1)]), 0
-            )
+        p_int = max(p_ub - p_lb, 0)
 
     if pub is not None:
         if pub < 0:
             pub = 0
         elif pub > 1:
             pub = 1
 
     if plb is not None:
         if plb < 0:
             plb = 0
         elif plb > 1:
             plb = 1
 
-    if plb is None:
-        v_lb = None
+    if plb is not None:
+        v_lb = stats.f.ppf(plb, df1, df2)
     else:
-        v_lb = stats.poisson.ppf(plb, lamb)
+        v_lb = None
 
-    if pub is None:
-        v_ub = None
+    if pub is not None:
+        v_ub = stats.f.ppf(pub, df1, df2)
     else:
-        v_ub = stats.poisson.ppf(pub, lamb)
+        v_ub = None
 
-    if plb is not None and pub is not None:
-        if plb > pub:
-            raise ValueError(
-                "Please ensure the lower bound is smaller than the upper bound probability"
-            )
+    check(lb, ub, plb, pub)
 
     return {
         "p_lb": p_lb,
         "p_ub": p_ub,
         "p_int": p_int,
         "v_lb": v_lb,
         "v_ub": v_ub,
-        "lamb": lamb,
+        "df1": df1,
+        "df2": df2,
         "lb": lb,
         "ub": ub,
         "plb": plb,
         "pub": pub,
-        "p_elb": p_elb,
-        "p_eub": p_eub,
     }
 
 
-def summary_prob_pois(dct, type="values", dec=3):
+def summary_prob_fdist(dct, type="values", dec=3):
     dct = {k: iround(v, dec) for k, v in dct.items()}
     print("Probability calculator")
-    print("Distribution: Poisson")
+    print("Distribution: F")
 
-    lamb = dct["lamb"]
-    print("Lambda      :", lamb)
-    print("Mean        :", lamb)
-    print("Variance    :", lamb)
+    df1, df2 = dct["df1"], dct["df2"]
+    print("Df 1        :", df1)
+    print("Df 2        :", df2)
+    m = round(df2 / (df2 - 2), dec) if df2 > 2 else "NA"
+    variance = (
+        round(
+            (2 * df2**2 * (df1 + df2 - 2)) / (df1 * (df2 - 2) ** 2 * (df2 - 4)), dec
+        )
+        if df2 > 4
+        else np.nan
+    )
+    print("Mean        :", m)
+    print("Variance    :", variance)
 
     if type == "values":
         lb, ub = dct["lb"], dct["ub"]
         p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
-        p_elb, p_eub = dct["p_elb"], dct["p_eub"]
 
-        print("Lower bound :", "" if lb is None else lb)
-        print("Upper bound :", "" if ub is None else ub)
+        print("Lower bound :", "0" if lb is None else lb)
+        print("Upper bound :", "Inf" if ub is None else ub)
 
         if ub is not None or lb is not None:
             print()
 
             if lb is not None:
-                print(f"P(X  = {lb}) = {p_elb}")
-                if lb > 0:
-                    print(f"P(X  < {lb}) = {p_lb}")
-                    print(f"P(X <= {lb}) = {round(p_lb + p_elb, dec)}")
-                print(f"P(X  > {lb}) = {round(1 - (p_lb + p_elb), dec)}")
-                print(f"P(X >= {lb}) = {round(1 - p_lb, dec)}")
+                lb = round(lb, dec)
+                print(f"P(X < {lb}) = {p_lb}")
+                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
 
             if ub is not None:
-                print(f"P(X  = {ub}) = {p_eub}")
-                if ub > 0:
-                    print(f"P(X  < {ub}) = {p_ub}")
-                    print(f"P(X <= {ub}) = {round(p_ub + p_eub, dec)}")
-                print(f"P(X  > {ub}) = {round(1 - (p_ub + p_eub), dec)}")
-                print(f"P(X >= {ub}) = {round(1 - p_ub, dec)}")
+                ub = round(ub, dec)
+                print(f"P(X < {ub}) = {p_ub}")
+                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
 
             if lb is not None and ub is not None:
-                print(f"P({lb} <= X <= {ub})     = {p_int}")
-                print(f"1 - P({lb} <= X <= {ub}) = {round(1 - p_int, dec)}")
+                print(f"P({lb} < X < {ub})     = {p_int}")
+                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
     else:
         plb, pub = dct["plb"], dct["pub"]
         v_lb, v_ub = dct["v_lb"], dct["v_ub"]
 
-        print("Lower bound :", "" if plb is None else f"{plb} ({v_lb})")
-        print("Upper bound :", "" if pub is None else f"{pub} ({v_ub})")
+        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
+        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
 
         if (pub is None or pub <= 1) or (plb is None or plb >= 0):
             print()
 
             if plb is not None and plb >= 0:
-                print(f"P(X  < {v_lb}) = {plb}")
-                print(f"P(X  > {v_lb}) = {round(1 - plb, dec)}")
+                v_lb = round(v_lb, dec)
+                print(f"P(X < {v_lb}) = {plb}")
+                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
 
             if pub is not None and pub <= 1:
-                print(f"P(X  < {v_ub}) = {pub}")
-                print(f"P(X  > {v_ub}) = {round(1 - pub, dec)}")
+                v_ub = round(v_ub, dec)
+                print(f"P(X < {v_ub}) = {pub}")
+                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
+
+            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
+                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
+                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
 
 
-def plot_prob_pois(dct, type="values"):
+def plot_prob_fdist(dct, type="values"):
     if type == "values":
         lb, ub = dct["lb"], dct["ub"]
     else:
         lb, ub = dct["v_lb"], dct["v_ub"]
 
-    lamb = dct["lamb"]
-    n = max(lb, ub) if lb is not None and ub is not None else 100
-
-    limits = range(int(stats.poisson.ppf(1 - 0.00001, lamb)))
-    probabilities = [stats.poisson.pmf(k, lamb) for k in limits]
-
-    fig, ax = plt.subplots()
-    if lb is not None and ub is not None:
-        colors = ["red" if i < lb else "blue" if i <= ub else "black" for i in limits]
-    elif lb is not None:
-        colors = ["red" if i < lb else "blue" if i == lb else "black" for i in limits]
-    elif ub is not None:
-        colors = ["red" if i < ub else "blue" if i == ub else "black" for i in limits]
-
-    ax.bar(limits, probabilities, color=colors, alpha=0.5)
+    df1, df2 = dct["df1"], dct["df2"]
+    x_range = np.linspace(0, stats.f.ppf(0.99, df1, df2), 1000)
+    y_range = stats.f.pdf(x_range, df1, df2)
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
 
 
 def prob_lnorm(meanlog, sdlog, lb=None, ub=None, plb=None, pub=None):
     if lb is None:
         lb = -np.inf
     if ub is None:
         ub = np.inf
@@ -1693,23 +941,15 @@
     )
     v_lb = (
         stats.lognorm.ppf(plb, sdlog, scale=np.exp(meanlog))
         if plb is not None
         else None
     )
 
-    if lb > ub:
-        raise ValueError(
-            "Please ensure the lower bound is smaller than the upper bound"
-        )
-
-    if plb is not None and pub is not None and plb > pub:
-        raise ValueError(
-            "Please ensure the lower bound is smaller than the upper bound"
-        )
+    check(lb, ub, plb, pub)
 
     return {
         "meanlog": meanlog,
         "sdlog": sdlog,
         "lb": lb,
         "ub": ub,
         "p_lb": p_lb,
@@ -1757,16 +997,16 @@
             print(f"P(X > {ub if ub is not None else 'Inf'}) = {round(1 - p_ub, dec)}")
     else:
         if pub is None:
             pub = 2
         if plb is None:
             plb = -1
 
-        print("Lower bound :", "0" if plb < 0 else plb)
-        print("Upper bound :", "1" if pub > 1 else pub)
+        print("Lower bound :", "0" if plb < 0 else plb, "(" + str(v_lb) + ")")
+        print("Upper bound :", "1" if pub > 1 else pub, "(" + str(v_ub) + ")")
 
         if pub <= 1 or plb >= 0:
             print()
 
             if plb >= 0:
                 print(f"P(X < {v_lb}) = {plb}")
                 print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
@@ -1781,209 +1021,526 @@
 
 
 def plot_prob_lnorm(dct, type="values"):
     meanlog, sdlog = dct["meanlog"], dct["sdlog"]
     lb = dct["lb"] if type == "values" else dct["v_lb"]
     ub = dct["ub"] if type == "values" else dct["v_ub"]
 
-    x_range = np.linspace(0, meanlog + 7 * sdlog, 1000)
+    def scale(lb, ub):
+        if (ub is None or abs(ub) == np.Inf) and (lb is None or abs(lb) == np.Inf):
+            return 3
+        elif ub is not None and abs(ub) != np.Inf:
+            return max(3, ub)
+        elif lb is not None and abs(lb) != np.Inf:
+            return max(3, lb)
+
+    x_range = np.linspace(0, (np.exp(meanlog) + scale(lb, ub)) * sdlog, 1000)
     y_range = stats.lognorm.pdf(x_range, sdlog, scale=np.exp(meanlog))
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
 
-    fig, ax = plt.subplots()
-    ax.plot(x_range, y_range, "k")
-    if ub is not None and lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=((x_range > lb) & (x_range < ub)),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(
-            x_range, y_range, where=((x_range > ub) | (x_range < lb)), color="salmon"
-        )
-    elif ub is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range < ub),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range > ub), color="salmon")
-    elif lb is not None:
-        ax.fill_between(
-            x_range,
-            y_range,
-            where=(x_range > lb),
-            color="blue",
-            alpha=0.5,
-        )
-        ax.fill_between(x_range, y_range, where=(x_range < lb), color="salmon")
+
+def prob_norm(mean, stdev, lb=None, ub=None, plb=None, pub=None):
+    if lb is not None:
+        p_lb = stats.norm.cdf(lb, mean, stdev)
     else:
-        ax.fill_between(
-            x_range,
-            y_range,
-        )
+        p_lb = None
+
+    if ub is not None:
+        p_ub = stats.norm.cdf(ub, mean, stdev)
+    else:
+        p_ub = None
+
+    if lb is not None and ub is not None:
+        p_int = max(p_ub - p_lb, 0)
+    else:
+        p_int = None
+
+    if plb is not None:
+        v_lb = stats.norm.ppf(plb, mean, stdev)
+    else:
+        v_lb = None
+
+    if pub is not None:
+        v_ub = stats.norm.ppf(pub, mean, stdev)
+    else:
+        v_ub = None
+
+    check(lb, ub, plb, pub)
+
+    return {
+        "p_lb": p_lb,
+        "p_ub": p_ub,
+        "p_int": p_int,
+        "v_lb": v_lb,
+        "v_ub": v_ub,
+        "mean": mean,
+        "stdev": stdev,
+        "lb": lb,
+        "ub": ub,
+        "plb": plb,
+        "pub": pub,
+    }
+
+
+def summary_prob_norm(dct, type="values", dec=3):
+    dct = {k: iround(v, dec) for k, v in dct.items()}
+    print("Probability calculator")
+    print("Distribution: Normal")
+
+    mean, stdev = dct["mean"], dct["stdev"]
+    print("Mean        :", round(mean, dec))
+    print("St. dev     :", round(stdev, dec))
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
+
+        print("Lower bound :", "-Inf" if lb is None else lb)
+        print("Upper bound :", "Inf" if ub is None else ub)
+
+        if ub is not None or lb is not None:
+            print()
+
+            if lb is not None:
+                lb = round(lb, dec)
+                print(f"P(X < {lb}) = {p_lb}")
+                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
+
+            if ub is not None:
+                ub = round(ub, dec)
+                print(f"P(X < {ub}) = {p_ub}")
+                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
+
+            if lb is not None and ub is not None:
+                print(f"P({lb} < X < {ub})     = {p_int}")
+                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
+    else:
+        plb, pub = dct["plb"], dct["pub"]
+        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
+
+        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
+        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
+
+        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
+            print()
+
+            if plb is not None and plb >= 0:
+                v_lb = round(v_lb, dec)
+                print(f"P(X < {v_lb}) = {plb}")
+                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
+
+            if pub is not None and pub <= 1:
+                v_ub = round(v_ub, dec)
+                print(f"P(X < {v_ub}) = {pub}")
+                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
+
+            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
+                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
+                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
+
+
+def plot_prob_norm(dct, type="values"):
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+    else:
+        lb, ub = dct["v_lb"], dct["v_ub"]
+
+    mean, stdev = dct["mean"], dct["stdev"]
+    x_range = np.linspace(mean - 3 * stdev, mean + 3 * stdev, 1000)
+    y_range = stats.norm.pdf(x_range, mean, stdev)
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
+
+
+def prob_pois(lamb, lb=None, ub=None, plb=None, pub=None):
+    if lamb <= 0:
+        raise ValueError("Lambda must be positive")
+
+    if lb is not None and lb < 0:
+        lb = 0
+    if ub is not None and ub < 0:
+        ub = 0
+
+    if lb is None:
+        p_lb = None
+        p_elb = None
+    else:
+        p_elb = stats.poisson.pmf(lb, lamb)
+        p_lelb = stats.poisson.cdf(lb, lamb)
+        if lb > 0:
+            p_lb = p_lelb - p_elb
+        else:
+            p_lb = 0
+
+    if ub is None:
+        p_ub = None
+        p_eub = None
+    else:
+        p_eub = stats.poisson.pmf(ub, lamb)
+        p_leub = stats.poisson.cdf(ub, lamb)
+        if ub > 0:
+            p_ub = p_leub - p_eub
+        else:
+            p_ub = 0
+
+    p_int = None
+    if lb is not None and ub is not None:
+        p_int = max(np.sum([stats.poisson.pmf(k, lamb) for k in range(lb, ub + 1)]), 0)
+
+    if pub is not None:
+        if pub < 0:
+            pub = 0
+        elif pub > 1:
+            pub = 1
+
+    if plb is not None:
+        if plb < 0:
+            plb = 0
+        elif plb > 1:
+            plb = 1
+
+    if plb is None:
+        v_lb = None
+    else:
+        v_lb = stats.poisson.ppf(plb, lamb)
+
+    if pub is None:
+        v_ub = None
+    else:
+        v_ub = stats.poisson.ppf(pub, lamb)
+
+    check(lb, ub, plb, pub)
+
+    return {
+        "p_lb": p_lb,
+        "p_ub": p_ub,
+        "p_int": p_int,
+        "v_lb": v_lb,
+        "v_ub": v_ub,
+        "lamb": lamb,
+        "lb": lb,
+        "ub": ub,
+        "plb": plb,
+        "pub": pub,
+        "p_elb": p_elb,
+        "p_eub": p_eub,
+    }
+
+
+def summary_prob_pois(dct, type="values", dec=3):
+    dct = {k: iround(v, dec) for k, v in dct.items()}
+    print("Probability calculator")
+    print("Distribution: Poisson")
+
+    lamb = dct["lamb"]
+    print("Lambda      :", lamb)
+    print("Mean        :", lamb)
+    print("Variance    :", lamb)
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
+        p_elb, p_eub = dct["p_elb"], dct["p_eub"]
+
+        print("Lower bound :", "" if lb is None else lb)
+        print("Upper bound :", "" if ub is None else ub)
+
+        if ub is not None or lb is not None:
+            print()
+
+            if lb is not None:
+                print(f"P(X  = {lb}) = {p_elb}")
+                if lb > 0:
+                    print(f"P(X  < {lb}) = {p_lb}")
+                    print(f"P(X <= {lb}) = {round(p_lb + p_elb, dec)}")
+                print(f"P(X  > {lb}) = {round(1 - (p_lb + p_elb), dec)}")
+                print(f"P(X >= {lb}) = {round(1 - p_lb, dec)}")
+
+            if ub is not None:
+                print(f"P(X  = {ub}) = {p_eub}")
+                if ub > 0:
+                    print(f"P(X  < {ub}) = {p_ub}")
+                    print(f"P(X <= {ub}) = {round(p_ub + p_eub, dec)}")
+                print(f"P(X  > {ub}) = {round(1 - (p_ub + p_eub), dec)}")
+                print(f"P(X >= {ub}) = {round(1 - p_ub, dec)}")
+
+            if lb is not None and ub is not None:
+                print(f"P({lb} <= X <= {ub})     = {p_int}")
+                print(f"1 - P({lb} <= X <= {ub}) = {round(1 - p_int, dec)}")
+    else:
+        plb, pub = dct["plb"], dct["pub"]
+        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
+
+        print("Lower bound :", "" if plb is None else f"{plb} ({v_lb})")
+        print("Upper bound :", "" if pub is None else f"{pub} ({v_ub})")
+
+        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
+            print()
+
+            if plb is not None and plb >= 0:
+                print(f"P(X  < {v_lb}) = {plb}")
+                print(f"P(X  > {v_lb}) = {round(1 - plb, dec)}")
+
+            if pub is not None and pub <= 1:
+                print(f"P(X  < {v_ub}) = {pub}")
+                print(f"P(X  > {v_ub}) = {round(1 - pub, dec)}")
+
+
+def plot_prob_pois(dct, type="values"):
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+    else:
+        lb, ub = dct["v_lb"], dct["v_ub"]
+
+    lamb = dct["lamb"]
+    n = max(lb, ub) if lb is not None and ub is not None else 100
+
+    x_range = range(int(stats.poisson.ppf(1 - 0.00001, lamb)))
+    y_range = [stats.poisson.pmf(k, lamb) for k in x_range]
+    make_barplot(ub, lb, x_range, y_range)
+
+
+def prob_tdist(df, lb=None, ub=None, plb=None, pub=None):
+    if lb is None:
+        p_lb = None
+    else:
+        p_lb = stats.t.cdf(lb, df)
+
+    if ub is None:
+        p_ub = None
+    else:
+        p_ub = stats.t.cdf(ub, df)
+
+    p_int = None
+    if lb is not None and ub is not None:
+        p_int = max(p_ub - p_lb, 0)
+
+    if pub is not None:
+        if pub < 0:
+            pub = 0
+        elif pub > 1:
+            pub = 1
+
+    if plb is not None:
+        if plb < 0:
+            plb = 0
+        elif plb > 1:
+            plb = 1
+
+    if plb is not None:
+        v_lb = stats.t.ppf(plb, df)
+    else:
+        v_lb = None
+
+    if pub is not None:
+        v_ub = stats.t.ppf(pub, df)
+    else:
+        v_ub = None
+
+    check(lb, ub, plb, pub)
+
+    return {
+        "p_lb": p_lb,
+        "p_ub": p_ub,
+        "p_int": p_int,
+        "v_lb": v_lb,
+        "v_ub": v_ub,
+        "df": df,
+        "lb": lb,
+        "ub": ub,
+        "plb": plb,
+        "pub": pub,
+    }
+
+
+def summary_prob_tdist(dct, type="values", dec=3):
+    dct = {k: iround(v, dec) for k, v in dct.items()}
+    print("Probability calculator")
+    print("Distribution: t")
+
+    df = dct["df"]
+    n = df + 1
+    print("Df          :", df)
+    print("Mean        :", 0)
+    if n > 2:
+        print("St. dev     :", round(n / (n - 2), dec))
+    else:
+        print("St. dev     :", "NA")
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
+
+        print("Lower bound :", "-Inf" if lb is None else lb)
+        print("Upper bound :", "Inf" if ub is None else ub)
+
+        if ub is not None or lb is not None:
+            print()
+
+            if lb is not None:
+                print(f"P(X < {lb}) = {p_lb}")
+                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
+
+            if ub is not None:
+                ub = round(ub, dec)
+                print(f"P(X < {ub}) = {p_ub}")
+                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
+
+            if lb is not None and ub is not None:
+                print(f"P({lb} < X < {ub})     = {p_int}")
+                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
+    else:
+        plb, pub = dct["plb"], dct["pub"]
+        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
+
+        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
+        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
+
+        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
+            print()
+
+            if plb is not None and plb >= 0:
+                v_lb = round(v_lb, dec)
+                print(f"P(X < {v_lb}) = {plb}")
+                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
+
+            if pub is not None and pub <= 1:
+                v_ub = round(v_ub, dec)
+                print(f"P(X < {v_ub}) = {pub}")
+                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
+
+            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
+                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
+                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
+
+
+def plot_prob_tdist(dct, type="values"):
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+    else:
+        lb, ub = dct["v_lb"], dct["v_ub"]
+
+    x_range = np.linspace(-3, 3, 1000)
+    y_range = stats.t.pdf(x_range, dct["df"])
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
+
+
+def prob_unif(min, max, lb=None, ub=None, plb=None, pub=None):
+    if min > max:
+        raise ValueError("The maximum value must be larger than the minimum value")
 
     if lb is not None:
-        ax.axvline(lb, color="black", linestyle="dashed", linewidth=0.5)
+        p_lb = stats.uniform.cdf(lb, min, max - min)
+    else:
+        p_lb = None
+
     if ub is not None:
-        ax.axvline(ub, color="black", linestyle="dashed", linewidth=0.5)
+        p_ub = stats.uniform.cdf(ub, min, max - min)
+    else:
+        p_ub = None
+
+    if lb is not None and ub is not None:
+        p_int = np.max(p_ub - p_lb, 0)
+    else:
+        p_int = None
+
+    if plb is not None:
+        v_lb = stats.uniform.ppf(plb, min, max - min)
+    else:
+        v_lb = None
+
+    if pub is not None:
+        v_ub = stats.uniform.ppf(pub, min, max - min)
+    else:
+        v_ub = None
+
+    mean = (max + min) / 2
+    stdev = np.sqrt((max - min) ** 2 / 12)
+
+    check(lb, ub, plb, pub)
+
+    return {
+        "p_lb": p_lb,
+        "p_ub": p_ub,
+        "p_int": p_int,
+        "v_lb": v_lb,
+        "v_ub": v_ub,
+        "mean": mean,
+        "stdev": stdev,
+        "min": min,
+        "max": max,
+        "lb": lb,
+        "ub": ub,
+        "plb": plb,
+        "pub": pub,
+    }
+
+
+def summary_prob_unif(dct, type="values", dec=3):
+    dct = {k: iround(v, dec) for k, v in dct.items()}
+    print("Probability calculator")
+    print("Distribution: Uniform")
+
+    min, max = dct["min"], dct["max"]
+    mean, stdev = dct["mean"], dct["stdev"]
+
+    print("Min         :", min)
+    print("Max         :", max)
+    print("Mean        :", round(mean, dec))
+    print("St. dev     :", round(stdev, dec))
+
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+        p_lb, p_ub, p_int = dct["p_lb"], dct["p_ub"], dct["p_int"]
 
+        print("Lower bound :", min if lb is None else lb)
+        print("Upper bound :", max if ub is None else ub)
+
+        if ub is not None or lb is not None:
+            print()
+
+            if lb is not None:
+                print(f"P(X < {lb}) = {p_lb}")
+                print(f"P(X > {lb}) = {round(1 - p_lb, dec)}")
+
+            if ub is not None:
+                print(f"P(X < {ub}) = {p_ub}")
+                print(f"P(X > {ub}) = {round(1 - p_ub, dec)}")
+
+            if lb is not None and ub is not None:
+                print(f"P({lb} < X < {ub})     = {p_int}")
+                print(f"1 - P({lb} < X < {ub}) = {round(1 - p_int, dec)}")
+    else:
+        plb, pub = dct["plb"], dct["pub"]
+        v_lb, v_ub = dct["v_lb"], dct["v_ub"]
+
+        print("Lower bound :", "0" if plb is None or plb < 0 else plb)
+        print("Upper bound :", "1" if pub is None or pub > 1 else pub)
+
+        if (pub is None or pub <= 1) or (plb is None or plb >= 0):
+            print()
 
-if __file__ == "__main__":
-    pt = prob_tdist(df=10, lb=-2.228, ub=2.228)
-    summary_prob_tdist(pt, type="values")
-    plot_prob_tdist(pt, type="values")
-    pt = prob_tdist(df=10, ub=2.228)
-    summary_prob_tdist(pt, type="values")
-    plot_prob_tdist(pt, type="values")
-    pt = prob_tdist(df=10, lb=-2.228)
-    plot_prob_tdist(pt, type="values")
-    pt = prob_tdist(df=10)
-    summary_prob_tdist(pt, type="values")
-    plot_prob_tdist(pt, type="values")
-
-    pt = prob_tdist(df=10, plb=0.025, pub=0.975)
-    summary_prob_tdist(pt, type="probs")
-    plot_prob_tdist(pt, type="prob")
-    pt = prob_tdist(df=10, pub=0.975)
-    summary_prob_tdist(pt, type="probs")
-    plot_prob_tdist(pt, type="probs")
-    pt = prob_tdist(df=10, plb=0.025)
-    summary_prob_tdist(pt, type="probs")
-    plot_prob_tdist(pt, type="probs")
-
-    pf = prob_fdist(df1=10, df2=10, lb=0.5, ub=2.978)
-    summary_prob_fdist(pf, type="values")
-    plot_prob_fdist(pf, type="values")
-    pf = prob_fdist(df1=10, df2=10, lb=0.5)
-    summary_prob_fdist(pf, type="values")
-    plot_prob_fdist(pf, type="values")
-    pf = prob_fdist(df1=10, df2=10, ub=2.978)
-    summary_prob_fdist(pf, type="values")
-    plot_prob_fdist(pf, type="values")
-
-    pf = prob_fdist(df1=10, df2=10, plb=0.05, pub=0.95)
-    summary_prob_fdist(pf, type="probs")
-    plot_prob_fdist(pf, type="probs")
-    pf = prob_fdist(df1=10, df2=10, plb=0.05)
-    summary_prob_fdist(pf, type="probs")
-    pf = prob_fdist(df1=10, df2=10, pub=0.95)
-    summary_prob_fdist(pf, type="probs")
-    plot_prob_fdist(pf, type="probs")
-
-    pn = prob_norm(mean=0, stdev=1, lb=-0.5, ub=0.5)
-    summary_prob_norm(pn, type="values")
-    plot_prob_norm(pn, type="values")
-    pn = prob_norm(mean=0, stdev=1, lb=-0.5)
-    summary_prob_norm(pn, type="values")
-    plot_prob_norm(pn, type="values")
-    pn = prob_norm(mean=0, stdev=1, ub=0.5)
-    summary_prob_norm(pn, type="values")
-    plot_prob_norm(pn, type="values")
-
-    pn = prob_norm(mean=0, stdev=1, plb=0.025, pub=0.975)
-    summary_prob_norm(pn, type="probs")
-    plot_prob_norm(pn, type="probs")
-    pn = prob_norm(mean=0, stdev=1, plb=0.025)
-    summary_prob_norm(pn, type="probs")
-    plot_prob_norm(pn, type="probs")
-    pn = prob_norm(mean=0, stdev=1, pub=0.975)
-    summary_prob_norm(pn, type="probs")
-    plot_prob_norm(pn, type="probs")
-
-    pc = prob_chisq(df=1, lb=1, ub=3.841)
-    summary_prob_chisq(pc, type="values")
-    plot_prob_chisq(pc, type="values")
-    pc = prob_chisq(df=1, lb=1)
-    summary_prob_chisq(pc, type="values")
-    plot_prob_chisq(pc, type="values")
-    pc = prob_chisq(df=1, ub=3.841)
-    summary_prob_chisq(pc, type="values")
-    plot_prob_chisq(pc, type="values")
-
-    pc = prob_chisq(df=1, plb=0.05, pub=0.95)
-    summary_prob_chisq(pc, type="probs")
-    plot_prob_chisq(pc, type="probs")
-    pc = prob_chisq(df=1, plb=0.05)
-    summary_prob_chisq(pc, type="probs")
-    plot_prob_chisq(pc, type="probs")
-    pc = prob_chisq(df=1, pub=0.95)
-    summary_prob_chisq(pc, type="probs")
-    plot_prob_chisq(pc, type="probs")
-
-    pu = prob_unif(min=0, max=1, lb=0.2, ub=0.8)
-    summary_prob_unif(pu, type="values")
-    plot_prob_unif(pu, type="values")
-    pu = prob_unif(min=0, max=1, lb=0.2)
-    summary_prob_unif(pu, type="values")
-    plot_prob_unif(pu, type="values")
-    pu = prob_unif(min=0, max=1, ub=0.8)
-    summary_prob_unif(pu, type="values")
-    plot_prob_unif(pu, type="values")
-
-    pu = prob_unif(min=0, max=1, plb=0.2, pub=0.8)
-    summary_prob_unif(pu, type="probs")
-    plot_prob_unif(pu, type="probs")
-    pu = prob_unif(min=0, max=1, plb=0.2)
-    summary_prob_unif(pu, type="probs")
-    plot_prob_unif(pu, type="probs")
-    pu = prob_unif(min=0, max=1, pub=0.8)
-    summary_prob_unif(pu, type="probs")
-    plot_prob_unif(pu, type="probs")
-
-    pb = prob_binom(n=10, p=0.3, lb=1, ub=3)
-    summary_prob_binom(pb, type="values")
-    plot_prob_binom(pb, type="values")
-    pb = prob_binom(n=10, p=0.3, lb=1)
-    summary_prob_binom(pb, type="values")
-    plot_prob_binom(pb, type="values")
-    pb = prob_binom(n=10, p=0.3, ub=3)
-    summary_prob_binom(pb, type="values")
-    plot_prob_binom(pb, type="values")
-
-    pb = prob_binom(n=10, p=0.3, plb=0.1, pub=0.8)
-    summary_prob_binom(pb, type="probs")
-    plot_prob_binom(pb, type="probs")
-    pb = prob_binom(n=10, p=0.3, plb=0.1)
-    summary_prob_binom(pb, type="probs")
-    plot_prob_binom(pb, type="probs")
-    pb = prob_binom(n=10, p=0.3, pub=0.8)
-    summary_prob_binom(pb, type="probs")
-    plot_prob_binom(pb, type="probs")
-
-    v = list(range(1, 7))
-    p = [1 / 6] * 6
-    pd = prob_disc(v, p, lb=2, ub=5)
-    summary_prob_disc(pd, type="values")
-    plot_prob_disc(pd, type="values")
-    pd = prob_disc(v, p, lb=2)
-    summary_prob_disc(pd, type="values")
-    plot_prob_disc(pd, type="values")
-    pd = prob_disc(v, p, ub=5)
-    summary_prob_disc(pd, type="values")
-    plot_prob_disc(pd, type="values")
-
-    v = list(range(1, 7))
-    p = [2 / 6, 2 / 6, 1 / 12, 1 / 12, 1 / 12, 1 / 12]
-    pd = prob_disc(v, p, plb=0.5, pub=0.8)
-    summary_prob_disc(pd, type="probs")
-    plot_prob_disc(pd, type="probs")
-    pd = prob_disc(v, p, plb=0.5)
-    summary_prob_disc(pd, type="probs")
-    plot_prob_disc(pd, type="probs")
-
-    v = list(range(1, 7))
-    p = [2 / 6, 2 / 6, 1 / 12, 1 / 12, 1 / 12, 1 / 12]
-    pd = prob_disc(v, p, plb=0.05, pub=0.95)
-    summary_prob_disc(pd, type="probs")
-    plot_prob_disc(pd, type="probs")
-
-    pd = prob_disc(v, p, pub=0.95)
-    summary_prob_disc(pd, type="probs")
-    plot_prob_disc(pd, type="probs")
-
-    pd = prob_disc(v, p, plb=0.05)
-    summary_prob_disc(pd, type="probs")
-    plot_prob_disc(pd, type="probs")
+            if plb is not None and plb >= 0:
+                print(f"P(X < {v_lb}) = {plb}")
+                print(f"P(X > {v_lb}) = {round(1 - plb, dec)}")
+
+            if pub is not None and pub <= 1:
+                print(f"P(X < {v_ub}) = {pub}")
+                print(f"P(X > {v_ub}) = {round(1 - pub, dec)}")
+
+            if (plb is not None and plb >= 0) and (pub is not None and pub <= 1):
+                print(f"P({v_lb} < X < {v_ub})     = {round(pub - plb, dec)}")
+                print(f"1 - P({v_lb} < X < {v_ub}) = {round(1 - (pub - plb), dec)}")
+
+
+def plot_prob_unif(dct, type="values"):
+    if type == "values":
+        lb, ub = dct["lb"], dct["ub"]
+    else:
+        lb, ub = dct["v_lb"], dct["v_ub"]
+
+    min, max = dct["min"], dct["max"]
+
+    x_range = np.linspace(min, max, 1000)
+    y_range = stats.uniform.pdf(x_range, min, max - min)
+    ax = make_colors_continuous(ub, lb, x_range, y_range)
+    ax.axvline(min, ymin=0.048, ymax=0.952, color="black", linewidth=1)
+    ax.axvline(max, ymin=0.048, ymax=0.952, color="black", linewidth=1)
```

### Comparing `pyrsm-0.8.9/pyrsm/basics/single_mean.py` & `pyrsm-0.9.0/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/basics/single_prop.py` & `pyrsm-0.9.0/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/bins.py` & `pyrsm-0.9.0/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.9.0/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/consider.parquet` & `pyrsm-0.9.0/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/consider_description.md` & `pyrsm-0.9.0/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.9.0/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.9.0/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.9.0/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/salary.parquet` & `pyrsm-0.9.0/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/basics/salary_description.md` & `pyrsm-0.9.0/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/avengers.parquet` & `pyrsm-0.9.0/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.9.0/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.9.0/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/publishers.parquet` & `pyrsm-0.9.0/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.9.0/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/titanic.parquet` & `pyrsm-0.9.0/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/data/titanic_description.md` & `pyrsm-0.9.0/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.9.0/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/catalog.parquet` & `pyrsm-0.9.0/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/catalog_description.md` & `pyrsm-0.9.0/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.9.0/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.9.0/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.9.0/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.9.0/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/dvd.parquet` & `pyrsm-0.9.0/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/dvd_description.md` & `pyrsm-0.9.0/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.9.0/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.9.0/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.9.0/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/ideal.parquet` & `pyrsm-0.9.0/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.9.0/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.9.0/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/ratings.parquet` & `pyrsm-0.9.0/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/titanic.parquet` & `pyrsm-0.9.0/pyrsm/data/model/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/model/titanic_description.md` & `pyrsm-0.9.0/pyrsm/data/model/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.9.0/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/example_data.py` & `pyrsm-0.9.0/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/logistic.py` & `pyrsm-0.9.0/pyrsm/logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,38 +120,42 @@
             else:
                 print("\nVariance inflation factors:")
                 print(f"\n{calc_vif(self.fitted).to_string()}")
 
         if test is not None and len(test) > 0:
             self.chisq_test(test=test, dec=dec)
 
-    def predict(self, df=None, cmd=None, dc=False, ci=False, conf=0.95) -> pd.DataFrame:
+    def predict(
+        self, data=None, cmd=None, dc=False, ci=False, conf=0.95
+    ) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
-        if df is None:
-            df = self.data
-        df = df.loc[:, self.evar].copy()
+        if data is None:
+            data = self.data
+        data = data.loc[:, self.evar].copy()
         if cmd is not None:
             if dc:
                 for k, v in cmd.items():
-                    df[k] = v
+                    data[k] = v
             else:
-                df = sim_prediction(df=df, vary=cmd)
+                data = sim_prediction(data=data, vary=cmd)
 
         if ci:
             if dc:
                 raise ValueError(
                     "Confidence intervals not available when using the Data & Command option"
                 )
             else:
-                return pd.concat([df, predict_ci(self.fitted, df, conf=conf)], axis=1)
+                return pd.concat(
+                    [data, predict_ci(self.fitted, data, conf=conf)], axis=1
+                )
         else:
-            pred = pd.DataFrame().assign(prediction=self.fitted.predict(df))
-            return pd.concat([df, pred], axis=1)
+            pred = pd.DataFrame().assign(prediction=self.fitted.predict(data))
+            return pd.concat([data, pred], axis=1)
 
     def plot(
         self,
         plots="or",
         alpha=0.05,
         intercept=False,
         incl=None,
```

### Comparing `pyrsm-0.8.9/pyrsm/model.py` & `pyrsm-0.9.0/pyrsm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -624,26 +624,26 @@
     norm_y = stats.norm.pdf(norm_x)
     sns.lineplot(x=norm_x, y=norm_y, lw=1, ax=axes[2, 1]).set(
         title="Residuals vs Normal density", xlabel="Residuals"
     )
 
 
 def sim_prediction(
-    df: pd.DataFrame,
+    data: pd.DataFrame,
     vary: list = [],
     nnv: int = 5,
     minq: float = 0,
     maxq: float = 1,
 ) -> pd.DataFrame:
     """
     Simulate data for prediction
 
     Parameters
     ----------
-    df : Pandas DataFrame
+    data : Pandas DataFrame
     vary : List of column names or Dictionary with keys and values to use
     nnv : int
         Number of values to use to simulate the effect of a numeric variable
     minq : float
         Quantile to use for the minimum value of numeric variables
     maxq : float
         Quantile to use for the maximum value of numeric variables
@@ -655,36 +655,36 @@
 
     def fix_value(s):
         if pd.api.types.is_numeric_dtype(s.dtype):
             return s.mean()
         else:
             return s.value_counts().idxmax()
 
-    dct = {c: [fix_value(df[c])] for c in df.columns}
-    dt = df.dtypes
+    dct = {c: [fix_value(data[c])] for c in data.columns}
+    dt = data.dtypes
     if isinstance(vary, dict):
         # user provided values and ranges
         for key, val in vary.items():
             dct[key] = val
     else:
         # auto derived values and ranges
         vary = ifelse(isinstance(vary, str), [vary], vary)
         for v in vary:
-            if pd.api.types.is_numeric_dtype(df[v].dtype):
-                nu = df[v].nunique()
+            if pd.api.types.is_numeric_dtype(data[v].dtype):
+                nu = data[v].nunique()
                 if nu > 2:
                     dct[v] = np.linspace(
-                        np.quantile(df[v], minq),
-                        np.quantile(df[v], maxq),
+                        np.quantile(data[v], minq),
+                        np.quantile(data[v], maxq),
                         min([nu, nnv]),
                     )
                 else:
-                    dct[v] = [df[v].min(), df[v].max()]
+                    dct[v] = [data[v].min(), data[v].max()]
             else:
-                dct[v] = df[v].unique()
+                dct[v] = data[v].unique()
 
     return expand_grid(dct, dt)
 
 
 def scatter_plot(
     fitted, df, nobs: int = 1000, figsize: tuple = None, resid=False
 ) -> None:
```

### Comparing `pyrsm-0.8.9/pyrsm/notebook.py` & `pyrsm-0.9.0/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/perf.py` & `pyrsm-0.9.0/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/props.py` & `pyrsm-0.9.0/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/compare_means.py` & `pyrsm-0.9.0/pyrsm/radiant/compare_means.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session, req
 import webbrowser, nest_asyncio, uvicorn
-import signal, os
+import signal, os, sys, tempfile
 import pyrsm as rsm
 from pyrsm.utils import ifelse
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 
 def ui_summary():
@@ -92,30 +92,41 @@
     "None": "None",
     "scatter": "Scatter plot",
     "density": "Density plot",
     "box": "Box plot",
     "bar": "Bar chart",
 }
 
+plots_extra = (
+    ui.panel_conditional(
+        "input.plots == 'scatter'",
+        ui.input_select(
+            "nobs",
+            "Number of data points plotted:",
+            {1_000: "1,000", -1: "All"},
+        ),
+    ),
+)
+
 
 class basics_compare_means:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
+    def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
                 "Basics > Compare means",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
-                        ru.ui_plot(choices),
+                        ru.ui_plot(choices, plots_extra),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
                 "https://github.com/vnijs/pyrsm/blob/main/examples/basics-compare-means.ipynb",
                 "Compare means example notebook",
@@ -247,15 +258,19 @@
             estimate,
             ret="cm",
             sum_fun=rsm.basics.compare_means.summary,
             sc=summary_code,
         )
 
         def plot_code():
-            return f"""ct.plot(output="{input.plots()}")"""
+            args = {"plots": input.plots(), "nobs": input.nobs()}
+            args_string = ru.drop_default_args(
+                args, rsm.basics.compare_means.plot, ignore=["nobs"]
+            )
+            return f"""cm.plot({args_string})"""
 
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
@@ -272,37 +287,40 @@
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
 def compare_means(
     data_dct: dict = None,
     descriptions_dct: dict = None,
-    open: bool = True,
+    code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
     Launch a Radiant-for-Python app for compare means hypothesis testing
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="salary")
-    rc = basics_compare_means(data_dct, descriptions_dct, open=open)
+    rc = basics_compare_means(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
+
+    # redirect stdout and stderr to the temporary file
+    temp = tempfile.NamedTemporaryFile()
+    sys.stdout = open(temp.name, "w")
+    sys.stderr = open(temp.name, "w")
+
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
-    # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
-    # single_mean(data_dct, descriptions_dct, open=True)
     compare_means()
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.9.0/pyrsm/radiant/goodness.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,192 +1,188 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import io, os, signal
+import signal, io, os, sys, tempfile
 import pyrsm as rsm
-from contextlib import redirect_stdout, redirect_stderr
+from contextlib import redirect_stdout
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "observed": "Observed",
     "expected": "Expected",
     "chisq": "Chi-squared",
     "dev_std": "Deviation std.",
-    "perc_row": "Row percentages",
-    "perc_col": "Column percentages",
-    "perc": "Table percentages",
 }
 
 
 def ui_summary():
     return ui.panel_conditional(
         "input.tabs == 'Summary'",
         ui.panel_well(
-            ui.output_ui("ui_var1"),
-            ui.output_ui("ui_var2"),
+            ui.output_ui("ui_var"),
+            ru.input_return_text_area(
+                "probs",
+                label="Probabilities:",
+                placeholder="Insert list [1/2, 1/2]",
+                value=None,
+            ),
             ui.input_checkbox_group(
-                id="select_output",
+                id="output",
                 label="Select output tables:",
                 choices=choices,
             ),
         ),
     )
 
 
 plots = {"None": "None"}
 plots.update(choices)
 
 
-class basics_cross_tabs:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
+class basics_goodness:
+    def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Cross-tabs",
+                "Basics > Goodness-of-fit",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
                         ru.ui_plot(plots),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",
-                "Cross-tabs example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-goodness.ipynb",
+                "Goodness-of-fit example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
         get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
-        @output(id="ui_var1")
+        @output(id="ui_var")
         @render.ui
         def ui_var1():
             isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
-                id="var1",
-                label="Select a categorical variable:",
-                selected=None,
-                choices=isCat,
-            )
-
-        @output(id="ui_var2")
-        @render.ui
-        def ui_var2():
-            isCat = get_data()["var_types"]["isCat"]
-            if (input.var1() is not None) and (input.var1() in isCat):
-                del isCat[input.var1()]
-
-            return ui.input_select(
-                id="var2",
+                id="var",
                 label="Select a categorical variable:",
                 selected=None,
                 choices=isCat,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
 
+            if ru.is_empty(input.probs()):
+                probs = None
+            else:
+                probs = input.probs()
+
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
-                "var1": input.var1(),
-                "var2": input.var2(),
+                "var": input.var(),
+                "probs": probs,
             }
 
-            args_string = ru.drop_default_args(args, rsm.basics.cross_tabs)
-            return f"""rsm.basics.cross_tabs({args_string})""", code
+            args_string = ru.drop_default_args(
+                args, rsm.basics.goodness, ignore=["data", "probs"]
+            )
+            return f"""rsm.basics.goodness({args_string})""", code
 
         show_code, estimate = mu.make_estimate(
             self,
             input,
             output,
             get_data,
-            fun="basics.cross_tabs",
-            ret="ct",
+            fun="basics.goodness",
+            ret="gf",
             ec=estimation_code,
             run=False,
             debug=True,
         )
 
         def summary_code():
-            args = [c for c in input.select_output()]
-            return f"""ct.summary(output={args})"""
+            args = [c for c in input.output()]
+            return f"""gf.summary(output={args})"""
 
         mu.make_summary(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="ct",
-            sum_fun=rsm.basics.cross_tabs.summary,
+            ret="gf",
+            sum_fun=rsm.basics.goodness.summary,
             sc=summary_code,
         )
 
         def plot_code():
-            return f"""ct.plot(output="{input.plots()}")"""
+            return f"""gf.plot(plots="{input.plots()}")"""
 
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="ct",
+            ret="gf",
             pc=plot_code,
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
             rsm.md(f"```python\n{self.stop_code}\n```")
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
-def cross_tabs(
+def goodness(
     data_dct: dict = None,
     descriptions_dct: dict = None,
-    open: bool = True,
+    code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for cross-tabs hypothesis testing
+    Launch a Radiant-for-Python app for goodness of fit analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
-    rc = basics_cross_tabs(data_dct, descriptions_dct, open=open)
+    rc = basics_goodness(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
+
+    # redirect stdout and stderr to the temporary file
+    temp = tempfile.NamedTemporaryFile()
+    sys.stdout = open(temp.name, "w")
+    sys.stderr = open(temp.name, "w")
+
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    import pyrsm as rsm
-
-    # newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
-    # data_dct, descriptions_dct = ru.get_dfs(name="newspaper")
-    # cross_tabs(data_dct, descriptions_dct, open=True)
-    # cross_tabs()
+    goodness()
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/goodness.py` & `pyrsm-0.9.0/pyrsm/basics/goodness.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,180 @@
-from shiny import App, render, ui, reactive, Inputs, Outputs, Session
-import webbrowser, nest_asyncio, uvicorn
-import io, os, signal
-import pyrsm as rsm
-from contextlib import redirect_stdout
-import pyrsm.radiant.utils as ru
-
-choices = {
-    "observed": "Observed",
-    "expected": "Expected",
-    "chisq": "Chi-squared",
-    "dev_std": "Deviation std.",
-}
-
-
-def ui_summary():
-    return ui.panel_conditional(
-        "input.tabs == 'Summary'",
-        ui.panel_well(
-            ui.output_ui("ui_var"),
-            ui.input_numeric(
-                "prob_1", "Probability 1", value=0.9, min=0, max=1, step=0.01
-            ),
-            ui.input_numeric(
-                "prob_2", "Probability 2", value=0.9, min=0, max=1, step=0.01
-            ),
-            ui.input_checkbox_group(
-                id="select_output",
-                label="Select output tables:",
-                choices=choices,
-            ),
-        ),
-    )
-
-
-def ui_plot():
-    plots = {"None": "None"}
-    plots.update(choices)
-    return (
-        ui.panel_conditional(
-            "input.tabs == 'Plot'",
-            ui.panel_well(
-                ui.input_select(
-                    id="select_plot",
-                    label="Select plot:",
-                    choices=plots,
-                ),
-            ),
-        ),
-    )
-
-
-def ui_main():
-    return ui.navset_tab_card(
-        ru.ui_data_main(),
-        ui.nav(
-            "Summary",
-            ui.output_ui("show_summary_code"),
-            ui.output_text_verbatim("summary"),
-        ),
-        ui.nav(
-            "Plot",
-            ui.output_ui("show_plot_code"),
-            ui.output_plot("plot", height="500px", width="700px"),
-        ),
-        id="tabs",
-    )
-
-
-class basics_goodness:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
-
-    def shiny_ui(self):
-        return ui.page_navbar(
-            ru.head_content(),
-            ui.nav(
-                "Basics > Goodness-of-fit",
-                ui.row(
-                    ui.column(
-                        3,
-                        ru.ui_data(self),
-                        ui_summary(),
-                        ui_plot(),
+from cmath import sqrt
+import matplotlib.pyplot as plt
+import pandas as pd
+from pyrsm.utils import ifelse
+from pyrsm.radiant import utils as ru
+from typing import Optional, Union
+from scipy.stats import chisquare
+
+
+class goodness:
+    def __init__(
+        self,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
+        var: str,
+        probs: Optional[tuple[float, ...]] = None,
+        figsize: tuple[float, float] = None,
+    ) -> None:
+        if isinstance(data, dict):
+            self.name = list(data.keys())[0]
+            self.data = data[self.name]
+        else:
+            self.data = data
+            self.name = "Not provided"
+
+        self.var = var
+        self.figsize = figsize
+        self.probs = probs
+
+        self.freq = self.data[self.var].value_counts().to_dict()
+        self.nlev = len(self.freq)
+        if self.probs is None:
+            self.probs = [1 / self.nlev] * self.nlev
+
+        self.observed = pd.DataFrame(
+            {k: [v] for k, v in self.freq.items()},
+            columns=sorted(self.freq.keys()),
+        )
+        self.observed["Total"] = self.observed[list(self.observed.columns)].sum(axis=1)
+        self.expected = pd.DataFrame(
+            {
+                sorted(self.freq.keys())[i]: [
+                    self.probs[i] * self.observed.at[0, "Total"],
+                ]
+                for i in range(len(self.freq.keys()))
+            },
+            columns=sorted(self.freq.keys()),
+        )
+        self.expected["Total"] = self.expected[list(self.expected.columns)].sum(axis=1)
+        self.chisq = pd.DataFrame(
+            {
+                column: [
+                    round(
+                        (
+                            (self.observed.at[0, column] - self.expected.at[0, column])
+                            ** 2
+                        )
+                        / self.expected.at[0, column],
+                        2,
+                    ),
+                ]
+                for column in self.expected.columns.tolist()[:-1]
+            },
+            columns=self.expected.columns.tolist(),
+        )
+        self.chisq["Total"] = self.chisq[list(self.chisq.columns)].sum(axis=1)
+
+        self.stdev = pd.DataFrame(
+            {
+                column: [
+                    round(
+                        (self.observed.at[0, column] - self.expected.at[0, column])
+                        / sqrt(self.expected.at[0, column]).real,
+                        2,
                     ),
-                    ui.column(8, ru.ui_main_basics()),
-                ),
-            ),
-            ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",  # no example notebook for goodness of fit
-                "Goodness-of-fit example notebook",
-            ),
-            ru.ui_stop(),
-            title="Radiant for Python",
-            inverse=True,
-            id="navbar_id",
-        )
-
-    def shiny_server(self, input: Inputs, output: Outputs, session: Session):
-        # --- section standard for all apps ---
-        get_data = ru.make_data_elements(self, input, output)
-
-        # --- section unique to each app ---
-        @output(id="ui_var")
-        @render.ui
-        def ui_var1():
-            isCat = get_data()["var_types"]["isCat"]
-            return ui.input_select(
-                id="var",
-                label="Select a categorical variable:",
-                selected=None,
-                choices=isCat,
+                ]
+                for column in self.expected.columns.tolist()[:-1]
+            },
+            columns=self.expected.columns.tolist()[:-1],
+        )
+
+    def summary(
+        self, output: list[str] = ["observed", "expected"], dec: int = 3
+    ) -> None:
+
+        pd.set_option("display.max_columns", 20)
+        pd.set_option("display.max_rows", 20)
+
+        output = ifelse(isinstance(output, str), [output], output)
+
+        print("Goodness of fit test")
+        print(f"Data         : {self.name}")
+        if self.var not in self.data.columns:
+            raise ValueError(f"{self.var} does not exist in chosen dataset")
+
+        print(f"Variable     : {self.var}")
+        if self.nlev != len(self.probs):
+            raise ValueError(
+                f'Number of elements in "probs" should match the number of levels in {self.var} ({self.nlev})'
             )
 
-        def estimation_code():
-            data_name, code = (get_data()[k] for k in ["data_name", "code"])
+        if not 0.999 <= sum(self.probs) <= 1.001:
+            raise ValueError("Probabilities do not sum to 1 ({sum(self.probs)})")
+
+        print(f'Probabilities: {" ".join(map(str, self.probs))}')
+        print(
+            f"Null hyp.    : The distribution of {self.var} is consistent with the specified distribution"
+        )
+        print(
+            f"Alt. hyp.    : The distribution of {self.var} is not consistent with the specified distribution"
+        )
+
+        if "observed" in output:
+            print("\nObserved:")
+            print(self.observed.to_string(index=False))
+
+        if "expected" in output:
+            print("\nExpected: total x p")
+            print(self.expected.to_string(index=False))
+
+        if "chisq" in output:
+            print("\nContribution to chi-squared: (observed - expected) ^ 2 / expected")
+            print(self.chisq.to_string(index=False))
+
+        if "dev_std" in output:
+            print("\nDeviation standardized: (observed - expected) / sqrt(expected)\n")
+            print(self.stdev.to_string(index=False))
+
+        chisq, p_val = chisquare(
+            [self.freq[key] for key in sorted(self.freq.keys())],
+            [self.expected.at[0, key] for key in sorted(self.freq.keys())],
+        )
+
+        if p_val < 0.001:
+            p_val = "< .001"
+        else:
+            p_val = round(p_val, dec)
+        print(
+            f"\nChi-squared: {round(chisq, dec)} df ({self.nlev - 1}), p.value {p_val}"
+        )
+
+    def plot(self, plots: list[str] = [], **kwargs) -> None:
+        plots = ifelse(isinstance(plots, str), [plots], plots)
 
-            args = {
-                "data": f"""{{"{data_name}": {data_name}}}""",
-                "variable": input.var(),
-                "probabilities": (input.prob_1(), input.prob_2()),
-            }
-
-            args_string = ru.drop_default_args(args, rsm.basics.goodness)
-            return f"""rsm.basics.goodness({args_string})""", code
-
-        def show_code():
-            sc = estimation_code()
-            return f"""{sc[1]}\nct = {sc[0]}"""
-
-        @reactive.Calc
-        def estimate():
-            locals()[input.datasets()] = self.datasets[
-                input.datasets()
-            ]  # get data into local scope
-            return eval(estimation_code()[0])
-
-        def summary_code():
-            args = [c for c in input.select_output()]
-            return f"""gf.summary(output={args})"""
-
-        @output(id="show_summary_code")
-        @render.text
-        def show_summary_code():
-            cmd = f"""{show_code()}\n{summary_code()}"""
-            return ru.code_formatter(cmd, self)
-
-        @output(id="summary")
-        @render.text
-        def summary():
-            out = io.StringIO()
-            with redirect_stdout(out):
-                gf = estimate()  # get the reactive object into local scope
-                eval(summary_code())
-            return out.getvalue()
-
-        def plot_code():
-            return f"""gf.plot(output="{input.select_plot()}")"""
-
-        @output(id="show_plot_code")
-        @render.text
-        def show_plot_code():
-            plots = input.select_plot()
-            if plots != "None":
-                cmd = f"""{show_code()}\n{plot_code()}"""
-                return ru.code_formatter(cmd, self)
-
-        @output(id="plot")
-        @render.plot
-        def plot():
-            plots = input.select_plot()
-            if plots != "None":
-                gf = estimate()  # get reactive object into local scope
-                cmd = f"""{plot_code()}"""
-                return eval(cmd)
-
-        # --- section standard for all apps ---
-        # stops returning code if moved to utils
-        @reactive.Effect
-        @reactive.event(input.stop, ignore_none=true)
-        async def stop_app():
-            rsm.md(f"```python\n{self.stop_code}\n```")
-            await session.app.stop()
-            os.kill(os.getpid(), signal.sigterm)
-
-
-def goodness(
-    data_dct: dict,
-    descriptions_dct: dict = None,
-    open: bool = True,
-    host: str = "0.0.0.0",
-    port: int = 8000,
-    log_level: str = "warning",
-):
-    """
-    Launch a Radiant-for-Python app for goodness of fit analysis
-    """
-    rc = basics_goodness(data_dct, descriptions_dct, open=open)
-    nest_asyncio.apply()
-    webbrowser.open(f"http://{host}:{port}")
-    print(f"Listening on http://{host}:{port}")
-    ru.message()
-    uvicorn.run(
-        App(rc.shiny_ui(), rc.shiny_server),
-        host=host,
-        port=port,
-        log_level=log_level,
-    )
+        args = {"rot": False}
+        if "observed" in plots:
+            tab = self.observed.copy().drop(columns="Total").transpose()
+            args["title"] = "Observed frequencies"
+            args.update(**kwargs)
+            fig = tab.plot.bar(**args, legend=False)
+        if "expected" in plots:
+            tab = self.expected.copy().drop(columns="Total").transpose()
+            args["title"] = "Expected frequencies"
+            args.update(**kwargs)
+            fig = tab.plot.bar(**args, legend=False)
+        if "chisq" in plots:
+            tab = self.chisq.drop(columns="Total").transpose()
+            args["title"] = "Contribution to chi-squared statistic"
+            args.update(**kwargs)
+            fig = tab.plot.bar(**args, legend=False)
+        if "dev_std" in plots:
+            tab = self.stdev.transpose()
+            args["title"] = "Deviation standardized"
+            args.update(**kwargs, legend=False)
+            fig, ax = plt.subplots()
+            tab.plot.bar(**args, ax=ax)
+            ax.axhline(y=1.96, color="black", linestyle="--")
+            ax.axhline(y=1.64, color="black", linestyle="--")
+            ax.axhline(y=-1.96, color="black", linestyle="--")
+            ax.axhline(y=-1.64, color="black", linestyle="--")
+            ax.annotate("95%", xy=(0, 2.1), va="bottom", ha="center")
+            ax.annotate("90%", xy=(0, 1.4), va="top", ha="center")
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
-    rc = basics_goodness(
-        {"newspaper": newspaper}, {"newspaper": newspaper_description}, open=True
-    )
-    app = App(rc.shiny_ui(), rc.shiny_server)
+    data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
+    gf = rsm.basics.goodness(data=data_dct, var="Income", probs=[1 / 2, 1 / 2])
+    gf.summary(output=["observed"])
+    gf.plot(plots=["observed", "expected", "chisq", "dev_std"])
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/logistic.py` & `pyrsm-0.9.0/pyrsm/radiant/logistic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from shiny import App, ui, render, reactive, Inputs, Outputs, Session
-import webbrowser, nest_asyncio, uvicorn, os, signal
+import webbrowser, nest_asyncio, uvicorn
+import signal, os, sys, tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     # "dist": "Distribution",
@@ -51,16 +52,16 @@
         ui.output_ui("ui_incl_evar"),
         ui.output_ui("ui_incl_interactions"),
     ),
 )
 
 
 class model_logistic:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
+    def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
                 "Model > Logistic regression (GLM)",
                 ui.row(
@@ -150,34 +151,40 @@
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
 def logistic(
     data_dct: dict = None,
     descriptions_dct: dict = None,
-    open: bool = True,
+    code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
     Launch a Radiant-for-Python app for logistic regression analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="model")
-    rc = model_logistic(data_dct, descriptions_dct, open=open)
+    rc = model_logistic(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
+
+    # redirect stdout and stderr to the temporary file
+    temp = tempfile.NamedTemporaryFile()
+    sys.stdout = open(temp.name, "w")
+    sys.stderr = open(temp.name, "w")
+
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     # titanic, titanic_description = rsm.load_data(pkg="data", name="titanic")
-    # logistic({"titanic": titanic}, {"titanic": titanic_description}, open=True)
+    # logistic({"titanic": titanic}, {"titanic": titanic_description}, code=True)
     logistic()
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/model_utils.py` & `pyrsm-0.9.0/pyrsm/radiant/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,22 +321,14 @@
     @render.text
     def show_plot_code():
         plots = input.plots()
         if plots != "None":
             cmd = f"""{show_code()}\n{plot_code()}"""
             return ru.code_formatter(cmd, self)
 
-    # functionality not yet available in shiny-for-python
-    # def plot_height():
-    #     plots = input.plots()
-    #     if plots == "pred":
-    #         return "800px"
-    #     else:
-    #         return "1000px"
-
     @reactive.Calc
     def gen_plot():
         locals()[ret] = estimate()
         eval(f"""{plot_code()}""")
         fig = plt.gcf()
         width, height = fig.get_size_inches()  # Get the size in inches
         return fig, width * 96, height * 96
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/regress.py` & `pyrsm-0.9.0/pyrsm/radiant/regress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from shiny import App, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn, os, signal
+import signal, os, io, sys, tempfile
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     "dist": "Distribution",
@@ -55,16 +56,16 @@
         ui.output_ui("ui_incl_evar"),
         ui.output_ui("ui_incl_interactions"),
     ),
 )
 
 
 class model_regress:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
+    def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
                 "Model > Linear regression (OLS)",
                 ui.row(
@@ -137,34 +138,38 @@
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
 def regress(
     data_dct: dict = None,
     descriptions_dct: dict = None,
-    open: bool = True,
+    code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
     Launch a Radiant-for-Python app for linear regression analysis
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="model")
-    rc = model_regress(data_dct, descriptions_dct, open=open)
+    rc = model_regress(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
+
+    # redirect stdout and stderr to the temporary file
+    temp = tempfile.NamedTemporaryFile()
+    sys.stdout = open(temp.name, "w")
+    sys.stderr = open(temp.name, "w")
+
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    # diamonds, diamonds_description = rsm.load_data(pkg="data", name="diamonds")
-    # regress({"diamonds": diamonds}, {"diamonds": diamonds_description}, open=True)
     regress()
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/single_mean.py` & `pyrsm-0.9.0/pyrsm/radiant/cross_tabs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,193 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import signal, os
+import signal, os, sys, tempfile
 import pyrsm as rsm
+from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
+choices = {
+    "observed": "Observed",
+    "expected": "Expected",
+    "chisq": "Chi-squared",
+    "dev_std": "Deviation std.",
+    "perc_row": "Row percentages",
+    "perc_col": "Column percentages",
+    "perc": "Table percentages",
+}
+
 
 def ui_summary():
-    return (
-        ui.panel_conditional(
-            "input.tabs == 'Summary'",
-            ui.panel_well(
-                ui.output_ui("ui_var"),
-                ui.input_select(
-                    id="alt_hyp",
-                    label="Alternative hypothesis:",
-                    selected="two-sided",
-                    choices={
-                        "two-sided": "Two sided",
-                        "greater": "Greater than",
-                        "less": "Less than",
-                    },
-                ),
-                ui.input_slider(
-                    id="conf",
-                    label="Confidence level:",
-                    min=0,
-                    max=1,
-                    value=0.95,
-                ),
-                ui.input_numeric(
-                    id="comp_value",
-                    label="Comparison value:",
-                    value=0,
-                ),
+    return ui.panel_conditional(
+        "input.tabs == 'Summary'",
+        ui.panel_well(
+            ui.output_ui("ui_var1"),
+            ui.output_ui("ui_var2"),
+            ui.input_checkbox_group(
+                id="output",
+                label="Select output tables:",
+                choices=choices,
             ),
         ),
     )
 
 
-choices = {
-    # "None": "None",
-    "hist": "Histogram",
-    # "sim": "Simulate",
-}
+plots = {"None": "None"}
+plots.update(choices)
 
 
-class basics_single_mean:
-    def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
-        ru.init(self, datasets, descriptions=descriptions, open=open)
+class basics_cross_tabs:
+    def __init__(self, datasets: dict, descriptions=None, code=True) -> None:
+        ru.init(self, datasets, descriptions=descriptions, code=code)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Single mean",
+                "Basics > Cross-tabs",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
-                        ru.ui_plot(choices),
+                        ru.ui_plot(plots),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
-                "Single mean example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",
+                "Cross-tabs example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
         get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
-        @output(id="ui_var")
+        @output(id="ui_var1")
+        @render.ui
+        def ui_var1():
+            isCat = get_data()["var_types"]["isCat"]
+            return ui.input_select(
+                id="var1",
+                label="Select a categorical variable:",
+                selected=None,
+                choices=isCat,
+            )
+
+        @output(id="ui_var2")
         @render.ui
-        def ui_var():
-            isNum = get_data()["var_types"]["isNum"]
+        def ui_var2():
+            isCat = get_data()["var_types"]["isCat"]
+            if (input.var1() is not None) and (input.var1() in isCat):
+                del isCat[input.var1()]
+
             return ui.input_select(
-                id="var",
-                label="Variable (select one)",
+                id="var2",
+                label="Select a categorical variable:",
                 selected=None,
-                choices=isNum,
+                choices=isCat,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
 
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
-                "var": input.var(),
-                "alt_hyp": input.alt_hyp(),
-                "conf": input.conf(),
-                "comp_value": input.comp_value(),
+                "var1": input.var1(),
+                "var2": input.var2(),
             }
 
-            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
-            return f"""rsm.basics.single_mean({args_string})""", code
+            args_string = ru.drop_default_args(args, rsm.basics.cross_tabs)
+            return f"""rsm.basics.cross_tabs({args_string})""", code
 
         show_code, estimate = mu.make_estimate(
             self,
             input,
             output,
             get_data,
-            fun="basics.single_mean",
-            ret="sm",
+            fun="basics.cross_tabs",
+            ret="ct",
             ec=estimation_code,
             run=False,
             debug=True,
         )
 
         def summary_code():
-            return f"""sm.summary()"""
+            args = [c for c in input.output()]
+            return f"""ct.summary(output={args})"""
 
         mu.make_summary(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="sm",
-            sum_fun=rsm.basics.single_mean.summary,
+            ret="ct",
+            sum_fun=rsm.basics.cross_tabs.summary,
             sc=summary_code,
         )
 
+        def plot_code():
+            return f"""ct.plot(plots="{input.plots()}")"""
+
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="sm",
+            ret="ct",
+            pc=plot_code,
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
             rsm.md(f"```python\n{self.stop_code}\n```")
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
-def single_mean(
+def cross_tabs(
     data_dct: dict = None,
     descriptions_dct: dict = None,
-    open: bool = True,
+    code: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for single_mean hypothesis testing
+    Launch a Radiant-for-Python app for cross-tabs hypothesis testing
     """
     if data_dct is None:
-        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="demand_uk")
-    rc = basics_single_mean(data_dct, descriptions_dct, open)
+        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
+    rc = basics_cross_tabs(data_dct, descriptions_dct, code=code)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
+
+    # redirect stdout and stderr to the temporary file
+    temp = tempfile.NamedTemporaryFile()
+    sys.stdout = open(temp.name, "w")
+    sys.stderr = open(temp.name, "w")
+
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    import pyrsm as rsm
-
-    # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
-    # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
-    # single_mean(data_dct, descriptions_dct, open=True)
-    single_mean()
+    cross_tabs()
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/utils.py` & `pyrsm-0.9.0/pyrsm/radiant/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from htmltools import tags, div, css
 from itertools import combinations
 from shiny import render, ui, reactive
 from faicons import icon_svg
 from pathlib import Path
 import pandas as pd
 import polars as pl
-from pyrsm.utils import ifelse, md
+from pyrsm.utils import ifelse
 from pyrsm.example_data import load_data
 
 
 def get_dfs(pkg=None, name=None, obj=pd.DataFrame):
     data_dct = {k: v for k, v in globals().items() if isinstance(v, obj)}
     descriptions_dct = {
         k: globals()[f"{k}_description"]
@@ -36,23 +36,30 @@
 
 
 def head_content():
     """
     Return the head content for the shiny app
     """
 
-    www_dir = Path(__file__).parent / "www"  # (8)
+    www_dir = Path(__file__).parent / "www"
+    ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png")
+
+    www_dir = Path(__file__).parent / "www"
     return ui.head_content(
         # from https://github.com/rstudio/py-shiny/issues/491#issuecomment-1579138681
         ui.tags.link(
             href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/agate.min.css",
             rel="stylesheet",
         ),
-        ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png"),
-        ui.tags.style((www_dir / "style.css").read_text()),
+        # ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png"),
+        ui.tags.link(rel="icon", type="image/png", href=f"{www_dir}/imgs/icon.png"),
+        ui.include_css((www_dir / "style.css")),
+        # ui.include_js(www_dir / "js/returnTextAreaBinding.js"),
+        # ui.include_js(www_dir / "js/radiantUI.js"), # too slow on startup? Throws an error
+        # ui.include_js(www_dir / "js/screenshot.js"),
         ui.tags.script(
             (www_dir / "js/returnTextAreaBinding.js").read_text(),
         ),
         ui.tags.script(
             (www_dir / "js/radiantUI.js").read_text(),
         ),
         ui.tags.script(
@@ -63,15 +70,15 @@
         ),
         ui.tags.script(
             src="//html2canvas.hertzen.com/dist/html2canvas.min.js",
         ),
     )
 
 
-def init(self, datasets, descriptions=None, open=True):
+def init(self, datasets, descriptions=None, code=True):
     """
     Initialize key 'self' values to be used in an app class
     """
     self.datasets = ifelse(isinstance(datasets, dict), datasets, {"dataset": datasets})
     if descriptions is None:
         self.descriptions = {
             k: "## No data description provided" for k in self.datasets.keys()
@@ -79,24 +86,24 @@
     else:
         self.descriptions = ifelse(
             isinstance(descriptions, dict),
             descriptions,
             {"description": descriptions},
         )
     self.dataset_list = list(datasets.keys())
-    self.open = open  # keep code windows open or closed by default
+    self.code = code  # keep code windows open or closed by default
     self.stop_code = ""
 
 
 def escape_quotes(cmd):
     return cmd.replace('"', '\\"').replace("'", "\\'")
 
 
-def quote(v, k):
-    if isinstance(v, str) and k not in ["data", "df"] and not (v[0] + v[-1] == "{}"):
+def quote(v, k, ignore=["data"]):
+    if isinstance(v, str) and k not in ignore and not (v[0] + v[-1] == "{}"):
         v = escape_quotes(v)
         return f'"{v}"'
     else:
         return v
 
 
 def copy_icon(cmd):
@@ -115,35 +122,42 @@
 def code_formatter(code, self):
     """
     Format python code using black
     """
     cmd = self.stop_code = black.format_str(code, mode=black.Mode())
     return ui.TagList(
         ui.HTML(
-            f"<details {ifelse(self.open, 'open', '')}><summary>View generated python code</summary>"
+            f"<details {ifelse(self.code, 'open', '')}><summary>View generated python code</summary>"
         ),
         copy_icon(cmd),
         ui.markdown(f"""\n```python\n{cmd.rstrip()}\n```"""),
         ui.tags.script("hljs.highlightAll();"),
         ui.HTML("</details>"),
         ui.br(),
     )
 
 
-def drop_default_args(args, func):
+def drop_default_args(args, func, ignore=["data"]):
     """
     Take a dictionary of arguments for a function and compare
     to the default arguments for that function
     Return a comma separate string of key-value pairs for
     non-default values where the value is quoted if it is a string
     """
     sig = inspect.signature(func).parameters
     keep = {k: args[k] for k, v in sig.items() if k in args and args[k] != v.default}
 
-    return ", ".join(f"{k}={quote(v, k)}" for k, v in keep.items())
+    return ", ".join(f"{k}={quote(v, k, ignore)}" for k, v in keep.items())
+
+
+def make_side_by_side(a, b):
+    """Put two inputs side-by-side in the UI"""
+    return ui.tags.table(
+        ui.tags.td(a, width="50%"), ui.tags.td(b, width="50%"), width="100%"
+    )
 
 
 def get_data(self, input):
     """
     Set up data access for the app
     """
     data_name = input.datasets()
@@ -354,15 +368,14 @@
             "Summary",
             ui.output_ui("show_summary_code"),
             ui.output_text_verbatim("summary"),
         ),
         ui.nav(
             "Plot",
             ui.output_ui("show_plot_code"),
-            # ui.output_plot("plot", height=height, width=width),
             ui.output_ui("plot_container"),
         ),
         id="tabs",
     )
 
 
 def ui_main_model():
```

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.9.0/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-nc-sa.png` & `pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-sa.png` & `pyrsm-0.9.0/pyrsm/radiant/www/imgs/by-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/imgs/icon.png` & `pyrsm-0.9.0/pyrsm/radiant/www/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/js/returnTextAreaBinding.js` & `pyrsm-0.9.0/pyrsm/radiant/www/js/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/js/screenshot.js` & `pyrsm-0.9.0/pyrsm/radiant/www/js/screenshot.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/radiant/www/style.css` & `pyrsm-0.9.0/pyrsm/radiant/www/style.css`

 * *Files 11% similar despite different names*

```diff
@@ -3,39 +3,43 @@
 }
 
 /* based on https://stackoverflow.com/a/30338814/1974918*/
 details pre {
     padding: 0;
 }
 
+#pc_well {
+    background-color: #ffffff;
+}
+
 pre {
     overflow: auto;
     white-space: pre;
     word-wrap: normal;
     background-color: #ffffff;
 }
 
 code,
 pre code {
     overflow: auto;
     white-space: pre;
     word-wrap: normal;
 }
 
-
 #copy {
     position: absolute;
     right: 14px;
     font-size: 14px;
-    color: white;
+    color: grey;
     padding: 5px;
-    opacity: 0.5;
+    opacity: 1;
 }
 
 #copy:hover {
+    color: white;
     opacity: 0.9;
 }
 
 #copy:active {
     opacity: 0.5;
 }
```

### Comparing `pyrsm-0.8.9/pyrsm/regress.py` & `pyrsm-0.9.0/pyrsm/regress.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,38 +142,42 @@
             else:
                 print("\nVariance inflation factors:")
                 print(f"\n{calc_vif(self.fitted).to_string()}")
 
         if test is not None and len(test) > 0:
             self.f_test(test=test, dec=dec)
 
-    def predict(self, df=None, cmd=None, dc=False, ci=False, conf=0.95) -> pd.DataFrame:
+    def predict(
+        self, data=None, cmd=None, dc=False, ci=False, conf=0.95
+    ) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
-        if df is None:
-            df = self.data
-        df = df.loc[:, self.evar].copy()
+        if data is None:
+            data = self.data
+        data = data.loc[:, self.evar].copy()
         if cmd is not None:
             if dc:
                 for k, v in cmd.items():
-                    df[k] = v
+                    data[k] = v
             else:
-                df = sim_prediction(df=df, vary=cmd)
+                data = sim_prediction(data=data, vary=cmd)
 
         if ci:
             if dc:
                 raise ValueError(
                     "Confidence intervals not available when using the Data & Command option"
                 )
             else:
-                return pd.concat([df, predict_ci(self.fitted, df, conf=conf)], axis=1)
+                return pd.concat(
+                    [data, predict_ci(self.fitted, data, conf=conf)], axis=1
+                )
         else:
-            pred = pd.DataFrame().assign(prediction=self.fitted.predict(df))
-            return pd.concat([df, pred], axis=1)
+            pred = pd.DataFrame().assign(prediction=self.fitted.predict(data))
+            return pd.concat([data, pred], axis=1)
 
     def plot(
         self,
         plots="dist",
         nobs: int = 1000,
         intercept=False,
         alpha=0.05,
```

### Comparing `pyrsm-0.8.9/pyrsm/stats.py` & `pyrsm-0.9.0/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/utils.py` & `pyrsm-0.9.0/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm/visualize.py` & `pyrsm-0.9.0/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.9.0/pyrsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.9/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.9.0/pyrsm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 pyrsm/data/multivariate/tpbrands_description.md
 pyrsm/radiant/__init__.py
 pyrsm/radiant/compare_means.py
 pyrsm/radiant/cross_tabs.py
 pyrsm/radiant/goodness.py
 pyrsm/radiant/logistic.py
 pyrsm/radiant/model_utils.py
+pyrsm/radiant/probability_calculator.py
 pyrsm/radiant/regress.py
 pyrsm/radiant/single_mean.py
 pyrsm/radiant/utils.py
 pyrsm/radiant/www/.DS_Store
 pyrsm/radiant/www/style.css
 pyrsm/radiant/www/imgs/by-nc-sa.png
 pyrsm/radiant/www/imgs/by-sa.png
```

### Comparing `pyrsm-0.8.9/setup.cfg` & `pyrsm-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_basics.py` & `pyrsm-0.9.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_bins.py` & `pyrsm-0.9.0/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_example_data.py` & `pyrsm-0.9.0/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_perf.py` & `pyrsm-0.9.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_regression.py` & `pyrsm-0.9.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_stats.py` & `pyrsm-0.9.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.9/tests/test_utils.py` & `pyrsm-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

