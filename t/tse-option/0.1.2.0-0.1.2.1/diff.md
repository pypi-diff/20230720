# Comparing `tmp/tse_option-0.1.2.0.tar.gz` & `tmp/tse_option-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tse_option-0.1.2.0.tar", last modified: Thu Jun 15 08:50:13 2023, max compression
+gzip compressed data, was "tse_option-0.1.2.1.tar", last modified: Thu Jul 20 14:15:02 2023, max compression
```

## Comparing `tse_option-0.1.2.0.tar` & `tse_option-0.1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.439190 tse_option-0.1.2.0/
--rw-rw-rw-   0        0        0     1097 2022-11-14 08:41:45.000000 tse_option-0.1.2.0/LICENSE
--rw-rw-rw-   0        0        0     5742 2023-06-15 08:50:13.439190 tse_option-0.1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5143 2023-06-15 08:49:00.000000 tse_option-0.1.2.0/README.md
--rw-rw-rw-   0        0        0      892 2023-06-15 08:12:07.000000 tse_option-0.1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 08:50:13.440187 tse_option-0.1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.312956 tse_option-0.1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.414357 tse_option-0.1.2.0/src/tse_option/
--rw-rw-rw-   0        0        0    18168 2023-06-15 08:12:13.000000 tse_option-0.1.2.0/src/tse_option/__init__.py
--rw-rw-rw-   0        0        0       72 2023-01-27 13:12:31.000000 tse_option-0.1.2.0/src/tse_option/example.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:50:13.438231 tse_option-0.1.2.0/src/tse_option.egg-info/
--rw-rw-rw-   0        0        0     5742 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 08:50:13.000000 tse_option-0.1.2.0/src/tse_option.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 14:15:02.193812 tse_option-0.1.2.1/
+-rw-rw-rw-   0        0        0     1097 2022-11-14 08:41:45.000000 tse_option-0.1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5923 2023-07-20 14:15:02.194810 tse_option-0.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5324 2023-07-20 14:13:39.000000 tse_option-0.1.2.1/README.md
+-rw-rw-rw-   0        0        0      892 2023-07-20 14:14:24.000000 tse_option-0.1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 14:15:02.196817 tse_option-0.1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 14:15:02.065209 tse_option-0.1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 14:15:02.160167 tse_option-0.1.2.1/src/tse_option/
+-rw-rw-rw-   0        0        0    18172 2023-07-20 14:11:46.000000 tse_option-0.1.2.1/src/tse_option/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-01-27 13:12:31.000000 tse_option-0.1.2.1/src/tse_option/example.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:15:02.191786 tse_option-0.1.2.1/src/tse_option.egg-info/
+-rw-rw-rw-   0        0        0     5923 2023-07-20 14:15:02.000000 tse_option-0.1.2.1/src/tse_option.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-20 14:15:02.000000 tse_option-0.1.2.1/src/tse_option.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:15:02.000000 tse_option-0.1.2.1/src/tse_option.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-20 14:15:02.000000 tse_option-0.1.2.1/src/tse_option.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 14:15:02.000000 tse_option-0.1.2.1/src/tse_option.egg-info/top_level.txt
```

### Comparing `tse_option-0.1.2.0/LICENSE` & `tse_option-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tse_option-0.1.2.0/PKG-INFO` & `tse_option-0.1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tse_option
-Version: 0.1.2.0
+Version: 0.1.2.1
 Summary: Option pricing in Tehran Stock Exchange (TSE) and Iran Farabourse (IFB)
 Author-email: Seyed Mohammad Sokout <sm.sokut@gmail.com>
 Project-URL: Homepage, https://github.com/sm-sokout/tse-option
 Keywords: Tehran Stock Exchange,TSE,Iran Farabourse,IFB,Option pricing,BSM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # tse_option
 
 
 
-این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند.
+این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند. 
 
 برخی از توابع این پروژه،از ماژول های [finpy_tse](https://github.com/ARahimiQuant/finpy-tse) و [tsemodule5](https://github.com/python4financeacademy/tsemodule5) اقتباس شده اند.
 
 ----------------------------------------------
 
 **توجه**: کلیه خروجی این ماژول از جمله قیمت گذاری و محاسبه تلاطم ضمنی و ... به جهت تسهیل در تصمیم گیری سرمایه گذاران است و هیچگونه پیشنهادی برای خرید یا فروش آن محسوب نمی شود. لذا تمامی عواقب سرمایه گذاری به عهده شخص سرمایه گذار است و توسعه دهندگان هیچ مسئولیتی در قبال زیان های احتمالی ندارند.
 
@@ -35,22 +35,25 @@
 
 
 2- رفع برخی مشکلات
 
 ----------------------------------------------
 
 
-**تغییرات نسخه جدید(0.1.2.0)**: 
+**تغییرات نسخه جدید(0.1.2.1)**: 
 
 
 1- بروزرسانی لینک های tsetmc
 
 
 2- امکان دریافت تاریخچه قیمت چندین نماد(مانند yfinance)
 
+
+3- بروزرسانی لینک سایت tse.ir
+
 ----------------------------------------------
 
 
 
 
 ### نصب
 ```python
@@ -138,9 +141,11 @@
 
 
 برای مشاهده مثال های بیشتر [اینجا](https://github.com/sm-sokout/tse-option/blob/master/Example/Example.ipynb) کلیک کنید.
 
 -----------------------------------------------------------------
 
 
+در صورت برخورد با هرگونه خطا، ممنون میشم به من اطلاع بدین (sm.sokut@gmail.com)
+
 
 This project on github [tse-option](https://github.com/sm-sokout/tse-option)
```

### Comparing `tse_option-0.1.2.0/README.md` & `tse_option-0.1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tse_option
 
 
 
-این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند.
+این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند. 
 
 برخی از توابع این پروژه،از ماژول های [finpy_tse](https://github.com/ARahimiQuant/finpy-tse) و [tsemodule5](https://github.com/python4financeacademy/tsemodule5) اقتباس شده اند.
 
 ----------------------------------------------
 
 **توجه**: کلیه خروجی این ماژول از جمله قیمت گذاری و محاسبه تلاطم ضمنی و ... به جهت تسهیل در تصمیم گیری سرمایه گذاران است و هیچگونه پیشنهادی برای خرید یا فروش آن محسوب نمی شود. لذا تمامی عواقب سرمایه گذاری به عهده شخص سرمایه گذار است و توسعه دهندگان هیچ مسئولیتی در قبال زیان های احتمالی ندارند.
 
@@ -20,22 +20,25 @@
 
 
 2- رفع برخی مشکلات
 
 ----------------------------------------------
 
 
-**تغییرات نسخه جدید(0.1.2.0)**: 
+**تغییرات نسخه جدید(0.1.2.1)**: 
 
 
 1- بروزرسانی لینک های tsetmc
 
 
 2- امکان دریافت تاریخچه قیمت چندین نماد(مانند yfinance)
 
+
+3- بروزرسانی لینک سایت tse.ir
+
 ----------------------------------------------
 
 
 
 
 ### نصب
 ```python
@@ -123,9 +126,11 @@
 
 
 برای مشاهده مثال های بیشتر [اینجا](https://github.com/sm-sokout/tse-option/blob/master/Example/Example.ipynb) کلیک کنید.
 
 -----------------------------------------------------------------
 
 
+در صورت برخورد با هرگونه خطا، ممنون میشم به من اطلاع بدین (sm.sokut@gmail.com)
+
 
 This project on github [tse-option](https://github.com/sm-sokout/tse-option)
```

### Comparing `tse_option-0.1.2.0/pyproject.toml` & `tse_option-0.1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "tse_option"
-version = "0.1.2.0"
+version = "0.1.2.1"
 authors = [
   { name="Seyed Mohammad Sokout", email="sm.sokut@gmail.com" },
 ]
 description = "Option pricing in Tehran Stock Exchange (TSE) and Iran Farabourse (IFB)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tse_option-0.1.2.0/src/tse_option/__init__.py` & `tse_option-0.1.2.1/src/tse_option/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     url = "http://old.tsetmc.com/tsev2/data/instinfofast.aspx?i="+id+"&c=34"
     tsetmc = rq.get(url)
     return int(tsetmc.text.split(";")[0].split(",")[2])
 
 #----------------------------------------
 
 def tse_options(symbol, stock=True):
-    url = "https://tse.ir/json/MarketWatch/MarketWatch_7.xml"
+    url = "https://old.tse.ir/json/MarketWatch/MarketWatch_7.xml"
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
     data = pd.read_html(url)[0]
     data = data[data["نماد"].notna()]
     if stock == True:
         data["نماد دارایی پایه"] = [data.iloc[i]['نام'].split("-")[0].split(" ")[1] for i in range(len(data))]
         data = data[data["نماد دارایی پایه"] == symbol]
     else:
```

### Comparing `tse_option-0.1.2.0/src/tse_option.egg-info/PKG-INFO` & `tse_option-0.1.2.1/src/tse_option.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tse-option
-Version: 0.1.2.0
+Version: 0.1.2.1
 Summary: Option pricing in Tehran Stock Exchange (TSE) and Iran Farabourse (IFB)
 Author-email: Seyed Mohammad Sokout <sm.sokut@gmail.com>
 Project-URL: Homepage, https://github.com/sm-sokout/tse-option
 Keywords: Tehran Stock Exchange,TSE,Iran Farabourse,IFB,Option pricing,BSM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # tse_option
 
 
 
-این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند.
+این پکیج جهت بررسی و قیمت گذاری اوراق اختیار معامله موجود در بورس اوراق بهادار تهران و فرابورس ایران ایجاد شده است. لازم به یادآوری است که در این ماژول از مدل ارائه شده توسط بلک-شولز-مرتون در سال 1973 برای قیمت گذاری اختیار معامله استفاده شد است. سعی بر آن است که در نسخه های بعدی سایر مدل های قیمت گذاری نیز اضافه شوند. 
 
 برخی از توابع این پروژه،از ماژول های [finpy_tse](https://github.com/ARahimiQuant/finpy-tse) و [tsemodule5](https://github.com/python4financeacademy/tsemodule5) اقتباس شده اند.
 
 ----------------------------------------------
 
 **توجه**: کلیه خروجی این ماژول از جمله قیمت گذاری و محاسبه تلاطم ضمنی و ... به جهت تسهیل در تصمیم گیری سرمایه گذاران است و هیچگونه پیشنهادی برای خرید یا فروش آن محسوب نمی شود. لذا تمامی عواقب سرمایه گذاری به عهده شخص سرمایه گذار است و توسعه دهندگان هیچ مسئولیتی در قبال زیان های احتمالی ندارند.
 
@@ -35,22 +35,25 @@
 
 
 2- رفع برخی مشکلات
 
 ----------------------------------------------
 
 
-**تغییرات نسخه جدید(0.1.2.0)**: 
+**تغییرات نسخه جدید(0.1.2.1)**: 
 
 
 1- بروزرسانی لینک های tsetmc
 
 
 2- امکان دریافت تاریخچه قیمت چندین نماد(مانند yfinance)
 
+
+3- بروزرسانی لینک سایت tse.ir
+
 ----------------------------------------------
 
 
 
 
 ### نصب
 ```python
@@ -138,9 +141,11 @@
 
 
 برای مشاهده مثال های بیشتر [اینجا](https://github.com/sm-sokout/tse-option/blob/master/Example/Example.ipynb) کلیک کنید.
 
 -----------------------------------------------------------------
 
 
+در صورت برخورد با هرگونه خطا، ممنون میشم به من اطلاع بدین (sm.sokut@gmail.com)
+
 
 This project on github [tse-option](https://github.com/sm-sokout/tse-option)
```

