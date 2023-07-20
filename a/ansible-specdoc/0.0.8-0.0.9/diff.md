# Comparing `tmp/ansible-specdoc-0.0.8.tar.gz` & `tmp/ansible-specdoc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-specdoc-0.0.8.tar", last modified: Mon May 23 18:52:59 2022, max compression
+gzip compressed data, was "ansible-specdoc-0.0.9.tar", last modified: Tue Jun 21 15:13:20 2022, max compression
```

## Comparing `ansible-specdoc-0.0.8.tar` & `ansible-specdoc-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-05-23 18:52:59.996520 ansible-specdoc-0.0.8/
--rw-r--r--   0 lgarber    (501) staff       (20)      336 2022-05-23 18:52:59.996096 ansible-specdoc-0.0.8/PKG-INFO
--rw-r--r--   0 lgarber    (501) staff       (20)     1127 2022-05-20 14:59:23.000000 ansible-specdoc-0.0.8/README.md
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-05-23 18:52:59.988031 ansible-specdoc-0.0.8/ansible_specdoc/
--rw-r--r--   0 lgarber    (501) staff       (20)       38 2022-05-20 14:59:23.000000 ansible-specdoc-0.0.8/ansible_specdoc/__init__.py
--rw-r--r--   0 lgarber    (501) staff       (20)    10444 2022-05-23 14:58:22.000000 ansible-specdoc-0.0.8/ansible_specdoc/cli.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-05-23 18:52:59.994854 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/
--rw-r--r--   0 lgarber    (501) staff       (20)      336 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/PKG-INFO
--rw-r--r--   0 lgarber    (501) staff       (20)      305 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/SOURCES.txt
--rw-r--r--   0 lgarber    (501) staff       (20)        1 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/dependency_links.txt
--rw-r--r--   0 lgarber    (501) staff       (20)      129 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/entry_points.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       44 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/requires.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       16 2022-05-23 18:52:59.000000 ansible-specdoc-0.0.8/ansible_specdoc.egg-info/top_level.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       38 2022-05-23 18:52:59.996768 ansible-specdoc-0.0.8/setup.cfg
--rw-r--r--   0 lgarber    (501) staff       (20)      776 2022-05-23 18:52:14.000000 ansible-specdoc-0.0.8/setup.py
+drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-06-21 15:13:20.955551 ansible-specdoc-0.0.9/
+-rw-r--r--   0 lgarber    (501) staff       (20)      336 2022-06-21 15:13:20.954803 ansible-specdoc-0.0.9/PKG-INFO
+-rw-r--r--   0 lgarber    (501) staff       (20)     1127 2022-05-20 14:59:23.000000 ansible-specdoc-0.0.9/README.md
+drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-06-21 15:13:20.949663 ansible-specdoc-0.0.9/ansible_specdoc/
+-rw-r--r--   0 lgarber    (501) staff       (20)       38 2022-05-20 14:59:23.000000 ansible-specdoc-0.0.9/ansible_specdoc/__init__.py
+-rw-r--r--   0 lgarber    (501) staff       (20)    10579 2022-06-21 15:06:48.000000 ansible-specdoc-0.0.9/ansible_specdoc/cli.py
+drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-06-21 15:13:20.954005 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/
+-rw-r--r--   0 lgarber    (501) staff       (20)      336 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/PKG-INFO
+-rw-r--r--   0 lgarber    (501) staff       (20)      305 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/SOURCES.txt
+-rw-r--r--   0 lgarber    (501) staff       (20)        1 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/dependency_links.txt
+-rw-r--r--   0 lgarber    (501) staff       (20)      129 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/entry_points.txt
+-rw-r--r--   0 lgarber    (501) staff       (20)       44 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/requires.txt
+-rw-r--r--   0 lgarber    (501) staff       (20)       16 2022-06-21 15:13:20.000000 ansible-specdoc-0.0.9/ansible_specdoc.egg-info/top_level.txt
+-rw-r--r--   0 lgarber    (501) staff       (20)       38 2022-06-21 15:13:20.955849 ansible-specdoc-0.0.9/setup.cfg
+-rw-r--r--   0 lgarber    (501) staff       (20)      776 2022-06-21 15:12:16.000000 ansible-specdoc-0.0.9/setup.py
```

### Comparing `ansible-specdoc-0.0.8/README.md` & `ansible-specdoc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ansible-specdoc-0.0.8/ansible_specdoc/cli.py` & `ansible-specdoc-0.0.9/ansible_specdoc/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,17 @@
 
             if 'elements' in param:
                 param_dict['elements'] = param.get('elements')
 
             if 'options' in param:
                 param_dict['suboptions'] = SpecDocModule.__spec_to_doc(param.get('options'))
 
+            if 'suboptions' in param:
+                param_dict['suboptions'] = SpecDocModule.__spec_to_doc(param.get('suboptions'))
+
             result[key] = param_dict
 
         return result
 
     def __generate_doc_dict(self) -> Dict[str, Any]:
         desc = self._metadata.get('description')
```

### Comparing `ansible-specdoc-0.0.8/setup.py` & `ansible-specdoc-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import setuptools
 
 setuptools.setup(
     name="ansible-specdoc",
-    version="0.0.8",
+    version="0.0.9",
     author="Lena Garber",
     author_email="lbgarber2@gmail.com",
     description=("A simple tool for generating Ansible collection documentation from module spec."),
     license="GNU General Public License v3.0",
     keywords="ansible",
     url="http://packages.python.org/ansible-specdoc",
     packages=['ansible_specdoc'],
```

