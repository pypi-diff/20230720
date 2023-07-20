# Comparing `tmp/types-setuptools-68.0.0.2.tar.gz` & `tmp/types-setuptools-68.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-68.0.0.2.tar", last modified: Sat Jul 15 21:13:19 2023, max compression
+gzip compressed data, was "types-setuptools-68.0.0.3.tar", last modified: Thu Jul 20 15:16:59 2023, max compression
```

## Comparing `types-setuptools-68.0.0.2.tar` & `types-setuptools-68.0.0.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-15 21:13:17.000000 types-setuptools-68.0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 21:13:17.000000 types-setuptools-68.0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.610585 types-setuptools-68.0.0.2/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 21:13:17.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.606585 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.610585 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/specifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-15 21:13:17.000000 types-setuptools-68.0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.614585 types-setuptools-68.0.0.2/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 21:13:17.000000 types-setuptools-68.0.0.2/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.614585 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.618585 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/_distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/py312compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-15 21:13:01.000000 types-setuptools-68.0.0.2/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:13:19.622585 types-setuptools-68.0.0.2/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-15 21:13:19.000000 types-setuptools-68.0.0.2/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-15 21:13:19.000000 types-setuptools-68.0.0.2/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:13:19.000000 types-setuptools-68.0.0.2/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-15 21:13:19.000000 types-setuptools-68.0.0.2/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.261661 types-setuptools-68.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-07-20 15:16:58.000000 types-setuptools-68.0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:58.000000 types-setuptools-68.0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-20 15:16:59.261661 types-setuptools-68.0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.245661 types-setuptools-68.0.0.3/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 15:16:58.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.241661 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.245661 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/specifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:59.261661 types-setuptools-68.0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-20 15:16:58.000000 types-setuptools-68.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.249661 types-setuptools-68.0.0.3/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 15:16:58.000000 types-setuptools-68.0.0.3/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.253661 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.253661 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/_distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.257661 types-setuptools-68.0.0.3/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.257661 types-setuptools-68.0.0.3/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.257661 types-setuptools-68.0.0.3/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/py312compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 15:15:13.000000 types-setuptools-68.0.0.3/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:59.257661 types-setuptools-68.0.0.3/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-20 15:16:59.000000 types-setuptools-68.0.0.3/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-20 15:16:59.000000 types-setuptools-68.0.0.3/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:59.000000 types-setuptools-68.0.0.3/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:16:59.000000 types-setuptools-68.0.0.3/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-68.0.0.2/CHANGELOG.md` & `types-setuptools-68.0.0.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 68.0.0.3 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 68.0.0.2 (2023-07-15)
 
 Add stubs for `pkg_resources._vendor.packaging` (#10423)
 
 ## 68.0.0.1 (2023-07-04)
 
 Bring back a few setuptools._distutils files (#10401)
```

### Comparing `types-setuptools-68.0.0.2/PKG-INFO` & `types-setuptools-68.0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 68.0.0.2
+Version: 68.0.0.3
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `47fc8362593cf29b160a3b19ddca3c8bdaf1f917` and was tested
-with mypy 1.4.1, pyright 1.1.317, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-setuptools-68.0.0.2/pkg_resources-stubs/__init__.pyi` & `types-setuptools-68.0.0.3/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/markers.pyi` & `types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/markers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/specifiers.pyi` & `types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/specifiers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/pkg_resources-stubs/_vendor/packaging/version.pyi` & `types-setuptools-68.0.0.3/pkg_resources-stubs/_vendor/packaging/version.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setup.py` & `types-setuptools-68.0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `47fc8362593cf29b160a3b19ddca3c8bdaf1f917` and was tested
-with mypy 1.4.1, pyright 1.1.317, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="68.0.0.2",
+      version="68.0.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
```

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/__init__.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/archive_util.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/ccompiler.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/sysconfig.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/_distutils/util.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/_distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/archive_util.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/build_meta.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/build_py.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/develop.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/editable_wheel.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/sdist.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/setopt.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/test.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/config/expand.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/depends.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/discovery.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/dist.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/errors.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/extension.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/msvc.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/package_index.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/setuptools-stubs/sandbox.pyi` & `types-setuptools-68.0.0.3/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-68.0.0.2/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-68.0.0.3/types_setuptools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 68.0.0.2
+Version: 68.0.0.3
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `47fc8362593cf29b160a3b19ddca3c8bdaf1f917` and was tested
-with mypy 1.4.1, pyright 1.1.317, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-setuptools-68.0.0.2/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-68.0.0.3/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

