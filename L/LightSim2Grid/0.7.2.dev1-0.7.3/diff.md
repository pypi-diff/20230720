# Comparing `tmp/LightSim2Grid-0.7.2.dev1.tar.gz` & `tmp/LightSim2Grid-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LightSim2Grid-0.7.2.dev1.tar", last modified: Fri Apr 28 14:27:30 2023, max compression
+gzip compressed data, was "LightSim2Grid-0.7.3.tar", last modified: Thu Jul 20 10:24:36 2023, max compression
```

## Comparing `LightSim2Grid-0.7.2.dev1.tar` & `LightSim2Grid-0.7.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.918510 LightSim2Grid-0.7.2.dev1/
--rw-r--r--   0 runner     (501) staff       (20)      449 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/AUTHORS.txt
--rw-r--r--   0 runner     (501) staff       (20)    16725 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    16725 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/LICENSE.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.888748 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    18311 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1527 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 14:27:29.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      304 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       32 2023-04-28 14:27:30.000000 LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)    18311 2023-04-28 14:27:30.917921 LightSim2Grid-0.7.2.dev1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    17147 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.897498 LightSim2Grid-0.7.2.dev1/lightsim2grid/
--rw-r--r--   0 runner     (501) staff       (20)     1639 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.898013 LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/
--rw-r--r--   0 runner     (501) staff       (20)     1216 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.904134 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/
--rw-r--r--   0 runner     (501) staff       (20)      553 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2950 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_dc_line.py
--rw-r--r--   0 runner     (501) staff       (20)     1430 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_gen.py
--rw-r--r--   0 runner     (501) staff       (20)     1989 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_line.py
--rw-r--r--   0 runner     (501) staff       (20)     1318 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_load.py
--rw-r--r--   0 runner     (501) staff       (20)     3132 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_sgen.py
--rw-r--r--   0 runner     (501) staff       (20)     1325 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_shunt.py
--rw-r--r--   0 runner     (501) staff       (20)     6047 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_slack.py
--rw-r--r--   0 runner     (501) staff       (20)     1394 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_storage.py
--rw-r--r--   0 runner     (501) staff       (20)     4373 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_trafo.py
--rw-r--r--   0 runner     (501) staff       (20)     2977 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_check_legit.py
--rw-r--r--   0 runner     (501) staff       (20)     4493 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/initGridModel.py
--rw-r--r--   0 runner     (501) staff       (20)    49089 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/lightSimBackend.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.905182 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12570 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/newtonpf.py
--rw-r--r--   0 runner     (501) staff       (20)     5582 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/physical_law_checker.py
--rw-r--r--   0 runner     (501) staff       (20)    13788 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/securityAnalysis.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.905647 LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/
--rw-r--r--   0 runner     (501) staff       (20)     2423 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11432 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/lightsim2grid/timeSerie.py
--rw-r--r--   0 runner     (501) staff       (20)      138 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-28 14:27:30.918630 LightSim2Grid-0.7.2.dev1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    15878 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 14:27:30.917118 LightSim2Grid-0.7.2.dev1/src/
--rw-r--r--   0 runner     (501) staff       (20)      767 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseConstants.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2980 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseMultiplePowerflow.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5849 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/BaseSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)      487 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/ChooseSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4867 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/Computers.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7403 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataConverter.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2520 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataDCLine.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16458 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataGen.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6449 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataGeneric.cpp
--rw-r--r--   0 runner     (501) staff       (20)    11757 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataLine.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4353 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataLoad.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6389 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataSGen.cpp
--rw-r--r--   0 runner     (501) staff       (20)     7133 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataShunt.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15457 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/DataTrafo.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4864 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GaussSeidelSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2239 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GaussSeidelSynchSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)    34888 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/GridModel.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2589 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/KLUSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9499 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/SecurityAnalysis.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1920 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/SparseLUSolver.cpp
--rw-r--r--   0 runner     (501) staff       (20)   110165 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/help_fun_msg.cpp
--rw-r--r--   0 runner     (501) staff       (20)    68726 2023-04-28 14:23:01.000000 LightSim2Grid-0.7.2.dev1/src/main.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:35.920128 LightSim2Grid-0.7.3/
+-rw-r--r--   0 runner     (501) staff       (20)      449 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/AUTHORS.txt
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/LICENSE.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:33.090052 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    18306 2023-07-20 10:24:31.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2023-07-20 10:24:32.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-20 10:24:31.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-20 10:24:28.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      314 2023-07-20 10:24:32.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       32 2023-07-20 10:24:32.000000 LightSim2Grid-0.7.3/LightSim2Grid.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)    18306 2023-07-20 10:24:35.879107 LightSim2Grid-0.7.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    17147 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:33.459214 LightSim2Grid-0.7.3/lightsim2grid/
+-rw-r--r--   0 runner     (501) staff       (20)     1634 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:33.541345 LightSim2Grid-0.7.3/lightsim2grid/elements/
+-rw-r--r--   0 runner     (501) staff       (20)     1216 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/elements/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:34.282148 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/
+-rw-r--r--   0 runner     (501) staff       (20)      553 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2950 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_dc_line.py
+-rw-r--r--   0 runner     (501) staff       (20)     1430 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_gen.py
+-rw-r--r--   0 runner     (501) staff       (20)     1989 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_line.py
+-rw-r--r--   0 runner     (501) staff       (20)     1318 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_load.py
+-rw-r--r--   0 runner     (501) staff       (20)     3132 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_sgen.py
+-rw-r--r--   0 runner     (501) staff       (20)     1325 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_shunt.py
+-rw-r--r--   0 runner     (501) staff       (20)     6047 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_slack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1394 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)     4373 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_trafo.py
+-rw-r--r--   0 runner     (501) staff       (20)     2977 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_check_legit.py
+-rw-r--r--   0 runner     (501) staff       (20)     4493 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/gridmodel/initGridModel.py
+-rw-r--r--   0 runner     (501) staff       (20)    49426 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/lightSimBackend.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:34.405043 LightSim2Grid-0.7.3/lightsim2grid/newtonpf/
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/newtonpf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12570 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/newtonpf/newtonpf.py
+-rw-r--r--   0 runner     (501) staff       (20)     5582 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/physical_law_checker.py
+-rw-r--r--   0 runner     (501) staff       (20)    13736 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/securityAnalysis.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:34.446371 LightSim2Grid-0.7.3/lightsim2grid/solver/
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/solver/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11432 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/lightsim2grid/timeSerie.py
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-20 10:24:35.920278 LightSim2Grid-0.7.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)    15898 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-20 10:24:35.796910 LightSim2Grid-0.7.3/src/
+-rw-r--r--   0 runner     (501) staff       (20)      767 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/BaseConstants.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2980 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/BaseMultiplePowerflow.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5849 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/BaseSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/ChooseSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4867 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/Computers.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7403 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataConverter.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataDCLine.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    16458 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataGen.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6449 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataGeneric.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    11757 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataLine.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4353 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataLoad.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6389 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataSGen.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     7133 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataShunt.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15457 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/DataTrafo.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4864 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/GaussSeidelSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2239 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/GaussSeidelSynchSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    34888 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/GridModel.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2589 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/KLUSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     9499 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/SecurityAnalysis.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1920 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/SparseLUSolver.cpp
+-rw-r--r--   0 runner     (501) staff       (20)   110165 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/help_fun_msg.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    68726 2023-07-20 10:19:54.000000 LightSim2Grid-0.7.3/src/main.cpp
```

### Comparing `LightSim2Grid-0.7.2.dev1/LICENSE` & `LightSim2Grid-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/LICENSE.md` & `LightSim2Grid-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/PKG-INFO` & `LightSim2Grid-0.7.3/LightSim2Grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightSim2Grid
-Version: 0.7.2.dev1
+Version: 0.7.3
 Summary: LightSim2Grid implements a c++ backend targeting the Grid2Op platform.
 Home-page: https://github.com/BDonnot/lightsim2grid/
 Author: Benjamin Donnot
 Author-email: benjamin.donnot@rte-france.com
 License: MPL 2.0
 Keywords: pandapower powergrid simulator KLU Eigen c++
 Platform: Windows
```

### Comparing `LightSim2Grid-0.7.2.dev1/LightSim2Grid.egg-info/SOURCES.txt` & `LightSim2Grid-0.7.3/LightSim2Grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/PKG-INFO` & `LightSim2Grid-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightSim2Grid
-Version: 0.7.2.dev1
+Version: 0.7.3
 Summary: LightSim2Grid implements a c++ backend targeting the Grid2Op platform.
 Home-page: https://github.com/BDonnot/lightsim2grid/
 Author: Benjamin Donnot
 Author-email: benjamin.donnot@rte-france.com
 License: MPL 2.0
 Keywords: pandapower powergrid simulator KLU Eigen c++
 Platform: Windows
```

### Comparing `LightSim2Grid-0.7.2.dev1/README.md` & `LightSim2Grid-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/__init__.py` & `LightSim2Grid-0.7.3/lightsim2grid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LightSim2grid, LightSim2grid implements a c++ backend targeting the Grid2Op platform.
 
 import faulthandler
 faulthandler.enable()
 
-__version__ = "0.7.2.dev1"
+__version__ = "0.7.3"
 
 __all__ = ["newtonpf", "SolverType", "ErrorType", "solver"]
 
 # import directly from c++ module
 from lightsim2grid.solver import SolverType
 from lightsim2grid.solver import ErrorType
```

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/elements/__init__.py` & `LightSim2Grid-0.7.3/lightsim2grid/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/__init__.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_dc_line.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_dc_line.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_gen.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_gen.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_line.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_line.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_load.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_load.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_sgen.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_sgen.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_shunt.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_shunt.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_slack.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_slack.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_storage.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_storage.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_add_trafo.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_add_trafo.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/_aux_check_legit.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/_aux_check_legit.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/gridmodel/initGridModel.py` & `LightSim2Grid-0.7.3/lightsim2grid/gridmodel/initGridModel.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/lightSimBackend.py` & `LightSim2Grid-0.7.3/lightsim2grid/lightSimBackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 import warnings
 import numpy as np
 import time
 
 from grid2op.Action import CompleteAction
 from grid2op.Backend import Backend
 from grid2op.Exceptions import BackendError, DivergingPowerFlow
-from grid2op.Action._BackendAction import _BackendAction
 from grid2op.dtypes import dt_float, dt_int, dt_bool
+try:
+    from grid2op.Action._backendAction import _BackendAction
+except ImportError as exc_:
+    from grid2op.Action._BackendAction import _BackendAction
 
 from lightsim2grid.gridmodel import init
 from lightsim2grid.solver import SolverType
 
 
 class LightSimBackend(Backend):
     """
@@ -78,16 +81,21 @@
 
         self.next_prod_p = None  # this vector is updated with the action that will modify the environment
         # it is done to keep track of the redispatching
 
         self.topo_vect = None
         self.shunt_topo_vect = None
 
-        self.init_pp_backend = PandaPowerBackend()
-
+        try:
+            self.init_pp_backend = PandaPowerBackend(with_numba=False)
+        except TypeError as exc_:
+            # oldest version of grid2op do not support the kwargs "with_numba"
+            # (before 1.9.1)
+            self.init_pp_backend = PandaPowerBackend()
+        
         self.V = None
         self.max_it = max_iter
         self.tol = tol  # tolerance for the solver
 
         self.prod_pu_to_kv = None
         self.load_pu_to_kv = None
         self.lines_or_pu_to_kv = None
@@ -647,14 +655,19 @@
 
     def apply_action(self, backendAction):
         """
         Specific implementation of the method to apply an action modifying a powergrid in the pandapower format.
         """
         active_bus, *_, topo__, shunts__ = backendAction()
 
+        # change the overall topology
+        chgt = backendAction.current_topo.changed
+        self._grid.update_topo(chgt, backendAction.current_topo.values)
+        self.topo_vect[chgt] = backendAction.current_topo.values[chgt]
+        
         # update the injections
         self._grid.update_gens_p(backendAction.prod_p.changed,
                                  backendAction.prod_p.values)
         self._grid.update_gens_v(backendAction.prod_v.changed,
                                  backendAction.prod_v.values / self.prod_pu_to_kv)
         self._grid.update_loads_p(backendAction.load_p.changed,
                                   backendAction.load_p.values)
@@ -683,15 +696,14 @@
                     else:
                         self._grid.change_bus_shunt(sh_id, self.shunt_to_subid[sh_id] + (new_bus == 2) * type(self).n_sub)
             for sh_id, new_p in shunt_p:
                 self._grid.change_p_shunt(sh_id, new_p)
             for sh_id, new_q in shunt_q:
                 self._grid.change_q_shunt(sh_id, new_q)
 
-        # and now change the overall topology
         # TODO hack for storage units: if 0. production i pretend they are disconnected on the
         # TODO c++ side
         # this is to deal with the test that "if a storage unit is alone on a bus, but produces 0, then it's fine)
         # if self.__has_storage and self.n_storage > 0:
         #     chgt = copy.copy(backendAction.current_topo.changed)
         #     my_val = 1 * backendAction.current_topo.values
         #     self._idx_hack_storage = np.where((backendAction.storage_power.values == 0.))[0]
@@ -699,17 +711,14 @@
         #     changed[idx_storage_topo] = my_val[idx_storage_topo] != -1
         #     my_val[idx_storage_topo] = -1
         # else:
         #     self._idx_hack_storage = []
         #     chgt = backendAction.current_topo.changed
         #     my_val = backendAction.current_topo.values
         # self._grid.update_topo(changed, my_val)
-        chgt = backendAction.current_topo.changed
-        self._grid.update_topo(chgt, backendAction.current_topo.values)
-        self.topo_vect[chgt] = backendAction.current_topo.values[chgt]
         # TODO c++ side: have a check to be sure that the set_***_pos_topo_vect and set_***_to_sub_id
         # TODO have been correctly called before calling the function self._grid.update_topo
         
         self._handle_dist_slack()
     
     def _handle_dist_slack(self):
         if self._dist_slack_non_renew:
```

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/__init__.py` & `LightSim2Grid-0.7.3/lightsim2grid/newtonpf/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/newtonpf/newtonpf.py` & `LightSim2Grid-0.7.3/lightsim2grid/newtonpf/newtonpf.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/physical_law_checker.py` & `LightSim2Grid-0.7.3/lightsim2grid/physical_law_checker.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/securityAnalysis.py` & `LightSim2Grid-0.7.3/lightsim2grid/securityAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,19 +68,15 @@
     Sometimes, the behaviour might differ from grid2op. For example, if simulating a contingency
     leads to a non connected grid, then this function will return "Nan" for the flows and 0. for
     the voltages.
 
     In grid2op, it would be, in this case, 0. for the flows and 0. for the voltages.
 
     """
-    try:
-        STR_TYPES = (str, np.str, np.str_)
-    except AttributeError:
-        # deprecation in numpy 1.24 of np.str
-        STR_TYPES = (str, np.str_)
+    STR_TYPES = (str, np.str_)  # np.str deprecated in numpy 1.20 and earlier versions not supported anyway
         
     def __init__(self, grid2op_env):
         if not isinstance(grid2op_env.backend, LightSimBackend):
             raise RuntimeError("This class only works with LightSimBackend")
         self.grid2op_env = grid2op_env.copy()
         self.computer = SecurityAnalysisCPP(self.grid2op_env.backend._grid)
         self._contingency_order = {}  # key: contingency (as tuple), value: order in which it is entered
```

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/solver/__init__.py` & `LightSim2Grid-0.7.3/lightsim2grid/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/lightsim2grid/timeSerie.py` & `LightSim2Grid-0.7.3/lightsim2grid/timeSerie.py`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/setup.py` & `LightSim2Grid-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup
 import sys
 import os
 import warnings
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
 
-__version__ = "0.7.2.dev1"
+__version__ = "0.7.3"
 KLU_SOLVER_AVAILABLE = False
 
 # Try to link against SuiteSparse (if available)
 # check that they exist (if SuiteSparse has been built with "make")
 suitesparse_path_make = os.path.abspath("./SuiteSparse")
 LIBS_MAKE = ["{}/KLU/Lib/libklu.a",
              "{}/BTF/Lib/libbtf.a",
@@ -344,15 +344,16 @@
         "recommended": [
             "grid2op>=1.6.4",
             "numba"
         ],
         "test": [
             "grid2op>=1.6.4",
             "numba",
-            "pandapower>=2.8.0"
+            "pandapower>=2.8.0",
+            "packaging"
         ]
     }
 }
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `LightSim2Grid-0.7.2.dev1/src/BaseConstants.cpp` & `LightSim2Grid-0.7.3/src/BaseConstants.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/BaseMultiplePowerflow.cpp` & `LightSim2Grid-0.7.3/src/BaseMultiplePowerflow.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/BaseSolver.cpp` & `LightSim2Grid-0.7.3/src/BaseSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/Computers.cpp` & `LightSim2Grid-0.7.3/src/Computers.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataConverter.cpp` & `LightSim2Grid-0.7.3/src/DataConverter.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataDCLine.cpp` & `LightSim2Grid-0.7.3/src/DataDCLine.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataGen.cpp` & `LightSim2Grid-0.7.3/src/DataGen.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataGeneric.cpp` & `LightSim2Grid-0.7.3/src/DataGeneric.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataLine.cpp` & `LightSim2Grid-0.7.3/src/DataLine.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataLoad.cpp` & `LightSim2Grid-0.7.3/src/DataLoad.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataSGen.cpp` & `LightSim2Grid-0.7.3/src/DataSGen.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataShunt.cpp` & `LightSim2Grid-0.7.3/src/DataShunt.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/DataTrafo.cpp` & `LightSim2Grid-0.7.3/src/DataTrafo.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/GaussSeidelSolver.cpp` & `LightSim2Grid-0.7.3/src/GaussSeidelSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/GaussSeidelSynchSolver.cpp` & `LightSim2Grid-0.7.3/src/GaussSeidelSynchSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/GridModel.cpp` & `LightSim2Grid-0.7.3/src/GridModel.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/KLUSolver.cpp` & `LightSim2Grid-0.7.3/src/KLUSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/SecurityAnalysis.cpp` & `LightSim2Grid-0.7.3/src/SecurityAnalysis.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/SparseLUSolver.cpp` & `LightSim2Grid-0.7.3/src/SparseLUSolver.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/help_fun_msg.cpp` & `LightSim2Grid-0.7.3/src/help_fun_msg.cpp`

 * *Files identical despite different names*

### Comparing `LightSim2Grid-0.7.2.dev1/src/main.cpp` & `LightSim2Grid-0.7.3/src/main.cpp`

 * *Files identical despite different names*

