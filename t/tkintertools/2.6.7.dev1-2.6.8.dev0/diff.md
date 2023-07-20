# Comparing `tmp/tkintertools-2.6.7.dev1.tar.gz` & `tmp/tkintertools-2.6.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.7.dev1.tar", last modified: Wed Jul  5 07:42:55 2023, max compression
+gzip compressed data, was "tkintertools-2.6.8.dev0.tar", last modified: Thu Jul 20 10:07:05 2023, max compression
```

## Comparing `tkintertools-2.6.7.dev1.tar` & `tkintertools-2.6.8.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.428696 tkintertools-2.6.7.dev1/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.7.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0     9152 2023-07-05 07:42:55.428696 tkintertools-2.6.7.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     8518 2023-07-05 07:41:33.000000 tkintertools-2.6.7.dev1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 07:42:55.429698 tkintertools-2.6.7.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-07-05 07:10:06.000000 tkintertools-2.6.7.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.417320 tkintertools-2.6.7.dev1/tkintertools/
--rw-rw-rw-   0        0        0     2335 2023-07-05 07:09:46.000000 tkintertools-2.6.7.dev1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    63634 2023-07-04 05:00:55.000000 tkintertools-2.6.7.dev1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2514 2023-07-03 06:06:54.000000 tkintertools-2.6.7.dev1/tkintertools/constants.py
--rw-rw-rw-   0        0        0    24194 2023-07-05 07:07:35.000000 tkintertools-2.6.7.dev1/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-07-05 07:42:55.426697 tkintertools-2.6.7.dev1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9152 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-05 07:42:55.000000 tkintertools-2.6.7.dev1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.409236 tkintertools-2.6.8.dev0/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.8.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9305 2023-07-20 10:07:05.408236 tkintertools-2.6.8.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     8671 2023-07-20 10:05:47.000000 tkintertools-2.6.8.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 10:07:05.409236 tkintertools-2.6.8.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-20 10:01:22.000000 tkintertools-2.6.8.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.390222 tkintertools-2.6.8.dev0/tkintertools/
+-rw-rw-rw-   0        0        0     2237 2023-07-20 10:00:58.000000 tkintertools-2.6.8.dev0/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    67589 2023-07-20 09:49:55.000000 tkintertools-2.6.8.dev0/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2580 2023-07-20 07:07:46.000000 tkintertools-2.6.8.dev0/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    24186 2023-07-06 15:11:02.000000 tkintertools-2.6.8.dev0/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.405235 tkintertools-2.6.8.dev0/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9305 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.7.dev1/LICENSE.txt` & `tkintertools-2.6.8.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.7.dev1/PKG-INFO` & `tkintertools-2.6.8.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,58 @@
-Metadata-Version: 2.1
-Name: tkintertools
-Version: 2.6.7.dev1
-Summary: An auxiliary module of the tkinter module.
-Home-page: https://github.com/Xiaokang2022/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-Maintainer: Xiaokang2022
-Maintainer-email: 2951256653@qq.com
-License: MulanPSL-2.0
-Keywords: tkinter,tkintertools,GUI
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
-[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
+[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.6`
-* Release/发布日期 : 2023/07/01 (UTC+08)
+* Version/最新版本 : `2.6.7`
+* Release/发布日期 : 2023/07/06 (UTC+08)
 
-这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
-稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
+这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6
+pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
-* Release/发布日期 : 2023/07/05 (UTC+08)
+* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/20 (UTC+08)
 
-这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
-开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
-大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
+这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev1
+pip install tkintertools==2.6.8.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -94,43 +73,46 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev1`**
+**最新版本: `tkintertools-v2.6.8.dev0`**
+
+> **Note**   
+> tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
+
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
 
-> **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
-> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
-
-下面是本次版本更新内容条目：
-
-- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
-3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
-- [X] Optimized some code and type hints  
-优化了部分代码和类型提示
-- [X] Removed abstract classes and abstract methods  
-移除了抽象类和抽象方法
+- [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
+新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
+- [X] Added constant `CONTROL`  
+新增常量 `CONTROL`
+- [X] Modified the name of the constant `FRAMES` to `FPS`  
+修改常量 `FRAMES` 的名称为 `FPS`
+- [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
+函数 `move` 即将被弃用，请用新类 `Animation` 来代替
+- [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
+类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
 * 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.gif)
 
-<details><summary><b>点击查看源代码</b></summary>
+<details><summary><b>CODE/源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
```

### Comparing `tkintertools-2.6.7.dev1/README.md` & `tkintertools-2.6.8.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,76 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.8.dev0
+Summary: An auxiliary module of the tkinter module.
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+Maintainer: Xiaokang2022
+Maintainer-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
-[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
+[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.6`
-* Release/发布日期 : 2023/07/01 (UTC+08)
+* Version/最新版本 : `2.6.7`
+* Release/发布日期 : 2023/07/06 (UTC+08)
 
-这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
-稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
+这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6
+pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
-* Release/发布日期 : 2023/07/05 (UTC+08)
+* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/20 (UTC+08)
 
-这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
-开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
-大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
+这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev1
+pip install tkintertools==2.6.8.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -76,43 +91,46 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev1`**
+**最新版本: `tkintertools-v2.6.8.dev0`**
+
+> **Note**   
+> tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
+
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
 
-> **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
-> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
-
-下面是本次版本更新内容条目：
-
-- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
-3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
-- [X] Optimized some code and type hints  
-优化了部分代码和类型提示
-- [X] Removed abstract classes and abstract methods  
-移除了抽象类和抽象方法
+- [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
+新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
+- [X] Added constant `CONTROL`  
+新增常量 `CONTROL`
+- [X] Modified the name of the constant `FRAMES` to `FPS`  
+修改常量 `FRAMES` 的名称为 `FPS`
+- [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
+函数 `move` 即将被弃用，请用新类 `Animation` 来代替
+- [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
+类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
 * 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.gif)
 
-<details><summary><b>点击查看源代码</b></summary>
+<details><summary><b>CODE/源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
```

### Comparing `tkintertools-2.6.7.dev1/setup.py` & `tkintertools-2.6.8.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 9. 删除多余文件
 """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.7.dev1',
+    version='2.6.8.dev0',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-2.6.7.dev1/tkintertools/__init__.py` & `tkintertools-2.6.8.dev0/tkintertools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,22 +38,21 @@
 [ChangeLog](https://github.com/Xiaokang2022/tkintertools/blob/master/CHANGELOG.md) ·
 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki)
 """
 
 import sys  # Get interpreter version information
 
 if sys.version_info < (3, 8):  # Version Check
-    error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.8 !\033[0m'
-    raise RuntimeError(error_info)
+    raise RuntimeError('Python version is too low (>=3.8)')
 
 from .__main__ import *
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.7.dev1'
+__version__ = '2.6.8.dev0'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
```

### Comparing `tkintertools-2.6.7.dev1/tkintertools/__main__.py` & `tkintertools-2.6.8.dev0/tkintertools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作 \ 
         `alpha`: 窗口的透明度，取值在 0~1 之间，且 1 为不透明 \ 
         `toolwindow`: 窗口是否为工具窗口 \ 
         `topmost`: 窗口是否置顶，为布尔值 \ 
         `transparentcolor`: 过滤掉该颜色 \ 
         `**kw`: 与 tkinter.Tk 类的其他参数相同
         """
-        if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
+        if type(self) == Tk:  # NOTE: 方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
         self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
         self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
         self._canvas = []  # type: list[Canvas]  # 子画布列表
 
         if width is not None and height is not None:
@@ -87,15 +87,15 @@
         for canvas in self._canvas:
             if canvas.expand and canvas._lock:
                 canvas._zoom(width/self.width[1], height/self.height[1])
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
     def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
-        # override: 添加修改初始宽高值的功能并兼容不同的DPI缩放
+        # override: 添加修改初始宽高值的功能并兼容不同的 DPI 缩放
         if newGeometry:
             width, height, _width, _height, * \
                 _ = map(int, (newGeometry+'+0+0').replace('+', 'x').split('x'))
             self.width, self.height = [width]*2, [height]*2
             geometry = '%dx%d+%d+%d' % (width, height, _width, _height)
             if not _:
                 geometry = geometry.split('+')[0]
@@ -205,15 +205,15 @@
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
         if x is not None and y is not None:
             self.place(x=x, y=y)
 
         self.bind('<Motion>', self._touch)  # 绑定鼠标触碰控件
-        self.bind('<Any-Key>', self._input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
+        self.bind('<Any-Key>', self._input)  # 绑定键盘输入字符（和 Ctrl+v 的代码顺序不可错）
         self.bind('<Button-1>', self._click)  # 绑定鼠标左键按下
         self.bind('<B1-Motion>', self._click)  # 绑定鼠标左键按下移动
         self.bind('<MouseWheel>', self._mousewheel)  # 绑定鼠标滚轮滚动
         self.bind('<ButtonRelease-1>', self._release)  # 绑定鼠标左键松开
         self.bind('<<Paste>>', lambda _: self._paste())  # 绑定粘贴快捷键
 
     def widget(self):  # type: () -> tuple[BaseWidget]
@@ -760,15 +760,15 @@
         self.flag = False  # 光标闪烁标志
         # 隐式值
         self._value = ['', text, ''] if type(text) == str else ['', *text]
 
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, '', justify,
                             borderwidth, font, image, color_text, color_fill, color_outline)
 
-        # 提示光标 NOTE:位置顺序不可乱动，font不可乱改
+        # NOTE: 提示光标代码的位置顺序不可乱动，font 不可乱改
         self._cursor = canvas.create_text(0, 0, fill=color_text[2], font=font)
         canvas._font[self._cursor][1] = canvas._font[self.text][1]
         font = canvas.itemcget(self.text, 'font')
         canvas.itemconfigure(self._cursor, font=font)
 
     def _touch_on(self):  # type: () -> None
         """ 鼠标悬停状态 """
@@ -820,15 +820,15 @@
             self.master.itemconfigure(self._cursor, text='')
 
     def _cursor_update(self, text=' '):  # type: (str) -> None
         """ 鼠标光标更新 """
         self.interval, self.flag = 300, False  # 恢复默认值
         if isinstance(self, Entry):
             self.master.coords(self._cursor, self.master.bbox(
-                self.text)[2], self.y1+self.height * self.master.ry / 2)  # BUG
+                self.text)[2], self.y1+self.height * self.master.ry / 2)  # BUG: 缩放后光标位置会略微显示错误
         elif isinstance(self, Text):
             _pos = self.master.bbox(self._text)
             self.master.coords(self._cursor, _pos[2], _pos[1])
         self.master.itemconfigure(
             self._cursor, text='' if not text else self.icursor)
 
     def _paste(self):  # type: () -> bool
@@ -1097,15 +1097,15 @@
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
                             cursor, borderwidth, font, image, color_text, color_fill, color_outline)
 
         _x = x + (width-radius-3 if justify == 'right' else width /
                   2 if justify == 'center' else radius+2)
         _anchor = 'n' if justify == 'center' else 'ne' if justify == 'right' else 'nw'
 
-        self._text = canvas.create_text(  # 位置确定文本 NOTE:位置不要乱动
+        self._text = canvas.create_text(  # NOTE: 位置确定文本，位置不要乱动
             _x, y+radius+2,
             justify=justify,
             anchor=_anchor,
             font=font,
             fill=color_text[0])
 
         self.read = read  # 只读模式
@@ -1204,30 +1204,30 @@
             _ = self.value.rsplit('\n', 1)[-1]
             self.master.itemconfigure(self._text, text=_)
 
             # 内容未超出框的大小
             if self.value == self.master.itemcget(self.text, 'text'):
                 _pos = self.master.bbox(self._text)
                 self.master.move(self._text, 0, _pos[1] - _pos[3])
-                # NOTE: 为了兼容Python3.8,放弃使用str.removesuffix方法，以temp取而代之
+                # NOTE: 为了兼容 Python3.8，放弃使用 str.removesuffix 方法，以 temp 取而代之
                 temp = self.value[:-
                                   len(_)] if self.value.endswith(_) else self.value
                 __ = temp[:-('\n' in self.value)]
             else:  # 内容已经超出框框的大小啦
                 text = self.master.itemcget(self.text, 'text')
                 temp = self.value[:-len(text)
                                   ] if self.value.endswith(text) else self.value
                 temp2 = text[:len(_)] if text.endswith(_) else text
                 __ = temp[:-1].rsplit('\n', 1)[-1]+'\n'+temp2[:-1]
 
             self.master.itemconfigure(self.text, text=__)
 
     def _scroll(self, event):  # type: (tkinter.Event) -> bool
         """ 鼠标滚轮滚动 """
-        return False  # TODO: 暂未实现
+        return False  # TODO: 实现滚轮滚动来查看内容
 
 
 class Progressbar(BaseWidget):
     """ 虚拟进度条控件 """
 
     def __init__(
         self,
@@ -1260,15 +1260,15 @@
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
     def load(self, percentage):  # type: (float) -> None
         """
         ### 加载
-        `percentage`: 进度条的值，范围 0 ~ 1
+        `percentage`: 进度条的值，范围 0~1
         """
         percentage = 0 if percentage < 0 else 1 if percentage > 1 else percentage
         x2 = self.x1 + self.width * percentage * self.master.rx
         self.master.coords(self.bar, self.x1, self.y1, x2, self.y2)
         self.configure(text='%.2f%%' % (percentage * 100))
 
 
@@ -1378,35 +1378,121 @@
                 for y in range(height):
                     image.put('#%02X%02X%02X' % self.get(
                         int(x/rate_x), int(y/rate_y)), (x, y))
 
         return image
 
 
+class Animation:
+    """ 动画 """
+
+    def __init__(
+        self,
+        widget,  # type: BaseWidget | tkinter.BaseWidget | int
+        ms,  # type: int
+        *,
+        control=CONTROL,  # type: tuple[Callable[[float], float], float, float]
+        translation=None,  # type: Iterable[float, float] | None
+        color=None,  # type: tuple[Callable[[str], None], str, str] | None
+        fps=FPS,  # type: int
+        start=None,  # type: Callable | None
+        step=None,  # type: Callable | None
+        stop=None,  # type: Callable | None
+        canvas=None  # type: tkinter.Canvas | None
+    ):  # type: (...) -> None
+        """
+        `widget`: 进行动画的控件 \ 
+        `ms`: 动画总时长（单位：毫秒） \ 
+        `control`: 控制函数，为元组 (函数, 起始值, 终止值) 的形式 \ 
+        `translation`: 平移运动 \ 
+        `color`: 颜色变换 \ 
+        `fps`: 每秒帧数 \ 
+        `start`: 动画开始前执行的函数 \ 
+        `step`: 动画每一帧结束后执行的函数（包括开始和结束）\ 
+        `stop`: 动画结束后执行的函数 \ 
+        `canvas`: 当 widget 是画布中的绘制对象时，应指定 canvas
+        """
+        self.widget = widget
+        self.master = canvas if isinstance(widget, int) else widget.master if isinstance(
+            widget, tkinter.Widget) else widget
+        self.start = start
+        self.step = step
+        self.stop = stop
+        self.translation = translation
+        self.color = color
+        self.sec = 1000 // fps  # 单帧间隔时间
+        self.count = ms * fps // 1000  # 总帧数
+        if self.count == 0:
+            self.count = 1  # 至少一帧
+        self.parts = self._parts(*control)
+
+    def _parts(self, control, up, down):
+        # type: (Callable[[float], float], float, float) -> list[float]
+        """ 部分比率 """
+        key = (down - up) / self.count
+        parts = [control(key * value) for value in range(1, self.count + 1)]
+        total = sum(parts)
+        return [elem / total for elem in parts]
+
+    def _run(self, _ind=0):  # type: (int) -> None
+        """ 执行动画 """
+        if _ind == self.count:
+            return None if self.stop is None else self.stop()
+        self.master.after(self.sec, self._run, _ind + 1)
+
+        if self.translation is not None:
+            self._translate(*[value * self.parts[_ind]
+                            for value in self.translation])
+        if self.color is not None:
+            self.color[0](color(self.color[1:], sum(self.parts[:_ind + 1])))
+
+        None if self.step is None else self.step()
+
+    def _translate(self, dx, dy):  # type: (int, int) -> None
+        """ 平移 """
+        if isinstance(self.widget, tkinter.Tk | tkinter.Toplevel):  # 窗口
+            size, x, y = self.widget.geometry().split('+')
+            self.widget.geometry('%s+%d+%d' % (size, int(x)+dx, int(y)+dy))
+        elif isinstance(self.widget, tkinter.Widget):  # tkinter 控件
+            place_info = self.widget.place_info()
+            origin_x, origin_y = float(place_info['x']), float(place_info['y'])
+            self.widget.place(x=origin_x+dx, y=origin_y+dy)
+        elif isinstance(self.widget, BaseWidget):  # tkintertools 控件
+            self.widget.move(dx, dy)
+        elif isinstance(self.widget, int):  # tkinter._CanvasItemId
+            self.master.move(self.widget, dx, dy)
+
+    def run(self):  # type: () -> None
+        """ 运行动画 """
+        None if self.start is None else self.start()
+        self._run()
+
+
 class Singleton(object):
     """ 单例模式类 """
 
     _instance = None
 
     def __new__(cls, *args, **kw):
+        print('Deprecation Warning: Class `Singleton` is about to be deprecated.')
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
 
 
 @overload
 def move(
     master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
     widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
     dx,  # type: int
     dy,  # type: int
     times,  # type: int
     *,
     mode,  # type: Literal['smooth', 'rebound', 'flat']
-    frames=FRAMES,  # type: int
+    frames=FPS,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     ...
 
 
 @overload
@@ -1414,15 +1500,15 @@
     master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
     widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
     dx,  # type: int
     dy,  # type: int
     times,  # type: int
     *,
     mode,  # type: tuple[Callable[[float], float], float, float]
-    frames=FRAMES,  # type: int
+    frames=FPS,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     ...
 
 
 def move(
@@ -1430,30 +1516,30 @@
     widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
     dx,  # type: int
     dy,  # type: int
     times,  # type: int
     *,
     mode,
     # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']
-    frames=FRAMES,  # type: int
+    frames=FPS,  # type: int
     end=None,  # type: Callable | None
     _ind=0  # type: int
 ):  # type: (...) -> None
     """
     ### 移动函数
     以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像 \ 
     或者按一定的函数规律来移动
     ---
     `master`: 控件所在的父控件 \ 
     `widget`: 要移动位置的控件 \ 
     `dx`: 横向移动的距离（单位：像素） \ 
     `dy`: 纵向移动的距离（单位：像素） \ 
     `times`: 移动总时长（单位：毫秒） \ 
     `mode`: 移动速度模式，为 smooth（顺滑）、rebound（回弹）和 flat（平移）这三种，或者为元组 (函数, 起始值, 终止值) 的形式 \ 
-    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1 ~ 100） \ 
+    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1~100） \ 
     `end`: 移动结束时执行的函数
     """
     if _ind:  # 记忆值
         dis = mode
     elif mode == 'flat':  # 平滑模式
         return move(master, widget, dx, dy, times, mode=(lambda _: 1, 0, 1), frames=frames, end=end)
     elif mode == 'smooth':  # 流畅模式
@@ -1479,14 +1565,16 @@
         widget.move(dis[_ind][0], dis[_ind][1])
     elif isinstance(widget, int):  # tkinter._CanvasItemId
         master.move(widget, dis[_ind][0], dis[_ind][1])
     else:  # 其他自定义情况
         widget.move(dis[_ind][0], dis[_ind][1])
 
     if _ind+1 == round(times*frames/1000):  # 停止条件
+        # NOTE: Deprecated
+        print('Deprecation Warning: The function `move` is about to be deprecated, please use the class `Animation` instead.')
         return end() if end else None
 
     master.after(
         round(times/frames),
         lambda: move(master, widget, dx, dy, times, mode=dis, frames=frames, end=end, _ind=_ind+1))  # 间隔一定时间执行函数
 
 
@@ -1536,15 +1624,15 @@
 ):  # type: (...) -> str
     """
     ### 颜色函数
     按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串 \ 
     或者给出已有 RGB 颜色字符串的对比色
     ---
     `color`: 颜色元组或列表 (初始颜色, 目标颜色)，或者一个颜色字符串（此时返回其对比色） \ 
-    `proportion`: 改变比例（浮点数，范围为 0 ~ 1）
+    `proportion`: 改变比例（浮点数，范围为 0~1）
     """
     rgb, _rgb = [[None]*3, [None]*3], 0
 
     if isinstance(color, str):  # 对比色的情况处理
         color = color, '#%06X' % (16777216-int(color[1:], 16))
 
     for i, c in enumerate(color):  # 解析颜色的 RGB
```

### Comparing `tkintertools-2.6.7.dev1/tkintertools/constants.py` & `tkintertools-2.6.8.dev0/tkintertools/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,26 @@
 LIMIT = -1
 """ Default widget text length limit """
 
 RADIUS = 0 if SYSTEM == 'Windows' and int(
     platform.version()[-5:]) < 22000 else 4
 """ Default widget fillet radius """
 
-FRAMES = 60
-""" Default move frame rate """
+FPS = 60
+""" Default animation FPS """
 
 TICK = '✓'
 """ Default checkbox symbol """
 
-
-### 3D constants ###
+CONTROL = lambda _: 1, 0, 1
+""" Default control function """
 
 
-CAMERA_DISTANCE = 1000
-""" Default 3D camera distance """
+### 3D constants ###
 
-ROTATE_CENTER = 0, 0, 0
-""" Default rotation center """
 
 COLOR_POINT_FILL = '#000000'
 """ Default point fill color """
 
 COLOR_POINT_OUTLINE = '#000000'
 """ Default point outline color """
 
@@ -98,14 +95,20 @@
 
 LINE_WDITH = 1
 """ Default line width """
 
 SIDE_WIDTH = 1
 """ Default side width """
 
+CAMERA_DISTANCE = 1000
+""" Default 3D camera distance """
+
+ROTATE_CENTER = 0, 0, 0
+""" Default rotation center """
+
 ORIGIN_COORDINATE = 0, 0, 0
 """ Default origin coordinate """
 
 ORIGIN_SIZE = POINT_SIZE
 """ Default origin size """
 
 ORIGIN_WIDTH = POINT_WIDTH
@@ -114,8 +117,8 @@
 ORIGIN_FILL = ''
 """ Default origin fill color """
 
 ORIGIN_OUTLINE = ''
 """ Default origin outline color """
 
 
-all_constants = [name for name in globals() if name.isupper()]
+all_constants = list(filter(lambda name: name.isupper(), globals()))
```

### Comparing `tkintertools-2.6.7.dev1/tkintertools/tools_3d.py` & `tkintertools-2.6.8.dev0/tkintertools/tools_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,15 @@
 
     def geos(self):  # type: () -> tuple[Geometry]
         """ 返回 `Canvas_3d` 类全部的几何体对象 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
         """ 空间位置排序 """  # BUG: 在距离比较近的两个对象时，仍会显示不正确
-        self._items_3d.sort(
-            key=lambda item: (not isinstance(item, Point), item._camera_distance()))
+        self._items_3d.sort(key=lambda item: item._camera_distance())
         for item in self._items_3d:
             self.lower(item.item)
 
 
 class Space(Canvas_3D):
     """ 三维空间 """
 
@@ -188,38 +187,38 @@
 
 @overload
 def rotate(coordinate, dx=0, *, axis):
     # type: (list[float], float,  ..., Iterable[Iterable[float]]) -> None
     ...
 
 
-def rotate(coordinate, dx=0, dy=0, dz=0, *, center, axis):
+def rotate(coordinate, dx=0, dy=0, dz=0, *, center, axis=None):
     # type: (list[float], float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
     """
     ### 旋转
     将一个三维空间中的点以一个点或线为参照进行旋转 \n
     ---
     `coordinate`: 点的空间坐标 \ 
     `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
     `dy`: y 方向旋转弧度 \ 
     `dz`: z 方向旋转弧度 \ 
     `center`: 旋转中心的空间坐标 \ 
     `axis`: 旋转轴线的空间坐标
     """
     if axis is not None:  # 参照为线（定轴转动）
-        center = _Line(*axis).center()
+        center = _Line(*axis).center()  # 旋转轴中点
         n = list(axis[0])
         for i in range(3):
             n[i] -= axis[1][i]
             coordinate[i] -= center[i]
         n_m = math.hypot(*n)
         for i in range(3):
             n[i] /= n_m
-        x_2, y_2, z_2 = (i**2 for i in n)
-        xy, yz, zx = n[0]*n[1], n[1]*n[2], n[2]*n[0]
+        x_2, y_2, z_2 = map(lambda _: _**2, n)
+        zx, xy, yz = [n[i-1]*v for i, v in enumerate(n)]
         s_θ, c_θ = math.sin(dx), math.cos(dx)
         _c_θ = 1 - c_θ
 
         matrix = [[x_2*_c_θ + c_θ, xy*_c_θ + n[2]*s_θ, zx*_c_θ - n[1]*s_θ],
                   [xy*_c_θ - n[2]*s_θ, y_2*_c_θ + c_θ, yz*_c_θ + n[0]*s_θ],
                   [zx*_c_θ + n[1]*s_θ, yz*_c_θ - n[0]*s_θ, z_2*_c_θ + c_θ]]
 
@@ -317,14 +316,15 @@
         return tuple(statistics.mean(xyz) for xyz in zip(*self.coordinates))
 
     def _project(self, distance):
         """
         ### 投影
         `distance`: 对象与观察者的距离
         """
+        # NOTE: 这里可能需要一些优化
 
 
 class _Point(_3D_Object):
     """ 点（基类） """
 
     def __init__(self, coordinate):  # type: (list[float]) -> None
         _3D_Object.__init__(self, coordinate)
@@ -550,15 +550,14 @@
         if center is None:
             center = self.center()
         for side in self.sides:
             side.scale(kx, ky, kz, center=center)
 
     def center(self):  # type: () -> tuple[float, float, float]
         """ 几何中心 """
-        # BUG: 公式对凹面几何体不成立
         return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coordinates)))
 
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
@@ -655,8 +654,8 @@
             Side(canvas, point_1, point_2, point_3, fill=colors[0]),
             Side(canvas, point_1, point_2, point_4, fill=colors[1]),
             Side(canvas, point_1, point_3, point_4, fill=colors[2]),
             Side(canvas, point_2, point_3, point_4, fill=colors[3]),
         ]
 
 
-__all__ = [name for name in globals() if '__' not in name]
+__all__ = list(filter(lambda name: '__' not in name, globals()))
```

### Comparing `tkintertools-2.6.7.dev1/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.8.dev0/tkintertools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.7.dev1
+Version: 2.6.8.dev0
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,57 +23,54 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/05-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
-[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
+[![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.6`
-* Release/发布日期 : 2023/07/01 (UTC+08)
+* Version/最新版本 : `2.6.7`
+* Release/发布日期 : 2023/07/06 (UTC+08)
 
-这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
-稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
+这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6
+pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.7.dev1` (第 2 个预发布版本)
-* Release/发布日期 : 2023/07/05 (UTC+08)
+* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/20 (UTC+08)
 
-这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
-开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
-大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
+这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.7.dev1
+pip install tkintertools==2.6.8.dev0
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -94,43 +91,46 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.7.dev1`**
+**最新版本: `tkintertools-v2.6.8.dev0`**
 
-> **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！  
-> tkintertools 的介绍和使用教程均在 Wiki 中，[点我传送](https://github.com/Xiaokang2022/tkintertools/wiki)
-
-下面是本次版本更新内容条目：
-
-- [X] The function `rotate` of the 3D submodule adds the keyword `axis` to provide the function of rotating around the axis  
-3D 子模块的函数 `rotate` 新增关键字参数 `axis` 来提供绕轴旋转的功能
-- [X] Optimized some code and type hints  
-优化了部分代码和类型提示
-- [X] Removed abstract classes and abstract methods  
-移除了抽象类和抽象方法
+> **Note**   
+> tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
+
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
+
+- [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
+新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
+- [X] Added constant `CONTROL`  
+新增常量 `CONTROL`
+- [X] Modified the name of the constant `FRAMES` to `FPS`  
+修改常量 `FRAMES` 的名称为 `FPS`
+- [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
+函数 `move` 即将被弃用，请用新类 `Animation` 来代替
+- [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
+类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
 * 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
 ![news](news.gif)
 
-<details><summary><b>点击查看源代码</b></summary>
+<details><summary><b>CODE/源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
```

