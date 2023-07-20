# Comparing `tmp/conjugate_models-0.1.1.tar.gz` & `tmp/conjugate_models-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjugate_models-0.1.1.tar", max compression
+gzip compressed data, was "conjugate_models-0.1.2.tar", max compression
```

## Comparing `conjugate_models-0.1.1.tar` & `conjugate_models-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-06-23 11:07:04.395485 conjugate_models-0.1.1/LICENSE
--rw-r--r--   0        0        0     1283 2023-07-09 14:15:32.199934 conjugate_models-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 11:08:52.007050 conjugate_models-0.1.1/conjugate/__init__.py
--rw-r--r--   0        0        0      602 2023-06-28 20:24:26.365975 conjugate_models-0.1.1/conjugate/_typing.py
--rw-r--r--   0        0        0     7185 2023-07-09 14:14:21.892133 conjugate_models-0.1.1/conjugate/distributions.py
--rw-r--r--   0        0        0     5252 2023-07-09 12:16:12.574649 conjugate_models-0.1.1/conjugate/models.py
--rw-r--r--   0        0        0     5586 2023-07-09 12:54:38.337368 conjugate_models-0.1.1/conjugate/plot.py
--rw-r--r--   0        0        0        0 2023-06-23 11:08:47.618556 conjugate_models-0.1.1/conjugate/py.typed
--rw-r--r--   0        0        0      427 2023-06-30 05:20:32.103345 conjugate_models-0.1.1/conjugate/slice.py
--rw-r--r--   0        0        0     1313 2023-07-09 14:12:27.858687 conjugate_models-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 conjugate_models-0.1.1/setup.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 conjugate_models-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-23 11:07:04.395485 conjugate_models-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1283 2023-07-09 14:15:32.199934 conjugate_models-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 11:08:52.007050 conjugate_models-0.1.2/conjugate/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-28 20:24:26.365975 conjugate_models-0.1.2/conjugate/_typing.py
+-rw-r--r--   0        0        0     7113 2023-07-20 12:22:40.859857 conjugate_models-0.1.2/conjugate/distributions.py
+-rw-r--r--   0        0        0     5587 2023-07-20 12:22:40.860011 conjugate_models-0.1.2/conjugate/models.py
+-rw-r--r--   0        0        0     5569 2023-07-20 12:22:40.860147 conjugate_models-0.1.2/conjugate/plot.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:08:47.618556 conjugate_models-0.1.2/conjugate/py.typed
+-rw-r--r--   0        0        0      428 2023-07-20 12:22:40.860263 conjugate_models-0.1.2/conjugate/slice.py
+-rw-r--r--   0        0        0     1313 2023-07-20 12:22:40.860387 conjugate_models-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 conjugate_models-0.1.2/setup.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 conjugate_models-0.1.2/PKG-INFO
```

### Comparing `conjugate_models-0.1.1/LICENSE` & `conjugate_models-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.1/README.md` & `conjugate_models-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.1/conjugate/_typing.py` & `conjugate_models-0.1.2/conjugate/_typing.py`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.1/conjugate/distributions.py` & `conjugate_models-0.1.2/conjugate/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     return alpha, beta
 
 
 @dataclass
 class Beta(ContinuousPlotDistMixin, SliceMixin):
     """Beta distribution.
 
-    Args: 
+    Args:
         alpha: shape parameter
         beta: shape parameter
-    
+
     """
 
     alpha: NUMERIC
     beta: NUMERIC
 
     def __post_init__(self) -> None:
         self.max_value = 1.0
@@ -88,23 +88,24 @@
         return cls(alpha=alpha, beta=beta)
 
     @property
     def dist(self):
         return stats.beta(self.alpha, self.beta)
 
 
-@dataclass 
+@dataclass
 class Binomial(DiscretePlotMixin, SliceMixin):
     """Binomial distribution.
-    
-    Args: 
+
+    Args:
         n: number of trials
         p: probability of success
-    
+
     """
+
     n: NUMERIC
     p: NUMERIC
 
     def __post_init__(self):
         if isinstance(self.n, np.ndarray):
             self.max_value = self.n.max()
         else:
@@ -127,18 +128,19 @@
         return np.stack([self.dist(param).mean() for param in self.params])
 
 
 @dataclass
 class Dirichlet(DirichletPlotDistMixin):
     """Dirichlet distribution.
 
-    Args: 
+    Args:
         alpha: shape parameter
-    
+
     """
+
     alpha: NUMERIC
 
     def __post_init__(self) -> None:
         self.max_value = 1.0
 
     @property
     def dist(self):
@@ -148,34 +150,34 @@
         return VectorizedDist(self.alpha, dist=stats.dirichlet)
 
 
 @dataclass
 class Exponential(ContinuousPlotDistMixin, SliceMixin):
     """Exponential distribution.
 
-    Args: 
+    Args:
         lam: rate parameter
-    
+
     """
 
     lam: NUMERIC
 
     @property
     def dist(self):
         return stats.expon(scale=self.lam)
 
 
 @dataclass
 class Gamma(ContinuousPlotDistMixin, SliceMixin):
     """Gamma distribution.
-    
+
     <a href=https://en.wikipedia.org/wiki/Gamma_distribution>Gamma Distribution</a>
     <a href=https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gamma.html>Scipy Docmentation</a>
 
-    Args: 
+    Args:
         alpha: shape parameter
         beta: rate parameter
     """
 
     alpha: NUMERIC
     beta: NUMERIC
 
@@ -188,20 +190,21 @@
 
     __rmul__ = __mul__
 
 
 @dataclass
 class NegativeBinomial(DiscretePlotMixin, SliceMixin):
     """Negative binomial distribution.
-    
-    Args: 
+
+    Args:
         n: number of successes
         p: probability of success
-    
+
     """
+
     n: NUMERIC
     p: NUMERIC
 
     @property
     def dist(self):
         return stats.nbinom(n=self.n, p=self.p)
 
@@ -215,41 +218,43 @@
 class Poisson(DiscretePlotMixin, SliceMixin):
     """Poisson distribution.
 
     Args:
         lam: rate parameter
 
     """
+
     lam: NUMERIC
 
     @property
     def dist(self):
         return stats.poisson(self.lam)
 
     def __mul__(self, other) -> "Poisson":
         return Poisson(lam=self.lam * other)
 
     __rmul__ = __mul__
 
-    def __add__(self, other) -> "Poisson": 
+    def __add__(self, other) -> "Poisson":
         return Poisson(self.lam + other.lam)
-    
+
     __radd__ = __add__
 
 
 @dataclass
 class BetaBinomial(DiscretePlotMixin, SliceMixin):
     """Beta binomial distribution.
-    
+
     Args:
         n: number of trials
         alpha: shape parameter
         beta: shape parameter
-    
+
     """
+
     n: NUMERIC
     alpha: NUMERIC
     beta: NUMERIC
 
     def __post_init__(self):
         if isinstance(self.n, np.ndarray):
             self.max_value = self.n.max()
@@ -260,76 +265,80 @@
     def dist(self):
         return stats.betabinom(self.n, self.alpha, self.beta)
 
 
 @dataclass
 class BetaNegativeBinomial(SliceMixin):
     """Beta negative binomial distribution.
-    
+
     Args:
         n: number of successes
         alpha: shape parameter
 
-    
+
     """
+
     n: NUMERIC
     alpha: NUMERIC
     beta: NUMERIC
 
 
 @dataclass
 class Geometric(DiscretePlotMixin, SliceMixin):
     """Geometric distribution.
-    
+
     Args:
         p: probability of success
 
     """
+
     p: NUMERIC
 
     @property
     def dist(self):
         return stats.geom(self.p)
 
 
 @dataclass
 class Normal(ContinuousPlotDistMixin, SliceMixin):
     """Normal distribution.
-    
+
     Args:
         mu: mean
         sigma: standard deviation
 
     """
+
     mu: NUMERIC
     sigma: NUMERIC
 
     @property
     def dist(self):
         return stats.norm(self.mu, self.sigma)
-    
+
     def __mul__(self, other):
-        sigma = ((self.sigma ** 2) * other) ** 0.5
+        sigma = ((self.sigma**2) * other) ** 0.5
         return Normal(mu=self.mu * other, sigma=sigma)
-    
+
     __rmul__ = __mul__
 
 
 @dataclass
 class Uniform(ContinuousPlotDistMixin, SliceMixin):
     """Uniform distribution.
-    
+
     Args:
         low: lower bound
         high: upper bound
 
     """
+
     low: NUMERIC
     high: NUMERIC
 
     def __post_init__(self):
         self.min_value = self.low
         self.max_value = self.high
 
     @property
     def dist(self):
-        return stats.uniform(self.low, self.high)
+        return stats.uniform(self.low, self.high)
```

### Comparing `conjugate_models-0.1.1/conjugate/models.py` & `conjugate_models-0.1.2/conjugate/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,67 +22,81 @@
     alpha_post = alpha_prior + x
     beta_post = beta_prior + (n - x)
 
     return alpha_post, beta_post
 
 
 def binomial_beta(n: NUMERIC, x: NUMERIC, beta_prior: Beta) -> Beta:
-    """Posterior distribution for a binomial likelihood with a beta prior. 
+    """Posterior distribution for a binomial likelihood with a beta prior.
 
-    Args: 
-        n: total number of trials 
+    Args:
+        n: total number of trials
         x: sucesses from that trials
         beta_prior: Beta distribution prior
-    
-    Returns: 
+
+    Returns:
         Beta distribution posterior
-    
+
     """
     alpha_post, beta_post = get_binomial_beta_posterior_params(
         beta_prior.alpha, beta_prior.beta, n, x
     )
 
     return Beta(alpha=alpha_post, beta=beta_post)
 
 
 def binomial_beta_posterior_predictive(n: NUMERIC, beta: Beta) -> BetaBinomial:
-    """Posterior predictive distribution for a binomial likelihood with a beta prior. 
-    
-    Args: 
+    """Posterior predictive distribution for a binomial likelihood with a beta prior.
+
+    Args:
         n: number of trials
         beta: Beta distribution
 
-    Returns: 
+    Returns:
         BetaBinomial posterior predictive distribution
 
     """
     return BetaBinomial(n=n, alpha=beta.alpha, beta=beta.beta)
 
 
 def negative_binomial_beta(r, n, x, beta_prior: Beta) -> Beta:
-    """Posterior distribution for a negative binomial likelihood with a beta prior. 
-    
-    Args: 
-        
+    """Posterior distribution for a negative binomial likelihood with a beta prior.
+
+    Args:
+
     """
     alpha_post = beta_prior.alpha + (r * n)
     beta_post = beta_prior.beta + x
 
     return Beta(alpha=alpha_post, beta=beta_post)
 
 
 def negative_binomial_beta_posterior_predictive(r, beta: Beta) -> BetaNegativeBinomial:
     """Posterior predictive distribution for a negative binomial likelihood with a beta prior"""
     return BetaNegativeBinomial(r=r, alpha=beta.alpha, beta=beta.beta)
 
 
-def geometric_beta(x, n, beta_prior: Beta) -> Beta:
-    """Posterior distribution for a geometric likelihood with a beta prior"""
+def geometric_beta(x_total, n, beta_prior: Beta, one_start: bool = True) -> Beta:
+    """Posterior distribution for a geometric likelihood with a beta prior.
+
+    Args:
+        x_total: sum of all trials outcomes
+        n: total number of trials
+        beta_prior: Beta distribution prior
+        one_start: whether to outcomes start at 1, defaults to True. False is 0 start.
+
+    Returns:
+        Beta distribution posterior
+
+    """
     alpha_post = beta_prior.alpha + n
-    beta_post = beta_prior.beta + x
+    beta_post = beta_prior.beta + x_total
+
+    if one_start:
+        beta_post = beta_post - n
 
     return Beta(alpha=alpha_post, beta=beta_post)
 
 
 def get_dirichlet_posterior_params(alpha_prior: NUMERIC, x: NUMERIC) -> NUMERIC:
     try:
         return alpha_prior + x
@@ -98,34 +112,37 @@
 
 def categorical_dirichlet(x: NUMERIC, dirichlet_prior: Dirichlet) -> Dirichlet:
     """Posterior distribution of Categorical model with Dirichlet prior."""
     alpha_post = get_dirichlet_posterior_params(dirichlet_prior.alpha, x)
 
     return Dirichlet(alpha=alpha_post)
 
+
 def get_multi_categorical_dirichlet_posterior_params(
     alpha_prior: NUMERIC, x: NUMERIC
 ) -> NUMERIC:
     return get_dirichlet_posterior_params(alpha_prior, x)
 
+
 def multinomial_dirichlet(x: NUMERIC, dirichlet_prior: Dirichlet) -> Dirichlet:
-    """Posterior distribution of Multinomial model with Dirichlet prior. 
+    """Posterior distribution of Multinomial model with Dirichlet prior.
 
-    Args: 
+    Args:
         x: counts
         dirichlet_prior: Dirichlet prior on the counts
 
-    Returns: 
+    Returns:
         Dirichlet posterior distribution
 
     """
     alpha_post = get_dirichlet_posterior_params(dirichlet_prior.alpha, x)
 
     return Dirichlet(alpha=alpha_post)
 
+
 def get_poisson_gamma_posterior_params(
     alpha: NUMERIC, beta: NUMERIC, x_total: NUMERIC, n: NUMERIC
 ) -> Tuple[NUMERIC, NUMERIC]:
     alpha_post = alpha + x_total
     beta_post = beta + n
 
     return alpha_post, beta_post
@@ -159,14 +176,15 @@
 
     return NegativeBinomial(n=n, p=p)
 
 
 # Just happen to be the same as above
 get_exponential_gamma_posterior_params = get_poisson_gamma_posterior_params
 
+
 def exponetial_gamma(x_total: NUMERIC, n: NUMERIC, gamma_prior: Gamma) -> Gamma:
     """Posterior distribution for an exponential likelihood with a gamma prior"""
     alpha_post, beta_post = get_exponential_gamma_posterior_params(
         alpha=gamma_prior.alpha, beta=gamma_prior.beta, x_total=x_total, n=n
     )
 
-    return Gamma(alpha=alpha_post, beta=beta_post)
+    return Gamma(alpha=alpha_post, beta=beta_post)
```

### Comparing `conjugate_models-0.1.1/conjugate/plot.py` & `conjugate_models-0.1.2/conjugate/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     def rvs(self, size, *args, **kwargs) -> np.ndarray:
         ...
 
 
 LABEL_INPUT = Union[str, Iterable[str], Callable[[int], str]]
 
+
 def resolve_label(label: LABEL_INPUT, yy: np.ndarray):
     """
 
     https://stackoverflow.com/questions/73662931/matplotlib-plot-a-numpy-array-as-many-lines-with-a-single-label
     """
     if yy.ndim == 1:
         return label
@@ -31,25 +32,26 @@
     ncols = yy.shape[1]
     if ncols != 1:
         if isinstance(label, str):
             return [f"{label} {i}" for i in range(1, ncols + 1)]
 
         if callable(label):
             return [label(i) for i in range(1, ncols + 1)]
-            
+
         if isinstance(label, Iterable):
             return label
 
         raise ValueError("Label must be a string, iterable, or callable.")
 
     return label
 
 
 class PlotDistMixin:
     """Base mixin in order to support plotting. Requires the dist attribute of the scipy distribution."""
+
     @property
     def dist(self) -> Distribution:
         raise NotImplementedError("Implement this property in the subclass.")
 
     @property
     def max_value(self) -> float:
         if not hasattr(self, "_max_value"):
@@ -76,39 +78,40 @@
 
     def _settle_axis(self, ax: Optional[plt.Axes] = None) -> plt.Axes:
         return ax if ax is not None else plt.gca()
 
 
 class ContinuousPlotDistMixin(PlotDistMixin):
     """Functionality for plot_pdf method of continuous distributions."""
+
     def plot_pdf(self, ax: Optional[plt.Axes] = None, **kwargs) -> plt.Axes:
         """Plot the pdf of distribution
 
-        Args: 
+        Args:
             ax: matplotlib Axes, optional
             **kwargs: Additonal kwargs to pass to matplotlib
 
-        Returns: 
+        Returns:
             new or modified Axes
-        
+
         """
         ax = self._settle_axis(ax=ax)
 
         x = self._create_x_values()
         x = self._reshape_x_values(x)
 
         return self._create_plot_on_axis(x, ax, **kwargs)
-    
-    @property 
+
+    @property
     def min_value(self) -> float:
         if not hasattr(self, "_min_value"):
             self._min_value = 0.0
 
         return self._min_value
-    
+
     @min_value.setter
     def min_value(self, value: float) -> None:
         self._min_value = value
 
     def set_min_value(self, value: float) -> "ContinuousPlotDistMixin":
         """Set the minimum value for plotting."""
         self.min_value = value
@@ -138,36 +141,38 @@
         self._setup_labels(ax=ax)
         ax.set_ylim(0, None)
         return ax
 
 
 class DirichletPlotDistMixin(ContinuousPlotDistMixin):
     """Plot the pdf using samples from the dirichlet distribution."""
+
     def plot_pdf(
         self, ax: Optional[plt.Axes] = None, samples: int = 1_000, **kwargs
     ) -> plt.Axes:
-        """Plots the pdf """
+        """Plots the pdf"""
         distribution_samples = self.dist.rvs(size=samples)
 
         ax = self._settle_axis(ax=ax)
         xx = self._create_x_values()
 
         for x in distribution_samples.T:
             kde = gaussian_kde(x)
 
             yy = kde(xx)
 
-            ax.plot(xx, yy)
+            ax.plot(xx, yy, **kwargs)
 
         self._setup_labels(ax=ax)
         return ax
 
 
 class DiscretePlotMixin(PlotDistMixin):
     """Adding the plot_pmf method to class."""
+
     def plot_pmf(
         self, ax: Optional[plt.Axes] = None, mark: str = "o-", **kwargs
     ) -> plt.Axes:
         ax = self._settle_axis(ax=ax)
 
         x = self._create_x_values()
         x = self._reshape_x_values(x)
```

### Comparing `conjugate_models-0.1.1/pyproject.toml` & `conjugate_models-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conjugate-models"
-version = "0.1.1"
+version = "0.1.2"
 description = "Bayesian Conjugate Models in Python"
 authors = ["Will Dean <wd60622@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://wd60622.github.io/conjugate/"
 documentation = "https://wd60622.github.io/conjugate/"
 repository = "https://github.com/wd60622/conjugate"
```

### Comparing `conjugate_models-0.1.1/setup.py` & `conjugate_models-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 modules = \
 ['py']
 install_requires = \
 ['matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.3,<2.0.0', 'pandas', 'scipy<1.10.0']
 
 setup_kwargs = {
     'name': 'conjugate-models',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Bayesian Conjugate Models in Python',
     'long_description': '# conjugate priors\nBayesian conjugate models in Python\n\n\n## Installation\n\n```bash \npip install conjugate-models\n```\n\n## Basic Usage\n\n```python \nfrom conjugate.distributions import Beta, BetaBinomial\nfrom conjugate.models import binomial_beta, binomial_beta_posterior_predictive\n\n# Observed Data\nX = 4\nN = 10\n\n# Analytics\nprior = Beta(1, 1)\nprior_predictive: BetaBinomial = binomial_beta_posterior_predictive(n=N, beta=prior)\n\nposterior: Beta = binomial_beta(n=N, x=X, beta_prior=prior)\nposterior_predictive: BetaBinomial = binomial_beta_posterior_predictive(n=N, beta=posterior) \n\n# Figure\nimport matplotlib.pyplot as plt\n\nfig, axes = plt.subplots(ncols=2)\n\nax = axes[0]\nax = posterior.plot_pdf(ax=ax, label="posterior")\nprior.plot_pdf(ax=ax, label="prior")\nax.axvline(x=X/N, color="black", ymax=0.05, label="MLE")\nax.set_title("Success Rate")\nax.legend()\n\nax = axes[1]\nposterior_predictive.plot_pmf(ax=ax, label="posterior predictive")\nprior_predictive.plot_pmf(ax=ax, label="prior predictive")\nax.axvline(x=X, color="black", ymax=0.05, label="Sample")\nax.set_title("Number of Successes")\nax.legend()\nplt.show()\n```\n\n<img height=400 src="docs/images/binomial-beta.png" title="Binomial Beta Comparison">\n\nMore examples on in the [documentation](https://wd60622.github.io/conjugate/).',
     'author': 'Will Dean',
     'author_email': 'wd60622@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://wd60622.github.io/conjugate/',
```

### Comparing `conjugate_models-0.1.1/PKG-INFO` & `conjugate_models-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conjugate-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bayesian Conjugate Models in Python
 Home-page: https://wd60622.github.io/conjugate/
 License: MIT
 Author: Will Dean
 Author-email: wd60622@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

