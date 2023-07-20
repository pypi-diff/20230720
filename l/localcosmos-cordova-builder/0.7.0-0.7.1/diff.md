# Comparing `tmp/localcosmos_cordova_builder-0.7.0.tar.gz` & `tmp/localcosmos_cordova_builder-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_cordova_builder-0.7.0.tar", last modified: Thu Apr 27 08:10:41 2023, max compression
+gzip compressed data, was "localcosmos_cordova_builder-0.7.1.tar", last modified: Thu Jul 20 14:10:30 2023, max compression
```

## Comparing `localcosmos_cordova_builder-0.7.0.tar` & `localcosmos_cordova_builder-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.676923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/
--rw-r--r--   0 tom       (1000) tom       (1000)     9443 2023-04-26 15:54:18.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/AppImageCreator.py
--rw-r--r--   0 tom       (1000) tom       (1000)    31637 2023-04-26 16:14:22.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/CordovaAppBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    19752 2023-01-31 15:32:09.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/JobManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/MetaAppDefinition.py
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4257 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/image_utils.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/logger.py
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/required_assets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.672923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/
--rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4077 2023-04-26 15:23:50.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/urllib_request_upload_files.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-27 08:10:41.676923 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      927 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       28 2023-04-27 08:10:41.000000 localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-27 08:10:41.680923 localcosmos_cordova_builder-0.7.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1007 2023-04-27 08:10:06.000000 localcosmos_cordova_builder-0.7.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1070 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)       57 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      214 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9443 2023-04-26 15:54:18.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/AppImageCreator.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31818 2023-07-20 14:05:57.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/CordovaAppBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    19819 2023-07-20 14:05:57.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/JobManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2102 2023-02-01 10:58:47.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/MetaAppDefinition.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2023-01-31 12:39:35.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4257 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/image_utils.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)      974 2022-12-08 09:26:06.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/logger.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-01-31 12:38:43.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/required_assets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)      283 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2154 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4077 2023-04-26 15:23:50.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2494 2022-12-05 13:13:59.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/urllib_request_upload_files.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2023-07-20 14:10:30.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      927 2023-07-20 14:10:30.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-20 14:10:30.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-07-20 14:10:30.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       28 2023-07-20 14:10:30.000000 localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-07-20 14:10:30.858355 localcosmos_cordova_builder-0.7.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1007 2023-07-20 14:09:03.000000 localcosmos_cordova_builder-0.7.1/setup.py
```

### Comparing `localcosmos_cordova_builder-0.7.0/LICENSE` & `localcosmos_cordova_builder-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/PKG-INFO` & `localcosmos_cordova_builder-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_cordova_builder
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/AppImageCreator.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/AppImageCreator.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/CordovaAppBuilder.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/CordovaAppBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         # add stuff to config
         # <preference name="SplashMaintainAspectRatio" value="true" />
         # <preference name="StatusBarStyle" value="blackopaque" />
         # <preference name="StatusBarOverlaysWebView" value="false" />
         # <preference name="StatusBarBackgroundColor" value="#000000" />
 
         preferences = [
-            #{'name' : 'SplashMaintainAspectRatio', 'value' : 'true'},
+            {'name' : 'SplashMaintainAspectRatio', 'value' : 'true'},
             {'name' : 'StatusBarStyle', 'value' : 'blackopaque'},
             {'name' : 'StatusBarOverlaysWebView', 'value' : 'false'},
             {'name' : 'StatusBarBackgroundColor', 'value' : '#000000'},
             {'name' : 'DisallowOverscroll', 'value': 'true'},
         ]
 
         for tag_attributes in preferences:
@@ -627,14 +627,17 @@
         self.set_ios_info_plist_value('NSPhotoLibraryUsageDescription',
                                       'photo library access is required for adding pictures to observations')
         
         # NSLocationAlwaysUsageDescription
         self.set_ios_info_plist_value('NSLocationAlwaysUsageDescription',
                                       'location access is required for observations and maps')
 
+        self.set_ios_info_plist_value('NSLocationAlwaysAndWhenInUseUsageDescription',
+                                      'location access is required for observations and maps')
+
         # enable wkwebview
         # self.config_xml_enable_wkwebview()
 
         self.logger.info('Adding ios platform')
         platform_version = self._get_cordova_platform_version(PLATFORM_IOS)
         add_ios_command = [self.cordova_bin, 'platform', 'add', platform_version]
```

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/JobManager.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/JobManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,16 @@
         
         response = request.execute()
         
         if response is not None:
 
             # results contain only unassigned jobs
             for job in response['results']:
+                
+                self.logger.info(json.dumps(job))
 
                 # meta_app_uuid and job_type
                 results = AppKitJob.select().where(AppKitJob.meta_app_uuid==job['meta_app_uuid'],
                                                    AppKitJob.job_type==job['job_type'])
 
                 result_count = len(results)
```

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/MetaAppDefinition.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/MetaAppDefinition.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/image_utils.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/image_utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/logger.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/logger.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/adaptive_launcher_background.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/resources/images/appLauncherIcon.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder/urllib_request_upload_files.py` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder/urllib_request_upload_files.py`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/PKG-INFO` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos-cordova-builder
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create android and ios app packages for Local Cosmos apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-cordova-builder
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: localcosmos,app kit,cordova builder
 Platform: OS Independent
```

### Comparing `localcosmos_cordova_builder-0.7.0/localcosmos_cordova_builder.egg-info/SOURCES.txt` & `localcosmos_cordova_builder-0.7.1/localcosmos_cordova_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_cordova_builder-0.7.0/setup.py` & `localcosmos_cordova_builder-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'lxml>=4.3.4',
     'tendo',
     'Pillow',
 ]
 
 setup(
     name='localcosmos_cordova_builder',
-    version='0.7.0',
+    version='0.7.1',
     description='Create android and ios app packages for Local Cosmos apps.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='localcosmos, app kit, cordova builder',
     author='Thomas Uher',
```

