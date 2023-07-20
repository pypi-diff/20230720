# Comparing `tmp/stable-ts-2.7.0.tar.gz` & `tmp/stable-ts-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.7.0.tar", last modified: Thu Jul 13 00:56:15 2023, max compression
+gzip compressed data, was "stable-ts-2.7.1.tar", last modified: Thu Jul 20 19:58:11 2023, max compression
```

## Comparing `stable-ts-2.7.0.tar` & `stable-ts-2.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.247666 stable-ts-2.7.0/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.0/LICENSE
--rw-rw-rw-   0        0        0    11472 2023-07-13 00:56:15.246663 stable-ts-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    11176 2023-07-13 00:51:01.000000 stable-ts-2.7.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 00:56:15.247666 stable-ts-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.226222 stable-ts-2.7.0/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11472 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-07-13 00:56:15.000000 stable-ts-2.7.0/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.244670 stable-ts-2.7.0/stable_whisper/
--rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-09 22:10:17.000000 stable-ts-2.7.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.0/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.0/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.0/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    42984 2023-07-13 00:51:01.000000 stable-ts-2.7.0/stable_whisper/result.py
--rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.0/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.0/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.805999 stable-ts-2.7.1/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.1/LICENSE
+-rw-rw-rw-   0        0        0    11472 2023-07-20 19:58:11.804998 stable-ts-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11176 2023-07-20 19:47:30.000000 stable-ts-2.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:58:11.807000 stable-ts-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.731932 stable-ts-2.7.1/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11472 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-20 19:58:11.000000 stable-ts-2.7.1/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 19:58:11.802997 stable-ts-2.7.1/stable_whisper/
+-rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.1/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.1/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-20 19:40:56.000000 stable-ts-2.7.1/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.1/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.1/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.1/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.1/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.1/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    43551 2023-07-20 19:56:22.000000 stable-ts-2.7.1/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.1/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.1/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.1/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.1/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.1/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.7.0/LICENSE` & `stable-ts-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/PKG-INFO` & `stable-ts-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.7.0
+Version: 2.7.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -143,22 +143,22 @@
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.0/README.md` & `stable-ts-2.7.1/stable_ts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: stable-ts
+Version: 2.7.1
+Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
+Home-page: https://github.com/jianfch/stable-ts
+Author: Jian
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Stabilizing Timestamps for Whisper
 
 This script modifies [OpenAI's Whisper](https://github.com/openai/whisper) to produce more reliable timestamps.
 
 https://user-images.githubusercontent.com/28970749/225826345-ef7115db-51e4-4b23-aedd-069389b8ae43.mp4
 
 * [Setup](#setup)
@@ -132,22 +143,22 @@
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -162,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.0/setup.py` & `stable-ts-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: stable-ts
-Version: 2.7.0
-Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
-Home-page: https://github.com/jianfch/stable-ts
-Author: Jian
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Stabilizing Timestamps for Whisper
 
 This script modifies [OpenAI's Whisper](https://github.com/openai/whisper) to produce more reliable timestamps.
 
 https://user-images.githubusercontent.com/28970749/225826345-ef7115db-51e4-4b23-aedd-069389b8ae43.mp4
 
 * [Setup](#setup)
@@ -143,22 +132,22 @@
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +162,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.0/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.7.1/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/audio.py` & `stable-ts-2.7.1/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/decode.py` & `stable-ts-2.7.1/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/enhancement.py` & `stable-ts-2.7.1/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/non_whisper.py` & `stable-ts-2.7.1/stable_whisper/non_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/quantization.py` & `stable-ts-2.7.1/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/result.py` & `stable-ts-2.7.1/stable_whisper/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,27 @@
         suppress_silence(self, silent_starts, silent_ends, min_word_dur)
         return self
 
     def rescale_time(self, scale_factor: float):
         self.start = round(self.start * scale_factor, 3)
         self.end = round(self.end * scale_factor, 3)
 
-    def clamp_max(self, max_dur: float, clip_start: bool = False):
+    def clamp_max(self, max_dur: float, clip_start: bool = False, verbose: bool = False):
         if self.duration > max_dur:
             if clip_start:
-                self.start = round(self.end - max_dur, 3)
+                new_start = round(self.end - max_dur, 3)
+                if verbose:
+                    print(f'Start: {self.start} -> {new_start}\nEnd: {self.end}\nText:"{self.word}"\n')
+                self.start = new_start
+
             else:
-                self.end = round(self.start + max_dur, 3)
+                new_end = round(self.start + max_dur, 3)
+                if verbose:
+                    print(f'Start: {self.start}\nEnd: {self.end} -> {new_end}\nText:"{self.word}"\n')
+                self.end = new_end
 
 
 @dataclass
 class Segment:
     start: float
     end: float
     text: str
@@ -807,58 +814,64 @@
 
         """
         if force_len:
             self.merge_all_segments()
         self._split_segments(lambda x: x.get_length_indices(max_chars=max_chars, max_words=max_words), lock=lock)
         return self
 
-    def clamp_max(self, medium_factor: float = 2.5, max_dur: float = None, clip_start: bool = None):
+    def clamp_max(
+            self,
+            medium_factor: float = 2.5,
+            max_dur: float = None,
+            clip_start: bool = None,
+            verbose: bool = True):
         """
 
         Clamp all word durations above certain value.
 
         Parameters
         ----------
         medium_factor: float
             Clamp durations above ([medium_factor] * medium duration) per segment. (Default: 2.5)
             If [medium_factor]=None/0 or segment has less than 3 words, it will be ignored and use only [max_dur].
         max_dur: float
             Clamp durations above [max_dur]. (Default: None)
         clip_start: bool
             Whether to clamp the start of a word. (Default: None)
             Default only clamps the start of first word and end of last word per segment.
+        verbose: bool
+            Whether to print out the timestamp changes. (Default: False)
 
         """
         if not (medium_factor or max_dur):
             raise ValueError('At least one of following arguments requires non-zero value: medium_factor; max_dur')
 
         if not self.has_words:
             warnings.warn('Cannot clamp due to missing/no word-timestamps')
             return self
 
         for seg in self.segments:
             curr_max_dur = None
             if medium_factor and len(seg.words) > 2:
                 durations = np.array([word.duration for word in seg.words])
-                print(durations)
                 durations.sort()
                 curr_max_dur = medium_factor * durations[len(durations)//2 + 1]
 
             if max_dur and (not curr_max_dur or curr_max_dur > max_dur):
                 curr_max_dur = max_dur
 
             if not curr_max_dur:
                 continue
 
             if clip_start is None:
-                seg.words[0].clamp_max(curr_max_dur, clip_start=True)
-                seg.words[-1].clamp_max(curr_max_dur, clip_start=False)
+                seg.words[0].clamp_max(curr_max_dur, clip_start=True, verbose=verbose)
+                seg.words[-1].clamp_max(curr_max_dur, clip_start=False, verbose=verbose)
             else:
                 for i, word in enumerate(seg.words):
-                    word.clamp_max(curr_max_dur, clip_start=clip_start)
+                    word.clamp_max(curr_max_dur, clip_start=clip_start, verbose=verbose)
 
             seg.update_seg_with_words()
 
         return self
 
     def regroup(self, regroup_algo: str = None, verbose: bool = False, only_show: bool = False):
         """
```

### Comparing `stable-ts-2.7.0/stable_whisper/stabilization.py` & `stable-ts-2.7.1/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/text_output.py` & `stable-ts-2.7.1/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/timing.py` & `stable-ts-2.7.1/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/video_output.py` & `stable-ts-2.7.1/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.0/stable_whisper/whisper_word_level.py` & `stable-ts-2.7.1/stable_whisper/whisper_word_level.py`

 * *Files identical despite different names*

