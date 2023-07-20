# Comparing `tmp/mazely-0.1.1.tar.gz` & `tmp/mazely-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazely-0.1.1.tar", last modified: Sat Jul  8 10:10:25 2023, max compression
+gzip compressed data, was "mazely-0.2.0.tar", last modified: Thu Jul 20 16:04:48 2023, max compression
```

## Comparing `mazely-0.1.1.tar` & `mazely-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.436617 mazely-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-06-21 09:11:43.000000 mazely-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3684 2023-07-08 10:10:25.437618 mazely-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2858 2023-07-08 09:33:51.000000 mazely-0.1.1/README.md
--rw-rw-rw-   0        0        0       50 2023-07-08 09:33:50.000000 mazely-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-07-03 09:38:28.000000 mazely-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0     1036 2023-07-08 10:10:25.438617 mazely-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-07-08 09:33:50.000000 mazely-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.404159 mazely-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.415212 mazely-0.1.1/src/mazely/
--rw-rw-rw-   0        0        0      189 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/__about__.py
--rw-rw-rw-   0        0        0      160 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.436617 mazely-0.1.1/src/mazely/algorithms/
--rw-rw-rw-   0        0        0      180 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/__init__.py
--rw-rw-rw-   0        0        0     2806 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/maze_generator.py
--rw-rw-rw-   0        0        0      812 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/maze_solver.py
--rw-rw-rw-   0        0        0     2351 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/recursive_backtracking.py
--rw-rw-rw-   0        0        0     2546 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/algorithms/shortest_path.py
--rw-rw-rw-   0        0        0     7367 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/maze.py
--rw-rw-rw-   0        0        0     8466 2023-07-08 09:33:50.000000 mazely-0.1.1/src/mazely/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-08 10:10:25.432618 mazely-0.1.1/src/mazely.egg-info/
--rw-rw-rw-   0        0        0     3684 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 10:10:25.000000 mazely-0.1.1/src/mazely.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.556498 mazely-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 16:04:34.000000 mazely-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 16:04:34.000000 mazely-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-20 16:04:48.556498 mazely-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-20 16:04:34.000000 mazely-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.540497 mazely-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.552498 mazely-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1004137 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/128x128-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   776824 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/16x16-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/2015apec-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/2015apec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    51473 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/2019japan-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41803 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/2019japan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  3534296 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/256x256-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  3159360 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   242116 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/32x128-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   193200 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/32x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    63775 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/32x32-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    48108 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/32x32.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   230361 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/64x64-solution.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   188175 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/images/64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.552498 mazely-0.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/reference/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/reference/maze.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-20 16:04:34.000000 mazely-0.2.0/docs/usage_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-20 16:04:34.000000 mazely-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:04:48.556498 mazely-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.536496 mazely-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.552498 mazely-0.2.0/src/mazely/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.556498 mazely-0.2.0/src/mazely/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/algorithms/maze_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/algorithms/maze_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/algorithms/recursive_backtracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/algorithms/shortest_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/maze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-20 16:04:34.000000 mazely-0.2.0/src/mazely/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.556498 mazely-0.2.0/src/mazely.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-20 16:04:48.000000 mazely-0.2.0/src/mazely.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-20 16:04:48.000000 mazely-0.2.0/src/mazely.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:04:48.000000 mazely-0.2.0/src/mazely.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 16:04:48.000000 mazely-0.2.0/src/mazely.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 16:04:48.000000 mazely-0.2.0/src/mazely.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.556498 mazely-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:04:48.556498 mazely-0.2.0/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/baseline/_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/baseline/hashes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/test_maze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/test_maze_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/test_maze_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-20 16:04:34.000000 mazely-0.2.0/tests/test_utilities.py
```

### Comparing `mazely-0.1.1/LICENSE` & `mazely-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Kenneth C.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Kenneth C.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mazely-0.1.1/PKG-INFO` & `mazely-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,148 @@
-Metadata-Version: 2.1
-Name: mazely
-Version: 0.1.1
-Summary: Implementation of maze-related algorithms
-Author: Kenneth C.
-License: MIT
-Project-URL: Documentation, https://mazely.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/Munckenh/mazely
-Keywords: mazely,maze,algorithms
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
-</p>
-
-# mazely
-
-[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](http://choosealicense.com/licenses/mit/)
-[![Read the Docs](https://img.shields.io/readthedocs/mazely)](http://mazely.readthedocs.io/)
-
-An API for solving and generating mazes, written in Python.
-
-## Documentation
-
-A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
-
-## Usage examples
-
-Run the Python scripts below from the repository directory.
-
-Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
-
-### Load and display a maze
-
-Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2015apec.maze")
-utils = Utilities()
-utils.show_grid(maze.grid)
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
-</p>
-
-### Solve a maze and display its solution
-
-A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2019japan.maze")
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
-</p>
-
-### Generate a maze and display its solution
-
-To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(32, 32)
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
-</p>
-
-## Maze files
-
-The library only supports a single maze format, as specified below.
-
-### File format
-
-Each cell is 3 characters wide and 3 characters tall.
-
-```
-+---+
-|   |
-+---+
-```
-
-To specify the goal cell, replace the center with `G`.
-
-```
-+---+
-| G |
-+---+
-```
-
-And replace with `S` for the start cell.
-
-```
-+---+
-| S |
-+---+
-```
-
-Here is an example of a 3x3 maze.
-
-```
-+---+---+---+
-|           |
-+   +---+   +
-|     G |   |
-+---+---+   +
-| S         |
-+---+---+---+
-```
-
-### Links
-
-Here are a couple links to collections of maze files (format may not be supported):
-
-- <https://github.com/micromouseonline/mazefiles>
-- <http://www.tcp4me.com/mmr/mazes/>
+Metadata-Version: 2.1
+Name: mazely
+Version: 0.2.0
+Summary: Implementation of maze-related algorithms
+Author: Kenneth C.
+License: MIT License
+Project-URL: Documentation, https://mazely.readthedocs.io
+Project-URL: Repository, https://github.com/Munckenh/mazely.git
+Keywords: mazely,maze,algorithms
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+<h1 align="center">Mazely</h1>
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
+</p>
+
+[![PyPI version](https://img.shields.io/pypi/v/mazely.svg)](https://pypi.org/project/mazely/)
+[![MIT License](https://img.shields.io/github/license/Munckenh/mazely
+)](https://choosealicense.com/licenses/mit/)
+[![Read the Docs](https://img.shields.io/readthedocs/mazely)](https://mazely.readthedocs.io/)
+[![GitHub workflow status](https://img.shields.io/github/actions/workflow/status/Munckenh/mazely/tests.yml?label=test)](https://github.com/Munckenh/mazely/actions?query=workflow%3ATests)
+
+An API for solving and generating mazes, written in Python.
+
+## Installation
+
+Install `mazely` with [pip](https://pip.pypa.io/en/stable/getting-started/):
+
+```shell
+pip install mazely
+```
+
+## Documentation
+
+A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
+
+## Usage examples
+
+Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
+
+### Load and display a maze
+
+Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2015apec.maze")
+utils = Utilities()
+utils.show_grid(maze.grid)
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
+</p>
+
+### Solve a maze and display its solution
+
+A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2019japan.maze")
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
+</p>
+
+### Generate a maze and display its solution
+
+To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(32, 32)
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
+</p>
+
+## Maze files
+
+The library only supports a single maze format, as specified below.
+
+### File format
+
+Each cell is 3 characters wide and 3 characters tall.
+
+```
++---+
+|   |
++---+
+```
+
+To specify the goal cell, replace the center with `G`.
+
+```
++---+
+| G |
++---+
+```
+
+And replace with `S` for the start cell.
+
+```
++---+
+| S |
++---+
+```
+
+Here is an example of a 3x3 maze.
+
+```
++---+---+---+
+|           |
++   +---+   +
+|     G |   |
++---+---+   +
+| S         |
++---+---+---+
+```
+
+### Links
+
+Here are a couple links to collections of maze files (format may not be supported):
+
+- <https://github.com/micromouseonline/mazefiles>
+- <http://www.tcp4me.com/mmr/mazes/>
```

### Comparing `mazely-0.1.1/README.md` & `mazely-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,125 @@
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
-</p>
-
-# mazely
-
-[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](http://choosealicense.com/licenses/mit/)
-[![Read the Docs](https://img.shields.io/readthedocs/mazely)](http://mazely.readthedocs.io/)
-
-An API for solving and generating mazes, written in Python.
-
-## Documentation
-
-A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
-
-## Usage examples
-
-Run the Python scripts below from the repository directory.
-
-Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
-
-### Load and display a maze
-
-Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2015apec.maze")
-utils = Utilities()
-utils.show_grid(maze.grid)
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
-</p>
-
-### Solve a maze and display its solution
-
-A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2019japan.maze")
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
-</p>
-
-### Generate a maze and display its solution
-
-To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(32, 32)
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
-</p>
-
-## Maze files
-
-The library only supports a single maze format, as specified below.
-
-### File format
-
-Each cell is 3 characters wide and 3 characters tall.
-
-```
-+---+
-|   |
-+---+
-```
-
-To specify the goal cell, replace the center with `G`.
-
-```
-+---+
-| G |
-+---+
-```
-
-And replace with `S` for the start cell.
-
-```
-+---+
-| S |
-+---+
-```
-
-Here is an example of a 3x3 maze.
-
-```
-+---+---+---+
-|           |
-+   +---+   +
-|     G |   |
-+---+---+   +
-| S         |
-+---+---+---+
-```
-
-### Links
-
-Here are a couple links to collections of maze files (format may not be supported):
-
-- <https://github.com/micromouseonline/mazefiles>
-- <http://www.tcp4me.com/mmr/mazes/>
+<h1 align="center">Mazely</h1>
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
+</p>
+
+[![PyPI version](https://img.shields.io/pypi/v/mazely.svg)](https://pypi.org/project/mazely/)
+[![MIT License](https://img.shields.io/github/license/Munckenh/mazely
+)](https://choosealicense.com/licenses/mit/)
+[![Read the Docs](https://img.shields.io/readthedocs/mazely)](https://mazely.readthedocs.io/)
+[![GitHub workflow status](https://img.shields.io/github/actions/workflow/status/Munckenh/mazely/tests.yml?label=test)](https://github.com/Munckenh/mazely/actions?query=workflow%3ATests)
+
+An API for solving and generating mazes, written in Python.
+
+## Installation
+
+Install `mazely` with [pip](https://pip.pypa.io/en/stable/getting-started/):
+
+```shell
+pip install mazely
+```
+
+## Documentation
+
+A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
+
+## Usage examples
+
+Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
+
+### Load and display a maze
+
+Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2015apec.maze")
+utils = Utilities()
+utils.show_grid(maze.grid)
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
+</p>
+
+### Solve a maze and display its solution
+
+A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2019japan.maze")
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
+</p>
+
+### Generate a maze and display its solution
+
+To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(32, 32)
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
+</p>
+
+## Maze files
+
+The library only supports a single maze format, as specified below.
+
+### File format
+
+Each cell is 3 characters wide and 3 characters tall.
+
+```
++---+
+|   |
++---+
+```
+
+To specify the goal cell, replace the center with `G`.
+
+```
++---+
+| G |
++---+
+```
+
+And replace with `S` for the start cell.
+
+```
++---+
+| S |
++---+
+```
+
+Here is an example of a 3x3 maze.
+
+```
++---+---+---+
+|           |
++   +---+   +
+|     G |   |
++---+---+   +
+| S         |
++---+---+---+
+```
+
+### Links
+
+Here are a couple links to collections of maze files (format may not be supported):
+
+- <https://github.com/micromouseonline/mazefiles>
+- <http://www.tcp4me.com/mmr/mazes/>
```

### Comparing `mazely-0.1.1/src/mazely/algorithms/maze_generator.py` & `mazely-0.2.0/src/mazely/algorithms/maze_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,79 @@
-import numpy as np
-
-
-class MazeGenerator:
-    """A base class for maze-generating algorithms."""
-
-    def __init__(self):
-        self._grid = None
-
-    def _remove_wall(self, cell: tuple[int, int], neighbor: tuple[int, int]):
-        """Remove the wall between a cell and its neighbor.
-
-        Parameters
-        ----------
-        cell : tuple[int, int]
-            The location of the cell.
-        neighbor : tuple[int, int]
-            The location of the cell's neighbor.
-        """
-        if cell[1] == neighbor[1]:  # If both cells share the same column.
-            # +---+
-            # | C |
-            # +---+
-            # | N |
-            # +---+
-            if cell[0] < neighbor[0]:
-                self._grid[cell[0]][cell[1]][1] = False
-                self._grid[neighbor[0]][neighbor[1]][0] = False
-            
-            # +---+
-            # | N |
-            # +---+
-            # | C |
-            # +---+
-            else:
-                self._grid[cell[0]][cell[1]][0] = False
-                self._grid[neighbor[0]][neighbor[1]][1] = False
-
-        elif cell[0] == neighbor[0]:  # If both cells share the same row.
-            # +---+---+
-            # | C | N |
-            # +---+---+
-            if cell[1] < neighbor[1]:
-                self._grid[cell[0]][cell[1]][2] = False
-                self._grid[neighbor[0]][neighbor[1]][3] = False
-
-            # +---+---+
-            # | N | C |
-            # +---+---+
-            else:
-                self._grid[cell[0]][cell[1]][3] = False
-                self._grid[neighbor[0]][neighbor[1]][2] = False
-
-    def _initiate_grid(self, rows: int, columns: int, walls: bool = False):
-        """Initiate a two-dimensional list of each cell's wall data.
-
-        The wall data is a list consisting of four Boolean values in NSEW order.
-
-        Parameters
-        ----------
-        rows : int
-            The total number of rows of the maze.
-        columns : int
-            The total number of columns of the maze.
-        walls : bool
-            Whether to initiate all the cell with walls. Defaults to ``False``.
-        """
-
-        self._grid = np.full((rows, columns, 4), [walls] * 4)
-
-    def generate(self, rows: int, columns: int):
-        """An abstract method to generate a maze.
-
-        Parameters
-        ----------
-        rows : int
-            The total number of rows of the maze.
-        columns : int
-            The total number of columns of the maze.
-
-        Raises
-        ------
-        NotImplementedError
-            If the method has not been implemented in a subclass.
-        """
-        raise NotImplementedError(
-            "The 'generate()' method must be implemented in the subclass."
-        )
+import numpy as np
+
+
+class MazeGenerator:
+    """A base class for maze-generating algorithms."""
+
+    def __init__(self):
+        self._grid = None
+
+    def _remove_wall(self, cell: tuple[int, int], neighbor: tuple[int, int]):
+        """Remove the wall between a cell and its neighbor.
+
+        Parameters
+        ----------
+        cell : tuple[int, int]
+            The location of the cell.
+        neighbor : tuple[int, int]
+            The location of the cell's neighbor.
+        """
+        if cell[1] == neighbor[1]:  # If both cells share the same column.
+            if cell[0] < neighbor[0]:
+                self._grid[cell[0]][cell[1]][1] = False
+                self._grid[neighbor[0]][neighbor[1]][0] = False
+            else:
+                self._grid[cell[0]][cell[1]][0] = False
+                self._grid[neighbor[0]][neighbor[1]][1] = False
+
+        elif cell[0] == neighbor[0]:  # If both cells share the same row.
+            if cell[1] < neighbor[1]:
+                self._grid[cell[0]][cell[1]][2] = False
+                self._grid[neighbor[0]][neighbor[1]][3] = False
+            else:
+                self._grid[cell[0]][cell[1]][3] = False
+                self._grid[neighbor[0]][neighbor[1]][2] = False
+
+    def _initiate_grid(self, rows: int, columns: int, walls: bool = False):
+        """Initiate a two-dimensional list of each cell's wall data.
+
+        The wall data is a list consisting of four Boolean values in NSEW
+        order.
+
+        Parameters
+        ----------
+        rows : int
+            The total number of rows of the maze.
+        columns : int
+            The total number of columns of the maze.
+        walls : bool
+            Whether to initiate all the cell with walls. Defaults to ``False``.
+        """
+
+        self._grid = np.full((rows, columns, 4), [walls] * 4)
+
+    def generate(
+        self,
+        rows: int,
+        columns: int,
+        seed: int | None = None
+    ) -> np.ndarray:
+        """An abstract method to generate a maze.
+
+        Parameters
+        ----------
+        rows : int
+            The total number of rows of the maze.
+        columns : int
+            The total number of columns of the maze.
+        seed : int, optional
+            The seed value used to initialize the random number generator.
+            Defaults to ``None``.
+
+        Raises
+        ------
+        NotImplementedError
+            If the method has not been implemented in a subclass.
+        """
+        raise NotImplementedError(
+            "The 'generate()' method must be implemented in the subclass."
+        )
```

### Comparing `mazely-0.1.1/src/mazely/algorithms/recursive_backtracking.py` & `mazely-0.2.0/src/mazely/algorithms/recursive_backtracking.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,85 @@
-import random
-import sys
-
-import numpy as np
-
-from .maze_generator import MazeGenerator
-
-
-class RecursiveBacktracking(MazeGenerator):
-    """A maze-generating algorithm that creates a perfect maze using a randomized version of depth-first search."""
-
-    def __init__(self):
-        super().__init__()
-        self._visited = None
-
-    def _visit_cell(self, row, column):
-        """Visit a cell using recursive backtracking.
-
-        Parameters
-        ----------
-        row : int
-            The row of the cell to be visited.
-        column : int
-            The column of the cell to be visited.
-        """
-        self._visited.add((row, column))  # Mark current cell as visited
-
-        # Iterate over the four directions in a randomized order
-        for row_delta, column_delta in random.sample(
-            ((-1, 0), (0, 1), (1, 0), (0, -1)), k=4
-        ):
-            # Get a random neighbor's row and column
-            neighbor = (row + row_delta, column + column_delta)
-
-            # See if the neighbor exists
-            if (
-                neighbor[0] < 0
-                or neighbor[0] >= len(self._grid)
-                or neighbor[1] < 0
-                or neighbor[1] >= len(self._grid[0])
-            ):
-                continue
-
-            # See if the neighbor is already visited
-            if neighbor in self._visited:
-                continue
-
-            # Remove the wall between the current cell and the selected neighbor
-            self._remove_wall((row, column), neighbor)
-
-            # Visit the neighbor recursively
-            self._visit_cell(neighbor[0], neighbor[1])
-
-    def generate(self, rows: int, columns: int) -> np.ndarray:
-        """Generate a maze.
-
-        Parameters
-        ----------
-        rows : int
-            The total number of rows of the maze.
-        columns : int
-            The total number of columns of the maze.
-
-        Returns
-        -------
-        numpy.ndarray
-            A two-dimensional array of cells representing a rectangular maze.
-        """
-        sys.setrecursionlimit(max(1000, rows * columns))
-        self._visited = set()
-        self._initiate_grid(rows, columns, walls=True)
-        self._visit_cell(random.randrange(rows), random.randrange(columns))
-        return self._grid
+import random
+import sys
+
+import numpy as np
+
+from .maze_generator import MazeGenerator
+
+
+class RecursiveBacktracking(MazeGenerator):
+    """A maze-generating algorithm that creates a perfect maze using a
+    randomized version of depth-first search."""
+
+    def __init__(self):
+        super().__init__()
+        self._visited = None
+
+    def _visit_cell(self, row, column):
+        """Visit a cell using recursive backtracking.
+
+        Parameters
+        ----------
+        row : int
+            The row of the cell to be visited.
+        column : int
+            The column of the cell to be visited.
+        """
+        self._visited.add((row, column))  # Mark current cell as visited
+
+        # Iterate over the four directions in a randomized order
+        for row_delta, column_delta in random.sample(
+            ((-1, 0), (1, 0), (0, 1), (0, -1)), k=4
+        ):
+            # Get a random neighbor's row and column
+            neighbor = (row + row_delta, column + column_delta)
+
+            # See if the neighbor exists
+            if (
+                neighbor[0] < 0
+                or neighbor[0] >= len(self._grid)
+                or neighbor[1] < 0
+                or neighbor[1] >= len(self._grid[0])
+            ):
+                continue
+
+            # See if the neighbor is already visited
+            if neighbor in self._visited:
+                continue
+
+            # Remove the wall between the current cell and the selected
+            # neighbor
+            self._remove_wall((row, column), neighbor)
+
+            # Visit the neighbor recursively
+            self._visit_cell(neighbor[0], neighbor[1])
+
+    def generate(
+        self,
+        rows: int,
+        columns: int,
+        seed: int | None = None
+    ) -> np.ndarray:
+        """Generate a maze.
+
+        Parameters
+        ----------
+        rows : int
+            The total number of rows of the maze.
+        columns : int
+            The total number of columns of the maze.
+        seed : int, optional
+            The seed value used to initialize the random number generator.
+            Defaults to ``None``
+
+        Returns
+        -------
+        numpy.ndarray
+            A two-dimensional array of cells representing a rectangular maze.
+        """
+
+        sys.setrecursionlimit(max(1000, rows * columns))
+        random.seed(seed)
+        self._visited = set()
+        self._initiate_grid(rows, columns, walls=True)
+        self._visit_cell(random.randrange(rows), random.randrange(columns))
+        return self._grid
```

### Comparing `mazely-0.1.1/src/mazely/algorithms/shortest_path.py` & `mazely-0.2.0/src/mazely/algorithms/shortest_path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,83 @@
-from collections import deque
-
-import numpy as np
-
-from .maze_solver import MazeSolver
-
-
-class ShortestPath(MazeSolver):
-    """A maze-solving algorithm that finds the shortest path using breadth-first search."""
-
-    def __init__(self):
-        pass
-
-    def solve(
-        self, grid: np.ndarray, start: tuple[int, int], goal: set[tuple[int, int]]
-    ) -> list[tuple[int, int]]:
-        """Solve the maze.
-
-        Parameters
-        ----------
-        grid : numpy.ndarray
-            A two-dimensional array of cells representing a rectangular maze.
-        start : tuple[int, int]
-            The location of the start cell.
-        goal : set[tuple[int, int]]
-            The location(s) of the goal cell(s).
-
-        Returns
-        -------
-        list[tuple[int, int]]
-            An ordered list of cell locations representing the solution path.
-        """
-        queue = deque([start])
-        visited = set()
-        path = {}
-        index_delta = ((-1, 0), (1, 0), (0, 1), (0, -1))
-
-        # Loop until the queue is empty.
-        while queue:
-            # Get the next cell.
-            current = queue.popleft()
-
-            # Save the solution path and break the loop if the current cell is the goal.
-            if current in goal:
-                solution_path = []
-
-                # Loop until the current cell is the start cell.
-                while current is not start:
-                    # Append current cell to the solution path.
-                    solution_path.append(current)
-
-                    # Get the next cell.
-                    current = path[current]
-                else:
-                    solution_path.append(start)
-
-                # Reverse the order of the list to get a proper solution path.
-                solution_path.reverse()
-
-                return solution_path
-
-            # Add the current cell to the visited list.
-            visited.add(current)
-
-            for direction, wall in enumerate(grid[current[0]][current[1]]):
-                if not wall:
-                    neighbor = (
-                        current[0] + index_delta[direction][0],
-                        current[1] + index_delta[direction][1],
-                    )
-
-                    # If the neighbor is not in the visited list.
-                    if neighbor not in visited:
-                        queue.append(neighbor)  # Add the neighbor to the queue.
-                        path[neighbor] = current  # Store the path.
+from collections import deque
+
+import numpy as np
+
+from .maze_solver import MazeSolver
+
+
+class ShortestPath(MazeSolver):
+    """A maze-solving algorithm that finds the shortest path using
+    breadth-first search."""
+
+    def __init__(self):
+        pass
+
+    def solve(
+        self,
+        grid: np.ndarray,
+        start: tuple[int, int],
+        goal: set[tuple[int, int]]
+    ) -> list[tuple[int, int]]:
+        """Solve the maze.
+
+        Parameters
+        ----------
+        grid : numpy.ndarray
+            A two-dimensional array of cells representing a rectangular maze.
+        start : tuple[int, int]
+            The location of the start cell.
+        goal : set[tuple[int, int]]
+            The location(s) of the goal cell(s).
+
+        Returns
+        -------
+        list[tuple[int, int]]
+            An ordered list of cell locations representing the solution path.
+        """
+        queue = deque([start])
+        visited = set()
+        path = {}
+        index_delta = ((-1, 0), (1, 0), (0, 1), (0, -1))
+
+        # Loop until the queue is empty.
+        while queue:
+            # Get the next cell.
+            current = queue.popleft()
+            # Save the solution path and break the loop if the current cell is
+            # the goal.
+            if current in goal:
+                solution_path = []
+
+                # Loop until the current cell is the start cell.
+                while current is not start:
+                    # Append current cell to the solution path.
+                    solution_path.append(current)
+
+                    # Get the next cell.
+                    current = path[current]
+                else:
+                    solution_path.append(start)
+
+                # Reverse the order of the list to get a proper solution path.
+                solution_path.reverse()
+
+                return solution_path
+
+            # Add the current cell to the visited list.
+            visited.add(current)
+
+            for direction, wall in enumerate(grid[current[0]][current[1]]):
+                if not wall:
+                    neighbor = (
+                        current[0] + index_delta[direction][0],
+                        current[1] + index_delta[direction][1],
+                    )
+
+                    # If the neighbor is not in the visited list.
+                    if neighbor not in visited:
+
+                        # Add the neighbor to the queue.
+                        queue.append(neighbor)
+
+                        # Store the path.
+                        path[neighbor] = current
```

### Comparing `mazely-0.1.1/src/mazely.egg-info/PKG-INFO` & `mazely-0.2.0/src/mazely.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,148 @@
-Metadata-Version: 2.1
-Name: mazely
-Version: 0.1.1
-Summary: Implementation of maze-related algorithms
-Author: Kenneth C.
-License: MIT
-Project-URL: Documentation, https://mazely.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/Munckenh/mazely
-Keywords: mazely,maze,algorithms
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
-</p>
-
-# mazely
-
-[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](http://choosealicense.com/licenses/mit/)
-[![Read the Docs](https://img.shields.io/readthedocs/mazely)](http://mazely.readthedocs.io/)
-
-An API for solving and generating mazes, written in Python.
-
-## Documentation
-
-A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
-
-## Usage examples
-
-Run the Python scripts below from the repository directory.
-
-Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
-
-### Load and display a maze
-
-Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2015apec.maze")
-utils = Utilities()
-utils.show_grid(maze.grid)
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
-</p>
-
-### Solve a maze and display its solution
-
-A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(path="resources/2019japan.maze")
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
-</p>
-
-### Generate a maze and display its solution
-
-To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
-
-```py
-from mazely import Maze, Utilities
-
-maze = Maze(32, 32)
-utils = Utilities()
-utils.show_solution()
-```
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
-</p>
-
-## Maze files
-
-The library only supports a single maze format, as specified below.
-
-### File format
-
-Each cell is 3 characters wide and 3 characters tall.
-
-```
-+---+
-|   |
-+---+
-```
-
-To specify the goal cell, replace the center with `G`.
-
-```
-+---+
-| G |
-+---+
-```
-
-And replace with `S` for the start cell.
-
-```
-+---+
-| S |
-+---+
-```
-
-Here is an example of a 3x3 maze.
-
-```
-+---+---+---+
-|           |
-+   +---+   +
-|     G |   |
-+---+---+   +
-| S         |
-+---+---+---+
-```
-
-### Links
-
-Here are a couple links to collections of maze files (format may not be supported):
-
-- <https://github.com/micromouseonline/mazefiles>
-- <http://www.tcp4me.com/mmr/mazes/>
+Metadata-Version: 2.1
+Name: mazely
+Version: 0.2.0
+Summary: Implementation of maze-related algorithms
+Author: Kenneth C.
+License: MIT License
+Project-URL: Documentation, https://mazely.readthedocs.io
+Project-URL: Repository, https://github.com/Munckenh/mazely.git
+Keywords: mazely,maze,algorithms
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+<h1 align="center">Mazely</h1>
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x128-solution.svg" alt="Solved 32x128 maze">
+</p>
+
+[![PyPI version](https://img.shields.io/pypi/v/mazely.svg)](https://pypi.org/project/mazely/)
+[![MIT License](https://img.shields.io/github/license/Munckenh/mazely
+)](https://choosealicense.com/licenses/mit/)
+[![Read the Docs](https://img.shields.io/readthedocs/mazely)](https://mazely.readthedocs.io/)
+[![GitHub workflow status](https://img.shields.io/github/actions/workflow/status/Munckenh/mazely/tests.yml?label=test)](https://github.com/Munckenh/mazely/actions?query=workflow%3ATests)
+
+An API for solving and generating mazes, written in Python.
+
+## Installation
+
+Install `mazely` with [pip](https://pip.pypa.io/en/stable/getting-started/):
+
+```shell
+pip install mazely
+```
+
+## Documentation
+
+A library reference can be found [here](https://mazely.readthedocs.io/en/latest/).
+
+## Usage examples
+
+Also, see the [examples](https://github.com/Munckenh/mazely/tree/main/examples) folder.
+
+### Load and display a maze
+
+Create an instance of `Maze` and pass a path to a maze file to load an existing maze. Use the `show_grid()` method from `Utilities` to display a grid of the maze.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2015apec.maze")
+utils = Utilities()
+utils.show_grid(maze.grid)
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2015apec.svg" alt="APEC 2015">
+</p>
+
+### Solve a maze and display its solution
+
+A solution is always made when you create an instance of `Maze`. To display the solution, use the `show_solution()` method from `Utilities`.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(path="resources/2019japan.maze")
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/2019japan-solution.svg" alt="Japan 2019">
+</p>
+
+### Generate a maze and display its solution
+
+To generate a maze, pass the row and column counts as you create a `Maze` instance. Refer to the previous section to display its solution.
+
+```python
+from mazely import Maze, Utilities
+
+maze = Maze(32, 32)
+utils = Utilities()
+utils.show_solution()
+```
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Munckenh/mazely/main/docs/images/32x32-solution.svg" alt="Solved 32x32 maze">
+</p>
+
+## Maze files
+
+The library only supports a single maze format, as specified below.
+
+### File format
+
+Each cell is 3 characters wide and 3 characters tall.
+
+```
++---+
+|   |
++---+
+```
+
+To specify the goal cell, replace the center with `G`.
+
+```
++---+
+| G |
++---+
+```
+
+And replace with `S` for the start cell.
+
+```
++---+
+| S |
++---+
+```
+
+Here is an example of a 3x3 maze.
+
+```
++---+---+---+
+|           |
++   +---+   +
+|     G |   |
++---+---+   +
+| S         |
++---+---+---+
+```
+
+### Links
+
+Here are a couple links to collections of maze files (format may not be supported):
+
+- <https://github.com/micromouseonline/mazefiles>
+- <http://www.tcp4me.com/mmr/mazes/>
```

