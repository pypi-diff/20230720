# Comparing `tmp/pycompall-0.1.9.tar.gz` & `tmp/pycompall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompall-0.1.9.tar", last modified: Fri Jul  7 05:51:43 2023, max compression
+gzip compressed data, was "pycompall-0.2.0.tar", last modified: Thu Jul 20 08:11:00 2023, max compression
```

## Comparing `pycompall-0.1.9.tar` & `pycompall-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.1.9/LICENSE
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.1.9/MANIFEST.in
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-07 05:51:43.376844 pycompall-0.1.9/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:15.000000 pycompall-0.1.9/README.md
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/app/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.1.9/app/__init__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.1.9/app/__main__.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     6214 2023-07-07 05:46:21.000000 pycompall-0.1.9/app/application.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/pycompall.egg-info/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      437 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/PKG-INFO
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      323 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/SOURCES.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/dependency_links.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       44 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/entry_points.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       13 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/requires.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-07 05:51:43.000000 pycompall-0.1.9/pycompall.egg-info/top_level.txt
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1379 2023-07-07 05:51:18.000000 pycompall-0.1.9/pycompall.py
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-07 05:51:43.376844 pycompall-0.1.9/setup.cfg
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      945 2023-07-07 05:51:40.000000 pycompall-0.1.9/setup.py
-drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-07 05:51:43.376844 pycompall-0.1.9/test/
--rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     8978 2023-07-07 05:50:44.000000 pycompall-0.1.9/test/test_compile.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-20 08:11:00.538993 pycompall-0.2.0/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      623 2023-07-07 19:11:59.000000 pycompall-0.2.0/.gitignore
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:18.000000 pycompall-0.2.0/LICENSE
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       27 2023-07-06 05:18:20.000000 pycompall-0.2.0/MANIFEST.in
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      573 2023-07-10 04:40:21.000000 pycompall-0.2.0/Makefile
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3029 2023-07-20 08:11:00.538993 pycompall-0.2.0/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     2342 2023-07-10 02:33:47.000000 pycompall-0.2.0/README.md
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 02:30:35.000000 pycompall-0.2.0/__init__.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-20 08:11:00.538993 pycompall-0.2.0/app/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 05:26:24.000000 pycompall-0.2.0/app/__init__.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-06 01:57:36.000000 pycompall-0.2.0/app/__main__.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-20 08:11:00.538993 pycompall-0.2.0/app/__pycache__/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      155 2023-07-06 05:35:38.000000 pycompall-0.2.0/app/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     5554 2023-07-20 08:09:40.000000 pycompall-0.2.0/app/__pycache__/application.cpython-310.pyc
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     6402 2023-07-20 08:08:54.000000 pycompall-0.2.0/app/application.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-20 08:11:00.538993 pycompall-0.2.0/pycompall.egg-info/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     3029 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/PKG-INFO
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)      472 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/SOURCES.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)        1 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/dependency_links.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       89 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/entry_points.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       23 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/requires.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       14 2023-07-20 08:11:00.000000 pycompall-0.2.0/pycompall.egg-info/top_level.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     2060 2023-07-20 08:07:43.000000 pycompall-0.2.0/pycompall.py
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1044 2023-07-20 08:10:52.000000 pycompall-0.2.0/pyproject.toml
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       25 2023-07-10 01:38:01.000000 pycompall-0.2.0/requirements.txt
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)       38 2023-07-20 08:11:00.538993 pycompall-0.2.0/setup.cfg
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     1087 2023-07-10 04:30:54.000000 pycompall-0.2.0/setup.py
+drwxrwxr-x   0 yongbeom  (1000) yongbeom  (1000)        0 2023-07-20 08:11:00.538993 pycompall-0.2.0/test/
+-rw-rw-r--   0 yongbeom  (1000) yongbeom  (1000)     9569 2023-07-10 04:44:39.000000 pycompall-0.2.0/test/test_compile.py
```

### Comparing `pycompall-0.1.9/setup.py` & `pycompall-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from setuptools import setup, find_packages
 
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-with open("requirements.txt", "r", encoding="utf-8") as fh:
-    requirements = fh.read()
+from setuptools import setup
 
-setup(
-    name='pycompall',
-    version='0.1.9',
-    author='Kim Yongbeom',
-    author_email='yongbeom.kim@u.nus.edu',
-    license='<the license you chose>',
-    description='Wrapper around the python compileall utility.',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://github.com/Yongbeom-Kim/py-compiler',
-    py_modules=['pycompall', 'app.application'],
-    packages=find_packages(),
-    install_requires=[requirements],
-    python_requires='>=3.7',
-    classifiers=[
-        "Programming Language :: Python :: 3.11",
-        "Operating System :: OS Independent",
-    ],
-    entry_points='''
-        [console_scripts]
-        pycompall=pycompall:cli
-    '''
-)
+setup()
+
+"""Below is DEPRECATED for pyproject.toml"""
+# from setuptools import setup, find_packages
+
+# with open("README.md", "r", encoding="utf-8") as fh:
+#     long_description = fh.read()
+# with open("requirements.txt", "r", encoding="utf-8") as fh:
+#     requirements = fh.read()
+
+# setup(
+#     name='pycompall',
+#     version='0.1.13',
+#     author='Kim Yongbeom',
+#     author_email='yongbeom.kim@u.nus.edu',
+#     license='<the license you chose>',
+#     description='Wrapper around the python compileall utility.',
+#     long_description=long_description,
+#     long_description_content_type="text/markdown",
+#     url='https://github.com/Yongbeom-Kim/py-compiler',
+#     py_modules=['pycompall', 'app.application'],
+#     packages=find_packages(),
+#     install_requires=[requirements],
+#     python_requires='>=3.7',
+#     classifiers=[
+#         "Programming Language :: Python :: 3.11",
+#         "Operating System :: OS Independent",
+#     ],
+#     entry_points='''
+#         [console_scripts]
+#         pycompall=pycompall:cli
+#     '''
+# )
```

### Comparing `pycompall-0.1.9/test/test_compile.py` & `pycompall-0.2.0/test/test_compile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple
 import pytest
 from pathlib import Path
-from app.application import _get_pycache_pyc_from_py, compile_command, rmtree
+from app.application import CompilationOptions, _get_pycache_pyc_from_py, compile_command, rmtree
 
 
 @pytest.fixture
 def temp_dir():
     temp_path = Path('./temp')
     temp_path.mkdir(exist_ok=True)
     yield temp_path
@@ -37,189 +37,201 @@
         rmtree(file.parent, missing_ok=True)
 
 
 class TestCompileOneFile:
     def test_compile_one_by_file(self, one_py_file: Tuple[Path, Path]):
         """Test compiling one file by file path, without replacing it."""
         dir, file = one_py_file
-        compile_command(file, recursive=False, in_place=False)
+        options = CompilationOptions(recursive=False, in_place=False)
+        compile_command(file, options)
         expected_pycache_file = _get_pycache_pyc_from_py(file)
         assert expected_pycache_file is not None
         assert expected_pycache_file.exists()
         assert file.exists()
 
     def test_compile_one_by_dir(self, one_py_file: Tuple[Path, Path]):
         """Test compiling one file by parent directory path, without replacing it."""
         dir, file = one_py_file
-        compile_command(file, recursive=False, in_place=False)
+        options = CompilationOptions(recursive=False, in_place=False)
+        compile_command(file, options)
         expected_pycache_file = _get_pycache_pyc_from_py(file)
         assert expected_pycache_file is not None
         assert expected_pycache_file.exists()
         assert file.exists()
 
     def test_compile_one_by_file_in_place(self, one_py_file: Tuple[Path, Path]):
         """Test compiling one file by file path, replacing it."""
         dir, file = one_py_file
-        compile_command(file, recursive=False, in_place=True)
+        options = CompilationOptions(recursive=False, in_place=True)
+        compile_command(file, options)
         expected_pyc_file = file.with_suffix('.pyc')
         assert expected_pyc_file is not None
         assert expected_pyc_file.exists()
         assert not file.exists()
 
     def test_compile_one_by_dir_in_place(self, one_py_file: Tuple[Path, Path]):
         """Test compiling one file by parent directory path, replacing it."""
         dir, file = one_py_file
-        compile_command(file, recursive=False, in_place=True)
+        options = CompilationOptions(recursive=False, in_place=True)
+        compile_command(file, options)
         expected_pyc_file = file.with_suffix('.pyc')
         assert expected_pyc_file is not None
         assert expected_pyc_file.exists()
         assert not file.exists()
 
 
 class TestCompileNestedFiles:
     def test_compile_nested_by_file(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by file path, without replacing it."""
         dir, files = nested_py_file
-        compile_command(files[0], recursive=False, in_place=False)
+        options = CompilationOptions(recursive=False, in_place=False)
+        compile_command(files[0], options)
         expected_pycache_file = _get_pycache_pyc_from_py(files[0])
         unexpected_pycache_files = [
             _get_pycache_pyc_from_py(file) for file in files[1:]]
 
         assert files[0].exists()
         assert expected_pycache_file is not None and expected_pycache_file.exists()
         for file, unexpected_pycache_file in zip(files[1:], unexpected_pycache_files):
             assert file.exists()
             assert unexpected_pycache_file is None or \
                 not unexpected_pycache_file.exists()
 
     def test_compile_nested_by_dir_non_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (non-recursive), without replacing it."""
         dir, files = nested_py_file
-        compile_command(dir, recursive=False, in_place=False)
+        options = CompilationOptions(recursive=False, in_place=False)
+        compile_command(dir, options)
         expected_pycache_files = [_get_pycache_pyc_from_py(
             file) for file in dir.glob('*.py')]
         for file in files:
             assert file.exists()
         for pycache_file in expected_pycache_files:
             assert pycache_file is not None and pycache_file.exists()
 
     def test_compile_nested_by_dir_recursive(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (recursive), without replacing it."""
         dir, files = nested_py_file
-        compile_command(dir, recursive=True, in_place=False)
+        options = CompilationOptions(recursive=True, in_place=False)
+        compile_command(dir, options)
         expected_pycache_files = [_get_pycache_pyc_from_py(
             file) for file in files]
 
         for file in files:
             assert file.exists()
         for pycache_file in expected_pycache_files:
             assert pycache_file is not None and pycache_file.exists()
 
     def test_compile_nested_by_dir_non_recursive_in_place(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (non-recursive), replacing it."""
         dir, files = nested_py_file
         expected_compiled_files = list(dir.glob('*.py'))
-        compile_command(dir, recursive=False, in_place=True)
+        compile_command(dir, CompilationOptions(
+            recursive=False, in_place=True))
 
         for file in files:
             if file in expected_compiled_files:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
             else:
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
 
     def test_compile_nested_by_dir_recursive_in_place(self, nested_py_file: Tuple[Path, List[Path]]):
         """Test compiling nested files by parent directory path (recursive), replacing it."""
         dir, files = nested_py_file
-        compile_command(dir, recursive=True, in_place=True)
+        compile_command(dir, CompilationOptions(recursive=True, in_place=True))
         for file in files:
             assert not file.exists()
             assert file.with_suffix('.pyc').exists()
 
 
 class TestCreateEmptyInit:
     def test_create_empty_init_by_file_fails(self, one_py_file: Tuple[Path, Path]):
         dir, file = one_py_file
         with pytest.raises(ValueError):
-            compile_command(file, create_empty_init=True)
+            compile_command(file, CompilationOptions(create_empty_init=True))
 
     def test_create_empty_init(self, one_py_file: Tuple[Path, Path]):
         dir, file = one_py_file
-        compile_command(dir, create_empty_init=True)
+        compile_command(dir, CompilationOptions(create_empty_init=True))
 
         assert file.exists()
         expected_pycache_file = _get_pycache_pyc_from_py(file)
         assert expected_pycache_file is not None and expected_pycache_file.exists()
         assert (dir / '__init__.py').exists()
 
 
 class TestExcludeFilePattern:
     def test_exclude_all_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         pattern = '*.py'
-        compile_command(dir, recursive=True, in_place=True,
-                        exclude_files=(pattern,))
+        options = CompilationOptions(
+            recursive=True, in_place=True, exclude_files=(pattern,))
+        compile_command(dir, options)
         for file in files:
             if (file.match(pattern)):
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
             else:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
 
     def test_exclude_one_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         pattern = 'one.py'
-        compile_command(dir, recursive=True, in_place=True,
-                        exclude_files=(pattern,))
+        options = CompilationOptions(
+            recursive=True, in_place=True, exclude_files=(pattern,))
+        compile_command(dir, options)
         for file in files:
             if (file.match(pattern)):
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
             else:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
 
 
 class TestExcludeDirPattern:
     def test_exclude_all_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         pattern = '*'
-        compile_command(dir, recursive=True, in_place=True, create_empty_init=True,
-                        exclude_dirs=(pattern,))
+        options = CompilationOptions(
+            recursive=True, in_place=True, create_empty_init=True, exclude_dirs=(pattern,))
+        compile_command(dir, options)
         for file in files:
             dir = file.parent
             init_file = dir / '__init__.py'
             assert not init_file.exists()
             assert file.exists()
             assert not file.with_suffix('.pyc').exists()
 
     def test_exclude_one_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
         print(dir)
         pattern = 'two'
-        compile_command(dir, recursive=True, in_place=True, create_empty_init=True,
-                        exclude_dirs=(pattern,))
+        options = CompilationOptions(
+            recursive=True, in_place=True, create_empty_init=True, exclude_dirs=(pattern,))
+        compile_command(dir, options)
         for file in files:
             if 'two' in str(file):
                 assert file.exists()
                 assert not file.with_suffix('.pyc').exists()
             else:
                 assert not file.exists()
                 assert file.with_suffix('.pyc').exists()
 
         init_file = dir / '__init__.py'
         assert init_file.exists()
 
     def test_exclude_base_pattern(self, nested_py_file: Tuple[Path, List[Path]]):
         dir, files = nested_py_file
-        print(dir)
         pattern = 'temp'
-        compile_command(dir, recursive=True, in_place=True,
-                        exclude_dirs=(pattern,))
+        options = CompilationOptions(
+            recursive=True, in_place=True, exclude_dirs=(pattern,))
+        compile_command(dir, options)
         for file in files:
             assert file.exists()
             assert not file.with_suffix('.pyc').exists()
 
         init_file = dir / '__init__.py'
         assert not init_file.exists()
```

