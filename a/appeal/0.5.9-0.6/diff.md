# Comparing `tmp/appeal-0.5.9.tar.gz` & `tmp/appeal-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.9.tar", last modified: Fri May  5 07:28:01 2023, max compression
+gzip compressed data, was "appeal-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `appeal-0.5.9.tar` & `appeal-0.6.tar`

### file list

```diff
@@ -1,13 +1,24 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.9/.gitignore
--rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.9/LICENSE
--rw-r--r--   0        0        0    69688 2023-05-05 07:27:29.162568 appeal-0.5.9/README.md
--rw-r--r--   0        0        0   168554 2023-05-05 07:15:41.683718 appeal-0.5.9/appeal/__init__.py
--rw-r--r--   0        0        0    23888 2023-05-05 07:12:51.458204 appeal-0.5.9/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.9/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.9/appeal/text.py
--rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.9/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/links.txt
--rw-r--r--   0        0        0    67934 2023-05-05 04:50:34.315935 appeal-0.5.9/tests/run_tests.py
--rw-r--r--   0        0        0    70182 1970-01-01 00:00:00.000000 appeal-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.6/.gitignore
+-rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.6/LICENSE
+-rw-r--r--   0        0        0    83589 2023-07-20 13:32:28.219271 appeal-0.6/README.md
+-rw-r--r--   0        0        0   278507 2023-07-20 13:28:58.640891 appeal-0.6/appeal/__init__.py
+-rw-r--r--   0        0        0    23888 2023-06-22 08:40:31.452281 appeal-0.6/appeal/argument_grouping.py
+-rwxr-xr-x   0        0        0     4637 2023-07-20 13:28:58.640891 appeal-0.6/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:57:46.416604 appeal-0.6/appeal/text.py
+-rwxr-xr-x   0        0        0     4721 2023-07-20 13:28:58.644891 appeal-0.6/appeal/want_prints.py
+-rw-r--r--   0        0        0      595 2023-07-20 13:28:58.644891 appeal-0.6/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.6/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.6/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.6/resources/links.txt
+-rw-r--r--   0        0        0      715 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky1.pky
+-rw-r--r--   0        0        0      319 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky2.pky
+-rw-r--r--   0        0        0      274 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky3.pky
+-rw-r--r--   0        0        0      323 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/perkytest1.pky
+-rw-r--r--   0        0        0    49711 2023-07-20 13:28:58.648891 appeal-0.6/tests/read_corpus/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0      290 2023-07-20 13:28:58.648891 appeal-0.6/tests/read_corpus/tomltest1.toml
+-rw-r--r--   0        0        0    77772 2023-07-20 13:28:58.648891 appeal-0.6/tests/test_all.py
+-rw-r--r--   0        0        0    12963 2023-07-20 13:28:58.648891 appeal-0.6/tests/test_read.py
+-rw-r--r--   0        0        0     1136 2023-06-17 11:18:04.335043 appeal-0.6/tests/want_prints_test_corpus/README.md
+-rw-r--r--   0        0        0      975 2023-06-17 11:13:44.684903 appeal-0.6/tests/want_prints_test_corpus/commented.py
+-rw-r--r--   0        0        0      917 2023-06-17 11:13:17.480679 appeal-0.6/tests/want_prints_test_corpus/uncommented.py
+-rw-r--r--   0        0        0    84177 1970-01-01 00:00:00.000000 appeal-0.6/PKG-INFO
```

### Comparing `appeal-0.5.9/LICENSE` & `appeal-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/README.md` & `appeal-0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1357,15 +1357,15 @@
 
 What's really going on here is that, from Appeal's perspective,
 *there's no difference between a "command function" and a
 "converter".*  A command function is just a converter that
 happens to be mapped to a command.  So anything you can do
 with a command function, you can do with a converter too.
 A converter can define options, it can be decorated with
-`app.option()` (or `app.argument()` which we haven't
+`app.option()` (or `app.parameter()` which we haven't
 discussed yet), it can have accept any kind of parameter defined
 by Python, and any parameter can use (almost) any converter.
 And those converters can recursively use other converters.
 
 Realy, anything can be used with anything:
 
 * Converters for positional parameters
@@ -1534,14 +1534,326 @@
 these bits of documentation together to produce the help for your
 command function.
 
 (One note: the main help for your program should be the docstring
 for your Appeal instance's global command.)
 
 
+## Appeal's latest superpower: reading config files
+
+Appeal allows for friction-free command-line APIs.  You write your
+command function, point Appeal at it, and whoosh! now you've got a
+command-line interface.  But there are other interfaces users may
+want to use to configure your program.  Now Appeal can work with
+those too.
+
+For example, your program may read configuration from environment
+variables.  Some programs launch an editor; for example `git` will
+open an editor when committing a revision.  Traditionally on
+UNIX-based platforms this is configurable using two environment
+variables, `VISUAL` and `EDITOR` in that order of preference.
+
+Appeal doesn't need to add explicit support for environment variables,
+as Python already has an easy-to-use interface.  For example, here's
+how to support the environment variables configuring your editor:
+
+However, many programs also support a configuration file, also called
+an "rc file"  on UNIX.  By convention settings in such a config file
+usually take precedence over environment variables.  For example, you
+can configure what editor `git` uses for commits with a value called
+`core.editor` stored in a config file.
+
+As of 0.6, Appeal has support for reading data from configuration
+files.  Note that Appeal doesn't read the data files itself; you
+already have a library for that.  Instead, Appeal has a generic
+mechanism for reading data from either an iterable or a mapping--
+either a list or a dict.
+
+The first step is to read in the values from the configuration file,
+and produce a dict or dict-like object.  You can use any library
+you like.  For example, the [`tomli`](https://pypi.org/project/tomli/) library
+works well for [TOML files.](https://en.wikipedia.org/wiki/TOML)
+JSON and YAML parsers also work nicely.  And this facility works
+*especially* well with my [`Perky`](https://pypi.org/project/perky/)
+file format.  Though that's just a coincidence, as they were designed
+separately, years apart.  Honest!
+
+(You can also use `configparser` to read your INI config file,
+but this doesn't mesh well with Appeal's model.  Better support
+for reading INI files is a possible future direction for Appeal.)
+
+Once you've got a dictionary containing your configuration information,
+you can get Appeal to read from it using a single method call:
+
+```Python
+    Appeal.read_mapping(self, callable, mapping)
+```
+
+Simply pass in the callable you want called, and the mapping--the dict--you
+read from your config file.  Appeal will read the names of the callable's
+parameters, pull values out of the mapping using those names, and pass those
+values in to a call to the callable.
+
+Of course, any mapping will work.  But this method works particularly
+well with classes decorated with `dataclasses.dataclass`.  In just a few
+lines, you can define a class to contain your configuration information,
+read it out of a file, and populate the class with values of all the correct
+types!
+
+In a lot of ways, this works very similarly to Appeal when it's processing
+a command-line.  For example:
+
+* Appeal will use the annotations and default values to convert
+  the values from the dictionary into the correct types.
+* Parameters with default values are optional; parameters without
+  default values are required.
+
+But there are differences too:
+
+* You can use positional-only, positional-or-keyword,
+  or keyword-only arguments.  However, var-positional
+  (`*args`) and var-keyword (`**kwargs`) are unsupported.
+
+
+Let's bring all of this together with an example.  Let's say we're
+writing a hypothetical program that may launch an editor.  Our
+sophisticated program has *five* ways to decide what program
+to run for the editor.  In decreasing order of importance:
+
+* Command-line options '-e' and '--editor' specify the
+  editor to use for this instnace.
+* The config file `~/.myprogramrc` is a Perky file, and it
+  can contain an `editor` value.
+* If the user has set an `VISUAL` environment variable, use that.
+* If the user has set an `EDITOR` environment variable, use that.
+* The default value is `/usr/bin/vi`.
+
+Here's sample Python code implementing those semantics:
+
+```Python
+    default_editor = os.environ.get("VISUAL",
+        os.environ.get("EDITOR", "/usr/bin/vi"))
+    @dataclasses.dataclass
+    class ConfigFile:
+        editor:str=default_editor
+
+    d = perky.load(os.path.expanduser("~/.myprogramrc"))
+    app = appeal.Appeal()
+    config_file = app.read_mapping(ConfigFile, d)
+
+    @app.global_command()
+    def global_command(*, editor=config_file.editor):
+        print(f"editor = {editor}")
+
+    app.main()
+```
+
+Note: using `os.path.expanduser` and a hard-coded filename
+like this is no longer considered best practice.  You should use 
+[`platformdirs`](https://pypi.org/project/platformdirs/) to
+define the paths to your config files.
+
+### Nesting
+
+Appeal's config file reader supports reading values from nested dicts.
+This maps directly onto nested function calls in annotations.  If an
+annotation takes two or more parameters, the name of the parameter
+with that annotation will be used as the name of the nested dict.
+
+Since that probably wasn't clear--sorry!--an example would probably help.
+Consider this example dictionary:
+
+```Python
+    d = {
+        'a': 33,
+        'b': {
+            'verbose': True,
+            'color': 'blue',
+        },
+    }
+```
+
+Here the value of `'b'` is a nested dict.  If we want Appeal to read
+a dict with this shape, it will have to descend into that nested dict.
+Appeal does that by default when a parameter has an annotation, and
+the annotation takes two or more parameters.  Here's sample Python
+showing how to read this dict using Appeal:
+
+```Python
+    def read_b(verbose=False, color='black'):
+        return (verbose, color)
+
+    def config_file(a: int, b: read_b):
+        return (a, b)
+```
+
+Because `read_b` is an annotation taking multiple parameters,
+Appeal will assume the value of `'b'` is a nested dict,
+and will get the values of `'verbose'` and `'color'` from
+that dict.
+
+If you don't want this behavior, you can disable it by
+decorating the annotation function with the `unnested`
+method on the Appeal object.  If we change the code to
+the following:
+
+```Python
+    @app.unnested()
+    def read_b(verbose=False, color='black'):
+        return (verbose, color)
+
+    def config_file(a: int, b: read_b):
+        return (a, b)
+```
+
+Appeal *won't* descend into a nested dict named `'b'`.
+In this case the dictionary would have to be be completely
+flat, like this:
+
+```Python
+    d = { 'a': 33, 'verbose': True, 'color': 'blue' }
+```
+
+### Iterables
+
+Appeal can also read from iterables inside the dictionary.
+The parameter that accepts an iterable should be annotated
+with a subclass of `MultiOption`.  Appeal will instantiate
+the `MultiOption` and use the MultiOption protocol to
+fill the object.
+
+For example, if your config file dict looked like this:
+
+```Python
+    d = {
+        'color': 'blue',
+        'lines': [
+            'line 1',
+            'here is line 2',
+            'and finally, line 3',
+            ]
+    }
+```
+
+Appeal could map it to this callable:
+
+```Python
+    @dataclasses.dataclass
+    class ConfigFile:
+        lines: appeal.accumulator
+        color:str = ''
+```
+
+If the `MultiOption` option takes multiple parameters,
+then the list must contain dictionaries.  For example,
+this Python code:
+
+```Python
+    class Resolutions(appeal.Multioption):
+        def init(self, default=None):
+            self.default = default
+            self.values = None
+
+        def option(self, width:int, height:int, depth:int):
+            if self.values is None:
+                self.values = []
+            self.values.append((width, height, depth))
+
+        def render(self):
+            if self.values is None:
+                return self.default
+            return self.values
+
+    @dataclasses.dataclass
+    class ConfigFile:
+        resolutions: Resolutions
+        color:str = ''
+```
+
+Would be able to read this mapping:
+
+```Python
+    d = {
+        'color': 'orange',
+        'resolutions': [
+            {'width': 1280, 'height': 1024, 'depth': 24},
+            {'width': 1600, 'height': 1200, 'depth': 16},
+        ],
+    }
+```
+
+
+### `read_iterable`
+
+In addition to Appeal's `read_mapping` method, Appeal
+also supports a `read_iterable` method.  The API is
+almost identical:
+
+```Python
+    Appeal.read_iterable(callable, iterable)
+```
+
+However this function is much simpler.  The iterable
+should itself be an iterable of iterables.  Appeal will
+call the callable you specify once for every nested
+iterable.  The result will be appended to a list, and
+`read_iterable` will return that list.
+
+As always, Appeal will handle converting values using
+the annotations you specify.  Unlike `read_mapping`,
+here you may pass in a function accepting `*args`,
+in which case Appeal will process an arbitrary number
+of trailing arguments.  Also unlike `read_mapping`,
+there's no support for testing--neither nested dictionaties
+nor (further) nested lists.  (Like when processing the
+command-line, when reading values from the iterable,
+nested annotations get flattened.)
+
+### CSV files
+
+Finally, Appeal has special support for reading CSV files.  This may
+seem like an odd thing to support--nobody uses CSV files as config
+files.  But CSV files were the proof-of-concept for Appeal's config
+file support, and it's proved useful in another project, so for
+now it's staying in.  There's a special method for reading CSV
+files:
+
+```Python
+    Appeal.read_csv(self, callable, csv_reader, *, first_row_map=None)
+```
+
+You pass in your callable, and a fresh `csv.reader` object.  Appeal
+will read the rows out of the `CSV` object, passing in the strings into
+the `callable`, and append the result to a list.  The return value is
+that list.
+
+If `first_row_map` is false, `read_csv` will ignore the first line of
+the CSV file (the "column names" line) and pass in the values from the
+CSV file by position.  If `first_row_map` is true, `read_csv` will use
+the rows from the first line of the CSV file as keys in a dictionary,
+populate the values with each subsequent row, and will pass the
+arguments by name.
+
+In other words, if `first_row_map` is false, Appeal calls
+
+```Python
+    callable(*row)
+```
+
+for every line after the first line in the CSV file.  And if `first_row_map`
+is true, Appeal calls
+
+```Python
+    d = {key: value for key, value in zip(column_headers, row)}
+    callable(**d)
+```
+
+for every line after the first line in the CSV file.
+
+
 ## API Reference
 
 `Appeal(help=True, version=None, positional_argument_usage_format="{name}", default_options=default_options)`
 
 Creates a new Appeal instance.
 
 If `help` is true, Appeal automatically adds help support to
@@ -1666,20 +1978,20 @@
 
 Raises `AppealConfigurationError` if any `option` has already been
 mapped inside this `Appeal` instance *with a different signature.*
 
 (Doesn't modify `callable` in any way.)
 
 
-`Appeal.argument(self, parameter_name, *, usage=None)`
+`Appeal.parameter(self, parameter_name, *, usage=None)`
 
 Used as a decorator.  Returns a callable that accepts a single
 parameter `callable`, which must be a callable.
 
-Allos for configuration of a positional (or positional-or-keyword)
+Allows for configuration of a positional (or positional-or-keyword)
 parameter on a command function or converter.  `parameter_name` is the
 name of the parameter; it must be a parameter of the decorated `callable`.
 
 Currently the only supported configuration is `usage`, which specifies
 the string that will represent this parameter in usage information.
 
 (Doesn't modify `callable` in any way.)
@@ -1887,14 +2199,28 @@
   with `appeal.split`.  But it also permits options that consume
   multiple separate opargs from the command-line.
 * POSIX requires that all options be specified before any positional
   arguments.  Appeal doesn't enforce this, and will happily consume
   options and positional arguments in any order.  In fact,
   "subcommands" require permitting options after positional arguments
   for anything beyond the simplest possible subcommand support.
+* POSIX requires that, if an option (short option) has a single
+  *optional* argument (oparg), its argument must be concatenated
+  to the option.  For example, if `-f` takes an optional argument,
+  and you want to specify the argument `guava`, you *must* write
+  this as `-fguava`, no other spelling is permissible.  While Appeal
+  supports this spelling, it also supports `-f=guava` and `-f guava`.
+  More importantly, if you specify `-f` on your command-line (and
+  not `-f=<something>` or `-f<something>`), Appeal *will* consume the
+  next argument on the command-line as an oparg, which is what POSIX
+  definitely does *not* want.  I feel Appeal's consistency is
+  more important than supporting this syntactic hack.  Note that
+  the oparg is still optional, so if `-f` is the last thing
+  on your command-line, that will achieve this "option with
+  default value" behavior.
 
 
 ## Additional Subtle Features And Behaviors
 
 * You can specify options and arguments in any order on a
   command-line, Appeal doesn't care.  If you want Appeal to
   stop recognizing arguments starting with dashes as options,
@@ -1921,15 +2247,15 @@
 * You shouldn't call `usage()` until you've added all the
   commands, options, and parameters information into your
   Appeal object.  Why?  Because, for example, `usage()`
   computes the default options for keyword-only parameters
   that haven't gotten any explicitly defined options.
   But if you then define one of those options, Appeal will
   throw an error at you.
-* Almost any callable can be a converter.  But not every
+* Almost any callable can be a converter--but not *every*
   function.  There are two limitations.  First, as already
   mentioned, in order for a function to be a legal converter,
   every keyword-only parameter must have a default value.
   The second requirement is more specific: in order to use
   a function as a converter for a `*args*` parameter,
   *somewhere* in the annotations tree under that function,
   some function must take a required positional parameter.
@@ -1965,14 +2291,68 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.6**
+
+A huge upgrade!
+
+* A new feature: Appeal can now read configuration files!
+  Check out the new APIs `Appeal.read_mapping`,
+  `Appeal.read_iterable`, and even `Appeal.read_csv`.
+  This was a massive undertaking and involved a big
+  overhaul of the compiler.
+
+* The biggest change to existing behavior: Appeal now
+  early-maps options.  (See issue #3.)
+  In short: when options are only defined in an optional group,
+  they get provisionally mapped (made available) *before* the first
+  argument in that group.  Using that option enters the group just
+  like specifying the first argument in that group.  You'll see
+  the difference in usage; an optional group that mapped an option
+  used to look like `[a [-v|--verbose] b c]` but now looks like
+  `[[-v|--verbose] a b c]`.
+
+* Appeal now handles multiple short options smashed together
+  (e.g. `-ace`) *identically* to them being specified separately
+  (e.g. `-a -c -e`).  This caused an observable change in behavior
+  regarding when child options get unmapped.
+
+  - Appeal only permits using child options in a limited context:
+    it must be after the parent option is executed, it
+    must be after the parent option has consumed all its required
+    *or optional* opargs, and it must be before any top-level
+    positional argument or option mapped before the parent option
+    was executed.  But Appeal was lax about enforcing these rules
+    when using multiple short options smashed together (e.g. `-ace`);
+    it would handle all the options and *then* unmap child options
+    as needed.  The good news: Appeal now enforces these rules here
+    too.  (The old behavior seems to have been *intentional* on my
+    part--what was I *thinking?!)*
+
+* The usage message raised for an unknown option is now much
+  better.  If the option is defined anywhere in the program
+  being run, it prints a different message telling you it
+  can't be used here, but also tells you where it can be used.
+  For example, if you use option `-x`, but that's a child
+  option mapped by `--parent`, the message would say
+  `-x can't be used here, it must be used immediately after --parent`.
+
+* Renamed `Appeal.argument` to `Appeal.parameter`.
+  This was one of those "what was I *thinking?"* moments.
+  The function affects the parameter, not the argument.
+  The old name still works but will be removed before 1.0.
+
+* `short_option_concatenated_oparg` is now more strictly
+  enforced: it's only permitted for short options that have
+  *exactly one* **optional** oparg, as specified by POSIX.
+
 **0.5.9**
 
 * Improved the error message generated when you have a
   required parameter after a `VAR_POSITIONAL` parameter.
   (This command-line can never succeed, because the
   `VAR_POSITIONAL` consumes all remaining arguments on
   the command-line, which means the subsequent required
```

### Comparing `appeal-0.5.9/appeal/__init__.py` & `appeal-0.6/appeal/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.9"
+__version__ = "0.6"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -26,23 +26,25 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-want_prints = 1
+# run appeal/want_prints.py to toggle debug prints on and off
 want_prints = 0
 
 
 from abc import abstractmethod, ABCMeta
+import base64
 import big.all as big
 from big.itertools import PushbackIterator
 import builtins
-import collections
+import collections.abc
+from collections.abc import Iterable, Iterator, Mapping
 import enum
 import functools
 import inspect
 import itertools
 import math
 import os.path
 from os.path import basename
@@ -50,14 +52,16 @@
 import shlex
 import string
 import sys
 import textwrap
 import time
 import types
 
+from collections import defaultdict
+
 try:
     from typing import Annotated
     AnnotatedType = type(Annotated[int, str])
     del Annotated
     def dereference_annotated(annotation):
         if isinstance(annotation, AnnotatedType):
             return annotation.__metadata__[-1]
@@ -75,22 +79,28 @@
 POSITIONAL_ONLY = inspect.Parameter.POSITIONAL_ONLY
 POSITIONAL_OR_KEYWORD = inspect.Parameter.POSITIONAL_OR_KEYWORD
 VAR_POSITIONAL = inspect.Parameter.VAR_POSITIONAL
 KEYWORD_ONLY = inspect.Parameter.KEYWORD_ONLY
 VAR_KEYWORD = inspect.Parameter.VAR_KEYWORD
 empty = inspect.Parameter.empty
 
-try:
-    # new in 3.7
-    from time import monotonic_ns as event_clock
-except ImportError:
-    from time import perf_counter
 
-    def event_clock():
-        return int(perf_counter() * 1000000000.0)
+# new in 3.8
+shlex_join = getattr(shlex, 'join', None)
+if not shlex_join:
+    # note: this doesn't have to be bullet-proof,
+    # we only use it for debug print statements.
+    def shlex_join(split_command):
+        quoted = []
+        for s in split_command:
+            fields = s.split()
+            if len(fields) > 1:
+                s = repr(s)
+            quoted.append(s)
+        return " ".join(quoted)
 
 
 def update_wrapper(wrapped, wrapper):
     """
     update_wrapper() adds a '__wrapped__'
     attribute.  inspect.signature() then
     follows that attribute, which means it
@@ -257,47 +267,47 @@
 
 def partial_rebind_method(partial, placeholder, instance):
     """
     Binds an unbound method curried with a placeholder
     object to an instance and returns the bound method.
 
     All these statements must be true:
-        * "parital" must be a functools.partial() object
+        * "partial" must be a functools.partial() object
           with exactly one curried positional argument
           and zero curried keyword arguments.
         * The one curried positional argument must be
           equal to "placeholder".
 
     If any of those statements are false, raises ValueError.
 
     If all those statements are true, this function:
         * extracts the callable from the partial,
-        * uses getattr(self, callable.__name__) to
-          bind callable to self.
+        * uses getattr(instance, callable.__name__) to
+          bind callable to the instance.
     """
     return _partial_rebind(partial, placeholder, instance, True)
 
 def partial_rebind_positional(partial, placeholder, instance):
     """
     Replaces the first positional argument of a
     functools.partial object with a different argument.
 
     All these statements must be true:
-        * "parital" must be a functools.partial() object
+        * "partial" must be a functools.partial() object
           with exactly one curried positional argument
           and zero curried keyword arguments.
         * The one curried positional argument must be
           equal to "placeholder".
 
     If any of those statements are false, raises ValueError.
 
     If all those statements are true, this function:
         * extracts the callable from the partial,
-        * uses getattr(self, callable.__name__) to
-          bind callable to self.
+        * uses getattr(instance, callable.__name__) to
+          bind callable to instance.
     """
     return _partial_rebind(partial, placeholder, instance, False)
 
 
 ##
 ## charm
 ##
@@ -310,99 +320,132 @@
 ##
 
 ## goal with bytecode design:
 ##   * no "if" statements inside implementation of any bytecode
 ##     (sadly, there's one, due to "option" on create_converter)
 ##
 ## the interpreter has registers:
+##    program
+##        the program currently being run.
 ##    ip
 ##        the instruction pointer.  an integer, indexes into "program".
+##    converters
+##        a dict mapping converter "keys" to converters.
+##        a converter "key" is any hashable; conceptually a
+##        converter key represents a specific instance of a
+##        converter being used in the annotation tree.
+##        (if you have two parameters annotated with int_float,
+##        these two instances get different converter keys.)
 ##    converter
-##        a reference to a converter (or None).
-##        the current converter context.
-##        conceptually an indirect register like SP or a segment register,
-##          you index through it to reference things.
-##          specifically:
+##        the current converter context.  a reference to a converter (or None).
+##        conceptually an indirect register like SP or a segment register.
+##        you index through it to interact with the attributes of a converter,
+##        specifically:
 ##              args
 ##                positional arguments, accessed with an index (-1 permitted).
 ##              kwargs
 ##                keyword-only arguments, accessed by name.
 ##          you can directly store str arguments in these attributes.
 ##          or, create converters and store (and possibly later retrieve)
 ##          converter objects in these attributes.
 ##    o
-##        a reference to a converter, a string, or None.
 ##        a general-purpose register.
-##        contains the result of create_converter, pop_converter,
-##         consume_argument, and load_converter.
-##    total
-##        argument counter object (or None).
-##        argument counts for this entire command function (so far).
+##        a reference to a converter, a string, or None.
+##    flag
+##        a boolean register.
+##        contains the result of o_is_* instructions.
 ##    group
 ##        argument counter object (or None).
 ##        local argument counts just for this argument group.
+##    iterator
+##        An iterator yielding objects (e.g. strings from the command-line).
+##        You can get the next object using next_to_o.
+##        There's also an iterator_stack, and you can push new iterators
+##        (e.g. to iterate over a list from a Perky file).
+##    mapping
+##        A dict-like object mapping strings to value.
+##        You can get a value with lookup_to_o.
 ##
-## the interpreter has a stack.  it's used to push/pop all registers
-## except ip (which is pushed/popped separately).
+## the interpreter has a stack.  it's used to push/pop registers
+## when making a "call".
 
 
 ## argument counter objects have these fields:
-##    count = how many arguments we've consumed
+##    count = how many arguments we've added to this group
 ##    minimum = the minimum "arguments" needed
 ##    maximum = the maximum "arguments" permissible
+##    optional = flag, is this an optional group?
+##    laden = flag, has anything
 
-class ArgumentCounter:
-    def __init__(self, minimum=0, maximum=0, optional=True):
-        self.minimum = minimum
-        self.maximum = maximum
-        self.count = 0
-        self.optional = optional
-
-    def satisfied(self):
-        return self.minimum <= self.count <= self.maximum
-
-    def __repr__(self):
-        return f"<ArgumentCounter optional={self.optional} minimum {self.minimum} <= count {self.count} <= maximum {self.maximum} == {bool(self)}>"
-
-    def copy(self):
-        return ArgumentCounter(self.minimum, self.maximum, self.optional)
-
-    def summary(self):
-        ok_no = "(ok)" if self.satisfied() else "(no)"
-        optional = "yes" if self.optional else "no"
-        return f"[optional {optional} min {self.minimum} <= cur {self.count} <= max {self.maximum} {ok_no}]"
+def serial_number_generator(*, prefix='', width=0, tuple=False):
+    """
+    Flexible serial number generator.
+    """
 
+    i = 1
+    # yield prefix + base64.b32hexencode(i.to_bytes(5, 'big')).decode('ascii').lower().lstrip('0').rjust(3, '0')
 
-class CharmProgram:
+    if tuple:
+        # if prefix isn't a conventional iterable
+        if not isinstance(prefix, (builtins.tuple, list)):
+            while True:
+                # yield 2-tuple
+                yield (prefix, i)
+                i += 1
+        # yield n-tuple starting with prefix and appending i
+        prefix = list(prefix)
+        prefix.append(0)
+        while True:
+            prefix[-1] = i
+            yield tuple(prefix)
+            i += 1
 
-    id_counter = 1
+    if width:
+        while True:
+            yield f"{prefix}{i:0{width}}"
+            i += 1
 
-    def __init__(self, name=None, minimum=0, maximum=0):
-        self.name = name
+    while True:
+        yield f"{prefix}{i}"
+        i += 1
 
-        self.id = CharmProgram.id_counter
-        CharmProgram.id_counter += 1
+class ArgumentGroup:
+    next_serial_number = serial_number_generator(prefix="ag-").__next__
 
-        self.opcodes = []
+    def __init__(self, *, id=None, optional=True):
+        if id is None:
+            id = ArgumentGroup.next_serial_number()
+        self.id = id
+        self.optional = optional
+        self.minimum = self.maximum = self.count = 0
+        # a flag you should set when you trigger
+        # an option in this group
+        self.laden = False
 
-        self.total = ArgumentCounter(minimum, maximum, False)
-        self.converter_key = 0
+    def satisfied(self):
+        if self.optional and (not (self.laden or self.count)):
+            return True
+        return self.minimum <= self.count <= self.maximum
 
     def __repr__(self):
-        s = f" {self.name!r}" if self.name else ""
-        return f"<CharmProgram {self.id:02}{s}>"
-
-    def __len__(self):
-        return len(self.opcodes)
+        return f"<ArgumentGroup {self.id} optional={self.optional} laden={self.laden} minimum {self.minimum} <= count {self.count} <= maximum {self.maximum} == {bool(self)}>"
 
-    def __iter__(self):
-        return iter(self.opcodes)
+    def copy(self):
+        o = ArgumentGroup(id=self.id, optional=self.optional)
+        o.minimum = self.minimum
+        o.maximum = self.maximum
+        o.count = self.count
+        o.laden = self.laden
+        return o
 
-    def __getitem__(self, index):
-        return self.opcodes[index]
+    def summary(self):
+        satisfied = "yes" if self.satisfied() else "no "
+        optional = "yes" if self.optional else "no "
+        laden = "yes" if self.laden else "no "
+        return f"['{self.id}' satisfied {satisfied} | optional {optional} | laden {laden} | min {self.minimum} <= cur {self.count} <= max {self.maximum}]"
 
 
 
 """
 # cpp
 
 # This is a preprocessor block.
@@ -413,86 +456,136 @@
         print(f"    {name.strip()} = {i}")
         i += 1
 
 print('class opcode(enum.Enum):')
 
 print_enum('''
     invalid
+    end
+    abort
     jump
-    branch_on_o
+    indirect_jump
+    branch_on_flag
+    branch_on_not_flag
+    literal_to_o
+    wrap_o_with_iterator
+    test_is_o_true
+    test_is_o_none
+    test_is_o_empty
+    test_is_o_iterable
+    test_is_o_mapping
+    test_is_o_str_or_bytes
     call
     create_converter
     load_converter
     load_o
-    append_args
-    store_kwargs
+    converter_to_o
+    push_o
+    pop_o
+    peek_o
+    push_flag
+    pop_flag
+    push_mapping
+    pop_mapping
+    push_iterator
+    pushback_o_to_iterator
+    pop_iterator
+    append_to_converter_args
+    set_in_converter_kwargs
     map_option
-    consume_argument
+    next_to_o
+    lookup_to_o
     flush_multioption
+    remember_converters
+    forget_converters
     set_group
-    push_context
-    pop_context
-    end
 
 ''')
 
 print('''
     # these are removed by the peephole optimizer.
     # the interpreter never sees them.
     # (well... unless you leave in comments during debugging.)
 ''')
 
 print_enum('''
     no_op
     comment
     label
     jump_to_label
-    branch_on_o_to_label
-''', i=100)
+    branch_on_flag_to_label
+    branch_on_not_flag_to_label
+    label_to_o
+''', i=200)
 
 print()
 
 """
 
 # Don't modify this stuff directly!
 # Everything from here to the
 #         # cpp
 # line below is generated.
 #
 # Modify the code in the quotes above and run
-#         % python3 cpp.py __init__.py
+#         % python3 cpp.py appeal/__init__.py
 # to regenerate.
 
 class opcode(enum.Enum):
     invalid = 0
-    jump = 1
-    branch_on_o = 2
-    call = 3
-    create_converter = 4
-    load_converter = 5
-    load_o = 6
-    append_args = 7
-    store_kwargs = 8
-    map_option = 9
-    consume_argument = 10
-    flush_multioption = 11
-    set_group = 12
-    push_context = 13
-    pop_context = 14
-    end = 15
+    end = 1
+    abort = 2
+    jump = 3
+    indirect_jump = 4
+    branch_on_flag = 5
+    branch_on_not_flag = 6
+    literal_to_o = 7
+    wrap_o_with_iterator = 8
+    test_is_o_true = 9
+    test_is_o_none = 10
+    test_is_o_empty = 11
+    test_is_o_iterable = 12
+    test_is_o_mapping = 13
+    test_is_o_str_or_bytes = 14
+    call = 15
+    create_converter = 16
+    load_converter = 17
+    load_o = 18
+    converter_to_o = 19
+    push_o = 20
+    pop_o = 21
+    peek_o = 22
+    push_flag = 23
+    pop_flag = 24
+    push_mapping = 25
+    pop_mapping = 26
+    push_iterator = 27
+    pushback_o_to_iterator = 28
+    pop_iterator = 29
+    append_to_converter_args = 30
+    set_in_converter_kwargs = 31
+    map_option = 32
+    next_to_o = 33
+    lookup_to_o = 34
+    flush_multioption = 35
+    remember_converters = 36
+    forget_converters = 37
+    set_group = 38
 
     # these are removed by the peephole optimizer.
     # the interpreter never sees them.
     # (well... unless you leave in comments during debugging.)
 
-    no_op = 100
-    comment = 101
-    label = 102
-    jump_to_label = 103
-    branch_on_o_to_label = 104
+    no_op = 200
+    comment = 201
+    label = 202
+    jump_to_label = 203
+    branch_on_flag_to_label = 204
+    branch_on_not_flag_to_label = 205
+    label_to_o = 206
 
 # cpp
 
 
 class CharmInstruction:
     __slots__ = ['op']
 
@@ -515,15 +608,48 @@
 
 class CharmInstructionNoOp(CharmInstruction): # CharmInstructionNoArgBase
 
     def __init__(self):
         self.op = opcode.no_op
 
     def __repr__(self):
-        return f"<no-op>"
+        return f"<no_op>"
+
+
+class CharmInstructionEnd(CharmInstruction):
+    """
+    end
+
+    Exits the current program.
+    """
+
+    __slots__ = ['name', 'id']
+
+    def __init__(self):
+        self.op = opcode.end
+
+    def __repr__(self):
+        return f"<end>"
+
+
+class CharmInstructionAbort(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    abort
+
+    Aborts processing with an error.
+    """
+
+    __slots__ = ['message']
+
+    def __init__(self, message):
+        self.op = opcode.abort
+        self.message = message
+
+    def __repr__(self):
+        return f"<abort>"
 
 
 class CharmInstructionJump(CharmInstruction): # CharmInstructionAddressBase
     """
     jump <address>
 
     Sets the 'ip' register to <address>.
@@ -536,34 +662,210 @@
         self.op = opcode.jump
         self.address = address
 
     def __repr__(self):
         return f"<jump address={self.address}>"
 
 
-class CharmInstructionBranchOnO(CharmInstruction): # CharmInstructionAddressBase
+class CharmInstructionIndirectJump(CharmInstruction): # CharmInstructionAddressBase
+    """
+    indirect_jump
+
+    Sets the 'ip' register to the value in the 'o' register.
+    The value must be an integer.
+    """
+
+    def __init__(self):
+        self.op = opcode.indirect_jump
+
+    def __repr__(self):
+        return f"<indirect_jump>"
+
+
+class CharmInstructionBranchOnFlag(CharmInstruction): # CharmInstructionAddressBase
+    """
+    branch_on_flag <address>
+
+    If the 'flag' register is True,
+    sets the 'ip' register to <address>.
+    <address> is an integer.
+    """
+
+    __slots__ = ['address']
+
+    def __init__(self, address):
+        self.op = opcode.branch_on_flag
+        self.address = address
+
+    def __repr__(self):
+        return f"<branch_on_flag address={self.address}>"
+
+class CharmInstructionBranchOnNotFlag(CharmInstruction): # CharmInstructionAddressBase
     """
-    branch_on_o <address>
+    branch_on_not_flag <address>
 
-    If the 'o' register is a true value,
+    If the 'flag' register is False,
     sets the 'ip' register to <address>.
     <address> is an integer.
     """
 
     __slots__ = ['address']
 
     def __init__(self, address):
-        self.op = opcode.branch_on_o
+        self.op = opcode.branch_on_not_flag
         self.address = address
 
     def __repr__(self):
-        return f"<branch_on_o address={self.address}>"
+        return f"<branch_on_not_flag address={self.address}>"
+
+class CharmInstructionLiteralToO(CharmInstruction): # CharmInstructionAddressBase
+    """
+    literal_to_o
+
+    Sets the 'o' register to a precompiled literal value.
+    """
+
+    __slots__ = ['value']
+
+    def __init__(self, value):
+        self.op = opcode.literal_to_o
+        self.value = value
+
+    def __repr__(self):
+        return f"<literal_to_o value={repr(self.value)}>"
+
+class CharmInstructionWrapOWithIterator(CharmInstruction): # CharmInstructionAddressBase
+    """
+    wrap_o_with_iterator
+
+    Replaces the value in the 'o' register with an iterator
+    which yields that value.
+
+    In other words:
+        o = iter( (o,) )
+    """
+
+    def __init__(self):
+        self.op = opcode.wrap_o_with_iterator
+
+    def __repr__(self):
+        return f"<wrap_o_with_iterator>"
+
+class CharmInstructionTestIsOTrue(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_true
+
+    If the 'o' register contains a true value,
+    set the 'flag' register to True,
+    otherwise set the 'flag' register to False.
+
+    In other words:
+        flag = bool(o)
+    """
+
+    def __init__(self):
+        self.op = opcode.test_is_o_true
+
+    def __repr__(self):
+        return f"<test_is_o_true>"
+
+class CharmInstructionTestIsONone(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_none
+
+    If the 'o' register contains None,
+    set the 'flag' register to True,
+    otherwise set the 'flag' register to False.
+
+    In other words:
+        flag = o == None
+    """
+
+    def __init__(self):
+        self.op = opcode.test_is_o_none
+
+    def __repr__(self):
+        return f"<test_is_o_none>"
+
+class CharmInstructionTestIsOEmpty(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_empty
+
+    If the 'o' register contains inspect.Parameter.Empty,
+    set the 'flag' register to True,
+    otherwise set the 'flag' register to False.
+
+    In other words:
+        flag = o == inspect.Parameter.empty
+    """
+
+    def __init__(self):
+        self.op = opcode.test_is_o_empty
+
+    def __repr__(self):
+        return f"<test_is_o_empty>"
+
+class CharmInstructionTestIsOIterable(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_iterable
+
+    If the 'o' register contains an instance
+    of an collections.abc.Iterable object, set the 'flag'
+    register to True, otherwise set it to False.
+
+    In other words:
+        flag = isinstance(o, collections.abc.Iterable)
+
+    Note that str objects and most Mapping objects (e.g. dict)
+    are iterable.  You may want to test for those first.
+    """
+
+    def __init__(self):
+        self.op = opcode.test_is_o_iterable
+
+    def __repr__(self):
+        return f"<test_is_o_iterable>"
+
+class CharmInstructionTestIsOMapping(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_mapping
+
+    If the 'o' register contains an instance
+    of an collections.abc.Mapping object, set the 'flag'
+    register to True, otherwise set it to False.
+
+    In other words:
+        flag = isinstance(o, collections.abc.Mapping)
+    """
+
+    def __init__(self):
+        self.op = opcode.test_is_o_mapping
+
+    def __repr__(self):
+        return f"<test_is_o_mapping>"
+
+class CharmInstructionTestIsOStrOrBytes(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    test_is_o_str_or_bytes
+
+    If the 'o' register contains an instance
+    of a str or bytes object, set the 'flag'
+    register to True, otherwise set it to False.
+
+    In other words:
+        flag = isinstance(o, (str, bytes))
+    """
 
+    def __init__(self):
+        self.op = opcode.test_is_o_str_or_bytes
 
-label_id_counter = 0
+    def __repr__(self):
+        return f"<test_is_o_str_or_bytes>"
+
+next_label_id = serial_number_generator(prefix='label-').__next__
 
 class CharmInstructionLabel(CharmInstruction):
     """
     label <name>
 
     Sets a destination in the program that can be
     jumped to by the jump_to_label instruction.
@@ -574,27 +876,24 @@
 
     label and *_to_label are both pseudo-instructions.
     They're removed by a pass in the peephole optimizer.
     """
     __slots__ = ['id', 'label']
 
     def __init__(self, label):
-        global label_id_counter
         self.op = opcode.label
-        label_id_counter += 1
-        self.id = label_id_counter
+        self.id = next_label_id()
         self.label = label
 
     def __repr__(self):
-        opcode = str(self.op).rpartition('.')[2]
         label = f" label={self.label!r}" if self.label else ""
-        return f"<{opcode} id={self.id}{label}>"
+        return f"<label id={self.id}{label}>"
 
     def __hash__(self):
-        return id(CharmInstructionLabel) ^ self.id
+        return hash(self.id)
 
 class CharmInstructionJumpToLabel(CharmInstruction): # CharmInstructionLabelBase
     """
     jump_to_label <label>
 
     Sets the 'ip' register to point to the instruction
     after the instance of the <label> instruction in the
@@ -608,40 +907,81 @@
 
     def __init__(self, label):
         self.op = opcode.jump_to_label
         self.label = label
 
     def __repr__(self):
         label = f" label={self.label!r}" if self.label else ""
-        return f"<jump-to-label {label}>"
+        return f"<jump_to_label{label}>"
 
 
-class CharmInstructionBranchOnOToLabel(CharmInstruction):
+class CharmInstructionBranchOnFlagToLabel(CharmInstruction):
     """
-    branch_on_o_to_label <label>
+    branch_on_flag_to_label <label>
 
-    If the 'o' register is a true value,
+    If the 'flag' register is True,
     sets the 'ip' register to point to the instruction
     after the instance of the <label> instruction in the
     current program.
 
     label and *_to_label are both pseudo-instructions.
     They're removed by a pass in the peephole optimizer.
     """
 
     __slots__ = ['label']
 
     def __init__(self, label):
-        self.op = opcode.branch_on_o_to_label
+        self.op = opcode.branch_on_flag_to_label
         self.label = label
 
     def __repr__(self):
         label = f" label={self.label!r}" if self.label else ""
-        return f"<branch-on-o-to-label {label}>"
+        return f"<branch_on_flag_to_label {label}>"
+
+
+class CharmInstructionBranchOnNotFlagToLabel(CharmInstruction):
+    """
+    branch_on_not_flag_to_label <label>
+
+    If the 'flag' register is False,
+    sets the 'ip' register to point to the instruction
+    after the instance of the <label> instruction in the
+    current program.
+
+    label and *_to_label are both pseudo-instructions.
+    They're removed by a pass in the peephole optimizer.
+    """
 
+    __slots__ = ['label']
+
+    def __init__(self, label):
+        self.op = opcode.branch_on_not_flag_to_label
+        self.label = label
+
+    def __repr__(self):
+        label = f" label={self.label!r}" if self.label else ""
+        return f"<branch_on_not_flag_to_label {label}>"
+
+class CharmInstructionLabelToO(CharmInstruction): # CharmInstructionAddressBase
+    """
+    label_to_o
+
+    Sets the 'o' register to the address of a label.
+    Is converted by the assembler into a literal_to_o instruction.
+    """
+
+    __slots__ = ['label']
+
+    def __init__(self, label):
+        self.op = opcode.label_to_o
+        self.label = label
+
+    def __repr__(self):
+        label = f" label={self.label!r}" if self.label else ""
+        return f"<label_to_o {label}>"
 
 class CharmInstructionCreateConverter(CharmInstruction):
     """
     create_converter <parameter> <key>
 
     Creates a Converter object using <parameter>,
     an inspect.Parameter object.
@@ -653,15 +993,15 @@
 
     def __init__(self, parameter, key):
         self.op = opcode.create_converter
         self.parameter = parameter
         self.key = key
 
     def __repr__(self):
-        return f"<create_converter parameter={parameter!r} key={self.key}>"
+        return f"<create_converter parameter={self.parameter!r} key={self.key}>"
 
 class CharmInstructionLoadConverter(CharmInstruction): # CharmInstructionKeyBase
     """
     load_converter <key>
 
     Loads a Converter object from 'converters[key]' and
     stores a reference in the 'converter' register.
@@ -687,149 +1027,362 @@
     __slots__ = ['key']
 
     def __init__(self, key):
         self.op = opcode.load_o
         self.key = key
 
     def __repr__(self):
-        return f"<load_converter key={self.key}>"
+        return f"<load_o key={self.key}>"
 
-class CharmInstructionAppendArgs(CharmInstruction):
+class CharmInstructionConverterToO(CharmInstruction): # CharmInstructionKeyBase
     """
-    append_args <parameter> <usage>
+    converter_to_o
+
+    Sets the 'o' register to the contents of the 'converter'
+    register.
+    """
+    def __init__(self):
+        self.op = opcode.converter_to_o
+
+    def __repr__(self):
+        return f"<converter_to_o>"
+
+class CharmInstructionAppendToConverterArgs(CharmInstruction):
+    """
+    append_to_converter_args <parameter> <discretionary> <usage>
 
     Takes a reference to the value in the 'o' register
     and appends it to 'converter.args'.
 
-    <callable> is a callable object.
-    <parameter> and <usage> are strings identifying
-    the name of the parameter.  These are all used in
-    generating usage information and documentation.
+    <parameter> is an inspect.Parameter representing
+    the positional parameter being filled here.
+    It's used to generate usage.
+
+    <discretionary> is a boolean value.
+    If True, this argument may or may not be used,
+    depending on what values we process at runtime.
+    If False, this argument is mandatory.
+
+    <usage> is a 2-tuple:
+        (usage_full_name, usage_name)
+    usage_full_name is a string of the form:
+        "{callable}.{parameter_name}"
+    This is the actual name of the parameter from
+    the actual callable.
+
+    usage_name is a string, the name of the
+    parameter as it should appear in usage documentation.
     """
 
-    __slots__ = ['callable', 'parameter', 'usage', 'usage_callable', 'usage_parameter']
+    __slots__ = ['parameter', 'discretionary', 'usage']
 
-    def __init__(self, callable, parameter, usage, usage_callable, usage_parameter):
-        self.op = opcode.append_args
-        self.callable = callable
+    def __init__(self, parameter, discretionary, usage):
+        self.op = opcode.append_to_converter_args
         self.parameter = parameter
+        self.discretionary = discretionary
         self.usage = usage
-        self.usage_callable = usage_callable
-        self.usage_parameter = usage_parameter
 
     def __repr__(self):
-        return f"<append_args callable={self.callable} parameter={self.parameter} usage={self.usage} usage_callable={self.usage_callable} usage_parameter={self.usage_parameter}>"
+        return f"<append_to_converter_args parameter={self.parameter} discretionary={self.discretionary} usage={self.usage}>"
 
-class CharmInstructionStoreKwargs(CharmInstruction):
+class CharmInstructionSetInConverterKwargs(CharmInstruction):
     """
-    store_kwargs <name>
+    set_in_converter_kwargs <name>
 
     Takes a reference to the object currently in
     the 'o' register and stores it in 'converter.kwargs[<name>]'.
     (Here 'converter' is the 'converter' register.)
 
     <name> is a string.
     """
 
     __slots__ = ['name']
 
     def __init__(self, name):
-        self.op = opcode.store_kwargs
+        self.op = opcode.set_in_converter_kwargs
         self.name = name
 
     def __repr__(self):
-        return f"<store_kwargs name={self.name}>"
+        return f"<set_in_converter_kwargs name={self.name}>"
+
+class CharmInstructionPushO(CharmInstruction):
+    """
+    push_o
+
+    Pushes the value currently in the 'o' register
+    onto to the 'data' stack.
+    """
+
+    def __init__(self):
+        self.op = opcode.push_o
+
+    def __repr__(self):
+        return f"<push_o>"
+
+class CharmInstructionPopO(CharmInstruction):
+    """
+    pop_o
+
+    Pops the top value from the 'data' stack and
+    sets it as the value of 'o''.
+
+    If the 'data' stack is empty,
+    you must abort processing and produce an error.
+    """
+
+    def __init__(self):
+        self.op = opcode.pop_o
+
+    def __repr__(self):
+        return f"<pop_o>"
+
+class CharmInstructionPeekO(CharmInstruction):
+    """
+    peek_o
+
+    Gets the top value from the 'data' stack (without popping)
+    and sets it as the value of 'o'.
+
+    If the 'data' stack is empty,
+    you must abort processing and produce an error.
+    """
+
+    def __init__(self):
+        self.op = opcode.peek_o
+
+    def __repr__(self):
+        return f"<peek_o>"
+
+class CharmInstructionPushFlag(CharmInstruction):
+    """
+    push_o
+
+    Pushes the value currently in the 'flag' register
+    onto to the 'data' stack.
+    """
+
+    def __init__(self):
+        self.op = opcode.push_flag
+
+    def __repr__(self):
+        return f"<push_flag>"
+
+class CharmInstructionPopFlag(CharmInstruction):
+    """
+    pop_o
+
+    Pops the top value from the 'data' stack and
+    sets it as the value of 'flag'.
+
+    If the 'data' stack is empty,
+    you must abort processing and produce an error.
+    """
+
+    def __init__(self):
+        self.op = opcode.pop_flag
+
+    def __repr__(self):
+        return f"<pop_flag>"
 
-class CharmInstructionPushContext(CharmInstruction): # CharmInstructionNoArgBase
+class CharmInstructionPushMapping(CharmInstruction):
     """
-    push_context
+    push_mapping
 
-    Pushes the current 'converter', 'group', 'o', 'option',
-    and 'total' registers on the stack.
+    Pushes the current mapping dict onto the mapping
+    stack, then takes a reference to the object currently
+    in the 'o' register and sets it as the new mapping dict.
+
+    If 'o' is not isinstance(o, collections.abc.Mapping)
+    you must abort processing and produce an error.
     """
+
     def __init__(self):
-        self.op = opcode.push_context
+        self.op = opcode.push_mapping
 
     def __repr__(self):
-        return f"<push_context>"
+        return f"<push_mapping>"
 
-class CharmInstructionPopContext(CharmInstruction): # CharmInstructionNoArgBase
+class CharmInstructionPopMapping(CharmInstruction):
     """
-    pop_context
+    pop_mapping
+
+    Pops the top value from the mapping stack and
+    sets it as the current mapping dict, overwriting
+    the reference to the current mapping dict.
 
-    Pops the top value from the stack, restoring
-    the previous values of the 'converter', 'group',
-    'o', 'option', and 'total' registers.
+    If the mapping stack is empty,
+    you must abort processing and produce an error.
     """
+
     def __init__(self):
-        self.op = opcode.pop_context
+        self.op = opcode.pop_mapping
 
     def __repr__(self):
-        return f"<pop_context>"
+        return f"<pop_mapping>"
+
+class CharmInstructionPushIterator(CharmInstruction):
+    """
+    push_iterator
+
+    Pushes the current iterator onto the iterator stack,
+    then takes a reference to the object currently in the
+    'o' register and sets it as the new iterator.
+
+    If 'o' is not isinstance(o, collections.abc.Iterator)
+    you must abort processing and produce an error.
+    """
+
+    def __init__(self):
+        self.op = opcode.push_iterator
+
+    def __repr__(self):
+        return f"<push_iterator>"
+
+class CharmInstructionPushbackOToIterator(CharmInstruction):
+    """
+    pushback_o_to_iterator
+
+    Pushes the value in the 'o' register back on the
+    iterator.
+    """
+
+    def __init__(self):
+        self.op = opcode.pushback_o_to_iterator
+
+    def __repr__(self):
+        return f"<pushback_o_to_iterator>"
+
+class CharmInstructionPopIterator(CharmInstruction):
+    """
+    pop_iterator
+
+    Pops the top value from the iterator stack and
+    sets it as the current iterator, overwriting
+    the reference to the current iterator.
+
+    If the iterator stack is empty,
+    you must abort processing and produce an error.
+    """
+
+    def __init__(self):
+        self.op = opcode.pop_iterator
+
+    def __repr__(self):
+        return f"<pop_iterator>"
 
 class CharmInstructionMapOption(CharmInstruction):
     """
-    map_option <option> <program> <callable> <parameter> <key>
+    map_option <group> <option> <program> <key> <parameter>
 
     Maps the option <option> to the program <program>.
 
+    <group> is the id of the ArgumentGroup this is mapped in.
+
     <program> is self-contained; if the option is invoked
-    on the command-line, you may simply 'push' the new
-    program on your current CharmInterpreter.
+    on the command-line, you may run it with
+    CharmInterpreter.call(program).
 
     <key> and <parameter> are used in generating
     usage information.  <key> is the converter key
-    for the converter, and <parameter> is the
-    parameter on that converter, that this option
-    maps to.
+    for the converter (callable) which accepts a keyword-only
+    parameter that will be filled by this option,
+    and <parameter> is the keyword-only
+    parameter accepted by that converter which this
+    option fills.  (The value returned by this program
+    becomes the argument for <parameter> when calling
+    the callable in <parameter.annotation>.)
     """
-    __slots__ = ['option', 'program', 'callable', 'parameter', 'key']
+    __slots__ = ['option', 'program', 'key', 'parameter', 'group']
 
-    def __init__(self, option, program, callable, parameter, key):
+    def __init__(self, group, option, program, key, parameter):
         self.op = opcode.map_option
+        self.group = group
         self.option = option
         self.program = program
-        self.callable = callable
-        self.parameter = parameter
         self.key = key
+        self.parameter = parameter
 
     def __repr__(self):
-        return f"<map_option option={self.option!r} program={self.program} key={self.key} parameter={self.parameter} key={self.key}>"
+        return f"<map_option option={self.option!r} program={self.program} key={self.key} parameter={self.parameter} key={self.key} group={self.group}>"
 
-class CharmInstructionConsumeArgument(CharmInstruction):
+class CharmInstructionNextToO(CharmInstruction):
     """
-    consume_argument <is_oparg>
+    next_to_o <required> <is_oparg>
 
-    Consumes an argument from the command-line,
-    and stores it in the 'o' register.
+    Consume the next value from the iterator
+    and store it in the 'o' register.
 
     <is_oparg> is a boolean flag:
-        * If <is_oparg> is True, you are consuming an oparg.
+        * If <is_oparg> is True, you're consuming an oparg.
           You should consume the next command-line argument
           no matter what it is--even if it starts with a
           dash, which would normally indicate a command-line
           option.
-        * If <is_oparg> is False, you are consuming a top-level
+        * If <is_oparg> is False, you're consuming a top-level
           command-line positional argument.  You should process
           command-line arguments normally, including
           processing options.  Continue processing until
           you find a command-line argument that isn't
           an option, nor is consumed by any options that
           you might have encountered while processing,
           and then consume that argument to satisfy this
           instruction.
-    """
-    __slots__ = ['is_oparg']
 
-    def __init__(self, is_oparg):
-        self.op = opcode.consume_argument
+    <required> is also a boolean flag, and is only considered
+    when the iterator is exhausted.
+        * If <required> is True, this argument is required.
+          If the iterator is exhausted, abort processing and
+          raise a usage exception.
+        * If <required> is False, this argument isn't
+          required.  If the iterator is exhausted, 'o'
+          is set to None and 'flag' to False.
+
+    'flag' is set to True if this consumed a value and set
+    it in the 'o' register, and False if it did not (and
+    <required> is false).
+    """
+    __slots__ = ['required', 'is_oparg']
+
+    def __init__(self, required, is_oparg):
+        self.op = opcode.next_to_o
+        self.required = required
         self.is_oparg = is_oparg
 
     def __repr__(self):
-        return f"<consume_argument is_oparg={self.is_oparg}>"
+        return f"<next_to_o required={self.required} is_oparg={self.is_oparg}>"
+
+class CharmInstructionLookupToO(CharmInstruction):
+    """
+    lookup_to_o <key> <required>
+
+    Retrieves the value named <key> from the mapping
+    and stores it in the 'o' register.
+
+    <key> is the key used to look up the value.
+
+    <required> is a boolean flag:
+        * If <required> is True, this value is required.
+          If <key> is not currently mapped, you must abort
+          processing and raise a usage exception.
+        * If <required> is False, this value isn't
+          required.  'o' will be set to empty.
+
+    'flag' is set to True if the lookup succeeded,
+    and False if the lookup failed (and <required> is false).
+    """
+    __slots__ = ['key', 'required']
+
+    def __init__(self, key, required):
+        self.op = opcode.lookup_to_o
+        self.key = key
+        self.required = required
+
+    def __repr__(self):
+        return f"<lookup_to_o key={self.key} required={self.required}>"
+
 
 class CharmInstructionFlushMultioption(CharmInstruction): # CharmInstructionNoArgBase
     """
     flush_multioption
 
     Calls the flush() method on the object stored in
     the 'o' register.
@@ -837,444 +1390,1352 @@
 
     def __init__(self):
         self.op = opcode.flush_multioption
 
     def __repr__(self):
         return f"<flush_multioption>"
 
+class CharmInstructionRememberConverters(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    remember_converters
+
+    Start tracking the converters created from this
+    point forward, until flush_mulitoption is invoked.
+
+    A bit of a hack--a bugfix for a design flaw.
+    The problem is with MappingCompiler: when you flush a
+    multioption, we should start fresh and recreate
+    all its child converters.  Most of the time we'll
+    create fresh converters automatically.  But if a child
+    converter is also a multioption, the bytecode we
+    generate detects whether or not the converter already
+    exists.
+
+    The correct fix for this will probably involve maintaining
+    a converter *stack*.  Either that, or, make MappingCompiler
+    use separate programs for multioptions, like AppealCompiler
+    does.
+    """
+
+    def __init__(self):
+        self.op = opcode.remember_converters
+
+    def __repr__(self):
+        return f"<remember_converters>"
+
+
+class CharmInstructionForgetConverters(CharmInstruction): # CharmInstructionNoArgBase
+    """
+    forget_converters
+
+    "forget" all remembered
+    converters--delete them from "converters".
+    """
+
+    def __init__(self):
+        self.op = opcode.forget_converters
+
+    def __repr__(self):
+        return f"<forget_converters>"
 
 class CharmInstructionSetGroup(CharmInstruction):
     """
-    set_group <minimum> <maximum> <optional> <repeating>
+    set_group <id> <minimum> <maximum> <optional> <repeating>
 
     Indicates that the program has entered a new argument
     group, and specifies the minimum and maximum arguments
     accepted by that group.  These numbers are stored as
     an ArgumentCount object in the 'group' register.
     """
 
-    __slots__ = ['group', 'optional', 'repeating']
+    __slots__ = ['group', 'id', 'optional', 'repeating']
 
-    def __init__(self, minimum, maximum, optional, repeating):
+    def __init__(self, id, optional, repeating):
         self.op = opcode.set_group
-        self.group = ArgumentCounter(minimum, maximum, optional)
+        self.group = ArgumentGroup(optional=optional, id=id)
+        self.id = id
         self.optional = optional
         self.repeating = repeating
 
     def __repr__(self):
-        return f"<set_group group={self.group.summary()} optional={self.optional} repeating={self.repeating}>"
+        return f"<set_group id={self.id} group={self.group.summary()} optional={self.optional} repeating={self.repeating}>"
 
-class CharmInstructionEnd(CharmInstruction):
+class CharmProgram:
+
+    next_id = serial_number_generator(prefix="program-").__next__
+
+    def __init__(self, name):
+        self.name = name
+
+        self.id = CharmProgram.next_id()
+
+        self.opcodes = []
+
+        # maps line number to list of comments
+        self.comments = {}
+
+        # same as self.comments, but for labels
+        # (presentation is slightly different)
+        self.labels = {}
+
+        # maps option to its parent option (if any)
+        # used for usage
+        self.options = None
+
+        self.total = ArgumentGroup(optional=False)
+
+    def __repr__(self):
+        s = f" {self.name!r}" if self.name else ""
+        return f"<CharmProgram {self.id}{s} minimum={self.total.minimum} maximum={self.total.maximum}>"
+
+    def __len__(self):
+        return len(self.opcodes)
+
+    def __iter__(self):
+        return iter(self.opcodes)
+
+    def __getitem__(self, index):
+        return self.opcodes[index]
+
+
+class CharmAssembler:
     """
-    end
+    Assembles CharmInstruction objects into a CharmProgram.
+    Has a function call for every instruction; calling
+    the function appends one of those instructions.
+    When you're done assembling, call finalize(), and
+    it will return the finished program.
 
-    Marks the end of a program.  A no-op, exists only
-    to provide some context when reading the trace from
-    a running interpreter.
+    You can also append a CharmAssembler.  That
+    indeed appends the assembler at that point in
+    the stream of instructions, and when it finalizes,
+    it flattens all the CharmAssemblers inline.
+    Every CharmAssembler you appended will be replaced
+    with the instructions appended to it, recursively.
     """
 
-    __slots__ = ['id', 'name']
+    PRESERVE = "_preserve_comment_instructions"
+    STRIP = "_strip_comments_completely"
+    EXTERNAL = "_move_comments_to_external_table"
 
-    def __init__(self, id, name):
-        self.op = opcode.end
-        self.id = id
+
+    next_id = serial_number_generator(prefix="asm-").__next__
+
+    def __init__(self, name=None):
         self.name = name
+        self.id = CharmAssembler.next_id()
+        self.clear()
+
+    def clear(self):
+        self.opcodes = opcodes = []
+        # first entry in contents is there for "spilling names"
+        self.contents = [[], opcodes]
+        self._append_opcode = opcodes.append
+
+        self.option_to_child_options = defaultdict(set)
+        self.option_to_parent_options = defaultdict(set)
 
     def __repr__(self):
-        return f"<end id={self.id} name={self.name!r}>"
+        name = f"name={self.name} " if self.name else ""
+        return f"<CharmAssembler {name}id={self.id}>"
 
+    def append(self, o):
+        if isinstance(o, CharmAssembler):
+            if not len(self.opcodes):
+                opcodes = self.contents.pop()
+            else:
+                self.opcodes = opcodes = []
+                self._append_opcode = opcodes.append
+            self.contents.append(o)
+            self.contents.append(opcodes)
+            return o
+        if isinstance(o, CharmInstruction):
+            self._append_opcode(o)
+            return o
+        raise TypeError('o must be CharmAssembler or CharmInstruction')
 
-class CharmAssembler:
-    def __init__(self, compiler):
-        self.compiler = compiler
-        self.opcodes = []
+    def __len__(self):
+        return sum(len(o) for o in self.contents)
 
-    def append(self, opcode):
-        self.opcodes.append(opcode)
-        return opcode
+    def __bool__(self):
+        return any(self.contents)
+
+    # opcodes
 
-    def extend(self, opcodes):
-        self.opcodes.extend(opcodes)
+    def abort(self, message):
+        op = CharmInstructionAbort(message)
+        self._append_opcode(op)
+        return op
+
+    def end(self):
+        op = CharmInstructionEnd()
+        self._append_opcode(op)
+        return op
 
     def no_op(self):
         op = CharmInstructionNoOp()
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
     def comment(self, comment):
         op = CharmInstructionComment(comment)
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
     def label(self, name):
         op = CharmInstructionLabel(name)
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
     def jump_to_label(self, label):
         op = CharmInstructionJumpToLabel(label)
-        return self.append(op)
+        self._append_opcode(op)
+        return op
+
+    def indirect_jump(self):
+        op = CharmInstructionIndirectJump()
+        self._append_opcode(op)
+        return op
+
+    def literal_to_o(self, value):
+        op = CharmInstructionLiteralToO(value)
+        self._append_opcode(op)
+        return op
+
+    def wrap_o_with_iterator(self):
+        op = CharmInstructionWrapOWithIterator()
+        self._append_opcode(op)
+        return op
+
+    def label_to_o(self, label):
+        op = CharmInstructionLabelToO(label)
+        self._append_opcode(op)
+        return op
 
     def call(self, program):
         op = CharmInstructionCall(program)
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
-    def create_converter(self, parameter):
-        key = self.compiler.program.converter_key
-        self.compiler.program.converter_key += 1
+    def create_converter(self, parameter, key):
         op = CharmInstructionCreateConverter(
             parameter=parameter,
             key=key,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
     def load_converter(self, key):
         op = CharmInstructionLoadConverter(
             key=key,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
     def load_o(self, key):
         op = CharmInstructionLoadO(
             key=key,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
-    def append_args(self, callable, parameter, usage, usage_callable, usage_parameter):
-        op = CharmInstructionAppendArgs(
-            callable = callable,
+    def converter_to_o(self):
+        op = CharmInstructionConverterToO()
+        self._append_opcode(op)
+        return op
+
+    def append_to_converter_args(self, parameter, discretionary, usage):
+        op = CharmInstructionAppendToConverterArgs(
             parameter = parameter,
+            discretionary = discretionary,
             usage = usage,
-            usage_callable = usage_callable,
-            usage_parameter = usage_parameter,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
-    def store_kwargs(self, name):
-        op = CharmInstructionStoreKwargs(
+    def set_in_converter_kwargs(self, name):
+        op = CharmInstructionSetInConverterKwargs(
             name=name,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
+
+    def push_o(self):
+        op = CharmInstructionPushO()
+        self._append_opcode(op)
+        return op
+
+    def pop_o(self):
+        op = CharmInstructionPopO()
+        self._append_opcode(op)
+        return op
+
+    def peek_o(self):
+        op = CharmInstructionPeekO()
+        self._append_opcode(op)
+        return op
+
+    def push_flag(self):
+        op = CharmInstructionPushFlag()
+        self._append_opcode(op)
+        return op
+
+    def pop_flag(self):
+        op = CharmInstructionPopFlag()
+        self._append_opcode(op)
+        return op
+
+    def push_mapping(self):
+        op = CharmInstructionPushMapping()
+        self._append_opcode(op)
+        return op
+
+    def pop_mapping(self):
+        op = CharmInstructionPopMapping()
+        self._append_opcode(op)
+        return op
+
+    def push_iterator(self):
+        op = CharmInstructionPushIterator()
+        self._append_opcode(op)
+        return op
+
+    def pushback_o_to_iterator(self):
+        op = CharmInstructionPushbackOToIterator()
+        self._append_opcode(op)
+        return op
 
-    def push_context(self):
-        op = CharmInstructionPushContext()
-        return self.append(op)
+    def pop_iterator(self):
+        op = CharmInstructionPopIterator()
+        self._append_opcode(op)
+        return op
+
+    def map_option(self, group, option, program, key, parameter):
+        self.option_to_child_options[option].update(program.option_to_child_options)
 
-    def pop_context(self):
-        op = CharmInstructionPopContext()
-        return self.append(op)
+        self.option_to_parent_options.update(program.option_to_parent_options)
+        for child_option in program.option_to_child_options:
+            self.option_to_parent_options[child_option].add(option)
 
-    def map_option(self, option, program, callable, parameter, key):
         op = CharmInstructionMapOption(
+            group = group,
             option = option,
             program = program,
-            callable = callable,
-            parameter = parameter,
             key = key,
+            parameter = parameter,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
 
-    def consume_argument(self, is_oparg=False):
-        op = CharmInstructionConsumeArgument(
+    def next_to_o(self, required=False, is_oparg=False):
+        op = CharmInstructionNextToO(
+            required=required,
             is_oparg=is_oparg,
             )
-        return self.append(op)
+        self._append_opcode(op)
+        return op
+
+    def lookup_to_o(self, key, required=False):
+        op = CharmInstructionLookupToO(
+            key=key,
+            required=required,
+            )
+        self._append_opcode(op)
+        return op
 
     def flush_multioption(self):
         op = CharmInstructionFlushMultioption()
-        return self.append(op)
+        self._append_opcode(op)
+        return op
+
+    def remember_converters(self):
+        op = CharmInstructionRememberConverters()
+        self._append_opcode(op)
+        return op
+
+    def forget_converters(self):
+        op = CharmInstructionForgetConverters()
+        self._append_opcode(op)
+        return op
+
+    def branch_on_flag_to_label(self, label):
+        op = CharmInstructionBranchOnFlagToLabel(label=label)
+        self._append_opcode(op)
+        return op
+
+    def branch_on_not_flag_to_label(self, label):
+        op = CharmInstructionBranchOnNotFlagToLabel(label=label)
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_true(self):
+        op = CharmInstructionTestIsOTrue()
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_none(self):
+        op = CharmInstructionTestIsONone()
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_empty(self):
+        op = CharmInstructionTestIsOEmpty()
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_iterable(self):
+        op = CharmInstructionTestIsOIterable()
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_mapping(self):
+        op = CharmInstructionTestIsOMapping()
+        self._append_opcode(op)
+        return op
+
+    def test_is_o_str_or_bytes(self):
+        op = CharmInstructionTestIsOStrOrBytes()
+        self._append_opcode(op)
+        return op
+
+    def set_group(self, id=None, optional=True, repeating=False):
+        op = CharmInstructionSetGroup(id=id, optional=optional, repeating=repeating)
+        self._append_opcode(op)
+        return op
+
+    def spill_names(self):
+        """
+        Recursively walk the tree of opcodes and assemblers
+        inside self.  If self has *any* opcodes, insert a
+        comment opcode at the front of this assembler's
+        opcode stream.  Also perform these insertions
+        for all the child assemblers.
+        """
+        stack = []
+        def new(assembler):
+            return assembler, iter(assembler.contents), 0
+        def push(assembler, iterator, count):
+            stack.append((assembler, iterator, count))
+        pop = stack.pop
+
+        push(*new(self))
+
+        while stack:
+            assembler, iterator, count = stack.pop()
+
+            for o in iterator:
+                if isinstance(o, list):
+                    count += len(o)
+                    continue
+                push(assembler, iterator, count)
+                push(*new(o))
+                break
+            else:
+                if count:
+                    # spill!
+                    first_opcodes = assembler.contents[0]
+                    assert isinstance(first_opcodes, list)
+                    assert len(first_opcodes) == 0, f"expected first_opcodes to be empty, but it's {first_opcodes}"
+                    first_opcodes.append(CharmInstructionComment(self.name))
+
+
+    def lists(self):
+        for o in self.contents:
+            if isinstance(o, list):
+                yield o
+                continue
+            yield from o.lists()
+
+    def __getitem__(self, index):
+        if not isinstance(index, int):
+            raise TypeError(f"CharmAssembler indices must be integers, not {type(index).__name__}")
+
+        for l in self.lists():
+            length = len(l)
+            if index >= length:
+                index -= length
+                continue
+            return l[index]
+
+        raise IndexError(f"CharmAssembler index out of range")
+
+    def assemble(self, *, comments=EXTERNAL):
+        """
+        Merges all the opcodes and the nested assemblers
+        into a single list, and processes
+
+        * Computes total and group min/max values.
+        * Convert label/jump_to_label pseudo-ops into
+          absolute jump ops (and removes labels).
+        * Handles comment instructions based on the 'comments'
+          argument:
+            * EXTERNAL means delete the instructions, but move
+              the comments themselves into an external table
+              (a la CPython's "lnotab").
+            * STRIP means simply delete the instructions.
+            * PRESERVE means preserve the comments.
+        * Removes no-ops.
+        * Removes redundant load_converter, load_o,
+          and converter_to_o instructions based on
+          rudimentary dataflow analysis.
+        * Simple jump-to-jumps peephole optimizer.
+        """
+
+        self.spill_names()
+
+        opcodes = []
+        for sublist in self.lists():
+            opcodes.extend(sublist)
+
+        if not (opcodes and (opcodes[-1].op == opcode.end)):
+            opcodes.append(CharmInstructionEnd())
+        end_op = opcodes[-1]
+
+        labels = {}
+        fixups = []
+
+        total = ArgumentGroup()
+        group = None
+        optional = False
+
+        # we store these as [index, s] lists initially
+        # then boil them down into dicts mapping index to lists of strings
+        # why? so we can fixup the indexes when we delete opcodes later
+        external_comments = []
+        external_labels = []
+
+        labels_seen = set()
+
+        # if 1:
+        #     print()
+        #     print("[assemble step 1 - {len(opcodes)} opcodes]")
+        #     for i, op in enumerate(opcodes):
+        #         print(f">> {i:02} | {op}")
+
+        index = 0
+        while index < len(opcodes):
+            op = opcodes[index]
+
+            # handle comments
+            if op.op == opcode.comment:
+                if comments == CharmAssembler.EXTERNAL:
+                    external_comments.append([index, op.comment])
+                    del opcodes[index]
+                elif comments == CharmAssembler.STRIP:
+                    del opcodes[index]
+                else:
+                    assert comments == CharmAssembler.PRESERVE
+                continue
+
+            # remove labels
+            if op.op == opcode.label:
+                if op in labels:
+                    raise AppealConfigurationError(f"label instruction used twice: {op}")
+                if op.label in labels_seen:
+                    raise AppealConfigurationError(f"label description used twice: '{op.label}'")
+                labels_seen.add(op.label)
+                labels[op] = index
+                external_labels.append([index, op.label])
+                del opcodes[index]
+                continue
+            elif op.op == opcode.jump_to_label:
+                fixups.append(index)
+            elif op.op == opcode.branch_on_flag_to_label:
+                fixups.append(index)
+            elif op.op == opcode.branch_on_not_flag_to_label:
+                fixups.append(index)
+            elif op.op == opcode.label_to_o:
+                fixups.append(index)
+
+            # remove no_ops
+            elif op.op == opcode.no_op:
+                del opcodes[index]
+                continue
+
+            index += 1
+
+        # if 1:
+        #     print()
+        #     print("[assemble step 2 - {len(opcodes)} opcodes]")
+        #     for i, op in enumerate(opcodes):
+        #         print(f">> {i:02} | {op}")
+
+        # now process jump fixups:
+        # replace *_to_label ops with absolute jump ops
+        replacement_op = {
+            opcode.jump_to_label: CharmInstructionJump,
+            opcode.branch_on_flag_to_label: CharmInstructionBranchOnFlag,
+            opcode.branch_on_not_flag_to_label: CharmInstructionBranchOnNotFlag,
+            opcode.label_to_o: CharmInstructionLiteralToO,
+        }
+        jump_ops = { opcode.jump_to_label, opcode.jump }
+        fixup_ops = []
+        for index in fixups:
+            op = opcodes[index]
+            address = labels.get(op.label)
+            if address is None:
+                raise AppealConfigurationError(f"unknown label {op.label}")
+            replacement = replacement_op[op.op](address)
+            opcodes[index] = replacement
+            fixup_ops.append(replacement)
+
+        # if 1:
+        #     print()
+        #     print("[assemble step 3 - {len(opcodes)} opcodes]")
+        #     for i, op in enumerate(opcodes):
+        #         print(f">> {i:02} | {op}")
+
+        jump_targets = set()
+        # and *now* do a jump-to-jump peephole optimization
+        # (I don't know if Appeal *can* actually generate jump-to-jumps)
+        for index in fixups:
+            while True:
+                op = opcodes[index]
+                op_attr = 'value' if op.op == opcode.literal_to_o else 'address'
+                address = getattr(op, op_attr)
+                # print(f"fixing up {op=}, at {index=}, {address=}")
+                op2 = opcodes[address]
+                if op2.op not in jump_ops:
+                    jump_targets.add(address)
+                    break
+                setattr(op, op_attr, op2.address)
+
+        jump_targets = list(jump_targets)
+        jump_targets.sort(reverse=True)
+
+        # remove redundant load_converter,
+        # load_o, and converter_to_o ops
 
-    def branch_on_o_to_label(self, label):
-        op = CharmInstructionBranchOnOToLabel(label=label)
-        return self.append(op)
-
-    def set_group(self, minimum=0, maximum=0, optional=True, repeating=False):
-        op = CharmInstructionSetGroup(minimum=minimum, maximum=maximum, optional=optional, repeating=repeating)
-        return self.append(op)
-
-    def end(self, id, name):
-        op = CharmInstructionEnd(id=id, name=name)
-        return self.append(op)
+        class Unknown:
+            def __repr__(self):
+                return "<Unknown>"
+
+        unknown = Unknown()
+        converter = unknown
+        o = unknown
+        stack = []
+        groups = []
 
+        def reset_registers():
+            # if 1 and want_prints:
+            #     print("*reset!* jump target!")
+            nonlocal converter
+            nonlocal o
+
+            converter = unknown
+            o = unknown
+
+        # if 1 and want_prints:
+        #     print("\nremoving redundant loads\n")
+        #     def print_op():
+        #         print(f"[{index:02}] {converter=} {o=} {op}", end=' ')
+
+        #     def nc():
+        #         print("no change")
+
+        def remove_op():
+            # if 1 and want_prints:
+            #     print(f" >>> deleting! redundant. <<<")
+            del opcodes[index]
+            for i in range(len(jump_targets)):
+                assert jump_targets[i] > index
+                jump_targets[i] -= 1
+            for op in fixup_ops:
+                op_attr = 'value' if op.op == opcode.literal_to_o else 'address'
+                address = getattr(op, op_attr)
+                if address > index:
+                    setattr(op, op_attr, address - 1)
+            for parent in (external_comments, external_labels):
+                for l in parent:
+                    if l[0] > index:
+                        l[0] -= 1
+
+        # if 1 and want_prints:
+        #     print("jump targets ", jump_targets)
+        index = 0
+        while index < len(opcodes):
+            if jump_targets and (jump_targets[-1] == index):
+                jump_targets.pop()
+                reset_registers()
+
+            op = opcodes[index]
+
+            # compute total and group values
+            # if 1 and want_prints:
+            #     print_op()
+            if op.op == opcode.set_group:
+                group = op.group
+                optional = op.optional
+                if op.repeating:
+                    total.maximum = math.inf
+                # if 1 and want_prints:
+                #     nc()
+            elif op.op == opcode.next_to_o:
+                if not optional:
+                    total.minimum += 1
+                total.maximum += 1
+
+                if group:
+                    group.minimum += 1
+                    group.maximum += 1
+
+                o = '(string value)'
+                # if 1 and want_prints:
+                #     print(f"o -> {o}")
+            elif op.op == opcode.lookup_to_o:
+                o = unknown
+                # if 1 and want_prints:
+                #     print(f"o -> {o}")
+            # discard redundant load_converter and load_o ops
+            # using dataflow analysis
+            elif op.op == opcode.load_converter:
+                if converter == op.key:
+                    remove_op()
+                    continue
+                converter = op.key
+                # if 1 and want_prints:
+                #     print(f"converter -> {converter}")
+            elif op.op == opcode.load_o:
+                if o == op.key:
+                    remove_op()
+                    continue
+                o = op.key
+                # if 1 and want_prints:
+                #     print(f"o -> {o}")
+            elif op.op == opcode.converter_to_o:
+                if o == converter:
+                    remove_op()
+                    continue
+                o = converter
+                # if 1 and want_prints:
+                #     print(f"o -> {o}")
+            elif op.op == opcode.create_converter:
+                o = op.key
+                # if 1 and want_prints:
+                #     print(f"o -> {o}")
+            else:
+                pass
+                # if 1 and want_prints:
+                #     nc()
+
+            index += 1
+
+        program = CharmProgram(self.name)
+        program.opcodes = opcodes
+        end_op.id = program.id
+        total.id = program.total.id
+        program.total = total
+        program.option_to_child_options = self.option_to_child_options
+        program.option_to_parent_options = self.option_to_parent_options
+
+        comments = defaultdict(list)
+        for index, comment in external_comments:
+            comments[index].append(comment)
+        program.comments = comments
+
+        labels = defaultdict(list)
+        for index, label in external_labels:
+            labels[index].append(label)
+        program.labels = labels
+
+        return program
 
 
 class CharmCompiler:
-    def __init__(self, appeal, *, name=None, converter_key=0):
+    """
+    Base compiler class.
+    You don't want to use this directly; you want one of the subclasses:
+
+    * CharmCommandCompiler compiles an Appeal "command".
+    * CharmOptionCompiler compiles an "option" for an Appeal "command".
+    * CharmMappingCompiler compiles a reader for a mapping.
+    * CharmIteratorCompiler compiles a reader for an iterator.
+
+    In general the workflow is like this:
+
+    * Construct the Compiler.  All compilers take the same arguments
+      in their constructor.
+    * Compile the thing, whatever it is, by calling the compiler object
+      (aka __call__).  These calls take context-specific arguments.
+    * Call the assemble method on the compiler.  This takes no arguments
+      and returns the finalized program.
+
+    (Why not have __call__ return the finalized program?  Because we might
+    want to modify the program after compliation but before final assembly.)
+    """
+
+    next_compilation_id = serial_number_generator(prefix="c-").__next__
+
+    def __init__(self, appeal, processor, *, indent='', name=''):
         self.appeal = appeal
+        self.root = appeal.root
+        self.processor = processor
+
         self.name = name
+        self.indent = indent
 
-        self.program = CharmProgram(name)
-        self.program.converter_key = converter_key
+        self.root_a = CharmAssembler(self.name)
 
-        self.root = appeal.root
+        self.next_converter_key = serial_number_generator(prefix=self.next_compilation_id() + '_k-').__next__
+
+    @staticmethod
+    def fake_parameter(kind, callable, default=empty):
+        parameter_name = callable.__name__
+        while True:
+            if parameter_name.startswith('<'):
+                parameter_name = parameter_name[1:-1]
+                continue
+            if parameter_name.endswith("()"):
+                parameter_name = parameter_name[:-2]
+                continue
+            break
+
+        # in Python 3.11, inspect.Parameter won't allow you to use
+        # 'lambda' (or '<lambda>') as a parameter name.  And we aren't
+        # doing that... not *really*.  It's not a *real* Parameter,
+        # we just use one of those because of the way _compile recurses.
+        # But if we're compiling a lambda function, we create a
+        # Parameter out of the function's name, which is '<lambda>',
+        # and, well... we gotta use *something*.  (hope this works!)
+
+        parameter = inspect.Parameter("___fake_name___", kind, annotation=callable, default=default)
+        parameter._name = parameter_name
+        return parameter
+
+    def clean_up_argument_group(self):
+        pass
+
+
+    def assemble(self):
+        """
+        Assembles all the instructions together to produce a final program.
+        """
+        if self.processor and self.processor.log:
+            self.processor.log.enter(f"assemble {self.name}")
+
+        self.clean_up_argument_group()
+
+        self.program = self.root_a.assemble()
+
+        if self.processor and self.processor.log:
+            self.processor.log.exit()
+
+        return self.program
 
-        self.total = ArgumentCounter()
-        self.group = ArgumentCounter()
 
-        self.initial_a = CharmAssembler(self)
-        self.final_a = CharmAssembler(self)
+class CharmAppealCompiler(CharmCompiler):
 
-        self.waiting_argument_group_options = None
+    def __init__(self, appeal, processor, parameter, *, indent='', name=''):
+        name = name or parameter.name
+        super().__init__(appeal, processor, indent=indent, name=name)
+        self.command_converter_key = None
 
-        self.assemblers = [self.initial_a]
+        # The compiler is effectively two passes.
+        #
+        # First, we iterate over the annotation tree generating instructions.
+        # These go into discrete "assemblers" which are carefully ordered in
+        # the self.assemblers list.
+        #
+        # Second, we root_a.finalize(), which assembles the final program.
+
+        callable = dereference_annotated(parameter.annotation)
+        default = parameter.default
 
-        self.option_depth = 0
+        indent = self.indent
 
         # options defined in the current argument group
-        self.argument_group_options = set()
-        self.argument_group_counter = 0
+        self.ag_a = self.ag_initialize_a = None
+        self.ag_options_a = self.ag_duplicate_options_a = None
+        self.ag_options = set()
+        self.ag_duplicate_options = set()
+        self.next_argument_group_id = serial_number_generator(prefix=f"{name} ag-").__next__
 
-        # options defined since the last consume_argument
-        self.consume_argument_options = set()
-        self.consume_argument_counter = 0
+        self.new_argument_group(optional=False, indent=indent)
 
-        self.new_argument_group_assemblers(optional=False)
-        self.after_consume_argument()
+        if self.processor:
+            self.processor.log.enter(f"compile {callable}")
 
-        self.name_to_callable = {}
+        # if want_prints:
+        #     print(f"[cc]")
+        #     print(f"[cc] {indent}Compiling '{self.name}'")
+        #     print(f"[cc]")
 
-    def new_consume_argument_assemblers(self):
-        if want_prints:
-            print(f"[cc]     -- new 'consume argument options' and 'body' assemblers")
-        self.consume_argument_options.clear()
+        if self.processor:
+            self.processor.log("parameter grouper")
+        def signature(p):
+            cls = self.appeal.map_to_converter(p)
+            signature = cls.get_signature(p)
+            return signature
+        pg = argument_grouping.ParameterGrouper(callable, default, signature=signature)
+        pgi = pg.iter_all()
 
-        self.consume_argument_options_a = a = CharmAssembler(self)
-        a.comment(f"{self.program.name} consume_argument {self.consume_argument_counter} options")
-        self.assemblers.append(a)
+        add_to_parent_a, is_degenerate = self.compile_parameter(parameter, pgi, 0, indent, name)
 
-        self.a = a = CharmAssembler(self)
-        a.comment(f"{self.program.name} body {self.consume_argument_counter}")
-        self.assemblers.append(a)
+        # if want_prints:
+        #     print(f"[cc] {indent}compilation of {parameter} complete.")
+        #     print(f"[cc]")
 
-        self.consume_argument_counter += 1
+        if self.processor:
+            self.processor.log.exit()
 
-    def new_argument_group_assemblers(self, *, optional):
-        if want_prints:
-            print(f"[cc]     -- new argument group 'converters' and 'options' assemblers")
+        self.add_to_parent_a = add_to_parent_a
 
-        self.flush_argument_group_options()
+    def clean_up_argument_group(self, indent=''):
+        if self.ag_a:
+            if self.ag_options:
+                # if want_prints:
+                #     print(f"[cc]")
+                #     print(f"[cc] {indent}flushing previous argument group's options.")
+                #     print(f"[cc]")
+                self.ag_initialize_a.append(self.ag_options_a)
+                self.ag_options.clear()
+
+            uninteresting_opcodes = set((opcode.comment, opcode.label))
+            # if we didn't put anything in one of our assemblers,
+            # clear it so we don't have the needless comment lying around
+            def maybe_clear_a(a):
+                # if length is 0, we don't need to bother clearing, it's already empty
+                # if length > 1, it has stuff in it
+                if a is None:
+                    return
+                if len(a) == 1:
+                    if a[0].op in uninteresting_opcodes:
+                        a.clear()
+
+            maybe_clear_a(self.ag_initialize_a)
+            maybe_clear_a(self.ag_options_a)
+            # is this redundant? maybe.
+            # but ag_duplicate_options_a is in body_a,
+            # so we should clear ag_duplicate_options_a
+            # before we try to clear body_a.
+            maybe_clear_a(self.ag_duplicate_options_a)
+            maybe_clear_a(self.body_a)
 
-        self.argument_group_options.clear()
+    def new_argument_group(self, *, optional, indent=''):
+        #
+        # Every argument group adds at least three assemblers:
+        #
+        #   * ag_initialize_a, the assembler for initialization code for
+        #     this argument group.  starts with a set_group instruction,
+        #     then has all the create_converter instructions.
+        #   * ag_options_a, the assembler for map_option instructions
+        #     for options that *haven't* been mapped before in this
+        #     argument group.
+        #   * ag_duplicate_options_a, the assembler for map_option
+        #     instructions for options that *have* been mapped before
+        #     in this argument group.  Initially this is None, and
+        #     then we create a fresh one after emitting every
+        #     next_to_o opcode.
+        #
+        # What's this about duplicate options?  It's Appeal trying
+        # to be a nice guy, to bend over backwards and allow crazy
+        # command-lines.
+        #
+        # Normally an option is mapped purely based on its membership
+        # in an optional group.  Consider this command:
+        #
+        #     def three_strs(d, e, f, *, o=False): ...
+        #
+        #     @app.command()
+        #     def base(a, b, c, three_strs: d_e_f=None, *, v=False): ...
+        #
+        # Its usage would look like this:
+        #
+        #     base [-v] a b c [ [-o] d e f ]
+        #
+        # -v is mapped the whole time, but -o is only mapped after
+        # you have three parameters.
+        #
+        # Now what if you change it to be like this?
+        #
+        #     def three_strs(d, e, f, *, o=False): ...
+        #
+        #     @app.command()
+        #     def base(a, b, c, d_e_f:three_strs=None, g_h_i:three_strs=None, *, v=False): ...
+        #
+        # Since the two mappings of -o are in different groups, it's okay.
+        # Usage looks like this:
+        #
+        #     base [-v] a b c [ [-o] d e f [ [-o] d e f ] ]
+        #
+        # Still not ambiguous.  But what if you do *this*?
+        #
+        #     def three_strs(d, e, f, *, o=False): ...
+        #
+        #     @app.command()
+        #     def base(a, b, c, d_e_f:three_strs, g_h_i:three_strs, *, v=False): ...
+        #
+        # Now everybody's in one big argument group.  And that means
+        # we map -o twice in the same group.
+        #
+        # Appeal permits this because it isn't actually ambiguous.
+        # It permits you to map the same option twice in one argument
+        # group *provided that* it can intelligently map the duplicate
+        # option after a next_to_o opcode--between positional
+        # parameters.  So usage looks like this:
+        #
+        #     base [-v] a b c [-o] d e f [-o] d e f
+        #
+        # It looks a little strange, but hey man, you're the one who
+        # asked Appeal to turn *that* into a command-line.  It's doing
+        # its best!
 
-        self.converters_a = a = CharmAssembler(self)
-        a.comment(f"{self.program.name} argument group {self.argument_group_counter} converters")
-        self.assemblers.append(a)
+        self.clean_up_argument_group(indent=indent)
 
-        self.argument_group_options_a = a = CharmAssembler(self)
-        assert not self.waiting_argument_group_options
-        self.waiting_argument_group_options = a
-        a.comment(f"{self.program.name} argument group {self.argument_group_counter} options")
+        self.group_id = group_id = self.next_argument_group_id()
 
-        self.argument_group_counter += 1
+        # if want_prints:
+        #     print(f"[cc] {indent}new argument group '{group_id}'")
+        #     indent += "  "
 
-        return self.converters_a.set_group(optional=optional)
+        self.ag_a = ag_a = CharmAssembler(group_id)
+        self.root_a.append(ag_a)
 
-    def new_argument_group(self, *, optional):
-        return_value = self.new_argument_group_assemblers(optional=optional)
-        self.new_consume_argument_assemblers()
-        return return_value
+        # "converters" represent functions we're going to fill with arguments and call.
+        # The top-level command is a converter, all the functions we call to convert
+        # arguments are converters.
+        self.ag_initialize_a = a = CharmAssembler(f"'{group_id}' initialize")
+        a.comment(f"{self.name} argument group '{group_id}' initialization")
+        ag_a.append(a)
+
+        self.ag_options_a = a = CharmAssembler(f"'{group_id}' options")
+        a.comment(f"{self.name} argument group '{group_id}' options")
+
+        self.body_a = a = CharmAssembler(f"'{group_id}' body")
+        a.comment(f"{self.name} argument group '{group_id}' body")
+        ag_a.append(a)
+
+        # initially in an argument group we don't allow duplicate options.
+        # you can only have duplicates after the first next_to_o
+        # opcode in an argument group.
+        self.ag_duplicate_options_a = None
+        self.ag_duplicate_options.clear()
 
-    def flush_argument_group_options(self):
-        if self.waiting_argument_group_options:
-            if want_prints:
-                print(f"[cc]     -- flushing argument group options")
-            self.assemblers.append(self.waiting_argument_group_options)
-            self.waiting_argument_group_options = None
+        self.group = self.ag_initialize_a.set_group(id=group_id, optional=optional)
+        return self.group
 
-    def after_consume_argument(self):
-        self.flush_argument_group_options()
-        self.new_consume_argument_assemblers()
+    def reset_duplicate_options_a(self):
+        """
+        Clear the "duplicate options" state, so that additional duplicates
+        can get mapped.
 
-    def compile_options(self, parent_callable, key, parameter, options, depth):
-        if want_prints:
-            indent = "  " * depth
-            print(f"[cc] {indent}compile_options options={options} key={key} parameter={parameter} parameter.kind={parameter.kind}")
+        Call this immediately after you append a positional argument
+        (append_to_converter_args).  Every time.
+        """
+        if self.ag_duplicate_options:
+            self.ag_duplicate_options.clear()
+        elif self.ag_duplicate_options_a:
+            self.ag_duplicate_options_a.clear()
+
+        group_id = self.group_id
+        self.ag_duplicate_options_a = a = CharmAssembler(f"{group_id} duplicate options")
+        a.comment(f"{self.name} argument group {group_id} duplicate options")
+        self.body_a.append(a)
+
+    def is_converter_discretionary(self, parameter, converter_class):
+        optional = (
+            # *args and **kwargs are not required
+            (parameter.kind in (VAR_POSITIONAL, VAR_KEYWORD))
+            or
+            # parameters of other types with a default are not required
+            (parameter.default is not empty)
+            )
+
+        # only actual Converter objects can be discretionary
+        is_converter = issubclass(converter_class, Converter)
+
+        return is_converter and optional
+
+    def compile_option(self, program_name, parameter, indent):
+        """
+        This compiles everything in the option except for the
+        last little bit where we store the result in the parent
+        converter's kwargs.
+        """
+
+        # if want_prints:
+        #     print(f"[cc] {indent}compile_option")
+        #     indent += "  "
+        #     print(f"[cc] {indent}program_name={program_name}")
+        #     print(f"[cc] {indent}parameter={parameter}")
+        #     print(f"[cc]")
 
         cls = self.appeal.root.map_to_converter(parameter)
+        converter = cls(parameter, self.appeal)
+        callable = converter.callable
 
-        assert options
-        name = parent_callable.__name__
-        option_names = [denormalize_option(o) for o in options]
-        assert option_names
-        option_names = " | ".join(option_names)
-        program_name = f"{name} {option_names}"
         if cls is SimpleTypeConverterStr:
-            if want_prints:
-                print(f"[cc] {indent}(hand-coded str option)")
-            program = CharmProgram(name=program_name, minimum=1, maximum=1)
-            a = CharmAssembler(self)
-            a.push_context()
-            a.set_group(1, 1, optional=False)
-            a.load_converter(key)
-            a.consume_argument(is_oparg=True)
-            a.store_kwargs(parameter.name)
-            a.pop_context()
-            a.end(name=program_name, id=program.id)
-            program.opcodes = a.opcodes
+            # hand-coded program to handle this option that takes
+            # a single required str argument.
+            # if want_prints:
+            #     print(f"[cc] {indent}hand-coded program for simple str")
+            a = CharmAssembler(program_name)
+            a.set_group(self.next_argument_group_id(), optional=False)
+            a.next_to_o(required=True, is_oparg=True)
+            add_to_self_a = cc = a
         else:
             annotation = dereference_annotated(parameter.annotation)
             if not is_legal_annotation(annotation):
-                raise AppealConfigurationError(f"{parent_callable.__name__}: parameter {parameter.name!r} annotation is {parameter.annotation}, which you can't use directly, you must call it")
+                raise AppealConfigurationError(f"precompile_option(): parameter {parameter.name!r} annotation is {parameter.annotation}, which you can't use directly, you must call it")
 
-            # self.ensure_callables_have_unique_names(callable)
-            multioption = issubclass(cls, MultiOption)
+            # if want_prints:
+            #     print(f"[cc] {indent}<< recurse on option >>")
 
-            cc = CharmCompiler(self.appeal, name=program_name, converter_key=self.program.converter_key)
-            a = cc.initial_a
-            a.push_context()
-
-            a = cc.final_a
-            a.pop_context()
-
-            store_kwargs = key, parameter.name
-            program = cc.compile(annotation, parameter.default, is_option=True, multioption=multioption, depth=depth+1, store_kwargs=store_kwargs)
-            assert self.program.converter_key != cc.program.converter_key
-            self.program.converter_key = cc.program.converter_key
+            cc = CharmOptionCompiler(self.appeal, self.processor, parameter, indent=indent, name=program_name)
+            add_to_self_a = cc.add_to_parent_a
 
-        for option in options:
-            # option doesn't have to be unique in this argument group,
-            # but it must be unique per consumed argument.
-            # (you can't define the same option twice without at least one consume_argument between.)
-            if option in self.consume_argument_options:
-                raise AppealConfigurationError(f"multiple definitions of option {denormalize_option(option)} are ambiguous (no arguments consumed in between definitions)")
-            self.consume_argument_options.add(option)
-
-            if option not in self.argument_group_options:
-                self.argument_group_options.add(option)
-                destination = self.argument_group_options_a
-            else:
-                destination = self.consume_argument_options_a
+        return cc, add_to_self_a
+
+    def map_options(self, callable, key, parameters, depth, indent):
+        # if want_prints:
+        #     print(f"[cc] {indent}map_options")
+        #     indent += "    "
+        #     print(f"[cc] {indent}automatically map keyword-only parameters to options")
 
-            if want_prints:
-                indent = "  " * depth
-                print(f"[cc] {indent}compile_options option={option} program={program} callable={parent_callable} parameter={parameter} key={key} destination={destination}")
-            destination.map_option(option, program, parent_callable, parameter, key)
-
-    def map_options(self, callable, parameter, signature, key, depth=0):
-        if want_prints:
-            indent = "  " * depth
-            print(f"[cc] {indent}{callable.__name__} map_options parameter={parameter} key={key} signature={signature}")
         _, kw_parameters, _ = self.appeal.fn_database_lookup(callable)
-        mappings = kw_parameters.get(parameter.name, ())
 
-        if not mappings:
-            p = signature.parameters.get(parameter.name)
-            assert p
-            annotation = dereference_annotated(p.annotation)
-            default = p.default
-            default_options = self.appeal.root.default_options
-            assert builtins.callable(default_options)
-            default_options(self.appeal, callable, parameter.name, annotation, default)
+        all_kwonly_names = []
 
-        parameter_index_to_options = collections.defaultdict(list)
-        parameters = []
-        for option_entry in kw_parameters[parameter.name]:
-            option, callable2, parameter = option_entry
-            # assert callable is not empty
-            assert callable == callable2
+        # step 1: populate explicit keyword-only options
+        #
+        # we have to iterate over parameters, because we need
+        # to force mapping with default_options.
+        var_keyword = None
+        for parameter in parameters.values():
+            if parameter.kind == KEYWORD_ONLY:
+                if parameter.default == empty:
+                    raise AppealConfigurationError(f"x: keyword-only argument {parameter.name} doesn't have a default value")
+                mappings = kw_parameters.get(parameter.name, None)
+                if not mappings:
+                    annotation = dereference_annotated(parameter.annotation)
+                    default_options = self.appeal.root.default_options
+                    assert builtins.callable(default_options)
+                    default_options(self.appeal, callable, parameter.name, annotation, parameter.default)
+                all_kwonly_names.append(parameter.name)
+                continue
+            if parameter.kind == VAR_KEYWORD:
+                var_keyword = parameter.name
+                continue
 
-            # not all parameters are hashable.  (default might be a list, etc.)
-            try:
-                parameter_index = parameters.index(parameter)
-            except ValueError:
-                parameter_index = len(parameters)
-                parameters.append(parameter)
+        # step 2: populate **kwargs-only options
+        # (options created with appeal.option(), where the parameter_name doesn't
+        #  appear in the function, so the output goes into **kwargs)
 
-            parameter_index_to_options[parameter_index].append(option)
+        # if want_prints:
+        #     print(f"[cc] {indent}map user-defined options")
 
-        for parameter_index, options in parameter_index_to_options.items():
-            parameter = parameters[parameter_index]
-            self.compile_options(callable, key, parameter, options, depth)
+        kw_parameters_unseen = set(kw_parameters) - set(all_kwonly_names)
+        if kw_parameters_unseen:
+            if not var_keyword:
+                raise AppealConfigurationError(f"x: there are options that must go into **kwargs, but this callable doesn't accept **kwargs.  options={kw_parameters_unseen}")
+            # avoid randomness
+            kw_parameters_unseen = list(kw_parameters_unseen)
+            kw_parameters_unseen.sort()
+            all_kwonly_names.extend(kw_parameters_unseen)
 
+        # if want_prints:
+        #     print(f"[cc] {indent}all keyword only parameters: {all_kwonly_names}")
 
-    def _compile(self, depth, parameter, pgi, usage_callable, usage_parameter, multioption=False, append=None, store_kwargs=None):
+        mapped_options = []
+        for name in all_kwonly_names:
+            # Group together all options for an individual Parameter object.
+            #
+            # There may be multiple *different* Parameter objects for a
+            # single parameter, because that's how we represent mapping multiple
+            # different converters to a single keyword-only parameter.
+            #
+            #     https://github.com/larryhastings/appeal#multiple-options-for-the-same-parameter
+            #
+            # But Parameter objects aren't necessarily hashable.
+            # (the default might be a list, etc.)
+            # Also!  You also can't rely on Parameter objects
+            # being unique.  There can be two Parameter objects
+            # with the same value.
+            #
+            # And it gets worse!  The official way to turn a parameter into a callable
+            # is through the converter factories via map_to_converter.  But the only way
+            # to get the converter out is to instantiate it.  And that might give you a
+            # bound method of a dynamically-generated class, which means nothing will
+            # compare the same because the instances are different.
+            #
+            # So we correlate them together by converter and default value.  And if the
+            # converter is an instance of a bound method, we yank out the class and the
+            # unbound method and use those.
+
+            work = []
+            parameter_ids = []
+            for option_entry in kw_parameters[name]:
+                option, redundant_callable, parameter = option_entry
+                assert callable == redundant_callable
+                mapped_options.append(option)
+
+                cls = self.root.map_to_converter(parameter)
+                converter = cls(parameter, self.appeal)
+                parameter_callable = converter.callable
+
+                # I can't believe it's come to this
+                if isinstance(parameter_callable, types.MethodType):
+                    parameter_callable = (parameter_callable.__self__.__class__, parameter_callable.__func__)
+
+                parameter_key = (parameter_callable, parameter.default)
+                for parameter_id, parameter_key2 in enumerate(parameter_ids):
+                    if parameter_key == parameter_key2:
+                        break
+                else:
+                    parameter_id = len(parameter_ids)
+                    parameter_ids.append(parameter_key)
+                    work.append((parameter, []))
+
+                options = work[parameter_id][1]
+                options.append(option)
+
+            for parameter, options in work:
+                # if want_prints:
+                #     print(f"[cc] {indent}work: {parameter=} {options=}")
+
+                option_names = [denormalize_option(o) for o in options]
+                assert option_names
+                option_names = " | ".join(option_names)
+                program_name = f"{callable.__name__} {option_names}"
+
+                cc, add_to_self_a = self.compile_option(program_name, parameter, indent)
+                add_to_self_a.load_converter(key=key)
+                add_to_self_a.set_in_converter_kwargs(name=parameter.name)
+                program = cc.assemble()
+
+                for option in options:
+                    # option doesn't have to be unique in this argument group,
+                    # but it must be unique per command-line argument.
+                    # (you can't define the same option twice without at least one next_to_o between.)
+
+                    if option not in self.ag_options:
+                        self.ag_options.add(option)
+                        self.ag_duplicate_options.add(option)
+                        destination = self.ag_options_a
+                    elif self.ag_duplicate_options_a is not None:
+                        if option in self.ag_duplicate_options:
+                            raise AppealConfigurationError(f"multiple definitions of option {denormalize_option(option)} are ambiguous (no command-line arguments between definitions)")
+                        destination = self.ag_duplicate_options_a
+                        self.ag_duplicate_options.add(option)
+                    else:
+                        raise AppealConfigurationError(f"argument group initialized with multiple definitions of option {denormalize_option(option)}, ambiguous")
+
+                    # if want_prints:
+                    #     print(f"[cc] {indent}option={option}")
+                    #     print(f"[cc] {indent}    program={program}")
+                    #     print(f"[cc] {indent}    destination={destination}")
+                    destination.map_option(self.group_id, option, program, key, parameter)
+
+        return mapped_options
+
+    def compile_parameter(self, parameter, pgi, depth, indent, usage_name):
         """
-        returns is_degenerate, a boolean, True if this entire subtree is "degenerate".
+        returns add_to_self_a, is_degenerate
+
+        add_to_self_a is an assembler inserted immediately after
+          the value for this parameter is read in / created.
+          (the value is either a string from the command-line
+          or a converter). at that moment, the value has loaded
+          in the 'o' register.
+        is_degenerate is a boolean, True if this entire subtree is "degenerate".
         """
+        if self.processor:
+            self.processor.log.enter(f"compile parameter {parameter.name}")
 
-        if want_prints:
-            indent = "  " * depth
-            print(f"[cc] {indent}compiling 'parameter={parameter}' depth={depth}, pgi, multioption={multioption} append={append}")
+        # if want_prints:
+        #     print(f"[cc] {indent}compile_parameter {parameter}")
+        #     indent += "    "
+        #     required = "yes" if parameter.default is empty else "no"
+        #     print(f"[cc] {indent}required? {required}")
+        #     print(f"[cc] {indent}depth={depth}")
+        #     print(f"[cc]")
 
         maps_to_positional = set((POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD, VAR_POSITIONAL))
         tracked_by_argument_grouping = set((POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD, VAR_POSITIONAL))
 
-        # hard-coded, at least for now
-        annotation = dereference_annotated(parameter.annotation)
-        if annotation is not empty:
-            cls = annotation
-        elif parameter.default is not empty:
-            cls = type(parameter.default)
-
-        callable = annotation
+        # the official and *only correct* way
+        # to produce a converter from a parameter.
         cls = self.root.map_to_converter(parameter)
+        converter = cls(parameter, self.appeal)
+        callable = converter.callable
+
         signature = cls.get_signature(parameter)
         parameters = signature.parameters
-        if want_prints:
-            print(f"[cc] {indent}cls={cls} signature={signature}")
 
-        if depth == 0:
-            # degenerate only applies to depth > 1.
-            is_degenerate = False
-        else:
-            is_degenerate = len(parameters) < 2
-        if want_prints:
-            print(f"[cc] {indent}is_degenerate={is_degenerate}, len(parameters){len(parameters)} < 2")
+        _, _, positionals = self.appeal.root.fn_database_lookup(callable)
+
+        # if want_prints:
+        #     print(f"[cc] {indent}cls={cls}")
+        #     if not parameters:
+        #         print(f"[cc] {indent}signature=()")
+        #     else:
+        #         print(f"[cc] {indent}signature=(")
+        #         for _k, _v in parameters.items():
+        #             print(f"[cc] {indent}    {_v},")
+        #         print(f"[cc] {indent}    )")
+        #     print(f"[cc]")
 
+        is_degenerate = (depth > 0) and (len(parameters) < 2)
+
+        # if want_prints:
+        #     print(f"[cc] {indent}is_degenerate={is_degenerate}")
+        #     print(f"[cc] {indent}len(parameters)={len(parameters)}")
+        #     print(f"[cc]")
+
+        # fix chicken-and-egg problem:
+        # create converter key here, so we can use it in multioption block
+        converter_key = self.next_converter_key()
+        if not self.command_converter_key:
+            # guarantee that the root converter has a special key
+            self.command_converter_key = converter_key
+
+        multioption = issubclass(cls, MultiOption)
         if multioption:
-            assert not append
+            # assert issubclass(cls, MultiOption), f"{cls=} is not a MultiOption"
             label_flush_multioption = CharmInstructionLabel("flush_multioption")
             label_after_multioption = CharmInstructionLabel("after_multioption")
 
-            load_o_op = self.converters_a.load_o(0)
-            self.converters_a.branch_on_o_to_label(label_flush_multioption)
-
-        op = self.converters_a.create_converter(parameter=parameter)
-        converter_key = op.key
-
-        append_op = None
-        if append:
-            self.a.load_o(key=converter_key)
-            append_op = self.a.append_args(**append)
-        elif store_kwargs:
-            parent_key, parameter_name = store_kwargs
-            self.a.load_converter(key=parent_key)
-            self.a.load_o(key=converter_key)
-            self.a.store_kwargs(name=parameter_name)
+            assert self.command_converter_key
+            load_o_op = self.ag_initialize_a.load_o(key=self.command_converter_key)
+            self.ag_initialize_a.test_is_o_true()
+            self.ag_initialize_a.branch_on_flag_to_label(label_flush_multioption)
+        # else:
+        #     assert not issubclass(cls, MultiOption), f"{cls=} IS a MultiOption"
+
+        self.ag_initialize_a.create_converter(parameter=parameter, key=converter_key)
+        add_to_parent_a = CharmAssembler()
+        add_to_parent_a.load_o(key=converter_key)
+        self.body_a.append(add_to_parent_a)
 
         if multioption:
             load_o_op.key = converter_key
-            self.converters_a.jump_to_label(label_after_multioption)
-            self.converters_a.append(label_flush_multioption)
-            op = self.converters_a.flush_multioption()
-            self.converters_a.append(label_after_multioption)
+            self.ag_initialize_a.jump_to_label(label_after_multioption)
+            self.ag_initialize_a.append(label_flush_multioption)
+            self.ag_initialize_a.flush_multioption()
+            self.ag_initialize_a.forget_converters()
+            self.ag_initialize_a.append(label_after_multioption)
+            self.ag_initialize_a.remember_converters()
 
-        var_keyword = None
-        kw_parameters_seen = set()
-        _, kw_parameters, positionals = self.appeal.fn_database_lookup(callable)
-
-        for i, (parameter_name, p) in enumerate(parameters.items()):
-            # populate options, and find var_keyword (if present)
-            if p.kind == KEYWORD_ONLY:
-                if p.default == empty:
-                    raise AppealConfigurationError(f"{usage_callable}: keyword-only argument {parameter_name} doesn't have a default value")
-                kw_parameters_seen.add(parameter_name)
-                self.map_options(callable, p, signature, converter_key, depth=depth)
-                continue
-            if p.kind == VAR_KEYWORD:
-                var_keyword = parameter_name
-                continue
+        # we need to delay mapping options sometimes.
+        #
+        # if depth=0, we're in the command function (or the root option function).
+        # all options go into the first argument group.
+        #
+        # if depth>0, we're in a child annotation function. all options go into
+        # the same group as the first argument (if any)
+        spilled_options = False
+        def spill_options():
+            nonlocal spilled_options
+            if spilled_options:
+                return
+            spilled_options = True
+            self.map_options(callable, converter_key, parameters, depth, indent)
 
-        # step 2: populate **kwargs-only options
-        # (options created with appeal.option(), where the parameter_name doesn't
-        #  appear in the function, so the output goes into **kwargs)
-        kw_parameters_unseen = set(kw_parameters) - kw_parameters_seen
-        if kw_parameters_unseen:
-            if not var_keyword:
-                raise AppealConfigurationError(f"{usage_callable}: there are options that must go into **kwargs, but this callable doesn't accept **kwargs.  options={parameters_unseen}")
-            for parameter_name in kw_parameters_unseen:
-                parameter = inspect.Parameter(parameter_name, KEYWORD_ONLY)
-                self.map_options(callable, parameter, signature, converter_key, depth=depth)
+        if not depth:
+            spill_options()
 
         group = None
 
         # Consider this:
         #
         #  def my_int(s): return int(s)
         #  @app.command()
@@ -1283,316 +2744,633 @@
         # In usage we'd rather see "abc" than "s".  So this is special-cased.
         # Appeal calls this a "degenerate converter tree"; it's a tree of converter
         # functions that only have one positional parameter each.  Appeal will by
         # default use the usage information from the parameter from the root parameter
         # of that degenerate converter tree--in this case, the parameter "abc" from
         # the function "foo".
 
+        # if want_prints:
+        #     print(f"[cc] {indent}compile positional parameters")
+        #     print(f"[cc]")
+        #     indent += "    "
+
         for i, (parameter_name, p) in enumerate(parameters.items()):
             if not p.kind in maps_to_positional:
                 continue
 
             annotation = dereference_annotated(p.annotation)
             if not is_legal_annotation(annotation):
                 raise AppealConfigurationError(f"{callable.__name__}: parameter {p.name!r} annotation is {p.annotation}, which you can't use directly, you must call it")
 
             # FIXME it's lame to do this here,
-            # you need to rewrite _compile so it
+            # you need to rewrite compile_parameter so it
             # always recurses for positional parameters
             cls = self.root.map_to_converter(p)
 
             if p.kind == VAR_POSITIONAL:
-                label = self.a.label("var_positional")
+                label = self.body_a.label("var_positional")
+                self.body_a.remember_converters()
                 index = -1
             else:
                 index = i
 
-            if is_degenerate:
-                usage_parameter = usage = None
-            else:
-                usage_callable = callable
-                usage = usage_parameter = parameter_name
-
-            usage = positionals.get(parameter_name, usage)
+            # if is_degenerate:
+            #     usage_parameter = usage = None
+            # else:
+            #     usage_callable = callable
+            #     usage = usage_parameter = parameter_name
 
-            if want_prints:
-                printable_default = "(empty)" if p.default is empty else repr(p.default)
-                print(f"[cc] {indent}{callable.__name__} positional parameter {i}: p={p} p.kind={p.kind!s} annotation={annotation.__name__} default={printable_default} cls={cls}")
+            # usage = positionals.get(parameter_name, usage)
+            # usage = "-x"
+            if not is_degenerate:
+                usage_name = parameter_name
+            # handle @app.parameter name override
+            override = positionals.get(parameter_name)
+            if override:
+                usage_name = override
 
             # only create new groups here if it's an optional group
             # (we pre-create the initial, required group)
             pgi_parameter = next(pgi)
-            if want_prints:
-                print(f"[cc] {indent}pgi_parameter={pgi_parameter}")
+
+            # if want_prints:
+            #     printable_default = "(empty)" if p.default is empty else repr(p.default)
+            #
+            #     print(f"[cc] {indent}positional parameter {i}: p={p}")
+            #     print(f"[cc] {indent}    p.kind={p.kind!s}")
+            #     print(f"[cc] {indent}    annotation={annotation.__name__}")
+            #     print(f"[cc] {indent}    default={printable_default} cls={cls}")
+            #     print(f"[cc] {indent}    cls={cls}")
+            #     print(f"[cc] {indent}    pgi_parameter={pgi_parameter}")
+
             if pgi_parameter.first_in_group and (not pgi_parameter.in_required_group):
-                if want_prints:
-                    print(f"[cc] {indent}{callable.__name__} new argument group optional=True")
-                group = self.new_argument_group(optional=True)
+                group = self.group = self.new_argument_group(optional=True, indent=indent + "    ")
+
+            spill_options()
 
-            self.a.load_converter(key=converter_key)
-            if cls is SimpleTypeConverterStr: # or (isinstance(callable, type) and issubclass(callable, Option)):
+            if cls is SimpleTypeConverterStr:
                 # if want_prints:
-                #     print(f"{indent_str}       LEAF {pgi_parameter} is_degenerate={is_degenerate}")
-                # ends_group = pgi_parameter.last_in_group
-                # starts_optional_group = pgi_parameter.first_in_group and not pgi_parameter.in_required_group
-                if want_prints:
-                    print(f"[cc] {indent}{parameter} consume_argument and append")
-                self.a.consume_argument(is_oparg=bool(self.option_depth))
-                op = self.a.append_args(callable=callable, parameter=p, usage=usage, usage_callable=usage_callable, usage_parameter=usage_parameter)
-                self.after_consume_argument()
+                #     print(f"[cc] {indent}    simple str converter, next_to_o and append.")
+                required = pgi_parameter.required
+                self.body_a.next_to_o(required=required, is_oparg=isinstance(self, CharmOptionCompiler))
+                if not required:
+                    label2 = CharmInstructionLabel(f'{callable.__name__}.{parameter_name}: exit after optional argument')
+                    self.body_a.branch_on_flag_to_label(label2)
+                    self.body_a.end()
+                    self.body_a.append(label2)
+
+                discretionary = False
+                add_to_self_a = self.body_a
+                self.reset_duplicate_options_a()
             else:
-                if want_prints:
-                    print(f"[cc] {indent}{callable.__name__} recurse into {parameter_name} p={p}")
-                # self.ensure_callables_have_unique_names(callable)
-                append = {'callable': callable, 'parameter': parameter_name, "usage": usage, 'usage_callable': usage_callable, 'usage_parameter': usage_parameter }
-                is_degenerate_subtree = self._compile(depth + 1, p, pgi, usage_callable, usage_parameter, None, append=append)
+                # if want_prints:
+                #     print(f"[cc] {indent}    << recurse on parameter >>")
+                discretionary = self.is_converter_discretionary(p, cls)
+                add_to_self_a, is_degenerate_subtree = self.compile_parameter(p, pgi, depth + 1, indent + "    ", usage_name)
                 is_degenerate = is_degenerate and is_degenerate_subtree
 
+            add_to_self_a.load_converter(key=converter_key)
+
+            usage_full_name = (f"{callable.__name__}.{p.name}", usage_name)
+            usage = (f"{callable.__name__}.{p.name}", usage_name)
+            add_to_self_a.append_to_converter_args(
+                parameter=parameter_name,
+                discretionary=discretionary,
+                usage=usage,
+                )
+
             if p.kind == VAR_POSITIONAL:
                 group.repeating = True
-                self.a.jump_to_label(label)
+                self.body_a.forget_converters()
+                self.body_a.jump_to_label(label)
 
-        # if want_prints:
-        #     print(f"{indent_str}<< callable={callable}")
+            # if want_prints:
+            #     print(f"[cc]")
 
-        if append_op and not is_degenerate:
-            if want_prints:
-                print(f"[cc] {indent}suppress usage for non-leaf parameter {append_op.usage}")
-            append_op.usage = None
+        spill_options()
 
-        return is_degenerate
+        if self.processor:
+            self.processor.log.exit()
 
+        return add_to_parent_a, is_degenerate
 
-    def compile(self, callable, default, is_option=False, multioption=None, store_kwargs=None, depth=0):
-        if self.name is None:
-            self.name = callable.__name__
-            self.program.name = self.name
 
-        parameter_name = callable.__name__
-        while True:
-            if parameter_name.startswith('<'):
-                parameter_name = parameter_name[1:-1]
-                continue
-            if parameter_name.endswith("()"):
-                parameter_name = parameter_name[:-2]
-                continue
-            break
+class CharmCommandCompiler(CharmAppealCompiler):
 
-        # in Python 3.11, inspect.Parameter won't allow you to use
-        # 'lambda' (or '<lambda>') as a parameter name.  And we aren't
-        # doing that, not really.  It's not a *real* Parameter, we
-        # just use one of those because of the way _compile recurses.
-        # But if we're compiling a lambda function, we create a
-        # Parameter out of the function's name, which is '<lambda>',
-        # and, well... we gotta use *something*.  (hope this works!)
-        fix_lambda = parameter_name == 'lambda'
-        if fix_lambda:
-            parameter_name = '_____lambda______'
+    def __init__(self, appeal, processor, callable, *, indent='', name=''):
+        parameter = self.fake_parameter(POSITIONAL_ONLY, callable, empty)
+        super().__init__(appeal, processor, parameter, indent=indent, name=name)
 
-        def signature(p):
-            cls = self.appeal.map_to_converter(p)
-            signature = cls.get_signature(p)
-            return signature
-        pg = argument_grouping.ParameterGrouper(callable, default, signature=signature)
-        pgi = pg.iter_all()
 
-        kind = KEYWORD_ONLY if is_option else POSITIONAL_ONLY
-        if is_option:
-            self.option_depth += 1
-        parameter = inspect.Parameter(parameter_name, kind, annotation=callable, default=default)
-        if fix_lambda and (getattr(parameter, '_name', '') == parameter_name):
-            parameter._name = 'lambda'
-        self._compile(depth, parameter, pgi, usage_callable=None, usage_parameter=None, multioption=multioption, store_kwargs=store_kwargs)
-        self.final_a.end(self.program.id, self.name)
-        self.assemblers.append(self.final_a)
+def charm_compile_command(appeal, processor, callable):
+    cc = CharmCommandCompiler(appeal, processor, callable)
+    return cc.assemble()
 
-        opcodes = self.finalize()
-        self.program.opcodes = opcodes
 
-        if is_option:
-            self.option_depth -= 1
 
-        return self.program
+class CharmOptionCompiler(CharmAppealCompiler):
+    pass
+
+
+
+class CharmMappingCompiler(CharmCompiler):
+
+    def __init__(self, appeal, processor, callable, *, indent='', name=''):
+        name = name or callable.__name__
+        super().__init__(appeal, processor, indent=indent, name=name)
 
+        if self.processor:
+            self.processor.log.enter(f"compile {name}")
 
-    def finalize(self):
+        # if want_prints:
+        #     print(f"[cm]")
+        #     print(f"[cm] {indent}Compiling '{self.name}'")
+        #     print(f"[cm]")
+
+        parameter = self.fake_parameter(POSITIONAL_ONLY, callable, empty)
+        self.compile_parameter(parameter, indent, force_unnested=True)
+
+        self.root_a.end()
+
+        if self.processor:
+            self.processor.log.exit()
+
+    # a "parent's name" can be a special value CONSUME
+
+    def compile_parameter(self, parameter, indent, *, by_name=True, degenerate_name=None, depth=0, degenerate_multioption=False, force_unnested=False):
+        """
+        returns 2-tuple
+            (child_converter_key, is_degenerate)
         """
-        Performs a finalization pass on program:
+        if self.processor:
+            self.processor.log.enter(f"compile parameter {parameter.name}")
 
-        * Computes total and group min/max values.
-        * Convert label/jump_to_label pseudo-ops into
-          absolute jump ops.
-        * Simple peephole optimizations to remove redundant
-          load_* ops and jump-to-jumps.
+        # if want_prints:
+        #     print(f"[cm] {indent}compile_parameter {parameter=}")
+        #     indent += "    "
+        #     required = "yes" if parameter.default is empty else "no"
+        #     print(f"[cm] {indent}by_name {by_name!r}")
+        #     print(f"[cm] {indent}degenerate_name {degenerate_name!r}")
+        #     print(f"[cm] {indent}degenerate_multioption {degenerate_multioption!r}")
+        #     print(f"[cm] {indent}depth {depth}")
+        #     print(f"[cm] {indent}required? {required}")
+        #     print(f"[cm]")
+
+        # the official and *only correct* way
+        # to produce a converter from a parameter.
+        cls = self.root.map_to_converter(parameter)
+        converter = cls(parameter, self.appeal)
+        callable = converter.callable
+
+        signature = cls.get_signature(parameter)
+        parameters = signature.parameters
+
+        if not len(parameters):
+            raise AppealConfigurationError("Sorry, can't process a converter that takes no parameters here")
+
+        converter_key = self.next_converter_key()
+        a = self.root_a
+
+        only_one_parameter = len(parameters) == 1
+        is_degenerate = (depth > 0) and only_one_parameter
+        multioption = issubclass(cls, MultiOption)
+        unnested_requested = callable in self.root.unnested_converters
+        nested = not (force_unnested or unnested_requested or multioption)
+        required = parameter.default is empty
+        force_non_recursive = False
+
+        if not is_degenerate:
+            degenerate_name = None
+
+        # if want_prints:
+        #     print(f"[cm] {indent}cls={cls}")
+        #     if not parameters:
+        #         print(f"[cm] {indent}signature=()")
+        #     else:
+        #         print(f"[cm] {indent}signature=(")
+        #         for _k, _v in parameters.items():
+        #             print(f"[cm] {indent}    {_v},")
+        #         print(f"[cm] {indent}    )")
+        #     print(f"[cm] {indent}is_degenerate={is_degenerate}")
+        #     print(f"[cm] {indent}multioption={multioption}")
+        #     print(f"[cm] {indent}nested={nested} (force_unnested={force_unnested}, callable in self.root.unnested_converters = {callable in self.root.unnested_converters})")
+        #     print(f"[cm] {indent}only_one_parameter={only_one_parameter}")
+        #     print(f"[cm] {indent}required={required}")
+        #     print(f"[cm]")
+
+        def get_argument_to_o(a, name, required):
+            if by_name:
+                a.lookup_to_o(name, required=required)
+            else:
+                a.next_to_o(required=required, is_oparg=True, usage_name=name)
+
+        if multioption:
+            by_name = False
+
+            label_prefix = f'[mo] {parameter.name}: '
+            def Label(s):
+                return CharmInstructionLabel(label_prefix + s)
+
+            label_next = Label('multioption, next')
+            label_done = Label(f'multioption, done')
+            label_flush = Label('multioption, flush')
+
+            # do we have a value to process with the multioption?
+            # if not, goto done.
+            a.append(label_next)
+            a.next_to_o(required=False, is_oparg=True, usage_name=parameter.name)
+            a.branch_on_not_flag_to_label(label_done)
+
+            # we do.  push o, so we can examine it later.
+            # has the converter been created?  if so, goto flush,
+            # else create it.
+            a.push_o()
+            a.load_o(key=converter_key)
+            a.branch_on_flag_to_label(label_flush)
+
+            # converter hasn't been created yet.
+            # and... why, lookee here!
+
+        a.create_converter(parameter=parameter, key=converter_key)
+
+        if multioption:
+            assert not nested
+            label_analyze_iterated_value = Label(f'{parameter.name}: multioption, analyze iterated value')
+            label_o_is_a_mapping = Label(f'{parameter.name}: multioption, o is a mapping')
+            label_pop_mapping = Label(f'{parameter.name}: multioption, pop mapping')
+            label_pop_iterator = Label(f'{parameter.name}: multioption, pop iterator')
+
+            # created converter, goto test is o a mapping.
+            a.jump_to_label(label_analyze_iterated_value)
+
+            # converter already existed, flush.
+            a.append(label_flush)
+            a.flush_multioption()
+            a.forget_converters()
+
+            a.append(label_analyze_iterated_value)
+            a.pop_o()
+            a.remember_converters()
+
+            if only_one_parameter:
+                a.wrap_o_with_iterator()
+                a.push_iterator()
+                by_name = False
+            else:
+                # is o a mapping?
+                a.test_is_o_mapping()
+                a.branch_on_flag_to_label(label_o_is_a_mapping)
+                a.abort("MultiOption {callable.__name__} requires multiple parameters, iterable only yielded an individual object")
+
+                # o is a mapping.  push it to mapping stack and process arguments.
+                a.append(label_o_is_a_mapping)
+                by_name = True
+                a.push_mapping()
+
+        elif nested:
+            label_o_is_a_mapping = CharmInstructionLabel(f"{parameter.name}: nested, o is a mapping")
+            label_process_arguments = CharmInstructionLabel(f"{parameter.name}: nested, process arguments")
+            name = degenerate_name or parameter.name
+            get_argument_to_o(a, name, required)
+            a.test_is_o_mapping()
+            a.push_flag()
+            a.branch_on_flag_to_label(label_o_is_a_mapping)
+            if not by_name:
+                a.pushback_o_to_iterator()
+            a.jump_to_label(label_process_arguments)
+            a.append(label_o_is_a_mapping)
+            a.push_mapping()
+            a.append(label_process_arguments)
+
+        for child in parameters.values():
+            if child.kind is VAR_POSITIONAL:
+                raise AppealConfigurationError(f"{callable.__name__}: parameter *{child.name} is unsupported for CharmMappingCompiler")
+            if child.kind is VAR_KEYWORD:
+                raise AppealConfigurationError(f"{callable.__name__}: parameter **{child.name} is unsupported for CharmMappingCompiler")
+
+            child_annotation = dereference_annotated(child.annotation)
+            if not is_legal_annotation(child_annotation):
+                raise AppealConfigurationError(f"{callable.__name__}: parameter {child.name} annotation is {child_annotation}, which you can't use directly, you must call it")
+
+            # FIXME it's lame to do this again here,
+            # you should rewrite compile_parameter so it
+            # always recurses for positional parameters
+            child_cls = self.root.map_to_converter(child)
+            child_converter = child_cls(child, self.appeal)
+            child_callable = child_converter.callable
+            child_multioption = issubclass(child_cls, MultiOption)
+
+            child_required = child.default is empty
+            child_discretionary = not child_required
+            child_write_to_kwargs = (child.kind is KEYWORD_ONLY) or ((child.kind is POSITIONAL_OR_KEYWORD) and child_discretionary)
+
+            label_got_value = CharmInstructionLabel(f"child {child.name}, got value")
+
+            # if want_prints:
+            #     print(f"[cm] {indent} {child=} {child_cls=} {child_converter=} {child_callable=} {child_multioption=}")
+            if child_cls is SimpleTypeConverterStr:
+                name = degenerate_name or child.name
+                get_argument_to_o(a, name, child_required)
+
+                label_got_value = CharmInstructionLabel(f"child {child.name}, got value")
+                a.branch_on_flag_to_label(label_got_value)
+                if child_discretionary:
+                    a.literal_to_o(child.default)
+                else:
+                    a.abort("{child.name} is required but was not set in the mapping")
+                a.append(label_got_value)
+
+            else:
+                if child_multioption:
+                    name = degenerate_name or child.name
+                    label_o_is_iterable = CharmInstructionLabel(f"child {child.name}, o is iterable")
+                    get_argument_to_o(a, name, child_required)
+
+                    a.branch_on_flag_to_label(label_got_value)
+                    if child_discretionary:
+                        a.literal_to_o(child.default)
+                    else:
+                        a.abort("{child.name} is required but was not available")
+                    a.append(label_got_value)
+
+                    a.test_is_o_iterable()
+                    a.branch_on_flag_to_label(label_o_is_iterable)
+                    a.abort("value in o is not iterable")
+                    a.append(label_o_is_iterable)
+                    a.push_iterator()
+
+                child_key, child_is_degenerate = self.compile_parameter(child, indent + "    ", depth=depth + 1, by_name=by_name, degenerate_name=degenerate_name or child.name)
+                # if want_prints:
+                #     print(f"[cm] {indent} {child_key=} {child_is_degenerate=}")
+
+                if child_multioption:
+                    # if want_prints:
+                    #     print(f"[cm] {indent} generate push / pop iterator (child_multioption)")
+                    a.pop_iterator()
+                    # I think multioptions can't be degenerate.
+                    is_degenerate = False
+
+                a.load_o(child_key)
+                is_degenerate = is_degenerate and child_is_degenerate
+
+            a.load_converter(converter_key)
+            if child_write_to_kwargs:
+                a.set_in_converter_kwargs(child.name)
+            else:
+                a.append_to_converter_args(parameter=child, discretionary=False, usage=None)
+
+            # if want_prints:
+            #     print(f"[cm]")
+
+        if multioption:
+            # okay.  we processed arguments.
+            if only_one_parameter:
+                a.pop_iterator()
+            else:
+                a.pop_mapping()
+            a.jump_to_label(label_next)
+            a.append(label_done)
+            a.forget_converters()
+        elif nested:
+            label_done = CharmInstructionLabel(f"{parameter.name}: nested, done")
+            a.pop_flag()
+            a.branch_on_not_flag_to_label(label_done)
+            a.pop_mapping()
+            a.append(label_done)
+
+        if self.processor:
+            self.processor.log.exit()
+
+        # if want_prints:
+        #     print(f"[cm] {indent}compile_parameter({parameter}) returning {converter_key=} {is_degenerate=}")
+        return converter_key, is_degenerate
+
+
+
+class CharmIteratorCompiler(CharmCompiler):
+
+    def __init__(self, appeal, processor, callable, *, indent='', name=''):
+        name = name or callable.__name__
+        super().__init__(appeal, processor, indent=indent, name=name)
+
+        if self.processor:
+            self.processor.log.enter(f"compile {name}")
+
+        # if want_prints:
+        #     print(f"[cm]")
+        #     print(f"[cm] {indent}Compiling '{self.name}'")
+        #     print(f"[cm]")
+
+        parameter = self.fake_parameter(POSITIONAL_ONLY, callable, empty)
+        self.root_a = CharmAssembler(name)
+
+        cls = self.root.map_to_converter(parameter)
+        converter = cls(parameter, self.appeal)
+        callable = converter.callable
+        self.label_done = CharmInstructionLabel('done')
+
+        child_key = self.compile_parameter(parameter, indent)
+
+        self.root_a.append(self.label_done)
+        self.root_a.end()
+
+        if self.processor:
+            self.processor.log.exit()
+
+    def compile_parameter(self, parameter, indent, *, depth=0, force_not_required = False):
+        """
+        returns 2-tuple
+            (child_converter_key, is_degenerate)
         """
+        if self.processor:
+            self.processor.log.enter(f"compile parameter {parameter.name}")
 
-        program = self.program.opcodes
-        for a in self.assemblers:
-            opcodes = a.opcodes
-            if not opcodes:
-                continue
-            if (len(opcodes) == 1) and (opcodes[0].op == opcode.comment):
-                continue
-            program.extend(opcodes)
+        # if want_prints:
+        #     print(f"[cm] {indent}compile_parameter {parameter=}")
+        #     indent += "    "
+        #     required = "yes" if parameter.default is empty else "no"
+        #     print(f"[cm] {indent}required? {required}")
+        #     print(f"[cm] {indent}depth {depth}")
+        #     print(f"[cm]")
 
-        p = program
+        # the official and *only correct* way
+        # to produce a converter from a parameter.
+        cls = self.root.map_to_converter(parameter)
+        converter = cls(parameter, self.appeal)
+        callable = converter.callable
 
-        labels = {}
-        jump_fixups = []
-        total = self.program.total
-        group = None
-        converter = None
-        o = None
-        option = None
-        stack = []
+        signature = cls.get_signature(parameter)
+        parameters = signature.parameters
 
-        optional = False
+        # if want_prints:
+        #     print(f"[cm] {indent}cls={cls}")
+        #     if not parameters:
+        #         print(f"[cm] {indent}signature=()")
+        #     else:
+        #         print(f"[cm] {indent}signature=(")
+        #         for _k, _v in parameters.items():
+        #             print(f"[cm] {indent}    {_v},")
+        #         print(f"[cm] {indent}    )")
+        #     print(f"[cm]")
 
-        i = 0
+        # if want_prints:
+        #     print(f"[cm] {indent}len(parameters)={len(parameters)}")
+        #     print(f"[cm]")
 
-        while i < len(p):
-            op = p[i]
+        converter_key = self.next_converter_key()
 
-            # remove labels
-            if op.op == opcode.label:
-                if op in labels:
-                    raise AppealConfigurationError(f"label used twice: {op}")
-                labels[op] = i
-                del p[i]
-                # forget current registers,
-                # who knows what state the interpreter
-                # will be in when we jump here.
-                converter = o = None
-                continue
-            if op.op in (opcode.jump_to_label, opcode.branch_on_o_to_label):
-                jump_fixups.append(i)
+        a = self.root_a
 
-            # remove no_ops
-            if op.op == opcode.no_op:
-                del p[i]
-                continue
-            if op.op == opcode.comment:
-                # if 1:
-                if not want_prints:
-                    del p[i]
-                    continue
+        a.create_converter(parameter=parameter, key=converter_key)
+        is_degenerate = (not depth) and (len(parameters) < 2)
 
-            # compute total and group values
-            if op.op == opcode.set_group:
-                group = op.group
-                optional = op.optional
-                if op.repeating:
-                    if total:
-                        total.maximum = math.inf
-            if op.op == opcode.consume_argument:
-                if total:
-                    if not optional:
-                        total.minimum += 1
-                    total.maximum += 1
-                if group:
-                    group.minimum += 1
-                    group.maximum += 1
+        for child in parameters.values():
+            child_annotation = dereference_annotated(child.annotation)
+            if not is_legal_annotation(child_annotation):
+                raise AppealConfigurationError(f"{callable.__name__}: parameter {p.name!r} annotation is {p.annotation}, which you can't use directly, you must call it")
 
-            # discard redundant load_converter and load_o ops
-            if op.op == opcode.load_converter:
-                if converter == op.key:
-                    del p[i]
-                    continue
-                converter = op.key
-            if op.op == opcode.load_o:
-                if o == op.key:
-                    del p[i]
-                    continue
-                o = op.key
-            if op.op == opcode.create_converter:
-                o = op.key
-            if op.op == opcode.consume_argument:
-                o = '(string value)'
-            if op.op == opcode.push_context:
-                stack.append(CharmContextStackEntry(converter, group, o, total))
-            if op.op == opcode.pop_context:
-                context = stack.pop()
-                converter = context.converter
-                group = context.group
-                o = context.o
-                total = context.total
+            if child.kind is KEYWORD_ONLY:
+                raise AppealConfigurationError("{callable.__name__}: keyword-only parameter {parameter.name!r} is unsupported for CharmIteratorCompiler")
+            if child.kind is VAR_KEYWORD:
+                raise AppealConfigurationError("{callable.__name__}: parameter **{parameter.name!r} is unsupported for CharmIteratorCompiler")
+            var_positional = child.kind is VAR_POSITIONAL
 
-            i += 1
 
-        # now process jump fixups:
-        # replace *_to_label ops with absolute jump ops
-        opcode_map = {
-            opcode.jump_to_label: CharmInstructionJump,
-            opcode.branch_on_o_to_label: CharmInstructionBranchOnO,
-        }
-        for i in jump_fixups:
-            op = p[i]
-            new_instruction_cls = opcode_map[op.op]
-            address = labels.get(op.label)
-            if address is None:
-                raise AppealConfigurationError(f"unknown label {op.label}")
-            p[i] = new_instruction_cls(address)
+            # FIXME it's lame to do this here,
+            # you need to rewrite compile_parameter so it
+            # always recurses for positional parameters
+            child_cls = self.root.map_to_converter(child)
+            child_converter = child_cls(child, self.appeal)
+            child_callable = child_converter.callable
+
+            if var_positional:
+                required = False
+                label_remember = CharmInstructionLabel('remember')
+                a.jump_to_label(label_remember)
+                label_again = a.label('again')
+                a.forget_converters()
+                a.append(label_remember)
+                a.remember_converters()
+            else:
+                required = (child.default is empty) and (not force_not_required)
 
-        # and *now* do a jump-to-jump peephole optimization
-        # (I don't know if Appeal can actually generate jump-to-jumps)
-        for i in jump_fixups:
-            op = p[i]
-            while True:
-                op2 = p[op.address]
-                if op2.op != opcode.jump:
-                    break
-                op.address = op2.address
+            # if want_prints:
+            #     print(f"[cm] {indent} {child=} {child_cls=} {child_converter=} {child_callable=}")
+            if child_cls is SimpleTypeConverterStr:
+                a.next_to_o(required=required, is_oparg=True, usage_name=child.name)
+                if not required:
+                    a.branch_on_not_flag_to_label(self.label_done)
+            else:
+                child_key, child_is_degenerate = self.compile_parameter(child, indent + "    ", depth=depth + 1, force_not_required=not required)
+                a.load_o(child_key)
+
+            a.load_converter(converter_key)
+            a.append_to_converter_args(parameter=child, discretionary=False, usage=None)
+
+            is_degenerate = is_degenerate and child_is_degenerate
+
+            if var_positional:
+                a.jump_to_label(label_again)
 
-        return p
+            # if want_prints:
+            #     print(f"[cm]")
 
+        if self.processor:
+            self.processor.log.exit()
+
+        return converter_key, is_degenerate
 
-def charm_compile(appeal, callable, default=empty, name=None, *, is_option=False):
-    if name is None:
-        name = callable.__name__
-    cc = CharmCompiler(appeal, name=name)
-    program = cc.compile(callable, default, is_option=is_option)
-    return program
 
 
 def charm_print(program, indent=''):
     programs = collections.deque((program,))
     print_divider = False
     seen = set((program.id,))
+    specially_formatted_opcodes = set((opcode.comment, opcode.label))
+
+    comments = program.comments
+    labels = program.labels
+
     while programs:
         if print_divider:
             print("________________")
             print()
         else:
             print_divider = True
         program = programs.popleft()
-        width = 2
+        width = math.floor(math.log10(len(program))) + 1
         padding = " " * width
         indent2 = indent + f"{padding}|   "
+        empty_line = indent2.rstrip()
         print(program)
+        print_leading_blank_line = False
+        comment_prefix = f"{indent}{' ':{width}}# "
+        label_prefix = f"{indent}{' ':{width}}: "
         for i, op in enumerate(program):
+            prefix = f"{indent}{i:0{width}}| "
+
+            print_blank = True
+            c = comments.get(i, ())
+            for comment in c:
+                if print_blank:
+                    print(indent2)
+                    print_blank = False
+                print(f"{comment_prefix}{comment}")
+                print_leading_blank_line = False
+
+            print_blank = True
+            l = labels.get(i, ())
+            for label in l:
+                if print_blank:
+                    print(indent2)
+                    print_blank = False
+                print(f"{label_prefix}{label}")
+                print_leading_blank_line = False
+
+            # specialized opcode printers
+            if op.op in specially_formatted_opcodes:
+                if print_leading_blank_line:
+                    print(empty_line)
+                    print_leading_blank_line = False
+                if op.op == opcode.comment:
+                    print(f"{prefix}# {op.comment}")
+                else:
+                    print(f"{prefix}{op.label}:")
+                print(empty_line)
+                continue
+
+            # generic opcode printer
+            if print_leading_blank_line:
+                print(empty_line)
+            print_leading_blank_line = True
             suffix = ""
             printable_op = str(op.op).rpartition(".")[2]
-            print(f"{indent}{i:0{width}}| {printable_op}{suffix}")
-            # for slot in op.__class__.__slots__:
-            for slot in dir(op):
+            print(f"{prefix}{printable_op}{suffix}")
+            for slot in op.__class__.__slots__:
+            # for slot in dir(op):
                 if slot.startswith("_") or slot in ("copy", "op"):
                     continue
                 value = getattr(op, slot, None)
                 if slot == "program":
                     print(f"{indent2}program={value}")
                     value_id = value.id
                     if value_id not in seen:
                         programs.append(value)
                         seen.add(value_id)
                     continue
                 if slot == "callable":
                     value = value.__name__ if value is not None else value
+                elif slot == "address":
+                    assert value is not None
+                    label_names = ", ".join(f"'{s}'" for s in labels.get(value, ()))
+                    assert label_names, f"didn't have any labels for index {value=}, {labels=}"
+                    value = f"{value} # {label_names}"
                 elif value == empty:
                     value = "(empty)"
-                elif isinstance(value, ArgumentCounter):
+                elif isinstance(value, ArgumentGroup):
                     value = value.summary()
                 else:
                     value = repr(value)
                 print(f"{indent2}{slot}={value}")
     print()
 
 
@@ -1602,904 +3380,1847 @@
 
     def __init__(self, program):
         self.program = program
         self.opcodes = program.opcodes
         self.length = len(program)
         self.ip = 0
 
+    def __repr__(self):
+        return f"<{self.__class__.__name__} program={self.program} ip={self.ip}>"
+
+    def __repr__(self):
+        return f"[{self.program}:{self.ip}]"
+
     def __next__(self):
         if not bool(self):
             raise StopIteration
         op = self.opcodes[self.ip]
         self.ip += 1
         if 0:
             print(f">> {hex(id(self))} ip -> ", op)
         return op
 
     def __bool__(self):
         return 0 <= self.ip < self.length
 
     def jump(self, address):
         self.ip = address
+        if not self:
+            raise RuntimeError(f"Jumped outside current program, ip={self.ip}, len(program)={self.length}")
 
     def jump_relative(self, delta):
         self.ip += delta
+        if not self:
+            raise RuntimeError(f"Jumped outside current program, ip={self.ip}, len(program)={self.length}")
 
+    def end(self):
+        self.ip = self.length
 
 
-class CharmStackEntry:
-    __slots__ = ['i', 'program', 'context_count']
-
-    def __init__(self, i, program, context_count=0):
-        self.i = i
-        self.program = program
-        self.context_count = context_count
-
-    def __repr__(self):
-        return f"<CharmStackEntry i={self.i} program={self.program.name!r} context_count={self.context_count}>"
-
-
-class CharmContextStackEntry:
-    __slots__ = ['converter', 'group', 'o', 'total']
-
-    def __init__(self, converter, group, o, total):
-        self.converter = converter
-        self.group = group
-        self.o = o
-        self.total = total
-
-    def __repr__(self):
-        return f"<CharmContextStackEntry converter={self.converter} group={self.group} o={self.o} total={self.total}>"
-
-
-class CharmInterpreter:
+class CharmBaseInterpreter:
+    """
+    A bare-bones interpreter for Charm programs.
+    Doesn't actually interpret anything;
+    it just provides the registers and the iterator
+    and some utility functions like jump, push, and pop.
+    Actually interpreting the instructions is up to
+    the user.
+    """
     def __init__(self, program, *, name=''):
         self.name = name
-        self.stack = []
-        self.context_stack = []
+        self.call_stack = []
+
+        self.iterator = None
+        self.iterator_stack = []
+
+        self.mapping = None
+        self.mapping_stack = []
 
         assert program
 
         # registers
+
+        self.program = program
+        # shh, don't tell anybody,
+        # the ip register technically lives *inside* the iterator.
+        self.ip = CharmProgramIterator(program)
+
         self.converter = None
         self.o = None
-        self.total = None
+        self.data_stack = []
+
+        self.flag = False
         self.group = None
+
         self.converters = {}
-        self.program = program
+        self.converter_keys = None
+        self.converter_keys_stack = []
 
-        self.op = None
+        self.groups = []
 
-        # ip register actually lives inside the iterator
-        self.i = CharmProgramIterator(program)
+        self.aborted = False
 
-    def repr_ip(self):
-        ip = "--"
-        if self.i:
-            width = math.floor(math.log10(len(self.i.program)) + 1)
-            ip = f"{self.i.ip:0{width}}"
-        return ip
+    def repr_ip(self, ip=None):
+        s = "--"
+
+        if self.ip is not None:
+            if ip is None:
+                ip = self.ip.ip
+            length = len(self.ip.program)
+            if 0 <= ip < length:
+                width = math.floor(math.log10(length) + 1)
+                s = f"{ip:0{width}}"
+        return s
 
     def __repr__(self):
         ip = self.repr_ip()
-        total = self.total and self.total.summary()
         group = self.group and self.group.summary()
         converter = self.repr_converter(self.converter)
         o = self.repr_converter(self.o)
-        return f"<CharmInterpreter [{ip}] converter={converter!s} o={o!s} group={group!s} total={total!s}>"
+        return f"<{self.__class__.__name__} [{ip}] converter={converter!s} o={o!s} group={group!s}>"
 
-    def repr_converter(self, converter):
+    def converter_to_key(self, converter):
         if self.converters:
-            width = math.floor(math.log10(len(self.converters)) + 1)
             for key, value in self.converters.items():
                 if converter == value:
-                    return [key]
-        return converter
+                    return key
+        return None
+
+    def repr_converter(self, converter):
+        if isinstance(converter, str) and self.converters:
+            key = self.converter_to_key(converter)
+            if key:
+                width = math.floor(math.log10(len(self.converters)) + 1)
+                return f"[{key}]={converter!r}"
+        return repr(converter)
+
+    def remember_converters(self):
+        self.converter_keys_stack.append(self.converter_keys)
+        self.converter_keys = set()
+
+    def forget_converters(self):
+        for key in self.converter_keys:
+            assert key in self.converters
+            del self.converters[key]
+        self.converter_keys = self.converter_keys_stack.pop()
+
+    @big.BoundInnerClass
+    class CharmProgramStackEntry:
+        __slots__ = ['interpreter', 'ip', 'program', 'converter', 'o', 'flag', 'group', 'groups']
+
+        def __init__(self, interpreter):
+            self.interpreter = interpreter
+            self.ip = interpreter.ip
+            self.program = interpreter.program
+            self.converter = interpreter.converter
+            self.o = interpreter.o
+            self.flag = interpreter.flag
+            self.group = interpreter.group
+            self.groups = interpreter.groups
+
+        def restore(self):
+            interpreter = self.interpreter
+            interpreter.ip = self.ip
+            interpreter.program = self.program
+            interpreter.converter = self.converter
+            interpreter.o = self.o
+            interpreter.flag = self.flag
+            interpreter.group = self.group
+            interpreter.groups = self.groups
+
+        def __repr__(self):
+            return f"<CharmProgramStackEntry ip={self.ip} program={self.program.name!r} converter={self.converter} o={self.o} flag={self.flag} group={self.group.summary() if self.group else 'None'} groups=[{len(self.groups)}]>"
 
     def __iter__(self):
         return self
 
     def __next__(self):
         while True:
-            if not (self.i or self.stack):
+            if not (self.ip or self.call_stack):
                 raise StopIteration
             try:
-                op = self.i.__next__()
-                if 0:
-                    print("()>", op)
-                return op
+                ip = self.ip.ip
+                op = self.ip.__next__()
+                return ip, op
             except StopIteration as e:
-                self.finish()
+                self.end()
                 continue
 
-    def __bool__(self):
-        return bool(self.i) or any(bool(cse.i) for cse in self.stack)
+    # def __bool__(self):
+    #     return bool(self.ip) or any(bool(cse.ip) for cse in self.call_stack)
+    def running(self):
+        return bool(self.ip) or any(bool(cse.ip) for cse in self.call_stack)
 
-    def rewind(self):
-        if self.i is None:
+    def rewind_one_instruction(self):
+        if self.ip is None:
             raise StopIteration
-        self.i.jump_relative(-1)
+        self.ip.jump_relative(-1)
 
     def call(self, program):
-        self.stack.append(CharmStackEntry(self.i, self.program))
-        self.program = program
-        self.i = CharmProgramIterator(program)
+        cpse = self.CharmProgramStackEntry()
+        self.call_stack.append(cpse)
 
-    def push_context(self):
-        context = CharmContextStackEntry(self.converter, self.group, self.o, self.total)
-        self.context_stack.append(context)
-        if self.stack:
-            self.stack[-1].context_count += 1
-
-    def _pop_context(self):
-        context = self.context_stack.pop()
-        self.converter = context.converter
-        self.group = context.group
-        self.o = context.o
-        self.total = context.total
-
-    def pop_context(self):
-        self._pop_context()
-        if self.stack:
-            self.stack[-1].context_count -= 1
-
-    def finish(self):
-        if self.stack:
-            cse = self.stack.pop()
-            self.i = cse.i
-            self.program = cse.program
-            for i in range(cse.context_count):
-                self._pop_context()
+        self.program = program
+        self.ip = CharmProgramIterator(program)
+        self.groups = []
+        self.converter = self.o = self.group = None
+        self.flag = False
+
+    def end(self):
+        if self.call_stack:
+            cpse = self.call_stack.pop()
+            cpse.restore()
         else:
-            self.i = None
+            self.ip = None
 
-    def abort(self):
-        self.i = None
-        self.stack.clear()
-        self.context_stack.clear()
+    def _stop(self):
+        self.ip = None
+        self.call_stack.clear()
+
+    def abort(self, message=''):
+        # print("ABORT MESSAGE:", message)
+        raise RuntimeError("ABORT MESSAGE: " + message)
+        self._stop()
+        self.aborted = True
+        return None
 
+    def unwind(self):
+        while self.call_stack:
+            self.end()
+        self._stop()
 
 
-def _charm_usage(program, usage, closing_brackets, formatter, arguments_values, option_values):
-    ci = CharmInterpreter(program)
+def _charm_usage(appeal, program, usage, closing_brackets, formatter, arguments_values, option_values):
+    ci = CharmBaseInterpreter(program)
     program_id_to_option = collections.defaultdict(list)
 
+    key_to_callable = {}
+
     def add_option(op):
         program_id_to_option[op.program.id].append(op)
 
     def flush_options():
-        for program_id, op_list in program_id_to_option.items():
+        for program_id, ops in program_id_to_option.items():
             options = []
-            for op in op_list:
+            key = None
+            for op in ops:
                 options.append(denormalize_option(op.option))
-            full_name = f"{op.callable.__name__}.{op.parameter.name}"
+                # these are grouped by program_id, so, op.key will
+                # be the same for all of them
+                if key is None:
+                    key = op.key
+                else:
+                    assert key == op.key, f"expected identical keys, but {key=} != {op.key=}"
+            callable = key_to_callable[key]
+            full_name = f"{callable.__name__}.{op.parameter.name}"
             option_value = "|".join(options)
             option_values[full_name] = option_value
 
-            usage.append(" [")
+            usage.append("[")
             usage.append(option_value)
 
             usage.append(" ")
             old_len_usage = len(usage)
-            _charm_usage(op.program, usage, closing_brackets, formatter, arguments_values, option_values)
+            _charm_usage(appeal, op.program, usage, closing_brackets, formatter, arguments_values, option_values)
             if len(usage) == old_len_usage:
                 # this option had no arguments, we don't want the space
                 usage.pop()
 
-            usage.append("]")
+            usage.append("] ")
+        program_id_to_option.clear()
 
-    last_op = None
     first_argument_in_group = True
-    for op in ci:
-        # print(f"op={op}")
-        if ((last_op == opcode.map_option)
-            and (op.op != last_op)):
-            flush_options()
+    add_to_usage = False
+
+    for ip, op in ci:
+        # print(f"[{ip:03}] {op}")
+
+        if op.op == opcode.create_converter:
+            # the official and *only correct* way
+            # to produce a converter from a parameter.
+            cls = appeal.map_to_converter(op.parameter)
+            converter = cls(op.parameter, appeal)
+            callable = converter.callable
+            key_to_callable[op.key] = callable
+            continue
 
         if op.op == opcode.map_option:
             add_option(op)
-        elif op.op == opcode.set_group:
+            continue
+        if program_id_to_option:
+            flush_options()
+
+        if op.op == opcode.set_group:
             if op.optional:
                 usage.append(" [")
                 closing_brackets.append("]")
                 if op.repeating:
                     closing_brackets.append("... ")
             first_argument_in_group = True
-        elif op.op == opcode.append_args:
-            # append_args can only be after one of those two opcodes!
-            # if last_op.op in (opcode.consume_argument, opcode.load_o):
-                if op.usage:
-                    if first_argument_in_group:
-                        first_argument_in_group = False
-                    else:
-                        usage.append(" ")
-                    full_name = f"{op.usage_callable.__name__}.{op.usage_parameter}"
-                    arguments_values[full_name] = op.usage
-                    usage.append(formatter(op.usage))
-        last_op = op
+            continue
+
+        if op.op == opcode.next_to_o:
+            add_to_usage = True
+            continue
+
+        if (op.op == opcode.set_in_converter_kwargs) and add_to_usage:
+            add_to_usage = False
+            continue
 
-    flush_options()
+        if op.op == opcode.append_to_converter_args:
+            usage_full_name, usage_name = op.usage
+            arguments_values[usage_full_name] = usage_name
+            if add_to_usage:
+                add_to_usage = False
+                if first_argument_in_group:
+                    first_argument_in_group = False
+                else:
+                    usage.append(" ")
+                usage.append(formatter(usage_name))
+            continue
+
+    if program_id_to_option:
+        flush_options()
 
 
-def charm_usage(program, *, formatter=str):
+def charm_usage(appeal, program, *, formatter=str):
     usage = []
     closing_brackets = []
     arguments_values = {}
     option_values = {}
-    _charm_usage(program, usage, closing_brackets, formatter, arguments_values, option_values)
+    _charm_usage(appeal, program, usage, closing_brackets, formatter, arguments_values, option_values)
     usage.extend(closing_brackets)
     # print(f"arguments_values={arguments_values}")
     # print(f"option_values={option_values}")
     return "".join(usage).strip(), arguments_values, option_values
 
 
 
-def charm_parse(appeal, program, argi):
-    (
-    option_space_oparg,
-
-    short_option_equals_oparg,
-    short_option_concatenated_oparg,
-    ) = appeal.root.option_parsing_semantics
-
-    ci = CharmInterpreter(program)
-    root = None
-
-    token_to_bucket = {}
-    bucket_to_token = {}
-
-    next_options_token = 0
-    options_stack = []
-    options_bucket = {}
-
-    options_bucket = None
-    options_token = None
-
-    if want_prints:
-        ip_spacer = '    '
-
-    def push_options():
-        nonlocal options_bucket
-        nonlocal options_token
-        nonlocal next_options_token
-        options_stack.append(options_bucket)
-        options_bucket = {}
-        options_token = next_options_token
-        next_options_token += 1
-        token_to_bucket[options_token] = options_bucket
-        bucket_to_token[id(options_bucket)] = options_token
-        if want_prints:
-            print(f"## {ip_spacer} push_options options_token={options_token}")
-
-    def pop_options():
-        nonlocal options_bucket
-        nonlocal options_token
-
-        token = bucket_to_token[id(options_bucket)]
-        del bucket_to_token[id(options_bucket)]
-        del token_to_bucket[token]
-
-        options_bucket = options_stack.pop()
-        options_token = bucket_to_token[id(options_bucket)]
-
-        if want_prints:
-            print(f"## {ip_spacer} pop_options, now at token {options_token}, popped options_bucket={options_bucket}")
-
-    def pop_options_to_token(token):
-        bucket = token_to_bucket.get(token)
-        if bucket is None:
-            return
-        pop_count = 0
-        while options_bucket != bucket:
-            pop_count += 1
-            pop_options()
-        if want_prints:
-            print(f"## {ip_spacer} pop_options_to_token token={token} took {pop_count} pops")
-
-    def pop_options_to_base():
-        if want_prints:
-            print(f"## {ip_spacer} pop_options_to_base, popping {len(options_stack)} times")
-        for _ in range(len(options_stack)):
-            pop_options()
-
-    def find_option(option):
-        depth = 0
-        bucket = options_bucket
-        bucket_iter = reversed(options_stack)
-        while True:
-            program = bucket.get(option, None)
-            if program is not None:
+from abc import ABCMeta, abstractmethod
+def _check_methods(C, *methods):
+    mro = C.__mro__
+    for method in methods:
+        for B in mro:
+            if method in B.__dict__:
+                if B.__dict__[method] is None:
+                    return NotImplemented
                 break
-            try:
-                bucket = next(bucket_iter)
-            except StopIteration:
-                raise AppealUsageError(f"unknown option {denormalize_option(option)}") from None
+        else:
+            return NotImplemented
+    return True
+
+
+class CharmInterpreter(CharmBaseInterpreter):
+    def __init__(self, processor, program, *, name=''):
+        super().__init__(program, name=name)
+        self.processor = processor
+        self.program = program
+
+        self.appeal = processor.appeal
+        i = processor.iterator
+        if i and not isinstance(i, big.PushbackIterator):
+            i = big.PushbackIterator(i)
+        self.iterator = i
+        self.mapping = processor.mapping
+
+        self.command_converter_key = None
+
+        # The first part of the __call__ loop consumes *opcodes.*
+        self.opcodes_prefix = "#---"
+        # The second part of the __call__ loop consumes *cmdline arguments.*
+        self.cmdline_prefix = "####"
+
+        self.options = self.Options()
 
-        token = bucket_to_token[id(bucket)]
-        return program, program.total.maximum, token
 
     ##
-    ## It can be hard to tell in advance whether or not
-    ## we have positional parameters waiting.  For example:
-    ##   * the first actual positional argument is optional
-    ##   * it's nested three levels deep in the annotation tree
-    ##   * we have command-line arguments waiting in argi but
-    ##     they're all options
-    ## In this scenario, the easiest thing is to just run the
-    ## program, create the converters, then discover we never
-    ## consumed any positional arguments and just remove &
-    ## destroy the converters.  This "undo" functionality
-    ## does exactly that: you write down all the positional
-    ## converters you create, and if you don't consume a
-    ## positional argument, you undo them.
+    ## "options"
     ##
-    ## Observe that:
-    ##   * we're only talking about optional groups, and
-    ##   * optional groups are only created if we consume arguments, and
-    ##   * we don't create options in an optional group until
-    ##     after we've consumed the first argument that ensures
-    ##     we've really entered that group.
+    ## Options in Appeal can be hierarchical.
+    ## One option can map in child options.
+    ## These child options have a limited lifespan.
+    ##
+    ## Example:
+    ##
+    ##     def color_option(color, *, brightness=0, hue=0): ...
+    ##     def position_option(x, y, z, *, polar=False): ...
+    ##
+    ##     @app.command()
+    ##     def frobnicate(a, b, c, *, color:color_option=Color('BLUE'), position:position_option=Position(0, 0, 0)): ...
+    ##
+    ## If you then run this command-line:
+    ##
+    ##     % python3 myscript frobnicate A --color red ...
+    ##                                                 ^
+    ##                                                 |
+    ##      +------------------------------------------+
+    ##      |
+    ## At THIS point. we've run the Charm program associated
+    ## with "--color".  It's mapped in two new options,
+    ## "--brightness" (and probably "-b") and "--hue" (and maybe "-h").
+    ## These are "child options"; they're children of "--color".
+    ##
+    ## If the next thing on the command-line is "--brightness"
+    ## or "--hue", we handle that option.  But if the next thing
+    ## is a positional argument to frobnicate (which will be
+    ## the argument supplied to parameter "b"), or the option
+    ## "--position", those two child options are *unmapped*.
+    ##
+    ## We manage these options lifetimes with a *stack* of options dicts.
+    ##
+    ##  self.options is the options dict at the top of the stack.
+    ##  self.stack is a stack of the remaining options dicts,
+    ##     with the bottom of the stack at self.options_stack[0].
     ##
-    ## This means we only need to undo the creation of
-    ## positional converters.  And those are only ever
-    ## appended to args_converters.  So the undo stack
-    ## is easy: just note each parent converter, and
-    ## for each one,
-    ##     parent_converter.arg_converters.pop()
+    ## An "options token" represents a particular options dict in
+    ## the stack.  Each entry in the stack gets a token.  We then
+    ## store the toke on the option.  This is how we unmap the
+    ## children of a sibling's option; when the user executes an
+    ## option on the command-line, we pop the options stack until
+    ## the options dict mapped to that token is at the top of the
+    ## stack.
     ##
-    ## Note, however, that we need to push/pop the undo
-    ## converters state when we push/pop the context
-    ## (when we start/finish parsing an option).
-
-    converters_are_undoable = True
-    undo_converters_list = []
-    undo_converters_stack = []
-
-    def reset_undo_converters():
-        nonlocal converters_are_undoable
-        converters_are_undoable = True
-        undo_converters_list.clear()
-        if want_prints:
-            print(f"## {ip_spacer} reset_undo_converters()")
-
-    def forget_undo_converters():
-        nonlocal converters_are_undoable
-        undo_converters_list.clear()
-        converters_are_undoable = False
-        if want_prints:
-            print(f"## {ip_spacer} forget_undo_converters()")
-
-    def add_undoable_converter(parent):
-        if converters_are_undoable:
-            undo_converters_list.append(parent)
-            if want_prints:
-                print(f"## {ip_spacer} add_undoable_converter(parent={parent})")
-
-    def push_undo_converters():
-        nonlocal undo_converters_list
-        nonlocal converters_are_undoable
-        undo_converters_stack.append((undo_converters_list, converters_are_undoable))
-        undo_converters_list = []
-        converters_are_undoable = True
-
-    def pop_undo_converters():
-        nonlocal undo_converters_list
-        nonlocal converters_are_undoable
-        undo_converters_list, converters_are_undoable = undo_converters_stack.pop()
-
-    def undo_converters():
-        print_spacer=True
-        for parent in reversed(undo_converters_list):
-            o = parent.args_converters.pop()
-            if want_prints:
-                if print_spacer:
-                    print(f"##")
-                    print_spacer = False
-                print(f"## {ip_spacer} undo converter")
-                print(f"## {ip_spacer}     parent={parent}")
-                print(f"## {ip_spacer}     popped o={o}")
-                print(f"## {ip_spacer}     arg_converters={parent.args_converters}")
-        undo_converters_list.clear()
-
-    if want_prints:
-        charm_separator_line = f"############################################################"
-        print(charm_separator_line)
-        print("##")
-        print('## charm_parse start')
-        print('##')
-        print('## create initial options bucket')
-
-    # create our first actual options bucket
-    push_options()
-    # ... but remove the useless None in the stack
-    options_stack.clear()
-
-    waiting_op = None
-    prev_op = None
-    while ci or argi:
-        if want_prints:
-            print('##')
-            print(charm_separator_line)
-            print(f"## cmdline {list(argi.values)}")
-
-        # first, run ci until we either
-        #    * finish the program, or
-        #    * must consume a command-line argument
-        for op in ci:
-            prev_op = waiting_op
-            waiting_op = op
-
-            if want_prints:
-                ip = f"[{ci.repr_ip()}]"
-                ip_spacer = " " * len(ip)
-                converter = ci.repr_converter(ci.converter)
-                o = ci.repr_converter(ci.o)
-                _total = ci.total and ci.total.summary()
-                _group = ci.group and ci.group.summary()
-                print(f"##")
-                print(f"## {ip} converter={converter} o={o}")
-                print(f"## {ip_spacer} - total={_total}")
-                print(f"## {ip_spacer} - group={_group}")
 
-            if op.op == opcode.create_converter:
-                r = None if op.parameter.kind == KEYWORD_ONLY else root
-                cls = appeal.map_to_converter(op.parameter)
-                converter = cls(op.parameter, appeal)
-                ci.converters[op.key] = ci.o = converter
-                if not root:
-                    root = converter
-                if want_prints:
-                    print(f"## {ip_spacer} create_converter key={op.key} parameter={op.parameter}")
-                    print(f"## {ip_spacer}   converter={converter}")
-                continue
+    @big.BoundInnerClass
+    class Options:
 
-            if op.op == opcode.load_converter:
-                ci.converter = ci.converters.get(op.key, None)
-                converter = ci.repr_converter(ci.converter)
-                if want_prints:
-                    print(f"## {ip_spacer} load_converter op.key={op.key} converter={converter!s}")
-                continue
+        def __init__(self, interpreter):
+            self.interpreter = interpreter
+            self.stack = []
+            self.token_to_dict = {}
+            self.dict_id_to_token = {}
+
+            # We want to sort options tokens.
+            # But serial_number_generator(tuple=True) is ugly and verbose.
+            # This seems nicer.
+
+            class OptionsToken:
+                def __init__(self, i):
+                    self.i = i
+                    self.repr = f"<options-{self.i}>"
+                def __repr__(self):
+                    return self.repr
+                def __lt__(self, other):
+                    return self.i < other.i
+                def __eq__(self, other):
+                    return self.i == other.i
+                def __hash__(self):
+                    return self.i
+
+            def token_generator():
+                i = 1
+                while True:
+                    yield OptionsToken(i)
+                    i += 1
+
+            self.next_token = token_generator().__next__
+            self.reset()
+
+        def reset(self):
+            self.options = options = {}
+            self.token = token = self.next_token()
+            self.token_to_dict[token] = options
+            self.dict_id_to_token[id(options)] = token
+            return token
+
+        def push(self):
+            self.stack.append((self.options, self.token))
+            token = self.reset()
+
+            # if want_prints:
+            #     print(f"{self.interpreter.cmdline_prefix} {self.interpreter.ip_spacer} Options.push, new options group {token}")
+
+        def pop(self):
+            options_id = id(self.options)
+            token = self.dict_id_to_token[options_id]
+            del self.dict_id_to_token[options_id]
+            del self.token_to_dict[token]
+
+            options, token = self.stack.pop()
+            self.options = options
+            self.token = token
+
+            # if want_prints:
+            #     options = [denormalize_option(option) for option in options]
+            #     options.sort(key=lambda s: s.lstrip('-'))
+            #     options = "{" + " ".join(options) + "}"
+            #     print(f"{self.interpreter.cmdline_prefix} {self.interpreter.ip_spacer} Options.pop: popped to options group {token}, options={options}")
 
-            if op.op == opcode.load_o:
-                ci.o = ci.converters.get(op.key, None)
-                if want_prints:
-                    o = ci.repr_converter(ci.o)
-                    print(f"## {ip_spacer} load_o op.key={op.key} o={o!s}")
-                continue
+        def pop_until_group(self, token):
+            if self.token == token:
+                # if want_prints:
+                #     print(f"{self.interpreter.cmdline_prefix} {self.interpreter.ip_spacer} Options.pop_until_group: current group has token {token}.  popped 0 times.")
+                return
+            options_to_stop_at = self.token_to_dict.get(token)
+            if not options_to_stop_at:
+                raise ValueError(f"Options.pop_until_token: specified non-existent options group token={token}")
+
+            count = 0
+            while self.stack and (self.options != options_to_stop_at):
+                count += 1
+                self.pop()
+
+            if self.options != options_to_stop_at:
+                raise ValueError(f"Options.pop_until_token: couldn't find options group with token={token}")
+
+            # if want_prints:
+            #     print(f"{self.interpreter.cmdline_prefix} {self.interpreter.ip_spacer} Options.pop_until_group: popped {count} times, down to options group {token}.")
+
+        def unmap_all_child_options(self):
+            """
+            This unmaps all the *child* options.
+
+            Note that we're only emptying the stack.
+            self.options is the top of the stack, and we aren't
+            blowing that away.  So when we empty self.stack,
+            there's still one options dict left, which was at the
+            bottom of the stack; this is the bottom options dict,
+            where all the permanently-mapped options live.
+            """
+            count = len(self.stack)
+            for _ in range(count):
+                self.pop()
+
+            # if want_prints:
+            #     print(f"{self.interpreter.cmdline_prefix} Options.unmap_all_child_options: popped {count} times.")
+
+        def __getitem__(self, option):
+            depth = 0
+            options = self.options
+            token = self.token
+            i = reversed(self.stack)
+            while True:
+                t = options.get(option, None)
+                if t is not None:
+                    break
+                try:
+                    options, token = next(i)
+                except StopIteration:
+                    parent_options = self.interpreter.program.option_to_parent_options.get(option)
+                    if parent_options:
+                        # parent_options = parent_options.replace("|", "or")
+                        parent_options = ", ".join(denormalize_option(o) for o in parent_options)
+                        fields = parent_options.rpartition(", ")
+                        if fields[1]:
+                            fields[1] = ' or '
+                        parent_options = "".join(fields)
+                        message = f"{denormalize_option(option)} can't be used here, it must be used immediately after {parent_options}"
+                    else:
+                        message = f"unknown option {denormalize_option(option)}"
+                    raise AppealUsageError(message) from None
 
-            if op.op == opcode.map_option:
-                options_bucket[op.option] = op.program
-                if want_prints:
-                    print(f"## {ip_spacer} map_option op.option={op.option} op.program={op.program} token {options_token}")
-                continue
+            program, group_id = t
+            total = program.total
+            return program, group_id, total.minimum, total.maximum, token
 
-            if op.op == opcode.append_args:
-                ci.converter.args_converters.append(ci.o)
-                add_undoable_converter(ci.converter)
-                if want_prints:
-                    o = ci.repr_converter(ci.o)
-                    print(f"## {ip_spacer} append_args o={o}")
-                continue
+        def __setitem__(self, option, value):
+            self.options[option] = value
 
-            if op.op == opcode.store_kwargs:
-                converter = ci.o
-                if op.name in ci.converter.kwargs_converters:
-                    existing = ci.converter.kwargs_converters[op.name]
-                    if not ((existing == converter) and isinstance(existing, MultiOption)):
-                        raise AppealUsageError(f"{program.name} specified more than once.")
-                    # we're setting the kwarg to the value it's already set to,
-                    # and it's a multioption, so this is fine.
-                    continue
-                ci.converter.kwargs_converters[op.name] = ci.o
-                if want_prints:
-                    o = ci.repr_converter(ci.o)
-                    print(f"## {ip_spacer} store_kwargs name={op.name} o={o}")
-                continue
 
-            if op.op == opcode.consume_argument:
-                if want_prints:
-                    print(f"## {ip_spacer} consume_argument is_oparg={op.is_oparg}")
-                if not argi:
-                    if want_prints:
-                        print(f"## {ip_spacer}     no more arguments, aborting program")
-                    ci.abort()
-                break
 
-            if op.op == opcode.push_context:
-                ci.push_context()
-                push_undo_converters()
-                if want_prints:
-                    print(f"## {ip_spacer} push_context")
-                continue
 
-            if op.op == opcode.pop_context:
-                pop_undo_converters()
-                ci.pop_context()
-                if want_prints:
-                    print(f"## {ip_spacer} pop_context")
-                continue
+    def __call__(self):
+        (
+        option_space_oparg,
 
-            if op.op == opcode.set_group:
-                ci.group = op.group.copy()
-                reset_undo_converters()
-                if want_prints:
-                    print(f"## {ip_spacer} set_group {ci.group.summary()}")
-                continue
+        short_option_equals_oparg,
+        short_option_concatenated_oparg,
+        ) = self.appeal.root.option_parsing_semantics
 
-            if op.op == opcode.flush_multioption:
-                assert isinstance(ci.o, MultiOption), f"expected instance of MultiOption but ci.o={ci.o}"
-                ci.o.flush()
-                if want_prints:
-                    o = ci.repr_converter(ci.o)
-                    print(f"## {ip_spacer} flush_multioption o={o}")
-                continue
+        # def print(s=None):
+        #     if not s:
+        #         return
+        #     with open("/tmp/xyz", "at") as f:
+        #         f.write(s + "\n")
 
-            if op.op == opcode.jump:
-                if want_prints:
-                    print(f"## {ip_spacer} jump op.address={op.address}")
-                ci.i.jump(op.address)
-                continue
+        if self.processor:
+            self.processor.log.enter(f"interpreter {self.program}")
 
-            if op.op == opcode.branch_on_o:
-                if want_prints:
-                    print(f"## {ip_spacer} branch_on_o o={ci.o} op.address={op.address}")
-                if ci.o:
-                    ci.i.jump(op.address)
-                continue
+        iterator = self.iterator
+        mapping = self.mapping
 
-            if op.op == opcode.comment:
-                if want_prints:
-                    print(f"## {ip_spacer} comment {op.comment!r}")
-                continue
+        id_to_group = {}
 
-            if op.op == opcode.end:
-                if want_prints:
-                    name = str(op.op).partition(".")[2]
-                    print(f"## {ip_spacer} {name} id={op.id} name={op.name!r}")
-                continue
+        command_converter = None
 
-            raise AppealConfigurationError(f"unhandled opcode op={op}")
+        force_positional = self.appeal.root.force_positional
 
-        else:
-            # we finished the program
-            if want_prints:
-                print(f"##")
-                print(f"## program finished.")
-                print(f"##")
-            op = None
-            forget_undo_converters()
-
-        assert (op == None) or (op.op == opcode.consume_argument)
-
-        # it's time to consume arguments.
-        # we've either paused or finished the program.
-        #   if we've paused, it's because the program wants us
-        #     to consume an argument.  in that case op
-        #     will be a 'consume_argument' op.
-        #   if we've finished the program, op will be None.
-        #
-        # technically this is a for loop over argi, but
-        # we usually only consume one argument at a time.
-        #
-        # for a in argi:
-        #    * if a is an option (or options),
-        #      push that program (programs) and resume
-        #      the charm interpreter.
-        #    * if a is the special value '--', remember
-        #      that all subsequent command-line arguments
-        #      can no longer be options, and continue to
-        #      the next a in argi.  (this is the only case
-        #      in which we'll consume more than one argument
-        #      in this loop.)
-        #    * else a is a positional argument.
-        #      * if op is consume_argument, consume it and
-        #        resume the charm interpreter.
-        #      * else, hmm, we have a positional argument
-        #        we don't know what to do with.  the program
-        #        is done, and we don't have a consume_argument
-        #        to give it to.  so push it back onto argi
-        #        and exit.  (hopefully the argument is the
-        #        name of a command/subcomand.)
-
-        for a in argi:
-            if want_prints:
-                print("#[]")
-
-            is_oparg = op and (op.op == opcode.consume_argument) and op.is_oparg
-            # if this is true, we're consuming a top-level command-line argument.
-            # if this is false, we're processing an oparg.
-            # what's the difference? opargs can't be options.
-            is_positional_argument = (
-                appeal.root.force_positional
-                or ((not a.startswith("-")) or (a == "-"))
-                or is_oparg
-                )
+        # if want_prints:
+        #     self.ip_spacer = '    '
 
-            if want_prints:
-                # print_op = "consume_argument" if op else None
-                print_op = op
-                print(f"#[]  process argument {a!r} {list(argi.values)}")
-                print(f"#[]  op={print_op}")
-
-            if is_positional_argument:
-                if not op:
-                    if want_prints:
-                        print(f"#[]  positional argument we can't handle.  exit.")
-                    argi.push(a)
-                    return ci.converters[0]
-
-                ci.o = a
-                forget_undo_converters()
-                if ci.group:
-                    ci.group.count += 1
-                if ci.total:
-                    ci.total.count += 1
-                if not is_oparg:
-                    pop_options_to_base()
-                if want_prints:
-                    print(f"#[]  positional argument.  o={ci.o!r}")
-                # return to the interpreter
-                break
+        # if want_prints:
+        #     charm_separator_line = f"{self.opcodes_prefix}{'-' * 58}"
+        #     print(charm_separator_line)
+        #     print(f"{self.opcodes_prefix}")
+        #     print(f'{self.opcodes_prefix} CharmInterpreter start')
+        #     print(f"{self.opcodes_prefix}")
+        #     all_options = list(denormalize_option(o) for o in self.program.option_to_child_options)
+        #     all_options.sort(key=lambda s: s.lstrip('-'))
+        #     all_options = " ".join(all_options)
+        #     print(f"{self.opcodes_prefix} all options supported: {all_options}")
+
+        waiting_op = None
+        prev_op = None
+
+        ip_zero = f"[{self.repr_ip(0)}]"
+        self.ip_spacer = " " * len(ip_zero)
+        self.register_spacer = " " * len(ip_zero)
+
+        sentinel = object()
+
+        register_width = 20
+        total_register_width = len(ip_zero) + 1 + register_width
+
+        def print_registers(**kwargs):
+            """
+            Call this *after* changing registers.
+            Pass in the *old value* of every registers
+            you changed, as a keyword argument named
+            for the register.
+
+            If you don't change any registers,
+            you should still call this, for
+            visual consistency.
+
+            (Why *changed* instead of *changing*?
+            That made it easier to copy with the
+            two-phase loop and printing next_to_o.)
+            """
+            nonlocal register_width
+
+            def format_options_group(token):
+                l = list(self.options.stack)
+                l.append((self.options.options, self.options.token))
+                l2 = list()
+                for t in l:
+                    l2.append(t)
+                    if t[1] == token:
+                        break
+                l2.reverse()
+                strings = [f"{token} {list(group)}" for group, token in l2]
+                s = " ".join(strings)
+                return s
+
+            for t in (
+                ('converter', None, self.repr_converter),
+                ('o', None, self.repr_converter),
+                ('flag', None, lambda value: str(bool(value))),
+                ('group', None, lambda value: value.summary() if value else repr(value) ),
+                ('groups', None, lambda value: str([group.id for group in value])),
+                ('iterator', None, str),
+                ('mapping', None, lambda value: 'None' if value is None else " ".join(k for k in value.keys())),
+                ('options group', 'options.token', format_options_group),
+                ):
+                name, attr, format = t
+                attr = attr or name
+
+                value = self
+
+                for field in attr.split('.'):
+                    value = getattr(value, field)
+
+                fields = [name.rjust(register_width), "|   "]
+
+                old = kwargs.pop(name, sentinel)
+                changed = (old != sentinel) and (value != old)
+                if changed:
+                    fields.append(format(old))
+                    fields.append("->")
+
+                fields.append(format(value))
+
+                result = " ".join(fields)
+                if len(result) < 50:
+                    print(f"{self.opcodes_prefix} {self.register_spacer} {result}")
+                else:
+                    # split it across two lines
+                    print(f"{self.opcodes_prefix} {name:>{total_register_width}} |    {fields[2]}")
+                    if changed:
+                        print(f"{self.opcodes_prefix} {'':{total_register_width}} | -> {fields[-1]}")
+
+            extras = kwargs.pop('extras', ())
+            assert not kwargs
+            # if they passed in *extra* stuff, just print it normal
+            for name, old, new in extras:
+                if (old != sentinel) and (old != new):
+                    print(f"{self.opcodes_prefix} {name:>{total_register_width}} |    {old}")
+                    print(f"{self.opcodes_prefix} {'  ':>{total_register_width}} | -> {new}")
+                else:
+                    print(f"{self.opcodes_prefix} {name:>{total_register_width}} |    {new}")
+
+        while self.running() or iterator:
+            # if want_prints:
+            #     print(f'{self.opcodes_prefix}')
+            #     print(charm_separator_line)
+            #     if iterator is not None:
+            #         try:
+            #             printable_iterator = shlex_join(list(reversed(iterator.stack)))
+            #         except TypeError:
+            #             printable_iterator = repr(iterator)
+            #     else:
+            #         printable_iterator = "None"
+            #     print(f"{self.opcodes_prefix} iterator: {printable_iterator}")
+
+            # The main interpreter loop.
+            #
+            # This loop has two "parts".
+            #
+            # In the first part, we iterate over bytecodes until either
+            #    * we finish the program, or
+            #    * we must consume a command-line argument
+            #      (we encounter a "next_to_o" bytecode).
+            # If we finish the program, obviously, we're done.
+            # If we must consume a command-line argument, we proceed
+            # to the second "part".
+            #
+            # In the second part, we consume a command-line argument.
+            # If it's an option, we process the option, and loop.
+            # If it's not an option, we consume it as normal and continue.
+
+            # First "part" of the loop: iterate over bytecodes.
+            # if want_prints:
+            #     print(f"{self.opcodes_prefix}")
+            #     print(f"{self.opcodes_prefix} loop part one: execute program {self.program}")
+            #     program_printed = self.program
+
+            for ip, op in self:
+                prev_op = waiting_op
+                waiting_op = op
 
-            # it's an option!  or "--".
+                # if want_prints:
+                #     print(f"{self.opcodes_prefix} ")
+                #     if program_printed != self.program:
+                #         print(f"{self.opcodes_prefix} now running program {self.program}")
+                #         program_printed = self.program
+                #         print(f"{self.opcodes_prefix} ")
+                #
+                #     prefix = f"[{self.repr_ip(ip)}]"
+
+                if op.op == opcode.load_converter:
+                    # if want_prints:
+                    #     old_converter = self.converter
+                    #     old_flag = self.flag
+                    converter = self.converters.get(op.key, sentinel)
+                    if converter is sentinel:
+                        converter = None
+                        self.flag = False
+                    else:
+                        self.flag = True
+                    self.converter = converter
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} load_converter | key {op.key}")
+                    #     print_registers(converter=old_converter, flag=old_flag)
+                    continue
+
+                if op.op == opcode.load_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    #     old_flag = self.flag
+                    o = self.converters.get(op.key, sentinel)
+                    if o is sentinel:
+                        o = None
+                        self.flag = False
+                    else:
+                        self.flag = True
+                    self.o = o
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} load_o | key {op.key}")
+                    #     print_registers(o=old_o, flag=old_flag)
+                    continue
 
-            if not option_space_oparg:
-                raise AppealConfigurationError("oops, option_space_oparg must currently be True")
+                if op.op == opcode.converter_to_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    self.o = self.converter
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} converter_to_o")
+                    #     print_registers(o=old_o)
+                    continue
 
-            queue = []
-            option_stack_tokens = []
+                if op.op == opcode.next_to_o:
+                    # proceed to second part of interpreter loop
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} next_to_o | switching from loop part 1 to loop part 2")
+                    break
 
-            # split_value is the value we "split" from the option string.
-            #  --option=X
-            #  -o=X
-            #  -oX
-            # it's set to X if the user specifies an X, otherwise it's None.
-            split_value = None
-
-            if a.startswith("--"):
-                if a == "--":
-                    # we shouldn't be able to reach this twice.
-                    # if the user specifies -- twice on the command-line,
-                    # the first time turns of option processing, which means
-                    # it should be impossible to get here.
-                    assert not appeal.root.force_positional
-                    appeal.root.force_positional = True
-                    if want_prints:
-                        print(f"#[]  '--', force_positional=True")
-                    continue
-
-                option, equals, _split_value = a.partition("=")
-                if equals:
-                    split_value = _split_value
-
-                program, maximum_arguments, token = find_option(option)
-                option_stack_tokens.append(token)
-                if want_prints:
-                    print(f"#[]  option {denormalize_option(option)} program={program}")
-                queue.append((option, program, maximum_arguments, split_value, True))
-            else:
-                options = collections.deque(a[1:])
+                if op.op == opcode.append_to_converter_args:
+                    o = self.o
+                    converter = self.converter
+                    # if want_prints:
+                    #     if op.discretionary:
+                    #         field_name = "args_queue"
+                    #         new = converter.args_queue
+                    #     else:
+                    #         field_name = "args_converters"
+                    #         new = converter.args_converters
+                    #     old = list(new.copy())
+
+                    # either queue or append o as indicated
+                    (converter.queue_converter if op.discretionary else converter.append_converter)(o)
+
+                    # if want_prints:
+                    #     discretionary = "yes" if op.discretionary else "no"
+                    #     print(f"{self.opcodes_prefix} {prefix} append_to_converter_args | parameter {op.parameter} | discretionary? {discretionary}")
+                    #     new = list(new)
+                    #     print_registers(extras = [
+                    #         (f'{self.converter_to_key(converter)}.{field_name}', old, new),
+                    #         ])
+                    continue
 
-                while options:
-                    option = options.popleft()
-                    equals = short_option_equals_oparg and options and (options[0] == '=')
-                    if equals:
-                        options.popleft()
-                        split_value = "".join(options)
-                        options = ()
-                    program, maximum_arguments, token = find_option(option)
-                    option_stack_tokens.append(token)
-                    # if it takes no arguments, proceed to the next option
-                    if not maximum_arguments:
-                        if want_prints:
-                            print(f"#[]  option {denormalize_option(option)}")
-                        queue.append([denormalize_option(option), program, maximum_arguments, split_value, False])
+                if op.op == opcode.set_in_converter_kwargs:
+                    name = op.name
+                    converter = self.converter
+                    o = self.o
+
+                    existing = converter.kwargs_converters.get(name, sentinel)
+                    if existing is not sentinel:
+                        if not ((existing == o) and isinstance(existing, MultiOption)):
+                            raise AppealUsageError(f"{program.name} specified more than once.")
+                        # we're setting the kwarg to the value it's already set to,
+                        # and it's a multioption.  it's fine, we just ignore it.
                         continue
-                    # this eats arguments.  if there are more characters waiting,
-                    # they must be the split value.
-                    if options:
-                        assert not split_value
-                        split_value = "".join(options)
-                        options = ()
-                        if not short_option_concatenated_oparg:
-                            raise AppealUsageError(f"'-{option}{split_value}' is not allowed, use '-{option} {split_value}'")
-                    if want_prints:
-                        print(f"#[]  option {denormalize_option(option)}")
-                    queue.append([denormalize_option(option), program, maximum_arguments, split_value, False])
-
-                # mark the last entry in the queue as last
-                queue[-1][-1] = True
-
-            assert queue and option_stack_tokens
-
-            # we have options to run.
-            # so the existing consume_argument op will have to wait.
-            if op:
-                ci.rewind()
+
+                    # if want_prints:
+                    #     new = converter.kwargs_converters
+                    #     old = new.copy()
+
+                    converter.unqueue()
+                    converter.kwargs_converters[name] = o
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} set_in_converter_kwargs | name {op.name}")
+                    #     print_registers(extras = [
+                    #         (f'{self.converter_to_key(converter)}.kwargs_converters', old, new),
+                    #         ])
+
+                    continue
+
+                if op.op == opcode.lookup_to_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    #     old_flag = self.flag
+
+                    value = mapping.get(op.key, sentinel)
+                    if value != sentinel:
+                        self.flag = True
+                        abort = False
+                    else:
+                        self.flag = False
+                        abort = op.required
+                        value = None
+
+                    self.o = value
+                    # if want_prints:
+                    #     required_yes_no = "yes" if op.required else "no"
+                    #     print(f"{self.opcodes_prefix} {prefix} lookup_to_o | key='{op.key}' | required? {required_yes_no}")
+                    #     abort_yes_no = "yes" if abort else "no"
+                    #     print_registers(o=old_o, flag=old_flag, extras=[('abort?', sentinel, abort_yes_no)])
+
+                    if abort:
+                        return self.abort()
+                    continue
+
+                if op.op == opcode.flush_multioption:
+                    assert isinstance(self.o, MultiOption), f"expected o to contain instance of MultiOption but o={self.o}"
+                    self.o.flush()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} flush_multioption")
+                    #     print_registers()
+                    continue
+
+                if op.op == opcode.remember_converters:
+                    self.remember_converters()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} remember_converters")
+                    #     print_registers()
+                    continue
+
+                if op.op == opcode.forget_converters:
+                    self.forget_converters()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} forget_converters")
+                    #     print_registers()
+                    continue
+
+                if op.op == opcode.map_option:
+                    # go-faster stripe!
+                    # map_option opcodes tend to clump together.
+                    # so, run a mini-interpreter loop here to
+                    # process all the map instructions at once.
+                    self.rewind_one_instruction()
+                    for ip, op in self:
+                        if op.op != opcode.map_option:
+                            break
+                        self.options[op.option] = (op.program, op.group)
+                        # if want_prints:
+                        #     print(f"{self.opcodes_prefix} {prefix} map_option | '{denormalize_option(op.option)}' -> {op.program} | options group {self.options.token}")
+                        #     print_registers()
+                    self.rewind_one_instruction()
+                    continue
+
+                if op.op == opcode.create_converter:
+                    # go-faster stripe!
+                    # create_converter opcodes tend to clump together.
+                    # so, run a mini-interpreter loop here to
+                    # process all the map instructions at once.
+                    self.rewind_one_instruction()
+                    for ip, op in self:
+                        if op.op != opcode.create_converter:
+                            break
+
+                        cls = self.appeal.map_to_converter(op.parameter)
+                        converter = cls(op.parameter, self.appeal)
+                        old_o = self.o
+                        self.converters[op.key] = self.o = converter
+                        if not command_converter:
+                            command_converter = converter
+                            self.command_converter_key = op.key
+
+                        if self.converter_keys is not None:
+                            self.converter_keys.add(op.key)
+
+                        # if want_prints:
+                        #     print(f"{self.opcodes_prefix} {prefix} create_converter | cls {cls.__name__} | parameter {op.parameter.name} | key {op.key}")
+                        #     print_registers(o=old_o)
+                    self.rewind_one_instruction()
+                    continue
+
+                if op.op == opcode.set_group:
+                    # if want_prints:
+                    #     if self.group is None:
+                    #         old_group = None
+                    #     else:
+                    #         old_group = self.group
+                    #     old_groups = self.groups.copy()
+                    self.group = group = op.group.copy()
+                    self.groups.append(group)
+                    id_to_group[group.id] = group
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} set_group")
+                    #     print_registers(group=old_group, groups=old_groups)
+                    continue
+
+                if op.op == opcode.jump:
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} jump | op.address {op.address}")
+                    #     print_registers()
+                    self.ip.jump(op.address)
+                    continue
+
+                if op.op == opcode.indirect_jump:
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} indirect_jump")
+                    #     print_registers()
+                    self.ip.jump(self.o)
+                    continue
+
+                if op.op == opcode.branch_on_flag:
+                    # if want_prints:
+                    #     branch = "yes" if self.flag else "no"
+                    #     print(f"{self.opcodes_prefix} {prefix} branch_on_flag | branch? {branch} | address {op.address}")
+                    #     print_registers()
+                    if self.flag:
+                        self.ip.jump(op.address)
+                    continue
+
+                if op.op == opcode.branch_on_not_flag:
+                    # if want_prints:
+                    #     branch = "yes" if (not self.flag) else "no"
+                    #     print(f"{self.opcodes_prefix} {prefix} branch_on_not_flag | branch? {branch} | address {op.address}")
+                    #     print_registers()
+                    if not self.flag:
+                        self.ip.jump(op.address)
+                    continue
+
+                if op.op == opcode.test_is_o_true:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    self.flag = bool(self.o)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_true")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.test_is_o_none:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    self.flag = self.o == None
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_none")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.test_is_o_empty:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    self.flag = self.o == empty
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_empty")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.test_is_o_iterable:
+                    # if want_prints:
+                    #     old_flag = self.flag
+
+                    # self.flag = isinstance(self.o, Iterator)
+                    self.flag = isinstance(self.o, Iterable)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_iterable")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.test_is_o_mapping:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    self.flag = isinstance(self.o, Mapping)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_mapping")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.test_is_o_str_or_bytes:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    self.flag = isinstance(self.o, (str, bytes))
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} test_is_o_str_or_bytes")
+                    #     print_registers(flag=old_flag)
+                    continue
+
+                if op.op == opcode.push_o:
+                    # if want_prints:
+                    #     old_data_stack = self.data_stack.copy()
+                    self.data_stack.append(self.o)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} push_o")
+                    #     print_registers(extras=[('data stack', old_data_stack, self.data_stack)])
+                    continue
+
+                if op.op == opcode.pop_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    #     old_data_stack = self.data_stack.copy()
+                    self.o = self.data_stack.pop()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} pop_o")
+                    #     print_registers(o=old_o, extras=[('data stack', old_data_stack, self.data_stack)])
+                    continue
+
+                if op.op == opcode.peek_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    self.o = self.data_stack[-1]
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} peek_o")
+                    #     print_registers(o=old_o)
+                    continue
+
+                if op.op == opcode.push_flag:
+                    # if want_prints:
+                    #     old_data_stack = self.data_stack.copy()
+                    self.data_stack.append(self.flag)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} push_flag")
+                    #     print_registers(extras=[('data stack', old_data_stack, self.data_stack)])
+                    continue
+
+                if op.op == opcode.pop_flag:
+                    # if want_prints:
+                    #     old_flag = self.flag
+                    #     old_data_stack = self.data_stack.copy()
+                    self.flag = self.data_stack.pop()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} pop_flag")
+                    #     print_registers(o=old_o, extras=[('data stack', old_data_stack, self.data_stack)])
+                    continue
+
+                if op.op == opcode.literal_to_o:
+                    # if want_prints:
+                    #     old_o = self.o
+                    self.o = op.value
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} literal_to_o | value={repr(op.value)}")
+                    #     print_registers(o=old_o)
+                    continue
+
+                if op.op == opcode.wrap_o_with_iterator:
+                    # if want_prints:
+                    #     old_o = self.o
+                    self.o = iter((self.o,))
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} wrap_o_with_iterator")
+                    #     print_registers(o=old_o)
+                    continue
+
+                if op.op == opcode.push_mapping:
+                    if not isinstance(self.o, Mapping):
+                        self.abort(f'object in o is not a Mapping, o={o}')
+                    # if want_prints:
+                    #     old_mapping_stack = self.mapping_stack.copy()
+                    self.mapping_stack.append(self.mapping)
+                    self.mapping = mapping = self.o
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} push_mapping")
+                    #     print_registers(extras=[('mapping stack', old_mapping_stack, self.mapping_stack)])
+                    continue
+
+                if op.op == opcode.pop_mapping:
+                    # if want_prints:
+                    #     old_mapping = self.mapping
+                    #     old_mapping_stack = self.mapping_stack.copy()
+                    self.mapping = mapping = self.mapping_stack.pop()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} pop_mapping")
+                    #     print_registers(mapping=old_mapping, extras=[('mapping stack', old_mapping_stack, self.mapping_stack)])
+                    continue
+
+                if op.op == opcode.push_iterator:
+                    if not isinstance(self.o, Iterable):
+                        self.abort(f'object in o is not an Iterator, o={self.o}')
+                    # if want_prints:
+                    #     old_iterator = self.iterator
+                    #     old_iterator_stack = self.iterator_stack.copy()
+                    self.iterator_stack.append(self.iterator)
+                    iterator = big.PushbackIterator(self.o)
+
+                    # if want_prints:
+                    #     # allow us to print the remaining contents of the iterator
+                    #     # by examining its stack
+                    #     l = list(iterator)
+                    #     l.reverse()
+                    #     iterator.stack.extend(l)
+                    #     iterator.i = None
+
+                    self.iterator = iterator
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} push_iterator")
+                    #     print_registers(iterator=old_iterator, extras=[('iterator stack', old_iterator_stack, self.iterator_stack)])
+                    continue
+
+                if op.op == opcode.pushback_o_to_iterator:
+                    if self.iterator is None:
+                        self.abort(f'iterator not set')
+                    self.iterator.push(self.o)
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} pushback_o_to_iterator")
+                    #     print_registers()
+                    continue
+
+                if op.op == opcode.pop_iterator:
+                    # if want_prints:
+                    #     old_iterator = self.iterator
+                    #     old_iterator_stack = self.iterator_stack.copy()
+                    self.iterator = iterator = self.iterator_stack.pop()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} pop_iterator")
+                    #     print_registers(iterator=old_iterator, extras=[('iterator stack', old_iterator_stack, self.iterator_stack)])
+                    continue
+
+                if op.op == opcode.comment:
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} # {op.comment!r}")
+                    continue
+
+                if op.op == opcode.no_op:
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} no_op")
+                    continue
+
+                if op.op == opcode.end:
+                    # if want_prints:
+                    #     cpse = self.CharmProgramStackEntry()
+                    self.end()
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} end")
+                    #     print_registers(
+                    #         converter=cpse.converter,
+                    #         o=cpse.o,
+                    #         flag=cpse.flag,
+                    #         group=cpse.group,
+                    #         groups=cpse.groups,
+                    #         )
+                    continue
+
+                if op.op == opcode.abort:
+                    # if want_prints:
+                    #     print(f"{self.opcodes_prefix} {prefix} abort | message '{op.message}'")
+                    #     print_registers()
+                    self.abort(op.message)
+                    continue
+
+                if op.op == opcode.create_converter:
+                    raise RuntimeError("huh? we should have handled all create_converter opcodes already.")
+
+                raise AppealConfigurationError(f"unhandled opcode | op {op}")
+
+            else:
+                # we finished the program
+                # if want_prints:
+                #     print(f"{self.opcodes_prefix} ")
+                #     if self.aborted:
+                #         print(f"{self.opcodes_prefix} aborted!")
+                #     else:
+                #         print(f"{self.opcodes_prefix} ended.")
+                #     print(f"{self.opcodes_prefix} ")
                 op = None
 
-            # pop to the *lowest* bucket!
-            option_stack_tokens.sort()
-            pop_options_to_token(option_stack_tokens[0])
-
-            # and now push on a new bucket.
-            push_options()
-
-            # process options in reverse here!
-            # that's because we push each program on the interpreter.  so, LIFO.
-            for error_option, program, maximum_arguments, split_value, is_last in reversed(queue):
-                if want_prints:
-                    print(f"#[]  executing option {option} split_value={split_value}")
-                    print(f"#[]  call program={program}")
-
-                if not is_last:
-                    total = program.total
-                    assert maximum_arguments == 0
-
-                if split_value is not None:
-                    assert is_last
-                    if maximum_arguments != 1:
-                        if maximum_arguments == 0:
-                            raise AppealUsageError(f"{error_option} doesn't take an argument")
-                        if maximum_arguments >= 2:
-                            raise AppealUsageError(f"{error_option} given a single argument but it requires multiple arguments, you must separate the arguments with spaces")
-                    argi.push(split_value)
-                    if want_prints:
-                        print(f"#[]  pushing split value {split_value!r} on argi")
+            if self.aborted:
+                break
 
-                ci.call(program)
-            break
 
-    undo_converters()
-    satisfied = True
-    if ci.total and not ci.total.satisfied():
-        satisfied = False
-        ag = ci.total
-    if ci.group and not ci.group.satisfied():
-        if (not ci.group.optional) or ci.group.count:
-            satisfied = False
-            ag = ci.group
-
-    if not satisfied:
-        if not ci.group.satisfied():
-            which = "in this argument group"
-            ag = ci.group
-        else:
-            which = "total"
-            ag = ci.total
-        if ag.minimum == ag.maximum:
-            plural = "" if ag.minimum == 1 else "s"
-            middle = f"{ag.minimum} argument{plural}"
-        else:
-            middle = f"at least {ag.minimum} arguments but no more than {ag.maximum} arguments"
-        program = ci.program
-        message = f"{program.name} requires {middle} {which}."
-
-        raise AppealUsageError(message)
-
-    if want_prints:
-        print(f"##")
-        print(f"## ending parse.")
-        finished_state = "did not finish" if ci else "finished"
-        print(f"##      program {finished_state}.")
-        if argi:
-            print(f"##      remaining cmdline: {list(argi.values)}")
-        else:
-            print(f"##      cmdline was completely consumed.")
-        print(f"############################################################")
-        print()
+            # Second "part" of the loop: consume a positional argument from the command-line.
+            #
+            # We've either paused or finished the program.
+            #   If we've paused, it's because the program wants us
+            #     to consume an argument.  In that case op
+            #     will be a 'next_to_o' op.
+            #   If we've finished the program, op will be None.
+            assert (op == None) or (op.op == opcode.next_to_o), f"op={op}, expected either None or next_to_o"
 
-    return ci.converters[0]
+            # Technically we *loop* over iterator.
+            # But in practice we usually only consume one argument at a time.
+            #
+            # for a in iterator:
+            #    * if a is an option (or options),
+            #      push that program (programs) and resume
+            #      the charm interpreter.
+            #    * if a is the special value '--', remember
+            #      that all subsequent command-line arguments
+            #      can no longer be options, and continue to
+            #      the next a in iterator.  (this is the only case
+            #      in which we'll consume more than one argument
+            #      in this loop.)
+            #    * else a is a positional argument.
+            #      * if op is next_to_o, consume it and
+            #        resume the charm interpreter.
+            #      * else, hmm, we have a positional argument
+            #        we don't know what to do with.  the program
+            #        is done, and we don't have a next_to_o
+            #        to give it to.  so push it back onto iterator
+            #        and exit.  (hopefully the argument is the
+            #        name of a command/subcomand.)
 
+            # if want_prints:
+            #     print_loop_start = True
 
-class SpecialSection:
-    def __init__(self, name, topic_names, topic_values, topic_definitions, topics_desired):
-        self.name = name
+            stay_in_loop_two = True
 
-        # {"short_name": "fn_name.parameter_name" }
-        self.topic_names = topic_names
-        # {"fn_name.parameter_name": "usage_name"}
-        self.topic_values = topic_values
-        # {"fn_name.parameter_name": docs... }
-        self.topic_definitions = topic_definitions
+            while stay_in_loop_two:
+                # if want_prints:
+                #     if print_loop_start:
+                #         if iterator is not None:
+                #             try:
+                #                 printable_iterator = shlex_join(list(reversed(iterator.stack)))
+                #             except TypeError:
+                #                 printable_iterator = repr(iterator)
+                #         else:
+                #             printable_iterator = "None"
+                #         print(f"{self.cmdline_prefix} ")
+                #         print(f"{self.cmdline_prefix} loop part 2: consume argument(s): op={op} iterator: {printable_iterator}")
+                #         print(f"{self.cmdline_prefix} ")
+                #         print_loop_start = False
+
+                if not iterator:
+                    # we need a positional argument, but we don't have one.
+                    # stop processing; we'll figure out if there was an error below.
+                    if self.ip:
+                        self.ip.end()
+                    self.call_stack.clear()
+                    break
 
-        # Appeal's "composable documentation" feature means that it merges
-        # up the docs for arguments and options from child converters.
-        # But what about opargs?  Those are "arguments" from the child
-        # converter tree, but you probably don't want them merged.
-        #
-        # So topics_desired lets you specify which topics Appeal should
-        # merge.
-        self.topics_desired = topics_desired
+                for a in iterator:
+                    # if want_prints:
+                    #     try:
+                    #         printable_iterator = shlex_join(list(reversed(iterator.stack)))
+                    #     except TypeError:
+                    #         printable_iterator = repr(iterator)
+                    #     print(f"{self.cmdline_prefix} argument: {a!r}  remaining: {printable_iterator}")
+                    #     print(f"{self.cmdline_prefix}")
+
+                    # Is this command-line argument a "positional argument", or an "option"?
+                    # In this context, a "positional argument" can be either a conventional
+                    # positional argument on the command-line, or an "oparg".
+
+                    # If force_positional is true, we encountered "--" on the command-line.
+                    # This forces Appeal to ignore dashes and process all subsequent
+                    # arguments as positional arguments.
+
+                    # If we're consuming opargs, we ignore leading dashes,
+                    # and all arguments are forced to be opargs
+                    # until we've consume all the opargs we need.
+                    is_oparg = op and (op.op == opcode.next_to_o) and op.is_oparg
+
+                    is_positional_argument = (
+                        force_positional
+                        or is_oparg
+                        )
+
+                    if (not is_positional_argument) and isinstance(a, str):
+                        # Only do these checks if a is actually a str.
+                        # (If it's a float from a TOML file or something,
+                        # it can't be an option, now can it!)
+
+                        # If the argument doesn't start with a dash,
+                        # it can't be an option, therefore it must be a positional argument.
+                        doesnt_start_with_a_dash = not a.startswith("-")
+
+                        # If the argument is a single dash, it isn't an option,
+                        # it's a positional argument.  This is an old UNIX idiom;
+                        # if you were expecting a filename and you got "-", you should
+                        # use the appropriate stdio file (stdin/stdout) there.
+                        is_a_single_dash = a == "-"
+
+                        is_positional_argument = (
+                            doesnt_start_with_a_dash
+                            or is_a_single_dash
+                            )
+
+                    if is_positional_argument:
+                        if not op:
+                            # if want_prints:
+                            #     print(f"{self.cmdline_prefix}  positional argument we don't want.")
+                            #     print(f"{self.cmdline_prefix}  maybe somebody else will consume it someday.")
+                            #     print(f"{self.cmdline_prefix}  exit.")
+                            iterator.push(a)
+                            return self.converters[self.command_converter_key]
+
+                        # set register "o" to our string and return to running bytecodes.
+                        # if want_prints:
+                        #     old_o = self.o
+                        #     if self.group is None:
+                        #         old_group = None
+                        #     else:
+                        #         old_group = self.group.copy()
+                        self.o = a
+                        self.flag = True
+                        if self.group:
+                            self.group.count += 1
+                            self.group.laden = True
+
+                        if not is_oparg:
+                            self.options.unmap_all_child_options()
+
+                        # if want_prints:
+                        #     print(f"{self.cmdline_prefix}")
+                        #     print(f"{self.opcodes_prefix} {prefix} next_to_o | required={op.required} | is_oparg={op.is_oparg} | usage_name={op.usage_name}")
+                        #     print(f"{self.opcodes_prefix} {prefix} got '{a}'")
+                        #     print_registers(o=old_o, group=old_group)
+
+                        stay_in_loop_two = False
+                        break
+
+                    if not option_space_oparg:
+                        raise AppealConfigurationError("oops, currently the only supported value of option_space_oparg is True")
+
+                    if a == "--":
+                        # we shouldn't be able to reach this twice.
+                        # if the user specifies -- twice on the command-line,
+                        # the first time turns of option processing, which means
+                        # it should be impossible to get here.
+                        assert not force_positional
+                        force_positional = self.appeal.root.force_positional = True
+                        # if want_prints:
+                        #     print(f"{self.cmdline_prefix}  '--', force_positional=True")
+                        continue
 
-        self.topics = {}
-        self.topics_seen = set()
+                    # it's an option!
+                    double_dash = a.startswith("--")
+                    pushed_remainder = False
+
+                    # split_value is the value we "split" from the option string.
+                    # In these example, split_value is 'X':
+                    #     --option=X
+                    #     -o=X
+                    # and, if o takes exactly one optional argument,
+                    # and short_option_concatenated_oparg is true:
+                    #     -oX
+                    # If none of these syntaxes (syntices?) is used,
+                    # split_value is None.
+                    #
+                    # Literally we handle it by splitting it off,
+                    # then pushing it *back* onto iterator, so the option
+                    # program can consume it.  Thus we actually transform
+                    # all the above examples into
+                    #     -o X
+                    #
+                    # Note: split_value can be an empty string!
+                    #     -f=
+                    # So, simply checking truthiness is insufficient.
+                    # You *must* check "if split_value is None".
+                    split_value = None
+
+                    try_to_split_value = double_dash or short_option_equals_oparg
+                    if try_to_split_value:
+                        a, equals, _split_value = a.partition("=")
+                        if equals:
+                            split_value = _split_value
+                    else:
+                        split_value = None
+
+                    if double_dash:
+                        option = a
+                        program, group_id, minimum_arguments, maximum_arguments, token = self.options[option]
+                    else:
+                        ## In Appeal,
+                        ##      % python3 myscript foo -abcde
+                        ## must be EXACTLY EQUIVALENT TO
+                        ##      % python3 myscript foo -a -b -c -d -e
+                        ##
+                        ## The best way to handle this is to transform the former
+                        ## into the latter.  Every time we encounter a single-dash
+                        ## option, consume just the first letter, and if the rest
+                        ## is more options, reconstruct the remaining short options
+                        ## and push it onto the 'iterator' pushback iterator.
+                        ## For example, if -a is an option that accepts no opargs,
+                        ## we transform
+                        ##      % python3 myscript foo -abcde
+                        ## into
+                        ##      % python3 myscript foo -a -bcde
+                        ## and then handle "-a".
+                        ##
+                        ## What about options that take opargs?  Except for
+                        ## the special case of short_option_concatenated_oparg,
+                        ## options that take opargs have to be the last short option.
+
+                        # strip off this short option by itself:
+                        option = a[1]
+                        program, group_id, minimum_arguments, maximum_arguments, token = self.options[option]
+
+                        # handle the remainder.
+                        remainder = a[2:]
+                        if remainder:
+                            if maximum_arguments == 0:
+                                # more short options.  push them back onto iterator.
+                                pushed_remainder = True
+                                remainder = "-" + remainder
+                                iterator.push(remainder)
+                                # if want_prints:
+                                #     print(f"{self.cmdline_prefix} isolating '-{option}', pushing remainder '{remainder}' back onto iterator")
+                            elif maximum_arguments >= 2:
+                                if minimum_arguments == maximum_arguments:
+                                    number_of_arguments = maximum_arguments
+                                else:
+                                    number_of_arguments = f"{minimum_arguments} to {maximum_arguments}"
+                                raise AppealUsageError(f"-{option}{remainder} isn't allowed, -{option} takes {number_of_arguments} arguments, it must be last")
+                            # in the remaining cases, we know maximum_arguments is 1
+                            elif short_option_concatenated_oparg and (minimum_arguments == 0):
+                                # Support short_option_concatenated_oparg.
+                                #
+                                # If a short option takes *exactly* one *optional*
+                                # oparg, you can smash the option and the oparg together.
+                                # For example, if short option "-f" takes exactly one
+                                # optional oparg, and you want to supplythe oparg "guava",
+                                # you can do
+                                #    -f=guava
+                                #    -f guava
+                                # and in ONLY THIS CASE
+                                #    -fguava
+                                #
+                                # Technically POSIX doesn't allow us to support this:
+                                #    -f guava
+                                #
+                                # On the other hand, there's a *long list* of things
+                                # POSIX doesn't allow us to support:
+                                #
+                                #    * short options with '=' (split_value, e.g. '-f=guava')
+                                #    * long options
+                                #    * subcommands
+                                #    * options that take multiple opargs
+                                #
+                                # So, clearly, exact POSIX compliance is not of
+                                # paramount importance to Appeal.
+                                #
+                                # Get with the times, you musty old fogeys!
+
+                                if split_value is not None:
+                                    raise AppealUsageError(f"-{option}{remainder}={split_value} isn't allowed, -{option} must be last because it takes an argument")
+                                split_value = remainder
+                            else:
+                                assert minimum_arguments == maximum_arguments == 1
+                                raise AppealUsageError(f"-{option}{remainder} isn't allowed, -{option} must be last because it takes an argument")
+
+                    laden_group = id_to_group[group_id]
+
+                    denormalized_option = denormalize_option(option)
+                    # if want_prints:
+                    #     print(f"{self.cmdline_prefix} option {denormalized_option}")
+                    #     print(f"{self.cmdline_prefix} {self.ip_spacer} program={program}")
+                    #     print(f"{self.cmdline_prefix} {self.ip_spacer} group={laden_group.summary()}")
+                    #     print(f"{self.cmdline_prefix}")
+
+                    # mark argument group as having had stuff done in it.
+                    laden_group.laden = True
+
+                    # we have an option to run.
+                    # the existing next_to_o op will have to wait.
+                    if op:
+                        assert op.op == opcode.next_to_o
+                        self.rewind_one_instruction()
+                        op = None
+
+                    # throw away child options mapped below our option's sibling.
+                    self.options.pop_until_group(token)
+
+                    # and push a fresh options dict.
+                    self.options.push()
+
+                    if split_value is not None:
+                        if maximum_arguments != 1:
+                            if maximum_arguments == 0:
+                                raise AppealUsageError(f"{denormalized_option}={split_value} isn't allowed, because {denormalize_option} doesn't take an argument")
+                            if maximum_arguments >= 2:
+                                raise AppealUsageError(f"{denormalized_option}={split_value} isn't allowed, because {denormalize_option} takes multiple arguments")
+                        iterator.push(split_value)
+                        # if want_prints:
+                        #     print(f"{self.cmdline_prefix} {self.ip_spacer} pushing split value {split_value!r} back onto iterator")
+
+                    # self.push_context()
+                    self.call(program)
+                    stay_in_loop_two = False
+
+                    # if want_prints:
+                    #     print(f"{self.cmdline_prefix}")
+                    #     print(f"{self.cmdline_prefix} call program={program}")
+                    #     print_registers(extras=[('pushed context', sentinel, self.call_stack[-1])])
+
+                    break
+
+        satisfied = True
+        if self.group:
+            ag = self.group
+            assert ag
+
+            if not ag.satisfied():
+                if ag.minimum == ag.maximum:
+                    plural = "" if ag.minimum == 1 else "s"
+                    middle = f"{ag.minimum} argument{plural}"
+                else:
+                    middle = f"at least {ag.minimum} arguments but no more than {ag.maximum} arguments"
+                program = self.program
+                message = f"{program.name} requires {middle} in this argument group."
+                raise AppealUsageError(message)
+
+        # if want_prints:
+        #     print(f"{self.opcodes_prefix}")
+        #     print(f"{self.opcodes_prefix} ending parse.")
+        #     finished_state = "did not finish" if self else "finished"
+        #     print(f"{self.opcodes_prefix}      program {finished_state}.")
+        #     if iterator:
+        #         print(f"{self.opcodes_prefix}      remaining cmdline: {list(reversed(iterator.stack))}")
+        #     else:
+        #         print(f"{self.opcodes_prefix}      cmdline was completely consumed.")
+
+        # if want_prints:
+        #     print(charm_separator_line)
+        #     print()
+
+        if self.processor:
+            self.processor.log.exit()
+
+        if self.aborted:
+            return None
+
+        return self.converters[self.command_converter_key]
 
 
 
 class Converter:
     """
     A Converter object calls a Python function, filling
     in its parameters using command-line arguments.
     It introspects the function passed in, creating
     a tree of sub-Converter objects underneath it.
 
     A Converter
     """
+    callable = None
     def __init__(self, parameter, appeal):
+        self.parameter = parameter
+        self.appeal = appeal
+
         callable = dereference_annotated(parameter.annotation)
         default = parameter.default
 
         # self.fn = callable
         self.callable = callable
 
         if not hasattr(self, '__signature__'):
             self.__signature__ = self.get_signature(parameter)
 
-        self.appeal = appeal
         # self.root = root or self
         self.default = default
+        self.name = parameter.name
 
         # output of analyze().  input of parse() and usage().
         # self.program = None
 
         self.docstring = self.callable.__doc__
 
         self.usage_str = None
         self.summary_str = None
         self.doc_str = None
 
         self.reset()
 
+    def __repr__(self):
+        return f"<{self.__class__.__name__} callable={self.callable.__name__}>"
+
     @classmethod
     def get_signature(cls, parameter):
         if hasattr(cls, "__signature__"):
             return cls.__signature__
         return inspect.signature(dereference_annotated(parameter.annotation), follow_wrapped=False)
 
     def reset(self):
+        """
+        Called to reset the mutable state of a converter.
+
+        Note that MultiOption is a subclass of Converter,
+        and calls reset() each time it's invoked.
+        """
+
+        # names of parameters that we filled with strings
+        # from the command-line.  if this converter throws
+        # a ValueError or TypeError when executed, and it's
+        # an interior node in the annotations tree, we'll know
+        # exactly which command-line argument failed to convert
+        # and can display more pertinent usage information.
+        self.string_parameters = []
+
+        # queued and args_queue are used to manage converters
+        # that might not actually be needed.  some converters
+        # are created proactively but are never actually used.
+        # Appeal used to queue them, then remove them; queueing
+        # them and not flushing them is easier.
+        #
+        # queued is a flag.  if queued is not None, it points to our
+        #     parent converter, and it represents a request to notify
+        #     the parent when you get a cmdline argument added to
+        #     you--either positional or keyword-only.
+        # args_queue is a list of child converters that are waiting to be
+        #     flushed into our args_converters.
+        #
+        # Note that self.queued may be set to our parent even when we
+        # *aren't* in our parent's args_queue.  Our converter might be
+        # a required argument to our parent, but our parent is optional and
+        # has been queued.  (Or our parent's parent, etc.  It's a tree.)
+        self.queued = None
+        self.args_queue = collections.deque()
+
         # collections of converters we'll use to compute *args and **kwargs.
-        # contains either raw strings or Converter
-        # objects which we'll call.  these are the
-        # output of parse() and the input of convert().
+        # contains either raw strings or Converter objects which we'll call.
+        #
+        # these are the output of parse(), specifically the CharmInterpreter,
+        # and the input of convert().
         self.args_converters = []
         self.kwargs_converters = {}
 
-        # the output of convert(), and the input
-        # for execute().
+        # these are the output of convert(), and the input for execute().
         self.args = []
         self.kwargs = {}
 
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__} callable={self.callable.__name__}>"
+    ## "discretionary" converters, and queueing and unqueueing
+    ##
+    ## If a group is "optional", that means there's at least
+    ## one parameter with a default value.  If that parameter
+    ## has a converter, we don't know in advance whether or not
+    ## we're actually gonna call it.  We'll only call it if we
+    ## fill one of its parameters with a positional argument,
+    ## and we can't really predict in advance whether or not
+    ## that's gonna happen.
+    ##
+    ## For example:
+    ##   * the first actual positional argument is optional
+    ##   * it's nested three levels deep in the annotation tree
+    ##   * we have command-line arguments waiting in iterator
+    ##     but the next argument is an option, and we don't know
+    ##     how many opargs it wants to consume until we run it
+    ##
+    ## Or:
+    ##   * all the parameters to the converter are optional
+    ##   * the converter maps an option
+    ##   * sometime in the deep future the user invokes
+    ##     that option on the command-line
+    ##
+    ## So... when should we create the converter?  The best
+    ## possible time would be "just-in-time", at the moment
+    ## we know we need it and no sooner.  But, the way Appeal
+    ## works internally, it makes things a lot smoother to
+    ## just pre-allocate a converter, then eventually throw it
+    ## away if we don't need it.
+    ##
+    ## Observe that:
+    ##   * First, we're only talking about optional groups.
+    ##     So this only applies to converters that get appended
+    ##     to args.
+    ##       * Converters that handle options get set in kwargs,
+    ##         so there's no mystery about whether or not they're
+    ##         getting used.  Appeal already creates *those*
+    ##         only on demand.
+    ##   * Second, optional groups only become required once we
+    ##     consume an argument in that group, or invoke one of
+    ##     the options mapped in that group.
+    ##
+    ## Here's what Appeal does.  In a nutshell, converters mapped
+    ## in optional groups get created early, but they don't get
+    ## appended to their parent's args_converters right away.
+    ## These converters that we might not need are called
+    ## "discretionary" converters.  Converters that aren't
+    ## discretionary are "mandatory" converters.  A "discretionary"
+    ## converter becomes mandatory at the moment it (or a
+    ## converter below it in the annotations tree) gets a string
+    ## argument from the command-line appended to it, or the user
+    ## invokes an option that maps to one of its (or one of
+    ## its children's) options.
+    ##
+    ## When the CharmInterpreter creates a mandatory converter
+    ## for a positional argument, that converter is immediately
+    ## queued in its parent converter's args_converters list.
+    ## But discretionary converters get "queued", which means
+    ## it goes to a different place: the parent converter's other
+    ## list, args_queue.
+    ##
+    ## At the moment that a discretionary converter becomes
+    ## mandatory--a string from the command-line gets appended
+    ## to that converter, or one of the options it maps gets
+    ## invoked--we "unqueue" that queued converter, moving it
+    ## from its parent's args_queue list to its parent's
+    ## args_converters list.
+    ##
+    ## Two complexities arise from this:
+    ##     * If there's a converter B queued in front of
+    ##       converter A in same parent, and B becomes mandatory,
+    ##       A becomes mandatory too.  And you need to flush
+    ##       it first, so that the parent gets its positional
+    ##       arguments in the right order.  So, when we want to
+    ##       flush a particular converter, we flush all the entries
+    ##       in the queue before it too.
+    ##     * An optional argument group can have an entire tree
+    ##       of converters underneath it, themselves variously
+    ##       optional or required.  So, when a converter has been
+    ##       queued, and it gets a child converter appended to it
+    ##       (or queued to it) it also tells its children "Tell me
+    ##       when I need to unqueue".  If one of these children
+    ##       gets a positional argument that is a string, or gets
+    ##       one of its options invoked, it'll tell its *parent*
+    ##       to unqueue.
+    ##
+    ## Internally, we only use one field in the child converter
+    ## for all this: "queued".
+    ##     * If "queued" is None, the converter is mandatory,
+    ##       and all its parents are mandatory.
+    ##     * If "queued" is not None, either the converter
+    ##       is optional, or one of its parents is optional,
+    ##       and "queued" points to its parent.
+    ##
+    ## -----
+    ##
+    ## One final note.  When I was testing this code against the
+    ## test suite, I was quite surprised to see the same converter
+    ## queued and flushed multiple times.  I investigated, and
+    ## found it wasn't actually the *same* converter, but it had
+    ## the same name and was going in the same place.  It was a
+    ## converter for *args, and the test case looped five times.
+    ## So it actually was five identical but different converters,
+    ## going so far as to use the same converter key.
+    ## (It might be nice to be able to tell them apart in the log.)
+
+    def append_converter(self, o):
+        """
+        Append o directly to our args_converters list.
+
+        If o is not a Converter, also unqueue ourselves
+        (and recursively all our parents too).
+
+        If o is a Converter, and we or one of our parents
+        is discretionary, ask o to notify us if it gets
+        a string positional argument appended to it,
+        or if one of its options is invoked.
+        """
+        # print(f">> {self=} appended to {parent=}\n")
+        self.args_converters.append(o)
+
+        if not isinstance(o, Converter):
+            self.unqueue()
+        else:
+            assert not o.queued
+            # ask
+            if self.queued:
+                o.queued = self
+
+    def queue_converter(self, o):
+        """
+        Append o to our args_queue list.
+        o must be a discretionary Converter object.
+        """
+        # print(f">> {self=} queued for {parent=}\n")
+        assert not o.queued
+        o.queued = self
+        self.args_queue.append(o)
+
+    def unqueue(self, converter=None):
+        """
+        Unqueue ourselves from our parent.
+
+        Also tells our parent to unqueue itself,
+        recursively back up to the root of this
+        discretionary converter subtree.
+
+        Also, if converter is not None,
+        and converter is in our args_queue,
+        converter is a discretionary converter
+        in our args_queue, and we flush the
+        args_queue until converter is unqueued
+        (aka flushed).  If converter isn't in
+        args_queue, args_queue doesn't change.
+        """
+        if self.queued:
+            self.queued.unqueue(self)
+            self.queued = None
+
+        if not converter:
+            return
+
+        try:
+            # if converter isn't in args_queue, this will throw ValueError
+            self.args_queue.index(converter)
+
+            while True:
+                child = self.args_queue.popleft()
+                self.args_converters.append(child)
+                child.queued = None
+                if child == converter:
+                    break
+        except ValueError:
+            pass
 
     def convert(self, processor):
-        # print(f"self={self} self.args_converters={self.args_converters} self.kwargs_converters={self.kwargs_converters}")
         for iterable in (self.args_converters, self.kwargs_converters.values()):
             for converter in iterable:
-                if converter and not isinstance(converter, str):
-                    # print(f"self={self}.convert, converter={converter}")
+                if converter and isinstance(converter, Converter):
                     converter.convert(processor)
 
-        for converter in self.args_converters:
-            if converter and not isinstance(converter, str):
-                converter = converter.execute(processor)
-            self.args.append(converter)
-        for name, converter in self.kwargs_converters.items():
-            if converter and not isinstance(converter, str):
-                converter = converter.execute(processor)
-            self.kwargs[name] = converter
+        try:
+            for converter in self.args_converters:
+                if converter and isinstance(converter, Converter):
+                    converter = converter.execute(processor)
+                self.args.append(converter)
+            for name, converter in self.kwargs_converters.items():
+                if converter and isinstance(converter, Converter):
+                    converter = converter.execute(processor)
+                self.kwargs[name] = converter
+        except ValueError as e:
+            # we can examine "converter", the exception must have
+            # happened in an execute call.
+            raise AppealUsageError(f"invalid value something something {converter=}, {dir(converter)=} {converter.args=}")
 
     def execute(self, processor):
-        # print(f"calling {self.callable}(*{self.args}, **{self.kwargs})")
-        # return processor.execute_preparers(self.callable)(self.args, self.kwargs)
-        rebound = processor.execute_preparers(self.callable)
-        # print(f"\nEXECUTE self.callable={self.callable} rebound={rebound} inspect.signature(rebound)={inspect.signature(rebound)} self.args={self.args} self.kwargs={self.kwargs}")
-        return rebound(*self.args, **self.kwargs)
+        executor = processor.execute_preparers(self.callable)
+        return executor(*self.args, **self.kwargs)
 
 
 class InferredConverter(Converter):
     def __init__(self, parameter, appeal):
         if not parameter.default:
             raise AppealConfigurationError(f"empty {type(parameter.default)} used as default, so we can't infer types")
         p2 = inspect.Parameter(parameter.name, kind=parameter.kind, annotation=type(parameter.default), default=parameter.default)
@@ -2534,33 +5255,52 @@
 
 
 class SimpleTypeConverter(Converter):
     def __init__(self, parameter, appeal):
         self.appeal = appeal
         self.default = parameter.default
 
+        self.name = parameter.name
+
+        self.string_parameters = []
+
         self.value = None
 
+        self.queued = None
+        self.args_queue = collections.deque()
         self.args_converters = []
-        # don't set kwargs_converters, let it esplody!
+        self.kwargs_converters = {}
 
         self.options_values = {}
         self.help_options = {}
         self.help_arguments = {}
 
     def __repr__(self):
-        return f"<{self.__class__.__name__} {self.callable} args_converters={self.args_converters} value={self.value}>"
+        return f"<{self.__class__.__name__} {self.callable} args_converters={self.args_converters} kwargs_converters={self.kwargs_converters} value={self.value}>"
 
     def convert(self, processor):
-        if not self.args_converters:
+        # if 1:
+        if self.value is not None:
+            raise RuntimeError("why a second time, fool")
+        argument_count = (len(self.args_converters) + len(self.kwargs_converters))
+        assert 0 <= argument_count <= 1, f"{self.__class__.__name__}: {argument_count=}, should be 0 or 1, {self.args_converters=} {self.kwargs_converters=}"
+        if not argument_count:
             # explicitly allow "make -j"
             if self.default is not empty:
                 return self.default
             raise AppealUsageError(f"no argument supplied for {self}, we should have raised an error earlier huh.")
-        self.value = self.callable(self.args_converters[0])
+        try:
+            if self.kwargs_converters:
+                for v in self.kwargs_converters.values():
+                    self.args_converters.append(v)
+                self.kwargs_converters.clear()
+            self.value = self.callable(self.args_converters[0])
+        except ValueError as e:
+            raise AppealUsageError(f"invalid value {self.args_converters[0]} for {self.name}, must be {self.callable.__name__}")
+
 
     def execute(self, processor):
         return self.value
 
 
 simple_type_signatures = {}
 
@@ -2695,38 +5435,40 @@
         return self.render()
 
     # Your subclass of SingleOption or MultiOption is required
     # to define its own option() and render() methods.
     # init() is optional.
 
     # init() is called at initialization time.
-    # This is a convenience; you can overload __init__
+    # This is a convenience; you can also overload __init__
     # if you like.  But that means staying in sync with
-    # the parameters to __init__ and those aren't
-    # settled yet.
+    # the parameters to __init__ and still change sometimes.
     def init(self, default):
         pass
 
     # option() is called every time your option is specified
     # on the command-line.  For an Option, this will be exactly
-    # one time.  For a MultiOption, this will be one or more
-    # times.  (If your option is never specified on the
-    # command-line, your Option subclass will never be created.)
+    # one time.  For a MultiOption, this will be one or more times.
+    # (Appeal will never construct your Option object unless
+    # it's going to call your option method at least once.)
     #
     # option() can take parameters, and these are translated
     # to command-line positional parameters or options in the
     # same way converters are.
     #
     # Note:
     #   * If option() takes no parameters, your option will
     #     consume no opargs or options, like a boolean option.
     #     It'll still be called every time, your option is
     #     specified.
     #   * You may (and are encouraged to!) specify annotations for
     #     the parameters to option().
+    #   * If your option method only has *optional* parameters,
+    #     it's possible Appeal will call it with zero arguments.
+    #     (This is how you implement "make -j" for example.)
     @abstractmethod
     def option(self):
         pass
 
     # render() is called exactly once, after option() has been
     # called for the last time.  it should return the "value"
     # for the option.
@@ -3001,15 +5743,16 @@
 @must_be_instance
 def validate_range(start, stop=None, *, type=None, clamp=False):
     """
     Creates a converter function that validates that
     a value from the command-line is within a range.
 
         start and stop are like the start and stop
-            arguments for range().
+            arguments for range(), except values
+            can be less-than *or equal to* stop.
 
         type is the type for the value.  If unspecified,
             it defaults to builtins.type(start).
 
     If the value from the command-line is within the
     range established by start and stop, returns value.
 
@@ -3039,23 +5782,16 @@
             else:
                 value = start
         return value
     return validate_range
 
 
 
-def no_arguments_callable(): pass
-no_arguments_signature = inspect.signature(no_arguments_callable)
-
-
-
-
-
-# this function isn't published as one of the _to_converter callables
-def simple_type_to_converter(parameter, callable):
+# utility function, not published as one of the _to_converter callables
+def _simple_type_to_converter(parameter, callable):
     cls = simple_type_signatures.get(callable)
     if not cls:
         return None
     if (callable == bool) and (parameter.kind == KEYWORD_ONLY):
         return BooleanOptionConverter
     return cls
 
@@ -3065,15 +5801,15 @@
         return SimpleTypeConverterStr
 
 
 def type_to_converter(parameter):
     annotation = dereference_annotated(parameter.annotation)
     if not isinstance(annotation, type):
         return None
-    cls = simple_type_to_converter(parameter, annotation)
+    cls = _simple_type_to_converter(parameter, annotation)
     if cls:
         return cls
     if issubclass(annotation, SingleOption):
         return annotation
     return None
 
 def callable_to_converter(parameter):
@@ -3088,15 +5824,15 @@
 
 def inferred_type_to_converter(parameter):
     annotation = dereference_annotated(parameter.annotation)
     if (annotation is not empty) or (parameter.default is empty):
         return None
     inferred_type = type(parameter.default)
     # print(f"inferred_type_to_converter(parameter={parameter})")
-    cls = simple_type_to_converter(parameter, inferred_type)
+    cls = _simple_type_to_converter(parameter, inferred_type)
     # print(f"  inferred_type={inferred_type} cls={cls}")
     if cls:
         return cls
     if issubclass(inferred_type, SingleOption):
         return inferred_type
     if inferred_type in illegal_inferred_types:
         return None
@@ -3158,14 +5894,40 @@
     Unbinds a callable.
     If the callable is bound to an object (a "method"),
     returns the unbound callable.  Otherwise returns callable.
     """
     return callable.__func__ if isinstance(callable, types.MethodType) else callable
 
 
+
+class SpecialSection:
+    def __init__(self, name, topic_names, topic_values, topic_definitions, topics_desired):
+        self.name = name
+
+        # {"short_name": "fn_name.parameter_name" }
+        self.topic_names = topic_names
+        # {"fn_name.parameter_name": "usage_name"}
+        self.topic_values = topic_values
+        # {"fn_name.parameter_name": docs... }
+        self.topic_definitions = topic_definitions
+
+        # Appeal's "composable documentation" feature means that it merges
+        # up the docs for arguments and options from child converters.
+        # But what about opargs?  Those are "arguments" from the child
+        # converter tree, but you probably don't want them merged.
+        #
+        # So topics_desired lets you specify which topics Appeal should
+        # merge.
+        self.topics_desired = topics_desired
+
+        self.topics = {}
+        self.topics_seen = set()
+
+
+
 unspecified = object()
 
 class Appeal:
     """
     An Appeal object can only process a single command-line.
     Once you have called main() or process() on an Appeal object,
     you can't call either of those methods again.
@@ -3177,15 +5939,15 @@
         default_options=default_options,
         repeat=False,
         parent=None,
 
         option_space_oparg = True,              # '--long OPARG' and '-s OPARG'
 
         short_option_equals_oparg = True,       # -s=OPARG
-        short_option_concatenated_oparg = True, # -sOPARG
+        short_option_concatenated_oparg = True, # -sOPARG, only supported if -s takes *exactly* one *optional* oparg
 
         positional_argument_usage_format = "{name}",
 
         # if true:
         #   * adds a "help" command (if your program supports commands)
         #   * supports lone "-h" and "--help" options which behave like the "help" command without arguments
         help=True,
@@ -3211,15 +5973,15 @@
         # note that when sorting, options that appear multiple times will only be shown
         # once.  the second and subsequent appearances will be discarded.
         usage_sort_options = None,
         usage_sort_arguments = None,
 
         usage_max_columns = 80,
 
-        log_events = bool(want_prints),
+        log_events = True,
 
         ):
         self.parent = parent
         self.repeat = repeat
 
         self.name = name
 
@@ -3362,14 +6124,16 @@
             self.converter_factories = [
                 unannotated_to_converter,
                 type_to_converter,
                 callable_to_converter,
                 inferred_type_to_converter,
                 sequence_to_converter,
                 ]
+
+            self.unnested_converters = set()
         else:
             self.root = self.parent.root
 
         # self.option_signature_database[option] = [signature, option_entry1, ...]
         #
         # stores the signature of the converter function for
         # this option.  stores an option_entry for each
@@ -3418,14 +6182,20 @@
         a = None
         if name is not None:
             a = self.commands.get(name)
         if not a:
             a = Appeal(name=name, parent=self)
         return a
 
+    def unnested(self):
+        def unnested(fn):
+            self.root.unnested_converters.add(fn)
+            return fn
+        return unnested
+
     def __call__(self, callable):
         assert callable and builtins.callable(callable)
         self._global = callable
         if self.root != self:
             if self.name is None:
                 self.name = callable.__name__
                 self._calculate_full_name()
@@ -3467,15 +6237,15 @@
                     return fn
             return prepare
 
     class CommandMethodPreparer(Rebinder):
         def __init__(self, appeal, *, bind_method=True):
             super().__init__(bind_method=bind_method)
             self.appeal = appeal
-            self.placeholder = f"_cmp_{hex(id(object()))}"
+            self.placeholder = f"_commandmethodpreparer_placeholder_{hex(id(object()))}"
 
         def command(self, name=None):
             def command(fn):
                 fn2 = self.wrap(fn)
                 self.appeal.command(name=name)(fn2)
                 return fn
             return command
@@ -3559,20 +6329,24 @@
                 return cls
             return app_class
 
         # print("appeal.app_class returning", app_class, command_method)
         return app_class, command_method
 
 
-    def argument(self, parameter, *, usage=None):
-        def argument(callable):
+    def parameter(self, parameter, *, usage=None):
+        p = parameter
+        def parameter(callable):
             _, _, positionals = self.fn_database_lookup(callable)
-            positionals[parameter] = usage
+            positionals[p] = usage
             return callable
-        return argument
+        return parameter
+
+    # old--and incorrect!--name
+    argument = parameter
 
     def option_signature(self, option):
         """
         Returns the option_signature_database entry for that option.
         if defined, the return value is a list:
             [option_signature, option_entry1, ...]
 
@@ -3682,15 +6456,15 @@
         if not self._global_program:
             self.analyze(None)
 
         callable = self._global
         fn_name = callable.__name__
 
         formatter = self.root.format_positional_parameter
-        usage_str, arguments_values, options_values = charm_usage(self._global_program, formatter=formatter)
+        usage_str, arguments_values, options_values = charm_usage(self.root, self._global_program, formatter=formatter)
 
         if commands:
             if usage_str and (not usage_str[-1].isspace()):
                 usage_str += ' '
             usage_str += formatter("command")
 
         # {"{command_name}" : "help string"}
@@ -3725,35 +6499,35 @@
         # underneath us, in deepest-to-shallowest order.
 
         # signature = callable_signature(callable)
         # positional_children = set()
         # option_children = set()
 
         # info = [self.callable, signature, 0, positional_children, option_children]
-        ci = CharmInterpreter(self._global_program, name=fn_name)
+        ci = CharmBaseInterpreter(self._global_program, name=fn_name)
 
         last_op = None
         option_depth = 0
         programs = {}
 
         two_lists = lambda: ([], [])
         mapped_options = collections.defaultdict(two_lists)
 
-        for op in ci:
-            # print(f"## op={op}")
+        for ip, op in ci:
+            # print(f"## [{ip:>3}] op={op}")
             if op.op == opcode.create_converter:
                 c = {'parameter': op.parameter, 'parameters': {}, 'options': collections.defaultdict(list)}
                 ci.converters[op.key] = ci.o = c
                 continue
 
             if op.op == opcode.load_converter:
                 ci.converter = ci.converters[op.key]
                 continue
 
-            if (op.op == opcode.append_args) and last_op and (last_op.op == opcode.consume_argument):
+            if (op.op == opcode.append_to_converter_args) and last_op and (last_op.op == opcode.next_to_o):
                 ci.converter['parameters'][op.parameter] = op.usage
                 continue
 
             if op.op == opcode.map_option:
                 parameter = c['parameter']
                 program = op.program
 
@@ -3819,29 +6593,29 @@
         # to the old unmodified code.
         #
         # Below this line is the old unmodified code.
         ################################################################
         #
 
         values.sort(key=lambda o: o[2], reverse=True)
-        if want_prints:
-            for current, signature, depth, positional_children, option_children in values:
-                if current in simple_type_signatures:
-                    continue
-                print(f"current={current}\n    depth={depth}\n    positional_children={positional_children}\n    option_children={option_children}\n    signature={signature}\n")
+        # if want_prints:
+        #     for current, signature, depth, positional_children, option_children in values:
+        #         if current in simple_type_signatures:
+        #             continue
+        #         print(f"current={current}\n    depth={depth}\n    positional_children={positional_children}\n    option_children={option_children}\n    signature={signature}\n")
 
         # step 2:
         # process the docstrings of those annotation functions, deepest to shallowest.
         # when we process a function, also merge up from its children.
 
         fn_to_docs = {}
 
-        if want_prints:
-            print(f"[] arguments_values={arguments_values}")
-            print(f"[] options_values={options_values}")
+        # if want_prints:
+        #     print(f"[] arguments_values={arguments_values}")
+        #     print(f"[] options_values={options_values}")
 
         # again! complicated.
         #
         # the "topic" is the thing in the left column in curly braces:
         #   {foo}
         # this literal string "foo" represents a parameter of some kind.  it gets
         # looked up and substituted a couple different ways.
@@ -4001,45 +6775,45 @@
                             value = f"{fn_name}.{name}"
                         child_parameters[name] = value
                 d.update(child_parameters)
 
             arguments_desired = set(arguments_topic_values)
             options_desired = set(options_topic_values)
 
-            if want_prints:
-                print("_"*79)
-                l = locals()
-
-                # arguments_and_opargs_topic_names
-                # arguments_and_opargs_topic_values
-                # arguments_and_opargs_topic_definitions
-
-                for name in """
-                    callable
-
-                    arguments_topic_names
-                    arguments_topic_values
-                    arguments_topic_definitions
-                    arguments_desired
-
-                    options_topic_names
-                    options_topic_values
-                    options_topic_definitions
-
-                    options_desired
-
-                    commands_definitions
-
-                    all_definitions
-
-                    doc
-                    """.strip().split():
-                    print(f">>> {name}:")
-                    pprint.pprint(l[name])
-                    print()
+            # if want_prints:
+            #     print("_"*79)
+            #     l = locals()
+            #
+            #     # arguments_and_opargs_topic_names
+            #     # arguments_and_opargs_topic_values
+            #     # arguments_and_opargs_topic_definitions
+            #
+            #     for name in """
+            #         callable
+            #
+            #         arguments_topic_names
+            #         arguments_topic_values
+            #         arguments_topic_definitions
+            #         arguments_desired
+            #
+            #         options_topic_names
+            #         options_topic_values
+            #         options_topic_definitions
+            #
+            #         options_desired
+            #
+            #         commands_definitions
+            #
+            #         all_definitions
+            #
+            #         doc
+            #         """.strip().split():
+            #         print(f">>> {name}:")
+            #         pprint.pprint(l[name])
+            #         print()
 
             ##
             ## parse docstring
             ##
 
             arguments_section = SpecialSection("[[arguments]]", arguments_topic_names, arguments_topic_values, arguments_topic_definitions, arguments_desired)
             options_section = SpecialSection("[[options]]", options_topic_names, options_topic_values, options_topic_definitions, options_desired)
@@ -4244,26 +7018,26 @@
 
                     # print("processed summary:")
                     # print(f"   summary_lines={summary_lines}")
                     # print(f"   first_section={first_section}")
 
                     split_summary = text.fancy_text_split("\n".join(summary_lines), allow_code=False)
 
-            if want_prints:
-                print(f"[] arguments_topic_names={arguments_topic_names}")
-                print(f"[] arguments_topic_values={arguments_topic_values}")
-                print(f"[] arguments_topic_definitions={arguments_topic_definitions}")
-                # print(f"[] arguments_and_opargs_topic_names={arguments_and_opargs_topic_names}")
-                # print(f"[] arguments_and_opargs_topic_values={arguments_and_opargs_topic_values}")
-                # print(f"[] arguments_and_opargs_topic_definitions={arguments_and_opargs_topic_definitions}")
-                print(f"[] arguments_desired={arguments_desired}")
-                print(f"[] options_topic_names={options_topic_names}")
-                print(f"[] options_topic_values={options_topic_values}")
-                print(f"[] options_topic_definitions={options_topic_definitions}")
-                print(f"[] options_desired={options_desired}")
+            # if want_prints:
+            #     print(f"[] arguments_topic_names={arguments_topic_names}")
+            #     print(f"[] arguments_topic_values={arguments_topic_values}")
+            #     print(f"[] arguments_topic_definitions={arguments_topic_definitions}")
+            #     # print(f"[] arguments_and_opargs_topic_names={arguments_and_opargs_topic_names}")
+            #     # print(f"[] arguments_and_opargs_topic_values={arguments_and_opargs_topic_values}")
+            #     # print(f"[] arguments_and_opargs_topic_definitions={arguments_and_opargs_topic_definitions}")
+            #     print(f"[] arguments_desired={arguments_desired}")
+            #     print(f"[] options_topic_names={options_topic_names}")
+            #     print(f"[] options_topic_values={options_topic_values}")
+            #     print(f"[] options_topic_definitions={options_topic_definitions}")
+            #     print(f"[] options_desired={options_desired}")
 
             fn_to_docs[callable] = (
                 arguments_topic_definitions,
                 arguments_topic_values,
                 # arguments_and_opargs_topic_definitions,
                 # arguments_and_opargs_topic_values,
                 options_topic_definitions,
@@ -4387,22 +7161,22 @@
             if self.commands:
                 docstring.append("Commands:\n\n[[commands]]\n[[end]]\n")
             docstring = "\n".join(docstring).rstrip()
             # self._global_command.docstring = docstring
             # print(f"self._global_command.docstring = {docstring!r}")
             # print(f"self.commands={self.commands}")
         usage_str, summary_str, doc_str = self.render_docstring(commands=self.commands, override_doc=docstring)
-        if want_prints:
-            print(f">> usage from {self}:")
-            print(">> usage")
-            print(usage_str)
-            print(">> summary")
-            print(summary_str)
-            print(">> doc")
-            print(doc_str)
+        # if want_prints:
+        #     print(f">> usage from {self}:")
+        #     print(">> usage")
+        #     print(usage_str)
+        #     print(">> summary")
+        #     print(summary_str)
+        #     print(">> doc")
+        #     print(doc_str)
         spacer = False
         if usage:
             print("usage:", self.full_name, usage_str)
             spacer = True
         if summary and summary_str:
             if spacer:
                 print()
@@ -4430,136 +7204,207 @@
         appeal = self
         for name in command:
             appeal = appeal.commands.get(name)
             if not appeal:
                 raise AppealUsageError(f'"{name}" is not a legal command.')
         appeal.usage(usage=True, summary=True, doc=True)
 
-    def _analyze_attribute(self, name):
+    def _analyze_attribute(self, name, processor):
         if not getattr(self, name):
             return None
         program_attr = name + "_program"
         program = getattr(self, program_attr)
         if not program:
             callable = getattr(self, name)
-            program = charm_compile(self, callable)
-            if want_prints:
-                print()
+            program = charm_compile_command(self, processor, callable)
+            # if want_prints:
+            #     print()
             setattr(self, program_attr, program)
-            # print(f"compiled program for {name}, {program}")
         return program
 
     def analyze(self, processor):
         if processor:
-            callable = getattr(self, "_global")
-            if callable:
-                name = getattr(callable, "__name__", repr(callable))
-            else:
-                name = "None"
-            processor.log_event(f"analyze start ({name})")
-        self._analyze_attribute("_global")
+            processor.log(f"analyze _global")
+        self._analyze_attribute("_global", processor)
 
     def _parse_attribute(self, name, processor):
-        program = self._analyze_attribute(name)
+        program = self._analyze_attribute(name, processor)
         if not program:
             return None
-        if want_prints:
-            charm_print(program)
-        converter = charm_parse(self, program, processor.argi)
+        # if want_prints:
+        #     charm_print(program)
+
+        interpreter = CharmInterpreter(processor, program)
+        converter = interpreter()
+        if converter == None:
+            raise AppealUsageError("unknown error")
         processor.commands.append(converter)
         return converter
 
     def parse(self, processor):
         callable = getattr(self, "_global")
-        if callable:
-            name = getattr(callable, "__name__", repr(callable))
-        else:
-            name = "None"
-        processor.log_event(f"parse start ({name})")
+        processor.log(f"parse _global")
 
         self._parse_attribute("_global", processor)
 
-        if not processor.argi:
+        if not processor.iterator:
             # if there are no arguments waiting here,
             # then they didn't want to run a command.
             # if any commands are defined, and they didn't specify one,
             # if there's a default command, run it.
             # otherwise, that's an error.
             default_converter = self._parse_attribute("_default", processor)
             if (not default_converter) and self.commands:
                 raise AppealUsageError("no command specified.")
             return
 
+        processor.log.enter(f"parsing commands")
         if self.commands:
             # okay, we have arguments waiting, and there are commands defined.
-            for command_name in processor.argi:
+            for command_name in processor.iterator:
                 sub_appeal = self.commands.get(command_name)
                 if not sub_appeal:
                     # partial spelling check would go here, e.g. "sta" being short for "status"
                     self.error(f"unknown command {command_name}")
                 # don't append! just parse.
                 # the recursive Appeal.parse call will append.
                 sub_appeal.analyze(processor)
                 sub_appeal.parse(processor)
-                if not (self.repeat and processor.argi):
+                if not (self.repeat and processor.iterator):
                     break
 
-        if processor.argi:
-            leftovers = " ".join(shlex.quote(s) for s in processor.argi)
+        if processor.iterator:
+            leftovers = " ".join(shlex.quote(s) for s in processor.iterator)
             raise AppealUsageError(f"leftover cmdline arguments! {leftovers!r}")
 
+        processor.log.exit()
+
     def convert(self, processor):
-        processor.log_event("convert start")
+        processor.log("convert start")
         for command in processor.commands:
             command.convert(processor)
 
     def execute(self, processor):
-        processor.log_event("execute start")
+        processor.log("execute start")
         result = None
         for command in processor.commands:
             result = command.execute(processor)
             if result:
                 break
         return result
 
     def processor(self):
         return Processor(self)
 
-    def process(self, args=None):
+    def process(self, args=None, kwargs=None):
+        processor = self.processor()
+        result = processor(args, kwargs)
+        return result
+
+    def main(self, args=None, kwargs=None):
+        if args is None:
+            args = sys.argv[1:]
+        processor = self.processor()
+        processor.main(args, kwargs)
+
+    def read_mapping(self, callable, mapping):
         processor = self.processor()
-        return processor(args)
 
-    def main(self, args=None):
+        cc = CharmMappingCompiler(self, processor, callable)
+        program = cc.assemble()
+
+        # why permit a Sequence here?
+        # if callable is a MultiOption,
+        # we start with iteration
+        if isinstance(mapping, Mapping):
+            processor.mapping = mapping
+        elif isinstance(mapping, Iterable):
+            processor.iterator = mapping
+        else:
+            raise TypeError("mapping must be a Mapping (or an Iterable)")
+        interpreter = CharmInterpreter(processor, program)
+
+        converter = interpreter()
+
+        converter.convert(processor)
+        return converter.execute(processor)
+
+    def read_iterable(self, callable, iterable):
         processor = self.processor()
-        processor.main(args)
+
+        compiler = CharmIteratorCompiler
+        cc = compiler(self, processor, callable)
+        program = cc.assemble()
+
+        processor.log.enter("iterable parse")
+        results = []
+        for row in iterable:
+            if not row:
+                continue
+
+            processor.iterator = row
+            interpreter = CharmInterpreter(processor, program)
+            converter = interpreter()
+
+            converter.convert(processor)
+            result = converter.execute(processor)
+            results.append(result)
+        processor.log.exit()
+
+        return results
+
+    def read_csv(self, callable, csv_reader, *, first_row_map=None):
+        processor = self.processor()
+
+        if first_row_map:
+            compiler = CharmMappingCompiler
+        else:
+            compiler = CharmIteratorCompiler
+        cc = compiler(self, processor, callable)
+        program = cc.assemble()
+
+        headings = next(csv_reader)
+        if first_row_map:
+            keys = [first_row_map.get(key, key) for key in headings]
+
+        processor.log.enter("csv parse")
+        results = []
+        for row in csv_reader:
+            if not row:
+                continue
+
+            if first_row_map:
+                d = {key: value for key, value in zip(keys, row)}
+                processor.mapping = d
+            else:
+                processor.iterator = row
+            interpreter = CharmInterpreter(processor, program)
+            converter = interpreter()
+
+            converter.convert(processor)
+            result = converter.execute(processor)
+            results.append(result)
+        processor.log.exit()
+
+        return results
 
 
 class Processor:
     def __init__(self, appeal):
-        self.events = []
-        self.log_event("process start")
-
         self.appeal = appeal
         self.preparers = []
+        self.reset()
 
+    def reset(self):
+        self.events = []
+        self.iterator = None
+        self.mapping = None
         self.commands = []
-        self.breadcrumbs = []
         self.result = None
-
-    def push_breadcrumb(self, breadcrumb):
-        self.breadcrumbs.append(breadcrumb)
-
-    def pop_breadcrumb(self):
-        return self.breadcrumbs.pop()
-
-    def format_breadcrumbs(self):
-        return " ".join(self.breadcrumbs)
-
-    def log_event(self, event):
-        self.events.append((event, event_clock()))
+        self.log = big.Log()
 
     def preparer(self, preparer):
         if not callable(preparer):
             raise ValueError(f"{preparer} is not callable")
         # print(f"((( adding preparer={preparer}")
         self.preparers.append(preparer)
 
@@ -4567,56 +7412,43 @@
         for preparer in self.preparers:
             try:
                 fn = preparer(fn)
             except ValueError:
                 pass
         return fn
 
+    def __call__(self, sequence=None, mapping=None):
+        self.reset()
+        self.log("process start")
 
-    def print_log(self):
-        if not self.events:
-            return
-        def format_time(t):
-            seconds = t // 1000000000
-            nanoseconds = t - seconds
-            return f"{seconds:02}.{nanoseconds:09}"
-
-        start_time = previous = self.events[0][1]
-        formatted = []
-        for i, (event, t) in enumerate(self.events):
-            elapsed = t - start_time
-            if i:
-                delta = elapsed - previous
-                formatted[-1][-1] = format_time(delta)
-            formatted.append([event, format_time(elapsed), "            "])
-            previous = elapsed
+        self.sequence = sequence
+        iterator = sequence
+        if (iterator is not None) and (not isinstance(sequence, PushbackIterator)):
+            iterator = PushbackIterator(iterator)
+        self.iterator = iterator
 
-        print()
-        print("[event log]")
-        print(f"  start         elapsed       event")
-        print(f"  ------------  ------------  -------------")
+        self.mapping = mapping
 
-        for event, start, elapsed in formatted:
-            print(f"  {start}  {elapsed}  {event}")
-
-    def __call__(self, args=None):
-        if args is None:
-            args = sys.argv[1:]
-        self.args = args
-        self.argi = argi = PushbackIterator(args)
+        # if want_prints:
+        #     # allow us to print the remaining contents of the iterator
+        #     # by examining its stack
+        #     l = list(iterator)
+        #     l.reverse()
+        #     iterator.stack.extend(l)
+        #     iterator.i = None
 
         appeal = self.appeal
         if appeal.support_version:
-            if (len(args) == 1) and args[0] in ("-v", "--version"):
+            if (len(sequence) == 1) and sequence[0] in ("-v", "--version"):
                 return appeal.version()
             if appeal.commands and (not "version" in appeal.commands):
                 appeal.command()(appeal.version)
 
         if appeal.support_help:
-            if (len(args) == 1) and args[0] in ("-h", "--help"):
+            if (len(sequence) == 1) and sequence[0] in ("-h", "--help"):
                 return appeal.help()
             if appeal.commands and (not "help" in appeal.commands):
                 appeal.command()(appeal.help)
 
         if appeal.appeal_preparer:
             # print(f"bind appeal.appeal_preparer to self.appeal={self.appeal}")
             self.preparer(appeal.appeal_preparer.bind(self.appeal))
@@ -4624,19 +7456,20 @@
             # print(f"bind appeal.processor_preparer to self={self}")
             self.preparer(appeal.processor_preparer.bind(self))
 
         appeal.analyze(self)
         appeal.parse(self)
         appeal.convert(self)
         result = self.result = appeal.execute(self)
-        self.log_event("process complete")
-        if want_prints:
-            self.print_log()
+        self.log("process complete")
+        # if want_prints:
+        #     self.log.print()
         return result
 
-    def main(self, args=None):
+    def main(self, args=None, kwargs=None):
         try:
-            sys.exit(self(args=args))
+            sys.exit(self(sequence=args, mapping=kwargs))
         except AppealUsageError as e:
             print("Error:", str(e))
             self.appeal.usage(usage=True)
             sys.exit(-1)
+
```

### Comparing `appeal-0.5.9/appeal/argument_grouping.py` & `appeal-0.6/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/appeal/cpp.py` & `appeal-0.6/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/appeal/text.py` & `appeal-0.6/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/pyproject.toml` & `appeal-0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,7 +20,10 @@
     ]
 dependencies = [
     "big >= 0.7.1",
 ]
 
 [project.urls]
 Source = "https://github.com/larryhastings/appeal/"
+
+[project.optional-dependencies]
+dev = ['perky', 'tomli']
```

### Comparing `appeal-0.5.9/resources/images/appeal.logo.png` & `appeal-0.6/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/resources/images/give.your.program.appeal.png` & `appeal-0.6/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.9/tests/run_tests.py` & `appeal-0.6/tests/test_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 
 def undo(a:nested_outer=0):
     return (undo, a)
 
 def hey_argparse_watch_this(*, i:int=None, f:float=None, c:complex=None):
     return (hey_argparse_watch_this, i, f, c)
 
+
 def inner_option(*, e=False, f=False):
     return (inner_option, e, f)
 
 def nested_option(*, c=False, d=False, nested:inner_option=(inner_option, False, False)):
     return (nested_option, c, d, nested)
 
 def options_stack(x='abc', *, a=False, b=False, option:nested_option=(nested_option, False, False, (inner_option, False, False))):
@@ -305,26 +306,56 @@
 def five_a(*, d:five_d=None, e=False, f=False):
     return (five_a, d, e, f)
 
 def five_level_stack(*, a:five_a=None, b=False, c=False):
     return (five_level_stack, a, b, c)
 
 
+def multiple_groups_child(child_a, child_b, child_c=None, *, flag=False, color:int_float_verbose=(0, 0.0, False)):
+    return (multiple_groups_child, child_a, child_b, child_c, flag, color)
+
+def multiple_groups(a,
+    b:multiple_groups_child=(multiple_groups_child, None, None, None, False, (0, 0.0, False)),
+    c:multiple_groups_child=(multiple_groups_child, None, None, None, False, (0, 0.0, False)),
+    d='',
+    ):
+    return (multiple_groups, a, b, c, d)
+
+def simple_defaults(a: int=0, b: str=''):
+    return (simple_defaults, a, b)
+
+
 class IntFloat:
     def __init__(self, integer:int, real:float):
         self.i = integer
         self.f = real
 
     def __repr__(self):
         return f"<IntFloat i={self.i!r} f={self.f!r}>"
 
 def str_i_f(value, i_f:IntFloat=None, *, option=None, verbose=False):
     return (str_i_f, value, i_f, option, verbose)
 
-class SmokeTests(unittest.TestCase):
+
+def earlier_int_float2(i2:int, f2:float, *, flag=False):
+    return (earlier_int_float2, i2, f2, flag)
+
+def earlier_int_float1(i1:int, f1:float, *, verbose=False):
+    return (earlier_int_float1, i1, f1, verbose)
+
+def earlier(a, b:earlier_int_float1, c:earlier_int_float2=(earlier_int_float2, 0, 0.0, False)):
+    return (earlier, a, b, c)
+
+
+class AppealTestsBase(unittest.TestCase):
+    maxDiff = None
+
+
+class SmokeTests(AppealTestsBase):
+
     def setUp(self):
         global app
         global command
         global process
         app = appeal.Appeal(
             usage_max_columns=80,
             usage_indent_definitions=2,
@@ -335,41 +366,41 @@
         def my_process(args):
             return app.process(args)
         process = my_process
 
     def assert_process(self, cmdline, result):
         self.assertEqual(process(shlex.split(cmdline)), result)
 
-    def assert_process_raises(self, cmdline, exception):
+    def assert_process_raises(self, cmdline, exception, text=None):
         e = None
         with self.assertRaises(exception):
             try:
                 process(shlex.split(cmdline))
             except exception as e2:
                 e = e2
                 raise e2
+        if text:
+            self.assertIn(text, str(e))
         return e
 
     def tearDown(self):
         global app
         global command
         app = command = None
 
     def test_test_usage(self):
         command(test)
         text = capture_stdout('help test')
         self.assertIn("Simple test command function.", text)
-        self.assertIn(" str1 ", text)
+        self.assertIn("test [-g|--gloop [-i|--intfloat [-v|--verbose] x_int y_float] gloopstr] str1 str2 [optional_int]", text)
         self.assertIn("A string!", text)
-        self.assertIn("-g|--gloop", text)
         self.assertIn("grab-bag", text)
         self.assertIn("for a in code:", text)
         self.assertIn("fifth section.", text)
 
-
     def test_test_1(self):
         command(test)
         self.assert_process(
             "test -g gloopy abc def",
             (test,'abc', 'def', 0, (gloopfn, 'gloopy', '(default value for intfloat)')),
             )
 
@@ -383,14 +414,49 @@
     def test_test_3(self):
         command(test)
         self.assert_process_raises(
             "test -g gloopy abc def -i 1 3.0 -v 336",
             appeal.AppealUsageError,
             )
 
+    def test_simple_defaults_1(self):
+        command(simple_defaults)
+        self.assert_process(
+            "simple_defaults",
+            (simple_defaults, 0, ''),
+            )
+
+    def test_simple_defaults_2(self):
+        command(simple_defaults)
+        self.assert_process(
+            "simple_defaults 5",
+            (simple_defaults, 5, ''),
+            )
+
+    def test_simple_defaults_3(self):
+        command(simple_defaults)
+        self.assert_process(
+            "simple_defaults 33 abc",
+            (simple_defaults, 33, 'abc'),
+            )
+
+    def test_simple_defaults_4(self):
+        command(simple_defaults)
+        self.assert_process_raises(
+            "simple_defaults 3.14159",
+            appeal.AppealUsageError,
+            )
+
+    def test_simple_defaults_5(self):
+        command(simple_defaults)
+        self.assert_process_raises(
+            "simple_defaults 33 abc xxx",
+            appeal.AppealUsageError,
+            )
+
 
     def bind_rip(self):
         command(rip)
         app.option("imaginary", "-i", "--imaginary")(rip)
 
     def test_rip_1(self):
         self.bind_rip()
@@ -405,15 +471,15 @@
                 ),
             )
 
     def test_rip_2(self):
         self.bind_rip()
 
         self.assert_process(
-            'rip abc 1 2 -v',
+            'rip abc -v 1 2',
             (rip,
                 'abc',
                 (int_float_verbose, 1, 2.0, 'verbose'),
                 "(b default)",
                 "(c default)",
                 {},
                 ),
@@ -468,19 +534,18 @@
                 (int_float_verbose, 1, 2.0, 'verbose'),
                 (int_float_verbose, 3, 4.0, 'verbose'),
                 (int_float_verbose, 5, 6.0, 'verbose'),
                 {},
                 )
             )
 
-
     def test_rip_7(self):
         self.bind_rip()
         self.assert_process(
-            'rip scooby 1 -v 2 3 4 --verbose 5 6 -v',
+            'rip scooby -v 1 2  --verbose 3 4 --verbose 5 6',
             (rip,
                 'scooby',
                 (int_float_verbose, 1, 2.0, 'verbose'),
                 (int_float_verbose, 3, 4.0, 'verbose'),
                 (int_float_verbose, 5, 6.0, 'verbose'),
                 {},
                 )
@@ -911,16 +976,16 @@
             'make2 a b c -j 88 99',
             (make2, (88, 99, 333), ('a', 'b', 'c')),
             )
 
 
     def bind_two_or_more_files(self):
         command(two_or_more_files)
-        app.argument("file2", usage="file")(two_or_more_files)
-        app.argument("files", usage="file")(two_or_more_files)
+        app.parameter("file2", usage="file")(two_or_more_files)
+        app.parameter("files", usage="file")(two_or_more_files)
 
     def test_two_or_more_files_usage(self):
         self.bind_two_or_more_files()
         text = capture_stdout('help two_or_more_files')
         self.assertIn("file file [file]...", text)
 
     def test_two_or_more_files_1(self):
@@ -1044,16 +1109,16 @@
             'undo',
             (undo, 0),
             )
 
     def test_undo_2(self):
         command(undo)
         self.assert_process(
-            'undo 3',
-            (undo, 3),
+            'undo 2',
+            (undo, 2),
             )
 
     def test_hey_argparse_watch_this_1(self):
         command(hey_argparse_watch_this)
         self.assert_process(
             'hey_argparse_watch_this',
             (hey_argparse_watch_this, None, None, None),
@@ -1115,56 +1180,66 @@
     def test_options_stack_2(self):
         command(options_stack)
         self.assert_process(
             'options_stack --option --nested',
             (options_stack, 'abc', False, False, (nested_option, False, False, (inner_option, False, False)))
             )
 
-    def test_options_stack_2(self):
+    def test_options_stack_3(self):
         command(options_stack)
         self.assert_process(
             'options_stack --option --nested -eca',
             (options_stack, 'abc', True, False, (nested_option, True, False, (inner_option, True, False)))
             )
 
-    def test_options_stack_3(self):
+    def test_options_stack_4(self):
         command(options_stack)
-        self.assert_process(
+        self.assert_process_raises(
             'options_stack --option --nested -ace',
-            (options_stack, 'abc', True, False, (nested_option, True, False, (inner_option, True, False)))
+            # (options_stack, 'abc', True, False, (nested_option, True, False, (inner_option, True, False)))
+            appeal.AppealUsageError,
             )
 
-    def test_options_stack_4(self):
+    def test_options_stack_5(self):
         command(options_stack)
-        self.assert_process(
+        self.assert_process_raises(
             'options_stack --option --nested -ace -b',
-            (options_stack, 'abc', True, True, (nested_option, True, False, (inner_option, True, False)))
+            # (options_stack, 'abc', True, True, (nested_option, True, False, (inner_option, True, False)))
+            appeal.AppealUsageError,
             )
 
-    def test_options_stack_5(self):
+    def test_options_stack_6(self):
         command(options_stack)
         self.assert_process_raises(
             'options_stack --option --nested -ace -bdf',
             appeal.AppealUsageError,
             )
 
-    def test_options_stack_6(self):
+    def test_options_stack_7(self):
         command(options_stack)
         self.assert_process_raises(
             'options_stack --option --nested -a -e',
             appeal.AppealUsageError,
             )
 
-    def test_options_stack_7(self):
+    def test_options_stack_8(self):
+        command(options_stack)
+        self.assert_process_raises(
+            'options_stack --option --nested -a -c',
+            appeal.AppealUsageError,
+            )
+
+    def test_options_stack_9(self):
         command(options_stack)
         self.assert_process_raises(
             'options_stack --option --nested -a -c',
             appeal.AppealUsageError,
             )
 
+
     def test_five_level_stack_1(self):
         command(five_level_stack)
         self.assert_process(
             "five_level_stack",
             (five_level_stack,  None, False, False),
             )
 
@@ -1267,44 +1342,190 @@
             "five_level_stack -a -d -g -j -mb -n",
             appeal.AppealUsageError,
             )
 
     def test_five_level_stack_16(self):
         command(five_level_stack)
         self.maxDiff=None
-        self.assert_process(
+        self.assert_process_raises(
             "five_level_stack -a -d -g -j -m -behknp",
-            (five_level_stack, (five_a, (five_d, (five_g, (five_j, (five_m, True, False, False), True, False), True, False), True, False), True, False), True, False),
+            # (five_level_stack, (five_a, (five_d, (five_g, (five_j, (five_m, True, False, False), True, False), True, False), True, False), True, False), True, False),
+            appeal.AppealUsageError,
+            )
+
+
+
+# def multiple_groups_child(child_a, child_b, child_c=None, *, flag=False, color:int_float_verbose=(0, 0.0, False)):
+#     return (multiple_groups_child, child_a, child_b, child_c, flag, color)
+
+# def multiple_groups(a, b:multiple_groups_child=(multiple_groups_child, None, None, None, False, (0, 0.0, False)), c:multiple_groups_child=(multiple_groups_child, None, None, None, False, (0, 0.0, False)), d=''):
+#     return (mixed, a, b, c, d)
+
+    def test_mixed_groups_1(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups abc",
+            (multiple_groups,
+                'abc',
+                (multiple_groups_child, None, None, None, False, (0, 0.0, False)),
+                (multiple_groups_child, None, None, None, False, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_2(self):
+        command(multiple_groups)
+        self.assert_process_raises(
+            "multiple_groups abc def",
+            appeal.AppealUsageError,
+            )
+
+    def test_mixed_groups_3(self):
+        command(multiple_groups)
+        self.assert_process_raises(
+            "multiple_groups abc -v",
+            appeal.AppealUsageError,
+            )
+
+    def test_mixed_groups_4(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb bc ca cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', False, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', False, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_5(self):
+        command(multiple_groups)
+        self.assert_process_raises(
+            "multiple_groups -f a ba bb bc ca cb cc",
+            appeal.AppealUsageError,
+            )
+
+    def test_mixed_groups_6(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a -f ba bb bc ca cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', True, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', False, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_7(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba -f bb bc ca cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', True, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', False, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_8(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb -f bc ca cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', True, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', False, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_9(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb bc -f ca cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', False, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', True, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_10(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb bc ca -f cb cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', False, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', True, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+    def test_mixed_groups_11(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb bc ca cb -f cc",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', False, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', True, (0, 0.0, False)),
+                ''
+                ),
             )
 
+    # the stuff in the final group sticks around forever
+    def test_mixed_groups_12(self):
+        command(multiple_groups)
+        self.assert_process(
+            "multiple_groups a ba bb bc ca cb cc -f",
+            (multiple_groups,
+                'a',
+                (multiple_groups_child, 'ba', 'bb', 'bc', False, (0, 0.0, False)),
+                (multiple_groups_child, 'ca', 'cb', 'cc', True, (0, 0.0, False)),
+                ''
+                ),
+            )
+
+
     def test_str_i_f_1(self):
         command(str_i_f)
         e = self.assert_process_raises(
             "str_i_f abc 1",
             appeal.AppealUsageError,
             )
         self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
 
+    def test_str_i_f_2(self):
+        command(str_i_f)
         # regression test:
         # when printing usage, we used to print the name of the last program
         # we'd called, regardless of whether or not it was currently running.
         # so this error used to read
         #   str_i_f, -v, --verbose requires 2 arguments in this argument group.
         e = self.assert_process_raises(
             "str_i_f abc 1 --verbose",
             appeal.AppealUsageError,
             )
         self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
 
+    def test_str_i_f_1(self):
+        command(str_i_f)
         e = self.assert_process_raises(
             "str_i_f abc 1 --option x",
             appeal.AppealUsageError,
             )
         self.assertEqual(str(e), "str_i_f requires 2 arguments in this argument group.")
 
+    def test_str_i_f_4(self):
+        command(str_i_f)
         e = self.assert_process_raises(
             "str_i_f abc 1 --option",
             appeal.AppealUsageError,
             )
         self.assertEqual(str(e), "str_i_f -o | --option requires 1 argument in this argument group.")
 
 
@@ -1335,14 +1556,95 @@
         self.assertEqual(result, None)
         self.assertEqual(len(instances), 1)
         instance = instances.pop()
         self.assertIsInstance(instance, MyApp)
         self.assertEqual(instance.dump(), (True, 'patt', 'file', 33))
 
 
+    def test_regression_raised_an_error_earlier_huh(self):
+        # there's a usage error:
+        # AppealUsageError(f"no argument supplied for {self}, we should have raised an error earlier huh.")
+        # this test used to trip it.
+        # (before I rewrote undoable converters to tie directly to argument groups)
+        # (which was before I rewrote it two more times and renamed them to "discretionary" converter)
+        command(earlier)
+        self.assert_process(
+            "earlier a  1  2.3 -v",
+            (earlier,
+                'a',
+                (earlier_int_float1, 1, 2.3, True),
+                (earlier_int_float2, 0, 0.0, False),
+                ),
+            )
+
+    def test_discretionary_converter_torture_test_1(self):
+        def first_child(*, verbose=False):
+            return (first_child, verbose)
+
+        def enfant_terrible(*, flag=0):
+            return (enfant_terrible, flag)
+
+        def parent(first_child: first_child=(first_child, False), enfant_terrible:enfant_terrible=(enfant_terrible, 0)):
+            return (parent, first_child, enfant_terrible)
+
+        @command
+        def grandparent(parent:parent=(parent, (first_child, False), (enfant_terrible, 0))):
+            return (grandparent, parent)
+
+        self.assert_process(
+            "grandparent --flag 3",
+            (grandparent,
+                (parent,
+                    (first_child, False),
+                    (enfant_terrible, 3),
+                    ),
+                ),
+            )
+
+    def test_custom_option(self):
+        class MyOption(appeal.Option):
+            def init(self, default):
+                self.value = default
+
+            def option(self, value:int=0):
+                self.value = value
+
+            def render(self):
+                return self.value
+
+        @command
+        def c(a, b, *, option:MyOption=0):
+            return (c, a, b, option)
+
+        self.assert_process(
+            "c aa bb",
+            (c, 'aa', 'bb', 0)
+            )
+
+        self.assert_process(
+            "c aa bb -o",
+            (c, 'aa', 'bb', 0)
+            )
+
+        self.assert_process(
+            "c aa bb -o 33",
+            (c, 'aa', 'bb', 33)
+            )
+
+        self.assert_process(
+            "c  xx -o 44 yy",
+            (c, 'xx', 'yy', 44)
+            )
+
+        self.assert_process(
+            "c  -o 55 xx yy",
+            (c, 'xx', 'yy', 55)
+            )
+
+
 
 ##
 ## I got tired of the examples in README.md not working
 ## or being out of sync with the implementation.
 ## So now I ensure the examples in README.md are always
 ## working--because I run them.
 ##
@@ -1440,15 +1742,15 @@
             t, counter = l
             print(f"    [ #{i}")
             for line in t.split("\n"):
                 print("   ", line)
             print("    ]")
 
 
-class ReadmeTests(unittest.TestCase):
+class ReadmeTests(AppealTestsBase):
 
     def exec_readme(self, section, index, cmdline, expected):
         global app
         global process
 
         l = readme_tests[section][index]
         text, count = l
@@ -1546,15 +1848,15 @@
         # let's search for a string that exists exactly once.
         # it's a little tricky because the string needs to be on the
         # command-line, and also in the output string that we're matching against.
         # so, we use automatic string concatenation to break up the special string.
         self.exec_readme(
             'Quickstart',
             1,
-            "fgrep xy" f"zzy '{appeal_dir}/tests/run_tests.py'",
+            "fgrep xy" f"zzy '{appeal_dir}/tests/test_all.py'",
             # xyzzy!
             "# xyz" "zy!",
             )
 
 
     # 'Our First Example'
     #     [ #0
@@ -1894,15 +2196,15 @@
             "fgrep pattern=[]",
             )
 
     def test_specifying_an_option_more_than_once_2_2(self):
         self.exec_readme(
             'Specifying An Option More Than Once',
             2,
-            "fgrep -p8",
+            "fgrep -p=8",
             "fgrep pattern=[8]",
             )
 
     def test_specifying_an_option_more_than_once_2_3(self):
         self.exec_readme(
             'Specifying An Option More Than Once',
             2,
@@ -1910,15 +2212,15 @@
             "fgrep pattern=[44, 22]",
             )
 
     def test_specifying_an_option_more_than_once_2_4(self):
         self.exec_readme(
             'Specifying An Option More Than Once',
             2,
-            "fgrep --pattern 2 -p 4 --pattern=6 -p=8 -p10",
+            "fgrep --pattern 2 -p 4 --pattern=6 -p=8 -p 10",
             "fgrep pattern=[2, 4, 6, 8, 10]",
             )
 
     # 'Data Validation'
     #     [ #0
     #     import appeal
     #     app = appeal.Appeal()
@@ -2133,15 +2435,15 @@
             "inception option=[33, False]",
             )
 
     def test_now_witness_the_power_of_this_etc_0_3(self):
         self.exec_readme(
             'Options that map other options',
             0,
-            "inception -o1965 -v",
+            "inception -o=1965 -v",
             "inception option=[1965, True]",
             )
 
     def test_now_witness_the_power_of_this_etc_0_4(self):
         self.exec_readme(
             'Options that map other options',
             0,
@@ -2171,15 +2473,15 @@
         self.exec_readme(
             "Multiple options that aren't MultiOptions",
             0,
             "repetition 0",
             "repetition args=([0, False],)",
             )
 
-    def test_now_witness_the_power_of_this_etc_1_2(self):
+    def test_now_witness_the_power_of_this_etc_1_3(self):
         self.exec_readme(
             "Multiple options that aren't MultiOptions",
             0,
             "repetition 0 1 -v 2 3 --verbose 4 5",
             "repetition args=([0, False], [1, False], [2, True], [3, False], [4, True], [5, False])",
             )
 
@@ -2218,23 +2520,23 @@
             "mixin log=<Logging verbose=True log_level=ascerbic>",
             )
 
     def test_now_witness_the_power_of_this_etc_2_3(self):
         self.exec_readme(
             'Positional parameters that only consume options',
             0,
-            "mixin -ldidactic  --verbose",
+            "mixin -l didactic  --verbose",
             "mixin log=<Logging verbose=True log_level=didactic>",
             )
 
     def test_now_witness_the_power_of_this_etc_2_4(self):
         self.exec_readme(
             'Positional parameters that only consume options',
             0,
-            "mixin -lelective",
+            "mixin -l=elective",
             "mixin log=<Logging verbose=False log_level=elective>",
             )
 
 
     # 'Classes, Instances, And Preparers'                                                 [202/1984]
     #     [ #0
     #     import appeal
```

### Comparing `appeal-0.5.9/PKG-INFO` & `appeal-0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.9
+Version: 0.6
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: big >= 0.7.1
+Requires-Dist: perky ; extra == "dev"
+Requires-Dist: tomli ; extra == "dev"
 Project-URL: Source, https://github.com/larryhastings/appeal/
+Provides-Extra: dev
 
 ![## Appeal](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/appeal.logo.png)
 
 ![## Give your program Appeal!](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
@@ -1370,15 +1373,15 @@
 
 What's really going on here is that, from Appeal's perspective,
 *there's no difference between a "command function" and a
 "converter".*  A command function is just a converter that
 happens to be mapped to a command.  So anything you can do
 with a command function, you can do with a converter too.
 A converter can define options, it can be decorated with
-`app.option()` (or `app.argument()` which we haven't
+`app.option()` (or `app.parameter()` which we haven't
 discussed yet), it can have accept any kind of parameter defined
 by Python, and any parameter can use (almost) any converter.
 And those converters can recursively use other converters.
 
 Realy, anything can be used with anything:
 
 * Converters for positional parameters
@@ -1547,14 +1550,326 @@
 these bits of documentation together to produce the help for your
 command function.
 
 (One note: the main help for your program should be the docstring
 for your Appeal instance's global command.)
 
 
+## Appeal's latest superpower: reading config files
+
+Appeal allows for friction-free command-line APIs.  You write your
+command function, point Appeal at it, and whoosh! now you've got a
+command-line interface.  But there are other interfaces users may
+want to use to configure your program.  Now Appeal can work with
+those too.
+
+For example, your program may read configuration from environment
+variables.  Some programs launch an editor; for example `git` will
+open an editor when committing a revision.  Traditionally on
+UNIX-based platforms this is configurable using two environment
+variables, `VISUAL` and `EDITOR` in that order of preference.
+
+Appeal doesn't need to add explicit support for environment variables,
+as Python already has an easy-to-use interface.  For example, here's
+how to support the environment variables configuring your editor:
+
+However, many programs also support a configuration file, also called
+an "rc file"  on UNIX.  By convention settings in such a config file
+usually take precedence over environment variables.  For example, you
+can configure what editor `git` uses for commits with a value called
+`core.editor` stored in a config file.
+
+As of 0.6, Appeal has support for reading data from configuration
+files.  Note that Appeal doesn't read the data files itself; you
+already have a library for that.  Instead, Appeal has a generic
+mechanism for reading data from either an iterable or a mapping--
+either a list or a dict.
+
+The first step is to read in the values from the configuration file,
+and produce a dict or dict-like object.  You can use any library
+you like.  For example, the [`tomli`](https://pypi.org/project/tomli/) library
+works well for [TOML files.](https://en.wikipedia.org/wiki/TOML)
+JSON and YAML parsers also work nicely.  And this facility works
+*especially* well with my [`Perky`](https://pypi.org/project/perky/)
+file format.  Though that's just a coincidence, as they were designed
+separately, years apart.  Honest!
+
+(You can also use `configparser` to read your INI config file,
+but this doesn't mesh well with Appeal's model.  Better support
+for reading INI files is a possible future direction for Appeal.)
+
+Once you've got a dictionary containing your configuration information,
+you can get Appeal to read from it using a single method call:
+
+```Python
+    Appeal.read_mapping(self, callable, mapping)
+```
+
+Simply pass in the callable you want called, and the mapping--the dict--you
+read from your config file.  Appeal will read the names of the callable's
+parameters, pull values out of the mapping using those names, and pass those
+values in to a call to the callable.
+
+Of course, any mapping will work.  But this method works particularly
+well with classes decorated with `dataclasses.dataclass`.  In just a few
+lines, you can define a class to contain your configuration information,
+read it out of a file, and populate the class with values of all the correct
+types!
+
+In a lot of ways, this works very similarly to Appeal when it's processing
+a command-line.  For example:
+
+* Appeal will use the annotations and default values to convert
+  the values from the dictionary into the correct types.
+* Parameters with default values are optional; parameters without
+  default values are required.
+
+But there are differences too:
+
+* You can use positional-only, positional-or-keyword,
+  or keyword-only arguments.  However, var-positional
+  (`*args`) and var-keyword (`**kwargs`) are unsupported.
+
+
+Let's bring all of this together with an example.  Let's say we're
+writing a hypothetical program that may launch an editor.  Our
+sophisticated program has *five* ways to decide what program
+to run for the editor.  In decreasing order of importance:
+
+* Command-line options '-e' and '--editor' specify the
+  editor to use for this instnace.
+* The config file `~/.myprogramrc` is a Perky file, and it
+  can contain an `editor` value.
+* If the user has set an `VISUAL` environment variable, use that.
+* If the user has set an `EDITOR` environment variable, use that.
+* The default value is `/usr/bin/vi`.
+
+Here's sample Python code implementing those semantics:
+
+```Python
+    default_editor = os.environ.get("VISUAL",
+        os.environ.get("EDITOR", "/usr/bin/vi"))
+    @dataclasses.dataclass
+    class ConfigFile:
+        editor:str=default_editor
+
+    d = perky.load(os.path.expanduser("~/.myprogramrc"))
+    app = appeal.Appeal()
+    config_file = app.read_mapping(ConfigFile, d)
+
+    @app.global_command()
+    def global_command(*, editor=config_file.editor):
+        print(f"editor = {editor}")
+
+    app.main()
+```
+
+Note: using `os.path.expanduser` and a hard-coded filename
+like this is no longer considered best practice.  You should use 
+[`platformdirs`](https://pypi.org/project/platformdirs/) to
+define the paths to your config files.
+
+### Nesting
+
+Appeal's config file reader supports reading values from nested dicts.
+This maps directly onto nested function calls in annotations.  If an
+annotation takes two or more parameters, the name of the parameter
+with that annotation will be used as the name of the nested dict.
+
+Since that probably wasn't clear--sorry!--an example would probably help.
+Consider this example dictionary:
+
+```Python
+    d = {
+        'a': 33,
+        'b': {
+            'verbose': True,
+            'color': 'blue',
+        },
+    }
+```
+
+Here the value of `'b'` is a nested dict.  If we want Appeal to read
+a dict with this shape, it will have to descend into that nested dict.
+Appeal does that by default when a parameter has an annotation, and
+the annotation takes two or more parameters.  Here's sample Python
+showing how to read this dict using Appeal:
+
+```Python
+    def read_b(verbose=False, color='black'):
+        return (verbose, color)
+
+    def config_file(a: int, b: read_b):
+        return (a, b)
+```
+
+Because `read_b` is an annotation taking multiple parameters,
+Appeal will assume the value of `'b'` is a nested dict,
+and will get the values of `'verbose'` and `'color'` from
+that dict.
+
+If you don't want this behavior, you can disable it by
+decorating the annotation function with the `unnested`
+method on the Appeal object.  If we change the code to
+the following:
+
+```Python
+    @app.unnested()
+    def read_b(verbose=False, color='black'):
+        return (verbose, color)
+
+    def config_file(a: int, b: read_b):
+        return (a, b)
+```
+
+Appeal *won't* descend into a nested dict named `'b'`.
+In this case the dictionary would have to be be completely
+flat, like this:
+
+```Python
+    d = { 'a': 33, 'verbose': True, 'color': 'blue' }
+```
+
+### Iterables
+
+Appeal can also read from iterables inside the dictionary.
+The parameter that accepts an iterable should be annotated
+with a subclass of `MultiOption`.  Appeal will instantiate
+the `MultiOption` and use the MultiOption protocol to
+fill the object.
+
+For example, if your config file dict looked like this:
+
+```Python
+    d = {
+        'color': 'blue',
+        'lines': [
+            'line 1',
+            'here is line 2',
+            'and finally, line 3',
+            ]
+    }
+```
+
+Appeal could map it to this callable:
+
+```Python
+    @dataclasses.dataclass
+    class ConfigFile:
+        lines: appeal.accumulator
+        color:str = ''
+```
+
+If the `MultiOption` option takes multiple parameters,
+then the list must contain dictionaries.  For example,
+this Python code:
+
+```Python
+    class Resolutions(appeal.Multioption):
+        def init(self, default=None):
+            self.default = default
+            self.values = None
+
+        def option(self, width:int, height:int, depth:int):
+            if self.values is None:
+                self.values = []
+            self.values.append((width, height, depth))
+
+        def render(self):
+            if self.values is None:
+                return self.default
+            return self.values
+
+    @dataclasses.dataclass
+    class ConfigFile:
+        resolutions: Resolutions
+        color:str = ''
+```
+
+Would be able to read this mapping:
+
+```Python
+    d = {
+        'color': 'orange',
+        'resolutions': [
+            {'width': 1280, 'height': 1024, 'depth': 24},
+            {'width': 1600, 'height': 1200, 'depth': 16},
+        ],
+    }
+```
+
+
+### `read_iterable`
+
+In addition to Appeal's `read_mapping` method, Appeal
+also supports a `read_iterable` method.  The API is
+almost identical:
+
+```Python
+    Appeal.read_iterable(callable, iterable)
+```
+
+However this function is much simpler.  The iterable
+should itself be an iterable of iterables.  Appeal will
+call the callable you specify once for every nested
+iterable.  The result will be appended to a list, and
+`read_iterable` will return that list.
+
+As always, Appeal will handle converting values using
+the annotations you specify.  Unlike `read_mapping`,
+here you may pass in a function accepting `*args`,
+in which case Appeal will process an arbitrary number
+of trailing arguments.  Also unlike `read_mapping`,
+there's no support for testing--neither nested dictionaties
+nor (further) nested lists.  (Like when processing the
+command-line, when reading values from the iterable,
+nested annotations get flattened.)
+
+### CSV files
+
+Finally, Appeal has special support for reading CSV files.  This may
+seem like an odd thing to support--nobody uses CSV files as config
+files.  But CSV files were the proof-of-concept for Appeal's config
+file support, and it's proved useful in another project, so for
+now it's staying in.  There's a special method for reading CSV
+files:
+
+```Python
+    Appeal.read_csv(self, callable, csv_reader, *, first_row_map=None)
+```
+
+You pass in your callable, and a fresh `csv.reader` object.  Appeal
+will read the rows out of the `CSV` object, passing in the strings into
+the `callable`, and append the result to a list.  The return value is
+that list.
+
+If `first_row_map` is false, `read_csv` will ignore the first line of
+the CSV file (the "column names" line) and pass in the values from the
+CSV file by position.  If `first_row_map` is true, `read_csv` will use
+the rows from the first line of the CSV file as keys in a dictionary,
+populate the values with each subsequent row, and will pass the
+arguments by name.
+
+In other words, if `first_row_map` is false, Appeal calls
+
+```Python
+    callable(*row)
+```
+
+for every line after the first line in the CSV file.  And if `first_row_map`
+is true, Appeal calls
+
+```Python
+    d = {key: value for key, value in zip(column_headers, row)}
+    callable(**d)
+```
+
+for every line after the first line in the CSV file.
+
+
 ## API Reference
 
 `Appeal(help=True, version=None, positional_argument_usage_format="{name}", default_options=default_options)`
 
 Creates a new Appeal instance.
 
 If `help` is true, Appeal automatically adds help support to
@@ -1679,20 +1994,20 @@
 
 Raises `AppealConfigurationError` if any `option` has already been
 mapped inside this `Appeal` instance *with a different signature.*
 
 (Doesn't modify `callable` in any way.)
 
 
-`Appeal.argument(self, parameter_name, *, usage=None)`
+`Appeal.parameter(self, parameter_name, *, usage=None)`
 
 Used as a decorator.  Returns a callable that accepts a single
 parameter `callable`, which must be a callable.
 
-Allos for configuration of a positional (or positional-or-keyword)
+Allows for configuration of a positional (or positional-or-keyword)
 parameter on a command function or converter.  `parameter_name` is the
 name of the parameter; it must be a parameter of the decorated `callable`.
 
 Currently the only supported configuration is `usage`, which specifies
 the string that will represent this parameter in usage information.
 
 (Doesn't modify `callable` in any way.)
@@ -1900,14 +2215,28 @@
   with `appeal.split`.  But it also permits options that consume
   multiple separate opargs from the command-line.
 * POSIX requires that all options be specified before any positional
   arguments.  Appeal doesn't enforce this, and will happily consume
   options and positional arguments in any order.  In fact,
   "subcommands" require permitting options after positional arguments
   for anything beyond the simplest possible subcommand support.
+* POSIX requires that, if an option (short option) has a single
+  *optional* argument (oparg), its argument must be concatenated
+  to the option.  For example, if `-f` takes an optional argument,
+  and you want to specify the argument `guava`, you *must* write
+  this as `-fguava`, no other spelling is permissible.  While Appeal
+  supports this spelling, it also supports `-f=guava` and `-f guava`.
+  More importantly, if you specify `-f` on your command-line (and
+  not `-f=<something>` or `-f<something>`), Appeal *will* consume the
+  next argument on the command-line as an oparg, which is what POSIX
+  definitely does *not* want.  I feel Appeal's consistency is
+  more important than supporting this syntactic hack.  Note that
+  the oparg is still optional, so if `-f` is the last thing
+  on your command-line, that will achieve this "option with
+  default value" behavior.
 
 
 ## Additional Subtle Features And Behaviors
 
 * You can specify options and arguments in any order on a
   command-line, Appeal doesn't care.  If you want Appeal to
   stop recognizing arguments starting with dashes as options,
@@ -1934,15 +2263,15 @@
 * You shouldn't call `usage()` until you've added all the
   commands, options, and parameters information into your
   Appeal object.  Why?  Because, for example, `usage()`
   computes the default options for keyword-only parameters
   that haven't gotten any explicitly defined options.
   But if you then define one of those options, Appeal will
   throw an error at you.
-* Almost any callable can be a converter.  But not every
+* Almost any callable can be a converter--but not *every*
   function.  There are two limitations.  First, as already
   mentioned, in order for a function to be a legal converter,
   every keyword-only parameter must have a default value.
   The second requirement is more specific: in order to use
   a function as a converter for a `*args*` parameter,
   *somewhere* in the annotations tree under that function,
   some function must take a required positional parameter.
@@ -1978,14 +2307,68 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.6**
+
+A huge upgrade!
+
+* A new feature: Appeal can now read configuration files!
+  Check out the new APIs `Appeal.read_mapping`,
+  `Appeal.read_iterable`, and even `Appeal.read_csv`.
+  This was a massive undertaking and involved a big
+  overhaul of the compiler.
+
+* The biggest change to existing behavior: Appeal now
+  early-maps options.  (See issue #3.)
+  In short: when options are only defined in an optional group,
+  they get provisionally mapped (made available) *before* the first
+  argument in that group.  Using that option enters the group just
+  like specifying the first argument in that group.  You'll see
+  the difference in usage; an optional group that mapped an option
+  used to look like `[a [-v|--verbose] b c]` but now looks like
+  `[[-v|--verbose] a b c]`.
+
+* Appeal now handles multiple short options smashed together
+  (e.g. `-ace`) *identically* to them being specified separately
+  (e.g. `-a -c -e`).  This caused an observable change in behavior
+  regarding when child options get unmapped.
+
+  - Appeal only permits using child options in a limited context:
+    it must be after the parent option is executed, it
+    must be after the parent option has consumed all its required
+    *or optional* opargs, and it must be before any top-level
+    positional argument or option mapped before the parent option
+    was executed.  But Appeal was lax about enforcing these rules
+    when using multiple short options smashed together (e.g. `-ace`);
+    it would handle all the options and *then* unmap child options
+    as needed.  The good news: Appeal now enforces these rules here
+    too.  (The old behavior seems to have been *intentional* on my
+    part--what was I *thinking?!)*
+
+* The usage message raised for an unknown option is now much
+  better.  If the option is defined anywhere in the program
+  being run, it prints a different message telling you it
+  can't be used here, but also tells you where it can be used.
+  For example, if you use option `-x`, but that's a child
+  option mapped by `--parent`, the message would say
+  `-x can't be used here, it must be used immediately after --parent`.
+
+* Renamed `Appeal.argument` to `Appeal.parameter`.
+  This was one of those "what was I *thinking?"* moments.
+  The function affects the parameter, not the argument.
+  The old name still works but will be removed before 1.0.
+
+* `short_option_concatenated_oparg` is now more strictly
+  enforced: it's only permitted for short options that have
+  *exactly one* **optional** oparg, as specified by POSIX.
+
 **0.5.9**
 
 * Improved the error message generated when you have a
   required parameter after a `VAR_POSITIONAL` parameter.
   (This command-line can never succeed, because the
   `VAR_POSITIONAL` consumes all remaining arguments on
   the command-line, which means the subsequent required
```

