# Comparing `tmp/mknodes-0.1.0.tar.gz` & `tmp/mknodes-0.2.0.tar.gz`

## Comparing `mknodes-0.1.0.tar` & `mknodes-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,67 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mknodes-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 mknodes-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mknodes-0.1.0/Makefile
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 mknodes-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mknodes-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mknodes-0.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 mknodes-0.1.0/docs/gen_pages.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mknodes-0.1.0/docs/gen_qt.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/admonition.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/baseclasstable.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/binaryimage.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classdiagram.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classhelpers.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classpage.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classtable.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/code.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/connectionbuilder.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/diagram.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/docstrings.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/image.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/link.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/list.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/markdownnode.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/mermaid.py
--rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/mkpage.py
--rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/moduledocumentation.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/modulepage.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/moduletable.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/nav.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/node.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/noderesolver.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/snippet.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/sourceandresult.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/table.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/tabs.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_add.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_docstrings.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_image.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_list.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_markdownnode.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_mkpage.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_tabblock.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_text.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 mknodes-0.1.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mknodes-0.1.0/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mknodes-0.1.0/README.md
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 mknodes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mknodes-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mknodes-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mknodes-0.2.0/Makefile
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 mknodes-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mknodes-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mknodes-0.2.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mknodes-0.2.0/docs/gen_pages.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mknodes-0.2.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/classhelpers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/connectionbuilder.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mermaid.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkbaseclasstable.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclasspage.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkclasstable.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkimage.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mklink.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mklist.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkmoduletable.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mknav.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mknode.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mkshields.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktable.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/mktext.py
+-rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/node.py
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/noderesolver.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 mknodes-0.2.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_add.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_admonition.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_image.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_list.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_manual.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_mkpage.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_modulepage.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mknodes-0.2.0/tests/test_text.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 mknodes-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mknodes-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mknodes-0.2.0/README.md
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 mknodes-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.2.0/PKG-INFO
```

### Comparing `mknodes-0.1.0/.pre-commit-config.yaml` & `mknodes-0.2.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,14 @@
       # args: [--ignore-missing-imports]
       additional_dependencies: [types-typed-ast]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   rev: v0.0.278
   hooks:
     - id: ruff
+
+- repo: https://github.com/commitizen-tools/commitizen
+  rev: 3.5.2
+  hooks:
+    - id: commitizen
+      stages: [commit-msg]
+      additional_dependencies: [typing-extensions]
```

### Comparing `mknodes-0.1.0/Makefile` & `mknodes-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/mkdocs.yml` & `mknodes-0.2.0/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 theme:
   name: material
   palette:
   # Palette toggle for light mode
   - media: "(prefers-color-scheme: light)"
     scheme: default
+    primary: orange
     toggle:
       icon: material/brightness-7
       name: Switch to dark mode
 
   # Palette toggle for dark mode
   - media: "(prefers-color-scheme: dark)"
     scheme: slate
+    primary: orange
     toggle:
       icon: material/brightness-4
       name: Switch to light mode
   features:
   - content.code.copy
   - content.code.select
   - content.code.annotate
```

### Comparing `mknodes-0.1.0/.github/workflows/build.yml` & `mknodes-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/.github/workflows/documentation.yml` & `mknodes-0.2.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/docs/gen_qt.py` & `mknodes-0.2.0/docs/gen_qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import prettyqt
 import mknodes
 
 prettyqt.import_all()
 
 QT_MODULE_ATTR = "QT_MODULE"
 
-root_nav = mknodes.Nav()
+root_nav = mknodes.MkNav()
 page = mknodes.MkPage(path="index.md", hide_toc=True, hide_nav=True)
 page.add_header("Not in the mood to write documentation? Let´s code it then!", level=3)
 page.write()
 
 qt_docs = root_nav.add_documentation(prettyqt, section_name="Qt modules")
 extra_docs = root_nav.add_documentation(prettyqt, section_name="Additional modules")
```

### Comparing `mknodes-0.1.0/mknodes/__init__.py` & `mknodes-0.2.0/mknodes/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 from __future__ import annotations
 
-from .admonition import Admonition
-from .markdownnode import MkNode, MkContainer, Text
-from .code import Code
-from .docstrings import DocStrings
-from .image import Image
-from .binaryimage import BinaryImage
-from .list import List
-from .diagram import Diagram
-from .classdiagram import ClassDiagram
+from .mkadmonition import MkAdmonition
+from .mknode import MkNode
+from .mktext import MkText
+from .mkcontainer import MkContainer
+from .mkcode import MkCode
+from .mkdocstrings import MkDocStrings
+from .mkimage import MkImage
+from .mkbinaryimage import MkBinaryImage
+from .mklist import MkList
+from .mkdiagram import MkDiagram
+from .mktable import MkTable
+from .mktabs import MkTabBlock, MkTabbed
+from .mksnippet import MkSnippet
+from .mkcritic import MkCritic
+from .mksourceandresult import MkSourceAndResult
+from .mkshields import MkShields
+from .mkpageinclude import MkPageInclude
+
+from .mkclassdiagram import MkClassDiagram
+
+from .mkbaseclasstable import MkBaseClassTable
+from .mkclasstable import MkClassTable
+from .mkmoduletable import MkModuleTable
+
 from .mkpage import MkPage
-from .classpage import ClassPage
-from .modulepage import ModulePage
-from .moduledocumentation import ModuleDocumentation
-from .nav import Nav
-from .table import Table
-from .baseclasstable import BaseClassTable
-from .classtable import ClassTable
-from .moduletable import ModuleTable
-from .tabs import TabBlock, Tabbed
-from .sourceandresult import SourceAndResult
-from .snippet import Snippet
+from .mkclasspage import MkClassPage
+from .mkmodulepage import MkModulePage
+
+from .mknav import MkNav
+from .mkdoc import MkDoc
 
 
 __all__ = [
     "MkNode",
     "MkContainer",
-    "Nav",
-    "DocStrings",
-    "Text",
-    "Code",
-    "Image",
-    "BinaryImage",
+    "MkNav",
+    "MkDocStrings",
+    "MkText",
+    "MkCode",
+    "MkImage",
+    "MkBinaryImage",
     "MkPage",
-    "Admonition",
-    "Diagram",
-    "ClassDiagram",
+    "MkAdmonition",
+    "MkDiagram",
+    "MkClassDiagram",
     "ConnectionBuilder",
-    "Table",
-    "BaseClassTable",
-    "ClassTable",
-    "List",
-    "ClassPage",
-    "ModulePage",
-    "ModuleTable",
-    "ModuleDocumentation",
-    "TabBlock",
-    "Tabbed",
-    "SourceAndResult",
-    "Snippet",
+    "MkTable",
+    "MkBaseClassTable",
+    "MkClassTable",
+    "MkList",
+    "MkClassPage",
+    "MkModulePage",
+    "MkModuleTable",
+    "MkDoc",
+    "MkTabBlock",
+    "MkTabbed",
+    "MkSourceAndResult",
+    "MkSnippet",
+    "MkShields",
+    "MkPageInclude",
+    "MkCritic",
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

### Comparing `mknodes-0.1.0/mknodes/admonition.py` & `mknodes-0.2.0/mknodes/mkadmonition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import textwrap
 
 from typing import Literal
 
-from mknodes import markdownnode
+from mknodes import mktext
 
 
 logger = logging.getLogger(__name__)
 
 AdmonitionTypeStr = Literal[
     "node",
     "abstract",
@@ -22,35 +22,38 @@
     "danger",
     "bug",
     "example",
     "quote",
 ]
 
 
-class Admonition(markdownnode.Text):
+class MkAdmonition(mktext.MkText):
     """Admonition info box."""
 
     def __init__(
         self,
-        typ: AdmonitionTypeStr,
         text: str,
+        typ: AdmonitionTypeStr = "info",
+        *,
         title: str | None = None,
         collapsible: bool = False,
         **kwargs,
     ):
         super().__init__(text=text, **kwargs)
         self.typ = typ
         self.title = title
         self.collapsible = collapsible
 
     def _to_markdown(self) -> str:
+        if not self.text:
+            return ""
         block_start = "???" if self.collapsible else "!!!"
-        title = f'"{self.title}"' if self.title else ""
+        title = f'" {self.title}"' if self.title else ""
         text = textwrap.indent(str(self.text), "    ")
-        return f"{block_start} {self.typ} {title}\n{text}\n\n"
+        return f"{block_start} {self.typ}{title}\n{text}\n"
 
     @staticmethod
     def examples():
         for typ in [
             "node",
             "abstract",
             "info",
@@ -64,27 +67,10 @@
             "example",
             "quote",
         ]:
             yield dict(typ=typ, text=f"This is type {typ}", title=typ)
         yield dict(typ="info", text="This is a collapsible menu", collapsible=True)
 
 
-# class TabWidget(Admonition):
-#     def __init__(
-#         self,
-#         items=None,
-#     ):
-#         super().__init__(header=header)
-#         self.items = items or []
-#         self.title = title
-
-#     def _to_markdown(self) -> str:
-#         lines = [f'!!! Example "{self.title}"']
-
-#         for item in self.items:
-#             header = f"=== {header!r}"
-#             text = textwrap.indent(item.to_markdown(), "        ")
-
-
 if __name__ == "__main__":
-    admonition = Admonition("info", "hello")
+    admonition = MkAdmonition("")
     print(admonition)
```

### Comparing `mknodes-0.1.0/mknodes/baseclasstable.py` & `mknodes-0.2.0/mknodes/mkbaseclasstable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 import logging
 
 from typing import Literal
 
-from mknodes import table, utils
+from mknodes import mktable, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class BaseClassTable(table.Table):
+class MkBaseClassTable(mktable.MkTable):
     """Table showing info for a list of classes."""
 
     def __init__(
         self,
         klasses: list[type],
         *,
-        layout: Literal["default", "extended"] = "extended",
+        layout: Literal["compact", "extended"] = "extended",
         filter_fn: Callable | None = None,
         **kwargs,
     ):
         self.klasses = klasses
         if filter_fn is None:
 
             def always_true(_):
@@ -30,39 +30,40 @@
 
             self.filter_fn = always_true
         else:
             self.filter_fn = filter_fn
         # STRIP_CODE = r"```[^\S\r\n]*[a-z]*\n.*?\n```"
         # docs = [re.sub(STRIP_CODE, '', k.__module__, 0, re.DOTALL) for k in klasses]
         match layout:
-            case "default":
+            case "compact":
                 data = [self.default_row_for_klass(kls) for kls in klasses]
             case "extended":
                 data = [self.extended_row_for_klass(kls) for kls in klasses]
             case _:
                 raise ValueError(layout)
 
         super().__init__(data=data, **kwargs)
 
     def __repr__(self):
         return utils.get_repr(self, klasses=self.klasses)
 
     @staticmethod
     def examples():
-        from mknodes import nav, table
+        from mknodes import mknav
 
-        yield dict(klasses=[table.Table, BaseClassTable, nav.Nav])
-        yield dict(klasses=[table.Table, BaseClassTable, nav.Nav], layout="extended")
+        yield dict(klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav])
+        yield dict(
+            klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav], layout="extended"
+        )
 
     def default_row_for_klass(self, kls: type) -> dict[str, str]:
-        desc = kls.__doc__.split("\n")[0] if isinstance(kls.__doc__, str) else ""
         return dict(
             Class=utils.link_for_class(kls),
             Module=kls.__module__,
-            Description=desc,
+            Description=utils.get_first_doc_line(kls),
         )
 
     def extended_row_for_klass(
         self, kls: type, shorten_lists_after: int = 10
     ) -> dict[str, str]:
         """Return a table row for given class.
 
@@ -72,23 +73,22 @@
         subclass_links = [utils.link_for_class(sub) for sub in subclasses]
         subclass_str = utils.to_html_list(
             subclass_links, shorten_after=shorten_lists_after
         )
         parents = kls.__bases__
         parent_links = [utils.link_for_class(parent) for parent in parents]
         parent_str = utils.to_html_list(parent_links, shorten_after=shorten_lists_after)
-        desc = kls.__doc__.split("\n")[0] if isinstance(kls.__doc__, str) else ""
-        desc = utils.escaped(desc)
+        desc = utils.get_first_doc_line(kls, escape=True)
         name = utils.link_for_class(kls, size=4, bold=True)
         module = utils.styled(kls.__module__, size=1, recursive=True)
         return dict(
             Name=f"{name}<br>{module}<br>{desc}",
             # Module=kls.__module__,
             Children=subclass_str,
             Inherits=parent_str,
             # Description=desc,
         )
 
 
 if __name__ == "__main__":
-    table = BaseClassTable(klasses=[table.Table], layout="extended")
+    table = MkBaseClassTable(klasses=[mktable.MkTable], layout="extended")
     print(table)
```

### Comparing `mknodes-0.1.0/mknodes/binaryimage.py` & `mknodes-0.2.0/mknodes/mkbinaryimage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import logging
 
-from mknodes import image
+from mknodes import mkimage
 
 
 logger = logging.getLogger(__name__)
 
 
-class BinaryImage(image.Image):
+class MkBinaryImage(mkimage.MkImage):
     """Binary data of an image which will become a file when the tree is written."""
 
     def __init__(
         self,
         data: bytes,
         path: str,
         *,
```

### Comparing `mknodes-0.1.0/mknodes/classdiagram.py` & `mknodes-0.2.0/mknodes/mkclassdiagram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import itertools
 
 from typing import Literal
 
-from mknodes import connectionbuilder, diagram, utils
+from mknodes import connectionbuilder, mkdiagram, utils
 
 
 DiagramModeStr = Literal["parent_tree", "subclass_tree", "mro"]
 
 
 class BaseClassConnectionBuilder(connectionbuilder.ConnectionBuilder):
     def __init__(
@@ -36,31 +36,37 @@
         #     return text
 
     def get_attributes(self, item) -> list[str]:
         return [i for i in dir(item) if not i.startswith("__")]
 
 
 class SubclassConnectionBuilder(BaseClassConnectionBuilder):
+    def _connect(self, objects):
+        super()._connect(objects)
+        self.connections = [(i[1], i[0]) for i in self.connections]
+
     def get_children(self, item: type) -> list[type]:
         return item.__subclasses__()
 
 
 class ParentClassConnectionBuilder(BaseClassConnectionBuilder):
     def get_children(self, item: type) -> tuple[type, ...]:
         return item.__bases__
 
 
 class MroConnectionBuilder(BaseClassConnectionBuilder):
     def _connect(self, objects):
         mro = list(objects[0].mro())
         self.item_dict = {self.get_id(kls): self.get_title(kls) for kls in mro}
-        self.connections = itertools.pairwise(mro)
+        self.connections = [
+            (self.get_id(i), self.get_id(j)) for i, j in itertools.pairwise(mro)
+        ]
 
 
-class ClassDiagram(diagram.Diagram):
+class MkClassDiagram(mkdiagram.MkDiagram):
     """Class diagram with several modes."""
 
     def __init__(
         self,
         klass: type,
         mode: DiagramModeStr = "parent_tree",
         **kwargs,
@@ -75,15 +81,15 @@
             klass=self.klass,
             mode=self.mode,
             orientation=self.orientation,
         )
 
     @staticmethod
     def examples():
-        yield dict(klass=ClassDiagram)
+        yield dict(klass=MkClassDiagram)
 
     def _to_markdown(self) -> str:
         match self.mode:
             case "subclass_tree":
                 builder = SubclassConnectionBuilder(self.klass)
                 item_str = builder.get_graph_connection_text()
             case "parent_tree":
@@ -95,9 +101,9 @@
             case _:
                 raise ValueError(self.mode)
         text = f"{self.graph_type} {self.orientation}\n{item_str}"
         return f"```mermaid\n{text}\n```"
 
 
 if __name__ == "__main__":
-    diagram = ClassDiagram(ClassDiagram, mode="mro")
+    diagram = MkClassDiagram(MkClassDiagram, mode="mro")
     print(diagram)
```

### Comparing `mknodes-0.1.0/mknodes/classhelpers.py` & `mknodes-0.2.0/mknodes/classhelpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             return tuple(module.__name__.split("."))
         case pathlib.Path() if not module.is_absolute():
             return module.parts
         case _:
             raise TypeError(module)
 
 
-def iter_classes_for_module(
+def iter_classes(
     module: types.ModuleType | str | tuple[str],
     *,
     type_filter: type | None | types.UnionType = None,
     module_filter: str | None = None,
     filter_by___all__: bool = False,
     recursive: bool = False,
 ) -> Iterator[type]:
@@ -116,15 +116,15 @@
     """
     mod = to_module(module)
     if not mod:
         return []
     if recursive:
         for _name, submod in inspect.getmembers(mod, inspect.ismodule):
             if submod.__name__.startswith(module_filter or ""):
-                yield from iter_classes_for_module(
+                yield from iter_classes(
                     submod,
                     type_filter=type_filter,
                     module_filter=submod.__name__,
                     filter_by___all__=filter_by___all__,
                     recursive=True,
                 )
     for klass_name, kls in inspect.getmembers(mod, inspect.isclass):
@@ -134,35 +134,42 @@
         if type_filter is not None and not issubclass(kls, type_filter):
             continue
         if module_filter is not None and not kls.__module__.startswith(module_filter):
             continue
         yield kls
 
 
-def get_topmost_module_path_for_klass(klass: type) -> str:
+def get_topmost_module_path(obj: type | types.FunctionType | types.MethodType) -> str:
     """Return path of topmost module containing given class.
 
     If a class is imported in any of its parent modules, return that "shorter" path.
 
     So for a class "submodule.classmodule.Class", it could return "submodule.Class"
 
     Arguments:
-        klass: Klass to get the path for.
+        obj: Klass to get the path for.
     """
-    path = klass.__module__
+    path = obj.__module__
+    match obj:
+        case type():
+            fn = inspect.isclass
+        case types.MethodType():
+            fn = inspect.ismethod
+        case types.FunctionType():
+            fn = inspect.isfunction
     parts = path.split(".")
     while parts:
         with contextlib.suppress(TypeError):
             new_path = ".".join(parts)
             mod = importlib.import_module(new_path)
-            klasses = [kls for _kls_name, kls in inspect.getmembers(mod, inspect.isclass)]
-            if klass in klasses:
+            objs = [i for _i_name, i in inspect.getmembers(mod, fn)]
+            if obj in objs:
                 path = new_path
         parts = parts[:-1]
     return path
 
 
 if __name__ == "__main__":
     from prettyqt import widgets
 
-    path = iter_classes_for_module(widgets, recursive=False)
+    path = iter_classes(widgets, recursive=False)
     print(len(list(path)))
```

### Comparing `mknodes-0.1.0/mknodes/classpage.py` & `mknodes-0.2.0/mknodes/mkmodulepage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,68 @@
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
+import types
 
-from typing import Any
-
-from mknodes import (
-    classdiagram,
-    classhelpers,
-    classtable,
-    docstrings,
-    mkpage,
-    utils,
-)
+from mknodes import classhelpers, mkbaseclasstable, mkdocstrings, mkpage, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class ClassPage(mkpage.MkPage):
-    """Page showing information about a class.
+class MkModulePage(mkpage.MkPage):
+    """Page showing information about a module.
 
     Arguments:
-        klass: class to show info for
-        module_path: If given, overrides module returned by class.__module__
-                     This can be useful if you want to link to an aliased class
-                     (for example a class imported to __init__.py)
-        path: some path for the file.
-        kwargs: keyword arguments passed to base class
+        module: ModuleType or path to model to show info for.
+        path: Some path for the file. Default is index.md
+        docstrings: Whether to show docstrings for given module.
+        show_class_table: ModuleType or path to model to show info for.
     """
 
     def __init__(
         self,
-        klass: type,
+        module: tuple[str, ...] | str | types.ModuleType,
         *,
-        module_path: tuple[str, ...] | str | None = None,
-        path: str | os.PathLike = "",
-        **kwargs: Any,
+        path: str | os.PathLike = "index.md",
+        docstrings: bool = False,
+        show_class_table: bool = True,
+        **kwargs,
     ):
-        path = pathlib.Path(f"{klass.__name__}.md")
+        path = pathlib.Path(path)
         super().__init__(path=path, **kwargs)
-        self.klass = klass
-        match module_path:
-            case None:
-                self.parts = klass.__module__.split(".")
-            case _:
-                self.parts = classhelpers.to_module_parts(module_path)
+        self.parts = classhelpers.to_module_parts(module)
+        self.module = classhelpers.to_module(module)
+        self.docstrings = docstrings
+        self.show_class_table = show_class_table
         self._build()
 
     def __repr__(self):
-        return utils.get_repr(self, klass=self.klass, path=str(self.path))
+        return utils.get_repr(self, module=self.module, path=str(self.path))
 
     @staticmethod
     def examples():
-        yield dict(klass=ClassPage)
+        import mknodes
 
-    def add_class_diagram(self, mode: classdiagram.DiagramModeStr = "parent_tree"):
-        diagram = classdiagram.ClassDiagram(self.klass, mode=mode)
-        self.append(diagram)
-        return diagram
+        yield dict(module=mknodes)
 
     def _build(self):
-        module_path = ".".join(self.parts).rstrip(".")
-        path = f"{module_path}.{self.klass.__name__}"
-        item = docstrings.DocStrings(path, header="DocStrings")
-        self.append(item)
-        if tbl := classtable.ClassTable(self.klass):
-            self.append(tbl)
-        item = classdiagram.ClassDiagram(self.klass, header="Inheritance diagram")
-        self.append(item)
+        if doc := self.module.__doc__:
+            self.append(doc)
+        if self.docstrings:
+            item = mkdocstrings.MkDocStrings(f'{".".join(self.parts)}')
+            self.append(item)
+        if self.show_class_table:
+            klasses = list(
+                classhelpers.iter_classes(module=self.parts, module_filter=self.parts[0])
+            )
+            table = mkbaseclasstable.MkBaseClassTable(klasses)
+            self.append(table)
 
 
 if __name__ == "__main__":
-    doc = ClassPage(ClassPage)
+    doc = MkModulePage(mkpage)
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
     # print(doc.children)
```

### Comparing `mknodes-0.1.0/mknodes/classtable.py` & `mknodes-0.2.0/mknodes/mkclasstable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import logging
 
 from typing import Literal
 
-from mknodes import baseclasstable, utils
+from mknodes import mkbaseclasstable, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class ClassTable(baseclasstable.BaseClassTable):
+class MkClassTable(mkbaseclasstable.MkBaseClassTable):
     """Table to show information about a specific class."""
 
     def __init__(
         self,
         klass: type,
         *,
+        layout: Literal["compact", "extended"] = "extended",
+        filter_fn: Callable | None = None,
         mode: Literal["sub_classes", "parent_classes"] = "sub_classes",
         **kwargs,
     ):
         self.mode = mode
         self.klass = klass
         match self.mode:
             case "sub_classes":
@@ -28,27 +31,27 @@
                     klasses = klass.__subclasses__()
                 except TypeError:
                     klasses = []
             case "parent_classes":
                 klasses = list(klass.__bases__)
             case _:
                 raise ValueError(self.mode)
-        super().__init__(klasses=klasses, **kwargs)
+        super().__init__(klasses=klasses, layout=layout, filter_fn=filter_fn, **kwargs)
 
     def __repr__(self):
         return utils.get_repr(
             self,
             klass=self.klass,
             mode=self.mode,
         )
 
     @staticmethod
     def examples():
-        from mknodes import nav
+        from mknodes import mknav
 
-        yield dict(klass=nav.Nav)
-        yield dict(klass=nav.Nav, mode="parent_classes")
+        yield dict(klass=mknav.MkNav)
+        yield dict(klass=mknav.MkNav, mode="parent_classes")
 
 
 if __name__ == "__main__":
-    table = ClassTable(klass=ClassTable, layout="extended")
+    table = MkClassTable(klass=MkClassTable, layout="extended")
     print(table)
```

### Comparing `mknodes-0.1.0/mknodes/code.py` & `mknodes-0.2.0/mknodes/mkcode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import inspect
 import logging
 import textwrap
 import types
 
+from typing import Any
+
 from typing_extensions import Self
 
-from mknodes import markdownnode, utils
+from mknodes import mknode, mktext, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class Code(markdownnode.Text):
+class MkCode(mktext.MkText):
     """Class representing a Code block."""
 
     REQUIRED_EXTENSIONS = [
         "pymdownx.highlight",
         "pymdownx.inlinehilite",
         "pymdownx.snippets",
         "pymdownx.superfences",
     ]
 
     def __init__(
         self,
-        code: str | markdownnode.MkNode = "",
+        code: str | mknode.MkNode = "",
         language: str = "py",
         *,
         title: str = "",
         header: str = "",
         linenums: int | None = None,
         highlight_lines: list[int] | None = None,
         parent=None,
     ):
-        if isinstance(code, Code):
+        if isinstance(code, MkCode):
             code = textwrap.indent(str(code), "    ")
         super().__init__(code, header=header, parent=parent)
         self.language = language
         self.title = title
         self.linenums = linenums
         self.highlight_lines = highlight_lines
 
@@ -56,15 +59,16 @@
         cls,
         obj: types.ModuleType
         | type
         | types.MethodType
         | types.FunctionType
         | types.TracebackType
         | types.FrameType
-        | types.CodeType,
+        | types.CodeType
+        | Callable[..., Any],
         *,
         dedent: bool = True,
         extract_body: bool = False,
         header: str = "",
     ) -> Self:
         if extract_body and isinstance(obj, type | types.FunctionType | types.MethodType):
             code = utils.get_function_body(obj)
@@ -73,9 +77,9 @@
         else:
             code = inspect.getsource(obj)
         code = textwrap.dedent(code) if dedent else code
         return cls(code=code, header=header)
 
 
 if __name__ == "__main__":
-    code = Code.for_object(Code, extract_body=True)
+    code = MkCode.for_object(MkCode, extract_body=True)
     print(code)
```

### Comparing `mknodes-0.1.0/mknodes/connectionbuilder.py` & `mknodes-0.2.0/mknodes/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/mknodes/diagram.py` & `mknodes-0.2.0/mknodes/mkdiagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import textwrap
 
 from typing import Literal
 
-from mknodes import markdownnode, utils
+from mknodes import mknode, utils
 
 
 GraphTypeStr = Literal["flow"]  # TODO
 
 
-class Diagram(markdownnode.MkNode):
+class MkDiagram(mknode.MkNode):
     """Class representing a mermaid diagram. Can show DAGs."""
 
     TYPE_MAP = dict(
         flow="graph",
         sequence="sequenceDiagram",
         state="stateDiagram-v2",
     )
@@ -57,9 +57,9 @@
         items = list(self.items) + [f"{a} --> {b}" for a, b in self.connections]
         item_str = textwrap.indent("\n".join(items), "  ")
         text = f"{self.graph_type} {self.orientation}\n{item_str}"
         return f"```mermaid\n{text}\n```"
 
 
 if __name__ == "__main__":
-    diagram = Diagram(graph_type="flow")
+    diagram = MkDiagram(graph_type="flow")
     print(diagram)
```

### Comparing `mknodes-0.1.0/mknodes/docstrings.py` & `mknodes-0.2.0/mknodes/mkdocstrings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 import importlib
 import logging
 import os
 import types
 
 from typing import Any, Literal
 
-from mknodes import classhelpers, markdownnode, utils
+from mknodes import classhelpers, mktext, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class DocStrings(markdownnode.Text):
+class MkDocStrings(mktext.MkText):
     """Docstring section (powered by mkdocstrings)."""
 
     REQUIRED_PLUGINS = "mkdocstrings"
     OPTIONS_DEFAULT: dict[str, Any] = {}
 
     def __init__(
         self,
-        obj: types.ModuleType | str | os.PathLike | type,
+        obj: types.ModuleType
+        | str
+        | os.PathLike
+        | type
+        | types.FunctionType
+        | types.MethodType,
         for_topmost: bool = False,
         allow_inspection: bool | None = None,
         show_bases: bool | None = None,
         show_source: bool | None = None,
         preload_modules: list[str] | None = None,
         heading_level: int | None = None,
         show_root_heading: bool | None = None,
@@ -113,17 +118,17 @@
             kwargs: Keyword arguments passed to super.
         """
         super().__init__(**kwargs)
         self.obj = obj
         match obj:
             case types.ModuleType():
                 self.obj_path = obj.__name__
-            case type():
+            case type() | types.FunctionType() | types.MethodType():
                 if for_topmost:
-                    topmost_path = classhelpers.get_topmost_module_path_for_klass(obj)
+                    topmost_path = classhelpers.get_topmost_module_path(obj)
                     self.obj_path = f"{topmost_path}.{obj.__qualname__}"
                 else:
                     self.obj_path = f"{obj.__module__}.{obj.__qualname__}"
             case str():
                 self.obj_path = obj  # for setting a manual path
             case tuple() | list():
                 self.obj_path = ".".join(obj)
@@ -171,9 +176,9 @@
         if self.options:
             options = "\n".join(f"      {k}: {v!r}" for k, v in self.options.items())
             md = f"{md}    options:\n{options}\n"
         return md
 
 
 if __name__ == "__main__":
-    docstrings = DocStrings("a.b", show_submodules=True)
+    docstrings = MkDocStrings("a.b", show_submodules=True)
     print(docstrings)
```

### Comparing `mknodes-0.1.0/mknodes/image.py` & `mknodes-0.2.0/mknodes/mkimage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import logging
 import pathlib
 
-from mknodes import markdownnode
+from mknodes import mknode
 
 
 logger = logging.getLogger(__name__)
 
 
-class Image(markdownnode.MkNode):
+class MkImage(mknode.MkNode):
     """Image including optional caption."""
 
     def __init__(
         self,
         path: str,
         *,
         caption: str = "",
@@ -28,7 +28,11 @@
 
     def _to_markdown(self) -> str:
         lines = ["<figure markdown>", f"  ![{self.title}]({self.path})"]
         if self.caption:
             lines.append(f"  <figcaption>{self.caption}</figcaption>")
         lines.append("</figure>")
         return "\n".join(lines) + "\n"
+
+
+if __name__ == "__main__":
+    img = MkImage("Some path")
```

### Comparing `mknodes-0.1.0/mknodes/list.py` & `mknodes-0.2.0/mknodes/mklist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import logging
 
-from mknodes import markdownnode, utils
+from mknodes import mkcontainer, mknode, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class List(markdownnode.MkContainer):
+class MkList(mkcontainer.MkContainer):
     """Class to show a formatted list."""
 
     def __init__(
         self,
-        items: list[str | markdownnode.MkNode] | None = None,
+        items: list[str | mknode.MkNode] | None = None,
         *,
+        ordered: bool = False,
         shorten_after: int | None = None,
         as_links: bool = False,
         header: str = "",
     ):
         # if as_links:
         #     items = [link.Link(i) for i in items]
         super().__init__(items=items, header=header)
+        self.ordered = ordered
         self.shorten_after = shorten_after
         self.as_links = as_links
 
     def __str__(self):
         return self.to_markdown()
 
     def __len__(self):
@@ -43,32 +45,34 @@
     def examples():
         yield dict(items=["Item 1", "Item 2", "Item 2"])
         yield dict(items=["Item"] * 6, shorten_after=3)
 
     def _prep(self, item):
         return utils.linked(item) if self.as_links else str(item)
 
-    def _to_markdown(self):
+    def _to_markdown(self) -> str:
         if not self.items:
             return ""
-        lines = [f"  - {self._prep(i)}" for i in self.items[: self.shorten_after]]
+        prefix = "1." if self.ordered else "*"
+        lines = [f"  {prefix} {self._prep(i)}" for i in self.items[: self.shorten_after]]
         if self.shorten_after and len(self.items) > self.shorten_after:
-            lines.append("  - ...")
+            lines.append(f"  {prefix} ...")
         return "\n".join(lines) + "\n"
 
-    def to_html(self):
+    def to_html(self) -> str:
         """Formats list in html as one single line.
 
         Can be useful for including in Tables.
         """
         if not self.items:
             return ""
+        tag_name = "ol" if self.ordered else "ul"
         items = [f"<li>{self._prep(i)}</li>" for i in self.items[: self.shorten_after]]
         item_str = "".join(items)
         if self.shorten_after and len(self.items) > self.shorten_after:
             item_str += "<li>...</li>"
-        return f"<ul>{item_str}</ul>"
+        return f"<{tag_name}>{item_str}</{tag_name}>"
 
 
 if __name__ == "__main__":
-    section = List(["a", "b"], header="test")
+    section = MkList(["a", "b"], header="test")
     print(section.to_html())
```

### Comparing `mknodes-0.1.0/mknodes/markdownnode.py` & `mknodes-0.2.0/mknodes/mknode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
 import logging
 import textwrap
 
 import mkdocs_gen_files
 
-from mknodes import connectionbuilder, node, utils
+from mknodes import connectionbuilder, node
 
 
 logger = logging.getLogger(__name__)
 
 
 class NodeConnectionBuilder(connectionbuilder.ConnectionBuilder):
     def get_children(self, item):
@@ -20,18 +19,18 @@
         # id() would be enough, but name is sometimes useful for debugging.
         return f"{type(item).__name__}_{id(item)}"
 
     def get_title(self, item) -> str:
         return f"{type(item).__name__}"
 
 
-class MkNode(node.BaseNode):
+class MkNode(node.Node):
     """Base class for everything which can be expressed as Markup.
 
-    The class inherits from BaseNode. The idea is that starting from the
+    The class inherits from Node. The idea is that starting from the
     root nav (aka Docs) down to nested Markup blocks, the whole project can be represented
     by one tree.
 
     Arguments:
         header: Optional header for contained Markup
         indent: Indentation of given Markup (unused ATM)
         parent: Parent for building the tree
@@ -45,33 +44,33 @@
     def __str__(self):
         return self.to_markdown()
 
     # @staticmethod
     # def examples():
     #     yield from ()
 
-    def _to_markdown(self):
+    def _to_markdown(self) -> str:
         return NotImplemented
 
     def to_markdown(self) -> str:
         """Outputs markdown for self and all children."""
         text = self._to_markdown()
         if self.indent:
             text = textwrap.indent(text, self.indent)
         return f"## {self.header}\n\n{text}" if self.header else text
 
     @property
     def resolved_parts(self) -> tuple[str, ...]:
         """Returns a tuple containing all section names."""
-        from mknodes import nav
+        from mknodes import mknav
 
         parent = self
-        parts = [self.section] if isinstance(self, nav.Nav) and self.section else []
+        parts = [self.section] if isinstance(self, mknav.MkNav) and self.section else []
         while parent := parent.parent_item:
-            if isinstance(parent, nav.Nav) and parent.section:
+            if isinstance(parent, mknav.MkNav) and parent.section:
                 parts.append(parent.section)
         return tuple(reversed(parts))
 
     @property
     def resolved_file_path(self) -> str:
         """Returns the resulting section/subsection/../filename.xyz path."""
         filename = str(self.path) if hasattr(self, "path") else ""
@@ -81,37 +80,39 @@
     def virtual_files(self):
         """Returns a dict containing the virtual files attached to this tree element.
 
         This can be overridden by nodes if they want files to be included in the build.
         """
         return {}
 
-    def all_virtual_files(self) -> dict[str, str | bytes]:
+    def all_virtual_files(self, only_children: bool = False) -> dict[str, str | bytes]:
         """Return a dictionary containing all virtual files of itself and all children.
 
         Dict key contains the filename, dict value contains the file content.
 
         The resulting filepath is determined based on the tree hierarchy.
         """
-        from mknodes import nav
+        from mknodes import mknav
 
         dct: dict[str, str | bytes] = {}
         for des in self.descendants:
-            sections = [i.section for i in des.ancestors if isinstance(i, nav.Nav)]
+            sections = [i.section for i in des.ancestors if isinstance(i, mknav.MkNav)]
             section = "/".join(i for i in reversed(sections) if i is not None)
             if section:
                 section += "/"
             files_for_item = {f"{section}{k}": v for k, v in des.virtual_files().items()}
             dct |= files_for_item
-        return dct | self.virtual_files()
+        if not only_children:
+            dct |= self.virtual_files()
+        return dct
 
-    def write(self):
+    def write(self, only_children: bool = False):
         # path = pathlib.Path(self.path)
         # path.parent.mkdir(parents=True, exist_ok=True)
-        for k, v in self.all_virtual_files().items():
+        for k, v in self.all_virtual_files(only_children=only_children).items():
             logger.info(f"Written file to {k}")
             mode = "w" if isinstance(v, str) else "wb"
             with mkdocs_gen_files.open(k, mode) as file:
                 file.write(v)
 
     def pretty_print(self, _indent: int = 0):
         """PrettyPrint node and its children."""
@@ -127,70 +128,9 @@
             orientation: Orientation of resulting graph
         """
         item_str = NodeConnectionBuilder([self]).get_graph_connection_text()
         text = f"graph {orientation}\n{item_str}"
         return f"```mermaid\n{text}\n```"
 
 
-class MkContainer(MkNode):
-    """A base class for Nodes containing other MkNodes."""
-
-    def __init__(self, items: list | None = None, **kwargs):
-        super().__init__(**kwargs)
-        self.items: list[MkNode] = []
-        for item in items or []:
-            self.append(item)  # noqa: PERF402
-
-    def __add__(self, other: str | MkNode):
-        self.append(other)
-        return self
-
-    def __iter__(self) -> Iterator[MkNode]:  # type: ignore
-        return iter(self.items)
-
-    def __repr__(self):
-        return utils.get_repr(self, items=self.items)
-
-    @staticmethod
-    def examples():
-        from mknodes import code
-
-        yield dict(items=[code.Code(code="a = 1 + 2"), Text("abc")])
-
-    def _to_markdown(self) -> str:
-        return "\n\n".join(i.to_markdown() for i in self.items)
-
-    def append(self, other: str | MkNode):
-        other = Text(other, parent=self) if isinstance(other, str) else other
-        self.items.append(other)
-
-    @property  # type: ignore
-    def children(self) -> list[MkNode]:
-        return self.items
-
-    @children.setter
-    def children(self, children: list[MkNode]):
-        self.items = children
-
-
-class Text(MkNode):
-    """Class for any Markup text.
-
-    All classes inheriting from MkNode can get converted to this Type.
-    """
-
-    def __init__(self, text: str | MkNode = "", header: str = "", parent=None):
-        super().__init__(header=header, parent=parent)
-        self.text = text
-
-    def __repr__(self):
-        return utils.get_repr(self, text=self.text)
-
-    def _to_markdown(self) -> str:
-        return self.text if isinstance(self.text, str) else self.text.to_markdown()
-
-
 if __name__ == "__main__":
     section = MkNode(header="fff")
-    for example in MkContainer.examples():
-        container = MkContainer(**example)
-        print(container)
```

### Comparing `mknodes-0.1.0/mknodes/mermaid.py` & `mknodes-0.2.0/mknodes/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/mknodes/mkpage.py` & `mknodes-0.2.0/mknodes/mkpage.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,45 +4,46 @@
 import logging
 import os
 import types
 
 from typing import Any, Literal
 
 from mknodes import (
-    admonition,
-    code as codeblock,
-    docstrings,
-    link,
-    markdownnode,
-    nav,
-    tabs,
+    mkadmonition,
+    mkcode,
+    mkcontainer,
+    mkdocstrings,
+    mklink,
+    mknav,
+    mknode,
+    mktabs,
     utils,
 )
 
 
 logger = logging.getLogger(__name__)
 
 HEADER = "---\n{options}\n---\n\n"
 
 
-class MkPage(markdownnode.MkContainer):
+class MkPage(mkcontainer.MkContainer):
     """A node container representing a Markdown page.
 
     A page contains a list of other Markdown nodes, has a virtual Markdown file
     associated, and can have metadata (added as header)
     """
 
     def __init__(
         self,
         path: str | os.PathLike = "",
         *,
         hide_toc: bool = False,
         hide_nav: bool = False,
         hide_path: bool = False,
-        parent: nav.Nav | None = None,
+        parent: mknav.MkNav | None = None,
         **kwargs: Any,
     ):
         super().__init__(parent=parent, **kwargs)
         self.path = path
         self.header_options: dict[str, Any] = {}
         if hide_toc:
             self.header_options.setdefault("hide", []).append("toc")
@@ -84,22 +85,22 @@
         """
         self.append("<br>" * num)
 
     def add_link(
         self,
         url: str,
         title: str = "",
-    ) -> link.Link:
+    ) -> mklink.MkLink:
         """Add a Link to the page.
 
         Arguments:
             url: URL to link to.
             title: Text to display for the link
         """
-        item = link.Link(url)
+        item = mklink.MkLink(url)
         self.append(item)
         return item
 
     def add_header(self, text: str, level: int = 2):
         """Add line separators to the page.
 
         Arguments:
@@ -108,30 +109,30 @@
         """
         prefix = "#" * level
         self.append(f"{prefix} {text}")
 
     def add_admonition(
         self,
         text: str,
-        typ: admonition.AdmonitionTypeStr = "info",
+        typ: mkadmonition.AdmonitionTypeStr = "info",
         *,
         title: str | None = None,
         collapsible: bool = False,
-    ) -> admonition.Admonition:
+    ) -> mkadmonition.MkAdmonition:
         """Add a Admonition info box to the page.
 
         Arguments:
             text: Text to display inside the box
             typ: the admonition type
             title: The title of the box
             collapsible: whether the box should be collapsible by the user.
         """
-        item = admonition.Admonition(
-            typ=typ,
+        item = mkadmonition.MkAdmonition(
             text=text,
+            typ=typ,
             title=title,
             collapsible=collapsible,
         )
         self.append(item)
         return item
 
     def add_mkdocstrings(
@@ -163,15 +164,15 @@
         show_if_no_docstring: bool | None = None,
         annotations_path: Literal["brief", "source"] | None = None,
         line_length: int | None = None,
         show_signature: bool | None = None,
         show_signature_annotations: bool | None = None,
         signature_crossrefs: bool | None = None,
         separate_signature: bool | None = None,
-    ) -> docstrings.DocStrings:
+    ) -> mkdocstrings.MkDocStrings:
         """Add a DocStrings section to the page.
 
         Arguments:
             obj: What to show Docstrings for
             header: Section header
             for_topmost: whether to try to find the most topmost module path for given
                          object
@@ -219,15 +220,15 @@
                                         and functions signatures.
             signature_crossrefs: Whether to render cross-references for type
                                  annotations in signatures.
             separate_signature: Whether to put the whole signature in a code
                                 block below the heading. If Black is installed,
                                 the signature is also formatted using it.
         """
-        item = docstrings.DocStrings(
+        item = mkdocstrings.MkDocStrings(
             obj=obj,
             header=header,
             for_topmost=for_topmost,
             allow_inspection=allow_inspection,
             show_bases=show_bases,
             show_source=show_source,
             preload_modules=preload_modules,
@@ -256,61 +257,61 @@
             separate_signature=separate_signature,
         )
         self.append(item)
         return item
 
     def add_code(
         self,
-        code: str | markdownnode.MkNode,
+        code: str | mknode.MkNode,
         language: str = "py",
         *,
         title: str = "",
         header: str = "",
         linenums: int | None = None,
         highlight_lines: list[int] | None = None,
-    ):
+    ) -> mkcode.MkCode:
         """Add code block to the page.
 
         Arguments:
             code: Code
             language: language for syntax highlighting
             title: Optional title for the code block
             header: Optional header for the code block
             linenums: Optional start line number for the code block
             highlight_lines: Optional highlighting of a line range.
         """
-        item = codeblock.Code(
+        item = mkcode.MkCode(
             code=code,
             language=language,
             title=title,
             header=header,
             linenums=linenums,
             highlight_lines=highlight_lines,
             parent=self,
         )
         self.append(item)
         return item
 
     def add_tabs(
         self,
-        data: Mapping[str, str | markdownnode.MkNode],
+        data: Mapping[str, str | mknode.MkNode],
         style: Literal["tabbed", "tabblock"] = "tabbed",
         **kwargs: Any,
     ):
         """Add tabs to the page.
 
         Arguments:
             data: tab data
             style: Whether to use new-style (tabblock) or old-style (tabbed) tabs.
             kwargs: Keyword arguments passed to Tabs
         """
         if style == "tabbed":
-            tabblock = tabs.Tabbed(data, parent=self, **kwargs)
+            tabblock = mktabs.MkTabbed(data, parent=self, **kwargs)
         else:
-            tabblock = tabs.TabBlock(data, parent=self, **kwargs)
+            tabblock = mktabs.MkTabBlock(data, parent=self, **kwargs)
         self.append(tabblock)
         return tabblock
 
 
 if __name__ == "__main__":
     doc = MkPage()
     doc.add_link("test")
```

### Comparing `mknodes-0.1.0/mknodes/moduledocumentation.py` & `mknodes-0.2.0/mknodes/mkdoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from __future__ import annotations
 
-from collections.abc import Callable, Iterator
+from collections.abc import Callable, Iterator, Sequence
 
 # import contextlib
 # import importlib
 import inspect
 import logging
 import pathlib
 import types
 
 from typing import Any
 
-from mknodes import classhelpers, classpage, modulepage, nav, utils
+from mknodes import classhelpers, mkclasspage, mkmodulepage, mknav, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class ModuleDocumentation(nav.Nav):
+class MkDoc(mknav.MkNav):
     """Nav for showing a module documenation.
 
     Arguments:
         module: Module to document
         filter_by___all__: Whether to filter stuff according to "__all__"
         exclude_modules: List of modules to exclude
         section_name: Optional section name override
     """
 
     def __init__(
         self,
-        module: types.ModuleType | str,
+        module: types.ModuleType | Sequence[str] | str,
         *,
         filter_by___all__: bool = False,
         exclude_modules: list[str] | None = None,
         section_name: str | None = None,
+        class_page=mkclasspage.MkClassPage,
         **kwargs,
     ):
         self.module = classhelpers.to_module(module)
+        self.ClassPage = class_page
         if self.module is None:
             raise RuntimeError(f"Couldnt load module {module!r}")
         self.is_package = hasattr(self.module, "__path__")
         self.filter_by___all__ = filter_by___all__
         self.module_name = self.module.__name__.split(".")[-1]
         self.module_path = self.module.__name__
         self.file_path = self.module.__file__
@@ -133,15 +135,14 @@
             return
         for submod_name, submod in inspect.getmembers(mod, inspect.ismodule):
             not_in_all = hasattr(mod, "__all__") and submod_name not in mod.__all__
             filtered_by_all = self.filter_by___all__ and not_in_all
             not_filtered_by_pred = predicate(submod) if predicate else True
             # if self.module_name in mod.__name__.split(".")
             if not filtered_by_all and not_filtered_by_pred:
-                print(submod_name, flush=True)
                 yield submod
             if recursive and submod not in seen:
                 seen.add(submod)
                 yield from self.iter_modules(
                     submodule=submod,
                     recursive=True,
                     predicate=predicate,
@@ -151,30 +152,30 @@
     def add_class_page(
         self,
         klass: type,
         *,
         find_topmost: bool = True,
         flatten: bool = False,
         **kwargs: Any,
-    ) -> classpage.ClassPage:
+    ) -> mkclasspage.MkClassPage:
         """Add a page showing information about a class.
 
         Arguments:
             klass: klass to build a page for
             find_topmost: Whether to use a module path from a parent package if available
             flatten: Put page into top level nav if nested.
             kwargs: keyword arguments passed to CLassPage
         """
         if find_topmost:
-            parts = classhelpers.get_topmost_module_path_for_klass(klass).split(".")
+            parts = classhelpers.get_topmost_module_path(klass).split(".")
         else:
             parts = klass.__module__.split(".")
         # parts = klass.__module__.split(".")
         path = pathlib.Path(f"{klass.__name__}.md")
-        page = classpage.ClassPage(
+        page = self.ClassPage(
             klass=klass,
             module_path=tuple(parts),
             path=path,
             parent=self,
             **kwargs,
         )
         section = (klass.__name__,) if flatten else (*parts[1:], klass.__name__)
@@ -190,25 +191,25 @@
     #     page += mknodes.ModuleTable(self.module_name, predicate=predicate)
     #     return page
 
     def add_module_overview(
         self,
         title: str | None = None,
         **kwargs: Any,
-    ) -> modulepage.ModulePage:
+    ) -> mkmodulepage.MkModulePage:
         """Add a page showing all submodules.
 
         Arguments:
             title: Override title for the section.
-            kwargs: kwargs passed to ModulePage.
+            kwargs: kwargs passed to MkModulePage.
         """
         # TODO: slugify?
         path = pathlib.Path("index.md" if title is None else f"{title}.md")
         # parts = path.parts[:-1]
-        page = modulepage.ModulePage(
+        page = mkmodulepage.MkModulePage(
             hide_toc=True,
             module=self.module,  # type: ignore
             path=path,
             parent=self,
             **kwargs,
         )
         self.nav[title or self.module_name] = page
@@ -247,10 +248,10 @@
     #         for klass in self.iter_classes(module, recursive=recursive):
     #             if (klass, path) not in seen or not avoid_duplicates:
     #                 seen.add((klass, path))
     #                 yield klass, path
 
 
 if __name__ == "__main__":
-    doc = ModuleDocumentation(module="mkdocs")
-    page = doc.add_class_page(ModuleDocumentation)
+    doc = MkDoc(module="mkdocs")
+    page = doc.add_class_page(MkDoc)
     print(page)
```

### Comparing `mknodes-0.1.0/mknodes/moduletable.py` & `mknodes-0.2.0/mknodes/mkmoduletable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 import inspect
 import logging
 import types
 
-from mknodes import classhelpers, table, utils
+from mknodes import classhelpers, mktable, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class ModuleTable(table.Table):
+class MkModuleTable(mktable.MkTable):
     """Class representing a formatted table containing information a module."""
 
     def __init__(
         self,
         module: types.ModuleType | str | tuple[str, ...],
         *,
         predicate: Callable | None = None,
@@ -29,18 +29,16 @@
         ]
         super().__init__(dicts, **kwargs)
 
     def get_row_for_module(self, module: types.ModuleType) -> dict[str, str]:
         return dict(
             Name=module.__name__,
             # utils.link_for_class(submod, size=4, bold=True),
-            Information=(
-                module.__doc__.split("\n")[0]
-                if module.__doc__
-                else "*No docstrings defined.*"
+            Information=utils.get_first_doc_line(
+                module, fallback="*No docstrings defined.*"
             ),
             Members=(
                 utils.to_html_list(module.__all__, make_link=True)
                 if hasattr(module, "__all__")
                 else ""
             ),
         )
@@ -52,9 +50,9 @@
     def examples():
         import mknodes
 
         yield dict(module=mknodes)
 
 
 if __name__ == "__main__":
-    table = ModuleTable(module=utils)
+    table = MkModuleTable(module=utils)
     print(table)
```

### Comparing `mknodes-0.1.0/mknodes/node.py` & `mknodes-0.2.0/mknodes/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from mknodes import utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class BaseNode:
+class Node:
     """A Node class that can be used to build trees."""
 
     # __slots__ = ("parent_item", "children")
 
     def __init__(self, parent: Self | None = None):
         self.parent_item = parent
         self.children: list[Self] = []
@@ -164,19 +164,19 @@
             return
         yield indent, self
         for child_item in self.children:
             yield from child_item.iter_nodes(indent + 1)
 
 
 def preorder_iter(
-    tree: BaseNode,
-    filter_condition: Callable[[BaseNode], bool] | None = None,
-    stop_condition: Callable[[BaseNode], bool] | None = None,
+    tree: Node,
+    filter_condition: Callable[[Node], bool] | None = None,
+    stop_condition: Callable[[Node], bool] | None = None,
     max_depth: int = 0,
-) -> Iterable[BaseNode]:
+) -> Iterable[Node]:
     """Iterate through all children of a tree.
 
     Pre-Order Iteration Algorithm, NLR
         1. Visit the current node.
         2. Recursively traverse the current node's left subtree.
         3. Recursively traverse the current node's right subtree.
 
@@ -224,12 +224,12 @@
         if not filter_condition or filter_condition(tree):
             yield tree
         for child in tree.children:
             yield from preorder_iter(child, filter_condition, stop_condition, max_depth)
 
 
 if __name__ == "__main__":
-    node = BaseNode()
-    sub = BaseNode(parent=node)
-    subsub = BaseNode(parent=sub)
+    node = Node()
+    sub = Node(parent=node)
+    subsub = Node(parent=sub)
     node.children = [sub, subsub]
     node.pprint()
```

### Comparing `mknodes-0.1.0/mknodes/noderesolver.py` & `mknodes-0.2.0/mknodes/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/mknodes/snippet.py` & `mknodes-0.2.0/mknodes/mksnippet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import logging
 import os
 
-from mknodes import markdownnode, utils
+from mknodes import mknode, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class Snippet(markdownnode.MkNode):
+class MkSnippet(mknode.MkNode):
     """Snippet to include markdown from another file.
 
     [More info](https://facelessuser.github.io/pymdown-extensions/extensions/snippets/)
     """
 
     REQUIRED_EXTENSIONS = "pymdownx.snippets"
 
@@ -23,14 +23,14 @@
 
     def __str__(self):
         return self.to_markdown()
 
     def __repr__(self):
         return utils.get_repr(self, path=str(self.path))
 
-    def _to_markdown(self):
+    def _to_markdown(self) -> str:
         return f"--8<--\n{self.path}\n--8<--\n"
 
 
 if __name__ == "__main__":
-    section = Snippet("test.md", header="test")
+    section = MkSnippet("test.md", header="test")
     print(section.to_markdown())
```

### Comparing `mknodes-0.1.0/mknodes/sourceandresult.py` & `mknodes-0.2.0/mknodes/mksourceandresult.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 import logging
 
-from mknodes import code, markdownnode, utils
+from mknodes import mkcode, mknode, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class SourceAndResult(markdownnode.MkNode):
+class MkSourceAndResult(mknode.MkNode):
     """Class to show the source of a Callable combined with its stringified result."""
 
-    def __init__(self, fn: Callable, header: str = ""):
+    def __init__(
+        self,
+        fn: Callable,
+        header: str = "",
+    ):
         super().__init__(header)
         self.fn = fn
 
     @staticmethod
     def examples():
         def test():
-            return code.Code(code="a = 2 + 4")
+            return mkcode.MkCode(code="a = 2 + 4")
 
         yield dict(fn=test)
 
     def __str__(self):
         return self.to_markdown()
 
     def __repr__(self):
         return utils.get_repr(self, fn=self.fn)
 
-    def _to_markdown(self):
-        code_block = code.Code.for_object(self.fn, extract_body=True)
+    def _to_markdown(self) -> str:
+        code_block = mkcode.MkCode.for_object(self.fn, extract_body=True)
         markdown = str(self.fn())
         return f"{code_block}\nresults in:\n\n{markdown}"
 
 
 if __name__ == "__main__":
-    test = code.Code(language="test")
-    section = SourceAndResult(test.to_markdown, header="test")
+    test = mkcode.MkCode(language="test")
+    section = MkSourceAndResult(test.to_markdown, header="test")
     print(section.to_markdown())
```

### Comparing `mknodes-0.1.0/mknodes/table.py` & `mknodes-0.2.0/mknodes/mktable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Mapping, Sequence
 import logging
 
-from mknodes import markdownnode
+from mknodes import mknode
 
 
 logger = logging.getLogger(__name__)
 
 
-class Table(markdownnode.MkNode):
+class MkTable(mknode.MkNode):
     """Class representing a formatted table."""
 
     REQUIRED_EXTENSIONS = "tables"
 
     def __init__(
         self,
         data: Sequence[Sequence[str]] | Sequence[dict] | dict[str, list] | None = None,
         columns: Sequence[str] | None = None,
         *,
         column_modifiers: dict[str, Callable[[str], str]] | None = None,
         header: str = "",
+        **kwargs,
     ):
-        super().__init__(header=header)
+        super().__init__(header=header, **kwargs)
         column_modifiers = column_modifiers or {}
         match data:
             case None:
                 self.data = {}
             case Mapping():
                 self.data = {str(k): [str(i) for i in v] for k, v in data.items()}
             case ((str(), *_), *_):
@@ -83,9 +84,9 @@
     @classmethod
     def for_items(cls, items, columns: dict[str, Callable]):
         ls = [{k: v(item) for k, v in columns.items()} for item in items]
         return cls(ls)
 
 
 if __name__ == "__main__":
-    table = Table(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
+    table = MkTable(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
     print(table)
```

### Comparing `mknodes-0.1.0/mknodes/tabs.py` & `mknodes-0.2.0/mknodes/mktabs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 import logging
 import textwrap
 
-from mknodes import markdownnode, utils
+from mknodes import mkcontainer, mknode, mktext, utils
 
 
 logger = logging.getLogger(__name__)
 
 
-class Tab(markdownnode.MkContainer):
+class MkTab(mkcontainer.MkContainer):
     def __init__(
         self,
         title: str,
         items: list | None = None,
         *,
         select: bool = False,
         attrs: dict | None = None,
@@ -26,28 +26,28 @@
         self.attrs = attrs
 
     @staticmethod
     def examples():
         yield from ()
 
 
-class BaseTabWidget(markdownnode.MkContainer):
+class MkBaseTabWidget(mkcontainer.MkContainer):
     def __init__(
         self,
-        tabs: Mapping[str, str | markdownnode.MkNode] | list[Tab],
+        tabs: Mapping[str, str | mknode.MkNode] | list[MkTab],
         header: str = "",
         **kwargs,
     ):
         if isinstance(tabs, list):
             items = tabs
         else:
             items = [
-                Tab(
+                MkTab(
                     k,
-                    items=[markdownnode.Text(v) if isinstance(v, str) else v],
+                    items=[mktext.MkText(v) if isinstance(v, str) else v],
                 )
                 for k, v in tabs.items()
             ]
         for tab in items:
             tab.parent_item = self
         super().__init__(items=items, header=header)
 
@@ -58,37 +58,37 @@
         return {tab.title: str(tab) for tab in self.items}
 
     @staticmethod
     def examples():
         yield dict(tabs={"Tab 1": "Some markdown", "Tab 2": "Other Markdown"})
 
 
-class Tabbed(BaseTabWidget):
+class MkTabbed(MkBaseTabWidget):
     """pymdownx-based Tab block."""
 
     REQUIRED_EXTENSIONS = "pymdownx.tabbed"
 
     def _to_markdown(self) -> str:
         lines: list[str] = []
         for tab in self.items:
             indented_text = textwrap.indent(str(tab).rstrip("\n"), prefix="    ")
             lines.extend((f'=== "{tab.title}"', indented_text))
         return "\n".join(lines) + "\n"
 
 
-class TabBlock(BaseTabWidget):
+class MkTabBlock(MkBaseTabWidget):
     """pymdownx-based Tab block."""
 
     REQUIRED_EXTENSIONS = "pymdownx.blocks.tab"
 
     def _to_markdown(self) -> str:
         lines: list[str] = []
         for tab in self.items:
             # TODO: perhaps always add "new: true" to first tab?
             lines.extend((f"/// tab | {tab.title}", str(tab).rstrip("\n"), "///\n"))
         return "\n".join(lines) + "\n"
 
 
 if __name__ == "__main__":
     tabs = dict(Tab1="Some text", Tab2="Another text")
-    tabblock = Tabbed(tabs)
+    tabblock = MkTabbed(tabs)
     print(tabblock)
```

### Comparing `mknodes-0.1.0/mknodes/utils.py` & `mknodes-0.2.0/mknodes/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,20 @@
 def slugify(text: str) -> str:
     text = text.lower()
     text = re.sub("[^0-9a-zA-Z_.]", "_", text)
     text = re.sub("^[^a-zA-Z_#]+", "", text)
     return text
 
 
-def groupby(data, keyfunc: Callable | None = None):
+def groupby(data, keyfunc: Callable | None = None) -> dict[str, list]:
     data = sorted(data, key=keyfunc or (lambda x: x))
     return {k: list(g) for k, g in itertools.groupby(data, keyfunc)}
 
 
-def groupby_first_letter(data, keyfunc: Callable | None = None):
+def groupby_first_letter(data, keyfunc: Callable | None = None) -> dict[str, list]:
     data = sorted(data, key=keyfunc or (lambda x: x))
 
     def first_letter(x):
         return keyfunc(x)[0] if keyfunc else x[0]
 
     return {k: list(g) for k, g in itertools.groupby(data, first_letter)}
 
@@ -160,15 +160,15 @@
         parts = klass.__module__.split(".")
         return f"{parts[1]}.{klass.__name__}"
     return f"{klass.__module__.split('.')[-1]}.{klass.__name__}"
 
 
 def to_html_list(
     ls: list[str], shorten_after: int | None = None, make_link: bool = False
-):
+) -> str:
     if not ls:
         return ""
     item_str = "".join(
         f"<li>{linked(i)}</li>" if make_link else f"<li>{i}</li>"
         for i in ls[:shorten_after]
     )
     if shorten_after and len(ls) > shorten_after:
@@ -200,10 +200,21 @@
         for line in source_lines:
             line = line.strip()
             if line.endswith(":"):
                 break
     return "".join(source_lines)
 
 
+def get_deprecated_message(obj) -> str | None:
+    return obj.__deprecated__ if hasattr(obj, "__deprecated__") else None
+
+
+def get_first_doc_line(obj, escape: bool = False, fallback: str = "") -> str:
+    doc = obj.__doc__.split("\n")[0] if isinstance(obj.__doc__, str) else fallback
+    if escape:
+        doc = escaped(doc)
+    return doc
+
+
 if __name__ == "__main__":
     strings = groupby_first_letter([str(i) for i in range(1000)])
     print(limit_repr.repr(strings))
```

### Comparing `mknodes-0.1.0/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.2.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from __future__ import annotations
-
-import collections
-import logging
-import os
-import pathlib
-import re
-import urllib.parse
-
-from mkdocs.plugins import BasePlugin
-import mkdocs.utils
-
-
-logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
-logger.addFilter(mkdocs.utils.warning_filter)
-
-# For Regex, match groups are:
-#       0: Whole markdown link e.g. [Alt-text](url)
-#       1: Alt text
-#       2: Full URL e.g. url + hash anchor
-#       3: Filename e.g. filename.md
-#       4: File extension e.g. .md, .png, etc.
-#       5. hash anchor e.g. #my-sub-heading-link
-AUTOLINK_RE = r"\[([^\]]+)\]\((([^)/]+\.(md|png|jpg))(#.*)*)\)"
-
-
-class AutoLinkReplacerPlugin:
-    def __init__(self, base_docs_url, page_url, mapping):
-        self.mapping = mapping
-        self.page_url = page_url
-        self.base_docs_url = pathlib.Path(base_docs_url)
-        # Absolute URL of the linker
-        self.linker_url = os.path.dirname(self.base_docs_url / page_url)  # noqa: PTH120
-
-    def __call__(self, match):
-        # Name of the markdown file
-        filename = urllib.parse.unquote(match.group(3).strip())
-        if filename not in self.mapping:
-            return f"`{match.group(3).replace('.md', '')}`"
-        filenames = self.mapping[filename]
-        if len(filenames) > 1:
-            logger.warning(
-                f"{self.page_url}: {match.group(3)} has multiple targets: {filenames}"
-            )
-        abs_link_url = (self.base_docs_url / self.mapping[filename][0]).parent
-        # need os.replath here bc pathlib.relative_to throws an exception
-        # when linking across drives
-        rel_path = os.path.relpath(abs_link_url, self.linker_url)
-        # html_filename = filename.replace(".md", ".html")
-        rel_link_url = os.path.join(rel_path, filename)  # noqa: PTH118
-        new_text = (
-            match.group(0).replace(match.group(2), rel_link_url)
-            if match.group(5) is None
-            else match.group(0).replace(match.group(2), rel_link_url + match.group(5))
-        )
-        new_text = new_text.replace("\\", "/")
-        logger.debug(
-            f"LinkReplacer: {self.page_url}: {match.group(3)=} -> {rel_link_url=}"
-        )
-        return new_text
-
-
-class LinkReplacerPlugin(BasePlugin):
-    def on_page_markdown(self, markdown, page, config, files, **kwargs):
-        base_docs_url = config["docs_dir"]
-        page_url = page.file.src_path
-        mapping = collections.defaultdict(list)
-        for file_ in files:
-            filename = os.path.basename(file_.abs_src_path)  # noqa: PTH119
-            mapping[filename].append(file_.url)
-        plugin = AutoLinkReplacerPlugin(base_docs_url, page_url, mapping)
-        markdown = re.sub(AUTOLINK_RE, plugin, markdown)
-        return markdown
+from __future__ import annotations
+
+import collections
+import logging
+import os
+import pathlib
+import re
+import urllib.parse
+
+from mkdocs.plugins import BasePlugin
+import mkdocs.utils
+
+
+logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
+logger.addFilter(mkdocs.utils.warning_filter)
+
+# For Regex, match groups are:
+#       0: Whole markdown link e.g. [Alt-text](url)
+#       1: Alt text
+#       2: Full URL e.g. url + hash anchor
+#       3: Filename e.g. filename.md
+#       4: File extension e.g. .md, .png, etc.
+#       5. hash anchor e.g. #my-sub-heading-link
+AUTOLINK_RE = r"\[([^\]]+)\]\((([^)/]+\.(md|png|jpg))(#.*)*)\)"
+
+
+class AutoLinkReplacerPlugin:
+    def __init__(self, base_docs_url, page_url, mapping):
+        self.mapping = mapping
+        self.page_url = page_url
+        self.base_docs_url = pathlib.Path(base_docs_url)
+        # Absolute URL of the linker
+        self.linker_url = os.path.dirname(self.base_docs_url / page_url)  # noqa: PTH120
+
+    def __call__(self, match):
+        # Name of the markdown file
+        filename = urllib.parse.unquote(match.group(3).strip())
+        if filename not in self.mapping:
+            return f"`{match.group(3).replace('.md', '')}`"
+        filenames = self.mapping[filename]
+        # if len(filenames) > 1:
+        #     logger.warning(
+        #         f"{self.page_url}: {match.group(3)} has multiple targets: {filenames}"
+        #     )
+        abs_link_url = (self.base_docs_url / filenames[0]).parent
+        # need os.replath here bc pathlib.relative_to throws an exception
+        # when linking across drives
+        rel_path = os.path.relpath(abs_link_url, self.linker_url)
+        # html_filename = filename.replace(".md", ".html")
+        rel_link_url = os.path.join(rel_path, filename)  # noqa: PTH118
+        new_text = (
+            match.group(0).replace(match.group(2), rel_link_url)
+            if match.group(5) is None
+            else match.group(0).replace(match.group(2), rel_link_url + match.group(5))
+        )
+        new_text = new_text.replace("\\", "/")
+        logger.debug(
+            f"LinkReplacer: {self.page_url}: {match.group(3)=} -> {rel_link_url=}"
+        )
+        return new_text
+
+
+class LinkReplacerPlugin(BasePlugin):
+    def on_page_markdown(self, markdown, page, config, files, **kwargs):
+        base_docs_url = config["docs_dir"]
+        page_url = page.file.src_path
+        mapping = collections.defaultdict(list)
+        for file_ in files:
+            filename = os.path.basename(file_.abs_src_path)  # noqa: PTH119
+            mapping[filename].append(file_.url)
+        plugin = AutoLinkReplacerPlugin(base_docs_url, page_url, mapping)
+        markdown = re.sub(AUTOLINK_RE, plugin, markdown)
+        return markdown
```

### Comparing `mknodes-0.1.0/mknodes/manual/page_1.py` & `mknodes-0.2.0/mknodes/manual/page_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,46 +11,48 @@
 Basically everything interesting in this library inherits from MkNode.
 It`s the base class for all tree nodes we are building. The tree goes from the root nav
 down to single markup elements. We can show the subclass tree by using
 the MkClassDiagram Node.
 """
 
 
-def create_page_1(root_nav: mknodes.Nav):
+def create_page_1(root_nav: mknodes.MkNav):
+    # Basic structure: Theres one root nav, navs can contain pages and other navs,
+    # pages contain more atomic markup nodes, like text, tables, and diagrams.
+    # These markup nodes in some cases can contain other Markup nodes.
+    # It`s all one big tree.
+
     home_nav = root_nav.add_nav("User guide")
-    overview = home_nav.add_page("Overview")
+    overview = home_nav.add_page("Overview", hide_toc=True)
 
-    # we are here right now.
+    # this here is what you are reading right now.
     overview.add_code(inspect.getsource(create_page_1))
     nodes_nav = home_nav.add_nav("Nodes")
 
-    # for convenience, we can add strs directly to pages.
+    # for convenience, we can add strings directly to pages.
     # they will get converted to a mknodes.Text node.
     overview += INTRO_TEXT
 
-    # Basic structure: Theres one root nav, navs can contain pages and other navs,
-    # pages contain more atomic markup nodes, like text, tables, and diagrams.
-    # These markup nodes in some cases can contain other Markup nodes.
-    # It`s all one big tree.
-
+    # Lets take a look at the relations of the included nodes.
+    # It`s easy to show different diagrams for classes.
     subcls_page = home_nav.add_page("Subclass tree", hide_toc=True)
-    subcls_page += mknodes.ClassDiagram(
-        mknodes.MkNode, mode="subclass_tree", orientation="RL"
+    subcls_page += mknodes.MkClassDiagram(
+        mknodes.MkNode, mode="subclass_tree", orientation="LR"
     )
     # let`s take a look at some of the mentioned Markup nodes.
     # Some of them have a `examples` classmethod which yields some example signatures
     #  to show the functionality.
     for kls in classhelpers.get_subclasses(mknodes.MkNode):
         # get_subclasses just calls __subclasses__ recursively.
         subpage = nodes_nav.add_page(kls.__name__)
         if hasattr(kls, "examples"):
-            subpage += mknodes.Code.for_object(kls.examples, header="Our combinations")
+            subpage += mknodes.MkCode.for_object(kls.examples, header="Signatures:")
             for i, sig in enumerate(kls.examples(), start=1):
-                subpage.add_header(f"Example {i} for class {kls.__name__!r}", level=2)
+                subpage.add_header(f"Trying signature {i}", level=2)
                 sig_txt = utils.format_kwargs(sig)
                 text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
                 subpage.add_code(code=text, title=f"example_{i}.py")
                 node = kls(**sig)
-                code = mknodes.Code(language="md", code=node, title=f"result_{i}.md")
+                code = mknodes.MkCode(language="md", code=node, title=f"result_{i}.md")
                 subpage.add_tabs({"Preview": str(node), "Generated markdown": str(code)})
                 subpage.add_newlines(3)
         subpage.add_mkdocstrings(kls)
```

### Comparing `mknodes-0.1.0/mknodes/manual/page_2.py` & `mknodes-0.2.0/mknodes/manual/page_2.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 
 
 INTRO_TEXT = """now lets create the documentation.
 This code will show how to build a simple documentation section.
 """
 
 
-def create_page_2(root_nav: mknodes.Nav):
+def create_page_2(root_nav: mknodes.MkNav):
     doc_section = root_nav.add_nav("Documentation")
 
-    overview = doc_section.add_page("Overview")
-    overview += mknodes.Text(INTRO_TEXT)
+    overview = doc_section.add_page("Overview", hide_toc=True)
+    overview += mknodes.MkText(INTRO_TEXT)
 
     # we are here right now.
     overview.add_code(inspect.getsource(create_page_2))
 
     # lets create the complete documentation for our module.
-    # we start by adding a nice overview page.
-    mknodes_docs = doc_section.add_documentation(module=mknodes)
+    # Each Documentation section can have global filters for what it should include.
+    # In this case, we only want to document stuff which is listed in "__all__".
+    mknodes_docs = doc_section.add_documentation(module=mknodes, filter_by___all__=True)
+    # we start by adding a nice overview page. This might gain some kwargs for different
+    # styles in the future.
     mknodes_docs.add_module_overview()
 
-    # now we add some pre-defined pages ("ClassPages") to our docs.
-    # they contain MkDocStrings, a table for eventual subclasses and an inheritance graph.
-    # It`s also possible to build custom pages of course.
+    # the Documentation Nav hast some helper methods to iterate through the submodules
+    # / classes of a module. We can also pass a predicate to filter specific subclasses,
+    # or do other fancy stuff to generate a customized, automated documentation.
     for klass in mknodes_docs.iter_classes(recursive=True):
+        # now we add some pre-defined pages ("MkClassPages") to our docs.
+        # they contain MkDocStrings, a table for eventual subclasses and an
+        # inheritance graph. It`s also possible to build custom pages of course.
         mknodes_docs.add_class_page(klass=klass)
 
     # Not enough documentation for your taste? Let`s document random stuff.
     # What about the std library?
     std_lib_nav = doc_section.add_nav("std_library")
     for stdlib_mod in ["pathlib", "inspect", "logging"]:
         docs = std_lib_nav.add_documentation(module=stdlib_mod)
         docs.add_module_overview()
         for klass in docs.iter_classes(recursive=True):
             docs.add_class_page(klass=klass)
 
-    overview.add_admonition(text="That was easy, right?", typ="info")
+    overview.add_admonition(text="That was easy, right?")
```

### Comparing `mknodes-0.1.0/mknodes/manual/page_3.py` & `mknodes-0.2.0/mknodes/manual/page_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
 
 INTRO_TEXT = """Lets show some info about the tree we built.
 The tree starts from the root nav down to the Markup elements.
 """
 
 
-def create_page_3(root_nav):
+def create_page_3(root_nav: mknodes.MkNav):
     internals_nav = root_nav.add_nav("Internals")
 
-    overview = internals_nav.add_page("Overview")
+    overview = internals_nav.add_page("Overview", hide_toc=True)
     overview += INTRO_TEXT
 
     # we are here right now.
     overview.add_code(inspect.getsource(create_page_3))
 
     # the "Tree" section in the left sidebar shows what we have done up to now.
     # we create a new page and add a formatted represenation of our Tree.
 
     tree_page = internals_nav.add_page("Tree", hide_toc=True)
     tree_page.add_header("This is the tree we built up to now.", level=3)
     lines = [f"{level * '    '} {node!r}" for level, node in root_nav.iter_nodes()]
-    tree_page += mknodes.Code("\n".join(lines))
+    tree_page += mknodes.MkCode("\n".join(lines))
 
     # Each tree item can carry virtual files. Lets dispay all files which are currently
     # attached to the tree:
     files_page = internals_nav.add_page("File map", hide_toc=True, hide_nav=True)
     files_page.add_header("These are the 'virtual' files attached to the tree:", level=3)
     virtual_files = root_nav.all_virtual_files()
     file_txt = pprint.pformat(list(virtual_files.keys()))
-    files_page += mknodes.Code(file_txt)
+    files_page += mknodes.MkCode(file_txt)
     # print(nodes_nav.to_tree_graph())
```

### Comparing `mknodes-0.1.0/.gitignore` & `mknodes-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/LICENSE` & `mknodes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/README.md` & `mknodes-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/pyproject.toml` & `mknodes-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mknodes-0.1.0/PKG-INFO` & `mknodes-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.1.0 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.2.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.10 Requires-Dist: mkdocs Requires-Dist: mkdocs-
 gen-files Requires-Dist: typing-extensions Description-Content-Type: text/
 markdown # MkNodes
                            Generate docs with ease.
```

