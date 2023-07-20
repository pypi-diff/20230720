# Comparing `tmp/kevlar-system-inspector-1.1.0a2.tar.gz` & `tmp/kevlar-system-inspector-1.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-0cbdsw9x/kevlar-system-inspector-1.1.0a2.tar", last modified: Thu Jul 13 14:56:21 2023, max compression
+gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-i3le9ppg/kevlar-system-inspector-1.1.0a3.tar", last modified: Wed Jul 19 19:45:56 2023, max compression
```

## Comparing `kevlar-system-inspector-1.1.0a2.tar` & `kevlar-system-inspector-1.1.0a3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5089 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4058 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/scripts/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/scripts/kevlar-system-inspector
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/
--rw-rw-rw-   0 root         (0) root         (0)     6025 2023-07-12 20:42:05.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16780 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/console.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-13 18:38:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-12 20:42:05.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/output.py
--rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/resources/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/failures.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/html5-template.txt
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/report.rst
--rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/starlab.css
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/successes.rst
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 14:24:35.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/summary.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/warnings.rst
--rw-rw-rw-   0 root         (0) root         (0)     5360 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_allowlisting.py
--rw-rw-rw-   0 root         (0) root         (0)     7875 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_config.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-06-16 19:17:04.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_sandboxing.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_offline_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     6668 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_secure_networking.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/access.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/kconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-13 16:06:35.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/mount.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2825 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/workdir.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-13 12:59:23.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5089 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-13 14:56:21.000000 kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2023-05-11 17:54:05.000000 kevlar-system-inspector-1.1.0a3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/scripts/kevlar-system-inspector
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2023-07-19 16:25:38.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2023-05-23 12:09:42.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16780 2023-06-16 18:07:28.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-13 18:39:20.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-12 20:43:03.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/output.py
+-rw-rw-rw-   0 root         (0) root         (0)    11627 2023-07-19 16:25:38.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-23 12:09:42.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-16 21:55:20.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/failures.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/html5-template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-16 17:55:02.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/report.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/starlab.css
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 18:07:28.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/successes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 14:28:48.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/summary.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:17:14.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/warnings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-07-18 17:36:36.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_allowlisting.py
+-rw-rw-rw-   0 root         (0) root         (0)     8309 2023-07-18 17:36:36.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_kernel_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-18 17:36:36.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_kernel_sandboxing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-07-19 16:25:38.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_offline_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6843 2023-07-18 17:36:36.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_secure_networking.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-18 17:36:36.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-23 12:09:42.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 18:46:09.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-23 12:09:42.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-07-19 16:25:38.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/kconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-13 16:07:34.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-07-19 16:25:38.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/mount.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-23 12:09:42.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2023-07-06 18:46:09.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-19 18:59:06.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-19 19:45:56.000000 kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/top_level.txt
```

### Comparing `kevlar-system-inspector-1.1.0a2/LICENSE` & `kevlar-system-inspector-1.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/PKG-INFO` & `kevlar-system-inspector-1.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kevlar-system-inspector-1.1.0a2/README.rst` & `kevlar-system-inspector-1.1.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/setup.cfg` & `kevlar-system-inspector-1.1.0a3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kevlar-system-inspector
-version = 1.1.0a2
+version = 1.1.0a3
 author = Star Lab
 author_email = info@starlab.io
 url = https://www.starlab.io/explore-kevlar-system-inspector
 license = MIT
 license_files = LICENSE
 description = A security scanner for Linux systems
 long_description = file: README.rst
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/__init__.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,41 @@
+"""
+A security inspector for embedded systems.
+"""
+
 import sys
 import os
 import argparse
 import shlex
 from typing import List, Any
 import platform
 
-"""
-A security inspector for embedded systems.
-"""
+
+# This MUST be here before we import anything outside of stdlib. Some of our
+# dependencies for the standalone version are un-importable on old Python
+# versions.
+def system_check() -> None:
+    """Is this a supported version of Python?"""
+    if sys.hexversion < 0x03070000:
+        sys.stderr.write(f"Detected Python version: {platform.python_version()}\n")
+        sys.stderr.write(
+            "This version is END-OF-LIFE and unsupported by Kevlar System Inspector.\n"
+        )
+        sys.exit(1)
+
+    if sys.platform != "linux":
+        sys.stderr.write(f"Detected platform: {sys.platform}\n")
+        sys.stderr.write(
+            "While we appreciate such an intrepid use of our software, Kevlar "
+            "System Inspector is, unfortunately Linux-only.\n"
+        )
+        sys.exit(1)
+
+
+system_check()
 
 
 # Set up vendored dependencies, if they exist.  This must come before 3rd party
 # imports
 _THIS_DIR = os.path.abspath(os.path.dirname(__file__))
 _VENDOR_ZIP = os.path.join(_THIS_DIR, "_vendor.zip")
 sys.path.insert(0, _VENDOR_ZIP)
@@ -39,34 +63,15 @@
         # These are usually set by terminal plugin. Various bits of pytest expect them to
         # be set. Mostly an issue only when we want to break into pdb.
         config.option.color = "yes"
         config.option.code_highlight = "yes"
         config.option.verbose = False
 
 
-def system_check() -> None:
-    """Is this a supported version of Python?"""
-    if sys.hexversion < 0x03070000:
-        sys.stderr.write(f"Detected Python version: {platform.python_version()}\n")
-        sys.stderr.write(
-            "This version is END-OF-LIFE and unsupported by Kevlar System Inspector.\n"
-        )
-        sys.exit(1)
-
-    if sys.platform != "linux":
-        sys.stderr.write(f"Detected platform: {sys.platform}\n")
-        sys.stderr.write(
-            "While we appreciate such an intrepid use of our software, Kevlar "
-            "System Inspector is, unfortunately Linux-only.\n"
-        )
-        sys.exit(1)
-
-
 def main() -> None:
-    system_check()
     parser = argparse.ArgumentParser(description=__doc__)
     output = parser.add_argument_group("Output Options")
     output.add_argument(
         "--output",
         action="store",
         help=f"""
              Print plaint text report to a file. This is the default, unless
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/conftest.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/conftest.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/console.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/console.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/decorators.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/decorators.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/output.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/output.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/report.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     lineno: int,
     inliner: states.Inliner,
     options: Optional[Dict[str, str]] = None,
     content: Optional[List[str]] = None,
 ) -> Tuple[List[docutils.nodes.Node], List[str]]:
     text = docutils.utils.unescape(text)
     code = f"SL-{text}"
-    uri = f"https://starlab.io/sl-{text}"
+    tag = "f" if is_full_version() else ""
+    uri = f"https://starlab.io/sl-{text}{tag}"
 
     try:
         options = roles.normalized_role_options(options)
     except AttributeError:
         # Old Yocto versions.
         options = {} if options is None else options
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/sysinfo.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/sysinfo.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/failures.rst` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/failures.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/report.rst` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/report.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/starlab.css` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/starlab.css`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/templates/summary.rst` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/templates/summary.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_allowlisting.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_allowlisting.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,16 @@
 @merge_tests
 class TestRunUnauthorizedBinary:
     """
     Attackers should not be able to introduce and execute binaries on a running system.
     ===================================================================================
 
     Only authorized binaries should be able to execute.
+
+    :kevlar-code:`201`
     """
 
     def test_attempt_to_run_unauthorized_binary(self, cat: Path) -> None:
         with raises(PermissionError, "An unauthorized binary was able to run."):
             subprocess.run([cat], stdin=subprocess.DEVNULL)
 
     @full_version_only
@@ -136,46 +138,54 @@
 
 def test_attempt_to_run_unauthorized_copied_binary(cat: Path) -> None:
     """
     Attackers should not able able to execute a copied binary.
     ==========================================================
 
     Copied binaries should not be authorized to execute.
+
+    :kevlar-code:`202`
     """
 
     with raises(PermissionError, "An unauthorized copied binary was able to run."):
         subprocess.run([cat], stdin=subprocess.DEVNULL)
 
 
 @full_version_only
 def test_attempt_to_load_library(libc: Path) -> None:
     """
     Attackers should not be able to introduce shared libraries.
     ===========================================================
 
     Only authorized shared libraries should be loadable.
+
+    :kevlar-code:`203`
     """
     ...
 
 
 @full_version_only
 def test_inject_via_env_var(dynamic_cat: Path, libc: Path, workdir: Path) -> None:
     """
     Attackers should not be able to inject code with environment variables.
     =======================================================================
 
     Environment variables should not facilitate injecting of arbitrary code
     into a process.
+
+    :kevlar-code:`204`
     """
     ...
 
 
 @full_version_only
 def test_attempt_to_overwrite_system_binary() -> None:
     """
     Attackers should not be able to modify protected locations.
     ===========================================================
 
     Locations such as /bin or /etc that can influence system execution or
     integrity should be read-only, even as root.
+
+    :kevlar-code:`205`
     """
     ...
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_config.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_kernel_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,98 +16,107 @@
 
 import pytest
 
 from .decorators import merge_tests, full_version_only
 from .utils.kconfig import KconfigSet
 
 
-KconfigCheckRow = Tuple[str, Optional[str], List[str], str]
+KconfigCheckRow = Tuple[str, Optional[str], List[str], str, str]
 
 KCONFIG_SIMPLE_CHECKS: List[KconfigCheckRow] = [
     # Each row:
     #   1. Config name
     #   1. String value, or NOT_PRESENT
     #   2. Dependencies. If they aren't all satisfied, this check is skipped.
     #   3. Description.
+    #   4. Code
     #
     # The config to check can appear multiple times. This is useful if there
     # are OR conditions in the dependencies like (X86_64 || X86_PAE).
     (
         "CONFIG_BUG_ON_DATA_CORRUPTION",
         "y",
         [],
         """
         The CONFIG_BUG_ON_DATA_CORRUPTION option will generate a BUG when data
         corruption is detected, rather than letting it pass with a warning.
         """,
+        "301",
     ),
     (
         "CONFIG_PAGE_POISONING",
         "y",
         [],
         """
         The CONFIG_PAGE_POISONING option will take proactive measures to mark
         freed memory pages as "poisoned" to mitigate a common class of
         vulnerabilities.
         """,
+        "302",
     ),
     (
         "CONFIG_SLAB_FREELIST_RANDOM",
         "y",
         [],
         """
         The CONFIG_SLAB_FREELIST_RANDOM option ensures that memory allocation is
         randomized to mitigate a common class of vulnerabilities.
         """,
+        "303",
     ),
     (
         "CONFIG_SLAB_FREELIST_HARDENED",
         "y",
         [],
         """
         The CONFIG_SLAB_FREELIST_HARDENED option adds additional consistency
         checks to memory allocation to mitigate a common class of
         vulnerabilities.
         """,
+        "304",
     ),
     (
         "CONFIG_PROC_KCORE",
         None,
         [],
         """
         The CONFIG_PROC_KCORE option controls the inclusion of the potentially
         dangerous /proc/kcore file.
         """,
+        "305",
     ),
     (
         "CONFIG_MODIFY_LDT_SYSCALL",
         None,
         ["CONFIG_X86=y"],
         """
         The CONFIG_MODIFY_LDT_SYSCALL option is meant for legacy 16-bit code,
         but provides attackers with an increased attack surface.
         """,
+        "306",
     ),
     (
         "CONFIG_DEVMEM",
         None,
         [],
         """
         The CONFIG_DEVMEM option controls whether userspace programs can
         directly access physical memory.
         """,
+        "307",
     ),
     (
         "CONFIG_DEBUG_CREDENTIALS",
         "y",
         ["CONFIG_DEBUG_KERNEL=y"],
         """
         The CONFIG_DEBUG_CREDENTIALS option enables additional consistency
         checking of process credentials, a common target of attackers.
         """,
+        "308",
     ),
 ]
 
 
 def _make_kconfig_ids() -> List[str]:
     seen: Dict[str, int] = defaultdict(int)
     ids = []
@@ -123,30 +132,33 @@
     return ids
 
 
 KCONFIG_SIMPLE_IDS = _make_kconfig_ids()
 
 
 @pytest.mark.parametrize(
-    ["name", "value", "dependencies", "description"],
+    ["name", "value", "dependencies", "description", "code"],
     KCONFIG_SIMPLE_CHECKS,
     ids=KCONFIG_SIMPLE_IDS,
 )
 def test_configuration_items(
     kconfig: KconfigSet,
     name: str,
     value: Optional[str],
     dependencies: List[str],
     description: Optional[str],
+    code: str,
 ) -> None:
     """
     {{ name }} should be {{ 'enabled' if value else 'disabled' }}.
     ==============================================================
 
     {{description | dedent}}
+
+    :kevlar-code:`{{code}}`.
     """
 
     if not value:
         config = f"# {name} is not set"
         message = f"{name} is **not** disabled."
     else:
         config = f"{name}={value}"
@@ -165,85 +177,99 @@
 ) -> None:
     """
     Kernel heap checks should be enabled.
     =====================================
 
     Kernel heap checks ensure the system detects and responds to memory
     corruption events involving the kernel heap.
+
+    :kevlar-code:`310`
     """
     ...
 
 
 @full_version_only
 def test_shadow_call_stack_enabled() -> None:
     """
     Shadow Call Stack should be enabled.
     ====================================
 
     The shadow call stack is a feature that prevents stack based buffer
     overflow vulnerabilities from being exploited.
+
+    :kevlar-code:`311`
     """
 
 
 @full_version_only
 def test_devices_not_enabled_via_standard_path() -> None:
     """
     Device path ``{{device_path}}`` should not be present.
     ==============================================================
 
     The ``{{device_path}}`` device enables a means of accessing physical memory
     of the system.
+
+    :kevlar-code:`312`
     """
     ...
 
 
 @full_version_only
 def test_devices_via_nonstandard_path() -> None:
     """
     ``{{device_path}}`` should be inaccessible even through indirect means.
     ============================================================================
 
     Deleting a device file path is not enough to render a device inaccessible.
     It needs to be removed from the kernel entirely.
+
+    :kevlar-code:`313`
     """
     ...
 
 
 @full_version_only
 def test_has_module_signing() -> None:
     """
     Kernel module signatures should be enabled.
     ===========================================
 
     The Linux kernel will check the integrity of loaded modules to guard
     against corruption and malware.
+
+    :kevlar-code:`314`
     """
     ...
 
 
 @full_version_only
 def test_has_strict_module_signing() -> None:
     """
     Unsigned kernel modules should not load.
     ========================================
 
     Unsigned modules should not be loadable, to guard against malware and
     corruption.
+
+    :kevlar-code:`315`
     """
     ...
 
 
 @full_version_only
 def test_has_strong_module_signing_hash() -> None:
     """
     Kernel module signatures should use strong hash functions.
     ==========================================================
 
     Only modern, cryptographically strong hash functions should be used to sign
     kernel modules.
+
+    :kevlar-code:`316`
     """
     ...
 
 
 @merge_tests
 class TestModulesUnsigned:
     """
@@ -253,14 +279,16 @@
     All kernel modules found in a running Linux system should have valid
     signatures.
 
     .. note::
 
        This test looks for the presence of a signature and validates its
        parameters, but it does not cryptographically verify the signature.
+
+    :kevlar-code:`317`
     """
 
     @full_version_only
     def test_any_modules_unsigned(self) -> None:
         ...
 
     @full_version_only
@@ -271,25 +299,29 @@
 @full_version_only
 def test_kernel_refuses_to_load_unsigned() -> None:
     """
     Kernel modules with stripped signatures should not load.
     ========================================================
 
     Attackers should not be able to strip signatures from existing modules.
+
+    :kevlar-code:`318`
     """
     ...
 
 
 @merge_tests
 class TestKernelRefusesToLoadCorrupted:
     """
     Corrupted kernel modules should not load.
     =========================================
 
     If a kernel module has been tampered with or modified, it should not load.
+
+    :kevlar-code:`319`
     """
 
     @full_version_only
     def test_kernel_refuses_to_load_corrupted_data(self) -> None:
         ...
 
     @full_version_only
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_kernel_sandboxing.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_kernel_sandboxing.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,13 +17,15 @@
 
 def test_clang_cfi_enabled(kconfig: KconfigSet) -> None:
     """
     Kernel sandboxing should be enabled.
     ====================================
 
     Kernel sandboxing support should be compiled into the kernel.
+
+    :kevlar-code:`801`.
     """
 
     if "CONFIG_ARCH_SUPPORTS_CFI_CLANG=y" not in kconfig:
         pytest.skip("N/A for this architecture")
 
     assert "CONFIG_CFI_CLANG=y" in kconfig, "Kernel sandboxing is not enabled!"
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_offline_integrity.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_offline_integrity.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,13 +87,15 @@
     """
     The root filesystem should be protected at the block level from offline modification.
     =====================================================================================
 
     The integrity of system binaries and configuration files in the root
     filesystem should be evaluated using the stronger block-based scheme vs a
     file-based scheme.
+
+    :kevlar-code:`501`
     """
 
     info = inspect_mountpoint("/")
     assert (
         info.has_integrity
     ), "Root file system is unprotected from offline modification at the block level."
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_secure_networking.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_secure_networking.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,38 +23,44 @@
     """
     DNSSEC enforcement should be enabled.
     =====================================
 
     DNSSEC is a standard that protects DNS lookups from spoofing or cache
     poisoning attacks. Without DNSSEC, there is no guarantee that the IP
     address the DNS server returned has not been maliciously altered.
+
+    :kevlar-code:`601`.
     """
     ...
 
 
 @full_version_only
 def test_dns_over_tls_is_enabled() -> None:
     """
     DNS-over-TLS should be enabled.
     ===============================
 
     Encrypting DNS using standard TLS ensures attackers cannot view or alter
     domain name lookups.
+
+    :kevlar-code:`602`.
     """
     ...
 
 
 @full_version_only
 def test_resolv_conf_uses_loopback() -> None:
     """
     ``/etc/resolv.conf`` should be configured to make secure DNS queries.
     =====================================================================
 
     By default a populated ``/etc/resolv.conf`` file will make insecure
     DNS queries.
+
+    :kevlar-code:`603`.
     """
     ...
 
 
 def _run(cmdline: List[str]) -> "subprocess.CompletedProcess[str]":
     """
     Run a command, capture output, and also make sure the output appears in the
@@ -124,14 +130,16 @@
 def test_inbound_firewall_present() -> None:
     """
     A system should be protected by an inbound firewall.
     ====================================================
 
     All systems should have an operational inbound firewall to mitigate
     attacker surveillance and other malicious activity.
+
+    :kevlar-code:`604`.
     """
     #
     # There are two failure scenarios that can be tested.
     # "No inbouund firewall", do not install nftables or iptables
     # "Firewall is configured to accept...", default INPUT policy is ACCEPT
     #
     # The test will pass if either iptables or nftables are installed and
@@ -173,14 +181,16 @@
     """
     A system should be protected by an outbound firewall.
     =====================================================
 
     All systems should have an operational outbound firewall to mitigate
     efforts by an attacker to communicate with remote access tools, pivot to
     other systems, or perform denial of service attacks.
+
+    :kevlar-code:`605`.
     """
     #
     # There is one failure scenario that can be tested.
     # "No outbouund firewall", do not install nftables or iptables
     #
     iptables_policy = _get_iptables_policy(IPTABLES_DIRECTION_OUTBOUND)
     nftables_policy = _get_nftables_policy(NFT_DIRECTION_OUTBOUND)
@@ -196,21 +206,25 @@
 def test_disallow_unencrypted_http() -> None:
     """
     Unencrypted Outbound web traffic should not be permitted.
     =========================================================
 
     All web traffic should be encrypted to prevent eavesdropping and tampering,
     even over the local network.
+
+    :kevlar-code:`606`.
     """
     ...
 
 
 @full_version_only
 def test_disallow_unencrypted_mqtt() -> None:
     """
     Unencrypted Outbound MQTT traffic should not be permitted.
     ==========================================================
 
     All MQTT traffic should be encrypted to prevent eavesdropping and
     tampering, even over the local network.
+
+    :kevlar-code:`607`.
     """
     ...
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/test_systemd_syscall_filtering.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/test_systemd_syscall_filtering.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 def test_systemd_has_seccomp_enabled() -> None:
     """
     Systemd should be built with application sandboxing support.
     ============================================================
 
     Systemd support for application sandboxing is a compile-time option that
     should be enabled.
+
+    :kevlar-code:`701`
     """
 
     result = subprocess.run(
         ["systemctl", "--version"], text=True, stdout=subprocess.PIPE
     )
     assert "+SECCOMP" in result.stdout, "Systemd was not compiled with seccomp support."
 
@@ -50,9 +52,11 @@
 @full_version_only
 def test_has_filter_installed() -> None:
     """
     The systemd-resolved service should be protected with application sandboxing.
     ===============================================================================================
 
     Application sandboxing is available for this service, and it should be enabled.
+
+    :kevlar-code:`702`
     """
     ...
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/__init__.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/elf.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/elf.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/kconfig.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/kconfig.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/modules.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/modules.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/mount.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/mount.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/systemd.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/systemd.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector/utils/workdir.py` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector/utils/workdir.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/PKG-INFO` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `kevlar-system-inspector-1.1.0a2/src/kevlar_system_inspector.egg-info/SOURCES.txt` & `kevlar-system-inspector-1.1.0a3/src/kevlar_system_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

