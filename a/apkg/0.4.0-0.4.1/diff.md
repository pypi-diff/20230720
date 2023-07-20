# Comparing `tmp/apkg-0.4.0.tar.gz` & `tmp/apkg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkg-0.4.0.tar", last modified: Mon Jul 18 11:08:02 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `apkg-0.4.0.tar` & `apkg-0.4.1.tar`

### file list

```diff
@@ -1,61 +1,52 @@
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.258638 apkg-0.4.0/
--rw-r--r--   0 jru       (1000) jru       (1000)    35427 2021-03-22 11:19:26.000000 apkg-0.4.0/COPYING
--rw-r--r--   0 jru       (1000) jru       (1000)     1308 2022-07-18 11:08:02.258638 apkg-0.4.0/PKG-INFO
--rw-r--r--   0 jru       (1000) jru       (1000)      525 2021-05-24 11:44:11.000000 apkg-0.4.0/README.md
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.258638 apkg-0.4.0/apkg/
--rw-r--r--   0 jru       (1000) jru       (1000)       65 2022-02-03 17:55:58.000000 apkg-0.4.0/apkg/__init__.py
--rw-r--r--   0 jru       (1000) jru       (1000)       35 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/__main__.py
--rw-r--r--   0 jru       (1000) jru       (1000)       60 2022-07-18 11:08:02.258638 apkg-0.4.0/apkg/_static_version.py
--rw-r--r--   0 jru       (1000) jru       (1000)     6322 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/_version.py
--rw-r--r--   0 jru       (1000) jru       (1000)     7944 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/adistro.py
--rw-r--r--   0 jru       (1000) jru       (1000)     5531 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/cache.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4537 2022-07-13 13:53:24.000000 apkg-0.4.0/apkg/cli.py
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.255305 apkg-0.4.0/apkg/commands/
--rw-r--r--   0 jru       (1000) jru       (1000)        0 2021-05-25 17:02:34.000000 apkg-0.4.0/apkg/commands/__init__.py
--rw-r--r--   0 jru       (1000) jru       (1000)     6123 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/commands/build.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4805 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/commands/build_dep.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1554 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/commands/clean.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4040 2022-07-13 13:53:24.000000 apkg-0.4.0/apkg/commands/compat.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4602 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/commands/get_archive.py
--rw-r--r--   0 jru       (1000) jru       (1000)     2885 2022-07-15 18:23:38.000000 apkg-0.4.0/apkg/commands/info.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4353 2021-10-05 16:20:09.000000 apkg-0.4.0/apkg/commands/install.py
--rw-r--r--   0 jru       (1000) jru       (1000)     3071 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/commands/make_archive.py
--rw-r--r--   0 jru       (1000) jru       (1000)     7276 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/commands/srcpkg.py
--rw-r--r--   0 jru       (1000) jru       (1000)     3416 2022-05-24 12:56:21.000000 apkg-0.4.0/apkg/commands/status.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1647 2022-07-13 04:16:21.000000 apkg-0.4.0/apkg/commands/system_setup.py
--rw-r--r--   0 jru       (1000) jru       (1000)     5619 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/commands/test.py
--rw-r--r--   0 jru       (1000) jru       (1000)     2777 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/commands/test_dep.py
--rw-r--r--   0 jru       (1000) jru       (1000)     2143 2022-07-13 13:53:24.000000 apkg-0.4.0/apkg/compat.py
--rw-r--r--   0 jru       (1000) jru       (1000)     3849 2022-07-13 13:53:24.000000 apkg-0.4.0/apkg/ex.py
--rw-r--r--   0 jru       (1000) jru       (1000)     6027 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/log.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1186 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/parse.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1735 2021-10-13 10:31:20.000000 apkg-0.4.0/apkg/pkgstyle.py
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.255305 apkg-0.4.0/apkg/pkgstyles/
--rw-r--r--   0 jru       (1000) jru       (1000)        0 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/pkgstyles/__init__.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4337 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/pkgstyles/arch.py
--rw-r--r--   0 jru       (1000) jru       (1000)    10430 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/pkgstyles/deb.py
--rw-r--r--   0 jru       (1000) jru       (1000)     3879 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/pkgstyles/nix.py
--rw-r--r--   0 jru       (1000) jru       (1000)     7815 2022-07-13 13:53:24.000000 apkg-0.4.0/apkg/pkgstyles/rpm.py
--rw-r--r--   0 jru       (1000) jru       (1000)     7785 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/pkgtemplate.py
--rw-r--r--   0 jru       (1000) jru       (1000)    12771 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/pkgtest.py
--rw-r--r--   0 jru       (1000) jru       (1000)    10032 2022-07-12 17:45:53.000000 apkg-0.4.0/apkg/project.py
--rw-r--r--   0 jru       (1000) jru       (1000)      811 2021-10-13 10:31:20.000000 apkg-0.4.0/apkg/terminal.py
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.258638 apkg-0.4.0/apkg/util/
--rw-r--r--   0 jru       (1000) jru       (1000)        0 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/util/__init__.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1610 2022-05-24 12:56:21.000000 apkg-0.4.0/apkg/util/archive.py
--rw-r--r--   0 jru       (1000) jru       (1000)     4092 2022-07-15 18:16:26.000000 apkg-0.4.0/apkg/util/common.py
--rw-r--r--   0 jru       (1000) jru       (1000)     8795 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/util/git.py
--rw-r--r--   0 jru       (1000) jru       (1000)     7775 2022-07-13 04:16:21.000000 apkg-0.4.0/apkg/util/run.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1042 2021-04-29 17:38:26.000000 apkg-0.4.0/apkg/util/shutil35.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1560 2022-06-29 13:29:52.000000 apkg-0.4.0/apkg/util/test.py
--rw-r--r--   0 jru       (1000) jru       (1000)     1633 2022-06-27 13:40:39.000000 apkg-0.4.0/apkg/util/upstreamversion.py
-drwxr-xr-x   0 jru       (1000) jru       (1000)        0 2022-07-18 11:08:02.255305 apkg-0.4.0/apkg.egg-info/
--rw-r--r--   0 jru       (1000) jru       (1000)     1308 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/PKG-INFO
--rw-r--r--   0 jru       (1000) jru       (1000)     1113 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/SOURCES.txt
--rw-r--r--   0 jru       (1000) jru       (1000)        1 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/dependency_links.txt
--rw-r--r--   0 jru       (1000) jru       (1000)       39 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/entry_points.txt
--rw-r--r--   0 jru       (1000) jru       (1000)       85 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/requires.txt
--rw-r--r--   0 jru       (1000) jru       (1000)        5 2022-07-18 11:08:02.000000 apkg-0.4.0/apkg.egg-info/top_level.txt
--rw-r--r--   0 jru       (1000) jru       (1000)      104 2021-04-29 17:38:26.000000 apkg-0.4.0/pyproject.toml
--rw-r--r--   0 jru       (1000) jru       (1000)     1102 2022-07-18 11:08:02.258638 apkg-0.4.0/setup.cfg
--rwxr-xr-x   0 jru       (1000) jru       (1000)      637 2021-04-29 17:38:26.000000 apkg-0.4.0/setup.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/CHANGELOG.md -> docs/news.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 apkg-0.4.1/requirements.txt
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apkg-0.4.1/setup.cfg
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 apkg-0.4.1/setup.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/__main__.py
+-rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/adistro.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/cache.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/cli.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/compat.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/ex.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/log.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/parse.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyle.py
+-rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgtemplate.py
+-rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgtest.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/project.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/__init__.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/build.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/build_dep.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/clean.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/compat.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/get_archive.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/info.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/install.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/make_archive.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/srcpkg.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/status.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/system_setup.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/test.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/test_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/__init__.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/arch.py
+-rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/deb.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/nix.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/rpm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/archive.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/common.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/git.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/run.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/shutil35.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/test.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/upstreamversion.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 apkg-0.4.1/scripts/make-archive.sh
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 apkg-0.4.1/scripts/upstream-version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 apkg-0.4.1/.gitignore
+-rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 apkg-0.4.1/COPYING
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apkg-0.4.1/README.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 apkg-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 apkg-0.4.1/PKG-INFO
```

### Comparing `apkg-0.4.0/COPYING` & `apkg-0.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/README.md` & `apkg-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/adistro.py` & `apkg-0.4.1/apkg/adistro.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,18 @@
         * names with release first
         * primary sort by name
         * secondary sort by release desc (for determinism)
     """
 
     def sort_key(o):
         distro_, _, rls = getattr(o, name_attr).rpartition('-')
-        rlsv = version.parse(rls)
+        try:
+            rlsv = version.parse(rls)
+        except version.InvalidVersion:
+            rlsv = rls
         return distro_, common.SortReversor(rlsv)
 
     plain_objs = []
     rls_objs = []
     for o in objs:
         if '-' in getattr(o, name_attr):
             rls_objs.append(o)
```

### Comparing `apkg-0.4.0/apkg/cache.py` & `apkg-0.4.1/apkg/cache.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/cli.py` & `apkg-0.4.1/apkg/cli.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/build.py` & `apkg-0.4.1/apkg/commands/build.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/build_dep.py` & `apkg-0.4.1/apkg/commands/build_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/clean.py` & `apkg-0.4.1/apkg/commands/clean.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/compat.py` & `apkg-0.4.1/apkg/commands/compat.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/get_archive.py` & `apkg-0.4.1/apkg/commands/get_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/info.py` & `apkg-0.4.1/apkg/commands/info.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/install.py` & `apkg-0.4.1/apkg/commands/install.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/make_archive.py` & `apkg-0.4.1/apkg/commands/make_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/srcpkg.py` & `apkg-0.4.1/apkg/commands/srcpkg.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/status.py` & `apkg-0.4.1/apkg/commands/status.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/system_setup.py` & `apkg-0.4.1/apkg/commands/system_setup.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/test.py` & `apkg-0.4.1/apkg/commands/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/commands/test_dep.py` & `apkg-0.4.1/apkg/commands/test_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/compat.py` & `apkg-0.4.1/apkg/compat.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/ex.py` & `apkg-0.4.1/apkg/ex.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/log.py` & `apkg-0.4.1/apkg/log.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/parse.py` & `apkg-0.4.1/apkg/parse.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/pkgstyle.py` & `apkg-0.4.1/apkg/pkgstyle.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/pkgstyles/arch.py` & `apkg-0.4.1/apkg/pkgstyles/arch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,20 @@
 import apkg.util.shutil35 as shutil
 
 
 log = getLogger(__name__)
 
 
 SUPPORTED_DISTROS = [
-    'arch'
+    'arch',
+    'manjaro',
 ]
+DISTRO_REQUIRES = {
+    'core': ['base-devel'],
+}
 
 
 RE_PKG_NAME = r'pkgname\s*=\s*(\S+)'
 
 
 def is_valid_template(path):
     pkgbuild = path / "PKGBUILD"
@@ -89,15 +93,15 @@
     return pkgs
 
 
 def install_distro_packages(
         packages,
         **kwargs):
     interactive = kwargs.get('interactive', False)
-    cmd = ['pacman', '-S']
+    cmd = ['pacman', '-S', '--needed']
     if not interactive:
         cmd += ['--noconfirm']
     cmd += packages
     sudo(cmd)
 
 
 def install_custom_packages(
```

### Comparing `apkg-0.4.0/apkg/pkgstyles/deb.py` & `apkg-0.4.1/apkg/pkgstyles/deb.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,22 @@
 import apkg.util.shutil35 as shutil
 
 
 log = getLogger(__name__)
 
 
 SUPPORTED_DISTROS = [
-    "ubuntu",
     "debian",
     "linuxmint",
+    "pop",
     "raspbian",
+    "ubuntu",
 ]
 DISTRO_REQUIRES = {
-    'core': ['devscripts'],
+    'core': ['build-essential'],
     'isolated': ['pbuilder'],
 }
 
 
 def format_date():
     """
     current date and time in Debian changelog format (RFC 2822)
```

### Comparing `apkg-0.4.0/apkg/pkgstyles/nix.py` & `apkg-0.4.1/apkg/pkgstyles/nix.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/pkgstyles/rpm.py` & `apkg-0.4.1/apkg/pkgstyles/rpm.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/pkgtemplate.py` & `apkg-0.4.1/apkg/pkgtemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,12 +247,23 @@
             pkgstyle_tps.append(template)
             continue
 
         # distro-specific template
         template.distro_rules = adistro.name2rule(template.name)
         distro_tps.append(template)
 
+    alias_tps = sort_alias_templates(alias_tps, distro_aliases)
     distro_tps = adistro.sort_by_name(distro_tps)
-    alias_tps.sort(key=lambda x: x.name)
     pkgstyle_tps.sort(key=lambda x: x.name)
     templates = alias_tps + distro_tps + pkgstyle_tps
     return templates
+
+
+def sort_alias_templates(alias_templates, distro_aliases):
+    result = []
+    for da in distro_aliases:
+        for at in alias_templates:
+            if at.name == da:
+                result.append(at)
+                break
+    assert len(alias_templates) == len(result)
+    return result
```

### Comparing `apkg-0.4.0/apkg/pkgtest.py` & `apkg-0.4.1/apkg/pkgtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,17 @@
     if tests_dir:
         tests_dir = Path(tests_dir)
     deps_text = msg['Depends']
     restrictions_text = msg['Restrictions']
 
     if deps_text:
         deps = re.split(r'[\s\n]*,[\s\n]*', deps_text.strip())
-        if '@' in deps:
-            # @ means "all packages built from source package"
-            # this is implicit with apkg tests
-            deps.remove('@')
+        # @ means "all packages built from source package"
+        # this is implicit with apkg tests
+        deps = [d for d in deps if d and d != '@']
 
     if restrictions_text:
         restrictions = re.split(r'[\s\n]+', restrictions_text.strip())
 
     if not (tests_text or test_command_text):
         log.warning("Test missing both Tests and Test-Command fields"
                     " - skipping. Test text:\n%s", test_text)
```

### Comparing `apkg-0.4.0/apkg/project.py` & `apkg-0.4.1/apkg/project.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/terminal.py` & `apkg-0.4.1/apkg/terminal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 class NullCallableString(str):
     """
-    This emulates blessings class for cases when blessings aren't available
+    This emulates blessed class for cases when blessed isn't available
     """
     def __new__(cls):
         return str.__new__(cls, '')
 
     def __call__(self, arg, *extra_args):
         if isinstance(arg, int):
             return ''
         return arg
 
 
 class PlainTerminal:
     """
-    Mock of blessings Terminal that ignores formatting
+    Mock of blessed Terminal that ignores formatting
     """
     nullstr = NullCallableString()
 
     def __getattr__(self, attr):
         setattr(self, attr, self.nullstr)
         return self.nullstr
 
 
 COLOR_TERMINAL = False
 try:
-    import blessings
+    try:
+        import blessed
+    except Exception:
+        import blessings as blessed
     # this can throw _curses.error: setupterm: could not find terminal
     # better find out now
-    blessings.Terminal()
-    Terminal = blessings.Terminal
+    blessed.Terminal()
+    Terminal = blessed.Terminal
     COLOR_TERMINAL = True
 except Exception:
     Terminal = PlainTerminal
```

### Comparing `apkg-0.4.0/apkg/util/archive.py` & `apkg-0.4.1/apkg/util/archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/util/common.py` & `apkg-0.4.1/apkg/util/common.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/util/git.py` & `apkg-0.4.1/apkg/util/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             return
         if remote_branch is None:
             for rbr in self.remote_branches():
                 br = rbr[rbr.find('/') + 1:]
                 if branch in [rbr, br]:
                     remote_branch = rbr
         elif remote_branch not in self.remote_branches():
-            raise Exception("Branch %s doesn't exist in remotes" %
-                            remote_branch)
+            raise ex.InvalidUsage(
+                msg="Branch %s doesn't exist in remotes" % remote_branch)
         self.create_branch(branch, remote_branch)
 
     def _parse_output(self, out):
         output = [o.strip() for o in out.split("\n") if o]
         return output
 
     def _parse_branch_output(self, out):
```

### Comparing `apkg-0.4.0/apkg/util/run.py` & `apkg-0.4.1/apkg/util/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,18 +155,18 @@
         sink.append(line_str)
         print(line_str, file=sys.stderr)
 
     loop = asyncio.get_event_loop_policy().get_event_loop()
     tasks = []
     if process.stdout:
         tasks.append(loop.create_task(_read_stream(
-            process.stdout, lambda l: tee_fun(l, out))))
+            process.stdout, lambda x: tee_fun(x, out))))
     if process.stderr:
         tasks.append(loop.create_task(_read_stream(
-            process.stderr, lambda l: tee_fun(l, err))))
+            process.stderr, lambda x: tee_fun(x, err))))
 
     await asyncio.wait(set(tasks))
 
     stdout = os.linesep.join(out) + os.linesep
     stderr = os.linesep.join(err) + os.linesep
 
     return subprocess.CompletedProcess(
```

### Comparing `apkg-0.4.0/apkg/util/shutil35.py` & `apkg-0.4.1/apkg/util/shutil35.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/util/test.py` & `apkg-0.4.1/apkg/util/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.0/apkg/util/upstreamversion.py` & `apkg-0.4.1/apkg/util/upstreamversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,21 @@
     v_max = version.parse('0')
     r = requests.get(html_listing_url)
     soup = bs4.BeautifulSoup(r.content, 'html.parser')
     for a in soup.find_all('a'):
         m = re.match(RE_ARCHIVE_VERSION, a.string)
         if not m:
             continue
-        v = version.parse(m.group(1))
+        v_str = m.group(1)
+        try:
+            v = version.parse(v_str)
+        except version.InvalidVersion:
+            log.verbose("Ignoring invalid upstream version: %s in %s",
+                        v_str, a.string)
+            continue
         v_max = max(v, v_max)
         found = True
     if found:
         return v_max
     return None
```

### Comparing `apkg-0.4.0/setup.cfg` & `apkg-0.4.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,49 @@
+# Backward compatbile with ancient setuptools.
+# Modern python packaging tools are supported through pyproject.toml.
 [metadata]
 name = apkg
 author = Jakub Ružicka
-author-email = jakub.ruzicka@nic.cz
+author_email = jakub.ruzicka@nic.cz
 description = cross-distro upstream packaging automation tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.nic.cz/packaging/apkg
-project_urls = 
-	Bug Tracker = https://gitlab.nic.cz/packaging/apkg/-/issues
-	Docs = https://apkg.readthedocs.io/
-classifiers = 
-	Development Status :: 4 - Beta
-	Environment :: Console
-	Intended Audience :: Developers
-	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-	Operating System :: OS Independent
-	Programming Language :: Python :: 3
-	Topic :: System :: Archiving :: Packaging
-	Topic :: Utilities
+project_urls =
+    Bug Tracker = https://gitlab.nic.cz/packaging/apkg/-/issues
+    Docs = https://apkg.readthedocs.io/
+classifiers =
+    Development Status :: 4 - Beta
+    Environment :: Console
+    Intended Audience :: Developers
+    License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+    Operating System :: OS Independent
+    Programming Language :: Python :: 3
+    Topic :: System :: Archiving :: Packaging
+    Topic :: Utilities
 
 [options]
 packages = find:
-install_requires = 
-	beautifulsoup4
-	blessings
-	cached_property
-	click
-	distro
-	jinja2
-	packaging
-	requests
-	toml
+install_requires =
+    beautifulsoup4
+    blessed
+    cached_property
+    click
+    distro
+    jinja2
+    packaging
+    requests
+    toml
 
 [options.packages.find]
-exclude = 
-	docs
+exclude =
+    docs
 
 [options.entry_points]
-console_scripts = 
-	apkg = apkg.cli:main
+console_scripts =
+    apkg = apkg.cli:main
 
 [pycodestyle]
-exclude = build,lib,.tox,third,*.egg,docs,packages,.eggs
+exclude=build,lib,.tox,third,*.egg,docs,packages,.eggs
+# E123, E125, W503 skipped as they are invalid PEP-8.
 ignore = E123,E125,W503
 show-source = True
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
```

