# Comparing `tmp/TEST_TC-1.1.0.tar.gz` & `tmp/TEST_TC-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-1.1.0.tar", last modified: Thu Jul 20 07:57:51 2023, max compression
+gzip compressed data, was "TEST_TC-1.1.1.tar", last modified: Thu Jul 20 10:38:28 2023, max compression
```

## Comparing `TEST_TC-1.1.0.tar` & `TEST_TC-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.836884 TEST_TC-1.1.0/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.752133 TEST_TC-1.1.0/LIB_tc/
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.772343 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 07:57:51.000000 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 07:57:51.000000 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:57:51.000000 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 07:57:51.000000 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 07:57:51.000000 TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/top_level.txt
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.774343 TEST_TC-1.1.0/LIB_tc/test_tc/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 07:51:56.000000 TEST_TC-1.1.0/LIB_tc/test_tc/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.785848 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6244 2023-07-20 07:56:53.000000 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/experiment.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 07:56:46.000000 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/job.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    22911 2023-07-20 07:56:32.000000 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/models.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15709 2023-07-20 07:56:14.000000 TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.791849 TEST_TC-1.1.0/LIB_tc/test_tc/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 07:55:56.000000 TEST_TC-1.1.0/LIB_tc/test_tc/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.798744 TEST_TC-1.1.0/LIB_tc/test_tc/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 07:55:40.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.804803 TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 07:55:12.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/preprocessing.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 07:54:59.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.808058 TEST_TC-1.1.0/LIB_tc/test_tc/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.817786 TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    12933 2023-07-19 17:03:11.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/plotPrediction.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-13 07:53:51.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-13 07:53:51.000000 TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/visualization.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 07:57:51.833882 TEST_TC-1.1.0/LIB_tc/test_tc/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/check_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15910 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/configuration_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 07:51:47.000000 TEST_TC-1.1.0/LIB_tc/test_tc/utility/tele_logger.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 07:57:51.835884 TEST_TC-1.1.0/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.0/README.md
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-13 07:53:51.000000 TEST_TC-1.1.0/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 07:57:51.837389 TEST_TC-1.1.0/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.373880 TEST_TC-1.1.1/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.275595 TEST_TC-1.1.1/LIB_tc/
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.300398 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1284 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      341 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        8 2023-07-20 10:38:28.000000 TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/top_level.txt
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.301207 TEST_TC-1.1.1/LIB_tc/test_tc/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-07-20 10:32:32.000000 TEST_TC-1.1.1/LIB_tc/test_tc/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.315021 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6535 2023-07-20 10:33:29.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/experiment.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7719 2023-07-20 07:56:46.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/job.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    24471 2023-07-20 10:36:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/models.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15714 2023-07-20 10:32:15.000000 TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.320031 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5777 2023-07-20 07:55:56.000000 TEST_TC-1.1.1/LIB_tc/test_tc/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.325519 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7303 2023-07-20 07:55:40.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.333539 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     4014 2023-07-20 07:55:12.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/preprocessing.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    25441 2023-07-20 07:54:59.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.335847 TEST_TC-1.1.1/LIB_tc/test_tc/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.348201 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        2 2023-07-10 10:31:23.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    12933 2023-07-19 17:03:11.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/plotPrediction.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14693 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    14566 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/visualization.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-07-20 10:38:28.369881 TEST_TC-1.1.1/LIB_tc/test_tc/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2822 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/check_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16242 2023-07-20 10:30:51.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/configuration_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1515 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1849 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2440 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6048 2023-07-20 07:51:47.000000 TEST_TC-1.1.1/LIB_tc/test_tc/utility/tele_logger.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      456 2023-07-20 10:38:28.372881 TEST_TC-1.1.1/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1873 2023-06-28 16:32:49.000000 TEST_TC-1.1.1/README.md
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1323 2023-07-13 07:53:51.000000 TEST_TC-1.1.1/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-07-20 10:38:28.373880 TEST_TC-1.1.1/setup.cfg
```

### Comparing `TEST_TC-1.1.0/LIB_tc/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-1.1.1/LIB_tc/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/experiment.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/experiment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-from typing import Any, Callable, Dict, Type
+from typing import Any, Callable, Dict, Type, Union, List
 from typing_extensions import Self
 import pandas as pd
 import logging
 
 from .models import ProphetModel
 from ..utility.check_utils import check_not_isinstance, check_not_in_iterable
 from ..utility.resources import get_module_and_function, log_exception
 from ..utility.tele_logger import logger
 
 @log_exception(logger)
 class ExperimentClass():
-    def __init__(self,  model: str, grid_params : Dict):
+    def __init__(self,  model: str, params : Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]] , config_path : str):
         """ Pass all the parameters that can be set as explicit keyword
         arguments.
         
         Parameters
         ----------
         model : str
             Parameter identifying model to use
-        params : Dict        
-            Dictionary representing the model parameters 
+        params : Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]]         
+            Dictionary representing the model parameters
+        config_path : str
+            Path in which resides the configuration files 
             
         """
         self.model_name = model.lower()
+        self.config_path = config_path
 
         if self.model_name == 'prophet':
             log_del = logging.getLogger('cmdstanpy')
             log_del.addHandler(logging.NullHandler())
             log_del.propagate = False
             log_del.setLevel(logging.CRITICAL)
 
-            self.Model = ProphetModel(grid_params=grid_params)
+            self.Model = ProphetModel(params=params, config_path=self.config_path)
         else:
             raise Exception()
 
 
     def check_consistency(self, X: pd.DataFrame):
         """_summary_
```

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/job.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/job.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/models.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,39 @@
 import pandas as pd
 from prophet import Prophet
 import numpy as np
 
 from hierarchicalforecast.core import HierarchicalReconciliation
 from hierarchicalforecast.methods import BottomUp, MinTrace, TopDown
 
-from .utils import model_tuning, create_zero_dataframe
+from .utils import model_tuning, create_zero_dataframe, grid_values_hyperparameters
 from ..analytics.evaluationMetrics import EvaluateModel
 from ..utility.tele_logger import logger
-from ..utility.resources import log_exception, get_module_and_function
+from ..utility.resources import log_exception, get_module_and_function, get_configuration
 from ..utility.check_utils import check_not_in_iterable, check_not_isinstance
 
 
 class ProphetModel():
-    def __init__(self, grid_params: Dict[str, List[Union[str, bool, int, float]]], max_na_ratio: float = 0.5):
+    def __init__(self, params: Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]], config_path: str, max_na_ratio: float = 0.5):
         """
         Initlization parameters for ProphetModel.
 
         Parameters
         ----------
-        dic_param : Dict[str, List[Union[str, bool, int, float]]]        
-            Dictionary representing the model parameters
+        dic_param : Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]]      
+            The dictionary of hyperparameters from the config file
         max_na_ratio : float
             Maximum ratio of NaNs and not null permitted in order to fit the model
         """
 
-        self.grid_params = grid_params
+        self.config_path = config_path
         self.max_na_ratio = max_na_ratio
+        params.update({'interval_width':['0.95']}) # Update params with the 95% CI since default is 80%
+
+        self.make_grid_params(params)
 
 
     def fit(self, X_train: pd.DataFrame, X_val: pd.DataFrame) -> Self:
         """Fits the models using a Train and Validations Set setting in the call arguments the 
         Dictionary of Best Parameters and Dictionary of Fitted models which used the respective Best Params.
 
         Parameters
@@ -90,14 +93,26 @@
                 continue
 
             count += 1
             logger.info(f"Remaining number of iteration - {total_runs-count}")
         
         logger.info(f"DONE Fitting Model.", important=True)
 
+        # Check consinstency of models_dict
+        count = 0
+        breaker = len(self.models_dict.keys())
+        for m in self.models_dict.values():
+            if m != None:
+                break
+            else:
+                count+=1
+
+        if count == breaker:
+            raise Exception('No models have been trained, check logs for insights on the reasoning.')
+
         return self
 
 
     def refit(self, X: pd.DataFrame) -> Self:
         """_summary_
 
         Parameters
@@ -238,14 +253,36 @@
 
         # Evaluate Standard Deviation from .95 Percentiles using normality rule
         preproc_df['Sigma'] = (preproc_df['Pi_Upper_95'] - preproc_df['Pi_Lower_95']) / (2 * 1.96) 
         # Round the float values and set tham as integers
         preproc_df[['Pred_Mean', 'Sigma', 'Pi_Lower_95', 'Pi_Upper_95']] = preproc_df[['Pred_Mean', 'Sigma', 'Pi_Lower_95', 'Pi_Upper_95']].round().astype(int)
         
         return preproc_df[['Timestamp', 'Id_Pred', 'Pred_Mean', 'Sigma', 'Pi_Lower_95', 'Pi_Upper_95']]
+    
+
+    def make_grid_params(self, params: Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]]):
+        """The function takes as input the dictionary of the config file 
+        and executes the grid_values_hyperparameters which generates the 
+        combination of grid search parameters.
+
+        Parameters
+        ----------
+        params : Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]]
+            The dictionary of hyperparameters from the config file
+        """
+
+        # LOAD DEFAULT STEPS  
+        ############################################
+        config_path = self.config_path
+        default_steps_config = "default_steps.toml"
+        default_steps = get_configuration('prophet', config_path, default_steps_config)
+        ############################################
+
+        self.grid_params = grid_values_hyperparameters(params, default_steps)
+
 
 
 @log_exception(logger)
 class HierarchicalReconcileModel():
     def __init__(self, model_name: str, S: pd.DataFrame, tags: Dict[str, List[str]], reconciler: List =None, max_na_ratio: float =0.5):
         """_summary_
```

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/algorithms/utils.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/algorithms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                                 default_steps: Dict[str, Union[int, float]]) -> Dict[str, List[Union[str, bool, int, float]]]:
     """
     The function takes as input the dictionary of the config file
     and generates the combination of grid search parameters
 
     Parameters
     ----------
-    config_hyperparameters: Dict[str, Union[List[str], Dict[str, Union[int, float]]]]
+    config_hyperparameters: Dict[str, Union[Dict[str, Union[int, float, str]], List[str]]]
         The dictionary of hyperparameters from the config file
     default_steps: Dict[str, Union[int, float]]
         The default steps used if it's not specified in the config file
 
     Returns
     -------
     Dict[str, List[Union[str, bool, int, float]]]
```

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/analytics/evaluationMetrics.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datahandler/datahandler.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/preprocessing.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datapreparation/utils.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datapreparation/utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/plotPrediction.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/plotPrediction.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/timeSeriesVisualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/datavisualization/visualization.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/datavisualization/visualization.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/check_utils.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/check_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/configuration_utils.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/configuration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         List of possible values for apply_hierarchical
     """
     check_not_isinstance(obj =  model_name, data_type = str, func = get_module_and_function())
     check_not_isinstance(obj =  reference_model_name, data_type = str, func = get_module_and_function())
     check_not_isinstance(obj =  apply_hierarchical, data_type = bool, func = get_module_and_function())
     check_not_in_iterable(obj = apply_hierarchical, iterable = reference_apply_hierarchical, func = get_module_and_function())
     if model_name != reference_model_name:
-        logger.error(f"model_name {model_name} MUST be equal to reference_model_name {reference_model_name}")
+        raise InputTypeError(func = get_module_and_function(), 
+                             message=f"model_name {model_name} MUST be equal to reference_model_name {reference_model_name}")
 
 def check_hyperparameters(hyperparameters: List[str], possible_hyperparameters: List[str]):
     """
     The function checks if the hyperparameters specified are allowed
 
     Parameters
     ----------
@@ -231,31 +232,34 @@
     check_not_isinstance(obj = test_obs, data_type = int, func = get_module_and_function())
     check_not_isinstance(obj = num_forecast_periods, data_type = int, func = get_module_and_function())
     check_not_isinstance(obj = start_date, data_type = str, func = get_module_and_function())
     check_datatype_convertible(obj = start_date, data_type_conversion = pd.to_datetime, func = get_module_and_function())
     
     # Check val - test - future consistency
     if validation_obs == 0 or test_obs == 0 or num_forecast_periods == 0:
-        logger.error(f"Validation size {validation_obs}, Test size {test_obs} and Future forecast periods {num_forecast_periods} MUST be greater than 0.")
+        raise InputTypeError(func = get_module_and_function(), 
+                             message=f"Validation size {validation_obs}, Test size {test_obs} and Future forecast periods {num_forecast_periods} MUST be greater than 0.")
     
     if test_obs >= validation_obs or num_forecast_periods >= validation_obs:
-        logger.error(f'Validation size {validation_obs} MUST be greater than Test size {test_obs} and Future forecast periods {num_forecast_periods}')
+        raise InputTypeError(func = get_module_and_function(), 
+                             message=f'Validation size {validation_obs} MUST be greater than Test size {test_obs} and Future forecast periods {num_forecast_periods}')
 
     # Check proportion consistency val - test - future depending on the time granularity
     if time_granularity == 'M':
         difference = 3
     if time_granularity == 'W': 
         difference = 4
     if time_granularity == 'D':
         difference = 7
     if time_granularity == 'H':
         difference = 24
     if (validation_obs - test_obs) < difference or (validation_obs - num_forecast_periods) < difference:
-        logger.error(f'Validation size {validation_obs} MUST be greater than Test size {test_obs} and Future forecast periods {num_forecast_periods} ' + 
-                     f'of at least {difference} for time granularity {time_granularity}')
+        raise InputTypeError(func = get_module_and_function(), 
+                             message=f'Validation size {validation_obs} MUST be greater than Test size {test_obs} and Future forecast periods {num_forecast_periods} ' + 
+                             f'of at least {difference} for time granularity {time_granularity}')
 
 def check_hierarchy(hierarchy: Dict[str, str]):
     """
     The function checks if the values of the hierarhcy are strings
 
     Parameters
     ----------
```

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/constants.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/exceptions.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/resources.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/LIB_tc/test_tc/utility/tele_logger.py` & `TEST_TC-1.1.1/LIB_tc/test_tc/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/README.md` & `TEST_TC-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-1.1.0/pyproject.toml` & `TEST_TC-1.1.1/pyproject.toml`

 * *Files identical despite different names*

