# Comparing `tmp/mccoygroup-psience-0.0.9.1.tar.gz` & `tmp/mccoygroup-psience-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-psience-0.0.9.1.tar", last modified: Tue Jul 11 18:54:10 2023, max compression
+gzip compressed data, was "mccoygroup-psience-0.0.9.2.tar", last modified: Thu Jul 20 19:45:08 2023, max compression
```

## Comparing `mccoygroup-psience-0.0.9.1.tar` & `mccoygroup-psience-0.0.9.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/AIMD/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AIMD/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AIMD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticModelConstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/Helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.848983 mccoygroup-psience-0.0.9.1/Psience/BasisReps/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/ClassicalBases.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30900 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/HarmonicOscillator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Representations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateIndexers.py
--rw-r--r--   0 runner    (1001) docker     (123)   184560 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateSpaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/BasisReps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/DGB/
--rw-r--r--   0 runner    (1001) docker     (123)    76300 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/DGB.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/Wavefunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DGB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/DVR/
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/BaseDVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/ColbertMiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/DVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/DirectProduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/FiniteBasisDVR.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/DVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Data/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/KEData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/
--rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/KEData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/Surfaces.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Molecools/
--rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/CoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/MolecularFunctionExpansion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55296 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/MoleculeInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Transformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/Vibrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Molecools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/Spectra/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Spectra/BaseSpectrum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.852983 mccoygroup-psience-0.0.9.1/Psience/VPT2/
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Analyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Common.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    45597 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/DegeneracySpecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49402 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    86022 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    99465 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Solver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   128543 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Terms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VPT2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/Psience/VSCF/
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VSCF/VSCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/VSCF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/Psience/Wavefun/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/DirectProduct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/Wavefunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/Wavefun/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/Psience/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 18:54:10.000000 mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:54:10.856983 mccoygroup-psience-0.0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-07-11 18:53:58.000000 mccoygroup-psience-0.0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.713374 mccoygroup-psience-0.0.9.2/Psience/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.713374 mccoygroup-psience-0.0.9.2/Psience/AIMD/
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AIMD/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AIMD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/AnalyticModelConstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/Helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/BasisReps/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18017 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/Bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/ClassicalBases.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31715 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/HarmonicOscillator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51651 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/Operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46924 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/Representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateIndexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   184674 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateSpaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10328 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/BasisReps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/DGB/
+-rw-r--r--   0 runner    (1001) docker     (123)    76300 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DGB/DGB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DGB/Wavefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DGB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/DVR/
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/BaseDVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/ColbertMiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/DVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/DirectProduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/FiniteBasisDVR.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/DVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/Data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Data/KEData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.717375 mccoygroup-psience-0.0.9.2/Psience/Data/PsiDatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Data/PsiDatasets/KEData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Data/PsiDatasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10276 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Data/Surfaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/Psience/Molecools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27306 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/CoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37771 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/MolecularFunctionExpansion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55296 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/MoleculeInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68334 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/Transformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20193 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/Vibrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Molecools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/Psience/Spectra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14581 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Spectra/BaseSpectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/Psience/VPT2/
+-rw-r--r--   0 runner    (1001) docker     (123)    87836 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Analyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      692 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45597 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/DegeneracySpecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49402 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86022 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99465 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Solver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   128543 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Terms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77064 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VPT2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/Psience/VSCF/
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VSCF/VSCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/VSCF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/Psience/Wavefun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Wavefun/DirectProduct.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11061 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Wavefun/Wavefunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/Wavefun/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/Psience/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3079 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-20 19:45:08.000000 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 19:45:08.000000 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:45:08.000000 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 19:45:08.000000 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 19:45:08.000000 mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:45:08.721375 mccoygroup-psience-0.0.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-07-20 19:44:56.000000 mccoygroup-psience-0.0.9.2/setup.py
```

### Comparing `mccoygroup-psience-0.0.9.1/LICENSE.txt` & `mccoygroup-psience-0.0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/PKG-INFO` & `mccoygroup-psience-0.0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.9.1/Psience/AIMD/Simulator.py` & `mccoygroup-psience-0.0.9.2/Psience/AIMD/Simulator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py` & `mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/AnalyticJacobianDotCalculator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/AnalyticModelConstructors.py` & `mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/AnalyticModelConstructors.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/AnalyticModels/Helpers.py` & `mccoygroup-psience-0.0.9.2/Psience/AnalyticModels/Helpers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Bases.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/Bases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/ClassicalBases.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/ClassicalBases.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/HarmonicOscillator.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/HarmonicOscillator.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,25 @@
         prefactor = cls.binom(a + b, a)
         coeffs = prefactor * cls.get_reduced_raising_lowering_coeffs(a, b)
         if shift != 0:
             coeffs = DensePolynomial._compute_shifted_coeffs(coeffs, shift)
         return coeffs
 
     @classmethod
+    def get_direction_change_poly(cls, delta, shift):
+        if not isinstance(delta, (int, np.integer)):
+            return [cls.get_direction_change_poly(d, s) for d,s in zip(delta, shift)]
+        sqrt_contrib = None
+        if delta != 0:
+            dir_change = np.sign(delta) == -np.sign(shift)  # avoid the zero case
+            if dir_change:
+                sqrt_contrib = HarmonicOscillatorRaisingLoweringPolyTerms.get_sqrt_remainder_coeffs(delta, shift)
+        return sqrt_contrib
+
+    @classmethod
     def get_sqrt_remainder_coeffs(cls, delta, k):
         # provides rising or falling coeffs with a starting shift
         # by essentially only providing rising coeffs but
         # shifting appropriately
         d = min(abs(delta), abs(k))
         if delta == 0:
             return 1
@@ -522,14 +533,16 @@
     @classmethod
     def _get_poly_coeffs(cls, terms, delta):
 
         if (delta % 2) != len(terms) % 2:
             return 0
         if abs(delta) > len(terms):
             return 0
+        if len(terms) == 0:
+            return [1] # just the constant overlap term
         # we know we need to change by delta
         # over
         if terms not in cls._size_blocks_cache:
             cls._size_blocks_cache[terms] = cls._build_xp_blocks(terms)
         sizes, parities = cls._size_blocks_cache[terms]
         # total_parity = (-1)**(np.count_nonzero(parities-1)//2)
         poly = None
@@ -550,15 +563,19 @@
         return poly / np.sqrt(2)**len(terms)
 
     def poly_coeffs(self, delta, shift=0):
         if (delta, shift) not in self._poly_cache:
             if delta not in self._poly_cache:
                 self._poly_cache[delta] = self._get_poly_coeffs(self.terms, delta)
             if shift != 0:
-                self._poly_cache[(delta, shift)] = DensePolynomial._compute_shifted_coeffs(self._poly_cache[delta], shift=shift)
+                base_coeffs = self._poly_cache[delta]
+                if isinstance(base_coeffs, (int, float, np.integer, np.floating)):
+                    self._poly_cache[(delta, shift)] = base_coeffs
+                else:
+                    self._poly_cache[(delta, shift)] = DensePolynomial._compute_shifted_coeffs(base_coeffs, shift=shift)
             else:
                 self._poly_cache[(delta, shift)] = self._poly_cache[delta]
         return self._poly_cache[(delta, shift)]
 
 
     @classmethod
     def get_poly_coeffs(cls, terms, delta, shift=0):
```

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Operators.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/Operators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Representations.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/Representations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateFilters.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateFilters.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateIndexers.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateIndexers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/StateSpaces.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/StateSpaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -3250,15 +3250,16 @@
                         )
                         ospace._indexer, sspace._indexer = subsortings
                         where_inds, _ = nput.find(oti, other_exclusions,
                                                   sorting=ospace._indexer
                                                   )
                     if len(where_inds) > 0:
                         where_inds = np.sort(where_inds)
-                        changes[i_new] = np.concatenate([changes[i_new], c2[where_inds]])
+                        changes[i_new] = np.concatenate([changes[i_new], *[c2[w] for w in where_inds]], axis=0)
+                        # changes[i_new] = np.concatenate([changes[i_new], c2[where_inds]])
                     # print(" >", changes[i_new])
 
                 new_spaces[i_new] = new_spaces[i_new].union(
                     other[i_old],
                     track_indices=track_indices,
                     track_excitations=track_excitations
                 )
```

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/Wavefunctions.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/BasisReps/__init__.py` & `mccoygroup-psience-0.0.9.2/Psience/BasisReps/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DGB/DGB.py` & `mccoygroup-psience-0.0.9.2/Psience/DGB/DGB.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DGB/Wavefunctions.py` & `mccoygroup-psience-0.0.9.2/Psience/DGB/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/BaseDVR.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/BaseDVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/ColbertMiller.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/ColbertMiller.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/DVR.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/DVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/DirectProduct.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/Extensions.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/Extensions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/FiniteBasisDVR.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/FiniteBasisDVR.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/Wavefunctions.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/DVR/__init__.py` & `mccoygroup-psience-0.0.9.2/Psience/DVR/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Data/KEData.py` & `mccoygroup-psience-0.0.9.2/Psience/Data/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Data/PsiDatasets/KEData.py` & `mccoygroup-psience-0.0.9.2/Psience/Data/PsiDatasets/KEData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Data/Surfaces.py` & `mccoygroup-psience-0.0.9.2/Psience/Data/Surfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Data/__init__.py` & `mccoygroup-psience-0.0.9.2/Psience/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/CoordinateSystems.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/CoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/MolecularFunctionExpansion.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/MolecularFunctionExpansion.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/Molecule.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/Molecule.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/MoleculeInterface.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/MoleculeInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/Properties.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/Transformations.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/Transformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Molecools/Vibrations.py` & `mccoygroup-psience-0.0.9.2/Psience/Molecools/Vibrations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Spectra/BaseSpectrum.py` & `mccoygroup-psience-0.0.9.2/Psience/Spectra/BaseSpectrum.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Analyzer.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Analyzer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Common.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Common.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Corrections.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Corrections.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/DegeneracySpecs.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/DegeneracySpecs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Hamiltonian.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Hamiltonian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Runner.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Runner.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Solver.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Solver.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Terms.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Terms.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/Wavefunctions.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VPT2/__init__.py` & `mccoygroup-psience-0.0.9.2/Psience/VPT2/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/VSCF/VSCF.py` & `mccoygroup-psience-0.0.9.2/Psience/VSCF/VSCF.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Wavefun/DirectProduct.py` & `mccoygroup-psience-0.0.9.2/Psience/Wavefun/DirectProduct.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/Wavefun/Wavefunctions.py` & `mccoygroup-psience-0.0.9.2/Psience/Wavefun/Wavefunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/Psience/__init__.py` & `mccoygroup-psience-0.0.9.2/Psience/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/README.md` & `mccoygroup-psience-0.0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/PKG-INFO` & `mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-psience
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # Psience [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/McCoyGroup/Binder-McUtils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FMcCoyGroup%252FPsience%26urlpath%3Dlab%252Ftree%252FPsience%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-psience-0.0.9.1/mccoygroup_psience.egg-info/SOURCES.txt` & `mccoygroup-psience-0.0.9.2/mccoygroup_psience.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-psience-0.0.9.1/setup.py` & `mccoygroup-psience-0.0.9.2/setup.py`

 * *Files identical despite different names*

