# Comparing `tmp/mdrpaLibrary-2.5.tar.gz` & `tmp/mdrpaLibrary-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrpaLibrary-2.5.tar", last modified: Tue Jul 11 11:19:44 2023, max compression
+gzip compressed data, was "mdrpaLibrary-2.6.tar", last modified: Thu Jul 20 13:14:17 2023, max compression
```

## Comparing `mdrpaLibrary-2.5.tar` & `mdrpaLibrary-2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 11:19:44.580352 mdrpaLibrary-2.5/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 11:19:44.580181 mdrpaLibrary-2.5/PKG-INFO
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 11:19:44.578841 mdrpaLibrary-2.5/mdrpaLibrary/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.5/mdrpaLibrary/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3325 2023-07-06 11:19:01.000000 mdrpaLibrary-2.5/mdrpaLibrary/clickButtonModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      529 2023-07-11 08:54:27.000000 mdrpaLibrary-2.5/mdrpaLibrary/getUiModels.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3352 2023-07-06 11:19:23.000000 mdrpaLibrary-2.5/mdrpaLibrary/inputFieldModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2005 2023-07-11 09:31:53.000000 mdrpaLibrary-2.5/mdrpaLibrary/modelDrivenRpa.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3366 2023-07-06 11:20:06.000000 mdrpaLibrary-2.5/mdrpaLibrary/selectCheckboxModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3425 2023-07-06 11:20:26.000000 mdrpaLibrary-2.5/mdrpaLibrary/selectFromDropdownModel.robot
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      743 2023-07-11 11:19:06.000000 mdrpaLibrary-2.5/mdrpaLibrary/sendReportModel.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 11:19:44.579826 mdrpaLibrary-2.5/mdrpaLibrary/utils/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.5/mdrpaLibrary/utils/__init__.py
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2350 2023-07-11 08:04:53.000000 mdrpaLibrary-2.5/mdrpaLibrary/utils/utils.robot
-drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-11 11:19:44.579520 mdrpaLibrary-2.5/mdrpaLibrary.egg-info/
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-11 11:19:44.000000 mdrpaLibrary-2.5/mdrpaLibrary.egg-info/PKG-INFO
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-11 11:19:44.000000 mdrpaLibrary-2.5/mdrpaLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-11 11:19:44.000000 mdrpaLibrary-2.5/mdrpaLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-11 11:19:44.000000 mdrpaLibrary-2.5/mdrpaLibrary.egg-info/top_level.txt
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-11 11:19:44.580430 mdrpaLibrary-2.5/setup.cfg
--rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-11 11:19:30.000000 mdrpaLibrary-2.5/setup.py
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-20 13:14:17.005044 mdrpaLibrary-2.6/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-20 13:14:17.004886 mdrpaLibrary-2.6/PKG-INFO
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-20 13:14:17.003423 mdrpaLibrary-2.6/mdrpaLibrary/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-06 11:24:56.000000 mdrpaLibrary-2.6/mdrpaLibrary/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3328 2023-07-20 13:13:18.000000 mdrpaLibrary-2.6/mdrpaLibrary/clickButtonModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      529 2023-07-11 08:54:27.000000 mdrpaLibrary-2.6/mdrpaLibrary/getUiModels.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3353 2023-07-20 13:12:15.000000 mdrpaLibrary-2.6/mdrpaLibrary/inputFieldModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2005 2023-07-11 09:31:53.000000 mdrpaLibrary-2.6/mdrpaLibrary/modelDrivenRpa.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3369 2023-07-20 13:13:00.000000 mdrpaLibrary-2.6/mdrpaLibrary/selectCheckboxModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     3429 2023-07-20 13:12:43.000000 mdrpaLibrary-2.6/mdrpaLibrary/selectFromDropdownModel.robot
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      743 2023-07-11 11:19:06.000000 mdrpaLibrary-2.6/mdrpaLibrary/sendReportModel.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-20 13:14:17.004522 mdrpaLibrary-2.6/mdrpaLibrary/utils/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        0 2023-07-05 13:00:07.000000 mdrpaLibrary-2.6/mdrpaLibrary/utils/__init__.py
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)     2350 2023-07-11 08:04:53.000000 mdrpaLibrary-2.6/mdrpaLibrary/utils/utils.robot
+drwxr-xr-x   0 alihussainkazmi   (501) staff       (20)        0 2023-07-20 13:14:17.004285 mdrpaLibrary-2.6/mdrpaLibrary.egg-info/
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       54 2023-07-20 13:14:16.000000 mdrpaLibrary-2.6/mdrpaLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      489 2023-07-20 13:14:16.000000 mdrpaLibrary-2.6/mdrpaLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)        1 2023-07-20 13:14:16.000000 mdrpaLibrary-2.6/mdrpaLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       13 2023-07-20 13:14:16.000000 mdrpaLibrary-2.6/mdrpaLibrary.egg-info/top_level.txt
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)       38 2023-07-20 13:14:17.005090 mdrpaLibrary-2.6/setup.cfg
+-rw-r--r--   0 alihussainkazmi   (501) staff       (20)      193 2023-07-20 13:13:39.000000 mdrpaLibrary-2.6/setup.py
```

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/clickButtonModel.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/clickButtonModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
 
     
     ${removed_keyword}=    Run Keyword If    '${current_mode}' == 'id'    Remove From List    ${keyword_list}    0
 ...    ELSE IF    '${current_mode}' == 'path'    Remove From List    ${keyword_list}    1
-...    ELSE IF    '${current_mode}' == 'label'    Remove From List    ${keyword_list}    2
+...    ELSE IF    '${current_mode}' == 'text'    Remove From List    ${keyword_list}    2
 
 
 
     Set Suite Variable  ${interaction_status}   ${EMPTY} 
 
     Run Keyword    ${removed_keyword}    
 
@@ -59,16 +59,16 @@
 
 Click Button By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element    xpath=${path}
     ...  ELSE  Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  path
 
 Click Button By Label
-    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
-    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element   xpath=//a[text()='${text}']
+    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//*[text()='${text}']  
+    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND  Click Element   xpath=//*[text()='${text}']  
     ...  ELSE    Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  text
 
 
 
 # The below keywords are to get a specific UI Element from the model
```

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/getUiModels.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/getUiModels.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/inputFieldModel.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/inputFieldModel.robot`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
 
 
     
     ${removed_keyword}=    Run Keyword If    '${current_mode}' == 'id'    Remove From List    ${keyword_list}    0
 ...    ELSE IF    '${current_mode}' == 'path'    Remove From List    ${keyword_list}    1
-...    ELSE IF    '${current_mode}' == 'label'    Remove From List    ${keyword_list}    2
+...    ELSE IF    '${current_mode}' == 'text'    Remove From List    ${keyword_list}    2
 
 
     Set Suite Variable  ${interaction_status}   ${EMPTY} 
 
     Run Keyword    ${removed_keyword}    
 
     FOR    ${keyword}    IN    @{keyword_list}
@@ -56,16 +56,16 @@
 
 Input Field By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Input Text  xpath=${path}    ${value}      
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  path
 
 Input Field By Label
-    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
-    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Input Text   xpath=//a[text()='${text}']  ${value} 
+    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//*[text()='${text}']  
+    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Input Text   xpath=//*[text()='${text}']  ${value} 
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}  text
```

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/modelDrivenRpa.py` & `mdrpaLibrary-2.6/mdrpaLibrary/modelDrivenRpa.py`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/selectCheckboxModel.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/selectCheckboxModel.robot`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
     
     ${removed_keyword}=    Run Keyword If    '${current_mode}' == 'id'    Remove From List    ${keyword_list}    0
 ...    ELSE IF    '${current_mode}' == 'path'    Remove From List    ${keyword_list}    1
-...    ELSE IF    '${current_mode}' == 'label'    Remove From List    ${keyword_list}    2
+...    ELSE IF    '${current_mode}' == 'text'    Remove From List    ${keyword_list}    2
 
 
     Set Suite Variable  ${interaction_status}   ${EMPTY} 
 
     Run Keyword    ${removed_keyword}    
 
     FOR    ${keyword}    IN    @{keyword_list}
@@ -58,16 +58,16 @@
 
 Select Checkbox By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select Checkbox  xpath=${path}       
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   path
 
 Select Checkbox By Label
-    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
-    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select Checkbox   xpath=//a[text()='${text}']  
+    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//*[text()='${text}']  
+    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select Checkbox   xpath=//*[text()='${text}']    
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   text
```

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/selectFromDropdownModel.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/selectFromDropdownModel.robot`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Set Suite Variable  ${path}   ${element_locators["dom"]["path"]}
     Set Suite Variable  ${text}   ${element_locators["dom"]["text"]}
     Set Suite Variable  ${image}  ${element_locators["surface"]["image"]}
     Set Suite Variable  ${value}
     
     ${removed_keyword}=    Run Keyword If    '${current_mode}' == 'id'    Remove From List    ${keyword_list}    0
 ...    ELSE IF    '${current_mode}' == 'path'    Remove From List    ${keyword_list}    1
-...    ELSE IF    '${current_mode}' == 'label'    Remove From List    ${keyword_list}   2 
+...    ELSE IF    '${current_mode}' == 'text'    Remove From List    ${keyword_list}   2 
 
 
     Set Suite Variable  ${interaction_status}   ${EMPTY} 
 
     Run Keyword    ${removed_keyword}    
 
     FOR    ${keyword}    IN    @{keyword_list}
@@ -57,16 +57,16 @@
 
 Select Value By Path
     ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=${path}
     Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select From List by Value  xpath=${path}    ${value}      
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   path
 
 Select Value By Label
-    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//a[text()='${text}']
-    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select From List by Value   xpath=//a[text()='${text}']  ${value} 
+    ${element_exists}    Run Keyword And Return Status    Element Should Be Visible    xpath=//*[text()='${text}']    
+    Run Keyword If    '${element_exists}' == 'True'  Run Keywords    Set Suite Variable    ${interaction_status}  Pass  AND   Select From List by Value  xpath=//*[text()='${text}']    ${value} 
     ...  ELSE   Run Keywords   Set Suite Variable    ${interaction_status}  Fail  AND  Create Error  ${model_name}  ${page_name}  ${element_name}   text
```

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/sendReportModel.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/sendReportModel.robot`

 * *Files identical despite different names*

### Comparing `mdrpaLibrary-2.5/mdrpaLibrary/utils/utils.robot` & `mdrpaLibrary-2.6/mdrpaLibrary/utils/utils.robot`

 * *Files identical despite different names*

