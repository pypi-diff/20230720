# Comparing `tmp/mend_sca_cleanup_tool-23.6.2-py3-none-any.whl.zip` & `tmp/mend_sca_cleanup_tool-23.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14810 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    22109 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     9287 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      847 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool-23.6.2.dist-info/RECORD
-9 files, 43901 bytes uncompressed, 13312 bytes compressed:  69.7%
+Zip file size: 14841 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    22383 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9291 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      847 b- defN 23-Jul-20 19:22 mend_sca_cleanup_tool-23.7.1.dist-info/RECORD
+9 files, 44179 bytes uncompressed, 13343 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/LICENSE
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/METADATA
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/METADATA
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/WHEEL
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/entry_points.txt
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/top_level.txt
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.2.dist-info/RECORD
+Filename: mend_sca_cleanup_tool-23.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.2"
+__version__ = "23.7.1"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -10,18 +10,20 @@
 from configparser import ConfigParser
 from mend_sca_cleanup_tool._version import __description__, __tool_name__, __version__
 
 
 ATTRIBUTION = "attribution"
 FILTER_PROJECTS_BY_UPDATE_TIME = "FilterProjectsByUpdateTime"
 FILTER_PROJECTS_BY_LAST_CREATED_COPIES = "FilterProjectsByLastCreatedCopies"
+AGENT_INFO = {
+    'agent': f"ps-{__tool_name__}".replace('_', '-'),
+    'agentVersion': __version__
+}
 HEADERS = {
     'Content-Type': 'application/json',
-    'agent': f"ps-{__tool_name__}".replace('_', '-'),
-    'agentVersion': __version__,
     'ctxId': uuid.uuid1().__str__()
 }
 IGNORED_ALERTS = "ignored_alerts"
 RESOLVED_ALERTS = "resolved_alerts"
 REJECTED_BY_POLICY = "alerts_rejected_by_policy"
 REPORTS = {
            "bugs": "getProjectBugsReport",
@@ -45,15 +47,15 @@
     global MAIN_API_CONNECTION
     if len(sys.argv) == 1:
         CONFIG = parse_config_file("params.config")
     elif not sys.argv[1].startswith('-'):
         CONFIG = parse_config_file(sys.argv[1])
     else:
         CONFIG = parse_args()
-    
+        
     setup_config()
 
     MAIN_API_CONNECTION = http.client.HTTPSConnection(CONFIG.mend_url)
 
     if CONFIG.dry_run:
         print("Dry Run enabled - no reports or deletions will occur")
 
@@ -107,15 +109,16 @@
 
 def delete_scan(product_token, project):
     print(f"Deleting project: {project['name']}")
     request = json.dumps({
                 "requestType": "deleteProject",
                 "userKey": CONFIG.mend_user_key,
                 "productToken": product_token,
-                "projectToken": project['token']
+                "projectToken": project['token'],
+                "agentInfo": AGENT_INFO
             })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         return
 
 def filter_projects_by_config(projects):
     projects_to_return = [project for project in projects if project['token'] not in CONFIG.excluded_project_tokens]
@@ -205,48 +208,52 @@
 
 def get_alerts_report(request_type, project_token, alertType):
     request = json.dumps({
         "requestType": request_type,
         "userKey": CONFIG.mend_user_key,
         "projectToken": project_token,
         "status": alertType,
-        "format": "xlsx"
+        "format": "xlsx",
+        "agentInfo": AGENT_INFO
     })
     return post_api_request(request)
 
 def get_alerts_by_type(request_type, project_token, alertType):
     request = json.dumps({
         "requestType": request_type,
         "userKey": CONFIG.mend_user_key,
         "projectToken": project_token,
-        "alertType": alertType
+        "alertType": alertType,
+        "agentInfo": AGENT_INFO
     })
     return post_api_request(request)
 
 def get_attribution_report(project_token):
     request = json.dumps({
         "requestType": REPORTS[ATTRIBUTION],
         "userKey": CONFIG.mend_user_key,
         "projectToken": project_token,
         "reportingAggregationMode": "BY_PROJECT",
-        "exportFormat": "html"
+        "exportFormat": "html",
+        "agentInfo": AGENT_INFO
     })
     return post_api_request(request)
 
 def get_config_file_value(config_val, default):
         if isinstance(config_val, int):
             return config_val if config_val is not None else default
         return config_val if config_val else default
 
 def get_excel_report(request_type, project_token):
     request = json.dumps({
         "requestType": request_type,
         "userKey": CONFIG.mend_user_key,
         "projectToken": project_token,
-        "format": "xlsx"
+        "format": "xlsx",
+        "agentInfo": AGENT_INFO
     })
     return post_api_request(request)
 
 def get_reports_to_generate():
     if len(CONFIG.report_types) == 0:
         return REPORTS
     else:
@@ -260,42 +267,45 @@
 
 
 def get_products():
     request = json.dumps({
         "requestType": "getAllProducts",
         "userKey": CONFIG.mend_user_key,
         "orgToken": CONFIG.mend_api_token,
+        "agentInfo": AGENT_INFO
     })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         exit()
     if len(CONFIG.included_product_tokens) == 0:
         return [product for product in response_obj['products'] if product['productToken'] not in CONFIG.excluded_product_tokens]
     else:
         return [product for product in response_obj['products'] if product['productToken'] in CONFIG.included_product_tokens and product['productToken'] not in CONFIG.excluded_product_tokens]
 
 def get_projects(product_token):
     request = json.dumps({
         "requestType": "getProductProjectVitals",
         "userKey": CONFIG.mend_user_key,
         "productToken": product_token,
+        "agentInfo": AGENT_INFO
     })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         exit()
     else:
         return [vital_Response for vital_Response in response_obj['projectVitals']]
 
 def get_project_tags(project):
     print(f"Getting tags for project {project['name']}")
     request = json.dumps({
-            "requestType": "getProjectTags",
-            "userKey": CONFIG.mend_user_key,
-            "projectToken": project['token'],
-        })
+        "requestType": "getProjectTags",
+        "userKey": CONFIG.mend_user_key,
+        "projectToken": project['token'],
+        "agentInfo": AGENT_INFO
+    })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         exit()
     return [project_tags['tags'] for project_tags in response_obj['projectTags']][0]
 
 def get_projects_to_remove():
     projects_to_remove = {}
@@ -417,8 +427,8 @@
     CONFIG.report_types = CONFIG.report_types if CONFIG.report_types else []
 
     if CONFIG.excluded_project_name_patterns:
         CONFIG.project_name_exclude_list = CONFIG.excluded_project_name_patterns
    
 
 if __name__ == "__main__":
-    main()
+    main()
```

## Comparing `mend_sca_cleanup_tool-23.6.2.dist-info/LICENSE` & `mend_sca_cleanup_tool-23.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_sca_cleanup_tool-23.6.2.dist-info/METADATA` & `mend_sca_cleanup_tool-23.7.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-sca-cleanup-tool
-Version: 23.6.2
+Version: 23.7.1
 Summary: Mend SCA Cleanup Tool
 Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
 Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -20,15 +20,15 @@
 
 [![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Mend projects cleanup](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml)
 [![Python 3.6](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Blue_Python_3.6%2B_Shield_Badge.svg/86px-Blue_Python_3.6%2B_Shield_Badge.svg.png)](https://www.python.org/downloads/release/python-360/)
 [![PyPI](https://img.shields.io/pypi/v/ws-cleanup-tool?style=plastic)](https://pypi.org/project/ws-cleanup-tool/)
 
-# Mend Projects Cleanup CLI Tool
+# Mend SCA Projects Cleanup CLI Tool
 * Current version v23.6.2
 * The self-hosted CLI tool features cleaning up projects and generating reports before deletion in 2 modes:
   * By stating _OperationMode=FilterProjectsByUpdateTime_ and how many days to keep (-r/ DaysToKeep=)
   * By stating _OperationMode=FilterProjectsByLastCreatedCopies_ and how many copies to keep (-r/ DaysToKeep=)
 * The reports are saved in the designated location as follows: _[Output_DIR]/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_  
   * The default location is the _[WORKING DIRECTORY]/Mend/Reports/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_
 * To review the outcome before actual deletion use _-y true_ / _DryRun=True_ flag. It will _NOT_ delete any project nor create reports
```

## Comparing `mend_sca_cleanup_tool-23.6.2.dist-info/RECORD` & `mend_sca_cleanup_tool-23.7.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mend_sca_cleanup_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_sca_cleanup_tool/_version.py,sha256=rEkk0BvfhbNofDLX6yUPXP5RvnCopTdO1oDh2vyn24c,100
-mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=55CjCPXrZedcMNXIBPnFq_JZX2N6WFjZbmRDnni8RKI,22109
-mend_sca_cleanup_tool-23.6.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_sca_cleanup_tool-23.6.2.dist-info/METADATA,sha256=_6xMMW1uonU6WSp4iatnIODvaybCQbMtIBVQbtSBfK8,9287
-mend_sca_cleanup_tool-23.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_sca_cleanup_tool-23.6.2.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
-mend_sca_cleanup_tool-23.6.2.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
-mend_sca_cleanup_tool-23.6.2.dist-info/RECORD,,
+mend_sca_cleanup_tool/_version.py,sha256=53HnZZFa4QUZD67Gh3ZP13vLkNtn0OWtDLO4jsiutbI,100
+mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=QkRFuc77NzwKBsqC6g_W3cNvJY-DHuHIdUupPviK7GM,22383
+mend_sca_cleanup_tool-23.7.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_sca_cleanup_tool-23.7.1.dist-info/METADATA,sha256=OYDCJ6I00W1omQd4I3Iyag1D8_ayQ9pMbiVvufEmSqc,9291
+mend_sca_cleanup_tool-23.7.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_sca_cleanup_tool-23.7.1.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
+mend_sca_cleanup_tool-23.7.1.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
+mend_sca_cleanup_tool-23.7.1.dist-info/RECORD,,
```

