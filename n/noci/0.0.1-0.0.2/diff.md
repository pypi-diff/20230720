# Comparing `tmp/noci-0.0.1.tar.gz` & `tmp/noci-0.0.2.tar.gz`

## Comparing `noci-0.0.1.tar` & `noci-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/noci.iml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 noci-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 noci-0.0.1/docs/build.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/util.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/.gitignore
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/misc.xml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/modules.xml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/noci_ugyys.iml
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/workspace.xml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 noci-0.0.1/src/noci/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 noci-0.0.1/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 noci-0.0.1/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 noci-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 noci-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/noci.iml
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 noci-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 noci-0.0.2/docs/release.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/__init__.py
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/util.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/.gitignore
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/misc.xml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/modules.xml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/noci_ugyys.iml
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/workspace.xml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 noci-0.0.2/src/noci/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 noci-0.0.2/LICENSE
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 noci-0.0.2/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 noci-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 noci-0.0.2/PKG-INFO
```

### Comparing `noci-0.0.1/.idea/workspace.xml` & `noci-0.0.2/src/noci/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `noci-0.0.1/.idea/workspace.xml` & `noci-0.0.2/src/noci/.idea/workspace.xml`

```diff
@@ -1,44 +1,39 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="aa06086a-e41d-4801-bd89-c5ab80800cf4" name="Default Changelist" comment=""/>
+    <list default="true" id="81a0b24f-b1db-4a3d-8ea0-7fdd9d0ea5ef" name="Default Changelist" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
-  <component name="ProjectId" id="2Bk3RoB2I8PJP3uutkCOAP9JvUs"/>
+  <component name="FileTemplateManagerImpl">
+    <option name="RECENT_TEMPLATES">
+      <list>
+        <option value="Python Script"/>
+      </list>
+    </option>
+  </component>
+  <component name="ProjectId" id="2Bk31C6hLGeY9udpq4PxsrCEZtd"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">
     <property name="RunOnceActivity.OpenProjectViewOnStart" value="true"/>
     <property name="RunOnceActivity.ShowReadmeOnStart" value="true"/>
-    <property name="last_opened_file_path" value="$PROJECT_DIR$"/>
-  </component>
-  <component name="RecentsManager">
-    <key name="MoveFile.RECENT_KEYS">
-      <recent name="D:\Code\Framework\noci"/>
-    </key>
   </component>
   <component name="SvnConfiguration">
     <configuration/>
   </component>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
-      <changelist id="aa06086a-e41d-4801-bd89-c5ab80800cf4" name="Default Changelist" comment=""/>
-      <created>1657436249185</created>
+      <changelist id="81a0b24f-b1db-4a3d-8ea0-7fdd9d0ea5ef" name="Default Changelist" comment=""/>
+      <created>1657436038000</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
-      <updated>1657436249185</updated>
+      <updated>1657436038000</updated>
     </task>
     <servers/>
   </component>
-  <component name="WindowStateProjectService">
-    <state x="1297" y="615" key="#com.intellij.fileTypes.FileTypeChooser" timestamp="1657436329637">
-      <screen x="0" y="0" width="1920" height="1040"/>
-    </state>
-    <state x="1297" y="615" key="#com.intellij.fileTypes.FileTypeChooser/0.0.1920.1040@0.0.1920.1040" timestamp="1657436329637"/>
-  </component>
 </project>
```

### Comparing `noci-0.0.1/src/noci/.idea/workspace.xml` & `noci-0.0.2/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `noci-0.0.1/src/noci/.idea/workspace.xml` & `noci-0.0.2/.idea/workspace.xml`

```diff
@@ -1,39 +1,48 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="81a0b24f-b1db-4a3d-8ea0-7fdd9d0ea5ef" name="Default Changelist" comment=""/>
+    <list default="true" id="aa06086a-e41d-4801-bd89-c5ab80800cf4" name="Default Changelist" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
-  <component name="FileTemplateManagerImpl">
-    <option name="RECENT_TEMPLATES">
-      <list>
-        <option value="Python Script"/>
-      </list>
-    </option>
-  </component>
-  <component name="ProjectId" id="2Bk31C6hLGeY9udpq4PxsrCEZtd"/>
+  <component name="ProjectId" id="2Bk3RoB2I8PJP3uutkCOAP9JvUs"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">
     <property name="RunOnceActivity.OpenProjectViewOnStart" value="true"/>
     <property name="RunOnceActivity.ShowReadmeOnStart" value="true"/>
+    <property name="last_opened_file_path" value="$PROJECT_DIR$"/>
+  </component>
+  <component name="RecentsManager">
+    <key name="MoveFile.RECENT_KEYS">
+      <recent name="D:\Code\Framework\noci"/>
+    </key>
   </component>
   <component name="SvnConfiguration">
     <configuration/>
   </component>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
-      <changelist id="81a0b24f-b1db-4a3d-8ea0-7fdd9d0ea5ef" name="Default Changelist" comment=""/>
-      <created>1657436038000</created>
+      <changelist id="aa06086a-e41d-4801-bd89-c5ab80800cf4" name="Default Changelist" comment=""/>
+      <created>1657436249185</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
-      <updated>1657436038000</updated>
+      <updated>1657436249185</updated>
     </task>
     <servers/>
   </component>
+  <component name="WindowStateProjectService">
+    <state x="1297" y="615" key="#com.intellij.fileTypes.FileTypeChooser" timestamp="1657436329637">
+      <screen x="0" y="0" width="1920" height="1040"/>
+    </state>
+    <state x="1297" y="615" key="#com.intellij.fileTypes.FileTypeChooser/0.0.1920.1040@0.0.1920.1040" timestamp="1657436329637"/>
+    <state x="623" y="225" width="672" height="678" key="search.everywhere.popup" timestamp="1657442594318">
+      <screen x="0" y="0" width="1920" height="1040"/>
+    </state>
+    <state x="623" y="225" width="672" height="678" key="search.everywhere.popup/0.0.1920.1040@0.0.1920.1040" timestamp="1657442594318"/>
+  </component>
 </project>
```

### Comparing `noci-0.0.1/LICENSE` & `noci-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noci-0.0.1/pyproject.toml` & `noci-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noci"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="ugyys", email="unigauldoth@gmail.com" },
 ]
-description = "noci is a utility package for ci tasks"
+description = "noci is a utility package for automation tasks"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=2.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 2.7",
     "License :: OSI Approved :: MIT License",
```

### Comparing `noci-0.0.1/PKG-INFO` & `noci-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: noci
-Version: 0.0.1
-Summary: noci is a utility package for ci tasks
+Version: 0.0.2
+Summary: noci is a utility package for automation tasks
 Author-email: ugyys <unigauldoth@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 unigauldoth@gmail.com
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,18 +20,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 
 # noci
 
 ## Concept
-noci is a utility package for ci tasks
+noci is a utility package for automation tasks
+
+## Packaging
+1. install twine
+
+    python3 -m pip install --upgrade twine
+
+2. upload
+
+    python3 -m twine upload --repository noci dist/*
```

