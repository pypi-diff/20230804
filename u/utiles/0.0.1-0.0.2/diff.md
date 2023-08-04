# Comparing `tmp/utiles-0.0.1.tar.gz` & `tmp/utiles-0.0.2.tar.gz`

## Comparing `utiles-0.0.1.tar` & `utiles-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 utiles-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 utiles-0.0.1/rust_src/utiles/Cargo.toml
--rw-r--r--   0     1001      123    10222 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/Cargo.lock
--rw-r--r--   0     1001      123    21380 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/README.md
--rw-r--r--   0     1001      123       54 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/bin/utiles.rs
--rw-r--r--   0     1001      123    24284 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/lib.rs
--rw-r--r--   0     1001      123     6421 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/purgatory/_coords.rs
--rw-r--r--   0     1001      123      141 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/mod.rs
--rw-r--r--   0     1001      123     4991 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pybbox.rs
--rw-r--r--   0     1001      123      966 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pyiters.rs
--rw-r--r--   0     1001      123     3144 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pylnglat.rs
--rw-r--r--   0     1001      123     4977 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pylnglatbbox.rs
--rw-r--r--   0     1001      123    13944 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pytile.rs
--rw-r--r--   0     1001      123      265 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/pytiles.rs
--rw-r--r--   0     1001      123     3008 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/tuple_slice.rs
--rw-r--r--   0     1001      123      106 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/pyutiles/zoom.rs
--rw-r--r--   0     1001      123      191 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/constants.rs
--rw-r--r--   0     1001      123     3627 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/libtiletype.rs
--rw-r--r--   0     1001      123    34323 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/mod.rs
--rw-r--r--   0     1001      123     4450 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/pmtiles.rs
--rw-r--r--   0     1001      123     1059 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/sibling_relationship.rs
--rw-r--r--   0     1001      123      649 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/traits.rs
--rw-r--r--   0     1001      123      282 2023-05-31 20:53:52.000000 utiles-0.0.1/rust_src/utiles/src/utiles/zoom.rs
--rw-r--r--   0     1001      123    10222 2023-05-31 20:53:52.000000 utiles-0.0.1/Cargo.lock
--rw-r--r--   0     1001      123    16691 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/cli.py
--rw-r--r--   0     1001      123     2876 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/__init__.py
--rw-r--r--   0     1001      123      260 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/__about__.py
--rw-r--r--   0     1001      123      817 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/__main__.py
--rw-r--r--   0     1001      123        0 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/py.typed
--rw-r--r--   0     1001      123     7137 2023-05-31 20:53:52.000000 utiles-0.0.1/python/utiles/libutiles.pyi
--rw-r--r--   0        0        0    21878 1970-01-01 00:00:00.000000 utiles-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 utiles-0.0.2/local_dependencies/utiles/Cargo.toml
+-rw-r--r--   0     1001      123       51 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/README.md
+-rw-r--r--   0     1001      123      191 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/constants.rs
+-rw-r--r--   0     1001      123    38223 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/lib.rs
+-rw-r--r--   0     1001      123     3627 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/libtiletype.rs
+-rw-r--r--   0     1001      123     4450 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/pmtiles.rs
+-rw-r--r--   0     1001      123     1051 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/sibling_relationship.rs
+-rw-r--r--   0     1001      123      649 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/traits.rs
+-rw-r--r--   0     1001      123      282 2023-08-04 20:37:31.000000 utiles-0.0.2/local_dependencies/utiles/src/zoom.rs
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 utiles-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 utiles-0.0.2/rust_src/utiles/Cargo.toml
+-rw-r--r--   0     1001      123    10130 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/Cargo.lock
+-rw-r--r--   0     1001      123    21380 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/README.md
+-rw-r--r--   0     1001      123       54 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/bin/utiles.rs
+-rw-r--r--   0     1001      123    25150 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/lib.rs
+-rw-r--r--   0     1001      123     6421 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/purgatory/_coords.rs
+-rw-r--r--   0     1001      123      141 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/mod.rs
+-rw-r--r--   0     1001      123     4977 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pybbox.rs
+-rw-r--r--   0     1001      123      966 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pyiters.rs
+-rw-r--r--   0     1001      123     3137 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pylnglat.rs
+-rw-r--r--   0     1001      123     4963 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pylnglatbbox.rs
+-rw-r--r--   0     1001      123    13994 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pytile.rs
+-rw-r--r--   0     1001      123      265 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/pytiles.rs
+-rw-r--r--   0     1001      123     3008 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/tuple_slice.rs
+-rw-r--r--   0     1001      123      106 2023-08-04 20:37:31.000000 utiles-0.0.2/rust_src/utiles/src/pyutiles/zoom.rs
+-rw-r--r--   0     1001      123    10130 2023-08-04 20:37:31.000000 utiles-0.0.2/Cargo.lock
+-rw-r--r--   0     1001      123      260 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/__about__.py
+-rw-r--r--   0     1001      123      817 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/__main__.py
+-rw-r--r--   0     1001      123     7334 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/libutiles.pyi
+-rw-r--r--   0     1001      123     2895 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/py.typed
+-rw-r--r--   0     1001      123    16691 2023-08-04 20:37:31.000000 utiles-0.0.2/python/utiles/cli.py
+-rw-r--r--   0        0        0    21905 1970-01-01 00:00:00.000000 utiles-0.0.2/PKG-INFO
```

### Comparing `utiles-0.0.1/pyproject.toml` & `utiles-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "utiles"
-version = "0.0.1"
+version = "0.0.2"
 description = "utiles = (utils + tiles) * rust"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `utiles-0.0.1/rust_src/utiles/Cargo.toml` & `utiles-0.0.2/rust_src/utiles/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [package]
-name = "utiles"
-version = "0.0.1"
+name = "pyutiles"
+version = "0.0.2"
 edition = "2021"
 include = ["src/**/*", "Cargo.toml", "LICENSE", "README.md"]
-
+license = "MIT OR Apache-2.0"
 
 [[bin]]
 name = "utiles"
 
 [lib]
 name = "libutiles"
 crate-type = ["cdylib"]
 
 [dependencies]
 fast_hilbert = "2.0.0"
 geo-types = "0.7.9"
 pyo3 = "0.18.3"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0.96"
+utiles = { path = "../../local_dependencies/utiles" }
 
 [profile.dev]
 opt-level = 0
 
 [profile.release]
 opt-level = 3
 strip = true
 
-[dev-dependencies]
-pyo3 = { version = "0.18.3", features = ["auto-initialize"] }
-
 [build-dependencies]
 pyo3-build-config = "0.18.3"
```

### Comparing `utiles-0.0.1/rust_src/utiles/Cargo.lock` & `utiles-0.0.2/rust_src/utiles/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -36,52 +36,52 @@
 checksum = "f8ec2bbe15af87954c739e236021f4411766c0f2b9c4a5f0b9317bcf6048ebf8"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "geo-types"
-version = "0.7.9"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5f0b3068e1537a4b861ec3734f4aa9c317d537cf0845bf6fb6221973499d26c"
+checksum = "9705398c5c7b26132e74513f4ee7c1d7dafd786004991b375c172be2be0eecaa"
 dependencies = [
  "approx",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -90,56 +90,56 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -197,190 +197,192 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "pyutiles"
+version = "0.0.2"
+dependencies = [
+ "fast_hilbert",
+ "geo-types",
+ "pyo3",
+ "pyo3-build-config",
+ "serde",
+ "serde_json",
+ "utiles",
+]
+
+[[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.181"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "6d3e73c93c3240c0bda063c239298e633114c69a888c3e37ca8bb33f343e9890"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.181"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "be02f6cb0cd3a5ec20bbcfbcbd749f57daddb1a0882dc2e46a6c236c90b977ed"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.104"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "076066c5f1078eac5b722a31827a8832fe108bed65dfa75e233c89f8206e976c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "04361975b3f5e348b2189d8dc55bc942f278b2d482a6a0365de5bdd62d351567"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "utiles"
 version = "0.0.1"
 dependencies = [
  "fast_hilbert",
  "geo-types",
- "pyo3",
- "pyo3-build-config",
  "serde",
  "serde_json",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `utiles-0.0.1/rust_src/utiles/README.md` & `utiles-0.0.2/rust_src/utiles/README.md`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/lib.rs` & `utiles-0.0.2/rust_src/utiles/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::collections::{HashMap, HashSet};
 
-use crate::utiles::BBox;
+use utiles::BBox;
 
 use pyo3::exceptions::{self, PyValueError};
 
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyTuple};
 use pyutiles::pybbox::PyBbox;
 use pyutiles::pyiters::CoordinateIterator;
@@ -13,15 +13,15 @@
 use pyutiles::pytile::PyTile;
 
 use utiles::zoom::ZoomOrZooms;
 
 use utiles::libtiletype;
 
 mod pyutiles;
-mod utiles;
+// mod utiles;
 
 #[derive(FromPyObject)]
 pub struct TileTuple(u32, u32, u8);
 
 impl From<PyTile> for TileTuple {
     fn from(tile: PyTile) -> Self {
         Self(tile.xyz.x, tile.xyz.y, tile.xyz.z)
@@ -425,42 +425,73 @@
         }
     }
 }
 
 #[pyclass]
 struct TilesGenerator {
     iter: Box<dyn Iterator<Item = PyTile> + Send>,
+    length: u64,
 }
 
 #[pymethods]
 impl TilesGenerator {
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
+
     fn __next__(mut slf: PyRefMut<'_, Self>) -> Option<PyTile> {
         slf.iter.next()
     }
+
+    fn __len__(slf: PyRefMut<'_, Self>) -> PyResult<usize> {
+        Ok(slf.length as usize)
+    }
+}
+
+#[pyfunction]
+fn tiles_count(
+    west: f64,
+    south: f64,
+    east: f64,
+    north: f64,
+    zooms: PyZoomOrZooms,
+    truncate: Option<bool>,
+) -> u64 {
+    let (west, south, east, north) =
+        utiles::bbox_truncate(west, south, east, north, truncate);
+
+    utiles::tiles_count((west, south, east, north), ZoomOrZooms::from(zooms))
 }
 
 #[pyfunction]
 fn tiles(
     west: f64,
     south: f64,
     east: f64,
     north: f64,
     zooms: PyZoomOrZooms,
     truncate: Option<bool>,
 ) -> TilesGenerator {
     let (west, south, east, north) =
         utiles::bbox_truncate(west, south, east, north, truncate);
-
-    let xyzs = utiles::tiles((west, south, east, north), ZoomOrZooms::from(zooms))
-        .map(PyTile::from);
+    let zooms_vec = match zooms {
+        PyZoomOrZooms::Zoom(z) => vec![z],
+        PyZoomOrZooms::Zooms(zs) => zs,
+    };
+    let zooms_vec_iter = zooms_vec.clone();
+    let ntiles =
+        utiles::tiles_count((west, south, east, north), ZoomOrZooms::from(zooms_vec));
+    let xyzs = utiles::tiles(
+        (west, south, east, north),
+        ZoomOrZooms::from(zooms_vec_iter),
+    )
+    .map(PyTile::from);
     TilesGenerator {
         iter: Box::new(xyzs),
+        length: ntiles,
     }
 }
 
 #[pyfunction]
 fn tiles_list(
     west: f64,
     south: f64,
@@ -666,25 +697,25 @@
             let coordsvec = coordsvec.iter.map(|(lng, lat)| (lng, lat)).collect();
             Ok(coordsvec)
         }
         Err(e) => Err(e),
     }
 }
 
-impl Iterator for utiles::LngLat {
-    type Item = (f64, f64);
+// impl Iterator for utiles::LngLat {
+//     type Item = (f64, f64);
 
-    fn next(&mut self) -> Option<Self::Item> {
-        let lng = self.xy.x;
-        let lat = self.xy.y;
-        self.xy.x += 1.0;
-        self.xy.y += 1.0;
-        Some((lng, lat))
-    }
-}
+//     fn next(&mut self) -> Option<Self::Item> {
+//         let lng = self.xy.x;
+//         let lat = self.xy.y;
+//         self.xy.x += 1.0;
+//         self.xy.y += 1.0;
+//         Some((lng, lat))
+//     }
+// }
 
 #[pyfunction]
 fn geojson_bounds(py: Python, obj: &PyAny) -> PyResult<PyLngLatBbox> {
     let coordsvec = _coords(py, obj);
     match coordsvec {
         Ok(coordsvec) => {
             let coordsvec: Vec<(f64, f64)> =
@@ -756,14 +787,15 @@
     m.add_function(wrap_pyfunction!(coords, m)?)?;
     // m.add_function(wrap_pyfunction!(merge, m)?)?;
     m.add_function(wrap_pyfunction!(simplify, m)?)?;
     m.add_function(wrap_pyfunction!(geojson_bounds, m)?)?;
     m.add_function(wrap_pyfunction!(feature, m)?)?;
 
     // utiles functions
+    m.add_function(wrap_pyfunction!(tiles_count, m)?)?;
     m.add_function(wrap_pyfunction!(tiles_list, m)?)?;
     m.add_function(wrap_pyfunction!(xyz, m)?)?;
     m.add_function(wrap_pyfunction!(parse_tiles, m)?)?;
     m.add_function(wrap_pyfunction!(xyz2quadkey, m)?)?;
     m.add_function(wrap_pyfunction!(quadkey2xyz, m)?)?;
     m.add_function(wrap_pyfunction!(from_tuple, m)?)?;
     m.add_function(wrap_pyfunction!(pmtileid, m)?)?;
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/purgatory/_coords.rs` & `utiles-0.0.2/rust_src/utiles/src/purgatory/_coords.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/pybbox.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/pybbox.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use crate::pyutiles::pytile::PyTile;
-use crate::utiles;
-use crate::utiles::BBox;
 use pyo3::basic::CompareOp;
 use pyo3::types::PyType;
 use pyo3::{
     exceptions, pyclass, pymethods, IntoPy, PyAny, PyErr, PyObject, PyRef, PyResult,
     Python,
 };
+use utiles;
+use utiles::BBox;
 
 #[pyclass(name = "Bbox")]
 #[derive(Clone)]
 pub struct PyBbox {
     pub bbox: BBox,
 }
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/pyiters.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/pyiters.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/pylnglat.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/pylnglat.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::pyutiles::pytile::PyTile;
-use crate::utiles;
 use pyo3::class::basic::CompareOp;
 use pyo3::exceptions::{self};
 use pyo3::prelude::*;
 use pyo3::types::PyType;
+use utiles;
 
 #[pyclass(name = "LngLat")]
 pub struct PyLngLat {
     lnglat: utiles::LngLat,
 }
 
 #[pymethods]
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/pylnglatbbox.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/pylnglatbbox.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use crate::pyutiles::pyiters::FloatIterator;
 use crate::pyutiles::pytile::PyTile;
-use crate::utiles;
-use crate::utiles::BBox;
 use pyo3::basic::CompareOp;
 use pyo3::types::PyType;
 use pyo3::{
     exceptions, pyclass, pymethods, IntoPy, Py, PyAny, PyErr, PyObject, PyRef,
     PyResult, Python,
 };
+use utiles;
+use utiles::BBox;
 
 #[pyclass(name = "LngLatBbox")]
 #[derive(Clone)]
 pub struct PyLngLatBbox {
     pub bbox: BBox,
 }
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/pytile.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/pytile.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use pyo3::prelude::*;
 use std::collections::HashMap;
 
 use crate::pyutiles::pyiters::IntIterator;
 use crate::pyutiles::tuple_slice;
-use crate::utiles::{BBox, Tile};
+use crate::TileTuple;
+use utiles::{BBox, Tile};
+
+use utiles;
 
-use crate::{utiles, TileTuple};
 use pyo3::basic::CompareOp;
 use pyo3::types::PyType;
 
 use pyo3::exceptions::PyValueError;
 use pyo3::{
     exceptions, pyclass, pymethods, IntoPy, Py, PyAny, PyErr, PyObject, PyRef,
     PyResult, Python,
@@ -24,15 +26,15 @@
 /// `PyTile` macro to create a new tile.
 ///  - do you need this? probably not
 ///  - Did I write to to figure out how to write a macro? yes
 #[macro_export]
 macro_rules! pytile {
     ($x:expr, $y:expr, $z:expr) => {
         PyTile {
-            xyz: utile!($x, $y, $z),
+            xyz: utiles::utile!($x, $y, $z),
         }
     };
 }
 
 #[pyclass(name = "Tile", sequence)]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize, Eq, Hash, Copy)]
 pub struct PyTile {
@@ -86,20 +88,20 @@
             iter: Box::new(
                 vec![slf.xyz.x, slf.xyz.y, u32::from(slf.xyz.z)].into_iter(),
             ),
         };
         Py::new(slf.py(), iter)
     }
 
-    pub fn fmt_zxy(&self) -> String {
-        self.xyz.fmt_zxy()
+    pub fn fmt_zxy(&self, sep: Option<&str>) -> String {
+        self.xyz.fmt_zxy(sep)
     }
 
-    pub fn fmt_zxy_ext(&self, ext: &str) -> String {
-        self.xyz.fmt_zxy_ext(ext)
+    pub fn fmt_zxy_ext(&self, ext: &str, sep: Option<&str>) -> String {
+        self.xyz.fmt_zxy_ext(ext, sep)
     }
 
     #[classmethod]
     pub fn from_quadkey(_cls: &PyType, quadkey: String) -> PyResult<Self> {
         let xyz = Tile::from_quadkey(&quadkey);
         match xyz {
             Ok(xyz) => Ok(PyTile::from(xyz)),
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/pyutiles/tuple_slice.rs` & `utiles-0.0.2/rust_src/utiles/src/pyutiles/tuple_slice.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/utiles/libtiletype.rs` & `utiles-0.0.2/local_dependencies/utiles/src/libtiletype.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/utiles/mod.rs` & `utiles-0.0.2/local_dependencies/utiles/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -810,20 +810,28 @@
     }
 
     pub fn from_pmtileid(id: u64) -> Self {
         let (x, y, z) = pmtiles::id2xyz(id);
         Tile::new(x, y, z)
     }
 
-    pub fn fmt_zxy(&self) -> String {
-        format!("{}/{}/{}", self.z, self.x, self.y)
+    pub fn fmt_zxy(&self, sep: Option<&str>) -> String {
+        match sep {
+            Some(sep) => format!("{}{}{}{}{}", self.z, sep, self.x, sep, self.y),
+            None => format!("{}/{}/{}", self.z, self.x, self.y),
+        }
     }
 
-    pub fn fmt_zxy_ext(&self, ext: &str) -> String {
-        format!("{}/{}/{}.{}", self.z, self.x, self.y, ext)
+    pub fn fmt_zxy_ext(&self, ext: &str, sep: Option<&str>) -> String {
+        match sep {
+            Some(sep) => {
+                format!("{}{}{}{}{}.{}", self.z, sep, self.x, sep, self.y, ext)
+            }
+            None => format!("{}/{}/{}.{}", self.z, self.x, self.y, ext),
+        }
     }
 
     pub fn parent_id(&self) -> u64 {
         pmtiles::parent_id(self.pmtileid())
     }
 
     pub fn from_quadkey(quadkey: &str) -> Result<Tile, Box<dyn Error>> {
@@ -1027,25 +1035,59 @@
         ZoomOrZooms::Zoom(zoom) => {
             vec![zoom]
         }
         ZoomOrZooms::Zooms(zooms) => zooms,
     }
 }
 
-pub struct TilesRange {
+pub struct TileRange {
     curx: u32,
     cury: u32,
-    pub minx: u32,
-    pub maxx: u32,
-    pub miny: u32,
-    pub maxy: u32,
-    pub zoom: u8,
+    minx: u32,
+    maxx: u32,
+    miny: u32,
+    maxy: u32,
+    zoom: u8,
 }
 
-impl Iterator for TilesRange {
+impl TileRange {
+    pub fn new(minx: u32, maxx: u32, miny: u32, maxy: u32, zoom: u8) -> Self {
+        Self {
+            curx: minx,
+            cury: miny,
+            minx,
+            maxx,
+            miny,
+            maxy,
+            zoom,
+        }
+    }
+
+    pub fn minx(&self) -> u32 {
+        self.minx
+    }
+    pub fn maxx(&self) -> u32 {
+        self.maxx
+    }
+    pub fn miny(&self) -> u32 {
+        self.miny
+    }
+    pub fn maxy(&self) -> u32 {
+        self.maxy
+    }
+    pub fn zoom(&self) -> u8 {
+        self.zoom
+    }
+
+    pub fn length(&self) -> u64 {
+        ((self.maxx - self.minx + 1) * (self.maxy - self.miny + 1)) as u64
+    }
+}
+
+impl Iterator for TileRange {
     type Item = (u32, u32, u8);
 
     fn next(&mut self) -> Option<Self::Item> {
         if self.curx > self.maxx {
             self.curx = self.minx;
             self.cury += 1;
         }
@@ -1059,19 +1101,45 @@
 
     fn size_hint(&self) -> (usize, Option<usize>) {
         let size = ((self.maxx - self.minx + 1) * (self.maxy - self.miny + 1)) as usize;
         (size, Some(size))
     }
 }
 
-pub struct TilesRanges {
-    ranges: Vec<TilesRange>,
+pub struct TileRanges {
+    ranges: Vec<TileRange>,
+}
+
+impl TileRanges {
+    pub fn new(minx: u32, maxx: u32, miny: u32, maxy: u32, zoom: u8) -> Self {
+        Self {
+            ranges: vec![TileRange::new(minx, maxx, miny, maxy, zoom)],
+        }
+    }
+
+    pub fn length(&self) -> u64 {
+        self.ranges.iter().map(|r| r.length()).sum()
+    }
+}
+
+impl From<TileRange> for TileRanges {
+    fn from(range: TileRange) -> Self {
+        Self {
+            ranges: vec![range],
+        }
+    }
+}
+
+impl From<Vec<TileRange>> for TileRanges {
+    fn from(ranges: Vec<TileRange>) -> Self {
+        Self { ranges }
+    }
 }
 
-impl Iterator for TilesRanges {
+impl Iterator for TileRanges {
     type Item = (u32, u32, u8);
 
     fn next(&mut self) -> Option<Self::Item> {
         if self.ranges.is_empty() {
             return None;
         }
         let mut range = self.ranges.remove(0);
@@ -1133,14 +1201,77 @@
 //     let minx = (minx * z2).floor() as i32;
 //     let miny = (miny * z2).floor() as i32;
 //     let maxx = (maxx * z2).floor() as i32;
 //     let maxy = (maxy * z2).floor() as i32;
 //     (minx, miny, maxx, maxy)
 // }
 
+pub fn tile_ranges(bounds: (f64, f64, f64, f64), zooms: ZoomOrZooms) -> TileRanges {
+    let zooms = as_zooms(zooms);
+    let bboxthing = BBox {
+        north: bounds.3,
+        south: bounds.1,
+        east: bounds.2,
+        west: bounds.0,
+    };
+    let bboxes: Vec<BBox> = bboxthing
+        .bboxes()
+        .into_iter()
+        .map(|bbox| {
+            // clip to web mercator extent
+            BBox {
+                north: bbox.north.min(85.051_129),
+                south: bbox.south.max(-85.051_129),
+                east: bbox.east.min(180.0),
+                west: bbox.west.max(-180.0),
+            }
+        })
+        .collect();
+    let ranges: Vec<TileRange> = bboxes
+        .into_iter()
+        .flat_map(move |bbox| {
+            let zooms = zooms.clone();
+            zooms.into_iter().map(move |zoom| {
+                let upper_left_lnglat = LngLat {
+                    xy: coord! { x: bbox.west, y: bbox.north },
+                };
+                let lower_right_lnglat = LngLat {
+                    xy: coord! { x: bbox.east, y: bbox.south },
+                };
+                let top_left_tile = Tile::from_lnglat_zoom(
+                    upper_left_lnglat.lng(),
+                    upper_left_lnglat.lat(),
+                    zoom,
+                    Some(false),
+                );
+                let bottom_right_tile = Tile::from_lnglat_zoom(
+                    lower_right_lnglat.lng() - LL_EPSILON,
+                    lower_right_lnglat.lat() + LL_EPSILON,
+                    zoom,
+                    Some(false),
+                );
+                TileRange::new(
+                    top_left_tile.x,
+                    bottom_right_tile.x,
+                    top_left_tile.y,
+                    bottom_right_tile.y,
+                    zoom,
+                )
+            })
+        })
+        .collect();
+
+    TileRanges::from(ranges)
+}
+
+pub fn tiles_count(bounds: (f64, f64, f64, f64), zooms: ZoomOrZooms) -> u64 {
+    let ranges = tile_ranges(bounds, zooms);
+    ranges.length()
+}
+
 pub fn tiles(
     bounds: (f64, f64, f64, f64),
     zooms: ZoomOrZooms,
 ) -> impl Iterator<Item = Tile> {
     let zooms = as_zooms(zooms);
     let bboxthing = BBox {
         north: bounds.3,
@@ -1247,14 +1378,26 @@
         let (new_set, changed) = merge(&root_set);
         root_set = new_set;
         is_merging = changed;
     }
     root_set
 }
 
+impl Iterator for LngLat {
+    type Item = (f64, f64);
+
+    fn next(&mut self) -> Option<Self::Item> {
+        let lng = self.xy.x;
+        let lat = self.xy.y;
+        self.xy.x += 1.0;
+        self.xy.y += 1.0;
+        Some((lng, lat))
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn zoom_or_zooms() {
         let z = as_zooms(1.into());
@@ -1273,14 +1416,17 @@
 
     #[test]
     fn tiles_single_zoom() {
         let bounds = (-105.0, 39.99, -104.99, 40.0);
         let tiles = tiles(bounds, 14.into());
         let expect = vec![Tile::new(3413, 6202, 14), Tile::new(3413, 6203, 14)];
         assert_eq!(tiles.collect::<Vec<Tile>>(), expect);
+
+        let ntiles = tiles_count(bounds, 14.into());
+        assert_eq!(ntiles, 2);
     }
 
     #[test]
     fn tiles_anti_meridian() {
         let bounds = (175.0, 5.0, -175.0, 10.0);
         let mut tiles: Vec<Tile> = tiles(bounds, 2.into()).collect();
         tiles.sort();
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/utiles/pmtiles.rs` & `utiles-0.0.2/local_dependencies/utiles/src/pmtiles.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/rust_src/utiles/src/utiles/sibling_relationship.rs` & `utiles-0.0.2/local_dependencies/utiles/src/sibling_relationship.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::utiles::Tile;
+use crate::Tile;
 
 pub enum SiblingRelationship {
     UpperLeft = 0,
     UpperRight = 1,
     LowerLeft = 2,
     LowerRight = 3,
 }
```

### Comparing `utiles-0.0.1/rust_src/utiles/src/utiles/traits.rs` & `utiles-0.0.2/local_dependencies/utiles/src/traits.rs`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/Cargo.lock` & `utiles-0.0.2/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -36,52 +36,52 @@
 checksum = "f8ec2bbe15af87954c739e236021f4411766c0f2b9c4a5f0b9317bcf6048ebf8"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "geo-types"
-version = "0.7.9"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5f0b3068e1537a4b861ec3734f4aa9c317d537cf0845bf6fb6221973499d26c"
+checksum = "9705398c5c7b26132e74513f4ee7c1d7dafd786004991b375c172be2be0eecaa"
 dependencies = [
  "approx",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -90,56 +90,56 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -197,190 +197,192 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "pyutiles"
+version = "0.0.2"
+dependencies = [
+ "fast_hilbert",
+ "geo-types",
+ "pyo3",
+ "pyo3-build-config",
+ "serde",
+ "serde_json",
+ "utiles",
+]
+
+[[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.181"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "6d3e73c93c3240c0bda063c239298e633114c69a888c3e37ca8bb33f343e9890"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.181"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "be02f6cb0cd3a5ec20bbcfbcbd749f57daddb1a0882dc2e46a6c236c90b977ed"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.28",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.104"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "076066c5f1078eac5b722a31827a8832fe108bed65dfa75e233c89f8206e976c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "04361975b3f5e348b2189d8dc55bc942f278b2d482a6a0365de5bdd62d351567"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "utiles"
 version = "0.0.1"
 dependencies = [
  "fast_hilbert",
  "geo-types",
- "pyo3",
- "pyo3-build-config",
  "serde",
  "serde_json",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `utiles-0.0.1/python/utiles/cli.py` & `utiles-0.0.2/python/utiles/cli.py`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/python/utiles/__init__.py` & `utiles-0.0.2/python/utiles/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     "pmtileid",
     "quadkey",
     "quadkey2xyz",
     "quadkey_to_tile",
     "simplify",
     "tile",
     "tiles",
+    "tiles_count",
     "tiles_list",
     "tiletype",
     "tiletype2headers",
     "tiletype_str",
     "truncate_lnglat",
     "ul",
     "xy",
```

### Comparing `utiles-0.0.1/python/utiles/__main__.py` & `utiles-0.0.2/python/utiles/__main__.py`

 * *Files identical despite different names*

### Comparing `utiles-0.0.1/python/utiles/libutiles.pyi` & `utiles-0.0.2/python/utiles/libutiles.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import (
     Any,
+    Collection,
     Iterable,
     Iterator,
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
@@ -123,14 +124,18 @@
     def neighbors(self) -> list[Tile]: ...
     def parent(self) -> Tile: ...
     def siblings(self) -> list[Tile]: ...
     def ul(self) -> LngLat: ...
     def ur(self) -> LngLat: ...
     def __eq__(self, other: Any) -> bool: ...
     def __ge__(self, other: Tile | tuple[int, int, int]) -> bool: ...
+    def qk(self) -> str: ...
+    def quadkey(self) -> str: ...
+    def fmt_zxy(self, sep: str | None) -> str: ...
+    def fmt_zxy_ext(self, ext: str, sep: str | None) -> str: ...
     # def __getitem__(self, index: int) -> bool: ...
 
     @overload
     def __getitem__(self, index: int) -> int: ...
     @overload
     def __getitem__(self, index: slice) -> tuple[int, ...]: ...
     def __gt__(self, other: Tile) -> bool: ...
@@ -188,15 +193,15 @@
 def tiles(
     west: float,
     south: float,
     east: float,
     north: float,
     zooms: list[int] | tuple[int, ...] | int,
     truncate: bool = ...,
-) -> Iterable[Tile]: ...
+) -> Collection[Tile]: ...
 def tiles_list(
     west: float,
     south: float,
     east: float,
     north: float,
     zooms: list[int] | tuple[int, ...] | int,
     truncate: bool = ...,
```

### Comparing `utiles-0.0.1/PKG-INFO` & `utiles-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: utiles
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: click>=7.1.2
 Summary: utiles = (utils + tiles) * rust
 Author-email: Jesse Rubin <jessekrubin@gmail.com>
 Maintainer-email: Jesse Rubin <jessekrubin@gmail.com>
+License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # utiles
 
 utiles = utils + tiles
```

