# Comparing `tmp/chatting_with_pdfs-0.0.11.tar.gz` & `tmp/chatting-with-pdfs-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatting_with_pdfs-0.0.11.tar", last modified: Mon Jul 17 08:18:18 2023, max compression
+gzip compressed data, was "chatting-with-pdfs-0.0.12.tar", last modified: Thu Jul 20 10:03:54 2023, max compression
```

## Comparing `chatting_with_pdfs-0.0.11.tar` & `chatting-with-pdfs-0.0.12.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.741321 chatting_with_pdfs-0.0.11/
--rw-rw-rw-   0        0        0     1086 2023-07-13 15:51:36.000000 chatting_with_pdfs-0.0.11/LICENSE
--rw-rw-rw-   0        0        0     3135 2023-07-17 08:18:18.741321 chatting_with_pdfs-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2023-07-13 16:12:42.000000 chatting_with_pdfs-0.0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.728170 chatting_with_pdfs-0.0.11/app/
-drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.739543 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/
--rw-rw-rw-   0        0        0     3135 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 08:18:18.742319 chatting_with_pdfs-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-17 08:17:41.000000 chatting_with_pdfs-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:03:54.062328 chatting-with-pdfs-0.0.12/
+-rw-rw-rw-   0        0        0     1081 2023-07-19 13:17:26.000000 chatting-with-pdfs-0.0.12/LICENSE.txt
+-rw-rw-rw-   0        0        0     3347 2023-07-20 10:03:54.058855 chatting-with-pdfs-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2913 2023-07-19 15:29:52.000000 chatting-with-pdfs-0.0.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 10:03:54.063206 chatting-with-pdfs-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-07-20 10:02:55.000000 chatting-with-pdfs-0.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:03:53.989666 chatting-with-pdfs-0.0.12/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 10:03:54.017444 chatting-with-pdfs-0.0.12/src/chat_pdf/
+-rw-rw-rw-   0        0        0        0 2023-07-19 15:07:38.000000 chatting-with-pdfs-0.0.12/src/chat_pdf/__init__.py
+-rw-rw-rw-   0        0        0     2623 2023-07-19 15:32:43.000000 chatting-with-pdfs-0.0.12/src/chat_pdf/chat_with_pdfs.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:03:54.051580 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-07-20 10:03:53.000000 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-20 10:03:53.000000 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:03:53.000000 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-07-20 10:03:53.000000 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 10:03:53.000000 chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/top_level.txt
```

### Comparing `chatting_with_pdfs-0.0.11/LICENSE` & `chatting-with-pdfs-0.0.12/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 ArjanCodes
+Copyright (c) 2023 Morne
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chatting_with_pdfs-0.0.11/PKG-INFO` & `chatting-with-pdfs-0.0.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: chatting_with_pdfs
-Version: 0.0.11
+Name: chatting-with-pdfs
+Version: 0.0.12
 Summary: Load a PDF file and ask questions via llama_index and GPT.
 Author: Morne
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # About Python Chat PDF (GPT Index) Project
 
 Load your PDFs data folder and ask questions via llama_index and GPT.
 
 ---
 
@@ -78,7 +78,18 @@
 - Run the script.
 
 ```bash
 python3 chat_with_pdfs.py <"data_folder_path"> <"open_api_key">
 ```
 
 - Ask any questions about the content of the PDF.
+
+### How to use our package:
+
+```bash
+from chat_pdf.chat_with_pdfs import ask_a_question
+import sys
+
+folder_name = sys.argv[1]
+api_key = sys.argv[2]
+print(ask_a_question(folder_name, api_key))
+```
```

### Comparing `chatting_with_pdfs-0.0.11/README.md` & `chatting-with-pdfs-0.0.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,19 @@
 
 - Run the script.
 
 ```bash
 python3 chat_with_pdfs.py <"data_folder_path"> <"open_api_key">
 ```
 
-- Ask any questions about the content of the PDF.
+- Ask any questions about the content of the PDF.
+
+### How to use our package:
+
+```bash
+from chat_pdf.chat_with_pdfs import ask_a_question
+import sys
+
+folder_name = sys.argv[1]
+api_key = sys.argv[2]
+print(ask_a_question(folder_name, api_key))
+```
```

### Comparing `chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/PKG-INFO` & `chatting-with-pdfs-0.0.12/src/chatting_with_pdfs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: chatting-with-pdfs
-Version: 0.0.11
+Version: 0.0.12
 Summary: Load a PDF file and ask questions via llama_index and GPT.
 Author: Morne
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # About Python Chat PDF (GPT Index) Project
 
 Load your PDFs data folder and ask questions via llama_index and GPT.
 
 ---
 
@@ -78,7 +78,18 @@
 - Run the script.
 
 ```bash
 python3 chat_with_pdfs.py <"data_folder_path"> <"open_api_key">
 ```
 
 - Ask any questions about the content of the PDF.
+
+### How to use our package:
+
+```bash
+from chat_pdf.chat_with_pdfs import ask_a_question
+import sys
+
+folder_name = sys.argv[1]
+api_key = sys.argv[2]
+print(ask_a_question(folder_name, api_key))
+```
```

### Comparing `chatting_with_pdfs-0.0.11/setup.py` & `chatting-with-pdfs-0.0.12/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from setuptools import find_packages, setup
 
-with open("app/README.md", "r", encoding="utf8") as f:
+with open("README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
-    name="chatting_with_pdfs",
-    version="0.0.11",
+    name="chatting-with-pdfs",
+    version="0.0.12",
     description="Load a PDF file and ask questions via llama_index and GPT.",
-    package_dir={"": "app"},
-    packages=find_packages(where="app"),
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Morne",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
-    install_requires=["bson >= 0.5.10"],
+    install_requires=[
+        "bson >= 0.5.10",
+        "openai >= 0.27.6",
+        "langchain >= 0.0.160",
+        "setuptools >= 67.8.0",
+        "llama-index >= 0.6.7",
+        "PyPDF2 >= 3.0.1"
+    ],
     extras_require={
-        "dev": ["pytest>=7.0", "twine>=4.0.2"],
+        "dev": ["pytest>=7.4.0", "twine>=4.0.2"],
     },
     python_requires=">=3.10",
 )
```

