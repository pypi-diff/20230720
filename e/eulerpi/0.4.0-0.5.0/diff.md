# Comparing `tmp/eulerpi-0.4.0.tar.gz` & `tmp/eulerpi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.4.0.tar", max compression
+gzip compressed data, was "eulerpi-0.5.0.tar", max compression
```

## Comparing `eulerpi-0.4.0.tar` & `eulerpi-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1117 2023-06-24 19:44:36.673968 eulerpi-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     4828 2023-06-24 19:44:36.673968 eulerpi-0.4.0/README.md
--rw-r--r--   0        0        0      564 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/__init__.py
--rw-r--r--   0        0        0     7531 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/data_transformation.py
--rw-r--r--   0        0        0      362 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/data_transformation_types.py
--rw-r--r--   0        0        0    11548 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      355 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0     6790 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/inference.py
--rw-r--r--   0        0        0      514 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     3684 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/kde.py
--rw-r--r--   0        0        0    16765 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/model.py
--rw-r--r--   0        0        0    18493 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    15655 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    21145 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     7581 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2560 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0       82 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/heat/__init__.py
--rw-r--r--   0        0        0     9613 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/heat/heat.py
--rw-r--r--   0        0        0     1811 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1133 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1859 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2340 2023-06-24 19:44:36.685968 eulerpi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6249 1970-01-01 00:00:00.000000 eulerpi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-07-20 13:56:40.296235 eulerpi-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4923 2023-07-20 13:56:40.296235 eulerpi-0.5.0/README.md
+-rw-r--r--   0        0        0      564 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0     7690 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/data_transformation.py
+-rw-r--r--   0        0        0      362 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/data_transformation_types.py
+-rw-r--r--   0        0        0    11548 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     6790 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    18113 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/model.py
+-rw-r--r--   0        0        0    18493 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    15903 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    21145 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     7581 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2560 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0       82 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/heat/__init__.py
+-rw-r--r--   0        0        0    10728 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/heat/heat.py
+-rw-r--r--   0        0        0     1811 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1160 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1576 2023-07-20 13:56:40.300235 eulerpi-0.5.0/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-07-20 13:56:40.304235 eulerpi-0.5.0/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2340 2023-07-20 13:56:40.304235 eulerpi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6344 1970-01-01 00:00:00.000000 eulerpi-0.5.0/PKG-INFO
```

### Comparing `eulerpi-0.4.0/LICENSE.md` & `eulerpi-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/README.md` & `eulerpi-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,19 +71,21 @@
 To evaluate the model and infer the parameter distribution, call:
 
 ```python
 from eulerpi.sampling import inference
 
 from my_model import MyModel
 
-central_param = np.array([0.5, -1.5, ...])
-param_limits = np.array([[0.0, 1.0], [-3.0, 0.0], ...])
+# This line is needed for multiprocessing in python
+if __name__ == "__main__":
+    central_param = np.array([0.5, -1.5, ...])
+    param_limits = np.array([[0.0, 1.0], [-3.0, 0.0], ...])
 
-model = MyModel(central_param, param_limits)
-inference(model=model, data="my_data.csv")
+    model = MyModel(central_param, param_limits)
+    inference(model=model, data="my_data.csv")
 ```
 
 The `data` argument can be a numpy-2d-array or a PathLike object that points to a CSV file. In the example shown above, the CSV file `my_data.csv` should contain the data in the following format:
 
 ```text
 datapoint_dim1, datapoint_dim2, datapoint_dim3, ..., datapoint_dimN
 datapoint_dim1, datapoint_dim2, datapoint_dim3, ..., datapoint_dimN
```

### Comparing `eulerpi-0.4.0/eulerpi/__init__.py` & `eulerpi-0.5.0/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/data_transformation.py` & `eulerpi-0.5.0/eulerpi/core/data_transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,18 +205,24 @@
 
         Args:
             data (jnp.ndarray): The data to be transformed.
 
         Returns:
             jnp.ndarray: The data projected onto and expressed in the basis of the principal components.
         """
-        return self.pca.transform(data.reshape(-1, data.shape[-1])).reshape(
+        result = self.pca.transform(data.reshape(-1, data.shape[-1])).reshape(
             -1, self.pca.n_components_
         )
 
+        # if the input data was 1D, the output should be 1D as well
+        if data.ndim == 1:
+            result = result.flatten()
+
+        return result
+
     def jacobian(self, data: jnp.ndarray) -> jnp.ndarray:
         """Return the jacobian of the pca transformation at the given data point(s).
 
         Args:
             data (jnp.ndarray): The data point(s) at which the jacobian should be evaluated.
 
         Returns:
```

### Comparing `eulerpi-0.4.0/eulerpi/core/dense_grid.py` & `eulerpi-0.5.0/eulerpi/core/dense_grid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/inference.py` & `eulerpi-0.5.0/eulerpi/core/inference.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/inference_types.py` & `eulerpi-0.5.0/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/kde.py` & `eulerpi-0.5.0/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/model.py` & `eulerpi-0.5.0/eulerpi/core/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Optional, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 from jax import jacrev, jit, vmap
 
 import amici
-from eulerpi import logger
 from eulerpi.jax_extension import value_and_jacrev
 
 
 class Model(ABC):
     """The base class for all models using the EPI algorithm.
 
     Args:
@@ -275,116 +274,155 @@
 
 
 class SBMLModel(Model):
     """The SBMLModel class is a wrapper for the AMICI python interface to simulate SBML models using this package.
 
     Args:
         sbml_file(str): The path to the SBML model file.
-        param_names(list): A list of parameter names. If None the parameter names are extracted from the SBML model.
-        tEnd(float): The end time of the simulation. (Default value = 1.0)
+        param_ids(list): A list of ids of parameter, which will be estimated during the inference. If None all parameter ids are extracted from the SBML model.
+        state_ids(list): A list of state ids, for which data will be given during the inference. If None all state ids are extracted from the SBML model.
+        timepoints(list): List of measurement time points, this is where the sbml model is evaluated and compared to the data
         skip_creation(bool): If True the model is not created againg based on the SBML file. Instead the model is loaded from a previously created model. (Default value = False)
         central_param(np.ndarray): The central parameter for the model
         param_limits(np.ndarray): The parameter limits for the model
     """
 
+    @staticmethod
+    def indices_from_ids(ids: list, all_ids: list) -> list:
+        """Returns the indices of the ids in the all_ids list.
+
+        Args:
+            ids(list): The ids for which the indices should be returned.
+            all_ids(list): The list of all ids.
+
+        Returns:
+            list: The indices of the ids in the all_ids list.
+
+        Throws:
+            ValueError: If one of the ids is not in the all_ids list.
+
+        """
+        indices = []
+        for id in ids:
+            try:
+                indices.append(all_ids.index(id))
+            except ValueError:
+                raise ValueError(
+                    f"Parameter / State id '{id}' is not in the list of the relevant ids {all_ids}"
+                )
+        return indices
+
     @property
     def param_dim(self):
         """The number of parameters of the model."""
-        return len(self.amici_model.getParameterIds())
+        return len(self.param_ids)
 
     @property
     def data_dim(self):
-        """The number of observables of the model."""
-        return len(self.amici_model.getStateIds())
+        """The dimension of a data point returned by the model."""
+        return len(self.state_ids) * len(self.timepoints)
 
     def __init__(
         self,
         sbml_file: str,
         central_param: np.ndarray,
         param_limits: np.ndarray,
-        param_names=None,
-        tEnd=1.0,
+        timepoints: list,
+        param_ids: Optional[list] = None,
+        state_ids: Optional[list] = None,
         skip_creation: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         super().__init__(central_param, param_limits, name, **kwargs)
 
-        self.tEnd = tEnd
-
         self.amici_model_name = self.name
         self.amici_model_dir = "./amici/" + self.amici_model_name
 
         # Generate python code
         if not skip_creation:
             sbml_importer = amici.SbmlImporter(sbml_file)
             sbml_importer.sbml2amici(
-                self.amici_model_name, self.amici_model_dir
+                self.amici_model_name,
+                self.amici_model_dir,
             )
 
-        self.param_names = param_names
-
         # Load the generated model
+        self.timepoints = timepoints
         self.load_amici_model_and_solver()
 
+        self.param_ids = param_ids or self.amici_model.getParametersIds()
+        self.state_ids = state_ids or self.amici_model.getStateIds()
+        self.param_indices = self.indices_from_ids(
+            self.param_ids, self.amici_model.getParameterIds()
+        )
+        self.state_indices = self.indices_from_ids(
+            self.state_ids, self.amici_model.getStateIds()
+        )
+        self.setSensitivities()
+
     def load_amici_model_and_solver(self):
         """Loads the AMICI model from the previously generated model."""
         amici_model_module = amici.import_model_module(
             self.amici_model_name, self.amici_model_dir
         )
         self.amici_model = amici_model_module.getModel()
         self.amici_solver = self.amici_model.getSolver()
 
-        # TODO: Maybe this is redundant when using settings to hdf5
-        self.amici_model.setTimepoints([self.tEnd])
+        self.amici_model.setTimepoints(self.timepoints)
+        self.amici_solver.setAbsoluteTolerance(1e-10)
 
-        if self.param_names is not None:
-            # We need the indices for setParameterList, not the ids or names
-            amici_param_indices = []
-            for i, param_id in enumerate(self.amici_model.getParameterIds()):
-                if param_id in self.param_names:
-                    amici_param_indices.append(i)
-                else:
-                    logger.warning(
-                        f"Parameter {param_id} is specified in the sbml file, but not in the passed parameter list. It will be ignored."
-                    )
-            self.amici_model.setParameterList(amici_param_indices)
-        else:
-            self.param_names = self.amici_model.getParameterIds()
+    def setSensitivities(self):
+        if self.param_ids == self.amici_model.getParameterIds():
             self.amici_model.requireSensitivitiesForAllParameters()
+        else:
+            self.amici_model.setParameterList(self.param_indices)
+
         self.amici_solver.setSensitivityMethod(amici.SensitivityMethod.forward)
         self.amici_solver.setSensitivityOrder(amici.SensitivityOrder.first)
 
     def forward(self, params):
         for i, param in enumerate(params):
-            self.amici_model.setParameterByName(self.param_names[i], param)
+            self.amici_model.setParameterById(self.param_ids[i], param)
         rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
-        return rdata.x[-1]
+        return rdata.x[:, self.state_indices].reshape(self.data_dim)
 
     def jacobian(self, params):
         for i, param in enumerate(params):
-            self.amici_model.setParameterByName(self.param_names[i], param)
+            self.amici_model.setParameterById(self.param_ids[i], param)
         rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
-        return rdata.sx[-1].T
+        return (
+            rdata.sx[:, :, self.state_indices]
+            .transpose(1, 0, 2)
+            .reshape(self.param_dim, self.data_dim)
+            .T
+        )
 
     def forward_and_jacobian(
         self, params: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
         for i, param in enumerate(params):
-            self.amici_model.setParameterByName(self.param_names[i], param)
+            self.amici_model.setParameterById(self.param_ids[i], param)
         rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
-        return rdata.x[-1], rdata.sx[-1].T
+        return (
+            rdata.x[:, self.state_indices].reshape(self.data_dim),
+            rdata.sx[:, :, self.state_indices]
+            .transpose(1, 0, 2)
+            .reshape(self.param_dim, self.data_dim)
+            .T,
+        )
 
     # Allow the model to be pickled
     def __getstate__(self):
         # Create a copy of the object's state
         state = self.__dict__.copy()
 
         # Save the amici solver settings to
         _fd, _file = tempfile.mkstemp()
+
         try:
             # write amici solver settings to file
             try:
                 amici.writeSolverSettingsToHDF5(self.amici_solver, _file)
             except AttributeError as e:
                 e.args += (
                     "Pickling the SBMLModel requires an AMICI "
@@ -409,14 +447,15 @@
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
         # Restore amici model and solver
         self.load_amici_model_and_solver()
+        self.setSensitivities()
 
         _fd, _file = tempfile.mkstemp()
         try:
             # write solver settings to temporary file
             with open(_fd, "wb", closefd=False) as f:
                 f.write(state["amici_solver_settings"])
             # read in solver settings
```

### Comparing `eulerpi-0.4.0/eulerpi/core/result_manager.py` & `eulerpi-0.5.0/eulerpi/core/result_manager.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/sampling.py` & `eulerpi-0.5.0/eulerpi/core/sampling.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         )
         # Extract the final walker position and close the pool of worker processes.
         final_walker_positions, _, _, _ = sampler.run_mcmc(
             initial_walker_positions, num_steps, tune=True, progress=True
         )
     except ValueError as e:
         # If the message equals "Probability function returned NaN."
-        if str(e) == "Probability function returned NaN.":
+        if "Probability function returned NaN" in str(e):
             raise ValueError(
                 "Probability function returned NaN. "
                 "You possibly have to exclude data dimensions which do not depend on the paramaters. "
                 "In addition your parameters should not be linearly dependent."
             )
         else:
             raise e
@@ -181,18 +181,22 @@
         TODO check: are those really log probabilities?
 
     """
     # Calculate the standard deviation of the data for each dimension
     data_stdevs = calc_kernel_width(data)
     sampling_dim = slice.shape[0]
     central_param = model.central_param
+    param_limits = model.param_limits
 
     # Initialize each walker at a Gaussian-drawn random, slightly different parameter close to the central parameter.
-    # TODO Make random variation of initial walker positions dependent on sampling limits?
-    initial_walker_positions = central_param[slice] + 0.002 * (
+    # compute element-wise min of the difference between the central parameter and the lower sampling limit and the difference between the central parameter and the upper sampling limit
+    d_min = np.minimum(
+        central_param - param_limits[:, 0], param_limits[:, 1] - central_param
+    )
+    initial_walker_positions = central_param[slice] + d_min[slice] * (
         np.random.rand(num_walkers, sampling_dim) - 0.5
     )
 
     # Count and print how many runs have already been performed for this model
     num_existing_files = result_manager.count_emcee_sub_runs(slice)
     logger.debug(f"{num_existing_files} existing files found")
```

### Comparing `eulerpi-0.4.0/eulerpi/core/sparsegrid.py` & `eulerpi-0.5.0/eulerpi/core/sparsegrid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/core/transformations.py` & `eulerpi-0.5.0/eulerpi/core/transformations.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.5.0/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/corona/corona.py` & `eulerpi-0.5.0/eulerpi/examples/corona/corona.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.5.0/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.5.0/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.5.0/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.5.0/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/heat/heat.py` & `eulerpi-0.5.0/eulerpi/examples/heat/heat.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     """
     dx = args[0]
     dy = args[1]
     param = args[2]
 
     # use the central difference scheme to approximate the derivatives. Gradient preserves the size of the array by using one-sided differences. We throw away the boundary points later.
     du_dx = jnp.gradient(u, dx, axis=0)
-    du_dy = jnp.gradient(u, dy, axis=1)
-    du_dx2 = jnp.gradient(du_dx, dx, axis=0)
-    du_dy2 = jnp.gradient(du_dy, dy, axis=1)
+    du_dx2 = (u[2:, 1:-1] - 2 * u[1:-1, 1:-1] + u[:-2, 1:-1]) / dx**2
+    du_dy2 = (u[1:-1, 2:] - 2 * u[1:-1, 1:-1] + u[1:-1, :-2]) / dy**2
     du_dx_dy = jnp.gradient(du_dx, dy, axis=1)
 
     # compute the right hand side of the heat equation
     rhs = jnp.zeros(u.shape)
     rhs = rhs.at[1:-1, 1:-1].set(
-        param[0] * du_dx2[1:-1, 1:-1]
-        + param[1] * du_dy2[1:-1, 1:-1]
+        param[0] * du_dx2
+        + param[1] * du_dy2
         + 2 * param[2] * du_dx_dy[1:-1, 1:-1]
     )
     return rhs
 
 
 class Heat(JaxModel):
     """A two-dimensional anisotropic heat conduction equation model on a square domain with four dirichlet boundaries.
@@ -100,25 +99,38 @@
         Returns:
             np.ndarray: The solution of the anisotropic heat conduction equation at time :math:`\\t=0.1`
         in five spacial points, which are arranged similar to the number "five" on a dice.
         """
 
         solution = cls.perform_simulation(kappa=param)
 
-        # the indices of the wanted evaluation points
-        evaluation_indices = jnp.multiply(
-            cls.evaluation_points,
-            jnp.array(solution.shape),
-        ).astype(int)
-
-        solution_at_evaluation_points = jnp.array(
-            solution[
-                evaluation_indices[:, 0],
-                evaluation_indices[:, 1],
-            ]
+        # linearly interpolate the solution at the evaluation points, use own interpolation function as jax doesn't support scipy.interpolate.interp2d and doesn't provide a 2d interpolation function
+        x = jnp.linspace(0, cls.plate_length[0], cls.num_grid_points)
+        y = jnp.linspace(0, cls.plate_length[1], cls.num_grid_points)
+
+        # compute the indices between which the evaluation points lie
+        x_indices = jnp.searchsorted(x, cls.evaluation_points[:, 0]) - 1
+        y_indices = jnp.searchsorted(y, cls.evaluation_points[:, 1]) - 1
+        dx = cls.plate_length[0] / cls.num_grid_points
+        dy = cls.plate_length[1] / cls.num_grid_points
+
+        # interpolate the solution at the evaluation points
+        solution_at_evaluation_points = (1 / (dx * dy)) * (
+            solution[x_indices, y_indices]
+            * (x[x_indices + 1] - cls.evaluation_points[:, 0])
+            * (y[y_indices + 1] - cls.evaluation_points[:, 1])
+            + solution[x_indices + 1, y_indices]
+            * (cls.evaluation_points[:, 0] - x[x_indices])
+            * (y[y_indices + 1] - cls.evaluation_points[:, 1])
+            + solution[x_indices, y_indices + 1]
+            * (x[x_indices + 1] - cls.evaluation_points[:, 0])
+            * (cls.evaluation_points[:, 1] - y[y_indices])
+            + solution[x_indices + 1, y_indices + 1]
+            * (cls.evaluation_points[:, 0] - x[x_indices])
+            * (cls.evaluation_points[:, 1] - y[y_indices])
         )
         return solution_at_evaluation_points
 
     def param_is_within_domain(self, param: np.ndarray) -> bool:
         """Checks whether a parameter is within the parameter domain of the model.
         This condition stems from thermodynamical considerations.
 
@@ -192,14 +204,15 @@
         return u
 
 
 class HeatArtificial(Heat, ArtificialModelInterface):
 
     CENTRAL_PARAM = np.array([1.5, 1.5, 0.5])
     PARAM_LIMITS = np.array([[1.0, 2.0], [1.0, 2.0], [0.0, 1.0]])
+    num_grid_points = 20
 
     def __init__(
         self,
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
         name: Optional[str] = None,
         **kwargs,
```

### Comparing `eulerpi-0.4.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.5.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.5.0/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import numpy as np
 
 from eulerpi.core.model import ArtificialModelInterface, SBMLModel
 
 
 class CaffeineSBMLModel(SBMLModel, ArtificialModelInterface):
 
-    param_dim = 2
-    data_dim = 1
-
     CENTRAL_PARAM = np.array([1.0, 1.0])
     PARAM_LIMITS = np.array([[0.0, 2.0], [0.0, 2.0]])
 
     def __init__(
         self,
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
         **kwargs,
     ) -> None:
         sbml_file = importlib.resources.path(
             "eulerpi.examples.sbml", "Caffeine_2Wks_Exponential_decay.xml"
         )
-        param_names = ["A", "B"]
+        param_ids = ["A", "B"]
+        timepoints = np.array([0.5, 1.0])
+
         super().__init__(
             sbml_file,
             central_param,
             param_limits,
-            param_names,
+            timepoints,
+            param_ids,
             **kwargs,
         )
 
     def generate_artificial_params(self, num_samples: int) -> np.ndarray:
         diff0 = 0.2
         diff1 = 0.2
         params = np.random.rand(num_samples, self.param_dim)
```

### Comparing `eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.5.0/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/simple_models.py` & `eulerpi-0.5.0/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.5.0/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/stock/stock.py` & `eulerpi-0.5.0/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.5.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.5.0/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.5.0/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/eulerpi/jax_extension.py` & `eulerpi-0.5.0/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.4.0/pyproject.toml` & `eulerpi-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.4.0"
+version = "0.5.0"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `eulerpi-0.4.0/PKG-INFO` & `eulerpi-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.4.0
+Version: 0.5.0
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -100,19 +100,21 @@
 To evaluate the model and infer the parameter distribution, call:
 
 ```python
 from eulerpi.sampling import inference
 
 from my_model import MyModel
 
-central_param = np.array([0.5, -1.5, ...])
-param_limits = np.array([[0.0, 1.0], [-3.0, 0.0], ...])
+# This line is needed for multiprocessing in python
+if __name__ == "__main__":
+    central_param = np.array([0.5, -1.5, ...])
+    param_limits = np.array([[0.0, 1.0], [-3.0, 0.0], ...])
 
-model = MyModel(central_param, param_limits)
-inference(model=model, data="my_data.csv")
+    model = MyModel(central_param, param_limits)
+    inference(model=model, data="my_data.csv")
 ```
 
 The `data` argument can be a numpy-2d-array or a PathLike object that points to a CSV file. In the example shown above, the CSV file `my_data.csv` should contain the data in the following format:
 
 ```text
 datapoint_dim1, datapoint_dim2, datapoint_dim3, ..., datapoint_dimN
 datapoint_dim1, datapoint_dim2, datapoint_dim3, ..., datapoint_dimN
```

