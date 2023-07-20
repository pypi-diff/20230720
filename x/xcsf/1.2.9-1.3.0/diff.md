# Comparing `tmp/xcsf-1.2.9.tar.gz` & `tmp/xcsf-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsf-1.2.9.tar", last modified: Sun Jul  9 17:49:46 2023, max compression
+gzip compressed data, was "xcsf-1.3.0.tar", last modified: Thu Jul 20 10:56:30 2023, max compression
```

## Comparing `xcsf-1.2.9.tar` & `xcsf-1.3.0.tar`

### file list

```diff
@@ -1,698 +1,702 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7267 2023-07-09 17:44:19.000000 xcsf-1.2.9/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-05-01 09:22:08.000000 xcsf-1.2.9/LICENSE.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-05-01 09:22:08.000000 xcsf-1.2.9/MANIFEST.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 17:49:46.020662 xcsf-1.2.9/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-05-05 14:22:38.000000 xcsf-1.2.9/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.gitattributes
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/.github/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.github/CONTRIBUTING.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/.github/workflows/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3308 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.github/workflows/CI.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      599 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.github/workflows/ci-fuzz.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      171 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    24882 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CHANGELOG.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10330 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3903 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CONTRIBUTORS.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27632 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/appveyor.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    77959 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16193 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    40729 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON_Utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/cJSON_Utils.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/fuzzing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/CMakeLists.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl-prepare-linux.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/cjson_read_fuzzer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/fuzz_main.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.bu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/json.dict
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/ossfuzz.sh
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/library_config/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/cJSONConfig.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/libcjson.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/libcjson_utils.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/uninstall.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/cjson_add.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/compare_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test1.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test10.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test11.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test2.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test3.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test4.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test5.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test7.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test8.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test9.expected
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.npmignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/package.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/spec_tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json_patch_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/minify_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28328 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/tests/misc_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/misc_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/old_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_examples.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_hex4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_with_opts.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/readme_examples.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/auto/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_prompt.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_reporter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_config.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_module.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/parse_output.rb
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/test_file_filter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/type_sanitizer.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_to_junit.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/docs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/license.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/unity_config.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.988664 xcsf-1.2.9/lib/cJSON/tests/unity/extras/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/release/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/release/build.info
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/release/version.info
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity_internals.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/.rubocop.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile_helper.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_file.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_strict.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_32.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_64.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/CException.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/Defs.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/cmock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/mockMock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testparameterized.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testunity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity_setup.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/valgrind.supp
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.004663 xcsf-1.2.9/lib/dSFMT/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/Makefile.me
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/README.jp.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/README.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/check.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params11213.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params1279.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params132049.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params19937.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params216091.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params2203.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params4253.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params44497.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params521.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params86243.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-ref.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.11213.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.1279.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.132049.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.19937.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.216091.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.2203.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.4253.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.44497.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.521.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.86243.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/debug.log
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/doxygen.cfg.bak
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.004663 xcsf-1.2.9/lib/dSFMT/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_defs.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_type.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/howto-compile.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/struct_d_s_f_m_t___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/union_w128___t.html
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/dSFMT/jump/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/Makefile.me
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-old.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-jump
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-jump.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/check-jump.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-calc-jump.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMText.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/debug.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/debug.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree.xlsx
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg.bak
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.2203.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/factorization
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/factorization.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.86243.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/dSFMT/jump/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/bdwn.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacedsfmt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespaces.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/struct_f_i_x___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.132049.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.86243.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/memo.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/params.csv
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.86243.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/readme-jp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/readme.html
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample1.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample2.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M11213
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M1279
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M132049
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M19937
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M216091
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M2203
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M4253
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M44497
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M521
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M86243
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample3.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6491 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/all_features/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/all_features/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/dll/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/executable/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/mpi/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/examples/mpi/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/scripts/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/cmake/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/assemble_single_header.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8999 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/doctest.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/doctestAddTests.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/exec_test.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/how_stuff_works/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/playground/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/playground/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11983 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/pybind11/include/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23959 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7069 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    65660 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28518 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    52930 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17869 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26305 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    42613 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    31450 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18140 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      316 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13471 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5002 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8262 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    79416 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9103 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2734 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/options.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   126420 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    94641 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/stl/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15337 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    29747 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21675 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tests/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2639 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tools/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2350 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11190 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      817 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/JoinPaths.cmake
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/check-style.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1040 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/libsize.py
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1311 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/make_changelog.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      196 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14033 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8960 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8361 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/pyproject.toml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2104 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1234 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-09 17:49:46.020662 xcsf-1.2.9/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4736 2023-07-09 17:44:13.000000 xcsf-1.2.9/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:08.000000 xcsf-1.2.9/test/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4521 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/__init__.pyi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_integer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_integer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5610 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/action.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/action.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/blas.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/blas.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19312 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21808 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2292 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dummy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dummy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ellipsoid.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ellipsoid.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_rectangle.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_rectangle.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ternary.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ternary.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/condition.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/condition.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/config.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/config.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23543 2023-07-09 16:06:08.000000 xcsf-1.2.9/xcsf/dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16108 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/ea.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/ea.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_csv.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_csv.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_maze.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_maze.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_mux.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_mux.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18174 2023-07-09 16:06:08.000000 xcsf-1.2.9/xcsf/gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4443 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/image.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/image.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/loss.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/loss.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/main.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_activations.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_activations.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22350 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_args.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_args.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_avgpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_avgpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_connected.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_connected.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21064 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_convolutional.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_convolutional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_dropout.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_dropout.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_lstm.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_lstm.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_maxpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_maxpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_noise.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_noise.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_recurrent.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_recurrent.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_softmax.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_softmax.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_upsample.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_upsample.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5411 2023-05-01 09:36:46.000000 xcsf-1.2.9/xcsf/pa.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pa.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    25930 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3375 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/param.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/perf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/perf.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_constant.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_constant.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11945 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_nlms.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_nlms.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_rls.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_rls.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/prediction.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/prediction.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    52149 2023-07-09 14:13:14.000000 xcsf-1.2.9/xcsf/pybind_wrapper.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/sam.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/sam.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf/utils/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/types.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/viz.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3501 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8386 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_rl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_rl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7283 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_supervised.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1410 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_supervised.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6272 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcsf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6725 2023-07-09 17:44:06.000000 xcsf-1.2.9/xcsf/xcsf.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21616 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/not-zip-safe
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/top_level.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7267 2023-07-20 10:48:26.000000 xcsf-1.3.0/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-07-20 10:48:26.000000 xcsf-1.3.0/LICENSE.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-07-20 10:48:26.000000 xcsf-1.3.0/MANIFEST.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-20 10:56:30.940587 xcsf-1.3.0/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-07-20 10:48:26.000000 xcsf-1.3.0/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.gitattributes
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/.github/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/CONTRIBUTING.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/.github/workflows/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3308 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/workflows/CI.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      599 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/workflows/ci-fuzz.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      171 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    24882 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CHANGELOG.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10330 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3903 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CONTRIBUTORS.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27632 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/appveyor.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    77959 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16193 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    40729 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON_Utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON_Utils.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/fuzzing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/CMakeLists.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl-prepare-linux.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/cjson_read_fuzzer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/fuzz_main.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.bu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/json.dict
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/ossfuzz.sh
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/library_config/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/cJSONConfig.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/libcjson.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/libcjson_utils.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/uninstall.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/cjson_add.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/compare_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test1.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test10.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test11.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test2.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test3.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test4.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test5.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test7.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test8.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test9.expected
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.npmignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/package.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/spec_tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json_patch_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/minify_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28328 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/misc_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/misc_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/old_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_examples.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_hex4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_with_opts.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/readme_examples.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/auto/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_prompt.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_reporter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_config.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_module.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/parse_output.rb
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/test_file_filter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/type_sanitizer.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_to_junit.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/docs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/license.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/unity_config.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/release/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/release/build.info
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/release/version.info
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity_internals.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/.rubocop.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile_helper.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_file.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_strict.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_32.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_64.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/CException.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/Defs.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/cmock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/mockMock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testparameterized.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testunity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity_setup.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/valgrind.supp
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.924587 xcsf-1.3.0/lib/dSFMT/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/dSFMT/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/Makefile.me
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/README.jp.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/README.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/check.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params11213.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params1279.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params132049.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params19937.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params216091.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params2203.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params4253.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params44497.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params521.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params86243.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-ref.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.11213.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.1279.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.132049.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.19937.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.216091.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.2203.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.4253.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.44497.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.521.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.86243.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/debug.log
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/doxygen.cfg.bak
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.924587 xcsf-1.3.0/lib/dSFMT/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_defs.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_type.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/howto-compile.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/struct_d_s_f_m_t___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/union_w128___t.html
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/dSFMT/jump/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/Makefile.me
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-old.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-jump
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-jump.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/check-jump.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-calc-jump.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMText.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/debug.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/debug.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree.xlsx
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg.bak
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.2203.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/factorization
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/factorization.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.86243.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/dSFMT/jump/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/bdwn.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacedsfmt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespaces.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/struct_f_i_x___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.132049.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.86243.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/memo.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/params.csv
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.86243.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/readme-jp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/readme.html
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample1.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample2.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M11213
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M1279
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M132049
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M19937
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M216091
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M2203
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M4253
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M44497
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M521
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M86243
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample3.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6491 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/all_features/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/all_features/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/dll/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/executable/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/mpi/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/mpi/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/scripts/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/cmake/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/assemble_single_header.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8999 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/doctest.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/doctestAddTests.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/exec_test.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/how_stuff_works/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/playground/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/playground/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11983 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/pybind11/include/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23959 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7069 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    65660 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28518 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    52930 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26305 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    42613 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    31450 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      316 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13471 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5002 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8262 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    79416 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9103 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2734 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   126420 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    94641 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15337 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29747 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21675 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2639 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tools/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2350 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11190 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      817 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/JoinPaths.cmake
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/check-style.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1040 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/libsize.py
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1311 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      196 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14033 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8960 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8361 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2104 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1234 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-20 10:56:30.940587 xcsf-1.3.0/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4736 2023-07-20 10:48:26.000000 xcsf-1.3.0/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1432 2023-07-20 10:48:26.000000 xcsf-1.3.0/test/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4641 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/__init__.pyi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_integer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_integer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5611 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/action.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/action.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/blas.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/blas.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19335 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23374 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2361 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dummy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dummy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ellipsoid.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ellipsoid.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_rectangle.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_rectangle.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ternary.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ternary.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/condition.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/condition.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/config.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/config.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23543 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16108 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/ea.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/ea.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_csv.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_csv.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_maze.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_maze.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_mux.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_mux.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18174 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4443 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/image.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/image.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/loss.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/loss.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2211 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/main.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_activations.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_activations.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22350 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_args.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_args.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_avgpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_avgpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_connected.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_connected.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21064 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_convolutional.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_convolutional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_dropout.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_dropout.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_lstm.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_lstm.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_maxpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_maxpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_noise.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_noise.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_recurrent.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_recurrent.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_softmax.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_softmax.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_upsample.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_upsample.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pa.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pa.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28009 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3520 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/param.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/perf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/perf.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_constant.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_constant.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11945 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_nlms.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_nlms.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_rls.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_rls.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/prediction.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/prediction.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1113 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3955 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback_checkpoint.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5460 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback_earlystop.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1465 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_utils.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    38402 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_wrapper.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/sam.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/sam.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf/utils/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/types.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/viz.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4015 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8322 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_rl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_rl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7287 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_supervised.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1447 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_supervised.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6318 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcsf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6927 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcsf.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21726 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/not-zip-safe
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/top_level.txt
```

### Comparing `xcsf-1.2.9/CMakeLists.txt` & `xcsf-1.3.0/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 cmake_minimum_required(VERSION 3.12)
 
 project(XCSF CXX C)
 set(PROJECT_VENDOR "Richard Preen")
 set(PROJECT_CONTACT "rpreen@gmail.com")
 set(PROJECT_URL "https://github.com/rpreen/xcsf")
 set(PROJECT_DESCRIPTION "XCSF: Learning Classifier System")
-set(PROJECT_VERSION "1.2.9")
+set(PROJECT_VERSION "1.3.0")
 
 set(CMAKE_C_STANDARD 11)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_C_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_VERBOSE_MAKEFILE OFF)
```

### Comparing `xcsf-1.2.9/LICENSE.md` & `xcsf-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/PKG-INFO` & `xcsf-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.2.9
+Version: 1.3.0
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.2.9/README.md` & `xcsf-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/.github/CONTRIBUTING.md` & `xcsf-1.3.0/lib/cJSON/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/.github/workflows/CI.yml` & `xcsf-1.3.0/lib/cJSON/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/.github/workflows/ci-fuzz.yml` & `xcsf-1.3.0/lib/cJSON/.github/workflows/ci-fuzz.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/.travis.yml` & `xcsf-1.3.0/lib/cJSON/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/CHANGELOG.md` & `xcsf-1.3.0/lib/cJSON/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/CMakeLists.txt` & `xcsf-1.3.0/lib/cJSON/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/CONTRIBUTORS.md` & `xcsf-1.3.0/lib/cJSON/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/LICENSE` & `xcsf-1.3.0/lib/cJSON/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/Makefile` & `xcsf-1.3.0/lib/cJSON/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/README.md` & `xcsf-1.3.0/lib/cJSON/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/appveyor.yml` & `xcsf-1.3.0/lib/cJSON/appveyor.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/cJSON.c` & `xcsf-1.3.0/lib/cJSON/cJSON.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/cJSON.h` & `xcsf-1.3.0/lib/cJSON/cJSON.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/cJSON_Utils.c` & `xcsf-1.3.0/lib/cJSON/cJSON_Utils.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/cJSON_Utils.h` & `xcsf-1.3.0/lib/cJSON/cJSON_Utils.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/CMakeLists.txt` & `xcsf-1.3.0/lib/cJSON/fuzzing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/afl.c` & `xcsf-1.3.0/lib/cJSON/fuzzing/afl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/cjson_read_fuzzer.c` & `xcsf-1.3.0/lib/cJSON/fuzzing/cjson_read_fuzzer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/fuzz_main.c` & `xcsf-1.3.0/lib/cJSON/fuzzing/fuzz_main.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test1` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.bu` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.bu`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uf` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uf`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uu` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uu`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test4` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test5` & `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/json.dict` & `xcsf-1.3.0/lib/cJSON/fuzzing/json.dict`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/fuzzing/ossfuzz.sh` & `xcsf-1.3.0/lib/cJSON/fuzzing/ossfuzz.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/library_config/cJSONConfig.cmake.in` & `xcsf-1.3.0/lib/cJSON/library_config/cJSONConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/library_config/uninstall.cmake` & `xcsf-1.3.0/lib/cJSON/library_config/uninstall.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/test.c` & `xcsf-1.3.0/lib/cJSON/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/CMakeLists.txt` & `xcsf-1.3.0/lib/cJSON/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/cjson_add.c` & `xcsf-1.3.0/lib/cJSON/tests/cjson_add.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/common.h` & `xcsf-1.3.0/lib/cJSON/tests/common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/compare_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/compare_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test1` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test3` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test4` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test4.expected` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test4.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test5` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/inputs/test5.expected` & `xcsf-1.3.0/lib/cJSON/tests/inputs/test5.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/README.md` & `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json` & `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/spec_tests.json` & `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/spec_tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/tests.json` & `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/json_patch_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/json_patch_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/minify_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/minify_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/misc_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/misc_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/misc_utils_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/misc_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/old_utils_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/old_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_array.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_examples.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_hex4.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_hex4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_number.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_object.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_string.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_value.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/parse_with_opts.c` & `xcsf-1.3.0/lib/cJSON/tests/parse_with_opts.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/print_array.c` & `xcsf-1.3.0/lib/cJSON/tests/print_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/print_number.c` & `xcsf-1.3.0/lib/cJSON/tests/print_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/print_object.c` & `xcsf-1.3.0/lib/cJSON/tests/print_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/print_string.c` & `xcsf-1.3.0/lib/cJSON/tests/print_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/print_value.c` & `xcsf-1.3.0/lib/cJSON/tests/print_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/readme_examples.c` & `xcsf-1.3.0/lib/cJSON/tests/readme_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/.gitattributes` & `xcsf-1.3.0/lib/cJSON/tests/unity/.gitattributes`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/.travis.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/README.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_prompt.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_prompt.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_reporter.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_reporter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_config.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_config.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_module.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_module.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_test_runner.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/parse_output.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/parse_output.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/stylize_as_junit.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/stylize_as_junit.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/test_file_filter.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/test_file_filter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.py` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_to_junit.py` & `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_to_junit.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/docs/license.txt` & `xcsf-1.3.0/lib/cJSON/tests/unity/docs/license.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/makefile` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/makefile` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/readme.txt` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/examples/unity_config.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/examples/unity_config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/readme.txt` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/Makefile` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity_internals.h` & `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/.rubocop.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/Makefile` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_def.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_param.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile_helper.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_file.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_file.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_strict.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_strict.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_32.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_64.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_64.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_msp430.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_msp430.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testparameterized.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testparameterized.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testunity.c` & `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testunity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/CHANGE-LOG.txt` & `xcsf-1.3.0/lib/dSFMT/CHANGE-LOG.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/FILES.txt` & `xcsf-1.3.0/lib/dSFMT/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/LICENSE.txt` & `xcsf-1.3.0/lib/dSFMT/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/Makefile` & `xcsf-1.3.0/lib/dSFMT/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/Makefile.me` & `xcsf-1.3.0/lib/dSFMT/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/README.jp.txt` & `xcsf-1.3.0/lib/dSFMT/README.jp.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/README.txt` & `xcsf-1.3.0/lib/dSFMT/README.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-common.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params11213.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params11213.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params1279.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params1279.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params132049.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params132049.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params19937.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params216091.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params216091.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params2203.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params2203.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params4253.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params4253.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params44497.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params44497.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params521.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params521.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-params86243.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT-params86243.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-ref.c` & `xcsf-1.3.0/lib/dSFMT/dSFMT-ref.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.tar.gz` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.zip` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.tar.gz` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.zip` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.tar.gz` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.zip` & `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.11213.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.11213.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.1279.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.1279.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.132049.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.132049.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.19937.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.19937.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.216091.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.216091.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.2203.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.2203.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.4253.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.4253.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.44497.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.44497.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.521.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.521.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.86243.out.txt` & `xcsf-1.3.0/lib/dSFMT/dSFMT.86243.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.c` & `xcsf-1.3.0/lib/dSFMT/dSFMT.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/dSFMT.h` & `xcsf-1.3.0/lib/dSFMT/dSFMT.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/doxygen.cfg` & `xcsf-1.3.0/lib/dSFMT/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/doxygen.cfg.bak` & `xcsf-1.3.0/lib/dSFMT/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/annotated.html` & `xcsf-1.3.0/lib/dSFMT/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/bc_s.png` & `xcsf-1.3.0/lib/dSFMT/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/classes.html` & `xcsf-1.3.0/lib/dSFMT/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8c.html` & `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h.html` & `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h_source.html` & `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/doxygen.css` & `xcsf-1.3.0/lib/dSFMT/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/doxygen.png` & `xcsf-1.3.0/lib/dSFMT/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/files.html` & `xcsf-1.3.0/lib/dSFMT/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/functions.html` & `xcsf-1.3.0/lib/dSFMT/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/functions_vars.html` & `xcsf-1.3.0/lib/dSFMT/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/globals.html` & `xcsf-1.3.0/lib/dSFMT/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/globals_defs.html` & `xcsf-1.3.0/lib/dSFMT/html/globals_defs.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/globals_func.html` & `xcsf-1.3.0/lib/dSFMT/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/globals_type.html` & `xcsf-1.3.0/lib/dSFMT/html/globals_type.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/globals_vars.html` & `xcsf-1.3.0/lib/dSFMT/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/howto-compile.html` & `xcsf-1.3.0/lib/dSFMT/html/howto-compile.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/index.html` & `xcsf-1.3.0/lib/dSFMT/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/jquery.js` & `xcsf-1.3.0/lib/dSFMT/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/mainpage_8txt.html` & `xcsf-1.3.0/lib/dSFMT/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/struct_d_s_f_m_t___t.html` & `xcsf-1.3.0/lib/dSFMT/html/struct_d_s_f_m_t___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/tabs.css` & `xcsf-1.3.0/lib/dSFMT/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/html/union_w128___t.html` & `xcsf-1.3.0/lib/dSFMT/html/union_w128___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/FILES.txt` & `xcsf-1.3.0/lib/dSFMT/jump/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/LICENSE.txt` & `xcsf-1.3.0/lib/dSFMT/jump/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/Makefile` & `xcsf-1.3.0/lib/dSFMT/jump/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/Makefile.me` & `xcsf-1.3.0/lib/dSFMT/jump/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic` & `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi` & `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-old.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-old.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-jump` & `xcsf-1.3.0/lib/dSFMT/jump/calc-jump`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/calc-jump.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/calc-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-calc-jump.hpp` & `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-calc-jump.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.c` & `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.h` & `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/dSFMText.hpp` & `xcsf-1.3.0/lib/dSFMT/jump/dSFMText.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/debug.fix.11213.txt` & `xcsf-1.3.0/lib/dSFMT/jump/debug.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/debug.txt` & `xcsf-1.3.0/lib/dSFMT/jump/debug.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/degree` & `xcsf-1.3.0/lib/dSFMT/jump/degree`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/degree.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/degree.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/degree.xlsx` & `xcsf-1.3.0/lib/dSFMT/jump/degree.xlsx`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg` & `xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg.bak` & `xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.11213.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.132049.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.2203.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.132049.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.216091.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.2203.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/factorization` & `xcsf-1.3.0/lib/dSFMT/jump/factorization`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/factorization.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/factorization.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.11213.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.132049.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.19937.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.2203.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.44497.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/fix.86243.txt` & `xcsf-1.3.0/lib/dSFMT/jump/fix.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/annotated.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/bc_s.png` & `xcsf-1.3.0/lib/dSFMT/jump/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/classes.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.css` & `xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.png` & `xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/files.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/functions.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/functions_vars.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/globals.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/globals_func.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/globals_vars.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/index.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/jquery.js` & `xcsf-1.3.0/lib/dSFMT/jump/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/mainpage_8txt.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/namespacedsfmt.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/namespacedsfmt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers_func.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/namespaces.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/namespaces.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/struct_f_i_x___t.html` & `xcsf-1.3.0/lib/dSFMT/jump/html/struct_f_i_x___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/html/tabs.css` & `xcsf-1.3.0/lib/dSFMT/jump/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.1279.txt` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.1279.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.132049.tar.gz` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.132049.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.tar.gz` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.txt` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.4253.txt` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/lcm.86243.tar.gz` & `xcsf-1.3.0/lib/dSFMT/jump/lcm.86243.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/mainpage.txt` & `xcsf-1.3.0/lib/dSFMT/jump/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/params.csv` & `xcsf-1.3.0/lib/dSFMT/jump/params.csv`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.11213.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.132049.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.19937.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.216091.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.2203.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.4253.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.44497.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/poly.86243.txt` & `xcsf-1.3.0/lib/dSFMT/jump/poly.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/readme-jp.html` & `xcsf-1.3.0/lib/dSFMT/jump/readme-jp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/readme.html` & `xcsf-1.3.0/lib/dSFMT/jump/readme.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/sample1` & `xcsf-1.3.0/lib/dSFMT/jump/sample1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/sample1.c` & `xcsf-1.3.0/lib/dSFMT/jump/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/sample2` & `xcsf-1.3.0/lib/dSFMT/jump/sample2`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/sample2.c` & `xcsf-1.3.0/lib/dSFMT/jump/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M11213` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M11213`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M1279` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M1279`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M132049` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M132049`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M19937` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M19937`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M216091` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M216091`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M2203` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M2203`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M4253` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M4253`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M44497` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M44497`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M521` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M521`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M86243` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M86243`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/jump/test-jump.cpp` & `xcsf-1.3.0/lib/dSFMT/jump/test-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/mainpage.txt` & `xcsf-1.3.0/lib/dSFMT/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/sample1.c` & `xcsf-1.3.0/lib/dSFMT/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/sample2.c` & `xcsf-1.3.0/lib/dSFMT/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/sample3.c` & `xcsf-1.3.0/lib/dSFMT/sample3.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/sample4.c` & `xcsf-1.3.0/lib/dSFMT/sample4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/dSFMT/test.c` & `xcsf-1.3.0/lib/dSFMT/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/CMakeLists.txt` & `xcsf-1.3.0/lib/doctest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/examples/all_features/CMakeLists.txt` & `xcsf-1.3.0/lib/doctest/examples/all_features/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt` & `xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt` & `xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake` & `xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt` & `xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/scripts/cmake/assemble_single_header.cmake` & `xcsf-1.3.0/lib/doctest/scripts/cmake/assemble_single_header.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/scripts/cmake/common.cmake` & `xcsf-1.3.0/lib/doctest/scripts/cmake/common.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/scripts/cmake/doctest.cmake` & `xcsf-1.3.0/lib/doctest/scripts/cmake/doctest.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/scripts/cmake/doctestAddTests.cmake` & `xcsf-1.3.0/lib/doctest/scripts/cmake/doctestAddTests.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/doctest/scripts/cmake/exec_test.cmake` & `xcsf-1.3.0/lib/doctest/scripts/cmake/exec_test.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/attr.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/buffer_info.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/cast.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/chrono.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/complex.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/class.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/common.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/descr.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/init.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/internals.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/typeid.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/matrix.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/tensor.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/embed.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/eval.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/functional.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/gil.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/iostream.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/numpy.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/operators.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/options.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/pybind11.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/pytypes.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/stl/filesystem.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/stl.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/include/pybind11/stl_bind.h` & `xcsf-1.3.0/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tests/test_embed/CMakeLists.txt` & `xcsf-1.3.0/lib/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/FindCatch.cmake` & `xcsf-1.3.0/lib/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/FindEigen3.cmake` & `xcsf-1.3.0/lib/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/FindPythonLibsNew.cmake` & `xcsf-1.3.0/lib/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/JoinPaths.cmake` & `xcsf-1.3.0/lib/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/check-style.sh` & `xcsf-1.3.0/lib/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/cmake_uninstall.cmake.in` & `xcsf-1.3.0/lib/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/codespell_ignore_lines_from_errors.py` & `xcsf-1.3.0/lib/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/libsize.py` & `xcsf-1.3.0/lib/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/make_changelog.py` & `xcsf-1.3.0/lib/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/pybind11Common.cmake` & `xcsf-1.3.0/lib/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/pybind11Config.cmake.in` & `xcsf-1.3.0/lib/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/pybind11NewTools.cmake` & `xcsf-1.3.0/lib/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/pybind11Tools.cmake` & `xcsf-1.3.0/lib/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/setup_global.py.in` & `xcsf-1.3.0/lib/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/lib/pybind11/tools/setup_main.py.in` & `xcsf-1.3.0/lib/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/setup.py` & `xcsf-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="xcsf",
-    version="1.2.9",
+    version="1.3.0",
     license="GPL-3.0",
     maintainer="Richard Preen",
     maintainer_email="rpreen@gmail.com",
     description="XCSF learning classifier system: rule-based evolutionary machine learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rpreen/xcsf",
```

### Comparing `xcsf-1.2.9/test/CMakeLists.txt` & `xcsf-1.3.0/test/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2020--2022 Richard Preen <rpreen@gmail.com>
+# Copyright (C) 2020--2023 Richard Preen <rpreen@gmail.com>
 #
 # Copyright (C) 2021 David Pätzel
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -14,27 +14,29 @@
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 set(XCSF_TESTS
+    clset_test.cpp
     cond_ellipsoid_test.cpp
     cond_rectangle_test.cpp
     cond_ternary_test.cpp
     loss_test.cpp
     neural_layer_connected_test.cpp
     neural_layer_convolutional_test.cpp
     neural_layer_lstm_test.cpp
     neural_layer_maxpool_test.cpp
     neural_layer_recurrent_test.cpp
     neural_test.cpp
     pa_test.cpp
     pred_nlms_test.cpp
     pred_rls_test.cpp
+    serialization_test.cpp
     util_test.cpp
     unit_tests.cpp)
 
 add_definitions(-DDSFMT_MEXP=19937)
 
 add_executable(tests ${XCSF_TESTS})
 target_link_libraries(tests xcs)
```

### Comparing `xcsf-1.2.9/xcsf/CMakeLists.txt` & `xcsf-1.3.0/xcsf/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -158,15 +158,20 @@
 endif()
 
 # ##############################################################################
 # target: xcsf.so / pyd - Python library
 # ##############################################################################
 
 if(XCSF_PYLIB)
-  set(XCSF_PY_SOURCES pybind_wrapper.cpp)
+  set(XCSF_PY_SOURCES
+      pybind_wrapper.cpp
+      pybind_utils.h
+      pybind_callback.h
+      pybind_callback_checkpoint.h
+      pybind_callback_earlystop.h)
   pybind11_add_module(xcsf ${XCSF_PY_SOURCES})
   if(PARALLEL AND OpenMP_FOUND)
     target_link_libraries(xcsf PUBLIC OpenMP::OpenMP_CXX)
   endif()
   if(WIN32) # https://cython.readthedocs.io/en/latest/src/tutorial/appendix.html
     target_link_libraries(
       xcsf
```

### Comparing `xcsf-1.2.9/xcsf/__init__.pyi` & `xcsf-1.3.0/xcsf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/act_integer.c` & `xcsf-1.3.0/xcsf/act_integer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/act_integer.h` & `xcsf-1.3.0/xcsf/act_integer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/act_neural.c` & `xcsf-1.3.0/xcsf/act_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/act_neural.h` & `xcsf-1.3.0/xcsf/act_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/action.c` & `xcsf-1.3.0/xcsf/action.c`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 /**
  * @brief Initialises default action parameters.
  * @param [in] xcsf The XCSF data structure.
  */
 void
 action_param_defaults(struct XCSF *xcsf)
 {
-    action_param_set_type(xcsf, ACT_TYPE_NEURAL);
+    action_param_set_type(xcsf, ACT_TYPE_INTEGER);
     act_neural_param_defaults(xcsf);
 }
 
 /**
  * @brief Returns a json formatted string of the action parameters.
  * @param [in] xcsf XCSF data structure.
  * @return String encoded in json format.
```

### Comparing `xcsf-1.2.9/xcsf/action.h` & `xcsf-1.3.0/xcsf/action.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/blas.c` & `xcsf-1.3.0/xcsf/blas.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/blas.h` & `xcsf-1.3.0/xcsf/blas.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cl.c` & `xcsf-1.3.0/xcsf/cl.c`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
     char *json_str = NULL;
     if (return_cond) {
         json_str = cond_json_export(xcsf, c);
         cJSON *condition = cJSON_Parse(json_str);
         cJSON_AddItemToObject(json, "condition", condition);
         free(json_str);
     }
-    if (return_act) {
+    if (return_act && xcsf->n_actions > 1) {
         json_str = act_json_export(xcsf, c);
         cJSON *action = cJSON_Parse(json_str);
         cJSON_AddItemToObject(json, "action", action);
         free(json_str);
     }
     if (return_pred) {
         json_str = pred_json_export(xcsf, c);
```

### Comparing `xcsf-1.2.9/xcsf/cl.h` & `xcsf-1.3.0/xcsf/cl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/clset.c` & `xcsf-1.3.0/xcsf/clset.c`

 * *Files 3% similar despite different names*

```diff
@@ -273,21 +273,47 @@
     while (iter != NULL) {
         sum += iter->cl->time * iter->cl->num;
         iter = iter->next;
     }
     return sum;
 }
 
+void
+clset_load_pop_file(struct XCSF *xcsf)
+{
+    FILE *f = fopen(xcsf->population_file, "rt");
+    if (f == NULL) {
+        printf("Error opening JSON file: %s\n", xcsf->population_file);
+        exit(EXIT_FAILURE);
+    }
+    fseek(f, 0, SEEK_END);
+    const long len = 1 + ftell(f);
+    fseek(f, 0, SEEK_SET);
+    char *json_buffer = malloc(sizeof(char) * len);
+    const size_t s = fread(json_buffer, sizeof(char), len - 1, f);
+    fclose(f);
+    json_buffer[len - 1] = '\0';
+    if (s == 0) {
+        printf("Error opening JSON file: %s\n", xcsf->population_file);
+        exit(EXIT_FAILURE);
+    }
+    clset_json_insert(xcsf, json_buffer);
+    free(json_buffer);
+}
+
 /**
  * @brief Initialises a new population of random classifiers.
  * @param [in] xcsf The XCSF data structure.
  */
 void
 clset_pset_init(struct XCSF *xcsf)
 {
+    if (strncmp(xcsf->population_file, "\0", 1) != 0) {
+        clset_load_pop_file(xcsf);
+    }
     if (xcsf->POP_INIT) {
         while (xcsf->pset.num < xcsf->POP_SIZE) {
             struct Cl *new = malloc(sizeof(struct Cl));
             cl_init(xcsf, new, xcsf->POP_SIZE, 0);
             cl_rand(xcsf, new);
             clset_add(&xcsf->pset, new);
         }
@@ -724,17 +750,41 @@
     cJSON_Delete(json);
     return string;
 }
 
 /**
  * @brief Creates a classifier from cJSON and inserts in the population set.
  * @param [in,out] xcsf The XCSF data structure.
- * @param [in] json cJSON object.
+ * @param [in] json cJSON representing a classifier.
  */
 void
-clset_json_insert(struct XCSF *xcsf, const cJSON *json)
+clset_json_insert_cl(struct XCSF *xcsf, const cJSON *json)
 {
     struct Cl *new = malloc(sizeof(struct Cl));
     cl_json_import(xcsf, new, json);
     clset_add(&xcsf->pset, new);
     clset_pset_enforce_limit(xcsf);
 }
+
+/**
+ * @brief Creates classifiers from JSON and inserts into the population.
+ * @param [in,out] xcsf The XCSF data structure.
+ * @param [in] json_str JSON formatted string representing classifiers.
+ */
+void
+clset_json_insert(struct XCSF *xcsf, const char *json_str)
+{
+    cJSON *json = cJSON_Parse(json_str);
+    utils_json_parse_check(json);
+    if (json->child != NULL && cJSON_IsArray(json->child)) {
+        cJSON *tail = json->child->child; // insert inverted for consistency
+        tail->prev = NULL; // this should have been set by cJSON!
+        while (tail->next != NULL) {
+            tail = tail->next;
+        }
+        while (tail != NULL) {
+            clset_json_insert_cl(xcsf, tail);
+            tail = tail->prev;
+        }
+    }
+    cJSON_Delete(json);
+}
```

### Comparing `xcsf-1.2.9/xcsf/clset.h` & `xcsf-1.3.0/xcsf/clset.h`

 * *Files 5% similar despite different names*

```diff
@@ -86,8 +86,11 @@
 
 char *
 clset_json_export(const struct XCSF *xcsf, const struct Set *set,
                   const bool return_cond, const bool return_act,
                   const bool return_pred);
 
 void
-clset_json_insert(struct XCSF *xcsf, const cJSON *json);
+clset_json_insert_cl(struct XCSF *xcsf, const cJSON *json);
+
+void
+clset_json_insert(struct XCSF *xcsf, const char *json_str);
```

### Comparing `xcsf-1.2.9/xcsf/clset_neural.c` & `xcsf-1.3.0/xcsf/clset_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/clset_neural.h` & `xcsf-1.3.0/xcsf/clset_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_dgp.c` & `xcsf-1.3.0/xcsf/cond_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_dgp.h` & `xcsf-1.3.0/xcsf/cond_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_dummy.c` & `xcsf-1.3.0/xcsf/cond_dummy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_dummy.h` & `xcsf-1.3.0/xcsf/cond_dummy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_ellipsoid.c` & `xcsf-1.3.0/xcsf/cond_ellipsoid.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_ellipsoid.h` & `xcsf-1.3.0/xcsf/cond_ellipsoid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_gp.c` & `xcsf-1.3.0/xcsf/cond_gp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_gp.h` & `xcsf-1.3.0/xcsf/cond_gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_neural.c` & `xcsf-1.3.0/xcsf/cond_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_neural.h` & `xcsf-1.3.0/xcsf/cond_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_rectangle.c` & `xcsf-1.3.0/xcsf/cond_rectangle.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_rectangle.h` & `xcsf-1.3.0/xcsf/cond_rectangle.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_ternary.c` & `xcsf-1.3.0/xcsf/cond_ternary.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/cond_ternary.h` & `xcsf-1.3.0/xcsf/cond_ternary.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/condition.c` & `xcsf-1.3.0/xcsf/condition.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/condition.h` & `xcsf-1.3.0/xcsf/condition.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/config.c` & `xcsf-1.3.0/xcsf/config.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/config.h` & `xcsf-1.3.0/xcsf/config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/dgp.c` & `xcsf-1.3.0/xcsf/dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/dgp.h` & `xcsf-1.3.0/xcsf/dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/ea.c` & `xcsf-1.3.0/xcsf/ea.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/ea.h` & `xcsf-1.3.0/xcsf/ea.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env.c` & `xcsf-1.3.0/xcsf/env.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env.h` & `xcsf-1.3.0/xcsf/env.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_csv.c` & `xcsf-1.3.0/xcsf/env_csv.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_csv.h` & `xcsf-1.3.0/xcsf/env_csv.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_maze.c` & `xcsf-1.3.0/xcsf/env_maze.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_maze.h` & `xcsf-1.3.0/xcsf/env_maze.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_mux.c` & `xcsf-1.3.0/xcsf/env_mux.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/env_mux.h` & `xcsf-1.3.0/xcsf/env_mux.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/gp.c` & `xcsf-1.3.0/xcsf/gp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/gp.h` & `xcsf-1.3.0/xcsf/gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/image.c` & `xcsf-1.3.0/xcsf/image.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/image.h` & `xcsf-1.3.0/xcsf/image.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/loss.c` & `xcsf-1.3.0/xcsf/loss.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/loss.h` & `xcsf-1.3.0/xcsf/loss.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/main.c` & `xcsf-1.3.0/xcsf/main.c`

 * *Files 3% similar despite different names*

```diff
@@ -36,33 +36,32 @@
 {
     if (argc < 3 || argc > 5) {
         printf("Usage: xcsf problemType{csv|mp|maze} ");
         printf("problem{.csv|size|maze} [config.json] [xcs.bin]\n");
         exit(EXIT_FAILURE);
     }
     struct XCSF *xcsf = malloc(sizeof(struct XCSF));
-    rand_init();
     env_init(xcsf, argv); // initialise environment and default parameters
     if (argc > 3) { // load parameter config
         config_read(xcsf, argv[3]);
     } else {
         config_read(xcsf, "default.json");
     }
     xcsf_init(xcsf); // initialise XCSF
     if (argc == 5) { // reload state of a previous experiment
         const size_t s = xcsf_load(xcsf, argv[4]);
         printf("XCSF loaded: %d elements\n", (int) s);
     }
     param_print(xcsf); // print parameters used
     if (strcmp(argv[1], "csv") == 0) { // supervised regression - csv file
         const struct EnvCSV *env = xcsf->env;
-        xcs_supervised_fit(xcsf, env->train_data, env->test_data, true);
+        xcs_supervised_fit(xcsf, env->train_data, env->test_data, true,
+                           xcsf->MAX_TRIALS);
     } else { // reinforcement learning - maze or mux
         xcs_rl_exp(xcsf);
     }
-    pa_free(xcsf); // clean up
-    env_free(xcsf);
+    env_free(xcsf); // clean up
     xcsf_free(xcsf);
     param_free(xcsf);
     free(xcsf);
     return EXIT_SUCCESS;
 }
```

### Comparing `xcsf-1.2.9/xcsf/neural.c` & `xcsf-1.3.0/xcsf/neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural.h` & `xcsf-1.3.0/xcsf/neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_activations.c` & `xcsf-1.3.0/xcsf/neural_activations.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_activations.h` & `xcsf-1.3.0/xcsf/neural_activations.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer.c` & `xcsf-1.3.0/xcsf/neural_layer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer.h` & `xcsf-1.3.0/xcsf/neural_layer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_args.c` & `xcsf-1.3.0/xcsf/neural_layer_args.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_args.h` & `xcsf-1.3.0/xcsf/neural_layer_args.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_avgpool.c` & `xcsf-1.3.0/xcsf/neural_layer_avgpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_avgpool.h` & `xcsf-1.3.0/xcsf/neural_layer_avgpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_connected.c` & `xcsf-1.3.0/xcsf/neural_layer_connected.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_connected.h` & `xcsf-1.3.0/xcsf/neural_layer_connected.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_convolutional.c` & `xcsf-1.3.0/xcsf/neural_layer_convolutional.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_convolutional.h` & `xcsf-1.3.0/xcsf/neural_layer_convolutional.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_dropout.c` & `xcsf-1.3.0/xcsf/neural_layer_dropout.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_dropout.h` & `xcsf-1.3.0/xcsf/neural_layer_dropout.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_lstm.c` & `xcsf-1.3.0/xcsf/neural_layer_lstm.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_lstm.h` & `xcsf-1.3.0/xcsf/neural_layer_lstm.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_maxpool.c` & `xcsf-1.3.0/xcsf/neural_layer_maxpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_maxpool.h` & `xcsf-1.3.0/xcsf/neural_layer_maxpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_noise.c` & `xcsf-1.3.0/xcsf/neural_layer_noise.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_noise.h` & `xcsf-1.3.0/xcsf/neural_layer_noise.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_recurrent.c` & `xcsf-1.3.0/xcsf/neural_layer_recurrent.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_recurrent.h` & `xcsf-1.3.0/xcsf/neural_layer_recurrent.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_softmax.c` & `xcsf-1.3.0/xcsf/neural_layer_softmax.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_softmax.h` & `xcsf-1.3.0/xcsf/neural_layer_softmax.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_upsample.c` & `xcsf-1.3.0/xcsf/neural_layer_upsample.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/neural_layer_upsample.h` & `xcsf-1.3.0/xcsf/neural_layer_upsample.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pa.c` & `xcsf-1.3.0/xcsf/pa.c`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
  */
 void
 pa_init(struct XCSF *xcsf)
 {
     xcsf->pa_size = xcsf->n_actions * xcsf->y_dim;
     xcsf->pa = malloc(sizeof(double) * xcsf->pa_size);
     xcsf->nr = malloc(sizeof(double) * xcsf->pa_size);
+    xcsf->cover = calloc(xcsf->pa_size, sizeof(double));
 }
 
 /**
  * @brief Builds the prediction array for the specified input.
  * @details Calculates the match set mean fitness weighted prediction for each
  * action. For supervised learning n_actions=1; reinforcement learning y_dim=1.
  * @param [in] xcsf The XCSF data structure.
@@ -186,8 +187,9 @@
  * @param [in] xcsf The XCSF data structure.
  */
 void
 pa_free(const struct XCSF *xcsf)
 {
     free(xcsf->pa);
     free(xcsf->nr);
+    free(xcsf->cover);
 }
```

### Comparing `xcsf-1.2.9/xcsf/pa.h` & `xcsf-1.3.0/xcsf/pa.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/param.c` & `xcsf-1.3.0/xcsf/param.c`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,31 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file param.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2015--2022.
+ * @date 2015--2023.
  * @brief Functions for setting and printing parameters.
  */
 
 #include "param.h"
 #include "action.h"
 #include "condition.h"
 #include "ea.h"
 #include "prediction.h"
 #include "utils.h"
 
 #ifdef PARALLEL
     #include <omp.h>
 #endif
 
+#define MAX_LEN 512 //!< Maximum length of a population filename
+
 /**
  * @brief Initialises default XCSF parameters.
  * @param [in] xcsf The XCSF data structure.
  * @param [in] x_dim The dimensionality of the input variables.
  * @param [in] y_dim The dimensionality of the prediction variables.
  * @param [in] n_actions The total number of possible actions.
  */
@@ -48,18 +50,21 @@
     xcsf->mset_size = 0;
     xcsf->aset_size = 0;
     xcsf->mfrac = 0;
     xcsf->ea = malloc(sizeof(struct ArgsEA));
     xcsf->act = malloc(sizeof(struct ArgsAct));
     xcsf->cond = malloc(sizeof(struct ArgsCond));
     xcsf->pred = malloc(sizeof(struct ArgsPred));
+    xcsf->population_file = malloc(sizeof(char));
+    xcsf->population_file[0] = '\0';
     param_set_n_actions(xcsf, n_actions);
     param_set_x_dim(xcsf, x_dim);
     param_set_y_dim(xcsf, y_dim);
     param_set_omp_num_threads(xcsf, 8);
+    param_set_random_state(xcsf, 0);
     param_set_pop_init(xcsf, true);
     param_set_max_trials(xcsf, 100000);
     param_set_perf_trials(xcsf, 1000);
     param_set_pop_size(xcsf, 2000);
     param_set_loss_func(xcsf, LOSS_MAE);
     param_set_huber_delta(xcsf, 1);
     param_set_e0(xcsf, 0.01);
@@ -83,14 +88,17 @@
     cond_param_defaults(xcsf);
     pred_param_defaults(xcsf);
 }
 
 void
 param_free(struct XCSF *xcsf)
 {
+    if (xcsf->population_file != NULL) {
+        free(xcsf->population_file);
+    }
     action_param_free(xcsf);
     cond_param_free(xcsf);
     pred_param_free(xcsf);
     free(xcsf->ea);
     free(xcsf->act);
     free(xcsf->cond);
     free(xcsf->pred);
@@ -108,14 +116,18 @@
     snprintf(v, 256, "%d.%d.%d", VERSION_MAJOR, VERSION_MINOR, VERSION_BUILD);
     cJSON *json = cJSON_CreateObject();
     cJSON_AddStringToObject(json, "version", v);
     cJSON_AddNumberToObject(json, "x_dim", xcsf->x_dim);
     cJSON_AddNumberToObject(json, "y_dim", xcsf->y_dim);
     cJSON_AddNumberToObject(json, "n_actions", xcsf->n_actions);
     cJSON_AddNumberToObject(json, "omp_num_threads", xcsf->OMP_NUM_THREADS);
+    cJSON_AddNumberToObject(json, "random_state", xcsf->RANDOM_STATE);
+    if (xcsf->population_file != NULL) {
+        cJSON_AddStringToObject(json, "population_file", xcsf->population_file);
+    }
     cJSON_AddBoolToObject(json, "pop_init", xcsf->POP_INIT);
     cJSON_AddNumberToObject(json, "max_trials", xcsf->MAX_TRIALS);
     cJSON_AddNumberToObject(json, "perf_trials", xcsf->PERF_TRIALS);
     cJSON_AddNumberToObject(json, "pop_size", xcsf->POP_SIZE);
     cJSON_AddStringToObject(json, "loss_func",
                             loss_type_as_string(xcsf->LOSS_FUNC));
     if (xcsf->LOSS_FUNC == LOSS_HUBER) {
@@ -176,26 +188,38 @@
  * @param [in,out] xcsf The XCSF data structure.
  * @param [in] json cJSON object.
  * @return Whether a parameter was found.
  */
 static bool
 param_json_import_general(struct XCSF *xcsf, const cJSON *json)
 {
-    if (strncmp(json->string, "version\0", 8) == 0 ||
-        strncmp(json->string, "x_dim\0", 6) == 0 ||
-        strncmp(json->string, "y_dim\0", 6) == 0 ||
-        strncmp(json->string, "n_actions\0", 10) == 0) {
-        return true; // set internally
+    if (strncmp(json->string, "version\0", 8) == 0) {
+        return true;
+    } else if (strncmp(json->string, "x_dim\0", 6) == 0 &&
+               cJSON_IsNumber(json)) {
+        catch_error(param_set_x_dim(xcsf, json->valueint));
+    } else if (strncmp(json->string, "y_dim\0", 6) == 0 &&
+               cJSON_IsNumber(json)) {
+        catch_error(param_set_y_dim(xcsf, json->valueint));
+    } else if (strncmp(json->string, "n_actions\0", 10) == 0 &&
+               cJSON_IsNumber(json)) {
+        catch_error(param_set_n_actions(xcsf, json->valueint));
     } else if (strncmp(json->string, "omp_num_threads\0", 16) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_omp_num_threads(xcsf, json->valueint));
+    } else if (strncmp(json->string, "random_state\0", 13) == 0 &&
+               cJSON_IsNumber(json)) {
+        catch_error(param_set_random_state(xcsf, json->valueint));
+    } else if (strncmp(json->string, "population_file\0", 16) == 0 &&
+               cJSON_IsString(json)) {
+        catch_error(param_set_population_file(xcsf, json->valuestring));
     } else if (strncmp(json->string, "pop_size\0", 9) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_pop_size(xcsf, json->valueint));
-    } else if (strncmp(json->string, "max_trials\0", 10) == 0 &&
+    } else if (strncmp(json->string, "max_trials\0", 11) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_max_trials(xcsf, json->valueint));
     } else if (strncmp(json->string, "pop_init\0", 9) == 0 &&
                cJSON_IsBool(json)) {
         catch_error(param_set_pop_init(xcsf, json->valueint));
     } else if (strncmp(json->string, "perf_trials\0", 12) == 0 &&
                cJSON_IsNumber(json)) {
@@ -448,24 +472,28 @@
  * @param [in] fp Pointer to the output file.
  * @return The total number of elements written.
  */
 size_t
 param_save(const struct XCSF *xcsf, FILE *fp)
 {
     size_t s = 0;
+    size_t len = sizeof(xcsf->population_file);
+    s += fwrite(&len, sizeof(size_t), 1, fp);
+    s += fwrite(xcsf->population_file, len, 1, fp);
     s += fwrite(&xcsf->time, sizeof(int), 1, fp);
     s += fwrite(&xcsf->error, sizeof(double), 1, fp);
     s += fwrite(&xcsf->mset_size, sizeof(double), 1, fp);
     s += fwrite(&xcsf->aset_size, sizeof(double), 1, fp);
     s += fwrite(&xcsf->mfrac, sizeof(double), 1, fp);
     s += fwrite(&xcsf->explore, sizeof(bool), 1, fp);
     s += fwrite(&xcsf->x_dim, sizeof(int), 1, fp);
     s += fwrite(&xcsf->y_dim, sizeof(int), 1, fp);
     s += fwrite(&xcsf->n_actions, sizeof(int), 1, fp);
     s += fwrite(&xcsf->OMP_NUM_THREADS, sizeof(int), 1, fp);
+    s += fwrite(&xcsf->RANDOM_STATE, sizeof(int), 1, fp);
     s += fwrite(&xcsf->POP_INIT, sizeof(bool), 1, fp);
     s += fwrite(&xcsf->MAX_TRIALS, sizeof(int), 1, fp);
     s += fwrite(&xcsf->PERF_TRIALS, sizeof(int), 1, fp);
     s += fwrite(&xcsf->POP_SIZE, sizeof(int), 1, fp);
     s += fwrite(&xcsf->LOSS_FUNC, sizeof(int), 1, fp);
     s += fwrite(&xcsf->HUBER_DELTA, sizeof(double), 1, fp);
     s += fwrite(&xcsf->GAMMA, sizeof(double), 1, fp);
@@ -497,28 +525,34 @@
  * @param [in] fp Pointer to the input file.
  * @return The total number of elements read.
  */
 size_t
 param_load(struct XCSF *xcsf, FILE *fp)
 {
     size_t s = 0;
+    size_t len = 0;
+    s += fread(&len, sizeof(size_t), 1, fp);
+    free(xcsf->population_file);
+    xcsf->population_file = malloc(len);
+    s += fread(xcsf->population_file, len, 1, fp);
     s += fread(&xcsf->time, sizeof(int), 1, fp);
     s += fread(&xcsf->error, sizeof(double), 1, fp);
     s += fread(&xcsf->mset_size, sizeof(double), 1, fp);
     s += fread(&xcsf->aset_size, sizeof(double), 1, fp);
     s += fread(&xcsf->mfrac, sizeof(double), 1, fp);
     s += fread(&xcsf->explore, sizeof(bool), 1, fp);
     s += fread(&xcsf->x_dim, sizeof(int), 1, fp);
     s += fread(&xcsf->y_dim, sizeof(int), 1, fp);
     s += fread(&xcsf->n_actions, sizeof(int), 1, fp);
     if (xcsf->x_dim < 1 || xcsf->y_dim < 1 || xcsf->n_actions < 1) {
         printf("param_load(): read error\n");
         exit(EXIT_FAILURE);
     }
     s += fread(&xcsf->OMP_NUM_THREADS, sizeof(int), 1, fp);
+    s += fread(&xcsf->RANDOM_STATE, sizeof(int), 1, fp);
     s += fread(&xcsf->POP_INIT, sizeof(bool), 1, fp);
     s += fread(&xcsf->MAX_TRIALS, sizeof(int), 1, fp);
     s += fread(&xcsf->PERF_TRIALS, sizeof(int), 1, fp);
     s += fread(&xcsf->POP_SIZE, sizeof(int), 1, fp);
     s += fread(&xcsf->LOSS_FUNC, sizeof(int), 1, fp);
     s += fread(&xcsf->HUBER_DELTA, sizeof(double), 1, fp);
     s += fread(&xcsf->GAMMA, sizeof(double), 1, fp);
@@ -563,14 +597,36 @@
 #ifdef PARALLEL
     omp_set_num_threads(xcsf->OMP_NUM_THREADS);
 #endif
     return NULL;
 }
 
 const char *
+param_set_random_state(struct XCSF *xcsf, const int a)
+{
+    xcsf->RANDOM_STATE = a;
+    if (a > 0) {
+        rand_init_seed(a);
+    } else {
+        rand_init();
+    }
+    return NULL;
+}
+
+const char *
+param_set_population_file(struct XCSF *xcsf, const char *a)
+{
+    free(xcsf->population_file);
+    size_t length = strnlen(a, sizeof(char) * MAX_LEN) + 1;
+    xcsf->population_file = malloc(sizeof(char) * length);
+    strncpy(xcsf->population_file, a, length);
+    return NULL;
+}
+
+const char *
 param_set_pop_init(struct XCSF *xcsf, const bool a)
 {
     xcsf->POP_INIT = a;
     return NULL;
 }
 
 const char *
```

### Comparing `xcsf-1.2.9/xcsf/param.h` & `xcsf-1.3.0/xcsf/param.h`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
 /* setters */
 
 const char *
 param_set_omp_num_threads(struct XCSF *xcsf, const int a);
 
 const char *
+param_set_random_state(struct XCSF *xcsf, const int a);
+
+const char *
+param_set_population_file(struct XCSF *xcsf, const char *a);
+
+const char *
 param_set_pop_init(struct XCSF *xcsf, const bool a);
 
 const char *
 param_set_max_trials(struct XCSF *xcsf, const int a);
 
 const char *
 param_set_perf_trials(struct XCSF *xcsf, const int a);
```

### Comparing `xcsf-1.2.9/xcsf/perf.c` & `xcsf-1.3.0/xcsf/perf.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/perf.h` & `xcsf-1.3.0/xcsf/perf.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_constant.c` & `xcsf-1.3.0/xcsf/pred_constant.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_constant.h` & `xcsf-1.3.0/xcsf/pred_constant.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_neural.c` & `xcsf-1.3.0/xcsf/pred_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_neural.h` & `xcsf-1.3.0/xcsf/pred_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_nlms.c` & `xcsf-1.3.0/xcsf/pred_nlms.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_nlms.h` & `xcsf-1.3.0/xcsf/pred_nlms.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_rls.c` & `xcsf-1.3.0/xcsf/pred_rls.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pred_rls.h` & `xcsf-1.3.0/xcsf/pred_rls.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/prediction.c` & `xcsf-1.3.0/xcsf/prediction.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/prediction.h` & `xcsf-1.3.0/xcsf/prediction.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/pybind_wrapper.cpp` & `xcsf-1.3.0/xcsf/pybind_wrapper.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -22,16 +22,18 @@
  * @brief Python library wrapper functions.
  */
 
 #ifdef _WIN32 // Try to work around https://bugs.python.org/issue11566
     #define _hypot hypot
 #endif
 
+#include <chrono>
 #include <cstdio>
 #include <fstream>
+#include <iomanip>
 #include <iostream>
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <sstream>
 #include <string>
 #include <vector>
@@ -47,86 +49,87 @@
 #include "param.h"
 #include "prediction.h"
 #include "utils.h"
 #include "xcs_rl.h"
 #include "xcs_supervised.h"
 }
 
+#include "pybind_callback.h"
+#include "pybind_callback_checkpoint.h"
+#include "pybind_callback_earlystop.h"
+#include "pybind_utils.h"
+
 /**
  * @brief Python XCSF class data structure.
  */
 class XCS
 {
   private:
     struct XCSF xcs; //!< XCSF data structure
     double *state; //!< Current input state for RL
     int action; //!< Current action for RL
     double payoff; //!< Current reward for RL
     struct Input *train_data; //!< Training data for supervised learning
     struct Input *test_data; //!< Test data for supervised learning
+    struct Input *val_data; //!< Validation data
+    py::dict params; //!< Dictionary of parameters and their values
+    py::list metric_train;
+    py::list metric_val;
+    py::list metric_trial;
+    py::list metric_psize;
+    py::list metric_msize;
+    py::list metric_mfrac;
+    int metric_counter;
 
   public:
     /**
+     * @brief Default Constructor.
+     */
+    XCS()
+    {
+        reset();
+        xcsf_init(&xcs);
+    }
+
+    /**
      * @brief Constructor.
-     * @param [in] x_dim The dimensionality of the input variables.
-     * @param [in] y_dim The dimensionality of the prediction variables.
-     * @param [in] n_actions The total number of possible actions.
-     */
-    XCS(const int x_dim, const int y_dim, const int n_actions)
-    {
-        param_init(&xcs, x_dim, y_dim, n_actions);
-        catch_error(param_set_n_actions(&xcs, n_actions));
-        catch_error(param_set_x_dim(&xcs, x_dim));
-        catch_error(param_set_y_dim(&xcs, y_dim));
+     * @param [in] kwargs Parameters and their values.
+     */
+    explicit XCS(py::kwargs kwargs)
+    {
+        reset();
+        set_params(kwargs);
         xcsf_init(&xcs);
+    }
+
+    /**
+     * @brief Resets basic constructor variables.
+     */
+    void
+    reset(void)
+    {
         state = NULL;
         action = 0;
         payoff = 0;
-        train_data = (struct Input *) malloc(sizeof(struct Input));
+        train_data = new struct Input;
         train_data->n_samples = 0;
         train_data->x_dim = 0;
         train_data->y_dim = 0;
         train_data->x = NULL;
         train_data->y = NULL;
-        test_data = (struct Input *) malloc(sizeof(struct Input));
+        test_data = new struct Input;
         test_data->n_samples = 0;
         test_data->x_dim = 0;
         test_data->y_dim = 0;
         test_data->x = NULL;
         test_data->y = NULL;
-    }
-
-    /**
-     * @brief Returns the XCSF major version number.
-     * @return Major version number.
-     */
-    int
-    version_major(void)
-    {
-        return VERSION_MAJOR;
-    }
-
-    /**
-     * @brief Returns the XCSF minor version number.
-     * @return Minor version number.
-     */
-    int
-    version_minor(void)
-    {
-        return VERSION_MINOR;
-    }
-
-    /**
-     * @brief Returns the XCSF build version number.
-     * @return Build version number.
-     */
-    int
-    version_build(void)
-    {
-        return VERSION_BUILD;
+        val_data = NULL;
+        metric_counter = 0;
+        param_init(&xcs, 1, 1, 1);
+        update_params();
     }
 
     /**
      * @brief Writes the entire current state of XCSF to a file.
      * @param [in] filename String containing the name of the output file.
      * @return The total number of elements written.
      */
@@ -140,15 +143,17 @@
      * @brief Reads the entire current state of XCSF from a file.
      * @param [in] filename String containing the name of the input file.
      * @return The total number of elements read.
      */
     size_t
     load(const char *filename)
     {
-        return xcsf_load(&xcs, filename);
+        size_t s = xcsf_load(&xcs, filename);
+        update_params();
+        return s;
     }
 
     /**
      * @brief Stores the current population in memory for later retrieval.
      */
     void
     store(void)
@@ -319,83 +324,247 @@
         payoff = reward;
         return xcs_rl_error(&xcs, action, payoff, done, max_p);
     }
 
     /* Supervised learning */
 
     /**
+     * @brief Sets XCSF input and output dimensions.
+     * @param [in] n_x_dim Number of input dimensions.
+     * @param [in] x1 Size of second input dimension.
+     * @param [in] n_y_dim Number of output dimensions.
+     * @param [in] y1 Size of second output dimension.
+     */
+    void
+    set_dims(int n_x_dim, int x1, int n_y_dim, int y1)
+    {
+        py::dict kwargs;
+        kwargs["n_actions"] = 1;
+        if (n_x_dim > 1) {
+            kwargs["x_dim"] = x1;
+        } else {
+            kwargs["x_dim"] = 1;
+        }
+        if (n_y_dim > 1) {
+            kwargs["y_dim"] = y1;
+        } else {
+            kwargs["y_dim"] = 1;
+        }
+        // update external params dict
+        for (const auto &item : kwargs) {
+            params[item.first] = item.second;
+        }
+        // flush param update to make sure neural nets resize
+        set_params(params);
+    }
+
+    /**
      * @brief Loads an input data structure for fitting.
      * @param [in,out] data Input data structure used to point to the data.
      * @param [in] X Vector of features with shape (n_samples, x_dim).
      * @param [in] Y Vector of truth values with shape (n_samples, y_dim).
      */
     void
     load_input(struct Input *data, const py::array_t<double> X,
                const py::array_t<double> Y)
     {
         const py::buffer_info buf_x = X.request();
         const py::buffer_info buf_y = Y.request();
+        if (buf_x.ndim < 1 || buf_x.ndim > 2) {
+            std::string error = "load_input(): X must be 1 or 2-D array";
+            throw std::invalid_argument(error);
+        }
+        if (buf_y.ndim < 1 || buf_y.ndim > 2) {
+            std::string error = "load_input(): Y must be 1 or 2-D array";
+            throw std::invalid_argument(error);
+        }
         if (buf_x.shape[0] != buf_y.shape[0]) {
-            std::string error =
-                "load_input(): X and Y n_samples are not equal.";
+            std::string error = "load_input(): X and Y n_samples are not equal";
             throw std::invalid_argument(error);
         }
-        if (buf_x.shape[1] != xcs.x_dim) {
+        if (buf_x.ndim > 1 && buf_x.shape[1] != xcs.x_dim) {
             std::ostringstream error;
-            error << "load_input(): x_dim != " << xcs.x_dim << std::endl;
-            error << "2-D arrays are required. Perhaps reshape your data.";
+            error << "load_input():";
+            error << " received x_dim: (" << buf_x.shape[1] << ")";
+            error << " but expected (" << xcs.x_dim << ")" << std::endl;
+            error << "Perhaps reshape your data.";
             throw std::invalid_argument(error.str());
         }
-        if (buf_y.shape[1] != xcs.y_dim) {
+        if (buf_y.ndim > 1 && buf_y.shape[1] != xcs.y_dim) {
             std::ostringstream error;
-            error << "load_input(): y_dim != " << xcs.y_dim << std::endl;
-            error << "2-D arrays are required. Perhaps reshape your data.";
+            error << "load_input():";
+            error << " received y_dim: (" << buf_y.shape[1] << ")";
+            error << " but expected (" << xcs.y_dim << ")" << std::endl;
+            error << "Perhaps reshape your data.";
             throw std::invalid_argument(error.str());
         }
         data->n_samples = buf_x.shape[0];
-        data->x_dim = buf_x.shape[1];
-        data->y_dim = buf_y.shape[1];
+        data->x_dim = xcs.x_dim;
+        data->y_dim = xcs.y_dim;
         data->x = (double *) buf_x.ptr;
         data->y = (double *) buf_y.ptr;
     }
 
     /**
-     * @brief Executes MAX_TRIALS number of XCSF learning iterations using the
-     * provided training data.
-     * @param [in] train_X The input values to use for training.
-     * @param [in] train_Y The true output values to use for training.
-     * @param [in] shuffle Whether to randomise the instances during training.
-     * @return The average XCSF training error using the loss function.
+     * @brief Prints the current performance metrics.
      */
-    double
-    fit(const py::array_t<double> train_X, const py::array_t<double> train_Y,
-        const bool shuffle)
+    void
+    print_status()
+    {
+        double trial = py::cast<double>(metric_trial[metric_trial.size() - 1]);
+        double train = py::cast<double>(metric_train[metric_train.size() - 1]);
+        double psize = py::cast<double>(metric_psize[metric_psize.size() - 1]);
+        double msize = py::cast<double>(metric_msize[metric_msize.size() - 1]);
+        double mfrac = py::cast<double>(metric_mfrac[metric_mfrac.size() - 1]);
+        std::ostringstream status;
+        status << get_timestamp();
+        status << " trials=" << trial;
+        status << " train=" << std::fixed << std::setprecision(5) << train;
+        if (val_data != NULL) {
+            double val = py::cast<double>(metric_val[metric_val.size() - 1]);
+            status << " val=" << std::fixed << std::setprecision(5) << val;
+        }
+        status << " pset=" << std::fixed << std::setprecision(1) << psize;
+        status << " mset=" << std::fixed << std::setprecision(1) << msize;
+        status << " mfrac=" << std::fixed << std::setprecision(2) << mfrac;
+        py::print(status.str());
+    }
+
+    /**
+     * @brief Updates performance metrics.
+     * @param [in] train The current training error.
+     * @param [in] val The current validation error.
+     * @param [in] n_trials Number of trials run.
+     */
+    void
+    update_metrics(const double train, const double val, const int n_trials)
+    {
+        const int trial = (1 + metric_counter) * n_trials;
+        metric_train.append(train);
+        metric_val.append(val);
+        metric_trial.append(trial);
+        metric_psize.append(xcs.pset.size);
+        metric_msize.append(xcs.mset_size);
+        metric_mfrac.append(xcs.mfrac);
+        ++metric_counter;
+    }
+
+    /**
+     * @brief Loads validation data if present in kwargs.
+     * @param [in] kwargs Parameters and their values.
+     */
+    void
+    load_validation_data(py::kwargs kwargs)
+    {
+        val_data = NULL;
+        if (kwargs.contains("validation_data")) {
+            py::tuple data = kwargs["validation_data"].cast<py::tuple>();
+            if (data) {
+                py::array_t<double> X_val = data[0].cast<py::array_t<double>>();
+                py::array_t<double> y_val = data[1].cast<py::array_t<double>>();
+                load_input(test_data, X_val, y_val);
+                val_data = test_data;
+                // use zeros for validation predictions instead of covering
+                memset(xcs.cover, 0, sizeof(double) * xcs.pa_size);
+            }
+        }
+    }
+
+    /**
+     * @brief Executes callbacks and returns whether to terminate.
+     * @param [in] callbacks The callbacks to perform.
+     * @return Whether to terminate early.
+     */
+    bool
+    callbacks_run(py::list callbacks)
+    {
+        bool terminate = false;
+        py::dict metrics = get_metrics();
+        for (py::handle item : callbacks) {
+            if (py::isinstance<Callback>(item)) {
+                Callback *cb = py::cast<Callback *>(item);
+                if (cb->run(&xcs, metrics)) {
+                    terminate = true;
+                }
+            } else {
+                std::ostringstream err;
+                err << "unsupported callback" << std::endl;
+                throw std::invalid_argument(err.str());
+            }
+        }
+        return terminate;
+    }
+
+    /**
+     * @brief Executes callback finish.
+     * @param [in] callbacks The callbacks to perform.
+     */
+    void
+    callbacks_finish(py::list callbacks)
     {
-        load_input(train_data, train_X, train_Y);
-        return xcs_supervised_fit(&xcs, train_data, NULL, shuffle);
+        for (py::handle item : callbacks) {
+            if (py::isinstance<Callback>(item)) {
+                Callback *cb = py::cast<Callback *>(item);
+                cb->finish(&xcs);
+            } else {
+                std::ostringstream err;
+                err << "unsupported callback" << std::endl;
+                throw std::invalid_argument(err.str());
+            }
+        }
     }
 
     /**
      * @brief Executes MAX_TRIALS number of XCSF learning iterations using the
-     * provided training data and test iterations using the test data.
-     * @param [in] train_X The input values to use for training.
-     * @param [in] train_Y The true output values to use for training.
-     * @param [in] test_X The input values to use for testing.
-     * @param [in] test_Y The true output values to use for testing.
+     * provided training data.
+     * @param [in] X_train The input values to use for training.
+     * @param [in] y_train The true output values to use for training.
      * @param [in] shuffle Whether to randomise the instances during training.
-     * @return The average XCSF training error using the loss function.
-     */
-    double
-    fit(const py::array_t<double> train_X, const py::array_t<double> train_Y,
-        const py::array_t<double> test_X, const py::array_t<double> test_Y,
-        const bool shuffle)
-    {
-        load_input(train_data, train_X, train_Y);
-        load_input(test_data, test_X, test_Y);
-        return xcs_supervised_fit(&xcs, train_data, test_data, shuffle);
+     * @param [in] warm_start Whether to continue with existing population.
+     * @param [in] verbose Whether to print learning metrics.
+     * @param [in] callbacks List of Callback objects or None.
+     * @param [in] kwargs Keyword arguments.
+     * @return The fitted XCSF model.
+     */
+    XCS &
+    fit(const py::array_t<double> X_train, const py::array_t<double> y_train,
+        const bool shuffle, const bool warm_start, const bool verbose,
+        py::object callbacks, py::kwargs kwargs)
+    {
+        if (!warm_start) { // re-initialise XCSF as necessary
+            xcsf_free(&xcs);
+            xcsf_init(&xcs);
+        }
+        load_input(train_data, X_train, y_train);
+        load_validation_data(kwargs);
+        // get callbacks
+        py::list calls;
+        if (py::isinstance<py::list>(callbacks)) {
+            calls = callbacks.cast<py::list>();
+        }
+        // break up the learning into epochs to track metrics
+        const int n = ceil(xcs.MAX_TRIALS / (double) xcs.PERF_TRIALS);
+        const int n_trials = std::min(xcs.MAX_TRIALS, xcs.PERF_TRIALS);
+        for (int i = 0; i < n; ++i) {
+            const double train =
+                xcs_supervised_fit(&xcs, train_data, NULL, shuffle, n_trials);
+            double val = 0;
+            if (val_data != NULL) {
+                val = xcs_supervised_score(&xcs, val_data, xcs.cover);
+            }
+            update_metrics(train, val, n_trials);
+            if (verbose) {
+                print_status();
+            }
+            if (callbacks_run(calls)) {
+                break;
+            }
+        }
+        callbacks_finish(calls);
+        return *this;
     }
 
     /**
      * @brief Returns the values specified in the cover array.
      * @param [in] cover The values to return for covering.
      * @return The cover array values.
      */
@@ -415,119 +584,85 @@
                 << xcs.y_dim << std::endl;
             throw std::invalid_argument(err.str());
         }
         return reinterpret_cast<double *>(buf_c.ptr);
     }
 
     /**
-     * @brief Returns the XCSF prediction array for the provided input.
-     * @param [in] X The input variables.
-     * @param [in] cover If cover is not NULL and the match set is empty, the
-     * prediction array will be set to this value instead of covering.
-     * @return The prediction array values.
+     * @brief Sets the XCSF cover array to values given, or zeros.
+     * @param [in] cover The values to use instead of covering.
      */
-    py::array_t<double>
-    get_predictions(const py::array_t<double> X, const double *cover)
+    void
+    set_cover(const py::object &cover)
     {
-        const py::buffer_info buf_x = X.request();
-        const int n_samples = buf_x.shape[0];
-        if (buf_x.shape[1] != xcs.x_dim) {
-            std::ostringstream err;
-            err << "predict(): x_dim (" << buf_x.shape[1]
-                << ") is not equal to: " << xcs.x_dim << std::endl;
-            err << "2-D arrays are required. Perhaps reshape your data.";
-            throw std::invalid_argument(err.str());
+        if (cover.is_none()) {
+            memset(xcs.cover, 0, sizeof(double) * xcs.pa_size);
+        } else {
+            py::array_t<double> cover_arr = cover.cast<py::array_t<double>>();
+            xcs.cover = get_cover(cover_arr);
         }
-        const double *input = reinterpret_cast<double *>(buf_x.ptr);
-        double *output =
-            (double *) malloc(sizeof(double) * n_samples * xcs.pa_size);
-        xcs_supervised_predict(&xcs, input, output, n_samples, cover);
-        return py::array_t<double>(
-            std::vector<ptrdiff_t>{ n_samples, xcs.pa_size }, output);
     }
 
     /**
      * @brief Returns the XCSF prediction array for the provided input.
      * @param [in] X The input variables.
      * @param [in] cover If the match set is empty, the prediction array will
      * be set to this value instead of covering.
      * @return The prediction array values.
      */
     py::array_t<double>
-    predict(const py::array_t<double> X, const py::array_t<double> cover)
-    {
-        const double *cov = get_cover(cover);
-        return get_predictions(X, cov);
-    }
-
-    /**
-     * @brief Returns the XCSF prediction array for the provided input,
-     * and executes covering for samples where the match set is empty.
-     * @param [in] X The input variables.
-     * @return The prediction array values.
-     */
-    py::array_t<double>
-    predict(const py::array_t<double> X)
+    predict(const py::array_t<double> X, const py::object &cover)
     {
-        return get_predictions(X, NULL);
+        const py::buffer_info buf_x = X.request();
+        if (buf_x.ndim < 1 || buf_x.ndim > 2) {
+            std::string error = "predict(): X must be 1 or 2-D array";
+            throw std::invalid_argument(error);
+        }
+        if (buf_x.ndim > 1 && buf_x.shape[1] != xcs.x_dim) {
+            std::ostringstream error;
+            error << "predict():";
+            error << " received x_dim: (" << buf_x.shape[1] << ")";
+            error << " but expected (" << xcs.x_dim << ")" << std::endl;
+            error << "Perhaps reshape your data.";
+            throw std::invalid_argument(error.str());
+        }
+        const int n_samples = buf_x.shape[0];
+        const double *input = reinterpret_cast<double *>(buf_x.ptr);
+        double *output =
+            (double *) malloc(sizeof(double) * n_samples * xcs.pa_size);
+        set_cover(cover);
+        xcs_supervised_predict(&xcs, input, output, n_samples, xcs.cover);
+        return py::array_t<double>(
+            std::vector<ptrdiff_t>{ n_samples, xcs.pa_size }, output);
     }
 
     /**
      * @brief Returns the error using N random samples from the provided data.
      * @param [in] X The input values to use for scoring.
      * @param [in] Y The true output values to use for scoring.
      * @param [in] N The maximum number of samples to draw randomly for scoring.
      * @param [in] cover If the match set is empty, the prediction array will
-     * be set to this value instead of covering.
+     * be set to this value, otherwise it is set to zeros.
      * @return The average XCSF error using the loss function.
      */
     double
-    get_score(const py::array_t<double> X, const py::array_t<double> Y,
-              const int N, const double *cover)
+    score(const py::array_t<double> X, const py::array_t<double> Y, const int N,
+          const py::object &cover)
     {
+        set_cover(cover);
         load_input(test_data, X, Y);
         if (N > 1) {
-            return xcs_supervised_score_n(&xcs, test_data, N, cover);
+            return xcs_supervised_score_n(&xcs, test_data, N, xcs.cover);
         }
-        return xcs_supervised_score(&xcs, test_data, cover);
-    }
-
-    /**
-     * @brief Returns the error using N random samples from the provided data.
-     * @param [in] X The input values to use for scoring.
-     * @param [in] Y The true output values to use for scoring.
-     * @param [in] N The maximum number of samples to draw randomly for scoring.
-     * @return The average XCSF error using the loss function.
-     */
-    double
-    score(const py::array_t<double> X, const py::array_t<double> Y, const int N)
-    {
-        return get_score(X, Y, N, NULL);
-    }
-
-    /**
-     * @brief Returns the error using N random samples from the provided data.
-     * @param [in] X The input values to use for scoring.
-     * @param [in] Y The true output values to use for scoring.
-     * @param [in] N The maximum number of samples to draw randomly for scoring.
-     * @param [in] cover If the match set is empty, the prediction array will
-     * be set to this value instead of covering.
-     * @return The average XCSF error using the loss function.
-     */
-    double
-    score(const py::array_t<double> X, const py::array_t<double> Y, const int N,
-          const py::array_t<double> cover)
-    {
-        const double *cov = get_cover(cover);
-        return get_score(X, Y, N, cov);
+        return xcs_supervised_score(&xcs, test_data, xcs.cover);
     }
 
     /**
      * @brief Implements pickle file writing.
-     * @defails Uses a temporary binary file.
+     * @details Uses a temporary binary file.
      * @return The pickled XCSF.
      */
     py::bytes
     serialize() const
     {
         // Write XCSF to a temporary binary file
         const char *filename = "_tmp_pickle.bin";
@@ -543,30 +678,32 @@
         }
         // Return the binary data as bytes
         return py::bytes(state);
     }
 
     /**
      * @brief Implements pickle file reading.
-     * @defails Uses a temporary binary file.
+     * @details Uses a temporary binary file.
      * @param state The pickled state of a saved XCSF.
      */
     static XCS
     deserialize(const py::bytes &state)
     {
         // Write the XCSF bytes to a temporary binary file
         const char *filename = "_tmp_pickle.bin";
         std::ofstream file(filename, std::ios::binary);
         file.write(state.cast<std::string>().c_str(),
                    state.cast<std::string>().size());
         file.close();
         // Create a new XCSF instance
-        XCS xcs(1, 1, 1);
+        XCS xcs = XCS();
         // Load XCSF
         xcsf_load(&xcs.xcs, filename);
+        // Update object params
+        xcs.update_params();
         // Delete the temporary file
         if (std::remove(filename) != 0) {
             perror("Error deleting temporary pickle file");
         }
         // Return the deserialized XCSF
         return xcs;
     }
@@ -579,132 +716,25 @@
      */
     double
     error(void)
     {
         return xcs.error;
     }
 
-    int
-    get_omp_num_threads(void)
-    {
-        return xcs.OMP_NUM_THREADS;
-    }
-
-    bool
-    get_pop_init(void)
-    {
-        return xcs.POP_INIT;
-    }
-
-    int
-    get_max_trials(void)
-    {
-        return xcs.MAX_TRIALS;
-    }
-
-    int
-    get_perf_trials(void)
+    py::dict
+    get_metrics(void)
     {
-        return xcs.PERF_TRIALS;
-    }
-
-    int
-    get_pop_max_size(void)
-    {
-        return xcs.POP_SIZE;
-    }
-
-    const char *
-    get_loss_func(void)
-    {
-        return loss_type_as_string(xcs.LOSS_FUNC);
-    }
-
-    double
-    get_huber_delta(void)
-    {
-        return xcs.HUBER_DELTA;
-    }
-
-    double
-    get_alpha(void)
-    {
-        return xcs.ALPHA;
-    }
-
-    double
-    get_beta(void)
-    {
-        return xcs.BETA;
-    }
-
-    double
-    get_delta(void)
-    {
-        return xcs.DELTA;
-    }
-
-    double
-    get_e0(void)
-    {
-        return xcs.E0;
-    }
-
-    double
-    get_init_error(void)
-    {
-        return xcs.INIT_ERROR;
-    }
-
-    double
-    get_init_fitness(void)
-    {
-        return xcs.INIT_FITNESS;
-    }
-
-    double
-    get_nu(void)
-    {
-        return xcs.NU;
-    }
-
-    int
-    get_m_probation(void)
-    {
-        return xcs.M_PROBATION;
-    }
-
-    bool
-    get_stateful(void)
-    {
-        return xcs.STATEFUL;
-    }
-
-    bool
-    get_compaction(void)
-    {
-        return xcs.COMPACTION;
-    }
-
-    int
-    get_theta_del(void)
-    {
-        return xcs.THETA_DEL;
-    }
-
-    int
-    get_theta_sub(void)
-    {
-        return xcs.THETA_SUB;
-    }
-
-    bool
-    get_set_subsumption(void)
-    {
-        return xcs.SET_SUBSUMPTION;
+        py::dict metrics;
+        metrics["train"] = metric_train;
+        metrics["val"] = metric_val;
+        metrics["trials"] = metric_trial;
+        metrics["psize"] = metric_psize;
+        metrics["msize"] = metric_msize;
+        metrics["mfrac"] = metric_mfrac;
+        return metrics;
     }
 
     int
     get_pset_size(void)
     {
         return xcs.pset.size;
     }
@@ -717,32 +747,14 @@
 
     int
     get_time(void)
     {
         return xcs.time;
     }
 
-    int
-    get_x_dim(void)
-    {
-        return xcs.x_dim;
-    }
-
-    int
-    get_y_dim(void)
-    {
-        return xcs.y_dim;
-    }
-
-    int
-    get_n_actions(void)
-    {
-        return xcs.n_actions;
-    }
-
     double
     get_pset_mean_cond_size(void)
     {
         return clset_mean_cond_size(&xcs, &xcs.pset);
     }
 
     double
@@ -807,511 +819,114 @@
 
     double
     get_mfrac(void)
     {
         return xcs.mfrac;
     }
 
-    int
-    get_teletransportation(void)
-    {
-        return xcs.TELETRANSPORTATION;
-    }
-
-    double
-    get_gamma(void)
-    {
-        return xcs.GAMMA;
-    }
-
-    double
-    get_p_explore(void)
-    {
-        return xcs.P_EXPLORE;
-    }
-
-    const char *
-    get_ea_select_type(void)
-    {
-        return ea_type_as_string(xcs.ea->select_type);
-    }
-
-    double
-    get_ea_select_size(void)
-    {
-        return xcs.ea->select_size;
-    }
-
-    double
-    get_theta_ea(void)
-    {
-        return xcs.ea->theta;
-    }
-
-    int
-    get_lambda(void)
-    {
-        return xcs.ea->lambda;
-    }
-
-    double
-    get_p_crossover(void)
-    {
-        return xcs.ea->p_crossover;
-    }
-
-    double
-    get_err_reduc(void)
-    {
-        return xcs.ea->err_reduc;
-    }
-
-    double
-    get_fit_reduc(void)
-    {
-        return xcs.ea->fit_reduc;
-    }
-
-    bool
-    get_ea_subsumption(void)
-    {
-        return xcs.ea->subsumption;
-    }
-
-    bool
-    get_ea_pred_reset(void)
-    {
-        return xcs.ea->pred_reset;
-    }
-
-    /* SETTERS */
-
-    /**
-     * @brief Sets the condition type.
-     * @param [in] type String representing a name of a condition type.
-     */
-    void
-    set_condition(const std::string &type)
-    {
-        if (cond_param_set_type_string(&xcs, type.c_str()) ==
-            COND_TYPE_INVALID) {
-            std::ostringstream msg;
-            msg << "Invalid condition type: " << type << ". Options: {"
-                << COND_TYPE_OPTIONS << "}" << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-    }
+    /* JSON */
 
     /**
-     * @brief Sets the action type.
-     * @param [in] type String representing a name of an action type.
+     * @brief Returns a JSON formatted string representing the population set.
+     * @param [in] condition Whether to return the condition.
+     * @param [in] action Whether to return the action.
+     * @param [in] prediction Whether to return the prediction.
+     * @return String encoded in json format.
      */
-    void
-    set_action(const std::string &type)
+    const char *
+    json_export(const bool condition, const bool action, const bool prediction)
     {
-        if (action_param_set_type_string(&xcs, type.c_str()) ==
-            ACT_TYPE_INVALID) {
-            std::ostringstream msg;
-            msg << "Invalid action type: " << type << ". Options: {"
-                << ACT_TYPE_OPTIONS << "}" << std::endl;
-            throw std::invalid_argument(msg.str());
+        if (xcs.pset.list != NULL) {
+            return clset_json_export(&xcs, &xcs.pset, condition, action,
+                                     prediction);
         }
+        return "null";
     }
 
     /**
-     * @brief Sets the prediction type.
-     * @param [in] type String representing a name of a prediction type.
+     * @brief Updates the Python object's parameter dictionary.
      */
     void
-    set_prediction(const std::string &type)
+    update_params()
     {
-        if (pred_param_set_type_string(&xcs, type.c_str()) ==
-            PRED_TYPE_INVALID) {
-            std::ostringstream msg;
-            msg << "Invalid prediction type: " << type << ". Options: {"
-                << PRED_TYPE_OPTIONS << "}" << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-    }
-
-    /**
-     * @brief Finds and replaces all occurrences of a substring.
-     * @param [in] subject String to be searched and replaced.
-     * @param [in] search String within the subject to find.
-     * @param [in] replace String to replace the found text with.
-     * @return String.
-     */
-    std::string
-    find_replace_all(std::string subject, const std::string &search,
-                     const std::string &replace)
-    {
-        size_t pos = 0;
-        while ((pos = subject.find(search, pos)) != std::string::npos) {
-            subject.replace(pos, search.length(), replace);
-            pos += replace.length();
-        }
-        return subject;
+        char *json_str = param_json_export(&xcs);
+        py::module json = py::module::import("json");
+        py::object parsed_json = json.attr("loads")(json_str);
+        py::dict result(parsed_json);
+        params = result;
+        free(json_str);
     }
 
     /**
-     * @brief Converts a Python dictionary to a C++ string (JSON).
-     * @param [in] kwargs Python dictionary of argument name:value pairs.
-     * @return JSON string representation of a dictionary.
+     * @brief Returns a dictionary of parameters.
+     * @param deep For sklearn compatibility.
+     * @return External parameter dictionary.
      */
-    cJSON *
-    dict_to_json(const py::dict &kwargs)
+    py::dict
+    get_params(const bool deep)
     {
-        py::str s = py::str(*kwargs);
-        std::string cs = s.cast<std::string>();
-        cs = find_replace_all(cs, "True", "true");
-        cs = find_replace_all(cs, "False", "false");
-        cs = find_replace_all(cs, "\'", "\"");
-        cJSON *json = cJSON_Parse(cs.c_str());
-        utils_json_parse_check(json);
-        return json;
+        (void) deep;
+        return params;
     }
 
     /**
-     * @brief Sets the condition type and initialisation arguments.
-     * @param [in] type String representing a name of a condition type.
-     * @param [in] kwargs Python dictionary of argument name:value pairs.
+     * @brief Sets parameter values.
+     * @param kwargs Parameters and their values.
+     * @return The XCSF object.
      */
-    void
-    set_condition(const std::string &type, const py::dict &kwargs)
+    XCS &
+    set_params(py::kwargs kwargs)
     {
-        set_condition(type);
-        cJSON *args = dict_to_json(kwargs);
-        const char *ret = cond_param_json_import(&xcs, args);
-        if (ret != NULL) {
-            std::ostringstream msg;
-            msg << "Invalid condition parameter: " << ret << std::endl;
-            throw std::invalid_argument(msg.str());
+        py::dict kwargs_dict(kwargs);
+        py::module json_module = py::module::import("json");
+        py::object json_dumps = json_module.attr("dumps")(kwargs_dict);
+        std::string json_str = json_dumps.cast<std::string>();
+        const char *json_params = json_str.c_str();
+        param_json_import(&xcs, json_params);
+        for (const auto &item : kwargs_dict) {
+            params[item.first] = item.second;
         }
-        cJSON_Delete(args);
+        return *this;
     }
 
     /**
-     * @brief Sets the action type and initialisation arguments.
-     * @param [in] type String representing a name of a condition type.
-     * @param [in] kwargs Python dictionary of argument name:value pairs.
+     * @brief Returns a dictionary of the internal parameters.
+     * @return Internal parameter dictionary.
      */
-    void
-    set_action(const std::string &type, const py::dict &kwargs)
+    py::dict
+    internal_params()
     {
-        set_action(type);
-        cJSON *args = dict_to_json(kwargs);
-        const char *ret = action_param_json_import(&xcs, args);
-        if (ret != NULL) {
-            std::ostringstream msg;
-            msg << "Invalid action parameter: " << ret << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-        cJSON_Delete(args);
-    }
-
-    /**
-     * @brief Sets the prediction type and initialisation arguments.
-     * @param [in] type String representing a name of a condition type.
-     * @param [in] kwargs Python dictionary of argument name:value pairs.
-     */
-    void
-    set_prediction(const std::string &type, const py::dict &kwargs)
-    {
-        set_prediction(type);
-        cJSON *args = dict_to_json(kwargs);
-        const char *ret = pred_param_json_import(&xcs, args);
-        if (ret != NULL) {
-            std::ostringstream msg;
-            msg << "Invalid prediction parameter: " << ret << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-        cJSON_Delete(args);
-    }
-
-    void
-    catch_error(const char *ret)
-    {
-        if (ret != NULL) {
-            std::ostringstream msg;
-            msg << ret << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-    }
-
-    void
-    set_omp_num_threads(const int a)
-    {
-        catch_error(param_set_omp_num_threads(&xcs, a));
-    }
-
-    void
-    set_pop_init(const bool a)
-    {
-        catch_error(param_set_pop_init(&xcs, a));
-    }
-
-    void
-    set_max_trials(const int a)
-    {
-        catch_error(param_set_max_trials(&xcs, a));
-    }
-
-    void
-    set_perf_trials(const int a)
-    {
-        catch_error(param_set_perf_trials(&xcs, a));
-    }
-
-    void
-    set_pop_max_size(const int a)
-    {
-        catch_error(param_set_pop_size(&xcs, a));
-    }
-
-    void
-    set_loss_func(const char *a)
-    {
-        if (param_set_loss_func_string(&xcs, a) == PARAM_INVALID) {
-            std::ostringstream msg;
-            msg << "Invalid loss function: " << a << ". Options: {"
-                << LOSS_OPTIONS << "}" << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-    }
-
-    void
-    set_huber_delta(const double a)
-    {
-        catch_error(param_set_huber_delta(&xcs, a));
-    }
-
-    void
-    set_alpha(const double a)
-    {
-        catch_error(param_set_alpha(&xcs, a));
-    }
-
-    void
-    set_beta(const double a)
-    {
-        catch_error(param_set_beta(&xcs, a));
-    }
-
-    void
-    set_delta(const double a)
-    {
-        catch_error(param_set_delta(&xcs, a));
-    }
-
-    void
-    set_e0(const double a)
-    {
-        catch_error(param_set_e0(&xcs, a));
-    }
-
-    void
-    set_init_error(const double a)
-    {
-        catch_error(param_set_init_error(&xcs, a));
-    }
-
-    void
-    set_init_fitness(const double a)
-    {
-        catch_error(param_set_init_fitness(&xcs, a));
-    }
-
-    void
-    set_nu(const double a)
-    {
-        catch_error(param_set_nu(&xcs, a));
-    }
-
-    void
-    set_m_probation(const int a)
-    {
-        catch_error(param_set_m_probation(&xcs, a));
-    }
-
-    void
-    set_theta_del(const int a)
-    {
-        catch_error(param_set_theta_del(&xcs, a));
-    }
-
-    void
-    set_theta_sub(const int a)
-    {
-        catch_error(param_set_theta_sub(&xcs, a));
-    }
-
-    void
-    set_set_subsumption(const bool a)
-    {
-        catch_error(param_set_set_subsumption(&xcs, a));
-    }
-
-    void
-    set_teletransportation(const int a)
-    {
-        catch_error(param_set_teletransportation(&xcs, a));
-    }
-
-    void
-    set_stateful(const bool a)
-    {
-        catch_error(param_set_stateful(&xcs, a));
-    }
-
-    void
-    set_compaction(const bool a)
-    {
-        catch_error(param_set_compaction(&xcs, a));
-    }
-
-    void
-    set_gamma(const double a)
-    {
-        catch_error(param_set_gamma(&xcs, a));
-    }
-
-    void
-    set_p_explore(const double a)
-    {
-        catch_error(param_set_p_explore(&xcs, a));
-    }
-
-    void
-    set_ea_select_type(const char *a)
-    {
-        if (ea_param_set_type_string(&xcs, a) == EA_SELECT_INVALID) {
-            std::ostringstream msg;
-            msg << "Invalid EA SELECT_TYPE: " << a << ". Options: {"
-                << EA_SELECT_OPTIONS << "}" << std::endl;
-            throw std::invalid_argument(msg.str());
-        }
-    }
-
-    void
-    set_ea_select_size(const double a)
-    {
-        catch_error(ea_param_set_select_size(&xcs, a));
-    }
-
-    void
-    set_theta_ea(const double a)
-    {
-        catch_error(ea_param_set_theta(&xcs, a));
-    }
-
-    void
-    set_lambda(const int a)
-    {
-        catch_error(ea_param_set_lambda(&xcs, a));
-    }
-
-    void
-    set_p_crossover(const double a)
-    {
-        catch_error(ea_param_set_p_crossover(&xcs, a));
-    }
-
-    void
-    set_err_reduc(const double a)
-    {
-        catch_error(ea_param_set_err_reduc(&xcs, a));
-    }
-
-    void
-    set_fit_reduc(const double a)
-    {
-        catch_error(ea_param_set_fit_reduc(&xcs, a));
-    }
-
-    void
-    set_ea_subsumption(const bool a)
-    {
-        catch_error(ea_param_set_subsumption(&xcs, a));
-    }
-
-    void
-    set_ea_pred_reset(const bool a)
-    {
-        catch_error(ea_param_set_pred_reset(&xcs, a));
-    }
-
-    void
-    seed(const uint32_t seed)
-    {
-        rand_init_seed(seed);
-    }
-
-    /* JSON */
-
-    /**
-     * @brief Returns a JSON formatted string representing the population set.
-     * @param [in] condition Whether to return the condition.
-     * @param [in] action Whether to return the action.
-     * @param [in] prediction Whether to return the prediction.
-     * @return String encoded in json format.
-     */
-    const char *
-    json_export(const bool condition, const bool action, const bool prediction)
-    {
-        if (xcs.pset.list != NULL) {
-            return clset_json_export(&xcs, &xcs.pset, condition, action,
-                                     prediction);
-        }
-        return "null";
-    }
-
-    /**
-     * @brief Returns a JSON formatted string representing the parameters.
-     * @return String encoded in json format.
-     */
-    const char *
-    json_parameters()
-    {
-        return param_json_export(&xcs);
+        char *json_str = param_json_export(&xcs);
+        py::module json_module = py::module::import("json");
+        py::dict internal_params = json_module.attr("loads")(json_str);
+        free(json_str);
+        return internal_params;
     }
 
     /**
      * @brief Creates a classifier from JSON and inserts into the population.
      * @param [in] json_str JSON formatted string representing a classifier.
      */
     void
     json_insert_cl(const std::string &json_str)
     {
         cJSON *json = cJSON_Parse(json_str.c_str());
         utils_json_parse_check(json);
-        clset_json_insert(&xcs, json);
+        clset_json_insert_cl(&xcs, json);
         cJSON_Delete(json);
     }
 
     /**
      * @brief Creates classifiers from JSON and inserts into the population.
      * @param [in] json_str JSON formatted string representing a classifier.
      */
     void
     json_insert(const std::string &json_str)
     {
-        cJSON *json = cJSON_Parse(json_str.c_str());
-        utils_json_parse_check(json);
-        if (json->child != NULL && cJSON_IsArray(json->child)) {
-            cJSON *tail = json->child->child; // insert inverted for consistency
-            tail->prev = NULL; // this should have been set by cJSON!
-            while (tail->next != NULL) {
-                tail = tail->next;
-            }
-            while (tail != NULL) {
-                clset_json_insert(&xcs, tail);
-                tail = tail->prev;
-            }
-        }
-        cJSON_Delete(json);
+        clset_json_insert(&xcs, json_str.c_str());
     }
 
     /**
      * @brief Writes the current population set to a file in JSON.
      * @param [in] filename Name of the output file.
      */
     void
@@ -1337,241 +952,108 @@
 };
 
 PYBIND11_MODULE(xcsf, m)
 {
     m.doc() = "XCSF learning classifier: rule-based online evolutionary "
               "machine learning.\nFor details on how to use this module see: "
               "https://github.com/rpreen/xcsf/wiki/Python-Library-Usage";
-    rand_init();
 
     double (XCS::*fit1)(const py::array_t<double>, const int, const double) =
         &XCS::fit;
-    double (XCS::*fit2)(const py::array_t<double>, const py::array_t<double>,
-                        const bool) = &XCS::fit;
-    double (XCS::*fit3)(const py::array_t<double>, const py::array_t<double>,
-                        const py::array_t<double>, const py::array_t<double>,
-                        const bool) = &XCS::fit;
-
-    py::array_t<double> (XCS::*predict1)(const py::array_t<double> test_X) =
-        &XCS::predict;
-    py::array_t<double> (XCS::*predict2)(const py::array_t<double> test_X,
-                                         const py::array_t<double> cover) =
-        &XCS::predict;
-
-    double (XCS::*score1)(const py::array_t<double> X,
-                          const py::array_t<double> Y, const int N) =
-        &XCS::score;
-
-    double (XCS::*score2)(const py::array_t<double> X,
-                          const py::array_t<double> Y, const int N,
-                          const py::array_t<double> cover) = &XCS::score;
+    XCS &(XCS::*fit2)(const py::array_t<double>, const py::array_t<double>,
+                      const bool, const bool, const bool, py::object,
+                      py::kwargs) = &XCS::fit;
 
     double (XCS::*error1)(void) = &XCS::error;
     double (XCS::*error2)(const double, const bool, const double) = &XCS::error;
 
-    void (XCS::*condition1)(const std::string &) = &XCS::set_condition;
-    void (XCS::*condition2)(const std::string &, const py::dict &) =
-        &XCS::set_condition;
-
-    void (XCS::*action1)(const std::string &) = &XCS::set_action;
-    void (XCS::*action2)(const std::string &, const py::dict &) =
-        &XCS::set_action;
-
-    void (XCS::*prediction1)(const std::string &) = &XCS::set_prediction;
-    void (XCS::*prediction2)(const std::string &, const py::dict &) =
-        &XCS::set_prediction;
+    py::class_<Callback, std::unique_ptr<Callback, py::nodelete>>(m,
+                                                                  "Callback");
+
+    py::class_<EarlyStoppingCallback, Callback,
+               std::unique_ptr<EarlyStoppingCallback, py::nodelete>>(
+        m, "EarlyStoppingCallback")
+        .def(py::init<py::str, int, bool, double, int, bool>(),
+             "Creates a callback for terminating the fit function early.",
+             py::arg("monitor") = "train", py::arg("patience") = 0,
+             py::arg("restore_best") = false, py::arg("min_delta") = 0,
+             py::arg("start_from") = 0, py::arg("verbose") = true);
+
+    py::class_<CheckpointCallback, Callback,
+               std::unique_ptr<CheckpointCallback, py::nodelete>>(
+        m, "CheckpointCallback")
+        .def(py::init<py::str, std::string, bool, int, bool>(),
+             "Creates a callback for automatically saving XCSF.",
+             py::arg("monitor") = "train", py::arg("filename") = "xcsf.bin",
+             py::arg("save_best_only") = false, py::arg("save_freq") = 0,
+             py::arg("verbose") = true);
 
     py::class_<XCS>(m, "XCS")
-        .def(py::init<const int, const int, const int>(),
-             "Creates a new XCSF class.", py::arg("x_dim"), py::arg("y_dim"),
-             py::arg("n_actions"))
-        .def("condition", condition1,
-             "Sets the condition type. Options: {" COND_TYPE_OPTIONS "}.",
-             py::arg("type"))
-        .def("condition", condition2,
-             "Sets the condition type and args. Options: {" COND_TYPE_OPTIONS
-             "}.",
-             py::arg("type"), py::arg("args"))
-        .def("action", action1,
-             "Sets the action type. Options: {" ACT_TYPE_OPTIONS "}.",
-             py::arg("type"))
-        .def("action", action2,
-             "Sets the action type and args. Options: {" ACT_TYPE_OPTIONS "}.",
-             py::arg("type"), py::arg("args"))
-        .def("prediction", prediction1,
-             "Sets the prediction type. Options: {" PRED_TYPE_OPTIONS "}.",
-             py::arg("type"))
-        .def("prediction", prediction2,
-             "Sets the prediction type and args. Options: {" PRED_TYPE_OPTIONS
-             "}.",
-             py::arg("type"), py::arg("args"))
+        .def(py::init(), "Creates a new XCSF class with default arguments.")
+        .def(py::init<py::kwargs>(),
+             "Creates a new XCSF class with specified arguments.")
         .def("fit", fit1,
              "Creates/updates an action set for a given (state, action, "
              "reward). state shape must be: (x_dim, ).",
              py::arg("state"), py::arg("action"), py::arg("reward"))
         .def("fit", fit2,
              "Executes MAX_TRIALS number of XCSF learning iterations using the "
              "provided training data. X_train shape must be: (n_samples, "
              "x_dim). y_train shape must be: (n_samples, y_dim).",
-             py::arg("X_train"), py::arg("y_train"), py::arg("shuffle") = true)
-        .def("fit", fit3,
-             "Executes MAX_TRIALS number of XCSF learning iterations using the "
-             "provided training data and test iterations using the test data. "
-             "X_train shape must be: (n_samples, x_dim). y_train shape must "
-             "be: (n_samples, y_dim). X_test shape must be: (n_samples, "
-             "x_dim). y_test shape must be: (n_samples, y_dim).",
-             py::arg("X_train"), py::arg("y_train"), py::arg("X_test"),
-             py::arg("y_test"), py::arg("shuffle") = true)
-        .def("score", score1,
-             "Returns the error using at most N random samples from the "
-             "provided data. X_val shape must be: (n_samples, x_dim). y_val "
-             "shape must be: (n_samples, y_dim).",
-             py::arg("X_val"), py::arg("y_val"), py::arg("N") = 0)
-        .def("score", score2,
-             "Returns the error using at most N random samples from the "
-             "provided data. X_val shape must be: (n_samples, x_dim). y_val "
-             "shape must be: (n_samples, y_dim).",
-             py::arg("X_val"), py::arg("y_val"), py::arg("N") = 0,
-             py::arg("cover"))
+             py::arg("X_train"), py::arg("y_train"), py::arg("shuffle") = true,
+             py::arg("warm_start") = false, py::arg("verbose") = true,
+             py::arg("callbacks") = py::none())
+        .def(
+            "score", &XCS::score,
+            "Returns the error using at most N random samples from the "
+            "provided data. N=0 uses all. X shape must be: (n_samples, x_dim). "
+            "y shape must be: (n_samples, y_dim). If the match set is empty "
+            "for a sample, the value of the cover array will be used "
+            "otherwise zeros.",
+            py::arg("X"), py::arg("y"), py::arg("N") = 0,
+            py::arg("cover") = py::none())
         .def("error", error1,
              "Returns a moving average of the system error, updated with step "
              "size BETA.")
         .def("error", error2,
              "Returns the reinforcement learning system prediction error.",
              py::arg("reward"), py::arg("done"), py::arg("max_p"))
-        .def("predict", predict1,
-             "Returns the XCSF prediction array for the provided input. X_test "
-             "shape must be: (n_samples, x_dim). Returns an array of shape: "
-             "(n_samples, y_dim). Covering will be invoked for samples where "
-             "the match set is empty.",
-             py::arg("X_test"))
-        .def("predict", predict2,
-             "Returns the XCSF prediction array for the provided input. X_test "
+        .def("predict", &XCS::predict,
+             "Returns the XCSF prediction array for the provided input. X "
              "shape must be: (n_samples, x_dim). Returns an array of shape: "
              "(n_samples, y_dim). If the match set is empty for a sample, the "
-             "value of the cover array will be used instead of covering. "
-             "cover must be an array of shape: y_dim.",
-             py::arg("X_test"), py::arg("cover"))
+             "value of the cover array will be used, otherwise zeros. "
+             "Cover must be an array of shape: y_dim.",
+             py::arg("X"), py::arg("cover") = py::none())
         .def("save", &XCS::save,
              "Saves the current state of XCSF to persistent storage.",
              py::arg("filename"))
         .def("load", &XCS::load,
              "Loads the current state of XCSF from persistent storage.",
              py::arg("filename"))
         .def("store", &XCS::store,
              "Stores the current XCSF population in memory for later "
              "retrieval, overwriting any previously stored population.")
         .def("retrieve", &XCS::retrieve,
              "Retrieves the previously stored XCSF population from memory.")
-        .def("version_major", &XCS::version_major,
-             "Returns the version major number.")
-        .def("version_minor", &XCS::version_minor,
-             "Returns the version minor number.")
-        .def("version_build", &XCS::version_build,
-             "Returns the version build number.")
         .def("init_trial", &XCS::init_trial, "Initialises a multi-step trial.")
         .def("end_trial", &XCS::end_trial, "Ends a multi-step trial.")
         .def("init_step", &XCS::init_step,
              "Initialises a step in a multi-step trial.")
         .def("end_step", &XCS::end_step, "Ends a step in a multi-step trial.")
         .def("decision", &XCS::decision,
              "Constructs the match set and selects an action to perform for "
              "reinforcement learning. state shape must be: (x_dim, )",
              py::arg("state"), py::arg("explore"))
         .def("update", &XCS::update,
              "Creates the action set using the previously selected action.",
              py::arg("reward"), py::arg("done"))
-        .def("seed", &XCS::seed, "Sets the random number seed.",
-             py::arg("seed"))
-        .def_property("OMP_NUM_THREADS", &XCS::get_omp_num_threads,
-                      &XCS::set_omp_num_threads, "Number of CPU cores to use.")
-        .def_property("POP_INIT", &XCS::get_pop_init, &XCS::set_pop_init,
-                      "Whether to seed the population with random rules.")
-        .def_property("MAX_TRIALS", &XCS::get_max_trials, &XCS::set_max_trials,
-                      "Number of problem instances to run in one experiment.")
-        .def_property("PERF_TRIALS", &XCS::get_perf_trials,
-                      &XCS::set_perf_trials,
-                      "Number of problem instances to avg performance output.")
-        .def_property("POP_SIZE", &XCS::get_pop_max_size,
-                      &XCS::set_pop_max_size,
-                      "Maximum number of micro-classifiers in the population.")
-        .def_property(
-            "LOSS_FUNC", &XCS::get_loss_func, &XCS::set_loss_func,
-            "Which loss/error function to apply. Options: {" LOSS_OPTIONS "}.")
-        .def_property("HUBER_DELTA", &XCS::get_huber_delta,
-                      &XCS::set_huber_delta,
-                      "Delta parameter for Huber loss calculation.")
-        .def_property(
-            "ALPHA", &XCS::get_alpha, &XCS::set_alpha,
-            "Linear coefficient used to calculate classifier accuracy.")
-        .def_property(
-            "BETA", &XCS::get_beta, &XCS::set_beta,
-            "Learning rate for updating error, fitness, and set size.")
-        .def_property("DELTA", &XCS::get_delta, &XCS::set_delta,
-                      "Fraction of population to increase deletion vote.")
-        .def_property(
-            "E0", &XCS::get_e0, &XCS::set_e0,
-            "Target error under which classifier accuracy is set to 1.")
-        .def_property("STATEFUL", &XCS::get_stateful, &XCS::set_stateful,
-                      "Whether classifiers should retain state across trials.")
-        .def_property("COMPACTION", &XCS::get_compaction, &XCS::set_compaction,
-                      "if sys err < E0: largest of 2 roulette spins deleted.")
-        .def_property("INIT_ERROR", &XCS::get_init_error, &XCS::set_init_error,
-                      "Initial classifier error value.")
-        .def_property("INIT_FITNESS", &XCS::get_init_fitness,
-                      &XCS::set_init_fitness,
-                      "Initial classifier fitness value.")
-        .def_property("NU", &XCS::get_nu, &XCS::set_nu,
-                      "Exponent used in calculating classifier accuracy.")
-        .def_property("M_PROBATION", &XCS::get_m_probation,
-                      &XCS::set_m_probation,
-                      "Trials since creation a cl must match at least 1 input.")
-        .def_property("THETA_DEL", &XCS::get_theta_del, &XCS::set_theta_del,
-                      "Min experience before fitness used during deletion.")
-        .def_property(
-            "THETA_SUB", &XCS::get_theta_sub, &XCS::set_theta_sub,
-            "Minimum experience of a classifier to become a subsumer.")
-        .def_property("SET_SUBSUMPTION", &XCS::get_set_subsumption,
-                      &XCS::set_set_subsumption,
-                      "Whether to perform match set subsumption.")
-        .def_property("TELETRANSPORTATION", &XCS::get_teletransportation,
-                      &XCS::set_teletransportation,
-                      "Maximum steps for a multi-step problem.")
-        .def_property("GAMMA", &XCS::get_gamma, &XCS::set_gamma,
-                      "Discount factor for multi-step reward.")
-        .def_property("P_EXPLORE", &XCS::get_p_explore, &XCS::set_p_explore,
-                      "Probability of exploring vs. exploiting.")
-        .def_property("EA_SELECT_TYPE", &XCS::get_ea_select_type,
-                      &XCS::set_ea_select_type,
-                      "EA parental selection type. Options: {" EA_SELECT_OPTIONS
-                      "}.")
-        .def_property("EA_SELECT_SIZE", &XCS::get_ea_select_size,
-                      &XCS::set_ea_select_size,
-                      "Fraction of set size for tournaments.")
-        .def_property("THETA_EA", &XCS::get_theta_ea, &XCS::set_theta_ea,
-                      "Average match set time between EA invocations.")
-        .def_property("P_CROSSOVER", &XCS::get_p_crossover,
-                      &XCS::set_p_crossover,
-                      "Probability of applying crossover.")
-        .def_property("LAMBDA", &XCS::get_lambda, &XCS::set_lambda,
-                      "Number of offspring to create each EA invocation.")
-        .def_property("ERR_REDUC", &XCS::get_err_reduc, &XCS::set_err_reduc,
-                      "Amount to reduce an offspring's error.")
-        .def_property("FIT_REDUC", &XCS::get_fit_reduc, &XCS::set_fit_reduc,
-                      "Amount to reduce an offspring's fitness.")
-        .def_property("EA_SUBSUMPTION", &XCS::get_ea_subsumption,
-                      &XCS::set_ea_subsumption,
-                      "Whether to try and subsume offspring classifiers.")
-        .def_property("EA_PRED_RESET", &XCS::get_ea_pred_reset,
-                      &XCS::set_ea_pred_reset,
-                      "Whether to reset or copy offspring predictions.")
         .def("time", &XCS::get_time, "Returns the current EA time.")
-        .def("x_dim", &XCS::get_x_dim, "Returns the x_dim.")
-        .def("y_dim", &XCS::get_y_dim, "Returns the y_dim.")
-        .def("n_actions", &XCS::get_n_actions, "Returns the number of actions.")
+        .def("get_metrics", &XCS::get_metrics,
+             "Returns a dictionary of performance metrics.")
         .def("pset_size", &XCS::get_pset_size,
              "Returns the number of macro-classifiers in the population.")
         .def("pset_num", &XCS::get_pset_num,
              "Returns the number of micro-classifiers in the population.")
         .def("pset_mean_cond_size", &XCS::get_pset_mean_cond_size,
              "Returns the average condition size of classifiers in the "
              "population.")
@@ -1619,19 +1101,21 @@
              py::arg("prediction") = true)
         .def("json_write", &XCS::json_write,
              "Writes the current population set to a file in JSON.",
              py::arg("filename"))
         .def("json_read", &XCS::json_read,
              "Reads classifiers from a JSON file and adds to the population.",
              py::arg("filename"))
-        .def("json_parameters", &XCS::json_parameters,
-             "Returns a JSON formatted string representing the parameters.")
+        .def("get_params", &XCS::get_params, py::arg("deep") = true,
+             "Returns a dictionary of parameters and their values.")
+        .def("set_params", &XCS::set_params, "Sets parameters.")
         .def("json_insert_cl", &XCS::json_insert_cl,
              "Creates a classifier from JSON and inserts into the population.",
              py::arg("json_str"))
         .def("json_insert", &XCS::json_insert,
              "Creates classifiers from JSON and inserts into the population.",
              py::arg("json_str"))
+        .def("internal_params", &XCS::internal_params, "Gets internal params.")
         .def(py::pickle(
             [](const XCS &obj) { return obj.serialize(); },
             [](const py::bytes &state) { return XCS::deserialize(state); }));
 }
```

### Comparing `xcsf-1.2.9/xcsf/rule_dgp.c` & `xcsf-1.3.0/xcsf/rule_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/rule_dgp.h` & `xcsf-1.3.0/xcsf/rule_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/rule_neural.c` & `xcsf-1.3.0/xcsf/rule_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/rule_neural.h` & `xcsf-1.3.0/xcsf/rule_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/sam.c` & `xcsf-1.3.0/xcsf/sam.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/sam.h` & `xcsf-1.3.0/xcsf/sam.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/utils/types.py` & `xcsf-1.3.0/xcsf/utils/types.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/utils/viz.py` & `xcsf-1.3.0/xcsf/utils/viz.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/utils.c` & `xcsf-1.3.0/xcsf/utils.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/utils.h` & `xcsf-1.3.0/xcsf/utils.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,24 @@
  */
 
 /**
  * @file utils.h
  * @author Richard Preen <rpreen@gmail.com>
  * @author David Pätzel
  * @copyright The Authors.
- * @date 2015--2022.
+ * @date 2015--2023.
  * @brief Utility functions for random number handling, etc.
  */
 
 #pragma once
 
 #include "../lib/cJSON/cJSON.h"
 #include "../lib/dSFMT/dSFMT.h"
 #include <math.h>
+#include <stdbool.h>
 #include <stdio.h>
 #include <stdlib.h>
 
 double
 rand_normal(const double mu, const double sigma);
 
 double
@@ -133,7 +134,26 @@
 catch_error(const char *ret)
 {
     if (ret != NULL) {
         printf("%s\n", ret);
         exit(EXIT_FAILURE);
     }
 }
+
+/**
+ * @brief Checks whether two double arrays are approximately equal.
+ * @param [in] arr1 Array.
+ * @param [in] arr2 Array.
+ * @param [in] size Length of the arrays.
+ * @return Whether the arrays are equal.
+ */
+static inline bool
+check_array_eq(const double *arr1, const double *arr2, int size)
+{
+    const double tol = 1e-5;
+    for (int i = 0; i < size; ++i) {
+        if (arr1[i] < arr2[i] - tol || arr1[i] > arr2[i] + tol) {
+            return false;
+        }
+    }
+    return true;
+}
```

### Comparing `xcsf-1.2.9/xcsf/xcs_rl.c` & `xcsf-1.3.0/xcsf/xcs_rl.c`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,14 @@
 /**
  * @brief Initialises a reinforcement learning trial.
  * @param [in] xcsf The XCSF data structure.
  */
 void
 xcs_rl_init_trial(struct XCSF *xcsf)
 {
-    if (xcsf->time == 0) {
-        clset_pset_init(xcsf);
-    }
     xcsf->prev_reward = 0;
     xcsf->prev_pred = 0;
     if (xcsf->x_dim < 1) { // memory allocation guard
         printf("xcs_rl_init_trial(): error x_dim less than 1\n");
         xcsf->x_dim = 1;
         exit(EXIT_FAILURE);
     }
```

### Comparing `xcsf-1.2.9/xcsf/xcs_rl.h` & `xcsf-1.3.0/xcsf/xcs_rl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.9/xcsf/xcs_supervised.c` & `xcsf-1.3.0/xcsf/xcs_supervised.c`

 * *Files 1% similar despite different names*

```diff
@@ -87,27 +87,26 @@
 /**
  * @brief Executes MAX_TRIALS number of XCSF learning iterations using the
  * training data and test iterations using the test data.
  * @param [in] xcsf The XCSF data structure.
  * @param [in] train_data The input data to use for training.
  * @param [in] test_data The input data to use for testing.
  * @param [in] shuffle Whether to randomise the instances during training.
+ * @param [in] trials Number of trials to execute.
  * @return The average XCSF training error using the loss function.
  */
 double
 xcs_supervised_fit(struct XCSF *xcsf, const struct Input *train_data,
-                   const struct Input *test_data, const bool shuffle)
+                   const struct Input *test_data, const bool shuffle,
+                   const int trials)
 {
-    if (xcsf->time == 0) {
-        clset_pset_init(xcsf);
-    }
     double err = 0; // training error: total over all trials
     double werr = 0; // training error: windowed total
     double wterr = 0; // testing error: windowed total
-    for (int cnt = 0; cnt < xcsf->MAX_TRIALS; ++cnt) {
+    for (int cnt = 0; cnt < trials; ++cnt) {
         // training sample
         int row = xcs_supervised_sample(train_data, cnt, shuffle);
         const double *x = &train_data->x[row * train_data->x_dim];
         const double *y = &train_data->y[row * train_data->y_dim];
         param_set_explore(xcsf, true);
         xcs_supervised_trial(xcsf, x, y, NULL);
         const double error = (xcsf->loss_ptr)(xcsf, xcsf->pa, y);
@@ -121,15 +120,15 @@
             y = &test_data->y[row * test_data->y_dim];
             param_set_explore(xcsf, false);
             xcs_supervised_trial(xcsf, x, y, NULL);
             wterr += (xcsf->loss_ptr)(xcsf, xcsf->pa, y);
         }
         perf_print(xcsf, &werr, &wterr, cnt);
     }
-    return err / xcsf->MAX_TRIALS;
+    return err / trials;
 }
 
 /**
  * @brief Calculates the XCSF predictions for the provided input.
  * @param [in] xcsf The XCSF data structure.
  * @param [in] x The input feature variables.
  * @param [out] pred The calculated XCSF predictions.
```

### Comparing `xcsf-1.2.9/xcsf/xcs_supervised.h` & `xcsf-1.3.0/xcsf/xcs_supervised.h`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 #pragma once
 
 #include "xcsf.h"
 
 double
 xcs_supervised_fit(struct XCSF *xcsf, const struct Input *train_data,
-                   const struct Input *test_data, const bool shuffle);
+                   const struct Input *test_data, const bool shuffle,
+                   const int trials);
 
 double
 xcs_supervised_score(struct XCSF *xcsf, const struct Input *data,
                      const double *cover);
 
 double
 xcs_supervised_score_n(struct XCSF *xcsf, const struct Input *data, const int N,
```

### Comparing `xcsf-1.2.9/xcsf/xcsf.c` & `xcsf-1.3.0/xcsf/xcsf.c`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     xcsf->error = xcsf->E0;
     xcsf->mset_size = 0;
     xcsf->aset_size = 0;
     xcsf->mfrac = 0;
     clset_init(&xcsf->pset);
     clset_init(&xcsf->prev_pset);
     pa_init(xcsf);
+    clset_pset_init(xcsf);
 }
 
 /**
  * @brief Frees XCSF population sets.
  * @param [in] xcsf The XCSF data structure.
  */
 void
@@ -56,14 +57,15 @@
     xcsf->time = 0;
     xcsf->error = xcsf->E0;
     xcsf->mset_size = 0;
     xcsf->aset_size = 0;
     xcsf->mfrac = 0;
     clset_kill(xcsf, &xcsf->pset);
     clset_kill(xcsf, &xcsf->prev_pset);
+    pa_free(xcsf);
 }
 
 /**
  * @brief Prints the current XCSF population.
  * @param [in] xcsf The XCSF data structure.
  * @param [in] print_cond Whether to print condition structures.
  * @param [in] print_act Whether to print action structures.
```

### Comparing `xcsf-1.2.9/xcsf/xcsf.h` & `xcsf-1.3.0/xcsf/xcsf.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 #include <stdbool.h>
 #include <stdint.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
 static const int VERSION_MAJOR = 1; //!< XCSF major version number
-static const int VERSION_MINOR = 2; //!< XCSF minor version number
-static const int VERSION_BUILD = 9; //!< XCSF build version number
+static const int VERSION_MINOR = 3; //!< XCSF minor version number
+static const int VERSION_BUILD = 0; //!< XCSF build version number
 
 /**
  * @brief Classifier data structure.
  */
 struct Cl {
     struct CondVtbl const *cond_vptr; //!< Functions acting on conditions
     struct PredVtbl const *pred_vptr; //!< Functions acting on predictions
@@ -100,14 +100,15 @@
     double aset_size; //!< Average action set size
     double mfrac; //!< Generalisation measure
     double prev_reward; //!< Reward from previous step in a multi-step trial
     double prev_pred; //!< Payoff prediction made on the previous step
     double *pa; //!< Prediction array (stores fitness weighted predictions)
     double *nr; //!< Prediction array (stores total fitness)
     double *prev_state; //!< Environment state on the previous step
+    double *cover; //!< Values to return for a prediction instead of covering
     int time; //!< Current number of EA executions
     int pa_size; //!< Prediction array size
     int x_dim; //!< Number of problem input variables
     int y_dim; //!< Number of problem output variables
     int n_actions; //!< Number of class labels / actions
     bool explore; //!< Whether the system is currently exploring or exploiting
     double (*loss_ptr)(const struct XCSF *, const double *,
@@ -127,18 +128,20 @@
     int PERF_TRIALS; //!< Number of problem instances to avg performance output
     int POP_SIZE; //!< Maximum number of micro-classifiers in the population
     int LOSS_FUNC; //!< Which loss/error function to apply
     int TELETRANSPORTATION; //!< Maximum steps for a multi-step problem
     int THETA_DEL; //!< Min experience before fitness used during deletion
     int M_PROBATION; //!< Trials since creation a cl must match at least 1 input
     int THETA_SUB; //!< Minimum experience of a classifier to become a subsumer
+    int RANDOM_STATE; //!< Random number seed
     bool POP_INIT; //!< Pop initially empty or filled with random conditions
     bool SET_SUBSUMPTION; //!< Whether to perform match set subsumption
     bool STATEFUL; //!< Whether classifiers should retain state across trials
     bool COMPACTION; //!< if sys err < E0: largest of 2 roulette spins deleted
+    char *population_file; //!< Name of a JSON file containing an initial pop
 };
 
 /**
  * @brief Input data structure.
  */
 struct Input {
     double *x; //!< Feature variables
```

### Comparing `xcsf-1.2.9/xcsf.egg-info/PKG-INFO` & `xcsf-1.3.0/xcsf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.2.9
+Version: 1.3.0
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.2.9/xcsf.egg-info/SOURCES.txt` & `xcsf-1.3.0/xcsf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -588,14 +588,18 @@
 xcsf/pred_neural.h
 xcsf/pred_nlms.c
 xcsf/pred_nlms.h
 xcsf/pred_rls.c
 xcsf/pred_rls.h
 xcsf/prediction.c
 xcsf/prediction.h
+xcsf/pybind_callback.h
+xcsf/pybind_callback_checkpoint.h
+xcsf/pybind_callback_earlystop.h
+xcsf/pybind_utils.h
 xcsf/pybind_wrapper.cpp
 xcsf/rule_dgp.c
 xcsf/rule_dgp.h
 xcsf/rule_neural.c
 xcsf/rule_neural.h
 xcsf/sam.c
 xcsf/sam.h
```

