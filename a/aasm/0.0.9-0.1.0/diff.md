# Comparing `tmp/aasm-0.0.9.tar.gz` & `tmp/aasm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aasm-0.0.9.tar", last modified: Sun Dec 26 01:26:51 2021, max compression
+gzip compressed data, was "aasm-0.1.0.tar", last modified: Thu Jul 20 12:20:03 2023, max compression
```

## Comparing `aasm-0.0.9.tar` & `aasm-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,90 @@
--rw-r--r--   0        0        0       25 2021-12-08 01:21:36.000000 aasm-0.0.9/.gitignore
--rw-r--r--   0        0        0      281 2021-12-23 00:23:12.642979 aasm-0.0.9/Pipfile
--rw-r--r--   0        0        0    45740 2021-12-23 00:23:12.646312 aasm-0.0.9/Pipfile.lock
--rw-r--r--   0        0        0     2116 2021-12-26 01:22:21.030054 aasm-0.0.9/README.md
--rw-r--r--   0        0        0      199 2021-12-26 01:23:38.713816 aasm-0.0.9/aasm/__init__.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/generating/__init__.py
--rw-r--r--   0        0        0      841 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/generating/code.py
--rw-r--r--   0        0        0      696 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/generating/python_code.py
--rw-r--r--   0        0        0     3112 2021-12-26 01:16:06.464684 aasm-0.0.9/aasm/generating/python_graph.py
--rw-r--r--   0        0        0    20486 2021-12-25 21:43:20.387973 aasm-0.0.9/aasm/generating/python_spade.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/__init__.py
--rw-r--r--   0        0        0     1993 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/action.py
--rw-r--r--   0        0        0     7612 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/intermediate/agent.py
--rw-r--r--   0        0        0    11623 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/intermediate/argument.py
--rw-r--r--   0        0        0     1391 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/behaviour.py
--rw-r--r--   0        0        0     1065 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/block.py
--rw-r--r--   0        0        0      400 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/declaration.py
--rw-r--r--   0        0        0     2484 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/intermediate/graph.py
--rw-r--r--   0        0        0     7019 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/instruction.py
--rw-r--r--   0        0        0     1790 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/message.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/__init__.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/__init__.py
--rw-r--r--   0        0        0     2060 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/action.py
--rw-r--r--   0        0        0     1389 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/agent.py
--rw-r--r--   0        0        0     2917 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/parsing/op/behav.py
--rw-r--r--   0        0        0      574 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/clr.py
--rw-r--r--   0        0        0     3002 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/conditional.py
--rw-r--r--   0        0        0     1220 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/decl.py
--rw-r--r--   0        0        0     2662 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/defg.py
--rw-r--r--   0        0        0      413 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/eblock.py
--rw-r--r--   0        0        0     1392 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/graph.py
--rw-r--r--   0        0        0      681 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/len.py
--rw-r--r--   0        0        0     1801 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/list.py
--rw-r--r--   0        0        0     1096 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/math.py
--rw-r--r--   0        0        0     1570 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/message.py
--rw-r--r--   0        0        0     4013 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/parsing/op/prm.py
--rw-r--r--   0        0        0     2284 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/rand.py
--rw-r--r--   0        0        0      722 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/remen.py
--rw-r--r--   0        0        0      575 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/round.py
--rw-r--r--   0        0        0      819 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/send.py
--rw-r--r--   0        0        0      678 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/set.py
--rw-r--r--   0        0        0      579 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/size.py
--rw-r--r--   0        0        0      794 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/subs.py
--rw-r--r--   0        0        0     4891 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/parse.py
--rw-r--r--   0        0        0     4227 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/state.py
--rw-r--r--   0        0        0     1632 2021-12-25 20:05:31.055501 aasm-0.0.9/aasm/translate.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/utils/__init__.py
--rw-r--r--   0        0        0      428 2021-12-08 02:46:46.000000 aasm-0.0.9/aasm/utils/exception.py
--rw-r--r--   0        0        0     1302 2021-12-25 20:05:31.055501 aasm-0.0.9/aasm/utils/validation.py
--rw-r--r--   0        0        0     2219 2021-12-26 01:25:27.754420 aasm-0.0.9/out
--rw-r--r--   0        0        0      273 2021-12-08 01:19:10.000000 aasm-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      413 2021-12-25 21:36:52.089081 aasm-0.0.9/test.aa
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 aasm-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       37 2022-12-17 05:36:13.052938 aasm-0.1.0/.gitignore
+-rw-r--r--   0        0        0      172 2023-05-22 10:06:04.170277 aasm-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      709 2022-12-17 01:24:38.903482 aasm-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11941 2023-07-18 15:16:59.750006 aasm-0.1.0/DOCS.md
+-rw-r--r--   0        0        0     1084 2023-05-22 10:07:10.253613 aasm-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0      349 2023-05-22 10:07:10.253613 aasm-0.1.0/Pipfile
+-rw-r--r--   0        0        0    66634 2023-05-22 10:07:10.256947 aasm-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0     3169 2022-12-17 01:24:38.906815 aasm-0.1.0/README.md
+-rw-r--r--   0        0        0      303 2023-07-20 12:19:13.796717 aasm-0.1.0/aasm/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/generating/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/code.py
+-rw-r--r--   0        0        0     1250 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/python_code.py
+-rw-r--r--   0        0        0    15718 2023-07-19 14:25:12.646717 aasm-0.1.0/aasm/generating/python_graph.py
+-rw-r--r--   0        0        0     1860 2023-07-20 12:15:22.310040 aasm-0.1.0/aasm/generating/python_module.py
+-rw-r--r--   0        0        0    49947 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/python_spade.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/intermediate/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/action.py
+-rw-r--r--   0        0        0     9515 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/agent.py
+-rw-r--r--   0        0        0    20777 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/intermediate/argument.py
+-rw-r--r--   0        0        0     1323 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/intermediate/behaviour.py
+-rw-r--r--   0        0        0     4263 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/block.py
+-rw-r--r--   0        0        0     1225 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/declaration.py
+-rw-r--r--   0        0        0     8031 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/graph.py
+-rw-r--r--   0        0        0    12166 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/instruction.py
+-rw-r--r--   0        0        0     4013 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/message.py
+-rw-r--r--   0        0        0       79 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/module.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/__init__.py
+-rw-r--r--   0        0        0     5094 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/instruction.py
+-rw-r--r--   0        0        0     8168 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/module.py
+-rw-r--r--   0        0        0      473 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/modules/type.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/__init__.py
+-rw-r--r--   0        0        0     2130 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/action.py
+-rw-r--r--   0        0        0     1474 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/agent.py
+-rw-r--r--   0        0        0     3033 2022-12-17 05:28:29.899621 aasm-0.1.0/aasm/parsing/op/behav.py
+-rw-r--r--   0        0        0      619 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/clr.py
+-rw-r--r--   0        0        0     2808 2022-12-17 05:28:29.922954 aasm-0.1.0/aasm/parsing/op/conditional.py
+-rw-r--r--   0        0        0     1942 2023-07-18 15:17:32.240008 aasm-0.1.0/aasm/parsing/op/decl.py
+-rw-r--r--   0        0        0     3956 2023-07-19 14:25:12.646717 aasm-0.1.0/aasm/parsing/op/defg.py
+-rw-r--r--   0        0        0      953 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/defnode.py
+-rw-r--r--   0        0        0     2340 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/deftype.py
+-rw-r--r--   0        0        0      427 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/eblock.py
+-rw-r--r--   0        0        0     2378 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/graph.py
+-rw-r--r--   0        0        0      690 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/len.py
+-rw-r--r--   0        0        0     1013 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/list_inclusion.py
+-rw-r--r--   0        0        0     1002 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/list_modification.py
+-rw-r--r--   0        0        0     1418 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/logs.py
+-rw-r--r--   0        0        0      771 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/lr.py
+-rw-r--r--   0        0        0      783 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/lw.py
+-rw-r--r--   0        0        0     1284 2022-12-17 05:28:30.012955 aasm-0.1.0/aasm/parsing/op/math.py
+-rw-r--r--   0        0        0     1056 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/math_exp.py
+-rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/math_mod.py
+-rw-r--r--   0        0        0     1695 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/message.py
+-rw-r--r--   0        0        0     1139 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/module.py
+-rw-r--r--   0        0        0      713 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/mparams.py
+-rw-r--r--   0        0        0     5561 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/parsing/op/prm.py
+-rw-r--r--   0        0        0     2289 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/rand.py
+-rw-r--r--   0        0        0      748 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/remen.py
+-rw-r--r--   0        0        0      620 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/round.py
+-rw-r--r--   0        0        0      606 2022-12-17 05:36:13.052938 aasm-0.1.0/aasm/parsing/op/scale.py
+-rw-r--r--   0        0        0      880 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/send.py
+-rw-r--r--   0        0        0      690 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/parsing/op/set.py
+-rw-r--r--   0        0        0      603 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/size.py
+-rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/subs.py
+-rw-r--r--   0        0        0      893 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/types.py
+-rw-r--r--   0        0        0     6593 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/parse.py
+-rw-r--r--   0        0        0     5804 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/state.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/__init__.py
+-rw-r--r--   0        0        0      839 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/constant.py
+-rw-r--r--   0        0        0     1484 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/macro.py
+-rw-r--r--   0        0        0     7930 2022-12-17 05:36:13.056271 aasm-0.1.0/aasm/preprocessor/preprocessor.py
+-rw-r--r--   0        0        0      292 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/preprocessor_item.py
+-rw-r--r--   0        0        0     2312 2023-07-20 12:15:22.313373 aasm-0.1.0/aasm/translate.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/__init__.py
+-rw-r--r--   0        0        0      428 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/exception.py
+-rw-r--r--   0        0        0      412 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/iteration.py
+-rw-r--r--   0        0        0     2074 2023-07-19 14:27:17.546723 aasm-0.1.0/aasm/utils/validation.py
+-rw-r--r--   0        0        0      673 2023-05-22 10:07:10.256947 aasm-0.1.0/examples/EXAMPLES.md
+-rw-r--r--   0        0        0      837 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/facebook.aasm
+-rw-r--r--   0        0        0      968 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/facebook_macro.aasm
+-rw-r--r--   0        0        0    14394 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/wolfsheep.aasm
+-rw-r--r--   0        0        0    11149 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/basic/wolfsheep_macro.aasm
+-rw-r--r--   0        0        0     1115 2023-07-19 14:25:12.646717 aasm-0.1.0/examples/graphs/barabasi-albert.aasm
+-rw-r--r--   0        0        0     1152 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/graphs/inhomogenous.aasm
+-rw-r--r--   0        0        0     1179 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/graphs/matrix.aasm
+-rw-r--r--   0        0        0     1129 2023-07-19 14:25:12.646717 aasm-0.1.0/examples/graphs/statistical.aasm
+-rw-r--r--   0        0        0     1153 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/modules/facebook_uuid.aasm
+-rw-r--r--   0        0        0      649 2023-07-18 15:21:47.523352 aasm-0.1.0/examples/modules/uuid.aasm.mod
+-rw-r--r--   0        0        0      499 2022-12-17 01:24:38.913482 aasm-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 aasm-0.1.0/PKG-INFO
```

### Comparing `aasm-0.0.9/Pipfile.lock` & `aasm-0.1.0/Pipfile.lock`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7550843253968255%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'7bc2286f2ec11c2899251ee6933ed10df989f3b6b0f622c32cb931b27b697f60'}}",*

 * * "'default'": "{replace: OrderedDict([('cfgv', OrderedDict([('hashes', "*

 * *              "['sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426', "*

 * *              "'sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736']), "*

 * *              '(\'markers\', "python_full_version >= \'3.6.1\'"), (\'version\', \'==3.3.1\')])), '*

 * *              "('distlib', Ordered […]*

```diff
@@ -1,25 +1,143 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "c3ba6183041a3be82a59a27e0a053f579dd1a35202852e08fb58217f6ee527d2"
+            "sha256": "7bc2286f2ec11c2899251ee6933ed10df989f3b6b0f622c32cb931b27b697f60"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
-    "default": {},
+    "default": {
+        "cfgv": {
+            "hashes": [
+                "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
+                "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
+            ],
+            "markers": "python_full_version >= '3.6.1'",
+            "version": "==3.3.1"
+        },
+        "distlib": {
+            "hashes": [
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+            ],
+            "version": "==0.3.6"
+        },
+        "filelock": {
+            "hashes": [
+                "sha256:3199fd0d3faea8b911be52b663dfccceb84c95949dd13179aa21436d1a79c4ce",
+                "sha256:e90b34656470756edf8b19656785c5fea73afa1953f3e1b0d645cef11cab3182"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.10.0"
+        },
+        "identify": {
+            "hashes": [
+                "sha256:69edcaffa8e91ae0f77d397af60f148b6b45a8044b2cc6d99cafa5b04793ff00",
+                "sha256:7671a05ef9cfaf8ff63b15d45a91a1147a03aaccb2976d4e9bd047cbbc508471"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.5.21"
+        },
+        "nodeenv": {
+            "hashes": [
+                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
+                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.7.0"
+        },
+        "platformdirs": {
+            "hashes": [
+                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
+                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.1"
+        },
+        "pre-commit": {
+            "hashes": [
+                "sha256:818f0d998059934d0f81bb3667e3ccdc32da6ed7ccaac33e43dc231561ddaaa9",
+                "sha256:f712d3688102e13c8e66b7d7dbd8934a6dda157e58635d89f7d6fecdca39ce8a"
+            ],
+            "index": "pypi",
+            "version": "==3.2.0"
+        },
+        "pyyaml": {
+            "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0"
+        },
+        "setuptools": {
+            "hashes": [
+                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
+                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==67.6.0"
+        },
+        "virtualenv": {
+            "hashes": [
+                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
+                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==20.21.0"
+        }
+    },
     "develop": {
         "aiohttp": {
             "hashes": [
                 "sha256:02f46fc0e3c5ac58b80d4d56eb0a7c7d97fcef69ace9326289fb9f1955e65cfe",
                 "sha256:0563c1b3826945eecd62186f3f5c7d31abb7391fedc893b7e2b26303b5a9f3fe",
                 "sha256:114b281e4d68302a324dd33abb04778e8557d88947875cbf4e842c2c01a030c5",
                 "sha256:14762875b22d0055f05d12abc7f7d61d5fd4fe4642ce1a249abdf8c700bf1fd8",
@@ -78,162 +196,258 @@
             "hashes": [
                 "sha256:d927a8f9d855c4c00dea9d88fb86ea0d09dd4e7642b2109d2bd93be2f4c17b4e"
             ],
             "version": "==0.5.0"
         },
         "aioxmpp": {
             "hashes": [
-                "sha256:fe655621b2baf73b69356564b839e8066b4789182916fe5200d7fb98f267a8f5"
+                "sha256:a2299e84f6d61137c6a046e2470aeebd8cd25515c1f3cefd681c322242d8056d"
+            ],
+            "version": "==0.13.3"
+        },
+        "anyio": {
+            "hashes": [
+                "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421",
+                "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"
             ],
-            "version": "==0.13.1"
+            "markers": "python_full_version >= '3.6.2'",
+            "version": "==3.6.2"
         },
         "arrow": {
             "hashes": [
-                "sha256:6b2914ef3997d1fd7b37a71ce9dd61a6e329d09e1c7b44f4d3099ca4a5c0933e",
-                "sha256:c2dde3c382d9f7e6922ce636bf0b318a7a853df40ecb383b29192e6c5cc82840"
+                "sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1",
+                "sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.2.1"
+            "version": "==1.2.3"
         },
         "async-timeout": {
             "hashes": [
                 "sha256:0c3c816a028d47f659d6ff5c745cb2acf1f966da1fe5c19c77a70282b25f4c5f",
                 "sha256:4291ca197d287d274d0b6cb5d6f8f8f82d434ed288f962539ff18cc9012f9ea3"
             ],
             "markers": "python_full_version >= '3.5.3'",
             "version": "==3.0.1"
         },
         "attrs": {
             "hashes": [
-                "sha256:149e90d6d8ac20db7a955ad60cf0e6881a3f20d37096140088356da6c716b0b1",
-                "sha256:ef6aaac3ca6cd92904cdd0d83f629a15f18053ec84e6432106f7a4d04ae4f5fb"
+                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
+                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==21.2.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==22.2.0"
         },
         "babel": {
             "hashes": [
-                "sha256:ab49e12b91d937cd11f0b67cb259a57ab4ad2b59ac7a3b41d6c06c0ac5b0def9",
-                "sha256:bc0c176f9f6a994582230df350aa6e05ba2ebe4b3ac317eab29d9be5d2768da0"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.9.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
+        },
+        "black": {
+            "hashes": [
+                "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd",
+                "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555",
+                "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481",
+                "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468",
+                "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9",
+                "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a",
+                "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958",
+                "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580",
+                "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26",
+                "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32",
+                "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8",
+                "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753",
+                "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b",
+                "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074",
+                "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651",
+                "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24",
+                "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6",
+                "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad",
+                "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac",
+                "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221",
+                "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06",
+                "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27",
+                "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648",
+                "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739",
+                "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"
+            ],
+            "index": "pypi",
+            "version": "==23.1.0"
+        },
+        "certifi": {
+            "hashes": [
+                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
+                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2022.12.7"
         },
         "cffi": {
             "hashes": [
-                "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3",
-                "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2",
-                "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636",
-                "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20",
-                "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728",
-                "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27",
-                "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66",
-                "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443",
-                "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0",
-                "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7",
-                "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39",
-                "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605",
-                "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a",
-                "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37",
-                "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029",
-                "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139",
-                "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc",
-                "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df",
-                "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14",
-                "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880",
-                "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2",
-                "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a",
-                "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e",
-                "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474",
-                "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024",
-                "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8",
-                "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0",
-                "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e",
-                "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a",
-                "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e",
-                "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032",
-                "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6",
-                "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e",
-                "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b",
-                "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e",
-                "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954",
-                "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962",
-                "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c",
-                "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4",
-                "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55",
-                "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962",
-                "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023",
-                "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c",
-                "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6",
-                "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8",
-                "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382",
-                "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7",
-                "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc",
-                "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
-                "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
-            "version": "==1.15.0"
+            "version": "==1.15.1"
         },
         "chardet": {
             "hashes": [
                 "sha256:0d6f53a15db4120f2b08c94f11e7d93d2c911ee118b6b30a04ec3ee8310179fa",
                 "sha256:f864054d66fd9118f2e67044ac8981a54775ec5b67aed0441892edb553d21da5"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==4.0.0"
         },
+        "click": {
+            "hashes": [
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.3"
+        },
         "cryptography": {
             "hashes": [
-                "sha256:0a817b961b46894c5ca8a66b599c745b9a3d9f822725221f0e0fe49dc043a3a3",
-                "sha256:2d87cdcb378d3cfed944dac30596da1968f88fb96d7fc34fdae30a99054b2e31",
-                "sha256:30ee1eb3ebe1644d1c3f183d115a8c04e4e603ed6ce8e394ed39eea4a98469ac",
-                "sha256:391432971a66cfaf94b21c24ab465a4cc3e8bf4a939c1ca5c3e3a6e0abebdbcf",
-                "sha256:39bdf8e70eee6b1c7b289ec6e5d84d49a6bfa11f8b8646b5b3dfe41219153316",
-                "sha256:4caa4b893d8fad33cf1964d3e51842cd78ba87401ab1d2e44556826df849a8ca",
-                "sha256:53e5c1dc3d7a953de055d77bef2ff607ceef7a2aac0353b5d630ab67f7423638",
-                "sha256:596f3cd67e1b950bc372c33f1a28a0692080625592ea6392987dba7f09f17a94",
-                "sha256:5d59a9d55027a8b88fd9fd2826c4392bd487d74bf628bb9d39beecc62a644c12",
-                "sha256:6c0c021f35b421ebf5976abf2daacc47e235f8b6082d3396a2fe3ccd537ab173",
-                "sha256:73bc2d3f2444bcfeac67dd130ff2ea598ea5f20b40e36d19821b4df8c9c5037b",
-                "sha256:74d6c7e80609c0f4c2434b97b80c7f8fdfaa072ca4baab7e239a15d6d70ed73a",
-                "sha256:7be0eec337359c155df191d6ae00a5e8bbb63933883f4f5dffc439dac5348c3f",
-                "sha256:94ae132f0e40fe48f310bba63f477f14a43116f05ddb69d6fa31e93f05848ae2",
-                "sha256:bb5829d027ff82aa872d76158919045a7c1e91fbf241aec32cb07956e9ebd3c9",
-                "sha256:ca238ceb7ba0bdf6ce88c1b74a87bffcee5afbfa1e41e173b1ceb095b39add46",
-                "sha256:ca28641954f767f9822c24e927ad894d45d5a1e501767599647259cbf030b903",
-                "sha256:e0344c14c9cb89e76eb6a060e67980c9e35b3f36691e15e1b7a9e58a0a6c6dc3",
-                "sha256:ebc15b1c22e55c4d5566e3ca4db8689470a0ca2babef8e3a9ee057a8b82ce4b1",
-                "sha256:ec63da4e7e4a5f924b90af42eddf20b698a70e58d86a72d943857c4c6045b3ee"
+                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
+                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
+                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
+                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
+                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
+                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
+                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
+                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
+                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
+                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
+                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
+                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
+                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
+                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
+                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
+                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
+                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
+                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
+                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
+                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
+                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
+                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
+                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==36.0.1"
+            "version": "==39.0.2"
         },
         "dnspython": {
             "hashes": [
-                "sha256:258d7ea3c86c8cea20705e904764fef5e93837c07d1499a13154e9ba0a93b420",
-                "sha256:84656be4dc8379066be55c594622e82250874f9bccc9993f73cf9df72fc4cffc"
+                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
+                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+            ],
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
+            "version": "==2.3.0"
+        },
+        "h11": {
+            "hashes": [
+                "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d",
+                "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.14.0"
+        },
+        "httpcore": {
+            "hashes": [
+                "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb",
+                "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"
             ],
-            "markers": "python_version >= '3.6' and python_version < '4.0'",
-            "version": "==2.2.0rc1"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.16.3"
+        },
+        "httpx": {
+            "hashes": [
+                "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9",
+                "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"
+            ],
+            "index": "pypi",
+            "version": "==0.23.3"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.3"
+            "version": "==3.4"
         },
         "isort": {
             "hashes": [
-                "sha256:6f62d78e2f89b4500b080fe3a81690850cd254227f27f75c3a0c491a1f351ba7",
-                "sha256:e8443a5e7a020e9d7f97f1d7d9cd17c88bcb3bc7e218bf9cf5095fe550be2951"
+                "sha256:0ec8b74806e80fec33e6e7ba89d35e17b3eb1c4c74316ea44cf877cc26e8b118",
+                "sha256:cde11e804641edbe1b6b95d56582eb541f27eebc77864c6015545944bb0e9c76"
             ],
             "index": "pypi",
-            "version": "==5.10.1"
+            "version": "==6.0.0b2"
         },
         "jinja2": {
             "hashes": [
                 "sha256:1f06f2da51e7b56b8f238affdd6b4e2c61e39598a378cc49345bc1bd42a978a4",
                 "sha256:703f484b47a6af502e743c9122595cc812b0271f661722403114f71a79d0f5a4"
             ],
             "markers": "python_version >= '3.6'",
@@ -244,152 +458,150 @@
                 "sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40",
                 "sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa"
             ],
             "version": "==0.2.0"
         },
         "lxml": {
             "hashes": [
-                "sha256:0607ff0988ad7e173e5ddf7bf55ee65534bd18a5461183c33e8e41a59e89edf4",
-                "sha256:09b738360af8cb2da275998a8bf79517a71225b0de41ab47339c2beebfff025f",
-                "sha256:0a5f0e4747f31cff87d1eb32a6000bde1e603107f632ef4666be0dc065889c7a",
-                "sha256:0b5e96e25e70917b28a5391c2ed3ffc6156513d3db0e1476c5253fcd50f7a944",
-                "sha256:1104a8d47967a414a436007c52f533e933e5d52574cab407b1e49a4e9b5ddbd1",
-                "sha256:13dbb5c7e8f3b6a2cf6e10b0948cacb2f4c9eb05029fe31c60592d08ac63180d",
-                "sha256:2a906c3890da6a63224d551c2967413b8790a6357a80bf6b257c9a7978c2c42d",
-                "sha256:317bd63870b4d875af3c1be1b19202de34c32623609ec803b81c99193a788c1e",
-                "sha256:34c22eb8c819d59cec4444d9eebe2e38b95d3dcdafe08965853f8799fd71161d",
-                "sha256:36b16fecb10246e599f178dd74f313cbdc9f41c56e77d52100d1361eed24f51a",
-                "sha256:38d9759733aa04fb1697d717bfabbedb21398046bd07734be7cccc3d19ea8675",
-                "sha256:3e26ad9bc48d610bf6cc76c506b9e5ad9360ed7a945d9be3b5b2c8535a0145e3",
-                "sha256:41358bfd24425c1673f184d7c26c6ae91943fe51dfecc3603b5e08187b4bcc55",
-                "sha256:447d5009d6b5447b2f237395d0018901dcc673f7d9f82ba26c1b9f9c3b444b60",
-                "sha256:44f552e0da3c8ee3c28e2eb82b0b784200631687fc6a71277ea8ab0828780e7d",
-                "sha256:490712b91c65988012e866c411a40cc65b595929ececf75eeb4c79fcc3bc80a6",
-                "sha256:4c093c571bc3da9ebcd484e001ba18b8452903cd428c0bc926d9b0141bcb710e",
-                "sha256:50d3dba341f1e583265c1a808e897b4159208d814ab07530202b6036a4d86da5",
-                "sha256:534e946bce61fd162af02bad7bfd2daec1521b71d27238869c23a672146c34a5",
-                "sha256:585ea241ee4961dc18a95e2f5581dbc26285fcf330e007459688096f76be8c42",
-                "sha256:59e7da839a1238807226f7143c68a479dee09244d1b3cf8c134f2fce777d12d0",
-                "sha256:5b0f782f0e03555c55e37d93d7a57454efe7495dab33ba0ccd2dbe25fc50f05d",
-                "sha256:5bee1b0cbfdb87686a7fb0e46f1d8bd34d52d6932c0723a86de1cc532b1aa489",
-                "sha256:610807cea990fd545b1559466971649e69302c8a9472cefe1d6d48a1dee97440",
-                "sha256:6308062534323f0d3edb4e702a0e26a76ca9e0e23ff99be5d82750772df32a9e",
-                "sha256:67fa5f028e8a01e1d7944a9fb616d1d0510d5d38b0c41708310bd1bc45ae89f6",
-                "sha256:6a2ab9d089324d77bb81745b01f4aeffe4094306d939e92ba5e71e9a6b99b71e",
-                "sha256:6c198bfc169419c09b85ab10cb0f572744e686f40d1e7f4ed09061284fc1303f",
-                "sha256:6e56521538f19c4a6690f439fefed551f0b296bd785adc67c1777c348beb943d",
-                "sha256:6ec829058785d028f467be70cd195cd0aaf1a763e4d09822584ede8c9eaa4b03",
-                "sha256:718d7208b9c2d86aaf0294d9381a6acb0158b5ff0f3515902751404e318e02c9",
-                "sha256:735e3b4ce9c0616e85f302f109bdc6e425ba1670a73f962c9f6b98a6d51b77c9",
-                "sha256:772057fba283c095db8c8ecde4634717a35c47061d24f889468dc67190327bcd",
-                "sha256:7b5e2acefd33c259c4a2e157119c4373c8773cf6793e225006a1649672ab47a6",
-                "sha256:82d16a64236970cb93c8d63ad18c5b9f138a704331e4b916b2737ddfad14e0c4",
-                "sha256:87c1b0496e8c87ec9db5383e30042357b4839b46c2d556abd49ec770ce2ad868",
-                "sha256:8e54945dd2eeb50925500957c7c579df3cd07c29db7810b83cf30495d79af267",
-                "sha256:9393a05b126a7e187f3e38758255e0edf948a65b22c377414002d488221fdaa2",
-                "sha256:9fbc0dee7ff5f15c4428775e6fa3ed20003140560ffa22b88326669d53b3c0f4",
-                "sha256:a1613838aa6b89af4ba10a0f3a972836128801ed008078f8c1244e65958f1b24",
-                "sha256:a1bbc4efa99ed1310b5009ce7f3a1784698082ed2c1ef3895332f5df9b3b92c2",
-                "sha256:a555e06566c6dc167fbcd0ad507ff05fd9328502aefc963cb0a0547cfe7f00db",
-                "sha256:a58d78653ae422df6837dd4ca0036610b8cb4962b5cfdbd337b7b24de9e5f98a",
-                "sha256:a5edc58d631170de90e50adc2cc0248083541affef82f8cd93bea458e4d96db8",
-                "sha256:a5f623aeaa24f71fce3177d7fee875371345eb9102b355b882243e33e04b7175",
-                "sha256:adaab25be351fff0d8a691c4f09153647804d09a87a4e4ea2c3f9fe9e8651851",
-                "sha256:ade74f5e3a0fd17df5782896ddca7ddb998845a5f7cd4b0be771e1ffc3b9aa5b",
-                "sha256:b1d381f58fcc3e63fcc0ea4f0a38335163883267f77e4c6e22d7a30877218a0e",
-                "sha256:bf6005708fc2e2c89a083f258b97709559a95f9a7a03e59f805dd23c93bc3986",
-                "sha256:d546431636edb1d6a608b348dd58cc9841b81f4116745857b6cb9f8dadb2725f",
-                "sha256:d5618d49de6ba63fe4510bdada62d06a8acfca0b4b5c904956c777d28382b419",
-                "sha256:dfd0d464f3d86a1460683cd742306d1138b4e99b79094f4e07e1ca85ee267fe7",
-                "sha256:e18281a7d80d76b66a9f9e68a98cf7e1d153182772400d9a9ce855264d7d0ce7",
-                "sha256:e410cf3a2272d0a85526d700782a2fa92c1e304fdcc519ba74ac80b8297adf36",
-                "sha256:e662c6266e3a275bdcb6bb049edc7cd77d0b0f7e119a53101d367c841afc66dc",
-                "sha256:ec9027d0beb785a35aa9951d14e06d48cfbf876d8ff67519403a2522b181943b",
-                "sha256:eed394099a7792834f0cb4a8f615319152b9d801444c1c9e1b1a2c36d2239f9e",
-                "sha256:f76dbe44e31abf516114f6347a46fa4e7c2e8bceaa4b6f7ee3a0a03c8eba3c17",
-                "sha256:fc15874816b9320581133ddc2096b644582ab870cf6a6ed63684433e7af4b0d3",
-                "sha256:fc9fb11b65e7bc49f7f75aaba1b700f7181d95d4e151cf2f24d51bfd14410b77"
+                "sha256:01d36c05f4afb8f7c20fd9ed5badca32a2029b93b1750f571ccc0b142531caf7",
+                "sha256:04876580c050a8c5341d706dd464ff04fd597095cc8c023252566a8826505726",
+                "sha256:05ca3f6abf5cf78fe053da9b1166e062ade3fa5d4f92b4ed688127ea7d7b1d03",
+                "sha256:090c6543d3696cbe15b4ac6e175e576bcc3f1ccfbba970061b7300b0c15a2140",
+                "sha256:0dc313ef231edf866912e9d8f5a042ddab56c752619e92dfd3a2c277e6a7299a",
+                "sha256:0f2b1e0d79180f344ff9f321327b005ca043a50ece8713de61d1cb383fb8ac05",
+                "sha256:13598ecfbd2e86ea7ae45ec28a2a54fb87ee9b9fdb0f6d343297d8e548392c03",
+                "sha256:16efd54337136e8cd72fb9485c368d91d77a47ee2d42b057564aae201257d419",
+                "sha256:1ab8f1f932e8f82355e75dda5413a57612c6ea448069d4fb2e217e9a4bed13d4",
+                "sha256:223f4232855ade399bd409331e6ca70fb5578efef22cf4069a6090acc0f53c0e",
+                "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67",
+                "sha256:2899456259589aa38bfb018c364d6ae7b53c5c22d8e27d0ec7609c2a1ff78b50",
+                "sha256:2a29ba94d065945944016b6b74e538bdb1751a1db6ffb80c9d3c2e40d6fa9894",
+                "sha256:2a87fa548561d2f4643c99cd13131acb607ddabb70682dcf1dff5f71f781a4bf",
+                "sha256:2e430cd2824f05f2d4f687701144556646bae8f249fd60aa1e4c768ba7018947",
+                "sha256:36c3c175d34652a35475a73762b545f4527aec044910a651d2bf50de9c3352b1",
+                "sha256:3818b8e2c4b5148567e1b09ce739006acfaa44ce3156f8cbbc11062994b8e8dd",
+                "sha256:3ab9fa9d6dc2a7f29d7affdf3edebf6ece6fb28a6d80b14c3b2fb9d39b9322c3",
+                "sha256:3efea981d956a6f7173b4659849f55081867cf897e719f57383698af6f618a92",
+                "sha256:4c8f293f14abc8fd3e8e01c5bd86e6ed0b6ef71936ded5bf10fe7a5efefbaca3",
+                "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457",
+                "sha256:58bfa3aa19ca4c0f28c5dde0ff56c520fbac6f0daf4fac66ed4c8d2fb7f22e74",
+                "sha256:5b4545b8a40478183ac06c073e81a5ce4cf01bf1734962577cf2bb569a5b3bbf",
+                "sha256:5f50a1c177e2fa3ee0667a5ab79fdc6b23086bc8b589d90b93b4bd17eb0e64d1",
+                "sha256:63da2ccc0857c311d764e7d3d90f429c252e83b52d1f8f1d1fe55be26827d1f4",
+                "sha256:6749649eecd6a9871cae297bffa4ee76f90b4504a2a2ab528d9ebe912b101975",
+                "sha256:6804daeb7ef69e7b36f76caddb85cccd63d0c56dedb47555d2fc969e2af6a1a5",
+                "sha256:689bb688a1db722485e4610a503e3e9210dcc20c520b45ac8f7533c837be76fe",
+                "sha256:699a9af7dffaf67deeae27b2112aa06b41c370d5e7633e0ee0aea2e0b6c211f7",
+                "sha256:6b418afe5df18233fc6b6093deb82a32895b6bb0b1155c2cdb05203f583053f1",
+                "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2",
+                "sha256:7b515674acfdcadb0eb5d00d8a709868173acece5cb0be3dd165950cbfdf5409",
+                "sha256:7b770ed79542ed52c519119473898198761d78beb24b107acf3ad65deae61f1f",
+                "sha256:7d2278d59425777cfcb19735018d897ca8303abe67cc735f9f97177ceff8027f",
+                "sha256:7e91ee82f4199af8c43d8158024cbdff3d931df350252288f0d4ce656df7f3b5",
+                "sha256:821b7f59b99551c69c85a6039c65b75f5683bdc63270fec660f75da67469ca24",
+                "sha256:822068f85e12a6e292803e112ab876bc03ed1f03dddb80154c395f891ca6b31e",
+                "sha256:8340225bd5e7a701c0fa98284c849c9b9fc9238abf53a0ebd90900f25d39a4e4",
+                "sha256:85cabf64adec449132e55616e7ca3e1000ab449d1d0f9d7f83146ed5bdcb6d8a",
+                "sha256:880bbbcbe2fca64e2f4d8e04db47bcdf504936fa2b33933efd945e1b429bea8c",
+                "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de",
+                "sha256:8e20cb5a47247e383cf4ff523205060991021233ebd6f924bca927fcf25cf86f",
+                "sha256:925073b2fe14ab9b87e73f9a5fde6ce6392da430f3004d8b72cc86f746f5163b",
+                "sha256:998c7c41910666d2976928c38ea96a70d1aa43be6fe502f21a651e17483a43c5",
+                "sha256:9b22c5c66f67ae00c0199f6055705bc3eb3fcb08d03d2ec4059a2b1b25ed48d7",
+                "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a",
+                "sha256:a08cff61517ee26cb56f1e949cca38caabe9ea9fbb4b1e10a805dc39844b7d5c",
+                "sha256:a0a336d6d3e8b234a3aae3c674873d8f0e720b76bc1d9416866c41cd9500ffb9",
+                "sha256:a35f8b7fa99f90dd2f5dc5a9fa12332642f087a7641289ca6c40d6e1a2637d8e",
+                "sha256:a38486985ca49cfa574a507e7a2215c0c780fd1778bb6290c21193b7211702ab",
+                "sha256:a5da296eb617d18e497bcf0a5c528f5d3b18dadb3619fbdadf4ed2356ef8d941",
+                "sha256:a6e441a86553c310258aca15d1c05903aaf4965b23f3bc2d55f200804e005ee5",
+                "sha256:a82d05da00a58b8e4c0008edbc8a4b6ec5a4bc1e2ee0fb6ed157cf634ed7fa45",
+                "sha256:ab323679b8b3030000f2be63e22cdeea5b47ee0abd2d6a1dc0c8103ddaa56cd7",
+                "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892",
+                "sha256:b23e19989c355ca854276178a0463951a653309fb8e57ce674497f2d9f208746",
+                "sha256:b264171e3143d842ded311b7dccd46ff9ef34247129ff5bf5066123c55c2431c",
+                "sha256:b26a29f0b7fc6f0897f043ca366142d2b609dc60756ee6e4e90b5f762c6adc53",
+                "sha256:b64d891da92e232c36976c80ed7ebb383e3f148489796d8d31a5b6a677825efe",
+                "sha256:b9cc34af337a97d470040f99ba4282f6e6bac88407d021688a5d585e44a23184",
+                "sha256:bc718cd47b765e790eecb74d044cc8d37d58562f6c314ee9484df26276d36a38",
+                "sha256:be7292c55101e22f2a3d4d8913944cbea71eea90792bf914add27454a13905df",
+                "sha256:c83203addf554215463b59f6399835201999b5e48019dc17f182ed5ad87205c9",
+                "sha256:c9ec3eaf616d67db0764b3bb983962b4f385a1f08304fd30c7283954e6a7869b",
+                "sha256:ca34efc80a29351897e18888c71c6aca4a359247c87e0b1c7ada14f0ab0c0fb2",
+                "sha256:ca989b91cf3a3ba28930a9fc1e9aeafc2a395448641df1f387a2d394638943b0",
+                "sha256:d02a5399126a53492415d4906ab0ad0375a5456cc05c3fc0fc4ca11771745cda",
+                "sha256:d17bc7c2ccf49c478c5bdd447594e82692c74222698cfc9b5daae7ae7e90743b",
+                "sha256:d5bf6545cd27aaa8a13033ce56354ed9e25ab0e4ac3b5392b763d8d04b08e0c5",
+                "sha256:d6b430a9938a5a5d85fc107d852262ddcd48602c120e3dbb02137c83d212b380",
+                "sha256:da248f93f0418a9e9d94b0080d7ebc407a9a5e6d0b57bb30db9b5cc28de1ad33",
+                "sha256:da4dd7c9c50c059aba52b3524f84d7de956f7fef88f0bafcf4ad7dde94a064e8",
+                "sha256:df0623dcf9668ad0445e0558a21211d4e9a149ea8f5666917c8eeec515f0a6d1",
+                "sha256:e5168986b90a8d1f2f9dc1b841467c74221bd752537b99761a93d2d981e04889",
+                "sha256:efa29c2fe6b4fdd32e8ef81c1528506895eca86e1d8c4657fda04c9b3786ddf9",
+                "sha256:f1496ea22ca2c830cbcbd473de8f114a320da308438ae65abad6bab7867fe38f",
+                "sha256:f49e52d174375a7def9915c9f06ec4e569d235ad428f70751765f48d5926678c"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==4.7.1"
+            "version": "==4.9.2"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:01a9b8ea66f1658938f65b93a85ebe8bc016e6769611be228d797c9d998dd298",
-                "sha256:023cb26ec21ece8dc3907c0e8320058b2e0cb3c55cf9564da612bc325bed5e64",
-                "sha256:0446679737af14f45767963a1a9ef7620189912317d095f2d9ffa183a4d25d2b",
-                "sha256:04635854b943835a6ea959e948d19dcd311762c5c0c6e1f0e16ee57022669194",
-                "sha256:0717a7390a68be14b8c793ba258e075c6f4ca819f15edfc2a3a027c823718567",
-                "sha256:0955295dd5eec6cb6cc2fe1698f4c6d84af2e92de33fbcac4111913cd100a6ff",
-                "sha256:0d4b31cc67ab36e3392bbf3862cfbadac3db12bdd8b02a2731f509ed5b829724",
-                "sha256:10f82115e21dc0dfec9ab5c0223652f7197feb168c940f3ef61563fc2d6beb74",
-                "sha256:168cd0a3642de83558a5153c8bd34f175a9a6e7f6dc6384b9655d2697312a646",
-                "sha256:1d609f577dc6e1aa17d746f8bd3c31aa4d258f4070d61b2aa5c4166c1539de35",
-                "sha256:1f2ade76b9903f39aa442b4aadd2177decb66525062db244b35d71d0ee8599b6",
-                "sha256:20dca64a3ef2d6e4d5d615a3fd418ad3bde77a47ec8a23d984a12b5b4c74491a",
-                "sha256:2a7d351cbd8cfeb19ca00de495e224dea7e7d919659c2841bbb7f420ad03e2d6",
-                "sha256:2d7d807855b419fc2ed3e631034685db6079889a1f01d5d9dac950f764da3dad",
-                "sha256:2ef54abee730b502252bcdf31b10dacb0a416229b72c18b19e24a4509f273d26",
-                "sha256:36bc903cbb393720fad60fc28c10de6acf10dc6cc883f3e24ee4012371399a38",
-                "sha256:37205cac2a79194e3750b0af2a5720d95f786a55ce7df90c3af697bfa100eaac",
-                "sha256:3c112550557578c26af18a1ccc9e090bfe03832ae994343cfdacd287db6a6ae7",
-                "sha256:3dd007d54ee88b46be476e293f48c85048603f5f516008bee124ddd891398ed6",
-                "sha256:4296f2b1ce8c86a6aea78613c34bb1a672ea0e3de9c6ba08a960efe0b0a09047",
-                "sha256:47ab1e7b91c098ab893b828deafa1203de86d0bc6ab587b160f78fe6c4011f75",
-                "sha256:49e3ceeabbfb9d66c3aef5af3a60cc43b85c33df25ce03d0031a608b0a8b2e3f",
-                "sha256:4dc8f9fb58f7364b63fd9f85013b780ef83c11857ae79f2feda41e270468dd9b",
-                "sha256:4efca8f86c54b22348a5467704e3fec767b2db12fc39c6d963168ab1d3fc9135",
-                "sha256:53edb4da6925ad13c07b6d26c2a852bd81e364f95301c66e930ab2aef5b5ddd8",
-                "sha256:5855f8438a7d1d458206a2466bf82b0f104a3724bf96a1c781ab731e4201731a",
-                "sha256:594c67807fb16238b30c44bdf74f36c02cdf22d1c8cda91ef8a0ed8dabf5620a",
-                "sha256:5b6d930f030f8ed98e3e6c98ffa0652bdb82601e7a016ec2ab5d7ff23baa78d1",
-                "sha256:5bb28c636d87e840583ee3adeb78172efc47c8b26127267f54a9c0ec251d41a9",
-                "sha256:60bf42e36abfaf9aff1f50f52644b336d4f0a3fd6d8a60ca0d054ac9f713a864",
-                "sha256:611d1ad9a4288cf3e3c16014564df047fe08410e628f89805e475368bd304914",
-                "sha256:6300b8454aa6930a24b9618fbb54b5a68135092bc666f7b06901f897fa5c2fee",
-                "sha256:63f3268ba69ace99cab4e3e3b5840b03340efed0948ab8f78d2fd87ee5442a4f",
-                "sha256:6557b31b5e2c9ddf0de32a691f2312a32f77cd7681d8af66c2692efdbef84c18",
-                "sha256:693ce3f9e70a6cf7d2fb9e6c9d8b204b6b39897a2c4a1aa65728d5ac97dcc1d8",
-                "sha256:6a7fae0dd14cf60ad5ff42baa2e95727c3d81ded453457771d02b7d2b3f9c0c2",
-                "sha256:6c4ca60fa24e85fe25b912b01e62cb969d69a23a5d5867682dd3e80b5b02581d",
-                "sha256:6fcf051089389abe060c9cd7caa212c707e58153afa2c649f00346ce6d260f1b",
-                "sha256:7d91275b0245b1da4d4cfa07e0faedd5b0812efc15b702576d103293e252af1b",
-                "sha256:89c687013cb1cd489a0f0ac24febe8c7a666e6e221b783e53ac50ebf68e45d86",
-                "sha256:8d206346619592c6200148b01a2142798c989edcb9c896f9ac9722a99d4e77e6",
-                "sha256:905fec760bd2fa1388bb5b489ee8ee5f7291d692638ea5f67982d968366bef9f",
-                "sha256:97383d78eb34da7e1fa37dd273c20ad4320929af65d156e35a5e2d89566d9dfb",
-                "sha256:984d76483eb32f1bcb536dc27e4ad56bba4baa70be32fa87152832cdd9db0833",
-                "sha256:99df47edb6bda1249d3e80fdabb1dab8c08ef3975f69aed437cb69d0a5de1e28",
-                "sha256:9f02365d4e99430a12647f09b6cc8bab61a6564363f313126f775eb4f6ef798e",
-                "sha256:a30e67a65b53ea0a5e62fe23682cfe22712e01f453b95233b25502f7c61cb415",
-                "sha256:ab3ef638ace319fa26553db0624c4699e31a28bb2a835c5faca8f8acf6a5a902",
-                "sha256:aca6377c0cb8a8253e493c6b451565ac77e98c2951c45f913e0b52facdcff83f",
-                "sha256:add36cb2dbb8b736611303cd3bfcee00afd96471b09cda130da3581cbdc56a6d",
-                "sha256:b2f4bf27480f5e5e8ce285a8c8fd176c0b03e93dcc6646477d4630e83440c6a9",
-                "sha256:b7f2d075102dc8c794cbde1947378051c4e5180d52d276987b8d28a3bd58c17d",
-                "sha256:baa1a4e8f868845af802979fcdbf0bb11f94f1cb7ced4c4b8a351bb60d108145",
-                "sha256:be98f628055368795d818ebf93da628541e10b75b41c559fdf36d104c5787066",
-                "sha256:bf5d821ffabf0ef3533c39c518f3357b171a1651c1ff6827325e4489b0e46c3c",
-                "sha256:c47adbc92fc1bb2b3274c4b3a43ae0e4573d9fbff4f54cd484555edbf030baf1",
-                "sha256:cdfba22ea2f0029c9261a4bd07e830a8da012291fbe44dc794e488b6c9bb353a",
-                "sha256:d6c7ebd4e944c85e2c3421e612a7057a2f48d478d79e61800d81468a8d842207",
-                "sha256:d7f9850398e85aba693bb640262d3611788b1f29a79f0c93c565694658f4071f",
-                "sha256:d8446c54dc28c01e5a2dbac5a25f071f6653e6e40f3a8818e8b45d790fe6ef53",
-                "sha256:deb993cacb280823246a026e3b2d81c493c53de6acfd5e6bfe31ab3402bb37dd",
-                "sha256:e0f138900af21926a02425cf736db95be9f4af72ba1bb21453432a07f6082134",
-                "sha256:e9936f0b261d4df76ad22f8fee3ae83b60d7c3e871292cd42f40b81b70afae85",
-                "sha256:f0567c4dc99f264f49fe27da5f735f414c4e7e7dd850cfd8e69f0862d7c74ea9",
-                "sha256:f5653a225f31e113b152e56f154ccbe59eeb1c7487b39b9d9f9cdb58e6c79dc5",
-                "sha256:f826e31d18b516f653fe296d967d700fddad5901ae07c622bb3705955e1faa94",
-                "sha256:f8ba0e8349a38d3001fae7eadded3f6606f0da5d748ee53cc1dab1d6527b9509",
-                "sha256:f9081981fe268bd86831e5c75f7de206ef275defcb82bc70740ae6dc507aee51",
-                "sha256:fa130dd50c57d53368c9d59395cb5526eda596d3ffe36666cd81a44d56e48872"
+                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
+                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
+                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
+                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
+                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
+                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
+                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
+                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
+                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
+                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
+                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
+                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
+                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
+                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
+                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
+                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
+                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
+                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
+                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
+                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
+                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
+                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
+                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
+                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
+                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
+                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
+                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
+                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
+                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
+                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
+                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
+                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
+                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
+                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
+                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
+                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
+                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
+                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
+                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
+                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
+                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
+                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
+                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
+                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
+                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
+                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
+                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
+                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
+                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
+                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.1.2"
         },
         "multidict": {
             "hashes": [
                 "sha256:024b8129695a952ebd93373e45b5d341dbb87c17ce49637b34000093f243dd4f",
                 "sha256:041e9442b11409be5e4fc8b6a97e4bcead758ab1e11768d1e69160bdde18acc3",
                 "sha256:045b4dd0e5f6121e6f314d81759abd2c257db4634260abcfe0d3f7083c4908ef",
                 "sha256:047c0a04e382ef8bd74b0de01407e8d8632d7d1b4db6f2561106af812a68741b",
@@ -418,41 +630,142 @@
                 "sha256:d1071414dd06ca2eafa90c85a079169bfeb0e5f57fd0b45d44c092546fcd6fd9",
                 "sha256:d3be11ac43ab1a3e979dac80843b42226d5d3cccd3986f2e03152720a4297cd7",
                 "sha256:db603a1c235d110c860d5f39988ebc8218ee028f07a7cbc056ba6424372ca31b"
             ],
             "markers": "python_full_version >= '3.4.1'",
             "version": "==4.5.2"
         },
+        "mypy-extensions": {
+            "hashes": [
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
+        },
+        "nodeenv": {
+            "hashes": [
+                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
+                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.7.0"
+        },
         "numpy": {
             "hashes": [
-                "sha256:07805b77c2b4582bc6888795c0463bf3d4bd758dee922fcd685413eb3274295f",
-                "sha256:0b5642efe2a36f2191102b44bb95ee1479f14c1adb2d7155303e50b2517e43bc",
-                "sha256:11fb5ee7b8a2a01bccdfb715889cb1a8490bfceeba1ab1ca9d01c92329ca5a4b",
-                "sha256:20016b0ed895bb80f37caadd224b01b6cc52520766ba67d8f5536ac16ef08002",
-                "sha256:222ce51bf9d4c77f2222049d75ea908f1862302cab7d5ccdb88773b9514e10af",
-                "sha256:2313aa9b9684b36b0bf07e44432d025e0803518286a1ecae5f0ea947b46008df",
-                "sha256:26271b883db7ff9e375df36ad92fc9921fc336480d0aabe4483503640c9b5dd3",
-                "sha256:301df2531616ff7dac8224c104b38d301adabb96c12650dae06d2036da53c385",
-                "sha256:3d0b6fb9796ba83500990dc18d8dbeaca49559c7f7f47da723fee902a99ee4bb",
-                "sha256:4315a66e64fe1adc7f7fa51116c87cdf5a78f2f8265c6d0ee27bfcbe845b3ddf",
-                "sha256:5b46584808f06d90df177520136cfeb5f2151b0e6a762e94c05a36f82140ff7b",
-                "sha256:6eaa053519d1ed5922621ecb04d33d64769508060860eb0b8a07502d55554a2c",
-                "sha256:6ebe0f0f40aa86c5cbe41e017e2028ba318e0743d93674a19f06a2401e602bd7",
-                "sha256:a0964771a7660fd3d2420d6be0a08144f49f14d684bbe85f67467ad81bd73180",
-                "sha256:af16e2163c1edfaa82ec43a220acc31ad0ff51619efcb41d79440dfc130e9562",
-                "sha256:af718720cb23c795a1470fde1a860c7fbbcd1387e1f3755cf734417f96124766",
-                "sha256:b445551ff10fe31adb76df0e6d0210e02c586686297faddcf453dd51ce2b2ea0",
-                "sha256:b63c2976f10a94af28c2860a74d7cf07ed9489ebfd36fbadb9816d3bf6ba8efb",
-                "sha256:c3a8d12b5bf04ce3495ad2b4d706a3058415185c16d3e8d094264a9de62d52e2",
-                "sha256:ced56665c49691ad8a31d553e42248566678f188e7c1813cadc947bfb91f3abd",
-                "sha256:e55a7a201e1972e2686ffee1dba1ddf5e041989018a707540ba10be8367331b1",
-                "sha256:f13703ad4849ef62d3dadc1af1e00ce2762458b4466d4f3e339d84e6b450af33"
+                "sha256:003a9f530e880cb2cd177cba1af7220b9aa42def9c4afc2a2fc3ee6be7eb2b22",
+                "sha256:150947adbdfeceec4e5926d956a06865c1c690f2fd902efede4ca6fe2e657c3f",
+                "sha256:2620e8592136e073bd12ee4536149380695fbe9ebeae845b81237f986479ffc9",
+                "sha256:2eabd64ddb96a1239791da78fa5f4e1693ae2dadc82a76bc76a14cbb2b966e96",
+                "sha256:4173bde9fa2a005c2c6e2ea8ac1618e2ed2c1c6ec8a7657237854d42094123a0",
+                "sha256:4199e7cfc307a778f72d293372736223e39ec9ac096ff0a2e64853b866a8e18a",
+                "sha256:4cecaed30dc14123020f77b03601559fff3e6cd0c048f8b5289f4eeabb0eb281",
+                "sha256:557d42778a6869c2162deb40ad82612645e21d79e11c1dc62c6e82a2220ffb04",
+                "sha256:63e45511ee4d9d976637d11e6c9864eae50e12dc9598f531c035265991910468",
+                "sha256:6524630f71631be2dabe0c541e7675db82651eb998496bbe16bc4f77f0772253",
+                "sha256:76807b4063f0002c8532cfeac47a3068a69561e9c8715efdad3c642eb27c0756",
+                "sha256:7de8fdde0003f4294655aa5d5f0a89c26b9f22c0a58790c38fae1ed392d44a5a",
+                "sha256:889b2cc88b837d86eda1b17008ebeb679d82875022200c6e8e4ce6cf549b7acb",
+                "sha256:92011118955724465fb6853def593cf397b4a1367495e0b59a7e69d40c4eb71d",
+                "sha256:97cf27e51fa078078c649a51d7ade3c92d9e709ba2bfb97493007103c741f1d0",
+                "sha256:9a23f8440561a633204a67fb44617ce2a299beecf3295f0d13c495518908e910",
+                "sha256:a51725a815a6188c662fb66fb32077709a9ca38053f0274640293a14fdd22978",
+                "sha256:a77d3e1163a7770164404607b7ba3967fb49b24782a6ef85d9b5f54126cc39e5",
+                "sha256:adbdce121896fd3a17a77ab0b0b5eedf05a9834a18699db6829a64e1dfccca7f",
+                "sha256:c29e6bd0ec49a44d7690ecb623a8eac5ab8a923bce0bea6293953992edf3a76a",
+                "sha256:c72a6b2f4af1adfe193f7beb91ddf708ff867a3f977ef2ec53c0ffb8283ab9f5",
+                "sha256:d0a2db9d20117bf523dde15858398e7c0858aadca7c0f088ac0d6edd360e9ad2",
+                "sha256:e3ab5d32784e843fc0dd3ab6dcafc67ef806e6b6828dc6af2f689be0eb4d781d",
+                "sha256:e428c4fbfa085f947b536706a2fc349245d7baa8334f0c5723c56a10595f9b95",
+                "sha256:e8d2859428712785e8a8b7d2b3ef0a1d1565892367b32f915c4a4df44d0e64f5",
+                "sha256:eef70b4fc1e872ebddc38cddacc87c19a3709c0e3e5d20bf3954c147b1dd941d",
+                "sha256:f64bb98ac59b3ea3bf74b02f13836eb2e24e48e0ab0145bbda646295769bd780",
+                "sha256:f9006288bcf4895917d02583cf3411f98631275bc67cce355a7f39f8c14338fa"
             ],
             "index": "pypi",
-            "version": "==1.22.0rc3"
+            "version": "==1.24.2"
+        },
+        "orjson": {
+            "hashes": [
+                "sha256:0204bc414bc6f7a595211569840b422d96649fd8686efa1fbbcb12eed5dd9521",
+                "sha256:022347dad2253081eaa25366834bb8b06a5aceb0e83b39c6b0aa865759e49d69",
+                "sha256:02f5b5db1e424706eb9f70f1c25699ff4cef16fadfc64af5b70f8628eafe4771",
+                "sha256:0dc4a52f1087baeec6b58248fd6b01f17c124fb99f6f770596851ea434a7be0b",
+                "sha256:18fcdea75d8b571dc9b185652b81397b62878ae7934fd62e6a0103a5b8448e34",
+                "sha256:1af1cfad5d90b68e15fd625c889c4f9f91d7a88f49512cdb89f01c3881e0c9d9",
+                "sha256:1b2abf93b727a6af7c5ec8816168cbdff39c716af18ced425dd50ae46d69765c",
+                "sha256:2006d9c046bbf335c951f61e016a27bd4f17323dd116f601e4a8a11739cd0a62",
+                "sha256:23447d38375a19d57975d4e32d9ce9f533803c197fd4292e10d3234c052037a8",
+                "sha256:24ad122d8dd057acf2a9965a2ffc1bc12fb310ae1cfe2912db930cbb9ef7eaba",
+                "sha256:28075c4b502d792fb6703e983d456b2a30d5d6f332d26092eb312dc782e64c64",
+                "sha256:28dfe774c345130f1117c4d023644ec52d9d50e3eaadb9bd1c668d91dc109bb5",
+                "sha256:2c2c5f3d3bbd61dba646e2b9c54a0dd7941b03fba49726bd31c1c23fedf0b9aa",
+                "sha256:306618884929b596e2e083f82b5617da812df25b0c467542371f1d51f0c5a6f5",
+                "sha256:317164f7d4c0540a6eb8b0a0faeec84ef011d359da05188423db762b65f84e1d",
+                "sha256:343124f84da0a33c83ee106a98b3e3c42767c88323d4a2809683cbe83816e8be",
+                "sha256:449d8ed1e0e6b24e9df5a06b59fd66ea7f7293e141257069601ae8ff9fad705c",
+                "sha256:4553d85bad4cbd634a40b7b5d36daaa197a6025f9ce3e2165b371e528759093d",
+                "sha256:4c2e19d2b46cc93c7218bf8180807bf922ff61dc9883458a06edc66d22970fff",
+                "sha256:4d7c9f3b1598a1ccd806ef02257a76a00c7ede09662ddb54eec2b4bd92874254",
+                "sha256:52293a6097750c2d434737966fe6e2a1ed489ac70cc8e584f5944af83de0b787",
+                "sha256:56bb6eb7a254eec3b15feba9b20f4172ccbe6ea50a54cf66cbc8e1e4a19585c2",
+                "sha256:57ee45d2cc6c11c50afb5a0c09d7cd559aea76c77250dbe996be6a03464d4a50",
+                "sha256:5e7e39357371d4ae5649f33c01886508a4c8e5fa5c7344554af041dc0f004c01",
+                "sha256:60fefd4bbd796b4296f478e705fe2c2c7defd28da98d3017743eb87c3238a380",
+                "sha256:66045850f286090800a18662d81d44f88c3fcb60ea3a9947d5caeab5d1efc92e",
+                "sha256:68d59e3ae84a9b6f14b45a89f7fde4a08a87ea5eb76bfc854b354640de8156f5",
+                "sha256:747bd4e09d8aa61e1ff677a7dd1cffd28a5d13c22f3769123c58ec988bf1b83d",
+                "sha256:81d3c5b253eebfc4a61cea1f255a576cb2b889afa99f4510f30ec13201d4f457",
+                "sha256:88bf40e5468444c04374d1b8f1877cebbaef6bb7406cb6b4a34a570c5cbb87bc",
+                "sha256:8e0bff5656b99dd975cae2e5230b39e5909d06c0692fd1f6f06dc46f1fe705d0",
+                "sha256:8f84116fcc3714e7ba3cbeb1b11ac5e4549e7d2726c50142f8299fff9dea7d53",
+                "sha256:9322450f392dceb49810d2f820b1932af22d66f67f1d45c31f160067dd06359f",
+                "sha256:9c98dc791aa44268ba7f6e21124cf885c813b155316c6bf257560571d243fe15",
+                "sha256:9cb36d4a14f3a911369219d5abc19b907bc41ed2730f7bfe0847b0fd3e834c87",
+                "sha256:9eda4c37e48ff549763183a1549c10eec6ea40439520b17d09359cd74a425069",
+                "sha256:a3eac485a15493164867729f44e1e1247b3094ff19d37708e8cdc9c88a93c623",
+                "sha256:a6bcb449537a99f55c5f05187bac00b4549a795e89c10dcca0d7629548852357",
+                "sha256:b90d171932b6a9d50e79fa2762cb303e3556bbf25c08bb316fe346ec58af9c19",
+                "sha256:c096d7a523bae6ffb9c4a228ba4691d66113f0f2231579dc945523fbef09c6da",
+                "sha256:c2f28a92a9bcb4e8635524b20db1b539bda8613872f306b36cdfd9d3577d03ac",
+                "sha256:d5514dfe200356a1d5a6039e00dca78d87d063f3da1eb6a371253e5a8b7ab5b0",
+                "sha256:dd7d86c5f5f820ac9d4783477e86eb984b63bdb32359935609eb33cf65049c54",
+                "sha256:ddfcc54793e266056fe1c257d0804c336bca1c5c1ee7979d674e1fc19cfb0a6a",
+                "sha256:e480d74d7bf415e6548a364669404119a85dbe0e3c6cd5f7cb4c7003eac20164",
+                "sha256:e6a6d55e01bce74516dff15302627a13b1f4edcb1c3942dd660978dee423ccf2",
+                "sha256:e991a5c2c5f2f299c77e1d07ef2812ff5b68e1d97a2aab01aca29cf756473aa3",
+                "sha256:edc65ddb6ae6f8fbb2bbf78ac98f75b729c9eeb0776d5508dd76d3a948dda1dd",
+                "sha256:f989f8580db86166aaaa938ccd1597ba1817e3f5df14c047baafe783e3d24173"
+            ],
+            "index": "pypi",
+            "version": "==3.8.8"
+        },
+        "packaging": {
+            "hashes": [
+                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
+                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.0"
+        },
+        "pathspec": {
+            "hashes": [
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
+        },
+        "platformdirs": {
+            "hashes": [
+                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
+                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.1"
         },
         "pyasn1": {
             "hashes": [
                 "sha256:1321d4b2f051410fe7302bb1619903d30b24ba1451d019c11d242d11b2a35444",
                 "sha256:2860a047f666afd23b197a65f33145313511c368ce919b2d9b1853ffd3e9d32d",
                 "sha256:2919babd43b3b44247c23201b71072c0c65a636daa595cad5bcd276094dbfc2d",
                 "sha256:437a23121602c0bb6c65320b27e31e334ffd73a9ca5c6c075b66b6270b1a8184",
@@ -491,43 +804,62 @@
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pyopenssl": {
             "hashes": [
-                "sha256:5e2d8c5e46d0d865ae933bef5230090bdaf5506281e9eec60fa250ee80600cb3",
-                "sha256:8935bd4920ab9abfebb07c41a4f58296407ed77f04bd1a92914044b848ba1ed6"
+                "sha256:c1cc5f86bcacefc84dada7d31175cae1b1518d5f60d3d0bb595a67822a868a6f",
+                "sha256:df5fc28af899e74e19fccb5510df423581047e10ab6f1f4ba1763ff5fde844c0"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==21.0.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==23.0.0"
+        },
+        "pyright": {
+            "hashes": [
+                "sha256:b3a9a6affa1252c52793e8663ade59ff966f8495ecfad6328deffe59cfc5a9a9",
+                "sha256:f34dfd0c2fcade34f9878b1fc69cb9456476dc78227e0a2fa046107ec55c0235"
+            ],
+            "index": "pypi",
+            "version": "==1.1.299"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
-        "pytz": {
-            "hashes": [
-                "sha256:3672058bc3453457b622aab7a1c3bfd5ab0bdae451512f6cf25f64ed37f5b87c",
-                "sha256:acad2d8b20a1af07d4e4c9d2e9285c5ed9104354062f275f3fcd88dcef4f1326"
-            ],
-            "version": "==2021.3"
-        },
         "pytz-deprecation-shim": {
             "hashes": [
                 "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6",
                 "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==0.1.0.post0"
         },
+        "rfc3986": {
+            "extras": [
+                "idna2008"
+            ],
+            "hashes": [
+                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
+                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
+            ],
+            "version": "==1.5.0"
+        },
+        "setuptools": {
+            "hashes": [
+                "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077",
+                "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==67.6.0"
+        },
         "singletonify": {
             "hashes": [
                 "sha256:51e8d6c895d8de72d126e0b523f3c34817442201245da517c91c4a29d82ad133",
                 "sha256:e04ba8278b3dee3d46877482cef9682f7d5df9bd305722f6828a49bbeb9a4def"
             ],
             "version": "==0.2.3"
         },
@@ -535,14 +867,22 @@
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
+        "sniffio": {
+            "hashes": [
+                "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
+                "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.3.0"
+        },
         "sortedcollections": {
             "hashes": [
                 "sha256:b07abbc73472cc459da9dd6e2607d73d1f3b9309a32dd9a57fa2c6fa882f4c6c",
                 "sha256:d8e9609d6c580a16a1224a3dc8965789e03ebc4c3e5ffd05ada54a2fed5dcacd"
             ],
             "version": "==2.1.0"
         },
@@ -551,119 +891,129 @@
                 "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88",
                 "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"
             ],
             "version": "==2.4.0"
         },
         "spade": {
             "git": "https://github.com/agent-based-information-flow-simulation/spade",
-            "ref": "6a857c2ae0a86b3bdfd20ccfcd28a11e1c6db81e"
+            "ref": "5bbe00b6cedec043886fe7b18a1db3bcd7359c4d"
         },
         "timeago": {
             "hashes": [
                 "sha256:f2acf144a9aabbc1e46a7f84387e6dd17bf41ff5fd87822c878621d06ef6b77c"
             ],
             "version": "==1.0.8"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "typing-extensions": {
             "hashes": [
-                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
-                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
+                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
+                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==4.5.0"
         },
         "tzdata": {
             "hashes": [
-                "sha256:3eee491e22ebfe1e5cfcc97a4137cd70f092ce59144d81f8924a844de05ba8f5",
-                "sha256:68dbe41afd01b867894bbdfd54fa03f468cfa4f0086bfb4adcd8de8f24f3ee21"
+                "sha256:2b88858b0e3120792a3c0635c23daf36a7d7eeeca657c323da299d2094402a0d",
+                "sha256:fe5f866eddd8b96e9fcba978f8e503c909b19ea7efda11e52e39494bad3a7bfa"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2021.5"
+            "version": "==2022.7"
         },
         "tzlocal": {
             "hashes": [
-                "sha256:0f28015ac68a5c067210400a9197fc5d36ba9bc3f8eaf1da3cbd59acdfed9e09",
-                "sha256:28ba8d9fcb6c9a782d6e0078b4f6627af1ea26aeaa32b4eab5324abc7df4149f"
+                "sha256:6f8d7ad7fd00cf8ef761672a8f1cb5cbe3bbc6252ce776052f5b5bab66a5f103",
+                "sha256:aff0a68c345e981c424b501ceb25a3630ac3288ff8b72cf1eca09861f4b28593"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==4.4b1"
         },
         "yarl": {
             "hashes": [
-                "sha256:044daf3012e43d4b3538562da94a88fb12a6490652dbc29fb19adfa02cf72eac",
-                "sha256:0cba38120db72123db7c58322fa69e3c0efa933040ffb586c3a87c063ec7cae8",
-                "sha256:167ab7f64e409e9bdd99333fe8c67b5574a1f0495dcfd905bc7454e766729b9e",
-                "sha256:1be4bbb3d27a4e9aa5f3df2ab61e3701ce8fcbd3e9846dbce7c033a7e8136746",
-                "sha256:1ca56f002eaf7998b5fcf73b2421790da9d2586331805f38acd9997743114e98",
-                "sha256:1d3d5ad8ea96bd6d643d80c7b8d5977b4e2fb1bab6c9da7322616fd26203d125",
-                "sha256:1eb6480ef366d75b54c68164094a6a560c247370a68c02dddb11f20c4c6d3c9d",
-                "sha256:1edc172dcca3f11b38a9d5c7505c83c1913c0addc99cd28e993efeaafdfaa18d",
-                "sha256:211fcd65c58bf250fb994b53bc45a442ddc9f441f6fec53e65de8cba48ded986",
-                "sha256:29e0656d5497733dcddc21797da5a2ab990c0cb9719f1f969e58a4abac66234d",
-                "sha256:368bcf400247318382cc150aaa632582d0780b28ee6053cd80268c7e72796dec",
-                "sha256:39d5493c5ecd75c8093fa7700a2fb5c94fe28c839c8e40144b7ab7ccba6938c8",
-                "sha256:3abddf0b8e41445426d29f955b24aeecc83fa1072be1be4e0d194134a7d9baee",
-                "sha256:3bf8cfe8856708ede6a73907bf0501f2dc4e104085e070a41f5d88e7faf237f3",
-                "sha256:3ec1d9a0d7780416e657f1e405ba35ec1ba453a4f1511eb8b9fbab81cb8b3ce1",
-                "sha256:45399b46d60c253327a460e99856752009fcee5f5d3c80b2f7c0cae1c38d56dd",
-                "sha256:52690eb521d690ab041c3919666bea13ab9fbff80d615ec16fa81a297131276b",
-                "sha256:534b047277a9a19d858cde163aba93f3e1677d5acd92f7d10ace419d478540de",
-                "sha256:580c1f15500e137a8c37053e4cbf6058944d4c114701fa59944607505c2fe3a0",
-                "sha256:59218fef177296451b23214c91ea3aba7858b4ae3306dde120224cfe0f7a6ee8",
-                "sha256:5ba63585a89c9885f18331a55d25fe81dc2d82b71311ff8bd378fc8004202ff6",
-                "sha256:5bb7d54b8f61ba6eee541fba4b83d22b8a046b4ef4d8eb7f15a7e35db2e1e245",
-                "sha256:6152224d0a1eb254f97df3997d79dadd8bb2c1a02ef283dbb34b97d4f8492d23",
-                "sha256:67e94028817defe5e705079b10a8438b8cb56e7115fa01640e9c0bb3edf67332",
-                "sha256:695ba021a9e04418507fa930d5f0704edbce47076bdcfeeaba1c83683e5649d1",
-                "sha256:6a1a9fe17621af43e9b9fcea8bd088ba682c8192d744b386ee3c47b56eaabb2c",
-                "sha256:6ab0c3274d0a846840bf6c27d2c60ba771a12e4d7586bf550eefc2df0b56b3b4",
-                "sha256:6feca8b6bfb9eef6ee057628e71e1734caf520a907b6ec0d62839e8293e945c0",
-                "sha256:737e401cd0c493f7e3dd4db72aca11cfe069531c9761b8ea474926936b3c57c8",
-                "sha256:788713c2896f426a4e166b11f4ec538b5736294ebf7d5f654ae445fd44270832",
-                "sha256:797c2c412b04403d2da075fb93c123df35239cd7b4cc4e0cd9e5839b73f52c58",
-                "sha256:8300401dc88cad23f5b4e4c1226f44a5aa696436a4026e456fe0e5d2f7f486e6",
-                "sha256:87f6e082bce21464857ba58b569370e7b547d239ca22248be68ea5d6b51464a1",
-                "sha256:89ccbf58e6a0ab89d487c92a490cb5660d06c3a47ca08872859672f9c511fc52",
-                "sha256:8b0915ee85150963a9504c10de4e4729ae700af11df0dc5550e6587ed7891e92",
-                "sha256:8cce6f9fa3df25f55521fbb5c7e4a736683148bcc0c75b21863789e5185f9185",
-                "sha256:95a1873b6c0dd1c437fb3bb4a4aaa699a48c218ac7ca1e74b0bee0ab16c7d60d",
-                "sha256:9b4c77d92d56a4c5027572752aa35082e40c561eec776048330d2907aead891d",
-                "sha256:9bfcd43c65fbb339dc7086b5315750efa42a34eefad0256ba114cd8ad3896f4b",
-                "sha256:9c1f083e7e71b2dd01f7cd7434a5f88c15213194df38bc29b388ccdf1492b739",
-                "sha256:a1d0894f238763717bdcfea74558c94e3bc34aeacd3351d769460c1a586a8b05",
-                "sha256:a467a431a0817a292121c13cbe637348b546e6ef47ca14a790aa2fa8cc93df63",
-                "sha256:aa32aaa97d8b2ed4e54dc65d241a0da1c627454950f7d7b1f95b13985afd6c5d",
-                "sha256:ac10bbac36cd89eac19f4e51c032ba6b412b3892b685076f4acd2de18ca990aa",
-                "sha256:ac35ccde589ab6a1870a484ed136d49a26bcd06b6a1c6397b1967ca13ceb3913",
-                "sha256:bab827163113177aee910adb1f48ff7af31ee0289f434f7e22d10baf624a6dfe",
-                "sha256:baf81561f2972fb895e7844882898bda1eef4b07b5b385bcd308d2098f1a767b",
-                "sha256:bf19725fec28452474d9887a128e98dd67eee7b7d52e932e6949c532d820dc3b",
-                "sha256:c01a89a44bb672c38f42b49cdb0ad667b116d731b3f4c896f72302ff77d71656",
-                "sha256:c0910c6b6c31359d2f6184828888c983d54d09d581a4a23547a35f1d0b9484b1",
-                "sha256:c10ea1e80a697cf7d80d1ed414b5cb8f1eec07d618f54637067ae3c0334133c4",
-                "sha256:c1164a2eac148d85bbdd23e07dfcc930f2e633220f3eb3c3e2a25f6148c2819e",
-                "sha256:c145ab54702334c42237a6c6c4cc08703b6aa9b94e2f227ceb3d477d20c36c63",
-                "sha256:c17965ff3706beedafd458c452bf15bac693ecd146a60a06a214614dc097a271",
-                "sha256:c19324a1c5399b602f3b6e7db9478e5b1adf5cf58901996fc973fe4fccd73eed",
-                "sha256:c2a1ac41a6aa980db03d098a5531f13985edcb451bcd9d00670b03129922cd0d",
-                "sha256:c6ddcd80d79c96eb19c354d9dca95291589c5954099836b7c8d29278a7ec0bda",
-                "sha256:c9c6d927e098c2d360695f2e9d38870b2e92e0919be07dbe339aefa32a090265",
-                "sha256:cc8b7a7254c0fc3187d43d6cb54b5032d2365efd1df0cd1749c0c4df5f0ad45f",
-                "sha256:cff3ba513db55cc6a35076f32c4cdc27032bd075c9faef31fec749e64b45d26c",
-                "sha256:d260d4dc495c05d6600264a197d9d6f7fc9347f21d2594926202fd08cf89a8ba",
-                "sha256:d6f3d62e16c10e88d2168ba2d065aa374e3c538998ed04996cd373ff2036d64c",
-                "sha256:da6df107b9ccfe52d3a48165e48d72db0eca3e3029b5b8cb4fe6ee3cb870ba8b",
-                "sha256:dfe4b95b7e00c6635a72e2d00b478e8a28bfb122dc76349a06e20792eb53a523",
-                "sha256:e39378894ee6ae9f555ae2de332d513a5763276a9265f8e7cbaeb1b1ee74623a",
-                "sha256:ede3b46cdb719c794427dcce9d8beb4abe8b9aa1e97526cc20de9bd6583ad1ef",
-                "sha256:f2a8508f7350512434e41065684076f640ecce176d262a7d54f0da41d99c5a95",
-                "sha256:f44477ae29025d8ea87ec308539f95963ffdc31a82f42ca9deecf2d505242e72",
-                "sha256:f64394bd7ceef1237cc604b5a89bf748c95982a84bcd3c4bbeb40f685c810794",
-                "sha256:fc4dd8b01a8112809e6b636b00f487846956402834a7fd59d46d4f4267181c41",
-                "sha256:fce78593346c014d0d986b7ebc80d782b7f5e19843ca798ed62f8e3ba8728576",
-                "sha256:fd547ec596d90c8676e369dd8a581a21227fe9b4ad37d0dc7feb4ccf544c2d59"
+                "sha256:009a028127e0a1755c38b03244c0bea9d5565630db9c4cf9572496e947137a87",
+                "sha256:0414fd91ce0b763d4eadb4456795b307a71524dbacd015c657bb2a39db2eab89",
+                "sha256:0978f29222e649c351b173da2b9b4665ad1feb8d1daa9d971eb90df08702668a",
+                "sha256:0ef8fb25e52663a1c85d608f6dd72e19bd390e2ecaf29c17fb08f730226e3a08",
+                "sha256:10b08293cda921157f1e7c2790999d903b3fd28cd5c208cf8826b3b508026996",
+                "sha256:1684a9bd9077e922300ecd48003ddae7a7474e0412bea38d4631443a91d61077",
+                "sha256:1b372aad2b5f81db66ee7ec085cbad72c4da660d994e8e590c997e9b01e44901",
+                "sha256:1e21fb44e1eff06dd6ef971d4bdc611807d6bd3691223d9c01a18cec3677939e",
+                "sha256:2305517e332a862ef75be8fad3606ea10108662bc6fe08509d5ca99503ac2aee",
+                "sha256:24ad1d10c9db1953291f56b5fe76203977f1ed05f82d09ec97acb623a7976574",
+                "sha256:272b4f1599f1b621bf2aabe4e5b54f39a933971f4e7c9aa311d6d7dc06965165",
+                "sha256:2a1fca9588f360036242f379bfea2b8b44cae2721859b1c56d033adfd5893634",
+                "sha256:2b4fa2606adf392051d990c3b3877d768771adc3faf2e117b9de7eb977741229",
+                "sha256:3150078118f62371375e1e69b13b48288e44f6691c1069340081c3fd12c94d5b",
+                "sha256:326dd1d3caf910cd26a26ccbfb84c03b608ba32499b5d6eeb09252c920bcbe4f",
+                "sha256:34c09b43bd538bf6c4b891ecce94b6fa4f1f10663a8d4ca589a079a5018f6ed7",
+                "sha256:388a45dc77198b2460eac0aca1efd6a7c09e976ee768b0d5109173e521a19daf",
+                "sha256:3adeef150d528ded2a8e734ebf9ae2e658f4c49bf413f5f157a470e17a4a2e89",
+                "sha256:3edac5d74bb3209c418805bda77f973117836e1de7c000e9755e572c1f7850d0",
+                "sha256:3f6b4aca43b602ba0f1459de647af954769919c4714706be36af670a5f44c9c1",
+                "sha256:3fc056e35fa6fba63248d93ff6e672c096f95f7836938241ebc8260e062832fe",
+                "sha256:418857f837347e8aaef682679f41e36c24250097f9e2f315d39bae3a99a34cbf",
+                "sha256:42430ff511571940d51e75cf42f1e4dbdded477e71c1b7a17f4da76c1da8ea76",
+                "sha256:44ceac0450e648de86da8e42674f9b7077d763ea80c8ceb9d1c3e41f0f0a9951",
+                "sha256:47d49ac96156f0928f002e2424299b2c91d9db73e08c4cd6742923a086f1c863",
+                "sha256:48dd18adcf98ea9cd721a25313aef49d70d413a999d7d89df44f469edfb38a06",
+                "sha256:49d43402c6e3013ad0978602bf6bf5328535c48d192304b91b97a3c6790b1562",
+                "sha256:4d04acba75c72e6eb90745447d69f84e6c9056390f7a9724605ca9c56b4afcc6",
+                "sha256:57a7c87927a468e5a1dc60c17caf9597161d66457a34273ab1760219953f7f4c",
+                "sha256:58a3c13d1c3005dbbac5c9f0d3210b60220a65a999b1833aa46bd6677c69b08e",
+                "sha256:5df5e3d04101c1e5c3b1d69710b0574171cc02fddc4b23d1b2813e75f35a30b1",
+                "sha256:63243b21c6e28ec2375f932a10ce7eda65139b5b854c0f6b82ed945ba526bff3",
+                "sha256:64dd68a92cab699a233641f5929a40f02a4ede8c009068ca8aa1fe87b8c20ae3",
+                "sha256:6604711362f2dbf7160df21c416f81fac0de6dbcf0b5445a2ef25478ecc4c778",
+                "sha256:6c4fcfa71e2c6a3cb568cf81aadc12768b9995323186a10827beccf5fa23d4f8",
+                "sha256:6d88056a04860a98341a0cf53e950e3ac9f4e51d1b6f61a53b0609df342cc8b2",
+                "sha256:705227dccbe96ab02c7cb2c43e1228e2826e7ead880bb19ec94ef279e9555b5b",
+                "sha256:728be34f70a190566d20aa13dc1f01dc44b6aa74580e10a3fb159691bc76909d",
+                "sha256:74dece2bfc60f0f70907c34b857ee98f2c6dd0f75185db133770cd67300d505f",
+                "sha256:75c16b2a900b3536dfc7014905a128a2bea8fb01f9ee26d2d7d8db0a08e7cb2c",
+                "sha256:77e913b846a6b9c5f767b14dc1e759e5aff05502fe73079f6f4176359d832581",
+                "sha256:7a66c506ec67eb3159eea5096acd05f5e788ceec7b96087d30c7d2865a243918",
+                "sha256:8c46d3d89902c393a1d1e243ac847e0442d0196bbd81aecc94fcebbc2fd5857c",
+                "sha256:93202666046d9edadfe9f2e7bf5e0782ea0d497b6d63da322e541665d65a044e",
+                "sha256:97209cc91189b48e7cfe777237c04af8e7cc51eb369004e061809bcdf4e55220",
+                "sha256:a48f4f7fea9a51098b02209d90297ac324241bf37ff6be6d2b0149ab2bd51b37",
+                "sha256:a783cd344113cb88c5ff7ca32f1f16532a6f2142185147822187913eb989f739",
+                "sha256:ae0eec05ab49e91a78700761777f284c2df119376e391db42c38ab46fd662b77",
+                "sha256:ae4d7ff1049f36accde9e1ef7301912a751e5bae0a9d142459646114c70ecba6",
+                "sha256:b05df9ea7496df11b710081bd90ecc3a3db6adb4fee36f6a411e7bc91a18aa42",
+                "sha256:baf211dcad448a87a0d9047dc8282d7de59473ade7d7fdf22150b1d23859f946",
+                "sha256:bb81f753c815f6b8e2ddd2eef3c855cf7da193b82396ac013c661aaa6cc6b0a5",
+                "sha256:bcd7bb1e5c45274af9a1dd7494d3c52b2be5e6bd8d7e49c612705fd45420b12d",
+                "sha256:bf071f797aec5b96abfc735ab97da9fd8f8768b43ce2abd85356a3127909d146",
+                "sha256:c15163b6125db87c8f53c98baa5e785782078fbd2dbeaa04c6141935eb6dab7a",
+                "sha256:cb6d48d80a41f68de41212f3dfd1a9d9898d7841c8f7ce6696cf2fd9cb57ef83",
+                "sha256:ceff9722e0df2e0a9e8a79c610842004fa54e5b309fe6d218e47cd52f791d7ef",
+                "sha256:cfa2bbca929aa742b5084fd4663dd4b87c191c844326fcb21c3afd2d11497f80",
+                "sha256:d617c241c8c3ad5c4e78a08429fa49e4b04bedfc507b34b4d8dceb83b4af3588",
+                "sha256:d881d152ae0007809c2c02e22aa534e702f12071e6b285e90945aa3c376463c5",
+                "sha256:da65c3f263729e47351261351b8679c6429151ef9649bba08ef2528ff2c423b2",
+                "sha256:de986979bbd87272fe557e0a8fcb66fd40ae2ddfe28a8b1ce4eae22681728fef",
+                "sha256:df60a94d332158b444301c7f569659c926168e4d4aad2cfbf4bce0e8fb8be826",
+                "sha256:dfef7350ee369197106805e193d420b75467b6cceac646ea5ed3049fcc950a05",
+                "sha256:e59399dda559688461762800d7fb34d9e8a6a7444fd76ec33220a926c8be1516",
+                "sha256:e6f3515aafe0209dd17fb9bdd3b4e892963370b3de781f53e1746a521fb39fc0",
+                "sha256:e7fd20d6576c10306dea2d6a5765f46f0ac5d6f53436217913e952d19237efc4",
+                "sha256:ebb78745273e51b9832ef90c0898501006670d6e059f2cdb0e999494eb1450c2",
+                "sha256:efff27bd8cbe1f9bd127e7894942ccc20c857aa8b5a0327874f30201e5ce83d0",
+                "sha256:f37db05c6051eff17bc832914fe46869f8849de5b92dc4a3466cd63095d23dfd",
+                "sha256:f8ca8ad414c85bbc50f49c0a106f951613dfa5f948ab69c10ce9b128d368baf8",
+                "sha256:fb742dcdd5eec9f26b61224c23baea46c9055cf16f62475e11b9b15dfd5c117b",
+                "sha256:fc77086ce244453e074e445104f0ecb27530d6fd3a46698e33f6c38951d5a0f1",
+                "sha256:ff205b58dc2929191f68162633d5e10e8044398d7a45265f90a0f1d51f85f72c"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.7.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.8.2"
         }
     }
 }
```

### Comparing `aasm-0.0.9/aasm/generating/code.py` & `aasm-0.1.0/aasm/generating/code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 from __future__ import annotations
 
 from typing import List
 
 
 class Code:
-    def __init__(self, agent_code_lines: List[str], graph_code_lines: List[str]):
+    def __init__(
+        self,
+        agent_code_lines: List[str],
+        graph_code_lines: List[str],
+        module_code_lines: List[str],
+    ):
         self.agent_code_lines: List[str] = agent_code_lines
         self.graph_code_lines: List[str] = graph_code_lines
+        self.module_code_lines: List[str] = module_code_lines
         self._iter_code_lines: List[str] | None = None
         self._iter_idx: int | None = None
         self._iter_num_code_lines: int | None = None
 
     def __iter__(self) -> Code:
-        self._iter_code_lines = self.agent_code_lines + self.graph_code_lines
+        self._iter_code_lines = (
+            self.agent_code_lines
+            + ["\n"]
+            + self.graph_code_lines
+            + ["\n"]
+            + self.module_code_lines
+        )
         self._iter_num_code_lines = len(self._iter_code_lines)
         self._iter_idx = -1
         return self
 
-    def __next__(self):
+    def __next__(self) -> str:
+        if (
+            self._iter_idx is None
+            or self._iter_code_lines is None
+            or self._iter_num_code_lines is None
+        ):
+            raise Exception("Code iterator not initialized")
+
         self._iter_idx += 1
         if self._iter_idx < self._iter_num_code_lines:
             return self._iter_code_lines[self._iter_idx]
         raise StopIteration
```

### Comparing `aasm-0.0.9/aasm/intermediate/action.py` & `aasm-0.1.0/aasm/intermediate/action.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,90 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List
 
-from aasm.intermediate.block import Block
+from aasm.intermediate.block import Block, Declarations
 
 if TYPE_CHECKING:
     from aasm.intermediate.declaration import Declaration
     from aasm.intermediate.instruction import Instruction
     from aasm.intermediate.message import Message
 
 
 class Action:
     def __init__(self, name: str):
         self.name: str = name
-        self._block_stack: List[Block] = [Block([])]
+        self._block_stack: List[Block] = [Block(Declarations())]
         self._nested_blocks_count: int = 0
-        
+
+    @property
+    def nested_blocks_count(self) -> int:
+        return self._nested_blocks_count
+
     @property
     def main_block(self) -> Block:
         return self._block_stack[0]
-    
+
     @property
     def current_block(self) -> Block:
         return self._block_stack[-1]
-    
+
     def is_declaration_in_scope(self, name: str) -> bool:
-        return name in self.current_block.declarations_in_scope
-    
-    def add_declaration(self, declaration: Declaration) -> None:
-        self.current_block.add_declaration(declaration)
-    
+        return name in self.current_block.declared_names_in_scope
+
+    def is_declared_float(self, name: str) -> bool:
+        return self.current_block.is_declared_float(name)
+
+    def is_declared_connection(self, name: str) -> bool:
+        return self.current_block.is_declared_connection(name)
+
+    def is_declared_module_variable(self, name: str) -> bool:
+        return self.current_block.is_declared_module_variable(name)
+
+    def get_module_variable_type(self, name: str) -> str:
+        return self.current_block.get_module_variable_type(name)
+
+    def add_float_declaration(self, declaration: Declaration) -> None:
+        self.current_block.add_float_declaration(declaration)
+
+    def add_connection_declaration(self, declaration: Declaration) -> None:
+        self.current_block.add_connection_declaration(declaration)
+
+    def add_module_variable_declaration(self, declaration: Declaration) -> None:
+        self.current_block.add_module_variable_declaration(declaration)
+
     def add_instruction(self, instruction: Instruction) -> None:
         self.current_block.add_statement(instruction)
-        
+
     def start_block(self) -> None:
-        new_block = Block(self.current_block._declared_names)
+        new_block = Block(self.current_block.get_declarations)
         self.current_block.add_statement(new_block)
         self._block_stack.append(new_block)
         self._nested_blocks_count += 1
-    
+
     def end_block(self) -> None:
         self._block_stack.pop()
         self._nested_blocks_count -= 1
-        
+
     def print(self) -> None:
-        print(f'Action {self.name}')
+        print(f"Action {self.name}")
         self.main_block.print()
 
 
 class ModifySelfAction(Action):
     def __init__(self, name: str):
         super().__init__(name)
-        
+
     def print(self) -> None:
-        print('ModifySelfAction')
+        print("ModifySelfAction")
         super().print()
 
 
 class SendMessageAction(Action):
     def __init__(self, name: str, message: Message):
         super().__init__(name)
         self.send_message: Message = message
-        
+
     def print(self) -> None:
-        print('SendMessageAction')
+        print("SendMessageAction")
         super().print()
         self.send_message.print()
```

### Comparing `aasm-0.0.9/aasm/intermediate/agent.py` & `aasm-0.1.0/aasm/intermediate/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,269 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List
 
+from aasm.utils.iteration import zip_consecutive_pairs
+
 if TYPE_CHECKING:
-    from aasm.intermediate.behaviour import (Behaviour, CyclicBehaviour,
-                                             MessageReceivedBehaviour,
-                                             OneTimeBehaviour, SetupBehaviour)
+    from aasm.intermediate.behaviour import (
+        Behaviour,
+        CyclicBehaviour,
+        MessageReceivedBehaviour,
+        OneTimeBehaviour,
+        SetupBehaviour,
+    )
 
 
 class InitFloatParam:
     def __init__(self, name: str, value: str):
         self.name: str = name
         self.value: str = value
-        
+
     def print(self) -> None:
-        print(f'InitFloatParam {self.name} = {self.value}')
+        print(f"InitFloatParam {self.name} = {self.value}")
 
 
 class DistNormalFloatParam:
     def __init__(self, name: str, mean: str, std_dev: str):
         self.name: str = name
         self.mean: str = mean
         self.std_dev: str = std_dev
 
     def print(self) -> None:
-        print(f'DistNormalFloatParam {self.name} = normal(mean={self.mean}, std_dev={self.std_dev})')
+        print(
+            f"DistNormalFloatParam {self.name} = normal(mean={self.mean}, std_dev={self.std_dev})"
+        )
 
 
 class DistExpFloatParam:
     def __init__(self, name: str, lambda_: str):
         self.name: str = name
         self.lambda_: str = lambda_
 
     def print(self) -> None:
-        print(f'DistExpFloatParam {self.name} = exp(lambda={self.lambda_})')
+        print(f"DistExpFloatParam {self.name} = exp(lambda={self.lambda_})")
+
+
+class DistUniformFloatParam:
+    def __init__(self, name: str, a: str, b: str):
+        self.name: str = name
+        self.a: str = a
+        self.b: str = b
+
+    def print(self) -> None:
+        print(f"DistUniformFloatParam {self.name} = uniform(a={self.a}, b={self.b})")
 
 
 class EnumParam:
     def __init__(self, name: str, enums: List[str]):
         self.name: str = name
-        self.enum_values: List[EnumValue] = [EnumValue(name, value, percentage) for value, percentage in zip(*[iter(enums)] * 2)]
-        
+        self.enum_values: List[EnumValue] = [
+            EnumValue(name, value, percentage)
+            for value, percentage in zip_consecutive_pairs(enums)
+        ]
+
     def print(self) -> None:
-        print(f'EnumParam {self.name} = {self.enum_values}')
+        print(f"EnumParam {self.name} = {self.enum_values}")
 
 
 class EnumValue:
     def __init__(self, from_enum: str, value: str, percentage: str):
         self.from_enum: str = from_enum
         self.value: str = value
         self.percentage: str = percentage
-        
+
     def __str__(self) -> str:
-        return f'({self.value}, {self.percentage}; from_enum={self.from_enum})'
+        return f"({self.value}, {self.percentage}; from_enum={self.from_enum})"
 
 
 class MessageListParam:
     def __init__(self, name: str):
         self.name: str = name
-        
+
     def print(self) -> None:
-        print(f'MessageListParam {self.name} = []')
+        print(f"MessageListParam {self.name} = []")
 
 
 class ConnectionListParam:
     def __init__(self, name: str):
         self.name: str = name
-        
+
+    def print(self) -> None:
+        print(f"ConnectionListParam {self.name} = []")
+
+
+class FloatListParam:
+    def __init__(self, name: str):
+        self.name: str = name
+
+    def print(self) -> None:
+        print(f"FloatListParam {self.name} = []")
+
+
+class ModuleVariableParam:
+    def __init__(self, name: str, type: str):
+        self.name: str = name
+        self.type: str = type
+
     def print(self) -> None:
-        print(f'ConnectionListParam {self.name} = []')
+        print(f"ModuleVariableParam {self.name}: {self.type}")
 
 
 class Agent:
-    RESERVED_LOCATION_PARAMS = [ 'location' ]
-    RESERVED_CONNECTION_LIST_PARAMS = [ 'connections' ]
-    RESERVED_FLOAT_PARAMS = [ 'connCount', 'msgRCount', 'msgSCount' ]
-    
+    RESERVED_CONNECTION_PARAMS = ["self"]
+    RESERVED_CONNECTION_LIST_PARAMS = ["connections"]
+    RESERVED_FLOAT_PARAMS = ["connCount", "msgRCount", "msgSCount"]
+
     def __init__(self, name: str):
         self.name: str = name
         self.init_floats: Dict[str, InitFloatParam] = {}
         self.dist_normal_floats: Dict[str, DistNormalFloatParam] = {}
         self.dist_exp_floats: Dict[str, DistExpFloatParam] = {}
+        self.dist_unifrom_floats: Dict[str, DistUniformFloatParam] = {}
         self.enums: Dict[str, EnumParam] = {}
         self.connection_lists: Dict[str, ConnectionListParam] = {}
         self.message_lists: Dict[str, MessageListParam] = {}
+        self.float_lists: Dict[str, FloatListParam] = {}
+        self.module_variables: Dict[str, ModuleVariableParam] = {}
         self.setup_behaviours: Dict[str, SetupBehaviour] = {}
         self.one_time_behaviours: Dict[str, OneTimeBehaviour] = {}
         self.cyclic_behaviours: Dict[str, CyclicBehaviour] = {}
         self.message_received_behaviours: Dict[str, MessageReceivedBehaviour] = {}
-        self._last_modified_behaviours: Dict[str, Behaviour] | None = None
-    
+        self._last_modified_behaviour: Behaviour | None = None
+
+    def get_module_variable_type(self, name):
+        return self.module_variables[name].type
+
     @property
     def last_behaviour(self) -> Behaviour:
-        return self._last_modified_behaviours[list(self._last_modified_behaviours.keys())[-1]]
-    
+        if self._last_modified_behaviour is None:
+            raise Exception("No behaviour added to agent")
+        return self._last_modified_behaviour
+
     @property
     def param_names(self) -> List[str]:
-        return [ *Agent.RESERVED_LOCATION_PARAMS,
-                 *Agent.RESERVED_CONNECTION_LIST_PARAMS,
-                 *Agent.RESERVED_FLOAT_PARAMS,
-                 *list(self.init_floats), 
-                 *list(self.dist_normal_floats),
-                 *list(self.dist_exp_floats),
-                 *list(self.enums), 
-                 *list(self.connection_lists),
-                 *list(self.message_lists) ]
-    
+        return [
+            *Agent.RESERVED_CONNECTION_PARAMS,
+            *Agent.RESERVED_CONNECTION_LIST_PARAMS,
+            *Agent.RESERVED_FLOAT_PARAMS,
+            *list(self.init_floats),
+            *list(self.dist_normal_floats),
+            *list(self.dist_exp_floats),
+            *list(self.dist_unifrom_floats),
+            *list(self.enums),
+            *list(self.connection_lists),
+            *list(self.message_lists),
+            *list(self.float_lists),
+            *list(self.module_variables),
+        ]
+
     @property
     def behaviour_names(self) -> List[str]:
-        return [ *list(self.setup_behaviours),
-                 *list(self.one_time_behaviours),
-                 *list(self.cyclic_behaviours),
-                 *list(self.message_received_behaviours) ]
-    
+        return [
+            *list(self.setup_behaviours),
+            *list(self.one_time_behaviours),
+            *list(self.cyclic_behaviours),
+            *list(self.message_received_behaviours),
+        ]
+
     @property
     def float_param_names(self) -> List[str]:
-        return [ *list(self.init_floats),
-                 *list(self.dist_normal_floats), 
-                 *list(self.dist_exp_floats) ]
-    
+        return [
+            *list(self.init_floats),
+            *list(self.dist_normal_floats),
+            *list(self.dist_exp_floats),
+            *list(self.dist_unifrom_floats),
+        ]
+
     def add_init_float(self, float_param: InitFloatParam) -> None:
         self.init_floats[float_param.name] = float_param
 
     def add_dist_normal_float(self, float_param: DistNormalFloatParam) -> None:
         self.dist_normal_floats[float_param.name] = float_param
-    
+
     def add_dist_exp_float(self, float_param: DistExpFloatParam) -> None:
         self.dist_exp_floats[float_param.name] = float_param
-    
+
+    def add_dist_uniform_float(self, float_param: DistUniformFloatParam) -> None:
+        self.dist_unifrom_floats[float_param.name] = float_param
+
     def add_enum(self, enum_param: EnumParam) -> None:
         self.enums[enum_param.name] = enum_param
-    
+
     def add_connection_list(self, list_param: ConnectionListParam) -> None:
         self.connection_lists[list_param.name] = list_param
-    
+
     def add_message_list(self, list_param: MessageListParam) -> None:
         self.message_lists[list_param.name] = list_param
-    
+
+    def add_float_list(self, list_param: FloatListParam) -> None:
+        self.float_lists[list_param.name] = list_param
+
+    def add_module_variable(self, variable_param: ModuleVariableParam) -> None:
+        self.module_variables[variable_param.name] = variable_param
+
     def add_setup_behaviour(self, behaviour: SetupBehaviour) -> None:
         self.setup_behaviours[behaviour.name] = behaviour
-        self._last_modified_behaviours = self.setup_behaviours
-    
+        self._last_modified_behaviour = behaviour
+
     def add_one_time_behaviour(self, behaviour: OneTimeBehaviour) -> None:
         self.one_time_behaviours[behaviour.name] = behaviour
-        self._last_modified_behaviours = self.one_time_behaviours
-    
+        self._last_modified_behaviour = behaviour
+
     def add_cyclic_behaviour(self, behaviour: CyclicBehaviour) -> None:
         self.cyclic_behaviours[behaviour.name] = behaviour
-        self._last_modified_behaviours = self.cyclic_behaviours
-    
-    def add_message_received_behaviour(self, behaviour: MessageReceivedBehaviour) -> None:
+        self._last_modified_behaviour = behaviour
+
+    def add_message_received_behaviour(
+        self, behaviour: MessageReceivedBehaviour
+    ) -> None:
         self.message_received_behaviours[behaviour.name] = behaviour
-        self._last_modified_behaviours = self.message_received_behaviours
+        self._last_modified_behaviour = behaviour
 
     def param_exists(self, name: str) -> bool:
         return name in self.param_names
-    
+
     def behaviour_exists(self, name: str) -> bool:
         return name in self.behaviour_names
 
     def name_exists(self, name: str) -> bool:
         return self.param_exists(name) or self.behaviour_exists(name)
-        
-    def behaviour_for_template_exists(self, msg_type: str, msg_performative: str):
+
+    def behaviour_for_template_exists(
+        self, msg_type: str, msg_performative: str
+    ) -> bool:
         for msg_rcv_behav in self.message_received_behaviours.values():
-            if msg_rcv_behav.received_message.type == msg_type and msg_rcv_behav.received_message.performative == msg_performative:
+            if (
+                msg_rcv_behav.received_message.type == msg_type
+                and msg_rcv_behav.received_message.performative == msg_performative
+            ):
                 return True
-    
+        return False
+
     def print(self) -> None:
-        print(f'Agent {self.name}')
+        print(f"Agent {self.name}")
         for init_float_param in self.init_floats.values():
             init_float_param.print()
         for dist_normal_float_param in self.dist_normal_floats.values():
             dist_normal_float_param.print()
         for dist_exp_float_param in self.dist_exp_floats.values():
             dist_exp_float_param.print()
+        for dist_uniform_float_param in self.dist_unifrom_floats.values():
+            dist_uniform_float_param.print()
         for enum_param in self.enums.values():
             enum_param.print()
         for connection_list_param in self.connection_lists.values():
             connection_list_param.print()
         for message_list_param in self.message_lists.values():
             message_list_param.print()
+        for float_list_param in self.float_lists.values():
+            float_list_param.print()
+        for module_variable in self.module_variables.values():
+            module_variable.print()
         for setup_behaviour in self.setup_behaviours.values():
             setup_behaviour.print()
         for one_time_behaviour in self.one_time_behaviours.values():
             one_time_behaviour.print()
         for cyclic_behaviour in self.cyclic_behaviours.values():
             cyclic_behaviour.print()
         for message_received_behaviour in self.message_received_behaviours.values():
```

### Comparing `aasm-0.0.9/aasm/intermediate/behaviour.py` & `aasm-0.1.0/aasm/intermediate/behaviour.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,45 +7,45 @@
     from aasm.intermediate.message import Message
 
 
 class Behaviour:
     def __init__(self, name: str):
         self.name = name
         self.actions: Dict[str, Action] = {}
-        
+
     @property
     def last_action(self) -> Action:
         return self.actions[list(self.actions.keys())[-1]]
-    
+
     def add_action(self, action: Action) -> None:
         self.actions[action.name] = action
-        
+
     def action_exists(self, name: str) -> bool:
         return name in self.actions
 
     def print(self) -> None:
-        print(f'Behaviour {self.name}')
+        print(f"Behaviour {self.name}")
         for action in self.actions.values():
             action.print()
 
 
 class SetupBehaviour(Behaviour):
     def __init__(self, name: str):
         super().__init__(name)
-        
-        
+
+
 class OneTimeBehaviour(Behaviour):
     def __init__(self, name: str, delay: str):
         super().__init__(name)
         self.delay: str = delay
-        
-        
+
+
 class CyclicBehaviour(Behaviour):
     def __init__(self, name: str, period: str):
         super().__init__(name)
         self.period: str = period
-        
-        
+
+
 class MessageReceivedBehaviour(Behaviour):
     def __init__(self, name: str, message: Message):
         super().__init__(name)
         self.received_message: Message = message
```

### Comparing `aasm-0.0.9/aasm/parsing/op/action.py` & `aasm-0.1.0/aasm/parsing/op/action.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,51 +7,62 @@
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def op_ACTION(state: State, name: str, category: str, args: List[str]) -> None:
     state.require(
-        state.in_behaviour, 
-        'Actions must be definied inside behaviours.', 
-        'Try defining new behaviours using BEHAV.'
+        state.in_behaviour,
+        "Actions must be definied inside behaviours.",
+        "Try defining new behaviours using BEHAV.",
     )
     state.require(
-        not state.in_action, 
-        'Cannot define an action in another action.', 
-        'Try finishing current action using EACTION.'
+        not state.in_action,
+        "Cannot define an action in another action.",
+        "Try finishing current action using EACTION.",
     )
-    state.require(not state.last_behaviour.action_exists(name), f'Action {name} already exists in current behaviour.')
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.last_behaviour.action_exists(name),
+        f"Action {name} already exists in current behaviour.",
     )
-    
+    state.require(
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+
     match category, args:
-        case 'modify_self', [ ]:
+        case "modify_self", []:
             state.last_behaviour.add_action(ModifySelfAction(name))
-            
-        case 'send_msg', [ msg_type, msg_performative ]:
+
+        case "send_msg", [msg_type, msg_performative]:
             state.require(
-                state.message_exists(msg_type, msg_performative), 
-                f'Message {msg_type}/{msg_performative} does not exist.', 
-                'Try defining new messages using MESSAGE.'
+                state.message_exists(msg_type, msg_performative),
+                f"Message {msg_type}/{msg_performative} does not exist.",
+                "Try defining new messages using MESSAGE.",
+            )
+
+            state.last_behaviour.add_action(
+                SendMessageAction(
+                    name, state.get_message_instance(msg_type, msg_performative)
+                )
             )
 
-            state.last_behaviour.add_action(SendMessageAction(name, state.get_message_instance(msg_type, msg_performative)))
-            
         case _:
-            state.panic(f'Incorrect operation: ACTION {category} {args}')
-    
+            state.panic(f"Incorrect operation: ACTION {category} {args}")
+
     state.in_action = True
 
 
-def op_EACTION(state: State) -> None:            
-    state.require(state.in_action, 'Not inside any action.', 'Try defining new actions using ACTION.')
+def op_EACTION(state: State) -> None:
     state.require(
-        state.last_action._nested_blocks_count == 0, 
-        'There are unclosed blocks.', 
-        'Try closing them using EBLOCK.'
+        state.in_action,
+        "Not inside any action.",
+        "Try defining new actions using ACTION.",
     )
-    
+    state.require(
+        state.last_action.nested_blocks_count == 0,
+        "There are unclosed blocks.",
+        "Try closing them using EBLOCK.",
+    )
+
     state.in_action = False
```

### Comparing `aasm-0.0.9/aasm/parsing/op/agent.py` & `aasm-0.1.0/aasm/parsing/op/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,35 +5,48 @@
 from aasm.intermediate.agent import Agent
 from aasm.utils.validation import is_valid_name, print_invalid_names
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_AGENT(state: State, name: str) -> None:    
-    state.require(not state.in_agent, 'Already inside an agent.', 'First end current agent using EAGENT.')
+def op_AGENT(state: State, name: str) -> None:
     state.require(
-        not state.in_message, 
-        'Cannot define agents inside messages.', 
-        'First end current message using EMESSAGE.'
+        not state.in_agent,
+        "Already inside an agent.",
+        "First end current agent using EAGENT.",
     )
-    state.require(not state.in_graph, 'Cannot define agents inside graphs.', 'First end current graph using EGRAPH.')
-    state.require(not state.agent_exists(name), f'Agent {name} already exists in the current environment.')
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.in_message,
+        "Cannot define agents inside messages.",
+        "First end current message using EMESSAGE.",
     )
-    
+    state.require(
+        not state.in_graph,
+        "Cannot define agents inside graphs.",
+        "First end current graph using EGRAPH.",
+    )
+    state.require(
+        not state.agent_exists(name),
+        f"Agent {name} already exists in the current environment.",
+    )
+    state.require(
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+
     state.in_agent = True
     state.add_agent(Agent(name))
 
 
-def op_EAGENT(state: State) -> None:    
-    state.require(state.in_agent, 'Not inside any agent.', 'Try defining new agents using AGENT.')
+def op_EAGENT(state: State) -> None:
     state.require(
-        not state.in_behaviour, 
-        'Cannot end an agent inside a behaviour.', 
-        'First end current behaviour using EBEHAV.'
+        state.in_agent, "Not inside any agent.", "Try defining new agents using AGENT."
     )
-    
+    state.require(
+        not state.in_behaviour,
+        "Cannot end an agent inside a behaviour.",
+        "First end current behaviour using EBEHAV.",
+    )
+
     state.in_agent = False
```

### Comparing `aasm-0.0.9/aasm/parsing/op/behav.py` & `aasm-0.1.0/aasm/parsing/op/behav.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,95 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List
 
-from aasm.intermediate.behaviour import (CyclicBehaviour,
-                                         MessageReceivedBehaviour,
-                                         OneTimeBehaviour, SetupBehaviour)
+from aasm.intermediate.behaviour import (
+    CyclicBehaviour,
+    MessageReceivedBehaviour,
+    OneTimeBehaviour,
+    SetupBehaviour,
+)
 from aasm.utils.validation import is_float, is_valid_name, print_invalid_names
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def op_BEHAV(state: State, name: str, category: str, args: List[str]):
-    state.require(state.in_agent, 'Cannot define behaviours outside agents.', 'Try defining new agents using AGENT.')
+    state.require(
+        state.in_agent,
+        "Cannot define behaviours outside agents.",
+        "Try defining new agents using AGENT.",
+    )
     state.require(
         not state.in_behaviour,
-        'Cannot define behaviours inside other behaviours.',
-        'First end current behaviour using EBEHAV.'
+        "Cannot define behaviours inside other behaviours.",
+        "First end current behaviour using EBEHAV.",
     )
-    state.require(not state.last_agent.name_exists(name), f'{name} already exists in current agent.')
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.last_agent.name_exists(name),
+        f"{name} already exists in current agent.",
     )
-    
+    state.require(
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+
     match category, args:
-        case 'setup', [ ]:
+        case "setup", []:
             state.last_agent.add_setup_behaviour(SetupBehaviour(name))
-            
-        case 'one_time', [ delay ]:
-            state.require(is_float(delay) and float(delay) >= 0, f'{delay} is not a valid delay value.')
+
+        case "one_time", [delay]:
+            state.require(
+                is_float(delay) and float(delay) >= 0,
+                f"{delay} is not a valid delay value.",
+            )
 
             state.last_agent.add_one_time_behaviour(OneTimeBehaviour(name, delay))
-            
-        case 'cyclic', [ period ]:
-            state.require(is_float(period) and float(period) > 0, f'{period} is not a valid period value.')
+
+        case "cyclic", [period]:
+            state.require(
+                is_float(period) and float(period) > 0,
+                f"{period} is not a valid period value.",
+            )
 
             state.last_agent.add_cyclic_behaviour(CyclicBehaviour(name, period))
-            
-        case 'msg_rcv', [ msg_type, msg_performative ]:
+
+        case "msg_rcv", [msg_type, msg_performative]:
             state.require(
-                state.message_exists(msg_type, msg_performative), 
-                f'Message {msg_type}/{msg_performative} does not exist.', 
-                'Try defining new messages using MESSAGE'
+                state.message_exists(msg_type, msg_performative),
+                f"Message {msg_type}/{msg_performative} does not exist.",
+                "Try defining new messages using MESSAGE",
             )
             state.require(
-                not state.last_agent.behaviour_for_template_exists(msg_type, msg_performative), 
-                f'Behaviour for template {msg_type}/{msg_performative} already exists in current agent.'
+                not state.last_agent.behaviour_for_template_exists(
+                    msg_type, msg_performative
+                ),
+                f"Behaviour for template {msg_type}/{msg_performative} already exists in current agent.",
             )
 
             state.last_agent.add_message_received_behaviour(
-                MessageReceivedBehaviour(name, state.get_message_instance(msg_type, msg_performative))
+                MessageReceivedBehaviour(
+                    name, state.get_message_instance(msg_type, msg_performative)
+                )
             )
-            
+
         case _:
-            state.panic(f'Incorrect operation: BEHAV {name} {category} {args}')
-    
+            state.panic(f"Incorrect operation: BEHAV {name} {category} {args}")
+
     state.in_behaviour = True
 
 
-def op_EBEHAV(state: State) -> None:            
-    state.require(state.in_behaviour, 'Not inside any behaviour.', 'Try defining new behaviours using BEHAV.')
+def op_EBEHAV(state: State) -> None:
+    state.require(
+        state.in_behaviour,
+        "Not inside any behaviour.",
+        "Try defining new behaviours using BEHAV.",
+    )
     state.require(
-        not state.in_action, 
-        'Cannot end behaviours inside actions.', 
-        'Try ending current action using EACTION.'
+        not state.in_action,
+        "Cannot end behaviours inside actions.",
+        "Try ending current action using EACTION.",
     )
-    
+
     state.in_behaviour = False
```

### Comparing `aasm-0.0.9/aasm/parsing/op/clr.py` & `aasm-0.1.0/aasm/parsing/op/lr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import Clear
+from aasm.intermediate.instruction import ListRead
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_CLR(state: State, arg1: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', 'CLR can be used inside actions.')
-    list_ = Argument(state, arg1)
-    state.require(list_.list_clear_context(), 'Mismatched type in the list clear context.', f'ARG {list_.explain()}')
+def op_LR(state: State, arg1: str, arg2: str, arg3: str) -> None:
+    state.require(
+        state.in_action, "Not inside any action.", "LR can be used inside actions."
+    )
+    dst = Argument(state, arg1)
+    list_ = Argument(state, arg2)
+    idx = Argument(state, arg3)
+    state.require(
+        dst.list_read_context(list_, idx),
+        "Mismatched types in the list read context.",
+        f"ARG1 {dst.explain()}, ARG2 {list_.explain()}, ARG3 {idx.explain()}",
+    )
 
-    state.last_action.add_instruction(Clear(list_))
+    state.last_action.add_instruction(ListRead(dst, list_, idx))
```

### Comparing `aasm-0.0.9/aasm/parsing/op/conditional.py` & `aasm-0.1.0/aasm/parsing/op/conditional.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,100 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import (IfEqual, IfGreaterThan,
-                                           IfGreaterThanOrEqual, IfLessThan,
-                                           IfLessThanOrEqual, IfNotEqual,
-                                           WhileEqual, WhileGreaterThan,
-                                           WhileGreaterThanOrEqual,
-                                           WhileLessThan, WhileLessThanOrEqual,
-                                           WhileNotEqual)
+from aasm.intermediate.instruction import (
+    IfEqual,
+    IfGreaterThan,
+    IfGreaterThanOrEqual,
+    IfLessThan,
+    IfLessThanOrEqual,
+    IfNotEqual,
+    WhileEqual,
+    WhileGreaterThan,
+    WhileGreaterThanOrEqual,
+    WhileLessThan,
+    WhileLessThanOrEqual,
+    WhileNotEqual,
+)
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def handle_unordered_conditional_statement(state: State, op: str, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'{op} can be used inside actions.')     
+def handle_unordered_conditional_statement(
+    state: State, op: str, arg1: str, arg2: str
+) -> None:
+    state.require(
+        state.in_action, "Not inside any action.", f"{op} can be used inside actions."
+    )
     lhs = Argument(state, arg1)
     rhs = Argument(state, arg2)
     state.require(
-        lhs.unordered_comparaison_context(rhs), 
-        'Mismatched types in the unordered comparaison context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        lhs.unordered_comparaison_context(rhs),
+        "Mismatched types in the unordered comparaison context.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
-    
+
     match op:
-        case 'IEQ':
+        case "IEQ":
             state.last_action.add_instruction(IfEqual(lhs, rhs))
 
-        case 'INEQ':
+        case "INEQ":
             state.last_action.add_instruction(IfNotEqual(lhs, rhs))
 
-        case 'WEQ':
+        case "WEQ":
             state.last_action.add_instruction(WhileEqual(lhs, rhs))
 
-        case 'WNEQ':
+        case "WNEQ":
             state.last_action.add_instruction(WhileNotEqual(lhs, rhs))
 
         case _:
-            state.panic(f'Unexpected error: {op} {arg1} {arg2}')
-    
+            state.panic(f"Unexpected error: {op} {arg1} {arg2}")
+
     state.last_action.start_block()
 
 
-def handle_ordered_conditional_statement(state: State, op: str, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'{op} can be used inside actions.')     
+def handle_ordered_conditional_statement(
+    state: State, op: str, arg1: str, arg2: str
+) -> None:
+    state.require(
+        state.in_action, "Not inside any action.", f"{op} can be used inside actions."
+    )
     lhs = Argument(state, arg1)
     rhs = Argument(state, arg2)
     state.require(
         lhs.ordered_comparaison_context(rhs),
-        'Mismatched types in the ordered comparaison context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        "Mismatched types in the ordered comparaison context.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
-    
+
     match op:
-        case 'IGT':
+        case "IGT":
             state.last_action.add_instruction(IfGreaterThan(lhs, rhs))
 
-        case 'IGTEQ':
+        case "IGTEQ":
             state.last_action.add_instruction(IfGreaterThanOrEqual(lhs, rhs))
 
-        case 'ILT':
+        case "ILT":
             state.last_action.add_instruction(IfLessThan(lhs, rhs))
 
-        case 'ILTEQ':
+        case "ILTEQ":
             state.last_action.add_instruction(IfLessThanOrEqual(lhs, rhs))
 
-        case 'WGT':
+        case "WGT":
             state.last_action.add_instruction(WhileGreaterThan(lhs, rhs))
 
-        case 'WGTEQ':
+        case "WGTEQ":
             state.last_action.add_instruction(WhileGreaterThanOrEqual(lhs, rhs))
 
-        case 'WLT':
+        case "WLT":
             state.last_action.add_instruction(WhileLessThan(lhs, rhs))
 
-        case 'WLTEQ':
+        case "WLTEQ":
             state.last_action.add_instruction(WhileLessThanOrEqual(lhs, rhs))
 
         case _:
-            state.panic(f'Unexpected error: {op} {arg1} {arg2}')
-    
+            state.panic(f"Unexpected error: {op} {arg1} {arg2}")
+
     state.last_action.start_block()
```

### Comparing `aasm-0.0.9/aasm/parsing/op/decl.py` & `aasm-0.1.0/aasm/parsing/op/decl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,57 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.declaration import Declaration
+from aasm.intermediate.declaration import (
+    ConnectionDeclaration,
+    FloatDeclaration,
+    ModuleVariableDeclaration,
+)
 from aasm.utils.validation import is_valid_name, print_invalid_names
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_DECL(state: State, name: str, value: str) -> None:            
-    state.require(state.in_action, 'Cannot declare variables outside actions.')
+def op_DECL(state: State, name: str, category: str, value: str) -> None:
+    state.require(state.in_action, "Cannot declare variables outside actions.")
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
     )
-    state.require(not state.last_agent.param_exists(name), f'{name} is already defined in current agent.')
     state.require(
-        not state.last_action.is_declaration_in_scope(name), 
-        f'{name} is already declared in current action scope.'
+        not state.last_agent.param_exists(name),
+        f"{name} is already defined in current agent.",
     )
-    lhs = Argument(state, name)
-    rhs = Argument(state, value)
     state.require(
-        lhs.declaration_context(rhs), 
-        'Mismatched types in the declaration context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        not state.last_action.is_declaration_in_scope(name),
+        f"{name} is already declared in current action scope.",
     )
-    
-    state.last_action.add_declaration(Declaration(lhs, rhs))
+    name_arg = Argument(state, name)
+    value_arg = Argument(state, value)
+    state.require(
+        name_arg.declaration_context(value_arg),
+        "Mismatched types in the declaration context.",
+        f"NAME {name_arg.explain()}, VALUE {value_arg.explain()}",
+    )
+
+    match category:
+        case "float":
+            state.last_action.add_float_declaration(
+                FloatDeclaration(name_arg, value_arg)
+            )
+
+        case "conn":
+            state.last_action.add_connection_declaration(
+                ConnectionDeclaration(name_arg, value_arg)
+            )
+
+        case _:
+            if category in state.get_module_types():
+                state.last_action.add_module_variable_declaration(
+                    ModuleVariableDeclaration(name_arg, value_arg, category)
+                )
+            else:
+                state.panic(f"Incorrect declaration: DECL {name} {category} {value}")
```

### Comparing `aasm-0.0.9/aasm/parsing/op/len.py` & `aasm-0.1.0/aasm/parsing/op/len.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from aasm.intermediate.instruction import Length
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def op_LEN(state: State, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', 'LEN can be used inside actions.')
+    state.require(
+        state.in_action, "Not inside any action.", "LEN can be used inside actions."
+    )
     lhs = Argument(state, arg1)
     rhs = Argument(state, arg2)
     state.require(
-        lhs.list_length_context(rhs), 
-        'Mismatched types in the list length context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        lhs.list_length_context(rhs),
+        "Mismatched types in the list length context.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
-    
+
     state.last_action.add_instruction(Length(lhs, rhs))
```

### Comparing `aasm-0.0.9/aasm/parsing/op/list.py` & `aasm-0.1.0/aasm/parsing/op/list_inclusion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,36 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import (AddElement, IfInList, IfNotInList,
-                                           RemoveElement)
+from aasm.intermediate.instruction import IfInList, IfNotInList
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def handle_list_modification(state: State, op: str, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', 'List modifications can be used inside actions.')
-    lhs = Argument(state, arg1)
-    rhs = Argument(state, arg2)
+def handle_list_inclusion(state: State, op: str, arg1: str, arg2: str):
     state.require(
-        lhs.list_modification_context(rhs), 
-        'Mismatched types in the list modification context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        state.in_action,
+        "Not inside any action.",
+        "List inclusion check can be used inside actions.",
     )
-    
-    match op:
-        case 'ADDE':
-            state.last_action.add_instruction(AddElement(lhs, rhs))
-
-        case 'REME':
-            state.last_action.add_instruction(RemoveElement(lhs, rhs))
-
-        case _:
-            state.panic(f'Unexpected error: {op} {arg1} {arg2}')
-
-
-def handle_list_inclusion(state: State, op: str, arg1: str, arg2: str):
-    state.require(state.in_action, 'Not inside any action.', 'List inclusion check can be used inside actions.')
     lhs = Argument(state, arg1)
     rhs = Argument(state, arg2)
     state.require(
-        lhs.list_inclusion_context(rhs), 
-        'Mismatched types in the list inclusion context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        lhs.list_inclusion_context(rhs),
+        "Mismatched types in the list inclusion context.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
-    
+
     match op:
-        case 'IN':
+        case "IN":
             state.last_action.add_instruction(IfInList(lhs, rhs))
 
-        case 'NIN':
+        case "NIN":
             state.last_action.add_instruction(IfNotInList(lhs, rhs))
 
         case _:
-            state.panic(f'Unexpected error: {op} {arg1} {arg2}')
-            
+            state.panic(f"Unexpected error: {op} {arg1} {arg2}")
+
     state.last_action.start_block()
```

### Comparing `aasm-0.0.9/aasm/parsing/op/math.py` & `aasm-0.1.0/aasm/parsing/op/math.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import Add, Divide, Multiply, Subtract
+from aasm.intermediate.instruction import Add, Cos, Divide, Multiply, Sin, Subtract
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def handle_math_statement(state: State, op: str, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action', f'{op} can be used inside actions.')
+    state.require(
+        state.in_action, "Not inside any action", f"{op} can be used inside actions."
+    )
     lhs = Argument(state, arg1)
     rhs = Argument(state, arg2)
     state.require(
         lhs.math_context(rhs),
-        'Mismatched types in the math statement.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        "Mismatched types in the math statement.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
 
     match op:
-        case 'ADD':
+        case "ADD":
             state.last_action.add_instruction(Add(lhs, rhs))
 
-        case 'SUBT':
+        case "SUBT":
             state.last_action.add_instruction(Subtract(lhs, rhs))
 
-        case 'MULT':
+        case "MULT":
             state.last_action.add_instruction(Multiply(lhs, rhs))
 
-        case 'DIV':
+        case "DIV":
             state.last_action.add_instruction(Divide(lhs, rhs))
 
+        case "SIN":
+            state.last_action.add_instruction(Sin(lhs, rhs))
+
+        case "COS":
+            state.last_action.add_instruction(Cos(lhs, rhs))
+
         case _:
-            state.panic(f'Unexpected error: {op} {arg1} {arg2}')
+            state.panic(f"Unexpected error: {op} {arg1} {arg2}")
```

### Comparing `aasm-0.0.9/aasm/parsing/op/message.py` & `aasm-0.1.0/aasm/parsing/op/message.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,50 @@
 from aasm.intermediate.message import Message
 from aasm.utils.validation import is_valid_name, print_invalid_names
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_MESSAGE(state: State, msg_type: str, msg_performative) -> None:
-    state.require(not state.in_message, 'Already inside a message.', 'First end current message using EMESSAGE.')
-    state.require(not state.in_agent, 'Cannot define messages inside agents.', 'First end current agent using EAGENT.')
-    state.require(not state.in_graph, 'Cannot define messages inside graphs.', 'First end current graph using EGRAPH.')
+def op_MESSAGE(state: State, msg_type: str, msg_performative: str) -> None:
     state.require(
-        not state.message_exists(msg_type, msg_performative), 
-        f'Message {msg_type}/{msg_performative} already exists in the current environment.'
+        not state.in_message,
+        "Already inside a message.",
+        "First end current message using EMESSAGE.",
     )
     state.require(
-        is_valid_name(msg_type), 
-        f'{msg_type} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.in_agent,
+        "Cannot define messages inside agents.",
+        "First end current agent using EAGENT.",
     )
     state.require(
-        is_valid_name(msg_performative), 
-        f'{msg_performative} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.in_graph,
+        "Cannot define messages inside graphs.",
+        "First end current graph using EGRAPH.",
     )
-    
+    state.require(
+        not state.message_exists(msg_type, msg_performative),
+        f"Message {msg_type}/{msg_performative} already exists in the current environment.",
+    )
+    state.require(
+        is_valid_name(msg_type),
+        f"{msg_type} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+    state.require(
+        is_valid_name(msg_performative),
+        f"{msg_performative} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+
     state.in_message = True
     state.add_message(Message(msg_type, msg_performative))
 
 
-def op_EMESSAGE(state: State) -> None:    
-    state.require(state.in_message, 'Not inside any message.', 'Try defining new messages using MESSAGE.')
-    
+def op_EMESSAGE(state: State) -> None:
+    state.require(
+        state.in_message,
+        "Not inside any message.",
+        "Try defining new messages using MESSAGE.",
+    )
+
     state.in_message = False
```

### Comparing `aasm-0.0.9/aasm/parsing/op/prm.py` & `aasm-0.1.0/aasm/parsing/op/prm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,144 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List
 
-from aasm.intermediate.agent import \
-    ConnectionListParam as AgentConnectionListParam
+from aasm.intermediate.agent import ConnectionListParam as AgentConnectionListParam
 from aasm.intermediate.agent import DistExpFloatParam as AgentDistExpFloatParam
-from aasm.intermediate.agent import \
-    DistNormalFloatParam as AgentDistNormalFloatParam
+from aasm.intermediate.agent import DistNormalFloatParam as AgentDistNormalFloatParam
+from aasm.intermediate.agent import DistUniformFloatParam as AgentDistUniformFloatParam
 from aasm.intermediate.agent import EnumParam as AgentEnumParam
+from aasm.intermediate.agent import FloatListParam as AgentFloatListParam
 from aasm.intermediate.agent import InitFloatParam as AgentInitFloatParam
 from aasm.intermediate.agent import MessageListParam as AgentMessageListParam
+from aasm.intermediate.agent import ModuleVariableParam as AgentModuleVariableParam
+from aasm.intermediate.message import ConnectionParam as MessageConnectionParam
 from aasm.intermediate.message import FloatParam as MessageFloatParam
-from aasm.utils.validation import (is_float, is_valid_enum_list, is_valid_name,
-                                   print_invalid_names)
+from aasm.intermediate.message import ModuleVariableParam as MessageModuleVariableParam
+from aasm.utils.validation import (
+    is_float,
+    is_valid_enum_list,
+    is_valid_name,
+    print_invalid_names,
+)
 
 if TYPE_CHECKING:
     from parsing.state import State
 
 
-def op_agent_PRM(state: State, name: str, category: str, args: List[str]) -> None:    
+def op_agent_PRM(state: State, name: str, category: str, args: List[str]) -> None:
     state.require(
-        state.in_agent, 
-        'Cannot define agent parameters outside agent scope.', 
-        'Try defining new agents using AGENT.'
+        state.in_agent,
+        "Cannot define agent parameters outside agent scope.",
+        "Try defining new agents using AGENT.",
     )
     state.require(
-        not state.in_behaviour, 
-        'Cannot define agent parameters inside a behaviour.', 
-        'Parameters must appear after AGENT.'
+        not state.in_behaviour,
+        "Cannot define agent parameters inside a behaviour.",
+        "Parameters must appear after AGENT.",
     )
-    state.require(not state.last_agent.name_exists(name), f'{name} already exists inside current agent.')
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        not state.last_agent.name_exists(name),
+        f"{name} already exists inside current agent.",
     )
-    
+    state.require(
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
+    )
+
     match category, args:
-        case 'float', [ 'init', value ]:
-            state.require(is_float(value), f'{value} is not a valid float.')
+        case "float", ["init", value]:
+            state.require(is_float(value), f"{value} is not a valid float.")
 
             state.last_agent.add_init_float(AgentInitFloatParam(name, value))
-            
-        case 'float', [ 'dist', 'normal', mean, std_dev ]:
-            state.require(is_float(mean), f'{mean} is not a valid float.')
-            state.require(is_float(std_dev), f'{std_dev} is not a valid float.')
-
-            state.last_agent.add_dist_normal_float(AgentDistNormalFloatParam(name, mean, std_dev))
-            
-        case 'float', [ 'dist', 'exp', lambda_ ]:
-            state.require(is_float(lambda_), f'{lambda_} is not a valid float.')
+
+        case "float", ["dist", "normal", mean, std_dev]:
+            state.require(is_float(mean), f"{mean} is not a valid float.")
+            state.require(is_float(std_dev), f"{std_dev} is not a valid float.")
             state.require(
-                float(lambda_) > 0, 
-                f'{lambda_} is not a valid lambda parameter.', 
-                'Lambda must be non-negative.'
+                float(std_dev) >= 0,
+                f"{std_dev} is not a valid standard deviation parameter.",
+                "Standard deviation must be non-negative.",
+            )
+
+            state.last_agent.add_dist_normal_float(
+                AgentDistNormalFloatParam(name, mean, std_dev)
+            )
+
+        case "float", ["dist", "exp", lambda_]:
+            state.require(is_float(lambda_), f"{lambda_} is not a valid float.")
+            state.require(
+                float(lambda_) > 0,
+                f"{lambda_} is not a valid lambda parameter.",
+                "Lambda must be positive.",
             )
 
             state.last_agent.add_dist_exp_float(AgentDistExpFloatParam(name, lambda_))
-            
-        case 'list', [ 'conn' ]:
+
+        case "float", ["dist", "uniform", a, b]:
+            state.require(is_float(a), f"{a} is not a valid float.")
+            state.require(is_float(b), f"{b} is not a valid float.")
+
+            state.last_agent.add_dist_uniform_float(
+                AgentDistUniformFloatParam(name, a, b)
+            )
+
+        case "list", ["conn"]:
             state.last_agent.add_connection_list(AgentConnectionListParam(name))
-            
-        case 'list', [ 'msg' ]:
+
+        case "list", ["msg"]:
             state.last_agent.add_message_list(AgentMessageListParam(name))
-            
-        case 'enum', enums:
+
+        case "list", ["float"]:
+            state.last_agent.add_float_list(AgentFloatListParam(name))
+
+        case "enum", enums:
             state.require(
                 is_valid_enum_list(enums),
-                f'{enums} is not a valid enum list.', 
-                'The correct pattern is [name, percent, ...], where percent(s) sum up to 100 (+/- 1).'
+                f"{enums} is not a valid enum list.",
+                "The correct pattern is [name, percent, ...], where percent(s) sum up to 100 (+/- 1).",
             )
 
             state.last_agent.add_enum(AgentEnumParam(name, enums))
-            
+
         case _:
-            state.panic(f'Incorrect operation: (agent) PRM {name} {category} {args}')
+            if category in state.get_module_types():
+                state.last_agent.add_module_variable(
+                    AgentModuleVariableParam(name, category)
+                )
+            else:
+                state.panic(
+                    f"Incorrect operation: (agent) PRM {name} {category} {args}"
+                )
 
 
-def op_message_PRM(state: State, name: str, category: str) -> None:    
+def op_message_PRM(state: State, name: str, category: str) -> None:
+    state.require(
+        state.in_message,
+        "Cannot define message parameters outside message scope.",
+        "Try defining new messages using MESSAGE.",
+    )
     state.require(
-        state.in_message, 
-        'Cannot define message parameters outside message scope.', 
-        'Try defining new messages using MESSAGE.'
+        not state.last_message.param_exists(name),
+        f"Parameter {name} already exists inside current message.",
     )
-    state.require(not state.last_message.param_exists(name), f'Parameter {name} already exists inside current message.')
     state.require(
-        is_valid_name(name), 
-        f'{name} is not a correct name.', 
-        f'Names can only contain alphanumeric signs, underscores and cannot be: {print_invalid_names()}.'
+        is_valid_name(name),
+        f"{name} is not a correct name.",
+        f"Names can only contain alphanumeric characters, underscores and cannot be: {print_invalid_names()}.",
     )
-    
+
     match category:
-        case 'float':
+        case "float":
             state.last_message.add_float(MessageFloatParam(name))
 
+        case "conn":
+            state.last_message.add_connection(MessageConnectionParam(name))
+
         case _:
-            state.panic(f'Incorrect operation: (message) PRM {name} {category}')
+            if category in state.get_module_types():
+                state.last_message.add_module_variable(
+                    MessageModuleVariableParam(name, category)
+                )
+            else:
+                state.panic(f"Incorrect operation: (message) PRM {name} {category}")
```

### Comparing `aasm-0.0.9/aasm/parsing/op/rand.py` & `aasm-0.1.0/aasm/parsing/op/rand.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,55 +7,57 @@
 from aasm.parsing.op.round import op_ROUND
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def op_RAND(state: State, arg1: str, arg2: str, arg3: str, args: List[str]) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'RAND can be used inside actions.')
+    state.require(
+        state.in_action, "Not inside any action.", f"RAND can be used inside actions."
+    )
     result = Argument(state, arg1)
 
     match arg3, args:
-        case 'uniform', [ a, b ]:
+        case "uniform", [a, b]:
             a_arg = Argument(state, a)
             b_arg = Argument(state, b)
             state.require(
-                result.random_number_generation_context(a_arg, b_arg), 
-                'Mismatched types in the random number generation context.', 
-                f'RESULT {result.explain()}, A {a_arg.explain()}, B {b_arg.explain()}'
+                result.random_number_generation_context(a_arg, b_arg),
+                "Mismatched types in the random number generation context.",
+                f"RESULT {result.explain()}, A {a_arg.explain()}, B {b_arg.explain()}",
             )
 
             state.last_action.add_instruction(UniformDist(result, a_arg, b_arg))
 
-        case 'normal', [ mean, std_dev ]:
+        case "normal", [mean, std_dev]:
             mean_arg = Argument(state, mean)
             std_dev_arg = Argument(state, std_dev)
             state.require(
-                result.random_number_generation_context(mean_arg, std_dev_arg), 
-                'Mismatched types in the random number generation context.', 
-                f'RESULT {result.explain()}, MEAN {mean_arg.explain()}, STD_DEV {std_dev_arg.explain()}'
+                result.random_number_generation_context(mean_arg, std_dev_arg),
+                "Mismatched types in the random number generation context.",
+                f"RESULT {result.explain()}, MEAN {mean_arg.explain()}, STD_DEV {std_dev_arg.explain()}",
             )
 
             state.last_action.add_instruction(NormalDist(result, mean_arg, std_dev_arg))
 
-        case 'exp', [ lambda_ ]:
+        case "exp", [lambda_]:
             lambda_arg = Argument(state, lambda_)
             state.require(
-                result.random_number_generation_context(lambda_arg), 
-                'Mismatched types in the random number generation context.', 
-                f'RESULT {result.explain()}, LAMBDA {lambda_arg.explain()}'
+                result.random_number_generation_context(lambda_arg),
+                "Mismatched types in the random number generation context.",
+                f"RESULT {result.explain()}, LAMBDA {lambda_arg.explain()}",
             )
 
             state.last_action.add_instruction(ExpDist(result, lambda_arg))
 
         case _:
-            state.panic(f'Incorrect operation: RAND {arg1} {arg2} {arg3} {args}')
+            state.panic(f"Incorrect operation: RAND {arg1} {arg2} {arg3} {args}")
 
     match arg2:
-        case 'float':
+        case "float":
             ...
 
-        case 'int':
+        case "int":
             op_ROUND(state, arg1)
 
         case _:
-            state.panic(f'Incorrect operation: RAND {arg1} {arg2} {arg3} {args}')
+            state.panic(f"Incorrect operation: RAND {arg1} {arg2} {arg3} {args}")
```

### Comparing `aasm-0.0.9/aasm/parsing/op/remen.py` & `aasm-0.1.0/aasm/parsing/op/subs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import RemoveNElements
+from aasm.intermediate.instruction import Subset
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_REMEN(state: State, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', 'List modifications can be used inside actions.')
-    lhs = Argument(state, arg1)
-    rhs = Argument(state, arg2)
+def op_SUBS(state: State, arg1: str, arg2: str, arg3: str) -> None:
     state.require(
-        lhs.list_n_removal_context(rhs), 
-        'Mismatched types in the list n removal context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
+        state.in_action, "Not inside any action.", f"SUBS can be used inside actions."
     )
-    
-    state.last_action.add_instruction(RemoveNElements(lhs, rhs))
+    dst_list = Argument(state, arg1)
+    src_list = Argument(state, arg2)
+    num = Argument(state, arg3)
+    state.require(
+        dst_list.list_subset_context(src_list, num),
+        "Mismatched types in the subset context.",
+        f"ARG1 {dst_list.explain()}, ARG2 {src_list.explain()}, ARG3 {num.explain()}",
+    )
+
+    state.last_action.add_instruction(Subset(dst_list, src_list, num))
```

### Comparing `aasm-0.0.9/aasm/parsing/op/round.py` & `aasm-0.1.0/aasm/parsing/op/round.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,12 +6,18 @@
 from aasm.intermediate.instruction import Round
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
 def op_ROUND(state: State, arg1: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'ROUND can be used inside actions.')
+    state.require(
+        state.in_action, "Not inside any action.", f"ROUND can be used inside actions."
+    )
     num = Argument(state, arg1)
-    state.require(num.round_number_context(), 'Mismatched type in the round number context.', f'NUM {num.explain()}')
+    state.require(
+        num.round_number_context(),
+        "Mismatched type in the round number context.",
+        f"NUM {num.explain()}",
+    )
 
     state.last_action.add_instruction(Round(num))
```

### Comparing `aasm-0.0.9/aasm/parsing/op/send.py` & `aasm-0.1.0/aasm/parsing/op/set.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from aasm.intermediate.action import SendMessageAction
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import Send
+from aasm.intermediate.instruction import Set
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_SEND(state: State, arg1: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', 'SEND can be used inside send_msg actions.')
+def op_SET(state: State, arg1: str, arg2: str) -> None:
     state.require(
-        isinstance(state.last_action, SendMessageAction), 
-        'Not inside send_msg action.', 
-        'SEND can be used inside send_msg actions.'
+        state.in_action, "Not inside any action.", f"SET can be used inside actions."
+    )
+    lhs = Argument(state, arg1)
+    rhs = Argument(state, arg2)
+    state.require(
+        lhs.assignment_context(rhs, state),
+        "Mismatched types in the assignment context.",
+        f"ARG1 {lhs.explain()}, ARG2 {rhs.explain()}",
     )
-    receivers = Argument(state, arg1)
-    state.require(receivers.send_context(), 'Mismatched type in the send context.', f'ARG1 {receivers.explain()}')
 
-    state.last_action.add_instruction(Send(receivers))
+    state.last_action.add_instruction(Set(lhs, rhs))
```

### Comparing `aasm-0.0.9/aasm/parsing/op/set.py` & `aasm-0.1.0/aasm/parsing/op/math_exp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import Set
+from aasm.intermediate.instruction import Logarithm, Power
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_SET(state: State, arg1: str, arg2: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'SET can be used inside actions.')
-    lhs = Argument(state, arg1)
-    rhs = Argument(state, arg2)
+def handle_math_exp_statement(
+    state: State, op: str, arg1: str, arg2: str, arg3: str
+) -> None:
     state.require(
-        lhs.assignment_context(rhs), 
-        'Mismatched types in the assignment context.', 
-        f'ARG1 {lhs.explain()}, ARG2 {rhs.explain()}'
-    )    
-    
-    state.last_action.add_instruction(Set(lhs, rhs))
+        state.in_action, "Not inside any action", f"{op} can be used inside actions."
+    )
+    dst = Argument(state, arg1)
+    base = Argument(state, arg2)
+    arg = Argument(state, arg3)
+    state.require(
+        dst.math_exponentiation_context(base, arg),
+        "Mismatched types in the math exponentiation statement.",
+        f"ARG1 {dst.explain()}, ARG2 {base.explain()}, ARG3 {arg.explain()}",
+    )
+
+    match op:
+        case "LOG":
+            state.last_action.add_instruction(Logarithm(dst, base, arg))
+
+        case "POW":
+            state.last_action.add_instruction(Power(dst, base, arg))
+
+        case _:
+            state.panic(f"Unexpected error: {op} {arg1} {arg2} {arg3}")
```

### Comparing `aasm-0.0.9/aasm/parsing/op/subs.py` & `aasm-0.1.0/aasm/parsing/op/lw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from aasm.intermediate.argument import Argument
-from aasm.intermediate.instruction import Subset
+from aasm.intermediate.instruction import ListWrite
 
 if TYPE_CHECKING:
     from aasm.parsing.state import State
 
 
-def op_SUBS(state: State, arg1: str, arg2: str, arg3: str) -> None:
-    state.require(state.in_action, 'Not inside any action.', f'SUBS can be used inside actions.')
-    dst_list = Argument(state, arg1)
-    src_list = Argument(state, arg2)
-    num = Argument(state, arg3)
+def op_LW(state: State, arg1: str, arg2: str, arg3: str) -> None:
     state.require(
-        dst_list.list_subset_context(src_list, num), 
-        'Mismatched types in the subset context.', 
-        f'ARG1 {dst_list.explain()}, ARG2 {src_list.explain()}, ARG3 {num.explain()}'
+        state.in_action, "Not inside any action.", "LW can be used inside actions."
     )
-    
-    state.last_action.add_instruction(Subset(dst_list, src_list, num))
+    list_ = Argument(state, arg1)
+    idx = Argument(state, arg2)
+    value = Argument(state, arg3)
+    state.require(
+        list_.list_write_context(idx, value),
+        "Mismatched types in the list write context.",
+        f"ARG1 {list_.explain()}, ARG2 {idx.explain()}, ARG3 {value.explain()}",
+    )
+
+    state.last_action.add_instruction(ListWrite(list_, idx, value))
```

### Comparing `aasm-0.0.9/aasm/parsing/parse.py` & `aasm-0.1.0/aasm/parsing/parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,129 +4,193 @@
 
 from aasm.parsing.op.action import op_ACTION, op_EACTION
 from aasm.parsing.op.agent import op_AGENT, op_EAGENT
 from aasm.parsing.op.behav import op_BEHAV, op_EBEHAV
 from aasm.parsing.op.clr import op_CLR
 from aasm.parsing.op.conditional import (
     handle_ordered_conditional_statement,
-    handle_unordered_conditional_statement)
+    handle_unordered_conditional_statement,
+)
 from aasm.parsing.op.decl import op_DECL
 from aasm.parsing.op.defg import op_DEFG
+from aasm.parsing.op.defnode import op_DEFNODE
 from aasm.parsing.op.eblock import op_EBLOCK
 from aasm.parsing.op.graph import op_EGRAPH, op_GRAPH
 from aasm.parsing.op.len import op_LEN
-from aasm.parsing.op.list import (handle_list_inclusion,
-                                  handle_list_modification)
+from aasm.parsing.op.list_inclusion import handle_list_inclusion
+from aasm.parsing.op.list_modification import handle_list_modification
+from aasm.parsing.op.logs import op_LOGS
+from aasm.parsing.op.lr import op_LR
+from aasm.parsing.op.lw import op_LW
 from aasm.parsing.op.math import handle_math_statement
+from aasm.parsing.op.math_exp import handle_math_exp_statement
+from aasm.parsing.op.math_mod import op_MOD
 from aasm.parsing.op.message import op_EMESSAGE, op_MESSAGE
 from aasm.parsing.op.prm import op_agent_PRM, op_message_PRM
 from aasm.parsing.op.rand import op_RAND
 from aasm.parsing.op.remen import op_REMEN
 from aasm.parsing.op.round import op_ROUND
+from aasm.parsing.op.scale import op_SCALE
 from aasm.parsing.op.send import op_SEND
 from aasm.parsing.op.set import op_SET
 from aasm.parsing.op.size import op_SIZE
+from aasm.parsing.op.mparams import op_MPARAMS
 from aasm.parsing.op.subs import op_SUBS
+from aasm.parsing.op.deftype import op_DEFTYPE
+from aasm.parsing.op.types import op_TYPES
+from aasm.parsing.op.module import op_MODULE
 from aasm.parsing.state import State
 
 if TYPE_CHECKING:
     from aasm.parsing.state import ParsedData
+    from aasm.modules.module import Module
 
 
-def parse_lines(lines: List[str], debug: bool) -> ParsedData:
-    state = State(lines, debug)
+def parse_lines(lines: List[str], debug: bool, modules: List[Module]) -> ParsedData:
+    state = State(lines, modules, debug)
     for tokens in state.tokens_from_lines():
-        match tokens:                                        
-            case [ 'AGENT', name ]:
+        match tokens:
+            case ["AGENT", name]:
                 op_AGENT(state, name)
-            
-            case [ 'EAGENT' ]:
+
+            case ["EAGENT"]:
                 op_EAGENT(state)
-                
-            case [ 'MESSAGE', name, performative ]:
+
+            case ["MESSAGE", name, performative]:
                 op_MESSAGE(state, name, performative)
-            
-            case [ 'EMESSAGE' ]:
+
+            case ["EMESSAGE"]:
                 op_EMESSAGE(state)
-                
-            case [ 'PRM', name, category ]:
+
+            case ["PRM", name, category]:
                 op_message_PRM(state, name, category)
-                
-            case [ 'PRM', name, category, *args ]:
+
+            case ["PRM", name, category, *args]:
                 op_agent_PRM(state, name, category, args)
-                
-            case [ 'BEHAV', name, category, *args ]:
+
+            case ["BEHAV", name, category, *args]:
                 op_BEHAV(state, name, category, args)
-                
-            case [ 'EBEHAV' ]:
+
+            case ["EBEHAV"]:
                 op_EBEHAV(state)
-                
-            case [ 'ACTION', name, category, *args ]:
+
+            case ["ACTION", name, category, *args]:
                 op_ACTION(state, name, category, args)
-                
-            case [ 'EACTION' ]:
+
+            case ["EACTION"]:
                 op_EACTION(state)
-                
-            case [ 'DECL', name, value ]:
-                op_DECL(state, name, value)
-                
-            case [ 'EBLOCK' ]:
+
+            case ["DECL", name, category, value]:
+                op_DECL(state, name, category, value)
+
+            case ["EBLOCK"]:
                 op_EBLOCK(state)
-                
-            case [ 'IEQ' | 'INEQ' | 'WEQ' | 'WNEQ' as op, arg1, arg2 ]:
+
+            case ["IEQ" | "INEQ" | "WEQ" | "WNEQ" as op, arg1, arg2]:
                 handle_unordered_conditional_statement(state, op, arg1, arg2)
-                
-            case [ 'IGT' | 'IGTEQ' | 'ILT' | 'ILTEQ' | 'WGT' | 'WGTEQ' | 'WLT' | 'WLTEQ' as op, arg1, arg2 ]:
+
+            case [
+                "IGT"
+                | "IGTEQ"
+                | "ILT"
+                | "ILTEQ"
+                | "WGT"
+                | "WGTEQ"
+                | "WLT"
+                | "WLTEQ" as op,
+                arg1,
+                arg2,
+            ]:
                 handle_ordered_conditional_statement(state, op, arg1, arg2)
-                
-            case [ 'ADD' | 'SUBT' | 'MULT' | 'DIV' as op, arg1, arg2 ]:
+
+            case ["ADD" | "SUBT" | "MULT" | "DIV" | "SIN" | "COS" as op, arg1, arg2]:
                 handle_math_statement(state, op, arg1, arg2)
-                
-            case [ 'ADDE' | 'REME' as op, list_, element ]:
+
+            case ["LOG" | "POW" as op, arg1, arg2, arg3]:
+                handle_math_exp_statement(state, op, arg1, arg2, arg3)
+
+            case ["MOD", dst, dividend, divisor]:
+                op_MOD(state, dst, dividend, divisor)
+
+            case ["ADDE" | "REME" as op, list_, element]:
                 handle_list_modification(state, op, list_, element)
-                
-            case [ 'LEN', result, list_ ]:
+
+            case ["LEN", result, list_]:
                 op_LEN(state, result, list_)
-                
-            case [ 'CLR', list_ ]:
+
+            case ["CLR", list_]:
                 op_CLR(state, list_)
-                
-            case [ 'IN' | 'NIN' as op, list_, element ]:
+
+            case ["IN" | "NIN" as op, list_, element]:
                 handle_list_inclusion(state, op, list_, element)
-                
-            case [ 'SEND', rcv_list ]:
+
+            case ["SEND", rcv_list]:
                 op_SEND(state, rcv_list)
-                
-            case [ 'SUBS', dst_list, src_list, num ]:
+
+            case ["SUBS", dst_list, src_list, num]:
                 op_SUBS(state, dst_list, src_list, num)
-                
-            case [ 'SET', arg1, arg2 ]:
+
+            case ["SET", arg1, arg2]:
                 op_SET(state, arg1, arg2)
-                
-            case [ 'REMEN', list_, num ]:
+
+            case ["REMEN", list_, num]:
                 op_REMEN(state, list_, num)
 
-            case [ 'RAND', result, cast_to, dist, *args ]:
+            case ["RAND", result, cast_to, dist, *args]:
                 op_RAND(state, result, cast_to, dist, args)
 
-            case [ 'ROUND', num ]:
+            case ["ROUND", num]:
                 op_ROUND(state, num)
-                
-            case [ 'SET', arg1, arg2 ]:
+
+            case ["SET", arg1, arg2]:
                 op_SET(state, arg1, arg2)
 
-            case [ 'GRAPH', category ]:
+            case ["GRAPH", category]:
                 op_GRAPH(state, category)
 
-            case [ 'EGRAPH' ]:
+            case ["EGRAPH"]:
                 op_EGRAPH(state)
 
-            case [ 'SIZE', size ]:
+            case ["SIZE", size]:
                 op_SIZE(state, size)
 
-            case [ 'DEFG',  agent_name, amount, *args ]:
+            case ["SCALE", scale]:
+                op_SCALE(state, scale)
+
+            case ["MPARAMS", m0, m_inc]:
+                op_MPARAMS(state, m0, m_inc)
+
+            case ["DEFG", agent_name, amount, *args]:
                 op_DEFG(state, agent_name, amount, args)
-                
-            case _:
-                state.panic(f'Unknown tokens: {tokens}')
+
+            case ["DEFNODE", agent_name, row]:
+                op_DEFNODE(state, agent_name, row)
+
+            case ["DEFTYPE", agent_type, amount, *args]:
+                op_DEFTYPE(state, agent_type, amount, args)
+
+            case ["TYPES", amount]:
+                op_TYPES(state, amount)
+
+            case ["LR", dst, list_, idx]:
+                op_LR(state, dst, list_, idx)
+
+            case ["LW", list_, idx, value]:
+                op_LW(state, list_, idx, value)
+
+            case ["LOGS", level, *args]:
+                op_LOGS(state, level, args)
+
+            case ["MODULE", name]:
+                op_MODULE(state, name)
+
+            case [OPCODE, *args]:
+                found = False
+                for module in state.loaded_modules:
+                    for instruction in module.instructions:
+                        if instruction.opcode == OPCODE:
+                            found = True
+                            instruction.op(state, args)
+                if not found:
+                    state.panic(f"Unknown tokens: {tokens}")
 
     return state.get_parsed_data()
```

