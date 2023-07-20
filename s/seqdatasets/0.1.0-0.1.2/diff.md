# Comparing `tmp/seqdatasets-0.1.0.tar.gz` & `tmp/seqdatasets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqdatasets-0.1.0.tar", max compression
+gzip compressed data, was "seqdatasets-0.1.2.tar", max compression
```

## Comparing `seqdatasets-0.1.0.tar` & `seqdatasets-0.1.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1066 2023-05-23 18:53:08.000000 seqdatasets-0.1.0/LICENSE
--rw-r--r--   0        0        0       14 2023-05-23 18:48:30.000000 seqdatasets-0.1.0/README.md
--rw-r--r--   0        0        0      351 2023-06-23 20:14:55.000000 seqdatasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      314 2023-06-14 18:43:55.000000 seqdatasets-0.1.0/seqdatasets/__init__.py
--rw-r--r--   0        0        0    12621 2023-06-14 19:05:15.000000 seqdatasets-0.1.0/seqdatasets/_datasets.py
--rw-r--r--   0        0        0     2684 2023-06-14 19:10:11.000000 seqdatasets-0.1.0/seqdatasets/_utils.py
--rw-r--r--   0        0        0     3554 2023-01-26 02:27:24.000000 seqdatasets-0.1.0/seqdatasets/datasets.csv
--rw-r--r--   0        0        0   320826 2023-01-26 02:27:25.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.tsv
--rw-r--r--   0        0        0       23 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/.zattrs
--rw-r--r--   0        0        0       24 2023-05-23 19:14:54.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/.zgroup
--rw-r--r--   0        0        0    13947 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/.zmetadata
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_0/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_0/.zattrs
--rw-r--r--   0        0        0     7047 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_0/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_1/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_1/.zattrs
--rw-r--r--   0        0        0     7047 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_1/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_2/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_2/.zattrs
--rw-r--r--   0        0        0     7048 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_2/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_3/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_3/.zattrs
--rw-r--r--   0        0        0     7047 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_3/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_4/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_4/.zattrs
--rw-r--r--   0        0        0     7051 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_4/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_5/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_5/.zattrs
--rw-r--r--   0        0        0     7045 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_5/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_6/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_6/.zattrs
--rw-r--r--   0        0        0     7048 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_6/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_7/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_7/.zattrs
--rw-r--r--   0        0        0     7048 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_7/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_8/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_8/.zattrs
--rw-r--r--   0        0        0     7045 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_8/0
--rw-r--r--   0        0        0      319 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_9/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_9/.zattrs
--rw-r--r--   0        0        0     7045 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_9/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_0/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_0/.zattrs
--rw-r--r--   0        0        0      244 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_0/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_1/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_1/.zattrs
--rw-r--r--   0        0        0      244 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_1/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_2/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_2/.zattrs
--rw-r--r--   0        0        0      244 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_2/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_3/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_3/.zattrs
--rw-r--r--   0        0        0      241 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_3/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_4/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_4/.zattrs
--rw-r--r--   0        0        0      244 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_4/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_5/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_5/.zattrs
--rw-r--r--   0        0        0      251 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_5/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_6/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_6/.zattrs
--rw-r--r--   0        0        0      243 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_6/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_7/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_7/.zattrs
--rw-r--r--   0        0        0      243 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_7/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_8/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_8/.zattrs
--rw-r--r--   0        0        0      235 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_8/0
--rw-r--r--   0        0        0      317 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_9/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:17.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_9/.zattrs
--rw-r--r--   0        0        0      247 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/label_9/0
--rw-r--r--   0        0        0      369 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/name/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/name/.zattrs
--rw-r--r--   0        0        0      556 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/name/0
--rw-r--r--   0        0        0      370 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/seq/.zarray
--rw-r--r--   0        0        0       56 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/seq/.zattrs
--rw-r--r--   0        0        0    29157 2023-05-25 21:45:16.000000 seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/seq/0
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 seqdatasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/LICENSE
+-rw-r--r--   0        0        0       14 2023-05-23 18:48:30.000000 seqdatasets-0.1.2/README.md
+-rw-r--r--   0        0        0      351 2023-07-20 19:58:31.000000 seqdatasets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      314 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/__init__.py
+-rw-r--r--   0        0        0    12980 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/_datasets.py
+-rw-r--r--   0        0        0     2684 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/_utils.py
+-rw-r--r--   0        0        0     3554 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/datasets.csv
+-rw-r--r--   0        0        0   320826 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.tsv
+-rw-r--r--   0        0        0       23 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/.zattrs
+-rw-r--r--   0        0        0       24 2023-07-20 18:29:48.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/.zgroup
+-rw-r--r--   0        0        0    13947 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/.zmetadata
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_0/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_0/.zattrs
+-rw-r--r--   0        0        0     7047 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_0/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_1/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_1/.zattrs
+-rw-r--r--   0        0        0     7047 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_1/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_2/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_2/.zattrs
+-rw-r--r--   0        0        0     7048 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_2/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_3/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_3/.zattrs
+-rw-r--r--   0        0        0     7047 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_3/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_4/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_4/.zattrs
+-rw-r--r--   0        0        0     7051 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_4/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_5/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_5/.zattrs
+-rw-r--r--   0        0        0     7045 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_5/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_6/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_6/.zattrs
+-rw-r--r--   0        0        0     7048 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_6/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_7/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_7/.zattrs
+-rw-r--r--   0        0        0     7048 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_7/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_8/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_8/.zattrs
+-rw-r--r--   0        0        0     7045 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_8/0
+-rw-r--r--   0        0        0      319 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_9/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_9/.zattrs
+-rw-r--r--   0        0        0     7045 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_9/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_0/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_0/.zattrs
+-rw-r--r--   0        0        0      244 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_0/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_1/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_1/.zattrs
+-rw-r--r--   0        0        0      244 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_1/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_2/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_2/.zattrs
+-rw-r--r--   0        0        0      244 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_2/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_3/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_3/.zattrs
+-rw-r--r--   0        0        0      241 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_3/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_4/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_4/.zattrs
+-rw-r--r--   0        0        0      244 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_4/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_5/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_5/.zattrs
+-rw-r--r--   0        0        0      251 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_5/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_6/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_6/.zattrs
+-rw-r--r--   0        0        0      243 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_6/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_7/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_7/.zattrs
+-rw-r--r--   0        0        0      243 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_7/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_8/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_8/.zattrs
+-rw-r--r--   0        0        0      235 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_8/0
+-rw-r--r--   0        0        0      317 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_9/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_9/.zattrs
+-rw-r--r--   0        0        0      247 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/label_9/0
+-rw-r--r--   0        0        0      369 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/name/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/name/.zattrs
+-rw-r--r--   0        0        0      556 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/name/0
+-rw-r--r--   0        0        0      370 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/seq/.zarray
+-rw-r--r--   0        0        0       56 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/seq/.zattrs
+-rw-r--r--   0        0        0    29157 2023-07-20 18:29:49.000000 seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/seq/0
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 seqdatasets-0.1.2/PKG-INFO
```

### Comparing `seqdatasets-0.1.0/LICENSE` & `seqdatasets-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/_datasets.py` & `seqdatasets-0.1.2/seqdatasets/_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,8 +317,20 @@
             sdata = sdata.merge(meta_xr)
             sd.to_zarr(sdata, outzarr, mode="w")
         else:
             print("Zarr file found. Opening existing zarr file.")
             sdata = sd.open_zarr(outzarr)
         return sdata
     else:
-        return paths
+        return paths
+
+def kopp21(
+    dataset="jund_binary", 
+    download_dir: str = None,
+    batch_size: int = 1000,
+    return_sdata=True, 
+):
+    if dataset == "":
+        sdata = sd.open_zarr("/cellar/users/aklie/data/eugene/revision/kopp21/kopp21_test.zarr")
+    else:
+        raise ValueError("dataset must be either 'jund_binary' or 'jund_continuous'.")
+    return sdata
```

### Comparing `seqdatasets-0.1.0/seqdatasets/_utils.py` & `seqdatasets-0.1.2/seqdatasets/_utils.py`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/datasets.csv` & `seqdatasets-0.1.2/seqdatasets/datasets.csv`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.tsv` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.tsv`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/.zmetadata` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_0/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_0/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_1/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_1/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_2/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_2/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_3/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_3/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_4/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_4/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_5/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_5/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_6/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_6/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_7/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_7/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_8/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_8/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/activity_9/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/activity_9/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/name/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/name/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/seqdatasets/random1000/random1000_seqs.zarr/seq/0` & `seqdatasets-0.1.2/seqdatasets/random1000/random1000_seqs.zarr/seq/0`

 * *Files identical despite different names*

### Comparing `seqdatasets-0.1.0/PKG-INFO` & `seqdatasets-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: seqdatasets
-Version: 0.1.0
+Version: 0.1.2
 Summary: Datasets for benchmarking, testing and developing in EUGENe
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: seqdata (==0.1.1)
+Requires-Dist: seqdata (>=0.1.1,<0.2.0)
 Requires-Dist: wget (==3.2)
 Description-Content-Type: text/markdown
 
 # SeqDatasets
```

