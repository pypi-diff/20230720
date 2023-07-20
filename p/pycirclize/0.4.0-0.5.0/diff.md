# Comparing `tmp/pycirclize-0.4.0.tar.gz` & `tmp/pycirclize-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-0.4.0.tar", max compression
+gzip compressed data, was "pycirclize-0.5.0.tar", max compression
```

## Comparing `pycirclize-0.4.0.tar` & `pycirclize-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1062 2023-05-05 12:51:25.158812 pycirclize-0.4.0/LICENSE
--rw-r--r--   0        0        0     4721 2023-05-05 12:51:25.158812 pycirclize-0.4.0/README.md
--rw-r--r--   0        0        0     1436 2023-05-05 12:51:25.298814 pycirclize-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       89 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    30836 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/circos.py
--rw-r--r--   0        0        0     2921 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/config.py
--rw-r--r--   0        0        0      232 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    18100 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    17331 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     7996 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0    12582 2023-05-05 12:51:25.298814 pycirclize-0.4.0/src/pycirclize/patches.py
--rw-r--r--   0        0        0    16431 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/sector.py
--rw-r--r--   0        0        0    46811 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/track.py
--rw-r--r--   0        0        0      534 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     6869 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     3774 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     9955 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/images/python_logo.png
--rw-r--r--   0        0        0     2314 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0     4991 2023-05-05 12:51:25.302814 pycirclize-0.4.0/src/pycirclize/utils/tree.py
--rw-r--r--   0        0        0        0 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1941 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     1752 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     1839 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_gff.py
--rw-r--r--   0        0        0     2090 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     2765 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_circos.py
--rw-r--r--   0        0        0    20530 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_plot.py
--rw-r--r--   0        0        0     2811 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_sector.py
--rw-r--r--   0        0        0      925 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/test_track.py
--rw-r--r--   0        0        0      755 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2023-05-05 12:51:25.302814 pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0   580710 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
--rw-r--r--   0        0        0    58530 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
--rw-r--r--   0        0        0        0 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2025 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2023-05-05 12:51:25.306814 pycirclize-0.4.0/tests/utils/test_helper.py
--rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 pycirclize-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-20 10:39:16.236024 pycirclize-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4721 2023-07-20 10:39:16.236024 pycirclize-0.5.0/README.md
+-rw-r--r--   0        0        0     1436 2023-07-20 10:39:16.380025 pycirclize-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    31266 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     2921 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/config.py
+-rw-r--r--   0        0        0      307 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    18122 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    17331 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     8115 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0     5324 2023-07-20 10:39:16.380025 pycirclize-0.5.0/src/pycirclize/parser/table.py
+-rw-r--r--   0        0        0    12582 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    16500 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    53505 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/track.py
+-rw-r--r--   0        0        0      534 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     6868 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     3774 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     9955 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/images/python_logo.png
+-rw-r--r--   0        0        0     2314 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0     4991 2023-07-20 10:39:16.384025 pycirclize-0.5.0/src/pycirclize/utils/tree.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1941 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/parser/__init__.py
+-rw-r--r--   0        0        0     2628 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     1839 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     4351 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/parser/test_matrix.py
+-rw-r--r--   0        0        0     2883 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/parser/test_table.py
+-rw-r--r--   0        0        0     2765 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/test_circos.py
+-rw-r--r--   0        0        0    23384 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/test_plot.py
+-rw-r--r--   0        0        0     2811 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/test_sector.py
+-rw-r--r--   0        0        0      925 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/test_track.py
+-rw-r--r--   0        0        0      755 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
+-rw-r--r--   0        0        0    30808 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
+-rw-r--r--   0        0        0   283582 2023-07-20 10:39:16.384025 pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
+-rw-r--r--   0        0        0   148834 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
+-rw-r--r--   0        0        0    36204 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/testdata/prokaryote/enterobacteria_phage.gff
+-rw-r--r--   0        0        0   580710 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
+-rw-r--r--   0        0        0    58530 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
+-rw-r--r--   0        0        0        0 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2025 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/utils/test_dataset.py
+-rw-r--r--   0        0        0     1839 2023-07-20 10:39:16.388025 pycirclize-0.5.0/tests/utils/test_helper.py
+-rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 pycirclize-0.5.0/PKG-INFO
```

### Comparing `pycirclize-0.4.0/LICENSE` & `pycirclize-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/README.md` & `pycirclize-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/pyproject.toml` & `pycirclize-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyCirclize"
-version = "0.4.0"
+version = "0.5.0"
 description = "Circular visualization in Python"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyCirclize/"
 repository = "https://github.com/moshi4/pyCirclize/"
 readme = "README.md"
 keywords = [
```

### Comparing `pycirclize-0.4.0/src/pycirclize/circos.py` & `pycirclize-0.5.0/src/pycirclize/circos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import itertools
 import math
+import textwrap
 from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable
 
 import matplotlib.pyplot as plt
 import pandas as pd
@@ -72,17 +73,27 @@
             if len(space) != space_num:
                 err_msg = f"{space=} is invalid.\n"
                 err_msg += f"Length of space list must be {space_num}."
                 raise ValueError(err_msg)
             space_list = list(space) + [0]
             space_deg_size = sum(space)
         else:
-            space_deg_size = space * space_num
             space_list = [space] * space_num + [0]
+            space_deg_size = space * space_num
         whole_deg_size_without_space = whole_deg_size - space_deg_size
+        if whole_deg_size_without_space < 0:
+            err_msg = textwrap.dedent(
+                f"""
+                Too large sector space size is set!!
+                Circos Degree Size = {whole_deg_size} ({start} - {end})
+                Total Sector Space Size = {space_deg_size}
+                List of Sector Space Size = {space_list}
+                """
+            )[1:-1]
+            raise ValueError(err_msg)
         sector_total_size = sum(sectors.values())
 
         rad_pos = math.radians(start)
         self._sectors: list[Sector] = []
         for idx, (sector_name, sector_size) in enumerate(sectors.items()):
             sector_size_ratio = sector_size / sector_total_size
             deg_size = whole_deg_size_without_space * sector_size_ratio
@@ -710,23 +721,21 @@
         savefile: str | Path,
         *,
         dpi: int = 100,
         pad_inches: float = 0.5,
     ) -> None:
         """Save figure to file
 
-        `circos.savefig("result.png")` is alias for the following code
-
-        >>> fig = circos.plotfig()
-        >>> fig.savefig("result.png")
+        `circos.savefig("result.png")` is alias for
+        `circos.plotfig().savefig("result.png")`
 
         Parameters
         ----------
         savefile : str | Path
-            Save file
+            Save file (`*.png`|`*.jpg`|`*.svg`|`*.pdf`)
         dpi : int, optional
             DPI
         pad_inches : float, optional
             Padding inches
         """
         figure = self.plotfig(dpi=dpi)
         figure.savefig(
```

### Comparing `pycirclize-0.4.0/src/pycirclize/config.py` & `pycirclize-0.5.0/src/pycirclize/config.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/parser/bed.py` & `pycirclize-0.5.0/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/parser/genbank.py` & `pycirclize-0.5.0/src/pycirclize/parser/genbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import bz2
 import gzip
 import zipfile
 from collections import defaultdict
-from io import TextIOWrapper
+from io import StringIO, TextIOWrapper
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
 from Bio.SeqFeature import FeatureLocation, Seq, SeqFeature
 from Bio.SeqRecord import SeqRecord
@@ -90,15 +90,15 @@
             return self._name
         if isinstance(self._gbk_source, (str, Path)):
             gbk_file = Path(self._gbk_source)
             if gbk_file.suffix in (".gz", ".bz2", ".zip"):
                 return gbk_file.with_suffix("").with_suffix("").name
             else:
                 return gbk_file.with_suffix("").name
-        elif isinstance(self._gbk_source, TextIOWrapper):
+        elif isinstance(self._gbk_source, (StringIO, TextIOWrapper)):
             return self._records[0].name
         else:
             raise NotImplementedError()
 
     @property
     def records(self) -> list[SeqRecord]:
         """Genbank records"""
```

### Comparing `pycirclize-0.4.0/src/pycirclize/parser/gff.py` & `pycirclize-0.5.0/src/pycirclize/parser/gff.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/parser/matrix.py` & `pycirclize-0.5.0/src/pycirclize/parser/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,19 @@
         return self._col_names
 
     @property
     def row_names(self) -> list[str]:
         """Row names"""
         return self._row_names
 
+    @property
+    def dataframe(self) -> pd.DataFrame:
+        """Matrix dataframe"""
+        return self._matrix
+
     def sort(self, order: str | list[str] = "asc") -> Matrix:
         """Sort order of matrix
 
         Parameters
         ----------
         order : str | list[str] | None, optional
             Sort order of matrix for plotting Chord Diagram.
@@ -216,14 +221,14 @@
         -------
         fromto_table : pd.DataFrame
             From-to table dataframe
         """
         fromto_table_data = []
         for row_name in self.row_names:
             for col_name in self.col_names:
-                value = self._matrix[col_name][row_name]
+                value = self.dataframe[col_name][row_name]
                 if value > 0:
                     fromto_table_data.append([row_name, col_name, value])
         return pd.DataFrame(fromto_table_data, columns=["from", "to", "value"])
 
     def __str__(self):
-        return str(self._matrix)
+        return str(self.dataframe)
```

### Comparing `pycirclize-0.4.0/src/pycirclize/patches.py` & `pycirclize-0.5.0/src/pycirclize/patches.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/sector.py` & `pycirclize-0.5.0/src/pycirclize/sector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import math
+import textwrap
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 import numpy as np
@@ -466,15 +467,17 @@
         self._plot_funcs.append(plot_raster)
 
     ############################################################
     # Private Method
     ############################################################
 
     def __str__(self):
-        return (
-            f"# Sector = '{self.name}'\n"
-            f"# Size = {self.size} ({self.start} - {self.end})\n"
-            f"# Radian size = {self.rad_size:.2f} "
-            f"({min(self.rad_lim):.2f} - {max(self.rad_lim):.2f})\n"
-            f"# Degree size = {self.deg_size:.2f} "
-            f"({min(self.deg_lim):.2f} - {max(self.deg_lim):.2f})\n"
-        )
+        min_deg_lim, max_deg_lim = min(self.deg_lim), max(self.deg_lim)
+        track_names = [t.name for t in self.tracks]
+        return textwrap.dedent(
+            f"""
+            # Sector = '{self.name}'
+            # Size = {self.size} ({self.start} - {self.end})
+            # Degree Size = {self.deg_size:.2f} ({min_deg_lim:.2f} - {max_deg_lim:.2f})
+            # Track List = {track_names}
+            """
+        )[1:]
```

### Comparing `pycirclize-0.4.0/src/pycirclize/track.py` & `pycirclize-0.5.0/src/pycirclize/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import math
+import textwrap
 from copy import deepcopy
 from io import StringIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 
 import matplotlib as mpl
 import numpy as np
+import pandas as pd
 from Bio.Phylo.BaseTree import Clade, Tree
 from Bio.SeqFeature import SeqFeature
 from matplotlib.colors import Colormap, Normalize
 from matplotlib.patches import Patch
 from matplotlib.projections.polar import PolarAxes
 
 from pycirclize import config, utils
+from pycirclize.parser import StackedBarTable
 from pycirclize.patches import ArcArrow, ArcLine, ArcRectangle
 
 if TYPE_CHECKING:
     # Avoid Sector <-> Track circular import error at runtime
     from pycirclize.sector import Sector
 
 
@@ -533,17 +536,14 @@
         text_kws = {} if text_kws is None else deepcopy(text_kws)
 
         # Check y, labels list length
         labels = [""] * len(y) if labels is None else labels
         if len(y) != len(labels):
             err_msg = f"List length is not match ({len(y)=}, {len(labels)=})"
             raise ValueError(err_msg)
-        # Check side value
-        if side not in ("right", "left"):
-            raise ValueError(f"{side=} is invalid ('right' or 'left').")
         # Set vmax & check if y is in min-max range
         vmax = max(y) if vmax is None else vmax
         self._check_value_min_max(y, vmin, vmax)
         # Temporarily set clockwise=True in this method
         original_clockwise = self.clockwise
         self.parent_sector._clockwise = True
 
@@ -561,14 +561,16 @@
                 ha = "right" if is_lower_loc else "left"
             elif side == "left":
                 x_lim = (self.start, self.start - x_tick_length)
                 x_text = self.start - (x_tick_length + x_label_margin)
                 deg_text = math.degrees(self.x_to_rad(x_text, True))
                 is_lower_loc = -270 <= deg_text < -90 or 90 <= deg_text < 270
                 ha = "left" if is_lower_loc else "right"
+            else:
+                raise ValueError(f"{side=} is invalid ('right' or 'left').")
             # Plot yticks
             if tick_length > 0:
                 self._simpleline(x_lim, (r_pos, r_pos), **line_kws)
             # Plot ylabels
             if label != "":
                 va = "center_baseline"
                 _text_kws = deepcopy(text_kws)
@@ -782,14 +784,180 @@
         rad_width = self.rad_size * (width / self.size)
 
         def plot_bar(ax: PolarAxes) -> None:
             ax.bar(rad, r_height, rad_width, r_bottom, align=align, **kwargs)
 
         self._plot_funcs.append(plot_bar)
 
+    def stacked_bar(
+        self,
+        table_data: str | Path | pd.DataFrame | StackedBarTable,
+        *,
+        delimiter: str = "\t",
+        width: float = 0.6,
+        cmap: str | dict[str, str] = "tab10",
+        vmax: float | None = None,
+        show_label: bool = True,
+        label_pos: str = "bottom",
+        label_margin: float = 2,
+        bar_kws: dict[str, Any] | None = None,
+        label_kws: dict[str, Any] | None = None,
+    ) -> StackedBarTable:
+        """Plot stacked bar from table data
+
+        Parameters
+        ----------
+        table_data : str | Path | pd.DataFrame | StackedBarTable
+            Table file or Table DataFrame or StackedBarTable
+        delimiter : str, optional
+            Table file delimiter
+        width : float, optional
+            Bar width ratio (0.0 - 1.0)
+        cmap : str | dict[str, str], optional
+            Colormap assigned to each stacked bar.
+            User can set matplotlib's colormap (e.g. `tab10`, `Set3`) or
+            col_name -> color dict (e.g. `dict(A="red", B="blue", C="green", ...)`)
+        vmax : float | None, optional
+            Stacked bar max value.
+            If None, max value in each row values sum is set.
+        show_label : bool, optional
+            Show table row names as labels
+        label_pos : str, optional
+            Label position (`bottom`|`top`)
+        label_margin : float, optional
+            Label margin size
+        bar_kws : dict[str, Any] | None, optional
+            Axes.bar properties (e.g. `dict(ec="black", lw=0.5, hatch="//", ...)`)
+            <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.bar.html>
+        label_kws : dict[str, Any] | None, optional
+            Text properties (e.g. `dict(size=12, orientation="vertical", ...)`)
+            <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
+
+        Returns
+        -------
+        sb_table : StackedBarTable
+            Stacked bar table
+        """
+        bar_kws = {} if bar_kws is None else deepcopy(bar_kws)
+        label_kws = {} if label_kws is None else deepcopy(label_kws)
+
+        if not 0.0 <= width <= 1.0:
+            raise ValueError(f"{width=} is invalid (0.0 <= width <= 1.0).")
+
+        # Load table data
+        if isinstance(table_data, StackedBarTable):
+            sb_table = table_data
+        else:
+            sb_table = StackedBarTable(table_data, delimiter=delimiter)
+
+        # Make column name & color dict
+        if isinstance(cmap, str):
+            col_name2color = sb_table.get_col_name2color(cmap)
+        else:
+            col_name2color = cmap
+
+        # Calculate bar plot parameters
+        x = sb_table.calc_bar_label_x_list(self.size)
+        width = (self.size / len(sb_table.row_names)) * width
+        vmax = sb_table.row_sum_vmax if vmax is None else vmax
+        heights, bottoms = sb_table.stacked_bar_heights, sb_table.stacked_bar_bottoms
+
+        # Plot bars
+        for col_name, height, bottom in zip(sb_table.col_names, heights, bottoms):
+            color = col_name2color[col_name]
+            self.bar(x, height, width, bottom, vmax=vmax, fc=color, **bar_kws)
+
+        # Plot bar labels
+        if show_label:
+            x_list = sb_table.calc_bar_label_x_list(self.size)
+            row_name2sum = sb_table.row_name2sum
+            for label, x in zip(sb_table.row_names, x_list):
+                # Calculate label r position
+                if label_pos == "top":
+                    bar_r_height = self.r_size * (row_name2sum[label] / vmax)
+                    r = min(self.r_lim) + bar_r_height + label_margin
+                    outer = True
+                elif label_pos == "bottom":
+                    r = min(self.r_lim) - label_margin
+                    outer = False
+                else:
+                    raise ValueError(f"{label_pos=} is invalid ('top' or 'bottom').")
+
+                # Set label text properties
+                if label_kws.get("orientation") is None:
+                    label_kws["orientation"] = "horizontal"
+                params = utils.plot.get_label_params_by_rad(
+                    self.x_to_rad(x), label_kws["orientation"], outer
+                )
+                label_kws.update(params)
+
+                self.text(label, x, r, adjust_rotation=False, **label_kws)
+
+        return sb_table
+
+    def stacked_barh(
+        self,
+        table_data: str | Path | pd.DataFrame | StackedBarTable,
+        *,
+        delimiter: str = "\t",
+        width: float = 0.6,
+        cmap: str | dict[str, str] = "tab10",
+        bar_kws: dict[str, Any] | None = None,
+    ) -> StackedBarTable:
+        """Plot horizontal stacked bar from table data
+
+        Parameters
+        ----------
+        table_data : str | Path | pd.DataFrame | StackedBarTable
+            Table file or Table DataFrame or StackedBarTable
+        delimiter : str, optional
+            Table file delimiter
+        width : float, optional
+            Bar width ratio (0.0 - 1.0)
+        cmap : str | dict[str, str], optional
+            Colormap assigned to each stacked bar.
+            User can set matplotlib's colormap (e.g. `tab10`, `Set3`) or
+            col_name -> color dict (e.g. `dict(A="red", B="blue", C="green", ...)`)
+        bar_kws : dict[str, Any] | None, optional
+            Patch properties for bar plot (e.g. `dict(ec="black, lw=0.2, ...)`)
+
+        Returns
+        -------
+        sb_table : StackedBarTable
+            Stacked bar table
+        """
+        bar_kws = {} if bar_kws is None else deepcopy(bar_kws)
+
+        if not 0.0 <= width <= 1.0:
+            raise ValueError(f"{width=} is invalid (0.0 <= width <= 1.0).")
+
+        # Load table data
+        if isinstance(table_data, StackedBarTable):
+            sb_table = table_data
+        else:
+            sb_table = StackedBarTable(table_data, delimiter=delimiter)
+
+        # Make column name & color dict
+        if isinstance(cmap, str):
+            col_name2color = sb_table.get_col_name2color(cmap)
+        else:
+            col_name2color = cmap
+
+        # Calculate bar plot parameters
+        r_lim_list = sb_table.calc_barh_r_lim_list(self.r_plot_lim, width)
+        heights, bottoms = sb_table.stacked_bar_heights, sb_table.stacked_bar_bottoms
+
+        # Plot bars
+        for col_name, height, bottom in zip(sb_table.col_names, heights, bottoms):
+            color = col_name2color[col_name]
+            for r_lim, h, b in zip(r_lim_list, height, bottom):
+                self.rect(b, b + h, r_lim=r_lim, fc=color, **bar_kws)
+
+        return sb_table
+
     def fill_between(
         self,
         x: list[float] | np.ndarray,
         y1: list[float] | np.ndarray,
         y2: float | list[float] | np.ndarray = 0,
         *,
         vmin: float = 0,
@@ -1212,15 +1380,17 @@
                     raise ValueError(err_msg)
         else:
             if not vmin <= value <= vmax:
                 err_msg = f"{value=} is not in valid range ({vmin=}, {vmax=})"
                 raise ValueError(err_msg)
 
     def __str__(self):
-        return (
-            f"# Track = '{self.name}' (Parent Sector = '{self.parent_sector.name}')\n"
-            f"# Size = {self.size} ({self.start} - {self.end})\n"
-            f"# Radius size = {self.r_size:.2f} "
-            f"({min(self.r_lim):.2f} - {max(self.r_lim):.2f})\n"
-            f"# Degree size = {self.deg_size:.2f} "
-            f"({min(self.deg_lim):.2f} - {max(self.deg_lim):.2f})\n"
-        )
+        min_deg_lim, max_deg_lim = min(self.deg_lim), max(self.deg_lim)
+        min_r_lim, max_r_lim = min(self.r_lim), max(self.r_lim)
+        return textwrap.dedent(
+            f"""
+            # Track = '{self.name}' (Parent Sector = '{self.parent_sector.name}')
+            # Size = {self.size} ({self.start} - {self.end})
+            # Degree Size = {self.deg_size:.2f} ({min_deg_lim:.2f} - {max_deg_lim:.2f})
+            # Radius Size = {self.r_size:.2f} ({min_r_lim:.2f} - {max_r_lim:.2f})
+            """
+        )[1:]
```

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/__init__.py` & `pycirclize-0.5.0/src/pycirclize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/dataset.py` & `pycirclize-0.5.0/src/pycirclize/utils/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 
 def fetch_genbank_by_accid(
     accid: str,
     gbk_outfile: str | Path | None = None,
     email: str | None = None,
 ) -> TextIOWrapper:
-    """Fetch genbank text by 'Accession ID'
+    """Fetch genbank text by `Accession ID`
 
     Parameters
     ----------
     accid : str
         Accession ID
     gbk_outfile : str | Path | None, optional
         If file path is set, write fetch data to file
@@ -175,15 +175,15 @@
     Returns
     -------
     TextIOWrapper
         Genbank data
 
     Examples
     --------
-    >>> gbk_fetch_data = fetch_genbank_by_accid("JX128258.1")
+    >>> gbk_fetch_data = fetch_genbank_by_accid("NC_002483")
     >>> gbk = Genbank(gbk_fetch_data)
     """
     Entrez.email = "" if email is None else email
     gbk_fetch_data: TextIOWrapper = Entrez.efetch(
         db="nucleotide",
         id=accid,
         rettype="gbwithparts",
```

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/helper.py` & `pycirclize-0.5.0/src/pycirclize/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/images/python_logo.png` & `pycirclize-0.5.0/src/pycirclize/utils/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/plot.py` & `pycirclize-0.5.0/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/src/pycirclize/utils/tree.py` & `pycirclize-0.5.0/src/pycirclize/utils/tree.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/conftest.py` & `pycirclize-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/parser/test_genbank.py` & `pycirclize-0.5.0/tests/parser/test_gff.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from pathlib import Path
 
-from pycirclize.parser import Genbank
+from pycirclize.parser import Gff
 
 
 def test_parse_complete_genome(prokaryote_testdata_dir: Path):
     """Test parse complete genome"""
-    gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
-    gbk = Genbank(gbk_file)
+    gff_file = prokaryote_testdata_dir / "enterobacteria_phage.gff"
+    gff = Gff(gff_file)
     seqid = "NC_000902.1"
-    assert gbk.name == "enterobacteria_phage"
+    assert gff.target_seqid == seqid
     max_genome_size = 60942
-    assert gbk.range_size == max_genome_size
-    assert gbk.genome_length == max_genome_size
-    assert gbk.full_genome_length == max_genome_size
-    assert gbk.min_range == 0
-    assert gbk.max_range == max_genome_size
-    assert gbk.get_seqid2size() == {seqid: max_genome_size}
+    assert gff.range_size == max_genome_size
+    assert gff.min_range == 0
+    assert gff.max_range == max_genome_size
+    assert gff.seq_region == (0, max_genome_size)
+    assert gff.seqid_list == [seqid]
+    assert gff.get_seqid2size() == {seqid: max_genome_size}
 
 
 def test_parse_contig_genomes(prokaryote_testdata_dir: Path):
     """Test parse contig genomes"""
-    gbk_file = prokaryote_testdata_dir / "mycoplasma_alvi.gbk.gz"
-    gbk = Genbank(gbk_file)
+    gff_file = prokaryote_testdata_dir / "mycoplasma_alvi.gff.gz"
+    gff = Gff(gff_file)
     seqid2size = {
         "NZ_JNJU01000001.1": 264665,
         "NZ_JNJU01000002.1": 190782,
         "NZ_KL370824.1": 158240,
         "NZ_KL370825.1": 155515,
         "NZ_JNJU01000007.1": 67647,
         "NZ_JNJU01000008.1": 2683,
         "NZ_JNJU01000009.1": 1108,
     }
-    total_genome_size = sum(list(seqid2size.values()))
+    seqid_list = list(seqid2size.keys())
+    size_list = list(seqid2size.values())
 
-    assert gbk.name == "mycoplasma_alvi"
-    assert gbk.range_size == total_genome_size
-    assert gbk.min_range == 0
-    assert gbk.max_range == total_genome_size
-    assert gbk.get_seqid2size() == seqid2size
+    assert gff.target_seqid == list(seqid2size.keys())[0]
+    assert gff.range_size == size_list[0]
+    assert gff.min_range == 0
+    assert gff.max_range == size_list[0]
+    assert gff.seq_region == (0, size_list[0])
+    assert gff.seqid_list == seqid_list
+    assert gff.get_seqid2size() == seqid2size
 
-    seqid2cds_features = gbk.get_seqid2features(pseudogene=None)
+    seqid2cds_features = gff.get_seqid2features(pseudogene=None)
     first_contig_cds_features = list(seqid2cds_features.values())[0]
     assert len(first_contig_cds_features) == 204
 
-    seqid2trna_features = gbk.get_seqid2features("tRNA", pseudogene=None)
+    seqid2trna_features = gff.get_seqid2features("tRNA", pseudogene=None)
     first_contig_trna_features = list(seqid2trna_features.values())[0]
     assert len(first_contig_trna_features) == 12
```

### Comparing `pycirclize-0.4.0/tests/parser/test_gff.py` & `pycirclize-0.5.0/tests/parser/test_genbank.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 from pathlib import Path
 
-from pycirclize.parser import Gff
+from pycirclize.parser import Genbank
 
 
 def test_parse_complete_genome(prokaryote_testdata_dir: Path):
     """Test parse complete genome"""
-    gff_file = prokaryote_testdata_dir / "enterobacteria_phage.gff"
-    gff = Gff(gff_file)
+    gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
+    gbk = Genbank(gbk_file)
     seqid = "NC_000902.1"
-    assert gff.target_seqid == seqid
+    assert gbk.name == "enterobacteria_phage"
     max_genome_size = 60942
-    assert gff.range_size == max_genome_size
-    assert gff.min_range == 0
-    assert gff.max_range == max_genome_size
-    assert gff.seq_region == (0, max_genome_size)
-    assert gff.seqid_list == [seqid]
-    assert gff.get_seqid2size() == {seqid: max_genome_size}
+    assert gbk.range_size == max_genome_size
+    assert gbk.genome_length == max_genome_size
+    assert gbk.full_genome_length == max_genome_size
+    assert gbk.min_range == 0
+    assert gbk.max_range == max_genome_size
+    assert gbk.get_seqid2size() == {seqid: max_genome_size}
 
 
 def test_parse_contig_genomes(prokaryote_testdata_dir: Path):
     """Test parse contig genomes"""
-    gff_file = prokaryote_testdata_dir / "mycoplasma_alvi.gff.gz"
-    gff = Gff(gff_file)
+    gbk_file = prokaryote_testdata_dir / "mycoplasma_alvi.gbk.gz"
+    gbk = Genbank(gbk_file)
     seqid2size = {
         "NZ_JNJU01000001.1": 264665,
         "NZ_JNJU01000002.1": 190782,
         "NZ_KL370824.1": 158240,
         "NZ_KL370825.1": 155515,
         "NZ_JNJU01000007.1": 67647,
         "NZ_JNJU01000008.1": 2683,
         "NZ_JNJU01000009.1": 1108,
     }
-    seqid_list = list(seqid2size.keys())
-    size_list = list(seqid2size.values())
+    total_genome_size = sum(list(seqid2size.values()))
 
-    assert gff.target_seqid == list(seqid2size.keys())[0]
-    assert gff.range_size == size_list[0]
-    assert gff.min_range == 0
-    assert gff.max_range == size_list[0]
-    assert gff.seq_region == (0, size_list[0])
-    assert gff.seqid_list == seqid_list
-    assert gff.get_seqid2size() == seqid2size
+    assert gbk.name == "mycoplasma_alvi"
+    assert gbk.range_size == total_genome_size
+    assert gbk.min_range == 0
+    assert gbk.max_range == total_genome_size
+    assert gbk.get_seqid2size() == seqid2size
 
-    seqid2cds_features = gff.get_seqid2features(pseudogene=None)
+    seqid2cds_features = gbk.get_seqid2features(pseudogene=None)
     first_contig_cds_features = list(seqid2cds_features.values())[0]
     assert len(first_contig_cds_features) == 204
 
-    seqid2trna_features = gff.get_seqid2features("tRNA", pseudogene=None)
+    seqid2trna_features = gbk.get_seqid2features("tRNA", pseudogene=None)
     first_contig_trna_features = list(seqid2trna_features.values())[0]
     assert len(first_contig_trna_features) == 12
+
+
+def test_calc_gc(prokaryote_testdata_dir: Path):
+    """Test GCskew, GCcontent calculation"""
+    gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
+    gbk = Genbank(gbk_file)
+    gbk.calc_gc_skew()
+    gbk.calc_gc_content()
+
+
+def test_write_cds_fasta(prokaryote_testdata_dir: Path, fig_outfile: Path):
+    """Test `gbk.write_cds_fasta()` (only check properly output file)"""
+    gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
+    gbk = Genbank(gbk_file)
+    gbk.write_cds_fasta(fig_outfile)
+    assert fig_outfile.exists()
+
+
+def test_genome_fasta(prokaryote_testdata_dir: Path, fig_outfile: Path):
+    """Test `gbk.write_genome_fasta()` (only check properly output file)"""
+    gbk_file = prokaryote_testdata_dir / "enterobacteria_phage.gbk"
+    gbk = Genbank(gbk_file)
+    gbk.write_genome_fasta(fig_outfile)
+    assert fig_outfile.exists()
```

### Comparing `pycirclize-0.4.0/tests/test_circos.py` & `pycirclize-0.5.0/tests/test_circos.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/test_plot.py` & `pycirclize-0.5.0/tests/test_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from Bio import Phylo
 
 from pycirclize import Circos
-from pycirclize.parser import Genbank, Gff
+from pycirclize.parser import Genbank, Gff, StackedBarTable
 from pycirclize.utils import (
     ColorCycler,
     load_eukaryote_example_dataset,
+    load_example_image_file,
     load_prokaryote_example_file,
 )
 
 np.random.seed(0)
 random.seed(0)
 
 
@@ -211,14 +212,33 @@
         start, end = sector.start + 3, sector.end - 3
         sector.rect(start, end, (30, 100), color="orange", alpha=0.2)
 
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
 
 
+def test_sector_raster_plot(fig_outfile: Path):
+    """Test `sector.raster()`"""
+    sectors = {"A": 10, "B": 15, "C": 12, "D": 20, "E": 15}
+    circos = Circos(sectors, space=5)
+    for sector in circos.sectors:
+        # Plot line in sector region
+        sector.axis(ec="grey")
+        for r in range(10, 100, 10):
+            sector.line(r=r, ec="lightgrey")
+        # Plot raster image (python logo)
+        logo_file = load_example_image_file("python_logo.png")
+        sector.raster(logo_file, r=110, label=sector.name)
+        sector.raster(logo_file, r=50, size=0.1, rotation="auto", border_width=5)
+        sector.text(sector.name, r=62)
+
+    circos.savefig(fig_outfile)
+    assert fig_outfile.exists()
+
+
 ###########################################################
 # Track Class Plot
 ###########################################################
 
 
 def test_track_axis_plot(fig_outfile: Path):
     """Test `track.axis()`"""
@@ -476,14 +496,69 @@
             vmax=vmax * 2,
         )
 
     circos.savefig(fig_outfile)
     assert fig_outfile.exists()
 
 
+def test_track_stacked_bar_plot(fig_outfile: Path):
+    """Test `track.stacked_bar()`"""
+    # Generate matrix data for stacked bar plot
+    row_num, col_num = 12, 6
+    matrix = np.random.randint(5, 20, (row_num, col_num))
+    row_names = [f"R{i}" for i in range(row_num)]
+    col_names = [f"group{i}" for i in range(col_num)]
+    table_df = pd.DataFrame(matrix, index=row_names, columns=col_names)
+
+    # Initialize Circos sector & track
+    circos = Circos(sectors=dict(bar=len(table_df.index)))
+    sector = circos.sectors[0]
+    track = sector.add_track((50, 100))
+
+    # Plot stacked bar
+    track.stacked_bar(
+        table_df,
+        width=0.6,
+        cmap="Set3",
+        bar_kws=dict(ec="black", lw=0.2),
+        label_pos="bottom",
+        label_kws=dict(size=10, orientation="horizontal"),
+    )
+
+    circos.savefig(fig_outfile)
+    assert fig_outfile.exists()
+
+
+def test_track_stacked_barh_plot(fig_outfile: Path):
+    """Test `track.stacked_barh()`"""
+    # Generate & load matrix data for horizontal stacked bar plot
+    row_names = list("ABCDEF")
+    col_names = ["group1", "group2", "group3", "group4", "group5", "group6"]
+    matrix = np.random.randint(5, 20, (len(row_names), len(col_names)))
+    table_df = pd.DataFrame(matrix, index=row_names, columns=col_names)
+    sb_table = StackedBarTable(table_df)
+
+    # Initialize Circos sector & track (0 <= range <= 270)
+    circos = Circos(sectors=dict(bar=sb_table.row_sum_vmax), start=0, end=270)
+    sector = circos.sectors[0]
+    track = sector.add_track((30, 100))
+    track.axis(fc="lightgrey", ec="black", alpha=0.5)
+
+    # Plot horizontal stacked bar & label & xticks
+    track.stacked_barh(sb_table.dataframe, cmap="tab10", width=0.6)
+    label_r_list = sb_table.calc_barh_label_r_list(track.r_plot_lim)
+    for label_r, row_name in zip(label_r_list, sb_table.row_names):
+        track.text(f"{row_name} ", x=0, r=label_r, ha="right")
+    track.xticks_by_interval(interval=5)
+    track.xticks_by_interval(interval=1, tick_length=1, show_label=False)
+
+    circos.savefig(fig_outfile)
+    assert fig_outfile.exists()
+
+
 def test_track_fill_between_plot(fig_outfile: Path):
     """Test `track.fill_between()`"""
     sectors = {"A": 10, "B": 20, "C": 15}
     circos = Circos(sectors, space=5)
     for sector in circos.sectors:
         vmin, vmax = 0, 10
         # Plot fill_between with simple lines
```

### Comparing `pycirclize-0.4.0/tests/test_sector.py` & `pycirclize-0.5.0/tests/test_sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/test_track.py` & `pycirclize-0.5.0/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_chr.bed` & `pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_chr.bed`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv` & `pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv` & `pycirclize-0.5.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gbk` & `pycirclize-0.5.0/tests/testdata/prokaryote/enterobacteria_phage.gbk`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/prokaryote/enterobacteria_phage.gff` & `pycirclize-0.5.0/tests/testdata/prokaryote/enterobacteria_phage.gff`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz` & `pycirclize-0.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz` & `pycirclize-0.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/utils/test_dataset.py` & `pycirclize-0.5.0/tests/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/tests/utils/test_helper.py` & `pycirclize-0.5.0/tests/utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.4.0/PKG-INFO` & `pycirclize-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycirclize
-Version: 0.4.0
+Version: 0.5.0
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
```

