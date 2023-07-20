# Comparing `tmp/BuoyanText-0.0.4.tar.gz` & `tmp/BuoyanText-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BuoyanText-0.0.4.tar", last modified: Thu Jul 20 08:40:11 2023, max compression
+gzip compressed data, was "BuoyanText-0.0.5.tar", last modified: Thu Jul 20 10:43:33 2023, max compression
```

## Comparing `BuoyanText-0.0.4.tar` & `BuoyanText-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:40:11.901380 BuoyanText-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-19 08:58:37.000000 BuoyanText-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2089 2023-07-20 08:40:11.901380 BuoyanText-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2023-07-20 07:46:33.000000 BuoyanText-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 08:40:11.901380 BuoyanText-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-07-20 08:39:57.000000 BuoyanText-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:40:11.890203 BuoyanText-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:40:11.894796 BuoyanText-0.0.4/src/BuoyanText/
--rw-rw-rw-   0        0        0     8611 2023-07-20 08:38:03.000000 BuoyanText-0.0.4/src/BuoyanText/ByTextNorm.py
--rw-rw-rw-   0        0        0     3300 2023-07-19 10:04:46.000000 BuoyanText-0.0.4/src/BuoyanText/ByTextReader.py
--rw-rw-rw-   0        0        0        0 2023-07-20 08:37:50.000000 BuoyanText-0.0.4/src/BuoyanText/__init__.py
--rw-rw-rw-   0        0        0     3321 2023-07-19 15:19:56.000000 BuoyanText-0.0.4/src/BuoyanText/contractions_English.json
--rw-rw-rw-   0        0        0      144 2023-07-11 03:00:16.000000 BuoyanText-0.0.4/src/BuoyanText/punctuation_Chinese.json
--rw-rw-rw-   0        0        0    22250 2023-07-19 15:19:56.000000 BuoyanText-0.0.4/src/BuoyanText/stopwords_Chinese.json
--rw-rw-rw-   0        0        0     2013 2023-07-19 15:19:56.000000 BuoyanText-0.0.4/src/BuoyanText/stopwords_English.json
-drwxrwxrwx   0        0        0        0 2023-07-20 08:40:11.898953 BuoyanText-0.0.4/src/BuoyanText.egg-info/
--rw-rw-rw-   0        0        0     2089 2023-07-20 08:40:11.000000 BuoyanText-0.0.4/src/BuoyanText.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-07-20 08:40:11.000000 BuoyanText-0.0.4/src/BuoyanText.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:40:11.000000 BuoyanText-0.0.4/src/BuoyanText.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-20 08:40:11.000000 BuoyanText-0.0.4/src/BuoyanText.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 08:40:11.000000 BuoyanText-0.0.4/src/BuoyanText.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.590951 BuoyanText-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-19 08:58:37.000000 BuoyanText-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2085 2023-07-20 10:43:33.589941 BuoyanText-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1510 2023-07-20 10:42:48.000000 BuoyanText-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 10:43:33.592176 BuoyanText-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-07-20 10:43:13.000000 BuoyanText-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.580252 BuoyanText-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.582538 BuoyanText-0.0.5/src/BuoyanText/
+-rw-rw-rw-   0        0        0     8664 2023-07-20 10:42:48.000000 BuoyanText-0.0.5/src/BuoyanText/TextNorm.py
+-rw-rw-rw-   0        0        0     3300 2023-07-19 10:04:46.000000 BuoyanText-0.0.5/src/BuoyanText/TextReader.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 08:37:50.000000 BuoyanText-0.0.5/src/BuoyanText/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.580252 BuoyanText-0.0.5/src/BuoyanText/data/
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.588933 BuoyanText-0.0.5/src/BuoyanText/data/norm/
+-rw-rw-rw-   0        0        0     3321 2023-07-19 15:19:56.000000 BuoyanText-0.0.5/src/BuoyanText/data/norm/contractions_English.json
+-rw-rw-rw-   0        0        0      144 2023-07-11 03:00:16.000000 BuoyanText-0.0.5/src/BuoyanText/data/norm/punctuation_Chinese.json
+-rw-rw-rw-   0        0        0    22250 2023-07-19 15:19:56.000000 BuoyanText-0.0.5/src/BuoyanText/data/norm/stopwords_Chinese.json
+-rw-rw-rw-   0        0        0     2013 2023-07-19 15:19:56.000000 BuoyanText-0.0.5/src/BuoyanText/data/norm/stopwords_English.json
+drwxrwxrwx   0        0        0        0 2023-07-20 10:43:33.586248 BuoyanText-0.0.5/src/BuoyanText.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-07-20 10:43:33.000000 BuoyanText-0.0.5/src/BuoyanText.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-07-20 10:43:33.000000 BuoyanText-0.0.5/src/BuoyanText.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:43:33.000000 BuoyanText-0.0.5/src/BuoyanText.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-20 10:43:33.000000 BuoyanText-0.0.5/src/BuoyanText.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 10:43:33.000000 BuoyanText-0.0.5/src/BuoyanText.egg-info/top_level.txt
```

### Comparing `BuoyanText-0.0.4/LICENSE` & `BuoyanText-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BuoyanText-0.0.4/PKG-INFO` & `BuoyanText-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: BuoyanText
-Version: 0.0.4
+Version: 0.0.5
 Summary: Normalizing English and Chinese Text
 Home-page: https://github.com/BuoyantXu/BuoyantText
 Author: Boyang Xu
 Author-email: by24225@163.com
 Project-URL: Bug Tracker, https://github.com/BuoyantXu/BuoyantText/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BuoyanText
-### v0.0.1 20230719
+### v0.0.5 20230720
 ___
-## ByTextNorm.py
+## TextNorm.py
 
 **TextNorm** class
 
 Normalizing English or Chinese text
 
 **Arguments:**
 
@@ -56,14 +56,14 @@
 
 (3) Chinese text arguments
 
 - split_words:      split words with jieba (default: True)
 - punctuation_drop: drop punctuations (default: True)
 
 ___
-## ByTextReader.py
+## TextReader.py
 
 **(1) file_reader**
 
 **(2) file_list_reader**
 
 **(3) pdf_to_txt**
```

### Comparing `BuoyanText-0.0.4/README.md` & `BuoyanText-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BuoyanText
-### v0.0.1 20230719
+### v0.0.5 20230720
 ___
-## ByTextNorm.py
+## TextNorm.py
 
 **TextNorm** class
 
 Normalizing English or Chinese text
 
 **Arguments:**
 
@@ -40,14 +40,14 @@
 
 (3) Chinese text arguments
 
 - split_words:      split words with jieba (default: True)
 - punctuation_drop: drop punctuations (default: True)
 
 ___
-## ByTextReader.py
+## TextReader.py
 
 **(1) file_reader**
 
 **(2) file_list_reader**
 
 **(3) pdf_to_txt**
```

### Comparing `BuoyanText-0.0.4/setup.py` & `BuoyanText-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BuoyanText",
-    version="0.0.4",
+    version="0.0.5",
     author="Boyang Xu",
     author_email="by24225@163.com",
     description="Normalizing English and Chinese Text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BuoyantXu/BuoyantText",
     install_requires=[
@@ -30,10 +30,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
     ],
     include_package_data=True,
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    package_data={"BuoyanText": ["*.json"]},
+    package_data={"BuoyanText": ["data/norm/*.json"]},
     python_requires=">=3.7",
 )
```

### Comparing `BuoyanText-0.0.4/src/BuoyanText/ByTextNorm.py` & `BuoyanText-0.0.5/src/BuoyanText/TextNorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 
 
 current_path = os.path.dirname(os.path.abspath(__file__))
 
 tokenizer = ToktokTokenizer()
 spacy_nlp = spacy.load('en_core_web_sm')
 
+# load data
 # English
-with open(os.path.join(current_path, 'stopwords_English.json'), 'r') as f:
+with open(os.path.join(current_path, 'data/norm/stopwords_English.json'), 'r') as f:
     stopwords_English = json.load(f)
-with open(os.path.join(current_path, 'contractions_English.json'), 'r') as f:
+with open(os.path.join(current_path, 'data/norm/contractions_English.json'), 'r') as f:
     contractions = json.load(f)
 # Chinese
-with open(os.path.join(current_path, 'stopwords_Chinese.json'), 'r') as f:
+with open(os.path.join(current_path, 'data/norm/stopwords_Chinese.json'), 'r') as f:
     stopwords_Chinese = json.load(f)
-with open(os.path.join(current_path, 'punctuation_Chinese.json'), 'r') as f:
+with open(os.path.join(current_path, 'data/norm/punctuation_Chinese.json'), 'r') as f:
     punctuation = json.load(f)
 
 
 class TextNorm:
     text = ""
     normalized_text = None
```

### Comparing `BuoyanText-0.0.4/src/BuoyanText/ByTextReader.py` & `BuoyanText-0.0.5/src/BuoyanText/TextReader.py`

 * *Files identical despite different names*

### Comparing `BuoyanText-0.0.4/src/BuoyanText/contractions_English.json` & `BuoyanText-0.0.5/src/BuoyanText/data/norm/contractions_English.json`

 * *Files identical despite different names*

### Comparing `BuoyanText-0.0.4/src/BuoyanText/stopwords_Chinese.json` & `BuoyanText-0.0.5/src/BuoyanText/data/norm/stopwords_Chinese.json`

 * *Files identical despite different names*

### Comparing `BuoyanText-0.0.4/src/BuoyanText/stopwords_English.json` & `BuoyanText-0.0.5/src/BuoyanText/data/norm/stopwords_English.json`

 * *Files identical despite different names*

### Comparing `BuoyanText-0.0.4/src/BuoyanText.egg-info/PKG-INFO` & `BuoyanText-0.0.5/src/BuoyanText.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: BuoyanText
-Version: 0.0.4
+Version: 0.0.5
 Summary: Normalizing English and Chinese Text
 Home-page: https://github.com/BuoyantXu/BuoyantText
 Author: Boyang Xu
 Author-email: by24225@163.com
 Project-URL: Bug Tracker, https://github.com/BuoyantXu/BuoyantText/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BuoyanText
-### v0.0.1 20230719
+### v0.0.5 20230720
 ___
-## ByTextNorm.py
+## TextNorm.py
 
 **TextNorm** class
 
 Normalizing English or Chinese text
 
 **Arguments:**
 
@@ -56,14 +56,14 @@
 
 (3) Chinese text arguments
 
 - split_words:      split words with jieba (default: True)
 - punctuation_drop: drop punctuations (default: True)
 
 ___
-## ByTextReader.py
+## TextReader.py
 
 **(1) file_reader**
 
 **(2) file_list_reader**
 
 **(3) pdf_to_txt**
```

