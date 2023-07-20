# Comparing `tmp/pytest-mongo-2.1.1.tar.gz` & `tmp/pytest-mongo-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mongo-2.1.1.tar", last modified: Mon Jun  7 12:14:01 2021, max compression
+gzip compressed data, was "pytest-mongo-3.0.0.tar", last modified: Thu Jul 20 14:14:53 2023, max compression
```

## Comparing `pytest-mongo-2.1.1.tar` & `pytest-mongo-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 12:14:01.010414 pytest-mongo-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7631 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6689 2021-06-07 12:14:01.010414 pytest-mongo-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2021-06-07 12:14:01.014414 pytest-mongo-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 12:14:01.010414 pytest-mongo-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 12:14:01.010414 pytest-mongo-2.1.1/src/pytest_mongo/
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/src/pytest_mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/src/pytest_mongo/executor_noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     6290 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/src/pytest_mongo/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-06-07 12:13:53.000000 pytest-mongo-2.1.1/src/pytest_mongo/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 12:14:01.010414 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6689 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-06-07 12:14:01.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-07 12:14:00.000000 pytest-mongo-2.1.1/src/pytest_mongo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:14:53.275295 pytest-mongo-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-20 14:14:53.275295 pytest-mongo-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:14:53.275295 pytest-mongo-3.0.0/pytest_mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pytest_mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pytest_mongo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pytest_mongo/executor_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pytest_mongo/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 14:14:37.000000 pytest-mongo-3.0.0/pytest_mongo/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:14:53.275295 pytest-mongo-3.0.0/pytest_mongo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 14:14:53.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:14:52.000000 pytest-mongo-3.0.0/pytest_mongo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:14:53.275295 pytest-mongo-3.0.0/setup.cfg
```

### Comparing `pytest-mongo-2.1.1/CONTRIBUTING.rst` & `pytest-mongo-3.0.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Contribute to pytest-mongo
-==============
+==========================
 
 Thank you for taking time to contribute to pytest-mongo!
 
 The following is a set of guidelines for contributing to pytest-mongo. These are just guidelines, not rules, use your best judgment and feel free to propose changes to this document in a pull request.
 
 Bug Reports
 -----------
```

### Comparing `pytest-mongo-2.1.1/LICENSE` & `pytest-mongo-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mongo-2.1.1/README.rst` & `pytest-mongo-3.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     .. code-block:: python
 
         mongo_proc = factories.mongo_proc(port=8888)
 
 * use ``--mongo-port`` command line option when you run your tests
 
-    .. code-block::
+    .. code-block:: sh
 
         py.test tests --mongo-port=8888
 
 
 * specify your directory as ``mongo_port`` in your ``pytest.ini`` file.
 
     To do so, put a line like the following under the ``[pytest]`` section of your ``pytest.ini``:
```

### Comparing `pytest-mongo-2.1.1/setup.py` & `pytest-mongo-3.0.0/pytest_mongo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,11 @@
 
 # pytest-mongo is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
-# along with pytest-mongo. If not, see <http://www.gnu.org/licenses/>.
-"""Package definition for pytest-mongo."""
-from setuptools import setup
+# along with pytest-mongo.  If not, see <http://www.gnu.org/licenses/>.
+"""pytest-mongo's main module."""
 
-
-setup()
+__version__ = "3.0.0"
```

### Comparing `pytest-mongo-2.1.1/src/pytest_mongo/executor_noop.py` & `pytest-mongo-3.0.0/pytest_mongo/executor_noop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """MongoDB Noop executor providing connection details for mongodb client."""
-import pymongo
+from typing import Optional
+
+from pymongo import MongoClient
 
 
 class NoopExecutor:  # pylint: disable=too-few-public-methods
-    """
-    Nooperator executor.
+    """Nooperator executor.
 
     This executor actually does nothing more than provide connection details
     for existing MongoDB server. I.E. one already started either on machine
     or with the use of containerisation like kubernetes or docker compose.
     """
 
-    def __init__(self, host, port):
-        """
-        Initialize nooperator executor mock.
+    def __init__(self, host: str, port: int) -> None:
+        """Initialize nooperator executor mock.
 
-        :param str host: MongoDB hostname
-        :param str|int port: MongoDB port
+        :param host: MongoDB hostname
+        :param port: MongoDB port
         """
         self.host = host
-        self.port = int(port)
-        self._version = None
+        self.port = port
+        self._version: Optional[str] = None
 
     @property
-    def version(self):
+    def version(self) -> str:
         """Get MongoDB's version."""
         if not self._version:
-            client = pymongo.MongoClient(host=self.host, port=self.port)
+            client: MongoClient = MongoClient(host=self.host, port=self.port)
             server_info = client.server_info()
             self._version = server_info["version"]
+        assert self._version
         return self._version
```

### Comparing `pytest-mongo-2.1.1/src/pytest_mongo/factories.py` & `pytest-mongo-3.0.0/pytest_mongo/factories.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,151 +15,135 @@
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-mongo.  If not, see <http://www.gnu.org/licenses/>.
 """Fixture factories."""
 import os
 from shutil import rmtree
 from tempfile import gettempdir
-from typing import Callable, Union
+from typing import Callable, Iterator, Optional
 
 import pytest
-import pymongo
 from mirakuru import TCPExecutor
-from _pytest.fixtures import FixtureRequest
 from port_for import get_port
+from port_for.api import PortType
+from pymongo import MongoClient
+from pytest import FixtureRequest
 
+from pytest_mongo.config import get_config
 from pytest_mongo.executor_noop import NoopExecutor
 
 
-def get_config(request):
-    """Return a dictionary with config options."""
-    config = {}
-    options = ["exec", "host", "port", "params", "logsdir", "tz_aware"]
-    for option in options:
-        option_name = "mongo_" + option
-        conf = request.config.getoption(option_name) or request.config.getini(
-            option_name
-        )
-        config[option] = conf
-    return config
-
-
-def mongo_proc(executable=None, params=None, host=None, port=-1, logsdir=None):
-    """
-    Mongo process fixture factory.
+def mongo_proc(
+    executable: Optional[str] = None,
+    params: Optional[str] = None,
+    host: Optional[str] = None,
+    port: Optional[PortType] = -1,
+    logsdir: Optional[str] = None,
+) -> Callable[[FixtureRequest], Iterator[TCPExecutor]]:
+    """Mongo process fixture factory.
 
     .. note::
         `mongod <http://docs.mongodb.org/v2.2/reference/mongod/>`_
 
-    :param str executable: path to mongod
-    :param str params: params
-    :param str host: hostname
-    :param str|int|tuple|set|list port:
-        exact port (e.g. '8000', 8000)
-        randomly selected port (None) - any random available port
-        [(2000,3000)] or (2000,3000) - random available port from a given range
-        [{4002,4003}] or {4002,4003} - random of 4002 or 4003 ports
-        [(2000,3000), {4002,4003}] -random of given range and set
-    :param str logsdir: path to store log files.
-    :rtype: func
+    :param executable: path to mongod
+    :param params: params
+    :param host: hostname
+    :param port:
+    :param logsdir: path to store log files.
     :returns: function which makes a mongo process
     """
 
     @pytest.fixture(scope="session")
-    def mongo_proc_fixture(request):
-        """
-        Mongodb process fixture.
+    def mongo_proc_fixture(request: FixtureRequest) -> Iterator[TCPExecutor]:
+        """Mongodb process fixture.
 
         :param FixtureRequest request: fixture request object
         :rtype: mirakuru.TCPExecutor
         :returns: tcp executor
         """
         config = get_config(request)
         tmpdir = gettempdir()
 
         mongo_exec = executable or config["exec"]
         mongo_params = params or config["params"]
 
         mongo_host = host or config["host"]
+        assert mongo_host
         mongo_port = get_port(port) or get_port(config["port"])
+        assert mongo_port
 
         mongo_logsdir = logsdir or config["logsdir"]
         mongo_logpath = os.path.join(mongo_logsdir, f"mongo.{mongo_port}.log")
         mongo_db_path = os.path.join(tmpdir, f"mongo.{mongo_port}")
         os.mkdir(mongo_db_path)
-        request.addfinalizer(
-            lambda: os.path.exists(mongo_db_path) and rmtree(mongo_db_path)
-        )
 
         mongo_executor = TCPExecutor(
             (
                 f"{mongo_exec} --bind_ip {mongo_host} --port {mongo_port} "
                 f"--dbpath {mongo_db_path} "
                 f"--logpath {mongo_logpath} {mongo_params}"
             ),
             host=mongo_host,
             port=mongo_port,
             timeout=60,
         )
-        mongo_executor.start()
-
-        request.addfinalizer(mongo_executor.stop)
-
-        return mongo_executor
+        with mongo_executor:
+            yield mongo_executor
+        os.path.exists(mongo_db_path)
+        rmtree(mongo_db_path)
 
     return mongo_proc_fixture
 
 
 def mongo_noproc(
-    host: str = None, port: Union[str, int] = None
-) -> Callable[[FixtureRequest], NoopExecutor]:
-    """
-    MongoDB noprocess factory.
+    host: Optional[str] = None, port: Optional[int] = None
+) -> Callable[[FixtureRequest], Iterator[NoopExecutor]]:
+    """MongoDB noprocess factory.
 
     :param host: hostname
     :param port: exact port (e.g. '8000', 8000)
     :param user: MongoDB username
     :param password: MongoDB password
     :param options: MongoDB connection options
     :returns: function which makes a postgresql process
     """
 
     @pytest.fixture(scope="session")
-    def mongo_noproc_fixture(request: FixtureRequest) -> NoopExecutor:
-        """
-        Noop Process fixture for MongoDB.
+    def mongo_noproc_fixture(request: FixtureRequest) -> Iterator[NoopExecutor]:
+        """Noop Process fixture for MongoDB.
 
         :param FixtureRequest request: fixture request object
         :returns: tcp executor-like object
         """
         config = get_config(request)
         mongo_host = host or config["host"]
         mongo_port = port or config["port"] or 27017
+        assert mongo_port
 
         noop_exec = NoopExecutor(host=mongo_host, port=mongo_port)
 
         yield noop_exec
 
     return mongo_noproc_fixture
 
 
-def mongodb(process_fixture_name, tz_aware=None):
-    """
-    Mongo database factory.
+def mongodb(
+    process_fixture_name: str, tz_aware: Optional[bool] = None
+) -> Callable[[FixtureRequest], Iterator[MongoClient]]:
+    """Mongo database factory.
 
     :param str process_fixture_name: name of the process fixture
     :param bool tz_aware: whether the client to be timezone aware or not
     :rtype: func
     :returns: function which makes a connection to mongo
     """
 
     @pytest.fixture
-    def mongodb_factory(request):
-        """
-        Client fixture for MongoDB.
+    def mongodb_factory(request: FixtureRequest) -> Iterator[MongoClient]:
+        """Client fixture for MongoDB.
 
         :param FixtureRequest request: fixture request object
         :rtype: pymongo.connection.Connection
         :returns: connection to mongo database
         """
         mongodb_process = request.getfixturevalue(process_fixture_name)
         config = get_config(request)
@@ -170,17 +154,17 @@
             config["tz_aware"], bool
         ):
             mongo_tz_aware = config["tz_aware"]
 
         mongo_host = mongodb_process.host
         mongo_port = mongodb_process.port
 
-        client = pymongo.MongoClient
-
-        mongo_conn = client(mongo_host, mongo_port, tz_aware=mongo_tz_aware)
+        mongo_conn: MongoClient = MongoClient(
+            mongo_host, mongo_port, tz_aware=mongo_tz_aware
+        )
 
         yield mongo_conn
 
         for db_name in mongo_conn.list_database_names():
             database = mongo_conn[db_name]
             for collection_name in database.list_collection_names():
                 collection = database[collection_name]
```

### Comparing `pytest-mongo-2.1.1/src/pytest_mongo/plugin.py` & `pytest-mongo-3.0.0/pytest_mongo/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-mongo.  If not, see <http://www.gnu.org/licenses/>.
 """Pytest-mongo plugin definition."""
 from tempfile import gettempdir
 
+from pytest import Parser
+
 from pytest_mongo import factories
 
 # pylint:disable=invalid-name
 _help_executable = "Path to MongoDB executable"
 _help_logsdir = "Path to logs directory"
 _help_params = "Additional MongoDB parameters"
 _help_host = "Host at which MongoDB will accept connections"
 _help_port = "Port at which MongoDB will accept connections"
 _help_tz_aware = "Have mongo client timezone aware"
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     """Configure pytest-mongo configuration options."""
     parser.addini(
         name="mongo_exec", help=_help_executable, default="/usr/bin/mongod"
     )
 
     parser.addini(name="mongo_params", help=_help_params, default="")
```

