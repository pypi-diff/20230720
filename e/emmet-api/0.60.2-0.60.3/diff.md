# Comparing `tmp/emmet-api-0.60.2.tar.gz` & `tmp/emmet-api-0.60.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.60.2.tar", last modified: Tue Jul 18 02:15:54 2023, max compression
+gzip compressed data, was "emmet-api-0.60.3.tar", last modified: Thu Jul 20 20:24:04 2023, max compression
```

## Comparing `emmet-api-0.60.2.tar` & `emmet-api-0.60.3.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.491812 emmet-api-0.60.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 02:15:45.000000 emmet-api-0.60.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 02:15:54.491812 emmet-api-0.60.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 02:15:45.000000 emmet-api-0.60.2/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.459811 emmet-api-0.60.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.467811 emmet-api-0.60.2/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.471811 emmet-api-0.60.2/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.475811 emmet-api-0.60.2/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.479812 emmet-api-0.60.2/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-18 02:15:45.000000 emmet-api-0.60.2/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 02:15:53.000000 emmet-api-0.60.2/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-18 02:15:54.000000 emmet-api-0.60.2/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:15:53.000000 emmet-api-0.60.2/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:15:53.000000 emmet-api-0.60.2/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 02:15:53.000000 emmet-api-0.60.2/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 02:15:53.000000 emmet-api-0.60.2/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 02:15:45.000000 emmet-api-0.60.2/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-18 02:15:45.000000 emmet-api-0.60.2/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-18 02:15:45.000000 emmet-api-0.60.2/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-18 02:15:45.000000 emmet-api-0.60.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:15:54.491812 emmet-api-0.60.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-18 02:15:45.000000 emmet-api-0.60.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-18 02:15:45.000000 emmet-api-0.60.2/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.463811 emmet-api-0.60.2/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.463811 emmet-api-0.60.2/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.483812 emmet-api-0.60.2/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.487812 emmet-api-0.60.2/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:54.491812 emmet-api-0.60.2/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-18 02:15:45.000000 emmet-api-0.60.2/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-20 20:23:57.000000 emmet-api-0.60.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 20:24:04.771165 emmet-api-0.60.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 20:23:57.000000 emmet-api-0.60.3/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.739164 emmet-api-0.60.3/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.747165 emmet-api-0.60.3/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.751165 emmet-api-0.60.3/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.755165 emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-20 20:23:57.000000 emmet-api-0.60.3/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.759165 emmet-api-0.60.3/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 20:24:03.000000 emmet-api-0.60.3/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-20 20:24:04.000000 emmet-api-0.60.3/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:24:03.000000 emmet-api-0.60.3/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:24:03.000000 emmet-api-0.60.3/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 20:24:03.000000 emmet-api-0.60.3/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 20:24:03.000000 emmet-api-0.60.3/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 20:23:57.000000 emmet-api-0.60.3/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-20 20:23:57.000000 emmet-api-0.60.3/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-20 20:23:57.000000 emmet-api-0.60.3/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-20 20:23:57.000000 emmet-api-0.60.3/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:24:04.771165 emmet-api-0.60.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 20:23:57.000000 emmet-api-0.60.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-20 20:23:57.000000 emmet-api-0.60.3/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.743165 emmet-api-0.60.3/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.763165 emmet-api-0.60.3/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.767165 emmet-api-0.60.3/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:24:04.771165 emmet-api-0.60.3/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-20 20:23:57.000000 emmet-api-0.60.3/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.60.2/Dockerfile` & `emmet-api-0.60.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/app.py` & `emmet-api-0.60.3/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/api.py` & `emmet-api-0.60.3/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.60.3/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.60.3/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/documentation.py` & `emmet-api-0.60.3/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/global_header.py` & `emmet-api-0.60.3/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/core/settings.py` & `emmet-api-0.60.3/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.60.3/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.60.3/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.60.3/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.60.3/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.60.3/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/_messages/resources.py` & `emmet-api-0.60.3/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/dois/resources.py` & `emmet-api-0.60.3/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.60.3/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.60.3/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.60.3/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.60.3/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.60.3/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.60.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.60.3/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.60.3/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.60.3/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.60.3/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/utils.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.60.3/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.60.3/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/legacy_resources.py` & `emmet-api-0.60.3/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/material_resources.py` & `emmet-api-0.60.3/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/molecule_resources.py` & `emmet-api-0.60.3/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/requirements/deployment.txt` & `emmet-api-0.60.3/requirements/deployment.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
@@ -38,36 +38,36 @@
     #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -81,15 +81,15 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (emmet/emmet-api/setup.py)
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn-tschaume
 httpcore==0.17.3
     # via dnspython
@@ -110,17 +110,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (emmet/emmet-api/setup.py)
@@ -175,14 +175,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
@@ -213,15 +214,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.14
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -242,31 +243,31 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.11
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.10.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.2
-    # via
-    #   anyio
-    #   cattrs
 fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -102,17 +106,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -164,14 +168,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
@@ -201,15 +206,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -230,31 +235,31 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -283,15 +288,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -311,15 +319,14 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
@@ -333,12 +340,12 @@
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -97,30 +101,44 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -137,17 +155,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -196,15 +214,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -232,15 +250,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -252,14 +270,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -267,15 +286,17 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -307,15 +328,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -347,53 +368,53 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -409,15 +430,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -446,49 +470,55 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via importlib-metadata
+zipp==3.16.2
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.11.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.100.0
     # via
@@ -73,18 +77,22 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -98,17 +106,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -160,14 +168,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
@@ -197,15 +206,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -226,31 +235,31 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -279,15 +288,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -328,12 +340,12 @@
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,30 +62,35 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
+exceptiongroup==1.1.2
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
 fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
@@ -92,30 +101,44 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -132,17 +155,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -191,15 +214,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -227,15 +250,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -247,14 +270,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -262,15 +286,17 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -302,15 +328,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -342,53 +368,53 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -404,15 +430,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -427,57 +456,69 @@
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
 threadpoolctl==3.2.0
     # via scikit-learn
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via importlib-metadata
+zipp==3.16.2
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.8.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.10.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -77,31 +81,28 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -109,17 +110,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -151,15 +152,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.24.4
+numpy==1.25.1
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -171,29 +172,28 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -210,15 +210,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -239,45 +239,45 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -292,15 +292,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -320,39 +323,34 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.16.2
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -97,40 +101,41 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -147,17 +152,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -206,15 +211,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -242,15 +247,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.24.4
+numpy==1.25.1
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -262,14 +267,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -277,17 +283,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -319,15 +323,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -359,53 +363,53 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -421,15 +425,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -458,15 +465,15 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
     #   aioitertools
     #   bytecode
@@ -485,28 +492,28 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.9.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -77,28 +81,28 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -106,17 +110,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -168,14 +172,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
@@ -205,15 +210,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -234,31 +239,31 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -287,15 +292,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -315,39 +323,34 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.16.2
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.10_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -97,37 +101,34 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -144,17 +145,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -203,15 +204,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -259,14 +260,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -274,15 +276,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -314,15 +316,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -354,39 +356,39 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -416,15 +418,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -453,55 +458,49 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.16.2
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.8.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -77,24 +81,35 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -102,17 +117,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -144,15 +159,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -164,27 +179,30 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -201,15 +219,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -230,45 +248,45 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -283,15 +301,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -311,34 +332,39 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via importlib-metadata
+zipp==3.16.2
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.11_extras.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,35 +62,30 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.2
-    # via
-    #   anyio
-    #   cattrs
-    #   pytest
 fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
@@ -97,22 +96,26 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -137,17 +140,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -196,15 +199,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -252,14 +255,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -267,15 +271,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -307,15 +311,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -347,39 +351,39 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -409,15 +413,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -432,35 +439,29 @@
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
 threadpoolctl==3.2.0
     # via scikit-learn
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   mypy
     #   pydantic
@@ -469,26 +470,26 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.8.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,96 +1,115 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
+exceptiongroup==1.1.2
+    # via
+    #   anyio
+    #   cattrs
 fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -98,17 +117,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -140,15 +159,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -160,27 +179,30 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -197,15 +219,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -226,45 +248,45 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -279,15 +301,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -307,33 +332,39 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via importlib-metadata
+zipp==3.16.2
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.100.0
     # via
@@ -92,22 +96,26 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -132,17 +140,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -191,15 +199,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -247,14 +255,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -262,15 +271,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -302,15 +311,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -342,39 +351,39 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -404,15 +413,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -436,15 +448,15 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
     #   ddtrace
     #   emmet-core
@@ -458,26 +470,26 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.9.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -77,31 +81,32 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -109,17 +114,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -151,15 +156,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.24.4
+numpy==1.25.1
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -171,29 +176,28 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -210,15 +214,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -239,45 +243,45 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -292,15 +296,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -345,14 +352,14 @@
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.60.3/requirements/macos-latest_py3.9_extras.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -97,40 +101,41 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -147,17 +152,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -206,15 +211,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -242,15 +247,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.24.4
+numpy==1.25.1
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -262,14 +267,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -277,17 +283,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -319,15 +323,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -359,53 +363,53 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -421,15 +425,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -458,15 +465,15 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
     #   aioitertools
     #   bytecode
@@ -485,28 +492,28 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.9.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
     # via matplotlib
 cryptography==41.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -77,18 +81,22 @@
     # via mongogrant
 fonttools==4.41.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
+httpcore==0.17.3
+    # via dnspython
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
@@ -106,17 +114,17 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 maggma==0.51.19
     # via emmet-api (setup.py)
@@ -168,14 +176,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
@@ -205,15 +214,15 @@
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
 pydash==7.0.5
     # via maggma
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -234,31 +243,31 @@
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -287,15 +296,18 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -340,14 +352,14 @@
     # via emmet-api (setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
+zipp==3.16.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.60.3/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via starlette
+    # via
+    #   httpcore
+    #   starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.3
+boto3==1.28.5
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.3
+botocore==1.31.5
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
-    # via requests
+    # via
+    #   httpcore
+    #   requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
-click==8.1.5
+click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
@@ -58,25 +62,25 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.16.0
+ddtrace==1.16.1
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.60.1
+emmet-core[all]==0.60.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
@@ -97,37 +101,34 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.32.0
+griffe==0.32.3
     # via mkdocstrings-python
-gunicorn==20.1.0
+gunicorn==21.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via uvicorn-tschaume
+    # via
+    #   httpcore
+    #   uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
+httpcore==0.17.3
+    # via dnspython
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -144,17 +145,17 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.3
+jsonschema==4.18.4
     # via maggma
-jsonschema-specifications==2023.6.1
+jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
@@ -203,15 +204,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.2
+mkdocstrings-python==1.2.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -259,14 +260,15 @@
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
 orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
+    #   gunicorn
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -274,15 +276,15 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.1
+platformdirs==3.9.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
@@ -314,15 +316,15 @@
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.7.11
+pymatgen==2023.7.17
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -354,39 +356,39 @@
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-referencing==0.29.1
+referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.10
+rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -416,15 +418,18 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   dnspython
+    #   httpcore
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -453,55 +458,49 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==68.0.0.1
+types-setuptools==68.0.0.2
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.23.1
+virtualenv==20.24.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.16.1
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.16.2
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.60.2/setup.py` & `emmet-api-0.60.3/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/_consumer/test_query_operators.py` & `emmet-api-0.60.3/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/_general_store/test_query_operators.py` & `emmet-api-0.60.3/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/core/test_mapi.py` & `emmet-api-0.60.3/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.60.3/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/electrodes/test_utils.py` & `emmet-api-0.60.3/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/materials/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/materials/test_utils.py` & `emmet-api-0.60.3/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/summary/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.60.3/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.60.3/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/synthesis/test_utils.py` & `emmet-api-0.60.3/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/tasks/test_utils.py` & `emmet-api-0.60.3/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/materials/xas/test_query_operators.py` & `emmet-api-0.60.3/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/tasks/test_utils.py` & `emmet-api-0.60.3/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.60.2/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.60.3/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

