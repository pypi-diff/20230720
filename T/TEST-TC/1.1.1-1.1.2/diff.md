# Comparing `tmp/TEST_TC-1.1.1.tar.gz` & `tmp/TEST_TC-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.1.1.tar", last modified: Thu Jul 20 10:38:28 2023, max compression
+gzip compressed data, was "TEST_TC-1.1.2.tar", last modified: Thu Jul 20 12:59:44 2023, max compression
```

## Comparing `TEST_TC-1.1.1.tar` & `TEST_TC-1.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.373880 TEST_TC-1.1.1/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.275595 TEST_TC-1.1.1/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.300398 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.301207 TEST_TC-1.1.1/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 10:32:32.000000 TEST_TC-1.1.1/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.315021 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 10:33:29.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/experiment.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 07:56:46.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 10:36:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 10:32:15.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.320031 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 07:55:56.000000 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.325519 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 07:55:40.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.333539 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 07:55:12.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/preprocessing.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 07:54:59.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.335847 TEST_TC-1.1.1/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.348201 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    12933 2023-07-19 17:03:11.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.369881 TEST_TC-1.1.1/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/check_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16242 2023-07-20 10:30:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/configuration_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 10:38:28.372881 TEST_TC-1.1.1/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.1/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 10:38:28.373880 TEST_TC-1.1.1/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.882831 TEST_TC-1.1.2/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.799688 TEST_TC-1.1.2/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.819129 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.822164 TEST_TC-1.1.2/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 12:59:24.000000 TEST_TC-1.1.2/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.833327 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/experiment.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.838241 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.842836 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.848834 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/preprocessing.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.850834 TEST_TC-1.1.2/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.862126 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    12935 2023-07-20 12:57:57.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.879639 TEST_TC-1.1.2/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/check_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16242 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/configuration_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 12:59:44.881640 TEST_TC-1.1.2/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.2/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-20 11:33:39.000000 TEST_TC-1.1.2/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 12:59:44.882831 TEST_TC-1.1.2/setup.cfg
```

### Comparing `TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/experiment.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/experiment.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/job.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/models.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/utils.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/preprocessing.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/utils.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Returns
     -------
     _type_
         _description_
     """
 
-    df.index = [i for i in range(int(df.shape[0]/df.Id_pred.unique().shape[0]))] * df.Id_pred.unique().shape[0]
+    df.index = [i for i in range(int(df.shape[0]/df[id_pred].unique().shape[0]))] * df[id_pred].unique().shape[0]
 
     if gerarchia == "Italia":
         n_level = len(gerarchia.split("/")) - 1
         split = np.array_split(df,df[id_pred].unique().shape[0])
         result = [i for i in split if i[id_pred].unique()[0].count("/") == n_level]
     else:
         n_level = len(gerarchia.split("/"))
```

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/check_utils.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/check_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/configuration_utils.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.1.2/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/README.md` & `TEST_TC-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.1/pyproject.toml` & `TEST_TC-1.1.2/pyproject.toml`

 * *Files identical despite different names*

