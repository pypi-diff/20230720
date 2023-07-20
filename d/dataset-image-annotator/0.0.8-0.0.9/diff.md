# Comparing `tmp/dataset-image-annotator-0.0.8.tar.gz` & `tmp/dataset-image-annotator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-image-annotator-0.0.8.tar", last modified: Sat Oct  8 19:01:32 2022, max compression
+gzip compressed data, was "dataset-image-annotator-0.0.9.tar", last modified: Sun Oct 30 21:02:07 2022, max compression
```

## Comparing `dataset-image-annotator-0.0.8.tar` & `dataset-image-annotator-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.824663 dataset-image-annotator-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.828663 dataset-image-annotator-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    34575 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.828663 dataset-image-annotator-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.828663 dataset-image-annotator-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9413 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.824663 dataset-image-annotator-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/src/dataset_image_annotator/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator/main_window.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-08 19:01:32.000000 dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 19:01:32.832663 dataset-image-annotator-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-08 19:01:20.000000 dataset-image-annotator-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.726838 dataset-image-annotator-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)    34575 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9413 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-10-30 21:02:07.734838 dataset-image-annotator-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/src/dataset_image_annotator/
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5288 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator/main_window.ui
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-30 21:02:07.000000 dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:02:07.730838 dataset-image-annotator-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-30 21:01:57.000000 dataset-image-annotator-0.0.9/tests/conftest.py
```

### Comparing `dataset-image-annotator-0.0.8/.coveragerc` & `dataset-image-annotator-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/.github/workflows/python-publish.yml` & `dataset-image-annotator-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/.gitignore` & `dataset-image-annotator-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/Dockerfile` & `dataset-image-annotator-0.0.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/LICENSE` & `dataset-image-annotator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/PKG-INFO` & `dataset-image-annotator-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-image-annotator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Image annotation tool
 Home-page: https://github.com/kamikaze/dataset-image-annotator
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/dataset-image-annotator/wiki
 Platform: any
```

### Comparing `dataset-image-annotator-0.0.8/docs/Makefile` & `dataset-image-annotator-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/docs/conf.py` & `dataset-image-annotator-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/docs/index.rst` & `dataset-image-annotator-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/requirements.txt` & `dataset-image-annotator-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/setup.cfg` & `dataset-image-annotator-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `dataset-image-annotator-0.0.8/src/dataset_image_annotator/main_window.ui` & `dataset-image-annotator-0.0.9/src/dataset_image_annotator/main_window.ui`

 * *Files 12% similar despite different names*

#### Comparing `dataset-image-annotator-0.0.8/src/dataset_image_annotator/main_window.ui` & `dataset-image-annotator-0.0.9/src/dataset_image_annotator/main_window.ui`

```diff
@@ -2,18 +2,24 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>800</width>
-        <height>600</height>
+        <width>906</width>
+        <height>769</height>
       </rect>
     </property>
+    <property name="sizePolicy">
+      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+        <horstretch>0</horstretch>
+        <verstretch>0</verstretch>
+      </sizepolicy>
+    </property>
     <property name="windowTitle">
       <string>Annotator</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <property name="sizePolicy">
         <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
           <horstretch>0</horstretch>
@@ -141,15 +147,57 @@
                   <bool>true</bool>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
         <item>
-          <widget class="QGraphicsView" name="photo_view"/>
+          <layout class="QHBoxLayout" name="horizontalLayout">
+            <item>
+              <widget class="QGraphicsView" name="photo_view">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="MinimumExpanding" vsizetype="MinimumExpanding">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
+                  </sizepolicy>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QListView" name="thumbnail_list_view">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="Fixed" vsizetype="Expanding">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
+                  </sizepolicy>
+                </property>
+                <property name="minimumSize">
+                  <size>
+                    <width>110</width>
+                    <height>0</height>
+                  </size>
+                </property>
+                <property name="maximumSize">
+                  <size>
+                    <width>110</width>
+                    <height>16777215</height>
+                  </size>
+                </property>
+                <property name="iconSize">
+                  <size>
+                    <width>80</width>
+                    <height>80</height>
+                  </size>
+                </property>
+                <property name="itemAlignment">
+                  <set>Qt::AlignCenter</set>
+                </property>
+              </widget>
+            </item>
+          </layout>
         </item>
         <item>
           <layout class="QHBoxLayout" name="pathHLayout">
             <item>
               <widget class="QLabel" name="path_label">
                 <property name="text">
                   <string>Path:</string>
@@ -167,45 +215,22 @@
                 <property name="text">
                   <string>...</string>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
-        <item>
-          <widget class="QScrollArea" name="thumbnail_scroll_area">
-            <property name="verticalScrollBarPolicy">
-              <enum>Qt::ScrollBarAlwaysOn</enum>
-            </property>
-            <property name="horizontalScrollBarPolicy">
-              <enum>Qt::ScrollBarAlwaysOn</enum>
-            </property>
-            <property name="widgetResizable">
-              <bool>true</bool>
-            </property>
-            <widget class="QWidget" name="scrollAreaWidgetContents">
-              <property name="geometry">
-                <rect>
-                  <x>0</x>
-                  <y>0</y>
-                  <width>766</width>
-                  <height>133</height>
-                </rect>
-              </property>
-            </widget>
-          </widget>
-        </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>800</width>
+          <width>906</width>
           <height>21</height>
         </rect>
       </property>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
   </widget>
   <resources/>
```

### Comparing `dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/PKG-INFO` & `dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-image-annotator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Image annotation tool
 Home-page: https://github.com/kamikaze/dataset-image-annotator
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/dataset-image-annotator/wiki
 Platform: any
```

### Comparing `dataset-image-annotator-0.0.8/src/dataset_image_annotator.egg-info/SOURCES.txt` & `dataset-image-annotator-0.0.9/src/dataset_image_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

