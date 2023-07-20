# Comparing `tmp/pyclowder-3.0.1.tar.gz` & `tmp/pyclowder-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyclowder-3.0.1.tar", last modified: Mon Jun  5 21:00:01 2023, max compression
+gzip compressed data, was "dist/pyclowder-3.0.2.tar", last modified: Thu Jul 20 19:34:19 2023, max compression
```

## Comparing `pyclowder-3.0.1.tar` & `pyclowder-3.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-05 20:59:53.000000 pyclowder-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 20:59:53.000000 pyclowder-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-05 21:00:01.000000 pyclowder-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-06-05 20:59:53.000000 pyclowder-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-05 20:59:53.000000 pyclowder-3.0.1/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v1/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/api/v2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    48150 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/geostreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-05 20:59:53.000000 pyclowder-3.0.1/pyclowder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 21:00:01.000000 pyclowder-3.0.1/pyclowder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:00:01.000000 pyclowder-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-05 20:59:53.000000 pyclowder-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-20 19:34:09.000000 pyclowder-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 19:34:09.000000 pyclowder-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-20 19:34:19.000000 pyclowder-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-20 19:34:09.000000 pyclowder-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-20 19:34:09.000000 pyclowder-3.0.2/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v1/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v1/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v2/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/api/v2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48150 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/geostreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-20 19:34:09.000000 pyclowder-3.0.2/pyclowder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 19:34:19.000000 pyclowder-3.0.2/pyclowder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:34:19.000000 pyclowder-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-20 19:34:09.000000 pyclowder-3.0.2/setup.py
```

### Comparing `pyclowder-3.0.1/LICENSE` & `pyclowder-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/PKG-INFO` & `pyclowder-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclowder
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python SDK for the Clowder Data Management System
 Home-page: https://clowderframework.org
 Author: Rob Kooper
 Author-email: kooper@illinois.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/clowder-framework/pyclowder/issues
 Project-URL: Source, https://github.com/clowder-framework/pyclowder
```

### Comparing `pyclowder-3.0.1/README.md` & `pyclowder-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,47 @@
 One of the most interesting aspects of Clowder is the ability to extract metadata from any file. This ability is
 created using extractors. To make it easy to create these extractors in python we have created a module called clowder.
 Besides wrapping often used api calls in convenient python calls, we have also added some code to make it easy to
 create new extractors.
 
 ## Setup
 
+It is recommended to create a Python virtual environment using the following commands before installing PyClowder.
+
+```shell
+python3 -m venv venv
+source venv/bin/activate
+pip install --upgrade pip
+```
+
 Install using pip (for most recent versions see: https://pypi.org/project/pyclowder/):
 
 ```
 pip install pyclowder==2.7.0
 ```
 
 Install pyClowder on your system by cloning this repo:
 
 ```
 git clone https://github.com/clowder-framework/pyclowder.git
 cd pyclowder
 pip install -r requirements.txt
 python setup.py install
 ```
+
 or directly from GitHub:
+
 ```
 pip install -r https://raw.githubusercontent.com/clowder-framework/pyclowder/master/requirements.txt git+https://github.com/clowder-framework/pyclowder.git
 ```
 
 ## Quickstart example
 
-See the [README](https://github.com/clowder-framework/pyclowder/tree/master/sample-extractors/wordcount#readme) in `sample-extractors/wordcount`. Using Docker, no install is required.
+See the [README](https://github.com/clowder-framework/pyclowder/tree/master/sample-extractors/wordcount#readme)
+in `sample-extractors/wordcount`. Using Docker, no install is required.
 
 ## Example Extractor
 
 Following is an example of the WordCount extractor. This example will allow the user to specify from the command line
 what connector to use, the number of connectors, you can get a list of the options by using the -h flag on the command
 line. This will also read some environment variables to initialize the defaults allowing for easy use of this extractor
 in a Docker container.
@@ -156,15 +167,15 @@
 extractor_info.json. This will allow the extractor to be triggered by Clowder events, or directly using its own name.
 
 The --no-bind flag will force the instance of the extractor you are starting to skip binding by the file type(s) in
 extractor_info.json, and instead bind only by extractor name. Assuming no other instances overwrite this binding, your
 extractor instance will then only be triggered via manual or direct messages (i.e. using extractor name), and not by
 upload events in Clowder.
 
-Note however that if any other instances of the extractor are running on the same RabbitMQ queue without --no-bind, 
+Note however that if any other instances of the extractor are running on the same RabbitMQ queue without --no-bind,
 they will still bind by file type as normal regardless of previously existing instances with --no-bind, so use caution
 when running multiple instances of one extractor while using --no-bind.
 
 # Connectors
 
 The system has two connectors defined by default. The connectors are used to star the extractors. The connector will
 look for messages and call the check_message and process_message of the extractor. The two connectors are
@@ -187,63 +198,66 @@
 argument, the logfile that is being monitored to send feedback back to clowder. This connector takes a single argument
 (which can be list):
 
 * picklefile [REQUIRED] : a single file, or list of files that are the pickled messages to be processed.
 
 ## LocalConnector
 
-The Local connector will execute an extractor as a standalone program. This can be used to process files that are 
-present in a local hard drive. After extracting the metadata, it stores the generated metadata in an output file in the 
+The Local connector will execute an extractor as a standalone program. This can be used to process files that are
+present in a local hard drive. After extracting the metadata, it stores the generated metadata in an output file in the
 local drive. This connector takes two arguments:
 
 * --input-file-path [REQUIRED] : Full path of the local input file that needs to be processed.
-* --output-file-path [OPTIONAL] : Full path of the output file (.json) to store the generated metadata. If no output 
-file path is provided, it will create a new file with the name <input_file_with_extension>.json in the same directory 
-as that of the input file.
+* --output-file-path [OPTIONAL] : Full path of the output file (.json) to store the generated metadata. If no output
+  file path is provided, it will create a new file with the name <input_file_with_extension>.json in the same directory
+  as that of the input file.
 
 # Clowder API wrappers
 
 Besides code to create extractors there are also functions that wrap the clowder API. They are broken up into modules
-that map to the routes endpoint of clowder, for example /api/files/:id/download will be in the clowder.files package.
+that map to the routes endpoint of clowder, for example /api/files/:id/download will be in the `clowder.files` package.
 
 ## utils
 
 The clowder.utils package contains some utility functions that should make it easier to create new code that works as
-an extractor or code that interacts with clowder. One of these functions is setup_logging, which will initialize the
+an extractor or code that interacts with clowder. One of these functions is `setup_logging`, which will initialize the
 logging system for you. The logging function takes a single argument that can be None. The argument is either a pointer
 to a file that is read with the configuration options.
 
 ## files
 
 # Dockerfile
 
-We recommend following the instructions at [clowder/generator](https://github.com/clowder-framework/generator) to build a Docker image from your Simple Extractor.
-
-You can also use the pyclowder:onbuild Docker image to easily convert your extractor into a docker container. This image is no longer maintained so it is recommeded to either use the clowder/generator linked above or build your own Dockerfile by choosing your own base image and installing pyClowder as described below.
+We recommend following the instructions at [clowder/generator](https://github.com/clowder-framework/generator) to build
+a Docker image from your Simple Extractor.
 
+You can also use the pyclowder:onbuild Docker image to easily convert your extractor into a docker container. This image
+is no longer maintained, so it is recommended to either use the clowder/generator linked above or build your own
+Dockerfile by choosing your own base image and installing pyClowder as described below.
 
 **This is deprecated and the onbuild image is no longer maintained**
 If you build the extractor as using the pyclowder:onbuild image, you will only need the following Dockerfile
 
 ```
 FROM clowder/pyclowder:onbuild
 
 ENV MAIN_SCRIPT="wordcount.py"
 ```
 
 The main piece is the MAIN_SCRIPT which should point to the python file that holds your main function.
 
-If you need additional packages installed, you will need a file called packages.apt with in this file a list of all
-packages that need to be installed. The docker build process will use this file to install those pacakges first in
+If you need additional packages installed, you will need a file called `packages.apt` with in this file a list of all
+packages that need to be installed. The docker build process will use this file to install those packages first in
 the docker container.
 
-If you need any python packages installed you will need to create file called requiremenets.txt. If this file exists
+If you need any python packages installed you will need to create file called requirements.txt. If this file exists
 the docker build process will use `pip install -r requirements.txt` to install these packages.
 
-To use the latest version of pyClowder we recommend choosing a base image of your choice and install pyClowder by adding it to the requirements.txt file. An example Dockerfile is below:
+To use the latest version of pyClowder we recommend choosing a base image of your choice and install pyClowder by adding
+it to the requirements.txt file. An example Dockerfile is below:
 
 ```
 # Base image
 FROM python:3-slim
 
 # Creating workdir
 WORKDIR /home/clowder
@@ -254,52 +268,65 @@
 
 # Adding necessary code to container under workdir
 COPY <MY.CODE>.py extractor_info.json /home/clowder/
 
 # Command to be run when container is run
 CMD python3 <MY.CODE>.py
 ```
+
 ## SimpleExtractor
-Motivation: design and implement a simple extractor to bridge Python developer and knowledge of PyClowder library. It requires little effort for Python developers to wrap their python code into Clowder's extractors.
 
-Simple extractors take developer defined main function as input parameter to do extraction and then parse and pack extraction's output into Simple extractor defined metadata data-struct and submit back to Clowder.
+Motivation: design and implement a simple extractor to bridge Python developer and knowledge of PyClowder library. It
+requires little effort for Python developers to wrap their python code into Clowder's extractors.
+
+Simple extractors take developer defined main function as input parameter to do extraction and then parse and pack
+extraction's output into Simple extractor defined metadata data-struct and submit back to Clowder.
 
 Users' function must have to return a ``dict'' object containing metdata and previews.
+
 ```markdown
 result = {
-  'metadata': {},
-  'previews': [
-      'filename',
-      {'file': 'filename'},
-      {'file': 'filename', 'metadata': {}, 'mimetype': 'image/jpeg'}
-  ]}
+'metadata': {},
+'previews': [
+'filename',
+{'file': 'filename'},
+{'file': 'filename', 'metadata': {}, 'mimetype': 'image/jpeg'}
+]}
 ```
 
-### Example: 
-`wordcount-simpleextractor` is the simplest example to illustrate how to wrap existing Python code as a Simple Extractor.
+### Example:
+
+`wordcount-simple-extractor` is the simplest example to illustrate how to wrap existing Python code as a Simple
+Extractor.
+
+wordcount.py is regular python file which is defined and provided by Python developers. In the code, wordcount
+invoke `wc` command to process input file to extract lines, words, characters. It packs metadata into python dict.
 
-wordcount.py is regular python file which is defined and provided by Python developers. In the code, wordcount invoke `wc` command to process input file to extract lines, words, characters. It packs metadata into python dict.
 ```markdown
 import subprocess
-  
+
 def wordcount(input_file):
-    result = subprocess.check_output(['wc', input_file], stderr=subprocess.STDOUT)
-    (lines, words, characters, _) = result.split()
-    metadata = {
-        'lines': lines,
-        'words': words,
-        'characters': characters
-    }
-    result = {
-        'metadata': metadata
-    }
-    return result
+result = subprocess.check_output(['wc', input_file], stderr=subprocess.STDOUT)
+(lines, words, characters, _) = result.split()
+metadata = {
+'lines': lines,
+'words': words,
+'characters': characters
+}
+result = {
+'metadata': metadata
+}
+return result
 ```
 
-To build wordcount as a an extractor docker image, users just simply assign two environment variables in Dockerfile shown below. EXTRACTION_FUNC is environment variable and has to be assigned as extraction function, where in wordcount.py, the extraction function is `wordcount`. Environment variable EXTRACTION_MODULE is the name of module file containing the definition of extraction function.
+To build wordcount as an extractor docker image, users just simply assign two environment variables in Dockerfile shown
+below. EXTRACTION_FUNC is environment variable and has to be assigned as extraction function, where in wordcount.py, the
+extraction function is `wordcount`. Environment variable EXTRACTION_MODULE is the name of module file containing the
+definition of extraction function.
+
 ```markdown
 FROM clowder/extractors-simple-extractor:onbuild
 
 ENV EXTRACTION_FUNC="wordcount"
 ENV EXTRACTION_MODULE="wordcount"
 ```
```

### Comparing `pyclowder-3.0.1/description.rst` & `pyclowder-3.0.2/description.rst`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/api/v1/datasets.py` & `pyclowder-3.0.2/pyclowder/api/v1/datasets.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/api/v1/files.py` & `pyclowder-3.0.2/pyclowder/api/v1/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 import json
 import logging
 import os
 import tempfile
 
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
-from urllib3.filepost import encode_multipart_formdata
 
-from pyclowder.datasets import get_file_list
 from pyclowder.collections import get_datasets, get_child_collections
+from pyclowder.datasets import get_file_list
 
 # Some sources of urllib3 support warning suppression, but not all
 try:
     from urllib3 import disable_warnings
     from requests.packages.urllib3.exceptions import InsecureRequestWarning
+
     requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 except:
     pass
 
+
 # pylint: disable=too-many-arguments
 def get_download_url(connector, client, fileid, intermediatefileid=None, ext=""):
     """Download file to be processed from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
@@ -40,14 +41,15 @@
     # TODO: intermediateid doesn't really seem to be used here, can we remove entirely?
     if not intermediatefileid:
         intermediatefileid = fileid
 
     url = '%s/api/files/%s?key=%s' % (client.host, intermediatefileid, client.key)
     return url
 
+
 # pylint: disable=too-many-arguments
 def download(connector, client, fileid, intermediatefileid=None, ext=""):
     """Download file to be processed from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
@@ -65,15 +67,15 @@
     url = '%s/api/files/%s?key=%s' % (client.host, intermediatefileid, client.key)
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True)
 
     (inputfile, inputfilename) = tempfile.mkstemp(suffix=ext)
 
     try:
         with os.fdopen(inputfile, "wb") as outputfile:
-            for chunk in result.iter_content(chunk_size=10*1024):
+            for chunk in result.iter_content(chunk_size=10 * 1024):
                 outputfile.write(chunk)
         return inputfilename
     except Exception:
         os.remove(inputfilename)
         raise
 
 
@@ -176,15 +178,16 @@
 
     for ds in dslist:
         submit_extractions_by_dataset(connector, client.host, client.key, ds['id'], extractorname, ext)
 
     if recursive:
         childcolls = get_child_collections(connector, client.host, client.key, collectionid)
         for coll in childcolls:
-            submit_extractions_by_collection(connector, client.host, client.key, coll['id'], extractorname, ext, recursive)
+            submit_extractions_by_collection(connector, client.host, client.key, coll['id'], extractorname, ext,
+                                             recursive)
 
 
 def upload_metadata(connector, client, fileid, metadata):
     """Upload file JSON-LD metadata to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
@@ -198,15 +201,15 @@
     headers = {'Content-Type': 'application/json'}
     url = '%s/api/files/%s/metadata.jsonld?key=%s' % (client.host, fileid, client.key)
     result = connector.post(url, headers=headers, data=json.dumps(metadata),
                             verify=connector.ssl_verify if connector else True)
 
 
 # pylint: disable=too-many-arguments
-def upload_preview(connector, client, fileid, previewfile, previewmetadata=None, preview_mimetype=None):
+def upload_preview(connector, client, fileid, previewfile, previewmetadata=None, preview_mimetype=None, **kwargs):
     """Upload preview to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     fileid -- the file that is currently being processed
     previewfile -- the file containing the preview
```

### Comparing `pyclowder-3.0.1/pyclowder/api/v2/datasets.py` & `pyclowder-3.0.2/pyclowder/api/v2/datasets.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/api/v2/files.py` & `pyclowder-3.0.2/pyclowder/api/v2/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 import json
 import logging
 import os
 import tempfile
 
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
-from urllib3.filepost import encode_multipart_formdata
-from pyclowder.client import ClowderClient
+
 from pyclowder.datasets import get_file_list
-from pyclowder.collections import get_datasets, get_child_collections
 
 # Some sources of urllib3 support warning suppression, but not all
 try:
     from urllib3 import disable_warnings
     from requests.packages.urllib3.exceptions import InsecureRequestWarning
+
     requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 except:
     pass
 
 
 def get_download_url(connector, client, fileid, intermediatefileid=None, ext=""):
     """Download file to be processed from Clowder.
@@ -40,30 +39,29 @@
     # TODO: intermediateid doesn't really seem to be used here, can we remove entirely?
     if not intermediatefileid:
         intermediatefileid = fileid
 
     url = '%s/api/v2/files/%s' % (client.host, intermediatefileid)
     return url
 
+
 # pylint: disable=too-many-arguments
 def download(connector, client, fileid, intermediatefileid=None, ext=""):
     """Download file to be processed from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     fileid -- the file that is currently being processed
     intermediatefileid -- either same as fileid, or the intermediate file to be used
     ext -- the file extension, the downloaded file will end with this extension
     """
 
     connector.message_process({"type": "file", "id": fileid}, "Downloading file.")
 
-
-
     # TODO: intermediateid doesn't really seem to be used here, can we remove entirely?
     if not intermediatefileid:
         intermediatefileid = fileid
 
     url = '%s/api/v2/files/%s' % (client.host, intermediatefileid)
     headers = {"X-API-KEY": client.key}
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
@@ -93,26 +91,26 @@
     headers = {"X-API-KEY": client.key}
     # fetch data
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
 
     return result
 
 
-def download_metadata(connector,client, fileid, extractor=None):
+def download_metadata(connector, client, fileid, extractor=None):
     """Download file JSON-LD metadata from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     fileid -- the file to fetch metadata of
     extractor -- extractor name to filter results (if only one extractor's metadata is desired)
     """
 
     filterstring = "" if extractor is None else "?extractor=%s" % extractor
-    url = '%s/api/v2/files/%s/metadata?%s' % (client.host, fileid, filterstring)
+    url = '%s/api/v2/files/%s/metadata%s' % (client.host, fileid, filterstring)
     headers = {"X-API-KEY": client.key}
 
     # fetch data
     result = connector.get(url, stream=True, verify=connector.ssl_verify if connector else True, headers=headers)
 
     return result
 
@@ -151,62 +149,97 @@
     headers = {'Content-Type': 'application/json',
                'X-API-KEY': client.key}
     url = '%s/api/v2/files/%s/metadata' % (client.host, fileid)
     result = connector.post(url, headers=headers, data=json.dumps(metadata),
                             verify=connector.ssl_verify if connector else True)
 
 
-
-# TODO not implemented in v2
 # pylint: disable=too-many-arguments
-def upload_preview(connector, client, fileid, previewfile, previewmetadata=None, preview_mimetype=None):
-    """Upload preview to Clowder.
+def upload_preview(connector, client, fileid, previewfile, previewmetadata=None, preview_mimetype=None,
+                   visualization_name=None, visualization_description=None, visualization_config_data=None,
+                   visualization_component_id=None):
+    """Upload visualization to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     client -- ClowderClient containing authentication credentials
     fileid -- the file that is currently being processed
     previewfile -- the file containing the preview
     previewmetadata -- any metadata to be associated with preview, can contain a section_id
                     to indicate the section this preview should be associated with.
     preview_mimetype -- (optional) MIME type of the preview file. By default, this is obtained from the
                     file itself and this parameter can be ignored. E.g. 'application/vnd.clowder+custom+xml'
     """
 
     connector.message_process({"type": "file", "id": fileid}, "Uploading file preview.")
-
     logger = logging.getLogger(__name__)
-    headers = {'Content-Type': 'application/json'}
 
-    # upload preview
-    url = '%s/api/previews?key=%s' % (client.host, client.key)
-    with open(previewfile, 'rb') as filebytes:
-        # If a custom preview file MIME type is provided, use it to generate the preview file object.
-        if preview_mimetype is not None:
-            result = connector.post(url, files={"File": (os.path.basename(previewfile), filebytes, preview_mimetype)},
-                                    verify=connector.ssl_verify if connector else True)
+    preview_id = None
+    visualization_config_id = None
+
+    if os.path.exists(previewfile):
+
+        # upload visualization URL
+        visualization_config_url = '%s/api/v2/visualizations/config' % client.host
+
+        if visualization_config_data is None:
+            visualization_config_data = dict()
+
+        payload = json.dumps({
+            "resource": {
+                "collection": "files",
+                "resource_id": fileid
+            },
+            "client": client.host,
+            "parameters": visualization_config_data,
+            "visualization_mimetype": preview_mimetype,
+            "visualization_component_id": visualization_component_id
+        })
+
+        headers = {
+            "X-API-KEY": client.key,
+            "Content-Type": "application/json"
+        }
+
+        response = connector.post(visualization_config_url, headers=headers, data=payload,
+                                  verify=connector.ssl_verify if connector else True)
+
+        if response.status_code == 200:
+            visualization_config_id = response.json()['id']
+            logger.debug("Uploaded visualization config ID = [%s]", visualization_config_id)
         else:
-            result = connector.post(url, files={"File": filebytes}, verify=connector.ssl_verify if connector else True)
+            logger.error("An error occurred when uploading visualization config to file: " + fileid)
 
-    previewid = result.json()['id']
-    logger.debug("preview id = [%s]", previewid)
+        if visualization_config_id is not None:
 
-    # associate uploaded preview with orginal file
-    if fileid and not (previewmetadata and 'section_id' in previewmetadata and previewmetadata['section_id']):
-        url = '%s/api/files/%s/previews/%s?key=%s' % (client.host, fileid, previewid, client.key)
-        result = connector.post(url, headers=headers, data=json.dumps({}),
-                                verify=connector.ssl_verify if connector else True)
+            # upload visualization URL
+            visualization_url = '%s/api/v2/visualizations?name=%s&description=%s&config=%s' % (
+                client.host, visualization_name, visualization_description, visualization_config_id)
+
+            filename = os.path.basename(previewfile)
+            if preview_mimetype is not None:
+                multipart_encoder_object = MultipartEncoder(
+                    fields={'file': (filename, open(previewfile, 'rb'), preview_mimetype)})
+            else:
+                multipart_encoder_object = MultipartEncoder(fields={'file': (filename, open(previewfile, 'rb'))})
+            headers = {'X-API-KEY': client.key,
+                       'Content-Type': multipart_encoder_object.content_type}
+            response = connector.post(visualization_url, data=multipart_encoder_object, headers=headers,
+                                      verify=connector.ssl_verify if connector else True)
+
+            if response.status_code == 200:
+                preview_id = response.json()['id']
+                logger.debug("Uploaded visualization data ID = [%s]", preview_id)
+            else:
+                logger.error("An error occurred when uploading the visualization data to file: " + fileid)
+    else:
+        logger.error("Visualization data file not found")
 
-    # associate metadata with preview
-    if previewmetadata is not None:
-        url = '%s/api/previews/%s/metadata?key=%s' % (client.host, previewid, client.key)
-        result = connector.post(url, headers=headers, data=json.dumps(previewmetadata),
-                                verify=connector.ssl_verify if connector else True)
+    return preview_id
 
-    return previewid
 
 # TODO not implemented in v2
 def upload_tags(connector, client, fileid, tags):
     """Upload file tag to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
@@ -218,42 +251,31 @@
     connector.message_process({"type": "file", "id": fileid}, "Uploading file tags.")
 
     headers = {'Content-Type': 'application/json'}
     url = '%s/api/files/%s/tags?key=%s' % (client.host, fileid, client.key)
     result = connector.post(url, headers=headers, data=json.dumps(tags),
                             verify=connector.ssl_verify if connector else True)
 
+
 # TODO not implemented in v2
 def upload_thumbnail(connector, client, fileid, thumbnail):
     """Upload thumbnail to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file that the thumbnail should be associated with
     thumbnail -- the file containing the thumbnail
     """
 
+    # TODO: Update the code below after V2 endpoint for uploading a thumbnail is ready.
     logger = logging.getLogger(__name__)
-    url = client.host + 'api/fileThumbnail?key=' + client.key
-
-    # upload preview
-    with open(thumbnail, 'rb') as inputfile:
-        result = connector.post(url, files={"File": inputfile}, verify=connector.ssl_verify if connector else True)
-    thumbnailid = result.json()['id']
-    logger.debug("thumbnail id = [%s]", thumbnailid)
-
-    # associate uploaded preview with orginal file/dataset
-    if fileid:
-        headers = {'Content-Type': 'application/json'}
-        url = client.host + 'api/files/' + fileid + '/thumbnails/' + thumbnailid + '?key=' + client.key
-        connector.post(url, headers=headers, data=json.dumps({}), verify=connector.ssl_verify if connector else True)
-
-    return thumbnailid
+    logger.info("Thumbnail upload is under construction and currently skipped in Clowder V2 extractors!")
+    pass
 
 
 def upload_to_dataset(connector, client, datasetid, filepath, check_duplicate=False):
     """Upload file to existing Clowder dataset.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
@@ -277,18 +299,18 @@
             return _upload_to_dataset_local(connector, client, datasetid, filepath)
 
     url = '%s/api/v2/datasets/%s/files' % (client.host, datasetid)
 
     if os.path.exists(filepath):
         filename = os.path.basename(filepath)
         m = MultipartEncoder(
-            fields={'file': (filename, open(filepath, 'rb'))}
+            fields={'File': (filename, open(filepath, 'rb'))}
         )
         headers = {"X-API-KEY": client.key,
-                    'Content-Type': m.content_type}
+                   'Content-Type': m.content_type}
         result = connector.post(url, data=m, headers=headers,
                                 verify=connector.ssl_verify if connector else True)
 
         uploadedfileid = result.json()['id']
         logger.debug("uploaded file id = [%s]", uploadedfileid)
 
         return uploadedfileid
@@ -317,15 +339,15 @@
                 break
 
         filename = os.path.basename(filepath)
         m = MultipartEncoder(
             fields={'file': (filename, open(filepath, 'rb'))}
         )
         headers = {"X-API-KEY": client.key,
-                    'Content-Type': m.content_type}
+                   'Content-Type': m.content_type}
         result = connector.post(url, data=m, headers=headers,
                                 verify=connector.ssl_verify if connector else True)
 
         uploadedfileid = result.json()['id']
         logger.debug("uploaded file id = [%s]", uploadedfileid)
 
         return uploadedfileid
```

### Comparing `pyclowder-3.0.1/pyclowder/client.py` & `pyclowder-3.0.2/pyclowder/client.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/collections.py` & `pyclowder-3.0.2/pyclowder/collections.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/connectors.py` & `pyclowder-3.0.2/pyclowder/connectors.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/datasets.py` & `pyclowder-3.0.2/pyclowder/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     key -- the secret key to login to clowder
     datasetid -- the dataset to delete
     """
     client = ClowderClient(host=host, key=key)
     if clowder_version == 2:
         result = v2datasets.delete(connector, client, datasetid)
     else:
-        result = v2datasets.delete(connector, client, datasetid)
+        result = v1datasets.delete(connector, client, datasetid)
     result.raise_for_status()
 
     return json.loads(result.text)
 
 
 def delete_by_collection(connector, host, key, collectionid, recursive=True, delete_colls=False):
     """Delete datasets from Clowder by iterating through collection.
```

### Comparing `pyclowder-3.0.1/pyclowder/extractors.py` & `pyclowder-3.0.2/pyclowder/extractors.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/files.py` & `pyclowder-3.0.2/pyclowder/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,113 +2,104 @@
 
 This module provides simple wrappers around the clowder Files API
 """
 
 import json
 import logging
 import os
-import tempfile
 
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
-from urllib3.filepost import encode_multipart_formdata
+
 from pyclowder.client import ClowderClient
-from pyclowder.datasets import get_file_list
 from pyclowder.collections import get_datasets, get_child_collections
-import pyclowder.api.v2.files as v2files
-import pyclowder.api.v1.files as v1files
+from pyclowder.datasets import get_file_list
 
 clowder_version = int(os.getenv('CLOWDER_VERSION', '1'))
+# Import files API methods based on Clowder version
+if clowder_version == 2:
+    import pyclowder.api.v2.files as files
+else:
+    import pyclowder.api.v1.files as files
 
 # Some sources of urllib3 support warning suppression, but not all
 try:
     from urllib3 import disable_warnings
     from requests.packages.urllib3.exceptions import InsecureRequestWarning
+
     requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 except:
     pass
 
+
 def get_download_url(connector, host, key, fileid, intermediatefileid=None, ext=""):
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        download_url = v2files.get_download_url(connector, client, fileid, intermediatefileid, ext)
-    else:
-        download_url = v1files.get_download_url(connector, client, fileid, intermediatefileid, ext)
+    download_url = files.get_download_url(connector, client, fileid, intermediatefileid, ext)
     return download_url
 
+
 # pylint: disable=too-many-arguments
 def download(connector, host, key, fileid, intermediatefileid=None, ext="", tracking=True):
     """Download file to be processed from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file that is currently being processed
     intermediatefileid -- either same as fileid, or the intermediate file to be used
     ext -- the file extension, the downloaded file will end with this extension
     tracking -- should the download action be tracked
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        inputfilename = v2files.download(connector, client, fileid, intermediatefileid, ext)
-    else:
-        inputfilename = v1files.download(connector, client, fileid, intermediatefileid, ext)
+    inputfilename = files.download(connector, client, fileid, intermediatefileid, ext)
     return inputfilename
 
+
 def download_info(connector, host, key, fileid):
     """Download file summary metadata from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file to fetch metadata of
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        result = v2files.download_info(connector, client, fileid)
-    else:
-        result = v1files.download_info(connector, client, fileid)
+    result = files.download_info(connector, client, fileid)
     return result.json()
 
 
 def download_metadata(connector, host, key, fileid, extractor=None):
     """Download file JSON-LD metadata from Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file to fetch metadata of
     extractor -- extractor name to filter results (if only one extractor's metadata is desired)
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        result = v2files.download_metadata(connector, client, fileid, extractor)
-    else:
-        result = v1files.download_metadata(connector, client, fileid, extractor)
+    result = files.download_metadata(connector, client, fileid, extractor)
     return result.json()
 
 
 def submit_extraction(connector, host, key, fileid, extractorname):
     """Submit file for extraction by given extractor.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file UUID to submit
     extractorname -- registered name of extractor to trigger
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        result = v2files.submit_extraction(connector, client, fileid, extractorname)
-    else:
-        result = v1files.submit_extraction(connector, client, fileid, extractorname)
+    result = files.submit_extraction(connector, client, fileid, extractorname)
     return result.json()
 
 
 def submit_extractions_by_dataset(connector, host, key, datasetid, extractorname, ext=False):
     """Manually trigger an extraction on all files in a dataset.
 
         This will iterate through all files in the given dataset and submit them to
@@ -167,67 +158,42 @@
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file that is currently being processed
     metadata -- the metadata to be uploaded
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        v2files.upload_metadata(connector, client, fileid, metadata)
-    else:
-        v1files.upload_metadata(connector, client, fileid, metadata)
+    files.upload_metadata(connector, client, fileid, metadata)
 
 
 # pylint: disable=too-many-arguments
-def upload_preview(connector, host, key, fileid, previewfile, previewmetadata=None, preview_mimetype=None):
+def upload_preview(connector, host, key, fileid, previewfile, previewmetadata=None, preview_mimetype=None,
+                   visualization_name=None, visualization_description=None, visualization_config_data=None,
+                   visualization_component_id=None):
     """Upload preview to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file that is currently being processed
     previewfile -- the file containing the preview
     previewmetadata -- any metadata to be associated with preview, can contain a section_id
                     to indicate the section this preview should be associated with.
     preview_mimetype -- (optional) MIME type of the preview file. By default, this is obtained from the
                     file itself and this parameter can be ignored. E.g. 'application/vnd.clowder+custom+xml'
     """
-    client = ClowderClient(host=host, key=key)
-    connector.message_process({"type": "file", "id": fileid}, "Uploading file preview.")
-
-    logger = logging.getLogger(__name__)
-    headers = {'Content-Type': 'application/json'}
-
-    # upload preview
-    url = '%sapi/previews?key=%s' % (client.host, client.key)
-    with open(previewfile, 'rb') as filebytes:
-        # If a custom preview file MIME type is provided, use it to generate the preview file object.
-        if preview_mimetype is not None:
-            result = connector.post(url, files={"File": (os.path.basename(previewfile), filebytes, preview_mimetype)},
-                                    verify=connector.ssl_verify if connector else True)
-        else:
-            result = connector.post(url, files={"File": filebytes}, verify=connector.ssl_verify if connector else True)
-
-    previewid = result.json()['id']
-    logger.debug("preview id = [%s]", previewid)
 
-    # associate uploaded preview with orginal file
-    if fileid and not (previewmetadata and 'section_id' in previewmetadata and previewmetadata['section_id']):
-        url = '%sapi/files/%s/previews/%s?key=%s' % (client.host, fileid, previewid, client.key)
-        result = connector.post(url, headers=headers, data=json.dumps({}),
-                                verify=connector.ssl_verify if connector else True)
-
-    # associate metadata with preview
-    if previewmetadata is not None:
-        url = '%sapi/previews/%s/metadata?key=%s' % (client.host, previewid, client.key)
-        result = connector.post(url, headers=headers, data=json.dumps(previewmetadata),
-                                verify=connector.ssl_verify if connector else True)
-
-    return previewid
+    client = ClowderClient(host=host, key=key)
+    preview_id = files.upload_preview(connector, client, fileid, previewfile, previewmetadata, preview_mimetype,
+                                      visualization_name=visualization_name,
+                                      visualization_description=visualization_description,
+                                      visualization_config_data=visualization_config_data,
+                                      visualization_component_id=visualization_component_id)
+    return preview_id
 
 
 def upload_tags(connector, host, key, fileid, tags):
     """Upload file tag to Clowder.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
@@ -251,31 +217,18 @@
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     fileid -- the file that the thumbnail should be associated with
     thumbnail -- the file containing the thumbnail
     """
+    
     client = ClowderClient(host=host, key=key)
-    logger = logging.getLogger(__name__)
-    url = client.host + 'api/fileThumbnail?key=' + client.key
-
-    # upload preview
-    with open(thumbnail, 'rb') as inputfile:
-        result = connector.post(url, files={"File": inputfile}, verify=connector.ssl_verify if connector else True)
-    thumbnailid = result.json()['id']
-    logger.debug("thumbnail id = [%s]", thumbnailid)
-
-    # associate uploaded preview with orginal file/dataset
-    if fileid:
-        headers = {'Content-Type': 'application/json'}
-        url = client.host + 'api/files/' + fileid + '/thumbnails/' + thumbnailid + '?key=' + client.key
-        connector.post(url, headers=headers, data=json.dumps({}), verify=connector.ssl_verify if connector else True)
-
-    return thumbnailid
+    thumbnail_id = files.upload_thumbnail(connector, client, fileid, thumbnail)
+    return thumbnail_id
 
 
 def upload_to_dataset(connector, host, key, datasetid, filepath, check_duplicate=False):
     """Upload file to existing Clowder dataset.
 
     Keyword arguments:
     connector -- connector information, used to get missing parameters and send status updates
@@ -283,15 +236,15 @@
     key -- the secret key to login to clowder
     datasetid -- the dataset that the file should be associated with
     filepath -- path to file
     check_duplicate -- check if filename already exists in dataset and skip upload if so
     """
     client = ClowderClient(host=host, key=key)
     if clowder_version == 2:
-        v2files.upload_to_dataset(connector, client, datasetid, filepath, check_duplicate)
+        files.upload_to_dataset(connector, client, datasetid, filepath, check_duplicate)
     else:
         logger = logging.getLogger(__name__)
 
         if check_duplicate:
             ds_files = get_file_list(connector, client, datasetid)
             for f in ds_files:
                 if f['filename'] == os.path.basename(filepath):
@@ -327,12 +280,9 @@
     connector -- connector information, used to get missing parameters and send status updates
     host -- the clowder host, including http and port, should end with a /
     key -- the secret key to login to clowder
     datasetid -- the dataset that the file should be associated with
     filepath -- path to file
     """
     client = ClowderClient(host=host, key=key)
-    if clowder_version == 2:
-        uploadedfileid = v2files._upload_to_dataset_local(connector, client, datasetid, filepath)
-    else:
-        uploadedfileid = v1files._upload_to_dataset_local(connector, client, datasetid, filepath)
-    return uploadedfileid
+    uploadedfileid = files._upload_to_dataset_local(connector, client, datasetid, filepath)
+    return uploadedfileid
```

### Comparing `pyclowder-3.0.1/pyclowder/geostreams.py` & `pyclowder-3.0.2/pyclowder/geostreams.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/sections.py` & `pyclowder-3.0.2/pyclowder/sections.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder/utils.py` & `pyclowder-3.0.2/pyclowder/utils.py`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/pyclowder.egg-info/PKG-INFO` & `pyclowder-3.0.2/pyclowder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclowder
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python SDK for the Clowder Data Management System
 Home-page: https://clowderframework.org
 Author: Rob Kooper
 Author-email: kooper@illinois.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/clowder-framework/pyclowder/issues
 Project-URL: Source, https://github.com/clowder-framework/pyclowder
```

### Comparing `pyclowder-3.0.1/pyclowder.egg-info/SOURCES.txt` & `pyclowder-3.0.2/pyclowder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclowder-3.0.1/setup.py` & `pyclowder-3.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'description.rst').read_text(encoding='utf-8')
 
 setup(
     name='pyclowder',
-    version='3.0.1',
+    version='3.0.2',
     description='Python SDK for the Clowder Data Management System',
     long_description=long_description,
 
     author='Rob Kooper',
     author_email='kooper@illinois.edu',
 
     url='https://clowderframework.org',
```

