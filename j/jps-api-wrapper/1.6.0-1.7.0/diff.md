# Comparing `tmp/jps_api_wrapper-1.6.0.tar.gz` & `tmp/jps_api_wrapper-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jps_api_wrapper-1.6.0.tar", last modified: Tue Jun 13 16:27:06 2023, max compression
+gzip compressed data, was "jps_api_wrapper-1.7.0.tar", last modified: Thu Jul 20 17:43:15 2023, max compression
```

## Comparing `jps_api_wrapper-1.6.0.tar` & `jps_api_wrapper-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.857386 jps_api_wrapper-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8112 2023-06-13 16:27:06.857386 jps_api_wrapper-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-13 16:27:06.858386 jps_api_wrapper-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.853386 jps_api_wrapper-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.855386 jps_api_wrapper-1.6.0/src/jps_api_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 16:26:40.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   262861 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/classic.py
--rw-rw-rw-   0 root         (0) root         (0)   312452 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/pro.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     6752 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.856386 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8112 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.856386 jps_api_wrapper-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)   290397 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/tests/test_classic.py
--rw-rw-rw-   0 root         (0) root         (0)   211163 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/tests/test_pro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.310837 jps_api_wrapper-1.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.312837 jps_api_wrapper-1.7.0/src/jps_api_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:42:45.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   262861 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   318985 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/pro.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.313837 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.313837 jps_api_wrapper-1.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   290397 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/tests/test_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   212692 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/tests/test_pro.py
```

### Comparing `jps_api_wrapper-1.6.0/LICENSE` & `jps_api_wrapper-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/PKG-INFO` & `jps_api_wrapper-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps_api_wrapper
-Version: 1.6.0
+Version: 1.7.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.6.0/README.md` & `jps_api_wrapper-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/setup.cfg` & `jps_api_wrapper-1.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jps_api_wrapper
-version = 1.6.0
+version = 1.7.0
 description = Jamf Pro Server API Python wrapper
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 readme = README.md
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `jps_api_wrapper-1.6.0/src/jps_api_wrapper/classic.py` & `jps_api_wrapper-1.7.0/src/jps_api_wrapper/classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/src/jps_api_wrapper/pro.py` & `jps_api_wrapper-1.7.0/src/jps_api_wrapper/pro.py`

 * *Files 0% similar despite different names*

```diff
@@ -2361,14 +2361,28 @@
         endpoint = "/api/v1/csa/token"
 
         return self._delete(
             endpoint, success_message="CSA Token Exchange successfully deleted."
         )
 
     """
+    dashboard
+    """
+
+    def get_dashboard(self) -> dict:
+        """
+        Returns all the dashboard information for widgets and setup tasks
+
+        :returns: Dashboard information in JSON
+        """
+        endpoint = "/api/v1/dashboard"
+
+        return self._get(endpoint)
+
+    """
     departments
     """
 
     def get_departments(
         self,
         page: int = None,
         page_size: int = None,
@@ -5229,15 +5243,17 @@
     def get_managed_software_updates_statuses(self, filter: str = None) -> dict:
         """
         Returns managed software update statuses
 
         :param filter:
             Query in the RSQL format, allowing to filter Managed Software
             Updates collection. Default filter is empty query - returning all
-            results for the requested page. Fields allowed in the query:
+            results for the requested page.
+
+            Options:
             osUpdatesStatusId, device.deviceId, device.objectType, downloaded,
             downloadPercentComplete, productKey, status, deferralsRemaining,
             maxDeferrals, nextScheduledInstall, created and updated.
 
         :returns: Managed software update statuses information in JSON
         """
         params = remove_empty_params({"filter": filter})
@@ -5335,15 +5351,15 @@
             Query in the RSQL format, allowing to filter, for a list of
             commands. All url must contain minimum one filter field. Fields
             allowed in the query: uuid, clientManagementId, command, status,
             clientType, dateSent, validAfter, dateCompleted, profileIdentifier,
             and active. This param can be combined with paging. Filter needs to
             be set to something otherwise it will return a 400 error.
 
-            Example: status==Pending
+            Example: 'status==Pending'
 
         :returns: All MDM commands in JSON
         """
         params = remove_empty_params(
             {
                 "page": page,
                 "page-size": page_size,
@@ -5472,15 +5488,15 @@
             Query in the RSQL format, allowing to filter department collection.
             Default filter is empty query - returning all results for the
             requested page. Fields allowed in the query: groupId, groupName,
             siteId. The siteId field can only be filtered by admins with full
             access. Any sited admin will have siteId filtered automatically.
             This param can be combined with paging and sorting.
 
-            Example: groupName=="staticGroup1"
+            Example: 'groupName=="staticGroup1"'
 
         :returns: All mobile device static groups in JSON
         """
         params = remove_empty_params(
             {"page": page, "page-size": page_size, "sort": sort, "filter": filter}
         )
         endpoint = "/api/v1/mobile-device-groups/static-groups"
@@ -5994,14 +6010,126 @@
                 "sort": sort,
             }
         )
         endpoint = "/api/v2/mobile-devices"
 
         return self._get(endpoint, params=params)
 
+    def get_mobile_devices_detail(
+        self,
+        section: List[str] = None,
+        page: int = None,
+        page_size: int = None,
+        sort: List[str] = ["date:desc"],
+        filter: str = None,
+    ) -> dict:
+        """
+        Returns all sorted and paginated mobile devices with detailed info
+
+        :param section:
+            Section of mobile device details, if not specified, General section
+            data is returned. Multiple section parameters are supported.
+
+            Options:
+            GENERAL, HARDWARE, USER_AND_LOCATION, PURCHASING, SECURITY,
+            APPLICATIONS, EBOOKS, NETWORK, SERVICE_SUBSCRIPTIONS, CERTIFICATES,
+            PROFILES, USER_PROFILES, PROVISIONING_PROFILES, SHARED_USERS,
+            EXTENSION_ATTRIBUTES
+
+            Example: ["GENERAL", "HARDWARE"]
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort is
+            displayName:asc. Multiple sort criteria are supported and must be
+            separated with a comma.
+
+            Options:
+            airPlayPassword, appAnalyticsEnabled, assetTag, availableSpaceMb,
+            batteryLevel, bluetoothLowEnergyCapable, bluetoothMacAddress,
+            capacityMb, lostModeEnabledDate,
+            declarativeDeviceManagementEnabled, deviceId,
+            deviceLocatorServiceEnabled, devicePhoneNumber,
+            diagnosticAndUsageReportingEnabled, displayName,
+            doNotDisturbEnabled, enrollmentSessionTokenValid, exchangeDeviceId,
+            cloudBackupEnabled, osBuild, osSupplementalBuildVersion, osVersion,
+            osRapidSecurityResponse, ipAddress, itunesStoreAccountActive,
+            mobileDeviceId, languages, lastBackupDate, lastEnrolledDate,
+            lastCloudBackupDate, lastInventoryUpdateDate, locales,
+            locationServicesForSelfServiceMobileEnabled, lostModeEnabled,
+            managed, mdmProfileExpirationDate, model, modelIdentifier,
+            modelNumber, modemFirmwareVersion, quotaSize, residentUsers,
+            serialNumber, sharedIpad, supervised, tethered, timeZone, udid,
+            usedSpacePercentage, wifiMacAddress, deviceOwnershipType, building,
+            department, emailAddress, fullName, userPhoneNumber, position,
+            room, username, appleCareId,
+            leaseExpirationDate,lifeExpectancyYears, poDate, poNumber,
+            purchasePrice, purchasedOrLeased, purchasingAccount,
+            purchasingContact, vendor, warrantyExpirationDate,
+            activationLockEnabled, blockEncryptionCapable, dataProtection,
+            fileEncryptionCapable, hardwareEncryptionSupported,
+            jailbreakStatus, passcodeCompliant, passcodeCompliantWithProfile,
+            passcodeLockGracePeriodEnforcedSeconds, passcodePresent,
+            personalDeviceProfileCurrent, carrierSettingsVersion,
+            cellularTechnology, currentCarrierNetwork,
+            currentMobileCountryCode, currentMobileNetworkCode,
+            dataRoamingEnabled, eid, network, homeMobileCountryCode,
+            homeMobileNetworkCode, iccid, imei, imei2, meid,
+            personalHotspotEnabled, voiceRoamingEnabled, roaming
+
+            Example: ["deviceId:desc", "displayName:asc"]
+
+        :param filter:
+            Query in the RSQL format, allowing to filter mobile device
+            collection. Default filter is empty query - returning all results
+            for the requested page.
+
+            Options:
+            airPlayPassword, appAnalyticsEnabled, assetTag, availableSpaceMb,
+            batteryLevel, bluetoothLowEnergyCapable, bluetoothMacAddress,
+            capacityMb, declarativeDeviceManagementEnabled, deviceId,
+            deviceLocatorServiceEnabled, devicePhoneNumber,
+            diagnosticAndUsageReportingEnabled, displayName,
+            doNotDisturbEnabled, exchangeDeviceId, cloudBackupEnabled, osBuild,
+            osSupplementalBuildVersion, osVersion, osRapidSecurityResponse,
+            ipAddress, itunesStoreAccountActive, mobileDeviceId, languages,
+            locales, locationServicesForSelfServiceMobileEnabled,
+            lostModeEnabled, managed, model, modelIdentifier, modelNumber,
+            modemFirmwareVersion, quotaSize, residentUsers, serialNumber,
+            sharedIpad, supervised, tethered, timeZone, udid,
+            usedSpacePercentage, wifiMacAddress, building, department,
+            emailAddress, fullName, userPhoneNumber, position, room, username,
+            appleCareId, lifeExpectancyYears, poNumber, purchasePrice,
+            purchasedOrLeased, purchasingAccount, purchasingContact, vendor,
+            activationLockEnabled, blockEncryptionCapable, dataProtection,
+            fileEncryptionCapable, passcodeCompliant,
+            passcodeCompliantWithProfile,
+            passcodeLockGracePeriodEnforcedSeconds, passcodePresent,
+            personalDeviceProfileCurrent, carrierSettingsVersion,
+            currentCarrierNetwork, currentMobileCountryCode,
+            currentMobileNetworkCode, dataRoamingEnabled, eid, network,
+            homeMobileCountryCode, homeMobileNetworkCode, iccid, imei, imei2,
+            meid, personalHotspotEnabled, roaming
+
+            Example: 'displayName=="iPad" and deviceId==1001'
+        """
+        params = remove_empty_params(
+            {
+                "section": section,
+                "page": page,
+                "page-size": page_size,
+                "sort": sort,
+                "filter": filter,
+            }
+        )
+        endpoint = "/api/v2/mobile-devices/detail"
+
+        return self._get(endpoint, params=params)
+
     def get_mobile_device(self, id: Union[int, str]) -> dict:
         """
         Returns mobile device with limited details by ID
 
         :param id: Mobile device ID
 
         :returns: Mobile device information in JSON
@@ -6594,27 +6722,44 @@
             Definition collection. Default filter is empty query - returning
             all results for the requested page. Fields allowed in the query:
             id, version, minimumOperatingSystem, releaseDate, reboot,
             standalone and absoluteOrderId. This param can be combined with
             paging and sorting.
 
             Example: 'id=="1001"'
+
+        :returns: Patch software title definition in JSON
         """
         params = remove_empty_params(
             {
                 "page": page,
                 "page-size": page_size,
                 "sort": sort,
                 "filter": filter,
             }
         )
         endpoint = f"/api/v2/patch-software-title-configurations/{id}/definitions"
 
         return self._get(endpoint, params=params)
 
+    def get_patch_software_title_configuration_dependencies(
+        self,
+        id: Union[int, str],
+    ) -> dict:
+        """
+        Returns Patch Software Title Configuration Dependencies by ID
+
+        :param id: Patch Software Title Configuration ID
+
+        :returns: Patch software title configuration dependencies in JSON
+        """
+        endpoint = f"/api/v2/patch-software-title-configurations/{id}/dependencies"
+
+        return self._get(endpoint)
+
     def get_patch_software_title_configuration_export(
         self,
         id: Union[int, str],
         columns_to_export: List[str] = ["all"],
         page: int = None,
         page_size: int = None,
         sort: List[str] = ["computerName:asc"],
```

### Comparing `jps_api_wrapper-1.6.0/src/jps_api_wrapper/request_builder.py` & `jps_api_wrapper-1.7.0/src/jps_api_wrapper/request_builder.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/src/jps_api_wrapper/utils.py` & `jps_api_wrapper-1.7.0/src/jps_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/PKG-INFO` & `jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps-api-wrapper
-Version: 1.6.0
+Version: 1.7.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.6.0/tests/test_classic.py` & `jps_api_wrapper-1.7.0/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.6.0/tests/test_pro.py` & `jps_api_wrapper-1.7.0/tests/test_pro.py`

 * *Files 0% similar despite different names*

```diff
@@ -1856,14 +1856,28 @@
     required params
     """
     responses.add(response_builder("DELETE", jps_url("/api/v1/csa/token")))
     assert pro.delete_csa() == "CSA Token Exchange successfully deleted."
 
 
 """
+dashboard
+"""
+
+
+@responses.activate
+def test_get_dashboard(pro):
+    """
+    Ensures that get_dashboard returns JSON when used
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/dashboard")))
+    assert pro.get_dashboard() == EXPECTED_JSON
+
+
+"""
 departments
 """
 
 
 @responses.activate
 def test_get_departments(pro):
     """
@@ -4145,29 +4159,29 @@
     assert pro.get_managed_software_updates_available() == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_managed_software_updates_statuses(pro):
     """
     Ensures that get_managed_software_updates_statuses returns JSON when used
-    without required params
+    without optional params
     """
     responses.add(
         response_builder(
             "GET", jps_url("/api/v1/managed-software-updates/update-statuses")
         )
     )
     assert pro.get_managed_software_updates_statuses() == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_managed_software_updates_statuses_optional_params(pro):
     """
     Ensures that get_managed_software_updates_statuses returns JSON when used
-    with all required params
+    with all optional params
     """
     responses.add(
         response_builder(
             "GET", jps_url("/api/v1/managed-software-updates/update-statuses")
         )
     )
     assert (
@@ -4768,14 +4782,40 @@
     params
     """
     responses.add(response_builder("GET", jps_url("/api/v2/mobile-devices")))
     assert pro.get_mobile_devices() == EXPECTED_JSON
 
 
 @responses.activate
+def test_get_mobile_devices_detail(pro):
+    """
+    Ensures that get_mobile_devices_detail returns JSON when used without
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v2/mobile-devices/detail")))
+    assert pro.get_mobile_devices_detail() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_mobile_devices_detail_optional_params(pro):
+    """
+    Ensures that get_mobile_devices_detail returns JSON when used with all
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v2/mobile-devices/detail")))
+    assert pro.get_mobile_devices_detail(
+        ["GENERAL", "HARDWARE"],
+        0,
+        100,
+        ["deviceId:desc", "displayName:asc"],
+        'displayName=="iPad" and deviceId==1001',
+    )
+
+
+@responses.activate
 def test_get_mobile_devices_optional_params(pro):
     """
     Ensures that get_mobile_device returns JSON when used with all optional
     params
     """
     responses.add(response_builder("GET", jps_url("/api/v2/mobile-devices")))
     assert pro.get_mobile_devices(0, 100, ["id:desc", "name:asc"]) == EXPECTED_JSON
@@ -5214,14 +5254,31 @@
             jps_url("/api/v2/patch-software-title-configurations/1001/definitions"),
         )
     )
     assert pro.get_patch_software_title_configuration_definitions(1001) == EXPECTED_JSON
 
 
 @responses.activate
+def test_get_patch_software_title_configuration_dependencies(pro):
+    """
+    Ensures that get_patch_software_title_configuration_dependencies returns
+    JSON when used
+    """
+    responses.add(
+        response_builder(
+            "GET",
+            jps_url("/api/v2/patch-software-title-configurations/1001/dependencies"),
+        )
+    )
+    assert (
+        pro.get_patch_software_title_configuration_dependencies(1001) == EXPECTED_JSON
+    )
+
+
+@responses.activate
 def test_get_patch_software_title_configuration_definitions_optional_params(pro):
     """
     Ensures that get_patch_software_title_configuration_definitions returns
     JSON when used with all optional params
     """
     responses.add(
         response_builder(
```

