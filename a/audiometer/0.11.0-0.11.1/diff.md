# Comparing `tmp/audiometer-0.11.0.tar.gz` & `tmp/audiometer-0.11.1.tar.gz`

## Comparing `audiometer-0.11.0.tar` & `audiometer-0.11.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 audiometer-0.11.0/Cargo.toml
--rw-r--r--   0      501       20      147 2022-08-27 08:42:08.000000 audiometer-0.11.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0      501       20      307 2022-08-27 08:42:08.000000 audiometer-0.11.0/.github/release-drafter-config.yml
--rw-r--r--   0      501       20      307 2022-08-27 08:42:08.000000 audiometer-0.11.0/.github/workflows/release-drafter.yml
--rw-r--r--   0      501       20     1503 2023-01-15 13:11:55.000000 audiometer-0.11.0/.github/workflows/release.yml
--rw-r--r--   0      501       20     1872 2023-01-15 12:45:34.000000 audiometer-0.11.0/.gitignore
--rw-r--r--   0      501       20      309 2022-08-27 08:42:08.000000 audiometer-0.11.0/.pre-commit-config.yaml
--rw-r--r--   0      501       20       77 2022-08-31 14:13:01.000000 audiometer-0.11.0/Makefile
--rw-r--r--   0      501       20       43 2022-08-31 14:13:01.000000 audiometer-0.11.0/README.md
--rw-r--r--   0      501       20      396 2023-01-15 13:10:26.000000 audiometer-0.11.0/pyproject.toml
--rw-r--r--   0      501       20        0 2023-01-15 12:52:38.000000 audiometer-0.11.0/python/__init__.py
--rw-r--r--   0      501       20      102 2023-01-15 13:08:12.000000 audiometer-0.11.0/python/audiometer/__init__.py
--rw-r--r--   0      501       20      692 2023-01-15 13:08:12.000000 audiometer-0.11.0/python/audiometer/_audiometer.py
--rw-r--r--   0      501       20      137 2023-01-15 13:05:51.000000 audiometer-0.11.0/rms.pyi
--rw-r--r--   0      501       20     1904 2023-01-15 13:05:20.000000 audiometer-0.11.0/src/lib.rs
--rw-r--r--   0      501       20       54 2022-08-27 08:42:08.000000 audiometer-0.11.0/tox.ini
--rw-r--r--   0      501       20     7415 2023-01-15 12:54:41.000000 audiometer-0.11.0/Cargo.lock
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 audiometer-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0      352 1970-01-01 00:00:00.000000 audiometer-0.11.1/Cargo.toml
+-rw-r--r--   0     1001      123      147 2023-02-01 14:32:45.000000 audiometer-0.11.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0     1001      123      307 2023-02-01 14:32:45.000000 audiometer-0.11.1/.github/release-drafter-config.yml
+-rw-r--r--   0     1001      123      307 2023-02-01 14:32:45.000000 audiometer-0.11.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      123     1516 2023-02-01 14:32:45.000000 audiometer-0.11.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1872 2023-02-01 14:32:45.000000 audiometer-0.11.1/.gitignore
+-rw-r--r--   0     1001      123      309 2023-02-01 14:32:45.000000 audiometer-0.11.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123       77 2023-02-01 14:32:45.000000 audiometer-0.11.1/Makefile
+-rw-r--r--   0     1001      123       43 2023-02-01 14:32:45.000000 audiometer-0.11.1/README.md
+-rw-r--r--   0     1001      123      396 2023-02-01 14:32:45.000000 audiometer-0.11.1/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-02-01 14:32:45.000000 audiometer-0.11.1/python/__init__.py
+-rw-r--r--   0     1001      123       99 2023-02-01 14:32:45.000000 audiometer-0.11.1/python/audiometer/__init__.py
+-rw-r--r--   0     1001      123      310 2023-02-01 14:32:45.000000 audiometer-0.11.1/python/audiometer/_audiometer.pyi
+-rw-r--r--   0     1001      123      685 2023-02-01 14:32:45.000000 audiometer-0.11.1/python/audiometer/_wrapper.py
+-rw-r--r--   0     1001      123        0 2023-02-01 14:32:45.000000 audiometer-0.11.1/python/audiometer/py.typed
+-rwxr-xr-x   0     1001      123      768 2023-02-01 14:33:21.000000 audiometer-0.11.1/run-maturin-action.sh
+-rw-r--r--   0     1001      123     2123 2023-02-01 14:32:45.000000 audiometer-0.11.1/src/lib.rs
+-rw-r--r--   0     1001      123       54 2023-02-01 14:32:45.000000 audiometer-0.11.1/tox.ini
+-rw-r--r--   0        0        0     7415 2023-02-01 14:34:24.000000 audiometer-0.11.1/Cargo.lock
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 audiometer-0.11.1/PKG-INFO
```

### Comparing `audiometer-0.11.0/.github/workflows/release.yml` & `audiometer-0.11.1/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: CI
+name: Release package
 
 on:
   release:
     types:
       - published
 
 jobs:
```

### Comparing `audiometer-0.11.0/.gitignore` & `audiometer-0.11.1/.gitignore`

 * *Files identical despite different names*

### Comparing `audiometer-0.11.0/python/audiometer/_audiometer.py` & `audiometer-0.11.1/python/audiometer/_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pydub
 
-from .audiometer import calculate_peak_inner, calculate_rms_inner
+from audiometer import _audiometer
 
 
 def calculate_rms(segment: pydub.AudioSegment) -> float:
     return round(
-        calculate_rms_inner(
+        _audiometer.calculate_rms_inner(
             samples=segment.get_array_of_samples(),
             channels=segment.channels,
             max_amplitude=segment.max_possible_amplitude,
             sample_rate=segment.frame_rate,
         ),
         1,
     )
 
 
 def calculate_peak(segment: pydub.AudioSegment) -> float:
     return round(
-        calculate_peak_inner(
+        _audiometer.calculate_peak_inner(
             samples=segment.get_array_of_samples(),
             channels=segment.channels,
             max_amplitude=segment.max_possible_amplitude,
         ),
         1,
     )
```

### Comparing `audiometer-0.11.0/src/lib.rs` & `audiometer-0.11.1/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 use pyo3::prelude::*;
 
+// Integration time 300ms을 2를 나눈 값인 150ms 만큼 지수이동평균 적용
+const INTEGRATION_TIME: f64 = 0.3 / 2.0;
+// AES17에 따라 RMS 값에 +3dB를 적용하기 위한 보정값 (log10(2) = 0.3)
 const AMPLITUDE_COEFFICIENT: f64 = 2.0;
 
 fn ratio_to_db(ratio: f64, using_amplitude: bool) -> f64 {
     if ratio == 0.0 {
         return f64::INFINITY;
     }
 
@@ -16,15 +19,15 @@
 #[pyfunction]
 fn calculate_rms_inner(
     samples: Vec<isize>,
     channels: usize,
     max_amplitude: f64,
     sample_rate: isize,
 ) -> f64 {
-    let decay_const = (-1.0 / sample_rate as f64 / (0.3 / 2.0)).exp();
+    let decay_const = (-1.0 / sample_rate as f64 / INTEGRATION_TIME).exp();
     let update_ratio = 1.0 - decay_const;
 
     let mut max_rms: f64 = 0.0;
     for i in 0..channels {
         let mut channel_max_rms: f64 = 0.0;
         let mut current_rms: f64 = 0.0;
         for channel_sample in samples[i..].iter().step_by(channels) {
@@ -53,12 +56,12 @@
     }
 
     ratio_to_db(max_peak, true)
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn audiometer(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _audiometer(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(calculate_rms_inner, m)?)?;
     m.add_function(wrap_pyfunction!(calculate_peak_inner, m)?)?;
     Ok(())
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `audiometer-0.11.0/Cargo.lock` & `audiometer-0.11.1/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
 version = "0.2.139"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
 
@@ -85,17 +85,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
```

