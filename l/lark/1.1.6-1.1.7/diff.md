# Comparing `tmp/lark-1.1.6.tar.gz` & `tmp/lark-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lark-1.1.6.tar", last modified: Tue Jul 18 06:46:16 2023, max compression
+gzip compressed data, was "lark-1.1.7.tar", last modified: Thu Jul 20 19:17:57 2023, max compression
```

## Comparing `lark-1.1.6.tar` & `lark-1.1.7.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.601302 lark-1.1.6/
--rw-rw-rw-   0        0        0     1073 2022-10-27 19:06:36.000000 lark-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      174 2022-05-27 06:53:04.000000 lark-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1671 2023-07-18 06:46:16.601302 lark-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     9478 2023-06-07 10:50:02.000000 lark-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.480528 lark-1.1.6/docs/
--rw-rw-rw-   0        0        0      622 2022-10-27 19:06:36.000000 lark-1.1.6/docs/Makefile
--rw-rw-rw-   0        0        0     2600 2022-10-27 19:06:36.000000 lark-1.1.6/docs/classes.rst
--rw-rw-rw-   0        0        0     5686 2023-06-10 14:39:54.000000 lark-1.1.6/docs/conf.py
--rw-rw-rw-   0        0        0     2200 2023-06-10 14:37:09.000000 lark-1.1.6/docs/features.md
--rw-rw-rw-   0        0        0     1989 2022-05-27 06:53:04.000000 lark-1.1.6/docs/forest.rst
--rw-rw-rw-   0        0        0     9839 2023-03-07 11:13:42.000000 lark-1.1.6/docs/grammar.md
--rw-rw-rw-   0        0        0     1831 2022-10-27 19:06:36.000000 lark-1.1.6/docs/how_to_develop.md
--rw-rw-rw-   0        0        0     6092 2023-05-05 08:59:47.000000 lark-1.1.6/docs/how_to_use.md
--rw-rw-rw-   0        0        0     3092 2023-05-05 08:59:47.000000 lark-1.1.6/docs/index.rst
--rw-rw-rw-   0        0        0    15471 2022-05-27 06:53:04.000000 lark-1.1.6/docs/json_tutorial.md
--rwxrwxrwx   0        0        0      808 2022-05-27 06:53:04.000000 lark-1.1.6/docs/make.bat
--rw-rw-rw-   0        0        0     5176 2022-05-27 06:53:04.000000 lark-1.1.6/docs/parsers.md
--rw-rw-rw-   0        0        0     2798 2022-10-27 19:06:36.000000 lark-1.1.6/docs/philosophy.md
--rw-rw-rw-   0        0        0     4989 2023-05-05 08:59:47.000000 lark-1.1.6/docs/recipes.md
--rw-rw-rw-   0        0        0      211 2023-06-10 14:13:24.000000 lark-1.1.6/docs/requirements.txt
--rw-rw-rw-   0        0        0     1971 2022-10-27 19:06:36.000000 lark-1.1.6/docs/tools.md
--rw-rw-rw-   0        0        0     3646 2022-05-27 06:53:04.000000 lark-1.1.6/docs/tree_construction.md
--rw-rw-rw-   0        0        0     3116 2022-10-27 19:06:36.000000 lark-1.1.6/docs/visitors.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.489530 lark-1.1.6/examples/
--rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.6/examples/__init__.py
--rw-rw-rw-   0        0        0     1707 2022-05-27 06:53:04.000000 lark-1.1.6/examples/calc.py
--rw-rw-rw-   0        0        0    93975 2021-12-05 10:20:58.000000 lark-1.1.6/examples/fruitflies.png
--rw-rw-rw-   0        0        0     1177 2022-05-27 06:53:04.000000 lark-1.1.6/examples/fruitflies.py
--rw-rw-rw-   0        0        0     1125 2022-10-27 19:06:36.000000 lark-1.1.6/examples/indented_tree.py
--rw-rw-rw-   0        0        0     2615 2023-05-05 08:59:43.000000 lark-1.1.6/examples/json_parser.py
--rw-rw-rw-   0        0        0     1071 2022-05-27 06:53:04.000000 lark-1.1.6/examples/lark_grammar.py
--rw-rw-rw-   0        0        0     2031 2022-05-27 06:53:04.000000 lark-1.1.6/examples/turtle_dsl.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.509529 lark-1.1.6/lark/
--rw-rw-rw-   0        0        0      782 2023-07-17 20:01:37.000000 lark-1.1.6/lark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.535530 lark-1.1.6/lark/__pyinstaller/
--rw-rw-rw-   0        0        0      188 2022-10-27 19:06:36.000000 lark-1.1.6/lark/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      613 2022-05-27 06:53:04.000000 lark-1.1.6/lark/__pyinstaller/hook-lark.py
--rw-rw-rw-   0        0        0     2151 2023-05-23 10:20:04.000000 lark-1.1.6/lark/ast_utils.py
--rw-rw-rw-   0        0        0     2982 2023-07-06 10:42:57.000000 lark-1.1.6/lark/common.py
--rw-rw-rw-   0        0        0    11231 2023-01-30 01:16:21.000000 lark-1.1.6/lark/exceptions.py
--rw-rw-rw-   0        0        0     3549 2022-05-27 06:53:04.000000 lark-1.1.6/lark/grammar.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.541529 lark-1.1.6/lark/grammars/
--rw-rw-rw-   0        0        0        0 2022-08-25 09:44:15.000000 lark-1.1.6/lark/grammars/__init__.py
--rw-rw-rw-   0        0        0      944 2022-05-27 06:53:04.000000 lark-1.1.6/lark/grammars/common.lark
--rw-rw-rw-   0        0        0     1603 2023-06-09 17:35:28.000000 lark-1.1.6/lark/grammars/lark.lark
--rw-rw-rw-   0        0        0    10943 2023-01-30 01:16:21.000000 lark-1.1.6/lark/grammars/python.lark
--rw-rw-rw-   0        0        0      103 2022-05-27 06:53:04.000000 lark-1.1.6/lark/grammars/unicode.lark
--rw-rw-rw-   0        0        0     3188 2022-05-27 06:53:04.000000 lark-1.1.6/lark/indenter.py
--rw-rw-rw-   0        0        0    28584 2023-07-06 09:07:59.000000 lark-1.1.6/lark/lark.py
--rw-rw-rw-   0        0        0    24191 2023-06-07 10:50:02.000000 lark-1.1.6/lark/lexer.py
--rw-rw-rw-   0        0        0    54906 2023-05-05 08:59:47.000000 lark-1.1.6/lark/load_grammar.py
--rw-rw-rw-   0        0        0    14718 2023-07-06 09:07:59.000000 lark-1.1.6/lark/parse_tree_builder.py
--rw-rw-rw-   0        0        0    10304 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parser_frontends.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.552528 lark-1.1.6/lark/parsers/
--rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.6/lark/parsers/__init__.py
--rw-rw-rw-   0        0        0    12532 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parsers/cyk.py
--rw-rw-rw-   0        0        0    14548 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parsers/earley.py
--rw-rw-rw-   0        0        0     1623 2022-10-27 19:06:36.000000 lark-1.1.6/lark/parsers/earley_common.py
--rw-rw-rw-   0        0        0    32181 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parsers/earley_forest.py
--rw-rw-rw-   0        0        0     6650 2023-05-05 08:59:47.000000 lark-1.1.6/lark/parsers/grammar_analysis.py
--rw-rw-rw-   0        0        0    11276 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parsers/lalr_analysis.py
--rw-rw-rw-   0        0        0     5446 2023-06-26 20:02:59.000000 lark-1.1.6/lark/parsers/lalr_interactive_parser.py
--rw-rw-rw-   0        0        0     7441 2023-06-07 10:50:02.000000 lark-1.1.6/lark/parsers/lalr_parser.py
--rw-rw-rw-   0        0        0     7664 2022-05-27 06:53:04.000000 lark-1.1.6/lark/parsers/xearley.py
--rw-rw-rw-   0        0        0        0 2022-05-27 06:53:04.000000 lark-1.1.6/lark/py.typed
--rw-rw-rw-   0        0        0     3822 2023-06-07 10:50:02.000000 lark-1.1.6/lark/reconstruct.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.557529 lark-1.1.6/lark/tools/
--rw-rw-rw-   0        0        0     2615 2023-03-09 09:50:28.000000 lark-1.1.6/lark/tools/__init__.py
--rw-rw-rw-   0        0        0     6467 2022-05-27 06:53:04.000000 lark-1.1.6/lark/tools/nearley.py
--rw-rw-rw-   0        0        0      997 2023-06-07 10:50:02.000000 lark-1.1.6/lark/tools/serialize.py
--rw-rw-rw-   0        0        0     5744 2022-10-27 18:18:30.000000 lark-1.1.6/lark/tools/standalone.py
--rw-rw-rw-   0        0        0     9025 2023-07-06 09:07:59.000000 lark-1.1.6/lark/tree.py
--rw-rw-rw-   0        0        0     6189 2023-01-30 01:16:21.000000 lark-1.1.6/lark/tree_matcher.py
--rw-rw-rw-   0        0        0     6139 2023-01-30 01:16:21.000000 lark-1.1.6/lark/tree_templates.py
--rw-rw-rw-   0        0        0    11319 2023-06-07 10:50:02.000000 lark-1.1.6/lark/utils.py
--rw-rw-rw-   0        0        0    21683 2022-10-27 19:06:36.000000 lark-1.1.6/lark/visitors.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.533527 lark-1.1.6/lark.egg-info/
--rw-rw-rw-   0        0        0     1671 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3058 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-18 06:46:16.000000 lark-1.1.6/lark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2698 2023-07-17 20:01:07.000000 lark-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 06:46:16.602303 lark-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.587303 lark-1.1.6/tests/
--rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1154 2022-10-27 18:18:30.000000 lark-1.1.6/tests/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.596305 lark-1.1.6/tests/grammars/
--rw-rw-rw-   0        0        0       95 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/ab.lark
--rw-rw-rw-   0        0        0       40 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/leading_underscore_grammar.lark
--rw-rw-rw-   0        0        0       36 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/templates.lark
--rw-rw-rw-   0        0        0       63 2021-12-05 10:20:58.000000 lark-1.1.6/tests/grammars/test.lark
--rw-rw-rw-   0        0        0      108 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/test_relative_import_of_nested_grammar.lark
--rw-rw-rw-   0        0        0      118 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/test_relative_import_of_nested_grammar__grammar_to_import.lark
--rw-rw-rw-   0        0        0       22 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/test_relative_import_of_nested_grammar__nested_grammar.lark
--rw-rw-rw-   0        0        0       27 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/test_unicode.lark
--rw-rw-rw-   0        0        0       48 2022-05-27 06:53:04.000000 lark-1.1.6/tests/grammars/three_rules_using_same_token.lark
--rw-rw-rw-   0        0        0     6365 2023-03-07 11:13:42.000000 lark-1.1.6/tests/test_cache.py
--rw-rw-rw-   0        0        0     9779 2022-10-27 19:06:36.000000 lark-1.1.6/tests/test_grammar.py
--rw-rw-rw-   0        0        0      490 2022-10-27 19:06:36.000000 lark-1.1.6/tests/test_lexer.py
--rw-rw-rw-   0        0        0     2849 2023-05-05 08:59:47.000000 lark-1.1.6/tests/test_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.598304 lark-1.1.6/tests/test_nearley/
--rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.6/tests/test_nearley/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:46:16.600304 lark-1.1.6/tests/test_nearley/grammars/
--rw-rw-rw-   0        0        0       36 2021-12-05 10:20:58.000000 lark-1.1.6/tests/test_nearley/grammars/include_unicode.ne
--rw-rw-rw-   0        0        0       12 2021-12-05 10:20:58.000000 lark-1.1.6/tests/test_nearley/grammars/unicode.ne
--rw-rw-rw-   0        0        0     3360 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_nearley/test_nearley.py
--rw-rw-rw-   0        0        0    95618 2023-05-23 12:11:53.000000 lark-1.1.6/tests/test_parser.py
--rw-rw-rw-   0        0        0     1188 2022-10-27 19:06:36.000000 lark-1.1.6/tests/test_pattern_matching.py
--rw-rw-rw-   0        0        0     7402 2022-10-27 19:06:36.000000 lark-1.1.6/tests/test_python_grammar.py
--rw-rw-rw-   0        0        0     5376 2023-01-30 01:16:21.000000 lark-1.1.6/tests/test_reconstructor.py
--rw-rw-rw-   0        0        0      107 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_import.lark
--rw-rw-rw-   0        0        0       58 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_import_preserves_leading_underscore.lark
--rw-rw-rw-   0        0        0      107 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_import_rename.lark
--rw-rw-rw-   0        0        0      171 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_import_rules_dependencies_imported_only_once.lark
--rw-rw-rw-   0        0        0       56 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_import_unicode.lark
--rw-rw-rw-   0        0        0       77 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_multi_import.lark
--rw-rw-rw-   0        0        0       66 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_rule_import.lark
--rw-rw-rw-   0        0        0       66 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_rule_import_drop_ignore.lark
--rw-rw-rw-   0        0        0       70 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_rule_import_rename.lark
--rw-rw-rw-   0        0        0       72 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_rule_import_subrule.lark
--rw-rw-rw-   0        0        0       86 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_relative_rule_import_subrule_no_conflict.lark
--rw-rw-rw-   0        0        0       92 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_templates_import.lark
--rw-rw-rw-   0        0        0     4109 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_tools.py
--rw-rw-rw-   0        0        0     7384 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_tree_forest_transformer.py
--rw-rw-rw-   0        0        0     9022 2022-08-25 09:44:15.000000 lark-1.1.6/tests/test_tree_templates.py
--rw-rw-rw-   0        0        0    14972 2022-05-27 06:53:04.000000 lark-1.1.6/tests/test_trees.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:57.119049 lark-1.1.7/
+-rw-rw-rw-   0        0        0     1073 2022-10-27 19:06:36.000000 lark-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      174 2022-05-27 06:53:04.000000 lark-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1671 2023-07-20 19:17:57.119049 lark-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9478 2023-06-07 10:50:02.000000 lark-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.747337 lark-1.1.7/docs/
+-rw-rw-rw-   0        0        0      622 2022-10-27 19:06:36.000000 lark-1.1.7/docs/Makefile
+-rw-rw-rw-   0        0        0     2600 2022-10-27 19:06:36.000000 lark-1.1.7/docs/classes.rst
+-rw-rw-rw-   0        0        0     5686 2023-06-10 14:39:54.000000 lark-1.1.7/docs/conf.py
+-rw-rw-rw-   0        0        0     2200 2023-06-10 14:37:09.000000 lark-1.1.7/docs/features.md
+-rw-rw-rw-   0        0        0     1989 2022-05-27 06:53:04.000000 lark-1.1.7/docs/forest.rst
+-rw-rw-rw-   0        0        0     9839 2023-03-07 11:13:42.000000 lark-1.1.7/docs/grammar.md
+-rw-rw-rw-   0        0        0     1831 2022-10-27 19:06:36.000000 lark-1.1.7/docs/how_to_develop.md
+-rw-rw-rw-   0        0        0     6092 2023-05-05 08:59:47.000000 lark-1.1.7/docs/how_to_use.md
+-rw-rw-rw-   0        0        0     3092 2023-05-05 08:59:47.000000 lark-1.1.7/docs/index.rst
+-rw-rw-rw-   0        0        0    15471 2022-05-27 06:53:04.000000 lark-1.1.7/docs/json_tutorial.md
+-rwxrwxrwx   0        0        0      808 2022-05-27 06:53:04.000000 lark-1.1.7/docs/make.bat
+-rw-rw-rw-   0        0        0     5176 2022-05-27 06:53:04.000000 lark-1.1.7/docs/parsers.md
+-rw-rw-rw-   0        0        0     2798 2022-10-27 19:06:36.000000 lark-1.1.7/docs/philosophy.md
+-rw-rw-rw-   0        0        0     4989 2023-05-05 08:59:47.000000 lark-1.1.7/docs/recipes.md
+-rw-rw-rw-   0        0        0      211 2023-06-10 14:13:24.000000 lark-1.1.7/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1971 2022-10-27 19:06:36.000000 lark-1.1.7/docs/tools.md
+-rw-rw-rw-   0        0        0     3646 2022-05-27 06:53:04.000000 lark-1.1.7/docs/tree_construction.md
+-rw-rw-rw-   0        0        0     3116 2022-10-27 19:06:36.000000 lark-1.1.7/docs/visitors.rst
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.804365 lark-1.1.7/examples/
+-rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.7/examples/__init__.py
+-rw-rw-rw-   0        0        0     1707 2022-05-27 06:53:04.000000 lark-1.1.7/examples/calc.py
+-rw-rw-rw-   0        0        0    93975 2021-12-05 10:20:58.000000 lark-1.1.7/examples/fruitflies.png
+-rw-rw-rw-   0        0        0     1177 2022-05-27 06:53:04.000000 lark-1.1.7/examples/fruitflies.py
+-rw-rw-rw-   0        0        0     1125 2022-10-27 19:06:36.000000 lark-1.1.7/examples/indented_tree.py
+-rw-rw-rw-   0        0        0     2615 2023-05-05 08:59:43.000000 lark-1.1.7/examples/json_parser.py
+-rw-rw-rw-   0        0        0     1071 2022-05-27 06:53:04.000000 lark-1.1.7/examples/lark_grammar.py
+-rw-rw-rw-   0        0        0     2031 2022-05-27 06:53:04.000000 lark-1.1.7/examples/turtle_dsl.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.836375 lark-1.1.7/lark/
+-rw-rw-rw-   0        0        0      782 2023-07-20 19:17:30.000000 lark-1.1.7/lark/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.865541 lark-1.1.7/lark/__pyinstaller/
+-rw-rw-rw-   0        0        0      188 2022-10-27 19:06:36.000000 lark-1.1.7/lark/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      613 2022-05-27 06:53:04.000000 lark-1.1.7/lark/__pyinstaller/hook-lark.py
+-rw-rw-rw-   0        0        0     2151 2023-05-23 10:20:04.000000 lark-1.1.7/lark/ast_utils.py
+-rw-rw-rw-   0        0        0     2982 2023-07-06 10:42:57.000000 lark-1.1.7/lark/common.py
+-rw-rw-rw-   0        0        0    11231 2023-01-30 01:16:21.000000 lark-1.1.7/lark/exceptions.py
+-rw-rw-rw-   0        0        0     3549 2022-05-27 06:53:04.000000 lark-1.1.7/lark/grammar.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.885540 lark-1.1.7/lark/grammars/
+-rw-rw-rw-   0        0        0        0 2022-08-25 09:44:15.000000 lark-1.1.7/lark/grammars/__init__.py
+-rw-rw-rw-   0        0        0      944 2022-05-27 06:53:04.000000 lark-1.1.7/lark/grammars/common.lark
+-rw-rw-rw-   0        0        0     1603 2023-06-09 17:35:28.000000 lark-1.1.7/lark/grammars/lark.lark
+-rw-rw-rw-   0        0        0    10943 2023-01-30 01:16:21.000000 lark-1.1.7/lark/grammars/python.lark
+-rw-rw-rw-   0        0        0      103 2022-05-27 06:53:04.000000 lark-1.1.7/lark/grammars/unicode.lark
+-rw-rw-rw-   0        0        0     3188 2022-05-27 06:53:04.000000 lark-1.1.7/lark/indenter.py
+-rw-rw-rw-   0        0        0    28584 2023-07-06 09:07:59.000000 lark-1.1.7/lark/lark.py
+-rw-rw-rw-   0        0        0    24191 2023-06-07 10:50:02.000000 lark-1.1.7/lark/lexer.py
+-rw-rw-rw-   0        0        0    54906 2023-05-05 08:59:47.000000 lark-1.1.7/lark/load_grammar.py
+-rw-rw-rw-   0        0        0    14717 2023-07-20 19:17:30.000000 lark-1.1.7/lark/parse_tree_builder.py
+-rw-rw-rw-   0        0        0    10304 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parser_frontends.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.905548 lark-1.1.7/lark/parsers/
+-rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.7/lark/parsers/__init__.py
+-rw-rw-rw-   0        0        0    12532 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parsers/cyk.py
+-rw-rw-rw-   0        0        0    14548 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parsers/earley.py
+-rw-rw-rw-   0        0        0     1623 2022-10-27 19:06:36.000000 lark-1.1.7/lark/parsers/earley_common.py
+-rw-rw-rw-   0        0        0    32181 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parsers/earley_forest.py
+-rw-rw-rw-   0        0        0     6650 2023-05-05 08:59:47.000000 lark-1.1.7/lark/parsers/grammar_analysis.py
+-rw-rw-rw-   0        0        0    11276 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parsers/lalr_analysis.py
+-rw-rw-rw-   0        0        0     5446 2023-06-26 20:02:59.000000 lark-1.1.7/lark/parsers/lalr_interactive_parser.py
+-rw-rw-rw-   0        0        0     7441 2023-06-07 10:50:02.000000 lark-1.1.7/lark/parsers/lalr_parser.py
+-rw-rw-rw-   0        0        0     7664 2022-05-27 06:53:04.000000 lark-1.1.7/lark/parsers/xearley.py
+-rw-rw-rw-   0        0        0        0 2022-05-27 06:53:04.000000 lark-1.1.7/lark/py.typed
+-rw-rw-rw-   0        0        0     3822 2023-06-07 10:50:02.000000 lark-1.1.7/lark/reconstruct.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.913548 lark-1.1.7/lark/tools/
+-rw-rw-rw-   0        0        0     2615 2023-03-09 09:50:28.000000 lark-1.1.7/lark/tools/__init__.py
+-rw-rw-rw-   0        0        0     6467 2022-05-27 06:53:04.000000 lark-1.1.7/lark/tools/nearley.py
+-rw-rw-rw-   0        0        0      997 2023-06-07 10:50:02.000000 lark-1.1.7/lark/tools/serialize.py
+-rw-rw-rw-   0        0        0     5744 2022-10-27 18:18:30.000000 lark-1.1.7/lark/tools/standalone.py
+-rw-rw-rw-   0        0        0     9025 2023-07-06 09:07:59.000000 lark-1.1.7/lark/tree.py
+-rw-rw-rw-   0        0        0     6189 2023-01-30 01:16:21.000000 lark-1.1.7/lark/tree_matcher.py
+-rw-rw-rw-   0        0        0     6139 2023-01-30 01:16:21.000000 lark-1.1.7/lark/tree_templates.py
+-rw-rw-rw-   0        0        0    11319 2023-06-07 10:50:02.000000 lark-1.1.7/lark/utils.py
+-rw-rw-rw-   0        0        0    21916 2023-07-20 19:17:30.000000 lark-1.1.7/lark/visitors.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:56.861541 lark-1.1.7/lark.egg-info/
+-rw-rw-rw-   0        0        0     1671 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3058 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-20 19:17:56.000000 lark-1.1.7/lark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2698 2023-07-17 20:01:07.000000 lark-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 19:17:57.119049 lark-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:57.032233 lark-1.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1154 2022-10-27 18:18:30.000000 lark-1.1.7/tests/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:57.103043 lark-1.1.7/tests/grammars/
+-rw-rw-rw-   0        0        0       95 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/ab.lark
+-rw-rw-rw-   0        0        0       40 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/leading_underscore_grammar.lark
+-rw-rw-rw-   0        0        0       36 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/templates.lark
+-rw-rw-rw-   0        0        0       63 2021-12-05 10:20:58.000000 lark-1.1.7/tests/grammars/test.lark
+-rw-rw-rw-   0        0        0      108 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/test_relative_import_of_nested_grammar.lark
+-rw-rw-rw-   0        0        0      118 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/test_relative_import_of_nested_grammar__grammar_to_import.lark
+-rw-rw-rw-   0        0        0       22 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/test_relative_import_of_nested_grammar__nested_grammar.lark
+-rw-rw-rw-   0        0        0       27 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/test_unicode.lark
+-rw-rw-rw-   0        0        0       48 2022-05-27 06:53:04.000000 lark-1.1.7/tests/grammars/three_rules_using_same_token.lark
+-rw-rw-rw-   0        0        0     6365 2023-03-07 11:13:42.000000 lark-1.1.7/tests/test_cache.py
+-rw-rw-rw-   0        0        0     9779 2022-10-27 19:06:36.000000 lark-1.1.7/tests/test_grammar.py
+-rw-rw-rw-   0        0        0      490 2022-10-27 19:06:36.000000 lark-1.1.7/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     2849 2023-05-05 08:59:47.000000 lark-1.1.7/tests/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:57.103043 lark-1.1.7/tests/test_nearley/
+-rw-rw-rw-   0        0        0        0 2021-12-05 10:20:58.000000 lark-1.1.7/tests/test_nearley/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 19:17:57.115044 lark-1.1.7/tests/test_nearley/grammars/
+-rw-rw-rw-   0        0        0       36 2021-12-05 10:20:58.000000 lark-1.1.7/tests/test_nearley/grammars/include_unicode.ne
+-rw-rw-rw-   0        0        0       12 2021-12-05 10:20:58.000000 lark-1.1.7/tests/test_nearley/grammars/unicode.ne
+-rw-rw-rw-   0        0        0     3360 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_nearley/test_nearley.py
+-rw-rw-rw-   0        0        0    95618 2023-05-23 12:11:53.000000 lark-1.1.7/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1188 2022-10-27 19:06:36.000000 lark-1.1.7/tests/test_pattern_matching.py
+-rw-rw-rw-   0        0        0     7402 2022-10-27 19:06:36.000000 lark-1.1.7/tests/test_python_grammar.py
+-rw-rw-rw-   0        0        0     5376 2023-01-30 01:16:21.000000 lark-1.1.7/tests/test_reconstructor.py
+-rw-rw-rw-   0        0        0      107 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_import.lark
+-rw-rw-rw-   0        0        0       58 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_import_preserves_leading_underscore.lark
+-rw-rw-rw-   0        0        0      107 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_import_rename.lark
+-rw-rw-rw-   0        0        0      171 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_import_rules_dependencies_imported_only_once.lark
+-rw-rw-rw-   0        0        0       56 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_import_unicode.lark
+-rw-rw-rw-   0        0        0       77 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_multi_import.lark
+-rw-rw-rw-   0        0        0       66 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_rule_import.lark
+-rw-rw-rw-   0        0        0       66 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_rule_import_drop_ignore.lark
+-rw-rw-rw-   0        0        0       70 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_rule_import_rename.lark
+-rw-rw-rw-   0        0        0       72 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_rule_import_subrule.lark
+-rw-rw-rw-   0        0        0       86 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_relative_rule_import_subrule_no_conflict.lark
+-rw-rw-rw-   0        0        0       92 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_templates_import.lark
+-rw-rw-rw-   0        0        0     4109 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_tools.py
+-rw-rw-rw-   0        0        0     7384 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_tree_forest_transformer.py
+-rw-rw-rw-   0        0        0     9022 2022-08-25 09:44:15.000000 lark-1.1.7/tests/test_tree_templates.py
+-rw-rw-rw-   0        0        0    14972 2022-05-27 06:53:04.000000 lark-1.1.7/tests/test_trees.py
```

### Comparing `lark-1.1.6/LICENSE` & `lark-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/PKG-INFO` & `lark-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lark
-Version: 1.1.6
+Version: 1.1.7
 Summary: a modern parsing library
 Author-email: Erez Shinan <erezshin@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lark-parser/lark
 Project-URL: Download, https://github.com/lark-parser/lark/tarball/master
 Keywords: Earley,LALR,parser,parsing,ast
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lark-1.1.6/README.md` & `lark-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/Makefile` & `lark-1.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/classes.rst` & `lark-1.1.7/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/conf.py` & `lark-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/features.md` & `lark-1.1.7/docs/features.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/forest.rst` & `lark-1.1.7/docs/forest.rst`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/grammar.md` & `lark-1.1.7/docs/grammar.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/how_to_develop.md` & `lark-1.1.7/docs/how_to_develop.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/how_to_use.md` & `lark-1.1.7/docs/how_to_use.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/index.rst` & `lark-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/json_tutorial.md` & `lark-1.1.7/docs/json_tutorial.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/make.bat` & `lark-1.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/parsers.md` & `lark-1.1.7/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/philosophy.md` & `lark-1.1.7/docs/philosophy.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/recipes.md` & `lark-1.1.7/docs/recipes.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/tools.md` & `lark-1.1.7/docs/tools.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/tree_construction.md` & `lark-1.1.7/docs/tree_construction.md`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/docs/visitors.rst` & `lark-1.1.7/docs/visitors.rst`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/calc.py` & `lark-1.1.7/examples/calc.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/fruitflies.png` & `lark-1.1.7/examples/fruitflies.png`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/fruitflies.py` & `lark-1.1.7/examples/fruitflies.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/indented_tree.py` & `lark-1.1.7/examples/indented_tree.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/json_parser.py` & `lark-1.1.7/examples/json_parser.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/lark_grammar.py` & `lark-1.1.7/examples/lark_grammar.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/examples/turtle_dsl.py` & `lark-1.1.7/examples/turtle_dsl.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/__init__.py` & `lark-1.1.7/lark/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from .lark import Lark
 from .lexer import Token
 from .tree import ParseTree, Tree
 from .utils import logger
 from .visitors import Discard, Transformer, Transformer_NonRecursive, Visitor, v_args
 
-__version__: str = "1.1.6"
+__version__: str = "1.1.7"
 
 __all__ = (
     "GrammarError",
     "LarkError",
     "LexError",
     "ParseError",
     "UnexpectedCharacters",
```

### Comparing `lark-1.1.6/lark/__pyinstaller/hook-lark.py` & `lark-1.1.7/lark/__pyinstaller/hook-lark.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/ast_utils.py` & `lark-1.1.7/lark/ast_utils.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/common.py` & `lark-1.1.7/lark/common.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/exceptions.py` & `lark-1.1.7/lark/exceptions.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/grammar.py` & `lark-1.1.7/lark/grammar.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/grammars/common.lark` & `lark-1.1.7/lark/grammars/common.lark`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/grammars/lark.lark` & `lark-1.1.7/lark/grammars/lark.lark`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/grammars/python.lark` & `lark-1.1.7/lark/grammars/python.lark`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/indenter.py` & `lark-1.1.7/lark/indenter.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/lark.py` & `lark-1.1.7/lark/lark.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/lexer.py` & `lark-1.1.7/lark/lexer.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/load_grammar.py` & `lark-1.1.7/lark/load_grammar.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parse_tree_builder.py` & `lark-1.1.7/lark/parse_tree_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     res_meta.end_line = getattr(last_meta, 'container_end_line', last_meta.end_line)
                     res_meta.end_column = getattr(last_meta, 'container_end_column', last_meta.end_column)
                     res_meta.end_pos = getattr(last_meta, 'container_end_pos', last_meta.end_pos)
                     res_meta.empty = False
 
                 res_meta.container_end_line = getattr(last_meta, 'container_end_line', last_meta.end_line)
                 res_meta.container_end_column = getattr(last_meta, 'container_end_column', last_meta.end_column)
-                res_meta.container_end_pos = getattr(first_meta, 'container_end_pos', last_meta.end_pos)
+                res_meta.container_end_pos = getattr(last_meta, 'container_end_pos', last_meta.end_pos)
 
         return res
 
     def _pp_get_meta(self, children):
         for c in children:
             if self.node_filter is not None and not self.node_filter(c):
                 continue
```

### Comparing `lark-1.1.6/lark/parser_frontends.py` & `lark-1.1.7/lark/parser_frontends.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/cyk.py` & `lark-1.1.7/lark/parsers/cyk.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/earley.py` & `lark-1.1.7/lark/parsers/earley.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/earley_common.py` & `lark-1.1.7/lark/parsers/earley_common.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/earley_forest.py` & `lark-1.1.7/lark/parsers/earley_forest.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/grammar_analysis.py` & `lark-1.1.7/lark/parsers/grammar_analysis.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/lalr_analysis.py` & `lark-1.1.7/lark/parsers/lalr_analysis.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/lalr_interactive_parser.py` & `lark-1.1.7/lark/parsers/lalr_interactive_parser.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/lalr_parser.py` & `lark-1.1.7/lark/parsers/lalr_parser.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/parsers/xearley.py` & `lark-1.1.7/lark/parsers/xearley.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/reconstruct.py` & `lark-1.1.7/lark/reconstruct.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tools/__init__.py` & `lark-1.1.7/lark/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tools/nearley.py` & `lark-1.1.7/lark/tools/nearley.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tools/serialize.py` & `lark-1.1.7/lark/tools/serialize.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tools/standalone.py` & `lark-1.1.7/lark/tools/standalone.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tree.py` & `lark-1.1.7/lark/tree.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tree_matcher.py` & `lark-1.1.7/lark/tree_matcher.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/tree_templates.py` & `lark-1.1.7/lark/tree_templates.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/utils.py` & `lark-1.1.7/lark/utils.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/lark/visitors.py` & `lark-1.1.7/lark/visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,26 +516,32 @@
     it applies to all the callback methods inside it.
 
     ``v_args`` can be applied to a single method, or to an entire class. When applied to both,
     the options given to the method take precedence.
 
     Parameters:
         inline (bool, optional): Children are provided as ``*args`` instead of a list argument (not recommended for very long lists).
-        meta (bool, optional): Provides two arguments: ``children`` and ``meta`` (instead of just the first)
+        meta (bool, optional): Provides two arguments: ``meta`` and ``children`` (instead of just the latter)
         tree (bool, optional): Provides the entire tree as the argument, instead of the children.
         wrapper (function, optional): Provide a function to decorate all methods.
 
     Example:
         ::
 
             @v_args(inline=True)
             class SolveArith(Transformer):
                 def add(self, left, right):
                     return left + right
 
+                @v_args(meta=True)
+                def mul(self, meta, children):
+                    logger.info(f'mul at line {meta.line}')
+                    left, right = children
+                    return left * right
+
 
             class ReverseNotation(Transformer_InPlace):
                 @v_args(tree=True)
                 def tree_node(self, tree):
                     tree.children = tree.children[::-1]
     """
     if tree and (meta or inline):
```

### Comparing `lark-1.1.6/lark.egg-info/PKG-INFO` & `lark-1.1.7/lark.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lark
-Version: 1.1.6
+Version: 1.1.7
 Summary: a modern parsing library
 Author-email: Erez Shinan <erezshin@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lark-parser/lark
 Project-URL: Download, https://github.com/lark-parser/lark/tarball/master
 Keywords: Earley,LALR,parser,parsing,ast
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lark-1.1.6/lark.egg-info/SOURCES.txt` & `lark-1.1.7/lark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/pyproject.toml` & `lark-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/__main__.py` & `lark-1.1.7/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_cache.py` & `lark-1.1.7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_grammar.py` & `lark-1.1.7/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_logger.py` & `lark-1.1.7/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_nearley/test_nearley.py` & `lark-1.1.7/tests/test_nearley/test_nearley.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_parser.py` & `lark-1.1.7/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_pattern_matching.py` & `lark-1.1.7/tests/test_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_python_grammar.py` & `lark-1.1.7/tests/test_python_grammar.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_reconstructor.py` & `lark-1.1.7/tests/test_reconstructor.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_tools.py` & `lark-1.1.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_tree_forest_transformer.py` & `lark-1.1.7/tests/test_tree_forest_transformer.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_tree_templates.py` & `lark-1.1.7/tests/test_tree_templates.py`

 * *Files identical despite different names*

### Comparing `lark-1.1.6/tests/test_trees.py` & `lark-1.1.7/tests/test_trees.py`

 * *Files identical despite different names*

