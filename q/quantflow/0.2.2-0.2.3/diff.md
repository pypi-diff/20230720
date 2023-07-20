# Comparing `tmp/quantflow-0.2.2.tar.gz` & `tmp/quantflow-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantflow-0.2.2.tar", max compression
+gzip compressed data, was "quantflow-0.2.3.tar", max compression
```

## Comparing `quantflow-0.2.2.tar` & `quantflow-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1461 2023-07-13 08:54:47.392163 quantflow-0.2.2/LICENSE
--rw-r--r--   0        0        0     1813 2023-07-13 08:54:47.396163 quantflow-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/__init__.py
--rw-r--r--   0        0        0     2840 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/client.py
--rw-r--r--   0        0        0     5374 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/data/fmp.py
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/__init__.py
--rw-r--r--   0        0        0     2032 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/bs.py
--rw-r--r--   0        0        0     7301 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/calibration.py
--rw-r--r--   0        0        0     1021 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/inputs.py
--rw-r--r--   0        0        0     4389 2023-07-13 08:54:47.396163 quantflow-0.2.2/quantflow/options/pricer.py
--rw-r--r--   0        0        0    19846 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/options/surface.py
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/__init__.py
--rwxr-xr-x   0        0        0     4580 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/base.py
--rw-r--r--   0        0        0     2448 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/bns.py
--rwxr-xr-x   0        0        0     5500 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/cir.py
--rwxr-xr-x   0        0        0     2054 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/dsp.py
--rw-r--r--   0        0        0     2576 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/heston.py
--rwxr-xr-x   0        0        0     4771 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/ou.py
--rwxr-xr-x   0        0        0     5921 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/poisson.py
--rw-r--r--   0        0        0     1531 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/sp/weiner.py
--rw-r--r--   0        0        0        0 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/__init__.py
--rw-r--r--   0        0        0      894 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/bins.py
--rw-r--r--   0        0        0      252 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/dates.py
--rw-r--r--   0        0        0      975 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/distributions.py
--rwxr-xr-x   0        0        0      496 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/functions.py
--rw-r--r--   0        0        0     1265 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/interest_rates.py
--rw-r--r--   0        0        0     9347 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/marginal.py
--rw-r--r--   0        0        0      370 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/numbers.py
--rwxr-xr-x   0        0        0     2698 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/paths.py
--rw-r--r--   0        0        0     3411 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/plot.py
--rw-r--r--   0        0        0     4884 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/transforms.py
--rw-r--r--   0        0        0      721 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/types.py
--rw-r--r--   0        0        0     2091 2023-07-13 08:54:47.400163 quantflow-0.2.2/quantflow/utils/volatility.py
--rw-r--r--   0        0        0     1179 2023-07-13 08:54:47.400163 quantflow-0.2.2/readme.md
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 quantflow-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-20 16:33:40.739003 quantflow-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1874 2023-07-20 16:33:40.747003 quantflow-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/data/__init__.py
+-rw-r--r--   0        0        0     2840 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/data/client.py
+-rw-r--r--   0        0        0     5374 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/data/fmp.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/options/__init__.py
+-rw-r--r--   0        0        0     2032 2023-07-20 16:33:40.747003 quantflow-0.2.3/quantflow/options/bs.py
+-rw-r--r--   0        0        0     7289 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/options/calibration.py
+-rw-r--r--   0        0        0     1021 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/options/inputs.py
+-rw-r--r--   0        0        0     5751 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/options/pricer.py
+-rw-r--r--   0        0        0    20309 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/options/surface.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/py.typed
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/__init__.py
+-rwxr-xr-x   0        0        0     6495 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/base.py
+-rw-r--r--   0        0        0     2479 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/bns.py
+-rwxr-xr-x   0        0        0     5307 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/cir.py
+-rwxr-xr-x   0        0        0     2079 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/dsp.py
+-rw-r--r--   0        0        0     4791 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/heston.py
+-rw-r--r--   0        0        0     2862 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/jump_diffusion.py
+-rwxr-xr-x   0        0        0     6032 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/ou.py
+-rwxr-xr-x   0        0        0     5764 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/poisson.py
+-rw-r--r--   0        0        0     1492 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/sp/weiner.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/bins.py
+-rw-r--r--   0        0        0      252 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/dates.py
+-rw-r--r--   0        0        0     3330 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/distributions.py
+-rwxr-xr-x   0        0        0      496 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/functions.py
+-rw-r--r--   0        0        0     1265 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/interest_rates.py
+-rw-r--r--   0        0        0     9909 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/marginal.py
+-rw-r--r--   0        0        0      370 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/numbers.py
+-rwxr-xr-x   0        0        0     3689 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/paths.py
+-rw-r--r--   0        0        0     4185 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/plot.py
+-rw-r--r--   0        0        0     5987 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/transforms.py
+-rw-r--r--   0        0        0      721 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/types.py
+-rw-r--r--   0        0        0     2091 2023-07-20 16:33:40.751003 quantflow-0.2.3/quantflow/utils/volatility.py
+-rw-r--r--   0        0        0     1342 2023-07-20 16:33:40.751003 quantflow-0.2.3/readme.md
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 quantflow-0.2.3/PKG-INFO
```

### Comparing `quantflow-0.2.2/LICENSE` & `quantflow-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/pyproject.toml` & `quantflow-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantflow"
-version = "0.2.2"
+version = "0.2.3"
 description = "quantitative analysis"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/quantmind/quantflow"
@@ -23,14 +23,18 @@
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
 mypy = "^1.4.0"
 ghp-import = "^2.0.2"
 ruff = "^0.0.277"
 pytest-asyncio = "^0.21.1"
 
+
+[tool.poetry.group.bok.dependencies]
+ipywidgets = "^8.0.7"
+
 [tool.poetry.extras]
 data = ["aiohttp"]
 
 [tool.poetry.group.book]
 optional = true
 
 [tool.poetry.group.book.dependencies]
```

### Comparing `quantflow-0.2.2/quantflow/data/client.py` & `quantflow-0.2.3/quantflow/data/client.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/data/fmp.py` & `quantflow-0.2.3/quantflow/data/fmp.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/options/bs.py` & `quantflow-0.2.3/quantflow/options/bs.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/options/calibration.py` & `quantflow-0.2.3/quantflow/options/calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             self.get_params(),
             method=self.minimize_method,
             bounds=self.get_bounds(),
             constraints=self.get_constraints(),
         )
 
     def cost_weight(self, ttm: float, moneyness: float) -> float:
-        return np.exp(-self.moneyness_weight * moneyness * moneyness)
+        return np.exp(-self.moneyness_weight * moneyness)
 
     def penalize(self) -> float:
         """Penalize the cost function"""
         return 0.0
 
     def cost_function(self, params: np.ndarray) -> float:
         """Calculate the cost function from the model prices"""
```

### Comparing `quantflow-0.2.2/quantflow/options/inputs.py` & `quantflow-0.2.3/quantflow/options/inputs.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/options/pricer.py` & `quantflow-0.2.3/quantflow/options/pricer.py`

 * *Files 20% similar despite different names*

```diff
@@ -94,17 +94,17 @@
     def black(self) -> MaturityPricer:
         """Calculate the Maturity Result for the Black model with same std"""
         return self._replace(
             call=black_call(self.moneyness, self.std / np.sqrt(self.ttm), ttm=self.ttm),
             name="Black",
         )
 
-    def plot(self, series: str = "implied_vol") -> Any:
+    def plot(self, series: str = "implied_vol", **kwargs: Any) -> Any:
         """Plot the results"""
-        return plot.plot_vol_cross(self.df, series=series)
+        return plot.plot_vol_cross(self.df, series=series, **kwargs)
 
 
 @dataclass
 class OptionPricer(Generic[M]):
     """Pricer for options"""
 
     model: M
@@ -125,17 +125,57 @@
             ttmr = ttm_int / TTM_FACTOR
             marginal = self.model.marginal(ttmr)
             transform = marginal.call_option(
                 self.n, max_moneyness=self.max_moneyness_ttm * np.sqrt(ttmr), **kwargs
             )
             self.ttm[ttm_int] = MaturityPricer(
                 ttm=ttmr,
-                std=np.max(marginal.std()),
+                std=float(np.max(marginal.std())),
                 moneyness=transform.x,
                 call=transform.y,
                 name=type(self.model).__name__,
             )
         return self.ttm[ttm_int]
 
     def call_price(self, ttm: float, moneyness: float) -> float:
         """Price a single call option"""
         return self.maturity(ttm).call_price(moneyness)
+
+    def plot3d(
+        self,
+        max_moneyness_ttm: float = 1.0,
+        support: int = 51,
+        ttm: FloatArray | None = None,
+        **kwargs: Any,
+    ) -> Any:
+        """Plot the implied vols surface
+
+        It requires plotly to be installed
+        """
+        if ttm is None:
+            ttm = np.arange(0.05, 1.0, 0.05)
+        moneyness_ttm = np.linspace(-max_moneyness_ttm, max_moneyness_ttm, support)
+        implied = np.zeros((len(ttm), len(moneyness_ttm)))
+        for i, t in enumerate(ttm):
+            maturity = self.maturity(t)
+            implied[i, :] = maturity.interp(moneyness_ttm * np.sqrt(t)).implied_vols
+        properties: dict = dict(
+            xaxis_title="moneyness_ttm",
+            yaxis_title="TTM",
+            colorscale="viridis",
+            scene=dict(
+                xaxis=dict(title="moneyness_ttm"),
+                yaxis=dict(title="TTM"),
+                zaxis=dict(title="implied_vol"),
+            ),
+            scene_camera=dict(eye=dict(x=1.2, y=-1.8, z=0.3)),
+            contours=dict(
+                x=dict(show=True, color="white"), y=dict(show=True, color="white")
+            ),
+        )
+        properties.update(kwargs)
+        return plot.plot3d(
+            x=moneyness_ttm,
+            y=ttm,
+            z=implied,
+            **properties,
+        )
```

### Comparing `quantflow-0.2.2/quantflow/options/surface.py` & `quantflow-0.2.3/quantflow/options/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,15 +391,15 @@
     def option_list(
         self,
         *,
         select: OptionSelection = OptionSelection.best,
         index: int | None = None,
         converged: bool = True,
     ) -> list[OptionPrice]:
-        "List of all option prices in the surface"
+        "List of selected option prices in the surface"
         return list(self.option_prices(select=select, index=index, converged=converged))
 
     def bs(
         self,
         *,
         select: OptionSelection = OptionSelection.best,
         index: int | None = None,
@@ -478,14 +478,24 @@
             moneyness=np.array(moneyness),
             price=np.array(price),
             ttm=np.array(ttm),
             implied_vol=np.array(vol),
             call_put=np.array(call_put),
         )
 
+    def disable_outliers(self, quantile: float = 0.99, repeat: int = 2) -> VolSurface:
+        for _ in range(repeat):
+            option_prices = self.option_list()
+            implied_vols = [o.implied_vol for o in option_prices]
+            exclude_above = np.quantile(implied_vols, quantile)
+            for option in option_prices:
+                if option.implied_vol > exclude_above:
+                    option.converged = False
+        return self
+
     def plot(
         self,
         *,
         index: int | None = None,
         select: OptionSelection = OptionSelection.best,
         **kwargs: Any,
     ) -> Any:
```

### Comparing `quantflow-0.2.2/quantflow/sp/bns.py` & `quantflow-0.2.3/quantflow/sp/bns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
 import numpy as np
 from pydantic import Field
 from scipy.special import xlogy
 
 from ..utils.paths import Paths
-from ..utils.types import Vector
+from ..utils.types import FloatArrayLike, Vector
 from .base import Im, StochasticProcess1D
 from .ou import GammaOU
 
 
 class BNS(StochasticProcess1D):
     """Barndorff-Nielson--Shephard (BNS) stochastic volatility model"""
 
     variance_process: GammaOU = Field(
-        default_factory=GammaOU, description="Variance process"
+        default_factory=GammaOU.create, description="Variance process"
     )
     rho: float = Field(default=0, ge=-1, le=1, description="Correlation")
 
     @classmethod
     def create(cls, vol: float, kappa: float, decay: float, rho: float) -> BNS:
         return cls(
             variance_process=GammaOU.create(rate=vol * vol, kappa=kappa, decay=decay),
             rho=rho,
         )
 
-    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+    def characteristic_exponent(self, t: FloatArrayLike, u: Vector) -> Vector:
         return -self._zeta(t, 0.5 * Im * u * u, self.rho * u)
 
     def sample(self, n: int, time_horizon: float = 1, time_steps: int = 100) -> Paths:
         return self.sample_from_draws(Paths.normal_draws(n, time_horizon, time_steps))
 
     def sample_from_draws(self, path_dw: Paths, *args: Paths) -> Paths:
         if args:
```

### Comparing `quantflow-0.2.2/quantflow/sp/cir.py` & `quantflow-0.2.3/quantflow/sp/cir.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import enum
 
 import numpy as np
 from pydantic import Field
 from scipy import special
 from scipy.optimize import Bounds
 
-from quantflow.utils.types import Vector
+from quantflow.utils.types import FloatArrayLike, Vector
 
 from ..utils.paths import Paths
-from .base import Im, IntensityProcess, StochasticProcess1DMarginal
+from .base import Im, IntensityProcess
 
 
 class SamplingAlgorithm(str, enum.Enum):
     euler = "euler"
     milstein = "milstein"
     implicit = "implicit"
 
@@ -47,17 +47,14 @@
     def is_positive(self) -> bool:
         return self.kappa * self.theta >= 0.5 * self.sigma2
 
     @property
     def sigma2(self) -> float:
         return self.sigma * self.sigma
 
-    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
-        return CIRMarginal(process=self, t=t)
-
     def sample(
         self, paths: int, time_horizon: float = 1, time_steps: int = 100
     ) -> Paths:
         draws = Paths.normal_draws(paths, time_horizon, time_steps)
         return self.sample_from_draws(draws)
 
     def sample_from_draws(self, paths: Paths, *args: Paths) -> Paths:
@@ -112,53 +109,51 @@
         sigma2 = sigma * sigma
         s2u = iu * sigma2
         c = s2u + (2 * kappa - s2u) * ekt
         b = 2 * kappa * iu / c
         a = 2 * kappa * self.theta * (kt + np.log(2 * kappa / c)) / sigma2
         return -a - b * self.rate
 
-    def cumulative_characteristic(self, t: Vector, u: Vector) -> Vector:
+    def integrated_log_laplace(self, t: Vector, u: Vector) -> Vector:
         iu = Im * u
         sigma = self.sigma
         kappa = self.kappa
         sigma2 = sigma * sigma
         gamma = np.sqrt(kappa * kappa - 2 * iu * sigma2)
         egt = np.exp(gamma * t)
         c = (gamma + kappa) * (1 - egt) - 2 * gamma
         d = 2 * gamma * np.exp(0.5 * (gamma + kappa) * t)
         a = 2 * self.theta * kappa * np.log(-d / c) / sigma2
         b = 2 * iu * (1 - egt) / c
-        return np.exp(a + b * self.rate)
+        return -a - b * self.rate
 
     def domain_range(self) -> Bounds:
         return Bounds(0, np.inf)
 
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
+        ekt = self.ekt(t)
+        return self.rate * ekt + self.theta * (1 - ekt)
 
-class CIRMarginal(StochasticProcess1DMarginal[CIR]):
-    def mean(self) -> Vector:
-        ekt = np.exp(-self.process.kappa * self.t)
-        return self.process.rate * ekt + self.process.theta * (1 - ekt)
-
-    def variance(self) -> Vector:
-        kappa = self.process.kappa
-        ekt = np.exp(-kappa * self.t)
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
+        kappa = self.kappa
+        ekt = self.ekt(t)
         return (
-            self.process.sigma2
+            self.sigma2
             * (1 - ekt)
-            * (self.process.rate * ekt + 0.5 * self.process.theta * (1 - ekt))
+            * (self.rate * ekt + 0.5 * self.theta * (1 - ekt))
             / kappa
         )
 
-    def pdf(self, x: Vector) -> Vector:
-        k = self.process.kappa
-        s2 = self.process.sigma2
-        ekt = np.exp(-k * self.t)
+    def analytical_pdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        k = self.kappa
+        s2 = self.sigma2
+        ekt = self.ekt(t)
         c = 2 * k / (1 - ekt) / s2
-        q = 2 * k * self.process.theta / s2 - 1
-        u = c * ekt * self.process.rate
+        q = 2 * k * self.theta / s2 - 1
+        u = c * ekt * self.rate
         v = c * x
         return (
             c
             * np.exp(-v - u)
             * np.power(v / u, 0.5 * q)
             * special.iv(q, 2 * np.sqrt(u * v))
         )
```

### Comparing `quantflow-0.2.2/quantflow/sp/dsp.py` & `quantflow-0.2.3/quantflow/sp/dsp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
-from typing import List
 
 import numpy as np
 from pydantic import Field
 
-from ..utils.types import Vector, as_array
+from ..utils.types import FloatArray, FloatArrayLike, Vector, as_array
 from .base import Im
 from .cir import CIR, IntensityProcess
 from .poisson import PoissonBase, PoissonProcess, poisson_arrivals
 
 
 class DSP(PoissonBase):
     r"""
@@ -41,21 +40,21 @@
     def cdf(self, t: float, n: Vector) -> Vector:
         """CDF of the number of events at time t.
 
         It is obtained form cumulative summation of :class:`pdf`
         """
         return np.cumsum(self.pdf(t, n))
 
-    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+    def characteristic_exponent(self, t: FloatArrayLike, u: Vector) -> Vector:
         return self.poisson.characteristic_exponent(t, u)
 
-    def characteristic(self, t: Vector, u: Vector) -> Vector:
+    def characteristic(self, t: FloatArrayLike, u: Vector) -> Vector:
         phi = self.characteristic_exponent(t, u)
-        return self.intensity.cumulative_characteristic(t, -Im * phi)
+        return np.exp(self.intensity.integrated_log_laplace(t, -Im * phi))
 
-    def arrivals(self, t: float = 1) -> List[float]:
+    def arrivals(self, t: float = 1) -> list[float]:
         paths = self.intensity.sample(1, t, math.ceil(100 * t)).integrate()
         intensity = paths.data[-1, 0]
         return poisson_arrivals(intensity, t)
 
-    def sample_jumps(self, n: int) -> np.ndarray:
+    def sample_jumps(self, n: int) -> FloatArray:
         return self.poisson.sample_jumps(n)
```

### Comparing `quantflow-0.2.2/quantflow/sp/ou.py` & `quantflow-0.2.3/quantflow/sp/ou.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,117 @@
 from __future__ import annotations
 
-from typing import cast
+from typing import Generic
 
 import numpy as np
 from pydantic import Field
+from scipy.optimize import Bounds
 from scipy.stats import gamma, norm
 
 from ..utils.distributions import Exponential
 from ..utils.paths import Paths
-from ..utils.types import Vector
-from .base import Im, IntensityProcess, StochasticProcess1DMarginal
-from .poisson import CompoundPoissonProcess
+from ..utils.types import FloatArrayLike, Vector
+from .base import Im, IntensityProcess
+from .poisson import CompoundPoissonProcess, D
 from .weiner import WeinerProcess
 
 
 class Vasicek(IntensityProcess):
+    """Gaussian OU process, also know as the Vasiceck model.
+
+    Strictly, it is not an intensity process since it is not positive
+    """
+
     bdlp: WeinerProcess = Field(
         default_factory=WeinerProcess,
         description="Background driving Weiner process",
     )
     theta: float = Field(default=1.0, gt=0, description="Mean rate")
 
+    def characteristic_exponent(self, t: FloatArrayLike, u: Vector) -> Vector:
+        mu = self.analytical_mean(t)
+        var = self.analytical_variance(t)
+        return u * (-complex(0, 1) * mu + 0.5 * var * u)
+
+    def integrated_log_laplace(self, t: FloatArrayLike, u: Vector) -> Vector:
+        raise NotImplementedError
+
+    def sample(self, n: int, time_horizon: float = 1, time_steps: int = 100) -> Paths:
+        paths = Paths.normal_draws(n, time_horizon, time_steps)
+        return self.sample_from_draws(paths)
+
+    def sample_from_draws(self, draws: Paths, *args: Paths) -> Paths:
+        kappa = self.kappa
+        theta = self.theta
+        dt = draws.dt
+        sdt = self.bdlp.sigma * np.sqrt(dt)
+        paths = np.zeros(draws.data.shape)
+        paths[0, :] = self.rate
+        for t in range(draws.time_steps):
+            w = sdt * draws.data[t, :]
+            x = paths[t, :]
+            dx = kappa * (theta - x) * dt + sdt * w
+            paths[t + 1, :] = x + dx
+        return Paths(t=draws.t, data=paths)
+
+    def domain_range(self) -> Bounds:
+        return Bounds(-np.inf, np.inf)
+
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
+        ekt = self.ekt(t)
+        return self.rate * ekt + self.theta * (1 - ekt)
 
-class NGOU(IntensityProcess):
-    bdlp: CompoundPoissonProcess = Field(
-        default_factory=CompoundPoissonProcess,
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
+        ekt = self.ekt(2 * t)
+        return 0.5 * self.bdlp.sigma2 * (1 - ekt) / self.kappa
+
+    def analytical_pdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        return norm.pdf(x, loc=self.analytical_mean(t), scale=self.analytical_std(t))
+
+    def analytical_cdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        return norm.cdf(x, loc=self.analytical_mean(t), scale=self.analytical_std(t))
+
+
+class NGOU(IntensityProcess, Generic[D]):
+    bdlp: CompoundPoissonProcess[D] = Field(
         description="Background driving Levy process",
     )
 
     def sample_from_draws(self, draws: Paths, *args: Paths) -> Paths:
         raise NotImplementedError
 
 
-class GammaOU(NGOU):
+class GammaOU(NGOU[Exponential]):
     @property
     def intensity(self) -> float:
         return self.bdlp.intensity
 
     @property
     def beta(self) -> float:
         # TODO: find a better way for this
-        return cast(Exponential, self.bdlp.jumps).decay
+        return self.bdlp.jumps.decay
 
     @classmethod
     def create(cls, rate: float = 1, decay: float = 1, kappa: float = 1) -> GammaOU:
         return cls(
             rate=rate,
             kappa=kappa,
-            bdlp=CompoundPoissonProcess(
+            bdlp=CompoundPoissonProcess[Exponential](
                 intensity=rate * decay, jumps=Exponential(decay=decay)
             ),
         )
 
-    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
-        return GammaOUMarginal(process=self, t=t)
-
-    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
+    def characteristic_exponent(self, t: FloatArrayLike, u: Vector) -> Vector:
         b = self.beta
         iu = Im * u
         c1 = iu * np.exp(-self.kappa * t)
         c0 = self.intensity * np.log((b - c1) / (b - iu))
         return -c0 - c1 * self.rate
 
-    def cumulative_characteristic(self, t: Vector, u: Vector) -> Vector:
+    def integrated_log_laplace(self, t: FloatArrayLike, u: Vector) -> Vector:
         kappa = self.kappa
         b = self.beta
         iu = Im * u
         iuk = iu / kappa
         ekt = np.exp(-kappa * t)
         c1 = iuk * (1 - ekt)
         c0 = self.intensity * (
@@ -101,44 +146,26 @@
         kappa = self.kappa
         t0 = i * dt
         t1 = t0 + dt
         a = arrival or t1
         pp[i] = x - kappa * x * (a - t0) - kappa * (x + jump) * (t1 - a) + jump
         return i + 1
 
-    def cumulative_characteristic2(self, t: float, u: Vector) -> Vector:
+    def cumulative_characteristic2(self, t: FloatArrayLike, u: Vector) -> Vector:
         """Formula from a paper"""
         kappa = self.kappa
         b = self.beta
         iu = Im * u
         iuk = iu / kappa
         ekt = np.exp(-kappa * t)
         c1 = iuk * (1 - ekt)
         c0 = self.intensity * (b * np.log(b / (b - c1)) - iu * t) / (iuk - b)
         return np.exp(c0 + c1 * self.rate)
 
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
+        return self.intensity / self.beta
 
-class GammaOUMarginal(StochasticProcess1DMarginal[GammaOU]):
-    def mean(self) -> float:
-        return self.process.intensity / self.process.beta
-
-    def variance(self) -> float:
-        return self.process.intensity / self.process.beta / self.process.beta
-
-    def pdf(self, x: Vector) -> Vector:
-        return gamma.pdf(x, self.process.intensity, scale=1 / self.process.beta)
-
-
-class VasicekMarginal(StochasticProcess1DMarginal[Vasicek]):
-    def mean(self) -> Vector:
-        ekt = self.process.ekt(self.t)
-        return self.process.rate * ekt + self.process.theta * (1 - ekt)
-
-    def variance(self) -> Vector:
-        ekt = self.process.ekt(2 * self.t)
-        return 0.5 * self.process.bdlp.sigma2 * (1 - ekt) / self.process.kappa
-
-    def pdf(self, n: Vector) -> Vector:
-        return norm.pdf(n, loc=self.mean(), scale=self.std())
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
+        return self.intensity / self.beta / self.beta
 
-    def cdf(self, n: Vector) -> Vector:
-        return norm.cdf(n, loc=self.mean(), scale=self.std())
+    def analytical_pdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        return gamma.pdf(x, self.intensity, scale=1 / self.beta)
```

### Comparing `quantflow-0.2.2/quantflow/sp/poisson.py` & `quantflow-0.2.3/quantflow/sp/poisson.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from abc import abstractmethod
+from typing import Generic, TypeVar
 
 import numpy as np
 from pydantic import Field
 from scipy.optimize import Bounds
 from scipy.stats import poisson
 
-from ..utils.distributions import Distribution1D, Exponential
+from ..utils.distributions import Distribution1D
 from ..utils.functions import factorial
 from ..utils.paths import Paths
-from ..utils.types import FloatArray, Vector
-from .base import Im, StochasticProcess1D, StochasticProcess1DMarginal
+from ..utils.types import FloatArray, FloatArrayLike, Vector
+from .base import Im, StochasticProcess1D
+
+D = TypeVar("D", bound=Distribution1D)
 
 
 class PoissonBase(StochasticProcess1D):
     @abstractmethod
     def sample_jumps(self, n: int) -> np.ndarray:
         """Generate a list of jump sizes"""
 
@@ -56,123 +59,111 @@
             arrivals.append(tt)
     return arrivals
 
 
 class PoissonProcess(PoissonBase):
     intensity: float = Field(default=1.0, ge=0, description="intensity rate")
 
-    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
-        return PoissonMarginal(process=self, t=t)
-
     def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
         return t * self.intensity * (1 - np.exp(Im * u))
 
     def arrivals(self, time_horizon: float = 1) -> list[float]:
         return poisson_arrivals(self.intensity, time_horizon)
 
     def sample_jumps(self, n: int) -> np.ndarray:
         """For a poisson process this is just a list of 1s"""
         return np.ones((n,))
 
-    def max_frequency(self, t: Vector) -> float:
-        """Maximum frequency of the process"""
-        return 2 * np.pi
+    def frequency_range(self, std: float, max_frequency: float | None = None) -> Bounds:
+        """Frequency range of the process"""
+        return Bounds(0, np.pi)
 
     def support(self, mean: float, std: float, points: int) -> FloatArray:
         """Support of the process at time `t`"""
         return np.linspace(0, points, points + 1)
 
-
-class CompoundPoissonProcess(PoissonBase):
-    r"""
-    1D Poisson process.
-
-    It's a process where the inter-arrival time is exponentially distributed
-    with rate :math:`\lambda`
-
-    .. attribute:: rate
-
-        The arrival rate of events. Must be positive.
-    """
-    intensity: float = Field(default=1.0, ge=0, description="intensity rate")
-    jumps: Distribution1D = Field(
-        default_factory=Exponential, description="Jump size distribution"
-    )
-
-    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
-        return CompoundPoissonMarginal(process=self, t=t)
-
-    def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
-        return t * self.intensity * (1 - self.jumps.characteristic(u))
-
-    def arrivals(self, time_horizon: float = 1) -> list[float]:
-        """Same as Poisson process"""
-        return poisson_arrivals(self.intensity, time_horizon)
-
-    def sample_jumps(self, n: int) -> np.ndarray:
-        """Sample jump sizes from an exponential distribution with rate
-        parameter :class:b
-        """
-        return self.jumps.sample(n)
-
-
-class PoissonMarginal(StochasticProcess1DMarginal[PoissonProcess]):
-    def mean(self) -> Vector:
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
         """Expected value at a time horizon"""
-        return self.process.intensity * self.t
+        return self.intensity * t
 
-    def variance(self) -> Vector:
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
         """Expected variance at a time horizon"""
-        return self.process.intensity * self.t
+        return self.intensity * t
 
-    def cdf(self, n: Vector) -> Vector:
+    def analytical_cdf(self, t: FloatArrayLike, n: FloatArrayLike) -> FloatArrayLike:
         r"""
         CDF of the number of events at time ``t``.
 
         It's given by
 
         .. math::
             :label: poisson_cdf
 
             F_{X}\left(n\right)=\frac{\Gamma\left(\left\lfloor n+1\right\rfloor
             ,\lambda\right)}{\left\lfloor n\right\rfloor !}
 
         where :math:`\Gamma` is the upper incomplete gamma function.
         """
-        return poisson.cdf(n, self.t * self.process.intensity)
+        return poisson.cdf(n, t * self.intensity)
 
-    def pdf(self, n: Vector = 0) -> Vector:
+    def analytical_pdf(self, t: FloatArrayLike, n: FloatArrayLike) -> FloatArrayLike:
         r"""
         Probability density function of the number of events at time ``t``.
 
         It's given by
 
         \begin{equation}
            f_{X}\left(n\right)=\frac{\lambda^{n}e^{-\lambda}}{n!}
         \end{equation}
         """
-        return poisson.pmf(n, self.t * self.process.intensity)
+        return poisson.pmf(n, t * self.intensity)
 
-    def cdf_jacobian(self, n: Vector) -> np.ndarray:
+    def cdf_jacobian(self, t: FloatArrayLike, n: Vector) -> np.ndarray:
         r"""
         Jacobian of the CDF
 
         It's given by
 
         .. math::
 
             \frac{\partial F}{\partial\lambda}=-\frac{\lambda^{\left\lfloor
             n\right\rfloor }e^{-\lambda}}{\left\lfloor n\right\rfloor !}
         """
         k = np.floor(n).astype(int)
-        rate = self.process.intensity
+        rate = self.intensity
         return np.array([-(rate**k) * np.exp(-rate)]) / factorial(k)
 
 
-class CompoundPoissonMarginal(StochasticProcess1DMarginal[CompoundPoissonProcess]):
-    def mean(self) -> Vector:
+class CompoundPoissonProcess(PoissonBase, Generic[D]):
+    r"""
+    1D Poisson process.
+
+    It's a process where the inter-arrival time is exponentially distributed
+    with rate :math:`\lambda`
+
+    .. attribute:: rate
+
+        The arrival rate of events. Must be positive.
+    """
+    intensity: float = Field(default=1.0, ge=0, description="intensity rate")
+    jumps: D = Field(description="Jump size distribution")
+
+    def characteristic_exponent(self, t: FloatArrayLike, u: Vector) -> Vector:
+        return t * self.intensity * (1 - self.jumps.characteristic(u))
+
+    def arrivals(self, time_horizon: float = 1) -> list[float]:
+        """Same as Poisson process"""
+        return poisson_arrivals(self.intensity, time_horizon)
+
+    def sample_jumps(self, n: int) -> FloatArray:
+        """Sample jump sizes from an exponential distribution with rate
+        parameter :class:b
+        """
+        return self.jumps.sample(n)
+
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
         """Expected value at a time horizon"""
-        return self.process.intensity * self.t * self.process.jumps.mean()
+        return self.intensity * t * self.jumps.mean()
 
-    def variance(self) -> Vector:
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
         """Expected variance at a time horizon"""
-        return 2 * self.process.intensity * self.t * self.process.jumps.variance()
+        return self.intensity * t * (self.jumps.variance() + self.jumps.mean() ** 2)
```

### Comparing `quantflow-0.2.2/quantflow/sp/weiner.py` & `quantflow-0.2.3/quantflow/sp/weiner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from __future__ import annotations
 
 import numpy as np
 from pydantic import Field
 from scipy.stats import norm
 
 from ..utils.paths import Paths
-from ..utils.types import Vector
-from .base import StochasticProcess1D, StochasticProcess1DMarginal
+from ..utils.types import FloatArrayLike, Vector
+from .base import StochasticProcess1D
 
 
 class WeinerProcess(StochasticProcess1D):
     sigma: float = Field(default=1, ge=0, description="volatility")
 
     @property
     def sigma2(self) -> float:
         return self.sigma * self.sigma
 
-    def marginal(self, t: Vector) -> StochasticProcess1DMarginal:
-        return WeinerMarginal(process=self, t=t)
-
     def characteristic_exponent(self, t: Vector, u: Vector) -> Vector:
         su = self.sigma * u
         return 0.5 * su * su * t
 
     def sample(self, n: int, time_horizon: float = 1, time_steps: int = 100) -> Paths:
         paths = Paths.normal_draws(n, time_horizon, time_steps)
         return self.sample_from_draws(paths)
 
     def sample_from_draws(self, draws: Paths, *args: Paths) -> Paths:
         self.sigma * np.sqrt(draws.dt)
         paths = np.zeros(draws.data.shape)
         paths[1:] = np.cumsum(draws.data[:-1], axis=0)
         return Paths(t=draws.t, data=paths)
 
+    def analytical_mean(self, t: FloatArrayLike) -> FloatArrayLike:
+        return 0 * t
 
-class WeinerMarginal(StochasticProcess1DMarginal[WeinerProcess]):
-    def mean(self) -> Vector:
-        return 0 * self.t
-
-    def variance(self) -> Vector:
-        s = self.process.sigma
-        return s * s * self.t
+    def analytical_variance(self, t: FloatArrayLike) -> FloatArrayLike:
+        return t * self.sigma2
 
-    def pdf(self, n: Vector) -> Vector:
-        return norm.pdf(n, scale=self.std())
+    def analytical_pdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        return norm.pdf(x, scale=self.analytical_std(t))
 
-    def cdf(self, n: Vector) -> Vector:
-        return norm.cdf(n, scale=self.std())
+    def analytical_cdf(self, t: FloatArrayLike, x: FloatArrayLike) -> FloatArrayLike:
+        return norm.cdf(x, scale=self.analytical_std(t))
```

### Comparing `quantflow-0.2.2/quantflow/utils/interest_rates.py` & `quantflow-0.2.3/quantflow/utils/interest_rates.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/utils/marginal.py` & `quantflow-0.2.3/quantflow/utils/marginal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,235 +1,250 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, cast
+from typing import Callable, cast
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel
 from scipy.optimize import Bounds
 
 from .transforms import Transform, TransformResult, default_bounds
-from .types import FloatArray, Vector
+from .types import FloatArray, FloatArrayLike, Vector
 
 
-class Marginal1D(BaseModel, ABC):
+class Marginal1D(BaseModel, ABC, extra="forbid"):
     """Marginal distribution"""
 
     @abstractmethod
     def characteristic(self, u: Vector) -> Vector:
         """
         Compute the characteristic function on support points `n`.
         """
 
     @abstractmethod
     def support(self, points: int = 100, *, std_mult: float = 3) -> FloatArray:
         """
         Compute the x axis.
         """
 
-    def mean(self) -> Vector:
+    def mean(self) -> FloatArrayLike:
         """Expected value
 
-        THis should be overloaded if a more efficient way of computing the mean
+        This should be overloaded if a more efficient way of computing the mean
         """
         return self.mean_from_characteristic()
 
-    def variance(self) -> Vector:
+    def variance(self) -> FloatArrayLike:
         """Variance
 
         This should be overloaded if a more efficient way of computing the
         """
         return self.variance_from_characteristic()
 
-    def max_frequency(self) -> float:
-        """Maximum frequency of the characteristic function
+    def domain_range(self) -> Bounds:
+        """The space domain range for the random variable
+
+        This should be overloaded if required
+        """
+        return default_bounds()
+
+    def frequency_range(self, max_frequency: float | None = None) -> float:
+        """The frequency domain range for the characteristic function
 
         This should be overloaded if required
         """
-        return 20
+        return Bounds(0, max_frequency or 20)
 
-    def std(self) -> Vector:
+    def std(self) -> FloatArrayLike:
         """Standard deviation at a time horizon"""
         return np.sqrt(self.variance())
 
-    def mean_from_characteristic(self) -> Vector:
+    def mean_from_characteristic(self) -> FloatArrayLike:
         """Calculate mean as first derivative of characteristic function at 0"""
         d = 0.001
         m = -0.5 * 1j * (self.characteristic(d) - self.characteristic(-d)) / d
         return cast(complex, m).real
 
-    def variance_from_characteristic(self) -> Vector:
+    def std_from_characteristic(self) -> FloatArrayLike:
+        """Calculate standard deviation as square root of variance"""
+        return np.sqrt(self.variance_from_characteristic())
+
+    def variance_from_characteristic(self) -> FloatArrayLike:
         """Calculate variance as second derivative of characteristic function at 0"""
         d = 0.001
         c1 = self.characteristic(d)
         c0 = self.characteristic(0)
         c2 = self.characteristic(-d)
         m = -0.5 * 1j * (c1 - c2) / d
         s = -(c1 - 2 * c0 + c2) / (d * d) - m * m
         return s.real
 
-    def pdf(self, n: Vector) -> Vector:
+    def pdf(self, x: FloatArrayLike) -> FloatArrayLike:
         """
         Computes the probability density (or mass) function of the process.
 
         It has a base implementation that computes the pdf from the
         :class:`cdf` method, but a subclass should overload this method if a
         more optimized way of computing it is available.
 
         :param n: Location in the stochastic process domain space. If a numpy array,
             the output should have the same shape as the input.
         """
-        return self.cdf(n) - self.cdf(n - 1)
+        return self.cdf(x) - self.cdf(x - 1)
 
     def pdf_from_characteristic(
         self,
         n: int | None = None,
         *,
         max_frequency: float | None = None,
         simpson_rule: bool = False,
         use_fft: bool = False,
     ) -> TransformResult:
         """
         Compute the probability density function from the characteristic function.
+
+        :param n: Number of discretization points to use in the transform.
+            If None, use 128.
+        :param max_frequency: The maximum frequency to use in the transform. If not
+            provided, the value from the :meth:`frequency_range` method is used.
+            Only needed for special cases/testing.
+        :param simpson_rule: Use Simpson's rule for integration. Default is False.
+        :param use_fft: Use FFT for the transform. Default is False.
         """
-        n = n or 128
-        if use_fft:
-            delta_x = None
-            transform = Transform(
-                n,
-                max_frequency=self.get_max_frequency(max_frequency),
-                domain_range=self.domain_range(),
-                simpson_rule=simpson_rule,
-            )
-        else:
-            x = self.support(n + 1)
-            min_x = float(np.min(x))
-            max_x = float(np.max(x))
-            delta_x = (max_x - min_x) / (len(x) - 1)
-            transform = Transform(
-                n,
-                max_frequency=self.get_max_frequency(max_frequency),
-                domain_range=Bounds(min_x, max_x),
-                simpson_rule=simpson_rule,
-            )
+        transform = self.get_transform(
+            n,
+            self.support,
+            max_frequency=max_frequency,
+            simpson_rule=simpson_rule,
+            use_fft=use_fft,
+        )
         psi = cast(np.ndarray, self.characteristic(transform.frequency_domain))
-        return transform(psi, delta_x)
+        return transform(psi, use_fft=use_fft)
 
     def call_option(
         self,
         n: int | None = None,
         *,
         max_frequency: float | None = None,
         max_moneyness: float = 1,
         alpha: float | None = None,
         simpson_rule: bool = False,
+        use_fft: bool = False,
     ) -> TransformResult:
-        n = n or 128
-        x = self.option_support(n + 1, max_moneyness=max_moneyness)
-        min_x = float(np.min(x))
-        max_x = float(np.max(x))
-        delta_x = (max_x - min_x) / (len(x) - 1)
-        transform = Transform(
+        transform = self.get_transform(
             n,
-            max_frequency=self.get_max_frequency(max_frequency),
-            domain_range=Bounds(min_x, max_x),
+            lambda m: self.option_support(m + 1, max_moneyness=max_moneyness),
+            max_frequency=max_frequency,
             simpson_rule=simpson_rule,
+            use_fft=use_fft,
         )
         alpha = alpha or self.option_alpha()
         phi = cast(
             np.ndarray,
             self.call_option_transform(transform.frequency_domain - 1j * alpha),
         )
-        result = transform(phi, delta_x)
+        result = transform(phi, use_fft=use_fft)
         return TransformResult(x=result.x, y=result.y * np.exp(-alpha * result.x))
 
     def option_time_value(
         self,
         n: int = 128,
         *,
         max_frequency: float | None = None,
         max_moneyness: float = 1,
         alpha: float = 1.1,
         simpson_rule: bool = False,
+        use_fft: bool = False,
     ) -> TransformResult:
         """Option time value"""
-        n = n or 128
-        x = self.option_support(n + 1, max_moneyness=max_moneyness)
-        min_x = float(np.min(x))
-        max_x = float(np.max(x))
-        delta_x = (max_x - min_x) / (len(x) - 1)
-        transform = Transform(
+        transform = self.get_transform(
             n,
-            max_frequency=self.get_max_frequency(max_frequency),
-            domain_range=Bounds(min_x, max_x),
+            lambda m: self.option_support(m + 1, max_moneyness=max_moneyness),
+            max_frequency=max_frequency,
             simpson_rule=simpson_rule,
+            use_fft=use_fft,
         )
         phi = cast(
             np.ndarray,
             self.option_time_value_transform(transform.frequency_domain, alpha),
         )
-        result = transform(phi, delta_x)
+        result = transform(phi, use_fft=use_fft)
         time_value = result.y / np.sinh(alpha * result.x)
         return TransformResult(x=result.x, y=time_value)
 
-    def domain_range(self) -> Bounds:
-        return default_bounds()
+    def characteristic_df(
+        self,
+        n: int | None = None,
+        *,
+        max_frequency: float | None = None,
+        simpson_rule: bool = False,
+    ) -> pd.DataFrame:
+        """
+        Compute the characteristic function with n discretization points
+        and a max frequency
+        """
+        transform = self.get_transform(
+            n,
+            self.support,
+            max_frequency=max_frequency,
+            simpson_rule=simpson_rule,
+        )
+        psi = self.characteristic(transform.frequency_domain)
+        return transform.characteristic_df(cast(np.ndarray, psi))
+
+    def get_transform(
+        self,
+        n: int | None,
+        support: Callable[[int], FloatArray],
+        *,
+        max_frequency: float | None = None,
+        simpson_rule: bool = False,
+        use_fft: bool = False,
+    ) -> Transform:
+        n = n or 128
+        if use_fft:
+            bounds = self.domain_range()
+        else:
+            x = support(n)
+            bounds = Bounds(float(np.min(x)), float(np.max(x)))
+        return Transform.create(
+            n,
+            frequency_range=self.frequency_range(max_frequency),
+            domain_range=bounds,
+            simpson_rule=simpson_rule,
+        )
 
-    def cdf(self, n: Vector) -> Vector:
+    def cdf(self, x: FloatArrayLike) -> FloatArrayLike:
         """
         Compute the cumulative distribution function
 
         :param n: Location in the stochastic process domain space. If a numpy array,
             the output should have the same shape as the input.
         """
         raise NotImplementedError("Analytical CFD not available")
 
-    def pdf_jacobian(self, n: Vector) -> np.ndarray:
+    def pdf_jacobian(self, x: FloatArrayLike) -> FloatArrayLike:
         """
         Jacobian of the pdf with respect to the parameters of the process.
         It has a base implementation that computes it from the
         :class:`cdf_jacobian` method, but a subclass should overload this method if a
         more optimized way of computing it is available.
         """
-        return self.cdf_jacobian(n) - self.cdf_jacobian(n - 1)
+        return self.cdf_jacobian(x) - self.cdf_jacobian(x - 1)
 
-    def cdf_jacobian(self, n: Vector) -> np.ndarray:
+    def cdf_jacobian(self, x: FloatArrayLike) -> np.ndarray:
         """
         Jacobian of the cdf with respect to the parameters of the process.
         It is useful for optimization purposes if necessary.
 
         Optional to implement, otherwise raises ``NotImplementedError`` if called.
         """
         raise NotImplementedError("Analytical CFD Jacobian not available")
 
-    def characteristic_df(
-        self, n: int | None, max_frequency: float | None = None, **kwargs: Any
-    ) -> pd.DataFrame:
-        """
-        Compute the characteristic function with n discretization points
-        and a max frequency
-        """
-        fre = Transform(
-            n=n, max_frequency=self.get_max_frequency(max_frequency), **kwargs
-        ).frequency_domain
-        psi = self.characteristic(fre)
-        return pd.concat(
-            (
-                pd.DataFrame(dict(frequency=fre, characteristic=psi.real, name="real")),
-                pd.DataFrame(dict(frequency=fre, characteristic=psi.imag, name="iamg")),
-            )
-        )
-
-    def get_max_frequency(self, max_frequency: float | None = None) -> float:
-        """
-        Get the maximum frequency to use for the characteristic function
-        """
-        return max_frequency if max_frequency is not None else self.max_frequency()
-
     def option_support(
         self, points: int = 101, max_moneyness: float = 1.0
     ) -> FloatArray:
         """
         Compute the x axis.
         """
         return np.linspace(-max_moneyness, max_moneyness, points)
```

### Comparing `quantflow-0.2.2/quantflow/utils/paths.py` & `quantflow-0.2.3/quantflow/utils/paths.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, cast
 
 import numpy as np
 import pandas as pd
 from numpy.random import normal
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, Field
 from scipy.integrate import cumtrapz
 
 from . import plot
+from .bins import pdf as bins_pdf
+from .types import FloatArray
 
 
-class Paths(BaseModel):
+class Paths(BaseModel, arbitrary_types_allowed=True):
     """Paths of a stochastic process"""
 
-    model_config = ConfigDict(arbitrary_types_allowed=True)
     t: float = Field(description="time horizon")
-    data: np.ndarray = Field(description="paths")
+    data: FloatArray = Field(description="paths")
 
     @property
     def dt(self) -> float:
         return self.t / self.time_steps
 
     @property
     def samples(self) -> int:
@@ -62,14 +63,41 @@
 
     def integrate(self) -> Paths:
         """Integrate paths"""
         return self.__class__(
             t=self.t, data=cumtrapz(self.data, dx=self.dt, axis=0, initial=0)
         )
 
+    def cross_section(self, t: float | None = None) -> FloatArray:
+        index = self.time_steps
+        if t is not None:
+            index = cast(int, t // self.dt)
+        return self.data[index, :]
+
+    def pdf(
+        self,
+        t: float | None = None,
+        num_bins: int | None = None,
+        delta: float | None = None,
+        symmetric: float | None = None,
+    ) -> pd.DataFrame:
+        """Probability density function of paths
+
+        Calculate a DataFrame with the probability density function of the paths
+        at a given cross section of time. By default it take the last section.
+
+        :param t: time at which to calculate the pdf
+        :param num_bins: number of bins
+        :param delta: optional size of bins (cannot be set with num_bins)
+        :param symmetric: optional center of bins
+        """
+        return bins_pdf(
+            self.cross_section(t), num_bins=num_bins, delta=delta, symmetric=symmetric
+        )
+
     def plot(self, **kwargs: Any) -> Any:
         return plot.plot_lines(self.df, **kwargs)
 
     @classmethod
     def normal_draws(
         cls,
         paths: int,
```

### Comparing `quantflow-0.2.2/quantflow/utils/plot.py` & `quantflow-0.2.3/quantflow/utils/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from typing import Any
 
 import pandas as pd
+from scipy.stats import norm
 
 from .marginal import Marginal1D
+from .types import FloatArray
 
 PLOTLY_THEME = os.environ.get("PLOTLY_THEME", "plotly_dark")
 
 try:
     import plotly.express as px  # type: ignore
     import plotly.graph_objects as go
     import plotly.io as pio
@@ -26,52 +28,64 @@
     check_plotly()
     return px.line(data, template=template, **kwargs)
 
 
 def plot_marginal_pdf(
     m: Marginal1D,
     n: int | None = None,
-    analytical: str = "lines",
+    *,
+    analytical: str | bool = "lines",
+    normal: bool = False,
     marker_size: int = 8,
     marker_color: str = "rgba(30, 186, 64, .5)",
+    log_y: bool = False,
     **kwargs: Any
 ) -> Any:
     """Plot the marginal pdf on an input support"""
     check_plotly()
-    result = m.pdf_from_characteristic(n, **kwargs)
-    xx = result.x
-    yy = result.y
+    pdf = m.pdf_from_characteristic(n, **kwargs)
     fig = go.Figure()
     if analytical:
         fig.add_trace(
             go.Scatter(
-                x=xx,
-                y=m.pdf(xx),
+                x=pdf.x,
+                y=m.pdf(pdf.x),
                 name="analytical",
                 mode=analytical,
             )
         )
+    if normal:
+        n = norm.pdf(pdf.x, loc=m.mean(), scale=m.std())
+        fig.add_trace(
+            go.Scatter(
+                x=pdf.x,
+                y=n,
+                name="normal",
+                mode="lines",
+            )
+        )
+
     fig.add_trace(
         go.Scatter(
-            x=xx,
-            y=yy,
-            name="characteristic",
+            x=pdf.x,
+            y=pdf.y,
+            name="characteristic PDF",
             mode="markers",
             marker_color=marker_color,
             marker_size=marker_size,
         )
     )
+    if log_y:
+        fig.update_yaxes(type="log")
     return fig
 
 
-def plot_characteristic(
-    m: Marginal1D, n: int | None = None, max_frequency: float | None = None
-) -> Any:
+def plot_characteristic(m: Marginal1D, n: int | None = None, **kwargs: Any) -> Any:
     check_plotly()
-    df = m.characteristic_df(n=n, max_frequency=max_frequency)
+    df = m.characteristic_df(n=n, **kwargs)
     return px.line(
         df,
         x="frequency",
         y="characteristic",
         color="name",
         markers=True,
     )
@@ -117,32 +131,52 @@
 ) -> Any:
     check_plotly()
     return px.scatter_3d(df, x="moneyness_ttm", y="ttm", z=series, color="side")
 
 
 def plot_vol_cross(
     data: pd.DataFrame,
+    *,
     data2: pd.DataFrame | None = None,
     series: str = "implied_vol",
     marker_size: int = 10,
+    fig: Any | None = None,
+    name: str = "model",
     **kwargs: Any
 ) -> Any:
     check_plotly()
-    fig = go.Figure()
+    fig = fig or go.Figure()
     fig.add_trace(
         go.Scatter(
             x=data["moneyness_ttm"],
             y=data[series],
-            name="model",
+            name=name,
             mode="lines",
         )
     )
     if data2 is not None:
         fig.add_trace(
             go.Scatter(
                 x=data2["moneyness_ttm"],
                 y=data2[series],
                 name="model",
                 mode="lines",
             )
         )
     return fig.update_layout(xaxis_title="moneyness_ttm", yaxis_title=series)
+
+
+def plot3d(
+    x: FloatArray,
+    y: FloatArray,
+    z: FloatArray,
+    contours: Any | None,
+    colorscale: str = "viridis",
+    **kwargs: Any
+) -> Any:
+    check_plotly()
+    fig = go.Figure(
+        data=[go.Surface(x=x, y=y, z=z, contours=contours, colorscale=colorscale)]
+    )
+    if kwargs:
+        fig.update_layout(**kwargs)
+    return fig
```

### Comparing `quantflow-0.2.2/quantflow/utils/transforms.py` & `quantflow-0.2.3/quantflow/utils/transforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, NamedTuple
 
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 from scipy.optimize import Bounds
 
 from .types import FloatArray
 
 
 class TransformError(RuntimeError):
     pass
@@ -21,14 +22,32 @@
     y: np.ndarray
 
 
 def grid(n: int) -> npt.NDArray[np.int_]:
     return np.arange(0, n, 1)
 
 
+def finite_bounds(bounds: Bounds) -> tuple[float, float]:
+    lb = float(bounds.lb[0])
+    ub = float(bounds.ub[0])
+    if np.isinf(lb) or np.isinf(ub):
+        raise ValueError(f"Bounds are not finite: {lb}, {ub}")
+    return lb, ub
+
+
+def grid_from_bounds(bounds: Bounds, n: int) -> FloatArray:
+    lb, ub = finite_bounds(bounds)
+    return np.linspace(lb, ub, n + 1)[:-1]
+
+
+def delta_from_bounds(bounds: Bounds, n: int) -> float:
+    lb, ub = finite_bounds(bounds)
+    return (ub - lb) / n
+
+
 def trapezoid(n: int) -> FloatArray:
     h = np.ones(n)
     h[0] = 0.5
     return h
 
 
 def simpson(n: int) -> FloatArray:
@@ -40,82 +59,88 @@
 
 def default_bounds() -> Bounds:
     return Bounds(-np.inf, np.inf)
 
 
 def lower_bound(b: Any, value: float) -> float:
     try:
-        return max(b[0], value)
+        v = float(b[0])
+        return value if np.isinf(v) else v
     except TypeError:
         return value
 
 
 def upper_bound(b: Any, value: float) -> float:
     try:
-        return min(b[0], value)
+        v = float(b[0])
+        return value if np.isinf(v) else v
     except TypeError:
         return value
 
 
+@dataclass
 class Transform:
-    """Transforms for option pricing"""
+    """Transform for inverting frequency-domain functions"""
+
+    frequency_domain: FloatArray
+    domain_range: Bounds
+    h: FloatArray
 
-    def __init__(
-        self,
-        n: int | None = None,
-        max_frequency: float | None = None,
+    @classmethod
+    def create(
+        cls,
+        n: int,
+        frequency_range: Bounds | None = None,
         domain_range: Bounds | None = None,
         simpson_rule: bool = False,
-    ) -> None:
-        n = n or 128
-        max_frequency = max_frequency or 20.0
-        self.delta_f = max_frequency / n
-        self.frequency_domain = self.delta_f * grid(n)
-        self.domain_range = domain_range or default_bounds()
-        self.h = simpson(n) if simpson_rule else trapezoid(n)
+    ) -> Transform:
+        return cls(
+            frequency_domain=grid_from_bounds(frequency_range or Bounds(0, 20), n),
+            domain_range=domain_range or default_bounds(),
+            h=simpson(n) if simpson_rule else trapezoid(n),
+        )
 
     @property
     def n(self) -> int:
         """Number of discretization points in the frequency and space domain"""
         return self.frequency_domain.shape[0]
 
     @property
+    def delta_f(self) -> float:
+        """Return the frequency discretization step"""
+        return self.frequency_domain[1] - self.frequency_domain[0]
+
+    @property
     def fft_zeta(self) -> float:
+        """Return the zeta parameter for the FFT"""
         return 2 * np.pi / self.n
 
     @property
     def fft_delta_x(self) -> float:
         return self.fft_zeta / self.delta_f
 
     def space_domain(self, delta_x: float) -> FloatArray:
         """Return the space domain discretization points"""
         b0 = lower_bound(self.domain_range.lb, -0.5 * delta_x * self.n)
         b1 = upper_bound(self.domain_range.ub, delta_x * self.n + b0)
         if not np.isclose((b1 - b0) / self.n, delta_x):
             raise TransformError("Incompatible delta_x with domain bounds")
         return delta_x * grid(self.n) + b0
 
-    def delta_x_from_bounds(self) -> float | None:
-        """Return the delta_x from the domain bounds"""
-        b0 = lower_bound(self.domain_range.lb, -np.inf)
-        b1 = upper_bound(self.domain_range.ub, np.inf)
-        if np.isinf(b0) or np.isinf(b1):
-            return None
-        return (b1 - b0) / self.n
-
-    def __call__(self, y: np.ndarray, delta_x: float | None = None) -> TransformResult:
-        return self.fft(y) if delta_x is None else self.frft(y, delta_x)
+    def __call__(self, y: np.ndarray, use_fft: bool = False) -> TransformResult:
+        return self.fft(y) if use_fft else self.frft(y)
 
     def fft(self, y: np.ndarray) -> TransformResult:
         """Transform using the Fast Fourier Transform"""
         x, f = self.transform(y, self.fft_delta_x)
         return TransformResult(x=x, y=np.fft.fft(f).real / self.n)
 
-    def frft(self, y: np.ndarray, delta_x: float) -> TransformResult:
+    def frft(self, y: np.ndarray) -> TransformResult:
         """Transform using the Fractional Fourier Transform"""
+        delta_x = delta_from_bounds(self.domain_range, self.n)
         x, f = self.transform(y, delta_x)
         r = FrFT.calculate(f, delta_x * self.delta_f)
         return TransformResult(x=x, y=r.result.real)
 
     def transform(self, y: np.ndarray, delta_x: float) -> TransformResult:
         if y.shape != self.frequency_domain.shape:
             raise TransformError("shapes not compatible")
@@ -127,14 +152,34 @@
             * np.exp(1j * self.frequency_domain * b)
             * y
             * self.delta_f
             / np.pi
         )
         return TransformResult(x=x, y=t)
 
+    def characteristic_df(self, psi: np.ndarray) -> pd.DataFrame:
+        return pd.concat(
+            (
+                pd.DataFrame(
+                    dict(
+                        frequency=self.frequency_domain,
+                        characteristic=psi.real,
+                        name="real",
+                    )
+                ),
+                pd.DataFrame(
+                    dict(
+                        frequency=self.frequency_domain,
+                        characteristic=psi.imag,
+                        name="iamg",
+                    )
+                ),
+            )
+        )
+
 
 @dataclass
 class FrFT:
     """Fractional Fourier Transfrom"""
 
     result: np.ndarray
     zeta: float
@@ -145,18 +190,14 @@
     fft_z: np.ndarray
     y_z: np.ndarray
 
     @property
     def n(self) -> int:
         return self.result.shape[0]
 
-    @property
-    def fft_zeta(self) -> float:
-        return 2 * np.pi / self.n
-
     @classmethod
     def calculate(cls, x: np.ndarray, zeta: float) -> FrFT:
         n = x.shape[0]
         g = grid(n)
         ez = coef(g, zeta)
         # ez2 = np.flip(ez)
         ez2 = coef(n - g, zeta)
```

### Comparing `quantflow-0.2.2/quantflow/utils/types.py` & `quantflow-0.2.3/quantflow/utils/types.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/quantflow/utils/volatility.py` & `quantflow-0.2.3/quantflow/utils/volatility.py`

 * *Files identical despite different names*

### Comparing `quantflow-0.2.2/readme.md` & `quantflow-0.2.3/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,84 @@
-00000000: 2320 5175 616e 7466 6c6f 770a 0a5b 215b  # Quantflow..[![
-00000010: 5079 5049 2076 6572 7369 6f6e 5d28 6874  PyPI version](ht
-00000020: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000030: 2e69 6f2f 7079 2f71 7561 6e74 666c 6f77  .io/py/quantflow
-00000040: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
-00000050: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
-00000060: 7175 616e 7466 6c6f 7729 0a5b 215b 5079  quantflow).[![Py
-00000070: 7468 6f6e 2076 6572 7369 6f6e 735d 2868  thon versions](h
-00000080: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000090: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-000000a0: 7369 6f6e 732f 7175 616e 7466 6c6f 772e  sions/quantflow.
-000000b0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-000000c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f71  pi.org/project/q
-000000d0: 7561 6e74 666c 6f77 290a 5b21 5b62 7569  uantflow).[![bui
-000000e0: 6c64 5d28 6874 7470 733a 2f2f 6769 7468  ld](https://gith
-000000f0: 7562 2e63 6f6d 2f71 7561 6e74 6d69 6e64  ub.com/quantmind
-00000100: 2f71 7561 6e74 666c 6f77 2f61 6374 696f  /quantflow/actio
-00000110: 6e73 2f77 6f72 6b66 6c6f 7773 2f62 7569  ns/workflows/bui
-00000120: 6c64 2e79 6d6c 2f62 6164 6765 2e73 7667  ld.yml/badge.svg
-00000130: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000140: 622e 636f 6d2f 7175 616e 746d 696e 642f  b.com/quantmind/
-00000150: 7175 616e 7466 6c6f 772f 6163 7469 6f6e  quantflow/action
-00000160: 732f 776f 726b 666c 6f77 732f 6275 696c  s/workflows/buil
-00000170: 642e 796d 6c29 0a5b 215b 636f 6465 636f  d.yml).[![codeco
-00000180: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
-00000190: 6f76 2e69 6f2f 6768 2f71 7561 6e74 6d69  ov.io/gh/quantmi
-000001a0: 6e64 2f71 7561 6e74 666c 6f77 2f62 7261  nd/quantflow/bra
-000001b0: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
-000001c0: 6164 6765 2e73 7667 3f74 6f6b 656e 3d77  adge.svg?token=w
-000001d0: 6b48 396c 594b 4f57 5029 5d28 6874 7470  kH9lYKOWP)](http
-000001e0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-000001f0: 682f 7175 616e 746d 696e 642f 7175 616e  h/quantmind/quan
-00000200: 7466 6c6f 7729 0a0a 5175 616e 7469 7461  tflow)..Quantita
-00000210: 7469 7665 2061 6e61 6c79 7369 7320 616e  tive analysis an
-00000220: 6420 7072 6963 696e 6720 746f 6f6c 732e  d pricing tools.
-00000230: 0a0a 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
-00000240: 6973 2061 7661 696c 6162 6c65 2061 7320  is available as 
-00000250: 5b71 7561 6e74 666c 6f77 206a 7570 7974  [quantflow jupyt
-00000260: 6572 2062 6f6f 6b5d 2868 7474 703a 2f2f  er book](http://
-00000270: 7175 616e 746d 696e 642e 6769 7468 7562  quantmind.github
-00000280: 2e69 6f2f 7175 616e 7466 6c6f 772f 292e  .io/quantflow/).
-00000290: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000002a0: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
-000002b0: 6e73 7461 6c6c 2071 7561 6e74 666c 6f77  nstall quantflow
-000002c0: 0a60 6060 0a0a 215b 6274 6376 6f6c 5d28  .```..![btcvol](
-000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000002e0: 6f6d 2f71 7561 6e74 6d69 6e64 2f71 7561  om/quantmind/qua
-000002f0: 6e74 666c 6f77 2f61 7373 6574 732f 3134  ntflow/assets/14
-00000300: 3433 3230 2f38 3865 6438 3564 312d 6333  4320/88ed85d1-c3
-00000310: 6335 2d34 3839 632d 6163 3037 2d32 3162  c5-489c-ac07-21b
-00000320: 3033 3635 3933 3231 3429 0a0a 0a23 2320  036593214)...## 
-00000330: 4d6f 6475 6c65 730a 0a2a 205b 7175 616e  Modules..* [quan
-00000340: 7466 6c6f 772e 6461 7461 5d28 6874 7470  tflow.data](http
-00000350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f71  s://github.com/q
-00000360: 7561 6e74 6d69 6e64 2f71 7561 6e74 666c  uantmind/quantfl
-00000370: 6f77 2f74 7265 652f 6d61 696e 2f71 7561  ow/tree/main/qua
-00000380: 6e74 666c 6f77 2f64 6174 6129 2064 6174  ntflow/data) dat
-00000390: 6120 4150 4973 2028 7265 7175 6972 6573  a APIs (requires
-000003a0: 2060 7175 616e 7466 6c6f 775b 6461 7461   `quantflow[data
-000003b0: 5d60 290a 2a20 5b71 7561 6e74 666c 6f77  ]`).* [quantflow
-000003c0: 2e6f 7074 696f 6e73 5d28 6874 7470 733a  .options](https:
-000003d0: 2f2f 6769 7468 7562 2e63 6f6d 2f71 7561  //github.com/qua
-000003e0: 6e74 6d69 6e64 2f71 7561 6e74 666c 6f77  ntmind/quantflow
-000003f0: 2f74 7265 652f 6d61 696e 2f71 7561 6e74  /tree/main/quant
-00000400: 666c 6f77 2f6f 7074 696f 6e73 2920 6f70  flow/options) op
-00000410: 7469 6f6e 2070 7269 6369 6e67 2061 6e64  tion pricing and
-00000420: 2063 616c 6962 7261 7469 6f6e 0a2a 205b   calibration.* [
-00000430: 7175 616e 7466 6c6f 772e 7370 5d28 6874  quantflow.sp](ht
-00000440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000450: 2f71 7561 6e74 6d69 6e64 2f71 7561 6e74  /quantmind/quant
-00000460: 666c 6f77 2f74 7265 652f 6d61 696e 2f71  flow/tree/main/q
-00000470: 7561 6e74 666c 6f77 2f73 7029 2073 746f  uantflow/sp) sto
-00000480: 6368 6173 7469 6320 7072 6f63 6573 7320  chastic process 
-00000490: 7072 696d 6974 6976 6573 0a              primitives.
+00000000: 2320 3c61 2068 7265 663d 2268 7474 7073  # <a href="https
+00000010: 3a2f 2f71 7561 6e74 6d69 6e64 2e67 6974  ://quantmind.git
+00000020: 6875 622e 696f 2f71 7561 6e74 666c 6f77  hub.io/quantflow
+00000030: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000040: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000050: 6572 636f 6e74 656e 742e 636f 6d2f 7175  ercontent.com/qu
+00000060: 616e 746d 696e 642f 7175 616e 7466 6c6f  antmind/quantflo
+00000070: 772f 6d61 696e 2f6e 6f74 6562 6f6f 6b73  w/main/notebooks
+00000080: 2f61 7373 6574 732f 7175 616e 7466 6c6f  /assets/quantflo
+00000090: 772d 6c69 6768 742e 7376 6722 2077 6964  w-light.svg" wid
+000000a0: 7468 3d33 3030 202f 3e3c 2f61 3e0a 0a5b  th=300 /></a>..[
+000000b0: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
+000000c0: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+000000d0: 7279 2e69 6f2f 7079 2f71 7561 6e74 666c  ry.io/py/quantfl
+000000e0: 6f77 2e73 7667 295d 2868 7474 7073 3a2f  ow.svg)](https:/
+000000f0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
+00000100: 792f 7175 616e 7466 6c6f 7729 0a5b 215b  y/quantflow).[![
+00000110: 5079 7468 6f6e 2076 6572 7369 6f6e 735d  Python versions]
+00000120: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000130: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00000140: 6572 7369 6f6e 732f 7175 616e 7466 6c6f  ersions/quantflo
+00000150: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
+00000160: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000170: 2f71 7561 6e74 666c 6f77 290a 5b21 5b62  /quantflow).[![b
+00000180: 7569 6c64 5d28 6874 7470 733a 2f2f 6769  uild](https://gi
+00000190: 7468 7562 2e63 6f6d 2f71 7561 6e74 6d69  thub.com/quantmi
+000001a0: 6e64 2f71 7561 6e74 666c 6f77 2f61 6374  nd/quantflow/act
+000001b0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+000001c0: 7569 6c64 2e79 6d6c 2f62 6164 6765 2e73  uild.yml/badge.s
+000001d0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+000001e0: 6875 622e 636f 6d2f 7175 616e 746d 696e  hub.com/quantmin
+000001f0: 642f 7175 616e 7466 6c6f 772f 6163 7469  d/quantflow/acti
+00000200: 6f6e 732f 776f 726b 666c 6f77 732f 6275  ons/workflows/bu
+00000210: 696c 642e 796d 6c29 0a5b 215b 636f 6465  ild.yml).[![code
+00000220: 636f 765d 2868 7474 7073 3a2f 2f63 6f64  cov](https://cod
+00000230: 6563 6f76 2e69 6f2f 6768 2f71 7561 6e74  ecov.io/gh/quant
+00000240: 6d69 6e64 2f71 7561 6e74 666c 6f77 2f62  mind/quantflow/b
+00000250: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+00000260: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000270: 3d77 6b48 396c 594b 4f57 5029 5d28 6874  =wkH9lYKOWP)](ht
+00000280: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000290: 2f67 682f 7175 616e 746d 696e 642f 7175  /gh/quantmind/qu
+000002a0: 616e 7466 6c6f 7729 0a0a 5175 616e 7469  antflow)..Quanti
+000002b0: 7461 7469 7665 2061 6e61 6c79 7369 7320  tative analysis 
+000002c0: 616e 6420 7072 6963 696e 6720 746f 6f6c  and pricing tool
+000002d0: 732e 0a0a 446f 6375 6d65 6e74 6174 696f  s...Documentatio
+000002e0: 6e20 6973 2061 7661 696c 6162 6c65 2061  n is available a
+000002f0: 7320 5b71 7561 6e74 666c 6f77 206a 7570  s [quantflow jup
+00000300: 7974 6572 2062 6f6f 6b5d 2868 7474 7073  yter book](https
+00000310: 3a2f 2f71 7561 6e74 6d69 6e64 2e67 6974  ://quantmind.git
+00000320: 6875 622e 696f 2f71 7561 6e74 666c 6f77  hub.io/quantflow
+00000330: 2f29 2e0a 0a23 2320 496e 7374 616c 6c61  /)...## Installa
+00000340: 7469 6f6e 0a0a 6060 6062 6173 680a 7069  tion..```bash.pi
+00000350: 7020 696e 7374 616c 6c20 7175 616e 7466  p install quantf
+00000360: 6c6f 770a 6060 600a 0a21 5b62 7463 766f  low.```..![btcvo
+00000370: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+00000380: 622e 636f 6d2f 7175 616e 746d 696e 642f  b.com/quantmind/
+00000390: 7175 616e 7466 6c6f 772f 6173 7365 7473  quantflow/assets
+000003a0: 2f31 3434 3332 302f 3838 6564 3835 6431  /144320/88ed85d1
+000003b0: 2d63 3363 352d 3438 3963 2d61 6330 372d  -c3c5-489c-ac07-
+000003c0: 3231 6230 3336 3539 3332 3134 290a 0a0a  21b036593214)...
+000003d0: 2323 204d 6f64 756c 6573 0a0a 2a20 5b71  ## Modules..* [q
+000003e0: 7561 6e74 666c 6f77 2e64 6174 615d 2868  uantflow.data](h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 7175 616e 746d 696e 642f 7175 616e  m/quantmind/quan
+00000410: 7466 6c6f 772f 7472 6565 2f6d 6169 6e2f  tflow/tree/main/
+00000420: 7175 616e 7466 6c6f 772f 6461 7461 2920  quantflow/data) 
+00000430: 6461 7461 2041 5049 7320 2872 6571 7569  data APIs (requi
+00000440: 7265 7320 6071 7561 6e74 666c 6f77 5b64  res `quantflow[d
+00000450: 6174 615d 6029 0a2a 205b 7175 616e 7466  ata]`).* [quantf
+00000460: 6c6f 772e 6f70 7469 6f6e 735d 2868 7474  low.options](htt
+00000470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000480: 7175 616e 746d 696e 642f 7175 616e 7466  quantmind/quantf
+00000490: 6c6f 772f 7472 6565 2f6d 6169 6e2f 7175  low/tree/main/qu
+000004a0: 616e 7466 6c6f 772f 6f70 7469 6f6e 7329  antflow/options)
+000004b0: 206f 7074 696f 6e20 7072 6963 696e 6720   option pricing 
+000004c0: 616e 6420 6361 6c69 6272 6174 696f 6e0a  and calibration.
+000004d0: 2a20 5b71 7561 6e74 666c 6f77 2e73 705d  * [quantflow.sp]
+000004e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000004f0: 636f 6d2f 7175 616e 746d 696e 642f 7175  com/quantmind/qu
+00000500: 616e 7466 6c6f 772f 7472 6565 2f6d 6169  antflow/tree/mai
+00000510: 6e2f 7175 616e 7466 6c6f 772f 7370 2920  n/quantflow/sp) 
+00000520: 7374 6f63 6861 7374 6963 2070 726f 6365  stochastic proce
+00000530: 7373 2070 7269 6d69 7469 7665 730a       ss primitives.
```

### Comparing `quantflow-0.2.2/PKG-INFO` & `quantflow-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7175 616e  : 2.1.Name: quan
 00000020: 7466 6c6f 770a 5665 7273 696f 6e3a 2030  tflow.Version: 0
-00000030: 2e32 2e32 0a53 756d 6d61 7279 3a20 7175  .2.2.Summary: qu
+00000030: 2e32 2e33 0a53 756d 6d61 7279 3a20 7175  .2.3.Summary: qu
 00000040: 616e 7469 7461 7469 7665 2061 6e61 6c79  antitative analy
 00000050: 7369 730a 4c69 6365 6e73 653a 2042 5344  sis.License: BSD
 00000060: 2d33 2d43 6c61 7573 650a 4175 7468 6f72  -3-Clause.Author
 00000070: 3a20 4c75 6361 0a41 7574 686f 722d 656d  : Luca.Author-em
 00000080: 6169 6c3a 206c 7563 6140 7175 616e 746d  ail: luca@quantm
 00000090: 696e 642e 636f 6d0a 5265 7175 6972 6573  ind.com.Requires
 000000a0: 2d50 7974 686f 6e3a 203e 3d33 2e31 302c  -Python: >=3.10,
@@ -47,82 +47,92 @@
 000002e0: 6e64 2f71 7561 6e74 666c 6f77 0a50 726f  nd/quantflow.Pro
 000002f0: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
 00000300: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
 00000310: 7468 7562 2e63 6f6d 2f71 7561 6e74 6d69  thub.com/quantmi
 00000320: 6e64 2f71 7561 6e74 666c 6f77 0a44 6573  nd/quantflow.Des
 00000330: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 00000340: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000350: 646f 776e 0a0a 2320 5175 616e 7466 6c6f  down..# Quantflo
-00000360: 770a 0a5b 215b 5079 5049 2076 6572 7369  w..[![PyPI versi
-00000370: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-00000380: 652e 6675 7279 2e69 6f2f 7079 2f71 7561  e.fury.io/py/qua
-00000390: 6e74 666c 6f77 2e73 7667 295d 2868 7474  ntflow.svg)](htt
-000003a0: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-000003b0: 696f 2f70 792f 7175 616e 7466 6c6f 7729  io/py/quantflow)
-000003c0: 0a5b 215b 5079 7468 6f6e 2076 6572 7369  .[![Python versi
-000003d0: 6f6e 735d 2868 7474 7073 3a2f 2f69 6d67  ons](https://img
-000003e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000003f0: 2f70 7976 6572 7369 6f6e 732f 7175 616e  /pyversions/quan
-00000400: 7466 6c6f 772e 7376 6729 5d28 6874 7470  tflow.svg)](http
-00000410: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000420: 6a65 6374 2f71 7561 6e74 666c 6f77 290a  ject/quantflow).
-00000430: 5b21 5b62 7569 6c64 5d28 6874 7470 733a  [![build](https:
-00000440: 2f2f 6769 7468 7562 2e63 6f6d 2f71 7561  //github.com/qua
-00000450: 6e74 6d69 6e64 2f71 7561 6e74 666c 6f77  ntmind/quantflow
-00000460: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000470: 7773 2f62 7569 6c64 2e79 6d6c 2f62 6164  ws/build.yml/bad
-00000480: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
-00000490: 2f67 6974 6875 622e 636f 6d2f 7175 616e  /github.com/quan
-000004a0: 746d 696e 642f 7175 616e 7466 6c6f 772f  tmind/quantflow/
-000004b0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000004c0: 732f 6275 696c 642e 796d 6c29 0a5b 215b  s/build.yml).[![
-000004d0: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
-000004e0: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f71  /codecov.io/gh/q
+00000350: 646f 776e 0a0a 2320 3c61 2068 7265 663d  down..# <a href=
+00000360: 2268 7474 7073 3a2f 2f71 7561 6e74 6d69  "https://quantmi
+00000370: 6e64 2e67 6974 6875 622e 696f 2f71 7561  nd.github.io/qua
+00000380: 6e74 666c 6f77 223e 3c69 6d67 2073 7263  ntflow"><img src
+00000390: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+000003a0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000003b0: 636f 6d2f 7175 616e 746d 696e 642f 7175  com/quantmind/qu
+000003c0: 616e 7466 6c6f 772f 6d61 696e 2f6e 6f74  antflow/main/not
+000003d0: 6562 6f6f 6b73 2f61 7373 6574 732f 7175  ebooks/assets/qu
+000003e0: 616e 7466 6c6f 772d 6c69 6768 742e 7376  antflow-light.sv
+000003f0: 6722 2077 6964 7468 3d33 3030 202f 3e3c  g" width=300 /><
+00000400: 2f61 3e0a 0a5b 215b 5079 5049 2076 6572  /a>..[![PyPI ver
+00000410: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
+00000420: 6467 652e 6675 7279 2e69 6f2f 7079 2f71  dge.fury.io/py/q
+00000430: 7561 6e74 666c 6f77 2e73 7667 295d 2868  uantflow.svg)](h
+00000440: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+00000450: 792e 696f 2f70 792f 7175 616e 7466 6c6f  y.io/py/quantflo
+00000460: 7729 0a5b 215b 5079 7468 6f6e 2076 6572  w).[![Python ver
+00000470: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
+00000480: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000490: 7069 2f70 7976 6572 7369 6f6e 732f 7175  pi/pyversions/qu
+000004a0: 616e 7466 6c6f 772e 7376 6729 5d28 6874  antflow.svg)](ht
+000004b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000004c0: 726f 6a65 6374 2f71 7561 6e74 666c 6f77  roject/quantflow
+000004d0: 290a 5b21 5b62 7569 6c64 5d28 6874 7470  ).[![build](http
+000004e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f71  s://github.com/q
 000004f0: 7561 6e74 6d69 6e64 2f71 7561 6e74 666c  uantmind/quantfl
-00000500: 6f77 2f62 7261 6e63 682f 6d61 696e 2f67  ow/branch/main/g
-00000510: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
-00000520: 6f6b 656e 3d77 6b48 396c 594b 4f57 5029  oken=wkH9lYKOWP)
-00000530: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-00000540: 762e 696f 2f67 682f 7175 616e 746d 696e  v.io/gh/quantmin
-00000550: 642f 7175 616e 7466 6c6f 7729 0a0a 5175  d/quantflow)..Qu
-00000560: 616e 7469 7461 7469 7665 2061 6e61 6c79  antitative analy
-00000570: 7369 7320 616e 6420 7072 6963 696e 6720  sis and pricing 
-00000580: 746f 6f6c 732e 0a0a 446f 6375 6d65 6e74  tools...Document
-00000590: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-000005a0: 6c65 2061 7320 5b71 7561 6e74 666c 6f77  le as [quantflow
-000005b0: 206a 7570 7974 6572 2062 6f6f 6b5d 2868   jupyter book](h
-000005c0: 7474 703a 2f2f 7175 616e 746d 696e 642e  ttp://quantmind.
-000005d0: 6769 7468 7562 2e69 6f2f 7175 616e 7466  github.io/quantf
-000005e0: 6c6f 772f 292e 0a0a 2323 2049 6e73 7461  low/)...## Insta
-000005f0: 6c6c 6174 696f 6e0a 0a60 6060 6261 7368  llation..```bash
-00000600: 0a70 6970 2069 6e73 7461 6c6c 2071 7561  .pip install qua
-00000610: 6e74 666c 6f77 0a60 6060 0a0a 215b 6274  ntflow.```..![bt
-00000620: 6376 6f6c 5d28 6874 7470 733a 2f2f 6769  cvol](https://gi
-00000630: 7468 7562 2e63 6f6d 2f71 7561 6e74 6d69  thub.com/quantmi
-00000640: 6e64 2f71 7561 6e74 666c 6f77 2f61 7373  nd/quantflow/ass
-00000650: 6574 732f 3134 3433 3230 2f38 3865 6438  ets/144320/88ed8
-00000660: 3564 312d 6333 6335 2d34 3839 632d 6163  5d1-c3c5-489c-ac
-00000670: 3037 2d32 3162 3033 3635 3933 3231 3429  07-21b036593214)
-00000680: 0a0a 0a23 2320 4d6f 6475 6c65 730a 0a2a  ...## Modules..*
-00000690: 205b 7175 616e 7466 6c6f 772e 6461 7461   [quantflow.data
-000006a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000006b0: 2e63 6f6d 2f71 7561 6e74 6d69 6e64 2f71  .com/quantmind/q
-000006c0: 7561 6e74 666c 6f77 2f74 7265 652f 6d61  uantflow/tree/ma
-000006d0: 696e 2f71 7561 6e74 666c 6f77 2f64 6174  in/quantflow/dat
-000006e0: 6129 2064 6174 6120 4150 4973 2028 7265  a) data APIs (re
-000006f0: 7175 6972 6573 2060 7175 616e 7466 6c6f  quires `quantflo
-00000700: 775b 6461 7461 5d60 290a 2a20 5b71 7561  w[data]`).* [qua
-00000710: 6e74 666c 6f77 2e6f 7074 696f 6e73 5d28  ntflow.options](
-00000720: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000730: 6f6d 2f71 7561 6e74 6d69 6e64 2f71 7561  om/quantmind/qua
-00000740: 6e74 666c 6f77 2f74 7265 652f 6d61 696e  ntflow/tree/main
-00000750: 2f71 7561 6e74 666c 6f77 2f6f 7074 696f  /quantflow/optio
-00000760: 6e73 2920 6f70 7469 6f6e 2070 7269 6369  ns) option prici
-00000770: 6e67 2061 6e64 2063 616c 6962 7261 7469  ng and calibrati
-00000780: 6f6e 0a2a 205b 7175 616e 7466 6c6f 772e  on.* [quantflow.
-00000790: 7370 5d28 6874 7470 733a 2f2f 6769 7468  sp](https://gith
-000007a0: 7562 2e63 6f6d 2f71 7561 6e74 6d69 6e64  ub.com/quantmind
-000007b0: 2f71 7561 6e74 666c 6f77 2f74 7265 652f  /quantflow/tree/
-000007c0: 6d61 696e 2f71 7561 6e74 666c 6f77 2f73  main/quantflow/s
-000007d0: 7029 2073 746f 6368 6173 7469 6320 7072  p) stochastic pr
-000007e0: 6f63 6573 7320 7072 696d 6974 6976 6573  ocess primitives
-000007f0: 0a0a                                     ..
+00000500: 6f77 2f61 6374 696f 6e73 2f77 6f72 6b66  ow/actions/workf
+00000510: 6c6f 7773 2f62 7569 6c64 2e79 6d6c 2f62  lows/build.yml/b
+00000520: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00000530: 3a2f 2f67 6974 6875 622e 636f 6d2f 7175  ://github.com/qu
+00000540: 616e 746d 696e 642f 7175 616e 7466 6c6f  antmind/quantflo
+00000550: 772f 6163 7469 6f6e 732f 776f 726b 666c  w/actions/workfl
+00000560: 6f77 732f 6275 696c 642e 796d 6c29 0a5b  ows/build.yml).[
+00000570: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00000580: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000590: 2f71 7561 6e74 6d69 6e64 2f71 7561 6e74  /quantmind/quant
+000005a0: 666c 6f77 2f62 7261 6e63 682f 6d61 696e  flow/branch/main
+000005b0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+000005c0: 3f74 6f6b 656e 3d77 6b48 396c 594b 4f57  ?token=wkH9lYKOW
+000005d0: 5029 5d28 6874 7470 733a 2f2f 636f 6465  P)](https://code
+000005e0: 636f 762e 696f 2f67 682f 7175 616e 746d  cov.io/gh/quantm
+000005f0: 696e 642f 7175 616e 7466 6c6f 7729 0a0a  ind/quantflow)..
+00000600: 5175 616e 7469 7461 7469 7665 2061 6e61  Quantitative ana
+00000610: 6c79 7369 7320 616e 6420 7072 6963 696e  lysis and pricin
+00000620: 6720 746f 6f6c 732e 0a0a 446f 6375 6d65  g tools...Docume
+00000630: 6e74 6174 696f 6e20 6973 2061 7661 696c  ntation is avail
+00000640: 6162 6c65 2061 7320 5b71 7561 6e74 666c  able as [quantfl
+00000650: 6f77 206a 7570 7974 6572 2062 6f6f 6b5d  ow jupyter book]
+00000660: 2868 7474 7073 3a2f 2f71 7561 6e74 6d69  (https://quantmi
+00000670: 6e64 2e67 6974 6875 622e 696f 2f71 7561  nd.github.io/qua
+00000680: 6e74 666c 6f77 2f29 2e0a 0a23 2320 496e  ntflow/)...## In
+00000690: 7374 616c 6c61 7469 6f6e 0a0a 6060 6062  stallation..```b
+000006a0: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+000006b0: 7175 616e 7466 6c6f 770a 6060 600a 0a21  quantflow.```..!
+000006c0: 5b62 7463 766f 6c5d 2868 7474 7073 3a2f  [btcvol](https:/
+000006d0: 2f67 6974 6875 622e 636f 6d2f 7175 616e  /github.com/quan
+000006e0: 746d 696e 642f 7175 616e 7466 6c6f 772f  tmind/quantflow/
+000006f0: 6173 7365 7473 2f31 3434 3332 302f 3838  assets/144320/88
+00000700: 6564 3835 6431 2d63 3363 352d 3438 3963  ed85d1-c3c5-489c
+00000710: 2d61 6330 372d 3231 6230 3336 3539 3332  -ac07-21b0365932
+00000720: 3134 290a 0a0a 2323 204d 6f64 756c 6573  14)...## Modules
+00000730: 0a0a 2a20 5b71 7561 6e74 666c 6f77 2e64  ..* [quantflow.d
+00000740: 6174 615d 2868 7474 7073 3a2f 2f67 6974  ata](https://git
+00000750: 6875 622e 636f 6d2f 7175 616e 746d 696e  hub.com/quantmin
+00000760: 642f 7175 616e 7466 6c6f 772f 7472 6565  d/quantflow/tree
+00000770: 2f6d 6169 6e2f 7175 616e 7466 6c6f 772f  /main/quantflow/
+00000780: 6461 7461 2920 6461 7461 2041 5049 7320  data) data APIs 
+00000790: 2872 6571 7569 7265 7320 6071 7561 6e74  (requires `quant
+000007a0: 666c 6f77 5b64 6174 615d 6029 0a2a 205b  flow[data]`).* [
+000007b0: 7175 616e 7466 6c6f 772e 6f70 7469 6f6e  quantflow.option
+000007c0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+000007d0: 622e 636f 6d2f 7175 616e 746d 696e 642f  b.com/quantmind/
+000007e0: 7175 616e 7466 6c6f 772f 7472 6565 2f6d  quantflow/tree/m
+000007f0: 6169 6e2f 7175 616e 7466 6c6f 772f 6f70  ain/quantflow/op
+00000800: 7469 6f6e 7329 206f 7074 696f 6e20 7072  tions) option pr
+00000810: 6963 696e 6720 616e 6420 6361 6c69 6272  icing and calibr
+00000820: 6174 696f 6e0a 2a20 5b71 7561 6e74 666c  ation.* [quantfl
+00000830: 6f77 2e73 705d 2868 7474 7073 3a2f 2f67  ow.sp](https://g
+00000840: 6974 6875 622e 636f 6d2f 7175 616e 746d  ithub.com/quantm
+00000850: 696e 642f 7175 616e 7466 6c6f 772f 7472  ind/quantflow/tr
+00000860: 6565 2f6d 6169 6e2f 7175 616e 7466 6c6f  ee/main/quantflo
+00000870: 772f 7370 2920 7374 6f63 6861 7374 6963  w/sp) stochastic
+00000880: 2070 726f 6365 7373 2070 7269 6d69 7469   process primiti
+00000890: 7665 730a 0a                             ves..
```

