# Comparing `tmp/azureml-assets-1.7.2.tar.gz` & `tmp/azureml-assets-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.7.2.tar", last modified: Thu Jul 20 18:44:18 2023, max compression
+gzip compressed data, was "azureml-assets-1.8.0.tar", last modified: Thu Jul 20 18:41:20 2023, max compression
```

## Comparing `azureml-assets-1.7.2.tar` & `azureml-assets-1.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.685279 azureml-assets-1.7.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:44:18.685279 azureml-assets-1.7.2/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.677279 azureml-assets-1.7.2/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.681279 azureml-assets-1.7.2/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37800 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.681279 azureml-assets-1.7.2/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17109 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.681279 azureml-assets-1.7.2/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13212 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.685279 azureml-assets-1.7.2/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15662 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17283 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:44:18.685279 azureml-assets-1.7.2/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:44:18.000000 azureml-assets-1.7.2/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-20 18:44:18.000000 azureml-assets-1.7.2/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-20 18:44:18.000000 azureml-assets-1.7.2/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-20 18:44:18.000000 azureml-assets-1.7.2/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-20 18:44:18.000000 azureml-assets-1.7.2/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-20 18:44:18.685279 azureml-assets-1.7.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-20 18:43:41.000000 azureml-assets-1.7.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.746642 azureml-assets-1.8.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37800 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17323 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13212 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.750642 azureml-assets-1.8.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15662 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17283 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-20 18:41:20.000000 azureml-assets-1.8.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-20 18:41:20.754642 azureml-assets-1.8.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-20 18:40:38.000000 azureml-assets-1.8.0/setup.py
```

### Comparing `azureml-assets-1.7.2/PKG-INFO` & `azureml-assets-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.7.2
+Version: 1.8.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.7.2/azureml/assets/__init__.py` & `azureml-assets-1.8.0/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/asset_utils.py` & `azureml-assets-1.8.0/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/config.py` & `azureml-assets-1.8.0/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/copy_assets.py` & `azureml-assets-1.8.0/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/deployment_config.py` & `azureml-assets-1.8.0/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/environment/build.py` & `azureml-assets-1.8.0/azureml/assets/environment/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 TASK_FILENAME = "_acr_build_task.yaml"
 BUILD_STEP_TIMEOUT_SECONDS = 60 * 90
 SCAN_STEP_TIMEOUT_SECONDS = 60 * 20
 TRIVY_TIMEOUT = "15m0s"
 SUCCESS_COUNT = "success_count"
 FAILED_COUNT = "failed_count"
 COUNTERS = [SUCCESS_COUNT, FAILED_COUNT]
+BUILT_IMAGES = "built_images"
 
 
 def create_acr_task(image_name: str,
                     dockerfile: str,
                     os: assets.Os,
                     task_filename: str,
                     test_command: str = None,
@@ -109,30 +110,30 @@
                 env_config: assets.EnvironmentConfig,
                 image_name: str,
                 build_log: Path,
                 resource_group: str = None,
                 registry: str = None,
                 test_command: str = None,
                 push: bool = False,
-                trivy_url: str = None) -> Tuple[assets.AssetConfig, int, str]:
+                trivy_url: str = None) -> Tuple[assets.AssetConfig, str, int, str]:
     """Build a Docker image locally or via ACR task.
 
     Args:
         asset_config (assets.AssetConfig): Asset config.
         env_config (assets.EnvironmentConfig): Environment config.
         image_name (str): Image name.
         build_log (Path): File to which the build log will be written.
         resource_group (str, optional): Resource group of the ACR. Defaults to None.
         registry (str, optional): ACR name. Defaults to None.
         test_command (str, optional): Command used to test the image. Defaults to None.
         push (bool, optional): Push the image to the ACR. Defaults to False.
         trivy_url (str, optional): URL to download Trivy for vulnerability scanning. Defaults to None.
 
     Returns:
-        Tuple[assets.AssetConfig, int, str]: Asset config, return code, and contents of stdout.
+        Tuple[assets.AssetConfig, str, int, str]: Asset config, image name, return code, and contents of stdout.
     """
     logger.print(f"Building image for {asset_config.name}")
     start = timer()
     with tempfile.TemporaryDirectory() as temp_dir:
         if registry is not None:
             # Build via ACR task
             temp_dir_path = Path(temp_dir)
@@ -152,15 +153,15 @@
                 stdout=PIPE,
                 stderr=STDOUT)
     end = timer()
     logger.print(f"Image for {asset_config.name} built in {timedelta(seconds=end-start)}")
     os.makedirs(build_log.parent, exist_ok=True)
     with open(build_log, "w") as f:
         f.write(p.stdout.decode())
-    return (asset_config, p.returncode, p.stdout.decode())
+    return (asset_config, image_name, p.returncode, p.stdout.decode())
 
 
 # Doesn't support ACR yet
 def get_image_digest(image_name: str) -> str:
     """Get image digest for a local image.
 
     Args:
@@ -265,33 +266,36 @@
             build_log = build_logs_dir / f"{asset_config.name}.log"
             futures.append(pool.submit(build_image, asset_config=asset_config, env_config=env_config,
                                        image_name=image_name, build_log=build_log, resource_group=resource_group,
                                        registry=registry, test_command=test_command, push=push_this_image,
                                        trivy_url=trivy_url))
 
         # Wait for builds to complete
+        built_images = []
         for future in as_completed(futures):
-            (asset_config, return_code, output) = future.result()
+            (asset_config, image_name, return_code, output) = future.result()
             logger.start_group(f"{asset_config.name} build log")
             logger.print(output)
             logger.end_group()
             if return_code != 0:
                 logger.log_error(f"Build of image for {asset_config.name} failed with exit status {return_code}",
                                  "Build failure")
                 counters[FAILED_COUNT] += 1
             else:
                 logger.log_debug(f"Successfully built image for {asset_config.name}")
                 counters[SUCCESS_COUNT] += 1
+                built_images.append(image_name)
                 if output_directory:
                     util.copy_asset_to_output_dir(asset_config=asset_config, output_directory=output_directory,
                                                   add_subdir=True, use_version_dir=use_version_dirs)
 
     # Set variables
     for counter_name in COUNTERS:
         logger.set_output(counter_name, counters[counter_name])
+    logger.set_output(BUILT_IMAGES, ",".join(built_images))
 
     if counters[FAILED_COUNT] > 0:
         logger.log_error(f"{counters[FAILED_COUNT]} environment image(s) failed to build")
         return False
     return True
```

### Comparing `azureml-assets-1.7.2/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.8.0/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.8.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.8.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.8.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.8.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/model/utils.py` & `azureml-assets-1.8.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/tag_released_assets.py` & `azureml-assets-1.8.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/update_assets.py` & `azureml-assets-1.8.0/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/update_spec.py` & `azureml-assets-1.8.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/util/__init__.py` & `azureml-assets-1.8.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/util/logger.py` & `azureml-assets-1.8.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/util/template.py` & `azureml-assets-1.8.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/util/util.py` & `azureml-assets-1.8.0/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml/assets/validate_assets.py` & `azureml-assets-1.8.0/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.8.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.7.2
+Version: 1.8.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.7.2/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.8.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.7.2/setup.py` & `azureml-assets-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.7.2",
+   version="1.8.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

