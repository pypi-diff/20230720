# Comparing `tmp/arkindex-cli-0.2.6.tar.gz` & `tmp/arkindex-cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-cli-0.2.6.tar", last modified: Wed Jun 28 15:37:32 2023, max compression
+gzip compressed data, was "arkindex-cli-0.2.7.tar", last modified: Thu Jul 20 08:33:35 2023, max compression
```

## Comparing `arkindex-cli-0.2.6.tar` & `arkindex-cli-0.2.7.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-28 15:36:31.000000 arkindex-cli-0.2.6/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.659961 arkindex-cli-0.2.6/arkindex_cli/
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/argtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     4208 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2621 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.659961 arkindex-cli-0.2.6/arkindex_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 15:37:29.000000 arkindex-cli-0.2.6/arkindex_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/elements/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8629 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/list.py
--rw-rw-rw-   0 root         (0) root         (0)    13082 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/ml_splits.py
--rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/page_copy.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/reject_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/unlink.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/elements/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/export/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18108 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/alto.py
--rw-rw-rw-   0 root         (0) root         (0)     9577 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    31338 2023-06-28 15:36:31.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/db.py
--rw-rw-rw-   0 root         (0) root         (0)     3175 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/entities.py
--rw-rw-rw-   0 root         (0) root         (0)    12609 2023-06-28 15:36:31.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2702 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/export/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/models/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4060 2023-06-28 15:36:31.000000 arkindex-cli-0.2.6/arkindex_cli/commands/models/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-06-28 15:36:31.000000 arkindex-cli-0.2.6/arkindex_cli/commands/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/process/
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6684 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/process/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/process/recover.py
--rw-rw-rw-   0 root         (0) root         (0)     3049 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/process/report.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/upload/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/upload/alto/
--rw-rw-rw-   0 root         (0) root         (0)    24937 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/alto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8850 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/alto/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     9303 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/iiif.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/
--rw-rw-rw-   0 root         (0) root         (0)     5111 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/minio_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8060 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/commands/upload/page_xml_import.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-06-23 08:28:16.000000 arkindex-cli-0.2.6/arkindex_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:37:32.659961 arkindex-cli-0.2.6/arkindex_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-28 15:37:32.000000 arkindex-cli-0.2.6/arkindex_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-23 08:28:17.000000 arkindex-cli-0.2.6/requirements-export.txt
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-23 08:28:17.000000 arkindex-cli-0.2.6/requirements-tests.txt
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-23 08:28:17.000000 arkindex-cli-0.2.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:37:32.663961 arkindex-cli-0.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-06-23 08:28:17.000000 arkindex-cli-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.863700 arkindex-cli-0.2.7/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-20 08:33:35.863700 arkindex-cli-0.2.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-20 08:32:49.000000 arkindex-cli-0.2.7/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.855700 arkindex-cli-0.2.7/arkindex_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/argtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4208 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2023-07-19 14:21:14.000000 arkindex-cli-0.2.7/arkindex_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 08:33:33.000000 arkindex-cli-0.2.7/arkindex_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/elements/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8629 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    13082 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/ml_splits.py
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/page_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/reject_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/unlink.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/elements/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/export/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17840 2023-07-19 14:21:14.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/alto.py
+-rw-rw-rw-   0 root         (0) root         (0)     9577 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    31338 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    12609 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/export/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/models/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/models/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     8404 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/process/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/process/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3068 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/process/recover.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/process/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/upload/
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/upload/alto/
+-rw-rw-rw-   0 root         (0) root         (0)    24937 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/alto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8850 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/alto/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9303 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/iiif.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.859700 arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/
+-rw-rw-rw-   0 root         (0) root         (0)     5111 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/minio_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8060 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/commands/upload/page_xml_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.863700 arkindex-cli-0.2.7/arkindex_cli/commands/worker/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-19 14:21:14.000000 arkindex-cli-0.2.7/arkindex_cli/commands/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2023-07-19 14:21:14.000000 arkindex-cli-0.2.7/arkindex_cli/commands/worker/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2023-07-19 14:21:14.000000 arkindex-cli-0.2.7/arkindex_cli/git.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/arkindex_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:33:35.855700 arkindex-cli-0.2.7/arkindex_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 08:33:35.000000 arkindex-cli-0.2.7/arkindex_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/requirements-export.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/requirements-tests.txt
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-20 08:32:49.000000 arkindex-cli-0.2.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 08:33:35.863700 arkindex-cli-0.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-07-19 13:43:32.000000 arkindex-cli-0.2.7/setup.py
```

### Comparing `arkindex-cli-0.2.6/PKG-INFO` & `arkindex-cli-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: export
```

### Comparing `arkindex-cli-0.2.6/README.md` & `arkindex-cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/argtypes.py` & `arkindex-cli-0.2.7/arkindex_cli/argtypes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/auth.py` & `arkindex-cli-0.2.7/arkindex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/cli.py` & `arkindex-cli-0.2.7/arkindex_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from arkindex_cli.commands.elements import add_elements_parser
 from arkindex_cli.commands.export import add_export_parser
 from arkindex_cli.commands.login import add_login_parser
 from arkindex_cli.commands.models import add_models_parser
 from arkindex_cli.commands.process import add_process_parser
 from arkindex_cli.commands.secrets import add_secrets_parser
 from arkindex_cli.commands.upload import add_upload_parser
+from arkindex_cli.commands.worker import add_worker_parser
 
 
 def get_version():
     version_file = Path(__file__).absolute().parent.parent / "VERSION"
     if version_file.is_file():
         with version_file.open() as f:
             return f.read().strip()
@@ -55,14 +56,15 @@
     add_elements_parser(subcommands)
     add_export_parser(subcommands)
     add_login_parser(subcommands)
     add_process_parser(subcommands)
     add_secrets_parser(subcommands)
     add_upload_parser(subcommands)
     add_models_parser(subcommands)
+    add_worker_parser(subcommands)
 
     return parser
 
 
 def main():
     # Ignore the deprecation warnings of the SQLite export functions, which are only intended for other scripts.
     warnings.filterwarnings(
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/benchmark.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/benchmark.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/classes.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/classes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/link.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/link.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/list.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/list.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/ml_splits.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/ml_splits.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/page_copy.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/page_copy.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/reject_classifications.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/reject_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/unlink.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/unlink.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/elements/utils.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/elements/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/alto.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/alto.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,17 @@
 import logging
 import xml.etree.ElementTree as ET
 from pathlib import Path
 from typing import List
 from uuid import UUID
 from xml.sax.saxutils import escape
 
-from arkindex_cli.commands.export.db import (
-    Element,
-    element_image,
-    filter_folder_id,
-    get_elements,
-    get_worker_version,
-    list_children,
-    list_folders,
-    recursive_element_transcriptions,
-)
 from arkindex_cli.commands.export.utils import BoundingBox
+from arkindex_export import Element, Image, Transcription, WorkerVersion, open_database
+from arkindex_export.queries import list_children
 
 logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
 logger = logging.getLogger(__name__)
 
 
 def add_alto_parser(subcommands):
     alto_parser = subcommands.add_parser(
@@ -93,15 +85,14 @@
     width, height = max_x - min_x, max_y - min_y
 
     return BoundingBox(min_x, min_y, width, height)
 
 
 def alto_xml_gen(
     folder: Element,
-    database_path,
     output_path: str,
     page_type,
     line_type,
     mets=False,
     **kwargs,
 ):
     """
@@ -109,22 +100,26 @@
     folder element.
     - Write  each page and relative lines as an alto xml file into the parent
     newly created folder at the specified output_path.
     - Write a mets file in the relevant folder, if the option is used.
     """
 
     layout_tag = kwargs.get("layout_tag", None)
-    page_list = list_children(database_path, folder.id, page_type)
+    page_list = (
+        list_children(folder.id)
+        .join(Image, on=(Image.id == Element.image))
+        .where(Element.type == page_type)
+    )
 
     # for the METS file
     alto_files = []
     image_files = []
 
     # validating the folder has pages, if not, no file is created
-    if page_list:
+    if page_list.count():
 
         # folder path to be reused
         folder_path = Path(output_path) / folder.id
         # creating folder directory
         folder_path.mkdir()
 
         # setting the namespaces from alto v3
@@ -179,26 +174,24 @@
 
             # adding page worker id in set and as page attribute if exists
             if page.worker_version_id is not None:
 
                 worker_set.add(page.worker_version_id)
                 alto_page.set("PROCESSINGREFS", f"worker_{page.worker_version_id}")
 
-            # getting the list of Transcriptions namedtuples for each page
-            page_transcriptions = recursive_element_transcriptions(
-                database_path, page.id
+            # getting the list of Transcriptions for each page
+            page_transcriptions = Transcription.select().where(
+                Transcription.element.in_(list_children(page.id))
             )
 
             # creating GraphicalElement tags for layout_tag elements if specified
             if layout_tag:
-                subelements = get_elements(
-                    database_path, folder.id, layout_tag, recursive=True
-                )
+                subelements = list_children(folder.id).where(Element.type == layout_tag)
                 # create the LayoutTag, if there are subelements in the document
-                if len(subelements) > 0:
+                if subelements.count():
                     alto_tags = ET.SubElement(alto_root, "Tags")
                     ET.SubElement(
                         alto_tags,
                         "LayoutTag",
                         attrib={"ID": layout_tag, "LABEL": layout_tag},
                     )
                 for item in subelements:
@@ -229,29 +222,29 @@
                     # creating the xml formatted string for the polygon
                     xml_pol_str = " ".join(
                         f"{x},{y}" for x, y in json.loads(item.polygon)
                     )
                     alto_subelement_polygon.set("POINTS", xml_pol_str)
 
             # adding textblock and textline subelements when page contains transcriptions
-            if page_transcriptions is not None:
+            if page_transcriptions.count():
 
                 # creating a dictionary where keys are lines ids and values are
                 # relative line transcriptions
                 transcriptions_dict = {
                     transcription.element_id: transcription
                     for transcription in page_transcriptions
                 }
 
                 alto_text_block = ET.SubElement(alto_print_space, "TextBlock")
 
                 # For now a page can have a single text block
                 alto_text_block.set("ID", f"page_{page.id}_textblock_{count}")
 
-                for line in list_children(database_path, page.id, line_type):
+                for line in list_children(page.id).where(Element.type == line_type):
 
                     # calling xml_bounding_box to fill textline attributes
                     line_box_dim = xml_bounding_box(line.polygon)
 
                     alto_line = ET.SubElement(
                         alto_text_block,
                         "TextLine",
@@ -307,31 +300,28 @@
                         if worker_version_id is not None:
                             alto_string.set(
                                 "PROCESSINGREFS",
                                 f"worker_{worker_version_id}",
                             )
                             worker_set.add(worker_version_id)
 
-            # calling element_image to get the url to insert in sourceImageInformation
-            # markup
-            image_info = element_image(database_path, page.id)
-            image_url = image_info.url
+            image_url = page.image.url
             alto_image_info = ET.SubElement(alto_description, "sourceImageInformation")
             alto_filename = ET.SubElement(alto_image_info, "fileName")
             alto_filename.text = image_url.split("/")[-1]
             alto_file_id = ET.SubElement(alto_image_info, "fileIdentifier")
             alto_file_id.text = image_url
             alto_doc_id = ET.SubElement(alto_image_info, "documentIdentifier")
             # document identifier is the page id
             alto_doc_id.text = page.id
 
-            for worker_id in worker_set:
+            for worker in WorkerVersion.select().where(
+                WorkerVersion.id.in_(worker_set)
+            ):
                 alto_processing = ET.SubElement(alto_description, "Processing")
-                # calling get_worker_version to get worker namedtuple
-                worker = get_worker_version(database_path, worker_id)
                 alto_processing.set("ID", f"worker_{worker.id}")
                 alto_category = ET.SubElement(alto_processing, "processingCategory")
                 alto_category.text = "contentGeneration"
                 alto_step_desc = ET.SubElement(
                     alto_processing, "processingStepDescription"
                 )
                 alto_step_desc.text = worker.type
@@ -352,20 +342,20 @@
 
             # for the METS file
             alto_files.append(
                 {
                     "id": page.id,
                     "mime": "application/xml",
                     "location": str(alto_file),
-                    "image_id": image_info.id,
+                    "image_id": page.image.id,
                 }
             )
             image_files.append(
                 {
-                    "id": image_info.id,
+                    "id": page.image.id,
                     "mime": "image/jpeg",
                     "location": image_url,
                     "page_id": page.id,
                 }
             )
 
             logger.info(f"created alto xml file at {alto_file}")
@@ -440,20 +430,21 @@
 ):
     database_path = database_path.absolute()
     assert database_path.is_file(), f"Database at {database_path} not found"
 
     output_path = output_path.absolute()
     assert output_path.is_dir(), f"Output path {output_path} is not a valid directory"
 
-    folders = list_folders(database_path, folder_type)
-    if folder_ids is not None:
-        folders = filter_folder_id(folders, folder_ids)
+    open_database(database_path)
+
+    folders = Element.select().where(Element.type == folder_type)
+    if folder_ids:
+        folders = folders.where(Element.id.in_(folder_ids))
 
-    assert folders, f"No '{folder_type}' folders were found"
+    assert folders.count(), f"No '{folder_type}' folders were found"
 
     for folder in folders:
         alto_xml_gen(
             folder,
-            database_path=database_path,
             output_path=output_path,
             **kwargs,
         )
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/csv.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/csv.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/db.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/db.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/entities.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/pdf.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/pdf.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/export/utils.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/export/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/login.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/models/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/models/publish.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/models/publish.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,41 +23,29 @@
 
 def add_publish_parser(subcommands) -> None:
     publish_parser = subcommands.add_parser(
         "publish",
         description="Publish every ML models of this git repository.",
         help="Publish ML models to Arkindex.",
     )
-    publish_parser.add_argument(
-        "--use-parent-folder",
-        action="store_true",
-        default=False,
-        help="Use the parent folder of the models found to build the archive",
-    )
-    publish_parser.add_argument(
-        "--rename",
-        help="Rename the single file of the archive to a different name",
-    )
     publish_parser.set_defaults(func=run)
 
 
 def publish_model(
     client: ArkindexClient,
     name: str,
     configuration: dict,
-    use_parent_folder: bool,
-    rename: Optional[str] = None,
 ) -> None:
     """This takes a model associated to a worker and publishes a new version of the model"""
     logger.info(f"Publishing {name}")
 
     # Find the model file associated
     model_path = configuration.pop("model")
     path_to_model = find_model_path(
-        config_model_path=model_path, use_parent_folder=use_parent_folder
+        config_model_path=model_path,
     )
 
     assert path_to_model, f"The model could not be loaded using {model_path}"
 
     # Try to create a model
     # On 201, use the given id
     # On 400, use the given id key='name'
@@ -70,17 +58,15 @@
         model_id=model_id,
         tag=os.environ.get("CI_COMMIT_TAG"),
         description=name,
         configuration=configuration,
     )
 
     # Create the zst archive, get its hash and size
-    with create_archive(
-        path=path_to_model, rename=rename, use_parent_folder=use_parent_folder
-    ) as (
+    with create_archive(path=path_to_model) as (
         path_to_archive,
         hash,
         size,
         archive_hash,
     ):
         upload_to_s3(archive_path=path_to_archive, model_version_details=model_version)
 
@@ -97,16 +83,14 @@
         logger.warning(
             f"Model version {model_version['id']} has been marked as erroneous and left aside. "
             f"Using existing model version {valid_version['id']}"
         )
 
 
 def run(
-    use_parent_folder: bool = False,
-    rename: Optional[str] = None,
     profile_slug: Optional[str] = None,
 ) -> None:
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Loading API client")
         client = Profiles().get_api_client_or_exit(profile_slug)
 
     # Parse .arkindex.yml => retrieve worker name, path and configuration
@@ -115,16 +99,14 @@
     # For each worker, do_publish
     for worker_name, worker_configuration in workers.items():
         try:
             publish_model(
                 client,
                 worker_name,
                 worker_configuration,
-                use_parent_folder=use_parent_folder,
-                rename=rename,
             )
         except Exception as e:
             msg = getattr(e, "content", repr(e))
             logger.exception(f"{worker_name} publishing has failed with error: {msg}")
             logger.error("Skipping this model.")
 
     logger.info("All done.")
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/models/utils.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/models/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,106 +16,99 @@
 from apistar.exceptions import ErrorResponse
 from arkindex import ArkindexClient
 
 logger = logging.getLogger(__name__)
 CHUNK_SIZE = 1024
 
 
-FilePath = NewType("FilePath", str)
+FilePath = NewType("FilePath", Path)
 Hash = NewType("Hash", str)
 FileSize = NewType("FileSize", int)
 Archive = Tuple[FilePath, Hash, FileSize]
 
 # Teklia's convention
-DEFAULT_MODEL_DIR = "/usr/share/teklia/"
+DEFAULT_MODEL_DIR = Path("/usr/share/teklia")
 
 
 def build_clean_payload(**kwargs):
     """
     Remove null attributes from an API body payload
     """
     return {key: value for key, value in kwargs.items() if value is not None}
 
 
-def find_model_path(config_model_path: str, use_parent_folder: bool = False) -> str:
+def find_model_path(config_model_path: str) -> Path:
     """We try the following paths in that order and return the first that exists
     - /usr/share/teklia/${config_model_path}
     - ${config_model_path}
     - ./models/${config_model_path}
     """
-    if use_parent_folder:
-        config_model_path = str(Path(config_model_path).parent)
 
     # Get relative path to model
     relative_path = config_model_path
     # If it follows Teklia's convention, we remove the prefix
-    if relative_path.startswith(DEFAULT_MODEL_DIR):
-        relative_path = relative_path.replace(DEFAULT_MODEL_DIR, "")
+    if relative_path.startswith(str(DEFAULT_MODEL_DIR)):
+        relative_path = Path(relative_path).relative_to(DEFAULT_MODEL_DIR)
 
     # Tested paths
     possible_paths = [
-        DEFAULT_MODEL_DIR + relative_path,
-        relative_path,
-        "models/" + relative_path,
+        DEFAULT_MODEL_DIR / relative_path,
+        Path(".") / relative_path,
+        Path("models") / relative_path,
     ]
     for path_to_model in possible_paths:
-        if os.path.exists(path_to_model):
+        if path_to_model.exists():
             logger.info(f"Found model in {path_to_model}.")
             return path_to_model
 
 
 @contextmanager
 def create_archive(
-    path: FilePath, rename: Optional[str] = None, use_parent_folder: bool = False
+    path: FilePath,
 ) -> Archive:
-    """First create a tar archive, then compress to a zst archive.
-    Finally, get its hash and size
     """
-    compressor = zstd.ZstdCompressor(level=3)
+    Create tar archive with everything that's in the folder at path
+    Keep the hierarchy but parent folder should not be included
+    Save the absolute path of each file added to compute their hash later
+    """
+
+    assert path.is_dir(), "This path must resolve to a directory"
+
     content_hasher = hashlib.md5()
-    archive_hasher = hashlib.md5()
 
     # Remove extension from the model filename
     _, path_to_tar_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar")
 
-    # Create an uncompressed tar archive with all the needed files
-    # Files hierarchy is kept in the archive.
     with tarfile.open(path_to_tar_archive, "w") as tar:
-        if use_parent_folder:
-            if rename is not None:
-                # Publish parent folder under new name
-                tar.add(path, arcname=f"./{rename}")
-            else:
-                # Only publish contents of the given folder without parent folder
-                tar.add(path, arcname=".")
-        elif rename is not None:
-            # Rename the single file to the given name
-            tar.add(path, arcname=rename)
-        else:
-            tar.add(path)
-        file_list = [member for member in tar.getnames() if os.path.isfile(member)]
-
-    # Sort by path
-    file_list.sort()
-
-    # Compute hash of the files
-    for file_path in file_list:
-        with open(file_path, "rb") as file_data:
-            for chunk in iter(lambda: file_data.read(CHUNK_SIZE), b""):
-                content_hasher.update(chunk)
+        tar.add(name=path, arcname=".")
 
-    _, path_to_zst_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar.zst")
+        # Walk and find each file in the dir
+        for member in tar.getnames():
+            filepath = path / member
+            if filepath.is_dir():
+                # We don't care about directories
+                continue
+
+            # Compute hash
+            with filepath.open("rb") as file_data:
+                for chunk in iter(lambda: file_data.read(CHUNK_SIZE), b""):
+                    content_hasher.update(chunk)
 
     # Compress the archive
-    with open(path_to_zst_archive, "wb") as archive_file:
-        with open(path_to_tar_archive, "rb") as model_data:
-            for model_chunk in iter(lambda: model_data.read(CHUNK_SIZE), b""):
-                compressed_chunk = compressor.compress(model_chunk)
-                archive_hasher.update(compressed_chunk)
-                archive_file.write(compressed_chunk)
+    _, path_to_zst_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar.zst")
+
+    compressor = zstd.ZstdCompressor(level=3)
+    archive_hasher = hashlib.md5()
+    with open(path_to_zst_archive, "wb") as archive_file, open(
+        path_to_tar_archive, "rb"
+    ) as model_data:
+        for model_chunk in iter(lambda: model_data.read(CHUNK_SIZE), b""):
+            compressed_chunk = compressor.compress(model_chunk)
+            archive_hasher.update(compressed_chunk)
+            archive_file.write(compressed_chunk)
 
     # Remove the tar archive
     os.remove(path_to_tar_archive)
 
     # Get content hash, archive size and hash
     hash = content_hasher.hexdigest()
     size = os.path.getsize(path_to_zst_archive)
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/process/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/process/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/process/base.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/process/base.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/process/recover.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/process/recover.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         progress.add_task(
             start=False, description=f"Selecting {len(failed_elements)} failed elements"
         )
         client.request("AddSelection", body={"ids": failed_elements})
 
     corpus_id = get_process(client, process_id)["corpus"]
     new_process_id = client.request(
-        "CreateElementsWorkflow",
+        "CreateProcess",
         body={
             "corpus": corpus_id,
             "selection": True,
             "load_children": False,
         },
     )["id"]
     config_url = urljoin(profile.url, f"process/{new_process_id}/configure")
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/process/report.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/process/report.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/secrets.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/alto/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/alto/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/alto/parser.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/alto/parser.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/iiif.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/iiif.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/__init__.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/cache.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/mets/parser.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/mets/parser.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/minio_client.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/minio_client.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/commands/upload/page_xml_import.py` & `arkindex-cli-0.2.7/arkindex_cli/commands/upload/page_xml_import.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli/utils.py` & `arkindex-cli-0.2.7/arkindex_cli/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.2.6/arkindex_cli.egg-info/PKG-INFO` & `arkindex-cli-0.2.7/arkindex_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: export
```

### Comparing `arkindex-cli-0.2.6/arkindex_cli.egg-info/SOURCES.txt` & `arkindex-cli-0.2.7/arkindex_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements-tests.txt
 requirements.txt
 setup.py
 arkindex_cli/__init__.py
 arkindex_cli/argtypes.py
 arkindex_cli/auth.py
 arkindex_cli/cli.py
+arkindex_cli/git.py
 arkindex_cli/utils.py
 arkindex_cli.egg-info/PKG-INFO
 arkindex_cli.egg-info/SOURCES.txt
 arkindex_cli.egg-info/dependency_links.txt
 arkindex_cli.egg-info/entry_points.txt
 arkindex_cli.egg-info/requires.txt
 arkindex_cli.egg-info/top_level.txt
@@ -47,8 +48,10 @@
 arkindex_cli/commands/upload/iiif.py
 arkindex_cli/commands/upload/minio_client.py
 arkindex_cli/commands/upload/page_xml_import.py
 arkindex_cli/commands/upload/alto/__init__.py
 arkindex_cli/commands/upload/alto/parser.py
 arkindex_cli/commands/upload/mets/__init__.py
 arkindex_cli/commands/upload/mets/cache.py
-arkindex_cli/commands/upload/mets/parser.py
+arkindex_cli/commands/upload/mets/parser.py
+arkindex_cli/commands/worker/__init__.py
+arkindex_cli/commands/worker/publish.py
```

### Comparing `arkindex-cli-0.2.6/setup.py` & `arkindex-cli-0.2.7/setup.py`

 * *Files identical despite different names*

