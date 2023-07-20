# Comparing `tmp/delvewheel-1.3.8.tar.gz` & `tmp/delvewheel-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.3.8.tar", last modified: Tue Jun 20 13:56:33 2023, max compression
+gzip compressed data, was "delvewheel-1.4.0.tar", last modified: Thu Jul 20 19:25:02 2023, max compression
```

## Comparing `delvewheel-1.3.8.tar` & `delvewheel-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/
--rw-rw-rw-   0        0        0     1073 2023-06-20 13:55:53.000000 delvewheel-1.3.8/LICENSE
--rw-rw-rw-   0        0        0    10414 2023-06-20 13:56:33.017228 delvewheel-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     9294 2023-06-20 13:55:53.000000 delvewheel-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/delvewheel/
--rw-rw-rw-   0        0        0        0 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     5156 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   139059 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    33153 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_version.py
--rw-rw-rw-   0        0        0    38741 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    10414 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-06-20 13:55:53.000000 delvewheel-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2023-06-20 13:56:33.017228 delvewheel-1.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.743006 delvewheel-1.4.0/
+-rw-rw-rw-   0        0        0     1073 2023-07-20 19:24:28.000000 delvewheel-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    10937 2023-07-20 19:25:02.743006 delvewheel-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9817 2023-07-20 19:24:28.000000 delvewheel-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.727445 delvewheel-1.4.0/delvewheel/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     5825 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   139059 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    33153 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    48135 2023-07-20 19:24:28.000000 delvewheel-1.4.0/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:25:02.743006 delvewheel-1.4.0/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    10937 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 19:25:02.000000 delvewheel-1.4.0/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-07-20 19:24:28.000000 delvewheel-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2023-07-20 19:25:02.743006 delvewheel-1.4.0/setup.cfg
```

### Comparing `delvewheel-1.3.8/LICENSE` & `delvewheel-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.8/PKG-INFO` & `delvewheel-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.8
+Version: 1.4.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -87,17 +87,19 @@
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
+- `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
+  - `--namespace-pkg package1` declares `package1` as a namespace package.
+  - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
-- `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.8/README.md` & `delvewheel-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,19 @@
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
+- `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
+  - `--namespace-pkg package1` declares `package1` as a namespace package.
+  - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
-- `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.8/delvewheel/__main__.py` & `delvewheel-1.4.0/delvewheel/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import re
 from ._wheel_repair import WheelRepair
 from ._version import __version__
 from . import _dll_utils
 
 
 def _subdir_suffix(s: str) -> str:
     """Helper for argument parser for validating a subdirectory suffix."""
@@ -17,14 +18,21 @@
     """Helper for argument parser for validating a list of DLL names"""
     for dll_name in filter(None, map(str.strip, s.split(os.pathsep))):
         if any(c in r'<>:"/\|?*' or ord(c) < 32 for c in dll_name):
             raise argparse.ArgumentTypeError(f'Invalid DLL name {dll_name!r}')
     return s
 
 
+def _namespace_pkgs(s: str) -> str:
+    for namespace_pkg in filter(None, s.split(os.pathsep)):
+        if any(c in r'<>:"/\|?*' or ord(c) < 32 for c in namespace_pkg) or not re.fullmatch(r'[^.]+(\.[^.]+)*', namespace_pkg):
+            raise argparse.ArgumentTypeError(f'Invalid namespace package {namespace_pkg!r}')
+    return s
+
+
 def main():
     """Main function"""
     # parse arguments
     parser = argparse.ArgumentParser(description=f'Delvewheel {__version__}: Create self-contained wheels for Windows')
     subparsers = parser.add_subparsers(dest='command', required=True)
     parser_show_description = 'Search a wheel for external DLL dependencies'
     parser_show = subparsers.add_parser('show', help=parser_show_description, description=parser_show_description)
@@ -42,14 +50,15 @@
         subparser.add_argument('--extract-dir', help=argparse.SUPPRESS)
         subparser.add_argument('--test', default='', help=argparse.SUPPRESS)  # comma-separated testing options, internal use only
     parser_repair.add_argument('-w', '--wheel-dir', dest='target', default='wheelhouse', help='directory to write repaired wheel')
     parser_repair.add_argument('--no-mangle', default='', metavar='DLLS', type=_dll_names, help=f'DLL names(s) not to mangle, {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-mangle-all', action='store_true', help="don't mangle any DLL names")
     parser_repair.add_argument('--strip', action='store_true', help='strip DLLs that contain trailing data when name-mangling')
     parser_repair.add_argument('-L', '--lib-sdir', default='.libs', type=_subdir_suffix, help='directory suffix in package to store vendored DLLs (default .libs)')
+    parser_repair.add_argument('--namespace-pkg', default='', metavar='PKGS', type=_namespace_pkgs, help=f'namespace package(s), {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-diagnostic', action='store_true', help=argparse.SUPPRESS)  # don't write diagnostic information to DELVEWHEEL metadata file
     parser_needed.add_argument('file', help='path to a DLL or PYD file')
     parser_needed.add_argument('-v', action='count', default=0, help='verbosity')
     args = parser.parse_args()
 
     # handle command
     if args.command in ('show', 'repair'):
@@ -66,15 +75,16 @@
 
         for wheel in args.wheel:
             wr = WheelRepair(wheel, args.extract_dir, add_dlls, no_dlls, args.ignore_in_wheel, args.v, args.test.split(','))
             if args.command == 'show':
                 wr.show()
             else:  # args.command == 'repair'
                 no_mangles = set(dll_name.lower() for dll_name in args.no_mangle.split(os.pathsep) if dll_name)
-                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic)
+                namespace_pkgs = set(tuple(namespace_pkg.split('.')) for namespace_pkg in args.namespace_pkg.split(os.pathsep) if namespace_pkg)
+                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic, namespace_pkgs)
     else:  # args.command == 'needed'
         for dll_name in sorted(_dll_utils.get_direct_needed(args.file, args.v), key=str.lower):
             print(dll_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `delvewheel-1.3.8/delvewheel/_dll_list.py` & `delvewheel-1.4.0/delvewheel/_dll_list.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.8/delvewheel/_dll_utils.py` & `delvewheel-1.4.0/delvewheel/_dll_utils.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.8/delvewheel/_wheel_repair.py` & `delvewheel-1.4.0/delvewheel/_wheel_repair.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,92 +7,97 @@
 import pathlib
 import pprint
 import re
 import shutil
 import sys
 import tempfile
 import typing
+import warnings
 import zipfile
 from . import _dll_utils
 from . import _dll_list
 from . import _version
 
 
-# Template for patching __init__.py so that the vendored DLLs are loaded at
+# Template for patching a .py file so that the vendored DLLs are loaded at
 # runtime. If the patch would be placed at the beginning of the file, an empty
 # triple-quoted string is placed at the beginning so that the comment
 # "start delvewheel patch" does not show up when the built-in help system
-# help() is invoked on the package. For non-Anaconda Python >= 3.8, we use the
-# os.add_dll_directory() function so that the folder containing the vendored
-# DLLs is added to the DLL search path. For Python 3.7 or lower, this function
-# is unavailable, so we preload the DLLs. Whenever Python needs a vendored DLL,
-# it will use the already-loaded DLL instead of searching for it. We also
-# preload the DLLs for Anaconda Python < 3.10, which has a bug where
+# help() is invoked on the package or file. For non-Anaconda Python >= 3.8, we
+# use the os.add_dll_directory() function so that the folder containing the
+# vendored DLLs is added to the DLL search path. For Python 3.7 or lower, this
+# function is unavailable, so we preload the DLLs. Whenever Python needs a
+# vendored DLL, it will use the already-loaded DLL instead of searching for it.
+# We also preload the DLLs for Anaconda Python < 3.10, which has a bug where
 # os.add_dll_directory() does not always take effect.
 #
 # The template must produce Python code that is compatible with Python 2.6, the
 # oldest supported target Python version.
 #
 # To use the template, call str.format(), passing in
 # 0. '""""""' if the patch would be at the start of the file else ''
 # 1. an identifying string such as the delvewheel version
-# 2. the name of the directory containing the vendored DLLs
-# 3. the name of the file containing the DLL load order.
-_patch_init_template = """
+# 2. a number of repeats of 'os.pardir, ' corresponding to the path depth of
+#    the file in site-packages upon wheel installation
+# 3. the name of the directory containing the vendored DLLs
+# 4. the name of the file containing the DLL load order.
+_patch_py_template = """
 
 {0}# start delvewheel patch
-def _delvewheel_init_patch_{1}():
+def _delvewheel_patch_{1}():
     import ctypes
     import os
     import platform
     import sys
-    libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, {2!r}))
+    libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), {2}{3!r}))
     is_conda_cpython = platform.python_implementation() == 'CPython' and (hasattr(ctypes.pythonapi, 'Anaconda_GetVersion') or 'packaged by conda-forge' in sys.version)
     if sys.version_info[:2] >= (3, 8) and not is_conda_cpython or sys.version_info[:2] >= (3, 10):
         if os.path.isdir(libs_dir):
             os.add_dll_directory(libs_dir)
     else:
-        load_order_filepath = os.path.join(libs_dir, {3!r})
+        load_order_filepath = os.path.join(libs_dir, {4!r})
         if os.path.isfile(load_order_filepath):
-            with open(os.path.join(libs_dir, {3!r})) as file:
+            with open(os.path.join(libs_dir, {4!r})) as file:
                 load_order = file.read().split()
             for lib in load_order:
                 lib_path = os.path.join(os.path.join(libs_dir, lib))
                 if os.path.isfile(lib_path) and not ctypes.windll.kernel32.LoadLibraryExW(ctypes.c_wchar_p(lib_path), None, 0x00000008):
                     raise OSError('Error loading {{}}; {{}}'.format(lib, ctypes.FormatError()))
 
 
-_delvewheel_init_patch_{1}()
-del _delvewheel_init_patch_{1}
+_delvewheel_patch_{1}()
+del _delvewheel_patch_{1}
 # end delvewheel patch
 
 """
 
-# Template for patching __init__.py for Python 3.10 and above. For these Python
+# Template for patching a .py file for Python 3.10 and above. For these Python
 # versions, os.add_dll_directory() is used as the exclusive strategy.
 #
 # The template must produce Python code that is compatible with Python 2.6, the
 # oldest supported target Python version.
 #
 # To use the template, call str.format(), passing in
 # 0. '""""""' if the patch would be at the start of the file else ''
 # 1. an identifying string such as the delvewheel version
-# 2. the name of the directory containing the vendored DLLs
-_patch_init_template_v2 = """
+# 2. a number of repeats of 'os.pardir, ' corresponding to the path depth of
+#    the file in site-packages upon wheel installation
+# 3. the name of the directory containing the vendored DLLs
+_patch_py_template_v2 = """
 
 {0}# start delvewheel patch
-def _delvewheel_init_patch_{1}():
+def _delvewheel_patch_{1}():
     import os
-    libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, {2!r}))
+    libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), {2}{3!r}))
     if os.path.isdir(libs_dir):
         os.add_dll_directory(libs_dir)
 
 
-_delvewheel_init_patch_{1}()
-del _delvewheel_init_patch_{1}
+_delvewheel_patch_{1}()
+del _delvewheel_patch_{1}
 # end delvewheel patch
 
 """
 
 pp = pprint.PrettyPrinter(indent=4)
 
 
@@ -103,14 +108,17 @@
     _test: typing.List[str]  # testing options for internal use
     _whl_path: str  # path to wheel
     _whl_name: str  # name of wheel
     _distribution_name: str
     _version: str  # wheel version
     _extract_dir_obj: typing.Optional[tempfile.TemporaryDirectory]  # wheel extraction directory object
     _extract_dir: str  # wheel extraction directory
+    _data_dir: str  # extracted path to .data directory, is set even if directory does not exist
+    _purelib_dir: str  # extracted path to .data/purelib directory, is set even if directory does not exist
+    _platlib_dir: str  # extracted path to .data/platlib directory, is set even if directory does not exist
     _add_dlls: typing.Set[str]  # additional DLLs to addd
     _no_dlls: typing.Set[str]  # DLLs to exclude
     _wheel_dirs: typing.Optional[typing.List[str]]  # extracted directories from inside wheel
     _ignore_in_wheel: bool  # whether to ignore DLLs that are already inside wheel
     _arch: _dll_list.MachineType  # CPU architecture of wheel
     _min_supported_python: typing.Optional[typing.Tuple[int, int]]
         # minimum supported Python version based on Python tags (ignoring the
@@ -163,14 +171,18 @@
             pass
         os.makedirs(self._extract_dir)
         if self._verbose >= 1:
             print(f'extracting {self._whl_name} to {self._extract_dir}')
         with zipfile.ZipFile(self._whl_path) as whl_file:
             whl_file.extractall(self._extract_dir)
 
+        self._data_dir = os.path.join(self._extract_dir, f'{self._distribution_name}-{self._version}.data')
+        self._purelib_dir = os.path.join(self._data_dir, 'purelib')
+        self._platlib_dir = os.path.join(self._data_dir, 'platlib')
+
         self._add_dlls = set() if add_dlls is None else add_dlls
         self._no_dlls = set() if no_dlls is None else no_dlls
 
         # Modify self._no_dlls to include those that are already part of every
         # Python distribution the wheel targets.
         abi_tags = whl_name_split[-2].split('.')
         platform_tag = whl_name_split[-1]
@@ -254,143 +266,180 @@
         hasher = hashlib.sha256(self._distribution_name.encode())
         buf = afile.read(blocksize)
         while len(buf) > 0:
             hasher.update(buf)
             buf = afile.read(blocksize)
         return hasher.hexdigest()[:length]
 
-    def _patch_init_contents(self, at_start: bool, libs_dir: str, load_order_filename: typing.Optional[str]) -> str:
-        """Return the contents of the patch to place in __init__.py.
+    def _patch_py_contents(self, at_start: bool, libs_dir: str, load_order_filename: typing.Optional[str], depth: int) -> str:
+        """Return the contents of the patch to place in a .py file.
 
-        at_start is whether the contents are placed at the beginning of
-            __init__.py
+        at_start is whether the contents are placed at the beginning of the file
         libs_dir is the name of the directory where DLLs are stored.
         load_order_filename is the name of the .load-order file, or None if the
-            file is not used"""
+            file is not used
+        depth is the number of parent directories to traverse to reach the
+            site-packages directory at runtime starting from the directory
+            containing the .py file"""
         if self._min_supported_python is None or self._min_supported_python < (3, 10):
             if load_order_filename is None:
                 raise ValueError('load_order_filename cannot be None')
-            return _patch_init_template.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), libs_dir, load_order_filename)
+            return _patch_py_template.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir, load_order_filename)
         else:
-            return _patch_init_template_v2.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), libs_dir)
+            return _patch_py_template_v2.format('""""""' if at_start else '', _version.__version__.replace('.', '_'), 'os.pardir, ' * depth, libs_dir)
 
-    def _patch_init(self, init_path: str, libs_dir: str, load_order_filename: typing.Optional[str]) -> None:
-        """Given the path to __init__.py, create or patch the file so that
-        vendored-in DLLs can be loaded at runtime. The patch is placed at the
+    def _patch_py_file(self, py_path: str, libs_dir: str, load_order_filename: typing.Optional[str], depth: int) -> None:
+        """Given the path to a .py file, create or patch the file so that
+        vendored DLLs can be loaded at runtime. The patch is placed at the
         topmost location after the docstring (if any) and any
         "from __future__ import" statements.
 
-        init_path is the path to the __init__.py file to patch
+        py_path is the path to the .py file to create or patch
         libs_dir is the name of the directory where DLLs are stored.
         load_order_filename is the name of the .load-order file, or None if the
-            file is not used"""
-        print(f'patching {os.path.relpath(init_path, self._extract_dir)}')
-
-        open(init_path, 'a+').close()  # create file if it doesn't exist
-        with open(init_path, newline='') as file:
+            file is not used
+        depth is the number of parent directories to traverse to reach the
+            site-packages directory at runtime starting from the directory
+            containing the .py file"""
+        print(f'patching {os.path.relpath(py_path, self._extract_dir)}')
+
+        py_name = os.path.basename(py_path)
+        open(py_path, 'a+').close()  # create file if it doesn't exist
+        with open(py_path, newline='') as file:
             line = file.readline()
         for newline in ('\r\n', '\r', '\n'):
             if line.endswith(newline):
                 break
         else:
             newline = '\r\n'
 
-        with open(init_path) as file:
-            init_contents = file.read()
-        node = ast.parse(init_contents)
+        with open(py_path) as file:
+            py_contents = file.read()
+        node = ast.parse(py_contents)
         docstring = ast.get_docstring(node, False)
         children = list(ast.iter_child_nodes(node))
         for child in reversed(children):
             if isinstance(child, ast.ImportFrom) and child.module == '__future__':
                 future_import_lineno = child.lineno
                 break
         else:
             future_import_lineno = 0  # no "from __future__ import" statement found
 
         if future_import_lineno > 0:
             # insert patch after the last __future__ import
-            patch_init_contents = self._patch_init_contents(False, libs_dir, load_order_filename)
-            init_contents_split = init_contents.splitlines(True)
-            with open(init_path, 'w', newline=newline) as file:
-                file.write(''.join(init_contents_split[:future_import_lineno]))
+            patch_py_contents = self._patch_py_contents(False, libs_dir, load_order_filename, depth)
+            py_contents_split = py_contents.splitlines(True)
+            with open(py_path, 'w', newline=newline) as file:
+                file.write(''.join(py_contents_split[:future_import_lineno]))
                 file.write('\n')
-                file.write(patch_init_contents)
-                file.write(''.join(init_contents_split[future_import_lineno:]))
+                file.write(patch_py_contents)
+                file.write(''.join(py_contents_split[future_import_lineno:]))
         elif docstring is None:
             # prepend patch
-            patch_init_contents = self._patch_init_contents(True, libs_dir, load_order_filename)
-            with open(init_path, 'w', newline=newline) as file:
-                file.write(patch_init_contents)
-                file.write(init_contents)
+            patch_py_contents = self._patch_py_contents(True, libs_dir, load_order_filename, depth)
+            with open(py_path, 'w', newline=newline) as file:
+                file.write(patch_py_contents)
+                file.write(py_contents)
         else:
             # place patch just after docstring
-            patch_init_contents = self._patch_init_contents(False, libs_dir, load_order_filename)
+            patch_py_contents = self._patch_py_contents(False, libs_dir, load_order_filename, depth)
             if len(children) == 0 or not isinstance(children[0], ast.Expr) or ast.literal_eval(children[0].value) != docstring:
                 # verify that the first child node is the docstring
-                raise ValueError('Error parsing __init__.py: docstring exists but is not the first element of the parse tree')
+                raise ValueError(f'Error parsing {py_name}: docstring exists but is not the first element of the parse tree')
             if len(children) == 1:
                 # append patch
-                with open(init_path, 'a') as file:
-                    file.write(patch_init_contents)
+                with open(py_path, 'a') as file:
+                    file.write(patch_py_contents)
             else:
                 # insert patch after docstring
-                init_contents = '\n'.join(init_contents.splitlines())  # normalize line endings
+                py_contents = '\n'.join(py_contents.splitlines())  # normalize line endings
                 docstring_search_start_index = 0
-                for line in init_contents.splitlines(True):
+                for line in py_contents.splitlines(True):
                     if line.lstrip().startswith('#'):
                         # ignore comments at start of file
                         docstring_search_start_index += len(line)
                     else:
                         break
-                double_quotes_index = init_contents.find('"""', docstring_search_start_index)
-                single_quotes_index = init_contents.find("'''", docstring_search_start_index)
+                double_quotes_index = py_contents.find('"""', docstring_search_start_index)
+                single_quotes_index = py_contents.find("'''", docstring_search_start_index)
                 if double_quotes_index == -1 and single_quotes_index == -1:
-                    raise ValueError('Error parsing __init__.py: docstring exists but does not start with triple quotes')
+                    raise ValueError(f'Error parsing {py_name}: docstring exists but does not start with triple quotes')
                 elif double_quotes_index == -1 or single_quotes_index != -1 and single_quotes_index < double_quotes_index:
                     docstring_start_index = single_quotes_index
                     quotes = "'''"
                 else:
                     docstring_start_index = double_quotes_index
                     quotes = '"""'
-                docstring_end_index = init_contents.find(quotes, docstring_start_index + 3)
+                docstring_end_index = py_contents.find(quotes, docstring_start_index + 3)
                 if docstring_end_index == -1:
-                    raise ValueError('Error parsing __init__.py: docstring exists but does not end with triple quotes')
+                    raise ValueError(f'Error parsing {py_name}: docstring exists but does not end with triple quotes')
                 docstring_end_index += 3
-                docstring_end_line = init_contents.find('\n', docstring_end_index)
+                docstring_end_line = py_contents.find('\n', docstring_end_index)
                 if docstring_end_line == -1:
-                    docstring_end_line = len(init_contents)
-                extra_text = init_contents[docstring_end_index: docstring_end_line]
+                    docstring_end_line = len(py_contents)
+                extra_text = py_contents[docstring_end_index: docstring_end_line]
                 if extra_text and not extra_text.isspace():
-                    raise ValueError(f'Error parsing __init__.py: extra text {extra_text!r} is on the line where the docstring ends. Move the extra text to a new line and try again.')
-                with open(init_path, 'w', newline=newline) as file:
-                    file.write(init_contents[:docstring_end_index])
+                    raise ValueError(f'Error parsing {py_name}: extra text {extra_text!r} is on the line where the docstring ends. Move the extra text to a new line and try again.')
+                with open(py_path, 'w', newline=newline) as file:
+                    file.write(py_contents[:docstring_end_index])
                     file.write('\n')
-                    file.write(patch_init_contents)
-                    file.write(init_contents[docstring_end_index:])
+                    file.write(patch_py_contents)
+                    file.write(py_contents[docstring_end_index:])
 
-        # verify that __init__.py can be parsed properly
-        with open(init_path) as file:
+        # verify that the file can be parsed properly
+        with open(py_path) as file:
             try:
                 ast.parse(file.read())
             except SyntaxError:
-                raise ValueError('Error parsing __init__.py: Patch failed. This might occur if a node is split across multiple lines.')
+                raise ValueError(f'Error parsing {py_name}: Patch failed. This might occur if a node is split across multiple lines.')
 
-    def _is_top_level_ext_module(self, path: str) -> bool:
-        """Return True if `path` refers to a top-level extension module. That
-        is, when the wheel is installed, the module is placed directly into the
-        site-packages directory and not inside a package. Otherwise, return
-        False.
-
-        Precondition: path must end with .pyd"""
-        top_level_dirs = [
-            pathlib.Path(self._extract_dir),
-            pathlib.Path(self._extract_dir) / f'{self._distribution_name}-{self._version}.data' / 'purelib',
-            pathlib.Path(self._extract_dir) / f'{self._distribution_name}-{self._version}.data' / 'platlib',
-        ]
-        return pathlib.Path(os.path.dirname(path)) in top_level_dirs
+    @staticmethod
+    def _get_init(dir: str) -> typing.Optional[str]:
+        """If directory dir contains any case variation of the __init__.py file,
+        then return the path to that file. Otherwise, return None.
+
+        Precondition: dir is an existing directory"""
+        for item in os.listdir(dir):
+            path = os.path.join(dir, item)
+            if item.lower() == '__init__.py' and os.path.isfile(path):
+                return path
+        return None
+
+    def _patch_package(self, package_dir: str, namespace_pkgs: typing.Set[typing.Tuple[str]], libs_dir: str, load_order_filename: str, depth: int) -> typing.Set[str]:
+        """Patch a package so that vendored DLLs can be found at runtime.
+        Return a set containing the absolute extracted paths of all .pyd
+        extension modules that are at the root of a namespace package within
+        the package.
+
+        package_dir is the absolute path to the extracted package
+        namespace_pkgs is a set of paths, relative to the parent of
+            package_dir, corresponding to the namespace packages. Each path is
+            represented as a tuple of path components.
+        libs_dir is the name of the directory where DLLs are stored.
+        load_order_filename is the name of the .load-order file, or None if the
+            file is not used
+        depth is the number of parent directories to traverse to reach the
+            site-packages directory at runtime starting from package_dir"""
+        package_name = os.path.basename(package_dir)
+        namespace_root_ext_modules = set()
+        if any(x[0] == package_name for x in namespace_pkgs):
+            for item in os.listdir(package_dir):
+                item_path = os.path.join(package_dir, item)
+                if os.path.isfile(item_path):
+                    item_lower = item.lower()
+                    if item_lower.endswith('.py') and item_lower != '__init__.py':
+                        self._patch_py_file(item_path, libs_dir, load_order_filename, depth)
+                    elif item_lower.endswith('.pyd'):
+                        namespace_root_ext_modules.add(item_path)
+                elif os.path.isdir(item_path) and \
+                        (item not in self._root_level_module_names(package_dir) or self._get_init(item_path)):
+                    namespace_root_ext_modules.update(self._patch_package(item_path, set(x[1:] for x in namespace_pkgs if x[0] == package_name and len(x) > 1), libs_dir, load_order_filename, depth + 1))
+        else:
+            self._patch_py_file(self._get_init(package_dir) or os.path.join(package_dir, '__init__.py'), libs_dir, load_order_filename, depth)
+        return namespace_root_ext_modules
 
     def _get_repair_version(self) -> str:
         """If this wheel has already been repaired, return the delvewheel
         version that performed the repair or '(unknown version)' if the version
         could not be determined. Return the empty string if the wheel has not
         been repaired."""
         filename = os.path.join(self._extract_dir, f'{self._distribution_name}-{self._version}.dist-info', 'DELVEWHEEL')
@@ -414,14 +463,80 @@
         for dependency_path in dependency_paths:
             if pathlib.Path(self._extract_dir) in pathlib.Path(dependency_path).parents:
                 dependency_paths_in_wheel.add(dependency_path)
             else:
                 dependency_paths_outside_wheel.add(dependency_path)
         return dependency_paths_in_wheel, dependency_paths_outside_wheel
 
+    def _get_site_packages_relpath(self, path: str) -> str:
+        """Given the path to a file or folder in the extracted wheel contents,
+        return the path relative to site-packages when the wheel is
+        installed."""
+        purelib_dir_obj = pathlib.Path(self._purelib_dir)
+        platlib_dir_obj = pathlib.Path(self._platlib_dir)
+        path_obj = pathlib.Path(path)
+        if path_obj == purelib_dir_obj or purelib_dir_obj in path_obj.parents:
+            return os.path.relpath(path, self._purelib_dir)
+        elif path_obj == platlib_dir_obj or platlib_dir_obj in path_obj.parents:
+            return os.path.relpath(path, self._platlib_dir)
+        else:
+            return os.path.relpath(path, self._extract_dir)
+
+    def _root_level_module_names(self, path: str) -> typing.Set[str]:
+        """Given the absolute path to the extracted wheel contents or to an
+        extracted package, return a set of original-case names of the Python
+        modules at the root of the wheel or package. A name does not include
+        the file extension or compatibility tag.
+
+        Precondition: path is to a folder that exists"""
+        module_names = set()
+        for top_level in (self._extract_dir, self._purelib_dir, self._platlib_dir):
+            search_dir = os.path.join(top_level, self._get_site_packages_relpath(path))
+            if os.path.isdir(search_dir):
+                filenames = os.listdir(search_dir)
+                for filename in filenames:
+                    if os.path.isfile(os.path.join(search_dir, filename)) and \
+                            (filename.lower().endswith('.py') or filename.lower().endswith('.pyd')):
+                        module_names.add(filename[:filename.index('.')])
+        return module_names
+
+    @staticmethod
+    def _isdir_case(root: str, remainder: typing.Tuple[str]) -> bool:
+        """Return True if remainder is an existing directory relative to root.
+        Regardless of the case sensitivity of the file system, treat remainder
+        as case-sensitive. Treat root using the file system's case sensitivity.
+
+        remainder is represented as a tuple of path components. If root is not
+        an existing directory, return False."""
+        if not os.path.isdir(root):
+            return False
+        for component in remainder:
+            new_root = os.path.join(root, component)
+            if component not in os.listdir(root) or not os.path.isdir(new_root):
+                return False
+            root = new_root
+        return True
+
+    def _namespace_pkg_sortkey(self, path: str) -> int:
+        """Given the path to a file or folder in the extracted wheel contents,
+        return an int that can be used to sort the path.
+
+        Return 3 if the path is in the purelib directory.
+        Return 2 if the path is in the platlib directory.
+        Return 1 otherwise."""
+        purelib_dir_obj = pathlib.Path(self._purelib_dir)
+        platlib_dir_obj = pathlib.Path(self._platlib_dir)
+        path_obj = pathlib.Path(path)
+        if path_obj == purelib_dir_obj or purelib_dir_obj in path_obj.parents:
+            return 3
+        elif path_obj == platlib_dir_obj or platlib_dir_obj in path_obj.parents:
+            return 2
+        else:
+            return 1
+
     def show(self) -> None:
         """Show the dependencies that the wheel has."""
         print(f'Analyzing {self._whl_name}\n')
 
         # check whether wheel has already been repaired
         repair_version = self._get_repair_version()
         if repair_version:
@@ -491,49 +606,52 @@
             for ignored_dll_name in ignored_dll_names:
                 print(f'    {ignored_dll_name}')
         else:
             print('    None')
         if not_found_dll_names:
             print('\nWarning: At least one dependent DLL needs to be copied into the wheel but was not found.')
 
-    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, no_diagnostic: bool) -> None:
+    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, no_diagnostic: bool, namespace_pkgs: typing.Set[typing.Tuple[str]]) -> None:
         """Repair the wheel in a manner similar to auditwheel.
         target is the target directory for storing the repaired wheel
         no_mangles is a set of lowercase DLL names that will not be mangled
         no_mangle_all is True if no DLL name mangling should happen at all
         strip is True if we should strip DLLs that contain trailing data when
             name-mangling
         lib_sdir is the suffix for the directory to store the DLLs
         no_diagnostic is True if no diagnostic information is written to the
-            DELVEWHEEL metadata file"""
+            DELVEWHEEL metadata file
+        namespace_pkgs is a set of paths, relative to the wheel root,
+            corresponding to the namespace packages. Each path is represented
+            as a tuple of path components"""
         print(f'repairing {self._whl_path}')
 
         # check whether wheel has already been repaired
         repair_version = self._get_repair_version()
         if repair_version:
             print(f'Delvewheel {repair_version} has already repaired this wheel.')
             return
 
         # find dependencies
         print('finding DLL dependencies')
         dependency_paths = set()
         ignored_dll_names = set()
         extension_module_paths = []
-        top_level_ext_module_names = set()
+        has_top_level_ext_module = False
         for root, _, filenames in os.walk(self._extract_dir):
             for filename in filenames:
                 if filename.lower().endswith('.pyd'):
                     extension_module_path = os.path.join(root, filename)
                     dll_arch = _dll_utils.get_arch(extension_module_path)
                     if dll_arch != self._arch:
                         raise RuntimeError(f'{os.path.relpath(extension_module_path, self._extract_dir)} has a CPU architecture that is not compatible with this wheel')
-                    if self._is_top_level_ext_module(extension_module_path):
+                    if self._get_site_packages_relpath(root) == os.curdir:
                         if self._verbose >= 1:
                             print(f'analyzing top-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
-                        top_level_ext_module_names.add(filename[:filename.index('.')])
+                        has_top_level_ext_module = True
                     elif self._verbose >= 1:
                         print(f'analyzing package-level extension module {os.path.relpath(extension_module_path, self._extract_dir)}')
                     extension_module_paths.append(extension_module_path)
                     discovered, ignored = _dll_utils.get_all_needed(extension_module_path, self._no_dlls, self._wheel_dirs, 'raise', self._verbose)[:2]
                     dependency_paths |= discovered
                     ignored_dll_names |= ignored
 
@@ -558,31 +676,44 @@
             if dll_name in dependency_names_lower:
                 continue
             path = _dll_utils.find_library(dll_name, None, self._arch)
             if path:
                 extra_dependency_paths.add(path)
             else:
                 raise FileNotFoundError(f'{dll_name} not found')
-
         if not dependency_paths and not extra_dependency_paths:
             print('no external dependencies are needed')
             return
+
+        # Warn if namespace package does not exist
+        not_found_namespace_pkgs = set()
+        for namespace_pkg in namespace_pkgs:
+            if not any(self._isdir_case(root, namespace_pkg) for root in (self._extract_dir, self._purelib_dir, self._platlib_dir)):
+                not_found_namespace_pkgs.add('.'.join(namespace_pkg))
+        if not_found_namespace_pkgs:
+            warnings.warn(
+                'Namespace package'
+                f'{"s" if len(not_found_namespace_pkgs) > 1 else ""} '
+                f'{not_found_namespace_pkgs} w'
+                f'{"as" if len(not_found_namespace_pkgs) == 1 else "ere"} '
+                f'not found', UserWarning)
+
         if self._verbose >= 1:
             to_copy = set(os.path.basename(p) for p in dependency_paths | extra_dependency_paths)
             ignored_dll_names -= {name.lower() for name in to_copy}
             print(f'External dependencies to copy into the wheel are\n{pp.pformat(to_copy)}')
             print(f'External dependencies not to copy into the wheel are\n{pp.pformat(ignored_dll_names)}')
-        if top_level_ext_module_names:
+        if has_top_level_ext_module:
             # At least 1 extension module is top-level, so we cannot use
             # __init__.py to insert the DLL search path at runtime. In this
             # case, DLLs are instead copied into the platlib folder, whose
             # contents are installed directly into site-packages during
             # installation.
             libs_dir_name = '.'
-            libs_dir = os.path.join(self._extract_dir, f'{self._distribution_name}-{self._version}.data', 'platlib')
+            libs_dir = self._platlib_dir
         else:
             libs_dir_name = self._distribution_name + lib_sdir
             libs_dir = os.path.join(self._extract_dir, libs_dir_name)
         os.makedirs(libs_dir, exist_ok=True)
         print(f'copying DLLs into {os.path.relpath(libs_dir, self._extract_dir)}')
         for dependency_path in dependency_paths | extra_dependency_paths:
             if self._verbose >= 1:
@@ -619,14 +750,82 @@
                 lib_path = os.path.join(libs_dir, lib_name)
                 needed = _dll_utils.get_direct_mangleable_needed(lib_path, self._no_dlls, no_mangles, self._verbose)
                 _dll_utils.replace_needed(lib_path, needed, name_mangler, strip, self._verbose, self._test)
                 if lib_name.lower() in name_mangler:
                     os.rename(lib_path, os.path.join(libs_dir, name_mangler[lib_name.lower()]))
 
         if self._min_supported_python is None or self._min_supported_python < (3, 10):
+            load_order_filename = f'.load-order-{self._distribution_name}-{self._version}'
+        else:
+            load_order_filename = None
+
+        # Patch each package to load dependent DLLs from correct location at
+        # runtime.
+        #
+        # However, if a module and a folder are next to each other and have the
+        # same name and case,
+        # - If the folder does not contain __init__.py, do not patch
+        #   the folder. Otherwise, the import resolution order of the module
+        #   and the folder may be swapped.
+        # - If the folder contains __init__.py, patch the module (if it is pure
+        #   Python) and the folder.
+        dist_info_foldername = f'{self._distribution_name}-{self._version}.dist-info'
+        namespace_root_ext_modules = set()
+        for item in os.listdir(self._extract_dir):
+            package_dir = os.path.join(self._extract_dir, item)
+            if os.path.isdir(package_dir) and \
+                    item != dist_info_foldername and \
+                    item != os.path.basename(self._data_dir) and \
+                    item != libs_dir_name and \
+                    (item not in self._root_level_module_names(self._extract_dir) or self._get_init(package_dir)):
+                namespace_root_ext_modules.update(self._patch_package(package_dir, namespace_pkgs, libs_dir_name, load_order_filename, 1))
+        for extra_dir in (self._purelib_dir, self._platlib_dir):
+            if os.path.isdir(extra_dir):
+                for item in os.listdir(extra_dir):
+                    package_dir = os.path.join(extra_dir, item)
+                    if os.path.isdir(package_dir) and \
+                            (item not in self._root_level_module_names(self._extract_dir) or self._get_init(package_dir)):
+                        namespace_root_ext_modules.update(self._patch_package(package_dir, namespace_pkgs, libs_dir_name, load_order_filename, 1))
+
+        # Copy libraries next to all extension modules that are at the root of
+        # a namespace package. If a namespace package contains extension
+        # modules that are split across at least 2 of the following:
+        # 1. the wheel root,
+        # 2. the platlib directory,
+        # 3. the purelib directory,
+        # then copy the libraries to the first in the above list containing
+        # this namespace package.
+        if namespace_root_ext_modules:
+            dirnames = set(self._get_site_packages_relpath(os.path.dirname(x)) for x in namespace_root_ext_modules)
+            filenames = set(map(os.path.basename, namespace_root_ext_modules))
+            warnings.warn(
+                f'Namespace package{"s" if len(dirnames) > 1 else ""} '
+                f'{os.pathsep.join(dirnames)} contain'
+                f'{"s" if len(dirnames) == 1 else ""} root-level extension '
+                f'module{"s" if len(filenames) > 1 else ""} '
+                f'{os.pathsep.join(filenames)} and need'
+                f'{"s" if len(dirnames) == 1 else ""} '
+                f'{"an " if len(dirnames) == 1 else ""}extra '
+                f'cop{"ies" if len(dirnames) > 1 else "y"} of the '
+                'vendored DLLs. To avoid duplicate DLLs, move extension '
+                'modules into regular (non-namespace) packages.', UserWarning)
+            dirnames = list(set(map(os.path.dirname, namespace_root_ext_modules)))
+            dirnames.sort(key=self._namespace_pkg_sortkey)
+            seen_relative = set()
+            for dirname in dirnames:
+                dirname_relative = self._get_site_packages_relpath(dirname)
+                if dirname_relative not in seen_relative:
+                    for lib_name in os.listdir(libs_dir):
+                        lib_path = os.path.join(libs_dir, lib_name)
+                        if self._verbose >= 1:
+                            print(f'copying {lib_path} -> {os.path.join(dirname, lib_name)}')
+                        shutil.copy2(lib_path, dirname)
+                    seen_relative.add(dirname_relative)
+
+        if load_order_filename is not None:
             # Create .load-order file containing list of DLLs to load during
             # import. Contrary to what the filename suggests, the DLLs are not
             # listed in any particular order. In an older version of
             # delvewheel, the DLLs needed to be listed in a particular order,
             # and the old filename has been kept to maintain backward
             # compatibility with re-bundling tools such as PyInstaller.
             for dependency_name in dependency_names.copy():
@@ -636,67 +835,35 @@
                     dependency_names.add(name_mangler[dependency_name.lower()])
             # If the wheel contains a top-level extension module, then the
             # load-order file will be installed directly into site-packages. To
             # avoid conflicts with load-order files from other distributions,
             # include the distribution name and version in the load-order
             # filename. Do this regardless of whether the wheel actually
             # contains a top-level extension module.
-            load_order_filename = f'.load-order-{self._distribution_name}-{self._version}'
             load_order_filepath = os.path.join(libs_dir, load_order_filename)
             if os.path.exists(load_order_filepath):
                 raise FileExistsError(f'{os.path.relpath(load_order_filepath, self._extract_dir)} already exists')
             with open(os.path.join(libs_dir, load_order_filename), 'w', newline='\n') as file:
                 file.write('\n'.join(dependency_names))
                 file.write('\n')
-        else:
-            load_order_filename = None
-
-        # Create or patch top-level __init__.py in each package to load
-        # dependent DLLs from correct location at runtime.
-        #
-        # This may cause problems for namespace packages where __init__.py must
-        # be absent for proper functionality. However, without __init__.py, we
-        # cannot load the dependent DLLs. For now, we do not handle this edge
-        # case and create __init__.py anyway.
-        #
-        # An exception is that if a top-level module and a top-level namespace
-        # package have the same name, do not create __init__.py in the package.
-        # Otherwise, the import resolution order of the module and the package
-        # would be swapped.
-        dist_info_foldername = f'{self._distribution_name}-{self._version}.dist-info'
-        for item in os.listdir(self._extract_dir):
-            init_path = os.path.join(self._extract_dir, item, '__init__.py')
-            if os.path.isdir(os.path.join(self._extract_dir, item)) and \
-                    item != dist_info_foldername and \
-                    item != f'{self._distribution_name}-{self._version}.data' and \
-                    item != libs_dir_name and \
-                    (item not in top_level_ext_module_names or os.path.isfile(init_path)):
-                self._patch_init(init_path, libs_dir_name, load_order_filename)
-        for extra_dir_name in ('purelib', 'platlib'):
-            extra_dir = os.path.join(self._extract_dir, f'{self._distribution_name}-{self._version}.data', extra_dir_name)
-            if os.path.isdir(extra_dir):
-                for item in os.listdir(extra_dir):
-                    init_path = os.path.join(extra_dir, item, '__init__.py')
-                    if os.path.isdir(os.path.join(extra_dir, item)) and \
-                            (item not in top_level_ext_module_names or os.path.isfile(init_path)):
-                        self._patch_init(init_path, libs_dir_name, load_order_filename)
 
         # Create .dist-info/DELVEWHEEL file to log repair information. The
         # first line of the file must be 'Version: ' followed by the delvewheel
         # version. Further lines are for information purposes only and are
         # subject to change without notice between delvewheel versions.
         filename = os.path.join(self._extract_dir, dist_info_foldername, 'DELVEWHEEL')
         with open(filename, 'w', newline='\n') as file:
             file.write(f'Version: {_version.__version__}\n')
             if not no_diagnostic:
                 file.write(f'Arguments: {sys.argv}\n')
 
         # update record file, which tracks wheel contents and their checksums
         record_filepath = os.path.join(self._extract_dir, dist_info_foldername, 'RECORD')
-        print(f'updating {os.path.join(dist_info_foldername, "RECORD")}')
+        if self._verbose >= 1:
+            print(f'updating {os.path.join(dist_info_foldername, "RECORD")}')
         filepath_list = []
         for root, _, files in os.walk(self._extract_dir):
             for file in files:
                 filepath_list.append(os.path.join(root, file))
         with open(record_filepath, 'w', newline='\n') as record_file:
             for file_path in filepath_list:
                 if file_path == record_filepath:
```

### Comparing `delvewheel-1.3.8/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.4.0/delvewheel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.8
+Version: 1.4.0
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -87,17 +87,19 @@
   - `-vv`: level 2, include warnings from `pefile`
 - `--extract-dir`: directory to store extracted contents of wheel for debug use (default is a temp directory)
 - `-w`,`--wheel-dir`: directory to write the repaired wheel (default is `wheelhouse` relative to current working directory)
 - `--no-mangle`: name(s) of DLL(s) not to mangle, path-separator-delimited
 - `--no-mangle-all`: don't mangle any DLL names
 - `--strip`: strip DLLs that contain trailing data when name-mangling. The GNU `strip` utility must be present in `PATH`.
 - `-L`,`--lib-sdir`: subdirectory suffix to store vendored DLLs (default `.libs`). For example, if your wheel is named `mywheel-0.0.1-cp310-cp310-win_amd64.whl`, then the vendored DLLs are stored in `mywheel.libs` by default. If your wheel contains a top-level extension module that is not in any package, then this setting is ignored, and vendored DLLs are instead placed directly into `site-packages` when the wheel is installed.
+- `--namespace-pkg`: namespace packages, specified in case-sensitive dot notation and delimited by the path separator. Normally, we patch or create `__init__.py` in each top-level package to add the vendored DLL location to the DLL search path at runtime. If you have a top-level namespace package that requires `__init__.py` to be absent or unmodified, then this technique can cause problems. This option tells `delvewheel` to use an alternate strategy that does not create or modify `__init__.py` at the root of the given namespace package(s). For example,
+  - `--namespace-pkg package1` declares `package1` as a namespace package.
+  - On Windows, `--namespace-pkg package1.package2;package3` declares `package1`, `package1\package2`, and `package3` as namespace packages.
 
 ## Limitations
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
-- `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
 - If your project has a [delay-load DLL dependency](https://learn.microsoft.com/en-us/cpp/build/reference/linker-support-for-delay-loaded-dlls), you must use a custom delay-load import hook when building the DLL that has the delay-load dependency. This ensures that the directory containing the vendored DLLs is included in the DLL search path when delay-loading. For convenience, we provide a suitable hook for Microsoft Visual C/C++ at [delayload/delayhook.c](delayload/delayhook.c). Add the file to your C/C++ project when building your DLL.
```

### Comparing `delvewheel-1.3.8/setup.cfg` & `delvewheel-1.4.0/setup.cfg`

 * *Files identical despite different names*

