# Comparing `tmp/Xplique-1.0.0.tar.gz` & `tmp/Xplique-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xplique-1.0.0.tar", last modified: Mon May 29 15:27:13 2023, max compression
+gzip compressed data, was "Xplique-1.0.2.tar", last modified: Thu Jul 20 20:43:57 2023, max compression
```

## Comparing `Xplique-1.0.0.tar` & `Xplique-1.0.2.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-29 15:27:01.000000 Xplique-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    21904 2023-05-29 15:27:13.355503 Xplique-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21378 2023-05-29 15:27:01.000000 Xplique-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/Xplique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21904 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 15:27:13.355503 Xplique-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-05-29 15:27:01.000000 Xplique-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_deconvnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_guided_backprop.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_hsic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_rise.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_sobol.py
--rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/commons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_model_override.py
--rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/test_cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/test_tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_preconditionning.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/generic/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     5983 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_mege.py
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/test_metric_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/test_timeseries_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/deconvnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     4972 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/kernels.py
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2317 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/guided_backpropagation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)    26149 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     7484 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/rise.py
--rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/square_grad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/vargrad.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/commons/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/callable_operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/model_override.py
--rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/operators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/tf_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     6520 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/optim.py
--rw-r--r--   0 runner    (1001) docker     (122)     5433 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/preconditioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16580 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)     8702 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/representativity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5389 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     5166 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/types/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-20 20:43:46.000000 Xplique-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    22482 2023-07-20 20:43:57.904782 Xplique-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21956 2023-07-20 20:43:46.000000 Xplique-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/Xplique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    22482 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 20:43:57.904782 Xplique-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-07-20 20:43:46.000000 Xplique-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/tests/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_deconvnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_guided_backprop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_sobol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/test_cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/test_tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_maco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_preconditionning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/generic/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5983 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_mege.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/test_metric_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/test_timeseries_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/xplique/
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/deconvnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2317 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/guided_backpropagation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26149 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7484 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/square_grad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/vargrad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/callable_operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/tf_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7083 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/maco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6520 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/preconditioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16580 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8702 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/representativity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6566 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5389 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5166 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/types/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/types/__init__.py
```

### Comparing `Xplique-1.0.0/LICENSE` & `Xplique-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/PKG-INFO` & `Xplique-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 1.0.0
+Version: 1.0.2
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -112,14 +112,15 @@
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE">
         <img width="95%" src="./docs/assets/concepts.jpeg">
     </a>
 </p>
 
 - [**Feature Visualization**: Getting started](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) </sub>
+- [**Modern Feature Visualization with MaCo**: Getting started](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v"> 
         <img width="95%" src="./docs/assets/feature_viz.jpeg">
     </a>
 </p>
 
@@ -257,14 +258,16 @@
 | :----------------------------------------------------------------------------------- | :------------ | :----------------------------------------------------------------------------------------------------------------- |
 | Neurons                                                                              | TF            | Optimizes for specific neurons                                                                              |
 | Layer                                                                                | TF            | Optimizes for specific layers                                                                               |
 | Channel                                                                              | TF            | Optimizes for specific channels                                                                             |
 | Direction                                                                            | TF            | Optimizes for specific vector                                                                               |
 | Fourrier Preconditioning                                                             | TF            | Optimize in Fourier basis (see [preconditioning](https://distill.pub/2017/feature-visualization/#preconditioning)) |
 | Objective combination                                                                | TF            | Allows to combine objectives                                                                                       |
+| MaCo                                                                                 | TF            | Fixed Magnitude optimisation, see [Paper](https://arxiv.org/pdf/2306.06805.pdf)                                                                                       |
+
 
 <div align="right">
   <i>methods with TF need a Tensorflow model. </i>
 </div>
 
 ## 👍 Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 1.0.0 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.2 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
@@ -59,15 +59,19 @@
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE)
                          [./docs/assets/concepts.jpeg]
 - [**Feature Visualization**: Getting started](https://
 colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v)
+colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) - [**Modern
+Feature Visualization with MaCo**: Getting started](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic)
                        [./docs/assets/feature_viz.jpeg]
 You can find a certain number of [other practical tutorials just here](https://
 github.com/deel-ai/xplique/blob/master/TUTORIALS.md). This section is actively
 developed and more contents will be included. We will try to cover all the
 possible usage of the library, feel free to contact us if you have any
 suggestions or recommandations towards tutorials you would like to see. ## ð
 Quick Start Xplique requires a version of python higher than 3.6 and several
@@ -183,15 +187,16 @@
 ----- | :------------ | :------------------------------------------------------
 ----------------------------------------------------------- | | Neurons | TF |
 Optimizes for specific neurons | | Layer | TF | Optimizes for specific layers |
 | Channel | TF | Optimizes for specific channels | | Direction | TF | Optimizes
 for specific vector | | Fourrier Preconditioning | TF | Optimize in Fourier
 basis (see [preconditioning](https://distill.pub/2017/feature-visualization/
 #preconditioning)) | | Objective combination | TF | Allows to combine
-objectives |
+objectives | | MaCo | TF | Fixed Magnitude optimisation, see [Paper](https://
+arxiv.org/pdf/2306.06805.pdf) |
                                        methods with TF need a Tensorflow model.
 ## ð Contributing Feel free to propose your ideas or come and contribute
 with us on the Xplique toolbox! We have a specific document where we describe
 in a simple way how to make your first pull request: [just here](https://
 github.com/deel-ai/xplique/blob/master/CONTRIBUTING.md). ## ð See Also This
 library is one approach of many to explain your model. We don't expect it to be
 the perfect solution; we create it to explore one point in the space of
```

### Comparing `Xplique-1.0.0/README.md` & `Xplique-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE">
         <img width="95%" src="./docs/assets/concepts.jpeg">
     </a>
 </p>
 
 - [**Feature Visualization**: Getting started](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) </sub>
+- [**Modern Feature Visualization with MaCo**: Getting started](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v"> 
         <img width="95%" src="./docs/assets/feature_viz.jpeg">
     </a>
 </p>
 
@@ -239,14 +240,16 @@
 | :----------------------------------------------------------------------------------- | :------------ | :----------------------------------------------------------------------------------------------------------------- |
 | Neurons                                                                              | TF            | Optimizes for specific neurons                                                                              |
 | Layer                                                                                | TF            | Optimizes for specific layers                                                                               |
 | Channel                                                                              | TF            | Optimizes for specific channels                                                                             |
 | Direction                                                                            | TF            | Optimizes for specific vector                                                                               |
 | Fourrier Preconditioning                                                             | TF            | Optimize in Fourier basis (see [preconditioning](https://distill.pub/2017/feature-visualization/#preconditioning)) |
 | Objective combination                                                                | TF            | Allows to combine objectives                                                                                       |
+| MaCo                                                                                 | TF            | Fixed Magnitude optimisation, see [Paper](https://arxiv.org/pdf/2306.06805.pdf)                                                                                       |
+
 
 <div align="right">
   <i>methods with TF need a Tensorflow model. </i>
 </div>
 
 ## 👍 Contributing
```

#### html2text {}

```diff
@@ -52,15 +52,19 @@
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE)
                          [./docs/assets/concepts.jpeg]
 - [**Feature Visualization**: Getting started](https://
 colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v)
+colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) - [**Modern
+Feature Visualization with MaCo**: Getting started](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic)
                        [./docs/assets/feature_viz.jpeg]
 You can find a certain number of [other practical tutorials just here](https://
 github.com/deel-ai/xplique/blob/master/TUTORIALS.md). This section is actively
 developed and more contents will be included. We will try to cover all the
 possible usage of the library, feel free to contact us if you have any
 suggestions or recommandations towards tutorials you would like to see. ## ð
 Quick Start Xplique requires a version of python higher than 3.6 and several
@@ -176,15 +180,16 @@
 ----- | :------------ | :------------------------------------------------------
 ----------------------------------------------------------- | | Neurons | TF |
 Optimizes for specific neurons | | Layer | TF | Optimizes for specific layers |
 | Channel | TF | Optimizes for specific channels | | Direction | TF | Optimizes
 for specific vector | | Fourrier Preconditioning | TF | Optimize in Fourier
 basis (see [preconditioning](https://distill.pub/2017/feature-visualization/
 #preconditioning)) | | Objective combination | TF | Allows to combine
-objectives |
+objectives | | MaCo | TF | Fixed Magnitude optimisation, see [Paper](https://
+arxiv.org/pdf/2306.06805.pdf) |
                                        methods with TF need a Tensorflow model.
 ## ð Contributing Feel free to propose your ideas or come and contribute
 with us on the Xplique toolbox! We have a specific document where we describe
 in a simple way how to make your first pull request: [just here](https://
 github.com/deel-ai/xplique/blob/master/CONTRIBUTING.md). ## ð See Also This
 library is one approach of many to explain your model. We don't expect it to be
 the perfect solution; we create it to explore one point in the space of
```

### Comparing `Xplique-1.0.0/Xplique.egg-info/PKG-INFO` & `Xplique-1.0.2/Xplique.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 1.0.0
+Version: 1.0.2
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -112,14 +112,15 @@
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE">
         <img width="95%" src="./docs/assets/concepts.jpeg">
     </a>
 </p>
 
 - [**Feature Visualization**: Getting started](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) </sub>
+- [**Modern Feature Visualization with MaCo**: Getting started](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v"> 
         <img width="95%" src="./docs/assets/feature_viz.jpeg">
     </a>
 </p>
 
@@ -257,14 +258,16 @@
 | :----------------------------------------------------------------------------------- | :------------ | :----------------------------------------------------------------------------------------------------------------- |
 | Neurons                                                                              | TF            | Optimizes for specific neurons                                                                              |
 | Layer                                                                                | TF            | Optimizes for specific layers                                                                               |
 | Channel                                                                              | TF            | Optimizes for specific channels                                                                             |
 | Direction                                                                            | TF            | Optimizes for specific vector                                                                               |
 | Fourrier Preconditioning                                                             | TF            | Optimize in Fourier basis (see [preconditioning](https://distill.pub/2017/feature-visualization/#preconditioning)) |
 | Objective combination                                                                | TF            | Allows to combine objectives                                                                                       |
+| MaCo                                                                                 | TF            | Fixed Magnitude optimisation, see [Paper](https://arxiv.org/pdf/2306.06805.pdf)                                                                                       |
+
 
 <div align="right">
   <i>methods with TF need a Tensorflow model. </i>
 </div>
 
 ## 👍 Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 1.0.0 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.2 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
@@ -59,15 +59,19 @@
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE)
                          [./docs/assets/concepts.jpeg]
 - [**Feature Visualization**: Getting started](https://
 colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v)
+colab.research.google.com/drive/1st43K9AH-UL4eZM1S4QdyrOi7Epa5K8v) - [**Modern
+Feature Visualization with MaCo**: Getting started](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1l0kag1o-qMY4NCbWuAwnuzkzd9sf92ic)
                        [./docs/assets/feature_viz.jpeg]
 You can find a certain number of [other practical tutorials just here](https://
 github.com/deel-ai/xplique/blob/master/TUTORIALS.md). This section is actively
 developed and more contents will be included. We will try to cover all the
 possible usage of the library, feel free to contact us if you have any
 suggestions or recommandations towards tutorials you would like to see. ## ð
 Quick Start Xplique requires a version of python higher than 3.6 and several
@@ -183,15 +187,16 @@
 ----- | :------------ | :------------------------------------------------------
 ----------------------------------------------------------- | | Neurons | TF |
 Optimizes for specific neurons | | Layer | TF | Optimizes for specific layers |
 | Channel | TF | Optimizes for specific channels | | Direction | TF | Optimizes
 for specific vector | | Fourrier Preconditioning | TF | Optimize in Fourier
 basis (see [preconditioning](https://distill.pub/2017/feature-visualization/
 #preconditioning)) | | Objective combination | TF | Allows to combine
-objectives |
+objectives | | MaCo | TF | Fixed Magnitude optimisation, see [Paper](https://
+arxiv.org/pdf/2306.06805.pdf) |
                                        methods with TF need a Tensorflow model.
 ## ð Contributing Feel free to propose your ideas or come and contribute
 with us on the Xplique toolbox! We have a specific document where we describe
 in a simple way how to make your first pull request: [just here](https://
 github.com/deel-ai/xplique/blob/master/CONTRIBUTING.md). ## ð See Also This
 library is one approach of many to explain your model. We don't expect it to be
 the perfect solution; we create it to explore one point in the space of
```

### Comparing `Xplique-1.0.0/Xplique.egg-info/SOURCES.txt` & `Xplique-1.0.2/Xplique.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 tests/commons/test_model_override.py
 tests/commons/test_operators.py
 tests/concepts/__init__.py
 tests/concepts/test_cav.py
 tests/concepts/test_tcav.py
 tests/features_visualizations/__init__.py
 tests/features_visualizations/test_losses.py
+tests/features_visualizations/test_maco.py
 tests/features_visualizations/test_objectives.py
 tests/features_visualizations/test_optim.py
 tests/features_visualizations/test_preconditionning.py
 tests/features_visualizations/test_regularizers.py
 tests/features_visualizations/test_transformations.py
 tests/generic/__init__.py
 tests/generic/test_wrapper.py
@@ -87,14 +88,15 @@
 xplique/commons/operators.py
 xplique/commons/tf_operations.py
 xplique/concepts/__init__.py
 xplique/concepts/cav.py
 xplique/concepts/tcav.py
 xplique/features_visualizations/__init__.py
 xplique/features_visualizations/losses.py
+xplique/features_visualizations/maco.py
 xplique/features_visualizations/objectives.py
 xplique/features_visualizations/optim.py
 xplique/features_visualizations/preconditioning.py
 xplique/features_visualizations/regularizers.py
 xplique/features_visualizations/transformations.py
 xplique/metrics/__init__.py
 xplique/metrics/base.py
```

### Comparing `Xplique-1.0.0/setup.py` & `Xplique-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as fh:
     README = fh.read()
 
 setup(
     name="Xplique",
-    version="1.0.0",
+    version="1.0.2",
     description="Explanations toolbox for Tensorflow 2",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Thomas FEL",
     author_email="thomas_fel@brown.edu",
     license="MIT",
     install_requires=['tensorflow>=2.1.0', 'numpy', 'scikit-learn', 'scikit-image',
```

### Comparing `Xplique-1.0.0/tests/attributions/test_callable.py` & `Xplique-1.0.2/tests/attributions/test_callable.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_common.py` & `Xplique-1.0.2/tests/attributions/test_common.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_deconvnet.py` & `Xplique-1.0.2/tests/attributions/test_deconvnet.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_grad_cam.py` & `Xplique-1.0.2/tests/attributions/test_grad_cam.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_grad_cam_pp.py` & `Xplique-1.0.2/tests/attributions/test_grad_cam_pp.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_gradient_input.py` & `Xplique-1.0.2/tests/attributions/test_gradient_input.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_guided_backprop.py` & `Xplique-1.0.2/tests/attributions/test_guided_backprop.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_hsic.py` & `Xplique-1.0.2/tests/attributions/test_hsic.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_integrated_gradients.py` & `Xplique-1.0.2/tests/attributions/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_kernel_shap.py` & `Xplique-1.0.2/tests/attributions/test_kernel_shap.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_lime.py` & `Xplique-1.0.2/tests/attributions/test_lime.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_object_detector.py` & `Xplique-1.0.2/tests/attributions/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_occlusion.py` & `Xplique-1.0.2/tests/attributions/test_occlusion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_rise.py` & `Xplique-1.0.2/tests/attributions/test_rise.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_saliency.py` & `Xplique-1.0.2/tests/attributions/test_saliency.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_smoothgrad.py` & `Xplique-1.0.2/tests/attributions/test_smoothgrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_sobol.py` & `Xplique-1.0.2/tests/attributions/test_sobol.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/attributions/test_tabular_data.py` & `Xplique-1.0.2/tests/attributions/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/commons/test_data_conversion.py` & `Xplique-1.0.2/tests/commons/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/commons/test_model_override.py` & `Xplique-1.0.2/tests/commons/test_model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/commons/test_operators.py` & `Xplique-1.0.2/tests/commons/test_operators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/concepts/test_cav.py` & `Xplique-1.0.2/tests/concepts/test_cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/concepts/test_tcav.py` & `Xplique-1.0.2/tests/concepts/test_tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_losses.py` & `Xplique-1.0.2/tests/features_visualizations/test_losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_objectives.py` & `Xplique-1.0.2/tests/features_visualizations/test_objectives.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_optim.py` & `Xplique-1.0.2/tests/features_visualizations/test_optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_preconditionning.py` & `Xplique-1.0.2/tests/features_visualizations/test_preconditionning.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_regularizers.py` & `Xplique-1.0.2/tests/features_visualizations/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/features_visualizations/test_transformations.py` & `Xplique-1.0.2/tests/features_visualizations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/generic/test_wrapper.py` & `Xplique-1.0.2/tests/generic/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/metrics/test_common.py` & `Xplique-1.0.2/tests/metrics/test_common.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/metrics/test_fidelity.py` & `Xplique-1.0.2/tests/metrics/test_fidelity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/metrics/test_mege.py` & `Xplique-1.0.2/tests/metrics/test_mege.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/metrics/test_stability.py` & `Xplique-1.0.2/tests/metrics/test_stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/plots/test_metric_plots.py` & `Xplique-1.0.2/tests/plots/test_metric_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/plots/test_timeseries_plots.py` & `Xplique-1.0.2/tests/plots/test_timeseries_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/tests/utils.py` & `Xplique-1.0.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/__init__.py` & `Xplique-1.0.2/xplique/attributions/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/base.py` & `Xplique-1.0.2/xplique/attributions/base.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/deconvnet.py` & `Xplique-1.0.2/xplique/attributions/deconvnet.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/__init__.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,41 +94,35 @@
 
         Returns
         -------
         Kernel matrix
         """
         raise NotImplementedError()
 
-    def __call__(self, masks, outputs, nb_design):
+    @tf.function
+    def estimator(self, masks, L, nb_dim, nb_design):
         """
-        Compute the test statistic using a self.output_kernel for the output and a kernel to be
-        defined in child classes for the input.
+        tf operations related to the estimator for performances
 
         Parameters
         ----------
         masks
             binary masks, each dimension corresponding to an image patch
         L
-            Kernel matrix for the outputs
-        n
-            number of points used to estimate HSIC
+            output samples kernel Gram matrix
         nb_dim
-            number of patches
+            number of input variables to consider
+        nb_design
+            number of points used to estimate HSIC
 
         Returns
         -------
         HSIC estimates
-            Array with HSIC estimates for each patch
+            Raw HSIC estimates in tensorflow
         """
-        nb_dim = self.masks_dim(masks)
-
-        Y = tf.cast(outputs, tf.float32)
-        Y = tf.reshape(Y, (nb_design, 1))
-        L = self.output_kernel_func(Y, tf.transpose(Y))
-
         X = tf.transpose(masks)
 
         X1 = tf.reshape(X, (nb_dim, 1, nb_design, 1))
         X2 = tf.transpose(X1, [0, 1, 3, 2])
         K = self.input_kernel_func(X1, X2)
         K = tf.math.reduce_prod(1 + K, axis=1)
 
@@ -136,14 +130,43 @@
         HK = tf.einsum("jk,ikl->ijl", H, K)
         HL = tf.einsum("jk,kl->jl", H, L)
 
         Kc = tf.einsum("ijk,kl->ijl", HK, H)
         Lc = tf.einsum("jk,kl->jl", HL, H)
 
         score = tf.math.reduce_sum(Kc * tf.transpose(Lc), axis=[1, 2]) / nb_design
+        return score
+
+    def __call__(self, masks, outputs, nb_design):
+        """
+        Compute the test statistic using a self.output_kernel_func kernel for the output
+        and self.input_kernel_func for the input, to be defined in child classes
+        for the input.
+
+        Parameters
+        ----------
+        masks
+            binary masks, each dimension corresponding to an image patch
+        outputs
+            samples of the output variable
+        nb_design
+            number of points used to estimate HSIC
+
+        Returns
+        -------
+        HSIC estimates
+            Array with HSIC estimates for each patch
+        """
+        nb_dim = self.masks_dim(masks)
+
+        Y = tf.cast(outputs, tf.float32)
+        Y = tf.reshape(Y, (nb_design, 1))
+        L = self.output_kernel_func(Y, tf.transpose(Y))
+
+        score = self.estimator(masks, L, nb_dim, nb_design)
 
         return self.post_process(score, masks)
 
 
 class BinaryEstimator(HsicEstimator):
     """
     Estimator based on the Dirac kernel for the input
```

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/kernels.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/kernels.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/perturbations.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/perturbations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/replicated_designs.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/replicated_designs.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/samplers.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/samplers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py` & `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/grad_cam.py` & `Xplique-1.0.2/xplique/attributions/grad_cam.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/grad_cam_pp.py` & `Xplique-1.0.2/xplique/attributions/grad_cam_pp.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/gradient_input.py` & `Xplique-1.0.2/xplique/attributions/gradient_input.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/guided_backpropagation.py` & `Xplique-1.0.2/xplique/attributions/guided_backpropagation.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/integrated_gradients.py` & `Xplique-1.0.2/xplique/attributions/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/kernel_shap.py` & `Xplique-1.0.2/xplique/attributions/kernel_shap.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/lime.py` & `Xplique-1.0.2/xplique/attributions/lime.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/object_detector.py` & `Xplique-1.0.2/xplique/attributions/object_detector.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/occlusion.py` & `Xplique-1.0.2/xplique/attributions/occlusion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/rise.py` & `Xplique-1.0.2/xplique/attributions/rise.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/saliency.py` & `Xplique-1.0.2/xplique/attributions/saliency.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/smoothgrad.py` & `Xplique-1.0.2/xplique/attributions/smoothgrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/square_grad.py` & `Xplique-1.0.2/xplique/attributions/square_grad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/attributions/vargrad.py` & `Xplique-1.0.2/xplique/attributions/vargrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/__init__.py` & `Xplique-1.0.2/xplique/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/callable_operations.py` & `Xplique-1.0.2/xplique/commons/callable_operations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/data_conversion.py` & `Xplique-1.0.2/xplique/commons/data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/exceptions.py` & `Xplique-1.0.2/xplique/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/model_override.py` & `Xplique-1.0.2/xplique/commons/model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/operators.py` & `Xplique-1.0.2/xplique/commons/operators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/commons/tf_operations.py` & `Xplique-1.0.2/xplique/commons/tf_operations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/concepts/cav.py` & `Xplique-1.0.2/xplique/concepts/cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/concepts/tcav.py` & `Xplique-1.0.2/xplique/concepts/tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/features_visualizations/losses.py` & `Xplique-1.0.2/xplique/features_visualizations/losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/features_visualizations/objectives.py` & `Xplique-1.0.2/xplique/features_visualizations/objectives.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/features_visualizations/optim.py` & `Xplique-1.0.2/xplique/features_visualizations/optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/features_visualizations/preconditioning.py` & `Xplique-1.0.2/xplique/features_visualizations/transformations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,191 +1,209 @@
 """
-Images preconditionners
-
-Adaptation of the original Lucid library :
-https://github.com/tensorflow/lucid/blob/master/lucid/optvis/param/color.py
-Credit is due to the original Lucid authors.
+Stochastic transformations
 """
 
-
-import numpy as np
 import tensorflow as tf
 
-from ..types import Tuple, Union, Callable
+from ..types import Tuple, Callable, List
+
+
+def random_blur(sigma_range: Tuple[float, float] = (1.0, 2.0),
+                kernel_size: int = 10) -> Callable:
+    """
+    Generate a function that apply a random gaussian blur to the batch.
+
+    Parameters
+    ----------
+    sigma_range
+        Min and max sigma (or scale) of the gaussian kernel.
+    kernel_size
+        Size of the gaussian kernel
+
+    Returns
+    -------
+    blur
+        Transformation function applying random blur.
+    """
+    uniform = tf.linspace(-(kernel_size - 1) / 2., (kernel_size - 1) / 2.,
+                          kernel_size)
+    uniform_xx, uniform_yy = tf.meshgrid(uniform, uniform)
+
+    kernel_size = tf.cast(kernel_size, tf.float32)
+    sigma_min = tf.cast(max(sigma_range[0], 0.1), tf.float32)
+    sigma_max = tf.cast(max(sigma_range[1], 0.1), tf.float32)
+
+    def blur(images: tf.Tensor) -> tf.Tensor:
+        sigma = tf.random.uniform([], minval=sigma_min, maxval=sigma_max,
+                                  dtype=tf.float32)
+
+        kernel = tf.exp(-0.5 * (uniform_xx ** 2 + uniform_yy ** 2) / sigma ** 2)
+        kernel /= tf.reduce_sum(kernel)
 
+        kernel = tf.reshape(kernel, (kernel_size, kernel_size, 1, 1))
+        kernel = tf.tile(kernel, [1, 1, 3, 1])
 
-imagenet_color_correlation = tf.cast(
-      [[0.56282854, 0.58447580, 0.58447580],
-       [0.19482528, 0.00000000,-0.19482528],
-       [0.04329450,-0.10823626, 0.06494176]], tf.float32
-)
+        return tf.nn.depthwise_conv2d(images, kernel, strides=[1, 1, 1, 1],
+                                      padding='SAME')
 
+    return blur
 
-def recorrelate_colors(images: tf.Tensor) -> tf.Tensor:
+
+def random_jitter(delta: int = 6) -> Callable:
     """
-    Map uncorrelated colors to 'normal colors' by using empirical color
-    correlation matrix of ImageNet (see https://distill.pub/2017/feature-visualization/)
+    Generate a function that perform a random jitter on batch of images.
 
     Parameters
     ----------
-    images
-        Input samples , with N number of samples, W & H the sample dimensions,
-        and C the number of channels.
+    delta
+        Max of the shift
 
     Returns
     -------
-    images
-        Images recorrelated.
+    jitter
+        Transformation function applying random jitter.
+
     """
-    images_flat = tf.reshape(images, [-1, 3])
-    images_flat = tf.matmul(images_flat, imagenet_color_correlation)
-    return tf.reshape(images_flat, tf.shape(images))
 
+    def jitter(images: tf.Tensor) -> tf.Tensor:
+        shape = tf.shape(images)
+        images = tf.image.random_crop(images, (shape[0], shape[1] - delta, shape[2] - delta,
+                                               shape[-1]))
+        return images
 
-def to_valid_rgb(images: tf.Tensor,
-                 normalizer: Union[str, Callable] = 'sigmoid',
-                 values_range: Tuple[float, float] = (0, 1)) -> tf.Tensor:
-    """
-    Apply transformations to map tensors to valid rgb images.
+    return jitter
 
 
+def random_scale(scale_range: Tuple[float, float] = (0.95, 1.05)) -> Callable:
+    """
+    Generate a function that apply a random scaling to the batch. Preserve
+    aspect ratio.
+
     Parameters
     ----------
-    images
-        Input samples, with N number of samples, W & H the sample dimensions,
-        and C the number of channels.
-    normalizer
-        Transformation to apply to map pixels in the range [0, 1]. Either 'clip' or 'sigmoid'.
-    values_range
-        Range of values of the inputs that will be provided to the model, e.g (0, 1) or (-1, 1).
+    scale_range
+        Min and max scaling factor.
 
     Returns
     -------
-    images
-        Images after correction
+    scale
+        Transformation function applying random scaling.
     """
-    images = recorrelate_colors(images)
-
-    if normalizer == 'sigmoid':
-        images = tf.nn.sigmoid(images)
-    elif normalizer == 'clip':
-        images = tf.clip_by_value(images, values_range[0], values_range[1])
-    else:
-        images = normalizer(images)
+    min_scale = tf.cast(scale_range[0], tf.float32)
+    max_scale = tf.cast(scale_range[1], tf.float32)
 
-    # rescale according to value range
-    images = images - tf.reduce_min(images, (1, 2, 3), keepdims=True)
-    images = images / tf.reduce_max(images, (1, 2, 3), keepdims=True)
-    images *= values_range[1] - values_range[0]
-    images += values_range[0]
+    def scale(images: tf.Tensor) -> tf.Tensor:
+        _, width, height, _ = images.shape
+        scale_factor = tf.random.uniform([], minval=min_scale, maxval=max_scale,
+                                         dtype=tf.float32)
+        return tf.image.resize(images, tf.cast([width * scale_factor,
+                                                height * scale_factor], tf.int32))
 
-    return images
+    return scale
 
 
-def fft_2d_freq(width: int, height: int) -> np.ndarray:
+def random_flip(horizontal: bool = True, vertical: bool = False) -> Callable:
     """
-    Return the fft samples frequencies for a given width/height.
-    As we deal with real values (pixels), the Discrete Fourier Transform is
-    Hermitian symmetric, tensorflow's reverse operation requires only
-    the unique components (width, height//2+1).
+    Generate a function that apply random flip (horizontal/vertical) to the
+    batch.
 
     Parameters
     ----------
-    width
-        Width of the image.
-    height
-        Height of the image.
+    horizontal
+        Whether to perform random horizontal flipping (left/right)
+    vertical
+        Whether to perform random vertical flipping (top/down)
 
     Returns
     -------
-    frequencies
-        Array containing the samples frequency bin centers in cycles per pixels
+    flip
+        Transformation function applying random flipping.
     """
-    freq_y = np.fft.fftfreq(height)[:, np.newaxis]
 
-    cut_off = int(width % 2 == 1)
-    freq_x = np.fft.fftfreq(width)[:width//2+1+cut_off]
+    def flip(images: tf.Tensor) -> tf.Tensor:
+        if horizontal:
+            images = tf.image.random_flip_left_right(images)
+        if vertical:
+            images = tf.image.random_flip_up_down(images)
+        return images
 
-    return np.sqrt(freq_x**2 + freq_y**2)
+    return flip
 
 
-def get_fft_scale(width: int, height: int, decay_power: float = 1.0) -> tf.Tensor:
+def pad(size: int = 6, pad_value: float = 0.0) -> Callable:
     """
-    Generate 'scaler' to normalize spectrum energy. Also scale the energy by the
-    dimensions to use similar learning rate regardless of image size.
-    adaptation of : https://github.com/tensorflow/lucid/blob/master/lucid/optvis/param/spatial.py
-    #L73
+    Generate a function that apply padding to a batch of images.
 
     Parameters
     ----------
-    width
-        Width of the image.
-    height
-        Height of the image.
-    decay_power
-        Control the allowed energy of the high frequency, a high value
-        suppresses high frequencies.
+    size
+        Size of the padding
+    pad_value
+        Value of the padded pixels
 
     Returns
     -------
-    fft_scale
-        Scale factor of the fft spectrum
+    pad_func
+        Transformation function applying padding.
     """
-    frequencies = fft_2d_freq(width, height)
-    fft_scale = 1.0 / np.maximum(frequencies, 1.0 / max(width, height)) ** decay_power
-    fft_scale = fft_scale * np.sqrt(width * height)
+    pad_array = [(0, 0), (size, size), (size, size), (0, 0)]
+    pad_value = tf.cast(pad_value, tf.float32)
 
-    return tf.convert_to_tensor(fft_scale, dtype=tf.complex64)
+    def pad_func(images: tf.Tensor) -> tf.Tensor:
+        return tf.pad(images, pad_array, mode="CONSTANT", constant_values=pad_value)
 
+    return pad_func
 
-def fft_to_rgb(shape: Tuple, buffer: tf.Tensor, fft_scale: tf.Tensor) -> tf.Tensor:
+
+def compose_transformations(transformations: List[Callable]) -> Callable:
     """
-    Convert a fft buffer into images.
+    Return a function that combine all the transformations passed and resize
+    the images at the end.
 
     Parameters
     ----------
-    shape
-        Shape of the images with N number of samples, W & H the sample
-        dimensions, and C the number of channels.
-    buffer
-        Image buffer in the fourier basis.
-    fft_scale
-        Scale factor of the fft spectrum
+    transformations
+        List of transformations, like the one in this module.
 
     Returns
     -------
-    images
-        Images in the 'pixels' basis.
+    composed_func
+        The combinations of the functions passed and a resize.
     """
-    batch, width, height, channels = shape
-    spectrum = tf.complex(buffer[0], buffer[1]) * fft_scale
 
-    image = tf.signal.irfft2d(spectrum)
-    image = tf.transpose(image, (0, 2, 3, 1))
-    image = image[:batch, :width, :height, :channels]
+    def composed_func(images: tf.Tensor) -> tf.Tensor:
+        for func in transformations:
+            images = func(images)
+        return images
 
-    return image / 4.0
+    return composed_func
 
 
-def fft_image(shape: Tuple, std: float = 0.01) -> tf.Tensor:
+def generate_standard_transformations(size: int) -> Callable:
     """
-    Generate the preconditioned image buffer
+    Prepare a set of (apparently) robust transformations.
 
     Parameters
     ----------
-    shape
-        Shape of the images with N number of samples, W & H the sample
-        dimensions, and C the number of channels.
-    std
-        Standard deviation of the normal for the buffer initialization
+    size
+        Input size of the image.
+
     Returns
     -------
-    buffer
-        Image buffer in the fourier basis.
+    transformations
+        A combinations of transformations to make the optimization robust.
     """
-    batch, width, height, channels = shape
-    frequencies = fft_2d_freq(width, height)
-
-    buffer = tf.random.normal((2, batch, channels)+frequencies.shape,
-                              stddev=std)
+    unit = int(size / 16)
 
-    return buffer
+    return compose_transformations([
+        pad(unit * 4, 0.0),
+        random_jitter(unit * 2),
+        random_jitter(unit * 2),
+        random_jitter(unit * 4),
+        random_jitter(unit * 4),
+        random_jitter(unit * 4),
+        random_scale((0.92, 0.96)),
+        random_blur(sigma_range=(1.0, 1.1)),
+        random_jitter(unit),
+        random_jitter(unit),
+        random_flip()
+    ])
```

### Comparing `Xplique-1.0.0/xplique/features_visualizations/regularizers.py` & `Xplique-1.0.2/xplique/features_visualizations/regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/metrics/base.py` & `Xplique-1.0.2/xplique/metrics/base.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/metrics/fidelity.py` & `Xplique-1.0.2/xplique/metrics/fidelity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/metrics/representativity.py` & `Xplique-1.0.2/xplique/metrics/representativity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/metrics/stability.py` & `Xplique-1.0.2/xplique/metrics/stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/plots/image.py` & `Xplique-1.0.2/xplique/plots/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,40 +27,39 @@
     image = np.array(image, np.float32)
 
     image -= image.min()
     image /= image.max()
 
     return image
 
-def _clip_percentile(heatmap: Union[tf.Tensor, np.ndarray],
+def _clip_percentile(tensor: Union[tf.Tensor, np.ndarray],
                      percentile: float) -> np.ndarray:
     """
-    Apply clip according to percentile value (percentile, 100-percentile) of a heatmap
+    Apply clip according to percentile value (percentile, 100-percentile) of a tensor
     only if percentile is not None.
 
     Parameters
     ----------
-    heatmap
-        Heatmap to clip.
+    tensor
+        tensor to clip.
 
     Returns
     -------
-    heatmap_clipped
-        Heatmap clipped accordingly to the percentile value.
+    tensor_clipped
+        Tensor clipped accordingly to the percentile value.
     """
-    assert len(heatmap.shape) == 2 or heatmap.shape[-1] == 1, "Clip percentile is only supposed"\
-                                                              "to be applied on heatmap."
+
     assert 0. <= percentile <= 100., "Percentile value should be in [0, 100]"
 
     if percentile is not None:
-        clip_min = np.percentile(heatmap, percentile)
-        clip_max = np.percentile(heatmap, 100. - percentile)
-        heatmap = np.clip(heatmap, clip_min, clip_max)
+        clip_min = np.percentile(tensor, percentile)
+        clip_max = np.percentile(tensor, 100. - percentile)
+        tensor = np.clip(tensor, clip_min, clip_max)
 
-    return heatmap
+    return tensor
 
 
 def plot_attribution(explanation,
                       image: Optional[np.ndarray] = None,
                       cmap: str = "jet",
                       alpha: float = 0.5,
                       clip_percentile: Optional[float] = 0.1,
@@ -184,7 +183,37 @@
             if img.shape[-1] == 1:
                 plt.imshow(img[:,:,0], cmap="Greys")
             else:
                 plt.imshow(img)
 
         plot_attribution(explanation, cmap=cmap, alpha=alpha, clip_percentile=clip_percentile,
                          absolute_value=absolute_value, **plot_kwargs)
+
+def plot_maco(image, alpha, percentile_image=1.0, percentile_alpha=80):
+    """
+    Plot maco feature visualization image (take care of merging the alpha).
+
+    Parameters
+    ----------
+    image
+        Image to plot.
+    alpha
+        Alpha channel to plot.
+    percentile_image
+        Percentile value to use to ceil the image and avoid extreme values.
+    percentile_alpha
+        Percentile value to use to ceil the alpha channel. A higher value will result in a more
+        transparent image with only the most important features.
+    """
+
+    image = np.array(image).copy()
+    image = _clip_percentile(image, percentile_image)
+
+    alpha = np.mean(np.array(alpha).copy(), -1, keepdims=True)
+    alpha = np.clip(alpha, 0, np.percentile(alpha, percentile_alpha))
+    alpha = alpha / alpha.max()
+
+    image = image * alpha
+    image = _normalize(image)
+
+    plt.imshow(np.concatenate([image, alpha], -1))
+    plt.axis('off')
```

### Comparing `Xplique-1.0.0/xplique/plots/metrics.py` & `Xplique-1.0.2/xplique/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/plots/tabular.py` & `Xplique-1.0.2/xplique/plots/tabular.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.0/xplique/plots/timeseries.py` & `Xplique-1.0.2/xplique/plots/timeseries.py`

 * *Files identical despite different names*

