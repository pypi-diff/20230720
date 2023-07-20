# Comparing `tmp/pyglove-0.4.1.dev20230719.tar.gz` & `tmp/pyglove-0.4.1.dev20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.1.dev20230719.tar", last modified: Wed Jul 19 08:06:39 2023, max compression
+gzip compressed data, was "pyglove-0.4.1.dev20230720.tar", last modified: Thu Jul 20 08:06:49 2023, max compression
```

## Comparing `pyglove-0.4.1.dev20230719.tar` & `pyglove-0.4.1.dev20230720.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.815286 pyglove-0.4.1.dev20230719/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-19 08:06:39.815286 pyglove-0.4.1.dev20230719/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-19 08:06:37.000000 pyglove-0.4.1.dev20230719/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.799286 pyglove-0.4.1.dev20230719/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.799286 pyglove-0.4.1.dev20230719/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.799286 pyglove-0.4.1.dev20230719/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.799286 pyglove-0.4.1.dev20230719/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.803286 pyglove-0.4.1.dev20230719/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.803286 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.803286 pyglove-0.4.1.dev20230719/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.807286 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78193 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    62670 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35049 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    83433 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.807286 pyglove-0.4.1.dev20230719/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.811286 pyglove-0.4.1.dev20230719/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.811286 pyglove-0.4.1.dev20230719/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.811286 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.811286 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.811286 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.815286 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:06:39.799286 pyglove-0.4.1.dev20230719/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-19 08:06:39.000000 pyglove-0.4.1.dev20230719/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-19 08:06:39.000000 pyglove-0.4.1.dev20230719/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:06:39.000000 pyglove-0.4.1.dev20230719/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 08:06:39.000000 pyglove-0.4.1.dev20230719/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 08:06:39.000000 pyglove-0.4.1.dev20230719/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:06:39.815286 pyglove-0.4.1.dev20230719/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-19 08:06:21.000000 pyglove-0.4.1.dev20230719/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-20 08:06:47.000000 pyglove-0.4.1.dev20230720/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.391942 pyglove-0.4.1.dev20230720/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.391942 pyglove-0.4.1.dev20230720/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.391942 pyglove-0.4.1.dev20230720/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.391942 pyglove-0.4.1.dev20230720/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.395942 pyglove-0.4.1.dev20230720/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.395942 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.395942 pyglove-0.4.1.dev20230720/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.399942 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78193 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62670 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36064 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83881 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.399942 pyglove-0.4.1.dev20230720/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.403942 pyglove-0.4.1.dev20230720/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.403942 pyglove-0.4.1.dev20230720/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.403942 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:06:49.391942 pyglove-0.4.1.dev20230720/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-20 08:06:49.000000 pyglove-0.4.1.dev20230720/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-20 08:06:49.000000 pyglove-0.4.1.dev20230720/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:06:49.000000 pyglove-0.4.1.dev20230720/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 08:06:49.000000 pyglove-0.4.1.dev20230720/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 08:06:49.000000 pyglove-0.4.1.dev20230720/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:06:49.407942 pyglove-0.4.1.dev20230720/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 08:06:38.000000 pyglove-0.4.1.dev20230720/setup.py
```

### Comparing `pyglove-0.4.1.dev20230719/LICENSE` & `pyglove-0.4.1.dev20230720/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/PKG-INFO` & `pyglove-0.4.1.dev20230720/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.1.dev20230719
+Version: 0.4.1.dev20230720
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.1.dev20230719/README.md` & `pyglove-0.4.1.dev20230720/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 Object = symbolic.Object
 ClassWrapper = symbolic.ClassWrapper
 Functor = symbolic.Functor
 
 # Decorator for declaring symbolic. members for `pg.Object`.
 members = symbolic.members
 
+# Decorator for updating the __init__ signature of `pg.Object`.
+use_init_args = symbolic.use_init_args
+
 #
 # Methods for making symbolic types.
 #
 
 # Function/Decorator for symbolizing existing types.
 symbolize = symbolic.symbolize
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/detouring/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.1.dev20230720/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/base.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/categorical.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/custom.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/custom_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/deduping.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/numerical.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/random.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/random_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/space.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/space_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/sweeping.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/base.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/categorical.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/custom.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/derived.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/iter.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/numerical.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/object_template.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/logging.py` & `pyglove-0.4.1.dev20230720/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/logging_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/missing.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/object_factory.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/rule_based.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.dict import Dict
 
 from pyglove.core.symbolic.object import ObjectMeta
 from pyglove.core.symbolic.object import Object
 from pyglove.core.symbolic.object import members
+from pyglove.core.symbolic.object import use_init_args
 
 from pyglove.core.symbolic.functor import Functor
 from pyglove.core.symbolic.functor import functor
 from pyglove.core.symbolic.functor import functor_class
 from pyglove.core.symbolic.functor import as_functor
 
 from pyglove.core.symbolic.class_wrapper import ClassWrapper
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/base.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/contextual.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/contextual.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/contextual_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/dict.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/diff.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,14 @@
     def __ne__(self, other):
       return not self.__eq__(other)
 
   MISSING = _Missing()
 
   def _on_bound(self):
     super()._on_bound()
-    if self.left == Diff.MISSING and self.right == Diff.MISSING:
-      raise ValueError(
-          'At least one of \'left\' and \'right\' should be specified.')
     if self.children:
       if not isinstance(self.left, type):
         raise ValueError(
             f'\'left\' must be a type when \'children\' is specified. '
             f'Encountered: {self.left!r}.')
       if not isinstance(self.right, type):
         raise ValueError(
@@ -106,15 +103,18 @@
       self,
       compact: bool = False,
       verbose: bool = True,
       root_indent: int = 0,
       **kwargs):
     """Override format to conditionally print the shared value or the diff."""
     if not bool(self):
-      # When there is no diff, we simply return the value.
+      if self.value == Diff.MISSING:
+        return 'No diff'
+      # When there is no diff, but the same value needs to be displayed
+      # we simply return the value.
       return object_utils.format(
           self.value, compact, verbose, root_indent, **kwargs)
     if self.is_leaf:
       exclude_keys = kwargs.pop('exclude_keys', None)
       exclude_keys = exclude_keys or set()
       exclude_keys.add('children')
       return super().format(
@@ -178,23 +178,20 @@
     class B(A):
       pass
 
 
     # Diff the same object.
     pg.diff(A(1, 2), A(1, 2))
 
-    >> None
+    >> No diff
 
     # Diff the same object with mode 'same'.
     pg.diff(A(1, 2), A(1, 2), mode='same')
 
-    >> A(
-    >>   x = 1,
-    >>   y = 2
-    >> )
+    >> A(1, 2)
 
     # Diff different objects of the same type.
     pg.diff(A(1, 2), A(1, 3))
 
     >> A(
     >>   y = Diff(
     >>     left=2,
@@ -335,11 +332,13 @@
         # no clash.
         if not same_type or mode != 'diff':
           diff_value['_type'] = Diff(xt, yt)
       else:
         diff_value = Diff(xt, yt, children=diff_value)
     return diff_value, has_diff
 
-  diff_value, _ = _diff(left, right)
+  diff_value, has_diff = _diff(left, right)
+  if not has_diff and mode == 'diff':
+    diff_value = Diff()
   if flatten:
     diff_value = object_utils.flatten(diff_value)
   return diff_value
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/diff_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,35 @@
     class B(Object):
       pass
 
     self.assertTrue(bool(Diff(1, 2)))
     self.assertTrue(bool(Diff(A, B)))
     self.assertTrue(bool(Diff(A(1), A(2))))
     self.assertTrue(bool(Diff(A, A, children={'x': Diff(1, 2)})))
+    self.assertFalse(bool(Diff()))
     self.assertFalse(bool(Diff(1, 1)))
     self.assertFalse(bool(Diff(A, A)))
     self.assertFalse(bool(Diff(A(1), A(1))))
 
     self.assertTrue(Diff(1, 2).is_leaf)
     self.assertFalse(
         Diff(int, int, children={'x': Diff(1, 2)}).is_leaf)
 
     self.assertEqual(Diff(1, 1), 1)
     self.assertEqual(Diff(1, 1), Diff(1, 1))
     self.assertNotEqual(Diff(1, 1), 2)
     self.assertNotEqual(Diff(1, 1), Diff(1, 2))
 
     self.assertEqual(
+        repr(Diff()), 'No diff')
+    self.assertEqual(
         repr(Diff(A(1), A(1))), 'A(x=1)')
     self.assertEqual(
+        repr(Dict(a=Diff(A(1), A(1)))), '{a=A(x=1)}')
+    self.assertEqual(
         repr(Diff(A(1), A(2))), 'Diff(left=A(x=1), right=A(x=2))')
     self.assertEqual(
         repr(Diff(A, A, children={'x': Diff(1, 2)})),
         'A(x=Diff(left=1, right=2))')
     self.assertEqual(
         repr(Diff(A, B, children={
             'x': Diff(1, 2),
@@ -72,19 +77,14 @@
             '0': Diff(1, 2),
             '1': Diff(Diff.MISSING, 3)
         })),
         '[0=Diff(left=1, right=2), 1=Diff(left=MISSING, right=3)]')
 
     with self.assertRaisesRegex(
         ValueError,
-        'At least one of \'left\' and \'right\' should be specified.'):
-      Diff()
-
-    with self.assertRaisesRegex(
-        ValueError,
         '\'left\' must be a type when \'children\' is specified.'):
       Diff(1, int, children={'x': Diff(3, 4)})
 
     with self.assertRaisesRegex(
         ValueError,
         '\'right\' must be a type when \'children\' is specified.'):
       Diff(int, 2, children={'x': Diff(3, 4)})
@@ -92,29 +92,30 @@
     with self.assertRaisesRegex(
         ValueError,
         '\'value\' cannot be accessed when \'left\' and \'right\' '
         'are not the same.'):
       _ = Diff(1, 2).value
 
   def test_diff_on_simple_types(self):
-    self.assertEqual(pg_diff(1, 1), Diff(1, 1))
+    self.assertEqual(pg_diff(1, 1), Diff())
     self.assertEqual(pg_diff(1, 1, mode='same'), Diff(1, 1))
     self.assertEqual(pg_diff(1, 1, flatten=True, mode='same'), Diff(1, 1))
     self.assertEqual(pg_diff(1, 2), Diff(1, 2))
     self.assertEqual(pg_diff(1, 2, mode='same'), Diff(1, 2))
     self.assertEqual(pg_diff(1, 2, flatten=True, mode='same'), Diff(1, 2))
 
   def test_diff_on_list(self):
 
     @pg_members([('x', pg_typing.Any())])
     class A(Object):
       pass
 
     # List vs. list.
-    self.assertEqual(pg_diff([A(1)], [A(1)]), Diff([A(1)], [A(1)]))
+    self.assertEqual(pg_diff([A(1)], [A(1)]), Diff())
+    self.assertEqual(pg_diff([A(1)], [A(1)], mode='same'), Diff([A(1)], [A(1)]))
     self.assertEqual(
         pg_diff([A(1)], [A(0)]),
         Diff(left=List, right=List, children={
             '0': Diff(A, A, children={
                 'x': Diff(1, 0)
             })}))
 
@@ -125,15 +126,19 @@
 
     @pg_members([('x', pg_typing.Any())])
     class A(Object):
       pass
 
     # Dict vs. dict.
     self.assertEqual(
-        pg_diff({'a': A(1)}, {'a': A(1)}), Diff({'a': A(1)}, {'a': A(1)}))
+        pg_diff({'a': A(1)}, {'a': A(1)}),
+        Diff())
+    self.assertEqual(
+        pg_diff({'a': A(1)}, {'a': A(1)}, mode='same'),
+        Diff({'a': A(1)}, {'a': A(1)}))
     self.assertEqual(
         pg_diff({'a': A(1), 'b': A(2), 'c': A(3)},
                 {'a': A(1), 'b': A(3), 'd': A(4)}),
         Diff(dict, dict, children={
             'b': Diff(A, A, children={
                 'x': Diff(2, 3)
             }),
@@ -169,15 +174,16 @@
     class B(Object):
       pass
 
     class C(B):
       pass
 
     # Same types.
-    self.assertEqual(pg_diff(A(1), A(1)), Diff(A(1), A(1)))
+    self.assertEqual(pg_diff(A(1), A(1)), Diff())
+    self.assertEqual(pg_diff(A(1), A(1), mode='same'), Diff(A(1), A(1)))
     self.assertEqual(
         pg_diff(B(1, 2), B(1, 3)),
         Diff(B, B, children={'y': Diff(2, 3)}))
 
     # Different types without collapse.
     self.assertEqual(
         pg_diff(B(1, 2), C(1, 2)),
@@ -251,15 +257,15 @@
     @pg_members([('x', pg_typing.Any()), ('y', pg_typing.Any())])
     class B(Object):
       pass
 
     class C(B):
       pass
 
-    self.assertEqual(pg_diff(A(1), A(1), mode='diff'), Diff(A(1), A(1)))
+    self.assertEqual(pg_diff(A(1), A(1), mode='diff'), Diff())
     self.assertEqual(pg_diff(A(1), A(1), mode='same'), Diff(A(1), A(1)))
     self.assertEqual(pg_diff(A(1), A(1), mode='both'), Diff(A(1), A(1)))
 
     self.assertEqual(
         pg_diff(B(1, 2), B(1, 3), mode='diff'),
         Diff(B, B, children={'y': Diff(2, 3)}))
     self.assertEqual(
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/flags.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/functor.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/list.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/object.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -943,7 +943,41 @@
         init_arg_list=init_arg_list,
         metadata=metadata,
         serialization_key=serialization_key,
         additional_keys=additional_keys,
     )
     return cls
   return typing.cast(pg_typing.Decorator, _decorator)
+
+
+def use_init_args(init_arg_list: Sequence[str]) -> pg_typing.Decorator:
+  """Decorator for updating the `__init__` signature of a `pg.Object` subclass.
+
+  Examples::
+
+    @pg.use_init_args(['x', 'y', '*z'])
+    class Foo(pg.Object):
+      y: int
+      x: str
+      z: list[int]
+
+    f = Foo('abc', 1, 2, 3)
+    assert f.x == 'abc'
+    assert f.y == 1
+    assert f.z == [2, 3]
+
+  Args:
+    init_arg_list: A sequence of attribute names that will be used as the
+      positional arguments of `__init__`. The last element could be the name of
+      a list-type attribute, indicating it's used as `*args`. Keyword-only
+      arguments are not needed to be present in this list, which will be figured
+      out automatically based on class' schema.
+
+  Returns:
+    a decorator function that updates the `__init__` signature.
+  """
+  def _decorator(cls):
+    schema_utils.update_schema(
+        cls, [], extend=True, init_arg_list=init_arg_list
+    )
+    return cls
+  return typing.cast(pg_typing.Decorator, _decorator)
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from pyglove.core.symbolic.base import query as pg_query
 from pyglove.core.symbolic.base import traverse as pg_traverse
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.functor import functor as pg_functor
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.object import members as pg_members
 from pyglove.core.symbolic.object import Object
+from pyglove.core.symbolic.object import use_init_args as pg_use_init_args
 from pyglove.core.symbolic.origin import Origin
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
 MISSING_VALUE = object_utils.MISSING_VALUE
 
@@ -1689,14 +1690,31 @@
     self.assertEqual(b.sym_init_args, dict(x=1, y1=2, y2=3, y3=4))
 
     # Not okay: `z` does not conform to regex `y.*`.
     with self.assertRaisesRegex(
         TypeError, 'got unexpected keyword argument: \'z\''):
       _ = B(1, z=2)
 
+  def test_use_init_args(self):
+
+    @pg_use_init_args(['x', 'y', '*z'])
+    class A(Object):
+      y: int
+      x: str
+      z: list[str]
+      p: str
+      q: int
+
+    a = A('foo', 1, 'a', 'b', p='bar', q=2)
+    self.assertEqual(a.x, 'foo')
+    self.assertEqual(a.y, 1)
+    self.assertEqual(a.z, ['a', 'b'])
+    self.assertEqual(a.p, 'bar')
+    self.assertEqual(a.q, 2)
+
   def test_serialization_key(self):
 
     @pg_members([
         ('x', pg_typing.Int())
     ], serialization_key='ClassA')
     class A(Object):
       pass
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/origin.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/backend.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/early_stopping.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/protocols.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/sample.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/annotation_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,25 @@
   # Handling list.
   if origin in (list, typing.List):
     return vs.List(
         _value_spec_from_annotation(
             args[0], True)) if args else vs.List(vs.Any())
   # Handling tuple.
   elif origin in (tuple, typing.Tuple):
-    if args:
-      return vs.Tuple([_value_spec_from_annotation(arg, True) for arg in args])
-    else:
+    if not args:
       return vs.Tuple(vs.Any())
+    else:
+      if args[-1] is ...:
+        if len(args) != 2:
+          raise TypeError(
+              f'Tuple with ellipsis should have exact 2 type arguments. '
+              f'Encountered: {annotation}.')
+        return vs.Tuple(_value_spec_from_type_annotation(args[0], False))
+      return vs.Tuple([_value_spec_from_type_annotation(arg, False)
+                       for arg in args])
   # Handle sequence.
   elif origin in (collections.abc.Sequence,):
     elem = _value_spec_from_annotation(args[0], True) if args else vs.Any()
     return vs.Union([vs.List(elem), vs.Tuple(elem)])
   # Handling dict.
   elif origin in (dict, typing.Dict, collections.abc.Mapping):
     if not args:
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/annotation_conversion_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,19 @@
 
   def test_tuple(self):
     self.assertEqual(ValueSpec.from_annotation(tuple, True), vs.Tuple(vs.Any()))
     self.assertEqual(
         ValueSpec.from_annotation(typing.Tuple, True), vs.Tuple(vs.Any()))
     self.assertEqual(
         ValueSpec.from_annotation(tuple[int], True), vs.Tuple([vs.Int()]))
+    self.assertEqual(
+        ValueSpec.from_annotation(tuple[int, ...], True), vs.Tuple(vs.Int()))
+    with self.assertRaisesRegex(
+        TypeError, 'Tuple with ellipsis should have exact 2 type arguments'):
+      ValueSpec.from_annotation(tuple[...], True)
 
   def test_sequence(self):
     self.assertEqual(
         ValueSpec.from_annotation(typing.Sequence[int], True),
         vs.Union([vs.List(vs.Int()), vs.Tuple(vs.Int())]))
 
   def test_dict(self):
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/key_specs.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/value_specs.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.1.dev20230720/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/base.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/neat.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/where.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/base.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/base.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/maths.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.1.dev20230720/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.1.dev20230720/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.1.dev20230719
+Version: 0.4.1.dev20230720
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.1.dev20230719/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.1.dev20230720/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230719/setup.py` & `pyglove-0.4.1.dev20230720/setup.py`

 * *Files identical despite different names*

