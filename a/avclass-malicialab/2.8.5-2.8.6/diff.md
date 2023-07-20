# Comparing `tmp/avclass-malicialab-2.8.5.tar.gz` & `tmp/avclass-malicialab-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.8.5.tar", last modified: Thu Jul 20 10:21:55 2023, max compression
+gzip compressed data, was "avclass-malicialab-2.8.6.tar", last modified: Thu Jul 20 13:14:13 2023, max compression
```

## Comparing `avclass-malicialab-2.8.5.tar` & `avclass-malicialab-2.8.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.5/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.5/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.5/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.5/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.5/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.5/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-07-20 10:20:10.000000 avclass-malicialab-2.8.5/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    56679 2023-07-20 10:20:10.000000 avclass-malicialab-2.8.5/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    41528 2023-07-20 10:20:10.000000 avclass-malicialab-2.8.5/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.5/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.5/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.5/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.5/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.5/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-20 10:21:55.000000 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-07-20 10:21:55.000000 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-07-20 10:21:55.000000 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-07-20 10:21:55.000000 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-07-20 10:21:55.000000 avclass-malicialab-2.8.5/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-07-20 10:21:21.000000 avclass-malicialab-2.8.5/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-07-20 10:21:55.885351 avclass-malicialab-2.8.5/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 13:14:13.035529 avclass-malicialab-2.8.6/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.6/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.6/MANIFEST.in
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-20 13:14:13.035529 avclass-malicialab-2.8.6/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.6/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 13:14:13.031529 avclass-malicialab-2.8.6/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.6/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.6/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 13:14:13.031529 avclass-malicialab-2.8.6/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.6/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-07-20 10:20:10.000000 avclass-malicialab-2.8.6/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56730 2023-07-20 13:12:59.000000 avclass-malicialab-2.8.6/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41678 2023-07-20 13:12:59.000000 avclass-malicialab-2.8.6/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.6/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.6/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.6/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.6/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.6/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-20 13:14:13.035529 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-20 13:14:13.000000 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-07-20 13:14:13.000000 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-07-20 13:14:13.000000 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-07-20 13:14:13.000000 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-07-20 13:14:13.000000 avclass-malicialab-2.8.6/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-07-20 13:13:46.000000 avclass-malicialab-2.8.6/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-07-20 13:14:13.035529 avclass-malicialab-2.8.6/setup.cfg
```

### Comparing `avclass-malicialab-2.8.5/LICENSE` & `avclass-malicialab-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/PKG-INFO` & `avclass-malicialab-2.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.5
+Version: 2.8.6
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.5/README.md` & `avclass-malicialab-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/common.py` & `avclass-malicialab-2.8.6/avclass/common.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/data/andropup.expansion` & `avclass-malicialab-2.8.6/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/data/default.tagging` & `avclass-malicialab-2.8.6/avclass/data/default.tagging`

 * *Files 0% similar despite different names*

```diff
@@ -1264,14 +1264,15 @@
 helldoor	hilldoor
 hello	helloxd
 hellocrypt	helloxd
 hellokitty	deathransom
 hellospy	spyoo
 helygula	flacher
 helygulad	flacher
+heodo	emotet
 hidcobra	nukesped
 hiddenad	hiddad
 hiddenads	hiddad
 hiddenbee	occamy
 hiddencobra	nukesped
 hiddeninstall	jsmshider
 hiddenroutine	strongvault
@@ -2760,14 +2761,15 @@
 temr	vobfus
 tenpast	10past
 tenpastthree	10past
 tepely	onlinegames
 tepfer	fareit
 termserv	termsrvpatch
 tescrypt	teslacrypt
+tesla	agenttesla
 test	testvirus
 testfile	testvirus
 testsample	testvirus
 texel	luder
 thancrypt	thanatos
 themas	careto
 thiefquest	evilquest
@@ -2830,14 +2832,15 @@
 treasurehunt	treasurehunter
 treemz	onlinegames
 trick	trickbot
 trickbotcrypt	trickbot
 trickbotmodule	trickbot
 trickbt	trickbot
 trickler	gator
+trickloader	trickbot
 trickpak	trickbot
 trickster	trickbot
 trickybot	trickbot
 trik	phorpiex
 triosir	trioris
 triplicate	tristate
 triusor	resur
```

### Comparing `avclass-malicialab-2.8.5/avclass/data/default.taxonomy` & `avclass-malicialab-2.8.6/avclass/data/default.taxonomy`

 * *Files 0% similar despite different names*

```diff
@@ -1149,14 +1149,15 @@
 FAM:gt32supportgeeks
 FAM:gtbot
 FAM:guard
 FAM:gudex
 FAM:guerrilla
 FAM:gugi
 FAM:guildma
+FAM:guloader
 FAM:gumen
 FAM:gupay
 FAM:gustuff
 FAM:gysad
 FAM:habitsrat
 FAM:hacdef
 FAM:hackback
@@ -1266,14 +1267,15 @@
 FAM:inmobi
 FAM:innovativesolutions
 FAM:inor
 FAM:inservice
 FAM:installbrain
 FAM:installcore
 FAM:installerex
+FAM:installermonetizer
 FAM:installiq
 FAM:installmetrix
 FAM:installmiez
 FAM:installmonetizer
 FAM:installmonster
 FAM:instally
 FAM:interception
@@ -1878,14 +1880,15 @@
 FAM:pasma
 FAM:pasnaino
 FAM:passcv
 FAM:passma
 FAM:passview
 FAM:pasur
 FAM:patacore
+FAM:patchupplus
 FAM:pay2key
 FAM:paycall
 FAM:pbot
 FAM:pcacceleratepro
 FAM:pccleaner
 FAM:pccleaners
 FAM:pcclient
@@ -1899,14 +1902,15 @@
 FAM:penguin
 FAM:pennybee
 FAM:pepperat
 FAM:perfectoptimizer
 FAM:perflogger
 FAM:perion
 FAM:perkel
+FAM:perkiler
 FAM:persirai
 FAM:petrolin
 FAM:petya
 FAM:phantomlance
 FAM:phantomnet
 FAM:phdet
 FAM:philadelphia
@@ -2324,14 +2328,15 @@
 FAM:skplanet
 FAM:skygofree
 FAM:skymobi
 FAM:skyrat
 FAM:slenfbot
 FAM:slic
 FAM:slickshoes
+FAM:slimdrivers
 FAM:slimware
 FAM:slingshot
 FAM:slisp
 FAM:sliver
 FAM:sload
 FAM:slocker
 FAM:slothfulmedia
@@ -3098,14 +3103,15 @@
 GEN:deepscan
 GEN:detection
 GEN:eheur
 GEN:encodefeature
 GEN:error
 GEN:file
 GEN:filerepmalware
+GEN:found
 GEN:gen
 GEN:gena
 GEN:generic
 GEN:generica
 GEN:generickd
 GEN:genericml
 GEN:genericr
@@ -3143,14 +3149,15 @@
 GEN:hack
 GEN:heur
 GEN:heuristic
 GEN:high
 GEN:highconfidence
 GEN:igeneric
 GEN:kcloud
+GEN:load
 GEN:lookslike
 GEN:malagent
 GEN:malcode
 GEN:maldroid
 GEN:malicious
 GEN:maltrec
 GEN:malware
@@ -3167,15 +3174,18 @@
 GEN:password
 GEN:posible
 GEN:possible
 GEN:possiblemalware
 GEN:possiblethreat
 GEN:probably
 GEN:program
+GEN:protect
+GEN:remote
 GEN:reputation
+GEN:sample
 GEN:sape
 GEN:score
 GEN:securityrisk
 GEN:siggen
 GEN:singleton
 GEN:software
 GEN:sonar
@@ -3188,14 +3198,15 @@
 GEN:suspicious
 GEN:symvt
 GEN:systemhijack
 GEN:threat
 GEN:trojan
 GEN:tscope
 GEN:tsgeneric
+GEN:unavailable
 GEN:unclassified
 GEN:unclassifiedmalware
 GEN:undef
 GEN:undefined
 GEN:unknown
 GEN:variant
 GEN:website
```

### Comparing `avclass-malicialab-2.8.5/avclass/evaluate.py` & `avclass-malicialab-2.8.6/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/labeler.py` & `avclass-malicialab-2.8.6/avclass/labeler.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/misp.py` & `avclass-malicialab-2.8.6/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/normalize.py` & `avclass-malicialab-2.8.6/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass/update.py` & `avclass-malicialab-2.8.6/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.5/avclass_malicialab.egg-info/PKG-INFO` & `avclass-malicialab-2.8.6/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.5
+Version: 2.8.6
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.5/pyproject.toml` & `avclass-malicialab-2.8.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.8.5"
+version = "2.8.6"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

