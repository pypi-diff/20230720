# Comparing `tmp/wordz-0.1.6.tar.gz` & `tmp/wordz-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordz-0.1.6.tar", last modified: Sun Jul 16 22:30:56 2023, max compression
+gzip compressed data, was "wordz-0.1.7.tar", last modified: Thu Jul 20 11:03:18 2023, max compression
```

## Comparing `wordz-0.1.6.tar` & `wordz-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.173904 wordz-0.1.6/
--rw-r--r--   0 robert     (501) staff       (20)     1516 2023-07-05 10:00:48.000000 wordz-0.1.6/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-16 22:30:56.173585 wordz-0.1.6/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     4419 2023-07-05 10:00:49.000000 wordz-0.1.6/README.md
--rw-r--r--   0 robert     (501) staff       (20)       38 2023-07-16 22:30:56.174000 wordz-0.1.6/setup.cfg
--rwxr-xr--   0 robert     (501) staff       (20)     1249 2023-05-09 10:42:42.000000 wordz-0.1.6/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.162684 wordz-0.1.6/src/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.168215 wordz-0.1.6/src/wordz/
--rw-r--r--   0 robert     (501) staff       (20)       71 2023-07-05 10:00:49.000000 wordz-0.1.6/src/wordz/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    11000 2023-07-16 22:20:12.000000 wordz-0.1.6/src/wordz/base.py
--rw-r--r--   0 robert     (501) staff       (20)     3222 2023-07-16 22:20:13.000000 wordz-0.1.6/src/wordz/cli.py
--rw-r--r--   0 robert     (501) staff       (20)      431 2023-07-05 10:00:50.000000 wordz-0.1.6/src/wordz/logs.py
--rw-r--r--   0 robert     (501) staff       (20)       62 2023-07-05 10:00:50.000000 wordz-0.1.6/src/wordz/version.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.171140 wordz-0.1.6/src/wordz.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      365 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       41 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/entry_points.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-16 22:21:33.000000 wordz-0.1.6/src/wordz.egg-info/not-zip-safe
--rw-r--r--   0 robert     (501) staff       (20)        6 2023-07-16 22:30:56.000000 wordz-0.1.6/src/wordz.egg-info/top_level.txt
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-16 22:30:56.172666 wordz-0.1.6/tests/
--rw-r--r--   0 robert     (501) staff       (20)     2577 2023-07-05 10:00:58.000000 wordz-0.1.6/tests/test_cli.py
--rw-r--r--   0 robert     (501) staff       (20)     3369 2023-07-16 12:28:58.000000 wordz-0.1.6/tests/test_combinator.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-20 11:03:18.682317 wordz-0.1.7/
+-rw-r--r--   0 robert     (501) staff       (20)     1516 2023-07-05 10:00:48.000000 wordz-0.1.7/LICENSE
+-rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-20 11:03:18.682053 wordz-0.1.7/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     4419 2023-07-05 10:00:49.000000 wordz-0.1.7/README.md
+-rw-r--r--   0 robert     (501) staff       (20)       38 2023-07-20 11:03:18.682444 wordz-0.1.7/setup.cfg
+-rwxr-xr--   0 robert     (501) staff       (20)     1249 2023-05-09 10:42:42.000000 wordz-0.1.7/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-20 11:03:18.675408 wordz-0.1.7/src/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-20 11:03:18.679391 wordz-0.1.7/src/wordz/
+-rw-r--r--   0 robert     (501) staff       (20)       71 2023-07-05 10:00:49.000000 wordz-0.1.7/src/wordz/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    11212 2023-07-20 09:34:54.000000 wordz-0.1.7/src/wordz/base.py
+-rw-r--r--   0 robert     (501) staff       (20)     3218 2023-07-20 09:47:25.000000 wordz-0.1.7/src/wordz/cli.py
+-rw-r--r--   0 robert     (501) staff       (20)      431 2023-07-05 10:00:50.000000 wordz-0.1.7/src/wordz/logs.py
+-rw-r--r--   0 robert     (501) staff       (20)       62 2023-07-20 11:02:33.000000 wordz-0.1.7/src/wordz/version.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2023-07-20 11:03:18.681661 wordz-0.1.7/src/wordz.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)     4980 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      322 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       41 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/entry_points.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/not-zip-safe
+-rw-r--r--   0 robert     (501) staff       (20)        6 2023-07-20 11:03:18.000000 wordz-0.1.7/src/wordz.egg-info/top_level.txt
```

### Comparing `wordz-0.1.6/LICENSE` & `wordz-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wordz-0.1.6/PKG-INFO` & `wordz-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordz
-Version: 0.1.6
+Version: 0.1.7
 Summary: Wordlists builder
 Home-page: https://github.com/tasooshi/wordz
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: BSD License
 Keywords: wordlists,bruteforce,dictionary,generator,hashcat
 Classifier: Development Status :: 4 - Beta
```

### Comparing `wordz-0.1.6/README.md` & `wordz-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `wordz-0.1.6/setup.py` & `wordz-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `wordz-0.1.6/src/wordz/base.py` & `wordz-0.1.7/src/wordz/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,19 @@
                 if not destination.is_file():
                     logs.logger.info(f'Combining `{left.stem}` with `{right.stem}`')
                     self.run_shell(f'{self.bin_combinator} {self.temp_dir}/{right.stem}+{left.stem}{self.DEFAULT_EXT} {right} > {destination}')
             else:
                 raise NotImplementedError
             logs.logger.info(f'Combined `{destination}`')
             return destination
+        else:
+            if self.exist(left):
+                raise Exception(f'Path {right} does not exist. Aborting')
+            else:
+                raise Exception(f'Path {left} does not exist. Aborting')
 
     def merge(self, destination, wordlists, compare=None):
         logs.logger.info(f'Merging: {destination}')
         self.ensure_path(destination)
         wordlists = [words for words in wordlists if words is not None]
         for wordlist in wordlists:
             if wordlist.stat().st_size == 0:
```

### Comparing `wordz-0.1.6/src/wordz/cli.py` & `wordz-0.1.7/src/wordz/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 def main():
     parser = get_parser()
     try:
         run(parser, sys.argv[1:])
     except Exception as exc:
-        logs.logger.error(exc)
-        parser.error(exc)
+        logs.logger.error(f'Error: {exc}')
+        sys.exit(1)
     except KeyboardInterrupt:
         logs.logger.info(f'Exiting')
 
 
 if __name__ == '__main__':
-    sys.exit(main())
+    main()
```

### Comparing `wordz-0.1.6/src/wordz.egg-info/PKG-INFO` & `wordz-0.1.7/src/wordz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordz
-Version: 0.1.6
+Version: 0.1.7
 Summary: Wordlists builder
 Home-page: https://github.com/tasooshi/wordz
 Author: tasooshi
 Author-email: tasooshi@pm.me
 License: BSD License
 Keywords: wordlists,bruteforce,dictionary,generator,hashcat
 Classifier: Development Status :: 4 - Beta
```

