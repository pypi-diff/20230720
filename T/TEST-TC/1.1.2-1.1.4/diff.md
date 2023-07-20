# Comparing `tmp/TEST_TC-1.1.2.tar.gz` & `tmp/TEST_TC-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.1.2.tar", last modified: Thu Jul 20 12:59:44 2023, max compression
+gzip compressed data, was "TEST_TC-1.1.4.tar", last modified: Thu Jul 20 16:26:49 2023, max compression
```

## Comparing `TEST_TC-1.1.2.tar` & `TEST_TC-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.882831 TEST_TC-1.1.2/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.799688 TEST_TC-1.1.2/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.819129 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 12:59:44.000000 TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.822164 TEST_TC-1.1.2/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 12:59:24.000000 TEST_TC-1.1.2/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.833327 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/experiment.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.838241 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.842836 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.848834 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/preprocessing.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.850834 TEST_TC-1.1.2/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.862126 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    12935 2023-07-20 12:57:57.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 12:59:44.879639 TEST_TC-1.1.2/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 11:33:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/check_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16242 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/configuration_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 11:37:38.000000 TEST_TC-1.1.2/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 12:59:44.881640 TEST_TC-1.1.2/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.2/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-20 11:33:39.000000 TEST_TC-1.1.2/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 12:59:44.882831 TEST_TC-1.1.2/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.205072 TEST_TC-1.1.4/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.137490 TEST_TC-1.1.4/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.155483 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 16:26:49.000000 TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.158217 TEST_TC-1.1.4/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 16:26:06.000000 TEST_TC-1.1.4/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.168143 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/experiment.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.172160 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.177008 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.181374 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/preprocessing.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.182443 TEST_TC-1.1.4/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.187916 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    13008 2023-07-20 16:25:46.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 16:26:49.200823 TEST_TC-1.1.4/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/check_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16272 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/configuration_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 16:26:49.203823 TEST_TC-1.1.4/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.4/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-20 16:00:24.000000 TEST_TC-1.1.4/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 16:26:49.205072 TEST_TC-1.1.4/setup.cfg
```

### Comparing `TEST_TC-1.1.2/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.1.4/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/experiment.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/experiment.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/job.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/models.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/models.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/algorithms/utils.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/preprocessing.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datapreparation/utils.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datapreparation/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
 
     df.index = [i for i in range(int(df.shape[0]/df[id_pred].unique().shape[0]))] * df[id_pred].unique().shape[0]
 
     if gerarchia == "Italia":
         n_level = len(gerarchia.split("/")) - 1
         split = np.array_split(df,df[id_pred].unique().shape[0])
-        result = [i for i in split if i[id_pred].unique()[0].count("/") == n_level]
+        result = [i for i in split if i[id_pred].unique()[0].count("/") >= n_level]
     else:
         n_level = len(gerarchia.split("/")) 
         split = np.array_split(df,df[id_pred].unique().shape[0])
         
         select = [i for i in split if i[id_pred].unique()[0].count("/") <= n_level]
         result = [i for i in select if gerarchia in i[id_pred][0]]
     
@@ -50,15 +50,15 @@
         self.data = data
         self.pred_mean = pred_mean
         self.pi_lower = pi_lower
         self.pi_upper = pi_upper
         self.use_case = use_case
 
     def plot_pred(self, df_pred: pd.DataFrame, id_pred: str = None,
-                  df_real: pd.DataFrame = None, data_real: str = None, target: str = None, confidence_interval: bool = False) -> plotly.graph_objs._figure.Figure:
+                  df_real: pd.DataFrame = None, id_pred_real: str = None, data_real: str = None, target: str = None, confidence_interval: bool = False) -> plotly.graph_objs._figure.Figure:
             
         """Plot prediction
 
         Parameters
         ----------
         df_pred : pd:DataFrame
             dataframe of prediction
@@ -83,15 +83,15 @@
         lista_fig = []
         for id_pre in lista_id:
             regione = id_pre
 
             df_pred_parz = df_pred[df_pred[self.id_pred] == id_pre]
 
             if not isinstance(df_real,type(None)):
-                df_real_parz = df_real[df_real[self.id_pred] == id_pre]
+                df_real_parz = df_real[df_real[id_pred_real] == id_pre]
                 real = [go.Scatter(
                         x=df_real_parz[data_real],
                         y=df_real_parz[target],
                         marker=dict(color="blue"),
                         mode="lines",
                         name="past value (true)",showlegend=True
                     )]
@@ -179,15 +179,15 @@
         )
 
         list_fig = [
             go.Scatter(
                 x=pred[self.data],
                 y=pred[self.pred_mean],
                 mode="lines",
-                name=pred["Id_pred"][0],
+                name=pred[self.id_pred][0],
                 showlegend=True,
             )
             for pred in lista_df_pred
         ]
 
         # list_fig = [go.Scatter(x=pred[data],y=pred[pred_mean],marker=dict(color=col),mode="lines",name=pred['Id_pred'][0],showlegend=True)
         #             for pred, col in zip(lista_df_pred,["red","blue"])]
@@ -236,31 +236,31 @@
         fig.add_traces(
             [
                 go.Scatter(
                     x=df_pred_tot[self.data],
                     y=df_pred_tot[self.pred_mean],
                     marker=dict(color="green"),
                     mode="lines",
-                    name=f"Predizione {df_pred_tot['Id_pred'][0]}",
+                    name=f"Predizione {df_pred_tot[self.id_pred][0]}",
                     showlegend=True,
                 ),
                 go.Scatter(
                     x=df_pred_tot[self.data],
                     y=tot_hier_pred.values,
                     marker=dict(color="blue"),
                     mode="lines",
-                    name=f"Somma predizioni {df_pred_tot['Id_pred'][0]}",
+                    name=f"Somma predizioni {df_pred_tot[self.id_pred][0]}",
                     showlegend=True,
                 ),
             ]
         )
 
         return fig
     
-    def dist_residuals(self, df_pred: pd.DataFrame, df_real: pd.DataFrame, target: str, id_pred: str = None) -> list:
+    def dist_residuals(self, df_pred: pd.DataFrame, df_real: pd.DataFrame, id_pred_real: str, target: str, id_pred: str = None) -> list:
 
         """Plots distribution of residuals
 
         Parameters
         ----------
         df_pred : dataframe of prediction
         df_real : pd.DataFrame
@@ -281,15 +281,15 @@
         else:
             lista_id = df_pred[self.id_pred].unique()
 
         lista_fig = []
         for id_pre in lista_id:
 
             df_pred_parz = df_pred[df_pred[self.id_pred] == id_pre]
-            df_real_parz = df_real[df_real[self.id_pred] == id_pre]
+            df_real_parz = df_real[df_real[id_pred_real] == id_pre]
 
             res = df_pred_parz[self.pred_mean] - df_real_parz[target]
 
             fig = px.histogram(res,
                                title="Distribuzione residui",
                                width=800,
                                height=500,
@@ -302,15 +302,15 @@
             
             fig.update_layout(xaxis_title="residual",showlegend=False)
 
             lista_fig += [fig]
 
             return lista_fig
         
-    def plot_residuals(self, df_pred: pd.DataFrame, df_real: pd.DataFrame, target: str, id_pred: str = None) -> list:
+    def plot_residuals(self, df_pred: pd.DataFrame, df_real: pd.DataFrame, id_pred_real: str, target: str, id_pred: str = None) -> list:
 
         """Plots residuals
 
         Parameters
         ----------
         df_pred : dataframe of prediction
         df_real : pd.DataFrame
@@ -331,15 +331,15 @@
         else:
             lista_id = df_pred[self.id_pred].unique()
 
         lista_fig = []
         for id_pre in lista_id:
             
             df_pred_parz = df_pred[df_pred[self.id_pred] == id_pre]
-            df_real_parz = df_real[df_real[self.id_pred] == id_pre]
+            df_real_parz = df_real[df_real[id_pred_real] == id_pre]
 
             res = df_pred_parz[self.pred_mean]-df_real_parz[target]
             import matplotlib.pyplot as plt
             fig_matplot = plt.subplot() 
             qqplot_data = qqplot(res, line='45',ax = fig_matplot).gca().lines
 
             fig = go.Figure()
```

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/check_utils.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/check_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/configuration_utils.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/configuration_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     Returns
     -------
     Tuple[dict, dict]
         Two dictionaries representing the two configuration files
     """
     config_file = get_configuration(config_dict['config_path'], config_dict['config_file'])
-    config_file_parsing = get_configuration(config_dict_parsing['config_path'], config_dict_parsing['config_file'])
+    config_file_parsing = get_configuration(os.path.join(config_dict_parsing['config_path'], 'config_check'), config_dict_parsing['config_file'])
     return config_file, config_file_parsing
 
 def config_key_parsing(config_file: Dict[str, Any], config_file_parsing: Dict[str, Any]):
     """
     The function checks if the config file and the REFERENCE config file have the same keys
 
     Parameters
```

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.1.4/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/README.md` & `TEST_TC-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.2/pyproject.toml` & `TEST_TC-1.1.4/pyproject.toml`

 * *Files identical despite different names*

