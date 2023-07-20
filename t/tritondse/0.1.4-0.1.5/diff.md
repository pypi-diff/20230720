# Comparing `tmp/tritondse-0.1.4.tar.gz` & `tmp/tritondse-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.4.tar", last modified: Wed Jun 28 14:11:11 2023, max compression
+gzip compressed data, was "tritondse-0.1.5.tar", last modified: Thu Jul 20 12:42:02 2023, max compression
```

## Comparing `tritondse-0.1.4.tar` & `tritondse-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:11.890111 tritondse-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 14:11:06.000000 tritondse-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-28 14:11:11.890111 tritondse-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-28 14:11:06.000000 tritondse-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 14:11:11.890111 tritondse-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-28 14:11:06.000000 tritondse-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:11.890111 tritondse-0.1.4/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:11.890111 tritondse-0.1.4/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:11.890111 tritondse-0.1.4/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    50962 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    75538 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    35948 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-28 14:11:06.000000 tritondse-0.1.4/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:11:11.890111 tritondse-0.1.4/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-28 14:11:11.000000 tritondse-0.1.4/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-28 14:11:11.000000 tritondse-0.1.4/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:11:11.000000 tritondse-0.1.4/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-28 14:11:11.000000 tritondse-0.1.4/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 14:11:11.000000 tritondse-0.1.4/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 12:41:58.000000 tritondse-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-20 12:42:02.297245 tritondse-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-20 12:41:58.000000 tritondse-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:42:02.297245 tritondse-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-20 12:41:58.000000 tritondse-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29681 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50989 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35983 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.4/LICENSE` & `tritondse-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/PKG-INFO` & `tritondse-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.4 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.5 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.4/README.md` & `tritondse-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/setup.py` & `tritondse-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.4",
+    version="0.1.5",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.4/tritondse/__init__.py` & `tritondse-0.1.5/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/arch.py` & `tritondse-0.1.5/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/callbacks.py` & `tritondse-0.1.5/tritondse/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # built-in imports
 from __future__ import annotations
-import logging
 from enum import Enum, auto
 from typing import Callable, Tuple, List, Optional, Union, Any
 import enum_tools.documentation
 # third-party imports
 from triton import CALLBACK, Instruction, MemoryAccess, OPCODE
 
 # local imports
 from tritondse.process_state import ProcessState
 from tritondse.types import Addr, Input, Register, Expression, Edge, SymExType
 from tritondse.thread_context import ThreadContext
 from tritondse.seed import Seed
 from tritondse.memory import MemoryAccessViolation
+import tritondse.logging
+
+logger = tritondse.logging.get()  # get root tritondse logger
 
 
 @enum_tools.documentation.document_enum
 class CbPos(Enum):
     """ Enmus representing callback position """
     BEFORE = auto()  # doc: Callback should be executed before the hook location interpretation
     AFTER = auto()   # doc: Callback should be executed after the hook location interpreation
@@ -207,15 +209,15 @@
         IMPORTANT You MUST call `unbind` once you finish using the
         SymbolicExecutor.
 
         :param se: SymbolicExecutor on which to bind callbacks
         :type se: SymbolicExecutor
         """
         if self.is_binded() and self._se != se:
-            logging.warning("Callback_manager already binded (on a different executor instance)")
+            logger.warning("Callback_manager already binded (on a different executor instance)")
         # assert not self.is_binded()
 
         # NOTE This creates a circular dependency between the SymbolicExecutor
         #      received and this object, as the SymbolicExecutor keeps a
         #      reference to it. Therefore, it is necessary to call `unbind`
         #      once you finish using the executor.
         self._se = se
@@ -241,17 +243,17 @@
                 for fname in list(self._func_to_register):
                     cbs = self._func_to_register.pop(fname)
                     addr = se.loader.find_function_addr(fname)
                     if addr:
                         for cb in cbs:
                             self.register_pre_addr_callback(addr, cb)
                     else:
-                        logging.warning(f"can't find function '{fname}' in {se.loader}")
+                        logger.warning(f"can't find function '{fname}' in {se.loader}")
             else:
-                logging.warning(f"function callback to resolve but no program provided")
+                logger.warning(f"function callback to resolve but no program provided")
 
 
     def register_addr_callback(self, pos: CbPos, addr: Addr, callback: AddrCallback) -> None:
         """
         Register a callback function on a given address before or after the execution
         of the associated instruction.
```

### Comparing `tritondse-0.1.4/tritondse/config.py` & `tritondse-0.1.5/tritondse/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,20 @@
                  exploration_timeout: int = 0,
                  exploration_limit: int = 0,
                  thread_scheduling: int = 200,
                  smt_queries_limit: int = 1200,
                  smt_enumeration_limit: int = 40,
                  coverage_strategy: CoverageStrategy = CoverageStrategy.BLOCK,
                  branch_solving_strategy: BranchSolvingStrategy = BranchSolvingStrategy.FIRST_LAST_NOT_COVERED,
-                 debug: bool = False,
                  workspace: str = "",
                  program_argv: List[str] = None,
                  time_inc_coefficient: float = 0.00001,
                  skip_unsupported_import: bool = False,
                  skip_unsupported_instruction: bool = False,
                  memory_segmentation: bool = True):
-        """
-        :param debug: Enable debugging logging
-        :type debug: bool
-        """
 
         self.seed_format: SeedFormat = seed_format
         """ Seed type is either Raw (raw bytes) or Composite (more expressive).
             See seeds.py for more information on each format.
         """
         
         self.pipe_stdout: bool = pipe_stdout
@@ -89,19 +84,14 @@
 
         self.branch_solving_strategy: BranchSolvingStrategy = branch_solving_strategy
         """ Branch solving strategy to apply for a single execution. For a given non-covered
         branch allows changing whether we try to solve it at all occurences or more seldomly.
         default: :py:obj:`BranchSolvingStrategy.FIRST_LAST_NOT_COVERED`
         """
 
-        self.debug: bool = debug
-        """ Enable debug logging or not. Value taken from constructor.
-        FIXME: What if the value is changed during execution ?
-        """
-
         self.workspace: str = workspace
         """ Workspace directory to use. *(default: 'workspace')* """
 
         self.program_argv: List[str] = [] if program_argv is None else program_argv
         """ Concrete program argument as given on the command line."""
 
         self.time_inc_coefficient: float = time_inc_coefficient
```

### Comparing `tritondse-0.1.4/tritondse/coverage.py` & `tritondse-0.1.5/tritondse/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # built-in imports
 from __future__ import annotations
-import json
 import hashlib
 import struct
-import logging
 from pathlib import Path
 from typing import List, Generator, Tuple, Set, Union, Dict, Optional
 from collections import Counter
 from enum import IntFlag, Enum, auto
 import pickle
 import enum_tools.documentation
 
 # third-party imports
 from triton import AST_NODE
 
 # local imports
 from tritondse.types import Addr, PathConstraint, PathBranch, SolverStatus, PathHash, Edge, SymExType
+import tritondse.logging
 
+logger = tritondse.logging.get()
 
 CovItem = Union[Addr, Edge, PathHash, Tuple[PathHash, Edge]]
 """
 Variant type representing a coverage item.
 It can be:
 
 * an address :py:obj:`tritondse.types.Addr` for block coverage
@@ -264,15 +264,15 @@
         elif self.strategy == CoverageStrategy.PREFIXED_EDGE:
             return f"({covitem[0][:6]}_0x{covitem[1][0]:08x}-0x{covitem[1][1]:08x})"
 
     def difference(self, other: CoverageSingleRun) -> Set[CovItem]:
         if self.strategy == other.strategy:
             return self.covered_items.keys() - other.covered_items.keys()
         else:
-            logging.error("Trying to make difference of coverage with different strategies")
+            logger.error("Trying to make difference of coverage with different strategies")
             return set()
 
     def __sub__(self, other) -> Set[CovItem]:
         return self.difference(other)
 
 
 class GlobalCoverage(CoverageSingleRun):
@@ -318,15 +318,15 @@
 
         :param path_constraints: list of path constraint to iterate
         :return: generator of path constraint and branches to solve. The first tuple
                  item is a list of PathConstraint to add in the path predicate and the second
                  is the branch to solve (but not to keep in path predicate)
         """
         if BranchSolvingStrategy.MANUAL in self.branch_strategy:
-            logging.info(f'Branch solving strategy set to MANUAL.')
+            logger.info(f'Branch solving strategy set to MANUAL.')
             return
 
         pending_csts = []
         current_hash = hashlib.md5()  # Current path hash for PATH coverage
 
         # NOTE: When we arrive here the CoverageSingleRun associated with the path_constraints
         # has already been merge. Thus covered, pending etc do include ones of the CoverageSingleRuns
@@ -367,15 +367,15 @@
                                 if BranchSolvingStrategy.TIMEOUT_ONCE in self.branch_strategy:
                                     self.uncoverable_items[covitem] = res
 
                             elif res == SolverStatus.UNKNOWN:
                                 pass
 
                             else: # status == None
-                                logging.debug(f'Branch skipped!')
+                                logger.debug(f'Branch skipped!')
 
                             pending_csts = []  # reset pending constraint added
 
                     else:
                         pass  # Branch was taken do nothing
 
                 # Add it the path predicate constraints and update current path hash
@@ -392,21 +392,21 @@
                     typ = SymExType(typ)
                     offset, addr = int(offset), int(addr)
                     if addr not in self.covered_symbolic_pointers:  # if the address pointer has never been covered
                         pred = pc.getTakenPredicate()
                         if pred.getType() == AST_NODE.EQUAL:
                             p1, p2 = pred.getChildren()
                             if p2.getType() == AST_NODE.BV:
-                                logging.info(f"Try to enumerate value {offset}:0x{addr:02x}: {p1}")
+                                logger.info(f"Try to enumerate value {offset}:0x{addr:02x}: {p1}")
                                 res = yield typ, pending_csts, p1, (addr, p2.evaluate()), i
                                 self.covered_symbolic_pointers.add(addr)  # add the pointer in covered regardless of result
                             else:
-                                logging.warning(f"memory constraint unexpected pattern: {pred}")
+                                logger.warning(f"memory constraint unexpected pattern: {pred}")
                         else:
-                            logging.warning(f"memory constraint unexpected pattern: {pred}")
+                            logger.warning(f"memory constraint unexpected pattern: {pred}")
 
                 if BranchSolvingStrategy.SOUND_MEM_ACCESS in self.branch_strategy:
                     pending_csts.append(pc)  # if sound add the mem dereference as a constraint in path predicate
                     # NOTE: in both case the branch is not taken in account in the current_path_hash
 
 
     def _get_covitem(self, path_hash, branch: PathBranch) -> CovItem:
```

### Comparing `tritondse-0.1.4/tritondse/exception.py` & `tritondse-0.1.5/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/heap_allocator.py` & `tritondse-0.1.5/tritondse/heap_allocator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import logging
-
 from tritondse.types import Addr, ByteSize, Perm
 from tritondse.memory import Memory
 from tritondse.exception import AllocatorException
+import tritondse.logging
+
+logger = tritondse.logging.get()
 
 
 class HeapAllocator(object):
     """
     Custom tiny heap allocator. Used by built-ins routines like malloc/free.
     This allocation manager also provides an API enabling checking whether
     a pointer is allocated freed etc.
@@ -51,15 +52,15 @@
         :type size: :py:obj:`tritondse.types.ByteSize`
         :raise AllocatorException: if not memory is available
         :return: The pointer address allocated
         :rtype: :py:obj:`tritondse.types.Addr`
         """
 
         if size <= 0:
-            logging.error(f"Heap: invalid allocation size {size}")
+            logger.error(f"Heap: invalid allocation size {size}")
             return 0
 
         ptr = None
         for sz in sorted(x for x in self.free_pool if x >= size):
             # get the free chunk
             ptr = self.free_pool[sz].pop().start
```

### Comparing `tritondse-0.1.4/tritondse/loaders/cle_loader.py` & `tritondse-0.1.5/tritondse/loaders/cle_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import Generator, Optional, Tuple
 from pathlib import Path
 import logging
 
+# Third-party imports
+import cle
+
+# Local imports
 from tritondse.loaders import Loader, LoadableSegment
 from tritondse.types import Addr, Architecture, PathLike, Platform, Perm
-
 from tritondse.routines import SUPPORTED_ROUTINES
+import tritondse.logging
 
-import cle
+logger = tritondse.logging.get("loader")
 
 _arch_mapper = {
     "ARMEL":   Architecture.ARM32,
     "AARCH64": Architecture.AARCH64,
     "AMD64":   Architecture.X86_64,
     "X86":   Architecture.X86,
 }
@@ -36,15 +40,14 @@
         if not self.path.is_file():
             raise FileNotFoundError(f"file {path} not found (or not a file)")
 
         self._disable_vex_loggers()  # disable logs of pyvex
 
         self.ld_path = ld_path if ld_path is not None else ()
         self.ld = cle.Loader(str(path), ld_path=self.ld_path)
-        self.longjmp_addr_cache = None
 
     def _disable_vex_loggers(self):
         for name, logger in logging.root.manager.loggerDict.items():
             if "pyvex" in name:
                 logger.propagate = False
 
     @property
@@ -66,48 +69,27 @@
         """
         Program entrypoint address as defined in the binary headers
 
         :rtype: :py:obj:`tritondse.types.Addr`
         """
         return self.ld.main_object.entry
 
-    @property
-    def longjmp_addr(self) -> Addr:
-        # TODO find a better way to do this
-        # There is no generic way but since the plt layout is known we could do 
-        # https://github.com/lief-project/LIEF/issues/762
-        if not self.longjmp_addr_cache:
-            import subprocess
-
-            try:
-                proc1 = subprocess.Popen(['objdump', '-D', f'{self.path}'], stdout=subprocess.PIPE)
-                proc2 = subprocess.Popen(['grep', '<longjmp@plt>:'], stdin=proc1.stdout,
-                                         stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-                proc1.stdout.close() # Allow proc1 to receive a SIGPIPE if proc2 exits.
-                out, err = proc2.communicate()
-                self.longjmp_addr_cache = int(out.split()[0], 16)
-            except:
-                self.longjmp_addr_cache = 0
-
-        return self.longjmp_addr_cache
-
     def memory_segments(self) -> Generator[LoadableSegment, None, None]:
         """
         :return: Generator of tuples addrs and content
         """
         for obj in self.ld.all_objects:
-            logging.debug(obj)
+            logger.debug(obj)
             for seg in obj.segments:
                 segdata = self.ld.memory.load(seg.vaddr, seg.memsize)
                 assert len(segdata) == seg.memsize
                 perms = (Perm.R if seg.is_readable else 0) | (Perm.W if seg.is_writable else 0) | (Perm.X if seg.is_executable else 0) 
                 if seg.__class__.__name__ != "ExternSegment":
                     # The format string in CLE is broken if the filesize is 0. This is a workaround.
-                    logging.debug(f"Loading segment {seg} - perms:{perms}")
+                    logger.debug(f"Loading segment {seg} - perms:{perms}")
                 yield LoadableSegment(seg.vaddr, perms, content=segdata, name=f"seg-{obj.binary_basename}")
         # Also return a specific map to put external symbols
         yield LoadableSegment(self.EXTERN_SYM_BASE, self.EXTERN_SYM_SIZE, Perm.R | Perm.W, name="[extern]")
         yield LoadableSegment(self.END_STACK, self.BASE_STACK-self.END_STACK+1, Perm.R | Perm.W, name="[stack]")
 
         # FIXME. Temporary solution to prevent crashes on access to the TLB e.g fs:28
         yield LoadableSegment(0, 0x2000, Perm.R | Perm.W, name="[fs]")
@@ -170,15 +152,15 @@
         the relocation address in the binary.
 
         :return: Generator of tuples with symbol name, relocation address
         """
         # TODO I think there's a problem here. We only deal with imports from the main binary
         for s in self.ld.main_object.symbols:
             if s.resolved and s._type == cle.SymbolType.TYPE_OBJECT:
-                logging.debug(f"CleLoader: hooking symbol {s.name} @ {s.relative_addr:#x} {s.resolved} {s.resolvedby} {s._type}")
+                logger.debug(f"CleLoader: hooking symbol {s.name} @ {s.relative_addr:#x} {s.resolved} {s.resolvedby} {s._type}")
                 s_addr = s.relative_addr + self.ld.main_object.mapped_base
                 yield s.name, s_addr
 
     def find_function_addr(self, name: str) -> Optional[Addr]:
         """
         Search for the function name in fonctions of the binary.
```

### Comparing `tritondse-0.1.4/tritondse/loaders/loader.py` & `tritondse-0.1.5/tritondse/loaders/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 # built-in imports
 from collections import namedtuple
 from pathlib import Path
 from typing import Optional, Generator, Tuple, Dict, Union, List
-import logging
 from dataclasses import dataclass
 
 # local imports
 from tritondse.types import Addr, Architecture, Platform, ArchMode, PathLike, Perm
 from tritondse.arch import ARCHS
+import tritondse.logging
+
+logger = tritondse.logging.get()
 
 
 @dataclass
 class LoadableSegment:
     """ Represent a Segment to load in memory.
     It can either provide a content and will thus be
     initialized in a context or virtual.
@@ -151,15 +153,15 @@
         self.maps = maps
         self._arch_mode = ArchMode.THUMB if set_thumb else None
         if self._platform and (self._architecture, self._platform) in ARCHS:
             self._archinfo = ARCHS[(self._architecture, self._platform)]
         elif self._architecture in ARCHS:
             self._archinfo = ARCHS[self._architecture]
         else: 
-            logging.error("Unknown architecture")
+            logger.error("Unknown architecture")
             assert False
 
     @property
     def name(self) -> str:
         """ Name of the loader"""
         return f"Monolithic({self.bin_path})"
```

### Comparing `tritondse-0.1.4/tritondse/loaders/program.py` & `tritondse-0.1.5/tritondse/loaders/program.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 # built-in imports
 from pathlib import Path
 from typing import Optional, Generator, Tuple
-import logging
 from collections import namedtuple
 
 # third party
 import lief
 
 # local imports
 from tritondse.types import PathLike, Addr, Architecture, Platform, ArchMode, Perm, Endian
 from tritondse.loaders import Loader, LoadableSegment
+import tritondse.logging
 
+logger = tritondse.logging.get("loader")
 
 _arch_mapper = {
     lief.ARCHITECTURES.ARM:   Architecture.ARM32,
     lief.ARCHITECTURES.ARM64: Architecture.AARCH64,
     lief.ARCHITECTURES.X86:   Architecture.X86
 }
 
@@ -209,15 +210,15 @@
                     yield rel.symbol.name, rel.address
 
                 # Iterate functions imported via mandatory relocation (e.g: __libc_start_main)
                 for rel in self._binary.dynamic_relocations:
                     if self._is_glob_dat(rel) and rel.has_symbol and not rel.symbol.is_variable:
                         yield rel.symbol.name, rel.address
             except Exception:
-                logging.error('Something wrong with the pltgot relocations')
+                logger.error('Something wrong with the pltgot relocations')
 
         else:
             raise NotImplementedError(f"Imported functions relocations not implemented for: {self.format.name}")
 
     def imported_variable_symbols_relocations(self) -> Generator[Tuple[str, Addr], None, None]:
         """
         Iterate over all imported variable symbols. Yield for each of them the name and
```

### Comparing `tritondse-0.1.4/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.5/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/memory.py` & `tritondse-0.1.5/tritondse/memory.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/probes/basic_trace.py` & `tritondse-0.1.5/tritondse/probes/basic_trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-import logging
 from tritondse import ProbeInterface, CbType, SymbolicExecutor, ProcessState, SymbolicExplorator
+import tritondse.logging
+
+logger = tritondse.logging.get("probe.basictrace")
 
 
 class BasicDebugTrace(ProbeInterface):
     """
     Basic probe that print instruction trace
     to logging debug.
     """
     NAME = "debugtrace-probe"
 
     def __init__(self):
         super(BasicDebugTrace, self).__init__()
         self._add_callback(CbType.PRE_INST, self.trace_debug)
 
     def trace_debug(self, exec: SymbolicExecutor, __: ProcessState, ins: 'Instruction'):
-        logging.debug(f"[tid:{ins.getThreadId()}] {exec.trace_offset} [0x{ins.getAddress():x}]: {ins.getDisassembly()}")
+        logger.debug(f"[tid:{ins.getThreadId()}] {exec.trace_offset} [0x{ins.getAddress():x}]: {ins.getDisassembly()}")
 
 
 
 class BasicTextTrace(ProbeInterface):
     """
     Basic probe that generate a txt execution trace
     for each run.
@@ -33,15 +35,14 @@
 
         # File in which to write the trace
         self._file = None
 
     def pre_execution(self, executor: SymbolicExecutor, _: ProcessState):
         # Triggered before each execution
         name = f"{executor.uid}-{executor.seed.hash}.txt"
-        print(f"Open file: {name}")
         file = executor.workspace.get_metadata_file_path(f"{self.NAME}/{name}")
         self._file = open(file, "w")
 
     def post_execution(self, executor: SymbolicExecutor, _: ProcessState):
         self._file.close()
 
     def trace_debug(self, exec: SymbolicExecutor, __: ProcessState, ins: 'Instruction'):
```

### Comparing `tritondse-0.1.4/tritondse/process_state.py` & `tritondse-0.1.5/tritondse/process_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # built-ins
 from __future__ import annotations
 
 import io
 import sys
 import time
-import logging
-import re
 from typing import Union, Callable, Tuple, Optional, List, Dict
 
 
 # third-party
 # import z3  # For direct value enumeration
 from triton import TritonContext, MemoryAccess, CALLBACK, CPUSIZE, Instruction, MODE, AST_NODE, SOLVER, EXCEPTION
 
@@ -17,14 +15,17 @@
 from tritondse.thread_context import ThreadContext
 from tritondse.heap_allocator import HeapAllocator
 from tritondse.types import Architecture, Addr, ByteSize, BitSize, PathConstraint, Register, Expression, \
                             AstNode, Registers, SolverStatus, Model, SymbolicVariable, ArchMode, Perm, FileDesc
 from tritondse.arch import ARCHS, CpuState
 from tritondse.loaders import Loader
 from tritondse.memory import Memory, MemoryAccessViolation
+import tritondse.logging
+
+logger = tritondse.logging.get()
 
 
 class ProcessState(object):
     """
     Current process state. This class keeps all the runtime related to a running
     process, namely current, instruction, thread, memory maps, file descriptors etc.
     It also wraps Triton execution and thus hold its context. At the top of this,
@@ -166,15 +167,15 @@
             # Schedule to the next thread
             thread.count = 0  # Reset the counter
             thread.restore(self.tt_ctx)
             self._tid = thread.tid
             return True
 
         except Exception as e:
-            logging.error(f"Error while doing context switch: {e}")
+            logger.error(f"Error while doing context switch: {e}")
             return False
 
     def spawn_new_thread(self, new_pc: Addr, args: Addr) -> ThreadContext:
         """
         Create a new thread in the process state. Parameters are the
         new program counter and a pointer to arguments to provide the thread.
 
@@ -1145,36 +1146,36 @@
         pstate.cpu.program_counter = loader.entry_point
 
         # Disable segmentation to map segments
         with pstate.memory.without_segmentation():
             # Load memory areas in memory
             for i, seg in enumerate(loader.memory_segments()):
                 if not seg.size and not seg.content:
-                    logging.warning(f"A segment have to provide either a size or a content {seg.name} (skipped)")
+                    logger.warning(f"A segment have to provide either a size or a content {seg.name} (skipped)")
                     continue
                 size = len(seg.content) if seg.content else seg.size
-                logging.debug(f"Loading 0x{seg.address:#08x} - {seg.address+size:#08x} size={size:#x}")
+                logger.debug(f"Loading 0x{seg.address:#08x} - {seg.address+size:#08x} size={size:#x}")
                 pstate.memory.map(seg.address, size, seg.perms, seg.name)
                 if seg.content:
                     pstate.memory.write(seg.address, seg.content)
 
         # Apply dynamic relocations
         cur_linkage_address = pstate.EXTERN_FUNC_BASE
 
         # Disable segmentation
         with pstate.memory.without_segmentation():
             # Link imported functions in EXTERN_FUNC_BASE
             for fname, rel_addr in loader.imported_functions_relocations():
-                logging.debug(f"Hooking {fname} at {rel_addr:#x}")
+                logger.debug(f"Hooking {fname} at {rel_addr:#x}")
 
                 # If we already linked this function (because another library uses it) we reuse the same
                 # linkage address.
                 if fname in pstate.dynamic_symbol_table:
                     (linkage_address, _) = pstate.dynamic_symbol_table[fname] 
-                    logging.debug(f"Already added. {fname} at {rel_addr:#x} linkage_addr={linkage_address:#x}")
+                    logger.debug(f"Already added. {fname} at {rel_addr:#x} linkage_addr={linkage_address:#x}")
                     pstate.memory.write_ptr(rel_addr, linkage_address)
 
                 else:
                     # Add symbol in dynamic_symbol_table
                     pstate.dynamic_symbol_table[fname] = (cur_linkage_address, True)
 
                     # Apply relocation to our custom address in process memory
@@ -1187,24 +1188,24 @@
         # Map the stack
         try:
             stack = pstate.memory.map_from_name(pstate.STACK_SEG)
             alloc = 1 * pstate.ptr_size
             pstate.write_register(pstate.base_pointer_register, stack.start+stack.size-alloc) # Pointing right-out of the stack
             pstate.write_register(pstate.stack_pointer_register, stack.start+stack.size-alloc)
         except AssertionError:
-            logging.warning("no stack segment has been created by the loader")
+            logger.warning("no stack segment has been created by the loader")
 
         # Search for a map to settle foreign symbols
         segs = pstate.memory.find_map(pstate.EXTERN_SEG)
         if segs:
             symb_base = segs[0].start
 
             # Link imported symbols
             for sname, rel_addr in loader.imported_variable_symbols_relocations():
-                logging.debug(f"Hooking {sname} at {rel_addr:#x}")
+                logger.debug(f"Hooking {sname} at {rel_addr:#x}")
 
                 if pstate.architecture == Architecture.X86_64:  # HACK: Keep rel_addr to directly write symbol on it
                     # Add symbol in dynamic_symbol_table
                     pstate.dynamic_symbol_table[sname] = (rel_addr, False)
                     #pstate.memory.write_ptr(rel_addr, cur_linkage_address)  # Do not write anything as symbolic executor will do it
                 else:
                     # Add symbol in dynamic_symbol_table
```

### Comparing `tritondse-0.1.4/tritondse/qbdi_trace.py` & `tritondse-0.1.5/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/routines.py` & `tritondse-0.1.5/tritondse/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 import logging
 import os
 import random
 import re
 import sys
 import time
 
-from typing import Union
+from tritondse.types import Architecture, FileDesc
+from tritondse.seed import SeedFormat, SeedStatus, Seed
+import tritondse.logging
 
-from triton                   import CPUSIZE, MemoryAccess
-from tritondse.thread_context import ThreadContext
-from tritondse.types          import Architecture, FileDesc
-from tritondse.seed           import SeedFormat, SeedStatus, Seed
+logger = tritondse.logging.get("routines")
 
 NULL_PTR = 0
 
 
 
 def rtn_ctype_b_loc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __ctype_b_loc behavior.
     """
-    logging.debug('__ctype_b_loc hooked')
+    logger.debug('__ctype_b_loc hooked')
 
     ctype  = b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     ctype += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     ctype += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     ctype += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     ctype += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     ctype += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
@@ -79,15 +78,15 @@
 
 def rtn_ctype_toupper_loc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     # FIXME: Not sure about the array and where to place the pointer 
     # https://codebrowser.dev/glibc/glibc/locale/C-ctype.c.html
     """
     The __ctype_toupper_loc behavior.
     """
-    logging.debug('__ctype_toupper_loc hooked')
+    logger.debug('__ctype_toupper_loc hooked')
 
     ctype  = b"\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f"
     ctype += b"\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f"
     ctype += b"\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf"
     ctype += b"\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf"
     ctype += b"\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf"
     ctype += b"\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf"
@@ -126,15 +125,15 @@
     return base_ctype
 
 
 def rtn_errno_location(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __errno_location behavior.
     """
-    logging.debug('__errno_location hooked')
+    logger.debug('__errno_location hooked')
 
     # Errno is a int* ptr, initialize it to zero
     # We consider it is located in the [extern] segment
     # Thus the process must have one of this map
     segs = pstate.memory.find_map(pstate.EXTERN_SEG)
     if segs:
         map = segs[0]
@@ -146,15 +145,15 @@
     return ERRNO
 
 
 def rtn_libc_start_main(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __libc_start_main behavior.
     """
-    logging.debug('__libc_start_main hooked')
+    logger.debug('__libc_start_main hooked')
 
     # Get arguments
     main = pstate.get_argument_value(0)
 
     # WARNING: Dirty trick to make sure to jump on main after
     # the emulation of that stub
     if pstate.architecture == Architecture.AARCH64:
@@ -174,15 +173,15 @@
 
     if pstate.architecture == Architecture.X86:
         # Because of the "Dirty trick" described above, we RET to main instead of CALLing it.
         # Because of that, the arguments end up 1 slot off on the stack
         pstate.write_argument_value(0 + 1, argc)
     else:
         pstate.write_argument_value(0, argc)
-    logging.debug(f"argc = {argc}")
+    logger.debug(f"argc = {argc}")
 
     # Define argv
     addrs = list()
 
     if se.config.is_format_composite() and se.seed.content.argv: # Use the seed provided (and ignore config.program_argv !!)
         argvs = se.seed.content.argv
         src = 'seed'
@@ -203,15 +202,15 @@
         pstate.memory.write(base, arg + b'\x00')
 
         if se.config.is_format_composite() and se.seed.content.argv: # Use the seed provided (and ignore config.program_argv !!)
             # Symbolize the argv string
             se.inject_symbolic_argv_memory(base, i, arg)
             # FIXME: Shall add a constraint on every char to be != \x00
 
-        logging.debug(f"({src}) argv[{i}] = {repr(pstate.memory.read(base, len(arg)))}")
+        logger.debug(f"({src}) argv[{i}] = {repr(pstate.memory.read(base, len(arg)))}")
         base += len(arg) + 1
 
 
     # NOTE: the array of pointers will be after the string themselves
     b_argv = base
     for addr in addrs:
         pstate.memory.write_ptr(base, addr)
@@ -227,26 +226,26 @@
     return None
 
 
 def rtn_stack_chk_fail(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __stack_chk_fail behavior.
     """
-    logging.debug('__stack_chk_fail hooked')
-    logging.critical('*** stack smashing detected ***: terminated')
+    logger.debug('__stack_chk_fail hooked')
+    logger.critical('*** stack smashing detected ***: terminated')
     se.seed.status = SeedStatus.CRASH
     pstate.stop = True
 
 
 # int __xstat(int ver, const char* path, struct stat* stat_buf);
 def rtn_xstat(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __xstat behavior.
     """
-    logging.debug('__xstat hooked')
+    logger.debug('__xstat hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # int ver
     arg1 = pstate.get_argument_value(1)  # const char* path
     arg2 = pstate.get_argument_value(2)  # struct stat* stat_buf
 
     if os.path.isfile(pstate.memory.read_string(arg1)):
@@ -281,15 +280,15 @@
 
         void abort(void);
 
     Mark the input seed as OK and stop execution.
 
     [`Man Page <https://man7.org/linux/man-pages/man3/abort.3.html>`_]
     """
-    logging.debug('abort hooked')
+    logger.debug('abort hooked')
     se.seed.status = SeedStatus.OK_DONE
     pstate.stop = True
 
 
 # int atoi(const char *nptr);
 def rtn_atoi(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """::
@@ -308,15 +307,15 @@
                  of an integer. It does not support negative integer nor values
                  prefixed by spaces.
 
     [`Man Page <https://man7.org/linux/man-pages/man3/abort.3.html>`_]
 
     :return: Symbolic value of the integer base on the symbolic string ``nptr``
     """
-    logging.debug('atoi hooked')
+    logger.debug('atoi hooked')
 
     ast = pstate.actx
     arg = pstate.get_argument_value(0)
 
     # FIXME: On ne concretize pas correctement la taille de la chaine
 
     cells = {i: pstate.read_symbolic_memory_byte(arg+i).getAst() for i in range(10)}
@@ -380,15 +379,15 @@
 
 
 # void *calloc(size_t nmemb, size_t size);
 def rtn_calloc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The calloc behavior.
     """
-    logging.debug('calloc hooked')
+    logger.debug('calloc hooked')
 
     # Get arguments
     nmemb = pstate.get_argument_value(0)
     size  = pstate.get_argument_value(1)
 
     # We use nmemb and size as concret values
     pstate.concretize_argument(0)  # will be concretized with nmemb value
@@ -407,15 +406,15 @@
 
 
 # int clock_gettime(clockid_t clockid, struct timespec *tp);
 def rtn_clock_gettime(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The clock_gettime behavior.
     """
-    logging.debug('clock_gettime hooked')
+    logger.debug('clock_gettime hooked')
 
     # Get arguments
     clockid = pstate.get_argument_value(0)
     tp      = pstate.get_argument_value(1)
 
     # We use tp as concret value
     pstate.concretize_argument(1)
@@ -436,25 +435,25 @@
     return 0
 
 
 def rtn_exit(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The exit behavior.
     """
-    logging.debug('exit hooked')
+    logger.debug('exit hooked')
     arg = pstate.get_argument_value(0)
     pstate.stop = True
     return arg
 
 
 def rtn_fclose(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fclose behavior.
     """
-    logging.debug('fclose hooked')
+    logger.debug('fclose hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0) # fd
 
     # We use fd as concret value
     pstate.concretize_argument(0)
 
@@ -471,15 +470,15 @@
     """
     The fseek behavior.
     """
 
     #define SEEK_SET    0   /* set file offset to offset */
     #define SEEK_CUR    1   /* set file offset to current plus offset */
     #define SEEK_END    2   /* set file offset to EOF plus offset */
-    logging.debug('fseek hooked')
+    logger.debug('fseek hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
     arg2 = pstate.get_argument_value(2)
 
     if arg2 not in [0, 1, 2]:
@@ -500,15 +499,15 @@
 
 
 def rtn_ftell(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The ftell behavior.
     """
 
-    logging.debug('ftell hooked')
+    logger.debug('ftell hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
 
     if pstate.file_descriptor_exists(arg0):
         desc = pstate.get_file_descriptor(arg0)
 
@@ -520,15 +519,15 @@
 
 
 # char *fgets(char *s, int size, FILE *stream);
 def rtn_fgets(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fgets behavior.
     """
-    logging.debug('fgets hooked')
+    logger.debug('fgets hooked')
 
     # Get arguments
     buff, buff_ast = pstate.get_full_argument(0)
     size, size_ast = pstate.get_full_argument(1)
     fd = pstate.get_argument_value(2)
     # We use fd as concret value
     pstate.concretize_argument(2)
@@ -544,66 +543,66 @@
             if se.seed.is_raw() and se.seed.is_bootstrap_seed() and not data_no_trail:
                 data = b'\x00' * size
 
             if len(data_no_trail) == size:  # if `size` limited the fgets its an indirect constraint
                 pstate.push_constraint(size_ast.getAst() == size)
 
             se.inject_symbolic_file_memory(buff, filedesc.name, data, offset)
-            logging.debug(f"fgets() in {filedesc.name} = {repr(data)}")
+            logger.debug(f"fgets() in {filedesc.name} = {repr(data)}")
         else:
             pstate.concretize_argument(1)
             pstate.memory.write(buff, data)
 
         return buff_ast if data_no_trail else NULL_PTR
     else:
-        logging.warning(f'File descriptor ({fd}) not found')
+        logger.warning(f'File descriptor ({fd}) not found')
         return NULL_PTR
 
 
 # fopen(const char *pathname, const char *mode);
 def rtn_fopen(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fopen behavior.
     """
-    logging.debug('fopen hooked')
+    logger.debug('fopen hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # const char *pathname
     arg1 = pstate.get_argument_value(1)  # const char *mode
     arg0s = pstate.memory.read_string(arg0)
     arg1s = pstate.memory.read_string(arg1)
 
     # Concretize the whole path name
     pstate.concretize_memory_bytes(arg0, len(arg0s)+1)  # Concretize the whole string + \0
 
     # We use mode as concrete value
     pstate.concretize_argument(1)
 
     if se.seed.is_file_defined(arg0s):
-        logging.info(f"opening an input file: {arg0s}")
+        logger.info(f"opening an input file: {arg0s}")
         # Program is opening an input
         data = se.seed.get_file_input(arg0s)
         filedesc = pstate.create_file_descriptor(arg0s, io.BytesIO(data))
         return filedesc.id
     else:
         # Try to open it as a regular file
         try:
             fd = open(arg0s, arg1s)
             filedesc = pstate.create_file_descriptor(arg0s, fd)
             return filedesc.id
         except Exception as e:
-            logging.debug(f"Failed to open {arg0s} {e}")
+            logger.debug(f"Failed to open {arg0s} {e}")
             return NULL_PTR
 
 
 def rtn_fprintf(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fprintf behavior.
     """
-    logging.debug('fprintf hooked')
+    logger.debug('fprintf hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
 
     # FIXME: ARM64
     # FIXME: pushPathConstraint
@@ -611,15 +610,15 @@
     arg1f = pstate.get_format_string(arg1)
     nbArgs = arg1f.count("{")
     args = pstate.get_format_arguments(arg1, [pstate.get_argument_value(x) for x in range(2, nbArgs+2)])
     try:
         s = arg1f.format(*args)
     except:
         # FIXME: Les chars UTF8 peuvent foutre le bordel. Voir avec ground-truth/07.input
-        logging.warning('Something wrong, probably UTF-8 string')
+        logger.warning('Something wrong, probably UTF-8 string')
         s = ""
 
     if pstate.file_descriptor_exists(arg0):
         fdesc = pstate.get_file_descriptor(arg0)
         if arg0 not in [1, 2] or (arg0 == 1 and se.config.pipe_stdout) or (arg0 == 2 and se.config.pipe_stderr):
             fdesc.fd.write(s)
             fdesc.fd.flush()
@@ -630,15 +629,15 @@
     return len(s)
 
 
 def rtn___fprintf_chk(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __fprintf_chk behavior.
     """
-    logging.debug('__fprintf_chk hooked')
+    logger.debug('__fprintf_chk hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     flag = pstate.get_argument_value(1)
     arg1 = pstate.get_argument_value(2)
 
     # FIXME: ARM64
@@ -647,15 +646,15 @@
     arg1f = pstate.get_format_string(arg1)
     nbArgs = arg1f.count("{")
     args = pstate.get_format_arguments(arg1, [pstate.get_argument_value(x) for x in range(3, nbArgs+2)])
     try:
         s = arg1f.format(*args)
     except:
         # FIXME: Les chars UTF8 peuvent foutre le bordel. Voir avec ground-truth/07.input
-        logging.warning('Something wrong, probably UTF-8 string')
+        logger.warning('Something wrong, probably UTF-8 string')
         s = ""
 
     if pstate.file_descriptor_exists(arg0):
         fdesc = pstate.get_file_descriptor(arg0)
         if arg0 not in [1, 2] or (arg0 == 1 and se.config.pipe_stdout) or (arg0 == 2 and se.config.pipe_stderr):
             fdesc.fd.write(s)
             fdesc.fd.flush()
@@ -667,15 +666,15 @@
 
 
 # fputc(int c, FILE *stream);
 def rtn_fputc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fputc behavior.
     """
-    logging.debug('fputc hooked')
+    logger.debug('fputc hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
 
     pstate.concretize_argument(0)
     pstate.concretize_argument(1)
@@ -695,15 +694,15 @@
 
 
 
 def rtn_fputs(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fputs behavior.
     """
-    logging.debug('fputs hooked')
+    logger.debug('fputs hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
 
     pstate.concretize_argument(0)
     pstate.concretize_argument(1)
@@ -733,15 +732,15 @@
     return len(s)
 
 
 def rtn_fread(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fread behavior.
     """
-    logging.debug('fread hooked')
+    logger.debug('fread hooked')
 
     # Get arguments
     ptr = pstate.get_argument_value(0) # ptr
     size_t, size_ast = pstate.get_full_argument(1) # size
     nmemb = pstate.get_argument_value(2) # nmemb
     fd = pstate.get_argument_value(3) # stream
     size = size_t * nmemb
@@ -758,45 +757,45 @@
             if se.seed.is_raw() and se.seed.is_bootstrap_seed() and not data:
                 data = b'\x00' * size
 
             if len(data) == size:  # if `size` limited the fgets its an indirect constraint
                 pstate.push_constraint(size_ast.getAst() == size)
 
             se.inject_symbolic_file_memory(ptr, filedesc.name, data, offset)
-            logging.debug(f"read in {filedesc.name} = {repr(data)}")
+            logger.debug(f"read in {filedesc.name} = {repr(data)}")
         else:
             pstate.concretize_argument(2)
             pstate.memory.write(ptr, data)
 
         return int(len(data)/size_t) if size_t else 0  # number of items read
     else:
-        logging.warning(f'File descriptor ({fd}) not found')
+        logger.warning(f'File descriptor ({fd}) not found')
         return 0
 
 
 def rtn_free(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The free behavior.
     """
-    logging.debug('free hooked')
+    logger.debug('free hooked')
 
     # Get arguments
     ptr = pstate.get_argument_value(0)
     if ptr == 0: # free(NULL) is a nop
         return None
     pstate.heap_allocator.free(ptr)
 
     return None
 
 
 def rtn_fwrite(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The fwrite behavior.
     """
-    logging.debug('fwrite hooked')
+    logger.debug('fwrite hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
     arg2 = pstate.get_argument_value(2)
     arg3 = pstate.get_argument_value(3)
     size = arg1 * arg2
@@ -823,15 +822,15 @@
     return size
 
 
 def rtn_write(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The write behavior.
     """
-    logging.debug('write hooked')
+    logger.debug('write hooked')
 
     # Get arguments
     fd = pstate.get_argument_value(0)
     buf = pstate.get_argument_value(1)
     size = pstate.get_argument_value(2)
     data = pstate.memory.read(buf, size)
 
@@ -856,15 +855,15 @@
     return size
 
 
 def rtn_gettimeofday(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The gettimeofday behavior.
     """
-    logging.debug('gettimeofday hooked')
+    logger.debug('gettimeofday hooked')
 
     # Get arguments
     tv = pstate.get_argument_value(0)
     tz = pstate.get_argument_value(1)
 
     if tv == 0:
         return pstate.minus_one
@@ -882,29 +881,29 @@
     return 0
 
 
 def rtn_malloc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The malloc behavior.
     """
-    logging.debug('malloc hooked')
+    logger.debug('malloc hooked')
 
     # Get arguments
     size = pstate.get_argument_value(0)
     ptr = pstate.heap_allocator.alloc(size)
 
     # Return value
     return ptr
 
 
 def rtn_open(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The open behavior.
     """
-    logging.debug('open hooked')
+    logger.debug('open hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # const char *pathname
     flags = pstate.get_argument_value(1)  # int flags
     mode = pstate.get_argument_value(2)  # we ignore it
     arg0s = pstate.memory.read_string(arg0)
 
@@ -924,50 +923,53 @@
         mode = "r+"
 
     if flags & 0x0100: # O_CREAT
         mode += "x"
     if flags & 0x0200: # O_APPEND
         mode = "a"  # replace completely value
 
+    # enforce using binary mode for open
+    mode += "b"
+
     if se.seed.is_file_defined(arg0s) and "r" in mode:  # input file and opened in reading
-        logging.info(f"opening an input file: {arg0s}")
+        logger.info(f"opening an input file: {arg0s}")
         # Program is opening an input
         data = se.seed.get_file_input(arg0s)
         filedesc = pstate.create_file_descriptor(arg0s, io.BytesIO(data))
         return filedesc.id
     else:
         # Try to open it as a regular file
         try:
             fd = open(arg0s, mode)  # use the mode here
             filedesc = pstate.create_file_descriptor(arg0s, fd)
             return filedesc.id
         except Exception as e:
-            logging.debug(f"Failed to open {arg0s} {e}")
+            logger.debug(f"Failed to open {arg0s} {e}")
             return pstate.minus_one
 
 def rtn_realloc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The realloc behavior.
     """
-    logging.debug('realloc hooked')
+    logger.debug('realloc hooked')
 
     # Get arguments
     oldptr = pstate.get_argument_value(0)
     size = pstate.get_argument_value(1)
 
     if oldptr == 0:
         # malloc behaviour
         ptr = pstate.heap_allocator.alloc(size)
         return ptr
 
     ptr = pstate.heap_allocator.alloc(size)
     if ptr == 0: return ptr
 
     if ptr not in pstate.heap_allocator.alloc_pool:
-        logging.warning("Invalid ptr passed to realloc")
+        logger.warning("Invalid ptr passed to realloc")
         pstate.heap_allocator.free(ptr) # This will raise an error
 
     old_memmap = pstate.heap_allocator.alloc_pool[oldptr]
     old_size = old_memmap.size
     size_to_copy = min(size, old_size)
 
     #data = pstate.memory.read(oldptr, size_to_copy)
@@ -983,15 +985,15 @@
     return ptr
 
 
 def rtn_memcmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The memcmp behavior.
     """
-    logging.debug('memcmp hooked')
+    logger.debug('memcmp hooked')
 
     s1 = pstate.get_argument_value(0)
     s2 = pstate.get_argument_value(1)
     size = pstate.get_argument_value(2)
 
     ptr_bit_size = pstate.ptr_bit_size
 
@@ -1013,15 +1015,15 @@
     return res
 
 
 def rtn_memcpy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The memcpy behavior.
     """
-    logging.debug('memcpy hooked')
+    logger.debug('memcpy hooked')
 
     dst, dst_ast = pstate.get_full_argument(0)
     src = pstate.get_argument_value(1)
     cnt = pstate.get_argument_value(2)
 
     # We constrain the logical value of size
     pstate.concretize_argument(2)
@@ -1034,15 +1036,15 @@
     return dst_ast
 
 
 def rtn_mempcpy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The mempcpy behavior.
     """
-    logging.debug('mempcpy hooked')
+    logger.debug('mempcpy hooked')
 
     dst, dst_ast = pstate.get_full_argument(0)
     src = pstate.get_argument_value(1)
     cnt = pstate.get_argument_value(2)
 
     # We constrain the logical value of size
     pstate.concretize_argument(2)
@@ -1055,15 +1057,15 @@
     return dst + cnt
 
 
 def rtn_memmem(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The memmem behavior.
     """
-    logging.debug('memmem hooked')
+    logger.debug('memmem hooked')
 
     haystack    = pstate.get_argument_value(0)  # const void*
     haystacklen = pstate.get_argument_value(1)  # size_t
     needle      = pstate.get_argument_value(2)  # const void *
     needlelen   = pstate.get_argument_value(3)  # size_t
 
     s1 = pstate.memory.read(haystack, haystacklen)  # haystack
@@ -1085,15 +1087,15 @@
     return haystack + offset
 
 
 def rtn_memmove(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The memmove behavior.
     """
-    logging.debug('memmove hooked')
+    logger.debug('memmove hooked')
 
     dst, dst_ast = pstate.get_full_argument(0)
     src = pstate.get_argument_value(1)
     cnt = pstate.get_argument_value(2)
 
     # We constrain the logical value of cnt
     pstate.concretize_argument(2)
@@ -1107,15 +1109,15 @@
     return dst_ast
 
 
 def rtn_memset(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The memset behavior.
     """
-    logging.debug('memset hooked')
+    logger.debug('memset hooked')
 
     dst, dst_ast = pstate.get_full_argument(0)
     src, src_ast = pstate.get_full_argument(1)
     size = pstate.get_argument_value(2)
 
     # We constrain the logical value of size
     pstate.concretize_argument(2)
@@ -1129,27 +1131,27 @@
     return dst_ast
 
 
 def rtn_printf(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The printf behavior.
     """
-    logging.debug('printf hooked')
+    logger.debug('printf hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
 
     arg0f = pstate.get_format_string(arg0)
     nbArgs = arg0f.count("{")
     args = pstate.get_format_arguments(arg0, [pstate.get_argument_value(x) for x in range(1, nbArgs+1)])
     try:
         s = arg0f.format(*args)
     except:
         # FIXME: Les chars UTF8 peuvent foutre le bordel. Voir avec ground-truth/07.input
-        logging.warning('Something wrong, probably UTF-8 string')
+        logger.warning('Something wrong, probably UTF-8 string')
         s = ""
 
     if se.config.pipe_stdout:
         stdout = pstate.get_file_descriptor(1)
         stdout.fd.write(s)
         stdout.fd.flush()
 
@@ -1157,15 +1159,15 @@
     return len(s)
 
 
 def rtn_pthread_create(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_create behavior.
     """
-    logging.debug('pthread_create hooked')
+    logger.debug('pthread_create hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0) # pthread_t *thread
     arg1 = pstate.get_argument_value(1) # const pthread_attr_t *attr
     arg2 = pstate.get_argument_value(2) # void *(*start_routine) (void *)
     arg3 = pstate.get_argument_value(3) # void *arg
 
@@ -1178,15 +1180,15 @@
     return 0
 
 
 def rtn_pthread_exit(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_exit behavior.
     """
-    logging.debug('pthread_exit hooked')
+    logger.debug('pthread_exit hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
 
     # Kill the thread
     pstate.current_thread.kill()
 
@@ -1197,103 +1199,103 @@
     return None
 
 
 def rtn_pthread_join(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_join behavior.
     """
-    logging.debug('pthread_join hooked')
+    logger.debug('pthread_join hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)
     arg1 = pstate.get_argument_value(1)
 
     if arg0 in pstate.threads:
         pstate.current_thread.join_thread(arg0)
-        logging.info(f"Thread id {pstate.current_thread.tid} joined thread id {arg0}")
+        logger.info(f"Thread id {pstate.current_thread.tid} joined thread id {arg0}")
     else:
         pstate.current_thread.cancel_join()
-        logging.debug(f"Thread id {arg0} already destroyed")
+        logger.debug(f"Thread id {arg0} already destroyed")
 
     # Return value
     return 0
 
 
 def rtn_pthread_mutex_destroy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_mutex_destroy behavior.
     """
-    logging.debug('pthread_mutex_destroy hooked')
+    logger.debug('pthread_mutex_destroy hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # pthread_mutex_t *restrict mutex
     pstate.memory.write_ptr(arg0, pstate.PTHREAD_MUTEX_INIT_MAGIC)
 
     return 0
 
 
 def rtn_pthread_mutex_init(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_mutex_init behavior.
     """
-    logging.debug('pthread_mutex_init hooked')
+    logger.debug('pthread_mutex_init hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # pthread_mutex_t *restrict mutex
     arg1 = pstate.get_argument_value(1)  # const pthread_mutexattr_t *restrict attr)
 
     pstate.memory.write_ptr(arg0, pstate.PTHREAD_MUTEX_INIT_MAGIC)
 
     return 0
 
 
 def rtn_pthread_mutex_lock(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_mutex_lock behavior.
     """
-    logging.debug('pthread_mutex_lock hooked')
+    logger.debug('pthread_mutex_lock hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # pthread_mutex_t *mutex
     mutex = pstate.memory.read_ptr(arg0)  # deref pointer and read a uint64 int
 
     # If the thread has been initialized and unused, define the tid has lock
     if mutex == pstate.PTHREAD_MUTEX_INIT_MAGIC:
-        logging.debug('mutex unlocked')
+        logger.debug('mutex unlocked')
         pstate.memory.write_ptr(arg0, pstate.current_thread.tid)
 
     # The mutex is locked and we are not allowed to continue the execution
     elif mutex != pstate.current_thread.tid:
-        logging.debug('mutex locked')
+        logger.debug('mutex locked')
         pstate.mutex_locked = True
 
     # Return value
     return 0
 
 
 def rtn_pthread_mutex_unlock(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The pthread_mutex_unlock behavior.
     """
-    logging.debug('pthread_mutex_unlock hooked')
+    logger.debug('pthread_mutex_unlock hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # pthread_mutex_t *mutex
 
     pstate.memory.write_ptr(arg0, pstate.PTHREAD_MUTEX_INIT_MAGIC)
 
     # Return value
     return 0
 
 
 def rtn_puts(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The puts behavior.
     """
-    logging.debug('puts hooked')
+    logger.debug('puts hooked')
 
     arg0 = pstate.get_string_argument(0)
 
     # Get arguments
     if se.config.pipe_stdout:  # Only perform printing if pipe_stdout activated
         sys.stdout.write(arg0 + '\n')
         sys.stdout.flush()
@@ -1302,31 +1304,31 @@
     return len(arg0) + 1
 
 
 def rtn_rand(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The rand behavior.
     """
-    logging.debug('rand hooked')
+    logger.debug('rand hooked')
     return random.randrange(0, 0xffffffff)
 
 
 def rtn_read(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The read behavior.
     """
-    logging.debug('read hooked')
+    logger.debug('read hooked')
 
     # Get arguments
     fd   = pstate.get_argument_value(0)
     buff = pstate.get_argument_value(1)
     size, size_ast = pstate.get_full_argument(2)
 
     if size_ast.isSymbolized():
-        logging.warning(f'Reading from the file descriptor ({fd}) with a symbolic size')
+        logger.warning(f'Reading from the file descriptor ({fd}) with a symbolic size')
 
     pstate.concretize_argument(0)
 
     if pstate.file_descriptor_exists(fd):
         filedesc = pstate.get_file_descriptor(fd)
         offset = filedesc.offset
         data = filedesc.read(size)
@@ -1336,51 +1338,51 @@
             if se.seed.is_raw() and se.seed.is_bootstrap_seed() and not data:
                 data = b'\x00' * size
 
             if len(data) == size:  # if `size` limited the fgets its an indirect constraint
                 pstate.push_constraint(size_ast.getAst() == size)
 
             se.inject_symbolic_file_memory(buff, filedesc.name, data, offset)
-            logging.debug(f"read in (input) {filedesc.name} = {repr(data)}")
+            logger.debug(f"read in (input) {filedesc.name} = {repr(data)}")
         else:
             pstate.concretize_argument(2)
             pstate.memory.write(buff, data)
 
         return len(data)
     else:
-        logging.warning(f'File descriptor ({fd}) not found')
+        logger.warning(f'File descriptor ({fd}) not found')
         return pstate.minus_one  # todo: set errno
 
 
 def rtn_getchar(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The getchar behavior.
     """
-    logging.debug('getchar hooked')
+    logger.debug('getchar hooked')
 
     # Get arguments
     filedesc = pstate.get_file_descriptor(0) # stdin
     offset = filedesc.offset
 
     data = filedesc.read(1)
     if data:
         if filedesc.is_input_fd():  # Reading into input
             data = ord(data) # convert to integer
             se.inject_symbolic_file_register(pstate.return_register, filedesc.name, data, offset)
-            logging.debug(f"read in {filedesc.name} = {repr(data)}")
+            logger.debug(f"read in {filedesc.name} = {repr(data)}")
         return data
     else:
         return pstate.minus_one
 
 
 def rtn_sem_destroy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_destroy behavior.
     """
-    logging.debug('sem_destroy hooked')
+    logger.debug('sem_destroy hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
 
     # Destroy the semaphore with the value
     pstate.memory.write_ptr(arg0, 0)
 
@@ -1388,15 +1390,15 @@
     return 0
 
 
 def rtn_sem_getvalue(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_getvalue behavior.
     """
-    logging.debug('sem_getvalue hooked')
+    logger.debug('sem_getvalue hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
     arg1 = pstate.get_argument_value(1)  # int *sval
 
     value = pstate.memory.read_ptr(arg0)  # deref pointer
 
@@ -1407,15 +1409,15 @@
     return 0
 
 
 def rtn_sem_init(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_init behavior.
     """
-    logging.debug('sem_init hooked')
+    logger.debug('sem_init hooked')
 
     # Get arguments
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
     arg1 = pstate.get_argument_value(1)  # int pshared
     arg2 = pstate.get_argument_value(2)  # unsigned int value
 
     # Init the semaphore with the value
@@ -1425,15 +1427,15 @@
     return 0
 
 
 def rtn_sem_post(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_post behavior.
     """
-    logging.debug('sem_post hooked')
+    logger.debug('sem_post hooked')
 
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
 
     # increments (unlocks) the semaphore pointed to by sem
     value = pstate.memory.read_ptr(arg0)
     pstate.memory.write_ptr(arg0, value + 1)
 
@@ -1441,15 +1443,15 @@
     return 0
 
 
 def rtn_sem_timedwait(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_timedwait behavior.
     """
-    logging.debug('sem_timedwait hooked')
+    logger.debug('sem_timedwait hooked')
 
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
     arg1 = pstate.get_argument_value(1)  # const struct timespec *abs_timeout
 
     # sem_timedwait() is the same as sem_wait(), except that abs_timeout specifies a limit
     # on the amount of time that the call should block if the decrement cannot be immediately
     # performed. The abs_timeout argument points to a structure that specifies an absolute
@@ -1467,43 +1469,43 @@
     # If  the operation can be performed immediately, then sem_timedwait() never fails with a
     # timeout error, regardless of the value of abs_timeout.  Furthermore, the validity of
     # abs_timeout is not checked in this case.
 
     # TODO: Take into account the abs_timeout argument
     value = pstate.memory.read_ptr(arg0)
     if value > 0:
-        logging.debug('semaphore still not locked')
+        logger.debug('semaphore still not locked')
         pstate.memory.write_ptr(arg0, value - 1)
         pstate.semaphore_locked = False
     else:
-        logging.debug('semaphore locked')
+        logger.debug('semaphore locked')
         pstate.semaphore_locked = True
 
     # Return success
     return 0
 
 
 def rtn_sem_trywait(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_trywait behavior.
     """
-    logging.debug('sem_trywait hooked')
+    logger.debug('sem_trywait hooked')
 
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
 
     # sem_trywait()  is  the  same as sem_wait(), except that if the decrement
     # cannot be immediately performed, then call returns an error (errno set to
     # EAGAIN) instead of blocking.
     value = pstate.memory.read_ptr(arg0)
     if value > 0:
-        logging.debug('semaphore still not locked')
+        logger.debug('semaphore still not locked')
         pstate.memory.write_ptr(arg0, value - 1)
         pstate.semaphore_locked = False
     else:
-        logging.debug('semaphore locked but continue')
+        logger.debug('semaphore locked but continue')
         pstate.semaphore_locked = False
 
         # Setting errno to EAGAIN (3406)
         segs = pstate.memory.find_map(pstate.EXTERN_SEG)
         if segs:
             map = segs[0]
             ERRNO = map.start + map.size - 4  # Point is last int of the mapping
@@ -1518,69 +1520,69 @@
     return 0
 
 
 def rtn_sem_wait(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sem_wait behavior.
     """
-    logging.debug('sem_wait hooked')
+    logger.debug('sem_wait hooked')
 
     arg0 = pstate.get_argument_value(0)  # sem_t *sem
 
     # decrements (locks) the semaphore pointed to by sem. If the semaphore's value
     # is greater than zero, then the decrement proceeds, and the function returns,
     # immediately. If the semaphore currently has the value zero, then the call blocks
     # until either it becomes possible to perform the decrement (i.e., the semaphore
     # value rises above zero).
     value = pstate.memory.read_ptr(arg0)
     if value > 0:
-        logging.debug('semaphore still not locked')
+        logger.debug('semaphore still not locked')
         pstate.memory.write_ptr(arg0, value - 1)
         pstate.semaphore_locked = False
     else:
-        logging.debug('semaphore locked')
+        logger.debug('semaphore locked')
         pstate.semaphore_locked = True
 
     # Return success
     return 0
 
 
 def rtn_sleep(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sleep behavior.
     """
-    logging.debug('sleep hooked')
+    logger.debug('sleep hooked')
 
     # Get arguments
     if not se.config.skip_sleep_routine:
         t = pstate.get_argument_value(0)
         time.sleep(t)
 
     # Return value
     return 0
 
 
 def rtn_sprintf(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The sprintf behavior.
     """
-    logging.debug('sprintf hooked')
+    logger.debug('sprintf hooked')
 
     # Get arguments
     buff = pstate.get_argument_value(0)
     arg0 = pstate.get_argument_value(1)
 
     try:
         arg0f = pstate.get_format_string(arg0)
         nbArgs = arg0f.count("{")
         args = pstate.get_format_arguments(arg0, [pstate.get_argument_value(x) for x in range(2, nbArgs+2)])
         s = arg0f.format(*args)
     except:
         # FIXME: Les chars UTF8 peuvent foutre le bordel. Voir avec ground-truth/07.input
-        logging.warning('Something wrong, probably UTF-8 string')
+        logger.warning('Something wrong, probably UTF-8 string')
         s = ""
 
     # FIXME: todo
 
     # FIXME: THIS SEEMS NOT OK
     # for index, c in enumerate(s):
     #     pstate.tt_ctx.concretizeMemory(buff + index)
@@ -1594,15 +1596,15 @@
     return len(s)
 
 
 def rtn_strcasecmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strcasecmp behavior.
     """
-    logging.debug('strcasecmp hooked')
+    logger.debug('strcasecmp hooked')
 
     s1 = pstate.get_argument_value(0)
     s2 = pstate.get_argument_value(1)
     size = min(len(pstate.memory.read_string(s1)), len(pstate.memory.read_string(s2)) + 1)
 
     #s = s1 if len(pstate.memory.read_string(s1)) < len(pstate.memory.read_string(s2)) else s2
     #for i in range(size):
@@ -1627,15 +1629,15 @@
     return res
 
 
 def rtn_strchr(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strchr behavior.
     """
-    logging.debug('strchr hooked')
+    logger.debug('strchr hooked')
 
     string = pstate.get_argument_value(0)
     char   = pstate.get_argument_value(1)
     ast    = pstate.actx
     ptr_bit_size = pstate.ptr_bit_size
 
     def rec(res, deep, maxdeep):
@@ -1655,15 +1657,15 @@
     return res
 
 
 def rtn_strcmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strcmp behavior.
     """
-    logging.debug('strcmp hooked')
+    logger.debug('strcmp hooked')
 
     s1 = pstate.get_argument_value(0)
     s2 = pstate.get_argument_value(1)
     size = min(len(pstate.memory.read_string(s1)), len(pstate.memory.read_string(s2))) + 1
     
     #s = s1 if len(pstate.memory.read_string(s1)) <= len(pstate.memory.read_string(s2)) else s2
     #for i in range(size):
@@ -1686,15 +1688,15 @@
     return res
 
 
 def rtn_strcpy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strcpy behavior.
     """
-    logging.debug('strcpy hooked')
+    logger.debug('strcpy hooked')
 
     dst  = pstate.get_argument_value(0)
     src  = pstate.get_argument_value(1)
     src_str = pstate.memory.read_string(src)
     size = len(src_str)
 
     # constraint src buff to be != \00 and last one to be \00 (indirectly concretize length)
@@ -1710,15 +1712,15 @@
     return dst
 
 
 def rtn_strdup(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strdup behavior.
     """
-    logging.debug('strdup hooked')
+    logger.debug('strdup hooked')
 
     s  = pstate.get_argument_value(0)
     s_str = pstate.memory.read_string(s)
     size = len(s_str)
 
     #print(f"strdup s={s:#x} s_str={s_str} size={size}")
 
@@ -1743,15 +1745,15 @@
     """
     The strerror behavior.
 
     :param se: The current symbolic execution instance
     :param pstate: The current process state
     :return: a concrete value
     """
-    logging.debug('strerror hooked')
+    logger.debug('strerror hooked')
 
     sys_errlist = [
         b"Success",
         b"Operation not permitted",
         b"No such file or directory",
         b"No such process",
         b"Interrupted system call",
@@ -1901,15 +1903,15 @@
     return ptr
 
 
 def rtn_strlen(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strlen behavior.
     """
-    logging.debug('strlen hooked')
+    logger.debug('strlen hooked')
 
     ptr_bit_size = pstate.ptr_bit_size
 
     # Get arguments
     s = pstate.get_argument_value(0)
     ast = pstate.actx
 
@@ -1935,15 +1937,15 @@
     return res
 
 
 def rtn_strncasecmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strncasecmp behavior.
     """
-    logging.debug('strncasecmp hooked')
+    logger.debug('strncasecmp hooked')
 
     s1 = pstate.get_argument_value(0)
     s2 = pstate.get_argument_value(1)
     sz = pstate.get_argument_value(2)
     maxlen = min(sz, min(len(pstate.memory.read_string(s1)), len(pstate.memory.read_string(s2))) + 1)
 
     ptr_bit_size = pstate.ptr_bit_size
@@ -1960,15 +1962,15 @@
     return res
 
 
 def rtn_strncmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strncmp behavior.
     """
-    logging.debug('strncmp hooked')
+    logger.debug('strncmp hooked')
 
     s1 = pstate.get_argument_value(0)
     s2 = pstate.get_argument_value(1)
     sz = pstate.get_argument_value(2)
     maxlen = min(sz, min(len(pstate.memory.read_string(s1)), len(pstate.memory.read_string(s2))) + 1)
 
     ptr_bit_size = pstate.ptr_bit_size
@@ -1983,15 +1985,15 @@
     return res
 
 
 def rtn_strncpy(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strncpy behavior.
     """
-    logging.debug('strncpy hooked')
+    logger.debug('strncpy hooked')
 
     dst = pstate.get_argument_value(0)
     src = pstate.get_argument_value(1)
     cnt = pstate.get_argument_value(2)
 
     pstate.concretize_argument(2)
 
@@ -2008,15 +2010,15 @@
     return dst
 
 
 def rtn_strtok_r(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strtok_r behavior.
     """
-    logging.debug('strtok_r hooked')
+    logger.debug('strtok_r hooked')
 
     string  = pstate.get_argument_value(0)
     delim   = pstate.get_argument_value(1)
     saveptr = pstate.get_argument_value(2)
     saveMem = pstate.memory.read_ptr(saveptr)
 
     if string == 0:
@@ -2053,15 +2055,15 @@
     return NULL_PTR
 
 
 def rtn_strtoul(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The strtoul behavior.
     """
-    logging.debug('strtoul hooked')
+    logger.debug('strtoul hooked')
 
     nptr   = pstate.get_argument_value(0)
     nptrs  = pstate.get_string_argument(0)
     endptr = pstate.get_argument_value(1)
     base   = pstate.get_argument_value(2)
 
     for i, c in enumerate(nptrs):
@@ -2082,15 +2084,15 @@
     # TODO
     name = pstate.get_argument_value(0)
 
     if name == 0:
         return NULL_PTR
 
     environ_name = pstate.memory.read_string(name)
-    logging.warning(f"Target called getenv({environ_name})")
+    logger.warning(f"Target called getenv({environ_name})")
     host_env_val = os.getenv(environ_name)
     return host_env_val if host_env_val is not None else 0
 
 
 #def rtn_tolower(se: 'SymbolicExecutor', pstate: 'ProcessState'):
 #    # TODO
 #    """
@@ -2121,67 +2123,67 @@
 def rtn_assert_fail(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The __assert_fail behavior.
     """
     msg = pstate.get_argument_value(0)
 
     msg = pstate.memory.read_string(msg)
-    logging.warning(f"__assert_fail called : {msg}")
+    logger.warning(f"__assert_fail called : {msg}")
 
     # Write 1 as return value of the program
     pstate.write_register(pstate.return_register, 1)
     se.abort()
 
 def rtn_setlocale(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The setlocale behavior.
     """
-    logging.debug('setlocale hooked')
+    logger.debug('setlocale hooked')
 
     category = pstate.get_argument_value(0)
     locale   = pstate.get_argument_value(1)
 
     if locale != 0:
-        logging.warning(f"Attempt to modify Locale. Currently not supported.")
+        logger.warning(f"Attempt to modify Locale. Currently not supported.")
         return 0
 
     # This is a bit hacky but we just store the LOCALEs in the [extern] segment
     segs = pstate.memory.find_map(pstate.EXTERN_SEG)
     if segs:
         map = segs[0]
         LC_ALL = map.start + map.size - 0x20 # Point to the end of seg. But keep in mind LC_ALL is at end - 4.
     else:
         assert False
     print(f"selocale writing at {LC_ALL:#x}")
 
     if category == 0:
         pstate.memory.write(LC_ALL, b"en_US.UTF-8\x00")
     else:
-        logging.warning(f"setlocale called with unsupported category={category}.")
+        logger.warning(f"setlocale called with unsupported category={category}.")
 
     return LC_ALL
 
 
 def rtn__setjmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The _setjmp behavior. 
     """
     # TODO
-    logging.warning("hooked _setjmp")
+    logger.warning("hooked _setjmp")
     return 0
 
 
 def rtn_longjmp(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The longjmp behavior.
     """
     # NOTE All the programs tested so far used `longjmp` as an error handling mechanism, right
     # before exiting. This is why, `longjmp` is currently considered an exit condition. 
     # TODO Real implementation
-    logging.debug('longjmp hooked')
+    logger.debug('longjmp hooked')
     pstate.stop = True
 
 def rtn_atexit(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     return 0
 
 
 SUPPORTED_ROUTINES = {
```

### Comparing `tritondse-0.1.4/tritondse/sanitizers.py` & `tritondse-0.1.5/tritondse/sanitizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
-import logging
 
-from triton import MemoryAccess, CPUSIZE, Instruction
+from triton import Instruction
 from tritondse.callbacks import CbType, ProbeInterface
 from tritondse.seed import Seed, SeedStatus
 from tritondse.types import Architecture, Addr, Tuple, SolverStatus
 from tritondse import SymbolicExecutor, ProcessState
+import tritondse.logging
+
+logger = tritondse.logging.get("sanitizers")
+
 
 
 def mk_new_crashing_seed(se, model) -> Seed:
     """
     This function is used by every sanitizers to dump the model found in order
     to trigger a bug into the crash directory.
 
@@ -51,15 +54,15 @@
         :param ptr: pointer address to check
         :type ptr: :py:obj:`tritondse.types.Addr`
         :param description: description string printed in logger if an issue is detected
         :return: True if the bug is present
         """
         if pstate.is_heap_ptr(ptr) and pstate.heap_allocator.is_ptr_freed(ptr):
             if description:
-                logging.critical(description)
+                logger.critical(description)
             se.seed.status = SeedStatus.CRASH
             pstate.stop = True
             return True
         return False
 
     @staticmethod
     def _memory_read(se, pstate, mem):
@@ -120,15 +123,15 @@
         # en fin de page mappée. Lors du fetching des opcodes, nous fetchons 16 bytes car
         # nous ne connaissons pas la taille d'une instruction, ici, en fetchant en fin de
         # page on déclenche ce sanitizer...
 
         # FIXME: Why do we call is_valid_memory_mapping ? It is not a "Null Deref vulnerability", it is more a segmentation error
         if ptr == 0 or (pstate.memory.segmentation_enabled and not pstate.memory.is_mapped(ptr)):
             if description:
-                logging.critical(description)
+                logger.critical(description)
             se.seed.status = SeedStatus.CRASH
             pstate.stop = True
             return True
 
         return False
 
     @staticmethod
@@ -183,15 +186,15 @@
         while se.pstate.memory.read_uchar(cur_ptr):  # while different from 0
             if se.pstate.is_memory_symbolic(cur_ptr, 1):
                 symbolic_cells.append(cur_ptr)
             cur_ptr += 1
 
         if symbolic_cells:
             extra = f"(function {extra_data[0]}@{extra_data[1]:#x})" if extra_data else ""
-            logging.warning(f'Potential format string of length {len(symbolic_cells)} on {fmt_ptr:x} {extra}')
+            logger.warning(f'Potential format string of length {len(symbolic_cells)} on {fmt_ptr:x} {extra}')
             se.seed.status = SeedStatus.OK_DONE
             pp_seeds = []
             nopp_seeds = []
 
             for i in range(int(len(symbolic_cells) / 2)):
                 # FIXME: Does not check that cell1 and cell2 are contiguous
                 cell1 = pstate.read_symbolic_memory_byte(symbolic_cells.pop(0)).getAst()
@@ -207,19 +210,19 @@
                 if st == SolverStatus.SAT and model:
                     pp_seeds.append(mk_new_crashing_seed(se, model))
 
             # If found some seeds
             if pp_seeds:
                 s = pp_seeds[-1]
                 se.enqueue_seed(s)  # Only keep last seed
-                logging.warning(f'Found model that might lead to a crash: {s.hash} (with path predicate)')
+                logger.warning(f'Found model that might lead to a crash: {s.hash} (with path predicate)')
             if nopp_seeds:
                 s = nopp_seeds[-1]
                 se.enqueue_seed(s)  # Only keep last seed
-                logging.warning(f'Found model that might lead to a crash: {s.hash} (without path predicate)')
+                logger.warning(f'Found model that might lead to a crash: {s.hash} (without path predicate)')
 
             # Do not stop the execution, just continue the execution
             pstate.stop = False
             return True
         return False
 
     @staticmethod
@@ -261,23 +264,23 @@
         """
         # This probe is only available for X86_64 and AARCH64
         assert(pstate.architecture == Architecture.X86_64 or pstate.architecture == Architecture.AARCH64)
 
         rf = (pstate.registers.of if pstate.architecture == Architecture.X86_64 else pstate.registers.v)
 
         if pstate.read_register(rf):
-            logging.warning(f'Integer overflow at {instruction}')
+            logger.warning(f'Integer overflow at {instruction}')
             # FIXME: What if it's normal behavior?
             se.seed.status = SeedStatus.CRASH
             return True
 
         else:  # if no overflow took place check if symbolic and if so, if it can be 1
             if pstate.is_register_symbolic(rf):
                 sym_flag = pstate.read_symbolic_register(rf)
                 _, model = pstate.solve_no_pp(sym_flag.getAst() == 1)
                 if model:
-                    logging.warning(f'Potential integer overflow at {instruction}')
+                    logger.warning(f'Potential integer overflow at {instruction}')
                     crash_seed = mk_new_crashing_seed(se, model)
                     se.enqueue_seed(crash_seed)
                     return True
 
         return False
```

### Comparing `tritondse-0.1.4/tritondse/seed.py` & `tritondse-0.1.5/tritondse/seed.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/seeds_manager.py` & `tritondse-0.1.5/tritondse/seeds_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # built-in imports
-import logging
 import time
 import json
 from typing import Generator, Optional, Type
 from collections import Counter
 
 # local imports
 from tritondse.seed              import Seed, SeedStatus
 from tritondse.callbacks         import CallbackManager
 from tritondse.coverage          import GlobalCoverage, CovItem, CoverageStrategy
 from tritondse.worklist          import WorklistAddressToSet, FreshSeedPrioritizerWorklist, SeedScheduler
 from tritondse.workspace         import Workspace
 from tritondse.symbolic_executor import SymbolicExecutor
 from tritondse.types             import SolverStatus, SymExType
+import tritondse.logging
+
+logger = tritondse.logging.get("seedmanager")
 
 
 class SeedManager:
     """
     Seed Manager.
     This class is in charge of providing the next seed to execute by prioritizing
     them. It also holds various sets of pending seeds, corpus, crashes etc and
@@ -134,72 +136,72 @@
         # Update instructions covered from the last execution into our exploration coverage
         self.coverage.merge(execution.coverage)
         self.worklist.update_worklist(execution.coverage)
 
         # if the seed have target checks that we covered it
         if seed.target:
             color = ("YES", 92) if execution.coverage.is_covered(seed.target) else ("NO", 91)
-            logging.info(f"Seed covered its target: \033[{color[1]}m{color[0]}\033[0m")
+            logger.info(f"Seed covered its target: \033[{color[1]}m{color[0]}\033[0m")
 
         # reset the current solving time
         self._current_solv_time = 0
 
         # Iterate all pending seeds to be added in the right location
         for s in execution.pending_seeds:
             if self.is_new_seed(s):
                 if not s.coverage_objectives:      # If they don't have objectives set the Ellipsis wildcard
                     s.coverage_objectives.add(...)
                 self._add_seed(s)  # will add the seed in both internal queues & workspace
             else:
-                logging.warning(f"dropping enqueued seed: {s.hash} (already seen)")
+                logger.warning(f"dropping enqueued seed: {s.hash} (already seen)")
 
         # Update the current seed queue
         if seed.status == SeedStatus.NEW:
-            logging.error(f"seed not meant to be NEW at the end of execution ({seed.hash}) (dropped)")
+            logger.error(f"seed not meant to be NEW at the end of execution ({seed.hash}) (dropped)")
             self.drop_seed(seed)
 
         elif seed.status in [SeedStatus.HANG, SeedStatus.CRASH]:
             self.archive_seed(seed)
             # NOTE: Do not perform further processing on the seed (like generating inputs from it)
 
         elif seed.status == SeedStatus.OK_DONE:
             if self.coverage.can_improve_coverage(execution.coverage) or self.coverage.can_cover_symbolic_pointers(execution):
                 items = self.coverage.new_items_to_cover(execution.coverage)
                 seed.coverage_objectives = items  # Set its new objectives
 
                 if self.worklist.can_solve_models() and solve_new_path:     # No fresh seeds pending thus can solve model
-                    logging.info(f'Seed {seed.hash} generate new coverage')
+                    logger.info(f'Seed {seed.hash} generate new coverage')
                     self._generate_new_inputs(execution)
                     self.archive_seed(seed)
                 else:
-                    logging.info(f"Seed {seed.hash} push back in worklist (to unstack fresh)")
+                    logger.info(f"Seed {seed.hash} push back in worklist (to unstack fresh)")
                     seed.status = SeedStatus.NEW  # Reset its status for later run
                     self.add_seed_queue(seed)  # will be pushed back in worklist
             else:
                 self.archive_seed(seed)
-                logging.info(f'Seed {seed.hash} archived cannot generate new coverage [{seed.status.name}]')
+                logger.info(f'Seed {seed.hash} archived cannot generate new coverage [{seed.status.name}]')
 
         else:
             assert False
 
-        logging.info(f"Corpus:{len(self.corpus)} Crash:{len(self.crash)}")
+        logger.info(f"Corpus:{len(self.corpus)} Crash:{len(self.crash)}")
         self.worklist.post_execution()
-        logging.info(f"Coverage instruction:{self.coverage.unique_instruction_covered} covitem:{self.coverage.unique_covitem_covered}")
+        logger.info(f"Coverage instruction:{self.coverage.unique_instruction_covered} covitem:{self.coverage.unique_covitem_covered}")
         return self._current_solv_time
 
     def _generate_new_inputs(self, execution: SymbolicExecutor):
         # Generate new inputs
         for new_input in self.__iter_new_inputs(execution):
             # Check if we already have executed this new seed
             if self.is_new_seed(new_input):
                 self.worklist.add(new_input)
                 self.workspace.save_seed(new_input)
-                logging.info(f'New seed model {new_input.filename} dumped [{new_input.status.name}]')
+                logger.info(f'New seed model {new_input.filename} dumped [{new_input.status.name}]')
             else:
-                logging.info(f"New seed {new_input.filename} has already been generated")
+                logger.info(f"New seed {new_input.filename} has already been generated")
 
     def __iter_new_inputs(self, execution: SymbolicExecutor) -> Generator[Seed, None, None]:
         # Get the astContext
         actx = execution.pstate.actx
 
         # We start with any input. T (Top)
         path_predicate = [actx.equal(actx.bvtrue(), actx.bvtrue())]
@@ -214,15 +216,15 @@
         path_generator = self.coverage.iter_new_paths(path_constraints)
 
         try:
             while True:
                 # If smt_queries_limit is zero: unlimited queries
                 # If smt_queries_limit is negative: no query
                 if self.smt_queries_limit < 0:
-                    logging.info(f'The configuration is defined as: no query')
+                    logger.info(f'The configuration is defined as: no query')
                     break
 
                 typ, p_prefix, branch, covitem, ith = path_generator.send(status)
 
                 # Create edge in case of conditional branch, for all the other the edge shall be already set
                 edge = (branch['srcAddr'], branch['dstAddr']) if typ == SymExType.CONDITIONAL_JMP else covitem
 
@@ -247,30 +249,30 @@
                     # all stats updates
                     solve_time = time.time() - ts
                     count = len(results)
                     status = SolverStatus.SAT if count else SolverStatus.UNSAT
                     self._update_solve_stats(None, status, solve_time, count)
 
                     results = [(x[0], (addr, x[1])) for x in results]   # extract results
-                    logging.info(f'pc:{ith}/{total_len} | Query n°{smt_queries}-{smt_queries+count}, enumerate:{expr} (time: {solve_time:.02f}s) values:[{count}:{self._pp_smt_status(status)}]')
+                    logger.info(f'pc:{ith}/{total_len} | Query n°{smt_queries}-{smt_queries+count}, enumerate:{expr} (time: {solve_time:.02f}s) values:[{count}:{self._pp_smt_status(status)}]')
                     smt_queries += count+1  # for the unsat
 
                 elif typ == SymExType.CONDITIONAL_JMP:
                     # if debug_pp=True solve the branch that has been taken
                     branch_cst = actx.lnot(branch['constraint']) if execution.debug_pp else branch['constraint']
                     constraint = actx.land(path_predicate + [branch_cst])
 
                     # Solve the constraint
                     ts = time.time()
                     status, model = execution.pstate.solve(constraint, with_pp=False)  # Do not use path predicate as we are iterating it
                     solve_time = time.time() - ts
                     self._update_solve_stats(covitem, status, solve_time)
                     results = [(model, covitem)]
                     smt_queries += 1
-                    logging.info(f'pc:{ith}/{total_len} | Query n°{smt_queries}, solve:{self.coverage.pp_item(covitem)} (time: {solve_time:.02f}s) [{self._pp_smt_status(status)}]')
+                    logger.info(f'pc:{ith}/{total_len} | Query n°{smt_queries}, solve:{self.coverage.pp_item(covitem)} (time: {solve_time:.02f}s) [{self._pp_smt_status(status)}]')
                 else:
                     assert False
 
                 if status == SolverStatus.SAT:
                     for model, covitem in results:
                         new_seed = execution.mk_new_seed_from_model(model)
                         # Trick to keep track of which target a seed is meant to cover
@@ -279,26 +281,26 @@
                         new_seed.target = covitem if typ == SymExType.CONDITIONAL_JMP else None
                         yield new_seed  # Yield the seed to get it added in the worklist
                 else:
                     pass
 
                 # Check if we reached the limit of query
                 if self.smt_queries_limit and smt_queries >= self.smt_queries_limit:
-                    logging.info(f'Limit of query reached. Stop asking for models')
+                    logger.info(f'Limit of query reached. Stop asking for models')
                     break
 
         except StopIteration:  # We have iterated the whole path generator
             pass
 
     def _update_solve_stats(self, covitem: Optional[CovItem], status: SolverStatus, solving_time: float, count=1):
         self._solv_count += count
         self._solv_time_sum += solving_time
         self._current_solv_time += solving_time
         self._solv_status[status] += count
-        logging.debug(f'Solve stats: solve_count={self._solv_count} solving_time={solving_time} solve_time_sum={self._solv_time_sum} current_solve_time={self._current_solv_time} solv_status={status} / {self._solv_status[status]}')
+        logger.debug(f'Solve stats: solve_count={self._solv_count} solving_time={solving_time} solve_time_sum={self._solv_time_sum} current_solve_time={self._current_solv_time} solv_status={status} / {self._solv_status[status]}')
 
         if covitem:
             if status == SolverStatus.SAT:
                 self._stat_branch_reverted[covitem] += count  # Update stats
                 if covitem in self._stat_branch_fail:
                     self._stat_branch_fail.pop(covitem)
             elif status == SolverStatus.UNSAT:
@@ -328,17 +330,17 @@
         The function uses its type to know where to add the seed.
 
         :param seed: seed to add
         :type seed: Seed
         """
         if self.is_new_seed(seed):
             self._add_seed(seed)
-            logging.debug(f'Seed {seed.filename} dumped [{seed.status.name}]')
+            logger.debug(f'Seed {seed.filename} dumped [{seed.status.name}]')
         else:
-            logging.debug(f"seed {seed} is already known (not adding it)")
+            logger.debug(f"seed {seed} is already known (not adding it)")
 
     def _add_seed(self, seed: Seed) -> None:
         """ Add the seed in both internal queues but also workspace """
         self.add_seed_queue(seed)
         self.workspace.save_seed(seed)
 
     def drop_seed(self, seed: Seed) -> None:
@@ -383,15 +385,15 @@
             "branch_reverted": {str(k): v for k, v in self._stat_branch_reverted.items()}, # convert covitem to str whatever it is
             "branch_not_solved": {str(k): v for k, v in self._stat_branch_fail.items()},  # convert covitem to str whatever it is
             "UNSAT": self._solv_status[SolverStatus.UNSAT],
             "SAT": self._solv_status[SolverStatus.SAT],
             "TIMEOUT": self._solv_status[SolverStatus.TIMEOUT]
         }
         self.workspace.save_metadata_file("solving_stats.json", json.dumps(stats, indent=2))
-        logging.info(f"Branches reverted: {len(self._stat_branch_reverted)}  Branches still fail: {len(self._stat_branch_fail)}")
+        logger.info(f"Branches reverted: {len(self._stat_branch_reverted)}  Branches still fail: {len(self._stat_branch_fail)}")
         self.worklist.post_exploration(self.workspace)
 
     @staticmethod
     def _pp_smt_status(status: SolverStatus) -> str:
         """ The pretty print function of the solver status """
         mapper = {SolverStatus.SAT: 92, SolverStatus.UNSAT: 91, SolverStatus.TIMEOUT: 93, SolverStatus.UNKNOWN: 95}
         return f"\033[{mapper[status]}m{status.name}\033[0m"
```

### Comparing `tritondse-0.1.4/tritondse/symbolic_executor.py` & `tritondse-0.1.5/tritondse/symbolic_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # built-in imports
 import io
-import logging
 import time
 import os
 import resource
-from typing import Optional, Union, List, NoReturn, Dict
+from typing import Optional, Union, List, NoReturn, Dict, Type
 
 # third party imports
 from triton import MODE, Instruction, CPUSIZE, MemoryAccess, CALLBACK
 
 # local imports
 from tritondse.config import Config
 from tritondse.coverage import CoverageSingleRun, BranchSolvingStrategy
@@ -19,14 +18,17 @@
 from tritondse.routines import SUPPORTED_ROUTINES, SUPORTED_GVARIABLES
 from tritondse.callbacks import CallbackManager
 from tritondse.workspace import Workspace
 from tritondse.heap_allocator import AllocatorException
 from tritondse.thread_context import ThreadContext
 from tritondse.exception import AbortExecutionException, SkipInstructionException, StopExplorationException
 from tritondse.memory import MemoryAccessViolation, Perm
+import tritondse.logging
+
+logger = tritondse.logging.get("executor")
 
 
 class SymbolicExecutor(object):
     """
     Single Program Execution Class.
     That module, is in charge of performing the process loading from the given
     program.
@@ -54,15 +56,15 @@
         if self.workspace is None:
             self.workspace = Workspace(config.workspace)
 
         self.seed: Seed = seed  #: The current seed used for the execution
 
         # Override config if there is a mismatch between seed format and config file
         if seed.format != self.config.seed_format:
-            logging.warning(f"seed format {seed.format} mismatch config {config.seed_format} (override config)")
+            logger.warning(f"seed format {seed.format} mismatch config {config.seed_format} (override config)")
             self.config.seed_format = seed.format
 
         self._symbolic_seed = self._init_symbolic_seed(seed)
 
         self.coverage: CoverageSingleRun = CoverageSingleRun(self.config.coverage_strategy)  #: Coverage of the execution
         self.rtn_table = dict()   # Addr -> Tuple[fname, routine]
         self.uid: int = uid       #: Unique identifier meant to unique accross Exploration instances
@@ -106,15 +108,15 @@
 
         :param loader: Loader describing how to load
         :return: None
         """
 
         # Initialize the process_state architecture (at this point arch is sure to be supported)
         self.loader = loader
-        logging.debug(f"Loading program {self.loader.name} [{self.loader.architecture}]")
+        logger.debug(f"Loading program {self.loader.name} [{self.loader.architecture}]")
         self.pstate = ProcessState.from_loader(loader)
         self._map_dynamic_symbols()
         self._load_seed_process_state(self.pstate, self.seed)
 
     def load_process(self, pstate: ProcessState) -> None:
         """
         Load the given process state. Do nothing but
@@ -192,15 +194,15 @@
         else:
             assert False
 
     def _configure_pstate(self) -> None:
         #for mode in [MODE.ALIGNED_MEMORY, MODE.AST_OPTIMIZATIONS, MODE.CONSTANT_FOLDING, MODE.ONLY_ON_SYMBOLIZED]:
         for mode in [MODE.ONLY_ON_SYMBOLIZED]:
             self.pstate.set_triton_mode(mode, True)
-        logging.info(f"configure pstate: time_inc:{self.config.time_inc_coefficient}  solver:{self.config.smt_solver.name}  timeout:{self.config.smt_timeout}")
+        logger.info(f"configure pstate: time_inc:{self.config.time_inc_coefficient}  solver:{self.config.smt_solver.name}  timeout:{self.config.smt_timeout}")
         self.pstate.time_inc_coefficient = self.config.time_inc_coefficient
         self.pstate.set_solver_timeout(self.config.smt_timeout)
         self.pstate.set_solver(self.config.smt_solver)
 
     def _fetch_next_thread(self, threads: List[ThreadContext]) -> Optional[ThreadContext]:
         """
         Given a list of threads, returns the next to execute. Iterating
@@ -247,38 +249,38 @@
         tgt_addr = mem.getAddress()
         lea_ast = mem.getLeaAst()
         if lea_ast is None:
             return
         if lea_ast.isSymbolized():
             s = "write" if bool(args) else "read"
             pc = self.pstate.cpu.program_counter
-            logging.debug(f"symbolic {s} at 0x{pc:x}: target: 0x{tgt_addr:x} [{lea_ast}]")
+            logger.debug(f"symbolic {s} at 0x{pc:x}: target: 0x{tgt_addr:x} [{lea_ast}]")
             self.pstate.push_constraint(lea_ast == tgt_addr, f"sym-{s}:{self.trace_offset}:{pc}")
 
     def __emulate(self):
         while not self.pstate.stop and self.pstate.threads:
             # Schedule thread if it's time
             self.__schedule_thread()
 
             if not self.pstate.current_thread.is_running():
-                logging.warning(f"After scheduling current thread is not running (probably in a deadlock state)")
+                logger.warning(f"After scheduling current thread is not running (probably in a deadlock state)")
                 break  # Were not able to find a suitable thread thus exit emulation
 
             # Fetch program counter (of the thread selected), at this point the current thread should be running!
             self.current_pc = self.pstate.cpu.program_counter  # should normally be already set but still.
 
             if self.current_pc == self._run_to_target:  # Hit the location we wanted to reach
                 break
 
             if self.current_pc == 0:
-                logging.error(f"PC=0, is it normal ? (stop)")
+                logger.error(f"PC=0, is it normal ? (stop)")
                 break
 
             if not self.pstate.memory.has_ever_been_written(self.current_pc, CPUSIZE.BYTE):
-                logging.error(f"Instruction not mapped: 0x{self.current_pc:x}")
+                logger.error(f"Instruction not mapped: 0x{self.current_pc:x}")
                 break
 
             instruction = self.pstate.fetch_instruction()
             opcode = instruction.getOpcode()
             mnemonic = instruction.getType()
 
             try:
@@ -301,24 +303,24 @@
                 pre_insts, post_insts = self.cbm.get_instruction_callbacks()
                 for cb in pre_insts:
                     cb(self, self.pstate, instruction)
             except SkipInstructionException as _:
                 continue
 
             if self.pstate.is_syscall():
-                logging.warning(f"execute syscall instruction {self.pstate.read_register(self.pstate._syscall_register)}")
+                logger.warning(f"execute syscall instruction {self.pstate.read_register(self.pstate._syscall_register)}")
 
             # Process
             prev_pc = self.current_pc
             self._in_processing = True
             if not self.pstate.process_instruction(instruction):
                 if self.pstate.is_halt_instruction():
-                    logging.info(f"hit {str(instruction)} instruction stop.")
+                    logger.info(f"hit {str(instruction)} instruction stop.")
                 else:
-                    logging.error('Instruction not supported: %s' % (str(instruction)))
+                    logger.error('Instruction not supported: %s' % (str(instruction)))
 
                 if self.config.skip_unsupported_instruction:
                     self.pstate.cpu.program_counter += instruction.getSize() # try to jump over the instruction
                 else:
                     break  # stop emulation
             self._in_processing = False
             # increment trace offset
@@ -334,15 +336,15 @@
             # Update coverage send it the last PathConstraint object if one was added
             if self.pstate.is_path_predicate_updated():
                 path_constraint = self.pstate.last_branch_constraint
 
                 if path_constraint.isMultipleBranches():
                     branches = path_constraint.getBranchConstraints()
                     if len(branches) != 2:
-                        logging.error("Branching condition has more than two branches")
+                        logger.error("Branching condition has more than two branches")
                     taken, not_taken = branches if branches[0]['isTaken'] else branches[::-1]
                     taken_addr, not_taken_addr = taken['dstAddr'], not_taken['dstAddr']
 
                     for cb in self.cbm.get_on_branch_covered_callback():
                         cb(self, self.pstate, (self.previous_pc, taken_addr))
 
                     self.coverage.add_covered_branch(self.previous_pc, taken_addr, not_taken_addr)
@@ -350,15 +352,15 @@
                 else:  # It is normally a dynamic jump or symbolic memory read/write
                     cmt = path_constraint.getComment()
                     if cmt.startswith("sym-read") or cmt.startswith("sym-write"):
                         pass
                         # NOTE: At the moment it does not seems suitable to count r/w pointers
                         # as part of the coverage. So does not have an influence on covered/not_covered.
                     else:
-                        logging.warning(f"New dynamic jump covered at: {self.previous_pc:08x}")
+                        logger.warning(f"New dynamic jump covered at: {self.previous_pc:08x}")
                         path_constraint.setComment(f"dyn-jmp:{self.trace_offset}:{self.previous_pc}")
                         self.coverage.add_covered_dynamic_branch(self.previous_pc, self.current_pc)
 
             # Trigger post-opcode callback
             for cb in post_opcode:
                 cb(self, self.pstate, opcode)
 
@@ -374,21 +376,21 @@
             for cb in post_cbs:
                 cb(self, self.pstate, self.previous_pc)
 
             # Simulate routines
             try:
                 self._routines_handler(instruction)
             except AllocatorException as e:
-                logging.info(f'An exception has been raised: {e}')
+                logger.info(f'An exception has been raised: {e}')
                 self.seed.status = SeedStatus.CRASH
                 return
 
             # Check timeout of the execution
             if self.config.execution_timeout and (time.time() - self.start_time) >= self.config.execution_timeout:
-                logging.info('Timeout of an execution reached')
+                logger.info('Timeout of an execution reached')
                 self.seed.status = SeedStatus.HANG
                 return
 
         if not self.seed.is_status_set():  # Set a status if it has not already been done
             self.seed.status = SeedStatus.OK_DONE
         return
 
@@ -409,15 +411,15 @@
 
         :param instruction: The current instruction executed
         :return: None
         """
         pc = self.pstate.cpu.program_counter
         if pc in self.rtn_table:
             routine_name, routine = self.rtn_table[pc]
-            logging.debug(f"Enter external routine: {routine_name}")
+            logger.debug(f"Enter external routine: {routine_name}")
 
             # Trigger pre-address callback
             pre_cbs, post_cbs = self.cbm.get_imported_routine_callbacks(routine_name)
 
             ret_val = None
             for cb in pre_cbs:
                 ret = cb(self, self.pstate, routine_name, pc)
@@ -481,24 +483,24 @@
                 self.pstate.memory.write_ptr(addr, SUPORTED_GVARIABLES[symbol])  # write directly at addr
                 # elif self.pstate.architecture == Architecture.AARCH64:
                 #     val = self.pstate.memory.read_ptr(addr)
                 #     self.pstate.memory.write_ptr(val, SUPORTED_GVARIABLES[symbol])
 
             else:  # the symbol is not supported
                 if self.uid == 0:  # print warning if first uid (so that it get printed once)
-                    logging.warning(f"symbol {symbol} imported but unsupported")
+                    logger.warning(f"symbol {symbol} imported but unsupported")
                 if is_func:
                     # Add link to a default stub function
                     self.rtn_table[addr] = (symbol, self.__default_stub)
                 else:
                     pass # do nothing on unsupported symbols
 
     def __default_stub(self, se: 'SymbolicExecutor', pstate: ProcessState):
         rtn_name, _ = self.rtn_table[pstate.cpu.program_counter]
-        logging.warning(f"calling {rtn_name} which is unsupported")
+        logger.warning(f"calling {rtn_name} which is unsupported")
         if self.config.skip_unsupported_import:
             return None  # Like if function did nothing
         else:
             self.abort()
 
     def abort(self) -> NoReturn:
         """
@@ -538,15 +540,15 @@
         :param stop_at: Address where to stop (if necessary)
         :return: None
         """
         if stop_at:
             self._run_to_target = stop_at
 
         if self.pstate is None:
-            logging.error(f"ProcessState is None (have you called \"load\"?")
+            logger.error(f"ProcessState is None (have you called \"load\"?")
             return
 
         self.start_time = time.time()
 
         # Configure memory segmentation using configuration
         self.pstate.memory.set_segmentation(self.config.memory_segmentation)
         if self.config.memory_segmentation:
@@ -559,15 +561,15 @@
         if BranchSolvingStrategy.COVER_SYM_WRITE in self.config.branch_solving_strategy:
             self.cbm.register_memory_write_callback(self._symbolic_mem_callback)
 
         # bind dbm callbacks on the process state (newly initialized)
         self.cbm.bind_to(self)  # bind call
 
         # Let's emulate the binary from the entry point
-        logging.info('Starting emulation')
+        logger.info('Starting emulation')
 
         # Get pre/post callbacks on execution
         pre_cb, post_cb = self.cbm.get_execution_callbacks()
         # Iterate through all pre exec callbacks
         for cb in pre_cb:
             cb(self, self.pstate)
 
@@ -575,15 +577,15 @@
         self._configure_pstate()
 
         try:
             self.__emulate()
         except AbortExecutionException as e:
             pass
         except MemoryAccessViolation as e:
-            logging.warning(f"Memory violation: {str(e)}")
+            logger.warning(f"Memory violation: {str(e)}")
 
             # Call all the callbacks on the memory violations
             for cb in self.callback_manager.get_memory_violation_callbacks():
                 cb(self, self.pstate, e)
 
             # Assign the seed the status of crash
             if not self.seed.is_status_set():
@@ -610,17 +612,17 @@
             self.cbm.unregister_callback(self._mem_accesses_callback)
 
         if BranchSolvingStrategy.COVER_SYM_READ in self.config.branch_solving_strategy:
             self.cbm.unregister_callback(self._symbolic_mem_callback)
         if BranchSolvingStrategy.COVER_SYM_WRITE in self.config.branch_solving_strategy:
             self.cbm.unregister_callback(self._symbolic_mem_callback)
 
-        logging.info(f"Emulation done [ret:{self.pstate.read_register(self.pstate.return_register):x}]  (time:{self.execution_time:.02f}s)")
-        logging.info(f"Instructions executed: {self.coverage.total_instruction_executed}  symbolic branches: {self.pstate.path_predicate_size}")
-        logging.info(f"Memory usage: {self.mem_usage_str()}")
+        logger.info(f"Emulation done [ret:{self.pstate.read_register(self.pstate.return_register):x}]  (time:{self.execution_time:.02f}s)")
+        logger.info(f"Instructions executed: {self.coverage.total_instruction_executed}  symbolic branches: {self.pstate.path_predicate_size}")
+        logger.info(f"Memory usage: {self.mem_usage_str()}")
 
     def _mem_accesses_callback(self, se: 'SymbolicExecutor', ps: ProcessState, mem: MemoryAccess, *args):
         """
         This callback is used to ensure memory accesses performed by side-effect of instructions
         semantic correctly checks memory segmentation. Thus we only do the check during the processing
         of an instruction.
         """
@@ -755,15 +757,15 @@
 
         :param reg: register identifier
         :param name: name of the file in the composite seed
         :param value: integer value
         :param offset: offset within the file
         """
         if reg.getSize != 1:
-            logging.error("can't call inject_symbolic_file_register with regsiter larger than 1!")
+            logger.error("can't call inject_symbolic_file_register with regsiter larger than 1!")
             return
         self.pstate.write_register(reg, value)  # Write concrete value in register
         sym_vars = self.pstate.symbolize_register(reg, f"{name}[{offset}]")  # Symbolize bytes
         sym_seed = self._symbolic_seed.files[name] if self.seed.is_composite() else self._symbolic_seed
         sym_seed[offset] = sym_vars  # Add symbolic variables to symbolic seed
 
     def inject_symbolic_variable_register(self, reg: Union[str, Register], name: str, value: int, offset: int = 0) -> None:
@@ -787,10 +789,10 @@
         be used for RAW seed type.
 
         :param addr: address where to inject input.
         :param data: content of the seed
         :param offset: offset within the content of the seed.
         """
         if self.seed.is_composite():
-            logging.warning("inject_symbolic_memory must not be used with composite seeds !")
+            logger.warning("inject_symbolic_memory must not be used with composite seeds !")
         else:
             self.inject_symbolic_file_memory(addr, "input", data, offset)
```

### Comparing `tritondse-0.1.4/tritondse/symbolic_explorator.py` & `tritondse-0.1.5/tritondse/symbolic_explorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-import logging
 import time
 import threading
 import gc
 from enum import Enum
 from typing import Union, Type
 from pathlib import Path
 import stat
 import enum_tools.documentation
 
 from tritondse.config            import Config
 from tritondse.process_state     import ProcessState
 from tritondse.loaders           import Loader
 from tritondse.seed              import Seed
-from tritondse.seeds_manager     import SeedManager
-from tritondse.worklist          import SeedScheduler
 from tritondse.symbolic_executor import SymbolicExecutor
-from tritondse.callbacks         import CallbackManager
 from tritondse.workspace         import Workspace
 from tritondse.coverage          import GlobalCoverage
 from tritondse.types             import Addr
 from tritondse.exception         import StopExplorationException
+from tritondse.seeds_manager import SeedManager
+from tritondse.worklist import SeedScheduler
+from tritondse.callbacks import CallbackManager
+import tritondse.logging
+
+
+logger = tritondse.logging.get("explorator")
 
 
 @enum_tools.documentation.document_enum
 class ExplorationStatus(Enum):
     """ Enum representing the current state of the exploration """
     NOT_RUNNING = 0  # doc: The explorator has not been started yet
     RUNNING     = 1  # doc: The explorator is running and performing exploration
@@ -62,16 +65,16 @@
         if self.loader:
             bin_path = self.workspace.get_binary_directory() / self.loader.bin_path.name
             if not bin_path.exists():  # If the program is not yet present
                 self.workspace.save_file(bin_path, self.loader.bin_path.read_bytes())
                 self.loader.bin_path = bin_path  # Patch its official new location
                 bin_path.chmod(stat.S_IRWXU)  # Make it executable
 
-        # Configure logfile
-        self._configure_file_logger()
+        # Configure logfile in workspace
+        tritondse.logging.enable_to_file(logger.level, self.workspace.logfile_path)
 
         # Initialize coverage
         self.coverage: GlobalCoverage = GlobalCoverage(self.config.coverage_strategy, self.config.branch_solving_strategy)
         """ GlobalCoverage object holding information about the global coverage.
         *(not really meant to be manipulated by the user)*
         """
         # Load workspace global coverage if any
@@ -117,24 +120,24 @@
         return self._exec_count
 
     def __time_delta(self):
         return time.time() - self.ts
 
     def _worker(self, seed, uid):
         """ Worker thread """
-        logging.info(f'Pick-up seed: {seed.filename} (fresh: {seed.is_fresh()})')
+        logger.info(f'Pick-up seed: {seed.filename} (fresh: {seed.is_fresh()})')
 
         if self.config.exploration_timeout and self.__time_delta() >= self.config.exploration_timeout:
-            logging.info('Exploration timeout')
+            logger.info('Exploration timeout')
             self.stop_exploration()
             return
 
         # Execute the binary with seeds
         cbs = None if self.cbm.is_empty() else self.cbm.fork()
-        logging.info(f"Initialize ProcessState with thread scheduling: {self.config.thread_scheduling}")
+        logger.info(f"Initialize ProcessState with thread scheduling: {self.config.thread_scheduling}")
         execution = SymbolicExecutor(self.config, seed=seed, workspace=self.workspace, uid=uid, callbacks=cbs)
         if self.loader:  # If doing the exploration from a program
             execution.load(self.loader)
         else:
             execution.load_process(ProcessState())
         self.current_executor = execution
 
@@ -143,39 +146,39 @@
 
         ts = time.time()
         try:
             execution.run(self._executor_stop_at)
             expl_ts = time.time() - ts
         except StopExplorationException:
             expl_ts = time.time() - ts
-            logging.info("Exploration interrupted (coverage not integrated)")
+            logger.info("Exploration interrupted (coverage not integrated)")
             self.stop_exploration()
 
         if self.config.exploration_limit and (uid+1) >= self.config.exploration_limit:
-            logging.info('Exploration limit reached')
+            logger.info('Exploration limit reached')
             self.stop_exploration()
 
         # Some analysis in post execution
         solve_time = self.seeds_manager.post_execution(execution, seed, not self._stop)
         self._total_emulation_time += expl_ts
 
-        logging.info(f"Emulation: {self._fmt_secs(expl_ts)} | Solving: {self._fmt_secs(solve_time)} | Elapsed: {self._fmt_secs(self.__time_delta())}\n")
+        logger.info(f"Emulation: {self._fmt_secs(expl_ts)} | Solving: {self._fmt_secs(solve_time)} | Elapsed: {self._fmt_secs(self.__time_delta())}\n")
 
     def step(self) -> None:
         """
         Perform a single exploration step. That means it execute
         a single :py:obj:`SymbolicExecutor`. Then it gives the hand
         back to the user.
         """
         # Take an input
         seed = self.seeds_manager.pick_seed()
 
         # If we don't have any new seed to process just switch exploration to idle
         if seed is None:
-            logging.info("worklist of seed to process is empty")
+            logger.info("worklist of seed to process is empty")
             self.status = ExplorationStatus.IDLE
             return
 
         # Iterate the callback to be called at each steps
         for cb in self.cbm.get_exploration_step_callbacks():
             cb(self)
 
@@ -207,28 +210,28 @@
         try:
             while self.seeds_manager.seeds_available() and not self._stop:
                 gc.collect()
                 self.step()
 
             if self.status == ExplorationStatus.RUNNING:
                 if not self.seeds_manager.seeds_available():
-                    logging.info("exploration step done (no new seed available)")
+                    logger.info("exploration step done (no new seed available)")
                     self.status = ExplorationStatus.IDLE
                 else:
-                    logging.warning(f'should not exit step() in RUNNING state (stop? {self._stop}, seeds available? {self.seeds_manager.seeds_available()})')
+                    logger.warning(f'should not exit step() in RUNNING state (stop? {self._stop}, seeds available? {self.seeds_manager.seeds_available()})')
 
         except KeyboardInterrupt:
-            logging.warning("keyboard interrupt, stop symbolic exploration")
+            logger.warning("keyboard interrupt, stop symbolic exploration")
             self.stop_exploration()
 
         self.post_exploration()
-        logging.info(f"Total time of the exploration: {self._fmt_secs(self.__time_delta())}")
+        logger.info(f"Total time of the exploration: {self._fmt_secs(self.__time_delta())}")
 
         if self.status == ExplorationStatus.IDLE:
-            logging.info("Execution IDLE no seeds to execute")
+            logger.info("Execution IDLE no seeds to execute")
 
         return self.status
 
     def add_input_seed(self, seed: Union[bytes, Seed]) -> None:
         """
         Add the given bytes or Seed object as input for the exploration.
 
@@ -254,14 +257,7 @@
         h, m = divmod(m, 60)
         return (f"{int(h)}h" if h else '')+f"{int(m)}m{int(s)}s"
 
     def post_exploration(self) -> None:
         """ Perform  all calls to post exploration functions"""
         self.seeds_manager.post_exploration()
         self.coverage.post_exploration(self.workspace)
-
-    def _configure_file_logger(self) -> None:
-        """ Configure the filehandler to log to file """
-        hldr = logging.FileHandler(self.workspace.logfile_path)
-        hldr.setLevel(logging.DEBUG)
-        hldr.setFormatter(logging.Formatter("%(asctime)s %(threadName)s [%(levelname)s] %(message)s"))
-        logging.root.addHandler(hldr)
```

### Comparing `tritondse-0.1.4/tritondse/thread_context.py` & `tritondse-0.1.5/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/trace.py` & `tritondse-0.1.5/tritondse/trace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # built-in imports
 import json
-import logging
 import os
 import subprocess
-import tempfile
-from abc import ABC
 from pathlib import Path
 from typing import List, Optional, Union
 from collections import Counter
 
 
 # local imports
 import tritondse # NOTE We need this import so we can use it to determine the path of this file.
 from tritondse import Config, Program, SymbolicExecutor, CoverageStrategy, CoverageSingleRun
+import tritondse.logging
+
+logger = tritondse.logging.get("tracer")
 
 
 class TraceException(Exception):
     pass
 
 
 class Trace:
@@ -128,15 +128,15 @@
         if stdin_file and not Path(stdin_file).exists():
             raise FileNotFoundError()
 
         args = [] if not args else args
 
         cmdlne = f'python -m pyqbdipreload {QBDITrace.QBDI_SCRIPT_FILEPATH}'.split(' ') + [binary_path] + args
 
-        logging.debug(f'Command line: {" ".join(cmdlne)}')
+        logger.debug(f'Command line: {" ".join(cmdlne)}')
 
         # Set environment variables.
         environ = {
             'PYQBDIPRELOAD_COVERAGE_STRATEGY': strategy.name,
             'PYQBDIPRELOAD_OUTPUT_FILEPATH': output_path,
             'PYQBDIPRELOAD_DUMP_TRACE': str(dump_trace),
             'LD_BIND_NOW': '1',
@@ -147,20 +147,20 @@
         stdin_fp = open(stdin_file, 'rb') if stdin_file else None
 
         # Run QBDI tool.
         process = subprocess.Popen(cmdlne, stdin=stdin_fp, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=cwd, env=environ)
         try:
             stdout, stderr = process.communicate(timeout=timeout)
             for line in stdout.split(b"\n"):
-                logging.debug(f"stdout: {line}")
+                logger.debug(f"stdout: {line}")
             for line in stderr.split(b"\n"):
-                logging.debug(f"stdout: {line}")
+                logger.debug(f"stdout: {line}")
         except subprocess.TimeoutExpired:
             process.wait()
-            logging.error('QBDI tracer timeout expired!')
+            logger.error('QBDI tracer timeout expired!')
             raise TraceException('QBDI tracer timeout expired')
 
         if stdin_fp:
             stdin_fp.close()
 
         return Path(output_path).exists()
 
@@ -169,15 +169,15 @@
         """Load coverage from a file.
 
         :param coverage_path: Path to the coverage file.
         :type coverage_path: :py:obj:`str`.
         """
         trace = QBDITrace()
 
-        logging.debug(f'Loading coverage file: {coverage_path}')
+        logger.debug(f'Loading coverage file: {coverage_path}')
         with open(coverage_path, 'rb') as fd:
             data = json.load(fd)
 
         cov = CoverageSingleRun(CoverageStrategy[data["coverage_strategy"]])
         cov.covered_instructions = Counter({int(k): v for k, v in data["covered_instructions"].items()})
 
         for (src, dst, not_taken) in data["covered_items"]:
@@ -196,15 +196,15 @@
     def coverage(self) -> CoverageSingleRun:
         """
         CoverageSingleRun associated with the trace.
 
         :return: coverage object
         """
         if not self._coverage:
-            logging.warning("Please .run() the trace before querying coverage")
+            logger.warning("Please .run() the trace before querying coverage")
 
         return self._coverage
 
     @property
     def trace(self) -> List[int]:
         """
         List of addresses executed.
@@ -216,13 +216,13 @@
 
 if __name__ == "__main__":
     import sys
     if len(sys.argv) < 2:
         print("Usage: trace.py program [args]")
         sys.exit(1)
 
-    logging.basicConfig(level=logging.DEBUG)
+    tritondse.logging.enable()
 
     if QBDITrace.run(CoverageStrategy.EDGE, sys.argv[1], sys.argv[2:], "/tmp/test.cov", dump_trace=False):
         coverage = QBDITrace.from_file("/tmp/test.cov")
     else:
         print("Something went wrong during trace generation")
```

### Comparing `tritondse-0.1.4/tritondse/types.py` & `tritondse-0.1.5/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.4/tritondse/worklist.py` & `tritondse-0.1.5/tritondse/worklist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # built-in imports
 import json
-import logging
 from typing import Optional
 
 # Local imports
 from tritondse.seed import Seed
 from tritondse.coverage import GlobalCoverage
 from tritondse.workspace import Workspace
+import tritondse.logging
+
+logger = tritondse.logging.get("seedmanager")
 
 
 class SeedScheduler:
     """
     Abstract class for all seed selection strategies.
     This class provides the base methods that all
     subclasses should implement to be compliant with
@@ -314,15 +316,15 @@
                 self.worklist.pop(it)
         return seed
 
     def post_execution(self) -> None:
         """
         Solely used to show intermediate statistics
         """
-        logging.info(f"Seed Scheduler: worklist:{len(self)} Coverage objectives:{len(self.worklist)}  (fresh:{len(self.fresh)})")
+        logger.info(f"Seed Scheduler: worklist:{len(self)} Coverage objectives:{len(self.worklist)}  (fresh:{len(self.fresh)})")
 
     def post_exploration(self, workspace: Workspace) -> None:
         """
         At the end of the execution, print the worklist to know
         its state before exit.
         """
         workspace.save_metadata_file("coverage_objectives.json", json.dumps(list(self.worklist.keys())))
```

### Comparing `tritondse-0.1.4/tritondse/workspace.py` & `tritondse-0.1.5/tritondse/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # built-in imports
 from __future__ import annotations
 import shutil
 from pathlib import Path
-import logging
 from typing import Generator, Optional, Union
 import time
 
 # local imports
 from tritondse.types import PathLike
 from tritondse.seed import Seed, SeedStatus
+import tritondse.logging
+
+logger = tritondse.logging.get()
 
 
 class Workspace(object):
     """
     Class to abstract the file tree of the current exploration workspace.
     A user willing to save additional files in the workspace is invited
     to do it from the workspace API as it somehow abstract the exact
@@ -50,15 +52,15 @@
 
         :param flush: if True deletes all files contained in the workspace
         :type flush: bool
         """
 
         for dir in (self.root_dir / x for x in [self.CORPUS_DIR, self.CRASH_DIR, self.HANG_DIR, self.WORKLIST_DIR, self.METADATA_DIR, self.BIN_DIR]):
             if not dir.exists():
-                logging.debug(f"Creating the {dir} directory")
+                logger.debug(f"Creating the {dir} directory")
                 dir.mkdir(parents=True)
             else:
                 if flush:
                     shutil.rmtree(dir)
                     dir.mkdir()
 
     def get_metadata_file(self, name: str) -> Optional[str]:
@@ -182,15 +184,15 @@
         :param seed: seed to move
         :type seed: Seed
         """
         old_p = (self.root_dir / self.WORKLIST_DIR) / seed.filename
         try:
             old_p.unlink()  # Remove the seed from the worklist
         except:
-            logging.warning(f"seed {seed} unlink failed")
+            logger.warning(f"seed {seed} unlink failed")
             pass  # FIXME: Not meant to get here
         self.save_seed(seed)
 
     def save_file(self, rel_path: PathLike, content: Union[str, bytes], override: bool = False):
         """
         Save a, arbitrary file in the workspace by providing the relative path
         of the file. If ``override`` is True, erase the previous file if any.
```

### Comparing `tritondse-0.1.4/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.5/tritondse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.4 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.5 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.4/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.5/tritondse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 tritondse/__init__.py
 tritondse/arch.py
 tritondse/callbacks.py
 tritondse/config.py
 tritondse/coverage.py
 tritondse/exception.py
 tritondse/heap_allocator.py
+tritondse/logging.py
 tritondse/memory.py
 tritondse/process_state.py
 tritondse/qbdi_trace.py
 tritondse/routines.py
 tritondse/sanitizers.py
 tritondse/seed.py
 tritondse/seeds_manager.py
```

