# Comparing `tmp/mys_goods_tool-2.1.0.tar.gz` & `tmp/mys_goods_tool-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mys_goods_tool-2.1.0.tar", max compression
+gzip compressed data, was "mys_goods_tool-2.1.0b1.tar", max compression
```

## Comparing `mys_goods_tool-2.1.0.tar` & `mys_goods_tool-2.1.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/LICENSE
--rw-r--r--   0        0        0     4978 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/__init__.py
--rw-r--r--   0        0        0     2278 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/__main__.py
--rw-r--r--   0        0        0    61194 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/api.py
--rw-r--r--   0        0        0     5536 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/custom_css.py
--rw-r--r--   0        0        0     7599 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/custom_widget.py
--rw-r--r--   0        0        0     9816 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/data_model.py
--rw-r--r--   0        0        0    18435 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/exchange_mode.py
--rw-r--r--   0        0        0    43948 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/exchange_plan_view.py
--rw-r--r--   0        0        0     6910 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/gt3-localized.html
--rw-r--r--   0        0        0     6840 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/gt3.html
--rw-r--r--   0        0        0     6890 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/index.html
--rw-r--r--   0        0        0    10861 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/gt.js
--rw-r--r--   0        0        0    14792 2023-07-20 20:59:44.761144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/gt4.js
--rw-r--r--   0        0        0   366500 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/jquery.js
--rw-r--r--   0        0        0     6831 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/localized.html
--rw-r--r--   0        0        0    10717 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/geetest.py
--rw-r--r--   0        0        0    22069 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/login_view.py
--rw-r--r--   0        0        0    14482 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/tui.py
--rw-r--r--   0        0        0    19244 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/user_data.py
--rw-r--r--   0        0        0    10534 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/mys_goods_tool/utils.py
--rw-r--r--   0        0        0     1639 2023-07-20 20:59:44.765144 mys_goods_tool-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 mys_goods_tool-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/LICENSE
+-rw-r--r--   0        0        0     4258 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/__init__.py
+-rw-r--r--   0        0        0     2278 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/__main__.py
+-rw-r--r--   0        0        0    60902 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/api.py
+-rw-r--r--   0        0        0     5536 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/custom_css.py
+-rw-r--r--   0        0        0     7599 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/custom_widget.py
+-rw-r--r--   0        0        0     9816 2023-07-11 09:58:25.816322 mys_goods_tool-2.1.0b1/mys_goods_tool/data_model.py
+-rw-r--r--   0        0        0    17998 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_mode.py
+-rw-r--r--   0        0        0    43948 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_plan_view.py
+-rw-r--r--   0        0        0     6910 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3-localized.html
+-rw-r--r--   0        0        0     6840 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3.html
+-rw-r--r--   0        0        0     6890 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/index.html
+-rw-r--r--   0        0        0    10861 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt.js
+-rw-r--r--   0        0        0    14792 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt4.js
+-rw-r--r--   0        0        0   366500 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/jquery.js
+-rw-r--r--   0        0        0     6831 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/localized.html
+-rw-r--r--   0        0        0    10717 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/geetest.py
+-rw-r--r--   0        0        0    22069 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/login_view.py
+-rw-r--r--   0        0        0    13749 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/tui.py
+-rw-r--r--   0        0        0    19168 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/user_data.py
+-rw-r--r--   0        0        0    10534 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/mys_goods_tool/utils.py
+-rw-r--r--   0        0        0     1646 2023-07-11 09:58:25.820322 mys_goods_tool-2.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 mys_goods_tool-2.1.0b1/PKG-INFO
```

### Comparing `mys_goods_tool-2.1.0/LICENSE` & `mys_goods_tool-2.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/README.md` & `mys_goods_tool-2.1.0b1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,24 +12,14 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-v2.1.0
-
-- 在兑换开始后的一段时间内不断尝试兑换，直到成功
-  > 完整流程：兑换开始后，数个线程同时进行，每个线程在一段时间内重复发送兑换请求  
-  >
-  原因：[太早兑换可能被认定不在兑换时间](https://github.com/Ljzd-PRO/Mys_Goods_Tool/discussions/135#discussioncomment-6487717)
-- 兑换开始后将不会延迟兑换，用户数据文件中 `preference.exchange_latency` 将作为同一线程下每个兑换请求之间的时间间隔
-  > `preference.exchange_latency` 为列表类型，包含两个浮点数，分别为最小延迟和最大延迟，单位为秒，可参考默认值
-- 兑换请求日志内容增加了发送请求时的时间戳
-
 v2.1.0-beta.1
 
 - 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
 - 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
 - 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
 - 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
 - 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
```

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/__main__.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/api.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1261,47 +1261,45 @@
         content.setdefault("address_id", plan.address.id)
     if plan.game_record is not None:
         content.setdefault("uid", plan.game_record.game_role_id)
         # 例: cn_gf01
         content.setdefault("region", plan.game_record.region)
         # 例: hk4e_cn
         content.setdefault("game_biz", plan.good.game_biz)
-    start_time = 0
     try:
-        start_time = time.time()
         async with httpx.AsyncClient() as client:
             res = await client.post(
                 URL_EXCHANGE, headers=headers, json=content,
                 cookies=plan.account.cookies.dict(cookie_type=True),
                 timeout=conf.preference.timeout)
         api_result = ApiResultHandler(res.json())
         if api_result.login_expired:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 登录失效 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 登录失效")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(login_expired=True), None
         if api_result.success:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换成功！可以自行确认 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换成功！可以自行确认。")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(success=True), ExchangeResult(result=True, return_data=res.json(), plan=plan)
         else:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换失败，可以自行确认 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换失败，可以自行确认。")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(success=True), ExchangeResult(result=False, return_data=res.json(), plan=plan)
     except Exception as e:
         if is_incorrect_return(e):
             logger.error(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 服务器没有正确返回 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(incorrect_return=True), None
         else:
             logger.exception(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 请求失败 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 请求失败")
             return ExchangeStatus(network_error=True), None
 
 
 def good_exchange_sync(plan: ExchangePlan) -> Tuple[ExchangeStatus, Optional[ExchangeResult]]:
     """
     执行米游币商品兑换
 
@@ -1320,41 +1318,39 @@
         content.setdefault("address_id", plan.address.id)
     if plan.game_record is not None:
         content.setdefault("uid", plan.game_record.game_role_id)
         # 例: cn_gf01
         content.setdefault("region", plan.game_record.region)
         # 例: hk4e_cn
         content.setdefault("game_biz", plan.good.game_biz)
-    start_time = 0
     try:
-        start_time = time.time()
         with httpx.Client() as client:
             res = client.post(
                 URL_EXCHANGE, headers=headers, json=content,
                 cookies=plan.account.cookies.dict(cookie_type=True),
                 timeout=conf.preference.timeout)
         api_result = ApiResultHandler(res.json())
         if api_result.login_expired:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 登录失效 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 登录失效")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(login_expired=True), None
         if api_result.success:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换成功！可以自行确认 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换成功！可以自行确认。")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(success=True), ExchangeResult(result=True, return_data=res.json(), plan=plan)
         else:
             logger.info(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换失败，可以自行确认 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 兑换失败，可以自行确认。")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(success=True), ExchangeResult(result=False, return_data=res.json(), plan=plan)
     except Exception as e:
         if is_incorrect_return(e):
             logger.error(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 服务器没有正确返回 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 服务器没有正确返回")
             logger.debug(f"网络请求返回: {res.text}")
             return ExchangeStatus(incorrect_return=True), None
         else:
             logger.exception(
-                f"米游币商品兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 请求失败 - 请求发送时间: {start_time}")
+                f"米游币商品兑换 - 执行兑换: 用户 {plan.account.bbs_uid} 商品 {plan.good.goods_id} 请求失败")
             return ExchangeStatus(network_error=True), None
```

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/custom_css.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/custom_css.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/custom_widget.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/custom_widget.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/data_model.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/data_model.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/exchange_mode.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,19 @@
 
 def exchange_begin(plan: ExchangePlan):
     """
     到点后执行兑换
 
     :param plan: 兑换计划
     """
-    duration = 0
     random_x, random_y = conf.preference.exchange_latency
-    exchange_status, exchange_result = ExchangeStatus(), None
-
-    # 在兑换开始后的一段时间内，不断尝试兑换，直到成功（因为太早兑换可能被认定不在兑换时间）
-    while duration < conf.preference.exchange_duration:
-        latency = random.uniform(random_x, random_y)
-        time.sleep(latency)
-        exchange_status, exchange_result = good_exchange_sync(plan)
-        if exchange_status and exchange_result.result:
-            break
-        duration += latency
-    return exchange_status, exchange_result
+    latency = random.uniform(random_x, random_y)
+    time.sleep(latency)
+    result = good_exchange_sync(plan)
+    return result
 
 
 def exchange_mode_simple():
     """
     普通文本模式（无Textual）
     """
     logger.add(sys.stdout, diagnose=True, format=LOG_FORMAT, level="DEBUG")
```

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/exchange_plan_view.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/exchange_plan_view.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/gt3-localized.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3-localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/gt3.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/gt3.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/index.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/index.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/gt.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/gt4.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/gt4.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/libs/jquery.js` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/libs/jquery.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest-webui/localized.html` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest-webui/localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/geetest.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/geetest.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/login_view.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/login_view.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/tui.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,14 @@
 from mys_goods_tool.utils import LOG_FORMAT, logger
 
 WELCOME_MD = """
 # Mys_Goods_Tool - 米游社商品兑换工具
 
 ## 更新说明
 
-v2.1.0
-
-- 在兑换开始后的一段时间内不断尝试兑换，直到成功
-  > 完整流程：兑换开始后，数个线程同时进行，每个线程在一段时间内重复发送兑换请求  
-  > 原因：[太早兑换可能被认定不在兑换时间](https://github.com/Ljzd-PRO/Mys_Goods_Tool/discussions/135#discussioncomment-6487717)
-- 兑换开始后将不会延迟兑换，用户数据文件中 `preference.exchange_latency` 将作为同一线程下每个兑换请求之间的时间间隔
-  > `preference.exchange_latency` 为列表类型，包含两个浮点数，分别为最小延迟和最大延迟，单位为秒，可参考默认值
-- 兑换请求日志内容增加了发送请求时的时间戳
-
-v2.1.0-beta.1
-
 - 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
 - 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
 - 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
 - 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
 - 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
 
 ## 功能和特性
```

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/user_data.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/user_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from json import JSONDecodeError
 from pathlib import Path
 from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
     Mapping
 
 from httpx import Cookies
 from loguru import logger
-from pydantic import BaseModel, ValidationError, BaseSettings, validator, Extra
+from pydantic import BaseModel, Extra, ValidationError, BaseSettings, validator
 
 from mys_goods_tool.data_model import BaseModelWithSetter, Good, Address, GameRecord, BaseModelWithUpdate
 
 ROOT_PATH = Path("./")
 """程序所在目录"""
 
 CONFIG_PATH = ROOT_PATH / "user_data.json"
 """用户数据文件默认路径"""
 
-VERSION = "2.1.0"
+VERSION = "2.1.0-beta.1"
 """程序当前版本"""
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     DictStrAny = Dict[str, Any]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
@@ -201,15 +201,15 @@
                 if not value:
                     empty_key.add(key)
             [cookies_dict.pop(key) for key in empty_key]
 
         return cookies_dict
 
 
-class UserAccount(BaseModelWithSetter):
+class UserAccount(BaseModelWithSetter, extra=Extra.ignore):
     """
     米游社账户数据
 
     >>> user_account = UserAccount(cookies=BBSCookies())
     >>> assert isinstance(user_account, UserAccount)
     >>> user_account.bbs_uid = "123"
     >>> assert user_account.bbs_uid == "123"
@@ -296,33 +296,28 @@
     """连接测试间隔（单位：秒）"""
     timeout: float = 10
     """网络请求超时时间（单位：秒）"""
     max_retry_times: Optional[int] = 3
     """最大网络请求重试次数"""
     retry_interval: float = 2
     """网络请求重试间隔（单位：秒）（除兑换请求外）"""
-
-    # TODO: 目前并没有实现使用同步后的时间进行兑换
     enable_ntp_sync: Optional[bool] = True
     """是否开启NTP时间同步（将调整实际发出兑换请求的时间，而不是修改系统时间）"""
     ntp_server: Optional[str] = "ntp.aliyun.com"
     """NTP服务器地址"""
-
     timezone: Optional[str] = "Asia/Shanghai"
     """兑换时所用的时区"""
     geetest_statics_path: Optional[Path]
     """GEETEST行为验证 网站静态文件目录（默认读取本地包自带的静态文件）"""
     geetest_listen_address: Optional[Tuple[str, int]] = ("localhost", 0)
     """登录时使用的 GEETEST行为验证 WEB服务 本地监听地址"""
     exchange_thread_count: int = 2
     """兑换线程数"""
-    exchange_latency: Tuple[float, float] = (0, 0.5)
-    """同一线程下，每个兑换请求之间的间隔时间"""
-    exchange_duration: float = 5
-    """兑换持续时间随机范围（单位：秒）"""
+    exchange_latency: Tuple[float, float] = (0, 0.2)
+    """兑换时间延迟随机范围（单位：秒）（防止因为发出请求的时间过于精准而被服务器认定为非人工操作）"""
     enable_log_output: bool = True
     """是否保存日志"""
     log_path: Optional[Path] = ROOT_PATH / "logs" / "mys_goods_tool.log"
     """日志保存路径"""
     override_device_and_salt: bool = False
     """是否读取用户数据文件中的 device_config 设备配置 和 salt_config 配置而不是默认配置（一般情况不建议开启）"""
 
@@ -413,30 +408,30 @@
     UA_PLATFORM: str = "\"macOS\""
     '''Headers所用的 sec-ch-ua-platform'''
 
     class Config(Preference.Config):
         pass
 
 
-class UserData(BaseModel, extra=Extra.ignore):
+class UserData(BaseModel):
     """
     用户数据类
     """
     version: str = VERSION
     """创建用户数据文件的程序版本号"""
-    preference: Preference = Preference()
-    """偏好设置"""
     exchange_plans: Union[Set[ExchangePlan], List[ExchangePlan]] = set()
     """兑换计划列表"""
-    accounts: Dict[str, UserAccount] = {}
-    """储存一些已绑定的账号数据"""
+    preference: Preference = Preference()
+    """偏好设置"""
     salt_config: SaltConfig = SaltConfig()
     """生成Headers - DS所用salt值"""
     device_config: DeviceConfig = DeviceConfig()
     """设备信息"""
+    accounts: Dict[str, UserAccount] = {}
+    """储存一些已绑定的账号数据"""
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         exchange_plans = self.exchange_plans
         self.exchange_plans = set()
         for plan in exchange_plans:
             plan = ExchangePlan.parse_obj(plan)
```

### Comparing `mys_goods_tool-2.1.0/mys_goods_tool/utils.py` & `mys_goods_tool-2.1.0b1/mys_goods_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.1.0/pyproject.toml` & `mys_goods_tool-2.1.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mys-goods-tool"
-version = "2.1.0"
+version = "2.1.0-beta.1"
 description = "米游社商品兑换工具|短信验证登录|终端TUI界面"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.ml>"]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 repository = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 documentation = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki"
 keywords = ["mihoyo", "mihoyobbs", "genshin impact", "textual", "tui"]
```

### Comparing `mys_goods_tool-2.1.0/PKG-INFO` & `mys_goods_tool-2.1.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mys-goods-tool
-Version: 2.1.0
+Version: 2.1.0b1
 Summary: 米游社商品兑换工具|短信验证登录|终端TUI界面
 Home-page: https://github.com/Ljzd-PRO/Mys_Goods_Tool
 Keywords: mihoyo,mihoyobbs,genshin impact,textual,tui
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,24 +44,14 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-v2.1.0
-
-- 在兑换开始后的一段时间内不断尝试兑换，直到成功
-  > 完整流程：兑换开始后，数个线程同时进行，每个线程在一段时间内重复发送兑换请求  
-  >
-  原因：[太早兑换可能被认定不在兑换时间](https://github.com/Ljzd-PRO/Mys_Goods_Tool/discussions/135#discussioncomment-6487717)
-- 兑换开始后将不会延迟兑换，用户数据文件中 `preference.exchange_latency` 将作为同一线程下每个兑换请求之间的时间间隔
-  > `preference.exchange_latency` 为列表类型，包含两个浮点数，分别为最小延迟和最大延迟，单位为秒，可参考默认值
-- 兑换请求日志内容增加了发送请求时的时间戳
-
 v2.1.0-beta.1
 
 - 兑换请求Headers增加与修改了 `Referer`, `x-rpc-device_fp`, `x-rpc-verify_key`, `Origin` 等字段，可能修复兑换失败的问题
 - 修复登陆时因为连接断开（client has been closed）而导致登陆失败的问题
 - 防止因配置文件中默认存在 `device_config`, `salt_config` 而导致更新后默认配置被原配置覆盖的问题
 - 若需要修改 `device_config` 配置，修改后还设置用户数据文件中 `preference.override_device_and_salt` 为 `true` 以覆盖默认值
 - 修复Unix下即使安装了 uvloop 也找不到，无法应用的问题
```

