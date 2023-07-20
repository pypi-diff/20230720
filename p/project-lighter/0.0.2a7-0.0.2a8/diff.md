# Comparing `tmp/project_lighter-0.0.2a7.tar.gz` & `tmp/project_lighter-0.0.2a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a7.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a8.tar", max compression
```

## Comparing `project_lighter-0.0.2a7.tar` & `project_lighter-0.0.2a8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-07-06 19:04:42.686131 project_lighter-0.0.2a7/LICENSE
--rw-r--r--   0        0        0     2164 2023-07-06 19:04:42.686131 project_lighter-0.0.2a7/README.md
--rw-r--r--   0        0        0       67 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    17473 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     6508 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    19962 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/system.py
--rw-r--r--   0        0        0       36 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/__init__.py
--rw-r--r--   0        0        0      627 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/cli.py
--rw-r--r--   0        0        0     2566 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/collate.py
--rw-r--r--   0        0        0     1547 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3866 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2278 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/misc.py
--rw-r--r--   0        0        0     6293 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/model.py
--rw-r--r--   0        0        0     2483 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/runner.py
--rw-r--r--   0        0        0       24 2023-07-06 19:05:07.194157 project_lighter-0.0.2a7/lighter/version.py
--rw-r--r--   0        0        0     4420 2023-07-06 19:05:07.142157 project_lighter-0.0.2a7/pyproject.toml
--rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 project_lighter-0.0.2a7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-20 10:02:32.698939 project_lighter-0.0.2a8/LICENSE
+-rw-r--r--   0        0        0     2164 2023-07-20 10:02:32.698939 project_lighter-0.0.2a8/README.md
+-rw-r--r--   0        0        0       67 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0     6631 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/freezer.py
+-rw-r--r--   0        0        0    17459 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    18288 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/system.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3896 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5736 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-07-20 10:02:32.702939 project_lighter-0.0.2a8/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-07-20 10:02:56.247092 project_lighter-0.0.2a8/lighter/version.py
+-rw-r--r--   0        0        0     4611 2023-07-20 10:02:56.183091 project_lighter-0.0.2a8/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 project_lighter-0.0.2a8/PKG-INFO
```

### Comparing `project_lighter-0.0.2a7/LICENSE` & `project_lighter-0.0.2a8/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/README.md` & `project_lighter-0.0.2a8/README.md`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/callbacks/logger.py` & `project_lighter-0.0.2a8/lighter/callbacks/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 # Reduce the loss and average it on each rank.
                 loss = trainer.strategy.reduce(loss, reduce_op="mean")
                 # Divide the accumulated loss by the number of steps in the epoch.
                 loss /= self.epoch_step_counter[mode]
 
             # Metrics
             # Get the torchmetrics.
-            metric_collection = getattr(pl_module, f"{mode}_metrics")
+            metric_collection = pl_module.metrics[mode]
             if metric_collection is not None:
                 # Compute the epoch metrics.
                 metrics = metric_collection.compute()
                 # Reset the metrics for the next epoch.
                 metric_collection.reset()
 
             # Log. Only on rank 0.
```

### Comparing `project_lighter-0.0.2a7/lighter/callbacks/utils.py` & `project_lighter-0.0.2a8/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a8/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a8/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a8/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/system.py` & `project_lighter-0.0.2a8/lighter/system.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,178 +8,137 @@
 from loguru import logger
 from torch.nn import Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader, Dataset, Sampler
 from torchmetrics import Metric, MetricCollection
 
 from lighter.utils.collate import collate_replace_corrupted
-from lighter.utils.misc import ensure_list, get_name, hasarg
-from lighter.utils.model import reshape_pred_if_single_value_prediction
+from lighter.utils.misc import apply_fns, ensure_dict_schema, ensure_list, get_name, hasarg
 
 
 class LighterSystem(pl.LightningModule):
     """_summary_
 
     Args:
         model (Module): the model.
         batch_size (int): batch size.
         drop_last_batch (bool, optional): whether the last batch in the dataloader
             should be dropped. Defaults to False.
         num_workers (int, optional): number of dataloader workers. Defaults to 0.
         pin_memory (bool, optional): whether to pin the dataloaders memory. Defaults to True.
-        optimizers (Optional[Union[Optimizer, List[Optimizer]]], optional):
+        optimizer (Optional[Union[Optimizer, List[Optimizer]]], optional):
             a single or a list of optimizers. Defaults to None.
-        schedulers (Optional[Union[Callable, List[Callable]]], optional):
+        scheduler (Optional[Union[Callable, List[Callable]]], optional):
             a single or a list of schedulers. Defaults to None.
         criterion (Optional[Callable], optional):
             criterion/loss function. Defaults to None.
-        cast_target_dtype_to (Optional[str], optional): whether to cast the target to the
-            specified type before calculating the loss. May be necessary for some criterions.
-            Defaults to None.
-        post_criterion_activation (Optional[str], optional): some criterions
-            (e.g. BCEWithLogitsLoss) require non-activated prediction for their calculaiton.
-            However, to calculate the metrics and log the data, it may be necessary to activate
-            the predictions. Defaults to None.
+        datasets (Optional[Dict[str, Optional[Dataset]]], optional):
+            datasets for train, val, test, and predict. Supports Defaults to None.
+        samplers (Optional[Dict[str, Optional[Sampler]]], optional):
+            samplers for train, val, test, and predict. Defaults to None.
+        collate_fns (Optional[Dict[str, Optional[Callable]]], optional):
+            collate functions for train, val, test, and predict. Defaults to None.
+        metrics (Optional[Dict[str, Optional[Union[Metric, List[Metric]]]]], optional):
+            metrics for train, val, and test. Supports a single metric or a list of metrics,
+            implemented using `torchmetrics`. Defaults to None.
+        postprocessing (Optional[Dict[str, Optional[Callable]]], optional):
+            Postprocessing functions for input, target, and pred, for three stages - criterion, metrics,
+            and logging. The postprocessing is done before each stage - for example, criterion postprocessing
+            will be done prior to loss calculation. Note that the postprocessing of a latter stage stacks on
+            top of the previous one(s) - for example, the logging postprocessing will be done on the data that
+            has been postprocessed for the criterion and metrics earlier. Defaults to None.
         inferer (Optional[Callable], optional): the inferer must be a class with a `__call__`
             method that accepts two arguments - the input to infer over, and the model itself.
             Used in 'val', 'test', and 'predict' mode, but not in 'train'. Typically, an inferer
             is a sliding window or a patch-based inferer that will infer over the smaller parts of
             the input, combine them, and return a single output. The inferers provided by MONAI
             cover most of such cases (https://docs.monai.io/en/stable/inferers.html). Defaults to None.
-        freezer (Optional[Callable], optional): the freezer must be a class with a `__call__`
-            method that accepts three arguments - the model, the step, and the epoch number.
-            Use `lighter.utils.freezer.LighterFreezer` or implement your own based on it. Defaults to None.
-        train_metrics (Optional[Union[Metric, List[Metric]]], optional): training metric(s).
-            They have to be implemented using `torchmetrics`. Defaults to None.
-        val_metrics (Optional[Union[Metric, List[Metric]]], optional): validation metric(s).
-            They have to be implemented using `torchmetrics`. Defaults to None.
-        test_metrics (Optional[Union[Metric, List[Metric]]], optional): test metric(s).
-            They have to be implemented using `torchmetrics`. Defaults to None.
-        train_dataset (Optional[Union[Dataset, List[Dataset]]], optional): training dataset(s).
-            Defaults to None.
-        val_dataset (Optional[Union[Dataset, List[Dataset]]], optional): validation dataset(s).
-            Defaults to None.
-        test_dataset (Optional[Union[Dataset, List[Dataset]]], optional): test dataset(s).
-            Defaults to None.
-        predict_dataset (Optional[Union[Dataset, List[Dataset]]], optional): predict dataset(s).
-            Defaults to None.
-        train_sampler (Optional[Sampler], optional): training sampler(s). Defaults to None.
-        val_sampler (Optional[Sampler], optional): validation sampler(s). Defaults to None.
-        test_sampler (Optional[Sampler], optional):  test sampler(s). Defaults to None.
-        predict_sampler (Optional[Sampler], optional):  predict sampler(s). Defaults to None.
-        train_collate (Optional[Callable], optional): custom training collate function. Defaults to None.
-        val_collate (Optional[Callable], optional): custom validation collate function. Defaults to None.
-        test_collate (Optional[Callable], optional):  custom test collate function. Defaults to None.
-        predict_collate (Optional[Callable], optional):  custom predict collate function. Defaults to None.
     """
 
     def __init__(
         self,
         model: Module,
         batch_size: int,
         drop_last_batch: bool = False,
         num_workers: int = 0,
         pin_memory: bool = True,
-        optimizers: Optional[Union[Optimizer, List[Optimizer]]] = None,
-        schedulers: Optional[Union[Callable, List[Callable]]] = None,
+        optimizer: Optional[Union[Optimizer, List[Optimizer]]] = None,
+        scheduler: Optional[Union[Callable, List[Callable]]] = None,
         criterion: Optional[Callable] = None,
-        cast_target_dtype_to: Optional[str] = None,
-        post_criterion_activation: Optional[str] = None,
+        datasets: Optional[Dict[str, Optional[Dataset]]] = None,
+        samplers: Optional[Dict[str, Optional[Sampler]]] = None,
+        collate_fns: Optional[Dict[str, Optional[Callable]]] = None,
+        metrics: Optional[Dict[str, Optional[Union[Metric, List[Metric]]]]] = None,
+        postprocessing: Optional[Dict[str, Optional[Callable]]] = None,
         inferer: Optional[Callable] = None,
-        freezer: Optional[Callable] = None,
-        train_metrics: Optional[Union[Metric, List[Metric]]] = None,
-        val_metrics: Optional[Union[Metric, List[Metric]]] = None,
-        test_metrics: Optional[Union[Metric, List[Metric]]] = None,
-        train_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
-        val_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
-        test_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
-        predict_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
-        train_sampler: Optional[Sampler] = None,
-        val_sampler: Optional[Sampler] = None,
-        test_sampler: Optional[Sampler] = None,
-        predict_sampler: Optional[Sampler] = None,
-        train_collate: Optional[Callable] = None,
-        val_collate: Optional[Callable] = None,
-        test_collate: Optional[Callable] = None,
-        predict_collate: Optional[Callable] = None,
     ) -> None:
         super().__init__()
         # Bypass LightningModule's check for default methods. We define them in self.setup().
         self._init_placeholders_for_dataloader_and_step_methods()
 
         # Model setup
         self.model = model
         self.batch_size = batch_size
         self.drop_last_batch = drop_last_batch
 
         # Criterion, optimizer, and scheduler
         self.criterion = criterion
-        self.optimizers = ensure_list(optimizers)
-        self.schedulers = ensure_list(schedulers)
+        self.optimizer = ensure_list(optimizer)
+        self.scheduler = ensure_list(scheduler)
 
-        # Datasets
-        self.train_dataset = train_dataset
-        self.val_dataset = val_dataset
-        self.test_dataset = test_dataset
-        self.predict_dataset = predict_dataset
+        # DataLoader specifics
         self.num_workers = num_workers
         self.pin_memory = pin_memory
 
-        # Samplers
-        self.train_sampler = train_sampler
-        self.val_sampler = val_sampler
-        self.test_sampler = test_sampler
-        self.predict_sampler = predict_sampler
-
-        # Collate functions
-        self.train_collate = train_collate
-        self.val_collate = val_collate
-        self.test_collate = test_collate
-        self.predict_collate = predict_collate
+        # Datasets, samplers, and collate functions
+        schema = {"train": None, "val": None, "test": None, "predict": None}
+        self.datasets = ensure_dict_schema(datasets, schema)
+        self.samplers = ensure_dict_schema(samplers, schema)
+        self.collate_fns = ensure_dict_schema(collate_fns, schema)
 
         # Metrics
-        self.train_metrics = MetricCollection(ensure_list(train_metrics))
-        self.val_metrics = MetricCollection(ensure_list(val_metrics))
-        self.test_metrics = MetricCollection(ensure_list(test_metrics))
-
-        # Criterion-specific activation function and data type casting
-        self._post_criterion_activation = post_criterion_activation
-        self._cast_target_dtype_to = cast_target_dtype_to
+        self.metrics = ensure_dict_schema(metrics, schema={"train": None, "val": None, "test": None})
+        self.metrics = {mode: MetricCollection(ensure_list(metric)) for mode, metric in self.metrics.items()}
+        # Register the metrics to allow the LightningModule to automatically move them to the correct device.
+        # Currently, a workaround is needed because of https://github.com/pytorch/pytorch/issues/71203.
+        # Once it's fixed, we can set `self.metrics = ModuleDict(self.metrics)` directly.
+        for mode, mode_metrics in self.metrics.items():
+            setattr(self, f"{mode}_metric", mode_metrics)
+            self.metrics[mode] = getattr(self, f"{mode}_metric")
+
+        # Postprocessing
+        schema = {"input": None, "target": None, "pred": None}
+        schema = {"criterion": schema, "metrics": schema, "logging": schema}
+        self.postprocessing = ensure_dict_schema(postprocessing, schema)
 
         # Inferer for val, test, and predict
         self.inferer = inferer
 
-        # Layer freezer
-        self.freezer = freezer
-
         # Checks
         self._lightning_module_methods_defined = False
         self._target_not_used_reported = False
         self._batch_type_reported = False
 
     def forward(self, input: Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor], Dict[str, torch.Tensor]]) -> Any:
         """Forward pass. Multi-input models are supported.
 
         Args:
             input (torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor], Dict[str, torch.Tensor]): input to the model.
 
         Returns:
             Any: output of the model.
         """
-        # Freeze the layers if specified so.
-        if self.freezer is not None:
-            self.freezer(self.model, self.global_step, self.current_epoch)
 
         # Keyword arguments to pass to the forward method
         kwargs = {}
+        # Add `epoch` argument if forward accepts it
         if hasarg(self.model.forward, "epoch"):
-            # Add `epoch` argument if forward accepts it
             kwargs["epoch"] = self.current_epoch
+        # Add `step` argument if forward accepts it
         if hasarg(self.model.forward, "step"):
-            # Add `step` argument if forward accepts it
             kwargs["step"] = self.global_step
 
         return self.model(input, **kwargs)
 
     def _base_step(self, batch: Union[List, Tuple], batch_idx: int, mode: str) -> Union[Dict[str, Any], Any]:
         """Base step for all modes ("train", "val", "test", "predict")
 
@@ -220,69 +179,83 @@
 
         # Forward
         if self.inferer and mode in ["val", "test", "predict"]:
             pred = self.inferer(input, self)
         else:
             pred = self(input)
 
-        pred = reshape_pred_if_single_value_prediction(pred, target)
+        # Data postprocessing for criterion.
+        input = apply_fns(input, self.postprocessing["criterion"]["input"])
+        target = apply_fns(target, self.postprocessing["criterion"]["target"])
+        pred = apply_fns(pred, self.postprocessing["criterion"]["pred"])
 
         # Calculate the loss.
-        loss = None
-        if mode in ["train", "val"]:
-            loss = self._calculate_loss(pred, target)
-            loss_name = "loss" if mode == "train" else f"{mode}_loss"
-            # Log the loss and for monitoring purposes.
-            self.log(loss_name, loss, on_step=True, on_epoch=True, sync_dist=False, logger=False, batch_size=self.batch_size)
-
-        # Apply the post-criterion activation. Necessary for measuring the metrics
-        # correctly in cases when using a criterion such as `BCELossWithLogits`` which
-        # requires the model to output logits, i.e. non-activated outputs.
-        if self._post_criterion_activation is not None:
-            pred = self._post_criterion_activation(pred)
+        loss = self._calculate_loss(pred, target) if mode in ["train", "val"] else None
+        # Log the loss for monitoring purposes.
+        self.log(
+            "loss" if mode == "train" else f"{mode}_loss",
+            loss,
+            on_step=True,
+            on_epoch=True,
+            sync_dist=True,
+            logger=False,
+            batch_size=self.batch_size,
+        )
 
+        # Log and return the results.
         if mode == "predict":
-            # In predict mode, skip the metrics and return the predicted value only.
             return pred
         else:
+            # Data postprocessing for metrics
+            input = apply_fns(input, self.postprocessing["metrics"]["input"])
+            target = apply_fns(target, self.postprocessing["metrics"]["target"])
+            pred = apply_fns(pred, self.postprocessing["metrics"]["pred"])
+
             # Calculate the metrics for the step.
-            metrics = getattr(self, f"{mode}_metrics")(pred, target)
+            metrics = self.metrics[mode](pred, target)
             # Log the metrics for monitoring purposes.
-            self.log_dict(metrics, on_step=True, on_epoch=True, sync_dist=False, logger=False, batch_size=self.batch_size)
+            self.log_dict(metrics, on_step=True, on_epoch=True, sync_dist=True, logger=False, batch_size=self.batch_size)
+
+            # Data postprocessing for logging.
+            input = apply_fns(input, self.postprocessing["logging"]["input"])
+            target = apply_fns(target, self.postprocessing["logging"]["target"])
+            pred = apply_fns(pred, self.postprocessing["logging"]["pred"])
+
             # Return the loss, metrics, input, target, and pred.
             return {"loss": loss, "metrics": metrics, "input": input, "target": target, "pred": pred}
 
     def _calculate_loss(
         self, pred: Union[torch.Tensor, List, Tuple, Dict], target: Union[torch.Tensor, List, Tuple, Dict, None]
     ) -> torch.Tensor:
-        """_summary_
+        """Calculates the loss.
+        The method handles cases where the criterion function does not accept a `target` argument. If the criterion
+        function does not accept a `target` argument, the LighterSystem passes only the predicted values to the criterion.
 
         Args:
-            pred (torch.Tensor, List, Tuple, Dict, None): the predicted values from the model.
+            pred (torch.Tensor, List, Tuple, Dict): the predicted values from the model.
             target (torch.Tensor, List, Tuple, Dict, None): the target/label.
 
         Returns:
             torch.Tensor: the calculated loss.
         """
+
         # Keyword arguments to pass to the loss/criterion function
         kwargs = {}
+        # Add `target` argument if forward accepts it.
         if hasarg(self.criterion.forward, "target"):
-            # Add `target` argument if forward accepts it. Cast it if it is a tensor and if the target type is specified.
-            kwargs["target"] = target if not isinstance(target, torch.Tensor) else target.to(dtype=self._cast_target_dtype_to)
+            kwargs["target"] = target
         else:
             if not self._target_not_used_reported and not self.trainer.sanity_checking:
                 self._target_not_used_reported = True
                 logger.info(
                     f"The criterion `{get_name(self.criterion, True)}` "
                     "has no `target` argument. In such cases, the LighterSystem "
                     "passes only the predicted values to the criterion. "
-                    "This is intended as a support for self-supervised "
-                    "losses where target is not used. If this is not the "
-                    "behavior you expected, redefine your criterion "
-                    "so that it has a `target` argument."
+                    "If this is not the behavior you expected, redefine your "
+                    "criterion so that it has a `target` argument."
                 )
         return self.criterion(pred, **kwargs)
 
     def _base_dataloader(self, mode: str) -> DataLoader:
         """Instantiate the dataloader for a mode (train/val/test/predict).
         Includes a collate function that enables the DataLoader to replace
         None's (alias for corrupted examples) in the batch with valid examples.
@@ -291,21 +264,20 @@
 
         Args:
             mode (str): mode for which to create the dataloader ["train", "val", "test", "predict"].
 
         Returns:
             DataLoader: instantiated DataLoader.
         """
-        dataset = getattr(self, f"{mode}_dataset")
-        sampler = getattr(self, f"{mode}_sampler")
-        collate_fn = getattr(self, f"{mode}_collate")
+        dataset = self.datasets[mode]
+        sampler = self.samplers[mode]
+        collate_fn = self.collate_fns[mode]
 
         if dataset is None:
-            logger.error(f"Please specify '{mode}_dataset' in the config. Exiting")
-            sys.exit()
+            raise ValueError(f"Please specify '{mode}' dataset in the 'datasets' key of the config.")
 
         # Batch size is 1 when using an inference for two reasons:
         # 1) Inferer separates an input into multiple parts, forming a batch of its own.
         # 2) The val/test/pred data usually differ in their shape, so they cannot be stacked into a batch.
         batch_size = self.batch_size
         if self.inferer is not None and mode in ["val", "test", "predict"]:
             logger.info(f"Setting the '{mode}' mode dataloader to batch size of 1 because an inferer is provided.")
@@ -315,38 +287,38 @@
         # function replaces None's with valid examples from the dataset.
         collate_fn = partial(collate_replace_corrupted, dataset=dataset, default_collate_fn=collate_fn)
         return DataLoader(
             dataset,
             sampler=sampler,
             shuffle=(mode == "train" and sampler is None),
             batch_size=batch_size,
-            drop_last=self.drop_last_batch,
+            drop_last=(self.drop_last_batch if mode == "train" else False),
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             collate_fn=collate_fn,
         )
 
     def configure_optimizers(self) -> Union[Optimizer, List[Dict[str, Union[Optimizer, "Scheduler"]]]]:
         """LightningModule method. Returns optimizers and, if defined, schedulers.
 
         Returns:
             Optimizer or a List of Dict of paired Optimizers and Schedulers: instantiated
                 optimizers and/or schedulers.
         """
-        if not self.optimizers:
-            logger.error("Please specify 'system.optimizers' in the config. Exiting.")
+        if not self.optimizer:
+            logger.error("Please specify 'system.optimizer' in the config. Exiting.")
             sys.exit()
-        if not self.schedulers:
-            return self.optimizers
+        if not self.scheduler:
+            return self.optimizer
 
-        if len(self.optimizers) != len(self.schedulers):
+        if len(self.optimizer) != len(self.scheduler):
             logger.error("Each optimizer must have its own scheduler.")
             sys.exit()
 
-        return [{"optimizer": opt, "lr_scheduler": sched} for opt, sched in zip(self.optimizers, self.schedulers)]
+        return [{"optimizer": opt, "lr_scheduler": sched} for opt, sched in zip(self.optimizer, self.scheduler)]
 
     def setup(self, stage: str) -> None:
         """Automatically called by the LightningModule after the initialization.
         `LighterSystem`'s setup checks if the required dataset is provided in the config and
         sets up LightningModule methods for the stage in which the system is.
 
         Args:
@@ -361,25 +333,25 @@
                 self.val_dataloader,
                 self.validation_step,
                 self.test_dataloader,
                 self.test_step,
                 self.predict_dataloader,
                 self.predict_step,
             )
-            # `Trainer.tune()` calls the `self.setup()` method whenever it runs for a new
-            #  parameter, and deleting the above methods again breaks it. This flag prevents it.
+            # Prevents the methods from being defined again. This is needed because `Trainer.tune()`
+            # calls the `self.setup()` method whenever it runs for a new parameter.
             self._lightning_module_methods_defined = True
 
         # Training methods.
         if stage in ["fit", "tune"]:
             self.train_dataloader = partial(self._base_dataloader, mode="train")
             self.training_step = partial(self._base_step, mode="train")
 
         # Validation methods. Required in 'validate' stage and optionally in 'fit' or 'tune' stage.
-        if stage == "validate" or (stage in ["fit", "tune"] and self.val_dataset is not None):
+        if stage == "validate" or (stage in ["fit", "tune"] and self.datasets["val"] is not None):
             self.val_dataloader = partial(self._base_dataloader, mode="val")
             self.validation_step = partial(self._base_step, mode="val")
 
         # Test methods.
         if stage == "test":
             self.test_dataloader = partial(self._base_dataloader, mode="test")
             self.test_step = partial(self._base_step, mode="test")
@@ -387,15 +359,15 @@
         # Predict methods.
         if stage == "predict":
             self.predict_dataloader = partial(self._base_dataloader, mode="predict")
             self.predict_step = partial(self._base_step, mode="predict")
 
     def _init_placeholders_for_dataloader_and_step_methods(self) -> None:
         """`LighterSystem` dynamically defines the `..._dataloader()`and `..._step()` methods
-        in the `self.setup()` method. However, `LightningModule` excepts them to be defined at
-        the initialization. To prevent it from throwing an error, the `..._dataloader()` and
-        `..._step()` are initially defined as `lambda: None`, before `self.setup()` is called.
+        in the `self.setup()` method. However, when `LightningModule` excepts them to be defined
+        at init. To prevent it from throwing an error, the `..._dataloader()` and `..._step()`
+        are initially defined as `lambda: None`, before `self.setup()` is called.
         """
         self.train_dataloader = self.training_step = lambda: None
         self.val_dataloader = self.validation_step = lambda: None
         self.test_dataloader = self.test_step = lambda: None
         self.predict_dataloader = self.predict_step = lambda: None
```

### Comparing `project_lighter-0.0.2a7/lighter/utils/cli.py` & `project_lighter-0.0.2a8/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/utils/collate.py` & `project_lighter-0.0.2a8/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a8/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/lighter/utils/model.py` & `project_lighter-0.0.2a8/lighter/utils/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,14 @@
 import torch
 from loguru import logger
 from torch.nn import Identity, Module, Sequential
 
 from lighter.utils.misc import setattr_dot_notation
 
 
-def reshape_pred_if_single_value_prediction(pred: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-    """When the task is to predict a single value, pred and target dimensions often
-    mismatch - dataloader returns the value in the (B) shape, while the network
-    returns predictions in the (B, 1) shape, where the second dim is redundant.
-
-    Args:
-        pred (torch.Tensor): predicted tensor.
-        target (torch.Tensor): target tensor.
-
-    Returns:
-        torch.Tensor: reshaped predicted tensor if that was necessary.
-    """
-    if isinstance(pred, torch.Tensor) and target is not None:
-        if len(pred.shape) == 2 and len(target.shape) == 1 == pred.shape[1]:
-            return pred.flatten()
-    return pred
-
-
 def replace_layer_with(model: Module, layer_name: str, new_layer: Module) -> Module:
     """Replaces the specified layer of the network with another layer.
 
     Args:
         model (Module): PyTorch model to be edited
         layer_name (string): Name of the layer which will be replaced.
             Dot-notation supported, e.g. "layer10.fc".
@@ -38,16 +20,15 @@
     """
     setattr_dot_notation(model, layer_name, new_layer)
     return model
 
 
 def replace_layer_with_identity(model: Module, layer_name: str) -> Module:
     """Replaces any layer of the network with an Identity layer.
-    Useful for removing the last layer of a network to be used as a backbone
-    of an SSL model.
+    Useful for removing layers of a network to be used as a backbone.
 
     Args:
         model (Module): PyTorch model to be edited
         layer_name (string): Name of the layer which will be replaced with an
             Identity function. Dot-notation supported, e.g. "layer10.fc".
 
     Returns:
@@ -93,18 +74,20 @@
     Raises:
         ValueError: If there is no overlap between checkpoint's and model's state_dict.
     """
 
     # Load checkpoint
     ckpt = torch.load(ckpt_path)
 
-    # Check if the checkpoint is a model's state_dict or a Lightning checkpoint.
-    # A Lightning checkpoint contains the model’s entire internal state, we only need its state_dict.
+    # Check if the checkpoint is a model's state_dict or a LighterSystem checkpoint.
+    # A LighterSystem checkpoint contains the model’s entire internal state, we only need its state_dict.
     if "state_dict" in ckpt:
         ckpt = ckpt["state_dict"]
+        # Remove the "model." prefix from the checkpoint's state_dict keys. This is characteristic to LighterSystem.
+        ckpt = {key.replace("model.", ""): value for key, value in ckpt.items()}
 
     # Adjust the keys in the checkpoint's state_dict to match the the model's state_dict's keys.
     if ckpt_to_model_prefix is not None:
         for ckpt_prefix, model_prefix in ckpt_to_model_prefix.items():
             # Add a dot at the end of the prefix if necessary.
             ckpt_prefix = ckpt_prefix if ckpt_prefix == "" or ckpt_prefix.endswith(".") else f"{ckpt_prefix}."
             model_prefix = model_prefix if model_prefix == "" or model_prefix.endswith(".") else f"{model_prefix}."
```

### Comparing `project_lighter-0.0.2a7/lighter/utils/runner.py` & `project_lighter-0.0.2a8/lighter/utils/runner.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a7/pyproject.toml` & `project_lighter-0.0.2a8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a7"
+version = "0.0.2a8"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
@@ -38,47 +38,60 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-torch = "^2.0"
+torch = "2.0"
 pandas = "^1.5.3"
 torchvision = "^0.15"
 pytorch-lightning = "^2.0.0"
 fire = "^0.5.0"
 loguru = "^0.6.0"
 lightly = "^1.2.43"
 torchmetrics = "^0.11.0"
-py = "^1.11.0"
 tensorboard = "^2.11.2"
 monai-weekly = "^1.2.dev2305"
 requests = "^2.31.0"
 
-[tool.poetry.group.dev.dependencies]
-bandit = "^1.7.4"
+[tool.poetry.group.safety]
+optional = true
+
+[tool.poetry.group.style]
+optional = true
+
+[tool.poetry.group.tests]
+optional = true
+
+[tool.poetry.group.safety.dependencies]
+bandit = "^1.7.5"
+safety = "^2.3.5"
+
+[tool.poetry.group.style.dependencies]
 black = {version = "^23.1a1", allow-prereleases = true}
 isort = {extras = ["colors"], version = "^5.11.4"}
 mypy = "^0.991"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.21.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.15.10"
-pytest = "^7.2.1"
 pyupgrade = "^3.3.1"
-safety = "^2.3.5"
-coverage = "^7.0.5"
-coverage-badge = "^1.1.0"
+
+[tool.poetry.group.tests.dependencies]
+pytest = "^7.4.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.0.0"
-aiohttp = "^3.8.3"
-py = "^1.11.0"
-poetry-bumpversion = "^0.3.0"
+coverage = "^7.0.5"
+coverage-badge = "^1.1.0"
+
+[tool.poetry.group.dev.dependencies]
 typing-extensions = "^4.4.0"
+aiohttp = "^3.8.3"
+
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 127
 color = true
```

### Comparing `project_lighter-0.0.2a7/PKG-INFO` & `project_lighter-0.0.2a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,19 +18,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: lightly (>=1.2.43,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: monai-weekly (>=1.2.dev2305,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: py (>=1.11.0,<2.0.0)
 Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
-Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: torch (==2.0)
 Requires-Dist: torchmetrics (>=0.11.0,<0.12.0)
 Requires-Dist: torchvision (>=0.15,<0.16)
 Project-URL: Repository, https://github.com/lighter/lighter
 Description-Content-Type: text/markdown
 
 <div align="center">
 <picture>
```

