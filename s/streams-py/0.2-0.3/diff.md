# Comparing `tmp/streams_py-0.2.tar.gz` & `tmp/streams_py-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-0.2.tar", max compression
+gzip compressed data, was "streams_py-0.3.tar", max compression
```

## Comparing `streams_py-0.2.tar` & `streams_py-0.3.tar`

### file list

```diff
@@ -1,25 +1,32 @@
--rw-r--r--   0        0        0    35149 2023-06-03 14:38:14.090693 streams_py-0.2/LICENSE
--rw-r--r--   0        0        0     9389 2023-06-03 14:38:14.090693 streams_py-0.2/README.md
--rw-r--r--   0        0        0      750 2023-06-03 14:38:14.094693 streams_py-0.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3483 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__stream.py
--rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     2970 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0    10186 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3733 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2672 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3020 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      646 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      508 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0     9223 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0    10290 1970-01-01 00:00:00.000000 streams_py-0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-20 18:17:11.485866 streams_py-0.3/LICENSE
+-rw-r--r--   0        0        0    10867 2023-07-20 18:17:11.485866 streams_py-0.3/README.md
+-rw-r--r--   0        0        0      731 2023-07-20 18:17:11.489866 streams_py-0.3/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__stream.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    13872 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3629 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2482 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3271 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 streams_py-0.3/PKG-INFO
```

### Comparing `streams_py-0.2/LICENSE` & `streams_py-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/README.md` & `streams_py-0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-![Header](assets/header.png)
+![Header](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/header.png)
 
 <h1 align="center">PyStreamAPI</h1>
 
 <p align="center">
   <a href="https://deepsource.io/gh/PickwickSoft/pystreamapi/?ref=repository-badge"><img src="https://deepsource.io/gh/PickwickSoft/pystreamapi.svg/?label=active+issues&show_trend=true&token=7lV9pH1U-N1oId03M-XKZL5B"  alt="DeepSource"/></a>
   <a href="https://github.com/PickwickSoft/pystreamapi/actions/workflows/unittests.yml"><img src="https://github.com/PickwickSoft/pystreamapi/actions/workflows/unittests.yml/badge.svg"  alt="Tests"/></a>
   <a href="https://github.com/PickwickSoft/pystreamapi/actions/workflows/pylint.yml"><img src="https://github.com/PickwickSoft/pystreamapi/actions/workflows/pylint.yml/badge.svg"  alt="Pylint"/></a>
   <a href="https://sonarcloud.io/summary/new_code?id=PickwickSoft_pystreamapi"><img src="https://sonarcloud.io/api/project_badges/measure?project=PickwickSoft_pystreamapi&metric=alert_status"  alt="Quality Gate"/></a>
   <a href="https://sonarcloud.io/summary/new_code?id=PickwickSoft_pystreamapi"><img src="https://sonarcloud.io/api/project_badges/measure?project=PickwickSoft_pystreamapi&metric=coverage"  alt="Coverage"/></a>
+  <a href="https://pypi.org/project/streams-py/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/streams.py"></a>
+  <a href="https://pypi.org/project/streams-py/"><img alt="PyPI" src="https://img.shields.io/pypi/v/streams.py"></a>
 </p>
 
 PyStreamAPI is a Python stream library that draws inspiration from the Java Stream API. 
 Although it closely mirrors the Java API, PyStreamAPI adds some innovative features to make streams in Python even more 
 innovative, declarative and easy to use.
 
 PyStreamAPI offers both sequential and parallel streams and utilizes lazy execution.
@@ -19,15 +21,15 @@
 Now you might be wondering why another library when there are already a few implementations? Well, here are a few advantages of this particular implementation:
 
 * It provides both sequential and parallel versions.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
-* It adds some cool innovative features like conditions and an even more declarative look
+* It adds some cool innovative features such as conditions or error handling and an even more declarative look.
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -92,18 +94,44 @@
 * It is designed to work seamlessly with lambda functions, enabling concise and expressive code.
 * It facilitates easy aggregation of results into lists, tuples, or sets.
 * It can be parallelized, allowing for concurrent execution of operations to improve performance.
 * It employs lazy evaluation, executing operations only when necessary.
 
 ## Use conditions to speed up your workflow!
 
-![Conditions](./assets/conditions.png)
+![Conditions](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
 
 Conditions provide a convenient means for performing logical operations within your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and more. With PyStreamAPI, you have access to a staggering 111 diverse conditions that enable you to process various data types including strings, types, numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that allows you to effortlessly combine multiple conditions, facilitating the implementation of highly intricate pipelines.
 
+## Error handling: Work with data that you don't know
+PyStreamAPI offers a powerful error handling mechanism that allows you to handle errors in a declarative manner. This is especially useful when working with data that you don't know.
+
+PyStreamAPI offers three different error levels:
+- `ErrorLevel.RAISE`: This is the default error level. It will raise an exception if an error occurs.
+- `ErrorLevel.IGNORE`: This error level will ignore any errors that occur and won't inform you.
+- `ErrorLevel.WARN`: This error level will warn you about any errors that occur and logs them as a warning with default logger.
+
+
+This is how you can use them:
+
+```python
+from pystreamapi import Stream, ErrorLevel
+
+Stream.of([" ", '3', None, "2", 1, ""]) \
+    .error_level(ErrorLevel.IGNORE) \
+    .map_to_int() \
+    .error_level(ErrorLevel.RAISE) \
+    .sorted() \
+    .for_each(print) # Output: 1 2 3
+```
+
+The code above will ignore all errors that occur during mapping to int and will just skip the elements.
+
+For more details on how to use error handling, please refer to the documentation.
+
 ## Get started: Installation
 
 To start using PyStreamAPI just install the module with this command:
 
 ```bash
 pip install streams.py  
 ```
```

#### html2text {}

```diff
@@ -1,108 +1,124 @@
-![Header](assets/header.png)
+![Header](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/
+assets/header.png)
                            ****** PyStreamAPI ******
-            [DeepSource] [Tests] [Pylint] [Quality_Gate] [Coverage]
+  [DeepSource] [Tests] [Pylint] [Quality_Gate] [Coverage] [PyPI_-_Downloads]
+                                    [PyPI]
 PyStreamAPI is a Python stream library that draws inspiration from the Java
 Stream API. Although it closely mirrors the Java API, PyStreamAPI adds some
 innovative features to make streams in Python even more innovative, declarative
 and easy to use. PyStreamAPI offers both sequential and parallel streams and
 utilizes lazy execution. Now you might be wondering why another library when
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
 versions. * Lazy execution is supported, enhancing performance. * It boasts
 high speed and efficiency. * The implementation achieves 100% test coverage. *
 It follows Pythonic principles, resulting in clean and readable code. * It adds
-some cool innovative features like conditions and an even more declarative look
-Let's take a look at a small example: ```python from pystreamapi import Stream
-Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \
-.map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map
-(int) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` And here's the
-equivalent code in Java: ```java Object[] words = { " ", '3', null, "2", 1, ""
-}; Arrays.stream( words ) .filter( Objects::nonNull ) .map( Objects::toString )
-.map( String::trim ) .filter( s -> ! s.isEmpty() ) .map( Integer::parseInt )
-.sorted() .forEach( System.out::println ); // Output: 1 2 3 ``` ## What is a
-Stream? A `Stream` is a powerful abstraction for processing sequences of data
-in a functional and declarative manner. It enables efficient and concise data
-manipulation and transformation. Similar to its counterparts in Java and
-Kotlin, a Stream represents a pipeline of operations that can be applied to a
-collection or any iterable data source. It allows developers to express complex
-data processing logic using a combination of high-level operations, promoting
-code reusability and readability. With Streams, you can perform a wide range of
-operations on your data, such as filtering elements, transforming values,
-aggregating results, sorting, and more. These operations can be seamlessly
-chained together to form a processing pipeline, where each operation processes
-the data and passes it on to the next operation. One of the key benefits of
-Stream is lazy evaluation. This means that the operations are executed only
-when the result is actually needed, optimizing resource usage and enabling
-efficient processing of large or infinite datasets. Furthermore, Stream
-supports both sequential and parallel execution. This allows you to leverage
-parallel processing capabilities when dealing with computationally intensive
-tasks or large amounts of data, significantly improving performance.
-`pystreamapi.Stream` represents a stream that facilitates the execution of one
-or more operations. Stream operations can be categorized as either intermediate
-or terminal. Terminal operations return a result of a specific type, while
-intermediate operations return the stream itself, enabling method chaining for
-multi-step operations. Let's examine an example using Stream: ```python
-Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ #
-Intermediate operation .map(str) \ # Intermediate operation .map(lambda x:
-x.strip()) \ # Intermediate operation .filter(lambda x: len(x) > 0) \ #
-Intermediate operation .map(int) \ # Intermediate operation .sorted() \ #
-Intermediate operation .for_each(print) # Terminal Operation (Output: 1 2 3)
-``` Operations can be performed on a stream either in parallel or sequentially.
-A parallel stream executes operations concurrently, while a sequential stream
-processes operations in order. Considering the above characteristics, a stream
-can be defined as follows: * It is not a data structure itself but operates on
-existing data structures. * It does not provide indexed access like traditional
-collections. * It is designed to work seamlessly with lambda functions,
-enabling concise and expressive code. * It facilitates easy aggregation of
-results into lists, tuples, or sets. * It can be parallelized, allowing for
-concurrent execution of operations to improve performance. * It employs lazy
-evaluation, executing operations only when necessary. ## Use conditions to
-speed up your workflow! ![Conditions](./assets/conditions.png) Conditions
-provide a convenient means for performing logical operations within your
-Stream, such as using `filter()`, `take_while()`, `drop_while()`, and more.
-With PyStreamAPI, you have access to a staggering 111 diverse conditions that
-enable you to process various data types including strings, types, numbers, and
-dates. Additionally, PyStreamAPI offers a powerful combiner that allows you to
-effortlessly combine multiple conditions, facilitating the implementation of
-highly intricate pipelines. ## Get started: Installation To start using
-PyStreamAPI just install the module with this command: ```bash pip install
-streams.py ``` Afterward, you can import it with: ```python from pystreamapi
-import Stream ``` :tada: PyStreamAPI is now ready to process your data ## Build
-a new Stream PyStreamAPI offers two types of Streams, both of which are
-available in either sequential or parallel versions: - (Normal) `Stream`:
-Offers operations that do not depend on the types. The same functionality as
-Streams in other programming languages. - `NumericStream`: This stream extends
-the capabilities of the default stream by introducing numerical operations. It
-is designed specifically for use with numerical data sources and can only be
-applied to such data. There are a few factory methods that create new Streams:
-```python Stream.of([1, 2, 3]) # Can return a sequential or a parallel stream
-``` Using the `of()` method will let the implementation decide which `Stream`
-to use. If the source is numerical, a `NumericStream` is created. > **Note** >
-> Currently, it always returns a `SequentialStream` or a
-`SequentialNumericStream` --- ```python Stream.parallel_of([1, 2, 3]) # Returns
-a parallel stream (Either normal or numeric) ``` --- ```python
-Stream.sequential_of([1, 2, 3]) # Returns a sequential stream (Either normal or
-numeric) ``` --- ```python # Can return a sequential or a parallel stream
-(Either normal or numeric) Stream.of_noneable([1, 2, 3]) # Returns a sequential
-or a parallel, empty stream (Either normal or numeric) Stream.of_noneable(None)
-``` If the source is `None`, you get an empty `Stream` --- ```python
-Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream of an infinite Iterator
-created by iterative application of a function f to an initial element seed,
-producing a Stream consisting of seed, f(seed), f(f(seed)), etc. > **Note** >
-Do not forget to limit the stream with `.limit()` --- ```python Stream.concat
-(Stream.of([1, 2]), Stream.of([3, 4])) # Like Stream.of([1, 2, 3, 4]) ```
-Creates a new Stream from multiple Streams. Order doesn't change. ## API
-Reference For a more detailed documentation view the docs on GitBook:
-[PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ## Complex Examples
-#### Get all numbers from list of different types. Use parallelization.
-```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x:
-x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len
-(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a
-Stream of 10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True:
-yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1
-1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel Streams are not always
-faster than sequential Streams. Especially when the number of elements is
-small, we can expect sequential Streams to be faster. ## Bug Reports Bug
-reports can be submitted in GitHub's [issue tracker](https://github.com/
-PickwickSoft/pystreamapi/issues). ## Contributing Contributions are welcome!
-Please submit a pull request or open an issue.
+some cool innovative features such as conditions or error handling and an even
+more declarative look. Let's take a look at a small example: ```python from
+pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
+(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
+(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
+3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
+'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
+.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
+.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
+1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
+processing sequences of data in a functional and declarative manner. It enables
+efficient and concise data manipulation and transformation. Similar to its
+counterparts in Java and Kotlin, a Stream represents a pipeline of operations
+that can be applied to a collection or any iterable data source. It allows
+developers to express complex data processing logic using a combination of
+high-level operations, promoting code reusability and readability. With
+Streams, you can perform a wide range of operations on your data, such as
+filtering elements, transforming values, aggregating results, sorting, and
+more. These operations can be seamlessly chained together to form a processing
+pipeline, where each operation processes the data and passes it on to the next
+operation. One of the key benefits of Stream is lazy evaluation. This means
+that the operations are executed only when the result is actually needed,
+optimizing resource usage and enabling efficient processing of large or
+infinite datasets. Furthermore, Stream supports both sequential and parallel
+execution. This allows you to leverage parallel processing capabilities when
+dealing with computationally intensive tasks or large amounts of data,
+significantly improving performance. `pystreamapi.Stream` represents a stream
+that facilitates the execution of one or more operations. Stream operations can
+be categorized as either intermediate or terminal. Terminal operations return a
+result of a specific type, while intermediate operations return the stream
+itself, enabling method chaining for multi-step operations. Let's examine an
+example using Stream: ```python Stream.of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ # Intermediate operation .map(str) \ #
+Intermediate operation .map(lambda x: x.strip()) \ # Intermediate operation
+.filter(lambda x: len(x) > 0) \ # Intermediate operation .map(int) \ #
+Intermediate operation .sorted() \ # Intermediate operation .for_each(print) #
+Terminal Operation (Output: 1 2 3) ``` Operations can be performed on a stream
+either in parallel or sequentially. A parallel stream executes operations
+concurrently, while a sequential stream processes operations in order.
+Considering the above characteristics, a stream can be defined as follows: * It
+is not a data structure itself but operates on existing data structures. * It
+does not provide indexed access like traditional collections. * It is designed
+to work seamlessly with lambda functions, enabling concise and expressive code.
+* It facilitates easy aggregation of results into lists, tuples, or sets. * It
+can be parallelized, allowing for concurrent execution of operations to improve
+performance. * It employs lazy evaluation, executing operations only when
+necessary. ## Use conditions to speed up your workflow! ![Conditions](https://
+raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
+Conditions provide a convenient means for performing logical operations within
+your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and
+more. With PyStreamAPI, you have access to a staggering 111 diverse conditions
+that enable you to process various data types including strings, types,
+numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that
+allows you to effortlessly combine multiple conditions, facilitating the
+implementation of highly intricate pipelines. ## Error handling: Work with data
+that you don't know PyStreamAPI offers a powerful error handling mechanism that
+allows you to handle errors in a declarative manner. This is especially useful
+when working with data that you don't know. PyStreamAPI offers three different
+error levels: - `ErrorLevel.RAISE`: This is the default error level. It will
+raise an exception if an error occurs. - `ErrorLevel.IGNORE`: This error level
+will ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`:
+This error level will warn you about any errors that occur and logs them as a
+warning with default logger. This is how you can use them: ```python from
+pystreamapi import Stream, ErrorLevel Stream.of([" ", '3', None, "2", 1, ""]) \
+.error_level(ErrorLevel.IGNORE) \ .map_to_int() \ .error_level
+(ErrorLevel.RAISE) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` The code
+above will ignore all errors that occur during mapping to int and will just
+skip the elements. For more details on how to use error handling, please refer
+to the documentation. ## Get started: Installation To start using PyStreamAPI
+just install the module with this command: ```bash pip install streams.py ```
+Afterward, you can import it with: ```python from pystreamapi import Stream ```
+:tada: PyStreamAPI is now ready to process your data ## Build a new Stream
+PyStreamAPI offers two types of Streams, both of which are available in either
+sequential or parallel versions: - (Normal) `Stream`: Offers operations that do
+not depend on the types. The same functionality as Streams in other programming
+languages. - `NumericStream`: This stream extends the capabilities of the
+default stream by introducing numerical operations. It is designed specifically
+for use with numerical data sources and can only be applied to such data. There
+are a few factory methods that create new Streams: ```python Stream.of([1, 2,
+3]) # Can return a sequential or a parallel stream ``` Using the `of()` method
+will let the implementation decide which `Stream` to use. If the source is
+numerical, a `NumericStream` is created. > **Note** > > Currently, it always
+returns a `SequentialStream` or a `SequentialNumericStream` --- ```python
+Stream.parallel_of([1, 2, 3]) # Returns a parallel stream (Either normal or
+numeric) ``` --- ```python Stream.sequential_of([1, 2, 3]) # Returns a
+sequential stream (Either normal or numeric) ``` --- ```python # Can return a
+sequential or a parallel stream (Either normal or numeric) Stream.of_noneable(
+[1, 2, 3]) # Returns a sequential or a parallel, empty stream (Either normal or
+numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
+`Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
+of an infinite Iterator created by iterative application of a function f to an
+initial element seed, producing a Stream consisting of seed, f(seed), f(f
+(seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
+- ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
+Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
+doesn't change. ## API Reference For a more detailed documentation view the
+docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ##
+Complex Examples #### Get all numbers from list of different types. Use
+parallelization. ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
+.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3
+``` #### Generate a Stream of 10 Fibonacci numbers ```python def fib(): a, b =
+0, 1 while True: yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \
+.for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel
+Streams are not always faster than sequential Streams. Especially when the
+number of elements is small, we can expect sequential Streams to be faster. ##
+Bug Reports Bug reports can be submitted in GitHub's [issue tracker](https://
+github.com/PickwickSoft/pystreamapi/issues). ## Contributing Contributions are
+welcome! Please submit a pull request or open an issue.
```

### Comparing `streams_py-0.2/pyproject.toml` & `streams_py-0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "streams.py"
-version = "0.2"
+version = "0.3"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
 packages = [
     { include = "pystreamapi" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-joblib = "~1.2.0"
-optional-py = "^1.3.2"
+joblib = ">=1.2,<1.4"
 
 [tool.poetry.group.test.dependencies]
 parameterized = "*"
 pylint = "*"
 coverage = "*"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `streams_py-0.2/pystreamapi/__stream.py` & `streams_py-0.3/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/pystreamapi/_lazy/process.py` & `streams_py-0.3/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/pystreamapi/_lazy/queue.py` & `streams_py-0.3/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/pystreamapi/_parallel/fork_and_join.py` & `streams_py-0.3/pystreamapi/_parallel/fork_and_join.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# pylint: disable=protected-access
 import os
 
-from functools import reduce
-from typing import Callable, Any
+from typing import Callable, Any, Optional
 
-from joblib import Parallel, delayed
+from pystreamapi._parallel.parallelizer import Parallel, delayed
+from pystreamapi._streams.error.__error import ErrorHandler
+from pystreamapi._streams.error.__levels import ErrorLevel
+from pystreamapi._itertools.tools import reduce
 
 
 class Parallelizer:
     r"""
     Implementation of the fork-and-join technology.
 
     A given list gets split into multiple sublists,
@@ -17,39 +20,52 @@
     Split: [[1, 2], [3, 4], [5, 6]]\n
     Filter/Reduce: [[3], [7], [11]]\n
     Combine: 21
     """
 
     def __init__(self):
         self.__src = None
+        self.__handler: Optional[ErrorHandler] = None
 
-    def set_source(self, src: list):
-        """Set the source list
+    def set_source(self, src: list, handler: ErrorHandler=None):
+        """
+        Set the source list
+        :param handler: The error handler to be used
         :param src: The source list
         """
         self.__src = src
+        self.__handler = handler
 
     def filter(self, function):
         """Parallel filter function"""
         parts = self.fork()
-        result = self.__run_job_in_parallel(parts, self.__filter, function)
+        if self.__handler is not None and self.__handler._get_error_level() != ErrorLevel.RAISE:
+            result = self.__run_job_in_parallel(parts, self._filter_ignore_errors, function)
+        else:
+            result = self.__run_job_in_parallel(parts, self.__filter, function)
         return [item for sublist in result for item in sublist]
 
+    @staticmethod
+    def __filter(function, src):
+        """Filter function used in the fork-and-join technology"""
+        return [element for element in src if function(element)]
+
+    def _filter_ignore_errors(self, function, src):
+        """Filter function used in the fork-and-join technology using an error handler"""
+        return [self.__handler._one(condition=function, item=element) for element in src]
+
     def reduce(self, function: Callable[[Any, Any], Any]):
         """Parallel reduce function using functools.reduce behind"""
         if len(self.__src) < 2:
             return self.__src
         parts = self.fork(min_nr_items=2)
-        result = self.__run_job_in_parallel(parts, reduce, function)
-        return reduce(function, result)
-
-    @staticmethod
-    def __filter(function, src):
-        """Filter function used in the fork-and-join technology"""
-        return [element for element in src if function(element)]
+        result = self.__run_job_in_parallel(
+            parts, lambda x, y: reduce(function=x, sequence=y, handler=self.__handler), function
+        )
+        return reduce(function, result, handler=self.__handler)
 
     def fork(self, min_nr_items=1):
         """
         Split the source list into multiple sublists.
         The number of sublists is calculated based on the number of CPU cores.
         :param min_nr_items: The minimum number of items per sublist
         :return: A list of sublists
@@ -73,12 +89,12 @@
         """Calculate the number of sublists"""
         if len(self.__src) < min_nr_items:
             return len(self.__src)
         if (len(self.__src) / min_nr_items) < os.cpu_count():
             return round(len(self.__src) / min_nr_items)
         return os.cpu_count() - 2 if os.cpu_count() > 2 else os.cpu_count()
 
-    @staticmethod
-    def __run_job_in_parallel(src, operation, op_function):
+    def __run_job_in_parallel(self, src, operation, op_function):
         """Run the operation in parallel"""
-        return Parallel(n_jobs=-1, prefer="processes")(delayed(operation)(op_function, part)
-                                                       for part in src)
+        return Parallel(n_jobs=-1, prefer="processes", handler=self.__handler)(
+            delayed(operation)(op_function, part) for part in src
+        )
```

### Comparing `streams_py-0.2/pystreamapi/_streams/__parallel_stream.py` & `streams_py-0.3/pystreamapi/_streams/__sequential_stream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,70 @@
-from functools import reduce as seq_reduce
-from typing import Callable, Any, Iterable
-
-from joblib import Parallel, delayed
-from optional import Optional
+from collections import defaultdict
+from typing import Callable, Any
 
 import pystreamapi._streams.__base_stream as stream
-from pystreamapi._lazy.process import Process
-from pystreamapi._parallel.fork_and_join import Parallelizer
+from pystreamapi.__optional import Optional
+from pystreamapi._streams.error.__error import _sentinel
+from pystreamapi._itertools.tools import reduce
 
 _identity_missing = object()
 
 
-class ParallelStream(stream.BaseStream):
-    """The parallel implementation of BaseStream"""
-
-    def __init__(self, source: Iterable[stream.K]):
-        super().__init__(source)
-        self.parallelizer = Parallelizer()
+class SequentialStream(stream.BaseStream):
+    """The sequential implementation of BaseStream"""
 
+    @stream.terminal
     def all_match(self, predicate: Callable[[Any], bool]):
-        self._trigger_exec()
-        return all(Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                                         for element in self._source))
-
-    def filter(self, predicate: Callable[[Any], bool]):
-        self._queue.append(Process(self.__filter, predicate))
-        return self
+        return all(self._itr(self._source, mapper=predicate))
 
-    def __filter(self, predicate: Callable[[Any], bool]):
-        self._set_parallelizer_src()
-        self._source = self.parallelizer.filter(predicate)
+    def _filter(self, predicate: Callable[[Any], bool]):
+        self._source = self._itr(self._source, condition=predicate)
 
+    @stream.terminal
     def find_any(self):
-        self._trigger_exec()
         if len(self._source) > 0:
             return Optional.of(self._source[0])
         return Optional.empty()
 
-    def flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
-        self._queue.append(Process(self.__flat_map, predicate))
-        return self
-
-    def __flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
+    def _flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
         new_src = []
-        for element in Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                                             for element in self._source):
+        for element in self._itr(self._source, mapper=predicate):
             new_src.extend(element.to_list())
         self._source = new_src
 
-    def for_each(self, predicate: Callable):
-        self._trigger_exec()
-        Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                              for element in self._source)
-
-    def map(self, mapper: Callable[[Any], Any]):
-        self._queue.append(Process(self.__map, mapper))
-        return self
-
-    def __map(self, predicate: Callable[[Any], Any]):
-        self._source = Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                                             for element in self._source)
-
-    def map_to_int(self):
-        self._queue.append(Process(self.__map_to_int))
-        return self
-
-    def __map_to_int(self):
-        self.__map(int)
+    def _group_to_dict(self, key_mapper: Callable[[Any], Any]):
+        groups = defaultdict(list)
 
-    def map_to_str(self):
-        self._queue.append(Process(self.__map_to_str))
-        return self
+        for element in self._source:
+            key = self._one(mapper=key_mapper, item=element)
+            if key == _sentinel:
+                continue
+            groups[key].append(element)
+        return groups
+
+    @stream.terminal
+    def for_each(self, action: Callable):
+        self._peek(action)
 
-    def __map_to_str(self):
-        self.__map(str)
+    def _map(self, mapper: Callable[[Any], Any]):
+        self._source = self._itr(self._source, mapper=mapper)
 
-    def peek(self, action: Callable):
-        self._queue.append(Process(self.__peek, action))
-        return self
+    def _peek(self, action: Callable):
+        self._itr(self._source, mapper=action)
 
-    def __peek(self, predicate: Callable):
-        Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                              for element in self._source)
-
-    def reduce(self, predicate: Callable[[Any, Any], Any], identity=_identity_missing,
-               depends_on_state=False):
-        self._trigger_exec()
-        self._set_parallelizer_src()
-        reduce_func = seq_reduce if depends_on_state else self.__reduce
+    @stream.terminal
+    def reduce(self, predicate: Callable, identity=_identity_missing, depends_on_state=False):
         if len(self._source) > 0:
             if identity is not _identity_missing:
-                return reduce_func(predicate, self._source)
-            return Optional.of(reduce_func(predicate, self._source))
+                return reduce(predicate, self._source)
+            return Optional.of(reduce(predicate, self._source, handler=self))
         return identity if identity is not _identity_missing else Optional.empty()
 
-    def __reduce(self, pred, _):
-        return self.parallelizer.reduce(pred)
-
-    def _set_parallelizer_src(self):
-        self.parallelizer.set_source(self._source)
+    @stream.terminal
+    def to_dict(self, key_mapper: Callable[[Any], Any]) -> dict:
+        return self._group_to_dict(key_mapper)
+
+    def _to_numeric_stream(self):
+        # pylint: disable=import-outside-toplevel
+        from pystreamapi._streams.numeric.__sequential_numeric_stream import SequentialNumericStream
+        self.__class__ = SequentialNumericStream
+        return self
```

### Comparing `streams_py-0.2/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-0.3/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,106 @@
 from abc import abstractmethod, ABC
 from collections import Counter
 from typing import Union
 
-from pystreamapi._streams.__base_stream import BaseStream
+from pystreamapi._streams.__base_stream import BaseStream, terminal
 
 
 class NumericBaseStream(BaseStream, ABC):
     """
     This stream extends the capabilities of the default stream by introducing numerical operations.
     It is designed specifically for use with numerical data sources and can only be applied
     to such data.
     """
 
+    @terminal
     def interquartile_range(self) -> Union[float, int, None]:
         """
         Calculates the iterquartile range of a numerical Stream
         :return: The iterquartile range, can be int or float
         """
-        self._trigger_exec()
-        return self.third_quartile() - self.first_quartile() if len(self._source) > 0 else None
+        return self._interquartile_range()
 
+    def _interquartile_range(self):
+        """Implementation of the interquartile range calculation"""
+        return self._third_quartile() - self._first_quartile() if len(self._source) > 0 else None
+
+    @terminal
     def first_quartile(self) -> Union[float, int, None]:
         """
         Calculates the first quartile of a numerical Stream
         :return: The first quartile, can be int or float
         """
-        self._trigger_exec()
+        return self._first_quartile()
+
+    def _first_quartile(self):
+        """Implementation of the first quartile calculation"""
         self._source = sorted(self._source)
         return self.__median(self._source[:(len(self._source)) // 2])
 
     @abstractmethod
+    @terminal
     def mean(self) -> Union[float, int]:
         """
         Calculates the mean of a numerical Stream
         :return: The mean, can be int or float
         """
 
+    @terminal
     def median(self) -> Union[float, int, None]:
         """
         Calculates the median of a numerical Stream
         :return: The median, can be int or float
         """
-        self._trigger_exec()
         return self.__median(self._source)
 
     @staticmethod
     def __median(source) -> Union[float, int, None]:
         """Calculates the median of a numerical Stream"""
         source = sorted(source)
         if not source:
             return None
         midpoint = len(source) // 2
         if len(source) % 2 == 0:
             return (source[midpoint] + source[midpoint - 1]) / 2
         return source[midpoint]
 
+    @terminal
     def mode(self) -> Union[list[Union[int, float]], None]:
         """
-        Calculates the mode(s) (most frequently occurring element) of a numerical Stream
+        Calculates the mode/modes (most frequently occurring element/elements) of a numerical Stream
         :return: The mode, can be int or float
         """
-        self._trigger_exec()
         frequency = Counter(self._source)
         if not frequency:
             return None
         max_frequency = max(frequency.values())
         return [number for number, count in frequency.items() if count == max_frequency]
 
+    @terminal
     def range(self) -> Union[float, int, None]:
         """
         Calculates the range of a numerical Stream
         :return: The range, can be int or float
         """
-        self._trigger_exec()
         return max(self._source) - min(self._source) if len(self._source) > 0 else None
 
+    @abstractmethod
+    @terminal
+    def sum(self) -> Union[float, int, None]:
+        """
+        Calculates the sum of all items of a numerical stream
+        :return: The sum, can be int or float
+        """
+
+    @terminal
     def third_quartile(self) -> Union[float, int, None]:
         """
         Calculates the third quartile of a numerical Stream
         :return: The third quartile, can be int or float
         """
-        self._trigger_exec()
+        return self._third_quartile()
+
+    def _third_quartile(self):
+        """Implementation of the third quartile calculation"""
         self._source = sorted(self._source)
         return self.__median(self._source[(len(self._source) + 1) // 2:])
```

### Comparing `streams_py-0.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-0.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from typing import Union
 
+from pystreamapi._streams.__base_stream import terminal
 from pystreamapi._streams.__parallel_stream import ParallelStream
 from pystreamapi._streams.numeric.__numeric_base_stream import NumericBaseStream
 
 
 class ParallelNumericStream(NumericBaseStream, ParallelStream):
     """Numeric Stream with parallel implementation"""
 
+    @terminal
     def mean(self) -> Union[float, int, None]:
         """Calculates mean of values"""
-        self._trigger_exec()
         return self.__sum() / len(self._source) if len(self._source) > 0 else None
 
+    @terminal
+    def sum(self) -> Union[float, int, None]:
+        """Calculates the sum of values"""
+        _sum = self.__sum()
+        return 0 if _sum == [] else _sum
+
     def __sum(self):
         """Parallel sum method"""
         self._set_parallelizer_src()
-        return self.parallelizer.reduce(lambda x, y: x + y)
+        return self._parallelizer.reduce(lambda x, y: x + y)
```

### Comparing `streams_py-0.2/pystreamapi/conditions/date.py` & `streams_py-0.3/pystreamapi/conditions/date.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,171 +1,188 @@
-from datetime import datetime as __datetime, timedelta as __timedelta, timezone as __timezone
+from datetime import datetime as __datetime, timedelta as __timedelta, timezone as __timezone, \
+    date as __date
+from typing import Union
 
 
-def before(d: __datetime):
+def before(d: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is before a given datetime.
     :param d: The datetime to check against.
     :return: A condition that checks if a datetime is before a given datetime.
     """
     return lambda y: y < d
 
 
-def after(d: __datetime):
+def after(d: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is after a given datetime.
     :param d: The datetime to check against.
     :return: A condition that checks if a datetime is after a given datetime.
     """
     return lambda y: y > d
 
 
-def before_or_equal(d: __datetime):
+def before_or_equal(d: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is before or equal to a given datetime.
     :param d: The datetime to check against.
     :return: A condition that checks if a datetime is before or equal to a given datetime.
     """
     return lambda y: y <= d
 
 
-def after_or_equal(d: __datetime):
+def after_or_equal(d: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is after or equal to a given datetime.
     :param d: The datetime to check against.
     :return: A condition that checks if a datetime is after or equal to a given datetime.
     """
     return lambda y: y >= d
 
 
-def between_or_equal(d: __datetime, y: __datetime):
+def between_or_equal(d: Union[__datetime, __date], y: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is between or equal to two given datetimes.
     :param d: The datetime to check against.
     :param y: The datetime to check against.
     :return: A condition that checks if a datetime is between or equal to two given datetimes.
     """
     return lambda z: d <= z <= y
 
 
-def not_between_or_equal(d: __datetime, y: __datetime):
+def not_between_or_equal(d: Union[__datetime, __date], y: Union[__datetime, __date]):
     """
     Returns a condition that checks if a datetime is not between or equal to two given datetimes.
     :param d: The datetime to check against.
     :param y: The datetime to check against.
     :return: A condition that checks if a datetime is not between or equal to two given datetimes.
     """
     return lambda z: not d <= z <= y
 
 
 def today():
     """
     The condition that checks if a datetime is today.
     :return: A condition that checks if a datetime is today.
     """
-    return lambda d: __datetime.now().date() == d.date()
+    return lambda d: __datetime.now().date() == d.date() if isinstance(d, __datetime) else \
+        __datetime.now().date() == d
 
 
 def today_utc():
     """
     The condition that checks if a datetime is today calculating in UTC (use without parenthesis
     in your Stream).
     :return: A condition that checks if a datetime is today.
     """
-    return lambda d: __datetime.now(__timezone.utc).date() == d.astimezone(__timezone.utc).date()
+    return lambda d: __datetime.now(__timezone.utc).date() == d.astimezone(__timezone.utc).date() \
+        if isinstance(d, __datetime) else __datetime.now(__timezone.utc).date() == d
 
 
 def yesterday():
     """
     The condition that checks if a datetime is yesterday.
     :return: A condition that checks if a datetime is yesterday.
     """
-    return lambda d: __datetime.now().date() - __timedelta(days=1) == d.date()
+    return lambda d: __datetime.now().date() - __timedelta(days=1) == d.date() if \
+        isinstance(d, __datetime) else __datetime.now().date() - __timedelta(days=1) == d
 
 
 def yesterday_utc():
     """
     The condition that checks if a datetime is yesterday calculating in UTC (use without
     parenthesis in your Stream).
     :return: A condition that checks if a datetime is yesterday.
     """
     return lambda d: __datetime.now(__timezone.utc).date() - __timedelta(days=1) == d.astimezone(
-        __timezone.utc).date()
+        __timezone.utc).date() if isinstance(d, __datetime) \
+        else __datetime.now(__timezone.utc).date() - __timedelta(days=1) == d
 
 
 def tomorrow():
     """
     A condition that checks if a datetime is tomorrow.
     :return: A condition that checks if a datetime is tomorrow.
     """
-    return lambda d: __datetime.now().date() + __timedelta(days=1) == d.date()
+    return lambda d: __datetime.now().date() + __timedelta(days=1) == d.date() if \
+        isinstance(d, __datetime) else __datetime.now().date() + __timedelta(days=1) == d
 
 
 def tomorrow_utc():
     """
     A condition that checks if a datetime is tomorrow calculating in UTC (use without parenthesis
     in your Stream).
     :return: A condition that checks if a datetime is tomorrow.
     """
     return lambda d: __datetime.now(__timezone.utc).date() + __timedelta(days=1) == d.astimezone(
-        __timezone.utc).date()
+        __timezone.utc).date() if isinstance(d, __datetime) \
+        else __datetime.now(__timezone.utc).date() + __timedelta(days=1) == d
 
 
 def this_week():
     """
     A condition that checks if a datetime is this week.
     :return: A condition that checks if a datetime is this week.
     """
-    return lambda d: __datetime.now().date().isocalendar()[1] == d.date().isocalendar()[1]
+    return lambda d: __datetime.now().date().isocalendar()[1] == d.date().isocalendar()[1] \
+        if isinstance(d, __datetime) \
+        else __datetime.now().date().isocalendar()[1] == d.isocalendar()[1]
 
 
 def this_week_utc():
     """
     A condition that checks if a datetime is this week calculating in UTC (use without
     parenthesis in your Stream).
     :return: A condition that checks if a datetime is this week.
     """
     return lambda d: __datetime.now(__timezone.utc).date().isocalendar()[1] == \
-        d.astimezone(__timezone.utc).date().isocalendar()[1]
+        d.astimezone(__timezone.utc).date().isocalendar()[1] if isinstance(d, __datetime) else \
+        __datetime.now(__timezone.utc).date().isocalendar()[1] == d.isocalendar()[1]
 
 
 def last_week():
     """
     A condition that checks if a datetime is last week.
     :return: A condition that checks if a datetime is last week.
     """
-    return lambda d: __datetime.now().date().isocalendar()[1] - 1 == d.date().isocalendar()[1]
+    return lambda d: __datetime.now().date().isocalendar()[1] - 1 == d.date().isocalendar()[1] if \
+        isinstance(d, __datetime) \
+        else __datetime.now().date().isocalendar()[1] - 1 == d.isocalendar()[1]
 
 
 def last_week_utc():
     """
     A condition that checks if a datetime is last week calculating in UTC (use without
     parenthesis in your Stream).
     :return: A condition that checks if a datetime is last week.
     """
     return lambda d: __datetime.now(__timezone.utc).date().isocalendar()[1] - 1 == \
-        d.astimezone(__timezone.utc).date().isocalendar()[1]
+        d.astimezone(__timezone.utc).date().isocalendar()[1] if isinstance(d, __datetime) else \
+        __datetime.now(__timezone.utc).date().isocalendar()[1] - 1 == d.isocalendar()[1]
 
 
 def next_week():
     """
     A condition that checks if a datetime is next week.
     :return: A condition that checks if a datetime is next week.
     """
-    return lambda d: __datetime.now().date().isocalendar()[1] + 1 == d.date().isocalendar()[1]
+    return lambda d: __datetime.now().date().isocalendar()[1] + 1 == d.date().isocalendar()[1] if \
+        isinstance(d, __datetime) \
+        else __datetime.now().date().isocalendar()[1] + 1 == d.isocalendar()[1]
 
 
 def next_week_utc():
     """
     A condition that checks if a datetime is next week calculating in UTC (use without
     parenthesis in your Stream).
     :return: A condition that checks if a datetime is next week.
     """
     return lambda d: __datetime.now(__timezone.utc).date().isocalendar()[1] + 1 == \
-        d.astimezone(__timezone.utc).date().isocalendar()[1]
+        d.astimezone(__timezone.utc).date().isocalendar()[1] if isinstance(d, __datetime) else \
+        __datetime.now(__timezone.utc).date().isocalendar()[1] + 1 == d.isocalendar()[1]
 
 
 def this_month():
     """
     A condition that checks if a datetime is this month.
     :return: A condition that checks if a datetime is this month.
     """
@@ -219,15 +236,16 @@
     """
     The actual function that checks if a datetime is a specific month also supporting
     UTC timezone and offsets.
     :param d: The datetime to check against.
     :param offset: The offset to check against.
     :param tz: The timezone to check against.
     """
-    return __datetime.now(tz).date().month + offset == d.astimezone(tz).date().month
+    return __datetime.now(tz).date().month + offset == d.astimezone(tz).date().month if \
+        isinstance(d, __datetime) else __datetime.now(tz).date().month + offset == d.month
 
 
 def this_year():
     """
     A condition that checks if a datetime is this year.
     :return: A condition that checks if a datetime is this year.
     """
@@ -279,8 +297,9 @@
 def __check_is_year(d: __datetime, offset: int = 0, tz: __timezone = None):
     """
     A condition that checks if a datetime is a specific year also supporting
     UTC timezone and offsets.
     :param d: The datetime to check against.
     :param offset: The offset to check against.
     """
-    return __datetime.now(tz).date().year + offset == d.astimezone(tz).date().year
+    return __datetime.now(tz).date().year + offset == d.astimezone(tz).date().year if \
+        isinstance(d, __datetime) else __datetime.now(tz).date().year + offset == d.year
```

### Comparing `streams_py-0.2/pystreamapi/conditions/numeric.py` & `streams_py-0.3/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/pystreamapi/conditions/string.py` & `streams_py-0.3/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/pystreamapi/conditions/types.py` & `streams_py-0.3/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.2/PKG-INFO` & `streams_py-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 0.2
+Version: 0.3
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: joblib (>=1.2.0,<1.3.0)
-Requires-Dist: optional-py (>=1.3.2,<2.0.0)
+Requires-Dist: joblib (>=1.2,<1.4)
 Project-URL: Repository, https://github.com/PickwickSoft/pystreamapi
 Description-Content-Type: text/markdown
 
-![Header](assets/header.png)
+![Header](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/header.png)
 
 <h1 align="center">PyStreamAPI</h1>
 
 <p align="center">
   <a href="https://deepsource.io/gh/PickwickSoft/pystreamapi/?ref=repository-badge"><img src="https://deepsource.io/gh/PickwickSoft/pystreamapi.svg/?label=active+issues&show_trend=true&token=7lV9pH1U-N1oId03M-XKZL5B"  alt="DeepSource"/></a>
   <a href="https://github.com/PickwickSoft/pystreamapi/actions/workflows/unittests.yml"><img src="https://github.com/PickwickSoft/pystreamapi/actions/workflows/unittests.yml/badge.svg"  alt="Tests"/></a>
   <a href="https://github.com/PickwickSoft/pystreamapi/actions/workflows/pylint.yml"><img src="https://github.com/PickwickSoft/pystreamapi/actions/workflows/pylint.yml/badge.svg"  alt="Pylint"/></a>
   <a href="https://sonarcloud.io/summary/new_code?id=PickwickSoft_pystreamapi"><img src="https://sonarcloud.io/api/project_badges/measure?project=PickwickSoft_pystreamapi&metric=alert_status"  alt="Quality Gate"/></a>
   <a href="https://sonarcloud.io/summary/new_code?id=PickwickSoft_pystreamapi"><img src="https://sonarcloud.io/api/project_badges/measure?project=PickwickSoft_pystreamapi&metric=coverage"  alt="Coverage"/></a>
+  <a href="https://pypi.org/project/streams-py/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/streams.py"></a>
+  <a href="https://pypi.org/project/streams-py/"><img alt="PyPI" src="https://img.shields.io/pypi/v/streams.py"></a>
 </p>
 
 PyStreamAPI is a Python stream library that draws inspiration from the Java Stream API. 
 Although it closely mirrors the Java API, PyStreamAPI adds some innovative features to make streams in Python even more 
 innovative, declarative and easy to use.
 
 PyStreamAPI offers both sequential and parallel streams and utilizes lazy execution.
@@ -41,15 +42,15 @@
 Now you might be wondering why another library when there are already a few implementations? Well, here are a few advantages of this particular implementation:
 
 * It provides both sequential and parallel versions.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
-* It adds some cool innovative features like conditions and an even more declarative look
+* It adds some cool innovative features such as conditions or error handling and an even more declarative look.
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -114,18 +115,44 @@
 * It is designed to work seamlessly with lambda functions, enabling concise and expressive code.
 * It facilitates easy aggregation of results into lists, tuples, or sets.
 * It can be parallelized, allowing for concurrent execution of operations to improve performance.
 * It employs lazy evaluation, executing operations only when necessary.
 
 ## Use conditions to speed up your workflow!
 
-![Conditions](./assets/conditions.png)
+![Conditions](https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
 
 Conditions provide a convenient means for performing logical operations within your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and more. With PyStreamAPI, you have access to a staggering 111 diverse conditions that enable you to process various data types including strings, types, numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that allows you to effortlessly combine multiple conditions, facilitating the implementation of highly intricate pipelines.
 
+## Error handling: Work with data that you don't know
+PyStreamAPI offers a powerful error handling mechanism that allows you to handle errors in a declarative manner. This is especially useful when working with data that you don't know.
+
+PyStreamAPI offers three different error levels:
+- `ErrorLevel.RAISE`: This is the default error level. It will raise an exception if an error occurs.
+- `ErrorLevel.IGNORE`: This error level will ignore any errors that occur and won't inform you.
+- `ErrorLevel.WARN`: This error level will warn you about any errors that occur and logs them as a warning with default logger.
+
+
+This is how you can use them:
+
+```python
+from pystreamapi import Stream, ErrorLevel
+
+Stream.of([" ", '3', None, "2", 1, ""]) \
+    .error_level(ErrorLevel.IGNORE) \
+    .map_to_int() \
+    .error_level(ErrorLevel.RAISE) \
+    .sorted() \
+    .for_each(print) # Output: 1 2 3
+```
+
+The code above will ignore all errors that occur during mapping to int and will just skip the elements.
+
+For more details on how to use error handling, please refer to the documentation.
+
 ## Get started: Installation
 
 To start using PyStreamAPI just install the module with this command:
 
 ```bash
 pip install streams.py  
 ```
```

#### html2text {}

```diff
@@ -1,120 +1,136 @@
-Metadata-Version: 2.1 Name: streams-py Version: 0.2 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 0.3 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: joblib (>=1.2.0,<1.3.0) Requires-Dist: optional-py (>=1.3.2,<2.0.0)
-Project-URL: Repository, https://github.com/PickwickSoft/pystreamapi
-Description-Content-Type: text/markdown ![Header](assets/header.png)
+Dist: joblib (>=1.2,<1.4) Project-URL: Repository, https://github.com/
+PickwickSoft/pystreamapi Description-Content-Type: text/markdown ![Header]
+(https://raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/
+header.png)
                            ****** PyStreamAPI ******
-            [DeepSource] [Tests] [Pylint] [Quality_Gate] [Coverage]
+  [DeepSource] [Tests] [Pylint] [Quality_Gate] [Coverage] [PyPI_-_Downloads]
+                                    [PyPI]
 PyStreamAPI is a Python stream library that draws inspiration from the Java
 Stream API. Although it closely mirrors the Java API, PyStreamAPI adds some
 innovative features to make streams in Python even more innovative, declarative
 and easy to use. PyStreamAPI offers both sequential and parallel streams and
 utilizes lazy execution. Now you might be wondering why another library when
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
 versions. * Lazy execution is supported, enhancing performance. * It boasts
 high speed and efficiency. * The implementation achieves 100% test coverage. *
 It follows Pythonic principles, resulting in clean and readable code. * It adds
-some cool innovative features like conditions and an even more declarative look
-Let's take a look at a small example: ```python from pystreamapi import Stream
-Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \
-.map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map
-(int) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` And here's the
-equivalent code in Java: ```java Object[] words = { " ", '3', null, "2", 1, ""
-}; Arrays.stream( words ) .filter( Objects::nonNull ) .map( Objects::toString )
-.map( String::trim ) .filter( s -> ! s.isEmpty() ) .map( Integer::parseInt )
-.sorted() .forEach( System.out::println ); // Output: 1 2 3 ``` ## What is a
-Stream? A `Stream` is a powerful abstraction for processing sequences of data
-in a functional and declarative manner. It enables efficient and concise data
-manipulation and transformation. Similar to its counterparts in Java and
-Kotlin, a Stream represents a pipeline of operations that can be applied to a
-collection or any iterable data source. It allows developers to express complex
-data processing logic using a combination of high-level operations, promoting
-code reusability and readability. With Streams, you can perform a wide range of
-operations on your data, such as filtering elements, transforming values,
-aggregating results, sorting, and more. These operations can be seamlessly
-chained together to form a processing pipeline, where each operation processes
-the data and passes it on to the next operation. One of the key benefits of
-Stream is lazy evaluation. This means that the operations are executed only
-when the result is actually needed, optimizing resource usage and enabling
-efficient processing of large or infinite datasets. Furthermore, Stream
-supports both sequential and parallel execution. This allows you to leverage
-parallel processing capabilities when dealing with computationally intensive
-tasks or large amounts of data, significantly improving performance.
-`pystreamapi.Stream` represents a stream that facilitates the execution of one
-or more operations. Stream operations can be categorized as either intermediate
-or terminal. Terminal operations return a result of a specific type, while
-intermediate operations return the stream itself, enabling method chaining for
-multi-step operations. Let's examine an example using Stream: ```python
-Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ #
-Intermediate operation .map(str) \ # Intermediate operation .map(lambda x:
-x.strip()) \ # Intermediate operation .filter(lambda x: len(x) > 0) \ #
-Intermediate operation .map(int) \ # Intermediate operation .sorted() \ #
-Intermediate operation .for_each(print) # Terminal Operation (Output: 1 2 3)
-``` Operations can be performed on a stream either in parallel or sequentially.
-A parallel stream executes operations concurrently, while a sequential stream
-processes operations in order. Considering the above characteristics, a stream
-can be defined as follows: * It is not a data structure itself but operates on
-existing data structures. * It does not provide indexed access like traditional
-collections. * It is designed to work seamlessly with lambda functions,
-enabling concise and expressive code. * It facilitates easy aggregation of
-results into lists, tuples, or sets. * It can be parallelized, allowing for
-concurrent execution of operations to improve performance. * It employs lazy
-evaluation, executing operations only when necessary. ## Use conditions to
-speed up your workflow! ![Conditions](./assets/conditions.png) Conditions
-provide a convenient means for performing logical operations within your
-Stream, such as using `filter()`, `take_while()`, `drop_while()`, and more.
-With PyStreamAPI, you have access to a staggering 111 diverse conditions that
-enable you to process various data types including strings, types, numbers, and
-dates. Additionally, PyStreamAPI offers a powerful combiner that allows you to
-effortlessly combine multiple conditions, facilitating the implementation of
-highly intricate pipelines. ## Get started: Installation To start using
-PyStreamAPI just install the module with this command: ```bash pip install
-streams.py ``` Afterward, you can import it with: ```python from pystreamapi
-import Stream ``` :tada: PyStreamAPI is now ready to process your data ## Build
-a new Stream PyStreamAPI offers two types of Streams, both of which are
-available in either sequential or parallel versions: - (Normal) `Stream`:
-Offers operations that do not depend on the types. The same functionality as
-Streams in other programming languages. - `NumericStream`: This stream extends
-the capabilities of the default stream by introducing numerical operations. It
-is designed specifically for use with numerical data sources and can only be
-applied to such data. There are a few factory methods that create new Streams:
-```python Stream.of([1, 2, 3]) # Can return a sequential or a parallel stream
-``` Using the `of()` method will let the implementation decide which `Stream`
-to use. If the source is numerical, a `NumericStream` is created. > **Note** >
-> Currently, it always returns a `SequentialStream` or a
-`SequentialNumericStream` --- ```python Stream.parallel_of([1, 2, 3]) # Returns
-a parallel stream (Either normal or numeric) ``` --- ```python
-Stream.sequential_of([1, 2, 3]) # Returns a sequential stream (Either normal or
-numeric) ``` --- ```python # Can return a sequential or a parallel stream
-(Either normal or numeric) Stream.of_noneable([1, 2, 3]) # Returns a sequential
-or a parallel, empty stream (Either normal or numeric) Stream.of_noneable(None)
-``` If the source is `None`, you get an empty `Stream` --- ```python
-Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream of an infinite Iterator
-created by iterative application of a function f to an initial element seed,
-producing a Stream consisting of seed, f(seed), f(f(seed)), etc. > **Note** >
-Do not forget to limit the stream with `.limit()` --- ```python Stream.concat
-(Stream.of([1, 2]), Stream.of([3, 4])) # Like Stream.of([1, 2, 3, 4]) ```
-Creates a new Stream from multiple Streams. Order doesn't change. ## API
-Reference For a more detailed documentation view the docs on GitBook:
-[PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ## Complex Examples
-#### Get all numbers from list of different types. Use parallelization.
-```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x:
-x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len
-(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a
-Stream of 10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True:
-yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1
-1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel Streams are not always
-faster than sequential Streams. Especially when the number of elements is
-small, we can expect sequential Streams to be faster. ## Bug Reports Bug
-reports can be submitted in GitHub's [issue tracker](https://github.com/
-PickwickSoft/pystreamapi/issues). ## Contributing Contributions are welcome!
-Please submit a pull request or open an issue.
+some cool innovative features such as conditions or error handling and an even
+more declarative look. Let's take a look at a small example: ```python from
+pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
+(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
+(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
+3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
+'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
+.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
+.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
+1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
+processing sequences of data in a functional and declarative manner. It enables
+efficient and concise data manipulation and transformation. Similar to its
+counterparts in Java and Kotlin, a Stream represents a pipeline of operations
+that can be applied to a collection or any iterable data source. It allows
+developers to express complex data processing logic using a combination of
+high-level operations, promoting code reusability and readability. With
+Streams, you can perform a wide range of operations on your data, such as
+filtering elements, transforming values, aggregating results, sorting, and
+more. These operations can be seamlessly chained together to form a processing
+pipeline, where each operation processes the data and passes it on to the next
+operation. One of the key benefits of Stream is lazy evaluation. This means
+that the operations are executed only when the result is actually needed,
+optimizing resource usage and enabling efficient processing of large or
+infinite datasets. Furthermore, Stream supports both sequential and parallel
+execution. This allows you to leverage parallel processing capabilities when
+dealing with computationally intensive tasks or large amounts of data,
+significantly improving performance. `pystreamapi.Stream` represents a stream
+that facilitates the execution of one or more operations. Stream operations can
+be categorized as either intermediate or terminal. Terminal operations return a
+result of a specific type, while intermediate operations return the stream
+itself, enabling method chaining for multi-step operations. Let's examine an
+example using Stream: ```python Stream.of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ # Intermediate operation .map(str) \ #
+Intermediate operation .map(lambda x: x.strip()) \ # Intermediate operation
+.filter(lambda x: len(x) > 0) \ # Intermediate operation .map(int) \ #
+Intermediate operation .sorted() \ # Intermediate operation .for_each(print) #
+Terminal Operation (Output: 1 2 3) ``` Operations can be performed on a stream
+either in parallel or sequentially. A parallel stream executes operations
+concurrently, while a sequential stream processes operations in order.
+Considering the above characteristics, a stream can be defined as follows: * It
+is not a data structure itself but operates on existing data structures. * It
+does not provide indexed access like traditional collections. * It is designed
+to work seamlessly with lambda functions, enabling concise and expressive code.
+* It facilitates easy aggregation of results into lists, tuples, or sets. * It
+can be parallelized, allowing for concurrent execution of operations to improve
+performance. * It employs lazy evaluation, executing operations only when
+necessary. ## Use conditions to speed up your workflow! ![Conditions](https://
+raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
+Conditions provide a convenient means for performing logical operations within
+your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and
+more. With PyStreamAPI, you have access to a staggering 111 diverse conditions
+that enable you to process various data types including strings, types,
+numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that
+allows you to effortlessly combine multiple conditions, facilitating the
+implementation of highly intricate pipelines. ## Error handling: Work with data
+that you don't know PyStreamAPI offers a powerful error handling mechanism that
+allows you to handle errors in a declarative manner. This is especially useful
+when working with data that you don't know. PyStreamAPI offers three different
+error levels: - `ErrorLevel.RAISE`: This is the default error level. It will
+raise an exception if an error occurs. - `ErrorLevel.IGNORE`: This error level
+will ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`:
+This error level will warn you about any errors that occur and logs them as a
+warning with default logger. This is how you can use them: ```python from
+pystreamapi import Stream, ErrorLevel Stream.of([" ", '3', None, "2", 1, ""]) \
+.error_level(ErrorLevel.IGNORE) \ .map_to_int() \ .error_level
+(ErrorLevel.RAISE) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` The code
+above will ignore all errors that occur during mapping to int and will just
+skip the elements. For more details on how to use error handling, please refer
+to the documentation. ## Get started: Installation To start using PyStreamAPI
+just install the module with this command: ```bash pip install streams.py ```
+Afterward, you can import it with: ```python from pystreamapi import Stream ```
+:tada: PyStreamAPI is now ready to process your data ## Build a new Stream
+PyStreamAPI offers two types of Streams, both of which are available in either
+sequential or parallel versions: - (Normal) `Stream`: Offers operations that do
+not depend on the types. The same functionality as Streams in other programming
+languages. - `NumericStream`: This stream extends the capabilities of the
+default stream by introducing numerical operations. It is designed specifically
+for use with numerical data sources and can only be applied to such data. There
+are a few factory methods that create new Streams: ```python Stream.of([1, 2,
+3]) # Can return a sequential or a parallel stream ``` Using the `of()` method
+will let the implementation decide which `Stream` to use. If the source is
+numerical, a `NumericStream` is created. > **Note** > > Currently, it always
+returns a `SequentialStream` or a `SequentialNumericStream` --- ```python
+Stream.parallel_of([1, 2, 3]) # Returns a parallel stream (Either normal or
+numeric) ``` --- ```python Stream.sequential_of([1, 2, 3]) # Returns a
+sequential stream (Either normal or numeric) ``` --- ```python # Can return a
+sequential or a parallel stream (Either normal or numeric) Stream.of_noneable(
+[1, 2, 3]) # Returns a sequential or a parallel, empty stream (Either normal or
+numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
+`Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
+of an infinite Iterator created by iterative application of a function f to an
+initial element seed, producing a Stream consisting of seed, f(seed), f(f
+(seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
+- ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
+Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
+doesn't change. ## API Reference For a more detailed documentation view the
+docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ##
+Complex Examples #### Get all numbers from list of different types. Use
+parallelization. ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \
+.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
+.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3
+``` #### Generate a Stream of 10 Fibonacci numbers ```python def fib(): a, b =
+0, 1 while True: yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \
+.for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel
+Streams are not always faster than sequential Streams. Especially when the
+number of elements is small, we can expect sequential Streams to be faster. ##
+Bug Reports Bug reports can be submitted in GitHub's [issue tracker](https://
+github.com/PickwickSoft/pystreamapi/issues). ## Contributing Contributions are
+welcome! Please submit a pull request or open an issue.
```

