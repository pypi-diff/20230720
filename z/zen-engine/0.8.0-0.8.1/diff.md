# Comparing `tmp/zen_engine-0.8.0.tar.gz` & `tmp/zen_engine-0.8.1.tar.gz`

## Comparing `zen_engine-0.8.0.tar` & `zen_engine-0.8.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.0/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    19250 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6816 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      783 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6339 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     4010 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     5318 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4286 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    14060 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2604 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9905 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    51034 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    22433 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.0/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123      972 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     5478 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3160 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.0/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-07-14 23:19:34.000000 zen_engine-0.8.0/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-07-14 23:19:34.000000 zen_engine-0.8.0/.gitignore
--rw-r--r--   0     1001      123     1057 2023-07-14 23:19:34.000000 zen_engine-0.8.0/LICENSE
--rw-r--r--   0     1001      123     5965 2023-07-14 23:19:34.000000 zen_engine-0.8.0/README.md
--rw-r--r--   0     1001      123     1578 2023-07-14 23:19:34.000000 zen_engine-0.8.0/index.py
--rw-r--r--   0     1001      123      966 2023-07-14 23:19:34.000000 zen_engine-0.8.0/pyproject.toml
--rw-r--r--   0     1001      123     1429 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/decision.rs
--rw-r--r--   0     1001      123     3012 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/value.rs
--rw-r--r--   0     1001      123    48278 2023-07-14 23:19:41.000000 zen_engine-0.8.0/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.1/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    19250 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6816 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      783 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6339 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     4010 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     5318 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4286 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    14053 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2604 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9905 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    51034 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    23163 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9097 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5185 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.1/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123      972 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     5478 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3160 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-07-20 20:44:12.000000 zen_engine-0.8.1/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.1/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-07-20 20:44:12.000000 zen_engine-0.8.1/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-07-20 20:44:12.000000 zen_engine-0.8.1/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-07-20 20:44:12.000000 zen_engine-0.8.1/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-07-20 20:44:12.000000 zen_engine-0.8.1/README.md
+-rw-r--r--   0     1001      123     1578 2023-07-20 20:44:12.000000 zen_engine-0.8.1/index.py
+-rw-r--r--   0     1001      123      966 2023-07-20 20:44:12.000000 zen_engine-0.8.1/pyproject.toml
+-rw-r--r--   0     1001      123     1429 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/decision.rs
+-rw-r--r--   0     1001      123     3012 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-07-20 20:44:12.000000 zen_engine-0.8.1/src/value.rs
+-rw-r--r--   0     1001      123    48279 2023-07-20 20:44:19.000000 zen_engine-0.8.1/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.1/PKG-INFO
```

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.8.1/local_dependencies/zen-expression/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Zen Expression Language"
 name = "zen-expression"
 license = "MIT"
-version = "0.7.0"
+version = "0.7.1"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 
 [dependencies]
 ahash = "0.8.3"
 bumpalo = "3.13.0"
```

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/README.md` & `zen_engine-0.8.1/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
                     name: self.iterator.str_value(token.value),
                     arguments: self.bump.alloc_slice_copy(&[arg]),
                 })
             }
             Arity::Dual => {
                 let arg1 = self.parse_expression(0)?;
                 self.iterator.expect(TokenKind::Operator, Some(&[","]))?;
-                let arg2 = self.parse_primary_expression()?;
+                let arg2 = self.parse_expression(0)?;
                 self.iterator.expect(TokenKind::Bracket, Some(&[")"]))?;
 
                 self.iterator.node(Node::BuiltIn {
                     name: self.iterator.str_value(token.value),
                     arguments: self.bump.alloc_slice_copy(&[arg1, arg2]),
                 })
             }
```

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/src/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -515,14 +515,35 @@
                 },
                 TestCase {
                     expr: r#"extract("foo.bar", "(\w+)\.(\w+)")"#,
                     result: json!(["foo.bar", "foo", "bar"]),
                 },
             ]),
         },
+        TestEnv {
+            env: json!({}),
+            cases: Vec::from([
+                TestCase {
+                    expr: r#"some(['a', 'b'], startsWith('a', #))"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"some(['a', 'b'], startsWith(#, 'a'))"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"some(['a', 'b'], startsWith('c', #))"#,
+                    result: json!(false),
+                },
+                TestCase {
+                    expr: r#"some(['a', 'b'], startsWith(#, 'c'))"#,
+                    result: json!(false),
+                },
+            ]),
+        },
     ]);
 
     let isolate = Isolate::default();
 
     for TestEnv { env, cases } in tests {
         isolate.inject_env(&env);
```

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/tests/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.8.1/local_dependencies/zen-expression/tests/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.8.1/local_dependencies/zen-engine/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Business rules engine"
 name = "zen-engine"
 license = "MIT"
-version = "0.7.0"
+version = "0.7.1"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 [lib]
 doctest = false
 
 [dependencies]
@@ -18,15 +18,15 @@
 bincode = { version = "2.0.0-rc.3", optional = true }
 serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
 serde = { version = "1.0.163", features = ["derive"] }
 serde_v8 = { version = "0.103.0" }
 once_cell = { version = "1.17.2" }
 futures = "0.3.28"
 v8 = { version = "0.74.0" }
-zen-expression = { path = "../zen-expression", version = "0.7.0" }
+zen-expression = { path = "../zen-expression", version = "0.7.1" }
 
 [features]
 bincode = ["dep:bincode"]
 
 [[bench]]
 harness = false
 name = "engine"
```

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/README.md` & `zen_engine-0.8.1/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/error.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.8.1/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/.gitignore` & `zen_engine-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/LICENSE` & `zen_engine-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/README.md` & `zen_engine-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/index.py` & `zen_engine-0.8.1/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/pyproject.toml` & `zen_engine-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/src/decision.rs` & `zen_engine-0.8.1/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/src/engine.rs` & `zen_engine-0.8.1/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/src/loader.rs` & `zen_engine-0.8.1/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/src/value.rs` & `zen_engine-0.8.1/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.0/Cargo.lock` & `zen_engine-0.8.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 name = "anstyle"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
@@ -92,26 +92,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -317,26 +317,26 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.12"
+version = "4.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eab9e8ceb9afdade1ab3f0fd8dbce5b1b2f468ad653baf10e771781b2b67b73"
+checksum = "5b0827b011f6f8ab38590295339817b0d26f344aa4932c3ced71b45b0c54b4a9"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.12"
+version = "4.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f2763db829349bf00cfc06251268865ed4363b93a943174f638daf3ecdba2cd"
+checksum = "9441b403be87be858db6a23edb493e7f694761acdc3343d5a0fcaafd304cbc9e"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -448,15 +448,15 @@
 [[package]]
 name = "ctor"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f34ba9a9bcb8645379e9de8cb3ecfcf4d1c85ba66d90deb3259206fa5aa193b"
 dependencies = [
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -572,15 +572,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -719,17 +719,17 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
@@ -979,15 +979,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
@@ -1048,17 +1048,17 @@
 checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
 dependencies = [
  "toml",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.64"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1149,17 +1149,17 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1347,79 +1347,79 @@
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.171"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
+checksum = "e91f70896d6720bc714a4a57d22fc91f1db634680e65c8efe13323f1fa38d53f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.11"
+version = "0.11.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a16be4fe5320ade08736447e3198294a5ea9a6d44dde6f35f0a5e06859c427a"
+checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.171"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
+checksum = "a6250dde8342e0232232be9ca3db7aa40aceb5a3e5dd9bddbc00d99a007cde49"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.102"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1474,34 +1474,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.25"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.9"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
 version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
@@ -1512,15 +1512,15 @@
 name = "thiserror-impl"
 version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1572,31 +1572,31 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
@@ -1604,17 +1604,17 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uuid"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
+checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
 
 [[package]]
 name = "v8"
 version = "0.74.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7568bf38565bd5b350d96abbf3d09417e8c9dd74fbb38860e91b759e46f9009c"
 dependencies = [
@@ -1675,15 +1675,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1697,15 +1697,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -1846,15 +1846,15 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zen-engine"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "anyhow",
  "async-recursion",
  "async-trait",
  "bincode",
  "criterion",
  "futures",
@@ -1866,15 +1866,15 @@
  "tokio",
  "v8",
  "zen-expression",
 ]
 
 [[package]]
 name = "zen-expression"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ahash 0.8.3",
  "bumpalo",
  "chrono",
  "criterion",
  "fastrand",
  "hashbrown 0.13.2",
@@ -1899,15 +1899,15 @@
  "napi-derive",
  "serde_json",
  "zen-engine",
 ]
 
 [[package]]
 name = "zen-python"
-version = "0.8.0"
+version = "0.8.1"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.8.0/PKG-INFO` & `zen_engine-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.8.0
+Version: 0.8.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

