# Comparing `tmp/flardl-0.0.7.tar.gz` & `tmp/flardl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.7.tar", max compression
+gzip compressed data, was "flardl-0.0.8.tar", max compression
```

## Comparing `flardl-0.0.7.tar` & `flardl-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1958 2023-08-03 23:12:16.444260 flardl-0.0.7/LICENSE
--rw-r--r--   0        0        0      243 2023-08-03 23:12:16.444260 flardl-0.0.7/LICENSE.logo.txt
--rw-r--r--   0        0        0     8565 2023-08-03 23:12:16.444260 flardl-0.0.7/README.md
--rw-r--r--   0        0        0     2922 2023-08-03 23:12:27.892380 flardl-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      673 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/__init__.py
--rw-r--r--   0        0        0     3380 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/common.py
--rw-r--r--   0        0        0     1581 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/dict_to_indexed_list.py
--rwxr-xr-x   0        0        0     8241 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/downloader.py
--rwxr-xr-x   0        0        0     4225 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/instrumented_streams.py
--rwxr-xr-x   0        0        0     7661 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/multidispatcher.py
--rw-r--r--   0        0        0        0 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/py.typed
--rw-r--r--   0        0        0      651 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/server_defs.py
--rwxr-xr-x   0        0        0    11622 2023-08-03 23:12:16.452261 flardl-0.0.7/src/flardl/stream_stats.py
--rw-r--r--   0        0        0     9910 1970-01-01 00:00:00.000000 flardl-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-08-04 17:22:20.352960 flardl-0.0.8/LICENSE
+-rw-r--r--   0        0        0      243 2023-08-04 17:22:20.352960 flardl-0.0.8/LICENSE.logo.txt
+-rw-r--r--   0        0        0     9815 2023-08-04 17:22:31.801209 flardl-0.0.8/README.md
+-rw-r--r--   0        0        0     2957 2023-08-04 17:22:31.801209 flardl-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      673 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3380 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     8278 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/downloader.py
+-rwxr-xr-x   0        0        0     4225 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/instrumented_streams.py
+-rwxr-xr-x   0        0        0     7734 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/py.typed
+-rw-r--r--   0        0        0      651 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/server_defs.py
+-rwxr-xr-x   0        0        0    11622 2023-08-04 17:22:20.356960 flardl-0.0.8/src/flardl/stream_stats.py
+-rw-r--r--   0        0        0    11181 1970-01-01 00:00:00.000000 flardl-0.0.8/PKG-INFO
```

### Comparing `flardl-0.0.7/LICENSE` & `flardl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/README.md` & `flardl-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,95 +48,111 @@
 long tails**. For collections with long-tail distributions, one
 finds many more examples of big files than of small files at
 a given additive distance above or below the peak (model) value.
 Examples of analytical forms of long-tail distributions include
 Zipf, power-law, and log-norm distributions. A real-world example
 of a long-tail distribution is shown in the figure below, which
 plots the file-size histogram for 1000 randomly-sampled examples
-CIF structure files from the [Protein Data Bank](https://rcsb.org) along with
-a kernel-density estimate and fits to log-normal and normal
-distributions.
+CIF structure files from the [Protein Data Bank](https://rcsb.org)
+along with a kernel-density estimate and fits to log-normal and
+normal distributions.
 
 ![sizedist](https://raw.githubusercontent.com/hydrationdynamics/flardl/main/docs/_static/file_size_distribution.png)
 
-The effects of
-the big files in the long tail are frequently ignored in queuing
-algorithms.
-
-The nature of long-tail distributions is such that **mean values are nearly
-worthless** because--unlike on normal distributions--means of runs drawn
+There are big effects on overall statistics from the big files in
+the long tail, effects that are frequently ignored in queueing
+literature and many queuing algorithms which treat collections
+as normal-ish. The biggest single issue, which can be seen in
+the difference between normal-distribution fits to a
+randomly-selected 5% and the full 1000 points in the figure above,
+is that **mean values are neither stable nor characteristic of the
+distribution**. Unlike on normal distributions--means of runs drawn
 from them grow larger with the size of the run. Because of the appreciable
-likelihood of drawing a really large file to be downloaded from a long-tail
-distribution, he total download time and therefore the mean downloading rate
-depends strongly on how many large-size outliers are included in your sample. Timings of algorithms that do
-If you are downloading multiple files simultaneously, the overall download
-time may also depend strongly on whether a large file happens to occur at
-the end of the list, causing an "overhang" of wwaiting for a single file.
-Theories and algorithms based on overall times or mean rates won't
-work very well on the long-tail distributions that often characterize
-real collections. T
-
-**Modal values are a good statistic for power-law distributions**, unlike
-means. To put that another way, the average download time $\overline{t_{dl}}$
-varies a lot
-between runs, but the _most-common_ download time
-$\tilde{t}_{dl}$ can be pretty
-consistent. The mode of file lengths and the mode of download bit rate
-are both quantities that are easy to estimate for a
-collection and a collection and rarely change. If one happens to select
-the biggest files for downloading, or if one happens to try downloading
-a long collection at the same time that someone is watching a high-bit-rate
-video on the same shared connection, then it's easy to adjust a bit
-for just that time.
-
-Here I propose a heuristic called **adaptive-depth queuing**
-that gives robust performance in real situations while being simple
-enough to be easily understood and coded.
+likelihood of drawing a really large file to be downloaded, the total
+download time $t_{\rm tot}$ and therefore the mean per-file download rate
+$\overline{k_{\rm file}}$ both depend strongly on how many big-file outliers
+are included in your sample. If you are downloading multiple files
+simultaneously, the overall download time may also depend strongly on
+where in the list the large files happen to occur, because those at
+the end can cause an "overhang" of a single stream waiting for that file.
+
+While the mean per-file download rate varies a lot between runs, the
+_most-common_ per-file download rate $\tilde{k}_{\rm file}$ can be more
+consistent, at least on the timescale of days. If you are downloading a
+long list of files at the same time that someone else on your LAN
+is watching a video, then you may not achieve the same saturation
+bit rate $b{\rm sat}$ as when you're the only network user. The modal
+file size of a collection can be quite stable over time, so we have hope
+that if we formulate download times in terms of the modal file size
+and that day's estimated server latencies and achievable download
+bit rate, the situation might be more tractable still.
 
 Even more than maximizing download rates, the highest priority must
 be to **avoid black-listing by a server**. Most public-facing servers
 have policies to recognize and defend against Denial-Of-Service (DOS)
-attacks. The response to a DOS event, at the very least, causes the server to
-dump your latest request, which is usually a minor nuisance
-as it can be retried later. Far worse is
-if the server responds by severely throttling further requests from your
-IP address for hours or sometime days.
-Worst of all, your IP address can get the "death penalty" and be put
-on a permanent blacklist that may require manual intervention for
-removal. You generally don't know thThe simplest
-possibility of le trigger levels for these policies.
-Worse still, it might not even be you. I have seen a practical class
-of 20 students brought to a complete halt
-by a server's 24-hour black-listing of the institution's IP address.
-
-Simply launching a large number of requests and letting the
-servers sort it out is a strategy that maximizes the chance
-of black-listing for two reasons. First, this strategy results in
-equal division of transfers without regard to varying transfer sizes or
-server latencies. Second,
-
-Given that a single server can saturate a gigabit
-connection, given enough simultaneous downloads, a better
-strategy is to **keep the total request-queue depth just high enough to
-achieve saturation**. This goal can be achieved by launching a large
-number of requests, up to some maximum permissible queue depth
-$Q_{\rm max}$ (either by guess or by previous knowledge of individual
-servers), during the server latency period when no transfers have been
-completed. As transfers are completed, one can then calculate the
-saturation bandwidth $B$ and
-the total-over-all-servers depth at which saturation was achieved,
-$Q_{\rm sat}$
-
-running the
-request For those who are lucky enough to be on
-a multi-gigabit connection, it's a good idea to limit the bandwidth
-to something you know the set of servers you are using won't complain
-about. It would be nice if one could query a server for an acceptable
-request queue depth which would guarantee no DOS response or other
-server throttling, but I have not seen such a mechanism implemented.
+attacks. The response to a DOS event, at the very least, causes the
+server to dump your latest request, which is usually a minor nuisance
+as it can be retried later. Far worse is if the server responds by
+severely throttling further requests from your IP address for hours
+or sometime days. Worst of all, your IP address can get the "death
+penalty" and be put on a permanent blacklist that may require manual
+intervention for removal. You generally don't know thThe simplest
+possibility of le trigger levels for these policies. Blacklisting
+might not even be your personal fault, but a collective problem.
+I have seen a practical class of 20 students brought to a complete
+halt by a server's 24-hour black-listing of the institution's
+public IP address.
+
+An analogy might help us here. Let's say you are a person who
+enjoys keeping track of statistics, and you decide to try
+fishing. At first, you have a single fishing rod and you go
+fishing at a series of local lakes where your catch consists
+of small bony fishes called "crappies". Your records reval
+that while the rate of catching fishes can vary from day to
+day--fish might be hungry or not--the average size of your
+catch is pretty stable. Bigger ponds tend to have bigger fish
+in them, and it might take slightly longer to reel in a bigger
+crappie than a small one, but big and small averages out to
+that pond.
+
+Then one day you decide you love fishing so much, you drive
+to the coast and charter a fishing boat. On that boat,
+you can set out as many lines as you want (up to some limit)
+and fish in parallel. At first, you seem to be catching the
+ocean-going equivalent of crappies, small bony fishes. But
+then you hook a small shark, which not only takes a lot of
+your time and attention to reel in, but which totally skews
+your estimate of average weight of your catch. You know that
+if you can catch a small shark, then maybe if you fish for
+long enough you might catch a big shark, or even a small whale.
+But you and your crew can only effecively reel in so
+many hooked lines at once. Putting out more lines than
+that effective limit of hooked- plus waiting-to-be-hooked
+lines only results in fishes waiting on the line, when they
+may break the line or get partly eaten before you can reel
+them in.
+
+Here I propose and implement a method called **adaptilastic
+queuing** that gives robust performance in real situations
+while being simple enough to be easily understood and coded.
+The basis of edaptilastic queueing is keeping the total
+request-queue depth just high enough to achieve saturation.
+The method launches a large number of requests at the most-likely
+per-file rate at saturation, up to some maximum permissible
+per-server queue depth $D_{i}_{\rm max}$ (either by guess or
+by previous knowledge of individual servers) during the period
+before any transfers have completed. As transfers are completed,
+the method estimates the total-over-all-servers depth at which
+saturation was achieved, and updates its estimate of the
+achievable line bit rate and the most-likely per-file return
+rate on a per-server basis as the bases for managing future
+requests. Servers that return modal-length files (crappies)
+more quickly thus are given a better chance at nabbing an
+open queue slot without penalizing a server that happened
+to draw a big download (whale).
 
 ## Requirements
 
 _Flardl_ is tested under python 3.11, on Linux, MacOS, and
 Windows and under 3.9 and 3.10 on Linux. Under the hood,
 _flardl_ relies on [httpx](https://www.python-httpx.org/) and is supported
 on whatever platforms that library works under, for both HTTP/1.1 and HTTP/2.
```

### Comparing `flardl-0.0.7/pyproject.toml` & `flardl-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.7"
+version = "0.0.8"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
@@ -23,14 +23,16 @@
 keywords = [
     "downloads",
     "asynchronous",
     "high-performance",
     "multi-dispatching",
     "queueing",
     "adaptive",
+    "elastic",
+    "adaptilastic",
     "federated"
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/hydrationdynamics/flardl/releases"
 
 [tool.poetry.dependencies]
```

### Comparing `flardl-0.0.7/src/flardl/__init__.py` & `flardl-0.0.8/src/flardl/__init__.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/src/flardl/common.py` & `flardl-0.0.8/src/flardl/common.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/src/flardl/dict_to_indexed_list.py` & `flardl-0.0.8/src/flardl/dict_to_indexed_list.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/src/flardl/downloader.py` & `flardl-0.0.8/src/flardl/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Downloads as a MultiDispatcher worker class."""
 
 import pathlib
 import sys
 from typing import Any
 from typing import Optional
+from typing import Union
 
 # third-party imports
 import anyio
 import httpx
 import loguru
 
 # module imports
@@ -60,15 +61,15 @@
 
     async def limiter(self):
         """Fake rate-limiting via sleep."""
         await anyio.sleep(self._limiter_delay(self.launch_rate))
 
     async def add_result(
         self,
-        data: bytes | str,
+        data: Union[bytes, str],
         filename: str,
         idx: int,
         worker_count: int,
         result_q: ResultStream,
         /,
         **kwargs: dict[str, SIMPLE_TYPES],
     ):
@@ -166,16 +167,16 @@
 
     async def worker(
         self,
         result_q: ResultStream,
         worker_count: int,
         /,
         idx: int,
-        code: str | None = None,
-        file_type: str | None = None,
+        code: Optional[str] = None,
+        file_type: Optional[str] = None,
     ):
         """Do a work unit."""
         if idx in self.SOFT_FAILS:
             async with self._lock:
                 self.n_soft_fails += 1
                 if idx in self.RESCUE_SOFT_FAILS:
                     self.SOFT_FAILS.remove(idx)
```

### Comparing `flardl-0.0.7/src/flardl/instrumented_streams.py` & `flardl-0.0.8/src/flardl/instrumented_streams.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/src/flardl/multidispatcher.py` & `flardl-0.0.8/src/flardl/multidispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Dispatch work to multiple workers and collect results via AnyIO streams."""
 
 import sys
 from typing import Any
 from typing import Optional
+from typing import Union
 
 # third-party imports
 import anyio
 import httpx
 import loguru
 from loguru import logger as mylogger
 
@@ -28,20 +29,20 @@
 class MultiDispatcher:
     """Runs multiple single-site dispatchers sharing streams."""
 
     def __init__(  # noqa: C901
         self,
         all_worker_defs: list[ServerDef],
         /,
-        worker_list: list[str] | None = None,
+        worker_list: Optional[list[str]] = None,
         max_retries: int = DEFAULT_MAX_RETRIES,
         logger: Optional["loguru.Logger"] = None,
         quiet: bool = False,
         history_len: int = 0,
-        output_dir: str | None = None,
+        output_dir: Optional[str] = None,
         mock: bool = False,
         runner: str = "production",
     ) -> None:
         """Save list of dispatchers."""
         if logger is None:
             self._logger = mylogger
         else:
@@ -96,17 +97,17 @@
         self.queue_stats = StreamStats(all_worker_names, history_len=history_len)
         self._lock = anyio.Lock()
         self.inflight: dict[str, SIMPLE_TYPES] = {}
         self.timer = MillisecondTimer()
 
     async def run(
         self,
-        args: (
-            list[dict[str, SIMPLE_TYPES]] | dict[str, NonStringIterable | SIMPLE_TYPES]
-        ),
+        args: Union[
+            list[dict[str, SIMPLE_TYPES]], dict[str, NonStringIterable, SIMPLE_TYPES]
+        ],
     ):
         """Run the multidispatcher queue."""
         if isinstance(args, list):
             arg_list = args
         elif isinstance(args, dict):
             arg_list = zip_dict_to_indexed_list(args)
         arg_q = ArgumentStream(arg_list, self.inflight, self.timer)
@@ -188,16 +189,18 @@
             except Exception as e:
                 # unhandled errors go to unhandled exception handler
                 idx = kwargs[INDEX_KEY]
                 await worker.unhandled_exception_handler(idx, e)
 
     def main(
         self,
-        arg_list: list[dict[str, SIMPLE_TYPES]]
-        | dict[str, NonStringIterable | SIMPLE_TYPES],
+        arg_list: Union[
+            list[dict[str, SIMPLE_TYPES]],
+            dict[str, Union[NonStringIterable, SIMPLE_TYPES]],
+        ],
     ):
         """Start the multidispatcher queue."""
         return anyio.run(
             self.run,
             arg_list,
             backend=self.backend,
             backend_options=self.backend_options,
```

### Comparing `flardl-0.0.7/src/flardl/server_defs.py` & `flardl-0.0.8/src/flardl/server_defs.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/src/flardl/stream_stats.py` & `flardl-0.0.8/src/flardl/stream_stats.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.7/PKG-INFO` & `flardl-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: flardl
-Version: 0.0.7
+Version: 0.0.8
 Summary: Flardl
 Home-page: https://github.com/hydrationdynamics/flardl
 License: BSD-3-Clause
-Keywords: downloads,asynchronous,high-performance,multi-dispatching,queueing,adaptive,federated
+Keywords: downloads,asynchronous,high-performance,multi-dispatching,queueing,adaptive,elastic,adaptilastic,federated
 Author: Joel Berendzen
 Author-email: joel@generisbio.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -81,95 +81,111 @@
 long tails**. For collections with long-tail distributions, one
 finds many more examples of big files than of small files at
 a given additive distance above or below the peak (model) value.
 Examples of analytical forms of long-tail distributions include
 Zipf, power-law, and log-norm distributions. A real-world example
 of a long-tail distribution is shown in the figure below, which
 plots the file-size histogram for 1000 randomly-sampled examples
-CIF structure files from the [Protein Data Bank](https://rcsb.org) along with
-a kernel-density estimate and fits to log-normal and normal
-distributions.
+CIF structure files from the [Protein Data Bank](https://rcsb.org)
+along with a kernel-density estimate and fits to log-normal and
+normal distributions.
 
 ![sizedist](https://raw.githubusercontent.com/hydrationdynamics/flardl/main/docs/_static/file_size_distribution.png)
 
-The effects of
-the big files in the long tail are frequently ignored in queuing
-algorithms.
-
-The nature of long-tail distributions is such that **mean values are nearly
-worthless** because--unlike on normal distributions--means of runs drawn
+There are big effects on overall statistics from the big files in
+the long tail, effects that are frequently ignored in queueing
+literature and many queuing algorithms which treat collections
+as normal-ish. The biggest single issue, which can be seen in
+the difference between normal-distribution fits to a
+randomly-selected 5% and the full 1000 points in the figure above,
+is that **mean values are neither stable nor characteristic of the
+distribution**. Unlike on normal distributions--means of runs drawn
 from them grow larger with the size of the run. Because of the appreciable
-likelihood of drawing a really large file to be downloaded from a long-tail
-distribution, he total download time and therefore the mean downloading rate
-depends strongly on how many large-size outliers are included in your sample. Timings of algorithms that do
-If you are downloading multiple files simultaneously, the overall download
-time may also depend strongly on whether a large file happens to occur at
-the end of the list, causing an "overhang" of wwaiting for a single file.
-Theories and algorithms based on overall times or mean rates won't
-work very well on the long-tail distributions that often characterize
-real collections. T
-
-**Modal values are a good statistic for power-law distributions**, unlike
-means. To put that another way, the average download time $\overline{t_{dl}}$
-varies a lot
-between runs, but the _most-common_ download time
-$\tilde{t}_{dl}$ can be pretty
-consistent. The mode of file lengths and the mode of download bit rate
-are both quantities that are easy to estimate for a
-collection and a collection and rarely change. If one happens to select
-the biggest files for downloading, or if one happens to try downloading
-a long collection at the same time that someone is watching a high-bit-rate
-video on the same shared connection, then it's easy to adjust a bit
-for just that time.
-
-Here I propose a heuristic called **adaptive-depth queuing**
-that gives robust performance in real situations while being simple
-enough to be easily understood and coded.
+likelihood of drawing a really large file to be downloaded, the total
+download time $t_{\rm tot}$ and therefore the mean per-file download rate
+$\overline{k_{\rm file}}$ both depend strongly on how many big-file outliers
+are included in your sample. If you are downloading multiple files
+simultaneously, the overall download time may also depend strongly on
+where in the list the large files happen to occur, because those at
+the end can cause an "overhang" of a single stream waiting for that file.
+
+While the mean per-file download rate varies a lot between runs, the
+_most-common_ per-file download rate $\tilde{k}_{\rm file}$ can be more
+consistent, at least on the timescale of days. If you are downloading a
+long list of files at the same time that someone else on your LAN
+is watching a video, then you may not achieve the same saturation
+bit rate $b{\rm sat}$ as when you're the only network user. The modal
+file size of a collection can be quite stable over time, so we have hope
+that if we formulate download times in terms of the modal file size
+and that day's estimated server latencies and achievable download
+bit rate, the situation might be more tractable still.
 
 Even more than maximizing download rates, the highest priority must
 be to **avoid black-listing by a server**. Most public-facing servers
 have policies to recognize and defend against Denial-Of-Service (DOS)
-attacks. The response to a DOS event, at the very least, causes the server to
-dump your latest request, which is usually a minor nuisance
-as it can be retried later. Far worse is
-if the server responds by severely throttling further requests from your
-IP address for hours or sometime days.
-Worst of all, your IP address can get the "death penalty" and be put
-on a permanent blacklist that may require manual intervention for
-removal. You generally don't know thThe simplest
-possibility of le trigger levels for these policies.
-Worse still, it might not even be you. I have seen a practical class
-of 20 students brought to a complete halt
-by a server's 24-hour black-listing of the institution's IP address.
-
-Simply launching a large number of requests and letting the
-servers sort it out is a strategy that maximizes the chance
-of black-listing for two reasons. First, this strategy results in
-equal division of transfers without regard to varying transfer sizes or
-server latencies. Second,
-
-Given that a single server can saturate a gigabit
-connection, given enough simultaneous downloads, a better
-strategy is to **keep the total request-queue depth just high enough to
-achieve saturation**. This goal can be achieved by launching a large
-number of requests, up to some maximum permissible queue depth
-$Q_{\rm max}$ (either by guess or by previous knowledge of individual
-servers), during the server latency period when no transfers have been
-completed. As transfers are completed, one can then calculate the
-saturation bandwidth $B$ and
-the total-over-all-servers depth at which saturation was achieved,
-$Q_{\rm sat}$
-
-running the
-request For those who are lucky enough to be on
-a multi-gigabit connection, it's a good idea to limit the bandwidth
-to something you know the set of servers you are using won't complain
-about. It would be nice if one could query a server for an acceptable
-request queue depth which would guarantee no DOS response or other
-server throttling, but I have not seen such a mechanism implemented.
+attacks. The response to a DOS event, at the very least, causes the
+server to dump your latest request, which is usually a minor nuisance
+as it can be retried later. Far worse is if the server responds by
+severely throttling further requests from your IP address for hours
+or sometime days. Worst of all, your IP address can get the "death
+penalty" and be put on a permanent blacklist that may require manual
+intervention for removal. You generally don't know thThe simplest
+possibility of le trigger levels for these policies. Blacklisting
+might not even be your personal fault, but a collective problem.
+I have seen a practical class of 20 students brought to a complete
+halt by a server's 24-hour black-listing of the institution's
+public IP address.
+
+An analogy might help us here. Let's say you are a person who
+enjoys keeping track of statistics, and you decide to try
+fishing. At first, you have a single fishing rod and you go
+fishing at a series of local lakes where your catch consists
+of small bony fishes called "crappies". Your records reval
+that while the rate of catching fishes can vary from day to
+day--fish might be hungry or not--the average size of your
+catch is pretty stable. Bigger ponds tend to have bigger fish
+in them, and it might take slightly longer to reel in a bigger
+crappie than a small one, but big and small averages out to
+that pond.
+
+Then one day you decide you love fishing so much, you drive
+to the coast and charter a fishing boat. On that boat,
+you can set out as many lines as you want (up to some limit)
+and fish in parallel. At first, you seem to be catching the
+ocean-going equivalent of crappies, small bony fishes. But
+then you hook a small shark, which not only takes a lot of
+your time and attention to reel in, but which totally skews
+your estimate of average weight of your catch. You know that
+if you can catch a small shark, then maybe if you fish for
+long enough you might catch a big shark, or even a small whale.
+But you and your crew can only effecively reel in so
+many hooked lines at once. Putting out more lines than
+that effective limit of hooked- plus waiting-to-be-hooked
+lines only results in fishes waiting on the line, when they
+may break the line or get partly eaten before you can reel
+them in.
+
+Here I propose and implement a method called **adaptilastic
+queuing** that gives robust performance in real situations
+while being simple enough to be easily understood and coded.
+The basis of edaptilastic queueing is keeping the total
+request-queue depth just high enough to achieve saturation.
+The method launches a large number of requests at the most-likely
+per-file rate at saturation, up to some maximum permissible
+per-server queue depth $D_{i}_{\rm max}$ (either by guess or
+by previous knowledge of individual servers) during the period
+before any transfers have completed. As transfers are completed,
+the method estimates the total-over-all-servers depth at which
+saturation was achieved, and updates its estimate of the
+achievable line bit rate and the most-likely per-file return
+rate on a per-server basis as the bases for managing future
+requests. Servers that return modal-length files (crappies)
+more quickly thus are given a better chance at nabbing an
+open queue slot without penalizing a server that happened
+to draw a big download (whale).
 
 ## Requirements
 
 _Flardl_ is tested under python 3.11, on Linux, MacOS, and
 Windows and under 3.9 and 3.10 on Linux. Under the hood,
 _flardl_ relies on [httpx](https://www.python-httpx.org/) and is supported
 on whatever platforms that library works under, for both HTTP/1.1 and HTTP/2.
```

