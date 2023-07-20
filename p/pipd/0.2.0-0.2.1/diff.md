# Comparing `tmp/pipd-0.2.0.tar.gz` & `tmp/pipd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.2.0.tar", last modified: Mon Jul 10 16:53:56 2023, max compression
+gzip compressed data, was "pipd-0.2.1.tar", last modified: Thu Jul 20 12:07:00 2023, max compression
```

## Comparing `pipd-0.2.0.tar` & `pipd-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 16:53:56.772686 pipd-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-10 16:53:46.000000 pipd-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.768686 pipd-0.2.0/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/pipd/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/merged.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/write_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/test_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.768686 pipd-0.2.0/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:53:56.772686 pipd-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-10 16:53:46.000000 pipd-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 12:07:00.889286 pipd-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-20 12:06:47.000000 pipd-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.885286 pipd-0.2.1/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/pipd/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/map_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/write_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/test_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.885286 pipd-0.2.1/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:07:00.889286 pipd-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 12:06:47.000000 pipd-0.2.1/setup.py
```

### Comparing `pipd-0.2.0/pipd/pipe.py` & `pipd-0.2.1/pipd/pipe.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,64 +34,84 @@
 def compose(source: Callable, target: Callable):
     def composed(*args):
         return target(source(*args))
 
     return composed
 
 
+class Chain:
+    def __init__(self, *iterables):
+        self.iterables = iterables
+
+    def __iter__(self):
+        for iterable in self.iterables:
+            yield from iterable
+
+
 def unpack_iterable(*iterable: Any) -> Iterable[T]:
     if len(iterable) == 1 and is_iterable(iterable[0]):
         iterable = iterable[0]
     return iterable
 
 
 class PipeMeta(type):
+    def __init__(cls, name, bases, attrs):
+        super().__init__(name, bases, attrs)
+        if name != "Pipe":
+            cls.register()
+
     def __getattr__(cls, name):
+        """Allows to use meta pipe with no iterable: e.g. Pipe.map"""
+
         def method(*args, **kwargs):
             return cls().__getattr__(name)(*args, **kwargs)
 
         return method
 
 
 class Pipe(metaclass=PipeMeta):
+    _iterable: Iterable = []
+    _function: Callable = identity
+    _handler: Callable = log_traceback_and_continue
     _pipes: Dict[str, Type[Pipe]] = {}
 
-    def __init__(self, *iterable, handler: Callable = log_traceback_and_continue):
-        self._iterable: Iterable = unpack_iterable(*iterable)
-        self._function = identity
-        self._handler = handler or log_traceback_and_continue
+    def __init__(self, *iterable, handler: Optional[Callable] = None):
+        self._iterable = unpack_iterable(*iterable)
+        self._handler = handler or self._handler  # type: ignore
+        self._function = identity  # type: ignore
 
     def __call__(self, iterable: Iterable[Any]) -> Iterator[Any]:
         return self._function(iterable)
 
     def __iter__(self):
-        for item in self(iter(self._iterable)):
+        for item in self(self._iterable):
             try:
                 yield item
             except Exception as e:
                 self._handler(e)
 
     def new(self):
         return Pipe()
 
+    def __or__(self, other: Pipe):
+        new = other.new()
+        new._function = compose(self, other)
+        new._iterable = Chain(self._iterable, other._iterable)
+        new._handler = self._handler
+        return new
+
     def __getattr__(self, name):
         def method(*args, **kwargs):
-            pipe_fn = self._pipes[name](*args, **kwargs)
-            pipe = pipe_fn.new()
-            pipe._function = compose(self, pipe_fn)
-            pipe._iterable = self._iterable
-            pipe._handler = self._handler
-            return pipe
+            other = self._pipes[name](*args, **kwargs)
+            return self | other
 
         return method
 
     def close(self):
         # Necessary to use `yield from` on a Pipe object
         pass
 
-    def list(self):
-        return list(self)
-
     @classmethod
-    def register(cls, pipe_type: Type[Pipe], name: Optional[str] = None):
-        pipe_name = camelcase_to_snakecase(pipe_type.__name__) if name is None else name
-        cls._pipes[pipe_name] = pipe_type
+    def register(cls, target: Optional[Type] = None, name: Optional[str] = None):
+        pipe_name = name or camelcase_to_snakecase(cls.__name__)
+        target = target or Pipe
+        target._pipes[pipe_name] = cls
```

### Comparing `pipd-0.2.0/pipd/pipes/batch.py` & `pipd-0.2.1/pipd/pipes/batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,10 +15,7 @@
         for item in items:
             batch.append(item)
             if len(batch) == self.size:
                 yield batch
                 batch = []
         if batch and self.partial:
             yield batch
-
-
-Pipe.register(Batch)
```

### Comparing `pipd-0.2.0/pipd/pipes/filter.py` & `pipd-0.2.1/pipd/pipes/filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,10 +13,7 @@
         self.args = args
         self.kwargs = kwargs
 
     def __call__(self, items: Iterable[T]) -> Iterator[T]:
         for item, keep in Map(self.fn, *self.args, **self.kwargs)(items):  # type: ignore
             if keep:  # type: ignore
                 yield item  # type: ignore
-
-
-Pipe.register(Filter)
```

### Comparing `pipd-0.2.0/pipd/pipes/filter_cached.py` & `pipd-0.2.1/pipd/pipes/filter_cached.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,10 +20,7 @@
         with open(self.filepath, "a") as file:
             for item in items:
                 value = str(self.key(item) if self.key is not None else item)
                 if value not in cache:
                     cache.add(value)
                     file.write(value + "\n")
                     yield item
-
-
-Pipe.register(FilterCached)
```

### Comparing `pipd-0.2.0/pipd/pipes/map.py` & `pipd-0.2.1/pipd/pipes/map.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,10 +55,7 @@
                         except Exception as e:
                             self.handler(e)
             for future in futures:
                 try:
                     yield future.result()
                 except Exception as e:
                     self.handler(e)
-
-
-Pipe.register(Map)
```

### Comparing `pipd-0.2.0/pipd/pipes/merged.py` & `pipd-0.2.1/pipd/pipes/mix.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Callable, Iterable, Iterator, Optional, Sequence, TypeVar
 
 from pipd import Pipe
 
 T = TypeVar("T")
 
 
-def merge_iters(
+def mix_iters(
     *iterators: Iterable[T],
     repeat: bool = False,
     repeat_callback: Optional[Callable] = None,
     random: bool = False,
     weights: Optional[Sequence[float]] = None,
 ) -> Iterator[T]:
     assert weights is None or random, "weights only works with random=True"
@@ -37,27 +37,27 @@
                     # Notify callback with pipe index
                     if repeat_callback is not None:
                         repeat_callback(i)
                 else:
                     return
 
 
-class MergedPipe(Pipe):
+class Mix(Pipe):
     def __init__(
         self,
-        *pipes,
+        *iters,
         repeat: bool = False,
         repeat_callback: Optional[Callable] = None,
         random: bool = False,
         weights: Optional[Sequence[float]] = None,
         **kwargs,
     ):
         super().__init__(
-            merge_iters(
-                *pipes,
+            mix_iters(
+                *iters,
                 repeat=repeat,
                 repeat_callback=repeat_callback,
                 random=random,
                 weights=weights,
             ),
             **kwargs,
         )
```

### Comparing `pipd-0.2.0/pipd/pipes/read_csv.py` & `pipd-0.2.1/pipd/pipes/read_csv.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,10 +15,7 @@
                 if self.header:
                     fieldnames = (
                         self.header if isinstance(self.header, Sequence) else None
                     )
                     yield from csv.DictReader(f, fieldnames=fieldnames)
                 else:
                     yield from csv.reader(f)
-
-
-Pipe.register(ReadCSV)
```

### Comparing `pipd-0.2.0/pipd/pipes/read_files.py` & `pipd-0.2.1/pipd/pipes/read_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,10 +54,7 @@
             if self.shuffle:
                 random.shuffle(files)
 
             for file in files:
                 yield file
             if self.watch:
                 yield from watchdir(os.path.dirname(filepath))
-
-
-Pipe.register(ReadFiles)
```

### Comparing `pipd-0.2.0/pipd/pipes/read_lines.py` & `pipd-0.2.1/pipd/pipes/read_lines.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,10 +23,7 @@
 class ReadLines(Pipe):
     def __init__(self, watch: bool = False) -> None:
         self.watch = watch
 
     def __call__(self, items: Iterable[str]) -> Iterator[str]:
         for filepath in items:
             yield from read_lines(filepath=filepath, watch=self.watch)
-
-
-Pipe.register(ReadLines)
```

### Comparing `pipd-0.2.0/pipd/pipes/shuffle.py` & `pipd-0.2.1/pipd/pipes/shuffle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from random import randint
-from typing import Iterator, List, Optional, TypeVar
+from typing import Iterable, Iterator, List, Optional, TypeVar
 
 from pipd import Pipe
 
 T = TypeVar("T")
 
 
 def pick(items: List[T], random: bool = False) -> T:
@@ -12,24 +12,22 @@
 
 
 class Shuffle(Pipe):
     def __init__(self, size: int, start: Optional[int] = None):
         self.size = size
         self.start = start or size
 
-    def __call__(self, items: Iterator[T]) -> Iterator[T]:  # type: ignore
+    def __call__(self, items: Iterable[T]) -> Iterator[T]:  # type: ignore
         buffer = []
-        for item in items:
+        it = iter(items)
+        for item in it:
             buffer.append(item)
             if len(buffer) < self.size:
                 try:
-                    buffer.append(next(items))
+                    buffer.append(next(it))
                 except StopIteration:
                     pass
             if len(buffer) >= self.start:
                 yield pick(buffer, random=True)
         # Empty buffer at the end
         while len(buffer) > 0:
             yield pick(buffer)
-
-
-Pipe.register(Shuffle)
```

### Comparing `pipd-0.2.0/pipd/pipes/side.py` & `pipd-0.2.1/pipd/pipes/side.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,10 +34,7 @@
         executors = dict(
             multithread=ThreadPoolExecutor, multiprocess=ProcessPoolExecutor
         )
         with executors[self.mode](max_workers=self.num_workers) as executor:
             for item in items:
                 executor.submit(self.fn, item)
                 yield item
-
-
-Pipe.register(Side)
```

### Comparing `pipd-0.2.0/pipd/pipes/write_csv.py` & `pipd-0.2.1/pipd/pipes/write_csv.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,10 +17,7 @@
             for i, item in enumerate(items):
                 if isinstance(item, dict):
                     if i == 0:  # Write headers only for the first dictionary item
                         writer.writerow(item.keys())
                     item = item.values()  # type: ignore
                 writer.writerow(item)
                 yield item
-
-
-Pipe.register(WriteCSV)
```

### Comparing `pipd-0.2.0/pipd/tests/test_pipes.py` & `pipd-0.2.1/pipd/tests/test_pipes.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     assert sorted(pipe) == [0, 2, 4, 6, 8]
 
     # Multiprocess doesn't support lambdas or closures
     pipe = Pipe(range(5)).map(double, num_workers=2, mode="multiprocess")
     assert sorted(pipe) == [0, 2, 4, 6, 8]
 
 
+def test_map_key():
+    pipe = Pipe([{"a": 1}, {"a": 2}, {"a": 3}]).map_key("a", lambda x: x * 2)
+    assert list(pipe) == [{"a": 2}, {"a": 4}, {"a": 6}]
+
+
 def test_filter():
     pipe = Pipe(range(5)).filter(lambda x: x % 2 == 0)
     assert list(pipe) == [0, 2, 4]
 
     pipe = Pipe(range(5)).filter(lambda x: x % 2 == 0, num_workers=2)
     assert sorted(pipe) == [0, 2, 4]
 
@@ -53,14 +58,19 @@
 
 
 def test_limit():
     pipe = Pipe(range(5)).limit(3)
     assert list(pipe) == [0, 1, 2]
 
 
+def test_repeat():
+    pipe = Pipe(range(5)).repeat(2)
+    assert list(pipe) == [0, 1, 2, 3, 4, 0, 1, 2, 3, 4]
+
+
 def test_read_lines():
     import os
     import tempfile
 
     with tempfile.NamedTemporaryFile(mode="w", delete=False) as f:
         f.write("1\n2\n3\n4\n5")
         f.close()
@@ -168,20 +178,20 @@
             f2.write("b")
         pipe = Pipe([f"{d}/*.txt"]).read_files(shuffle=True)
         assert sorted(list(pipe)) == sorted([f1.name, f2.name])
         os.remove(f1.name)
         os.remove(f2.name)
 
 
-def test_merged_pipe():
-    from pipd import MergedPipe
+def test_mix_pipe():
+    from pipd import Mix
 
     pipe = Pipe([0, 1, 2, 3])
     pipe1 = Pipe(["a", "b", "c", "d", "e"])
-    merged = MergedPipe(pipe, pipe1)
+    merged = Mix(pipe, pipe1)
 
     it = iter(merged)
     assert next(it) == 0
     assert next(it) == "a"
     assert next(it) == 1
     assert next(it) == "b"
     assert next(it) == 2
@@ -189,22 +199,24 @@
     assert next(it) == 3
     assert next(it) == "d"
     with pytest.raises(StopIteration):
         next(it)
 
     pipe = Pipe([0, 1, 2, 3])
     pipe1 = Pipe(["a", "b", "c", "d", "e"])
-    merged = MergedPipe(pipe, pipe1, repeat=True)
-
+    merged = Mix(pipe, pipe1, repeat=True)
     it = iter(merged)
     assert next(it) == 0
     assert next(it) == "a"
     assert next(it) == 1
     assert next(it) == "b"
     assert next(it) == 2
     assert next(it) == "c"
     assert next(it) == 3
     assert next(it) == "d"
     assert next(it) == 0
     assert next(it) == "e"
     assert next(it) == 1
     assert next(it) == "a"
+
+    items = list(Pipe.mix(Pipe([0, 1, 2, 3]), Pipe(["a", "b", "c", "d", "e"])))
+    assert items == [0, "a", 1, "b", 2, "c", 3, "d"]
```

### Comparing `pipd-0.2.0/pipd.egg-info/SOURCES.txt` & `pipd-0.2.1/pipd.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 pipd/pipes/__init__.py
 pipd/pipes/batch.py
 pipd/pipes/filter.py
 pipd/pipes/filter_cached.py
 pipd/pipes/limit.py
 pipd/pipes/log.py
 pipd/pipes/map.py
-pipd/pipes/merged.py
+pipd/pipes/map_key.py
+pipd/pipes/mix.py
 pipd/pipes/read_csv.py
 pipd/pipes/read_files.py
 pipd/pipes/read_lines.py
+pipd/pipes/repeat.py
 pipd/pipes/shuffle.py
 pipd/pipes/side.py
 pipd/pipes/sleep.py
 pipd/pipes/tqdm.py
 pipd/pipes/unbatch.py
 pipd/pipes/write_csv.py
 pipd/pipes/write_lines.py
```

