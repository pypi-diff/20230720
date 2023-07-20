# Comparing `tmp/fsrs4anki_optimizer-4.1.3.tar.gz` & `tmp/fsrs4anki_optimizer-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.1.3.tar", last modified: Thu Jul 20 03:08:32 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.2.0.tar", last modified: Thu Jul 20 13:28:15 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.1.3.tar` & `fsrs4anki_optimizer-4.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:08:32.541928 fsrs4anki_optimizer-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 03:08:32.537928 fsrs4anki_optimizer-4.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:08:32.537928 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 03:08:21.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 03:08:21.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51385 2023-07-20 03:08:21.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:08:32.537928 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 03:08:32.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 03:08:32.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:08:32.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 03:08:32.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 03:08:32.000000 fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 03:08:21.000000 fsrs4anki_optimizer-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:08:32.541928 fsrs4anki_optimizer-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 03:08:21.000000 fsrs4anki_optimizer-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51550 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 13:28:15.000000 fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:28:15.648733 fsrs4anki_optimizer-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 13:28:01.000000 fsrs4anki_optimizer-4.2.0/setup.py
```

### Comparing `fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.1.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.2.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,31 +396,35 @@
         t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
 
-        # def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
-        #     threshold = np.mean(group['delta_t']) * 1.5
-        #     # threshold = group['delta_t'].quantile(0.95)
-        #     group = group[group['delta_t'] < threshold]
-        #     return group
-
-        # df = df.groupby(by=['r_history', 't_history'], as_index=False, group_keys=False).apply(remove_outliers)
-
-        # def remove_non_continuous_rows(group):
-        #     discontinuity = group['i'].diff().fillna(1).ne(1)
-        #     if not discontinuity.any():
-        #         return group
-        #     else:
-        #         first_non_continuous_index = discontinuity.idxmax()
-        #         return group.loc[:first_non_continuous_index-1]
+        def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
+            # threshold = np.mean(group['delta_t']) * 1.5
+            # threshold = group['delta_t'].quantile(0.95)
+            Q1 = group['delta_t'].quantile(0.25)
+            Q3 = group['delta_t'].quantile(0.75)
+            IQR = Q3 - Q1
+            threshold = Q3 + 1.5 * IQR
+            group = group[group['delta_t'] < threshold]
+            return group
+
+        df[df['i'] == 2] = df[df['i'] == 2].groupby(by=['r_history', 't_history'], as_index=False, group_keys=False).apply(remove_outliers)
+
+        def remove_non_continuous_rows(group):
+            discontinuity = group['i'].diff().fillna(1).ne(1)
+            if not discontinuity.any():
+                return group
+            else:
+                first_non_continuous_index = discontinuity.idxmax()
+                return group.loc[:first_non_continuous_index-1]
 
-        # df = df.groupby('cid', as_index=False, group_keys=False).progress_apply(remove_non_continuous_rows)
+        df = df.groupby('cid', as_index=False, group_keys=False).progress_apply(remove_non_continuous_rows)
 
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         tqdm.write("Trainset saved.")
 
         S0_dataset = df[df['i'] == 2]
         self.S0_dataset_group = S0_dataset.groupby(by=['r_history', 'delta_t'], group_keys=False).agg({'y': ['mean', 'count']}).reset_index()
         self.S0_dataset_group.to_csv('stability_for_pretrain.tsv', sep='\t', index=None)
```

