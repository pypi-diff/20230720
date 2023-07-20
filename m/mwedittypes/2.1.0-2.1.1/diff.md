# Comparing `tmp/mwedittypes-2.1.0.tar.gz` & `tmp/mwedittypes-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edit-types/edit-types/dist/.tmp-ujfntg0j/mwedittypes-2.1.0.tar", last modified: Thu Jul 13 18:59:14 2023, max compression
+gzip compressed data, was "/home/runner/work/edit-types/edit-types/dist/.tmp-__nkrvck/mwedittypes-2.1.1.tar", last modified: Thu Jul 20 19:19:47 2023, max compression
```

## Comparing `mwedittypes-2.1.0.tar` & `mwedittypes-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25376 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/mwedittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/node_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/simple_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32230 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/tree_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_edittypes_structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_edittypes_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_tree_differ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/mwedittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/node_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/simple_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33357 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/tree_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/mwedittypes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/mwedittypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:19:47.000000 mwedittypes-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/tests/test_edittypes_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/tests/test_edittypes_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-20 19:19:36.000000 mwedittypes-2.1.1/tests/test_tree_differ.py
```

### Comparing `mwedittypes-2.1.0/LICENSE` & `mwedittypes-2.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `mwedittypes-2.1.0/PKG-INFO` & `mwedittypes-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwedittypes
-Version: 2.1.0
+Version: 2.1.1
 Summary: Edit diffs and type detection for Wikipedia
 Home-page: https://github.com/geohci/edit-types
 Author: geohci & Amamgbu (Isaac Johnson & Jesse Amamgbu)
 Author-email: <amamgbujesse@yahoo.com>
 License: MIT License
 Keywords: python,wikipedia,edit types,edit diffs,wiki,edit detection
 Classifier: Development Status :: 4 - Beta
@@ -84,29 +84,29 @@
                          changes=[('parameter', ('1', 'Austrian painter'), ('1', 'Austrian [[landscape painter]]'))])],
  'text-edits': []}
 ```
 
 In most cases (~90%), the two approaches agree in their overall results. They differ in the following situations:
 * Very large diffs -- when `timeout` is set to `True`, the StructuredEditTypes class is more likely to fall-back to a simple diff and miss some details as a result
 * Content moves -- the simplified library cannot detect moves
-* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted 
+* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted
 
 A good example of a diff where they vary in outputs is revision 1107840666 on English Wikipedia ([diff](https://en.wikipedia.org/w/index.php?diff=1107840666&oldid=1094519551&title=Blumenthal,_Saskatchewan&diffmode=source); [model output](https://wiki-topic.toolforge.org/diff-tagging?lang=en&revid=1107840666)).
 
 ## Language Coverage
 Almost everything in this library is language-agnostic and so works consistently for any language of Wikipedia.
 For links, the namespace identification varies but we use a list of prefixes that covers all languages (at the time of generation).
 Sentences are semi-challenging in that we must build a list of sentence-ending punctuation that covers all languages. We believe we have done a good job of this but have not explicitly tested this. The list can be found in `mwedittypes/constants.py` under `SENTENCE_BREAKS_REGEX`.
 Words are the most challenging aspect and the one place where you will see varying behavior. For them we take two strategies:
 * For most languages, we split text based on whitespace. This is the default behavior.
 * There are many languages that either don't separate words with whitespace or use whitespace to instead delineate syllables. These can be found in `mwedittypes/constants.py` under `NON_WHITESPACE_LANGUAGES`. For these languages, we instead report the number of characters affected.
 
 ## Known Issues
 Wikitext/language is verrrrrrry complicated and so there are certain things we can't feasibly extract consistently. The ones we know about:
-* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence. 
+* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence.
 * Words: we have done our best to extract words for whitespace-delimited languages but some languages use special spacing characters that may falsely split up words -- e.g., Bengali. We have done our best to detect account for these languages but may have missed some.
 * Media: images/audio/video can be included in articles via bracketed links, templates, and galleries. Each have their own syntax, and, in particular templates separate the image name from its formatting options. For galleries/bracket-links, we associate the formatting/caption options with the media and changes to them will trigger as media changes. For templates, we cannot do this.
 * Text Formatting: parsing text formatting is quite complicated and context-dependent. We parse the wikitext section-by-section so text formatting split up between sections might parse unexpectedly.
 
 For links, we assume that if the prefix is not for media or a category, the link is a wikilink to namespace 0. This is generally reasonable for current versions of Wikipedia articles
 but would overload the `Wikilink` class with e.g., user page links on talk pages or interwiki links for older versions of articles.
 
@@ -152,8 +152,7 @@
 * If something fails, you can always rollback the release (Github UI) and delete the associated tag (on your local repository: `git tag -d [tag]; git push origin :[tag]`) and retry.
 * This relies on a PyPi secret so you must have correct privileges on the Github repo.
 
 ## Documentation
 * For more background, see: https://meta.wikimedia.org/wiki/Research:Wikipedia_Edit_Types
 * To test out the code, see: https://wiki-topic.toolforge.org/diff-tagging?lang=en
 * To see how the code is used in an API, see: https://github.com/wikimedia/research-api-endpoint-template/tree/edit-types
-
```

### Comparing `mwedittypes-2.1.0/README.md` & `mwedittypes-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
                          changes=[('parameter', ('1', 'Austrian painter'), ('1', 'Austrian [[landscape painter]]'))])],
  'text-edits': []}
 ```
 
 In most cases (~90%), the two approaches agree in their overall results. They differ in the following situations:
 * Very large diffs -- when `timeout` is set to `True`, the StructuredEditTypes class is more likely to fall-back to a simple diff and miss some details as a result
 * Content moves -- the simplified library cannot detect moves
-* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted 
+* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted
 
 A good example of a diff where they vary in outputs is revision 1107840666 on English Wikipedia ([diff](https://en.wikipedia.org/w/index.php?diff=1107840666&oldid=1094519551&title=Blumenthal,_Saskatchewan&diffmode=source); [model output](https://wiki-topic.toolforge.org/diff-tagging?lang=en&revid=1107840666)).
 
 ## Language Coverage
 Almost everything in this library is language-agnostic and so works consistently for any language of Wikipedia.
 For links, the namespace identification varies but we use a list of prefixes that covers all languages (at the time of generation).
 Sentences are semi-challenging in that we must build a list of sentence-ending punctuation that covers all languages. We believe we have done a good job of this but have not explicitly tested this. The list can be found in `mwedittypes/constants.py` under `SENTENCE_BREAKS_REGEX`.
 Words are the most challenging aspect and the one place where you will see varying behavior. For them we take two strategies:
 * For most languages, we split text based on whitespace. This is the default behavior.
 * There are many languages that either don't separate words with whitespace or use whitespace to instead delineate syllables. These can be found in `mwedittypes/constants.py` under `NON_WHITESPACE_LANGUAGES`. For these languages, we instead report the number of characters affected.
 
 ## Known Issues
 Wikitext/language is verrrrrrry complicated and so there are certain things we can't feasibly extract consistently. The ones we know about:
-* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence. 
+* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence.
 * Words: we have done our best to extract words for whitespace-delimited languages but some languages use special spacing characters that may falsely split up words -- e.g., Bengali. We have done our best to detect account for these languages but may have missed some.
 * Media: images/audio/video can be included in articles via bracketed links, templates, and galleries. Each have their own syntax, and, in particular templates separate the image name from its formatting options. For galleries/bracket-links, we associate the formatting/caption options with the media and changes to them will trigger as media changes. For templates, we cannot do this.
 * Text Formatting: parsing text formatting is quite complicated and context-dependent. We parse the wikitext section-by-section so text formatting split up between sections might parse unexpectedly.
 
 For links, we assume that if the prefix is not for media or a category, the link is a wikilink to namespace 0. This is generally reasonable for current versions of Wikipedia articles
 but would overload the `Wikilink` class with e.g., user page links on talk pages or interwiki links for older versions of articles.
 
@@ -126,8 +126,7 @@
 * If something fails, you can always rollback the release (Github UI) and delete the associated tag (on your local repository: `git tag -d [tag]; git push origin :[tag]`) and retry.
 * This relies on a PyPi secret so you must have correct privileges on the Github repo.
 
 ## Documentation
 * For more background, see: https://meta.wikimedia.org/wiki/Research:Wikipedia_Edit_Types
 * To test out the code, see: https://wiki-topic.toolforge.org/diff-tagging?lang=en
 * To see how the code is used in an API, see: https://github.com/wikimedia/research-api-endpoint-template/tree/edit-types
-
```

### Comparing `mwedittypes-2.1.0/mwedittypes/constants.py` & `mwedittypes-2.1.1/mwedittypes/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,55 @@
 from mwconstants.constants.c_media import MEDIA_EXTENSIONS
 
 # https://en.wikipedia.org/wiki/Help:Wikitext
 # bold, italic, strikethrough, underline
 # horizontal rule and line break (hr is not really text formatting but close enough)
 # pre and nowiki are for mono-spaced text (I leave out `code` because it generally contains code not text)
 # small / big / sub / sup all affect text size
-TEXT_FORMATTING_TAGS = ('b', 'i', 's', 'u', 'del', 'ins','hr', 'br','pre', 'nowiki','small',
-                         'big', 'sub', 'sup', 'font', 'blockquote', 'span', 'center')
-TABLE_ELEMENTS_TAGS = ('th', 'tr', 'td')
-LIST_TAGS = ('li', 'dt', 'dd', 'ul', 'ol', 'dl')
+TEXT_FORMATTING_TAGS = (
+    "b",
+    "i",
+    "s",
+    "u",
+    "del",
+    "ins",
+    "hr",
+    "br",
+    "pre",
+    "nowiki",
+    "small",
+    "big",
+    "sub",
+    "sup",
+    "font",
+    "blockquote",
+    "span",
+    "center",
+)
+TABLE_ELEMENTS_TAGS = ("th", "tr", "td")
+LIST_TAGS = ("li", "dt", "dd", "ul", "ol", "dl")
 
 # CJK period/question/exclamation; Bengali full-stops; Armenian verǰaket (full-stop; resembles a colon)
-NON_ENGLISH_FULL_STOPS = '。？！।॥։'
+NON_ENGLISH_FULL_STOPS = "。？！।॥։"
 # This regex identifies end-of-sentence punctuation and new-lines as sentence breaks
 # It avoids matching dots between two digits but takes into account ellipses and fullstops.
 # fuller explanation:
 # [!?...] - 1 or more !, ?, new-line, or non-english stops
 # | - or
 # (?<!\.) - next character must not precede a fullstop
 # \. - next character
 # (?<=\d.) - must be preceded by a digit containing a fullstop
 # (?!(?<=\d.)\d) -  next character must not be followed by matching dots between two digits
 # (?!\.) - next character must not be followed by fullstop
-SENTENCE_BREAKS_REGEX = r'[!?\n{0}]+|(?<!\.)\.(?!(?<=\d.)\d)(?!\.)'.format(NON_ENGLISH_FULL_STOPS)
+SENTENCE_BREAKS_REGEX = r"[!?\n{0}]+|(?<!\.)\.(?!(?<=\d.)\d)(?!\.)".format(
+    NON_ENGLISH_FULL_STOPS
+)
 
 # TODO non-English quotation marks -- e.g., German
-NON_ENGLISH_UNICODE = '''[\u0609\u060a\u060c\u060d\u061b\u061e\u061f\u066a\u066b\u066c
+NON_ENGLISH_UNICODE = """[\u0609\u060a\u060c\u060d\u061b\u061e\u061f\u066a\u066b\u066c
 \u070a\u070b\u070c\u070d\u07f7\u07f8\u07f9\u0830\u0831\u0832\u0833\u0834\u0835
 \u0836\u0837\u0838\u0839\u083a\u083b\u083c\u083d\u083e\u085e\u0964
 \u0965\u0970\u09fd\u0a76\u0af0\u0c77\u0c84\u0df4
 \u0e4f\u0e5a\u0e5b\u0f04\u0f05\u0f06\u0f07\u0f08\u0f09\u0f0a\u0f0b
 \u0f0c\u0f0d\u0f0e\u0f0f\u0f10\u0f11\u0f12\u0f14\u0f85\u0fd0\u0fd1
 \u0fd2\u0fd3\u0fd4\u0fd9\u0fda\u104a\u104b\u104c\u104d\u104e\u104f
 \u10fb\u1360\u1361\u1362\u1363\u1364\u1365\u1366\u1367\u1368\u166e
@@ -42,27 +62,31 @@
 \u1b60\u1bfc\u1bfd\u1bfe\u1bff\u1c3b\u1c3c\u1c3d\u1c3e\u1c3f\u1c7e
 \u1c7f\u1cc0\u1cc1\u1cc2\u1cc3\u1cc4\u1cc5\u1cc6\u1cc7\u1cd3\u2016
 \u2017\u2020\u2021\u2022\u2023\u2025\u2026\u2027\u2030\u2031
 \u2032\u2033\u2034\u2035\u2036\u2037\u2038\u203b\u203c\u203d\u203e
 \u2041\u2042\u2043\u2047\u2048\u2049\u204a\u204b\u204c\u204d\u204e
 \u204f\u2050\u2051\u2053\u2055\u2056\u2057\u2058\u2059\u205a\u205b
 \u205c\u205d\u205e\u2cf9\u2cfa\u2cfb\u2cfc\u2cfe\u2cff
-\u3000-\u303f\uff0c\uff01\uff1f\uff1b\uff1a\uff08\uff3b\u3010\u09E4\u09E5]'''.replace('\n','')
+\u3000-\u303f\uff0c\uff01\uff1f\uff1b\uff1a\uff08\uff3b\u3010\u09E4\u09E5]""".replace(
+    "\n", ""
+)
 
-ENGLISH_UNICODE = '[\u00b7\u00bf]'
+ENGLISH_UNICODE = "[\u00b7\u00bf]"
 
 # build regex that checks for all media extensions
-EXTEN_REGEX = ('(' + '|'.join([e + r'\b' for e in MEDIA_EXTENSIONS]) + ')').replace('.', r'\.')
-# join in the extension regex with one that requiries at least one alphanumeric and/or a few special characters before it
-EXTEN_PATTERN = re.compile(fr'([\w ,().-]+){EXTEN_REGEX}', flags=re.UNICODE)
+EXTEN_REGEX = ("(" + "|".join([e + r"\b" for e in MEDIA_EXTENSIONS]) + ")").replace(
+    ".", r"\."
+)
+# join in the extension regex with one that requires at least one alphanumeric and/or special characters before it
+EXTEN_PATTERN = re.compile(rf"([\w ,().-]+){EXTEN_REGEX}", flags=re.UNICODE)
 
-MEDIA_PREFIXES = ['File', 'Image', 'Media']
-CAT_PREFIXES = ['Category']
+MEDIA_PREFIXES = ["File", "Image", "Media"]
+CAT_PREFIXES = ["Category"]
 
-# Source: for each Wikipedia language code (example shown for "ab"), aliases for namespaces -2 and 6 accessed via this API call:
+# Source: for each Wikipedia language code (ex. shown for "ab"), aliases for namespaces 6 accessed via this API call:
 # https://ab.wikipedia.org/w/api.php?action=query&meta=siteinfo&siprop=namespacealiases|namespaces&format=json&formatversion=2
 # Last accessed: 21 December 2021
 MEDIA_ALIASES = {
     "ab": ["Медиа", "Файл", "Афаил", "Амедиа", "Изображение"],
     "ace": ["Beureukaih", "Gambar", "Alat", "Berkas"],
     "ady": ["Медиа"],
     "af": ["Lêer", "Beeld"],
@@ -265,15 +289,24 @@
     "se": ["Fiila"],
     "sg": ["Média", "Fichier"],
     "sh": ["Mediji", "Slika", "Медија", "Datoteka", "Medija", "Слика"],
     "si": ["රූපය", "මාධ්‍යය", "ගොනුව"],
     "sk": ["Súbor", "Obrázok", "Médiá"],
     "sl": ["Slika", "Datoteka"],
     "sq": ["Figura", "Skeda"],
-    "sr": ["Датотека", "Medij", "Slika", "Медија", "Datoteka", "Медиј", "Medija", "Слика"],
+    "sr": [
+        "Датотека",
+        "Medij",
+        "Slika",
+        "Медија",
+        "Datoteka",
+        "Медиј",
+        "Medija",
+        "Слика",
+    ],
     "srn": ["Afbeelding", "Gefre"],
     "stq": ["Bielde", "Bild"],
     "su": ["Média", "Gambar"],
     "sv": ["Fil", "Bild"],
     "sw": ["Faili", "Picha"],
     "szl": ["Plik", "Grafika"],
     "ta": ["படிமம்", "ஊடகம்"],
@@ -312,15 +345,15 @@
     "zea": ["Afbeelding", "Plaetje"],
     "zh": ["媒体文件", "F", "文件", "媒體", "档案", "图像", "圖像", "媒体", "檔案"],
     "zh-classical": ["文件", "媒體", "圖像", "檔案"],
     "zh-min-nan": ["tóng-àn", "文件", "媒體", "Mûi-thé", "圖像", "檔案"],
     "zh-yue": ["檔", "档", "文件", "图", "媒體", "圖", "档案", "图像", "圖像", "媒体", "檔案"],
 }
 
-# Source: for each Wikipedia language code (example shown for "ab"), aliases for namespace 14 accessed via this API call:
+# Source: for each Wikipedia language code (ex. shown for "ab"), aliases for namespace 14 accessed via this API call:
 # https://ab.wikipedia.org/w/api.php?action=query&meta=siteinfo&siprop=namespacealiases|namespaces&format=json&formatversion=2
 # Last accessed: 21 December 2021
 CAT_ALIASES = {
     "ab": ["Категория", "Акатегориа"],
     "ace": ["Kawan", "Kategori"],
     "af": ["Kategorie"],
     "ak": ["Nkyekyem"],
@@ -437,15 +470,23 @@
     "kl": ["Sumut_atassuseq", "Kategori", "Sumut atassuseq"],
     "km": ["ចំនាត់ថ្នាក់ក្រុម", "ចំណាត់ក្រុម", "ចំណាត់ថ្នាក់ក្រុម"],
     "kn": ["ವರ್ಗ"],
     "ko": ["분류"],
     "koi": ["Категория"],
     "krc": ["Категория"],
     "ks": ["زٲژ"],
-    "ksh": ["Saachjropp", "Saachjrop", "Katejori", "Kategorie", "Saachjrupp", "Kattejori", "Sachjrop"],
+    "ksh": [
+        "Saachjropp",
+        "Saachjrop",
+        "Katejori",
+        "Kategorie",
+        "Saachjrupp",
+        "Kattejori",
+        "Sachjrop",
+    ],
     "ku": ["Kategorî", "پۆل"],
     "kv": ["Категория"],
     "kw": ["Class", "Klass"],
     "ky": ["Категория"],
     "la": ["Categoria"],
     "lad": ["Kateggoría", "Katēggoría", "Categoría"],
     "lb": ["Kategorie"],
@@ -568,8 +609,8 @@
     "yo": ["Ẹ̀ka"],
     "za": ["分类"],
     "zea": ["Categorie"],
     "zh": ["分类", "分類", "CAT"],
     "zh-classical": ["分類", "CAT"],
     "zh-min-nan": ["分類", "Lūi-pia̍t"],
     "zh-yue": ["分类", "分類", "类", "類"],
-}
+}
```

### Comparing `mwedittypes-2.1.0/mwedittypes/node_differ.py` & `mwedittypes-2.1.1/mwedittypes/node_differ.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from collections import namedtuple
+
 import mwparserfromhell as mw
+from mwconstants.media import parse_image_options
 
 from mwedittypes.tokenizer import parse_change_text
-from mwconstants.media import parse_image_options
 
-NodeEdit = namedtuple('NodeEdit', ['type', 'edittype', 'section', 'name', 'changes'])
-TextEdit = namedtuple('TextEdit', ['type', 'edittype', 'text', 'count'])
-Context = namedtuple('Context', ['type', 'edittype', 'count'])
+NodeEdit = namedtuple("NodeEdit", ["type", "edittype", "section", "name", "changes"])
+TextEdit = namedtuple("TextEdit", ["type", "edittype", "text", "count"])
+Context = namedtuple("Context", ["type", "edittype", "count"])
 
 
-def get_node_diff(node_type, prev_wikitext='', curr_wikitext='', lang='en'):
+def get_node_diff(  # noqa: C901
+    node_type, prev_wikitext="", curr_wikitext="", lang="en"
+):
     """Identify fine-grained changes between two wikitext nodes.
 
     Parameters
     ----------
     node_type: str
         Node type -- e.g., Template, Category
     prev_wikitext : str
@@ -27,240 +30,302 @@
     -------
     changes
         List with specific differences between previous and current nodes. Most whitespace changes are ignored.
     """
     name = None
     changes = []
     try:
-        prev_wc = mw.parse(prev_wikitext, skip_style_tags=True).nodes[0] if prev_wikitext else None
-        curr_wc = mw.parse(curr_wikitext, skip_style_tags=True).nodes[0] if curr_wikitext else None
+        prev_wc = (
+            mw.parse(prev_wikitext, skip_style_tags=True).nodes[0]
+            if prev_wikitext
+            else None
+        )
+        curr_wc = (
+            mw.parse(curr_wikitext, skip_style_tags=True).nodes[0]
+            if curr_wikitext
+            else None
+        )
 
-        if node_type == 'Template':
+        if node_type == "Template":
             # separate between name changes and parameter changes
             pt_name = prev_wc.name.strip() if prev_wc else None
             ct_name = curr_wc.name.strip() if curr_wc else None
             name = pt_name if pt_name else ct_name
-            pt_params = {str(p.name).strip(): str(p.value).strip() for p in prev_wc.params} if prev_wc else {}
-            ct_params = {str(p.name).strip(): str(p.value).strip() for p in curr_wc.params} if curr_wc else {}
+            pt_params = (
+                {str(p.name).strip(): str(p.value).strip() for p in prev_wc.params}
+                if prev_wc
+                else {}
+            )
+            ct_params = (
+                {str(p.name).strip(): str(p.value).strip() for p in curr_wc.params}
+                if curr_wc
+                else {}
+            )
             if pt_name != ct_name:
-                changes.append(('name', pt_name, ct_name))
+                changes.append(("name", pt_name, ct_name))
             params = set(pt_params).union(set(ct_params))
             for p in params:
                 if pt_params.get(p) != ct_params.get(p):
-                    changes.append(('parameter',
-                                    (p, pt_params[p]) if p in pt_params else None,
-                                    (p, ct_params[p]) if p in ct_params else None))
+                    changes.append(
+                        (
+                            "parameter",
+                            (p, pt_params[p]) if p in pt_params else None,
+                            (p, ct_params[p]) if p in ct_params else None,
+                        )
+                    )
 
-        elif node_type == 'Media':
+        elif node_type == "Media":
             # Media can be in three different formats:
             # Brackets: [[File:filename.ext|formatting options|caption]]
             # Template: File:filename.ext
             # Gallery: filename.ext|formatting options|caption
-            pm_title, pm_caption, pm_options = parse_image_options(prev_wc if prev_wc else '', lang=lang)
-            cm_title, cm_caption, cm_options = parse_image_options(curr_wc if curr_wc else '', lang=lang)
+            pm_title, pm_caption, pm_options = parse_image_options(
+                prev_wc if prev_wc else "", lang=lang
+            )
+            cm_title, cm_caption, cm_options = parse_image_options(
+                curr_wc if curr_wc else "", lang=lang
+            )
             # remove leading/trailing whitespace as we don't want it affecting perceived changes
             pm_title = pm_title.strip() if pm_title else None
             cm_title = cm_title.strip() if cm_title else None
             name = pm_title if pm_title else cm_title
             if pm_title != cm_title:
-                changes.append(('filename', pm_title, cm_title))
+                changes.append(("filename", pm_title, cm_title))
 
             if pm_caption != cm_caption:
-                changes.append(('caption', pm_caption, cm_caption))
+                changes.append(("caption", pm_caption, cm_caption))
 
             options = set(pm_options).union(set(cm_options))
             for o in options:
                 if o not in pm_options:
-                    changes.append(('option', None, o))
+                    changes.append(("option", None, o))
                 elif o not in cm_options:
-                    changes.append(('option', o, None))
+                    changes.append(("option", o, None))
 
-        elif node_type == 'Category':
+        elif node_type == "Category":
             # identify if category name changes in likely meaningful way
-            prev_cat = prev_wc.title.split(':', maxsplit=1)[1].replace('_', ' ') if prev_wc else None
-            curr_cat = curr_wc.title.split(':', maxsplit=1)[1].replace('_', ' ') if curr_wc else None
+            prev_cat = (
+                prev_wc.title.split(":", maxsplit=1)[1].replace("_", " ")
+                if prev_wc
+                else None
+            )
+            curr_cat = (
+                curr_wc.title.split(":", maxsplit=1)[1].replace("_", " ")
+                if curr_wc
+                else None
+            )
             name = prev_cat if prev_cat else curr_cat
             if prev_cat != curr_cat:
-                changes.append(('title', prev_cat, curr_cat))
+                changes.append(("title", prev_cat, curr_cat))
 
-        elif node_type == 'Wikilink':
+        elif node_type == "Wikilink":
             # separate between title (destination) and text (display) changes
             pl_title = prev_wc.title.strip() if prev_wc and prev_wc.title else None
             cl_title = curr_wc.title.strip() if curr_wc and curr_wc.title else None
             name = pl_title if pl_title else cl_title
             if pl_title != cl_title:
-                changes.append(('title', pl_title, cl_title))
+                changes.append(("title", pl_title, cl_title))
 
             pl_text = prev_wc.text.strip() if prev_wc and prev_wc.text else None
             cl_text = curr_wc.text.strip() if curr_wc and curr_wc.text else None
             if pl_text != cl_text:
-                changes.append(('text', pl_text, cl_text))
+                changes.append(("text", pl_text, cl_text))
 
-        elif node_type == 'Reference':
+        elif node_type == "Reference":
             # Separate between attributes and contents changes
             pr_name = None
             for a in prev_wc.attributes:
-                if a.name == 'name':
+                if a.name == "name":
                     pr_name = a.value.strip()
             cr_name = None
             for a in curr_wc.attributes:
-                if a.name == 'name':
+                if a.name == "name":
                     cr_name = a.value.strip()
             if pr_name != cr_name:
-                changes.append(('name', pr_name, cr_name))
+                changes.append(("name", pr_name, cr_name))
 
             # ref text -- ignoring templates etc.
             pr_text = prev_wc.contents.strip_code().strip() if prev_wc else None
             cr_text = curr_wc.contents.strip_code().strip() if curr_wc else None
             if pr_text != cr_text:
-                changes.append(('text', pr_text, cr_text))
+                changes.append(("text", pr_text, cr_text))
 
             if pr_name:
                 name = pr_name
             elif cr_name:
                 name = cr_name
 
             # heuristic -- check first template too
             try:
                 pr_temp = str(prev_wc.contents.filter_templates(recursive=False)[0])
             except Exception:
-                pr_temp = ''
+                pr_temp = ""
             try:
                 cr_temp = str(curr_wc.contents.filter_templates(recursive=False)[0])
             except Exception:
-                cr_temp = ''
+                cr_temp = ""
 
             if pr_temp != cr_temp:
-                changes.append(('ref-template', pr_temp, cr_temp))
+                changes.append(("ref-template", pr_temp, cr_temp))
 
-        elif node_type == 'Table':
+        elif node_type == "Table":
             # check for attribute changes, header changes, cell changes
-            pt_attrs = {str(a.name).strip(): str(a.value).strip() for a in prev_wc.attributes} if prev_wc else {}
-            ct_attrs = {str(a.name).strip(): str(a.value).strip() for a in curr_wc.attributes} if curr_wc else {}
+            pt_attrs = (
+                {str(a.name).strip(): str(a.value).strip() for a in prev_wc.attributes}
+                if prev_wc
+                else {}
+            )
+            ct_attrs = (
+                {str(a.name).strip(): str(a.value).strip() for a in curr_wc.attributes}
+                if curr_wc
+                else {}
+            )
             attrs = set(pt_attrs).union(set(ct_attrs))
             for a in attrs:
                 if pt_attrs.get(a) != ct_attrs.get(a):
-                    changes.append(('attribute',
-                                    (a, pt_attrs[a]) if a in pt_attrs else None,
-                                    (a, ct_attrs[a]) if a in ct_attrs else None))
+                    changes.append(
+                        (
+                            "attribute",
+                            (a, pt_attrs[a]) if a in pt_attrs else None,
+                            (a, ct_attrs[a]) if a in ct_attrs else None,
+                        )
+                    )
 
             pt_caption = None
             pt_cells = {}
             if prev_wc:
                 for te in mw.parse(prev_wikitext, skip_style_tags=True).filter_tags():
-                    if te.tag == 'td' or te.tag == 'th':
-                        if '+' in [a.name for a in te.attributes] or te.contents.startswith('+'):
-                            pt_caption = te.contents.lstrip('+')
+                    if te.tag == "td" or te.tag == "th":
+                        if "+" in [
+                            a.name for a in te.attributes
+                        ] or te.contents.startswith("+"):
+                            pt_caption = te.contents.lstrip("+")
                         else:
                             cell = hash(te.contents.strip())
                             pt_cells[cell] = pt_cells.get(cell, 0) + 1
 
             ct_caption = None
             ct_cells = {}
             if curr_wc:
                 for te in mw.parse(curr_wikitext, skip_style_tags=True).filter_tags():
-                    if te.tag == 'td' or te.tag == 'th':
-                        if '+' in [a.name for a in te.attributes] or te.contents.startswith('+'):
-                            ct_caption = te.contents.lstrip('+')
+                    if te.tag == "td" or te.tag == "th":
+                        if "+" in [
+                            a.name for a in te.attributes
+                        ] or te.contents.startswith("+"):
+                            ct_caption = te.contents.lstrip("+")
                         else:
                             cell = hash(te.contents.strip())
                             ct_cells[cell] = ct_cells.get(cell, 0) + 1
 
             if pt_caption != ct_caption:
-                changes.append(('caption', pt_caption, ct_caption))
+                changes.append(("caption", pt_caption, ct_caption))
 
             allcells = set(pt_cells.keys()).union(set(ct_cells.keys()))
             changed = 0
             inserted = max(0, sum(ct_cells.values()) - sum(pt_cells.values()))
             removed = max(0, sum(pt_cells.values()) - sum(ct_cells.values()))
             for c in allcells:
                 changed += abs(pt_cells.get(c, 0) - ct_cells.get(c, 0))
-            changed -= (inserted + removed)
-            changed = changed / 2  # each change results in two no-longer-matching cell values
+            changed -= inserted + removed
+            changed = (
+                changed / 2
+            )  # each change results in two no-longer-matching cell values
             if inserted:
-                changes.append(('cells', 'insert', inserted))
+                changes.append(("cells", "insert", inserted))
             if removed:
-                changes.append(('cells', 'remove', removed))
+                changes.append(("cells", "remove", removed))
             if changed:
-                changes.append(('cells', 'change', changed))
+                changes.append(("cells", "change", changed))
 
-        elif node_type == 'Text Formatting':
+        elif node_type == "Text Formatting":
             # check if format type / contents changed
             # Note this will skip '''text''' -> <b>text</b> which are both `b` tags (same for italics)
-            if prev_wikitext is not None and '>' in prev_wikitext:
-                prev_wikitext = prev_wikitext[:prev_wikitext.find('>') + 1]
-            if curr_wikitext is not None and '>' in curr_wikitext:
-                curr_wikitext = curr_wikitext[:curr_wikitext.find('>') + 1]
+            if prev_wikitext is not None and ">" in prev_wikitext:
+                prev_wikitext = prev_wikitext[: prev_wikitext.find(">") + 1]
+            if curr_wikitext is not None and ">" in curr_wikitext:
+                curr_wikitext = curr_wikitext[: curr_wikitext.find(">") + 1]
             if prev_wikitext != curr_wikitext:
-                changes.append(('format tag', prev_wikitext, curr_wikitext))
+                changes.append(("format tag", prev_wikitext, curr_wikitext))
 
-        elif node_type == 'HTMLEntity':
+        elif node_type == "HTMLEntity":
             # check if display value of the HTMLEntity has changed
             # This will ignore code differences that don't affect output
             # e.g., '&Delta;' vs. '&#916;' vs. '&#x0394;' are all the equivalent of 'Δ'
             prev_ent = prev_wc.normalize() if prev_wc else None
             curr_ent = curr_wc.normalize() if curr_wc else None
             if prev_ent != curr_ent:
-                changes.append(('display-value', prev_ent, curr_ent))
+                changes.append(("display-value", prev_ent, curr_ent))
 
-        elif node_type == 'List':
+        elif node_type == "List":
             # check if list type changed
             prev_tag = str(prev_wc.tag) if prev_wc else None
             curr_tag = str(curr_wc.tag) if curr_wc else None
             if prev_tag != curr_tag:
-                changes.append(('list item', prev_tag, curr_tag))
+                changes.append(("list item", prev_tag, curr_tag))
 
-        elif node_type == 'Gallery':
+        elif node_type == "Gallery":
             # Ignore contents changes as they should be captured my media changes
-            pr_attrs = {str(a.name).strip(): str(a.value).strip() for a in prev_wc.attributes} if prev_wc else {}
-            cr_attrs = {str(a.name).strip(): str(a.value).strip() for a in curr_wc.attributes} if curr_wc else {}
+            pr_attrs = (
+                {str(a.name).strip(): str(a.value).strip() for a in prev_wc.attributes}
+                if prev_wc
+                else {}
+            )
+            cr_attrs = (
+                {str(a.name).strip(): str(a.value).strip() for a in curr_wc.attributes}
+                if curr_wc
+                else {}
+            )
             attrs = set(pr_attrs).union(set(cr_attrs))
             for a in attrs:
                 if pr_attrs.get(a) != cr_attrs.get(a):
-                    changes.append(('attribute',
-                                    (a, pr_attrs[a]) if a in pr_attrs else None,
-                                    (a, cr_attrs[a]) if a in cr_attrs else None))
+                    changes.append(
+                        (
+                            "attribute",
+                            (a, pr_attrs[a]) if a in pr_attrs else None,
+                            (a, cr_attrs[a]) if a in cr_attrs else None,
+                        )
+                    )
 
-        elif node_type == 'Heading':
+        elif node_type == "Heading":
             # separate between level and title changes
             ph_level = prev_wc.level if prev_wc else None
             ch_level = curr_wc.level if curr_wc else None
             if ph_level != ch_level:
-                changes.append(('level', ph_level, ch_level))
+                changes.append(("level", ph_level, ch_level))
             ph_title = prev_wc.title.strip() if prev_wc else None
             ch_title = curr_wc.title.strip() if curr_wc else None
             name = ph_title if ph_title else ch_title
             if ph_title != ch_title:
-                changes.append(('title', ph_title, ch_title))
+                changes.append(("title", ph_title, ch_title))
 
-        elif node_type == 'Comment':
+        elif node_type == "Comment":
             # check if comment contents changed
             pc_contents = prev_wc.contents.strip() if prev_wc else None
             cc_contents = curr_wc.contents.strip() if curr_wc else None
             if pc_contents != cc_contents:
-                changes.append(('comment', pc_contents, cc_contents))
+                changes.append(("comment", pc_contents, cc_contents))
 
-        elif node_type == 'ExternalLink':
+        elif node_type == "ExternalLink":
             # separate between url and text (display) changes
             pe_url = prev_wc.url.strip() if prev_wc else None
             ce_url = curr_wc.url.strip() if curr_wc else None
             name = pe_url if pe_url else ce_url
             if pe_url != ce_url:
-                changes.append(('url', pe_url, ce_url))
+                changes.append(("url", pe_url, ce_url))
 
             pl_display = prev_wc.title.strip() if prev_wc else None
             cl_display = curr_wc.title.strip() if curr_wc else None
             if pl_display != cl_display:
-                changes.append(('text', pl_display, cl_display))
+                changes.append(("text", pl_display, cl_display))
     except Exception:
         pass
     return name, changes
 
 
-def get_diff_count(result, lang='en'):
+def get_diff_count(result, lang="en"):  # noqa: C901
     """Prepares more complete edit type summary based on tree diff result.
 
     Parameters
     ----------
     result : dict
         The tree diff result containing inserts, removes, changes, and moves made in a Wikipedia revision.
     lang : string
@@ -268,113 +333,143 @@
     Returns
     -------
     dict
         a dict containing each occurrence of a change
     """
     node_edits = []
     text_edits = []
+    section_edits = []
     context = []
-    section_titles = set()
     prev_text = []
     curr_text = []
 
     # go through each type of action (insert, remove, change, move) and compute edit types
     # for text-formatting, the starting tags -- e.g., '' -- are captured independently of the
     # ending tags. This means that insert/removal/change of a standard block of text-formatting will
     # trigger two text-formatting changes in the tree differ. To account for that, we essentially skip
     # every other text-formatting result.
     tf_removes = set()
-    for r in result['remove']:
-        text = r['text']  # wikitext of the node
-        et = r['type']
-        if et == 'Text Formatting' and text.startswith("'"):
-            if text in tf_removes:  # already added 'start' of text-formatting -- don't duplicate
+    for r in result["remove"]:
+        text = r["text"]  # wikitext of the node
+        et = r["type"]
+        if et == "Text Formatting" and text.startswith("'"):
+            if (
+                text in tf_removes
+            ):  # already added 'start' of text-formatting -- don't duplicate
                 tf_removes.remove(text)
                 continue
             else:
                 tf_removes.add(text)
-        section_titles.add(r['section'])
         # if node is text, just check whether there's anything and retain for later
         # because all the text is processed at once at the end
-        if et == 'Text' and text:
+        if et == "Text" and text:
             prev_text.append(text)
         # non-text node: verify/fine-tune the edit type and add to results dictionary
+        elif et == "Section":
+            section_edits.append({"edittype": "remove", "section": r["section"]})
         else:
-            name, changes = get_node_diff(node_type=et, prev_wikitext=text, curr_wikitext='', lang=lang)
-            node_edits.append(NodeEdit(et, 'remove', r['section'], name, changes))
+            name, changes = get_node_diff(
+                node_type=et, prev_wikitext=text, curr_wikitext="", lang=lang
+            )
+            node_edits.append(NodeEdit(et, "remove", r["section"], name, changes))
     tf_inserts = set()
-    for i in result['insert']:
-        text = i['text']
-        et = i['type']
-        if et == 'Text Formatting' and text.startswith("'"):
-            if text in tf_inserts:  # already added 'start' of text-formatting -- don't duplicate
+    for i in result["insert"]:
+        text = i["text"]
+        et = i["type"]
+        if et == "Text Formatting" and text.startswith("'"):
+            if (
+                text in tf_inserts
+            ):  # already added 'start' of text-formatting -- don't duplicate
                 tf_inserts.remove(text)
                 continue
             else:
                 tf_inserts.add(text)
-        section_titles.add(i['section'])
-        if et == 'Text' and text:
+        if et == "Text" and text:
             curr_text.append(text)
+        elif et == "Section":
+            section_edits.append({"edittype": "insert", "section": i["section"]})
         else:
-            name, changes = get_node_diff(node_type=et, prev_wikitext='', curr_wikitext=text, lang=lang)
-            node_edits.append(NodeEdit(et, 'insert', i['section'], name, changes))
+            name, changes = get_node_diff(
+                node_type=et, prev_wikitext="", curr_wikitext=text, lang=lang
+            )
+            node_edits.append(NodeEdit(et, "insert", i["section"], name, changes))
     tf_changes = set()
-    for c in result['change']:
-        et = c['prev']['type']
-        ptext = c['prev']['text']
-        ctext = c['curr']['text']
-        if et == 'Text Formatting' and ptext.startswith("'"):
-            if ptext in tf_changes:  # already added 'start' of text-formatting -- don't duplicate
+    for c in result["change"]:
+        et = c["prev"]["type"]
+        ptext = c["prev"]["text"]
+        ctext = c["curr"]["text"]
+        if et == "Text Formatting" and ptext.startswith("'"):
+            if (
+                ptext in tf_changes
+            ):  # already added 'start' of text-formatting -- don't duplicate
                 tf_changes.remove(ptext)
                 continue
             else:
                 tf_changes.add(ptext)
-        section_titles.add(c['curr']['section'])
-        section_titles.add(c['prev']['section'])
-        if et == 'Text' and ptext != ctext:
+        if et == "Text" and ptext != ctext:
             prev_text.append(ptext)
             curr_text.append(ctext)
+        elif et == "Section":
+            section_edits.append(
+                {"edittype": "change", "section": c["prev"]["section"]}
+            )
         else:
-            name, changes = get_node_diff(node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang)
-            node_edits.append(NodeEdit(et, 'change', c['prev']['section'], name, changes))
+            name, changes = get_node_diff(
+                node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang
+            )
+            node_edits.append(
+                NodeEdit(et, "change", c["prev"]["section"], name, changes)
+            )
     tf_moves = set()
-    for m in result['move']:
-        et = m['prev']['type']
-        ptext = m['prev']['text']
-        ctext = m['curr']['text']
-        if et == 'Text Formatting' and ptext.startswith("'"):
-            if ptext in tf_moves:  # already added 'start' of text-formatting -- don't duplicate
+    for m in result["move"]:
+        et = m["prev"]["type"]
+        ptext = m["prev"]["text"]
+        ctext = m["curr"]["text"]
+        if et == "Text Formatting" and ptext.startswith("'"):
+            if (
+                ptext in tf_moves
+            ):  # already added 'start' of text-formatting -- don't duplicate
                 tf_moves.remove(ptext)
                 continue
             else:
                 tf_moves.add(ptext)
-        section_titles.add(m['curr']['section'])
-        section_titles.add(m['prev']['section'])
-        name, changes = get_node_diff(node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang)
-        node_edits.append(NodeEdit(et, 'move', m['prev']['section'], name, changes))
+        if et == "Section":
+            section_edits.append({"edittype": "move", "section": m["prev"]["section"]})
+        else:
+            name, changes = get_node_diff(
+                node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang
+            )
+            node_edits.append(NodeEdit(et, "move", m["prev"]["section"], name, changes))
 
     # give raw insert/remove counts
     # changes can be assumed to be overlap between insert+remove -- e.g., 5 insert and 3 remove -> 3 change, 2 insert
     # but would require more work to align well enough to know where words were likely changed vs. inserted/removed
     if prev_text or curr_text:
-        is_text_change_found = parse_change_text(''.join(prev_text), ''.join(curr_text), lang=lang, summarize=False)
+        is_text_change_found = parse_change_text(
+            "".join(prev_text), "".join(curr_text), lang=lang, summarize=False
+        )
         if is_text_change_found:
             for text_subcat, text_et in is_text_change_found.items():
                 for txt, et_count in text_et.items():
                     if et_count > 0:
-                        text_edits.append(TextEdit(text_subcat, 'insert', txt, et_count))
+                        text_edits.append(
+                            TextEdit(text_subcat, "insert", txt, et_count)
+                        )
                     elif et_count < 0:
-                        text_edits.append(TextEdit(text_subcat, 'remove', txt, abs(et_count)))
-
-    # identify how many sections have been edited based on a few heuristics
-    if section_titles:
-        sec_remove = sum([1 for n in node_edits if n.type == 'Heading' and n.edittype == 'remove']) + int('curr-no-content' in result)
-        sec_insert = sum([1 for n in node_edits if n.type == 'Heading' and n.edittype == 'insert']) + int('prev-no-content' in result)
-        sec_change = len(section_titles) - sec_remove - sec_insert
-        if sec_remove:
-            context.append(Context('Section', 'remove', sec_remove))
-        if sec_insert:
-            context.append(Context('Section', 'insert', sec_insert))
-        if sec_change:
-            context.append(Context('Section', 'change', sec_change))
+                        text_edits.append(
+                            TextEdit(text_subcat, "remove", txt, abs(et_count))
+                        )
+
+    sec_remove = sum([1 for n in section_edits if n["edittype"] == "remove"])
+    sec_insert = sum([1 for n in section_edits if n["edittype"] == "insert"])
+    sec_move = sum([1 for n in section_edits if n["edittype"] == "move"])
+    sec_change = sum([1 for n in section_edits if n["edittype"] == "change"])
+    if sec_remove:
+        context.append(Context("Section", "remove", sec_remove))
+    if sec_insert:
+        context.append(Context("Section", "insert", sec_insert))
+    if sec_change:
+        context.append(Context("Section", "change", sec_change))
+    if sec_move:
+        context.append(Context("Section", "move", sec_move))
 
-    return {'node-edits': node_edits, 'text-edits': text_edits, 'context': context}
+    return {"node-edits": node_edits, "text-edits": text_edits, "context": context}
```

### Comparing `mwedittypes-2.1.0/mwedittypes/simple_differ.py` & `mwedittypes-2.1.1/mwedittypes/simple_differ.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,107 @@
 import re
 
 import mwparserfromhell as mw
 
 from mwedittypes.tokenizer import parse_change_text
-from mwedittypes.utils import find_nested_media, node_to_name, sec_to_name, simple_node_class, wikitext_to_plaintext
+from mwedittypes.utils import (
+    find_nested_media,
+    node_to_name,
+    sec_to_name,
+    simple_node_class,
+    wikitext_to_plaintext,
+)
 
 
 # equivalent of main function
-def get_diff(prev_wikitext, curr_wikitext, lang='en'):
+def get_diff(prev_wikitext, curr_wikitext, lang="en"):
     """Run through full process of getting diff between two wikitext revisions."""
     prev_tree = WikitextBag(wikitext=prev_wikitext, lang=lang)
     curr_tree = WikitextBag(wikitext=curr_wikitext, lang=lang)
     d = Differ(prev_tree, curr_tree)
     result = d.count_actions()
     return result
 
 
 class Node:
     """
     Basic object for wrapping mwparserfromhell wikitext nodes
     """
 
-    def __init__(self, name, ntype='Text', mwnode=None, section=None):
+    def __init__(self, name, ntype="Text", mwnode=None, section=None):
         self.name = name  # For debugging purposes
         self.ntype = ntype  # Type of node for result
         self.mwnode = mwnode
         self.text = str(mwnode)  # Text that is needed if unnesting the node
         # Content hash is used for quickly computing equality for most nodes.
         # Generally this just a simple hash of self.text (wikitext associated with a node) but
         # the text hash for sections is based on all the content within the section
         # so it can be used for pruning while self.text is just the text that creates the section
         # e.g., "==Section==\nThis is a section." would have as text "==Section==" but hash the full.
         # so the Differ doesn't identify a section as changing when content within it is changed
         self.content_hash = hash(self.text)
         self.section = section  # section that the node is a part of -- useful for formatting final diff
 
-    def unnest(self, lang='en'):
+    def unnest(self, lang="en"):
         """Expand a node to also include all of its subnodes.
         This approach starts with a single wikitext node -- e.g., a single Tag node with nested link nodes etc.:
         <ref>{{cite web|title=[[Gallery]]|url=http://digital.belvedere.at|publisher=Digitales Belvedere}}</ref>
-        and splits it into its component parts (ref, template, wikilink, externallink) to identify fine-grained changes.
+        and splits it into its component parts (ref, template, wikilink, externallink) to find fine-grained changes.
         """
         nodes = []
         # Using string mixin methods such as wt.find(x) for subnodes in the for
         # loop below means doing str(wt) everytime, which is expensive because
         # it recursively converts each node to str. Better to create a string using
         # the node's text and use built-in string methods instead.
-        if self.ntype == 'Gallery':
+        if self.ntype == "Gallery":
             # strip leading / trailing gallery tags so parser correctly parses everything in between
             # otherwise links, formatting, etc. is treated as text
-            gallery_start = self.text.find('>')
-            gallery_end = self.text.rfind('<')
+            gallery_start = self.text.find(">")
+            gallery_end = self.text.rfind("<")
             try:
                 # the <br> is a hack; it'll be skipped in the ifilter loop; otherwise first image skipped
-                wt = mw.parse('<br>' + self.text[gallery_start+1:gallery_end], skip_style_tags=True)
+                wt = mw.parse(
+                    "<br>" + self.text[gallery_start + 1 : gallery_end],
+                    skip_style_tags=True,
+                )
             except Exception:  # fallback
                 wt = mw.parse(self.mwnode)
         else:
             wt = mw.parse(self.mwnode)
         for idx, nn in enumerate(wt.ifilter(recursive=True)):
             if idx == 0:
                 continue  # skip root node -- already set
             ntype = simple_node_class(nn, lang)
-            if ntype == 'Text':
+            if ntype == "Text":
                 # media w/o bracket will be IDed as text by mwparserfromhell
                 # templates / galleries are where we find this nested media
-                if self.ntype == 'Template' or self.ntype == 'Gallery':
-                    for m in find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery')):
-                        nn_node = Node(f'Media: {m[:10]}...',
-                                       ntype='Media',
-                                       mwnode=m,
-                                       section=self.section)
+                if self.ntype == "Template" or self.ntype == "Gallery":
+                    for m in find_nested_media(
+                        str(nn), is_gallery=(self.ntype == "Gallery")
+                    ):
+                        nn_node = Node(
+                            f"Media: {m[:10]}...",
+                            ntype="Media",
+                            mwnode=m,
+                            section=self.section,
+                        )
                         nodes.append(nn_node)
             # tables are very highly-structured and produce a ton of nodes (each cell and more)
             # so we just extract links, formatting, etc. that appears in the table and skip the cells
             # because changes to those will generally be caught in the overall table changes and text changes
             # this leads to much faster parsing in exchange for not knowing how many table cells were edited
-            elif ntype == 'Table Element':
+            elif ntype == "Table Element":
                 pass
             else:
-                nn_node = Node(node_to_name(nn, lang=lang), ntype=ntype, mwnode=nn, section=self.section)
+                nn_node = Node(
+                    node_to_name(nn, lang=lang),
+                    ntype=ntype,
+                    mwnode=nn,
+                    section=self.section,
+                )
                 nodes.append(nn_node)
         return nodes
 
 
 class WikitextBag:
     """
     Structure for extracting and holding an unordered collection of wikitext nodes based on mwparserfromhell
@@ -102,43 +120,80 @@
         """
         wt = mw.parse(wikitext, skip_style_tags=True)
         for sidx, s in enumerate(wt.get_sections(flat=True)):
             if s:
                 sec_id = sec_to_name(s, sidx)
                 s_node = Node(sec_id, ntype="Section", mwnode=s, section=sec_id)
                 self.secname_to_text[sec_id] = s_node.text
-                self.nodes[s_node.content_hash] = self.nodes.get(s_node.content_hash, []) + [s_node]
-                for n in s.nodes:  # this is just top-level of nodes so e.g., table but not all the table rows etc.
+                self.nodes[s_node.content_hash] = self.nodes.get(
+                    s_node.content_hash, []
+                ) + [s_node]
+                for (
+                    n
+                ) in (
+                    s.nodes
+                ):  # this is just top-level of nodes so e.g., table but not all the table rows etc.
                     ntype = simple_node_class(n, self.lang)
-                    if ntype != 'Text':
-                        n_node = Node(node_to_name(n, self.lang), ntype=ntype, mwnode=n, section=s_node.name)
-                        self.nodes[n_node.content_hash] = self.nodes.get(n_node.content_hash, []) + [n_node]
+                    if ntype != "Text":
+                        n_node = Node(
+                            node_to_name(n, self.lang),
+                            ntype=ntype,
+                            mwnode=n,
+                            section=s_node.name,
+                        )
+                        self.nodes[n_node.content_hash] = self.nodes.get(
+                            n_node.content_hash, []
+                        ) + [n_node]
                 if "''" in s_node.text:
-                    for line in s_node.text.split('\n'):
+                    for line in s_node.text.split("\n"):
                         if "''" in line:
                             line, bt_found = re.subn("'{5}", "", line)
                             for _ in range(bt_found // 2):
-                                tfn = Node("Bold-Italic", ntype='Text Formatting', mwnode="'''''",
-                                           section=s_node.name)
-                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
+                                tfn = Node(
+                                    "Bold-Italic",
+                                    ntype="Text Formatting",
+                                    mwnode="'''''",
+                                    section=s_node.name,
+                                )
+                                self.nodes[tfn.content_hash] = self.nodes.get(
+                                    tfn.content_hash, []
+                                ) + [tfn]
                             line, b_found = re.subn("'{3}", "", line)
                             for _ in range(b_found // 2):
-                                tfn = Node("Bold", ntype='Text Formatting', mwnode="'''", section=s_node.name)
-                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
+                                tfn = Node(
+                                    "Bold",
+                                    ntype="Text Formatting",
+                                    mwnode="'''",
+                                    section=s_node.name,
+                                )
+                                self.nodes[tfn.content_hash] = self.nodes.get(
+                                    tfn.content_hash, []
+                                ) + [tfn]
                             line, t_found = re.subn("'{2}", "", line)
                             for _ in range(t_found // 2):
-                                tfn = Node("Italic", ntype='Text Formatting', mwnode="''", section=s_node.name)
-                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
+                                tfn = Node(
+                                    "Italic",
+                                    ntype="Text Formatting",
+                                    mwnode="''",
+                                    section=s_node.name,
+                                )
+                                self.nodes[tfn.content_hash] = self.nodes.get(
+                                    tfn.content_hash, []
+                                ) + [tfn]
 
     def expand_nested(self):
         """Expand nested nodes in tree -- e.g., Ref tags with templates/links contained in them."""
         to_add = {}
         for n_hash in self.nodes:
             for n in self.nodes[n_hash]:
-                if n.ntype not in ('Section', 'Heading', 'Text'):  # leaves tag, link, etc.
+                if n.ntype not in (
+                    "Section",
+                    "Heading",
+                    "Text",
+                ):  # leaves tag, link, etc.
                     for nn in n.unnest(self.lang):
                         to_add[nn.content_hash] = to_add.get(nn.content_hash, []) + [nn]
 
         for n_hash in to_add:
             for n in to_add[n_hash]:
                 self.nodes[n_hash] = self.nodes.get(n_hash, []) + [n]
 
@@ -178,56 +233,56 @@
                 # extras in t1: remove from t2 and keep just extras in t1
                 elif diff > 0:
                     t2n.pop(n_hash)
                     t1n[n_hash] = t1n[n_hash][:diff]
                 # extras in t2: remove from t1 and keep just extras in t2
                 elif diff < 0:
                     t1n.pop(n_hash)
-                    t2n[n_hash] = t2n[n_hash][:abs(diff)]
+                    t2n[n_hash] = t2n[n_hash][: abs(diff)]
         # no need to loop through t2n because what's left in it doesn't have any matches
 
     def count_actions(self):
         """Explain differences."""
         edit_types = {}
         prev_text_sections = set()
         curr_text_sections = set()
 
         # aggregate by node type to identify non-matching nodes
         prev_ntypes = {}
         for n_hash in self.t1.nodes:
             for n in self.t1.nodes[n_hash]:
                 prev_ntypes[n.ntype] = prev_ntypes.get(n.ntype, 0) + 1
-                if n.ntype == 'Section':
+                if n.ntype == "Section":
                     prev_text_sections.add(n.section)
         curr_ntypes = {}
         for n_hash in self.t2.nodes:
             for n in self.t2.nodes[n_hash]:
                 curr_ntypes[n.ntype] = curr_ntypes.get(n.ntype, 0) + 1
-                if n.ntype == 'Section':
+                if n.ntype == "Section":
                     curr_text_sections.add(n.section)
 
         all_ntypes = set(prev_ntypes.keys()).union(set(curr_ntypes.keys()))
         for n_type in all_ntypes:
             # change is overlap in nodes; removal are extras in previous; insert are extras in current
             chg = min(prev_ntypes.get(n_type, 0), curr_ntypes.get(n_type, 0))
             rem = prev_ntypes.get(n_type, 0) - chg
             ins = curr_ntypes.get(n_type, 0) - chg
             edit_types[n_type] = {}
             if chg > 0:
-                edit_types[n_type]['change'] = chg
+                edit_types[n_type]["change"] = chg
             if rem > 0:
-                edit_types[n_type]['remove'] = rem
+                edit_types[n_type]["remove"] = rem
             if ins > 0:
-                edit_types[n_type]['insert'] = ins
+                edit_types[n_type]["insert"] = ins
 
         lang = self.t1.lang
-        prev_text = ''
+        prev_text = ""
         for s in prev_text_sections:
             prev_text += wikitext_to_plaintext(self.t1.secname_to_text[s], lang=lang)
-        curr_text = ''
+        curr_text = ""
         for s in curr_text_sections:
             curr_text += wikitext_to_plaintext(self.t2.secname_to_text[s], lang=lang)
 
         text_changes = parse_change_text(prev_text, curr_text, lang=lang)
         edit_types.update(text_changes)
 
         return edit_types
```

### Comparing `mwedittypes-2.1.0/mwedittypes/tokenizer.py` & `mwedittypes-2.1.1/mwedittypes/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,51 @@
-from collections import Counter
 import re
 import string
+from collections import Counter
 
 from mwconstants import NON_WHITESPACE_LANGUAGES
 
-from mwedittypes.constants import ENGLISH_UNICODE, NON_ENGLISH_UNICODE, SENTENCE_BREAKS_REGEX
+from mwedittypes.constants import (
+    ENGLISH_UNICODE,
+    NON_ENGLISH_UNICODE,
+    SENTENCE_BREAKS_REGEX,
+)
 
 
 class Tokenizer:
-
-    def __init__(self, english_unicode, non_english_unicode, lang='en'):
-        self.english_punc_regex = r'[{0}]'.format(re.escape(string.punctuation))
+    def __init__(self, english_unicode, non_english_unicode, lang="en"):
+        self.english_punc_regex = r"[{0}]".format(re.escape(string.punctuation))
         self.english_unicode = english_unicode
         self.non_english_unicode = non_english_unicode
         self.lang = lang
 
     def get_punctuations(self, text):
         # get ellipses
-        ellipses = re.findall(r'\.{3,}', text)
-        text = re.sub(r'\.{3,}', '', text)
+        ellipses = re.findall(r"\.{3,}", text)
+        text = re.sub(r"\.{3,}", "", text)
 
         # get other punctuation
         english_punc_regex = re.findall(self.english_punc_regex, text)
 
         english_unicode_pattern = re.compile(self.english_unicode, re.UNICODE)
         english_unicode_regex = re.findall(english_unicode_pattern, text)
 
         non_english_unicode_pattern = re.compile(self.non_english_unicode, re.UNICODE)
         non_english_punc_regex = re.findall(non_english_unicode_pattern, text)
 
-        return ellipses + english_punc_regex + english_unicode_regex + non_english_punc_regex
+        return (
+            ellipses
+            + english_punc_regex
+            + english_unicode_regex
+            + non_english_punc_regex
+        )
 
     def get_whitespace(self, text):
         # Get whitespaces. Detects newlines, return characters as well as spaces as whitespaces.
-        whitespace = re.findall(r'[\s]', text)
+        whitespace = re.findall(r"[\s]", text)
         return whitespace
 
     def get_words(self, text):
         # This extracts words inclusive of those with hyphens and apostrophes
         if self.lang in NON_WHITESPACE_LANGUAGES:
             word_list = re.findall(r"[\w]", text)
 
@@ -45,32 +53,40 @@
             # Get words with optionally hyphens and apostrophe:
             # \b - word breaks at start and end of word
             # [\w...]+ - matches 1 or more alphanumeric characters
             # \w captures most characters with some exceptions, especially for languages with spacing characters
             # \u0980-\u09FF represents Bengali
             # \u0901-\u0963 represents Devanagari (Hindi, Marathi, etc.)
             # [-']? allows for hyphen/apostrophes within word
-            # ((?:...)+) capturing group (extract words) made up of 1+ non-capturing sequences of
-            # alphanumeric + hyphen/apostrophe. this allows for many-time-hyphenated words and the non-capturing wrapped
-            # in capturing is to only gather the entire word (otherwise capturing groups only capture the last instance)
-            word_list = re.findall(r"\b((?:[\w\u0980-\u09FF\u0901-\u0963]+[-']?)+)\b", text)
+            # ((?:...)+) capturing group (extract words) made up of 1+ non-capturing sequences of alphanumeric +
+            # hyphen/apostrophe. this allows for many-time-hyphenated words and the non-capturing wrapped in capturing
+            # is to only gather the entire word (otherwise capturing groups only capture the last instance)
+            word_list = re.findall(
+                r"\b((?:[\w\u0980-\u09FF\u0901-\u0963]+[-']?)+)\b", text
+            )
         return word_list
 
     def get_sentences(self, text):
         # minimum sentence size is two words, otherwise contributes to words etc. but not sentences
         # we ignored leading/trailing whitespace differences on sentences when comparing as those aren't really changes
         # the whitespace differences are still captured by the whitespace counts
         min_sentence_size = 2
         sentences = re.split(SENTENCE_BREAKS_REGEX, text)
-        sentences = [s.strip() for s in sentences if len(self.get_words(s)) >= min_sentence_size]
+        sentences = [
+            s.strip() for s in sentences if len(self.get_words(s)) >= min_sentence_size
+        ]
         return sentences
 
     def get_paragraphs(self, text):
-        if text != '':
-            paragraphs = [p.strip() for p in re.split(r'\n{2}', text) if len(self.get_words(p)) > 0]
+        if text != "":
+            paragraphs = [
+                p.strip()
+                for p in re.split(r"\n{2}", text)
+                if len(self.get_words(p)) > 0
+            ]
             return paragraphs
         return []
 
     def tokenize_and_get_occurrence(self, text):
         whitespaces = self.get_whitespace(text)
         punctuation = self.get_punctuations(text)
         words = self.get_words(text)
@@ -80,51 +96,62 @@
         whitespace_occurrence = Counter(whitespaces)
         punctuation_occurrence = Counter(punctuation)
         words_occurrence = Counter(words)
         sentences_occurrence = Counter(sentences)
         paragraphs_occurrence = Counter(paragraphs)
 
         if self.lang in NON_WHITESPACE_LANGUAGES:
-            word_key = 'Character'
+            word_key = "Character"
         else:
-            word_key = 'Word'
+            word_key = "Word"
         return {
-            'Whitespace': dict(whitespace_occurrence),
-            'Punctuation': dict(punctuation_occurrence),
+            "Whitespace": dict(whitespace_occurrence),
+            "Punctuation": dict(punctuation_occurrence),
             word_key: dict(words_occurrence),
-            'Sentence': dict(sentences_occurrence),
-            'Paragraph': dict(paragraphs_occurrence)
+            "Sentence": dict(sentences_occurrence),
+            "Paragraph": dict(paragraphs_occurrence),
         }
 
 
-def parse_change_text(prev_wikitext='', curr_wikitext='', lang='en', summarize=True):
+def parse_change_text(prev_wikitext="", curr_wikitext="", lang="en", summarize=True):
     # Initialize tokenizer class
     tokenizer = Tokenizer(ENGLISH_UNICODE, NON_ENGLISH_UNICODE, lang=lang)
 
     prev_tokenizer = tokenizer.tokenize_and_get_occurrence(prev_wikitext)
     curr_tokenizer = tokenizer.tokenize_and_get_occurrence(curr_wikitext)
 
     result = {}
     for text_category in curr_tokenizer.keys():
-        items_diff_list = list(set(curr_tokenizer[text_category].items()) ^ set(prev_tokenizer[text_category].items()))
+        items_diff_list = list(
+            set(curr_tokenizer[text_category].items())
+            ^ set(prev_tokenizer[text_category].items())
+        )
         for item in items_diff_list:
-            diff = curr_tokenizer[text_category].get(item[0], 0) - prev_tokenizer[text_category].get(item[0], 0)
-            result[text_category] = dict(result.get(text_category, {}), **{item[0]: diff})
+            diff = curr_tokenizer[text_category].get(item[0], 0) - prev_tokenizer[
+                text_category
+            ].get(item[0], 0)
+            result[text_category] = dict(
+                result.get(text_category, {}), **{item[0]: diff}
+            )
 
         # Get the maximum value between the sum of positives and sum of negatives
         if summarize and len(result.get(text_category, {})) > 0:
-            removals = sum(abs(item) for item in result[text_category].values() if item < 0)
-            additions = sum(abs(item) for item in result[text_category].values() if item > 0)
+            removals = sum(
+                abs(item) for item in result[text_category].values() if item < 0
+            )
+            additions = sum(
+                abs(item) for item in result[text_category].values() if item > 0
+            )
             change = min(removals, additions)
             result[text_category] = {}
             removals -= change
             additions -= change
 
             if removals > 0:
-                result[text_category]['remove'] = removals
+                result[text_category]["remove"] = removals
 
             if additions > 0:
-                result[text_category]['insert'] = additions
+                result[text_category]["insert"] = additions
 
             if change > 0:
-                result[text_category]['change'] = change
+                result[text_category]["change"] = change
     return result
```

### Comparing `mwedittypes-2.1.0/mwedittypes/tree_differ.py` & `mwedittypes-2.1.1/mwedittypes/tree_differ.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-from anytree import PostOrderIter, NodeMixin
-from anytree.util import leftsibling
 import mwparserfromhell as mw
+from anytree import NodeMixin, PostOrderIter
+from anytree.util import leftsibling
 
-from mwedittypes.utils import (find_nested_media, find_nested_textformatting, node_to_name, sec_to_name,
-                               simple_node_class, wikitext_to_plaintext)
+from mwedittypes.utils import (
+    find_nested_media,
+    find_nested_textformatting,
+    node_to_name,
+    sec_to_name,
+    simple_node_class,
+    wikitext_to_plaintext,
+)
 
 
 # equivalent of main function
-def get_diff(prev_wikitext, curr_wikitext, lang='en', timeout=False):
+def get_diff(prev_wikitext, curr_wikitext, lang="en", timeout=False):
     """Run through full process of getting tree diff between two wikitext revisions."""
     # To provide proper structure, need all content to be nested under a section
     prev_tree = WikitextTree(wikitext=prev_wikitext, lang=lang)
     curr_tree = WikitextTree(wikitext=curr_wikitext, lang=lang)
     d = Differ(prev_tree, curr_tree, timeout=timeout)
     diff = d.get_corresponding_nodes()
-    result = diff.post_process(prev_tree.secname_to_text, curr_tree.secname_to_text, lang=lang)
-    # this helps the node differ know that the lede is also a new section
-    # otherwise depends on headings to track changes to sections
-    if not prev_wikitext:
-        result['prev-no-content'] = True
-    if not curr_wikitext:
-        result['curr-no-content'] = True
+    result = diff.post_process(
+        prev_tree.secname_to_text, curr_tree.secname_to_text, lang=lang
+    )
     return result
 
 
 class OrderedNode(NodeMixin):
     """
     Extension of anytree library node to support tree differ.
     """
 
-    def __init__(self, name, ntype='Text', idx=-1, mwnode=None, section=None,
-                 parent=None, children=None):
+    def __init__(
+        self,
+        name,
+        ntype="Text",
+        idx=-1,
+        mwnode=None,
+        section=None,
+        parent=None,
+        children=None,
+    ):
         super(OrderedNode, self).__init__()
         self.name = name  # For debugging purposes
         self.ntype = ntype  # Different node types can be treated differently when computing equality
         self.mwnode = mwnode
-        self.text = str(mwnode) if mwnode is not None else ''  # Text that can then be passed to a diffing library
+        self.text = (
+            str(mwnode) if mwnode is not None else ""
+        )  # Text that can then be passed to a diffing library
         # Used for quickly computing equality for most nodes.
         # Generally this just a simple hash of self.mwnode (wikitext associated with a node) but
         # the text hash for sections is based on all the content within the section
         # so it can be used for pruning while self.text is just the text that creates the section
         # e.g., "==Section==\nThis is a section." would have as text "==Section==" but hash the full.
         # so the Differ doesn't identify a section as changing when content within it is changed
         self.content_hash = hash(self.text)
@@ -51,120 +63,147 @@
         self.leftmostidx = None
 
     def leftmost(self):
         if self.leftmostidx is None:
             self.leftmostidx = self.idx if self.is_leaf else self.children[0].leftmost()
         return self.leftmostidx
 
-    def unnest(self, lang='en'):
+    def unnest(self, lang="en"):
         """Build tree of document nodes by recursing within a single wikitext node.
 
         This approach starts with a single wikitext node -- e.g., a single Tag node with nested link nodes etc.:
         <ref>{{cite web|title=[[Gallery]]|url=http://digital.belvedere.at|publisher=Digitales Belvedere}}</ref>
         and splits it into its component pieces to then identify what has changed between revisions.
 
         Example above would take a Reference node as input and build the following tree (in-place):
         <--rest-of-tree-- Reference <--child-of-- Template (cite web) <--child-of-- WikiLink (Gallery)
                                                                 ^--------child-of-- External Link (http://digital...)
         """
-        if self.ntype == 'Gallery':
+        if self.ntype == "Gallery":
             # strip leading / trailing gallery tags so parser correctly parses everything in between
             # otherwise links, templates, etc. is treated as text
-            gallery_start = self.text.find('>')
-            gallery_end = self.text.rfind('<')
+            gallery_start = self.text.find(">")
+            gallery_end = self.text.rfind("<")
             try:
                 # the break is a hack; it'll be skipped in the ifilter loop; otherwise first image skipped
-                wt = mw.parse('<br>' + self.text[gallery_start+1:gallery_end], skip_style_tags=True)
+                wt = mw.parse(
+                    "<br>" + self.text[gallery_start + 1 : gallery_end],
+                    skip_style_tags=True,
+                )
             except Exception:  # fallback
                 wt = mw.parse(self.mwnode)  # automatically carries over skip_style_tags
         else:
             wt = mw.parse(self.mwnode)  # automatically carries over skip_style_tags
-        parent_ranges = [(0, len(self.text), self)]  # (start idx of node, end idx of node, node object)
+        parent_ranges = [
+            (0, len(self.text), self)
+        ]  # (start idx of node, end idx of node, node object)
         for idx, nn in enumerate(wt.ifilter(recursive=True)):
             if idx == 0:
                 continue  # skip root node -- already set or placeholder <br> node for galleries
             ntype = simple_node_class(nn, lang)
-            if ntype == 'Text':
+            if ntype == "Text":
                 # media w/o bracket will be IDed as text by mwparserfromhell
                 # templates / galleries are where we find this nested media
-                # any discovered media will just be the start and aren't guaranteed to be the whole image + caption etc.
-                if self.ntype == 'Template' or self.ntype == 'Gallery':
-                    for m in find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery')):
-                        nn_node = OrderedNode(f'Media: {m[:10]}...',
-                                              ntype='Media',
-                                              mwnode=m,
-                                              section=self.section,
-                                              parent=self)
+                # any discovered media will just be the start and aren't guaranteed to be the whole image+caption etc.
+                if self.ntype == "Template" or self.ntype == "Gallery":
+                    for m in find_nested_media(
+                        str(nn), is_gallery=(self.ntype == "Gallery")
+                    ):
+                        nn_node = OrderedNode(
+                            f"Media: {m[:10]}...",
+                            ntype="Media",
+                            mwnode=m,
+                            section=self.section,
+                            parent=self,
+                        )
                         offset = self.text.find(str(m), parent_ranges[0][0])
                         parent_ranges.insert(0, (offset, offset + len(m), nn_node))
             # tables are very highly-structured and produce a ton of nodes (each cell and more)
             # so we just extract links, formatting, etc. that appears in the table and skip the cells
             # because changes to those will generally be caught in the overall table changes and text changes
             # this leads to much faster parsing in exchange for not knowing how many table cells were edited
-            elif ntype == 'Table Element':
+            elif ntype == "Table Element":
                 pass
             else:
                 # start looking from the start of the latest node
                 node_start = self.text.find(str(nn), parent_ranges[0][0])
                 # identify direct parent of node
                 for parent_start, parent_end, parent_node in parent_ranges:
-                    if node_start < parent_end:  # starts before end of a previous node; already know it begins after it
-                        nn_node = OrderedNode(node_to_name(nn, lang=lang), ntype=ntype, mwnode=nn,
-                                              section=self.section, parent=parent_node)
-                        parent_ranges.insert(0, (node_start, node_start + len(nn), nn_node))
+                    if (
+                        node_start < parent_end
+                    ):  # starts before end of a previous node; already know it begins after it
+                        nn_node = OrderedNode(
+                            node_to_name(nn, lang=lang),
+                            ntype=ntype,
+                            mwnode=nn,
+                            section=self.section,
+                            parent=parent_node,
+                        )
+                        parent_ranges.insert(
+                            0, (node_start, node_start + len(nn), nn_node)
+                        )
                         break
         if "''" in self.text:
             for tfnode, tfspan in find_nested_textformatting(self.text):
                 for parent_start, parent_end, parent_node in parent_ranges:
                     if tfspan[0] >= parent_start and tfspan[1] <= parent_end:
-                        nn_node = OrderedNode(f'Text-Formatting: {tfnode}',
-                                              ntype='Text Formatting',
-                                              mwnode=tfnode,
-                                              section=self.section,
-                                              parent=parent_node)
+                        nn_node = OrderedNode(
+                            f"Text-Formatting: {tfnode}",
+                            ntype="Text Formatting",
+                            mwnode=tfnode,
+                            section=self.section,
+                            parent=parent_node,
+                        )
                         break
 
     def dump(self):
-        return {'type': self.ntype,
-                'text': self.text,
-                'section': self.section}
+        return {"type": self.ntype, "text": self.text, "section": self.section}
+
 
 class WikitextTree:
     """
     Tree structure for wikitext based on mwparserfromhell
     """
 
     def __init__(self, wikitext, lang="en"):
         self.lang = lang
-        self.root = OrderedNode('root', ntype="Article")
+        self.root = OrderedNode("root", ntype="Article")
         self.secname_to_text = {}
-        self.wikitext_to_tree(wikitext)
+        if wikitext:
+            self.wikitext_to_tree(wikitext)
         self.key_roots = None
 
     def wikitext_to_tree(self, wikitext):
         """Build tree of document nodes from Wikipedia article.
 
         This approach builds a tree with an artificial 'root' node on the 1st level,
         all of the article sections nested flatly underneath (including the Lede section),
         and all of the text, link, template, etc. nodes nested under their respective sections.
         """
         wt = mw.parse(wikitext, skip_style_tags=True)
         for sidx, s in enumerate(wt.get_sections(flat=True)):
             sec_id = sec_to_name(s, sidx)
-            sec_text = ''.join([str(n) for n in s.nodes])
+            sec_text = "".join([str(n) for n in s.nodes])
             self.secname_to_text[sec_id] = sec_text
-            s_node = OrderedNode(sec_id, ntype="Section", mwnode=s, section=sec_id, parent=self.root)
+            s_node = OrderedNode(
+                sec_id, ntype="Section", mwnode=s, section=sec_id, parent=self.root
+            )
             for n in s.nodes:
-                n_node = OrderedNode(node_to_name(n, self.lang), ntype=simple_node_class(n, self.lang), mwnode=n,
-                                     section=s_node.name, parent=s_node)
+                _ = OrderedNode(
+                    node_to_name(n, self.lang),
+                    ntype=simple_node_class(n, self.lang),
+                    mwnode=n,
+                    section=s_node.name,
+                    parent=s_node,
+                )
 
     def expand_nested(self):
         """Expand nested nodes in tree -- e.g., Ref tags with templates/links contained in them."""
         for n in PostOrderIter(self.root):
-            if n.ntype not in ('Article', 'Section'):
+            if n.ntype not in ("Article", "Section"):
                 n.unnest(self.lang)
 
 
 class Differ:
     """
     Find structural differences between two WikitextTrees
     """
@@ -185,15 +224,17 @@
             n.idx = i
             self.t2.append(n)
             if n.is_root or leftsibling(n) is not None:
                 self.t2_keyroots.append(n)
         self.ins_cost = 1
         self.rem_cost = 1
         self.chg_cost = 1
-        self.nodetype_chg_cost = 10  # arbitrarily high to encourage remove+insert when node types change
+        self.nodetype_chg_cost = (
+            10  # arbitrarily high to encourage remove+insert when node types change
+        )
 
         # Permanent store of transactions such that transactions[x][y] is the minimum
         # transactions to get from the sub-tree rooted at node x (in tree1) to the sub-tree
         # rooted at node y (in tree2).
         self.transactions = {None: {}}
         # Indices for each transaction, to avoid high performance cost of creating the
         # transactions multiple times
@@ -223,30 +264,44 @@
             self.transactions[i] = {}
         self.populate_transactions(transactions)
 
     def prune_trees(self, t1, t2, expand_nodes=False):
         """Quick heuristic preprocessing to reduce tree differ time by removing matching sections."""
         self.prune_sections(t1, t2)
         # arbitrary: more than 500 nodes altogether even after pruning and before unnesting -- just diff sections
-        if self.timeout and (sum(1 for n in PostOrderIter(t1.root)) + sum(1 for n in PostOrderIter(t2.root))) > 500:
+        if (
+            self.timeout
+            and (
+                sum(1 for n in PostOrderIter(t1.root))
+                + sum(1 for n in PostOrderIter(t2.root))
+            )
+            > 500
+        ):
             self.prune_to_sections(t1, t2)
         # arbitrary: seems like manageable number of total nodes -- unnest fully before diffing
-        elif expand_nodes and (not self.timeout or
-                               (sum([len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t1.root)]) +
-                               sum([len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t2.root)])) < 1000):
+        elif expand_nodes and (
+            not self.timeout
+            or (
+                sum([len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t1.root)])
+                + sum(
+                    [len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t2.root)]
+                )
+            )
+            < 1000
+        ):
             t1.expand_nested()
             t2.expand_nested()
 
     def prune_to_sections(self, t1, t2):
         """Remove all non-section nodes."""
         for n in PostOrderIter(t1.root):
-            if n.ntype == 'Section':
+            if n.ntype == "Section":
                 n.children = []
         for n in PostOrderIter(t2.root):
-            if n.ntype == 'Section':
+            if n.ntype == "Section":
                 n.children = []
 
     def prune_sections(self, t1, t2):
         """Prune nodes from any sections that align across revisions"""
         t1_sections = [n for n in PostOrderIter(t1.root) if n.ntype == "Section"]
         t2_sections = [n for n in PostOrderIter(t2.root) if n.ntype == "Section"]
         for secnode1 in t1_sections:
@@ -277,16 +332,24 @@
 
                 # get the diff
                 self.find_minimum_transactions(kr1, kr2, transactions)
 
         if self.transactions:
             for i in range(0, len(self.t1)):
                 for j in range(0, len(self.t2)):
-                    if self.transactions.get(i, {}).get(j) and len(self.transactions[i][j]) > 0:
-                        self.transactions[i][j] = tuple([self.idx_to_transaction[idx] for idx in self.transactions[i][j]])
+                    if (
+                        self.transactions.get(i, {}).get(j)
+                        and len(self.transactions[i][j]) > 0
+                    ):
+                        self.transactions[i][j] = tuple(
+                            [
+                                self.idx_to_transaction[idx]
+                                for idx in self.transactions[i][j]
+                            ]
+                        )
 
     def get_node_distance(self, n1, n2):
         """
         Get the cost of:
         * removing a node from the first tree,
         * inserting a node into the second tree,
         * or relabelling a node from the first tree to a node from the second tree.
@@ -299,20 +362,14 @@
             return self.rem_cost
         # Inserts/Removes are easy. Changes are more complicated and should only be within same node type.
         # Use arbitrarily high-value for nodetype changes to effectively ban.
         elif n1.ntype != n2.ntype:
             return self.nodetype_chg_cost
         elif n1.content_hash == n2.content_hash:
             return 0
-        # if both sections, assert no cost (changes will be captured by headings)
-        # except we want to detect moves of sections
-        elif n1.ntype == 'Section':
-            if not n1.children and not n2.children:
-                return self.chg_cost
-            return 0
         # otherwise, same node types and not the same, then change cost
         else:
             return self.chg_cost
 
     def get_lowest_cost(self, rc, ic, cc):
         min_cost = rc
         index = 0
@@ -340,17 +397,19 @@
 
                 if n1.leftmost() == kr1.leftmost() and n2.leftmost() == kr2.leftmost():
                     rem = transactions[i_minus_1][j]
                     ins = transactions[i][j_minus_1]
                     chg = transactions[i_minus_1][j_minus_1]
                     node_distance = self.get_node_distance(n1, n2)
                     # cost of each transaction
-                    transaction = self.get_lowest_cost(len(rem) + self.rem_cost,
-                                                       len(ins) + self.ins_cost,
-                                                       len(chg) + node_distance)
+                    transaction = self.get_lowest_cost(
+                        len(rem) + self.rem_cost,
+                        len(ins) + self.ins_cost,
+                        len(chg) + node_distance,
+                    )
                     if transaction == 0:
                         # record a remove
                         rc = rem.copy()
                         rc.append(self.transaction_to_idx[i][None])
                         transactions[i][j] = rc
                     elif transaction == 1:
                         # record an insert
@@ -375,17 +434,19 @@
                         k1 = n1.leftmost() - 1
                     if n2.leftmost() - 1 < kr2.leftmost():
                         k2 = None
                     else:
                         k2 = n2.leftmost() - 1
                     chg = transactions[k1][k2]
 
-                    transaction = self.get_lowest_cost(len(rem) + self.rem_cost,
-                                                       len(ins) + self.ins_cost,
-                                                       len(chg) + len(self.transactions[i][j]))
+                    transaction = self.get_lowest_cost(
+                        len(rem) + self.rem_cost,
+                        len(ins) + self.ins_cost,
+                        len(chg) + len(self.transactions[i][j]),
+                    )
                     if transaction == 0:
                         # record a remove
                         rc = rem.copy()
                         rc.append(self.transaction_to_idx[i][None])
                         transactions[i][j] = rc
                     elif transaction == 1:
                         # record an insert
@@ -395,46 +456,43 @@
                     else:
                         # record a change
                         cc = chg.copy()
                         cc.extend(self.transactions[i][j])
                         transactions[i][j] = cc
 
     def get_corresponding_nodes(self):
-        """Explain transactions.
-
-        Skip 'Section' operations as they aren't real nodes and
-        any changes to them will be captured via Headings etc.
-        """
+        """Explain transactions."""
         if self.transactions:
             transactions = self.transactions[len(self.t1) - 1][len(self.t2) - 1]
             remove = []
             insert = []
             change = []
             for i in range(0, len(transactions)):
                 if transactions[i][0] is None:
                     ins_node = self.t2[transactions[i][1]]
-                    # this second clause allows us to later detect moved sections
-                    if ins_node.ntype != 'Section' or not ins_node.children:
-                        insert.append(ins_node)
+                    insert.append(ins_node)
                 elif transactions[i][1] is None:
                     rem_node = self.t1[transactions[i][0]]
-                    if rem_node.ntype != 'Section' or not rem_node.children:
-                        remove.append(rem_node)
+                    remove.append(rem_node)
                 else:
                     prev_node = self.t1[transactions[i][0]]
                     curr_node = self.t2[transactions[i][1]]
-                    if prev_node.ntype != 'Section' or not prev_node.children:
-                        change.append((prev_node, curr_node))
-            diff = {'remove': remove, 'insert': insert, 'change': change}
+                    change.append((prev_node, curr_node))
+            diff = {"remove": remove, "insert": insert, "change": change}
             self.detect_moves(diff)
-            return Diff(nodes_removed=diff['remove'], nodes_inserted=diff['insert'],
-                        nodes_changed=diff['change'], nodes_moved=diff['move'])
+            return Diff(
+                nodes_removed=diff["remove"],
+                nodes_inserted=diff["insert"],
+                nodes_changed=diff["change"],
+                nodes_moved=diff["move"],
+            )
         else:
-            return Diff(nodes_removed=[], nodes_inserted=[],
-                        nodes_changed=[], nodes_moved=[])
+            return Diff(
+                nodes_removed=[], nodes_inserted=[], nodes_changed=[], nodes_moved=[]
+            )
 
     def detect_moves(self, diff):
         """Detect when nodes were moved (as opposed to removed/inserted/changed) and update diff.
 
         Easy case:
         * If a removed node from the previous wikitext matches an inserted node from the current wikitext,
           then remove those nodes from the corresponding remove/insert spots and combine into a "move". Examples:
@@ -447,82 +505,102 @@
           Input: Change(A,B) and Insert(A) -> Move(A,A) and Insert(B)
           Input: Change(A,B) and Remove(B) -> Remove(A) and Move(B,B)
           Input: Change(A,B) and Change(C,A) -> Move(A,A) and Insert(B) and Remove(C)
           Input: Change(A,B) and Change(B,A) -> Move(A,A) and Move(B,B)
         """
 
         # build list of all prev and curr nodes to compare for matches
-        ntypes_to_ignore = ('Text', 'Text Formatting', 'List')
-        prev_nodes = [('remove', i, pn) for i, pn in enumerate(diff['remove']) if pn.ntype not in ntypes_to_ignore]
-        curr_nodes = [('insert', j, cn) for j, cn in enumerate(diff['insert']) if cn.ntype not in ntypes_to_ignore]
-        for k in range(len(diff['change'])):
-            if diff['change'][k][0].ntype not in ntypes_to_ignore:
-                prev_nodes.append(('change', k, diff['change'][k][0]))
-                curr_nodes.append(('change', k, diff['change'][k][1]))
+        ntypes_to_ignore = ("Text", "Text Formatting", "List")
+        prev_nodes = [
+            ("remove", i, pn)
+            for i, pn in enumerate(diff["remove"])
+            if pn.ntype not in ntypes_to_ignore
+        ]
+        curr_nodes = [
+            ("insert", j, cn)
+            for j, cn in enumerate(diff["insert"])
+            if cn.ntype not in ntypes_to_ignore
+        ]
+        for k in range(len(diff["change"])):
+            if diff["change"][k][0].ntype not in ntypes_to_ignore:
+                prev_nodes.append(("change", k, diff["change"][k][0]))
+                curr_nodes.append(("change", k, diff["change"][k][1]))
 
         # loop through prev/curr nodes and look for matches. constraints:
         # * nodes can only match with one other node
         # * if a node is part of a change, make sure it's corresponding node is moved to insert/remove accordingly
         prev_moved = []
         curr_moved = []
         curr_found = set()
         change_to_insert = {}
         change_to_remove = {}
         for pet, pidx, pn in prev_nodes:
             for cet, cidx, cn in curr_nodes:
-                cid = f'{cet}-{cidx}'
+                cid = f"{cet}-{cidx}"
                 # same type/text and not already part of a move
-                if pn.ntype == cn.ntype and pn.content_hash == cn.content_hash and cid not in curr_found:
+                if (
+                    pn.ntype == cn.ntype
+                    and pn.content_hash == cn.content_hash
+                    and cid not in curr_found
+                ):
                     prev_moved.append((pet, pidx))
                     curr_moved.append((cet, cidx))
                     curr_found.add(cid)
-                    if pet == 'change':
-                        corresponding_changed_node = diff['change'][pidx][1]
+                    if pet == "change":
+                        corresponding_changed_node = diff["change"][pidx][1]
                         change_to_insert[pidx] = corresponding_changed_node
-                    if cet == 'change':
-                        corresponding_changed_node = diff['change'][cidx][0]
+                    if cet == "change":
+                        corresponding_changed_node = diff["change"][cidx][0]
                         change_to_remove[cidx] = corresponding_changed_node
                     break
 
         # populate move list
         # if from a change, make sure it also isn't set to be moved to insert/remove
-        diff['move'] = []
+        diff["move"] = []
         if prev_moved:
             for i in range(len(prev_moved)):
                 pet, pidx = prev_moved[i]
                 cet, cidx = curr_moved[i]
                 pn = diff[pet][pidx]
-                if pet == 'change':  # pn is not the node but tuple of (prev_node, curr_node)
+                if (
+                    pet == "change"
+                ):  # pn is not the node but tuple of (prev_node, curr_node)
                     pn = pn[0]
-                    if pidx in change_to_remove:  # don't add to remove -- was involved in its own move
+                    if (
+                        pidx in change_to_remove
+                    ):  # don't add to remove -- was involved in its own move
                         change_to_remove.pop(pidx)
                 cn = diff[cet][cidx]
-                if cet == 'change':
+                if cet == "change":
                     cn = cn[1]
                     if cidx in change_to_insert:
-                        change_to_insert.pop(cidx)  # don't add to insert -- was involved in its own move
-                diff['move'].append((pn, cn))
+                        change_to_insert.pop(
+                            cidx
+                        )  # don't add to insert -- was involved in its own move
+                diff["move"].append((pn, cn))
             moved = sorted(set(prev_moved + curr_moved), reverse=True)
             for et, idx in moved:
                 diff[et].pop(idx)
 
-            diff['insert'].extend(list(change_to_insert.values()))
-            diff['remove'].extend(list(change_to_remove.values()))
+            diff["insert"].extend(list(change_to_insert.values()))
+            diff["remove"].extend(list(change_to_remove.values()))
 
 
 class Diff:
     """
     Diff result with helper functions for post-processing / cleaning up the result
     """
 
     def __init__(self, nodes_removed, nodes_inserted, nodes_changed, nodes_moved):
         self.remove = [n.dump() for n in nodes_removed]
         self.insert = [n.dump() for n in nodes_inserted]
-        self.change = [{'prev': pn.dump(), 'curr': cn.dump()} for pn, cn in nodes_changed]
-        self.move = [{'prev': pn.dump(), 'curr': cn.dump()} for pn, cn in nodes_moved]
+        self.change = [
+            {"prev": pn.dump(), "curr": cn.dump()} for pn, cn in nodes_changed
+        ]
+        self.move = [{"prev": pn.dump(), "curr": cn.dump()} for pn, cn in nodes_moved]
         self.sections_p_to_c = {}
         self.sections_c_to_p = {}
         self.processed = False
 
     def post_process(self, sections_prev, sections_curr, lang):
         if not self.processed:
             self._section_mapping(sections_prev, sections_curr)
@@ -531,128 +609,166 @@
             self.processed = True
         return self.result
 
     def _build_result(self, sections_prev, sections_curr):
         sp = {}
         sc = {}
         for n in self.remove:
-            sec_name = n['section']
+            sec_name = n["section"]
             sp[sec_name] = sections_prev[sec_name]
         for n in self.insert:
-            sec_name = n['section']
+            sec_name = n["section"]
             # update name to section in previous revision for consistency (if it exists)
             sec_id = self.sections_c_to_p[sec_name] or sec_name
-            n['section'] = sec_id
+            n["section"] = sec_id
             sc[sec_id] = sections_curr[sec_name]
         for n in self.change + self.move:
-            pn = n['prev']
-            cn = n['curr']
-            psec_name = pn['section']
+            pn = n["prev"]
+            cn = n["curr"]
+            psec_name = pn["section"]
             sp[psec_name] = sections_prev[psec_name]
-            csec_name = cn['section']
+            csec_name = cn["section"]
             # update name to section in previous revision for consistency (if it exists)
             csec_id = self.sections_c_to_p[csec_name] or csec_name
-            cn['section'] = csec_id
+            cn["section"] = csec_id
             sc[csec_id] = sections_curr[csec_name]
 
-        self.result = {'remove': self.remove, 'insert': self.insert, 'change': self.change, 'move': self.move}
+        self.result = {
+            "remove": self.remove,
+            "insert": self.insert,
+            "change": self.change,
+            "move": self.move,
+        }
 
     def _section_mapping(self, sections_prev, sections_curr):
         """Build mapping of sections between previous and current versions of article."""
         prev = list(sections_prev.keys())
         curr = list(sections_curr.keys())
         p_to_c = {}
         c_to_p = {}
         removed = []
         # removed sections map to null in current; inserted sections map to null in previous
         for n in self.remove:
-            if n['type'] == 'Heading':
+            if n["type"] == "Section":
                 for i, s in enumerate(prev):
-                    if s == n['section']:
+                    if s == n["section"]:
                         removed.append(i)
                         break
         for idx in sorted(removed, reverse=True):
             p_to_c[prev[idx]] = None
             prev.pop(idx)
+
         inserted = []
         for n in self.insert:
-            if n['type'] == 'Heading':
+            if n["type"] == "Section":
                 for i, s in enumerate(curr):
-                    if s == n['section']:
+                    if s == n["section"]:
                         inserted.append(i)
                         break
         for idx in sorted(inserted, reverse=True):
             c_to_p[curr[idx]] = None
             curr.pop(idx)
 
         # changes happen in place so don't effect structure of doc and can be ignored
         # for moved sections, reorder mapping so they are aligned again for dumping
         for c in self.move:
-            pn = c['prev']
-            cn = c['curr']
-            if pn['type'] == 'Heading':
+            pn = c["prev"]
+            cn = c["curr"]
+            if pn["type"] == "Section":
                 prev_idx = None
                 curr_idx = None
                 for i, s in enumerate(prev):
-                    if s == pn['section']:
+                    if s == pn["section"]:
                         prev_idx = i
                         break
                 for i, s in enumerate(curr):
-                    if s == cn['section']:
+                    if s == cn["section"]:
                         curr_idx = i
                         break
                 if prev_idx is not None and curr_idx is not None:
                     s = curr.pop(curr_idx)
                     curr.insert(prev_idx, s)
 
         for i in range(len(prev)):
             p_to_c[prev[i]] = curr[i]
             c_to_p[curr[i]] = prev[i]
 
         self.sections_p_to_c = p_to_c
         self.sections_c_to_p = c_to_p
 
-    def _merge_text_changes(self, sections_prev, sections_curr, lang='en'):
+    def _merge_text_changes(self, sections_prev, sections_curr, lang="en"):
         """Replace isolated text changes with section-level text changes."""
         changes = []
         # check each previous section and add if not a match with its corresponding current section
         for psec in self.sections_p_to_c:
             csec = self.sections_p_to_c[psec]
             if csec is None:
                 prev_text = wikitext_to_plaintext(sections_prev[psec], lang=lang)
-                changes.append({'prev': {'name': node_to_name(prev_text), 'type': 'Text', 'text': prev_text,
-                                         'section': psec, 'offset': 0}})
+                changes.append(
+                    {
+                        "prev": {
+                            "name": node_to_name(prev_text),
+                            "type": "Text",
+                            "text": prev_text,
+                            "section": psec,
+                            "offset": 0,
+                        }
+                    }
+                )
             elif sections_prev[psec] != sections_curr[csec]:
                 prev_text = wikitext_to_plaintext(sections_prev[psec], lang=lang)
                 curr_text = wikitext_to_plaintext(sections_curr[csec], lang=lang)
                 if prev_text != curr_text:
-                    changes.append({'prev': {'name': node_to_name(prev_text), 'type': 'Text', 'text': prev_text,
-                                             'section': psec, 'offset': 0},
-                                    'curr': {'name': node_to_name(curr_text), 'type': 'Text', 'text': curr_text,
-                                             'section': csec, 'offset': 0}})
+                    changes.append(
+                        {
+                            "prev": {
+                                "name": node_to_name(prev_text),
+                                "type": "Text",
+                                "text": prev_text,
+                                "section": psec,
+                                "offset": 0,
+                            },
+                            "curr": {
+                                "name": node_to_name(curr_text),
+                                "type": "Text",
+                                "text": curr_text,
+                                "section": csec,
+                                "offset": 0,
+                            },
+                        }
+                    )
         # add in unmatched sections from current (new sections)
         for csec in self.sections_c_to_p:
             psec = self.sections_c_to_p[csec]
             if psec is None:
                 curr_text = wikitext_to_plaintext(sections_curr[csec], lang=lang)
-                changes.append({'curr': {'name': node_to_name(curr_text), 'type': 'Text', 'text': curr_text,
-                                         'section': csec, 'offset': 0}})
+                changes.append(
+                    {
+                        "curr": {
+                            "name": node_to_name(curr_text),
+                            "type": "Text",
+                            "text": curr_text,
+                            "section": csec,
+                            "offset": 0,
+                        }
+                    }
+                )
 
         # remove individual text changes
         for idx in range(len(self.remove) - 1, -1, -1):
-            if self.remove[idx]['type'] == 'Text':
+            if self.remove[idx]["type"] == "Text":
                 self.remove.pop(idx)
         for idx in range(len(self.insert) - 1, -1, -1):
-            if self.insert[idx]['type'] == 'Text':
+            if self.insert[idx]["type"] == "Text":
                 self.insert.pop(idx)
         for idx in range(len(self.change) - 1, -1, -1):
-            if self.change[idx]['prev']['type'] == 'Text':
+            if self.change[idx]["prev"]["type"] == "Text":
                 self.change.pop(idx)
 
         # add in section-level text changes
         for c in changes:
-            if 'prev' in c and 'curr' in c:
+            if "prev" in c and "curr" in c:
                 self.change.append(c)
-            elif 'prev' in c:
-                self.remove.append(c['prev'])
-            elif 'curr' in c:
-                self.insert.append(c['curr'])
+            elif "prev" in c:
+                self.remove.append(c["prev"])
+            elif "curr" in c:
+                self.insert.append(c["curr"])
```

### Comparing `mwedittypes-2.1.0/mwedittypes/utils.py` & `mwedittypes-2.1.1/mwedittypes/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,123 @@
 # helper functions for handling mwparserfromhell / wikitext
 import re
 
 import mwparserfromhell as mw
 
-from mwedittypes.constants import *
+from mwedittypes.constants import (
+    CAT_ALIASES,
+    CAT_PREFIXES,
+    EXTEN_PATTERN,
+    LIST_TAGS,
+    MEDIA_ALIASES,
+    MEDIA_PREFIXES,
+    TABLE_ELEMENTS_TAGS,
+    TEXT_FORMATTING_TAGS,
+)
 
 
-def simple_node_class(mwnode, lang='en'):
+def simple_node_class(mwnode, lang="en"):
     """e.g., "<class 'mwparserfromhell.nodes.heading.Heading'>" -> "Heading"."""
     if type(mwnode) == str:
-        return 'Text'
+        return "Text"
     else:
-        nc = str(type(mwnode)).split('.')[-1].split("'")[0]
-        if nc == 'Wikilink':
-            n_prefix = mwnode.title.split(':', maxsplit=1)[0].lower()
-            if n_prefix in [m.lower() for m in MEDIA_PREFIXES + MEDIA_ALIASES.get(lang, [])]:
-                nc = 'Media'
-            elif n_prefix in [c.lower() for c in CAT_PREFIXES + CAT_ALIASES.get(lang, [])]:
-                nc = 'Category'
-        elif nc == 'Tag':
+        nc = str(type(mwnode)).split(".")[-1].split("'")[0]
+        if nc == "Wikilink":
+            n_prefix = mwnode.title.split(":", maxsplit=1)[0].lower()
+            if n_prefix in [
+                m.lower() for m in MEDIA_PREFIXES + MEDIA_ALIASES.get(lang, [])
+            ]:
+                nc = "Media"
+            elif n_prefix in [
+                c.lower() for c in CAT_PREFIXES + CAT_ALIASES.get(lang, [])
+            ]:
+                nc = "Category"
+        elif nc == "Tag":
             tag_type = str(mwnode.tag).lower()
             if tag_type in TEXT_FORMATTING_TAGS:
-                return 'Text Formatting'
+                return "Text Formatting"
             elif tag_type in LIST_TAGS:
-                return 'List'
-            elif tag_type == 'table':
-                return 'Table'
+                return "List"
+            elif tag_type == "table":
+                return "Table"
             elif tag_type in TABLE_ELEMENTS_TAGS:
-                return 'Table Element'
-            elif tag_type == 'gallery':
-                return 'Gallery'
-            elif tag_type == 'ref':
-                return 'Reference'
-            elif tag_type == 'noinclude':
-                return 'Comment'
+                return "Table Element"
+            elif tag_type == "gallery":
+                return "Gallery"
+            elif tag_type == "ref":
+                return "Reference"
+            elif tag_type == "noinclude":
+                return "Comment"
             # any others I missed -- e.g., div, meta, etc.
             else:
-                return 'Other Tag'
+                return "Other Tag"
         return nc
 
 
 def sec_to_name(mwsection, sidx):
     """Converts a section to an interpretible and unique name."""
     if sidx == 0:
-        sectitle = 'Lede'
+        sectitle = "Lede"
     else:
         try:
             sectitle = str(mwsection.nodes[0])
         except IndexError:
-            sectitle = ''
-    return f'{sidx}: {sectitle}'
+            sectitle = ""
+    return f"{sidx}: {sectitle}"
 
 
-def node_to_name(mwnode, lang='en'):
+def node_to_name(mwnode, lang="en"):
     """Converts a mwparserfromhell node to an interpretible name."""
     n_txt = mwnode.replace("\n", "\\n")
     if len(n_txt) > 13:
-        return f'{simple_node_class(mwnode, lang)}: {n_txt[:10]}...'
+        return f"{simple_node_class(mwnode, lang)}: {n_txt[:10]}..."
     else:
-        return f'{simple_node_class(mwnode, lang)}: {n_txt}'
+        return f"{simple_node_class(mwnode, lang)}: {n_txt}"
 
 
-def wikitext_to_plaintext(wt, lang='en'):
+def wikitext_to_plaintext(wt, lang="en"):
     """Helper function for converting wikitext to plaintext.
 
     Removes text-formatting syntax (italic '', bold ''', bold-italic ''''') from nodes because
     skip_style_tags is set to True and so these syntax are treated as text by mwparserfromhell.
     This is to avoid parsing issues that arise from unclosed text-formatting syntax.
     """
-    return ''.join([re.sub("'{2,}", "", extract_text(n, lang)) for n in mw.parse(wt, skip_style_tags=True).nodes])
+    return "".join(
+        [
+            re.sub("'{2,}", "", extract_text(n, lang))
+            for n in mw.parse(wt, skip_style_tags=True).nodes
+        ]
+    )
 
 
-def extract_text(mwnode, lang='en'):
+def extract_text(mwnode, lang="en"):
     """Extract what text would be displayed from any node."""
     ntype = simple_node_class(mwnode, lang)
-    if ntype == 'Text':
+    if ntype == "Text":
         return str(mwnode)
-    elif ntype == 'HTMLEntity':
+    elif ntype == "HTMLEntity":
         return mwnode.normalize()
-    elif ntype == 'Wikilink':
+    elif ntype == "Wikilink":
         if mwnode.text:
             return mwnode.text.strip_code()
         else:
             return mwnode.title.strip_code()
-    elif ntype == 'ExternalLink' and mwnode.title:
+    elif ntype == "ExternalLink" and mwnode.title:
         return mwnode.title.strip_code()
     # tables can have tons of nested references etc. so can't just go through standard strip_code
-    elif ntype == 'Table':
+    elif ntype == "Table":
         # don't collapse whitespace for tables because otherwise strip_code sometimes merges text across cells
         return mwnode.contents.strip_code(collapse=False)
-    elif ntype == 'Text Formatting':
-        return ''.join(extract_text(mwn) for mwn in mwnode.contents.nodes)
-    # Heading, Template, Comment, Argument, Category, Media, References, URLs without display text
+    elif ntype == "Text Formatting":
+        return "".join(extract_text(mwn) for mwn in mwnode.contents.nodes)
+    # Article, Section, Heading, Template, Comment, Argument, Category, Media, References, URLs without display text
     # Tags not listed here (div, gallery, etc.) that almost never have true text content and can be super messy
     # Table elements (they duplicate the text if included)
     else:
-        return ''
+        return ""
 
 
 def find_nested_media(wikitext, is_gallery=False, max_link_length=240):
     """Case-insensitive search for media files (lacking brackets) in wikitext -- i.e. in Templates and Galleries.
     For setting max_link_length: https://commons.wikimedia.org/wiki/Commons:File_naming#Length
 
     In templates, image name is a parameter and all formatting/caption options are separate parameters
@@ -116,21 +134,21 @@
         m = EXTEN_PATTERN.search(lc_wt, pos=end)
         if m is None:
             break
         start, end = m.span()
         if end - start <= max_link_length:
             media_wikitext = wikitext[start:end]
             if is_gallery:
-                end_of_line = wikitext.find('\n', end)
+                end_of_line = wikitext.find("\n", end)
                 if end_of_line == -1:  # no new-line at end of gallery
                     media_options = wikitext[end:]
                 else:
                     media_options = wikitext[end:end_of_line]
                 media_wikitext += media_options
-            yield(media_wikitext.strip())
+            yield (media_wikitext.strip())
 
 
 def find_nested_textformatting(wikitext):
     """Context-insensitive search for likely text-formatting in wikitext.
 
     Specifically, there are three viable options:
     ''italics'' (2 '), '''bold''' (3 '), and '''''bold-italic''''' (5 ')
@@ -140,43 +158,43 @@
     text-formatting that are 2, 3, or 5 ' and treat them as text-formatting regardless
     of whether they are the start or end of a block (which is not knowable). The number
     of final text-formatting nodes across an entire article then has to be divided by
     two to reach a more accurate count of how many text-formatting blocks there are.
     """
     if "''" in wikitext:
         for tf in re.finditer("'{2,5}", wikitext):
-            yield(tf.group(), tf.span())
+            yield (tf.group(), tf.span())
 
 
 def full_diff_to_simple(full_diff):
     """Extract simple edit type summary from full edit type response."""
     result = {}
-    for ne in full_diff['node-edits']:
+    for ne in full_diff["node-edits"]:
         if ne.type not in result:
             result[ne.type] = {}
         result[ne.type][ne.edittype] = result[ne.type].get(ne.edittype, 0) + 1
     te_types = set()
-    for te in full_diff['text-edits']:
+    for te in full_diff["text-edits"]:
         if te.type not in result:
             result[te.type] = {}
             te_types.add(te.type)
         result[te.type][te.edittype] = result[te.type].get(te.edittype, 0) + te.count
     for tet in te_types:
-        change = min(result[tet].get('insert', 0), result[tet].get('remove', 0))
+        change = min(result[tet].get("insert", 0), result[tet].get("remove", 0))
         if change:
-            result[tet]['change'] = change
-            if 'insert' in result[tet]:
-                if result[tet]['insert'] == change:
-                    result[tet].pop('insert')
+            result[tet]["change"] = change
+            if "insert" in result[tet]:
+                if result[tet]["insert"] == change:
+                    result[tet].pop("insert")
                 else:
-                    result[tet]['insert'] = result[tet]['insert'] - change
-            if 'remove' in result[tet]:
-                if result[tet]['remove'] == change:
-                    result[tet].pop('remove')
+                    result[tet]["insert"] = result[tet]["insert"] - change
+            if "remove" in result[tet]:
+                if result[tet]["remove"] == change:
+                    result[tet].pop("remove")
                 else:
-                    result[tet]['remove'] = result[tet]['remove'] - change
-    for ce in full_diff['context']:
+                    result[tet]["remove"] = result[tet]["remove"] - change
+    for ce in full_diff["context"]:
         if ce.type not in result:
             result[ce.type] = {}
         result[ce.type][ce.edittype] = result[ce.type].get(ce.edittype, 0) + ce.count
 
     return result
```

### Comparing `mwedittypes-2.1.0/mwedittypes.egg-info/PKG-INFO` & `mwedittypes-2.1.1/mwedittypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwedittypes
-Version: 2.1.0
+Version: 2.1.1
 Summary: Edit diffs and type detection for Wikipedia
 Home-page: https://github.com/geohci/edit-types
 Author: geohci & Amamgbu (Isaac Johnson & Jesse Amamgbu)
 Author-email: <amamgbujesse@yahoo.com>
 License: MIT License
 Keywords: python,wikipedia,edit types,edit diffs,wiki,edit detection
 Classifier: Development Status :: 4 - Beta
@@ -84,29 +84,29 @@
                          changes=[('parameter', ('1', 'Austrian painter'), ('1', 'Austrian [[landscape painter]]'))])],
  'text-edits': []}
 ```
 
 In most cases (~90%), the two approaches agree in their overall results. They differ in the following situations:
 * Very large diffs -- when `timeout` is set to `True`, the StructuredEditTypes class is more likely to fall-back to a simple diff and miss some details as a result
 * Content moves -- the simplified library cannot detect moves
-* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted 
+* Changes vs. Inserts+Removes -- the simplified library does not distinguish between e.g., a template being changed vs. a template being removed and separate template being inserted
 
 A good example of a diff where they vary in outputs is revision 1107840666 on English Wikipedia ([diff](https://en.wikipedia.org/w/index.php?diff=1107840666&oldid=1094519551&title=Blumenthal,_Saskatchewan&diffmode=source); [model output](https://wiki-topic.toolforge.org/diff-tagging?lang=en&revid=1107840666)).
 
 ## Language Coverage
 Almost everything in this library is language-agnostic and so works consistently for any language of Wikipedia.
 For links, the namespace identification varies but we use a list of prefixes that covers all languages (at the time of generation).
 Sentences are semi-challenging in that we must build a list of sentence-ending punctuation that covers all languages. We believe we have done a good job of this but have not explicitly tested this. The list can be found in `mwedittypes/constants.py` under `SENTENCE_BREAKS_REGEX`.
 Words are the most challenging aspect and the one place where you will see varying behavior. For them we take two strategies:
 * For most languages, we split text based on whitespace. This is the default behavior.
 * There are many languages that either don't separate words with whitespace or use whitespace to instead delineate syllables. These can be found in `mwedittypes/constants.py` under `NON_WHITESPACE_LANGUAGES`. For these languages, we instead report the number of characters affected.
 
 ## Known Issues
 Wikitext/language is verrrrrrry complicated and so there are certain things we can't feasibly extract consistently. The ones we know about:
-* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence. 
+* Sentences: full stop punctuation is used for [many things](https://en.wikipedia.org/wiki/Full_stop#Usage). Abbreviations are particularly challenging and will falsely split up sentences. On the other hand, Thai has no sentence punctuation so each paragraph is (incorrectly) considered the equivalent of a single sentence.
 * Words: we have done our best to extract words for whitespace-delimited languages but some languages use special spacing characters that may falsely split up words -- e.g., Bengali. We have done our best to detect account for these languages but may have missed some.
 * Media: images/audio/video can be included in articles via bracketed links, templates, and galleries. Each have their own syntax, and, in particular templates separate the image name from its formatting options. For galleries/bracket-links, we associate the formatting/caption options with the media and changes to them will trigger as media changes. For templates, we cannot do this.
 * Text Formatting: parsing text formatting is quite complicated and context-dependent. We parse the wikitext section-by-section so text formatting split up between sections might parse unexpectedly.
 
 For links, we assume that if the prefix is not for media or a category, the link is a wikilink to namespace 0. This is generally reasonable for current versions of Wikipedia articles
 but would overload the `Wikilink` class with e.g., user page links on talk pages or interwiki links for older versions of articles.
 
@@ -152,8 +152,7 @@
 * If something fails, you can always rollback the release (Github UI) and delete the associated tag (on your local repository: `git tag -d [tag]; git push origin :[tag]`) and retry.
 * This relies on a PyPi secret so you must have correct privileges on the Github repo.
 
 ## Documentation
 * For more background, see: https://meta.wikimedia.org/wiki/Research:Wikipedia_Edit_Types
 * To test out the code, see: https://wiki-topic.toolforge.org/diff-tagging?lang=en
 * To see how the code is used in an API, see: https://github.com/wikimedia/research-api-endpoint-template/tree/edit-types
-
```

### Comparing `mwedittypes-2.1.0/mwedittypes.egg-info/SOURCES.txt` & `mwedittypes-2.1.1/mwedittypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.1.0/setup.py` & `mwedittypes-2.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-from setuptools import setup, find_packages
 import codecs
 import os
 
+from setuptools import find_packages, setup
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.0'
-DESCRIPTION = 'Edit diffs and type detection for Wikipedia'
-LONG_DESCRIPTION = 'A package that allows edit diffs and type detection for Wikipedia.'
+VERSION = "2.1.1"
+DESCRIPTION = "Edit diffs and type detection for Wikipedia"
+LONG_DESCRIPTION = "A package that allows edit diffs and type detection for Wikipedia."
 
 # Dev dependencies
 EXTRAS_REQUIRE = {
     "tests": ["pytest>=6.2.5"],
 }
 
-EXTRAS_REQUIRE["dev"] = (
-    EXTRAS_REQUIRE["tests"]
-)
+EXTRAS_REQUIRE["dev"] = EXTRAS_REQUIRE["tests"]
 
 # Setting up
 setup(
     name="mwedittypes",
     version=VERSION,
     author="geohci & Amamgbu (Isaac Johnson & Jesse Amamgbu)",
     author_email="<amamgbujesse@yahoo.com>",
     url="https://github.com/geohci/edit-types",
     license="MIT License",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['mwparserfromhell', 'anytree', 'mwconstants'],
-    keywords=['python', 'wikipedia', 'edit types', 'edit diffs', 'wiki', 'edit detection'],
+    install_requires=["mwparserfromhell", "anytree", "mwconstants"],
+    keywords=[
+        "python",
+        "wikipedia",
+        "edit types",
+        "edit diffs",
+        "wiki",
+        "edit detection",
+    ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-        
     ],
     extras_require=EXTRAS_REQUIRE,
     include_package_data=True,
     zip_safe=False,
-)
+)
```

### Comparing `mwedittypes-2.1.0/tests/test_edittypes_structured.py` & `mwedittypes-2.1.1/tests/test_edittypes_structured.py`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.1.0/tests/test_edittypes_summary.py` & `mwedittypes-2.1.1/tests/test_edittypes_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import pytest
+from context import (
+    SimpleEditTypes,
+    StructuredEditTypes,
+    cjk_prev_wikitext,
+    full_diff_to_simple,
+    prev_wikitext,
+)
 
-from context import cjk_prev_wikitext, StructuredEditTypes, full_diff_to_simple, prev_wikitext, SimpleEditTypes
 
 # Text tests
 def test_text_change():
     curr_wikitext = prev_wikitext.replace('Aigen was born in Olomouc on 8 October 1685, the son of a goldsmith.',
                                           'Aigen-Abe was born in Olomouc on 9 October 1685, the daughter of a goldsmith.',
                                           1)
     expected_changes = {'Paragraph': {'change': 1}, 'Sentence': {'change': 1}, 'Word': {'change': 3},
@@ -65,20 +71,20 @@
     expected_changes = {'Text Formatting': {'insert': 1}, 'Reference': {'insert': 1}, 'ExternalLink': {'insert': 1},
                         'Section': {'change': 1}}
     diff = SimpleEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
     assert diff == expected_changes
     full_diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
     assert full_diff_to_simple(full_diff) == expected_changes
 
-@pytest.mark.xfail(reason="Tree Differ can't currently detect simple shifts in text formatting start-stops.")
+@pytest.mark.xfail(reason="Differs can't currently detect simple shifts in text formatting start-stops.")
 def test_change_formatting_length():
     curr_wikitext = prev_wikitext.replace("'''Karl Josef Aigen''' (8 October 1684 – 22 October 1762) was a landscape painter, born at",
                                           "'''Karl Josef Aigen (8 October 1684 – 22 October 1762) was a landscape painter, born at'''",
                                           1)
-    expected_changes = {'Section': {'change': 1}}
+    expected_changes = {'Section': {'change': 1}, 'Text Formatting': {'change': 1}}
     diff = SimpleEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
     assert diff == expected_changes
     full_diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff = full_diff.get_diff()
     assert full_diff_to_simple(diff) == expected_changes
 
 
@@ -295,26 +301,30 @@
     curr_wikitext = prev_wikitext.replace("\nHe died at Vienna",
                                           "===Death===\nHe died at Vienna",
                                           1)
     # category change in later section
     curr_wikitext = curr_wikitext.replace("[[Category:Artists from Olomouc]]",
                                           "[[Category:Artists in Olomouc]]",
                                           1)
-    expected_changes = {'Heading': {'insert': 1}, 'Category': {'change': 1}, 'Section': {'insert': 1, 'change': 2}}
+    simple_expected_changes = {'Heading': {'insert': 1}, 'Category': {'change': 1},
+                                   'Section': {'insert': 1, 'change': 2}}
     diff = SimpleEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
-    assert diff == expected_changes
+    assert diff == simple_expected_changes
+    # NOTE: simple expected changes are a bit more realistic but this is acceptable
+    structured_expected_changes = {'Heading': {'insert': 1}, 'Category': {'change': 1},
+                        'Section': {'insert': 2, 'change': 1, 'remove': 1}}
     full_diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
-    assert full_diff_to_simple(full_diff) == expected_changes
+    assert full_diff_to_simple(full_diff) == structured_expected_changes
 
 
 def test_moved_section():
     # swap Works and References sections with no other changess
     curr_wikitext = prev_wikitext.replace(
         "\n\n===Works===\nThe [[Österreichische Galerie Belvedere|Gallery of the Belvedere]] in Vienna has two works by him, both scenes with figures.<ref>{{Bryan (3rd edition)|title=Aigen, Karl |volume=1}}</ref>\n\n==References==\n{{reflist}}",
         "\n\n==References==\n{{reflist}}\n\n===Works===\nThe [[Österreichische Galerie Belvedere|Gallery of the Belvedere]] in Vienna has two works by him, both scenes with figures.<ref>{{Bryan (3rd edition)|title=Aigen, Karl |volume=1}}</ref>",
         1)
     simple_expected_changes = {}
-    full_expected_changes = {'Section':{'move':1, 'change':2}}
+    full_expected_changes = {'Section':{'move':1}}
     diff = SimpleEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
     assert diff == simple_expected_changes
     full_diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en').get_diff()
     assert full_diff_to_simple(full_diff) == full_expected_changes
```

### Comparing `mwedittypes-2.1.0/tests/test_tokenizer.py` & `mwedittypes-2.1.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.1.0/tests/test_tree_differ.py` & `mwedittypes-2.1.1/tests/test_tree_differ.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,57 +27,63 @@
     assert not errors
 
 
 def test_insert_category():
     curr_wikitext = prev_wikitext.replace('[[Category:Artists from Olomouc]]\n',
                                           '[[Category:Artists from Olomouc]]\n[[Category:TEST CATEGORY]]',
                                           1)
-    expected_changes = [('insert', '4: ==External links==', 'Category')]
+    expected_changes = [('insert', '4: ==External links==', 'Category'),
+                        ('change', '4: ==External links==', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 def test_insert_link():
     curr_wikitext = prev_wikitext.replace('He was a pupil of the Olomouc painter',
                                           'He was a [[pupil]] of the Olomouc painter',
                                           1)
-    expected_changes = [('insert', '1: ==Life==', 'Wikilink')]
+    expected_changes = [('insert', '1: ==Life==', 'Wikilink'),
+                        ('change', '1: ==Life==', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 def test_move_template():
     curr_wikitext = prev_wikitext.replace('{{Austria-painter-stub}}',
                                           '',
                                           1)
     curr_wikitext = '{{Austria-painter-stub}}' + curr_wikitext
-    expected_changes = [('move', '4: ==External links==', 'Template')]
+    expected_changes = [('move', '4: ==External links==', 'Template'),
+                        ('change', '4: ==External links==', 'Section'),
+                        ('change', '0: Lede', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 def test_change_heading():
     curr_wikitext = prev_wikitext.replace('===Works===',
                                           '===NotWorks===',
                                           1)
-    expected_changes = [('change', '2: ===Works===', 'Heading')]
+    expected_changes = [('change', '2: ===Works===', 'Heading'),
+                        ('change', '2: ===Works===', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 def test_remove_formatting():
     curr_wikitext = prev_wikitext.replace("'''Karl Josef Aigen'''",
                                           "Karl Josef Aigen",
                                           1)
     # two tf-spans removed; won't be reduced to a single block until the node differ
-    expected_changes = [('remove', '0: Lede', 'Text Formatting'), ('remove', '0: Lede', 'Text Formatting')]
+    expected_changes = [('remove', '0: Lede', 'Text Formatting'), ('remove', '0: Lede', 'Text Formatting'),
+                        ('change', '0: Lede', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 table = """{| border="1" cellspacing="0" cellpadding="5"
 |- bgcolor="#cccccc"
@@ -110,15 +116,16 @@
     expected_changes = [('insert', '4: ==External links==', 'Table'),
                         ('change', '4: ==External links==', 'Text'),
                         ('insert', '4: ==External links==', 'Wikilink'),
                         ('insert', '4: ==External links==', 'Wikilink'),
                         ('insert', '4: ==External links==', 'Text Formatting'),
                         ('insert', '4: ==External links==', 'Text Formatting'),
                         ('insert', '4: ==External links==', 'Text Formatting'),
-                        ('insert', '4: ==External links==', 'Text Formatting')]
+                        ('insert', '4: ==External links==', 'Text Formatting'),
+                        ('change', '4: ==External links==', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 gallery = """<gallery widths="190px" heights="190px" perrow="4">
 File:Lucas Cranach d.Ä. - Bildnis des Moritz Büchner.jpg|[[Lucas Cranach the Elder]], ''Portrait of Moritz'', 1518
@@ -129,20 +136,22 @@
     curr_wikitext = prev_wikitext + '\n' + gallery
     # two tf-spans removed; won't be reduced to a single block until the node differ
     expected_changes = [('insert', '4: ==External links==', 'Gallery'),
                         ('change', '4: ==External links==', 'Text'),
                         ('insert', '4: ==External links==', 'Media'),
                         ('insert', '4: ==External links==', 'Wikilink'),
                         ('insert', '4: ==External links==', 'Text Formatting'),
-                        ('insert', '4: ==External links==', 'Text Formatting')]
+                        ('insert', '4: ==External links==', 'Text Formatting'),
+                        ('change', '4: ==External links==', 'Section')]
     diff = StructuredEditTypes(prev_wikitext, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
 
 
 def test_table_change():
     curr_wikitext = table.replace('general election', 'gen elec', 1)
     expected_changes = [('change', '0: Lede', 'Wikilink'),
-                        ('change', '0: Lede', 'Table')]
+                        ('change', '0: Lede', 'Table'),
+                        ('change', '0: Lede', 'Section')]
     diff = StructuredEditTypes(table, curr_wikitext, lang='en')
     diff.get_diff()
     check_change_counts(diff.tree_diff, expected_changes)
```

