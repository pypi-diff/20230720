# Comparing `tmp/pip-rating-0.0.1.tar.gz` & `tmp/pip-rating-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-rating-0.0.1.tar", last modified: Wed Jul 12 06:34:02 2023, max compression
+gzip compressed data, was "pip-rating-0.1.0.tar", last modified: Thu Jul 20 20:38:52 2023, max compression
```

## Comparing `pip-rating-0.0.1.tar` & `pip-rating-0.1.0.tar`

### file list

```diff
@@ -1,64 +1,45 @@
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.905526 pip-rating-0.0.1/
--rw-r--r--   0 nekmo     (1000) users      (100)      149 2023-06-30 01:00:25.000000 pip-rating-0.0.1/AUTHORS.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     3413 2023-07-11 23:52:04.000000 pip-rating-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       89 2023-06-30 01:00:25.000000 pip-rating-0.0.1/HISTORY.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1065 2023-06-30 01:00:25.000000 pip-rating-0.0.1/LICENSE
--rw-r--r--   0 nekmo     (1000) users      (100)      377 2023-06-30 01:00:25.000000 pip-rating-0.0.1/MANIFEST.in
--rw-r--r--   0 nekmo     (1000) users      (100)     2555 2023-07-12 06:34:02.905526 pip-rating-0.0.1/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     1471 2023-07-11 23:52:04.000000 pip-rating-0.0.1/README.rst
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.898860 pip-rating-0.0.1/docs/
--rw-r--r--   0 nekmo     (1000) users      (100)      678 2023-07-11 23:49:43.000000 pip-rating-0.0.1/docs/Makefile
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.898860 pip-rating-0.0.1/docs/_static/
--rw-r--r--   0 nekmo     (1000) users      (100)     7791 2023-07-11 03:33:35.000000 pip-rating-0.0.1/docs/_static/forkme_right_darkblue_121621.png
--rw-r--r--   0 nekmo     (1000) users      (100)       28 2023-06-30 01:00:26.000000 pip-rating-0.0.1/docs/authors.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     2171 2023-07-11 23:52:04.000000 pip-rating-0.0.1/docs/conf.py
--rw-r--r--   0 nekmo     (1000) users      (100)       33 2023-06-30 01:00:26.000000 pip-rating-0.0.1/docs/contributing.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       28 2023-06-30 01:00:26.000000 pip-rating-0.0.1/docs/history.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      549 2023-07-11 23:52:04.000000 pip-rating-0.0.1/docs/index.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1397 2023-07-11 23:52:04.000000 pip-rating-0.0.1/docs/installation.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      800 2023-07-11 03:02:36.000000 pip-rating-0.0.1/docs/make.bat
--rw-r--r--   0 nekmo     (1000) users      (100)       67 2023-07-11 23:53:20.000000 pip-rating-0.0.1/docs/modules.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     7132 2023-07-11 23:52:04.000000 pip-rating-0.0.1/docs/overview.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1481 2023-07-11 23:53:20.000000 pip-rating-0.0.1/docs/pip_rating.req_files.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1183 2023-07-11 23:53:20.000000 pip-rating-0.0.1/docs/pip_rating.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1058 2023-07-11 23:53:20.000000 pip-rating-0.0.1/docs/pip_rating.sources.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       27 2023-06-30 01:00:26.000000 pip-rating-0.0.1/docs/readme.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       33 2023-06-30 01:00:26.000000 pip-rating-0.0.1/docs/troubleshooting.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     8038 2023-07-11 23:52:04.000000 pip-rating-0.0.1/docs/usage.rst
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.902193 pip-rating-0.0.1/pip_rating/
--rw-r--r--   0 nekmo     (1000) users      (100)      174 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)      690 2023-07-11 15:08:10.000000 pip-rating-0.0.1/pip_rating/_compat.py
--rw-r--r--   0 nekmo     (1000) users      (100)     5049 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/dependencies.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1764 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/exceptions.py
--rw-r--r--   0 nekmo     (1000) users      (100)     5872 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/management.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3347 2023-07-11 23:49:43.000000 pip-rating-0.0.1/pip_rating/packages.py
--rw-r--r--   0 nekmo     (1000) users      (100)    10704 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/rating.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.905526 pip-rating-0.0.1/pip_rating/req_files/
--rw-r--r--   0 nekmo     (1000) users      (100)     1466 2023-07-11 23:49:43.000000 pip-rating-0.0.1/pip_rating/req_files/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1444 2023-07-08 22:13:19.000000 pip-rating-0.0.1/pip_rating/req_files/base.py
--rw-r--r--   0 nekmo     (1000) users      (100)      903 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/req_files/package_list.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1017 2023-07-11 23:49:43.000000 pip-rating-0.0.1/pip_rating/req_files/pipfile.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3370 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/req_files/pyproject.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1776 2023-07-11 23:49:43.000000 pip-rating-0.0.1/pip_rating/req_files/requirements.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1076 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/req_files/setupcfg.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1800 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/req_files/setuppy.py
--rw-r--r--   0 nekmo     (1000) users      (100)    10067 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/results.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.905526 pip-rating-0.0.1/pip_rating/sources/
--rw-r--r--   0 nekmo     (1000) users      (100)        0 2023-07-07 14:57:52.000000 pip-rating-0.0.1/pip_rating/sources/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)     2491 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/sources/audit.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1248 2023-07-11 23:52:04.000000 pip-rating-0.0.1/pip_rating/sources/base.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3093 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/sources/pypi.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3151 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/sources/sourcecode_page.py
--rw-r--r--   0 nekmo     (1000) users      (100)     2570 2023-07-11 23:49:44.000000 pip-rating-0.0.1/pip_rating/sources/sourcerank.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-12 06:34:02.902193 pip-rating-0.0.1/pip_rating.egg-info/
--rw-r--r--   0 nekmo     (1000) users      (100)     2555 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     1356 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/SOURCES.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/dependency_links.txt
--rw-r--r--   0 nekmo     (1000) users      (100)       60 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/entry_points.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/not-zip-safe
--rw-r--r--   0 nekmo     (1000) users      (100)      232 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/requires.txt
--rw-r--r--   0 nekmo     (1000) users      (100)       11 2023-07-12 06:34:02.000000 pip-rating-0.0.1/pip_rating.egg-info/top_level.txt
--rw-r--r--   0 nekmo     (1000) users      (100)      275 2023-06-30 01:00:25.000000 pip-rating-0.0.1/pyproject.toml
--rw-r--r--   0 nekmo     (1000) users      (100)      230 2023-07-09 18:44:41.000000 pip-rating-0.0.1/requirements.in
--rw-r--r--   0 nekmo     (1000) users      (100)     1834 2023-07-09 18:47:33.000000 pip-rating-0.0.1/requirements.txt
--rw-r--r--   0 nekmo     (1000) users      (100)     1690 2023-07-12 06:34:02.905526 pip-rating-0.0.1/setup.cfg
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/
+-rw-r--r--   0 nekmo     (1000) users      (100)      149 2023-06-30 01:00:25.000000 pip-rating-0.1.0/AUTHORS.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)     3413 2023-07-11 23:52:04.000000 pip-rating-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)       89 2023-06-30 01:00:25.000000 pip-rating-0.1.0/HISTORY.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)     1065 2023-06-30 01:00:25.000000 pip-rating-0.1.0/LICENSE
+-rw-r--r--   0 nekmo     (1000) users      (100)      304 2023-07-20 20:38:42.000000 pip-rating-0.1.0/MANIFEST.in
+-rw-r--r--   0 nekmo     (1000) users      (100)     5761 2023-07-20 20:38:52.143433 pip-rating-0.1.0/PKG-INFO
+-rw-r--r--   0 nekmo     (1000) users      (100)     4727 2023-07-20 20:38:48.000000 pip-rating-0.1.0/README.rst
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.136766 pip-rating-0.1.0/pip_rating/
+-rw-r--r--   0 nekmo     (1000) users      (100)      174 2023-07-20 19:57:00.000000 pip-rating-0.1.0/pip_rating/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)      690 2023-07-11 15:08:10.000000 pip-rating-0.1.0/pip_rating/_compat.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     5432 2023-07-17 14:50:17.000000 pip-rating-0.1.0/pip_rating/dependencies.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1799 2023-07-18 02:42:23.000000 pip-rating-0.1.0/pip_rating/exceptions.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     6828 2023-07-17 15:05:40.000000 pip-rating-0.1.0/pip_rating/management.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3530 2023-07-18 12:14:07.000000 pip-rating-0.1.0/pip_rating/packages.py
+-rw-r--r--   0 nekmo     (1000) users      (100)    11032 2023-07-19 21:53:29.000000 pip-rating-0.1.0/pip_rating/rating.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/pip_rating/req_files/
+-rw-r--r--   0 nekmo     (1000) users      (100)     1493 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1475 2023-07-17 14:41:01.000000 pip-rating-0.1.0/pip_rating/req_files/base.py
+-rw-r--r--   0 nekmo     (1000) users      (100)      909 2023-07-20 12:26:26.000000 pip-rating-0.1.0/pip_rating/req_files/package_list.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1018 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/pipfile.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3575 2023-07-20 13:49:50.000000 pip-rating-0.1.0/pip_rating/req_files/pyproject.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1916 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/requirements.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1077 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/setupcfg.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1869 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/setuppy.py
+-rw-r--r--   0 nekmo     (1000) users      (100)    10621 2023-07-20 01:02:43.000000 pip-rating-0.1.0/pip_rating/results.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/pip_rating/sources/
+-rw-r--r--   0 nekmo     (1000) users      (100)        0 2023-07-07 14:57:52.000000 pip-rating-0.1.0/pip_rating/sources/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     2551 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/audit.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1283 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/base.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3065 2023-07-18 02:27:12.000000 pip-rating-0.1.0/pip_rating/sources/pypi.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     4494 2023-07-17 15:51:54.000000 pip-rating-0.1.0/pip_rating/sources/sourcecode_page.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     2592 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/sourcerank.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.140099 pip-rating-0.1.0/pip_rating.egg-info/
+-rw-r--r--   0 nekmo     (1000) users      (100)     5761 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/PKG-INFO
+-rw-r--r--   0 nekmo     (1000) users      (100)     1007 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/SOURCES.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/dependency_links.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)       60 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/entry_points.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-20 20:38:50.000000 pip-rating-0.1.0/pip_rating.egg-info/not-zip-safe
+-rw-r--r--   0 nekmo     (1000) users      (100)      232 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/requires.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)       17 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/top_level.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)      275 2023-06-30 01:00:25.000000 pip-rating-0.1.0/pyproject.toml
+-rw-r--r--   0 nekmo     (1000) users      (100)      230 2023-07-09 18:44:41.000000 pip-rating-0.1.0/requirements.in
+-rw-r--r--   0 nekmo     (1000) users      (100)     1834 2023-07-18 02:22:09.000000 pip-rating-0.1.0/requirements.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)     1668 2023-07-20 20:38:52.146766 pip-rating-0.1.0/setup.cfg
```

### Comparing `pip-rating-0.0.1/CONTRIBUTING.rst` & `pip-rating-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pip-rating-0.0.1/LICENSE` & `pip-rating-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-rating-0.0.1/pip_rating/_compat.py` & `pip-rating-0.1.0/pip_rating/_compat.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.0.1/pip_rating/dependencies.py` & `pip-rating-0.1.0/pip_rating/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 if TYPE_CHECKING:
     from pip_rating.req_files.base import ReqFileBase
     from pip_rating.results import Results
 
 
 COMMENT_REGEX = re.compile(r"(#.*)")
-version_resolver_threads = os.environ.get("VERSION_RESOLVER_THREADS", max(8, cpu_count() * 2))
+version_resolver_threads = os.environ.get(
+    "VERSION_RESOLVER_THREADS", max(8, cpu_count() * 2)
+)
 
 
 class DependenciesVersionSolver(VersionSolver):
     def __init__(self, results: "Results", source: "PackageSource", threads: int = 1):
         self.results = results
         super().__init__(source, threads=threads)
 
@@ -34,32 +36,43 @@
         return super()._propagate(package)
 
 
 class Dependencies:
     """
     Dependencies class. This class is responsible for getting the packages tree.
     """
-    def __init__(self, results: "Results", req_file: "ReqFileBase", cache_dir: Optional[str] = None,
-                 index_url: Optional[str] = None, extra_index_url: Optional[str] = None, pre: bool = False):
+
+    def __init__(
+        self,
+        results: "Results",
+        req_file: "ReqFileBase",
+        cache_dir: Optional[str] = None,
+        index_url: Optional[str] = None,
+        extra_index_url: Optional[str] = None,
+        pre: bool = False,
+        ignore_packages: Optional[list] = None,
+    ):
         """Initialize the Dependencies class using the given req_file.
 
         :param results: The results instance. This instance will be used to print the results in the console.
         :param req_file: Dependencies list as req_file.
         :param cache_dir: The cache directory path.
         :param index_url: The index URL.
         :param extra_index_url: The extra index URL.
         :param pre: Whether to include pre-release and development versions. Defaults to False.
+        :param ignore_packages: List of packages to ignore.
         """
         self.results = results
         self.req_file = req_file
         self.cache_dir = cache_dir
         self.index_url = index_url
         self.extra_index_url = extra_index_url
         self.pre = pre
         self.packages = {}  # type: Dict[str, Package]
+        self.ignore_packages = ignore_packages or []
 
     @cached_property
     def package_source(self) -> PackageSource:
         """Describe requirements, and discover dependencies on demand."""
         return PackageSource(
             cache_dir=self.cache_dir,
             index_url=self.index_url,
@@ -68,15 +81,17 @@
         )
 
     @cached_property
     def version_solution(self) -> Union[SolverResult, PartialSolution]:
         """Get the version solution for the packages. The version solver that finds a
         set of package versions that satisfy the root package's dependencies.
         """
-        solver = DependenciesVersionSolver(self.results, self.package_source, threads=version_resolver_threads)
+        solver = DependenciesVersionSolver(
+            self.results, self.package_source, threads=version_resolver_threads
+        )
         for root_dependency in self.req_file:
             self.package_source.root_dep(root_dependency)
         try:
             return solver.solve()
         except RuntimeError as e:
             if "Failed to download/build wheel" not in str(e):
                 # only continue handling expected RuntimeErrors
@@ -92,33 +107,40 @@
                 continue
             decision_packages[package] = version
         tree_root, packages_tree_dict, packages_flat = build_tree(
             self.package_source, decision_packages
         )
         return tree_root
 
-    def add_node_package(self, node: Node) -> Package:
+    def add_node_package(self, node: Node) -> Optional[Package]:
         """Add the package as a node to the packages' dict."""
+        if node.name in self.ignore_packages:
+            return
         if node.name not in self.packages:
             self.packages[node.name] = Package(self, node.name)
         self.packages[node.name].add_node(node)
         return self.packages[node.name]
 
     def get_packages(self):
         for dependency_node in self.dependencies_tree.children:
             self.add_node_package(dependency_node)
         return self.packages
 
     @cached_property
     def total_size(self):
-        return sum(sum([node.size for node in package.nodes]) for package in self.packages.values())
+        return sum(
+            sum([node.size for node in package.nodes])
+            for package in self.packages.values()
+        )
 
     def get_global_rating_score(self):
         final_global_rating_score = None
         packages = dict(self.get_packages()).values()
         for package in packages:
             global_rating_score = package.rating.get_global_rating_score()
             if final_global_rating_score is None:
                 final_global_rating_score = global_rating_score
             else:
-                final_global_rating_score = min(global_rating_score, final_global_rating_score)
+                final_global_rating_score = min(
+                    global_rating_score, final_global_rating_score
+                )
         return final_global_rating_score
```

### Comparing `pip-rating-0.0.1/pip_rating/exceptions.py` & `pip-rating-0.1.0/pip_rating/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 """Exceptions for pip-rating."""
 import sys
 
 from rich.console import Console
 
 
 class RequirementsRatingError(Exception):
-    body = ''
+    body = ""
     exit_code = 10
 
-    def __init__(self, extra_body=''):
+    def __init__(self, extra_body=""):
         self.extra_body = extra_body
 
     def __str__(self):
         msg = self.__class__.__name__
         if self.body:
-            msg += ': {}'.format(self.body)
+            msg += ": {}".format(self.body)
         if self.extra_body:
-            msg += ('. {}' if self.body else ': {}').format(self.extra_body)
+            msg += (". {}" if self.body else ": {}").format(self.extra_body)
         return msg
 
 
 class RequirementsRatingParseError(RequirementsRatingError):
     exit_code = 11
 
 
@@ -40,21 +40,24 @@
 
 def catch(fn):
     def wrap(*args, **kwargs):
         console = Console(stderr=True)
         try:
             fn(*args, **kwargs)
         except RequirementsRatingMissingReqFile as e:
-            command = sys.argv[0].split('/')[-1]
+            command = sys.argv[0].split("/")[-1]
             console.print(
-                ":exclamation:  Requirements file not found in [bold orange1]{}[/bold orange1]".format(e.directory)
+                ":exclamation:  Requirements file not found in [bold orange1]{}[/bold orange1]".format(
+                    e.directory
+                )
             )
             console.print(
                 ":information:  You can specify the requirements file using "
-                f"\"[bold]{command} analyze-file --req-file [grey53]<requirements_file>[/grey53][/bold]\"",
-                highlight=False
+                f'"[bold]{command} analyze-file --req-file [grey53]<requirements_file>[/grey53][/bold]"',
+                highlight=False,
             )
             sys.exit(e.exit_code)
         except RequirementsRatingError as e:
-            sys.stderr.write('[Error] pip-rating Exception:\n{}\n'.format(e))
+            console.print("[Error] pip-rating Exception:\n{}\n".format(e))
             sys.exit(e.exit_code)
+
     return wrap
```

### Comparing `pip-rating-0.0.1/pip_rating/management.py` & `pip-rating-0.1.0/pip_rating/management.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # -*- coding: utf-8 -*-
 """Console script for pip-rating."""
 import os
 import platform
 import sys
+import warnings
 from pathlib import Path
 from typing import Optional, List
 
 import click
 import requests
 from requests import RequestException
 from rich.console import Console
-from pkg_resources import parse_version
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    from pkg_resources import parse_version
 
 import pip_rating
 from pip_rating import project_name, __version__
 from pip_rating._compat import USER_CACHE_DIR
 from pip_rating.dependencies import Dependencies
 from pip_rating.exceptions import catch
 from pip_rating.req_files import get_req_file_cls, REQ_FILE_CLASSES, find_in_directory
@@ -22,15 +26,17 @@
 from pip_rating.results import Results, FORMATS
 
 
 def is_last_version() -> Optional[bool]:
     try:
         with requests.get(f"https://pypi.org/pypi/{project_name}/json") as response:
             response.raise_for_status()
-            return parse_version(__version__) >= parse_version(response.json()["info"]["version"])
+            return parse_version(__version__) >= parse_version(
+                response.json()["info"]["version"]
+            )
     except RequestException:
         return None
 
 
 @click.group(invoke_without_command=True)
 @click.option("--version", "-v", is_flag=True, help="Show version and exit.")
 @click.pass_context
@@ -42,35 +48,46 @@
 
     If your file is not detected (or you want to parse another file, like your development dependencies)
     you can use the ``analyze-file`` command.
     """
     if version:
         latest_version = is_last_version()
         console = Console()
-        console.print(f"[bold]{project_name}[/bold] [bold green]{__version__}[/bold green]")
         console.print(
-            "  :top_arrow: This is the latest version." if latest_version
-    else f"  :boom: There is a newer version available. Update it using 'pip install -U {project_name}'"
+            f"[bold]{project_name}[/bold] [bold green]{__version__}[/bold green]"
+        )
+        console.print(
+            "  :top_arrow: This is the latest version."
+            if latest_version
+            else f"  :boom: There is a newer version available. Update it using 'pip install -U {project_name}'"
         )
         console.print(f"  :snake: Python version: {sys.version.split()[0]}")
-        console.print(f"  :computer: Platform: [bold blue]{platform.platform()}[/bold blue]")
-        console.print(f"  :package: Installation path: {os.path.dirname(pip_rating.__file__)}")
+        console.print(
+            f"  :computer: Platform: [bold blue]{platform.platform()}[/bold blue]"
+        )
+        console.print(
+            f"  :package: Installation path: {os.path.dirname(pip_rating.__file__)}"
+        )
         console.print(f"  :file_folder: Current path: {os.getcwd()}")
         ctx.exit(0)
     elif ctx.invoked_subcommand is None:
         req_file = find_in_directory(Path.cwd())
-        Console().print(f"Autodetected requirements file: [bold green]{req_file}[/bold green]")
+        Console().print(
+            f"Autodetected requirements file: [bold green]{req_file}[/bold green]"
+        )
         ctx.invoke(analyze_file, file=str(req_file.path))
 
 
 def common_options(function):
     function = click.option(
         "--cache-dir",
         envvar="PIP_CACHE_DIR",
-        type=click.Path(exists=False, file_okay=False, dir_okay=True, resolve_path=True),
+        type=click.Path(
+            exists=False, file_okay=False, dir_okay=True, resolve_path=True
+        ),
         default=os.path.join(USER_CACHE_DIR, "wheels", "pip-rating"),
         help="Use a custom cache dir.",
     )(function)
     function = click.option(
         "--index-url",
         # envvar="PIP_INDEX_URL",  # let pip discover
         # default="https://pypi.org/simple",
@@ -86,50 +103,101 @@
         "-f",
         "format_name",
         type=click.Choice(FORMATS),
         # envvar="PIP_EXTRA_INDEX_URL",  # let pip discover
         default="text",
         help=f"Output format. Supported formats: {', '.join(FORMATS)}. By default it uses 'text'.",
     )(function)
+    function = click.option(
+        "--ignore-package",
+        "ignore_packages",
+        type=str,
+        multiple=True,
+        help="Ignore a package. You can use this option multiple times.",
+    )(function)
     return function
 
 
 @cli.command()
-@click.argument('file', type=click.Path(exists=True, dir_okay=False))
-@click.option('--file-type', type=click.Choice(list(REQ_FILE_CLASSES.keys())), default=None)
+@click.argument("file", type=click.Path(exists=True, dir_okay=False))
+@click.option(
+    "--file-type", type=click.Choice(list(REQ_FILE_CLASSES.keys())), default=None
+)
 @common_options
-def analyze_file(file: str, file_type: Optional[str], cache_dir: str, index_url: str, extra_index_url: str,
-                 format_name: str):
+def analyze_file(
+    file: str,
+    file_type: Optional[str],
+    cache_dir: str,
+    index_url: str,
+    extra_index_url: str,
+    format_name: str,
+    ignore_packages: List[str],
+):
     """Analyze a requirements file. A requirements file is required as argument. By default, it tries to detect the
     type of the file, but you can force it using the ``--file-type`` option. The supported file types are:
     *requirements.txt, requirements.in, setup.py, setup.cfg, Pipfile and pyproject.toml*.
     """
     results = Results()
     file = Path(file)
     if file_type is None:
         req_file_cls = get_req_file_cls(file)
     else:
         req_file_cls = REQ_FILE_CLASSES[file_type]
     results.status.update(f"Read requirements file [bold green]{file}[/bold green]")
-    dependencies = Dependencies(results, req_file_cls(file), cache_dir, index_url, extra_index_url)
+    dependencies = Dependencies(
+        results,
+        req_file_cls(file),
+        cache_dir,
+        index_url,
+        extra_index_url,
+        ignore_packages=ignore_packages,
+    )
     results.show_results(dependencies, format_name)
 
 
 @cli.command()
-@click.argument('package_names', nargs=-1, required=True)
+@click.argument("package_names", nargs=-1, required=True)
 @common_options
-def analyze_package(package_names: List[str], cache_dir: str, index_url: str, extra_index_url: str, format_name: str):
+def analyze_package(
+    package_names: List[str],
+    cache_dir: str,
+    index_url: str,
+    extra_index_url: str,
+    format_name: str,
+    ignore_packages: List[str],
+):
     """Analyze a package. A package name is required as argument. The syntax is the same as pip install. For example:
     ``Django==4.2.3``. If only one package is specified, it will show their dependencies in detail.
     """
     results = Results()
     req_file = PackageList(package_names)
-    dependencies = Dependencies(results, req_file, cache_dir, index_url, extra_index_url)
+    dependencies = Dependencies(
+        results,
+        req_file,
+        cache_dir,
+        index_url,
+        extra_index_url,
+        ignore_packages=ignore_packages,
+    )
     if len(package_names) == 1:
         nodes = dependencies.dependencies_tree.children[0].children
-        packages = PackageList(list(package_names) + [f"{node.name}=={node.version}" for node in nodes])
-        dependencies = Dependencies(results, packages, cache_dir, index_url, extra_index_url)
+        packages = PackageList(
+            list(package_names) + [f"{node.name}=={node.version}" for node in nodes]
+        )
+        dependencies = Dependencies(
+            results,
+            packages,
+            cache_dir,
+            index_url,
+            extra_index_url,
+            ignore_packages=ignore_packages,
+        )
     results.show_results(dependencies, format_name)
 
 
-if __name__ == '__main__':
+def manage():
+    """Entry point for the console script."""
     catch(cli)()
+
+
+if __name__ == "__main__":
+    manage()
```

### Comparing `pip-rating-0.0.1/pip_rating/packages.py` & `pip-rating-0.1.0/pip_rating/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     dependencies: List["PackageJson"]
 
 
 class Package:
     nodes: Set[Node]
 
     def __init__(self, dependencies: "Dependencies", name: str):
-        self.name = name
         self.dependencies = dependencies
+        self.name = name
         self.nodes = set()
 
     @cached_property
     def first_node(self) -> Node:
         return next(iter(sorted(self.nodes, key=lambda n: n.depth)))
 
     @property
@@ -56,43 +56,52 @@
     def get_audit(self, node: Node) -> "Audit":
         return Audit(self.name, node.version)
 
     @cached_property
     def rating(self) -> "PackageRating":
         return PackageRating(self)
 
-    def get_node_from_parent(self, from_package: Optional["Package"]) -> Optional["Node"]:
+    def get_node_from_parent(
+        self, from_package: Optional["Package"] = None
+    ) -> Optional["Node"]:
         """Given this package and a parent package, return the node in the package that
         is a descendant of the parent package
         """
         if from_package is None:
             return self.first_node
         for node in self.nodes:
             for parent_node in from_package.nodes:
                 if node in parent_node.descendants:
                     return node
 
     def get_descendant_packages(self) -> Iterator["Package"]:
         for descendant in self.first_node.descendants:
-            yield self.dependencies.add_node_package(descendant)
+            package = self.dependencies.add_node_package(descendant)
+            if package:
+                yield package
 
     def get_child_packages(self) -> Iterator["Package"]:
         for child in self.first_node.children:
-            yield self.dependencies.add_node_package(child)
+            package = self.dependencies.add_node_package(child)
+            if package:
+                yield package
 
     def add_node(self, node: Node):
         self.nodes.add(node)
 
     def as_json(self, from_package: Optional["Package"] = None) -> PackageJson:
         node = self.get_node_from_parent(from_package)
         return {
             "name": self.name,
             "version": node.version,
             "sourcerank_breakdown": self.sourcerank.breakdown,
             "pypi_package": self.pypi.package,
             "audit_vulnerabilities": self.get_audit(node).vulnerabilities,
             "rating": self.rating.as_json(from_package),
-            "dependencies": [self.dependencies.packages[subnode.name].as_json(self) for subnode in node.children],
+            "dependencies": [
+                self.dependencies.packages[subnode.name].as_json(self)
+                for subnode in node.children
+            ],
         }
 
     def __repr__(self) -> str:
         return f"<Package {self.name}>"
```

### Comparing `pip-rating-0.0.1/pip_rating/rating.py` & `pip-rating-0.1.0/pip_rating/rating.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 from functools import cached_property
 from pathlib import Path
 from typing import TYPE_CHECKING, TypedDict, Optional, Union, List, Tuple, Dict
 
 from platformdirs import user_cache_dir
-from requests import __version__
+from pip_rating import __version__
 from pip_rating._compat import cache
 from pip_rating.sources.audit import Vulnerability
 
 from pip_rating.sources.sourcerank import SourceRankBreakdown
 
 if TYPE_CHECKING:
     from pip_rating.packages import Package
@@ -77,67 +77,73 @@
     def __init__(self, max_score: int, current_score: int = 0):
         self.max_score = max_score
         self.current_score = current_score
 
     def __add__(self, other: ScoreBase):
         if isinstance(other, ScoreValue):
             score = self.current_score + int(other)
-            self.current_score = max(self.max_score, score)
+            self.current_score = min(self.max_score, score)
         if isinstance(other, Max) and other.max_score < self.max_score:
-            other.current_score = self.current_score
+            other.current_score += self.current_score
             return other
+        if isinstance(other, Max) and other.max_score > self.max_score:
+            self.current_score += other.current_score
+            return self
         return self
 
     def __int__(self) -> int:
-        return self.max_score
+        return min(self.current_score, self.max_score)
 
     def __str__(self):
         return f"Max({self.max_score})"
 
     def __repr__(self) -> str:
         return f"<Max current: {self.current_score} max: {self.max_score}>"
 
 
 class BreakdownBase:
     breakdown_key: str
 
     def get_score(self, package_rating: "PackageRating") -> ScoreBase:
         raise NotImplementedError
 
-    def get_breakdown_value(self, package_rating: "PackageRating") -> Union[int, bool, str]:
+    def get_breakdown_value(
+        self, package_rating: "PackageRating"
+    ) -> Union[int, bool, str]:
         value = package_rating.params
         for subkey in self.breakdown_key.split("."):
             value = value[subkey]
         return value
 
 
 class PackageBreakdown(BreakdownBase):
     def __init__(self, breakdown_key: str, score: Optional[Union[int, Max]] = None):
         self.breakdown_key = breakdown_key
         self._score = score
 
-    def get_score(self, package_rating: "PackageRating") -> ScoreBase:
+    def get_score(self, package_rating: "PackageRating") -> ScoreValue:
         value = self.get_breakdown_value(package_rating)
         if value and self._score:
             return ScoreValue(self._score)
         if not value and self._score:
-            return ScoreValue(0)
+            return ScoreValue(0)  # the default is 0
         if isinstance(value, bool):
             raise ValueError("Cannot calculate score for boolean value")
         return ScoreValue(value)
 
 
 class DateBreakdown(BreakdownBase):
-
-    def __init__(self, breakdown_key: str, scores: Dict[datetime.timedelta, int], default: int):
+    def __init__(
+        self, breakdown_key: str, scores: Dict[datetime.timedelta, int], default: int
+    ):
         self.breakdown_key = breakdown_key
         self.scores = scores
         self.default = default
 
-    def get_score(self, package_rating: "PackageRating") -> ScoreBase:
+    def get_score(self, package_rating: "PackageRating") -> ScoreValue:
         iso_dt = self.get_breakdown_value(package_rating)
         if not iso_dt:
             return ScoreValue(0)
         dt = datetime.datetime.fromisoformat(iso_dt)
         dt_delta = datetime.datetime.now(datetime.timezone.utc) - dt
         for delta, score in self.scores.items():
             if dt_delta < delta:
@@ -171,58 +177,63 @@
             datetime.timedelta(days=30 * 4): 4,
             datetime.timedelta(days=30 * 6): 3,
             datetime.timedelta(days=365): 2,
             datetime.timedelta(days=365 + (30 * 6)): 1,
             datetime.timedelta(days=365 * 3): 0,
             datetime.timedelta(days=365 * 4): -2,
         },
-        default=-4
+        default=-4,
     ),
     DateBreakdown(
         "pypi_package.first_upload_iso_dt",
         {
             datetime.timedelta(days=15): Max(0),
             datetime.timedelta(days=30): -3,
             datetime.timedelta(days=60): -2,
             datetime.timedelta(days=90): -1,
             datetime.timedelta(days=180): 0,
             datetime.timedelta(days=360): 1,
             datetime.timedelta(days=360 * 2): 2,
             datetime.timedelta(days=360 * 4): 3,
         },
-        default=4
+        default=4,
     ),
     NullBoolBreakdown(
         "sourcecode_page.package_in_readme",
-        {True: ScoreValue(1), False: Max(0), None: ScoreValue(0)}
+        {True: ScoreValue(1), False: Max(0), None: ScoreValue(0)},
     ),
 ]
 
 
 class PackageRatingJson(TypedDict):
     rating_score: int
     global_rating_score: int
     vulnerabilities: List[Vulnerability]
     params: PackageRatingParams
 
 
 class PackageRating:
-    def __init__(self, package: "Package", params: Optional[PackageRatingParams] = None):
+    def __init__(
+        self, package: "Package", params: Optional[PackageRatingParams] = None
+    ):
         self.package = package
         if not params and self.is_cache_expired:
             params = self.get_params_from_package()
             self.save_to_cache()
         elif not params:
             params = self.get_params_from_cache()
         self.params: PackageRatingParams = params
 
     @property
     def is_cache_expired(self) -> bool:
-        return not self.cache_path.exists() or \
-            self.cache_path.stat().st_mtime < (datetime.datetime.now() - MAX_CACHE_AGE).timestamp()
+        return (
+            not self.cache_path.exists()
+            or self.cache_path.stat().st_mtime
+            < (datetime.datetime.now() - MAX_CACHE_AGE).timestamp()
+        )
 
     @property
     def cache_path(self) -> Path:
         return RATING_CACHE_DIR / f"{self.package.name}.json"
 
     def get_from_cache(self) -> Optional[PackageRatingCache]:
         with open(self.cache_path) as file:
@@ -254,15 +265,15 @@
             "sourcerank_breakdown": self.package.sourcerank.breakdown,
             "pypi_package": {
                 "latest_upload_iso_dt": self.package.pypi.latest_upload_iso_dt,
                 "first_upload_iso_dt": self.package.pypi.first_upload_iso_dt,
             },
             "sourcecode_page": {
                 "package_in_readme": self.package.sourcecode_page.package_in_readme,
-            }
+            },
         }
 
     @cached_property
     def breakdown_scores(self) -> List[Tuple[str, ScoreBase]]:
         return [
             (breakdown.breakdown_key, breakdown.get_score(self))
             for breakdown in BREAKDOWN_SCORES
@@ -280,36 +291,41 @@
         scores = dict(self.breakdown_scores).values()
         value = ScoreValue(0)
         for score in scores:
             value += score
         return int(value)
 
     @cache
-    def get_vulnerabilities(self, from_package: Optional["Package"] = None) -> List["Vulnerability"]:
+    def get_vulnerabilities(
+        self, from_package: Optional["Package"] = None
+    ) -> List["Vulnerability"]:
         node = None
         if from_package is not None:
             node = self.package.get_node_from_parent(from_package)
         elif from_package is None:
             node = self.package.first_node
         # get_audit requires a node, so we only call it if we have one and this is used
         # instead of the package's own rating score
         if node is not None:
             return self.package.get_audit(node).vulnerabilities
         return []
 
     def get_rating_score(self, from_package: Optional["Package"] = None) -> int:
-        self.package.dependencies.results.analizing_package(self.package.name, self.package.dependencies.total_size)
+        self.package.dependencies.results.analizing_package(
+            self.package.name, self.package.dependencies.total_size
+        )
         if len(self.get_vulnerabilities(from_package)):
             return 0
         return self.rating_score
 
     def get_global_rating_score(self, from_package: Optional["Optional"] = None) -> int:
         return min(
-            [self.get_rating_score(from_package)] + list(dict(self.descendant_rating_scores).values()),
-            default=0
+            [self.get_rating_score(from_package)]
+            + list(dict(self.descendant_rating_scores).values()),
+            default=0,
         )
 
     def as_json(self, from_package: Optional["Package"] = None) -> PackageRatingJson:
         return {
             "rating_score": self.get_rating_score(from_package),
             "global_rating_score": self.get_global_rating_score(from_package),
             "vulnerabilities": self.get_vulnerabilities(from_package),
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/__init__.py` & `pip-rating-0.1.0/pip_rating/req_files/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from pathlib import Path
 from typing import Union, Type
 
-from pip_rating.exceptions import RequirementsRatingInvalidFile, RequirementsRatingMissingReqFile
+from pip_rating.exceptions import (
+    RequirementsRatingInvalidFile,
+    RequirementsRatingMissingReqFile,
+)
 from pip_rating.req_files.base import ReqFileBase
 from pip_rating.req_files.pipfile import PipfileReqFile
 from pip_rating.req_files.pyproject import PyprojectReqFile
 from pip_rating.req_files.requirements import RequirementsReqFile
 from pip_rating.req_files.setupcfg import SetupcfgReqFile
 from pip_rating.req_files.setuppy import SetuppyReqFile
 
@@ -20,15 +23,17 @@
 
 
 def get_req_file_cls(path: Union[str, Path]) -> Type[ReqFileBase]:
     """Get the requirement file class for the given path."""
     for req_file_cls in REQ_FILE_CLASSES.values():
         if req_file_cls.is_valid(path):
             return req_file_cls
-    raise RequirementsRatingInvalidFile(f"Could not find requirement file class for {path}")
+    raise RequirementsRatingInvalidFile(
+        f"Could not find requirement file class for {path}"
+    )
 
 
 def find_in_directory(directory: Union[str, Path]) -> ReqFileBase:
     """Find requirement file in the given directory."""
     if isinstance(directory, str):
         directory = Path(directory)
     for req_file_cls in REQ_FILE_CLASSES.values():
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/base.py` & `pip-rating-0.1.0/pip_rating/req_files/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union, List, Optional
 
 from pkg_resources import Requirement
 
 
 class ReqFileBase(list):
     """Base class for requirement files."""
+
     def __init__(self, path: Union[str, Path]):
         """Initialize the requirement file."""
         if isinstance(path, str):
             path = Path(path)
         self.path = path
         if not self.path.exists():
             raise IOError(f"File {self.path} does not exist")
@@ -29,15 +30,17 @@
         """Get the dependencies from the file."""
         raise NotImplementedError
 
     def __contains__(self, item: str) -> bool:
         req = Requirement(item)
         for package in self:
             package = Requirement(package)
-            if (not req.specifier and package.name.lower() == req.name.lower()) or package == req:
+            if (
+                not req.specifier and package.name.lower() == req.name.lower()
+            ) or package == req:
                 return True
         return False
 
     def __str__(self) -> str:
         return self.path.name
 
     def __repr__(self) -> str:
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/package_list.py` & `pip-rating-0.1.0/pip_rating/req_files/package_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
     @classmethod
     def is_valid(cls, path: Union[str, Path]) -> bool:
         """Check if the given path is a valid requirement file."""
         raise NotImplementedError
 
     def __str__(self) -> str:
-        return str(self)
+        return str(list(self))
 
     def __repr__(self) -> str:
         return f"<ReqFile ({len(self)})>"
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/pipfile.py` & `pip-rating-0.1.0/pip_rating/req_files/pipfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pipfile import Pipfile
 
 from pip_rating.req_files import ReqFileBase
 
 
 class PipfileReqFile(ReqFileBase):
     """Parse packages from Pipfile file."""
+
     @classmethod
     def find_in_directory(cls, directory: Union[str, Path]) -> "PipfileReqFile":
         """Find setup.cfg in the given directory."""
         if isinstance(directory, str):
             directory = Path(directory)
         path = directory / "Pipfile"
         if path.exists():
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/pyproject.py` & `pip-rating-0.1.0/pip_rating/req_files/pyproject.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,43 +14,49 @@
     if version is None:
         return ""
     if isinstance(version, dict):
         version_value = version.get("version")
         output = poetry_version(version_value)
         markers = []
         if version.get("python"):
-            python_version = poetry_version(version['python']).split(",")
-            python_version = [re.sub(r"(\d.*)", r"'\1'", version.strip()) for version in python_version]
-            markers.append(" and ".join(f"python_version {version}" for version in python_version))
+            python_version = poetry_version(version["python"]).split(",")
+            python_version = [
+                re.sub(r"(\d.*)", r"'\1'", version.strip())
+                for version in python_version
+            ]
+            markers.append(
+                " and ".join(f"python_version {version}" for version in python_version)
+            )
         if version.get("markers"):
-            markers.append(version['markers'])
+            markers.append(version["markers"])
         if version.get("platform"):
             markers.append(f"platform_system=='{version['platform']}'")
         if markers:
             output += f" ; {' and '.join(markers)}"
         return output
     if version.startswith("^"):
         version = Version(version[1:])
-        if version.major:
+        if version.major or version.base_version == "0":
             return f">={version},<{version.major + 1}.0.0"
-        elif version.minor:
+        elif version.minor or version.base_version == "0.0":
             return f">={version},<{version.major}.{version.minor + 1}.0"
         elif version.micro:
             return f">={version},<{version.major}.{version.minor}.{version.micro + 1}"
         else:
             raise RequirementsRatingParseError(f"Invalid version '{version}'")
-    if version and (version[0].isdigit() or version[0].startswith('*.')):
+    if version and (version[0].isdigit() or version[0] == "*"):
         return f"=={version}"
     if version and version[0] in "=<>!":
         return version
     raise RequirementsRatingParseError(f"Invalid version '{version}'")
 
 
 class PyprojectReqFile(ReqFileBase):
     """Parse dependencies from pyproject.toml file."""
+
     @classmethod
     def find_in_directory(cls, directory: Union[str, Path]) -> "PyprojectReqFile":
         """Find pyproject.toml in the given directory."""
         if isinstance(directory, str):
             directory = Path(directory)
         path = directory / "pyproject.toml"
         if path.exists():
@@ -67,14 +73,19 @@
         """Get the dependencies from the pyproject.toml file."""
         with open(str(self.path), "rb") as file:
             data = tomllib.load(file)
         sentinel = object()
         project_dependencies = data.get("project", {}).get("dependencies") or sentinel
         if project_dependencies is not sentinel:
             return project_dependencies
-        poetry_dependencies = data.get("tool", {}).get("poetry", {}).get("dependencies", {})
+        poetry_dependencies = (
+            data.get("tool", {}).get("poetry", {}).get("dependencies", {}) or sentinel
+        )
         if poetry_dependencies is not sentinel:
             return [
                 f"{name}{poetry_version(version)}"
-                for name, version in poetry_dependencies.items() if name != "python"
+                for name, version in poetry_dependencies.items()
+                if name != "python"
             ]
-        raise RequirementsRatingParseError(f"Dependencies not found in the file '{self.path}'.")
+        raise RequirementsRatingParseError(
+            f"Dependencies not found in the file '{self.path}'."
+        )
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/requirements.py` & `pip-rating-0.1.0/pip_rating/req_files/requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,43 @@
 from typing import Union, List, Optional
 
 from pip_rating.req_files.base import ReqFileBase
 
 
 COMMENT_REGEX = re.compile(r"(#.*)")
 REQUIREMENTS_FILES = [
-    "requirements.in", "requirements.txt",
-    re.compile(r".*requirements.*\.in"), re.compile(r".*requirements.*\.txt")
+    "requirements.in",
+    "requirements.txt",
+    re.compile(r".*requirements.*\.in"),
+    re.compile(r".*requirements.*\.txt"),
 ]
 
 
 class RequirementsReqFile(ReqFileBase):
     """Requirements requirement file."""
+
     @classmethod
     def find_in_directory(cls, directory: Union[str, Path]) -> Optional["ReqFileBase"]:
         """Find requirement file in the given directory."""
         if isinstance(directory, str):
             directory = Path(directory)
         for requirements_file in REQUIREMENTS_FILES:
-            if isinstance(requirements_file, str) and (directory / requirements_file).exists():
+            if (
+                isinstance(requirements_file, str)
+                and (directory / requirements_file).exists()
+            ):
                 return cls(directory / requirements_file)
             if isinstance(requirements_file, re.Pattern):
-                requirements_file = next(filter(lambda file: requirements_file.match(str(file)),
-                                                directory.iterdir()), None)
+                requirements_file = next(
+                    filter(
+                        lambda file: requirements_file.match(str(file)),
+                        directory.iterdir(),
+                    ),
+                    None,
+                )
                 if requirements_file:
                     return cls(requirements_file)
 
     @classmethod
     def is_valid(cls, path: Union[str, Path]) -> bool:
         """Check if the given path is a valid requirement file."""
         if isinstance(path, str):
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/setupcfg.py` & `pip-rating-0.1.0/pip_rating/req_files/setupcfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from setuptools.config.setupcfg import read_configuration
 
 from pip_rating.req_files import ReqFileBase
 
 
 class SetupcfgReqFile(ReqFileBase):
     """Parse install_requires from Setup.cfg file."""
+
     @classmethod
     def find_in_directory(cls, directory: Union[str, Path]) -> "SetupcfgReqFile":
         """Find setup.cfg in the given directory."""
         if isinstance(directory, str):
             directory = Path(directory)
         path = directory / "setup.cfg"
         if path.exists():
```

### Comparing `pip-rating-0.0.1/pip_rating/req_files/setuppy.py` & `pip-rating-0.1.0/pip_rating/req_files/setuppy.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pip_rating.exceptions import RequirementsRatingParseError
 from pip_rating.req_files import ReqFileBase
 
 
 class SetuppyReqFile(ReqFileBase):
     """Parse install_requires from Setup.py file."""
+
     @classmethod
     def find_in_directory(cls, directory: Union[str, Path]) -> "SetuppyReqFile":
         """Find setup.py in the given directory."""
         if isinstance(directory, str):
             directory = Path(directory)
         path = directory / "setup.py"
         if path.exists():
@@ -22,22 +23,26 @@
         """Check if the given path is a valid setup.py file."""
         if isinstance(path, str):
             path = Path(path)
         return path.exists() and path.name == "setup.py"
 
     def get_dependencies(self) -> List[str]:
         """Get the dependencies from the setup.py file."""
-        with patch("setuptools.setup") as mock_setuptools_setup, \
-             patch("distutils.core.setup") as mock_distutils_setup, \
-             open(self.path, "r") as file:
+        with patch("setuptools.setup") as mock_setuptools_setup, patch(
+            "distutils.core.setup"
+        ) as mock_distutils_setup, open(self.path, "r") as file:
             try:
                 exec(file.read())
             except Exception as e:
-                raise RequirementsRatingParseError(f"Error executing '{self.path}' to parse dependencies.") from e
+                raise RequirementsRatingParseError(
+                    f"Error executing '{self.path}' to parse dependencies."
+                ) from e
             mock_setup = None
             if mock_setuptools_setup.call_count:
                 mock_setup = mock_setuptools_setup
             elif mock_distutils_setup.call_count:
                 mock_setup = mock_distutils_setup
             if mock_setup is None:
-                raise RequirementsRatingParseError(f"setup() function not called in '{self.path}'.")
+                raise RequirementsRatingParseError(
+                    f"setup() function not called in '{self.path}'."
+                )
             return mock_setup.mock_calls[0].kwargs.get("install_requires") or []
```

### Comparing `pip-rating-0.0.1/pip_rating/results.py` & `pip-rating-0.1.0/pip_rating/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import datetime
 import json
-from typing import Optional, TYPE_CHECKING, Union, TypedDict, List
+from typing import Optional, TYPE_CHECKING, Union, TypedDict, List, Any
 
-from requests import __version__
+from pip_rating import __version__
 from rich.console import Console
-from rich.progress import Progress, TaskID, TaskProgressColumn, TextColumn, BarColumn, TimeRemainingColumn
+from rich.progress import (
+    Progress,
+    TaskID,
+    TaskProgressColumn,
+    TextColumn,
+    BarColumn,
+    TimeRemainingColumn,
+)
 from rich.status import Status
 from rich.table import Table
 from rich.tree import Tree
 
 
 if TYPE_CHECKING:
     from pip_rating.packages import Package
@@ -32,31 +39,41 @@
 def colorize_rating(score: Union["ScoreBase", int]) -> "RatingLetter":
     """Colorize the rating."""
     for rating_letter in RATING_LETTERS:
         if max(0, int(score)) >= rating_letter.score:
             return rating_letter
 
 
-def colorize_rating_package(package: "Package", parent_package: Optional["Package"] = None) -> str:
+def colorize_rating_package(
+    package: "Package", parent_package: Optional["Package"] = None
+) -> str:
     """Colorize the rating of the package."""
     colorized_rating = colorize_rating(package.rating.get_rating_score(parent_package))
-    colorized_global_rating = colorize_rating(package.rating.get_global_rating_score(parent_package))
+    colorized_global_rating = colorize_rating(
+        package.rating.get_global_rating_score(parent_package)
+    )
     if colorized_rating > colorized_global_rating:
         return f"{colorized_rating} -> {colorized_global_rating}"
     else:
         return f"{colorized_rating}"
 
 
-def add_tree_node(dependencies: "Dependencies", tree: "Tree", package: "Package",
-                  parent_package: Optional["Package"] = None):
+def add_tree_node(
+    dependencies: "Dependencies",
+    tree: "Tree",
+    package: "Package",
+    parent_package: Optional["Package"] = None,
+):
     if parent_package is None:
         tree = tree.add(
             f"[bold]:package: {package.name} ({colorize_rating_package(package)})[/bold]"
         )
     for child in package.get_node_from_parent(parent_package).children:
+        if child.name not in dependencies.packages:
+            continue
         subpackage = dependencies.packages[child.name]
         subtree_package = tree.add(
             f"[bold]{child.name} ({colorize_rating_package(subpackage, package)})[/bold]"
         )
         add_tree_node(dependencies, subtree_package, subpackage, package)
 
 
@@ -113,14 +130,15 @@
     global_rating_letter: str
     global_rating_score: int
     packages: List[dict]
 
 
 class Results:
     """Print pip-ratings results to the terminal."""
+
     _status: Optional[Status]
     progress: Optional[Progress]
     task: Optional[TaskID]
 
     def __init__(self):
         self.console = Console()
         self.console.status("[bold green]Loading...")
@@ -131,15 +149,15 @@
     @property
     def status(self) -> Optional[Status]:
         if not self._status:
             self._status = self.console.status("[bold green]Waiting...")
             self._status.start()
         return self._status
 
-    def processing_package(self, package):
+    def processing_package(self, package: Any):
         self.status.update(f"Processing package [bold green]{package}[/bold green]...")
 
     def analizing_package(self, package: str, total: int):
         if self._status:
             self._status.stop()
         if not self.progress:
             self.progress = Progress(
@@ -150,29 +168,32 @@
                 console=self.console,
             )
             self.task = self.progress.add_task("Analizing packages...", total=total)
             self.progress.start()
         spaces = " " * (MIN_PACKAGE_NAME - len(package))
         self.progress.update(
             self.task,
-            description=f"Analizing package [bold blue]{package}[/bold blue]..." + spaces,
+            description=f"Analizing package [bold blue]{package}[/bold blue]..."
+            + spaces,
             advance=1,
             refresh=True,
         )
 
     def get_global_rating_score(self, dependencies: "Dependencies") -> int:
         global_rating_score = dependencies.get_global_rating_score()
         if self.progress:
-            self.progress.update(self.task, description="[bold green]Analyzed all packages[/bold green]", refresh=True)
+            self.progress.update(
+                self.task,
+                description="[bold green]Analyzed all packages[/bold green]",
+                refresh=True,
+            )
             self.progress.stop()
         return global_rating_score
 
     def show_results(self, dependencies: "Dependencies", format_name: str = "text"):
-        if format_name not in FORMATS:
-            raise ValueError(f"Format name must be one of {FORMATS}")
         if format_name == "text":
             self.show_packages_results(dependencies)
         elif format_name == "tree":
             self.show_tree_results(dependencies)
         elif format_name == "json":
             self.show_json_results(dependencies)
         elif format_name == "only-rating":
@@ -181,34 +202,50 @@
             raise ValueError(f"Format name must be one of {', '.join(FORMATS)}")
 
     def show_packages_results(self, dependencies: "Dependencies"):
         global_rating_score = self.get_global_rating_score(dependencies)
         for package in dependencies.packages.values():
             if package.name not in dependencies.req_file:
                 continue
-            global_rating_score = package.rating.get_global_rating_score()
-            global_rating_score_letter = colorize_rating(global_rating_score)
+            package_global_rating_score = package.rating.get_global_rating_score()
+            package_global_rating_score_letter = colorize_rating(
+                package_global_rating_score
+            )
             rating_score_letter = colorize_rating(package.rating.get_rating_score())
             vulnerabilities = []
-            if not global_rating_score:
+            if not package_global_rating_score:
                 vulnerabilities = package.rating.get_vulnerabilities()
-            if vulnerabilities or global_rating_score_letter >= rating_score_letter:
-                print_score = f"{global_rating_score_letter}"
+            if (
+                vulnerabilities
+                or package_global_rating_score_letter >= rating_score_letter
+            ):
+                print_score = f"{package_global_rating_score_letter}"
             else:
-                print_score = f"{rating_score_letter} -> {global_rating_score_letter}"
+                print_score = (
+                    f"{rating_score_letter} -> {package_global_rating_score_letter}"
+                )
             self.console.print(
-                f":package: Package [bold blue]{package.name}[/bold blue]: " + print_score
+                f":package: Package [bold blue]{package.name}[/bold blue]: "
+                + print_score
             )
             for key, value in package.rating.breakdown_scores:
-                key = key.split(".")[-1].replace("iso_dt", "").replace("_", " ").capitalize()
-                self.console.print(f"  :black_medium-small_square: {key}: {colorize_score(value)}")
-            if global_rating_score < package.rating.rating_score:
+                key = (
+                    key.split(".")[-1]
+                    .replace("iso_dt", "")
+                    .replace("_", " ")
+                    .capitalize()
+                )
+                self.console.print(
+                    f"  :black_medium-small_square: {key}: {colorize_score(value)}"
+                )
+            if package_global_rating_score < package.rating.rating_score:
                 low_rating_dependences = [
-                    f'{pkg.name} ({colorize_rating(score)})' for pkg, score
-                    in package.rating.descendant_rating_scores if colorize_rating(score) < rating_score_letter
+                    f"{pkg.name} ({colorize_rating(score)})"
+                    for pkg, score in package.rating.descendant_rating_scores
+                    if colorize_rating(score) < rating_score_letter
                 ]
                 self.console.print(
                     f"  :arrow_lower_right: Low rating dependencies: {', '.join(low_rating_dependences)}"
                 )
             if vulnerabilities:
                 self.console.print(
                     f"  :biohazard: Vulnerabilities found: [bold grey53]"
@@ -218,32 +255,40 @@
         self.console.print("")
         table = Table(show_header=False)
         table.add_row(f"Global rating score: {colorize_rating(global_rating_score)}")
         self.console.print(table)
 
     def show_tree_results(self, dependencies: "Dependencies"):
         global_rating_score = self.get_global_rating_score(dependencies)
-        req_file_name = str(dependencies.req_file) if dependencies.req_file else "Packages list"
-        tree = Tree(f"[bold]{req_file_name} ({colorize_rating(global_rating_score)})[/bold]")
+        req_file_name = (
+            str(dependencies.req_file) if dependencies.req_file else "Packages list"
+        )
+        tree = Tree(
+            f"[bold]{req_file_name} ({colorize_rating(global_rating_score)})[/bold]"
+        )
         for package in dependencies.packages.values():
             if package.name not in dependencies.req_file:
                 continue
             add_tree_node(dependencies, tree, package)
         self.console.print(tree)
 
     def get_json_results(self, dependencies: "Dependencies"):
         global_rating_score = self.get_global_rating_score(dependencies)
-        packages = [package for package in dependencies.packages.values() if package.name in dependencies.req_file]
+        packages = [
+            package
+            for package in dependencies.packages.values()
+            if package.name in dependencies.req_file
+        ]
         return {
             "requirements": dependencies.req_file,
             "updated_at": datetime.datetime.now().isoformat(),
             "schema_version": __version__,
             "global_rating_letter": colorize_rating(global_rating_score).letter,
             "global_rating_score": global_rating_score,
-            "packages": [package.as_json() for package in packages]
+            "packages": [package.as_json() for package in packages],
         }
 
     def show_json_results(self, dependencies: "Dependencies"):
         self.console = Console(stderr=True)
         results = self.get_json_results(dependencies)
         print(json.dumps(results, indent=4, sort_keys=False))
```

### Comparing `pip-rating-0.0.1/pip_rating/sources/audit.py` & `pip-rating-0.1.0/pip_rating/sources/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 def vulns_to_dict(vulnerabilities: List[VulnerabilityResult]) -> List[Vulnerability]:
     return [
         {
             "id": vulnerability.id,
             "description": vulnerability.description,
             "fix_versions": [str(version) for version in vulnerability.fix_versions],
             "aliases": list(vulnerability.aliases),
-            "published_iso_dt": vulnerability.published.isoformat() if vulnerability.published else None,
+            "published_iso_dt": vulnerability.published.isoformat()
+            if vulnerability.published
+            else None,
         }
         for vulnerability in vulnerabilities
     ]
 
 
 class Audit(SourceBase):
     """Audit source"""
@@ -40,15 +42,18 @@
 
     def __init__(self, package_name: str, version: str):
         self.version = version
         super().__init__(package_name)
 
     @property
     def cache_file(self) -> Path:
-        return self.cache_dir / f"{self.package_name}_{sha1(self.version.encode('utf-8')).hexdigest()}.json"
+        return (
+            self.cache_dir
+            / f"{self.package_name}_{sha1(self.version.encode('utf-8')).hexdigest()}.json"
+        )
 
     @cached_property
     def vulnerabilities(self) -> List[Vulnerability]:
         if not self.is_cache_expired:
             cache = self.get_from_cache()
         else:
             cache = self.save_to_cache()
```

### Comparing `pip-rating-0.0.1/pip_rating/sources/base.py` & `pip-rating-0.1.0/pip_rating/sources/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 from platformdirs import user_cache_dir
 
 
 class SourceBase:
     """Base class for all sources"""
+
     source_name: str
     max_cache_age = datetime.timedelta(days=7)
 
     def __init__(self, package_name: str):
         self.package_name = package_name
 
     @property
@@ -21,16 +22,19 @@
 
     @property
     def cache_file(self) -> Path:
         return self.cache_dir / f"{self.package_name}.json"
 
     @cached_property
     def is_cache_expired(self) -> bool:
-        return not self.cache_file.exists() or \
-            self.cache_file.stat().st_mtime < (datetime.datetime.now() - self.max_cache_age).timestamp()
+        return (
+            not self.cache_file.exists()
+            or self.cache_file.stat().st_mtime
+            < (datetime.datetime.now() - self.max_cache_age).timestamp()
+        )
 
     def get_from_cache(self) -> dict:
         with open(self.cache_file) as file:
             return json.load(file)
 
     def get_cache_data(self) -> dict:
         raise NotImplementedError
```

### Comparing `pip-rating-0.0.1/pip_rating/sources/pypi.py` & `pip-rating-0.1.0/pip_rating/sources/pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import datetime
 from functools import cached_property
 from itertools import chain
-from typing import TypedDict, Optional, List
+from typing import TypedDict, Optional, List, Dict
 
 import requests
 
 from pip_rating.sources.base import SourceBase
 
 URL = "https://pypi.org/pypi/{package_name}/json"
 
 
 class PyPackageInfo(TypedDict):
     author: str
     author_email: str
     bugtrack_url: str
-    classifiers: list[str]
+    classifiers: List[str]
     description: str
     description_content_type: str
     docs_url: str
     download_url: str
-    downloads: dict[str, int]
+    downloads: Dict[str, int]
     home_page: str
     keywords: str
     license: str
     maintainer: str
     maintainer_email: str
     name: str
     package_url: str
     platform: Optional[str]
     project_url: str
-    project_urls: dict[str, str]
+    project_urls: Dict[str, str]
     release_url: str
-    requires_dist: list[str]
+    requires_dist: List[str]
     requires_python: Optional[str]
     summary: str
     version: str
     yanked: bool
     yanked_reason: Optional[str]
 
 
 class PypiPackageReleaseUpload(TypedDict):
     comment_text: str
-    digests: dict[str, str]
+    digests: Dict[str, str]
     downloads: int
     filename: str
     has_sig: bool
     md5_digest: str
     packagetype: str
     python_version: str
     requires_python: Optional[str]
@@ -56,15 +56,15 @@
     yanked: bool
     yanked_reason: Optional[str]
 
 
 class PypiPackage(TypedDict):
     info: PyPackageInfo
     last_serial: int
-    releases: dict[str, list[PypiPackageReleaseUpload]]
+    releases: Dict[str, List[PypiPackageReleaseUpload]]
 
 
 class PypiCacheDict(TypedDict):
     package_name: str
     updated_at: str
     package: PypiPackage
 
@@ -86,18 +86,15 @@
         else:
             cache = self.save_to_cache()
         return cache["package"]
 
     @cached_property
     def uploads(self) -> List[PypiPackageReleaseUpload]:
         uploads = chain(*list(self.package["releases"].values()))
-        return sorted(
-            uploads,
-            key=lambda upload: upload.get("upload_time_iso_8601")
-        )
+        return sorted(uploads, key=lambda upload: upload.get("upload_time_iso_8601"))
 
     @property
     def latest_upload(self) -> Optional[PypiPackageReleaseUpload]:
         return self.uploads[-1] if self.uploads else None
 
     @property
     def first_upload(self) -> Optional[PypiPackageReleaseUpload]:
```

### Comparing `pip-rating-0.0.1/pip_rating/sources/sourcerank.py` & `pip-rating-0.1.0/pip_rating/sources/sourcerank.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,17 @@
         if not self.is_cache_expired:
             cache = self.get_from_cache()
         else:
             cache = self.save_to_cache()
         return cache["breakdown"]
 
     def get_breakdown(self) -> Iterator[Tuple[str, int]]:
-        with requests.get(SOURCERANK_URL.format(package_name=self.package_name)) as response:
+        with requests.get(
+            SOURCERANK_URL.format(package_name=self.package_name)
+        ) as response:
             response.raise_for_status()
             content = response.content
         soup = BeautifulSoup(content, "html.parser")
         for item in soup.find_all("li", "list-group-item"):
             stripped_strings = list(item.stripped_strings)
             if stripped_strings[1] in BREAKDOWN_MAPPING:
                 yield BREAKDOWN_MAPPING[stripped_strings[1]], int(stripped_strings[0])
```

### Comparing `pip-rating-0.0.1/requirements.txt` & `pip-rating-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pip-rating-0.0.1/setup.cfg` & `pip-rating-0.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[bumpversion]
+current_version = 0.1.0
+commit = True
+tag = True
+
 [metadata]
 name = pip-rating
 version = attr: pip_rating.__version__
 description = Check the health of your project's requirements and get a rating for each dependency.
 long-description = file: README.rst
 keywords = pip-rating
 author = Nekmo
@@ -11,15 +16,14 @@
 license = MIT license
 license-files = 
 	LICENSE
 platform = any
 classifiers = 
 	Development Status :: 3 - Alpha
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
@@ -45,29 +49,24 @@
 formats = zip, gztar
 
 [check]
 metadata = True
 restructuredtext = True
 strict = True
 
-[bumpversion]
-current_version = 0.0.1
-commit = True
-tag = True
-
-[bumpversion:file:setup.py]
-search = version='{current_version}'
-replace = version='{new_version}'
-
 [bumpversion:file:pip_rating/__init__.py]
-search = __version__ = '{current_version}'
-replace = __version__ = '{new_version}'
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
 
 [flake8]
 exclude = docs
+ignore = E203, E266, E501, W503, F403, F401, E122
+max-line-length = 120
+max-complexity = 18
+select = B,C,E,F,W,T4,B9
 
 [aliases]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

