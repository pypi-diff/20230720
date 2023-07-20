# Comparing `tmp/mongodriver-1.2.0.tar.gz` & `tmp/mongodriver-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.0.tar", last modified: Sat Aug 27 05:08:45 2022, max compression
+gzip compressed data, was "mongodriver-1.2.1.tar", last modified: Thu Jul 20 15:40:50 2023, max compression
```

## Comparing `mongodriver-1.2.0.tar` & `mongodriver-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2022-08-27 05:08:45.680357 mongodriver-1.2.0/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.0/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3341 2022-08-27 05:08:45.680432 mongodriver-1.2.0/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2022-08-27 05:08:05.000000 mongodriver-1.2.0/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       79 2022-08-27 05:08:45.680731 mongodriver-1.2.0/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      867 2022-08-27 05:08:41.000000 mongodriver-1.2.0/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2022-08-27 05:08:45.678583 mongodriver-1.2.0/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2022-08-27 05:08:45.679402 mongodriver-1.2.0/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.0/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     5247 2022-08-27 05:05:05.000000 mongodriver-1.2.0/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2022-08-27 05:08:45.680246 mongodriver-1.2.0/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3341 2022-08-27 05:08:45.000000 mongodriver-1.2.0/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      289 2022-08-27 05:08:45.000000 mongodriver-1.2.0/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2022-08-27 05:08:45.000000 mongodriver-1.2.0/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       16 2022-08-27 05:08:45.000000 mongodriver-1.2.0/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2022-08-27 05:08:45.000000 mongodriver-1.2.0/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.175050 mongodriver-1.2.1/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.1/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-20 15:40:50.175156 mongodriver-1.2.1/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.1/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.1/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-07-20 15:40:50.175441 mongodriver-1.2.1/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      891 2023-07-20 14:49:45.000000 mongodriver-1.2.1/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.172850 mongodriver-1.2.1/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.174056 mongodriver-1.2.1/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)        0 2022-02-01 18:07:29.000000 mongodriver-1.2.1/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     7887 2023-07-20 15:20:58.000000 mongodriver-1.2.1/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-07-20 15:40:50.174916 mongodriver-1.2.1/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3323 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      304 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2023-07-20 15:40:50.000000 mongodriver-1.2.1/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.0/LICENSE` & `mongodriver-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.0/PKG-INFO` & `mongodriver-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.0
+Version: 1.2.1
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MongoDriver
 
 An object-oriented package for interacting with MongoDB documents
 
@@ -35,30 +34,31 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
+
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
 # print the value of "foo"
 print(new_document.foo)  # 1
 
 # change the value of "foo"
@@ -69,55 +69,57 @@
 
 new_document.foo.update(3)
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
 
 new_document.set({"new_val1": 15, "new_val2": 10})
 
 # OR
 
 new_document.new_val1 = 15
 new_document.new_val2 = 10
 
 print(new_document)
 
 ```
-
```

### Comparing `mongodriver-1.2.0/README.md` & `mongodriver-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
+
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
 # print the value of "foo"
 print(new_document.foo)  # 1
 
 # change the value of "foo"
@@ -52,47 +53,50 @@
 
 new_document.foo.update(3)
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
 
 new_document.set({"new_val1": 15, "new_val2": 10})
 
 # OR
```

### Comparing `mongodriver-1.2.0/setup.py` & `mongodriver-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.2.0',
+    version='1.2.1',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
     packages=find_packages('src'),
     url='https://github.com/jakestrouse00/mongodriver',
     package_dir={'': 'src'},
     keywords='mongodb',
     install_requires=[
         'pymongo==3.12.0',
+        'pymongo[srv]'
     ],
     description='Object-oriented interactions with MongoDB',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.10",
 
 )
```

### Comparing `mongodriver-1.2.0/src/mongodriver/mongodriver.py` & `mongodriver-1.2.1/src/mongodriver/mongodriver.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,36 +11,41 @@
     client: pymongo.collection.Collection = field(repr=False)
     _initialized: bool = field(repr=False, default=False)
 
     def __post_init__(self):
         if "_id" in self.variables.keys():
             self.variables.pop("_id")
         for variable in self.variables.keys():
-            class_value = Variable(self._id, variable, self.variables[variable], self.client, self)
+            class_value = Variable(
+                self._id, variable, self.variables[variable], self.client, self
+            )
             setattr(self, variable, class_value)
         self._initialized = True
 
     def set(self, new_values: dict):
         """ADDS NEW VARIABLES TO THE DOCUMENT"""
         # removing _id in case it was passed. Don't want to try and update that lol
         if "_id" in new_values.keys():
             new_values.pop("_id")
         self.client.find_one_and_update(
             {"_id": ObjectId(self._id)},
-            {
-                "$set": new_values
-            },
+            {"$set": new_values},
         )
         for variable in new_values.keys():
-            class_value = Variable(self._id, variable, new_values[variable], self.client, self)
+            class_value = Variable(
+                self._id, variable, new_values[variable], self.client, self
+            )
 
             self.variables[variable] = new_values[variable]
             # setattr(self, variable, class_value)
             self.__dict__[variable] = class_value
 
+    def remove(self):
+        self.client.find_one_and_delete({"_id": ObjectId(self._id)})
+
     def asdict(self) -> dict:
         return self.variables
 
     def __setattr__(self, key, value):
         """UPDATE VARIABLES DIRECTLY
         Document.variable = 10
         instead of
@@ -80,55 +85,108 @@
                     self.key: new_value,
                 }
             },
         )
         self.value = new_value
         self.parent_document.variables[self.key] = new_value
 
+    def remove(self):
+        self.client.find_one_and_update(
+            {"_id": ObjectId(self._id)}, {"$unset": {self.key: ""}}
+        )
+        self.parent_document.variables.pop(self.key)
+        self.parent_document.__dict__.pop(self.key)
+
 
 @dataclass
 class Driver:
     connection_url: str = field(repr=True)
     db_name: str = field(repr=True)
     collection_name: str = field(repr=True)
 
     def __post_init__(self):
         """CONNECT TO THE DB"""
-        self.client = pymongo.MongoClient(self.connection_url)[self.db_name][self.collection_name]
+        self.client = pymongo.MongoClient(self.connection_url)[self.db_name][
+            self.collection_name
+        ]
 
     def create(self, data: dict) -> Document:
         """CREATE A DOCUMENT FROM A DICT AND RETURN THE Document OBJECT"""
         document = self.client.insert_one(data)
         python_document = Document(document.inserted_id, data, self.client)
         return python_document
 
+    def update(self, data: dict | Document, new_values: dict, sort: dict = None) -> Document:
+        if "_id" in new_values.keys():
+            new_values.pop("_id")
+        if isinstance(data, Document):
+            if sort is not None:
+                sort = sort.items()
+            self.client.find_one_and_update(filter={"_id": ObjectId(data._id)}, update={"$set" :new_values}, sort=sort, return_document=True)
+            for _, (key, value) in enumerate(new_values.items()):
+                class_value = Variable(
+                    data._id, key, value, self.client, data
+                )
+
+                data.variables[key] = new_values[key]
+                # setattr(self, variable, class_value)
+                data.__dict__[key] = class_value
+            return data
+        else:
+            document = self.client.find_one_and_update(filter=data, update={"$set": update},
+                                                       sort=sort.items(), return_document=True)
+            return Document(document.inserted_id, data, self.client)
+
+
+    def remove(self, data: dict | Document):
+        if isinstance(data, Document):
+            self.client.find_one_and_delete({"_id": ObjectId(data._id)})
+        else:
+            if "_id" in data.keys() and not isinstance(data["_id"], ObjectId):
+                data["_id"] = ObjectId(data["_id"])
+            self.client.find_one_and_delete(data)
+
     def load(self) -> List[Document]:
         """LOADS ALL DOCUMENTS FROM DB INTO Document CLASSES"""
         documents = self.client.find({})
         loaded_documents = []
         for document in documents:
             doc_id = document["_id"]
             document.pop("_id")
             python_document = Document(str(doc_id), document, self.client)
             loaded_documents.append(python_document)
         return loaded_documents
 
-    def find(self, search_terms: dict) -> List[Document]:
+    def find(self, search_terms: dict) -> List[Document] | None:
         """FIND A DOCUMENT AND RETURN IT AS A Document CLASS"""
-        if "_id" in search_terms.keys():
-            if type(search_terms["_id"]) != ObjectId:
-                search_terms["_id"] = ObjectId(search_terms["_id"])
+        if "_id" in search_terms.keys() and not isinstance(search_terms["_id"], ObjectId):
+            search_terms["_id"] = ObjectId(search_terms["_id"])
         processed_documents = []
         documents = self.client.find(search_terms)
+        if len(documents) == 0:
+            return None
         for document in documents:
             doc_id = str(document["_id"])
             python_document = Document(doc_id, document, self.client)
             processed_documents.append(python_document)
         return processed_documents
 
+    def find_one(self, search_terms: dict) -> Document | None:
+        if "_id" in search_terms.keys() and not isinstance(search_terms["_id"], ObjectId):
+            search_terms["_id"] = ObjectId(search_terms["_id"])
+        document = self.client.find_one(search_terms)
+        if document is None:
+            return None
+        doc_id = str(document["_id"])
+        python_document = Document(doc_id, document, self.client)
+        return python_document
+
+
+
+
 
 class ObjectPacker:
     # packing and unpacking objects is simple and technically this implementation may not be needed.
     # But I thought it was a nice touch just in case :)
 
     @staticmethod
     def pack(input_dict: dict, packed_name: str = "PackedObject"):
@@ -138,15 +196,23 @@
 
     @staticmethod
     def unpack(input_object):
         """UNPACK A PYTHON CLASS INTO IT'S DICT"""
         return input_object.__dict__
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
+    # mongodb+srv://Influxes:test@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
     x = Driver(
         connection_url="mongodb+srv://Influxes:test@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="ev_runtime", collection_name="test_model")
-    doc = x.create({"name": "dude", "year": 2007})
-    print(doc)
-    doc.size = "XL"
-    print(doc)
+        db_name="ev_runtime",
+        collection_name="test_model",
+    )
+    # x.remove({"_id": "64b94bcbc98f284f29a7a502"})
+    # doc = x.create({"name": "dude", "year": 2007})
+    # print(doc)
+    # doc.size = "UP"
+    # print(doc)
+    # x.update(doc, {"name": "charlie"})
+    # print(doc)
+    # x.remove(doc)
+    print(x.find_one({"_id": "64b94bcbc98f284f29a7a503"}))
```

### Comparing `mongodriver-1.2.0/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.2.1/src/mongodriver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.0
+Version: 1.2.1
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MongoDriver
 
 An object-oriented package for interacting with MongoDB documents
 
@@ -35,30 +34,31 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
+
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
 # print the value of "foo"
 print(new_document.foo)  # 1
 
 # change the value of "foo"
@@ -69,55 +69,57 @@
 
 new_document.foo.update(3)
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
+
 ```python
-from mongodriver.mongodriver import Driver
+from mongodriver.src.mongodriver import Driver
 
 driver = Driver(
-        connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
-        db_name="example_db", collection_name="example_collection")
+    connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
+    db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
 
 new_document.set({"new_val1": 15, "new_val2": 10})
 
 # OR
 
 new_document.new_val1 = 15
 new_document.new_val2 = 10
 
 print(new_document)
 
 ```
-
```

