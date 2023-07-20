# Comparing `tmp/cadence_detector-0.2.2.tar.gz` & `tmp/cadence_detector-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadence_detector-0.2.2.tar", last modified: Tue Jul 18 05:27:49 2023, max compression
+gzip compressed data, was "cadence_detector-0.2.3.tar", last modified: Thu Jul 20 16:21:18 2023, max compression
```

## Comparing `cadence_detector-0.2.2.tar` & `cadence_detector-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.269268 cadence_detector-0.2.2/
--rw-r--r--   0 matanba  (223682273) 418804322     1058 2023-04-18 10:24:48.000000 cadence_detector-0.2.2/LICENSE
--rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-07-18 05:27:49.268772 cadence_detector-0.2.2/PKG-INFO
--rw-r--r--   0 matanba  (223682273) 418804322      672 2023-04-22 15:45:43.000000 cadence_detector-0.2.2/README.md
--rw-r--r--   0 matanba  (223682273) 418804322      704 2023-07-18 05:27:25.000000 cadence_detector-0.2.2/pyproject.toml
--rw-r--r--   0 matanba  (223682273) 418804322       38 2023-07-18 05:27:49.269394 cadence_detector-0.2.2/setup.cfg
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.220396 cadence_detector-0.2.2/src/
--rw-r--r--   0 matanba  (223682273) 418804322        0 2023-04-22 08:05:31.000000 cadence_detector-0.2.2/src/__init__.py
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.225490 cadence_detector-0.2.2/src/cadence_detector/
--rw-r--r--   0 matanba  (223682273) 418804322     1654 2023-07-10 18:21:33.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetectData.py
--rw-r--r--   0 matanba  (223682273) 418804322    61394 2023-07-17 14:52:20.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetectStateMachine.py
--rw-r--r--   0 matanba  (223682273) 418804322    64926 2023-07-18 05:25:02.000000 cadence_detector-0.2.2/src/cadence_detector/CadenceDetector.py
--rw-r--r--   0 matanba  (223682273) 418804322        1 2023-04-22 08:31:36.000000 cadence_detector-0.2.2/src/cadence_detector/__init__.py
--rw-r--r--   0 matanba  (223682273) 418804322     2277 2023-04-22 14:52:32.000000 cadence_detector-0.2.2/src/cadence_detector/cadence_detector.py
-drwxr-xr-x   0 matanba  (223682273) 418804322        0 2023-07-18 05:27:49.268166 cadence_detector-0.2.2/src/cadence_detector.egg-info/
--rw-r--r--   0 matanba  (223682273) 418804322     1233 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/PKG-INFO
--rw-r--r--   0 matanba  (223682273) 418804322      473 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/SOURCES.txt
--rw-r--r--   0 matanba  (223682273) 418804322        1 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/dependency_links.txt
--rw-r--r--   0 matanba  (223682273) 418804322       26 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/requires.txt
--rw-r--r--   0 matanba  (223682273) 418804322       26 2023-07-18 05:27:49.000000 cadence_detector-0.2.2/src/cadence_detector.egg-info/top_level.txt
+drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-07-20 16:21:18.353209 cadence_detector-0.2.3/
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1058 2023-04-18 10:24:48.000000 cadence_detector-0.2.3/LICENSE
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1233 2023-07-20 16:21:18.352796 cadence_detector-0.2.3/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      672 2023-04-22 15:45:43.000000 cadence_detector-0.2.3/README.md
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      704 2023-07-20 16:20:50.000000 cadence_detector-0.2.3/pyproject.toml
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       38 2023-07-20 16:21:18.353317 cadence_detector-0.2.3/setup.cfg
+drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-07-20 16:21:18.345542 cadence_detector-0.2.3/src/
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-04-22 08:05:31.000000 cadence_detector-0.2.3/src/__init__.py
+drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-07-20 16:21:18.348729 cadence_detector-0.2.3/src/cadence_detector/
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1654 2023-07-10 18:21:33.000000 cadence_detector-0.2.3/src/cadence_detector/CadenceDetectData.py
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)    62219 2023-07-20 15:48:52.000000 cadence_detector-0.2.3/src/cadence_detector/CadenceDetectStateMachine.py
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)    64926 2023-07-20 15:30:45.000000 cadence_detector-0.2.3/src/cadence_detector/CadenceDetector.py
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        1 2023-04-22 08:31:36.000000 cadence_detector-0.2.3/src/cadence_detector/__init__.py
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     2277 2023-04-22 14:52:32.000000 cadence_detector-0.2.3/src/cadence_detector/cadence_detector.py
+drwxr-xr-x   0 matanba  (223682273) WAVES\Domain Users (418804322)        0 2023-07-20 16:21:18.352290 cadence_detector-0.2.3/src/cadence_detector.egg-info/
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)     1233 2023-07-20 16:21:18.000000 cadence_detector-0.2.3/src/cadence_detector.egg-info/PKG-INFO
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)      473 2023-07-20 16:21:18.000000 cadence_detector-0.2.3/src/cadence_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)        1 2023-07-20 16:21:18.000000 cadence_detector-0.2.3/src/cadence_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       26 2023-07-20 16:21:18.000000 cadence_detector-0.2.3/src/cadence_detector.egg-info/requires.txt
+-rw-r--r--   0 matanba  (223682273) WAVES\Domain Users (418804322)       26 2023-07-20 16:21:18.000000 cadence_detector-0.2.3/src/cadence_detector.egg-info/top_level.txt
```

### Comparing `cadence_detector-0.2.2/LICENSE` & `cadence_detector-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.2/PKG-INFO` & `cadence_detector-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence_detector
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadence_detector-0.2.2/README.md` & `cadence_detector-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.2/pyproject.toml` & `cadence_detector-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cadence_detector"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Matan Ben-Asher", email="mbenasher@yahoo.com" },
 ]
 description = "A python package for cadence detection"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cadence_detector-0.2.2/src/cadence_detector/CadenceDetectData.py` & `cadence_detector-0.2.3/src/cadence_detector/CadenceDetectData.py`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.2/src/cadence_detector/CadenceDetectStateMachine.py` & `cadence_detector-0.2.3/src/cadence_detector/CadenceDetectStateMachine.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,14 +336,31 @@
                     retVal = 0
                     break
         return retVal
 
     def verifyHCHarmony(self, HarmonicState):
         return self.isVMajorExclusive(HarmonicState)
 
+    def isTonicHarmony(self, HarmonicState):
+        retVal = 1
+        IpitchClass = self.CurrHarmonicState.Key.tonic.pitchClass
+        if HarmonicState.Key.mode == 'major':
+            # major triad
+            tonic_triad_offsets = [0, 4, 7]
+        else:
+            # minor triad
+            tonic_triad_offsets = [0, 3, 7]
+        IchordPitchClass = [(IpitchClass + mto) % 12 for mto in tonic_triad_offsets]
+        if not HarmonicState.Chord.isRest:
+            for p in HarmonicState.Chord.pitches:
+                if p.pitchClass not in IchordPitchClass:
+                    retVal = 0
+                    break
+        return retVal
+
     def isUnison(self):
         retVal = 1
         Pitch0 = self.CurrHarmonicState.Chord.pitches[0].pitchClass
         for p in self.CurrHarmonicState.Chord.pitches:
             if p.pitchClass != Pitch0:
                 retVal = 0
                 break
@@ -570,15 +587,17 @@
                             self.tryGetBeatStrength() < 1.0 and\
                             self.verifyHCGrouping(self.CurrHarmonicState) and\
                             self.verifyHCHarmony(self.CurrHarmonicState) and\
                             self.verifySopranoVoiceLeading(cadence_type='HC'):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                     elif self.isTonicBass():
                         # harmony  - chordal inversion
-                        if (self.CurrHarmonicState.ChordInversion == CDHarmonicChordInversions.Root.value or self.isRootedHarmony()) and\
+                        if (self.CurrHarmonicState.ChordInversion == CDHarmonicChordInversions.Root.value or
+                            self.isRootedHarmony() or
+                            self.isTonicHarmony(HarmonicState=self.CurrHarmonicState)) and\
                                 self.verifyPACGrouping(HarmonicState=self.CurrHarmonicState):
                             # ==I after V after IV or II6, cadential arrival
                             # melody  - soprano degree
                             if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC'):
                                 if curr_state==CDCadentialStates.CadInevitable:
                                     curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
                                 elif self.verifySopranoVoiceLeading(cadence_type='IAC') and self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
@@ -678,15 +697,15 @@
                             self.verifySopranoVoiceLeading(cadence_type='HC'):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.HCArrival, curr_state)
                     elif self.isI64(self.CurrHarmonicState):  # I64 can be HC appoggiaturra on dominant bass
                         curr_state = CDCadentialStates.HCArrivalExpected
                     else:
                         curr_state = CDCadentialStates.CadInevitable
                 elif self.isTonicBass() and\
-                        self.CurrHarmonicState.Chord.isConsonant() and\
+                        (self.CurrHarmonicState.Chord.isConsonant() or self.isTonicHarmony(HarmonicState=self.CurrHarmonicState)) and\
                         not self.harmonyContainsPitchDegree(HarmonicState=self.CurrHarmonicState, degree=6):
                     if self.isSopranoOnDegree(1) and self.verifySopranoVoiceLeading(cadence_type='PAC') and\
                             (not self.IsChallenger or self.verifyPACGrouping(self.CurrHarmonicState)):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.PACArrival, curr_state)
                     elif self.isSopranoOnDegree([3, 5]) and self.verifySopranoVoiceLeading(cadence_type='IAC') and\
                             self.verifyIACGrouping(HarmonicState=self.CurrHarmonicState):
                         curr_state = self.setCadenceOrPostCadence(CDCadentialStates.IACArrival, curr_state)
```

### Comparing `cadence_detector-0.2.2/src/cadence_detector/CadenceDetector.py` & `cadence_detector-0.2.3/src/cadence_detector/CadenceDetector.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,15 +668,15 @@
         # loop on measures:
         try:
             # for debugging a measure range
             # range_with_holes = itertools.chain(range(0, 4), range(70, 84))
             # for currMeasureIndex in range_with_holes:
             for currMeasureIndex in range(0,self.NumMeasures):
                 # debug per measure
-                if currMeasureIndex == 79:
+                if currMeasureIndex == 15:
                     bla = 0
                 # true measures start with 1, pickups will start from zero, but not all corpora will abide to this
                 # for example, data that originates from midi cannot contain this info
                 # to overcome this, we attempt to find the pickup via initial rests and discard it
                 # also, we count the empty measures and index them out while writing the label
                 measure_number = currMeasureIndex + 1
                 # print(f"measure number {measure_number}")
```

### Comparing `cadence_detector-0.2.2/src/cadence_detector/cadence_detector.py` & `cadence_detector-0.2.3/src/cadence_detector/cadence_detector.py`

 * *Files identical despite different names*

### Comparing `cadence_detector-0.2.2/src/cadence_detector.egg-info/PKG-INFO` & `cadence_detector-0.2.3/src/cadence_detector.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadence-detector
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for cadence detection
 Author-email: Matan Ben-Asher <mbenasher@yahoo.com>
 Project-URL: Homepage, https://github.com/MusicalStateMachines/CadenceDetector
 Project-URL: Bug Tracker, https://github.com/MusicalStateMachines/CadenceDetector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

