# Comparing `tmp/syntaxlight-0.0.2.tar.gz` & `tmp/syntaxlight-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.2.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.3.tar", max compression
```

## Comparing `syntaxlight-0.0.2.tar` & `syntaxlight-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.2/LICENSE
--rw-r--r--   0        0        0      464 2023-07-20 06:46:11.144892 syntaxlight-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-07-19 08:50:34.683953 syntaxlight-0.0.2/README.md
--rw-r--r--   0        0        0      191 2023-07-19 07:19:43.518938 syntaxlight-0.0.2/syntaxlight/__init__.py
--rw-r--r--   0        0        0    13872 2023-07-19 09:12:22.898053 syntaxlight-0.0.2/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.2/syntaxlight/css/all.css
--rw-r--r--   0        0        0     2081 2023-07-19 08:12:53.632477 syntaxlight-0.0.2/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.2/syntaxlight/css/index.css
--rw-r--r--   0        0        0      485 2023-07-19 08:11:30.544637 syntaxlight-0.0.2/syntaxlight/css/json.css
--rw-r--r--   0        0        0     2551 2023-07-19 08:24:17.554978 syntaxlight-0.0.2/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.2/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.2/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.2/syntaxlight/error.py
--rw-r--r--   0        0        0     1810 2023-07-20 06:43:05.238275 syntaxlight-0.0.2/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.2/syntaxlight/export.py
--rw-r--r--   0        0        0      406 2023-07-12 03:19:24.095469 syntaxlight-0.0.2/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0    12379 2023-07-19 02:03:36.729775 syntaxlight-0.0.2/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     2219 2023-07-04 09:22:19.741835 syntaxlight-0.0.2/syntaxlight/lexers/ebnf_lexer.py
--rw-r--r--   0        0        0     1864 2023-07-04 09:20:59.243201 syntaxlight-0.0.2/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    19627 2023-07-19 02:25:52.820410 syntaxlight-0.0.2/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.2/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.2/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3538 2023-07-06 06:05:23.042009 syntaxlight-0.0.2/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4578 2023-07-11 14:54:57.917125 syntaxlight-0.0.2/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      205 2023-07-12 06:09:50.252799 syntaxlight-0.0.2/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0   100635 2023-07-19 06:32:03.955082 syntaxlight-0.0.2/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0      989 2023-07-04 09:23:16.797987 syntaxlight-0.0.2/syntaxlight/parsers/ebnf_parser.py
--rw-r--r--   0        0        0     5758 2023-07-10 15:27:05.012220 syntaxlight-0.0.2/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0     8881 2023-07-18 14:16:16.403941 syntaxlight-0.0.2/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.2/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11786 2023-07-16 15:52:23.224969 syntaxlight-0.0.2/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-15 15:57:39.737127 syntaxlight-0.0.2/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     3784 2023-07-19 09:11:40.206441 syntaxlight-0.0.2/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.2/syntaxlight/template.html
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 syntaxlight-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.3/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-20 10:03:28.191668 syntaxlight-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1632 2023-07-20 09:56:07.920078 syntaxlight-0.0.3/README.md
+-rw-r--r--   0        0        0      191 2023-07-19 07:19:43.518938 syntaxlight-0.0.3/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    13864 2023-07-20 09:35:37.730553 syntaxlight-0.0.3/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.3/syntaxlight/css/all.css
+-rw-r--r--   0        0        0     2081 2023-07-19 08:12:53.632477 syntaxlight-0.0.3/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.3/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      485 2023-07-19 08:11:30.544637 syntaxlight-0.0.3/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.3/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.3/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.3/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.3/syntaxlight/error.py
+-rw-r--r--   0        0        0     1995 2023-07-20 08:23:56.191983 syntaxlight-0.0.3/syntaxlight/example.py
+-rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.3/syntaxlight/export.py
+-rw-r--r--   0        0        0      406 2023-07-12 03:19:24.095469 syntaxlight-0.0.3/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0    12379 2023-07-19 02:03:36.729775 syntaxlight-0.0.3/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     2219 2023-07-04 09:22:19.741835 syntaxlight-0.0.3/syntaxlight/lexers/ebnf_lexer.py
+-rw-r--r--   0        0        0     1864 2023-07-04 09:20:59.243201 syntaxlight-0.0.3/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    19627 2023-07-19 02:25:52.820410 syntaxlight-0.0.3/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.3/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.3/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3538 2023-07-06 06:05:23.042009 syntaxlight-0.0.3/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4578 2023-07-11 14:54:57.917125 syntaxlight-0.0.3/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      205 2023-07-12 06:09:50.252799 syntaxlight-0.0.3/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0   100655 2023-07-20 10:00:41.507850 syntaxlight-0.0.3/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0      989 2023-07-04 09:23:16.797987 syntaxlight-0.0.3/syntaxlight/parsers/ebnf_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-10 15:27:05.012220 syntaxlight-0.0.3/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0     8883 2023-07-20 08:24:16.172052 syntaxlight-0.0.3/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.3/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11786 2023-07-16 15:52:23.224969 syntaxlight-0.0.3/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-15 15:57:39.737127 syntaxlight-0.0.3/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     3835 2023-07-20 09:36:05.046073 syntaxlight-0.0.3/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.3/syntaxlight/template.html
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 syntaxlight-0.0.3/PKG-INFO
```

### Comparing `syntaxlight-0.0.2/LICENSE` & `syntaxlight-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/README.md` & `syntaxlight-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 ## 快速开始
 
 syntaxlight 提供了一个简易的 API 用于预览结果: `syntaxlight.example_display`
 
 ```python
 import syntaxlight
 
-syntaxlight.example_display('./test/c/2.c')
+syntaxlight.example_display('./1.c')
 
 # syntaxlight.example_display('./your-code.c', style='one-dark-pro')
 ```
 
-运行可以得到 `syntaxlight_example/` 文件夹, 使用浏览器打开其中的 index.html 即可预览
+运行可以得到 `syntaxlight_example/` 文件夹, 使用浏览器打开其中的 index.html 即可预览. 同时会生成解析得到的抽象语法树 ast.dot, Vscode 用户可以下载 [graphviz-interactive-preview](https://marketplace.visualstudio.com/items?itemName=tintinweb.graphviz-interactive-preview) 插件预览, 或者安装 [graphviz](https://graphviz.org/) 之后使用下面的命令导出 png
+
+```bash
+dot -Tpng ./ast.dot -o ast.png
+```
 
 ## 文档和 API
 
 关于详细的 API 使用方法, 以及对于默认配置的修改情况请参阅 [syntaxlight 使用文档](https://luzhixing12345.github.io/syntaxlight/)
 
 ## 参考
```

### Comparing `syntaxlight-0.0.2/syntaxlight/ast.py` & `syntaxlight-0.0.3/syntaxlight/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,19 @@
         """
         node_visitor.depth -= 1  # 到达叶节点, 退出到上一层
         # print(f'visit {self.class_name}, depth = {self.depth}')
 
     def formatter(self, depth: int = 0):
         raise NotImplementedError(self.class_name + " should override format function to display")
 
-    # def __str__(self) -> str:
-    #     return self.formatter()
+    def __str__(self) -> str:
+        return self.formatter()
 
-    # def __repr__(self) -> str:
-    #     return self.__str__()
+    def __repr__(self) -> str:
+        return self.__str__()
 
     def get_node_info(self):
         # f'depth={self.depth}\\n'
         node_content = self._node_info + "\\n" + f"depth={self.depth}"
         return f'node{self.created_index} [label="{node_content}"]'
```

### Comparing `syntaxlight-0.0.2/syntaxlight/css/all.css` & `syntaxlight-0.0.3/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/css/c.css` & `syntaxlight-0.0.3/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/css/index.css` & `syntaxlight-0.0.3/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/css/themes.json` & `syntaxlight-0.0.3/syntaxlight/css/themes.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984567901234568%*

 * *Differences: {"'monokai'": "{'extension': {'c': OrderedDict([('.Token.Typedefine', 'border-bottom: 1px solid "*

 * *              "--struct;'), ('.Token.StorageType', 'color: --define')])}}"}*

```diff
@@ -14,14 +14,18 @@
         "--operator": "#F92672",
         "--punctuator": "#F8F8F2",
         "--string": "#E6D663",
         "--struct": "#7ED92E",
         "--type": "#66D9EF",
         "--variant": "#F8F8F2",
         "extension": {
+            "c": {
+                ".Token.StorageType": "color: --define",
+                ".Token.Typedefine": "border-bottom: 1px solid --struct;"
+            },
             "json": {
                 ".Token.Pair.Key": "color: --type; font-style: italic;"
             },
             "toml": {
                 ".Token.TableArrayHeader.Path": "color: --struct;",
                 ".Token.TableHeader.Path": "color: --struct;"
             }
```

### Comparing `syntaxlight-0.0.2/syntaxlight/css/toml.css` & `syntaxlight-0.0.3/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/error.py` & `syntaxlight-0.0.3/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/example.py` & `syntaxlight-0.0.3/syntaxlight/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from .syntax_parse import parse_file, guess_language
 import os
 import shutil
 from .export import export_css
 from typing import Union, List
 
-def example_display(file_path: Union[str,List[str]] = None, language: str = "guess", style="vscode"):
+
+def example_display(
+    file_path: Union[str, List[str]] = None,
+    style="vscode",
+    save_ast_tree=True,
+    language: str = "guess",
+):
     example_folder_name = os.path.join(os.getcwd(), "syntaxlight_example")
     if language == "guess":
-        language = guess_language(file_path)
+        if type(file_path) == list:
+            language = guess_language(file_path[0])
+        else:
+            language = guess_language(file_path)
 
     syntaxlight_path = os.path.dirname(__file__)
     html_template_file = os.path.join(syntaxlight_path, "template.html")
     index_css_file = os.path.join(syntaxlight_path, "css", "index.css")
     css_files = [index_css_file]
     css_scope = f"<link rel='stylesheet' href='./{language}.css' />"
 
@@ -21,15 +30,15 @@
         os.mkdir(example_folder_name)
 
     if type(file_path) == str:
         file_path = [file_path]
 
     code_html = ""
     for fp in file_path:
-        html = parse_file(fp, language)
+        html = parse_file(fp, language, save_ast_tree=save_ast_tree)
         if html is None:
             continue
         code_html += f'<pre class="language-{language}"><code>{html}</code></pre>'
 
     code_html = f'<div class="markdown-body">{code_html}</div>'
     with open(html_template_file, "r", encoding="utf-8") as f:
         content = f.read().replace("html-scope", code_html).replace("css-scope", css_scope)
```

### Comparing `syntaxlight-0.0.2/syntaxlight/export.py` & `syntaxlight-0.0.3/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/ebnf_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/ebnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.3/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/c_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,21 +601,23 @@
     def __init__(self) -> None:
         super().__init__()
         self.keyword = None
         self.id: Identifier = None
         self.paramters = None
         self.parameterization = None
         self.pp_tokens = None
+        self.group = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.keyword)
         node_visitor.link(self, self.id)
         node_visitor.link(self, self.paramters)
         node_visitor.link(self, self.parameterization)
         node_visitor.link(self, self.pp_tokens)
+        node_visitor.link(self, self.group)
         return super().visit(node_visitor)
 
 
 class HeaderName(AST):
     def __init__(self) -> None:
         super().__init__()
         self.file_path = None
@@ -639,15 +641,14 @@
         super().__init__(lexer, skip_invisible_characters, skip_space)
         self.cfirst_set = CTokenSet()
         self.in_preprocessing = False  # 进入预处理阶段, 影响 after_eat
         self.preprocessing_keywords = [
             "ifdef",
             "ifndef",
             "elif",
-            "else",  # 预处理命令中的 else,
             "endif",
             "include",
             "define",
             "undef",
             "line",
             "error",
             "pragma",
```

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/ebnf_parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/ebnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..ast import AST
 from typing import List
 import sys
 import html
 import traceback
 
 DEBUG = False
-DEBUG = True
+# DEBUG = True
 
 
 class Parser:
     def __init__(
         self, lexer, skip_invisible_characters=True, skip_space=True, display_warning=True
     ):
         self.lexer: Lexer = lexer
```

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.3/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.2/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.3/syntaxlight/syntax_parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     lexer = get_lexer(text, language)
     if file_path is not None:
         lexer.file_path = file_path
     parser = get_parser(lexer)
 
     try:
         parser.parse()
-        # display_ast(parser.node)
     except Error as e:
         sys.stderr.write(e.message)
         if show_error_context:
             sys.stderr.write(e.context)
     else:
         display_ast(parser.node, save_ast_tree = save_ast_tree)
+        # print(parser.node)
         return parser.to_html()
 
 
 def parse_file(
     file_path: str, language: str = "guess", show_error_context=True, save_ast_tree=False
 ) -> str:
     if not os.path.exists(file_path):
@@ -52,14 +52,17 @@
         file_path=file_path,
         show_error_context=show_error_context,
         save_ast_tree=save_ast_tree,
     )
 
 
 def guess_language(file_path: str) -> str:
+    '''
+    通过文件名猜测文法类型
+    '''
     file_name = file_path.split(os.sep)[-1]
 
     languages = {
         "json": ["json"],
         "c": ["c", "h"],
         "lua": ["lua"],
         "bnf": ["bnf"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syntaxlight-0.0.2/PKG-INFO` & `syntaxlight-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.2
+Version: 0.0.3
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,20 +32,24 @@
 ## 快速开始
 
 syntaxlight 提供了一个简易的 API 用于预览结果: `syntaxlight.example_display`
 
 ```python
 import syntaxlight
 
-syntaxlight.example_display('./test/c/2.c')
+syntaxlight.example_display('./1.c')
 
 # syntaxlight.example_display('./your-code.c', style='one-dark-pro')
 ```
 
-运行可以得到 `syntaxlight_example/` 文件夹, 使用浏览器打开其中的 index.html 即可预览
+运行可以得到 `syntaxlight_example/` 文件夹, 使用浏览器打开其中的 index.html 即可预览. 同时会生成解析得到的抽象语法树 ast.dot, Vscode 用户可以下载 [graphviz-interactive-preview](https://marketplace.visualstudio.com/items?itemName=tintinweb.graphviz-interactive-preview) 插件预览, 或者安装 [graphviz](https://graphviz.org/) 之后使用下面的命令导出 png
+
+```bash
+dot -Tpng ./ast.dot -o ast.png
+```
 
 ## 文档和 API
 
 关于详细的 API 使用方法, 以及对于默认配置的修改情况请参阅 [syntaxlight 使用文档](https://luzhixing12345.github.io/syntaxlight/)
 
 ## 参考
```

