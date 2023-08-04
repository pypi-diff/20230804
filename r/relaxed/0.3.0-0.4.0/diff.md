# Comparing `tmp/relaxed-0.3.0.tar.gz` & `tmp/relaxed-0.4.0.tar.gz`

## Comparing `relaxed-0.3.0.tar` & `relaxed-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 relaxed-0.3.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relaxed-0.3.0/.gitattributes
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relaxed-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 relaxed-0.3.0/.readthedocs.yml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 relaxed-0.3.0/CITATION.cff
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 relaxed-0.3.0/list_of_operations.md
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 relaxed-0.3.0/noxfile.py
--rw-r--r--   0        0        0    32802 2020-02-02 00:00:00.000000 relaxed-0.3.0/relaxed-logo.png
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 relaxed-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 relaxed-0.3.0/binder/postBuild
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/Makefile
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/conf.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/index.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/make.bat
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/modules.rst
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed-101.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.infer.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.metrics.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.mle.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.3.0/docs/relaxed.ops.rst
--rw-r--r--   0        0        0   268660 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/binning.ipynb
--rw-r--r--   0        0        0   154655 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/cuts.ipynb
--rw-r--r--   0        0        0    50427 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/diffable_histograms.ipynb
--rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/neos.ipynb
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/requirements.txt
--rw-r--r--   0        0        0   198248 2020-02-02 00:00:00.000000 relaxed-0.3.0/examples/simple-analysis-optimisation.ipynb
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/infer.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/metrics.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/mle.py
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/ops.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/py.typed
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/_compat/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 relaxed-0.3.0/src/relaxed/_compat/typing.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/dummy_pyhf.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_fit.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_infer.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_metrics.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_ops.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 relaxed-0.3.0/tests/test_package.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 relaxed-0.3.0/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 relaxed-0.3.0/LICENSE
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 relaxed-0.3.0/README.md
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 relaxed-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7615 2020-02-02 00:00:00.000000 relaxed-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 relaxed-0.4.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relaxed-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relaxed-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 relaxed-0.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 relaxed-0.4.0/CITATION.cff
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 relaxed-0.4.0/list_of_operations.md
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 relaxed-0.4.0/noxfile.py
+-rw-r--r--   0        0        0    32802 2020-02-02 00:00:00.000000 relaxed-0.4.0/relaxed-logo.png
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 relaxed-0.4.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 relaxed-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 relaxed-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 relaxed-0.4.0/binder/postBuild
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/modules.rst
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/relaxed-101.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/relaxed.infer.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/relaxed.metrics.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/relaxed.mle.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 relaxed-0.4.0/docs/relaxed.ops.rst
+-rw-r--r--   0        0        0   268660 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/binning.ipynb
+-rw-r--r--   0        0        0   154655 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/cuts.ipynb
+-rw-r--r--   0        0        0    50427 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/diffable_histograms.ipynb
+-rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/neos.ipynb
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/requirements.txt
+-rw-r--r--   0        0        0   198248 2020-02-02 00:00:00.000000 relaxed-0.4.0/examples/simple-analysis-optimisation.ipynb
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/__init__.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/infer.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/metrics.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/mle.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/ops.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/py.typed
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/_compat/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 relaxed-0.4.0/src/relaxed/_compat/typing.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/dummy_pyhf.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/test_fit.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/test_infer.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/test_ops.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 relaxed-0.4.0/tests/test_package.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 relaxed-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 relaxed-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 relaxed-0.4.0/README.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 relaxed-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 relaxed-0.4.0/PKG-INFO
```

### Comparing `relaxed-0.3.0/.pre-commit-config.yaml` & `relaxed-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/list_of_operations.md` & `relaxed-0.4.0/list_of_operations.md`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/noxfile.py` & `relaxed-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/relaxed-logo.png` & `relaxed-0.4.0/relaxed-logo.png`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/.github/CONTRIBUTING.md` & `relaxed-0.4.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/.github/workflows/ci.yml` & `relaxed-0.4.0/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -37,33 +37,41 @@
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.11"]
-        runs-on: [ubuntu-latest, macos-latest]
+        python-version: ["3.9", "3.11"]
+        runs-on: [ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
 
       - name: Install package
         run: python -m pip install .[test]
 
+      - name: Install jaxopt from source (temp -- my lbfgs fix)
+        run:
+          python -m pip install --upgrade --force-reinstall git+https://github.com/google/jaxopt.git
+
+      - name: Install pyhf from source (temp -- jax devicearray not found fix)
+        run:
+          python -m pip install --upgrade --force-reinstall
+          git+https://github.com/scikit-hep/pyhf.git
+
       - name: Test package
         run: >-
-          python -m pip install --upgrade git+https://github.com/phinate/jaxopt.git@fix-lbfgsb-grad
           pytest -ra --cov --cov-report=xml --cov-report=term --durations=20
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v3.1.4
 
     ## skip these for now until things are stable
     #   - name: Run examples
```

### Comparing `relaxed-0.3.0/docs/Makefile` & `relaxed-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/docs/conf.py` & `relaxed-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/docs/index.rst` & `relaxed-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/docs/make.bat` & `relaxed-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/examples/binning.ipynb` & `relaxed-0.4.0/examples/binning.ipynb`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/examples/cuts.ipynb` & `relaxed-0.4.0/examples/cuts.ipynb`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/examples/diffable_histograms.ipynb` & `relaxed-0.4.0/examples/diffable_histograms.ipynb`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/examples/neos.ipynb` & `relaxed-0.4.0/examples/neos.ipynb`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/examples/simple-analysis-optimisation.ipynb` & `relaxed-0.4.0/examples/simple-analysis-optimisation.ipynb`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/src/relaxed/metrics.py` & `relaxed-0.4.0/src/relaxed/metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 __all__ = ("asimov_sig", "gaussianity")
 
-from functools import partial
 from typing import TYPE_CHECKING, Any, cast
 
+import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
-from jax import Array
+from jax import Array, flatten_util
 from jax.random import multivariate_normal
 
 from relaxed.ops import fisher_info
 
 if TYPE_CHECKING:
     PyTree = Any
+    from jax.typing import ArrayLike
 
 
 @jax.jit
 def asimov_sig(s: Array, b: Array) -> float:
     """Median expected significance for a counting experiment, valid in the asymptotic regime.
     Also valid for the multi-bin case.
 
@@ -39,59 +40,51 @@
 
 
 def _gaussian_logpdf(
     bestfit_pars: Array,
     data: Array,
     cov: Array,
 ) -> Array:
-    return cast(
-        Array, jsp.stats.multivariate_normal.logpdf(data, bestfit_pars, cov)
-    ).reshape(
-        1,
-    )
+    return cast(Array, jsp.stats.multivariate_normal.logpdf(data, bestfit_pars, cov))
 
 
-@partial(
-    jax.jit,
-    static_argnames=[
-        "n_samples",
-    ],
-)
+@eqx.filter_jit
 def gaussianity(
     model: PyTree,
-    bestfit_pars: Array,
+    bestfit_pars: dict[str, ArrayLike],
     data: Array,
     rng_key: Any,
     n_samples: int = 1000,
 ) -> Array:
     # - compare the likelihood of the fitted model with a gaussian approximation
     # that has the same MLE (fitted_pars)
     # - do this across a number of points in parspace (sampled from the gaussian approx)
     # and take the mean squared diff
     # - centre the values wrt the best-fit vals to scale the differences
 
     cov_approx = jnp.linalg.inv(fisher_info(model, bestfit_pars, data))
-
+    flat_bestfit_pars, tree_structure = flatten_util.ravel_pytree(bestfit_pars)
     gaussian_parspace_samples = multivariate_normal(
         key=rng_key,
-        mean=bestfit_pars,
+        mean=flat_bestfit_pars,
         cov=cov_approx,
         shape=(n_samples,),
     )
 
     relative_nlls_model = jax.vmap(
         lambda pars, data: -(
-            model.logpdf(pars, data)[0] - model.logpdf(bestfit_pars, data)[0]
+            model.logpdf(pars=tree_structure(pars), data=data)
+            - model.logpdf(pars=bestfit_pars, data=data)
         ),  # scale origin to bestfit pars
         in_axes=(0, None),
     )(gaussian_parspace_samples, data)
 
     relative_nlls_gaussian = jax.vmap(
         lambda pars, data: -(
-            _gaussian_logpdf(pars, data, cov_approx)[0]
-            - _gaussian_logpdf(bestfit_pars, data, cov_approx)[0]
+            _gaussian_logpdf(pars, data, cov_approx)
+            - _gaussian_logpdf(flat_bestfit_pars, data, cov_approx)
         ),  # data fixes the lhood shape
         in_axes=(0, None),
-    )(gaussian_parspace_samples, bestfit_pars)
+    )(gaussian_parspace_samples, flat_bestfit_pars)
 
     diffs = relative_nlls_model - relative_nlls_gaussian
     return jnp.nanmean(diffs**2, axis=0)
```

### Comparing `relaxed-0.3.0/src/relaxed/ops.py` & `relaxed-0.4.0/src/relaxed/ops.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 __all__ = ("cut", "hist", "fisher_info", "cramer_rao_uncert")
 
 from functools import partial
 from typing import Any
 
+import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
-from jax import Array
+from jax import Array, flatten_util
 
 
 @partial(jax.jit, static_argnames=["keep"])
 def cut(data: Array, cut_val: float, slope: float = 1.0, keep: str = "above") -> Array:
     """Use a sigmoid function as an approximate cut. Same as a hard cut in the limit of infinite slope.
     Note: this function returns weights, not indices.
 
@@ -90,37 +91,47 @@
             + jnp.array([0] * (len(counts) - 3) + [counts[-1]])
         )
 
     return counts
 
 
 @jax.jit
-def fisher_info(model: Any, pars: Array, data: Array) -> Array:
+def fisher_info(model: Any, pars: dict[str, Array], data: Array) -> Array:
     """Fisher information matrix for a model with a logpdf method.
 
     Parameters
     ----------
     model : Any
         The model to compute the Fisher information matrix for.
         Needs to have a logpdf method (that returns list[float] for now).
-    pars : Array
-        The (MLE) parameters of the model.
+    pars : dict[str, Array]
+        The (MLE) parameters of the model, as a dict of arrays/floats.
     data : Array
         The data to compute the Fisher information matrix for.
 
     Returns
     -------
     Array
-        Fisher information matrix.
+        Fisher information matrix of shape (num_pars, num_pars).
+        Order of columns is the same as the order of the parameters in pars.
+        Parameters with multiple dimensions are flattened into their own columns.
     """
-    return jnp.linalg.inv(-jax.hessian(lambda p, d: model.logpdf(p, d)[0])(pars, data))
 
+    flat_pars, tree_structure = flatten_util.ravel_pytree(pars)
 
-@jax.jit
-def cramer_rao_uncert(model: Any, pars: Array, data: Array) -> Array:
+    def lpdf(pars, data):  # handle keyword arguments
+        return model.logpdf(pars=tree_structure(pars), data=data)
+
+    return jnp.linalg.inv(-jax.hessian(lpdf)(flat_pars, data))
+
+
+@eqx.filter_jit
+def cramer_rao_uncert(
+    model: Any, pars: dict[str, Array], data: Array, return_tree=True
+) -> Array:
     """Approximate uncertainties on MLE parameters for a model with a logpdf method.
     Defined as the square root of the diagonal of the Fisher information matrix, valid
     via the Cramer-Rao lower bound.
 
     Parameters
     ----------
     model : Any
@@ -132,8 +143,13 @@
         The data to compute the uncertainty for.
 
     Returns
     -------
     Array
         Cramer-Rao uncertainty on the MLE parameters.
     """
-    return jnp.sqrt(jnp.diag(fisher_info(model, pars, data)))
+    fisher = fisher_info(model, pars, data)
+    uncert = jnp.sqrt(jnp.diag(fisher))
+    if return_tree:
+        _, tree_structure = flatten_util.ravel_pytree(pars)
+        return tree_structure(uncert)
+    return uncert
```

### Comparing `relaxed-0.3.0/src/relaxed/_compat/typing.py` & `relaxed-0.4.0/src/relaxed/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/tests/test_metrics.py` & `relaxed-0.4.0/tests/test_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import jax.numpy as jnp
 import numpy as np
-import pyhf
 import pytest
-from dummy_pyhf import example_model, uncorrelated_background
-from jax import jacrev
+from dummy_pyhf import example_model
+from jax import jacrev, tree_map
 from jax.random import PRNGKey
 
 import relaxed
 
 
 @pytest.fixture()
 def data():
@@ -18,31 +17,31 @@
     bins = np.linspace(0, 70, 10)
     background = np.histogram(np.random.normal(40, 10, nBg), bins=bins)[0]
     signal = np.histogram(np.random.normal(50, 5, nSig), bins=bins)[0]
     return signal, background
 
 
 def test_gaussianity():
-    pyhf.set_backend("jax")
-    m = uncorrelated_background(
-        jnp.array([5.0, 5.0]),
-        jnp.array([10.0, 10.0]),
-        jnp.array([0.1, 0.1]),
-    )
-    pars = jnp.asarray(m.config.suggested_init())
-    data = jnp.asarray(m.expected_data(pars))
-    relaxed.metrics.gaussianity(m, pars, data, PRNGKey(0))
+    model = example_model(5.0, n_bins=2)
+    pars = {"mu": jnp.array(0.0), "shapesys": jnp.array([1.0, 1.0])}
+    data = model.expected_data(pars)
+    relaxed.metrics.gaussianity(model, pars, data, PRNGKey(0))
 
 
 def test_gaussianity_grad():
     def pipeline(x):
-        model = example_model(5.0)
-        pars = model.config.suggested_init()
+        model = example_model(5.0, n_bins=2)
+        pars = {"mu": jnp.array(0.0), "shapesys": jnp.array([1.0, 1.0])}
         data = model.expected_data(pars)
-        return relaxed.metrics.gaussianity(model, pars * x, data * x, PRNGKey(0))
+        return relaxed.metrics.gaussianity(
+            model,
+            tree_map(lambda a: a * x, pars),
+            (data[0] * x, data[1] * x),
+            PRNGKey(0),
+        )
 
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
 def test_significance(data):
     signal, background = data
```

### Comparing `relaxed-0.3.0/tests/test_ops.py` & `relaxed-0.4.0/tests/test_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pyhf
 import pytest
-from dummy_pyhf import example_model, uncorrelated_background
-from jax import jacrev, vmap
+from dummy_pyhf import HEPDataLike, example_model
+from jax import jacrev, tree_map, vmap
 from jax.random import PRNGKey, normal
 
 import relaxed
 
 jax.config.update("jax_enable_x64", True)
 
 
@@ -100,70 +100,92 @@
     assert np.allclose(
         relaxed_grads, grads, atol=0.01, rtol=0.05
     )  # tols are a bit high because the grads are a little noisy/biased
 
 
 def test_fisher_info():
     pyhf.set_backend("jax")
-    model = example_model(5.0)
-    pars = model.config.suggested_init()
+    model = example_model(1.0, n_bins=1)
+    pars = {"mu": 1.0, "shapesys": 1.0}
     data = model.expected_data(pars)
     # just check that it doesn't crash
     relaxed.fisher_info(model, pars, data)
 
 
-def test_fisher_uncerts_validity():
+@pytest.mark.parametrize("n_bins", [1, 2, 10])
+def test_fisher_uncerts_validity(n_bins):
     pyhf.set_backend("jax", pyhf.optimize.minuit_optimizer(verbose=1))
-    m = pyhf.simplemodels.uncorrelated_background([5], [50], [5])
-    data = jnp.array([50.0, *m.config.auxdata])
+    m = pyhf.simplemodels.uncorrelated_background(
+        [5] * n_bins, [50] * n_bins, [5] * n_bins
+    )
+    data = jnp.array([*[50.0] * n_bins, *m.config.auxdata])
 
     fit_res = pyhf.infer.mle.fit(
         data,
         m,
         return_uncertainties=True,
         par_bounds=[
             [-1, 10],
-            [-1, 10],
+            *[[-1, 10]] * n_bins,
         ],  # fit @ boundary produces unstable uncerts
     )
 
     # minuit fit uncerts
     mle_pars, mle_uncerts = fit_res[:, 0], fit_res[:, 1]
-
+    mle_pars_dict = {"mu": mle_pars[0], "shapesys": mle_pars[1:]}
     # uncertainties from autodiff hessian
-    dummy_m = uncorrelated_background(
-        jnp.array([5]),
-        jnp.array([50]),
-        jnp.array([5]),
+    dummy_m = HEPDataLike(
+        jnp.array([5] * n_bins),
+        jnp.array([50] * n_bins),
+        jnp.array([5] * n_bins),
     )
-    relaxed_uncerts = relaxed.cramer_rao_uncert(dummy_m, mle_pars, data)
-    assert np.allclose(mle_uncerts, relaxed_uncerts, rtol=0.05)
+    data_rlx = jnp.array([50.0] * n_bins), jnp.array(m.config.auxdata)
 
+    fisher_rlx = relaxed.fisher_info(dummy_m, mle_pars_dict, data_rlx)
+    fisher_pyhf = jnp.linalg.inv(
+        -jax.hessian(lambda p, d: m.logpdf(p, d)[0])(mle_pars, data)
+    )
 
-def test_fisher_info_grad():
-    pyhf.set_backend("jax")
+    # compare
+    assert np.allclose(fisher_rlx, fisher_pyhf)  # exact match for fisher info
+    relaxed_uncerts = relaxed.cramer_rao_uncert(
+        dummy_m, mle_pars_dict, data_rlx, return_tree=False
+    )
+    assert np.allclose(
+        mle_uncerts, relaxed_uncerts, rtol=5e-2
+    )  # within 5%, don't expect exact match with minuit
 
+
+def test_fisher_info_grad():
     def pipeline(x):
-        model = example_model(5.0)
-        pars = model.config.suggested_init()
+        model = example_model(5.0, n_bins=2)
+        pars = {"mu": jnp.array(0.0), "shapesys": jnp.array([1.0, 1.0])}
         data = model.expected_data(pars)
-        return relaxed.fisher_info(model, pars * x, data * x)
+        return relaxed.fisher_info(
+            model, tree_map(lambda a: a * x, pars), tree_map(lambda a: a * x, data)
+        )
 
+    pipeline(4.0)  # just check you can calc it w/o exception
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
-def test_fisher_uncert_grad():
-    pyhf.set_backend("jax")
-
+@pytest.mark.parametrize("return_tree", [True, False])
+def test_fisher_uncert_grad(return_tree):
     def pipeline(x):
-        model = example_model(5.0)
-        pars = model.config.suggested_init()
+        model = example_model(5.0, n_bins=2)
+        pars = {"mu": jnp.array(0.0), "shapesys": jnp.array([1.0, 1.0])}
         data = model.expected_data(pars)
-        return relaxed.cramer_rao_uncert(model, pars * x, data * x)
+        return relaxed.cramer_rao_uncert(
+            model,
+            tree_map(lambda a: a * x, pars),
+            (data[0] * x, data[1] * x),
+            return_tree=return_tree,
+        )
 
+    pipeline(4.0)  # just check you can calc it w/o exception
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
 @pytest.mark.parametrize("keep", ["above", "below"])
 def test_cut_validity(big_sample, keep):
     """Recover hard cut in large slope case."""
     weights = relaxed.cut(big_sample, 0, slope=100000, keep=keep)
@@ -174,17 +196,15 @@
 
     assert np.allclose(weights, np_cut)
 
 
 @pytest.mark.parametrize("keep", ["above", "below"])
 def test_cut_grad(keep):
     def pipeline(x):
-        model = example_model(5.0)
-        pars = model.config.suggested_init()
-        data = model.expected_data(pars)
+        data = jnp.array([1.0, 2.0, 3.0])
         return relaxed.cut(data, x, keep=keep)
 
     jacrev(pipeline)(4.0)  # just check you can calc it w/o exception
 
 
 def test_invalid_cut_keep():
     with pytest.raises(ValueError, match="keep must be one of"):
```

### Comparing `relaxed-0.3.0/.gitignore` & `relaxed-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/LICENSE` & `relaxed-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/README.md` & `relaxed-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `relaxed-0.3.0/pyproject.toml` & `relaxed-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,43 @@
 [project]
 name = "relaxed"
 authors = [
   { name = "Nathan Simpson", email = "nsimpson@turing.ac.uk" },
 ]
 description = "Differentiable versions of common HEP operations."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-  "equinox",
-  "jaxopt>=0.7",   # LBFGSB
-  "optax>=0.1.2",  # deprecated jax.tree_multimap
+  "equinox>=0.10.6", # eqx.field
+  "jaxopt>=0.7",     # LBFGSB
   "typing_extensions >=4.6; python_version<'3.11'",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
-  "pyhf[jax] >=0.7.0",
+  "pyhf[jax]", # should be pyhf[jax] >=0.7.1, but not released yet
   "iminuit",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
 docs = [
@@ -90,15 +88,15 @@
   'pragma: no cover',
   '\.\.\.',
   'if typing.TYPE_CHECKING:',
 ]
 
 [tool.mypy]
 files = ["src", "tests"]
-python_version = "3.8"
+python_version = "3.9"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
```

### Comparing `relaxed-0.3.0/PKG-INFO` & `relaxed-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relaxed
-Version: 0.3.0
+Version: 0.4.0
 Summary: Differentiable versions of common HEP operations.
 Project-URL: Homepage, https://github.com/gradhep/relaxed
 Project-URL: Bug Tracker, https://github.com/gradhep/relaxed/issues
 Project-URL: Discussions, https://github.com/gradhep/relaxed/discussions
 Project-URL: Changelog, https://github.com/gradhep/relaxed/releases
 Author-email: Nathan Simpson <nsimpson@turing.ac.uk>
 License-File: LICENSE
@@ -12,39 +12,37 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Requires-Dist: equinox
+Requires-Python: >=3.9
+Requires-Dist: equinox>=0.10.6
 Requires-Dist: jaxopt>=0.7
-Requires-Dist: optax>=0.1.2
 Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: iminuit; extra == 'test'
-Requires-Dist: pyhf[jax]>=0.7.0; extra == 'test'
+Requires-Dist: pyhf[jax]; extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="40%" alt="relaxed logo" src=relaxed-logo.png><br>
   <br>
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: relaxed Version: 0.3.0 Summary: Differentiable
+Metadata-Version: 2.1 Name: relaxed Version: 0.4.0 Summary: Differentiable
 versions of common HEP operations. Project-URL: Homepage, https://github.com/
 gradhep/relaxed Project-URL: Bug Tracker, https://github.com/gradhep/relaxed/
 issues Project-URL: Discussions, https://github.com/gradhep/relaxed/discussions
 Project-URL: Changelog, https://github.com/gradhep/relaxed/releases Author-
 email: Nathan Simpson
 turing.ac.uk> License-File: LICENSE Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Scientific/Engineering Classifier: Typing :: Typed Requires-Python:
->=3.8 Requires-Dist: equinox Requires-Dist: jaxopt>=0.7 Requires-Dist:
-optax>=0.1.2 Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering Classifier: Typing
+:: Typed Requires-Python: >=3.9 Requires-Dist: equinox>=0.10.6 Requires-Dist:
+jaxopt>=0.7 Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
 Provides-Extra: dev Requires-Dist: pytest-cov>=3; extra == 'dev' Requires-Dist:
 pytest>=6; extra == 'dev' Provides-Extra: docs Requires-Dist: furo; extra ==
 'docs' Requires-Dist: myst-parser>=0.13; extra == 'docs' Requires-Dist: sphinx-
 autodoc-typehints; extra == 'docs' Requires-Dist: sphinx-book-theme>=0.1.0;
 extra == 'docs' Requires-Dist: sphinx-copybutton; extra == 'docs' Requires-
 Dist: sphinx>=4.0; extra == 'docs' Provides-Extra: test Requires-Dist: iminuit;
-extra == 'test' Requires-Dist: pyhf[jax]>=0.7.0; extra == 'test' Requires-Dist:
+extra == 'test' Requires-Dist: pyhf[jax]; extra == 'test' Requires-Dist:
 pytest-cov>=3; extra == 'test' Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
                                 [relaxed logo]
 
 [GitHub_Workflow_Status] [Read_the_Docs] [Read_the_Docs] [Zenodo_DOI] [Binder]
 [actions-badge]: https://github.com/gradhep/relaxed/workflows/CI/badge.svg
 [actions-link]: https://github.com/gradhep/relaxed/actions [black-badge]:
```

