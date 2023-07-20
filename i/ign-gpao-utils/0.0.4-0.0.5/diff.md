# Comparing `tmp/ign-gpao-utils-0.0.4.tar.gz` & `tmp/ign-gpao-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-utils-0.0.4.tar", last modified: Fri Jul  7 13:50:19 2023, max compression
+gzip compressed data, was "ign-gpao-utils-0.0.5.tar", last modified: Thu Jul 20 08:22:04 2023, max compression
```

## Comparing `ign-gpao-utils-0.0.4.tar` & `ign-gpao-utils-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/gpao_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/gpao_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/gpao_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/gpao_utils/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/gpao_utils/utils_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/ign_gpao_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-07 13:50:19.000000 ign-gpao-utils-0.0.4/ign_gpao_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 13:50:19.000000 ign-gpao-utils-0.0.4/ign_gpao_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:50:19.000000 ign-gpao-utils-0.0.4/ign_gpao_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 13:50:19.000000 ign-gpao-utils-0.0.4/ign_gpao_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:50:19.031216 ign-gpao-utils-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 13:50:11.000000 ign-gpao-utils-0.0.4/test/test_utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/gpao_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/test/test_utils_store.py
```

### Comparing `ign-gpao-utils-0.0.4/gpao_utils/utils_store.py` & `ign-gpao-utils-0.0.5/gpao_utils/utils_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         return res
 
     def to_win(self, dir: str):
         res = dir.replace(self._unix_path, self._win_path)
         # res = res.replace("/", "\\")
         return res
 
-@staticmethod    
 def frame_store(i: int, L: list):
     if len(L)!=i :
         raise RuntimeError(f"Not the same number of store in parameters. Number : {i}, List : {L}")
     layout_store = []
     for j in range(i):
         layout_store.append([   sg.Text(f" {j} - Lettre (sur ma machine Windows)", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN-LETTER", "L:"), key=f"-MAP-STORE{j}-WIN-LETTER", size=(iu.size_text_big,{j})) ])
         layout_store.append([   sg.Text(f" {j} - store Windows ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN", f"//store.ign.fr/{L[j]}"), key=f"-MAP-STORE{j}-WIN", size=(iu.size_text_big, 1))])
```

### Comparing `ign-gpao-utils-0.0.4/setup.py` & `ign-gpao-utils-0.0.5/setup.py`

 * *Files identical despite different names*

