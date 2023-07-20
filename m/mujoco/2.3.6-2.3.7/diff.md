# Comparing `tmp/mujoco-2.3.6.tar.gz` & `tmp/mujoco-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-2.3.6.tar", last modified: Tue Jun 20 17:18:03 2023, max compression
+gzip compressed data, was "mujoco-2.3.7.tar", last modified: Thu Jul 20 09:17:45 2023, max compression
```

## Comparing `mujoco-2.3.6.tar` & `mujoco-2.3.7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.050249 mujoco-2.3.6/
--rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-06-20 17:18:02.000000 mujoco-2.3.6/LICENSE
--rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-06-20 17:18:02.000000 mujoco-2.3.6/LICENSES_THIRD_PARTY.md
--rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-06-20 17:18:02.000000 mujoco-2.3.6/MANIFEST.in
--rw-r--r--   0 jenkins    (502) staff       (20)    34962 2023-06-20 17:18:03.050111 mujoco-2.3.6/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2994 2023-06-20 17:18:02.000000 mujoco-2.3.6/README.md
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.039011 mujoco-2.3.6/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/CheckAvxSupport.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/FindOrFetch.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoHarden.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoLinkOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1568 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoMacOS.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/ShellTests.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/TargetAddRpath.cmake
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.043945 mujoco-2.3.6/mujoco/
--rw-r--r--   0 jenkins    (502) staff       (20)    13479 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    50462 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/bindings_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/callbacks.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.044894 mujoco-2.3.6/mujoco/cgl/
--rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/cgl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/cgl/cgl.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/constants.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.045145 mujoco-2.3.6/mujoco/egl/
--rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/egl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/egl/egl_ext.py
--rw-r--r--   0 jenkins    (502) staff       (20)    31952 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/enum_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/enums.cc
--rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/errors.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7571 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/errors.h
--rw-r--r--   0 jenkins    (502) staff       (20)   127064 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/function_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)    53742 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/functions.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/functions.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/gl_context.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.045283 mujoco-2.3.6/mujoco/glfw/
--rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/glfw/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexer_xmacro.h
--rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexers.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexers.h
--rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjdata_meta.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.046277 mujoco-2.3.6/mujoco/mjpython/
--rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/Info.plist
--rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.icns
--rw-r--r--   0 jenkins    (502) staff       (20)    12145 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.046404 mujoco-2.3.6/mujoco/osmesa/
--rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/osmesa/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     1032 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/private.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/raw.h
--rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/render.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/render_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/renderer.py
--rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/renderer_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout.py
--rw-r--r--   0 jenkins    (502) staff       (20)    18157 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/serialization.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.048271 mujoco-2.3.6/mujoco/simulate/
--rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/array_safety.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.048541 mujoco-2.3.6/mujoco/simulate/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/cmake/SimulateDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/cmake/SimulateOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     7725 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_corevideo.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_corevideo.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_dispatch.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_dispatch.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/macos_gui.mm
--rw-r--r--   0 jenkins    (502) staff       (20)    14298 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/main.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     6095 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3319 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)    79042 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     8995 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/simulate.h
--rw-r--r--   0 jenkins    (502) staff       (20)     6913 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    71515 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/structs.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    31373 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/structs.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.049891 mujoco-2.3.6/mujoco/util/
--rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/array_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/array_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/crossplatform.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_wrap.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_wrap_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/tuple_tools.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/tuple_tools_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    12239 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/viewer.py
--rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/viewer_test.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.044627 mujoco-2.3.6/mujoco.egg-info/
--rw-r--r--   0 jenkins    (502) staff       (20)    34962 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2147 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/requires.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-06-20 17:18:03.050283 mujoco-2.3.6/setup.cfg
--rw-r--r--   0 jenkins    (502) staff       (20)    14312 2023-06-20 17:18:02.000000 mujoco-2.3.6/setup.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.046399 mujoco-2.3.7/
+-rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-07-20 09:17:44.000000 mujoco-2.3.7/LICENSE
+-rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-07-20 09:17:44.000000 mujoco-2.3.7/LICENSES_THIRD_PARTY.md
+-rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-07-20 09:17:44.000000 mujoco-2.3.7/MANIFEST.in
+-rw-r--r--   0 jenkins    (502) staff       (20)    34912 2023-07-20 09:17:45.046255 mujoco-2.3.7/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2994 2023-07-20 09:17:44.000000 mujoco-2.3.7/README.md
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.036615 mujoco-2.3.7/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/CheckAvxSupport.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/FindOrFetch.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/MujocoDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/MujocoHarden.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/MujocoLinkOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1789 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/MujocoMacOS.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/MujocoOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/ShellTests.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-07-20 09:17:44.000000 mujoco-2.3.7/cmake/TargetAddRpath.cmake
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.040645 mujoco-2.3.7/mujoco/
+-rw-r--r--   0 jenkins    (502) staff       (20)    13503 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    50950 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/bindings_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/callbacks.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.041429 mujoco-2.3.7/mujoco/cgl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/cgl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/cgl/cgl.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/constants.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.041658 mujoco-2.3.7/mujoco/egl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/egl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/egl/egl_ext.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    32027 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/enum_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/enums.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/errors.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7571 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/errors.h
+-rw-r--r--   0 jenkins    (502) staff       (20)   128565 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/function_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    53882 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/functions.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/functions.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/gl_context.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.041857 mujoco-2.3.7/mujoco/glfw/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/glfw/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/indexer_xmacro.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/indexers.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/indexers.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/mjdata_meta.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.042612 mujoco-2.3.7/mujoco/mjpython/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/mjpython/Info.plist
+-rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/mjpython/mjpython.icns
+-rw-r--r--   0 jenkins    (502) staff       (20)    10942 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/mjpython/mjpython.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/mjpython/mjpython.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.042727 mujoco-2.3.7/mujoco/osmesa/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/osmesa/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     1032 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/private.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/raw.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/render.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/render_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/renderer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/renderer_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/rollout.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/rollout.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    18157 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/rollout_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/serialization.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.044319 mujoco-2.3.7/mujoco/simulate/
+-rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/array_safety.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.044537 mujoco-2.3.7/mujoco/simulate/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/cmake/SimulateDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/cmake/SimulateOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     7745 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_corevideo.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_corevideo.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_dispatch.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/glfw_dispatch.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/macos_gui.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)    14298 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/main.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     6119 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/platform_ui_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3378 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/platform_ui_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    80185 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     9241 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate/simulate.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    11098 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    71515 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/structs.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    31373 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/structs.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.046028 mujoco-2.3.7/mujoco/util/
+-rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/array_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/array_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/crossplatform.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/func_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/func_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/func_wrap.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/func_wrap_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/tuple_tools.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/util/tuple_tools_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    13230 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/viewer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-07-20 09:17:44.000000 mujoco-2.3.7/mujoco/viewer_test.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-07-20 09:17:45.041210 mujoco-2.3.7/mujoco.egg-info/
+-rw-r--r--   0 jenkins    (502) staff       (20)    34912 2023-07-20 09:17:45.000000 mujoco-2.3.7/mujoco.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2147 2023-07-20 09:17:45.000000 mujoco-2.3.7/mujoco.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-07-20 09:17:45.000000 mujoco-2.3.7/mujoco.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-07-20 09:17:45.000000 mujoco-2.3.7/mujoco.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-07-20 09:17:45.000000 mujoco-2.3.7/mujoco.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-07-20 09:17:45.046431 mujoco-2.3.7/setup.cfg
+-rw-r--r--   0 jenkins    (502) staff       (20)    14263 2023-07-20 09:17:44.000000 mujoco-2.3.7/setup.py
```

### Comparing `mujoco-2.3.6/LICENSE` & `mujoco-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/LICENSES_THIRD_PARTY.md` & `mujoco-2.3.7/LICENSES_THIRD_PARTY.md`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/PKG-INFO` & `mujoco-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.6
+Version: 2.3.7
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
 Author: Google DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSES_THIRD_PARTY.md
 
 # MuJoCo Python Bindings
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
```

### Comparing `mujoco-2.3.6/README.md` & `mujoco-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/CheckAvxSupport.cmake` & `mujoco-2.3.7/cmake/CheckAvxSupport.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/FindOrFetch.cmake` & `mujoco-2.3.7/cmake/FindOrFetch.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/MujocoDependencies.cmake` & `mujoco-2.3.7/cmake/MujocoDependencies.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Build configuration for third party libraries used in MuJoCo.
 
-# Override the BUILD_SHARED_LIBS setting, just for building third party libs (since we always want
-# static libraries). The ccd CMakeLists.txt doesn't expose an option to build a static ccd library,
-# unless BUILD_SHARED_LIBS is set.
-
 set(MUJOCO_DEP_VERSION_lodepng
     b4ed2cd7ecf61d29076169b49199371456d4f90b
     CACHE STRING "Version of `lodepng` to be fetched."
 )
 set(MUJOCO_DEP_VERSION_tinyxml2
     9a89766acc42ddfa9e7133c7d81a5bda108a0ade
     CACHE STRING "Version of `tinyxml2` to be fetched."
@@ -35,15 +31,15 @@
     CACHE STRING "Version of `ccd` to be fetched."
 )
 set(MUJOCO_DEP_VERSION_qhull
     0c8fc90d2037588024d9964515c1e684f6007ecc
     CACHE STRING "Version of `qhull` to be fetched."
 )
 set(MUJOCO_DEP_VERSION_Eigen3
-    969c31eefcdfaab11da763bea3f7502086673ab0
+    211c5dfc6741a5570ad007983c113ef4d144f9f3
     CACHE STRING "Version of `Eigen3` to be fetched."
 )
 
 set(MUJOCO_DEP_VERSION_abseil
     c2435f8342c2d0ed8101cb43adfd605fdc52dca2 # LTS 20230125.3
     CACHE STRING "Version of `abseil` to be fetched."
 )
@@ -67,14 +63,18 @@
 mark_as_advanced(MUJOCO_DEP_VERSION_abseil)
 mark_as_advanced(MUJOCO_DEP_VERSION_gtest)
 mark_as_advanced(MUJOCO_DEP_VERSION_benchmark)
 
 include(FetchContent)
 include(FindOrFetch)
 
+# Override the BUILD_SHARED_LIBS setting, just for building third party libs (since we always want
+# static libraries). The ccd CMakeLists.txt doesn't expose an option to build a static ccd library,
+# unless BUILD_SHARED_LIBS is set.
+
 # We force all the dependencies to be compiled as static libraries.
 # TODO(fraromano) Revisit this choice when adding support for install.
 set(BUILD_SHARED_LIBS_OLD ${BUILD_SHARED_LIBS})
 set(BUILD_SHARED_LIBS
     OFF
     CACHE INTERNAL "Build SHARED libraries"
 )
```

### Comparing `mujoco-2.3.6/cmake/MujocoHarden.cmake` & `mujoco-2.3.7/cmake/MujocoHarden.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/MujocoLinkOptions.cmake` & `mujoco-2.3.7/cmake/MujocoLinkOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/MujocoMacOS.cmake` & `mujoco-2.3.7/cmake/MujocoMacOS.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 if(APPLE)
-  # 10.12 is the oldest version of macOS that supports C++17, launched 2016.
-  set(MUJOCO_MACOSX_VERSION_MIN 10.12)
+  # Target the oldest version of macOS that is still supported by Apple.
+  # We follow https://endoflife.date/macos, which considers a version to become
+  # unsupported the first time it is excluded from a macOS security update
+  # (e.g. https://github.com/endoflife-date/endoflife.date/issues/1602).
+  set(MUJOCO_MACOSX_VERSION_MIN 11)
 
   # We are setting the -mmacosx-version-min compiler flag directly rather than using the
   # CMAKE_OSX_DEPLOYMENT_TARGET variable since we do not want to affect choice of SDK,
   # and also we only want to apply the version restriction locally.
   set(MUJOCO_MACOS_COMPILE_OPTIONS -mmacosx-version-min=${MUJOCO_MACOSX_VERSION_MIN}
                                    -Werror=partial-availability -Werror=unguarded-availability
   )
```

### Comparing `mujoco-2.3.6/cmake/MujocoOptions.cmake` & `mujoco-2.3.7/cmake/MujocoOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/ShellTests.cmake` & `mujoco-2.3.7/cmake/ShellTests.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/cmake/TargetAddRpath.cmake` & `mujoco-2.3.7/cmake/TargetAddRpath.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/CMakeLists.txt` & `mujoco-2.3.7/mujoco/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -80,23 +80,23 @@
     # On macOS, check if we are using mujoco.framework first.
     # Framework headers are searched differently from normal headers.
     # We need to use -F instead of the usual target_include_directories.
     find_path(MUJOCO_FRAMEWORK mujoco.Framework HINTS ${MUJOCO_FRAMEWORK_DIR})
     if(MUJOCO_FRAMEWORK)
       message("MuJoCo framework is at ${MUJOCO_FRAMEWORK}/mujoco.framework")
       set(MUJOCO_LIBRARY
-          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.6.dylib
+          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.7.dylib
       )
       target_compile_options(mujoco INTERFACE -F${MUJOCO_FRAMEWORK})
     endif()
   endif()
 
   if(NOT MUJOCO_FRAMEWORK)
     find_library(
-      MUJOCO_LIBRARY mujoco mujoco.2.3.6 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
+      MUJOCO_LIBRARY mujoco mujoco.2.3.7 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
     )
     find_path(MUJOCO_INCLUDE mujoco/mujoco.h HINTS ${MUJOCO_INCLUDE_DIR} REQUIRED)
     message("MuJoCo is at ${MUJOCO_LIBRARY}")
     message("MuJoCo headers are at ${MUJOCO_INCLUDE}")
     target_include_directories(mujoco INTERFACE "${MUJOCO_INCLUDE}")
   endif()
 
@@ -169,15 +169,15 @@
   PACKAGE_NAME
   Eigen3
   LIBRARY_NAME
   eigen
   GIT_REPO
   https://gitlab.com/libeigen/eigen
   GIT_TAG
-  969c31eefcdfaab11da763bea3f7502086673ab0
+  211c5dfc6741a5570ad007983c113ef4d144f9f3
   TARGETS
   Eigen3::Eigen
   EXCLUDE_FROM_ALL
 )
 
 # ==================== PYBIND11 ================================================
 findorfetch(
@@ -186,15 +186,15 @@
   PACKAGE_NAME
   pybind11
   LIBRARY_NAME
   pybind11
   GIT_REPO
   https://github.com/pybind/pybind11
   GIT_TAG
-  5b0a6fc2017fcc176545afe3e09c9f9885283242 # v2.10.4
+  8a099e44b3d5f85b20f05828d919d2332a8de841 # v2.11.1
   TARGETS
   pybind11::pybind11_headers
   EXCLUDE_FROM_ALL
 )
 
 # ==================== MUJOCO PYTHON BINDINGS ==================================
 set(SIMULATE_BUILD_EXECUTABLE OFF)
@@ -401,14 +401,15 @@
 )
 
 mujoco_pybind11_module(_simulate simulate.cc)
 target_link_libraries(
   _simulate
   PRIVATE mujoco
           mujoco::libsimulate
+          errors_header
           raw
           structs_header
 )
 
 set(LIBRARIES_FOR_WHEEL
     "$<TARGET_FILE:_callbacks>"
     "$<TARGET_FILE:_constants>"
```

### Comparing `mujoco-2.3.6/mujoco/__init__.py` & `mujoco-2.3.7/mujoco/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/bindings_test.py` & `mujoco-2.3.7/mujoco/bindings_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1109,14 +1109,29 @@
     self.assertGreater(np.linalg.norm(df_dq), eps)
     self.assertGreater(np.linalg.norm(df_dv), eps)
     self.assertGreater(np.linalg.norm(df_da), eps)
     self.assertGreater(np.linalg.norm(ds_dq), eps)
     self.assertGreater(np.linalg.norm(ds_dv), eps)
     self.assertGreater(np.linalg.norm(ds_da), eps)
 
+  def test_mjd_sub_quat(self):
+    quat1 = np.array((0.2, 0.3, 0.3, 0.4))
+    quat2 = np.array((0.2, 0.3, 0.3, 0.4))
+    d1 = np.empty(9, np.float64)
+    d2 = np.empty(9, np.float64)
+    mujoco.mjd_subQuat(quat1, quat2, d1, d2)
+
+  def test_mjd_quat_intergrate(self):
+    scale = 0.1
+    vel = np.array((0.2, 0.3, 0.3))
+    d_quat = np.empty(9, np.float64)
+    d_vel = np.empty(9, np.float64)
+    d_h = np.empty(3, np.float64)
+    mujoco.mjd_quatIntegrate(vel, scale, d_quat, d_vel, d_h)
+
   def test_banded(self):
     n_total = 4
     n_band = 1
     n_dense = 1
     dense = np.array([[1.0, 0, 0, 0.1],
                       [0, 2.0, 0, 0.2],
                       [0, 0, 3.0, 0.3],
```

### Comparing `mujoco-2.3.6/mujoco/callbacks.cc` & `mujoco-2.3.7/mujoco/callbacks.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/cgl/__init__.py` & `mujoco-2.3.7/mujoco/cgl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/cgl/cgl.py` & `mujoco-2.3.7/mujoco/cgl/cgl.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/constants.cc` & `mujoco-2.3.7/mujoco/constants.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/egl/__init__.py` & `mujoco-2.3.7/mujoco/egl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/egl/egl_ext.py` & `mujoco-2.3.7/mujoco/egl/egl_ext.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/enum_traits.h` & `mujoco-2.3.7/mujoco/enum_traits.h`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,15 @@
     std::make_pair("mjSENS_JOINTPOS", ::mjtSensor::mjSENS_JOINTPOS),
     std::make_pair("mjSENS_JOINTVEL", ::mjtSensor::mjSENS_JOINTVEL),
     std::make_pair("mjSENS_TENDONPOS", ::mjtSensor::mjSENS_TENDONPOS),
     std::make_pair("mjSENS_TENDONVEL", ::mjtSensor::mjSENS_TENDONVEL),
     std::make_pair("mjSENS_ACTUATORPOS", ::mjtSensor::mjSENS_ACTUATORPOS),
     std::make_pair("mjSENS_ACTUATORVEL", ::mjtSensor::mjSENS_ACTUATORVEL),
     std::make_pair("mjSENS_ACTUATORFRC", ::mjtSensor::mjSENS_ACTUATORFRC),
+    std::make_pair("mjSENS_JOINTACTFRC", ::mjtSensor::mjSENS_JOINTACTFRC),
     std::make_pair("mjSENS_BALLQUAT", ::mjtSensor::mjSENS_BALLQUAT),
     std::make_pair("mjSENS_BALLANGVEL", ::mjtSensor::mjSENS_BALLANGVEL),
     std::make_pair("mjSENS_JOINTLIMITPOS", ::mjtSensor::mjSENS_JOINTLIMITPOS),
     std::make_pair("mjSENS_JOINTLIMITVEL", ::mjtSensor::mjSENS_JOINTLIMITVEL),
     std::make_pair("mjSENS_JOINTLIMITFRC", ::mjtSensor::mjSENS_JOINTLIMITFRC),
     std::make_pair("mjSENS_TENDONLIMITPOS", ::mjtSensor::mjSENS_TENDONLIMITPOS),
     std::make_pair("mjSENS_TENDONLIMITVEL", ::mjtSensor::mjSENS_TENDONLIMITVEL),
```

### Comparing `mujoco-2.3.6/mujoco/enums.cc` & `mujoco-2.3.7/mujoco/enums.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/errors.cc` & `mujoco-2.3.7/mujoco/errors.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/errors.h` & `mujoco-2.3.7/mujoco/errors.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/function_traits.h` & `mujoco-2.3.7/mujoco/function_traits.h`

 * *Files 0% similar despite different names*

```diff
@@ -1626,23 +1626,34 @@
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return *reinterpret_cast<type*>(&::mjv_initGeom);
   }
 };
 
 struct mjv_makeConnector {
   static constexpr char name[] = "mjv_makeConnector";
-  static constexpr char doc[] = "Set (type, size, pos, mat) for connector-type geom between given points. Assume that mjv_initGeom was already called to set all other properties. Width of mjGEOM_LINE is denominated in pixels.";
+  static constexpr char doc[] = "Set (type, size, pos, mat) for connector-type geom between given points. Assume that mjv_initGeom was already called to set all other properties. Width of mjGEOM_LINE is denominated in pixels. Deprecated: use mjv_connector.";
   using type = void (mjvGeom *, int, mjtNum, mjtNum, mjtNum, mjtNum, mjtNum, mjtNum, mjtNum);
   static constexpr auto param_names = std::make_tuple("geom", "type", "width", "a0", "a1", "a2", "b0", "b1", "b2");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mjv_makeConnector;
   }
 };
 
+struct mjv_connector {
+  static constexpr char name[] = "mjv_connector";
+  static constexpr char doc[] = "Set (type, size, pos, mat) for connector-type geom between given points. Assume that mjv_initGeom was already called to set all other properties. Width of mjGEOM_LINE is denominated in pixels.";
+  using type = void (mjvGeom *, int, mjtNum, const mjtNum (*)[3], const mjtNum (*)[3]);
+  static constexpr auto param_names = std::make_tuple("geom", "type", "width", "from", "to");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return *reinterpret_cast<type*>(&::mjv_connector);
+  }
+};
+
 struct mjv_defaultScene {
   static constexpr char name[] = "mjv_defaultScene";
   static constexpr char doc[] = "Set default abstract scene.";
   using type = void (mjvScene *);
   static constexpr auto param_names = std::make_tuple("scn");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
@@ -3351,14 +3362,36 @@
   static constexpr auto param_names = std::make_tuple("m", "d", "eps", "flg_actuation", "DfDq", "DfDv", "DfDa", "DsDq", "DsDv", "DsDa", "DmDq");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mjd_inverseFD;
   }
 };
 
+struct mjd_subQuat {
+  static constexpr char name[] = "mjd_subQuat";
+  static constexpr char doc[] = "Derivatives of mju_subQuat.";
+  using type = void (const mjtNum (*)[4], const mjtNum (*)[4], mjtNum (*)[9], mjtNum (*)[9]);
+  static constexpr auto param_names = std::make_tuple("qa", "qb", "Da", "Db");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return *reinterpret_cast<type*>(&::mjd_subQuat);
+  }
+};
+
+struct mjd_quatIntegrate {
+  static constexpr char name[] = "mjd_quatIntegrate";
+  static constexpr char doc[] = "Derivatives of mju_quatIntegrate.";
+  using type = void (const mjtNum (*)[3], mjtNum, mjtNum (*)[9], mjtNum (*)[9], mjtNum (*)[3]);
+  static constexpr auto param_names = std::make_tuple("vel", "scale", "Dquat", "Dvel", "Dscale");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return *reinterpret_cast<type*>(&::mjd_quatIntegrate);
+  }
+};
+
 struct mjp_defaultPlugin {
   static constexpr char name[] = "mjp_defaultPlugin";
   static constexpr char doc[] = "Set default plugin definition.";
   using type = void (mjpPlugin *);
   static constexpr auto param_names = std::make_tuple("plugin");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
```

### Comparing `mujoco-2.3.6/mujoco/functions.cc` & `mujoco-2.3.7/mujoco/functions.cc`

 * *Files 0% similar despite different names*

```diff
@@ -598,14 +598,15 @@
   Def<traits::mjv_select>(pymodule);
 
   // Visualization
   Def<traits::mjv_defaultOption>(pymodule);
   Def<traits::mjv_defaultFigure>(pymodule);
   Def<traits::mjv_initGeom>(pymodule);
   Def<traits::mjv_makeConnector>(pymodule);
+  Def<traits::mjv_connector>(pymodule);
   // Skipped: mjv_defaultScene (have MjvScene.__init__, memory managed by
   // MjvScene).
   // Skipped: mjv_makeScene (have MjvScene.__init__)
   // Skipped: mjv_freeScene (have MjvScene.__del__)
   Def<traits::mjv_updateScene>(
       pymodule,
       [](const raw::MjModel* m, raw::MjData* d, const raw::MjvOption* opt,
@@ -1234,14 +1235,19 @@
       });
   DEF_WITH_OMITTED_PY_ARGS(traits::mju_insertionSortInt, "n")(
       pymodule,
       [](Eigen::Ref<Eigen::Vector<int, Eigen::Dynamic>> res) {
         return InterceptMjErrors(::mju_insertionSortInt)(
             res.data(), res.size());
       });
+  Def<traits::mju_Halton>(pymodule);
+  // Skipped: mju_strncpy (doesn't make sense in Python)
+  Def<traits::mju_sigmoid>(pymodule);
+
+  // Derivatives
   Def<traits::mjd_transitionFD>(
       pymodule,
       [](const raw::MjModel* m, raw::MjData* d,
          mjtNum eps, mjtByte flg_centered,
          std::optional<Eigen::Ref<EigenArrayXX>> A,
          std::optional<Eigen::Ref<EigenArrayXX>> B,
          std::optional<Eigen::Ref<EigenArrayXX>> C,
@@ -1314,13 +1320,12 @@
             DfDv.has_value() ? DfDv->data() : nullptr,
             DfDa.has_value() ? DfDa->data() : nullptr,
             DsDq.has_value() ? DsDq->data() : nullptr,
             DsDv.has_value() ? DsDv->data() : nullptr,
             DsDa.has_value() ? DsDa->data() : nullptr,
             DmDq.has_value() ? DmDq->data() : nullptr);
       });
-  Def<traits::mju_Halton>(pymodule);
-  // Skipped: mju_strncpy (doesn't make sense in Python)
-  Def<traits::mju_sigmoid>(pymodule);
+  Def<traits::mjd_subQuat>(pymodule);
+  Def<traits::mjd_quatIntegrate>(pymodule);
 }  // PYBIND11_MODULE NOLINT(readability/fn_size)
 }  // namespace
 }  // namespace mujoco::python
```

### Comparing `mujoco-2.3.6/mujoco/functions.h` & `mujoco-2.3.7/mujoco/functions.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/gl_context.py` & `mujoco-2.3.7/mujoco/gl_context.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/glfw/__init__.py` & `mujoco-2.3.7/mujoco/glfw/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/indexer_xmacro.h` & `mujoco-2.3.7/mujoco/indexer_xmacro.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/indexers.cc` & `mujoco-2.3.7/mujoco/indexers.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/indexers.h` & `mujoco-2.3.7/mujoco/indexers.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/mjdata_meta.h` & `mujoco-2.3.7/mujoco/mjdata_meta.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/mjpython/Info.plist` & `mujoco-2.3.7/mujoco/mjpython/Info.plist`

 * *Files 19% similar despite different names*

#### Comparing `mujoco-2.3.6/mujoco/mjpython/Info.plist` & `mujoco-2.3.7/mujoco/mjpython/Info.plist`

```diff
@@ -5,21 +5,21 @@
 <plist version="1.0">
   <dict>
     <key>CFBundleName</key>
     <string>mjpython</string>
     <key>CFBundleIdentifier</key>
     <string>org.mujoco.mjpython</string>
     <key>CFBundleVersion</key>
-    <string>2.3.6</string>
+    <string>2.3.7</string>
     <key>CFBundleGetInfoString</key>
-    <string>2.3.6</string>
+    <string>2.3.7</string>
     <key>CFBundleLongVersionString</key>
-    <string>2.3.6</string>
+    <string>2.3.7</string>
     <key>CFBundleShortVersionString</key>
-    <string>2.3.6</string>
+    <string>2.3.7</string>
     <key>CFBundleExecutable</key>
     <string>mjpython</string>
     <key>CFBundleIconFile</key>
     <string>mjpython.icns</string>
     <key>CFBundlePackageType</key>
     <string>APPL</string>
     <key>NSHumanReadableCopyright</key>
```

### Comparing `mujoco-2.3.6/mujoco/mjpython/mjpython.icns` & `mujoco-2.3.7/mujoco/mjpython/mjpython.icns`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/mjpython/mjpython.mm` & `mujoco-2.3.7/mujoco/mjpython/mjpython.mm`

 * *Files 8% similar despite different names*

```diff
@@ -38,46 +38,32 @@
   [NSApp setActivationPolicy:NSApplicationActivationPolicyAccessory];
 }
 __attribute__((used)) void mjpython_show_dock_icon() {
   [NSApp setActivationPolicy:NSApplicationActivationPolicyRegular];
 }
 }  // extern "C"
 
-// TODO(b/273744079): Remove Python 3.7 code after end-of-life (27 Jun 2023).
 namespace {
 // 16MiB is the default Python thread stack size on macOS as of Python 3.11
 // https://bugs.python.org/issue18075
 constexpr rlim_t kThreadStackSize = 0x1000000;
 
 struct {
 #define CPYTHON_FN(fname) decltype(&::fname) fname
 
-#if PY_MINOR_VERSION >= 8
   // go/keep-sorted start
   CPYTHON_FN(PyConfig_Clear);
   CPYTHON_FN(PyConfig_InitPythonConfig);
   CPYTHON_FN(PyConfig_SetBytesArgv);
-  CPYTHON_FN(Py_InitializeFromConfig);
-  CPYTHON_FN(Py_RunMain);
-  // go/keep-sorted end
-#else
-  // go/keep-sorted start
-  CPYTHON_FN(PyMem_RawFree);
-  CPYTHON_FN(Py_DecodeLocale);
-  CPYTHON_FN(Py_Initialize);
-  CPYTHON_FN(Py_Main);
-  CPYTHON_FN(Py_SetProgramName);
-  // go/keep-sorted end
-#endif
-
-  // go/keep-sorted start
   CPYTHON_FN(PyGILState_Ensure);
   CPYTHON_FN(PyGILState_Release);
   CPYTHON_FN(PyRun_SimpleStringFlags);
   CPYTHON_FN(Py_FinalizeEx);
+  CPYTHON_FN(Py_InitializeFromConfig);
+  CPYTHON_FN(Py_RunMain);
   // go/keep-sorted end
 
 #undef CPYTHON_FN
 } cpython;
 
 std::atomic_bool py_initialized = false;
 
@@ -88,29 +74,19 @@
 
 // The Python main thread (distinct from the macOS main thread, which executes the main function).
 void* mjpython_pymain(void* vargs) {
   Args* args = static_cast<Args*>(vargs);
   PyGILState_STATE gil;
 
   // Initialize the Python interpreter.
-#if PY_MINOR_VERSION >= 8
   PyConfig config;
   cpython.PyConfig_InitPythonConfig(&config);
   cpython.PyConfig_SetBytesArgv(&config, args->argc, args->argv);
   cpython.Py_InitializeFromConfig(&config);
   cpython.PyConfig_Clear(&config);
-#else
-  // Convert each argv to wchar_t* (needed for Py_Main).
-  wchar_t** wargv = static_cast<wchar_t**>(std::calloc(args->argc, sizeof(wchar_t*)));
-  for (int i = 0; i < args->argc; ++i) {
-    wargv[i] = cpython.Py_DecodeLocale(args->argv[i], nullptr);
-  }
-  cpython.Py_SetProgramName(wargv[0]);
-  cpython.Py_Initialize();
-#endif
 
   // Set up the condition variable to pass control back to the macOS main thread.
   gil = cpython.PyGILState_Ensure();
   cpython.PyRun_SimpleStringFlags("import threading; cond = threading.Condition()", nullptr);
   py_initialized.store(true);
 
   // Wait until GLFW is initialized on macOS main thread, set up the queue and an atexit hook
@@ -135,20 +111,20 @@
 
   def __init__(self):
     self._cond = threading.Condition()
     self._task = None
     self._termination = self.__class__.NOT_TERMINATED
     self._busy = False
 
-  def launch_on_ui_thread(self, model, data, handle_return):
+  def launch_on_ui_thread(self, model, data, handle_return, key_callback):
     with self._cond:
       if self._busy or self._task is not None:
         raise RuntimeError('another MuJoCo viewer is already open')
       else:
-        self._task = (model, data, handle_return)
+        self._task = (model, data, handle_return, key_callback)
         self._cond.notify()
 
   def terminate(self):
     with self._cond:
       self._termination = self.__class__.TERMINATION_REQUESTED
       self._cond.notify()
       self._cond.wait_for(
@@ -183,30 +159,18 @@
 
 with cond:
   cond.notify()
 del cond  # Don't pollute globals for user script.
 )", nullptr);
 
   // Run the Python interpreter main loop.
-#if PY_MINOR_VERSION >= 8
   cpython.Py_RunMain();
-#else
-  cpython.Py_Main(args->argc, wargv);
-#endif
 
   // Tear down the interpreter.
   cpython.Py_FinalizeEx();
-#if PY_MINOR_VERSION < 8
-  for (int i = 0; i < args->argc; ++i) {
-    cpython.PyMem_RawFree(wargv[i]);
-    wargv[i] = nullptr;
-  }
-  std::free(wargv);
-  wargv = nullptr;
-#endif
   return nullptr;
 }
 }  // namespace
 
 int main(int argc, char** argv) {
   const char* libpython_path = getenv("MJPYTHON_LIBPYTHON");
   if (!libpython_path || !libpython_path[0]) {
@@ -256,37 +220,24 @@
     cpython.fname = reinterpret_cast<decltype(cpython.fname)>(dlsym(libpython, #fname)); \
     if (!cpython.fname) {                                                                \
       std::cerr << "failed to dlsym '" << #fname << "': " << dlerror() << "\n";          \
       return EXIT_FAILURE;                                                               \
     }                                                                                    \
   }
 
-#if PY_MINOR_VERSION >= 8
   // go/keep-sorted start
   CPYTHON_INITFN(PyConfig_Clear);
   CPYTHON_INITFN(PyConfig_InitPythonConfig);
   CPYTHON_INITFN(PyConfig_SetBytesArgv);
-  CPYTHON_INITFN(Py_InitializeFromConfig);
-  CPYTHON_INITFN(Py_RunMain);
-  // go/keep-sorted end
-#else
-  // go/keep-sorted start
-  CPYTHON_INITFN(PyMem_RawFree);
-  CPYTHON_INITFN(Py_DecodeLocale);
-  CPYTHON_INITFN(Py_Initialize);
-  CPYTHON_INITFN(Py_Main);
-  CPYTHON_INITFN(Py_SetProgramName);
-  // go/keep-sorted end
-#endif
-
-  // go/keep-sorted start
   CPYTHON_INITFN(PyGILState_Ensure);
   CPYTHON_INITFN(PyGILState_Release);
   CPYTHON_INITFN(PyRun_SimpleStringFlags);
   CPYTHON_INITFN(Py_FinalizeEx);
+  CPYTHON_INITFN(Py_InitializeFromConfig);
+  CPYTHON_INITFN(Py_RunMain);
   // go/keep-sorted end
 
 #undef CPYTHON_INITFN
 
   // Package up argc and argv together to pass to pthread_create.
   Args args{argc, argv};
 
@@ -339,18 +290,19 @@
 
     # None means that we are exiting.
     if task is None:
       glfw.terminate()
       break
 
     # Otherwise, launch the viewer.
-    model, data, handle_return = task
+    model, data, handle_return, key_callback = task
     ctypes.CDLL(None).mjpython_show_dock_icon()
     mujoco.viewer._launch_internal(
-        model, data, run_physics_thread=False, handle_return=handle_return)
+        model, data, run_physics_thread=False, handle_return=handle_return,
+        key_callback=key_callback)
     ctypes.CDLL(None).mjpython_hide_dock_icon()
 
   finally:
     mujoco.viewer._MJPYTHON.done()
 )", nullptr);
   cpython.PyGILState_Release(gil);
```

### Comparing `mujoco-2.3.6/mujoco/mjpython/mjpython.py` & `mujoco-2.3.7/mujoco/mjpython/mjpython.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/osmesa/__init__.py` & `mujoco-2.3.7/mujoco/osmesa/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/private.h` & `mujoco-2.3.7/mujoco/private.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/raw.h` & `mujoco-2.3.7/mujoco/raw.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/render.cc` & `mujoco-2.3.7/mujoco/render.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/render_test.py` & `mujoco-2.3.7/mujoco/render_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/renderer.py` & `mujoco-2.3.7/mujoco/renderer.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/renderer_test.py` & `mujoco-2.3.7/mujoco/renderer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/rollout.cc` & `mujoco-2.3.7/mujoco/rollout.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/rollout.py` & `mujoco-2.3.7/mujoco/rollout.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/rollout_test.py` & `mujoco-2.3.7/mujoco/rollout_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/serialization.h` & `mujoco-2.3.7/mujoco/serialization.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/CMakeLists.txt` & `mujoco-2.3.7/mujoco/simulate/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 set(MUJOCO_DEP_VERSION_lodepng
     b4ed2cd7ecf61d29076169b49199371456d4f90b
     CACHE STRING "Version of `lodepng` to be fetched."
 )
 
 project(
   mujoco_simulate
-  VERSION 2.3.6
+  VERSION 2.3.7
   DESCRIPTION "MuJoCo simulate binaries"
   HOMEPAGE_URL "https://mujoco.org"
 )
 
 enable_language(C)
 enable_language(CXX)
 if(APPLE)
```

### Comparing `mujoco-2.3.6/mujoco/simulate/array_safety.h` & `mujoco-2.3.7/mujoco/simulate/array_safety.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/cmake/SimulateDependencies.cmake` & `mujoco-2.3.7/mujoco/simulate/cmake/SimulateDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/cmake/SimulateOptions.cmake` & `mujoco-2.3.7/mujoco/simulate/cmake/SimulateOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_adapter.cc` & `mujoco-2.3.7/mujoco/simulate/glfw_adapter.cc`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
       });
 
   // make context current
   Glfw().glfwMakeContextCurrent(window_);
 }
 
 GlfwAdapter::~GlfwAdapter() {
+  FreeMjrContext();
   Glfw().glfwMakeContextCurrent(nullptr);
   Glfw().glfwDestroyWindow(window_);
 }
 
 std::pair<double, double> GlfwAdapter::GetCursorPosition() const {
   double x, y;
   Glfw().glfwGetCursorPos(window_, &x, &y);
```

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_adapter.h` & `mujoco-2.3.7/mujoco/simulate/glfw_adapter.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_corevideo.h` & `mujoco-2.3.7/mujoco/simulate/glfw_corevideo.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_corevideo.mm` & `mujoco-2.3.7/mujoco/simulate/glfw_corevideo.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_dispatch.cc` & `mujoco-2.3.7/mujoco/simulate/glfw_dispatch.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/glfw_dispatch.h` & `mujoco-2.3.7/mujoco/simulate/glfw_dispatch.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/macos_gui.mm` & `mujoco-2.3.7/mujoco/simulate/macos_gui.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/main.cc` & `mujoco-2.3.7/mujoco/simulate/main.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.cc` & `mujoco-2.3.7/mujoco/simulate/platform_ui_adapter.cc`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #include <chrono>
 
 namespace mujoco {
 PlatformUIAdapter::PlatformUIAdapter() {
   mjr_defaultContext(&con_);
 }
 
-PlatformUIAdapter::~PlatformUIAdapter() {
+void PlatformUIAdapter::FreeMjrContext() {
   mjr_freeContext(&con_);
 }
 
 bool PlatformUIAdapter::RefreshMjrContext(const mjModel* m, int fontscale) {
   if (m != last_model_ || fontscale != last_fontscale_) {
     mjr_makeContext(m, &con_, fontscale);
     last_model_ = m;
@@ -72,14 +72,16 @@
   state_.keytime = std::chrono::duration<double>(
       std::chrono::steady_clock::now().time_since_epoch()).count();
 
   // application-specific processing
   if (event_callback_) {
     event_callback_(&state_);
   }
+
+  last_key_ = mj_key;
 }
 
 void PlatformUIAdapter::OnMouseButton(int button, int act)  {
   // translate API-specific mouse button code
   mjtButton mj_button = TranslateMouseButton(button);
 
   // update state
```

### Comparing `mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.h` & `mujoco-2.3.7/mujoco/simulate/platform_ui_adapter.h`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #include <utility>
 
 #include <mujoco/mujoco.h>
 
 namespace mujoco {
 class PlatformUIAdapter {
  public:
-  virtual ~PlatformUIAdapter();
+  virtual ~PlatformUIAdapter() = default;
 
   inline mjuiState& state() { return state_; }
   inline const mjuiState& state() const { return state_; }
 
   inline mjrContext& mjr_context() { return con_; }
   inline const mjrContext& mjr_context() const { return con_; }
 
@@ -34,15 +34,15 @@
     event_callback_ = event_callback;
   }
 
   inline void SetLayoutCallback(void (*layout_callback)(mjuiState*)) {
     layout_callback_ = layout_callback;
   }
 
-  // Optionally overrideable function to (re)create an mjrContext for an mjModel
+  // Optionally overridable function to (re)create an mjrContext for an mjModel
   virtual bool RefreshMjrContext(const mjModel* m, int fontscale);
 
   virtual bool EnsureContextSize();
 
   // Pure virtual functions to be implemented by individual adapters
   virtual std::pair<double, double> GetCursorPosition() const = 0;
   virtual double GetDisplayPixelsPerInch() const = 0;
@@ -69,25 +69,27 @@
   virtual bool IsKeyDownEvent(int act) const = 0;
 
   virtual int TranslateKeyCode(int key) const = 0;
   virtual mjtButton TranslateMouseButton(int button) const = 0;
 
  protected:
   PlatformUIAdapter();
+  void FreeMjrContext();
 
   // Event handlers
   void OnFilesDrop(int count, const char** paths);
-  void OnKey(int key, int scancode, int act);
+  virtual void OnKey(int key, int scancode, int act);
   void OnMouseButton(int button, int act);
   void OnMouseMove(double x, double y);
   void OnScroll(double xoffset, double yoffset);
   void OnWindowRefresh();
   void OnWindowResize(int width, int height);
 
   mjuiState state_;
+  int last_key_;
   void (*event_callback_)(mjuiState*);
   void (*layout_callback_)(mjuiState*);
 
   mjrContext con_;
   const mjModel* last_model_ = nullptr;
   int last_fontscale_ = -1;
```

### Comparing `mujoco-2.3.6/mujoco/simulate/simulate.cc` & `mujoco-2.3.7/mujoco/simulate/simulate.cc`

 * *Files 2% similar despite different names*

```diff
@@ -699,15 +699,15 @@
     {mjITEM_SEPARATOR, "OpenGL Effects", 1},
     {mjITEM_END}
   };
 
   // add model cameras, up to UI limit
   for (int i=0; i<mjMIN(m->ncam, mjMAXUIMULTI-2); i++) {
     // prepare name
-    char camname[mjMAXUITEXT] = "\n";
+    char camname[mjMAXUINAME] = "\n";
     if (m->names[m->name_camadr[i]]) {
       mju::strcat_arr(camname, m->names+m->name_camadr[i]);
     } else {
       mju::sprintf_arr(camname, "\nCamera %d", i);
     }
 
     // check string length
@@ -1616,14 +1616,16 @@
       pert(*pert),
       platform_ui(std::move(platform_ui)),
       uistate(this->platform_ui->state()) {
   mjv_defaultSceneState(&scnstate_);
 }
 
 void Simulate::Sync() {
+  MutexLock lock(this->mtx);
+
   if (!m_) {
     return;
   }
 
   bool update_profiler = this->profiler && (this->run || !this->m_);
   bool update_sensor = this->sensor && (this->run || !this->m_);
 
@@ -1896,17 +1898,15 @@
     mjv_applyPerturbForce(m_, d_, &this->pert);
   } else {
     mjv_applyPerturbPose(m_, d_, &this->pert, 1);  // mocap and dynamic bodies
   }
 }
 
 //------------------------- Tell the render thread to load a file and wait -------------------------
-void Simulate::Load(mjModel* m,
-                                mjData* d,
-                                const char* displayed_filename) {
+void Simulate::Load(mjModel* m, mjData* d, const char* displayed_filename) {
   this->mnew_ = m;
   this->dnew_ = d;
   mju::strcpy_arr(this->filename, displayed_filename);
 
   {
     MutexLock lock(mtx);
     this->loadrequest = 2;
@@ -1919,90 +1919,90 @@
 }
 
 //------------------------------------- load mjb or xml model --------------------------------------
 void Simulate::LoadOnRenderThread() {
   this->m_ = this->mnew_;
   this->d_ = this->dnew_;
 
-  ncam_ = this->mnew_->ncam;
-  nkey_ = this->mnew_->nkey;
-  body_parentid_.resize(this->mnew_->nbody);
-  std::memcpy(body_parentid_.data(), this->mnew_->body_parentid,
-              sizeof(this->mnew_->body_parentid[0]) * this->mnew_->nbody);
-
-  jnt_type_.resize(this->mnew_->njnt);
-  std::memcpy(jnt_type_.data(), this->mnew_->jnt_type,
-              sizeof(this->mnew_->jnt_type[0]) * this->mnew_->njnt);
-
-  jnt_group_.resize(this->mnew_->njnt);
-  std::memcpy(jnt_group_.data(), this->mnew_->jnt_group,
-              sizeof(this->mnew_->jnt_group[0]) * this->mnew_->njnt);
-
-  jnt_qposadr_.resize(this->mnew_->njnt);
-  std::memcpy(jnt_qposadr_.data(), this->mnew_->jnt_qposadr,
-              sizeof(this->mnew_->jnt_qposadr[0]) * this->mnew_->njnt);
+  ncam_ = this->m_->ncam;
+  nkey_ = this->m_->nkey;
+  body_parentid_.resize(this->m_->nbody);
+  std::memcpy(body_parentid_.data(), this->m_->body_parentid,
+              sizeof(this->m_->body_parentid[0]) * this->m_->nbody);
+
+  jnt_type_.resize(this->m_->njnt);
+  std::memcpy(jnt_type_.data(), this->m_->jnt_type,
+              sizeof(this->m_->jnt_type[0]) * this->m_->njnt);
+
+  jnt_group_.resize(this->m_->njnt);
+  std::memcpy(jnt_group_.data(), this->m_->jnt_group,
+              sizeof(this->m_->jnt_group[0]) * this->m_->njnt);
+
+  jnt_qposadr_.resize(this->m_->njnt);
+  std::memcpy(jnt_qposadr_.data(), this->m_->jnt_qposadr,
+              sizeof(this->m_->jnt_qposadr[0]) * this->m_->njnt);
 
   jnt_range_.clear();
-  jnt_range_.reserve(this->mnew_->njnt);
-  for (int i = 0; i < this->mnew_->njnt; ++i) {
-    if (this->mnew_->jnt_limited[i]) {
+  jnt_range_.reserve(this->m_->njnt);
+  for (int i = 0; i < this->m_->njnt; ++i) {
+    if (this->m_->jnt_limited[i]) {
       jnt_range_.push_back(
-          std::make_pair(this->mnew_->jnt_range[2 * i], this->mnew_->jnt_range[2 * i + 1]));
+          std::make_pair(this->m_->jnt_range[2 * i], this->m_->jnt_range[2 * i + 1]));
     } else {
       jnt_range_.push_back(std::nullopt);
     }
   }
 
   jnt_names_.clear();
-  jnt_names_.reserve(this->mnew_->njnt);
-  for (int i = 0; i < this->mnew_->njnt; ++i) {
-    jnt_names_.emplace_back(this->mnew_->names + this->mnew_->name_jntadr[i]);
+  jnt_names_.reserve(this->m_->njnt);
+  for (int i = 0; i < this->m_->njnt; ++i) {
+    jnt_names_.emplace_back(this->m_->names + this->m_->name_jntadr[i]);
   }
 
-  actuator_group_.resize(this->mnew_->nu);
-  std::memcpy(actuator_group_.data(), this->mnew_->actuator_group,
-              sizeof(this->mnew_->actuator_group[0]) * this->mnew_->nu);
+  actuator_group_.resize(this->m_->nu);
+  std::memcpy(actuator_group_.data(), this->m_->actuator_group,
+              sizeof(this->m_->actuator_group[0]) * this->m_->nu);
 
   actuator_ctrlrange_.clear();
-  actuator_ctrlrange_.reserve(this->mnew_->nu);
-  for (int i = 0; i < this->mnew_->nu; ++i) {
-    if (this->mnew_->actuator_ctrllimited[i]) {
+  actuator_ctrlrange_.reserve(this->m_->nu);
+  for (int i = 0; i < this->m_->nu; ++i) {
+    if (this->m_->actuator_ctrllimited[i]) {
       actuator_ctrlrange_.push_back(std::make_pair(
-          this->mnew_->actuator_ctrlrange[2 * i], this->mnew_->actuator_ctrlrange[2 * i + 1]));
+          this->m_->actuator_ctrlrange[2 * i], this->m_->actuator_ctrlrange[2 * i + 1]));
     } else {
       actuator_ctrlrange_.push_back(std::nullopt);
     }
   }
 
   actuator_names_.clear();
-  actuator_names_.reserve(this->mnew_->nu);
-  for (int i = 0; i < this->mnew_->nu; ++i) {
-    actuator_names_.emplace_back(this->mnew_->names + this->mnew_->name_actuatoradr[i]);
+  actuator_names_.reserve(this->m_->nu);
+  for (int i = 0; i < this->m_->nu; ++i) {
+    actuator_names_.emplace_back(this->m_->names + this->m_->name_actuatoradr[i]);
   }
 
-  qpos_.resize(this->mnew_->nq);
-  std::memcpy(qpos_.data(), this->dnew_->qpos, sizeof(this->dnew_->qpos[0]) * this->mnew_->nq);
+  qpos_.resize(this->m_->nq);
+  std::memcpy(qpos_.data(), this->d_->qpos, sizeof(this->d_->qpos[0]) * this->m_->nq);
   qpos_prev_ = qpos_;
 
-  ctrl_.resize(this->mnew_->nu);
-  std::memcpy(ctrl_.data(), this->dnew_->ctrl, sizeof(this->dnew_->ctrl[0]) * this->mnew_->nu);
+  ctrl_.resize(this->m_->nu);
+  std::memcpy(ctrl_.data(), this->d_->ctrl, sizeof(this->d_->ctrl[0]) * this->m_->nu);
   ctrl_prev_ = ctrl_;
 
   // re-create scene and context
   if (this->fully_managed_) {
-    mjv_makeScene(this->mnew_, &this->scn, kMaxGeom);
+    mjv_makeScene(this->m_, &this->scn, kMaxGeom);
   } else {
-    mjopt_prev_ = mnew_->opt;
+    mjopt_prev_ = m_->opt;
     opt_prev_ = opt;
     cam_prev_ = cam;
-    warn_vgeomfull_prev_ = dnew_->warning[mjWARN_VGEOMFULL].number;
-    mjv_makeSceneState(this->mnew_, this->dnew_, &this->scnstate_, kMaxGeom);
+    warn_vgeomfull_prev_ = d_->warning[mjWARN_VGEOMFULL].number;
+    mjv_makeSceneState(this->m_, this->d_, &this->scnstate_, kMaxGeom);
   }
 
-  this->platform_ui->RefreshMjrContext(this->mnew_, 50*(this->font+1));
+  this->platform_ui->RefreshMjrContext(this->m_, 50*(this->font+1));
   UiModify(&this->ui0, &this->uistate, &this->platform_ui->mjr_context());
   UiModify(&this->ui1, &this->uistate, &this->platform_ui->mjr_context());
 
   if (!this->platform_ui->IsGPUAccelerated()) {
     this->scn.flags[mjRND_SHADOW] = 0;
     this->scn.flags[mjRND_REFLECTION] = 0;
   }
@@ -2011,54 +2011,54 @@
   this->pert.active = 0;
   this->pert.select = 0;
   this->pert.skinselect = -1;
 
   // align and scale view unless reloading the same file
   if (this->filename[0] &&
       mju::strcmp_arr(this->filename, this->previous_filename)) {
-    AlignAndScaleView(this, this->mnew_);
+    AlignAndScaleView(this, this->m_);
     mju::strcpy_arr(this->previous_filename, this->filename);
   }
 
   // update scene
   if (fully_managed_) {
-    mjv_updateScene(this->mnew_, this->dnew_,
+    mjv_updateScene(this->m_, this->d_,
                     &this->opt, &this->pert, &this->cam, mjCAT_ALL, &this->scn);
   } else {
-    mjv_updateSceneState(this->mnew_, this->dnew_, &this->opt, &this->scnstate_);
+    mjv_updateSceneState(this->m_, this->d_, &this->opt, &this->scnstate_);
   }
 
   // set window title to model name
-  if (this->mnew_->names) {
+  if (this->m_->names) {
     char title[200] = "MuJoCo : ";
-    mju::strcat_arr(title, this->mnew_->names);
+    mju::strcat_arr(title, this->m_->names);
     platform_ui->SetWindowTitle(title);
   }
 
   // set keyframe range and divisions
   this->ui0.sect[SECT_SIMULATION].item[5].slider.range[0] = 0;
-  this->ui0.sect[SECT_SIMULATION].item[5].slider.range[1] = mjMAX(0, this->mnew_->nkey - 1);
-  this->ui0.sect[SECT_SIMULATION].item[5].slider.divisions = mjMAX(1, this->mnew_->nkey - 1);
+  this->ui0.sect[SECT_SIMULATION].item[5].slider.range[1] = mjMAX(0, this->m_->nkey - 1);
+  this->ui0.sect[SECT_SIMULATION].item[5].slider.divisions = mjMAX(1, this->m_->nkey - 1);
 
   // rebuild UI sections
-  MakeUiSections(this, this->mnew_, this->dnew_);
+  MakeUiSections(this, this->m_, this->d_);
 
   // full ui update
   UiModify(&this->ui0, &this->uistate, &this->platform_ui->mjr_context());
   UiModify(&this->ui1, &this->uistate, &this->platform_ui->mjr_context());
-  UpdateSettings(this, this->mnew_);
+  UpdateSettings(this, this->m_);
 
   // clear request
   this->loadrequest = 0;
   cond_loadrequest.notify_all();
 
   // set real time index
   int numclicks = sizeof(this->percentRealTime) / sizeof(this->percentRealTime[0]);
   float min_error = 1e6;
-  float desired = mju_log(100*this->mnew_->vis.global.realtime);
+  float desired = mju_log(100*this->m_->vis.global.realtime);
   for (int click=0; click<numclicks; click++) {
     float error = mju_abs(mju_log(this->percentRealTime[click]) - desired);
     if (error < min_error) {
       min_error = error;
       this->real_time_index = click;
     }
   }
@@ -2379,14 +2379,35 @@
       } else if (this->loadrequest>1) {
         this->loadrequest = 1;
       }
 
       // poll and handle events
       this->platform_ui->PollEvents();
 
+      // upload assets if requested
+      bool upload_notify = false;
+      if (hfield_upload_ != -1) {
+        mjr_uploadHField(m_, &platform_ui->mjr_context(), hfield_upload_);
+        hfield_upload_ = -1;
+        upload_notify = true;
+      }
+      if (mesh_upload_ != -1) {
+        mjr_uploadMesh(m_, &platform_ui->mjr_context(), mesh_upload_);
+        mesh_upload_ = -1;
+        upload_notify = true;
+      }
+      if (texture_upload_ != -1) {
+        mjr_uploadTexture(m_, &platform_ui->mjr_context(), texture_upload_);
+        texture_upload_ = -1;
+        upload_notify = true;
+      }
+      if (upload_notify) {
+        cond_upload_.notify_all();
+      }
+
       // update scene, doing a full sync if in fully managed mode
       if (this->fully_managed_) {
         Sync();
       } else {
         scnstate_.data.warning[mjWARN_VGEOMFULL].number += mjv_updateSceneFromState(
             &scnstate_, &this->opt, &this->pert, &this->cam, mjCAT_ALL, &this->scn);
       }
@@ -2410,8 +2431,35 @@
     mjv_freeScene(&this->scn);
   } else {
     mjv_freeSceneState(&scnstate_);
   }
 
   this->exitrequest.store(2);
 }
+
+void Simulate::UpdateHField(int hfieldid) {
+  MutexLock lock(this->mtx);
+  if (!m_ || hfieldid < 0 || hfieldid >= m_->nhfield) {
+    return;
+  }
+  hfield_upload_ = hfieldid;
+  cond_upload_.wait(lock, [this]() { return hfield_upload_ == -1; });
+}
+
+void Simulate::UpdateMesh(int meshid) {
+  MutexLock lock(this->mtx);
+  if (!m_ || meshid < 0 || meshid >= m_->nmesh) {
+    return;
+  }
+  mesh_upload_ = meshid;
+  cond_upload_.wait(lock, [this]() { return mesh_upload_ == -1; });
+}
+
+void Simulate::UpdateTexture(int texid) {
+  MutexLock lock(this->mtx);
+  if (!m_ || texid < 0 || texid >= m_->ntex) {
+    return;
+  }
+  texture_upload_ = texid;
+  cond_upload_.wait(lock, [this]() { return texture_upload_ == -1; });
+}
 }  // namespace mujoco
```

### Comparing `mujoco-2.3.6/mujoco/simulate/simulate.h` & `mujoco-2.3.7/mujoco/simulate/simulate.h`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,18 @@
       mjvScene* scn, mjvCamera* cam,
       mjvOption* opt, mjvPerturb* pert, bool fully_managed);
 
   // Synchronize mjModel and mjData state with UI inputs, and update
   // visualization.
   void Sync();
 
+  void UpdateHField(int hfieldid);
+  void UpdateMesh(int meshid);
+  void UpdateTexture(int texid);
+
   // Request that the Simulate UI thread render a new model
   // optionally delete the old model and data when done
   void Load(mjModel* m, mjData* d, const char* displayed_filename);
 
   // functions below are used by the renderthread
   // load mjb or xml model that has been requested by load()
   void LoadOnRenderThread();
@@ -275,11 +279,17 @@
     {mjITEM_STATIC,    "Value",         2, nullptr,              " "},
     {mjITEM_END}
   };
 
   // info strings
   char info_title[Simulate::kMaxFilenameLength] = {0};
   char info_content[Simulate::kMaxFilenameLength] = {0};
+
+  // pending uploads
+  std::condition_variable_any cond_upload_;
+  int texture_upload_ = -1;
+  int mesh_upload_ = -1;
+  int hfield_upload_ = -1;
 };
 }  // namespace mujoco
 
 #endif
```

### Comparing `mujoco-2.3.6/mujoco/structs.cc` & `mujoco-2.3.7/mujoco/structs.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/structs.h` & `mujoco-2.3.7/mujoco/structs.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/CMakeLists.txt` & `mujoco-2.3.7/mujoco/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/array_traits.h` & `mujoco-2.3.7/mujoco/util/array_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/array_traits_test.cc` & `mujoco-2.3.7/mujoco/util/array_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/crossplatform.h` & `mujoco-2.3.7/mujoco/util/crossplatform.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/func_traits.h` & `mujoco-2.3.7/mujoco/util/func_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/func_traits_test.cc` & `mujoco-2.3.7/mujoco/util/func_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/func_wrap.h` & `mujoco-2.3.7/mujoco/util/func_wrap.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/func_wrap_test.cc` & `mujoco-2.3.7/mujoco/util/func_wrap_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/tuple_tools.h` & `mujoco-2.3.7/mujoco/util/tuple_tools.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/util/tuple_tools_test.cc` & `mujoco-2.3.7/mujoco/util/tuple_tools_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco/viewer.py` & `mujoco-2.3.7/mujoco/viewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 MAX_SYNC_MISALIGN = 0.1
 
 # Fraction of refresh available for simulation.
 SIM_REFRESH_FRACTION = 0.7
 
 CallbackType = Callable[[mujoco.MjModel, mujoco.MjData], None]
 LoaderType = Callable[[], Tuple[mujoco.MjModel, mujoco.MjData]]
+KeyCallbackType = Callable[[int], None]
 
 # Loader function that also returns a file path for the GUI to display.
 _LoaderWithPathType = Callable[[], Tuple[mujoco.MjModel, mujoco.MjData, str]]
 _InternalLoaderType = Union[LoaderType, _LoaderWithPathType]
 
 _Simulate = _simulate.Simulate
 
@@ -92,15 +93,15 @@
   @property
   def perturb(self):
     return self._pert
 
   def close(self):
     sim = self._sim()
     if sim is not None:
-      sim.exitrequest = 1
+      sim.exit()
 
   def is_running(self) -> bool:
     sim = self._sim()
     if sim is not None:
       return sim.exitrequest < 2
     return False
 
@@ -109,32 +110,53 @@
     if sim is not None:
       return sim.lock()
     return contextlib.nullcontext()
 
   def sync(self):
     sim = self._sim()
     if sim is not None:
-      with sim.lock():
-        sim.sync()
+      sim.sync()  # locks internally
+
+  def update_hfield(self, hfieldid: int):
+    sim = self._sim()
+    if sim is not None:
+      sim.update_hfield(hfieldid)  # locks internally and blocks until done
+
+  def update_mesh(self, meshid: int):
+    sim = self._sim()
+    if sim is not None:
+      sim.update_mesh(meshid)  # locks internally and blocks until done
+
+  def update_texture(self, texid: int):
+    sim = self._sim()
+    if sim is not None:
+      sim.update_texture(texid)  # locks internally and blocks until done
 
   def __enter__(self):
     return self
 
   def __exit__(self, exc_type, exc_val, exc_tb):
     self.close()
 
 
 # Abstract base dispatcher class for systems that require UI calls to be made
 # on a specific thread (e.g. macOS). This is subclassed by system-specific
 # Python launcher (mjpython) to implement the required dispatching mechanism.
 class _MjPythonBase(metaclass=abc.ABCMeta):
 
-  def launch_on_ui_thread(self, model: mujoco.MjModel, data: mujoco.MjData):
+  def launch_on_ui_thread(
+      self,
+      model: mujoco.MjModel,
+      data: mujoco.MjData,
+      handle_return: Optional['queue.Queue[Handle]'],
+      key_callback: Optional[KeyCallbackType],
+  ):
     pass
 
+
 # When running under mjpython, the launcher initializes this object.
 _MJPYTHON: Optional[_MjPythonBase] = None
 
 
 def _file_loader(path: str) -> _LoaderWithPathType:
   """Loads an MJCF model from file path."""
 
@@ -281,14 +303,15 @@
 def _launch_internal(
     model: Optional[mujoco.MjModel] = None,
     data: Optional[mujoco.MjData] = None,
     *,
     run_physics_thread: bool,
     loader: Optional[_InternalLoaderType] = None,
     handle_return: Optional['queue.Queue[Handle]'] = None,
+    key_callback: Optional[KeyCallbackType] = None,
 ) -> None:
   """Internal API, so that the public API has more readable type annotations."""
   if model is None and data is not None:
     raise ValueError('mjData is specified but mjModel is not')
   elif callable(model) and data is not None:
     raise ValueError(
         'mjData should not be specified when an mjModel loader is used')
@@ -309,15 +332,15 @@
   if model and not run_physics_thread:
     scn = mujoco.MjvScene(model, _Simulate.MAX_GEOM)
   else:
     scn = mujoco.MjvScene()
   cam = mujoco.MjvCamera()
   opt = mujoco.MjvOption()
   pert = mujoco.MjvPerturb()
-  simulate = _Simulate(scn, cam, opt, pert, run_physics_thread)
+  simulate = _Simulate(scn, cam, opt, pert, run_physics_thread, key_callback)
 
   # Initialize GLFW if not using mjpython.
   if _MJPYTHON is None:
     if not glfw.init():
       raise mujoco.FatalError('could not initialize GLFW')
     atexit.register(glfw.terminate)
 
@@ -330,26 +353,27 @@
   if run_physics_thread:
     side_thread = threading.Thread(
         target=_physics_loop, args=(simulate, loader))
   else:
     side_thread = threading.Thread(
         target=_reload, args=(simulate, loader, notify_loaded))
 
-  def make_exit_requester(simulate):
-    def exit_requester():
-      simulate.exitrequest = True
-    return exit_requester
+  def make_exit(simulate):
+    def exit_simulate():
+      simulate.exit()
+    return exit_simulate
 
-  exit_requester = make_exit_requester(simulate)
-  atexit.register(exit_requester)
+  exit_simulate = make_exit(simulate)
+  atexit.register(exit_simulate)
 
   side_thread.start()
   simulate.render_loop()
-  atexit.unregister(exit_requester)
+  atexit.unregister(exit_simulate)
   side_thread.join()
+  simulate.destroy()
 
 
 def launch(model: Optional[mujoco.MjModel] = None,
            data: Optional[mujoco.MjData] = None,
            *,
            loader: Optional[LoaderType] = None) -> None:
   """Launches the Simulate GUI."""
@@ -358,38 +382,50 @@
 
 
 def launch_from_path(path: str) -> None:
   """Launches the Simulate GUI from file path."""
   _launch_internal(run_physics_thread=True, loader=_file_loader(path))
 
 
-def launch_passive(model: mujoco.MjModel, data: mujoco.MjData) -> Handle:
+def launch_passive(
+    model: mujoco.MjModel,
+    data: mujoco.MjData,
+    *,
+    key_callback: Optional[KeyCallbackType] = None,
+) -> Handle:
   """Launches a passive Simulate GUI without blocking the running thread."""
   if not isinstance(model, mujoco.MjModel):
     raise ValueError(f'`model` is not a mujoco.MjModel: got {model!r}')
   if not isinstance(data, mujoco.MjData):
     raise ValueError(f'`data` is not a mujoco.MjData: got {data!r}')
+  if key_callback is not None and not callable(key_callback):
+    raise ValueError(
+        f'`key_callback` is not callable: got {key_callback!r}')
 
   mujoco.mj_forward(model, data)
   handle_return = queue.Queue(1)
 
   if sys.platform != 'darwin':
     thread = threading.Thread(
         target=_launch_internal,
         args=(model, data),
-        kwargs=dict(run_physics_thread=False, handle_return=handle_return),
+        kwargs=dict(
+            run_physics_thread=False,
+            handle_return=handle_return,
+            key_callback=key_callback,
+        ),
     )
     thread.daemon = True
     thread.start()
   else:
     if not isinstance(_MJPYTHON, _MjPythonBase):
       raise RuntimeError(
           '`launch_passive` requires that the Python script be run under '
           '`mjpython` on macOS')
-    _MJPYTHON.launch_on_ui_thread(model, data, handle_return)
+    _MJPYTHON.launch_on_ui_thread(model, data, handle_return, key_callback)
 
   return handle_return.get()
 
 
 if __name__ == '__main__':
   from absl import app  # pylint: disable=g-import-not-at-top
   from absl import flags  # pylint: disable=g-import-not-at-top
```

### Comparing `mujoco-2.3.6/mujoco/viewer_test.py` & `mujoco-2.3.7/mujoco/viewer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/mujoco.egg-info/PKG-INFO` & `mujoco-2.3.7/mujoco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.6
+Version: 2.3.7
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
 Author: Google DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSES_THIRD_PARTY.md
 
 # MuJoCo Python Bindings
 
 [![PyPI Python Version][pypi-versions-badge]][pypi]
```

### Comparing `mujoco-2.3.6/mujoco.egg-info/SOURCES.txt` & `mujoco-2.3.7/mujoco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.6/setup.py` & `mujoco-2.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import setuptools
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command import build_ext
 from setuptools.command import install_scripts
 
-__version__ = '2.3.6'
+__version__ = '2.3.7'
 
 MUJOCO_CMAKE = 'MUJOCO_CMAKE'
 MUJOCO_CMAKE_ARGS = 'MUJOCO_CMAKE_ARGS'
 MUJOCO_PATH = 'MUJOCO_PATH'
 MUJOCO_PLUGIN_PATH = 'MUJOCO_PLUGIN_PATH'
 
 EXT_PREFIX = 'mujoco.'
@@ -359,15 +359,14 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
     ],
     cmdclass=dict(
@@ -381,15 +380,15 @@
         CMakeExtension('mujoco._errors'),
         CMakeExtension('mujoco._functions'),
         CMakeExtension('mujoco._render'),
         CMakeExtension('mujoco._rollout'),
         CMakeExtension('mujoco._simulate'),
         CMakeExtension('mujoco._structs'),
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'absl-py',
         'glfw',
         'numpy',
         'pyopengl',
     ],
     tests_require=[
```

