# Comparing `tmp/docx_charts-0.1.8.tar.gz` & `tmp/docx_charts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.8.tar", max compression
+gzip compressed data, was "docx_charts-0.1.9.tar", max compression
```

## Comparing `docx_charts-0.1.8.tar` & `docx_charts-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.8/LICENSE
--rw-r--r--   0        0        0      490 2023-07-18 19:42:35.683348 docx_charts-0.1.8/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.8/docx_charts/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-18 20:06:11.157424 docx_charts-0.1.8/docx_charts/chart.py
--rw-r--r--   0        0        0     2860 2023-07-18 20:03:48.566416 docx_charts-0.1.8/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-18 20:07:58.752430 docx_charts-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 docx_charts-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.9/LICENSE
+-rw-r--r--   0        0        0      620 2023-07-18 20:18:57.867465 docx_charts-0.1.9/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.9/docx_charts/__init__.py
+-rw-r--r--   0        0        0     3518 2023-07-18 21:27:44.124685 docx_charts-0.1.9/docx_charts/chart.py
+-rw-r--r--   0        0        0     2860 2023-07-18 21:22:35.413669 docx_charts-0.1.9/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-18 21:29:04.100690 docx_charts-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 docx_charts-0.1.9/PKG-INFO
```

### Comparing `docx_charts-0.1.8/LICENSE` & `docx_charts-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.8/docx_charts/chart.py` & `docx_charts-0.1.9/docx_charts/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Series = dict[str, float]  # category: value
 ChartData = dict[str, Series]  # series_name: Series
 
 
 def series_name(series: minidom.Element) -> str | None:
 	if not series.getElementsByTagName('c:tx'):
 		return None
-	return series.getElementsByTagName('c:tx')[0].getElementsByTagName('c:v')[0].firstChild.nodeValue.lower().replace(' ', '_')  # type: ignore
+	return series.getElementsByTagName('c:tx')[0].getElementsByTagName('c:v')[0].firstChild.nodeValue  # type: ignore
 
 
 class Chart:
 	'''
 	Represents a chart in a Word document.
 
 	Attributes:
@@ -60,15 +60,15 @@
 		Gets the internal table data the chart is based on.
 
 		Returns:
 			A dictionary of Series dicts representing data for the chart.
 		'''
 		dom = minidom.parse(self.file)
 		series = {
-			series_name(series) or f'series{i+1}':
+			series_name(series) or f'Series{i+1}':
 			dict(zip(
 				[cat.firstChild.nodeValue for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 					if cat.firstChild and isinstance(cat.firstChild, minidom.Text) and isinstance(cat.firstChild.nodeValue, str)],
 				[float(val.firstChild.nodeValue) for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 					if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 			))
 			for i, series in enumerate(dom.getElementsByTagName('c:ser'))
@@ -88,25 +88,25 @@
 			The names of the series and categories must be the same as in the original data.
 			However, unchanged series and categories may be left out.
 		'''
 		dom = minidom.parse(self.file)
 
 		for (new_series_name, new_series) in data.items():
 			try:
-				series = [series for i, series in enumerate(dom.getElementsByTagName('c:ser')) if (series_name(series) or f'series{i+1}') == new_series_name][0]
+				series = [series for i, series in enumerate(dom.getElementsByTagName('c:ser')) if (series_name(series) or f'Series{i+1}') == new_series_name][0]
 			except IndexError:
-				raise ValueError(f'Chart {self.name} does not contain a series named {new_series_name}.')
+				raise ValueError(f'Chart "{self.name}" does not contain a series named "{new_series_name}".')
 			cats = [cat.firstChild for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 				if cat.firstChild and isinstance(cat.firstChild, minidom.Text)]
 			vals = [val.firstChild for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 				if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 
 			for new_cat, new_val in new_series.items():
 				if new_cat not in [cat.nodeValue for cat in cats]:
-					raise ValueError(f'Chart {self.name} does not contain a category named {new_cat}.')
+					raise ValueError(f'Chart "{self.name}" does not contain a category named "{new_cat}".')
 				for cat, val in zip(cats, vals):
 					if cat.nodeValue == new_cat:
 						val.replaceWholeText(str(new_val))
 						break
 
 		self.file.seek(0)
 		self.file.truncate()
```

### Comparing `docx_charts-0.1.8/docx_charts/document.py` & `docx_charts-0.1.9/docx_charts/document.py`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.8/PKG-INFO` & `docx_charts-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646f 6378  : 2.1.Name: docx
 00000020: 2d63 6861 7274 730a 5665 7273 696f 6e3a  -charts.Version:
-00000030: 2030 2e31 2e38 0a53 756d 6d61 7279 3a20   0.1.8.Summary: 
+00000030: 2030 2e31 2e39 0a53 756d 6d61 7279 3a20   0.1.9.Summary: 
 00000040: 5079 7468 6f6e 206c 6962 7261 7279 2066  Python library f
 00000050: 6f72 206d 616e 6970 756c 6174 696e 6720  or manipulating 
 00000060: 6368 6172 7420 6461 7461 2069 6e20 776f  chart data in wo
 00000070: 7264 2064 6f63 756d 656e 7473 0a41 7574  rd documents.Aut
 00000080: 686f 723a 204a 756c 6961 2076 616e 2064  hor: Julia van d
 00000090: 6572 204b 7269 730a 4175 7468 6f72 2d65  er Kris.Author-e
 000000a0: 6d61 696c 3a20 6a75 6c69 6140 6a75 7575  mail: julia@juuu
@@ -20,38 +20,46 @@
 00000130: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
 00000140: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000150: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 00000160: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
 00000170: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000180: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 00000190: 6172 6b64 6f77 6e0a 0a23 2064 6f63 782d  arkdown..# docx-
-000001a0: 6368 6172 7473 0a0a 5079 7468 6f6e 206c  charts..Python l
-000001b0: 6962 7261 7279 2066 6f72 206d 616e 6970  ibrary for manip
-000001c0: 756c 6174 696e 6720 6368 6172 7420 6461  ulating chart da
-000001d0: 7461 2069 6e20 776f 7264 2064 6f63 756d  ta in word docum
-000001e0: 656e 7473 0a0a 4469 7363 6c61 696d 6572  ents..Disclaimer
-000001f0: 3a20 7468 6973 2069 7320 6120 7072 6f6a  : this is a proj
-00000200: 6563 7420 6d61 6465 2066 6f72 2061 2076  ect made for a v
-00000210: 6572 7920 7370 6563 6966 6963 2075 7365  ery specific use
-00000220: 6361 7365 2c20 6265 6361 7573 6520 6e6f  case, because no
-00000230: 7468 696e 6720 6265 7474 6572 2065 7869  thing better exi
-00000240: 7374 6564 2079 6574 2e20 4e6f 2073 7461  sted yet. No sta
-00000250: 6269 6c69 7479 2067 7561 7261 6e74 6565  bility guarantee
-00000260: 7320 6172 6520 6d61 6465 2c20 616e 6420  s are made, and 
-00000270: 7468 6520 4150 4920 6973 2073 7562 6a65  the API is subje
-00000280: 6374 2074 6f20 6368 616e 6765 203a 290a  ct to change :).
-00000290: 0a26 6e62 7370 3b0a 0a23 2045 7861 6d70  .&nbsp;..# Examp
-000002a0: 6c65 0a60 6060 7079 0a66 726f 6d20 646f  le.```py.from do
-000002b0: 6378 5f63 6861 7274 7320 696d 706f 7274  cx_charts import
-000002c0: 2044 6f63 756d 656e 740a 0a64 6f63 203d   Document..doc =
-000002d0: 2044 6f63 756d 656e 7428 2765 7861 6d70   Document('examp
-000002e0: 6c65 2e64 6f63 7827 290a 6368 6172 7420  le.docx').chart 
-000002f0: 3d20 646f 632e 6669 6e64 5f63 6861 7274  = doc.find_chart
-00000300: 735f 6279 5f6e 616d 6528 2743 6861 7274  s_by_name('Chart
-00000310: 2031 2729 5b30 5d0a 6461 7461 203d 2063   1')[0].data = c
-00000320: 6861 7274 2e64 6174 6128 290a 6461 7461  hart.data().data
-00000330: 5b27 7374 7564 656e 745f 746f 7461 6c27  ['student_total'
-00000340: 5d5b 2743 5442 3130 3032 204c 696e 6561  ]['CTB1002 Linea
-00000350: 7220 416c 6765 6272 6127 5d20 3d20 302e  r Algebra'] = 0.
-00000360: 360a 6368 6172 742e 7772 6974 6528 6461  6.chart.write(da
-00000370: 7461 290a 646f 632e 7361 7665 2829 0a60  ta).doc.save().`
-00000380: 6060 0a0a                                ``..
+000001a0: 6368 6172 7473 0a0a 3c61 2068 7265 663d  charts..<a href=
+000001b0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000001c0: 672f 7072 6f6a 6563 742f 646f 6378 2d63  g/project/docx-c
+000001d0: 6861 7274 732f 223e 0a09 3c69 6d67 2073  harts/">..<img s
+000001e0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000001f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000200: 762f 646f 6378 5f63 6861 7274 733f 6c61  v/docx_charts?la
+00000210: 6265 6c3d 646f 6378 2d63 6861 7274 7322  bel=docx-charts"
+00000220: 202f 3e0a 3c2f 613e 0a0a 5079 7468 6f6e   />.</a>..Python
+00000230: 206c 6962 7261 7279 2066 6f72 206d 616e   library for man
+00000240: 6970 756c 6174 696e 6720 6368 6172 7420  ipulating chart 
+00000250: 6461 7461 2069 6e20 776f 7264 2064 6f63  data in word doc
+00000260: 756d 656e 7473 0a0a 4469 7363 6c61 696d  uments..Disclaim
+00000270: 6572 3a20 7468 6973 2069 7320 6120 7072  er: this is a pr
+00000280: 6f6a 6563 7420 6d61 6465 2066 6f72 2061  oject made for a
+00000290: 2076 6572 7920 7370 6563 6966 6963 2075   very specific u
+000002a0: 7365 6361 7365 2c20 6265 6361 7573 6520  secase, because 
+000002b0: 6e6f 7468 696e 6720 6265 7474 6572 2065  nothing better e
+000002c0: 7869 7374 6564 2079 6574 2e20 4e6f 2073  xisted yet. No s
+000002d0: 7461 6269 6c69 7479 2067 7561 7261 6e74  tability guarant
+000002e0: 6565 7320 6172 6520 6d61 6465 2c20 616e  ees are made, an
+000002f0: 6420 7468 6520 4150 4920 6973 2073 7562  d the API is sub
+00000300: 6a65 6374 2074 6f20 6368 616e 6765 203a  ject to change :
+00000310: 290a 0a26 6e62 7370 3b0a 0a23 2045 7861  )..&nbsp;..# Exa
+00000320: 6d70 6c65 0a60 6060 7079 0a66 726f 6d20  mple.```py.from 
+00000330: 646f 6378 5f63 6861 7274 7320 696d 706f  docx_charts impo
+00000340: 7274 2044 6f63 756d 656e 740a 0a64 6f63  rt Document..doc
+00000350: 203d 2044 6f63 756d 656e 7428 2765 7861   = Document('exa
+00000360: 6d70 6c65 2e64 6f63 7827 290a 6368 6172  mple.docx').char
+00000370: 7420 3d20 646f 632e 6669 6e64 5f63 6861  t = doc.find_cha
+00000380: 7274 735f 6279 5f6e 616d 6528 2743 6861  rts_by_name('Cha
+00000390: 7274 2031 2729 5b30 5d0a 6461 7461 203d  rt 1')[0].data =
+000003a0: 2063 6861 7274 2e64 6174 6128 290a 6461   chart.data().da
+000003b0: 7461 5b27 7374 7564 656e 745f 746f 7461  ta['student_tota
+000003c0: 6c27 5d5b 2743 5442 3130 3032 204c 696e  l']['CTB1002 Lin
+000003d0: 6561 7220 416c 6765 6272 6127 5d20 3d20  ear Algebra'] = 
+000003e0: 302e 360a 6368 6172 742e 7772 6974 6528  0.6.chart.write(
+000003f0: 6461 7461 290a 646f 632e 7361 7665 2829  data).doc.save()
+00000400: 0a60 6060 0a0a                           .```..
```

