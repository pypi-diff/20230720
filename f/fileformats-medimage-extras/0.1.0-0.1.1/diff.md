# Comparing `tmp/fileformats_medimage_extras-0.1.0.tar.gz` & `tmp/fileformats_medimage_extras-0.1.1.tar.gz`

## Comparing `fileformats_medimage_extras-0.1.0.tar` & `fileformats_medimage_extras-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.codespell-ignorewords
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/_version.py
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/LICENSE
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/README.rst
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    19272 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/_version.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/README.rst
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.1/PKG-INFO
```

### Comparing `fileformats_medimage_extras-0.1.0/.pre-commit-config.yaml` & `fileformats_medimage_extras-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.0/conftest.py` & `fileformats_medimage_extras-0.1.1/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 import os
 import logging
 from pathlib import Path
 import tempfile
 import pytest
-try:
-    from pydra import set_input_validator
-except ImportError:
-    pass
-else:
-    set_input_validator(True)
 from fileformats.medimage.dicom import DicomDir
 
 # Set DEBUG logging for unittests
 
 log_level = logging.WARNING
 
 logger = logging.getLogger("fileformats")
```

### Comparing `fileformats_medimage_extras-0.1.0/.github/workflows/publish.yml` & `fileformats_medimage_extras-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.0/.github/workflows/tests.yml` & `fileformats_medimage_extras-0.1.1/.github/workflows/tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -15,19 +15,39 @@
   build:
     strategy:
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.8", "3.11"]
       fail-fast: false
     runs-on: ${{ matrix.os }}
+    defaults:
+      run:
+        shell: bash -l {0}
     steps:
     - uses: actions/checkout@v2
     - name: Disable etelemetry
       run:  echo "NO_ET=TRUE" >> $GITHUB_ENV
 
+    - name: Install Dcm2niix
+      run: |
+        curl -fLO https://github.com/rordenlab/dcm2niix/releases/latest/download/dcm2niix_lnx.zip
+        unzip dcm2niix_lnx.zip
+        mv dcm2niix /usr/local/bin
+
+    - name: Install Minconda
+      uses: conda-incubator/setup-miniconda@v2
+      with:
+        auto-activate-base: true
+        activate-environment: ""
+
+    - name: Install MRtrix via Conda
+      run: |
+        conda install -c mrtrix3 mrtrix3
+        mrconvert --version
+
     - name: Set up Python ${{ matrix.python-version }} on ${{ matrix.os }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Update build tools
       run: python -m pip install --upgrade pip
```

### Comparing `fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/converters.py` & `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 import attrs
 import json
 import typing as ty
 import tempfile
 from fileformats.core import mark
-from fileformats.core.utils import MissingExtendedDependency
 from fileformats.medimage.base import MedicalImage
 from fileformats.medimage.dicom import DicomDir, DicomCollection, DicomSet
 from fileformats.medimage import (
     Analyze,
     Nifti,
     NiftiGz,
     NiftiX,
@@ -16,30 +15,18 @@
     MrtrixImage,
     MrtrixImageHeader,
     NiftiXBvec,
     NiftiBvec,
     NiftiGzBvec,
     NiftiGzXBvec,
 )
-try:
-    import jq
-except ImportError:
-    jq = MissingExtendedDependency("jq", __name__)
-try:
-    import pydra
-except ImportError:
-    pydra = MissingExtendedDependency("pydra", __name__)
-try:
-    import pydra.tasks.mrtrix3.utils as pydra_mrtrix3_utils
-except ImportError:
-    pydra_mrtrix3_utils = MissingExtendedDependency("pydra.tasks.mrtrix3", __name__)
-try:
-    import pydra.tasks.dcm2niix as pydra_dcm2niix
-except ImportError:
-    pydra_dcm2niix = MissingExtendedDependency("pydra.tasks.dcm2niix", __name__)
+import jq
+import pydra
+from pydra.tasks.mrtrix3.utils import MRConvert
+from pydra.tasks.dcm2niix import Dcm2Niix
 
 
 @mark.converter(source_format=MedicalImage, target_format=Analyze, out_ext=Analyze.ext)
 @mark.converter(
     source_format=MedicalImage, target_format=MrtrixImage, out_ext=MrtrixImage.ext
 )
 @mark.converter(
@@ -58,15 +45,15 @@
         extension of the output file, used by MRConvert to determine the desired format
 
     Returns
     -------
     pydra.ShellCommandTask
         the converter task
     """
-    return pydra_mrtrix3_utils.MRConvert(name=name, out_file="out" + out_ext)
+    return MRConvert(name=name, out_file="out" + out_ext)
 
 
 @pydra.mark.task
 def ensure_dicom_dir(dicom: DicomCollection) -> DicomDir:
     if isinstance(dicom, DicomSet):
         dicom_dir_fspath = tempfile.mkdtemp()
         dicom.copy(dicom_dir_fspath, link_type="symbolic")
@@ -146,37 +133,37 @@
         ensure_dicom_dir(
             dicom=wf.lzin.in_file,
             name="ensure_dicom_dir",
         )
     )
 
     if file_postfix is None:
-        file_postfix = attrs.NOTHING
+        file_postfix = attrs.NOTHING  # type: ignore
     wf.add(
-        pydra_dcm2niix.Dcm2Niix(
+        Dcm2Niix(
             in_dir=wf.ensure_dicom_dir.lzout.out,
-            out_dir=".",
+            out_dir=Path("."),
             name="dcm2niix",
             compress=compress,
             file_postfix=file_postfix,
         )
     )
     out_file = wf.dcm2niix.lzout.out_file
     out_json = wf.dcm2niix.lzout.out_json
     # Add MRConvert step to either select a single volume of a 4D dataset or the inverse,
     # wrap a single volume in a 4D dataset
     if extract_volume is not None or to_4d:
         if extract_volume:
             coord = [3, extract_volume]
             axes = [0, 1, 2]
         else:  # to_4d
-            coord = attrs.NOTHING
+            coord = attrs.NOTHING  # type: ignore
             axes = [0, 1, 2, -1]
         wf.add(
-            pydra_mrtrix3_utils.MRConvert(
+            MRConvert(
                 in_file=out_file,
                 coord=coord,
                 axes=axes,
                 name="mrconvert",
             )
         )
         out_file = wf.mrconvert.lzout.out_file
```

### Comparing `fileformats_medimage_extras-0.1.0/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage_extras-0.1.1/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     NiftiGzX,
     NiftiGzXBvec,
     NiftiBvec,
     MrtrixImage,
     MrtrixImageHeader,
     Analyze,
 )
-import fileformats.extras.medimage  # noqa
 from logging import getLogger
 
 
 logger = getLogger("fileformats")
 
 
 @pytest.mark.xfail(reason="refactoring of side car handling incomplete")
@@ -36,17 +35,17 @@
     nifti_gz_x_imaginary = NiftiGzX.convert(
         dummy_mixedfmap_dicom, file_postfix="_imaginary"
     )
     nifti_gz_x_real = NiftiGzX.convert(
         dummy_mixedfmap_dicom, file_postfix="_real"
     )
 
-    assert list(nifti_gz_x_ph.dims) == [256, 256, 60]
-    assert list(nifti_gz_x_imaginary.dims) == [256, 256, 60]
-    assert list(nifti_gz_x_real.dims) == [256, 256, 60]
+    assert list(nifti_gz_x_ph.dims()) == [256, 256, 60]
+    assert list(nifti_gz_x_imaginary.dims()) == [256, 256, 60]
+    assert list(nifti_gz_x_real.dims()) == [256, 256, 60]
 
 
 def test_dicom_to_nifti_with_extract_volume(dummy_dwi_dicom):
 
     nifti_gz_x_e1 = NiftiGzX.convert(dummy_dwi_dicom, extract_volume=30)
     assert nifti_gz_x_e1.metadata["dim"][0] == 3
```

### Comparing `fileformats_medimage_extras-0.1.0/LICENSE` & `fileformats_medimage_extras-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.0/README.rst` & `fileformats_medimage_extras-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-FileFormats-medimage Extras
+FileFormats Medimage Extras
 ===========================
 .. image:: https://github.com/arcanaframework/fileformats-medimage-extras/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/arcanaframework/fileformats-medimage-extras/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats-medimage-extras/branch/main/graph/badge.svg?token=UIS0OGPST7
     :target: https://codecov.io/gh/arcanaframework/fileformats-medimage-extras
-.. image:: https://img.shields.io/github/stars/ArcanaFramework/fileformats-medimage-extras.svg
-    :alt: GitHub stars
-    :target: https://github.com/ArcanaFramework/fileformats-medimage
+.. image:: https://img.shields.io/pypi/pyversions/fileformats-medimage-extras.svg
+   :target: https://pypi.python.org/pypi/fileformats-medimage-extras/
+   :alt: Supported Python versions
 .. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
     :target: https://arcanaframework.github.io/fileformats/
     :alt: Documentation Status
 
 
-How to customise this template
-------------------------------
+This is a extras module for the
+`fileformats-medimage <https://github.com/ArcanaFramework/fileformats-medimage>`__ package, which provides
+additional functionality to format classes (i.e. aside from basic identification and validation), such as
+conversion tools, metadata parsers, test data generators, etc...
 
-#. Name your repository with the name fileformats-<SUBPACKAGE-TO-ADD-EXTRAS-TO>-extras
-#. Rename the `fileformats/extras/medimage` directory to the name of the fileformats subpackage the extras are for
-#. Search and replace "medimage" with the name of the fileformats subpackage the extras are to be added
-#. Replace name + email placeholders in `pyproject.toml` for developers and maintainers
-#. Implement selected "extras" by implementing functions decorated by one of the ``*_extra`` hooks defined in the target fileformats class
-#. Ensure that the decorated are imported into the extras package root, i.e. `fileformats/extra/medimage`
-#. Delete these instructions
 
+Prerequisites
+-------------
 
-...
+In order to perform conversions between DICOM and neuroimaging formats such as NIfTI you
+will need to install the following packages
 
+* `Dcm2niix <https://github.com/rordenlab/dcm2niix>`__
+* `MRtrix3 <https://github.com/MRtrix3/MRtrix3>`__
 
-This is a extras module for the
-[fileformats-medimage](https://github.com/ArcanaFramework/fileformats-medimage) package, which provides
-additional functionality to format classes (i.e. aside from basic identification and validation), such as
-conversion tools, metadata parsers, test data generators, etc...
+Please see their installation instructions for the best method for your system
+(alternatively the
+`Test GitHub action <https://github.com/ArcanaFramework/fileformats-medimage-extras/blob/main/.github/workflows/tests.yml>`__
+contains an example installation for Ubuntu)
 
 
-Quick Installation
-------------------
+Installation
+------------
 
 This extension can be installed for Python 3 using *pip*::
 
     $ pip3 install fileformats-medimage-extras
 
-This will install the core package and any other dependencies
 
 License
 -------
 
 This work is licensed under a
 `Creative Commons Attribution 4.0 International License <http://creativecommons.org/licenses/by/4.0/>`_
```

### Comparing `fileformats_medimage_extras-0.1.0/pyproject.toml` & `fileformats_medimage_extras-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requires-python = ">=3.8"
 dependencies = [
     "fileformats >= 0.6",
     "fileformats-medimage >= 0.3",
     "jq >=1.4.0",
     "nibabel >=5.0.0",
     "numpy >=1.20",
+    "medimages4tests >=0.3.0",
     "pydicom >=2.3.1",
     "pydra >= 0.22.0",
     "pydra-dcm2niix",
     "pydra-mrtrix3",
 ]
 license = {file = "LICENSE"}
 authors = [
@@ -33,15 +34,14 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
@@ -84,8 +84,8 @@
 [tool.flake8]
 doctests = true
 per-file-ignores = [
     "__init__.py:F401"
 ]
 max-line-length = 88
 select = "C,E,F,W,B,B950"
-extend-ignore = ['E203', 'E501', 'E129']
+extend-ignore = ['E203', 'E501', 'E129', 'F403']
```

### Comparing `fileformats_medimage_extras-0.1.0/PKG-INFO` & `fileformats_medimage_extras-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage-extras
-Version: 0.1.0
+Version: 0.1.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -101,24 +101,24 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: fileformats-medimage>=0.3
 Requires-Dist: fileformats>=0.6
 Requires-Dist: jq>=1.4.0
+Requires-Dist: medimages4tests>=0.3.0
 Requires-Dist: nibabel>=5.0.0
 Requires-Dist: numpy>=1.20
 Requires-Dist: pydicom>=2.3.1
 Requires-Dist: pydra-dcm2niix
 Requires-Dist: pydra-mrtrix3
 Requires-Dist: pydra>=0.22.0
 Provides-Extra: dev
@@ -131,57 +131,56 @@
 Requires-Dist: codecov; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
-FileFormats-medimage Extras
+FileFormats Medimage Extras
 ===========================
 .. image:: https://github.com/arcanaframework/fileformats-medimage-extras/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/arcanaframework/fileformats-medimage-extras/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats-medimage-extras/branch/main/graph/badge.svg?token=UIS0OGPST7
     :target: https://codecov.io/gh/arcanaframework/fileformats-medimage-extras
-.. image:: https://img.shields.io/github/stars/ArcanaFramework/fileformats-medimage-extras.svg
-    :alt: GitHub stars
-    :target: https://github.com/ArcanaFramework/fileformats-medimage
+.. image:: https://img.shields.io/pypi/pyversions/fileformats-medimage-extras.svg
+   :target: https://pypi.python.org/pypi/fileformats-medimage-extras/
+   :alt: Supported Python versions
 .. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
     :target: https://arcanaframework.github.io/fileformats/
     :alt: Documentation Status
 
 
-How to customise this template
-------------------------------
+This is a extras module for the
+`fileformats-medimage <https://github.com/ArcanaFramework/fileformats-medimage>`__ package, which provides
+additional functionality to format classes (i.e. aside from basic identification and validation), such as
+conversion tools, metadata parsers, test data generators, etc...
 
-#. Name your repository with the name fileformats-<SUBPACKAGE-TO-ADD-EXTRAS-TO>-extras
-#. Rename the `fileformats/extras/medimage` directory to the name of the fileformats subpackage the extras are for
-#. Search and replace "medimage" with the name of the fileformats subpackage the extras are to be added
-#. Replace name + email placeholders in `pyproject.toml` for developers and maintainers
-#. Implement selected "extras" by implementing functions decorated by one of the ``*_extra`` hooks defined in the target fileformats class
-#. Ensure that the decorated are imported into the extras package root, i.e. `fileformats/extra/medimage`
-#. Delete these instructions
 
+Prerequisites
+-------------
 
-...
+In order to perform conversions between DICOM and neuroimaging formats such as NIfTI you
+will need to install the following packages
 
+* `Dcm2niix <https://github.com/rordenlab/dcm2niix>`__
+* `MRtrix3 <https://github.com/MRtrix3/MRtrix3>`__
 
-This is a extras module for the
-[fileformats-medimage](https://github.com/ArcanaFramework/fileformats-medimage) package, which provides
-additional functionality to format classes (i.e. aside from basic identification and validation), such as
-conversion tools, metadata parsers, test data generators, etc...
+Please see their installation instructions for the best method for your system
+(alternatively the
+`Test GitHub action <https://github.com/ArcanaFramework/fileformats-medimage-extras/blob/main/.github/workflows/tests.yml>`__
+contains an example installation for Ubuntu)
 
 
-Quick Installation
-------------------
+Installation
+------------
 
 This extension can be installed for Python 3 using *pip*::
 
     $ pip3 install fileformats-medimage-extras
 
-This will install the core package and any other dependencies
 
 License
 -------
 
 This work is licensed under a
 `Creative Commons Attribution 4.0 International License <http://creativecommons.org/licenses/by/4.0/>`_
```

