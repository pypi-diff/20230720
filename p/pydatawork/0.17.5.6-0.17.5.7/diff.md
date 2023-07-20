# Comparing `tmp/pydatawork-0.17.5.6.tar.gz` & `tmp/pydatawork-0.17.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.6.tar", last modified: Tue Jul 18 09:36:18 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.7.tar", last modified: Thu Jul 20 18:19:07 2023, max compression
```

## Comparing `pydatawork-0.17.5.6.tar` & `pydatawork-0.17.5.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.6/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52820 2023-07-18 09:35:29.000000 pydatawork-0.17.5.6/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-18 09:36:18.000000 pydatawork-0.17.5.6/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-18 09:30:14.000000 pydatawork-0.17.5.6/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.7/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    53278 2023-07-20 18:16:53.000000 pydatawork-0.17.5.7/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-20 18:19:07.000000 pydatawork-0.17.5.7/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-20 18:17:43.000000 pydatawork-0.17.5.7/setup.py
```

### Comparing `pydatawork-0.17.5.6/PKG-INFO` & `pydatawork-0.17.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.6
+Version: 0.17.5.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.5.6/README.md` & `pydatawork-0.17.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.5.6/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.7/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.6
+Version: 0.17.5.7
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.5.6/pydatawork.py` & `pydatawork-0.17.5.7/pydatawork.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,110 +71,105 @@
 #     print("\n")
 
 
 def hello_jkzhou(): # 为什么要定义主函数？ @知识卡片
     # 先定义需要用到的函数
     def menu():
         print("\n==pydatawork官方文档==")
-        # print("------------------------功能菜单------------------------------------")
-        # print("\t\t1.basic functions")
-        # print("\t\t2.data processing")
-        # print("\t\t3.data analysis")
-        # print("\t\t4.查找")
-        # print("\t\t5.工作台")
-        # print("\t\t6.知识库")
-        # print("\t\t7.数据库")
-        # print("\t\t8.联系与帮助")
-        # print("\t\t0.退出")
-        # print("1.basic functions", end="")
-        # print("\t2.data processing", end="")
-        # print("\t3.data analysis")
-        # print("4.查找", end="")
-        # print("\t5.工作台", end="")
-        # print("\t6.知识库", end="")
-        # print("\t7.数据库", end="")
-        # print("\t8.联系与帮助")
-        # print("0.退出")
-        # print("--------------------")
-        print("1.basic functions")
-        print("2.data processing")
-        print("3.data analysis")
-        print("4.查找")
-        print("5.工作台")
-        print("6.知识库")
-        print("7.数据库")
-        print("8.联系与帮助")
+        print("1.basic functions") # 基础函数索引
+        print("2.data processing") # 数据处理函数索引
+        print("3.data analysis") # 数据分析函数索引
+        print("4.查找") # 根据用户输入的关键词，提示对方用哪个函数
+        print("5.工作台") # 关于使用pydatawork的相关路径设置，专门为使用pydatawork而设定
+        print("6.知识库") # wiki，数据工作相关的知识卡片
+        print("7.数据库") # 存放相关信息到工作台中的路径下，卸载pydatawork后数据已还在，专门为使用pydatawork而设定
+        print("8.联系与帮助") # 联系方式
         print("0.退出")
         print("----------------------")
 
     def basic_functions():
         while True:
             print("basic functions:")
-            print("file_split")
-            print("get_current_folder_name")
-            print("get_file_name")
-            print("copy_files")
-            print("copy_all_files")
-            print("copy_files_by_keyword")
-            print("move_files")
-            print("move_all_files")
-            print("move_files_by_keyword")
-            print("rename_by_re") 
+            print("file_split()")
+            print("get_current_folder_name()")
+            print("get_file_name()")
+            print("copy_files()")
+            print("copy_all_files()")
+            print("copy_files_by_keyword()")
+            print("move_files()")
+            print("move_all_files()")
+            print("move_files_by_keyword()")
+            print("rename_by_re()") 
             print("rename_by_insert_keyword()")
-            print("renamer_folder_numeric_serialize")
+            print("renamer_folder_numeric_serialize()")
             print("\n")
 
             answer = input("输入 n/N 退出，按 回车 继续...") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
 
     def data_processing():
         while True:
             print("data processing:")
-            print("obsidian_move_md_or_canvas_linked_images")
-            print("obsidian_bookmarks_merge_and_deduplicate")
-            print("get_weibo")
+            print("obsidian_move_md_or_canvas_linked_images()")
+            print("obsidian_bookmarks_merge_and_deduplicate()")
+            print("get_weibo()")
             print("\n")
 
             answer = input("输入 n/N 退出，按 回车 继续...") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
 
 
     def data_analysis():
         while True:
             print("data analysis:")
-            print("game_number_guessing")
-            print("get_BMI")
+            print("game_number_guessing()")
+            print("get_BMI()")
             print("\n")
 
             answer = input("输入 n/N 退出，按 回车 继续...") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
 
 
     def search():
+        """
+        功能：询问用户需要做什么；提示用户输入自己要做的事情；根据关键词推荐用户使用某个函数。
+        """
         pass
 
     def workspaces():
+        """
+        功能：引导用户建立工作台，以便于在后续能更方便地获得各种处理结果。
+        """
         pass
 
     def wiki():
+        """
+        功能:：数据工作相关的知识卡片，提供知识服务。如各种数据类型、数据结构、基本路径设置、计算机基础、pydatawork使用常见注意事项等等。
+        """
         pass
 
     def database():
+        """
+        功能：存放关于使用pydatawork产生的各种底层数据，主要是类似日志的东西，主要用于帮助大家了解数据处理过程，可能会存放一些数据运行时产生的过程数据，如历史指令等。
+        """
         pass
 
     def get_help():
+        """
+        功能：提供联系方式。
+        """
         print("\nHi, 感谢你使用pydatawork，下面的信息可能对你有用，试试看：")    
         print("1.pydatawork的官方文档中提供了函数说明和一些示例。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
         print("2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
         print("3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
         # print("\n")
 
     while True: # 为什么选择使用while循环。布尔值和while循环用在一起，通常为了实现什么目的。每个对象都有一个布尔值。 @知识卡片
```

### Comparing `pydatawork-0.17.5.6/setup.py` & `pydatawork-0.17.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.6',
+    version='0.17.5.7',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

