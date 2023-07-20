# Comparing `tmp/fsrs4anki_optimizer-4.2.0.tar.gz` & `tmp/fsrs4anki_optimizer-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.2.0.tar", last modified: Thu Jul 20 13:28:15 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.2.1.tar", last modified: Thu Jul 20 14:40:08 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.2.0.tar` & `fsrs4anki_optimizer-4.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51550 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.442014 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51551 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:40:08.000000 fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:40:08.446015 fsrs4anki_optimizer-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:39:55.000000 fsrs4anki_optimizer-4.2.1/setup.py
```

### Comparing `fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.2.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
             # threshold = np.mean(group['delta_t']) * 1.5
             # threshold = group['delta_t'].quantile(0.95)
             Q1 = group['delta_t'].quantile(0.25)
             Q3 = group['delta_t'].quantile(0.75)
             IQR = Q3 - Q1
             threshold = Q3 + 1.5 * IQR
-            group = group[group['delta_t'] < threshold]
+            group = group[group['delta_t'] <= threshold]
             return group
 
         df[df['i'] == 2] = df[df['i'] == 2].groupby(by=['r_history', 't_history'], as_index=False, group_keys=False).apply(remove_outliers)
 
         def remove_non_continuous_rows(group):
             discontinuity = group['i'].diff().fillna(1).ne(1)
             if not discontinuity.any():
```

