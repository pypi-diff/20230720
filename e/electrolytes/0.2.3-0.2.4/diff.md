# Comparing `tmp/electrolytes-0.2.3.tar.gz` & `tmp/electrolytes-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.2.3.tar", last modified: Mon Jul 17 05:53:39 2023, max compression
+gzip compressed data, was "electrolytes-0.2.4.tar", last modified: Thu Jul 20 21:42:38 2023, max compression
```

## Comparing `electrolytes-0.2.3.tar` & `electrolytes-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.449792 electrolytes-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-17 05:53:26.000000 electrolytes-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-17 05:53:39.449792 electrolytes-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-17 05:53:26.000000 electrolytes-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-17 05:53:26.000000 electrolytes-0.2.3/electrolytes/db1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 05:53:39.000000 electrolytes-0.2.3/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-17 05:53:26.000000 electrolytes-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 05:53:39.449792 electrolytes-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 05:53:26.000000 electrolytes-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:53:39.445792 electrolytes-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 05:53:26.000000 electrolytes-0.2.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 05:53:26.000000 electrolytes-0.2.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-20 21:42:28.000000 electrolytes-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-20 21:42:38.151828 electrolytes-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-20 21:42:28.000000 electrolytes-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-20 21:42:28.000000 electrolytes-0.2.4/electrolytes/db1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 21:42:38.000000 electrolytes-0.2.4/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-20 21:42:28.000000 electrolytes-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:42:38.151828 electrolytes-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:42:38.151828 electrolytes-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 21:42:28.000000 electrolytes-0.2.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-20 21:42:28.000000 electrolytes-0.2.4/tests/test_cli.py
```

### Comparing `electrolytes-0.2.3/LICENSE.txt` & `electrolytes-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.3/PKG-INFO` & `electrolytes-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.3
+Version: 0.2.4
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -33,14 +33,15 @@
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
```

### Comparing `electrolytes-0.2.3/README.md` & `electrolytes-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
```

### Comparing `electrolytes-0.2.3/electrolytes/__init__.py` & `electrolytes-0.2.4/electrolytes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from warnings import warn
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from typer import get_app_dir
 
 _APP_NAME = "electrolytes"
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 
 class Constituent(BaseModel):
     model_config = ConfigDict(populate_by_name=True, validate_default=True)
 
     id: int = -1
     name: str
```

### Comparing `electrolytes-0.2.3/electrolytes/__main__.py` & `electrolytes-0.2.4/electrolytes/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from . import _APP_NAME, database, Constituent
 
 
 app = typer.Typer()
 
 
-def complete_name(ctx: Context, patam: Parameter, incomplete: str) -> List[str]:
+def complete_name(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
     return [name for name in database if name.startswith(incomplete)]
 
-def complete_name_user_defined(ctx: Context, patam: Parameter, incomplete: str) -> List[str]:
+def complete_name_user_defined(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
     return [name for name in database.user_defined() if name.startswith(incomplete)]
 
 
 @app.command()
 def add(name: str = typer.Argument(..., shell_complete=complete_name_user_defined),
         p1: Tuple[float, float] = typer.Option((None, None), "+1", help="Mobility (*1e-9) and pKa for +1"),
         p2: Tuple[float, float] = typer.Option((None, None), "+2", help="Mobility (*1e-9) and pKa for +2"),
@@ -84,14 +84,16 @@
         typer.echo(f"Error: {e}", err=True)
         raise typer.Exit(code=1)
 
 
 @app.command()
 def info(name: str = typer.Argument(..., shell_complete=complete_name)) -> None:
     """Show the properties of a component"""
+    name = name.upper()
+
     try:
         constituent = database[name]
     except KeyError:
         typer.echo(f"Error: {name}: no such component", err=True)
         raise typer.Exit(code=1)
 
     charges = list(constituent.charges_pos[::-1]) + list(constituent.charges_neg[::-1])
```

### Comparing `electrolytes-0.2.3/electrolytes/db1.json` & `electrolytes-0.2.4/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.3/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.2.4/electrolytes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.3
+Version: 0.2.4
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -33,14 +33,15 @@
 
 [![CI](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml/badge.svg)](https://github.com/microfluidica/electrolytes/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/microfluidica/electrolytes/branch/main/graph/badge.svg)](https://codecov.io/gh/microfluidica/electrolytes)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
 **electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
```

### Comparing `electrolytes-0.2.3/pyproject.toml` & `electrolytes-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.3/tests/test_api.py` & `electrolytes-0.2.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.3/tests/test_cli.py` & `electrolytes-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

