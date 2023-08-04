# Comparing `tmp/openprotein_python-0.1.1b8.tar.gz` & `tmp/openprotein_python-0.1.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.1.1b8.tar", max compression
+gzip compressed data, was "openprotein_python-0.1.1b9.tar", max compression
```

## Comparing `openprotein_python-0.1.1b8.tar` & `openprotein_python-0.1.1b9.tar`

### file list

```diff
@@ -1,27 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b8/LICENSE.txt
--rw-r--r--   0        0        0     2925 2023-08-04 03:37:46.856592 openprotein_python-0.1.1b8/README.md
--rw-r--r--   0        0        0     2101 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/__init__.py
--rw-r--r--   0        0        0      120 2023-08-04 06:46:01.435537 openprotein_python-0.1.1b8/openprotein_python/_version.py
--rw-r--r--   0        0        0      127 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/__init__.py
--rw-r--r--   0        0        0      337 2023-08-04 06:44:47.298834 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13440 2023-08-04 06:44:47.298834 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     9314 2023-08-04 06:44:47.738838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/design.cpython-38.pyc
--rw-r--r--   0        0        0    23908 2023-08-04 06:44:47.750838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/embedding.cpython-38.pyc
--rw-r--r--   0        0        0    14445 2023-08-04 06:44:47.706838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/jobs.cpython-38.pyc
--rw-r--r--   0        0        0    39618 2023-08-04 06:44:47.750838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/poet.cpython-38.pyc
--rw-r--r--   0        0        0    16779 2023-08-04 06:44:47.742838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/predict.cpython-38.pyc
--rw-r--r--   0        0        0    18101 2023-08-04 06:44:47.742838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/train.cpython-38.pyc
--rw-r--r--   0        0        0    13265 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/data.py
--rw-r--r--   0        0        0     8575 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/design.py
--rw-r--r--   0        0        0    22251 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/embedding.py
--rw-r--r--   0        0        0    14423 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/jobs.py
--rw-r--r--   0        0        0    41938 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/poet.py
--rw-r--r--   0        0        0    17793 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/predict.py
--rw-r--r--   0        0        0    19488 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/train.py
--rw-r--r--   0        0        0     3083 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/base.py
--rw-r--r--   0        0        0      170 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/config.py
--rw-r--r--   0        0        0     1146 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/fasta.py
--rw-r--r--   0        0        0     8636 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/models.py
--rw-r--r--   0        0        0      558 2023-08-04 06:45:54.967476 openprotein_python-0.1.1b8/pyproject.toml
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     3137 2023-08-04 07:23:14.064735 openprotein_python-0.1.1b9/README.md
+-rw-r--r--   0        0        0     2038 2023-08-04 07:48:08.230937 openprotein_python-0.1.1b9/openprotein/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-04 07:45:18.805327 openprotein_python-0.1.1b9/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b9/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-04 07:48:16.095012 openprotein_python-0.1.1b9/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-04 07:48:18.115031 openprotein_python-0.1.1b9/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-04 07:48:20.099050 openprotein_python-0.1.1b9/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14402 2023-08-04 07:48:21.987068 openprotein_python-0.1.1b9/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41896 2023-08-04 07:48:24.079088 openprotein_python-0.1.1b9/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-04 07:48:26.059107 openprotein_python-0.1.1b9/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-04 07:48:28.387129 openprotein_python-0.1.1b9/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-04 07:48:10.634960 openprotein_python-0.1.1b9/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b9/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b9/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b9/openprotein/fasta.py
+-rw-r--r--   0        0        0     8629 2023-08-04 07:48:12.450977 openprotein_python-0.1.1b9/openprotein/models.py
+-rw-r--r--   0        0        0      604 2023-08-04 07:47:38.574655 openprotein_python-0.1.1b9/pyproject.toml
+-rw-r--r--   0        0        0     3967 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b9/PKG-INFO
```

### Comparing `openprotein_python-0.1.1b8/LICENSE.txt` & `openprotein_python-0.1.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b8/README.md` & `openprotein_python-0.1.1b9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+[![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
+[![Coverage](./apidocs/source/coverage.svg)](https://pypi.org/project/openprotein-python/)
+
 # openprotein-python
 Python interface for the OpenProtein.AI REST API.
 
 ## Installation 
 
 You can install with pip: 
 
 ```
 pip install openprotein_python
 ```
 ## Getting started
 
 First, create a session using your login credentials.
 ```
-import openprotein
+import openprotein_python
 session = openprotein.connect(USERNAME, PASSWORD)
 ```
 
 Async calls return `AsyncJobFuture` objects that allow tracking the status of the job and retrieving the result when it's ready.
 
 Given a future, check its status and retrieve results
 ```
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/__init__.py` & `openprotein_python-0.1.1b9/openprotein/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from openprotein_python._version import __version__
+from openprotein._version import __version__
 
-from openprotein_python.base import APISession
-from openprotein_python.api.jobs import JobsAPI, Job
-from openprotein_python.api.data import DataAPI
-from openprotein_python.api.poet import PoetAPI
-from openprotein_python.api.embedding import EmbeddingAPI
-from openprotein_python.api.train import TrainingAPI
-from openprotein_python.api.design import DesignAPI
-from openprotein_python.api.predict import PredictAPI
+from openprotein.base import APISession
+from openprotein.api.jobs import JobsAPI, Job
+from openprotein.api.data import DataAPI
+from openprotein.api.poet import PoetAPI
+from openprotein.api.embedding import EmbeddingAPI
+from openprotein.api.train import TrainingAPI
+from openprotein.api.design import DesignAPI
+from openprotein.api.predict import PredictAPI
 class OpenProtein(APISession):
     """
     The base class for accessing OpenProtein API functionality.
     """
 
     def wait(self, job: Job, *args, **kwargs):
         return job.wait(self, *args, **kwargs)
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/train.cpython-38.pyc` & `openprotein_python-0.1.1b9/openprotein/api/train.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1132 +1,1216 @@
-00000000: 550d 0d0a 0000 0000 549e cc64 204c 0000  U.......T..d L..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 d601 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 0100 6400 6402 6c04 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
-00000080: 6406 6c0f 6d10 5a10 6d11 5a11 6d12 5a12  d.l.m.Z.m.Z.m.Z.
-00000090: 0100 6400 6407 6c13 6d14 5a14 6d15 5a15  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 6506 6516 6502 6408 9c03 6409 640a  ..e.e.e.d...d.d.
-000000b0: 8404 5a17 642c 6506 6516 6518 6509 640c  ..Z.d,e.e.e.e.d.
-000000c0: 9c04 640d 640e 8405 5a19 642d 6506 6516  ..d.d...Z.d-e.e.
-000000d0: 6501 6518 1900 6501 6518 1900 650e 640f  e.e...e.e...e.d.
-000000e0: 9c05 6410 6411 8405 5a1a 642e 6506 6516  ..d.d...Z.d.e.e.
-000000f0: 6514 6503 6516 6502 6516 1900 6602 1900  e.e.e.e.e...f...
-00000100: 6516 6501 651b 1900 650d 6414 9c07 6415  e.e.e...e.d...d.
-00000110: 6416 8405 5a1c 642f 6506 6514 6503 6516  d...Z.d/e.e.e.e.
-00000120: 6502 6516 1900 6602 1900 6516 6501 651b  e.e...f...e.e.e.
-00000130: 1900 6417 9c05 6418 6419 8405 5a1d 6430  ..d...d.d...Z.d0
-00000140: 6506 6514 6503 6516 6502 6516 1900 6602  e.e.e.e.e.e...f.
-00000150: 1900 6516 6501 651b 1900 6417 9c05 641a  ..e.e.e...d...d.
-00000160: 641b 8405 5a1e 6431 6506 6514 6503 6516  d...Z.d1e.e.e.e.
-00000170: 6502 6516 1900 6602 1900 6516 6501 651b  e.e...f...e.e.e.
-00000180: 1900 6417 9c05 641c 641d 8405 5a1f 6506  ..d...d.d...Z.e.
-00000190: 6516 650b 6408 9c03 641e 641f 8404 5a20  e.e.d...d.d...Z 
-000001a0: 6506 6516 650d 6408 9c03 6420 6421 8404  e.e.e.d...d d!..
-000001b0: 5a21 4700 6422 6423 8400 6423 8302 5a22  Z!G.d"d#..d#..Z"
-000001c0: 4700 6424 6425 8400 6425 6522 6508 8304  G.d$d%..d%e"e...
-000001d0: 5a23 4700 6426 6427 8400 6427 8302 5a24  Z#G.d&d'..d'..Z$
-000001e0: 4700 6428 6429 8400 6429 6524 6508 8304  G.d(d)..d)e$e...
-000001f0: 5a25 4700 642a 642b 8400 642b 8302 5a26  Z%G.d*d+..d+..Z&
-00000200: 6402 5300 2932 e900 0000 0029 03da 084f  d.S.)2.....)...O
-00000210: 7074 696f 6e61 6cda 044c 6973 74da 0555  ptional..List..U
-00000220: 6e69 6f6e 4e29 01da 0a41 5049 5365 7373  nionN)...APISess
-00000230: 696f 6e29 02da 0e41 7379 6e63 4a6f 6246  ion)...AsyncJobF
-00000240: 7574 7572 65da 034a 6f62 2904 da0a 5472  uture..Job)...Tr
-00000250: 6169 6e47 7261 7068 da07 4a6f 6254 7970  ainGraph..JobTyp
-00000260: 65da 074a 6f62 706c 7573 da09 4356 5265  e..Jobplus..CVRe
-00000270: 7375 6c74 7329 03da 1549 6e76 616c 6964  sults)...Invalid
-00000280: 5061 7261 6d65 7465 7245 7272 6f72 da08  ParameterError..
-00000290: 4150 4945 7272 6f72 da0a 496e 7661 6c69  APIError..Invali
-000002a0: 644a 6f62 2902 da0c 4173 7361 7944 6174  dJob)...AssayDat
-000002b0: 6173 6574 da0d 4173 7361 794d 6574 6164  aset..AssayMetad
-000002c0: 6174 6129 03da 0773 6573 7369 6f6e da06  ata)...session..
-000002d0: 6a6f 625f 6964 da06 7265 7475 726e 6302  job_id..returnc.
-000002e0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000002f0: 0000 0043 0000 0073 1e00 0000 6401 7d02  ...C...s....d.}.
-00000300: 7c00 6a00 7c02 6402 7c01 6901 6403 8d02  |.j.|.d.|.i.d...
-00000310: 7d03 7c03 a001 a100 5300 2904 7ae8 0a20  }.|.....S.).z.. 
-00000320: 2020 204c 6973 7420 6d6f 6465 6c73 2061     List models a
-00000330: 7373 6f69 6361 7465 6420 7769 7468 206a  ssoicated with j
-00000340: 6f62 0a0a 2020 2020 5061 7261 6d65 7465  ob..    Paramete
-00000350: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00000360: 2d0a 2020 2020 7365 7373 696f 6e20 3a20  -.    session : 
-00000370: 4150 4953 6573 7369 6f6e 0a20 2020 2020  APISession.     
-00000380: 2020 2053 6573 7369 6f6e 206f 626a 6563     Session objec
-00000390: 7420 666f 7220 4150 4920 636f 6d6d 756e  t for API commun
-000003a0: 6963 6174 696f 6e2e 0a20 2020 206a 6f62  ication..    job
-000003b0: 5f69 6420 3a20 7374 720a 2020 2020 2020  _id : str.      
-000003c0: 2020 6a6f 6220 4944 0a0a 2020 2020 5265    job ID..    Re
-000003d0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-000003e0: 2d0a 2020 2020 4c69 7374 0a20 2020 2020  -.    List.     
-000003f0: 2020 204c 6973 7420 6f66 206d 6f64 656c     List of model
-00000400: 730a 2020 2020 7a09 7631 2f6d 6f64 656c  s.    z.v1/model
-00000410: 7372 1200 0000 a901 da06 7061 7261 6d73  sr........params
-00000420: 2902 da03 6765 74da 046a 736f 6ea9 0472  )...get..json..r
-00000430: 1100 0000 7212 0000 00da 0865 6e64 706f  ....r......endpo
-00000440: 696e 74da 0872 6573 706f 6e73 65a9 0072  int..response..r
-00000450: 1b00 0000 fa44 2f68 6f6d 652f 7562 756e  .....D/home/ubun
-00000460: 7475 2f77 6f72 6b2f 6f70 656e 7072 6f74  tu/work/openprot
-00000470: 6569 6e2d 7079 7468 6f6e 2f6f 7065 6e70  ein-python/openp
-00000480: 726f 7465 696e 5f70 7974 686f 6e2f 6170  rotein_python/ap
-00000490: 692f 7472 6169 6e2e 7079 da0b 6c69 7374  i/train.py..list
-000004a0: 5f6d 6f64 656c 730b 0000 0073 0600 0000  _models....s....
-000004b0: 0010 0401 1201 721d 0000 00e9 0500 0000  ......r.........
-000004c0: 2904 7211 0000 00da 0c74 7261 696e 5f6a  ).r......train_j
-000004d0: 6f62 5f69 64da 086e 5f73 706c 6974 7372  ob_id..n_splitsr
-000004e0: 1300 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000004f0: 0005 0000 0005 0000 0043 0000 0073 2800  .........C...s(.
-00000500: 0000 6401 7d03 7c00 6a00 7c03 7c01 7c02  ..d.}.|.j.|.|.|.
-00000510: 6402 9c02 6403 8d02 7d04 7401 a002 7403  d...d...}.t...t.
-00000520: 7c04 a004 a100 a102 5300 2904 7ad7 0a20  |.......S.).z.. 
-00000530: 2020 2053 7562 6d69 7420 6120 6372 6f73     Submit a cros
-00000540: 732d 7661 6c69 6461 7469 6f6e 206a 6f62  s-validation job
-00000550: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00000560: 2020 2020 2073 6573 7369 6f6e 2028 4150       session (AP
-00000570: 4953 6573 7369 6f6e 293a 2061 7574 6820  ISession): auth 
-00000580: 7365 7373 696f 6e0a 2020 2020 2020 2020  session.        
-00000590: 6a6f 625f 6964 2028 7374 7229 3a20 6a6f  job_id (str): jo
-000005a0: 6220 6964 0a20 2020 2020 2020 206e 5f73  b id.        n_s
-000005b0: 706c 6974 7320 2869 6e74 2c20 6f70 7469  plits (int, opti
-000005c0: 6f6e 616c 293a 204e 206f 6620 4356 2073  onal): N of CV s
-000005d0: 706c 6974 732e 2044 6566 6175 6c74 7320  plits. Defaults 
-000005e0: 746f 2035 2e0a 0a20 2020 2052 6574 7572  to 5...    Retur
-000005f0: 6e73 3a0a 2020 2020 2020 2020 4a6f 623a  ns:.        Job:
-00000600: 0a20 2020 207a 1976 312f 776f 726b 666c  .    z.v1/workfl
-00000610: 6f77 2f63 726f 7373 7661 6c69 6461 7465  ow/crossvalidate
-00000620: 2902 721f 0000 0072 2000 0000 2901 7217  ).r....r ...).r.
-00000630: 0000 0029 05da 0470 6f73 74da 0870 7964  ...)...post..pyd
-00000640: 616e 7469 63da 0c70 6172 7365 5f6f 626a  antic..parse_obj
-00000650: 5f61 7372 0700 0000 7217 0000 0029 0572  _asr....r....).r
-00000660: 1100 0000 721f 0000 0072 2000 0000 7219  ....r....r ...r.
-00000670: 0000 0072 1a00 0000 721b 0000 0072 1b00  ...r....r....r..
-00000680: 0000 721c 0000 00da 0d63 726f 7373 7661  ..r......crossva
-00000690: 6c69 6461 7465 2000 0000 730c 0000 0000  lidate ...s.....
-000006a0: 0c04 0104 0102 0008 ff06 0372 2400 0000  ...........r$...
-000006b0: 2905 7211 0000 0072 1200 0000 da09 7061  ).r....r......pa
-000006c0: 6765 5f73 697a 65da 0b70 6167 655f 6f66  ge_size..page_of
-000006d0: 6673 6574 7213 0000 0063 0400 0000 0000  fsetr....c......
-000006e0: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
-000006f0: 0000 7344 0000 0064 017c 019b 009d 027d  ..sD...d.|.....}
-00000700: 047c 027c 0364 029c 027d 057c 006a 007c  .|.|.d...}.|.j.|
-00000710: 047c 0564 038d 027d 067c 066a 0164 046b  .|.d...}.|.j.d.k
-00000720: 0272 3474 0264 0583 0182 0174 03a0 0474  .r4t.d.....t...t
-00000730: 057c 06a0 06a1 00a1 0253 0029 067a 990a  .|.......S.).z..
-00000740: 2020 2020 4765 7420 4356 2072 6573 756c      Get CV resul
-00000750: 7473 0a0a 2020 2020 4172 6773 3a0a 2020  ts..    Args:.  
-00000760: 2020 2020 2020 7365 7373 696f 6e20 2841        session (A
-00000770: 5049 5365 7373 696f 6e29 3a20 6175 7468  PISession): auth
-00000780: 2764 2073 6573 7369 6f6e 0a20 2020 2020  'd session.     
-00000790: 2020 206a 6f62 5f69 6420 2873 7472 293a     job_id (str):
-000007a0: 204a 6f62 2069 640a 0a20 2020 2052 6574   Job id..    Ret
-000007b0: 7572 6e73 3a0a 2020 2020 2020 2020 5f74  urns:.        _t
-000007c0: 7970 655f 3a20 5f64 6573 6372 6970 7469  ype_: _descripti
-000007d0: 6f6e 5f0a 2020 2020 7a1a 7631 2f77 6f72  on_.    z.v1/wor
-000007e0: 6b66 6c6f 772f 6372 6f73 7376 616c 6964  kflow/crossvalid
-000007f0: 6174 652f a902 7225 0000 0072 2600 0000  ate/..r%...r&...
-00000800: 7214 0000 0069 9401 0000 7a2a 4e6f 2043  r....i....z*No C
-00000810: 5620 6a6f 6220 6861 7320 6265 656e 2073  V job has been s
-00000820: 7562 6d69 7474 6564 2066 6f72 2074 6869  ubmitted for thi
-00000830: 7320 6a6f 6221 2907 7216 0000 00da 0b73  s job!).r......s
-00000840: 7461 7475 735f 636f 6465 720e 0000 0072  tatus_coder....r
-00000850: 2200 0000 7223 0000 0072 0b00 0000 7217  "...r#...r....r.
-00000860: 0000 0029 0772 1100 0000 7212 0000 0072  ...).r....r....r
-00000870: 2500 0000 7226 0000 0072 1900 0000 7215  %...r&...r....r.
-00000880: 0000 0072 1a00 0000 721b 0000 0072 1b00  ...r....r....r..
-00000890: 0000 721c 0000 00da 1367 6574 5f63 726f  ..r......get_cro
-000008a0: 7373 7661 6c69 6461 7469 6f6e 3300 0000  ssvalidation3...
-000008b0: 730c 0000 0000 100a 010a 010e 010a 0108  s...............
-000008c0: 0172 2900 0000 da00 4629 0772 1100 0000  .r).....F).r....
-000008d0: 7219 0000 00da 0c61 7373 6179 6461 7461  r......assaydata
-000008e0: 7365 74da 106d 6561 7375 7265 6d65 6e74  set..measurement
-000008f0: 5f6e 616d 65da 0a6d 6f64 656c 5f6e 616d  _name..model_nam
-00000900: 65da 1066 6f72 6365 5f70 7265 7072 6f63  e..force_preproc
-00000910: 6573 7372 1300 0000 6306 0000 0000 0000  essr....c.......
-00000920: 0000 0000 000a 0000 0005 0000 0043 0000  .............C..
-00000930: 0073 ae00 0000 7400 7c02 7401 8302 7312  .s....t.|.t...s.
-00000940: 7402 6401 8301 8201 7400 7c03 7403 8302  t.d.....t.|.t...
-00000950: 7222 7c03 6701 7d03 7c03 4400 5d1e 7d06  r"|.g.}.|.D.].}.
-00000960: 7c06 7c02 6a04 6b07 7226 7402 6402 7c06  |.|.j.k.r&t.d.|.
-00000970: 9b00 6403 9d03 8301 8201 7126 7c02 6a05  ..d.......q&|.j.
-00000980: 6404 1900 6405 6b00 725c 7402 6406 8301  d...d.k.r\t.d...
-00000990: 8201 7c04 6407 6b08 7268 6408 7d04 7c02  ..|.d.k.rhd.}.|.
-000009a0: 6a06 7c03 7c04 6409 9c03 7d07 640a 7403  j.|.|.d...}.d.t.
-000009b0: 7c05 8301 a007 a100 6901 7d08 7c00 6a08  |.......i.}.|.j.
-000009c0: 7c01 7c08 7c07 640b 8d03 7d09 7c09 a009  |.|.|.d...}.|...
-000009d0: a100 0100 740a a00b 740c 7c09 a00d a100  ....t...t.|.....
-000009e0: a102 5300 290c e171 0400 000a 2020 2020  ..S.)..q....    
-000009f0: 4372 6561 7465 2061 2074 7261 696e 696e  Create a trainin
-00000a00: 6720 6a6f 622e 0a0a 2020 2020 5661 6c69  g job...    Vali
-00000a10: 6461 7465 2069 6e70 7574 732c 2066 6f72  date inputs, for
-00000a20: 6d61 7420 2064 6174 612c 2073 656e 6473  mat  data, sends
-00000a30: 2074 6865 206a 6f62 2074 7261 696e 696e   the job trainin
-00000a40: 6720 7265 7175 6573 7420 746f 2074 6865  g request to the
-00000a50: 2065 6e64 706f 696e 742c 0a0a 2020 2020   endpoint,..    
-00000a60: 5061 7273 6573 2074 6865 2072 6573 706f  Parses the respo
-00000a70: 6e73 6520 696e 746f 2061 2060 4a6f 6260  nse into a `Job`
-00000a80: 206f 626a 6563 742e 0a0a 2020 2020 5061   object...    Pa
-00000a90: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00000aa0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7365 7373  -------.    sess
-00000ab0: 696f 6e20 3a20 4150 4953 6573 7369 6f6e  ion : APISession
-00000ac0: 0a20 2020 2020 2020 2054 6865 2063 7572  .        The cur
-00000ad0: 7265 6e74 2041 5049 2073 6573 7369 6f6e  rent API session
-00000ae0: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-00000af0: 6f6e 2077 6974 6820 7468 6520 7365 7276  on with the serv
-00000b00: 6572 2e0a 2020 2020 656e 6470 6f69 6e74  er..    endpoint
-00000b10: 203a 2073 7472 0a20 2020 2020 2020 2054   : str.        T
-00000b20: 6865 2065 6e64 706f 696e 7420 746f 2077  he endpoint to w
-00000b30: 6869 6368 2074 6865 206a 6f62 2074 7261  hich the job tra
-00000b40: 696e 696e 6720 7265 7175 6573 7420 6973  ining request is
-00000b50: 2074 6f20 6265 2073 656e 742e 0a20 2020   to be sent..   
-00000b60: 2061 7373 6179 6461 7461 7365 7420 3a20   assaydataset : 
-00000b70: 4173 7361 7944 6174 6173 6574 0a20 2020  AssayDataset.   
-00000b80: 2020 2020 2041 6e20 4173 7361 7944 6174       An AssayDat
-00000b90: 6173 6574 206f 626a 6563 7420 6672 6f6d  aset object from
-00000ba0: 2077 6869 6368 2074 6865 2061 7373 6179   which the assay
-00000bb0: 5f69 6420 6973 2065 7874 7261 6374 6564  _id is extracted
-00000bc0: 2e0a 2020 2020 6d65 6173 7572 656d 656e  ..    measuremen
-00000bd0: 745f 6e61 6d65 203a 2073 7472 206f 7220  t_name : str or 
-00000be0: 4c69 7374 5b73 7472 5d0a 2020 2020 2020  List[str].      
-00000bf0: 2020 5468 6520 6e61 6d65 2873 2920 6f66    The name(s) of
-00000c00: 2074 6865 206d 6561 7375 7265 6d65 6e74   the measurement
-00000c10: 2873 2920 746f 2062 6520 7573 6564 2069  (s) to be used i
-00000c20: 6e20 7468 6520 7472 6169 6e69 6e67 206a  n the training j
-00000c30: 6f62 2e0a 2020 2020 6d6f 6465 6c5f 6e61  ob..    model_na
-00000c40: 6d65 203a 2073 7472 2c20 6f70 7469 6f6e  me : str, option
-00000c50: 616c 0a20 2020 2020 2020 2054 6865 206e  al.        The n
-00000c60: 616d 6520 746f 2067 6976 6520 7468 6520  ame to give the 
-00000c70: 6d6f 6465 6c2e 0a20 2020 2066 6f72 6365  model..    force
-00000c80: 5f70 7265 7072 6f63 6573 7320 3a20 626f  _preprocess : bo
-00000c90: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-00000ca0: 2020 2020 2049 6620 7365 7420 746f 2054       If set to T
-00000cb0: 7275 652c 2070 7265 7072 6f63 6573 7369  rue, preprocessi
-00000cc0: 6e67 2069 7320 666f 7263 6564 2065 7665  ng is forced eve
-00000cd0: 6e20 6966 2070 7265 7072 6f63 6573 7365  n if preprocesse
-00000ce0: 6420 6461 7461 2061 6c72 6561 6479 2065  d data already e
-00000cf0: 7869 7374 732e 0a0a 2020 2020 5265 7475  xists...    Retu
-00000d00: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00000d10: 2020 2020 4a6f 620a 2020 2020 2020 2020      Job.        
-00000d20: 4120 4a6f 620a 0a20 2020 2052 6169 7365  A Job..    Raise
-00000d30: 730a 2020 2020 2d2d 2d2d 2d2d 0a20 2020  s.    ------.   
-00000d40: 2049 6e76 616c 6964 5061 7261 6d65 7465   InvalidParamete
-00000d50: 7245 7272 6f72 0a20 2020 2020 2020 2049  rError.        I
-00000d60: 6620 7468 6520 6061 7373 6179 6461 7461  f the `assaydata
-00000d70: 7365 7460 2069 7320 6e6f 7420 616e 2041  set` is not an A
-00000d80: 7373 6179 4461 7461 7365 7420 6f62 6a65  ssayDataset obje
-00000d90: 6374 2c0a 2020 2020 2020 2020 4966 2061  ct,.        If a
-00000da0: 6e79 206d 6561 7375 7265 6d65 6e74 206e  ny measurement n
-00000db0: 616d 6520 7072 6f76 6964 6564 2064 6f65  ame provided doe
-00000dc0: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
-00000dd0: 6865 2041 7373 6179 4461 7461 7365 742c  he AssayDataset,
-00000de0: 0a20 2020 2020 2020 206f 7220 6966 2074  .        or if t
-00000df0: 6865 2041 7373 6179 4461 7461 7365 7420  he AssayDataset 
-00000e00: 6861 7320 6665 7765 7220 7468 616e 2033  has fewer than 3
-00000e10: 2064 6174 6120 706f 696e 7473 2e0a 2020   data points..  
-00000e20: 2020 4854 5450 4572 726f 720a 2020 2020    HTTPError.    
-00000e30: 2020 2020 4966 2074 6865 2072 6571 7565      If the reque
-00000e40: 7374 2074 6f20 7468 6520 7365 7276 6572  st to the server
-00000e50: 2066 6169 6c73 2e0a 2020 2020 7a2e 6173   fails..    z.as
-00000e60: 7361 7964 6174 6173 6574 2073 686f 756c  saydataset shoul
-00000e70: 6420 6265 2061 6e20 6173 7361 7964 6174  d be an assaydat
-00000e80: 6120 4a6f 6220 7265 7375 6c74 7a03 4e6f  a Job resultz.No
-00000e90: 207a 1520 696e 206d 6561 7375 7265 6d65   z. in measureme
-00000ea0: 6e74 206e 616d 6573 7201 0000 00e9 0300  nt namesr.......
-00000eb0: 0000 7a31 4173 7361 7964 6174 6120 6d75  ..z1Assaydata mu
-00000ec0: 7374 2068 6176 6520 3e3d 3320 6461 7461  st have >=3 data
-00000ed0: 2070 6f69 6e74 7320 666f 7220 7472 6169   points for trai
-00000ee0: 6e69 6e67 214e 722a 0000 0029 03da 0861  ning!Nr*...)...a
-00000ef0: 7373 6179 5f69 6472 2c00 0000 722d 0000  ssay_idr,...r-..
-00000f00: 0072 2e00 0000 2902 7215 0000 0072 1700  .r....).r....r..
-00000f10: 0000 290e da0a 6973 696e 7374 616e 6365  ..)...isinstance
-00000f20: 720f 0000 0072 0c00 0000 da03 7374 72da  r....r......str.
-00000f30: 116d 6561 7375 7265 6d65 6e74 5f6e 616d  .measurement_nam
-00000f40: 6573 da05 7368 6170 65da 0269 64da 056c  es..shape..id..l
-00000f50: 6f77 6572 7221 0000 00da 1072 6169 7365  owerr!.....raise
-00000f60: 5f66 6f72 5f73 7461 7475 7372 2200 0000  _for_statusr"...
-00000f70: 7223 0000 0072 0a00 0000 7217 0000 0029  r#...r....r....)
-00000f80: 0a72 1100 0000 7219 0000 0072 2b00 0000  .r....r....r+...
-00000f90: 722c 0000 0072 2d00 0000 722e 0000 005a  r,...r-...r....Z
-00000fa0: 0b6d 6561 7375 7265 6d65 6e74 da04 6461  .measurement..da
-00000fb0: 7461 7215 0000 0072 1a00 0000 721b 0000  tar....r....r...
-00000fc0: 0072 1b00 0000 721c 0000 00da 0a5f 7472  .r....r......_tr
-00000fd0: 6169 6e5f 6a6f 624b 0000 0073 2600 0000  ain_jobK...s&...
-00000fe0: 002c 0a01 0801 0a01 0602 0801 0a01 1201  .,..............
-00000ff0: 0e01 0801 0801 0403 0401 0201 02fd 0605  ................
-00001000: 1002 1001 0801 723a 0000 0029 0572 1100  ......r:...).r..
-00001010: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00001020: 0072 2e00 0000 6305 0000 0000 0000 0000  .r....c.........
-00001030: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
-00001040: 1600 0000 6401 7d05 7400 7c00 7c05 7c01  ....d.}.t.|.|.|.
-00001050: 7c02 7c03 7c04 8306 5300 2902 722f 0000  |.|.|...S.).r/..
-00001060: 007a 1176 312f 776f 726b 666c 6f77 2f74  .z.v1/workflow/t
-00001070: 7261 696e a901 723a 0000 00a9 0672 1100  rain..r:.....r..
-00001080: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00001090: 0072 2e00 0000 7219 0000 0072 1b00 0000  .r....r....r....
-000010a0: 721b 0000 0072 1c00 0000 da10 6372 6561  r....r......crea
-000010b0: 7465 5f74 7261 696e 5f6a 6f62 9000 0000  te_train_job....
-000010c0: 7312 0000 0000 2b04 0102 0102 0002 0002  s.....+.........
-000010d0: 0002 0002 0002 ff72 3d00 0000 6305 0000  .......r=...c...
-000010e0: 0000 0000 0000 0000 0006 0000 0007 0000  ................
-000010f0: 0043 0000 0073 1600 0000 6401 7d05 7400  .C...s....d.}.t.
-00001100: 7c00 7c05 7c01 7c02 7c03 7c04 8306 5300  |.|.|.|.|.|...S.
-00001110: 2902 fa1a 416c 6961 7320 666f 7220 6372  )...Alias for cr
-00001120: 6561 7465 5f74 7261 696e 5f6a 6f62 7a14  eate_train_jobz.
-00001130: 7631 2f77 6f72 6b66 6c6f 772f 7472 6169  v1/workflow/trai
-00001140: 6e2f 6272 723b 0000 0072 3c00 0000 721b  n/brr;...r<...r.
-00001150: 0000 0072 1b00 0000 721c 0000 00da 145f  ...r....r......_
-00001160: 6372 6561 7465 5f74 7261 696e 5f6a 6f62  create_train_job
-00001170: 5f62 72c1 0000 0073 1200 0000 0008 0401  _br....s........
-00001180: 0201 0200 0200 0200 0200 0200 02ff 723f  ..............r?
-00001190: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-000011a0: 0600 0000 0700 0000 4300 0000 7316 0000  ........C...s...
-000011b0: 0064 017d 0574 007c 007c 057c 017c 027c  .d.}.t.|.|.|.|.|
-000011c0: 037c 0483 0653 0029 0272 3e00 0000 7a14  .|...S.).r>...z.
-000011d0: 7631 2f77 6f72 6b66 6c6f 772f 7472 6169  v1/workflow/trai
-000011e0: 6e2f 6770 723b 0000 0072 3c00 0000 721b  n/gpr;...r<...r.
-000011f0: 0000 0072 1b00 0000 721c 0000 00da 145f  ...r....r......_
-00001200: 6372 6561 7465 5f74 7261 696e 5f6a 6f62  create_train_job
-00001210: 5f67 70cf 0000 0073 1200 0000 0008 0401  _gp....s........
-00001220: 0201 0200 0200 0200 0200 0200 02ff 7240  ..............r@
-00001230: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001240: 0400 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-00001250: 0064 017c 019b 009d 027d 027c 00a0 007c  .d.|.....}.|...|
-00001260: 02a1 017d 0374 0166 007c 03a0 02a1 008e  ...}.t.f.|......
-00001270: 0153 0029 027a 2c47 6574 2054 7261 696e  .S.).z,Get Train
-00001280: 696e 6720 7265 7375 6c74 7320 2865 2e67  ing results (e.g
-00001290: 2e20 6c6f 7373 2065 7463 2920 6f66 206a  . loss etc) of j
-000012a0: 6f62 2e7a 1276 312f 776f 726b 666c 6f77  ob.z.v1/workflow
-000012b0: 2f74 7261 696e 2f29 0372 1600 0000 7208  /train/).r....r.
-000012c0: 0000 0072 1700 0000 7218 0000 0072 1b00  ...r....r....r..
-000012d0: 0000 721b 0000 0072 1c00 0000 da14 6765  ..r....r......ge
-000012e0: 745f 7472 6169 6e69 6e67 5f72 6573 756c  t_training_resul
-000012f0: 7473 dd00 0000 7306 0000 0000 020a 010a  ts....s.........
-00001300: 0172 4100 0000 6302 0000 0000 0000 0000  .rA...c.........
-00001310: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-00001320: 2400 0000 6401 7c01 9b00 9d02 7d02 7c00  $...d.|.....}.|.
-00001330: a000 7c02 a101 7d03 7401 a002 7403 7c03  ..|...}.t...t.|.
-00001340: a004 a100 a102 5300 2902 6191 0100 000a  ......S.).a.....
-00001350: 2020 2020 5265 6c6f 6164 2061 2053 7562      Reload a Sub
-00001360: 6d69 7474 6564 206a 6f62 2074 6f20 7265  mitted job to re
-00001370: 7375 6d65 2066 726f 6d20 7768 6572 6520  sume from where 
-00001380: 796f 7520 6c65 6674 206f 6666 210a 0a0a  you left off!...
-00001390: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000013a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000013b0: 2020 7365 7373 696f 6e20 3a20 4150 4953    session : APIS
-000013c0: 6573 7369 6f6e 0a20 2020 2020 2020 2054  ession.        T
-000013d0: 6865 2063 7572 7265 6e74 2041 5049 2073  he current API s
-000013e0: 6573 7369 6f6e 2066 6f72 2063 6f6d 6d75  ession for commu
-000013f0: 6e69 6361 7469 6f6e 2077 6974 6820 7468  nication with th
-00001400: 6520 7365 7276 6572 2e0a 2020 2020 6a6f  e server..    jo
-00001410: 625f 6964 203a 2073 7472 0a20 2020 2020  b_id : str.     
-00001420: 2020 2054 6865 2069 6465 6e74 6966 6965     The identifie
-00001430: 7220 6f66 2074 6865 206a 6f62 2077 686f  r of the job who
-00001440: 7365 2064 6574 6169 6c73 2061 7265 2074  se details are t
-00001450: 6f20 6265 206c 6f61 6465 642e 0a0a 2020  o be loaded...  
-00001460: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00001470: 2d2d 2d2d 2d0a 2020 2020 4a6f 620a 2020  -----.    Job.  
-00001480: 2020 2020 2020 4a6f 620a 0a20 2020 2052        Job..    R
-00001490: 6169 7365 730a 2020 2020 2d2d 2d2d 2d2d  aises.    ------
-000014a0: 0a20 2020 2048 5454 5045 7272 6f72 0a20  .    HTTPError. 
-000014b0: 2020 2020 2020 2049 6620 7468 6520 7265         If the re
-000014c0: 7175 6573 7420 746f 2074 6865 2073 6572  quest to the ser
-000014d0: 7665 7220 6661 696c 732e 0a0a 2020 2020  ver fails...    
-000014e0: 7a16 7631 2f77 6f72 6b66 6c6f 772f 7472  z.v1/workflow/tr
-000014f0: 6169 6e2f 6a6f 622f 2905 7216 0000 0072  ain/job/).r....r
-00001500: 2200 0000 7223 0000 0072 0a00 0000 7217  "...r#...r....r.
-00001510: 0000 0072 1800 0000 721b 0000 0072 1b00  ...r....r....r..
-00001520: 0000 721c 0000 00da 086c 6f61 645f 6a6f  ..r......load_jo
-00001530: 62e4 0000 0073 0600 0000 0017 0a01 0a01  b....s..........
-00001540: 7242 0000 0063 0000 0000 0000 0000 0000  rB...c..........
-00001550: 0000 0000 0000 0400 0000 4000 0000 734c  ..........@...sL
-00001560: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00001570: 0365 0465 0564 023c 0065 0665 0564 033c  .e.e.d.<.e.e.d.<
-00001580: 0065 0765 0564 043c 0064 0564 0684 005a  .e.e.d.<.d.d...Z
-00001590: 0864 0c65 0965 0a19 0065 0965 0a19 0064  .d.e.e...e.e...d
-000015a0: 099c 0264 0a64 0b84 055a 0b64 0753 0029  ...d.d...Z.d.S.)
-000015b0: 0dda 0d43 5646 7574 7572 654d 6978 696e  ...CVFutureMixin
-000015c0: 6164 0200 000a 2020 2020 4120 6d69 7869  ad....    A mixi
-000015d0: 6e20 636c 6173 7320 746f 2070 726f 7669  n class to provi
-000015e0: 6465 2063 726f 7373 2d76 616c 6964 6174  de cross-validat
-000015f0: 696f 6e20 6a6f 6220 7375 626d 6973 7369  ion job submissi
-00001600: 6f6e 2061 6e64 2072 6574 7269 6576 616c  on and retrieval
-00001610: 2e0a 0a20 2020 2041 7474 7269 6275 7465  ...    Attribute
-00001620: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00001630: 0a20 2020 2073 6573 7369 6f6e 203a 2041  .    session : A
-00001640: 5049 5365 7373 696f 6e0a 2020 2020 2020  PISession.      
-00001650: 2020 5468 6520 7365 7373 696f 6e20 6f62    The session ob
-00001660: 6a65 6374 2074 6f20 7573 6520 666f 7220  ject to use for 
-00001670: 4150 4920 636f 6d6d 756e 6963 6174 696f  API communicatio
-00001680: 6e2e 0a20 2020 2074 7261 696e 5f6a 6f62  n..    train_job
-00001690: 5f69 6420 3a20 7374 720a 2020 2020 2020  _id : str.      
-000016a0: 2020 5468 6520 6964 206f 6620 7468 6520    The id of the 
-000016b0: 7472 6169 6e69 6e67 206a 6f62 2061 7373  training job ass
-000016c0: 6f63 6961 7465 6420 7769 7468 2074 6869  ociated with thi
-000016d0: 7320 6372 6f73 732d 7661 6c69 6461 7469  s cross-validati
-000016e0: 6f6e 206a 6f62 2e0a 2020 2020 6a6f 6220  on job..    job 
-000016f0: 3a20 4a6f 620a 2020 2020 2020 2020 5468  : Job.        Th
-00001700: 6520 4a6f 6220 6f62 6a65 6374 2066 6f72  e Job object for
-00001710: 2074 6869 7320 6372 6f73 732d 7661 6c69   this cross-vali
-00001720: 6461 7469 6f6e 206a 6f62 2e0a 0a20 2020  dation job...   
-00001730: 204d 6574 686f 6473 0a20 2020 202d 2d2d   Methods.    ---
-00001740: 2d2d 2d2d 0a20 2020 2063 726f 7373 7661  ----.    crossva
-00001750: 6c69 6461 7465 2829 3a0a 2020 2020 2020  lidate():.      
-00001760: 2020 5375 626d 6974 7320 6120 6372 6f73    Submits a cros
-00001770: 732d 7661 6c69 6461 7469 6f6e 206a 6f62  s-validation job
-00001780: 2074 6f20 7468 6520 7365 7276 6572 2e0a   to the server..
-00001790: 2020 2020 6765 745f 6372 6f73 7376 616c      get_crossval
-000017a0: 6964 6174 696f 6e28 7061 6765 5f73 697a  idation(page_siz
-000017b0: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-000017c0: 203d 204e 6f6e 652c 2070 6167 655f 6f66   = None, page_of
-000017d0: 6673 6574 3a20 4f70 7469 6f6e 616c 5b69  fset: Optional[i
-000017e0: 6e74 5d20 3d20 3029 3a0a 2020 2020 2020  nt] = 0):.      
-000017f0: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
-00001800: 7265 7375 6c74 7320 6f66 2074 6865 2063  results of the c
-00001810: 726f 7373 2d76 616c 6964 6174 696f 6e20  ross-validation 
-00001820: 6a6f 622e 0a20 2020 2072 1100 0000 721f  job..    r....r.
-00001830: 0000 00da 036a 6f62 6301 0000 0000 0000  .....jobc.......
-00001840: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00001850: 0073 2c00 0000 7c00 6a00 6401 6b08 7220  .s,...|.j.d.k.r 
-00001860: 7401 7c00 6a02 7c00 6a03 8302 7c00 5f00  t.|.j.|.j...|._.
-00001870: 7c00 6a00 5300 7404 6402 8301 8201 6401  |.j.S.t.d.....d.
-00001880: 5300 2903 615d 0100 000a 2020 2020 2020  S.).a]....      
-00001890: 2020 5375 626d 6974 2061 2063 726f 7373    Submit a cross
-000018a0: 2d76 616c 6964 6174 696f 6e20 6a6f 6220  -validation job 
-000018b0: 746f 2074 6865 2073 6572 7665 722e 0a0a  to the server...
-000018c0: 2020 2020 2020 2020 4966 2074 6865 206a          If the j
-000018d0: 6f62 2068 6173 2061 6c72 6561 6479 2062  ob has already b
-000018e0: 6565 6e20 7375 626d 6974 7465 642c 2061  een submitted, a
-000018f0: 6e20 496e 7661 6c69 644a 6f62 2065 7863  n InvalidJob exc
-00001900: 6570 7469 6f6e 2069 7320 7261 6973 6564  eption is raised
-00001910: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001920: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00001930: 2d2d 0a20 2020 2020 2020 204a 6f62 0a20  --.        Job. 
-00001940: 2020 2020 2020 2020 2020 2054 6865 204a             The J
-00001950: 6f62 206f 626a 6563 7420 666f 7220 7468  ob object for th
-00001960: 6973 2063 726f 7373 2d76 616c 6964 6174  is cross-validat
-00001970: 696f 6e20 6a6f 622e 0a0a 2020 2020 2020  ion job...      
-00001980: 2020 5261 6973 6573 0a20 2020 2020 2020    Raises.       
-00001990: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
-000019a0: 496e 7661 6c69 644a 6f62 0a20 2020 2020  InvalidJob.     
-000019b0: 2020 2020 2020 2049 6620 7468 6520 6a6f         If the jo
-000019c0: 6220 6861 7320 616c 7265 6164 7920 6265  b has already be
-000019d0: 656e 2073 7562 6d69 7474 6564 2e0a 2020  en submitted..  
-000019e0: 2020 2020 2020 4e7a 4543 5620 4a6f 6220        NzECV Job 
-000019f0: 6861 7320 616c 7265 6164 7920 6265 656e  has already been
-00001a00: 2073 7562 6d69 7474 6564 2e20 5573 6520   submitted. Use 
-00001a10: 6765 745f 6372 6f73 7376 616c 6964 6174  get_crossvalidat
-00001a20: 696f 6e28 2920 696e 7374 6561 642e 2905  ion() instead.).
-00001a30: 7244 0000 0072 2400 0000 7211 0000 0072  rD...r$...r....r
-00001a40: 1f00 0000 720e 0000 00a9 01da 0473 656c  ....r........sel
-00001a50: 6672 1b00 0000 721b 0000 0072 1c00 0000  fr....r....r....
-00001a60: 7224 0000 0019 0100 0073 0c00 0000 0010  r$.......s......
-00001a70: 0a01 1001 0602 0201 02ff 7a1b 4356 4675  ..........z.CVFu
-00001a80: 7475 7265 4d69 7869 6e2e 6372 6f73 7376  tureMixin.crossv
-00001a90: 616c 6964 6174 654e 7201 0000 0072 2700  alidateNr....r'.
-00001aa0: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00001ab0: 0000 0005 0000 0043 0000 0073 2a00 0000  .......C...s*...
-00001ac0: 7c00 6a00 6401 6b09 721e 7401 7c00 6a02  |.j.d.k.r.t.|.j.
-00001ad0: 7c00 6a00 6a03 7c01 7c02 8304 5300 7404  |.j.j.|.|...S.t.
-00001ae0: 6402 8301 8201 6401 5300 2903 6141 0200  d.....d.S.).aA..
-00001af0: 000a 2020 2020 2020 2020 5265 7472 6965  ..        Retrie
-00001b00: 7665 7320 7468 6520 7265 7375 6c74 7320  ves the results 
-00001b10: 6f66 2074 6865 2063 726f 7373 2d76 616c  of the cross-val
-00001b20: 6964 6174 696f 6e20 6a6f 622e 0a0a 2020  idation job...  
-00001b30: 2020 2020 2020 4966 206e 6f20 6a6f 6220        If no job 
-00001b40: 6861 7320 6265 656e 2073 7562 6d69 7474  has been submitt
-00001b50: 6564 2c20 616e 2049 6e76 616c 6964 4a6f  ed, an InvalidJo
-00001b60: 6220 6578 6365 7074 696f 6e20 6973 2072  b exception is r
-00001b70: 6169 7365 642e 0a0a 2020 2020 2020 2020  aised...        
-00001b80: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00001b90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00001ba0: 2020 2020 2020 7061 6765 5f73 697a 6520        page_size 
-00001bb0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-00001bc0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001bd0: 6e75 6d62 6572 206f 6620 6974 656d 7320  number of items 
-00001be0: 746f 2072 6574 7269 6576 6520 696e 2061  to retrieve in a
-00001bf0: 2073 696e 676c 6520 7265 7175 6573 742e   single request.
-00001c00: 2e0a 2020 2020 2020 2020 7061 6765 5f6f  ..        page_o
-00001c10: 6666 7365 7420 3a20 696e 742c 206f 7074  ffset : int, opt
-00001c20: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00001c30: 2020 5468 6520 6f66 6673 6574 2074 6f20    The offset to 
-00001c40: 7374 6172 7420 7265 7472 6965 7669 6e67  start retrieving
-00001c50: 2069 7465 6d73 2066 726f 6d2e 2044 6566   items from. Def
-00001c60: 6175 6c74 2069 7320 302e 0a0a 2020 2020  ault is 0...    
-00001c70: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00001c80: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00001c90: 2020 2020 6469 6374 0a20 2020 2020 2020      dict.       
-00001ca0: 2020 2020 2054 6865 2072 6573 756c 7473       The results
-00001cb0: 206f 6620 7468 6520 6372 6f73 732d 7661   of the cross-va
-00001cc0: 6c69 6461 7469 6f6e 206a 6f62 2e0a 0a20  lidation job... 
-00001cd0: 2020 2020 2020 2052 6169 7365 730a 2020         Raises.  
-00001ce0: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00001cf0: 2020 2020 2049 6e76 616c 6964 4a6f 620a       InvalidJob.
-00001d00: 2020 2020 2020 2020 2020 2020 4966 206e              If n
-00001d10: 6f20 6a6f 6220 6861 7320 6265 656e 2073  o job has been s
-00001d20: 7562 6d69 7474 6564 2e0a 2020 2020 2020  ubmitted..      
-00001d30: 2020 4e7a 414e 6f20 4356 204a 6f62 2068    NzANo CV Job h
-00001d40: 6173 2062 6565 6e20 7375 626d 6974 7465  as been submitte
-00001d50: 6421 2043 616c 6c20 6372 6f73 7376 616c  d! Call crossval
-00001d60: 6964 6174 6528 2920 616e 6420 7472 7920  idate() and try 
-00001d70: 6167 6169 6e2e 2905 7244 0000 0072 2900  again.).rD...r).
-00001d80: 0000 7211 0000 0072 1200 0000 720e 0000  ..r....r....r...
-00001d90: 0029 0372 4600 0000 7225 0000 0072 2600  .).rF...r%...r&.
-00001da0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001db0: 0072 2900 0000 3101 0000 7314 0000 0000  .r)...1...s.....
-00001dc0: 190a 0102 0104 0006 0002 0002 ff04 0402  ................
-00001dd0: 0102 ff7a 2143 5646 7574 7572 654d 6978  ...z!CVFutureMix
-00001de0: 696e 2e67 6574 5f63 726f 7373 7661 6c69  in.get_crossvali
-00001df0: 6461 7469 6f6e 2902 4e72 0100 0000 290c  dation).Nr....).
-00001e00: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001e10: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001e20: 6d65 5f5f da07 5f5f 646f 635f 5f72 0500  me__..__doc__r..
-00001e30: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-00001e40: 735f 5f72 3300 0000 7207 0000 0072 2400  s__r3...r....r$.
-00001e50: 0000 7202 0000 00da 0369 6e74 7229 0000  ..r......intr)..
-00001e60: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00001e70: 721c 0000 0072 4300 0000 0001 0000 7316  r....rC.......s.
-00001e80: 0000 000a 0104 1408 0108 0108 0208 1900  ................
-00001e90: 0000 ff02 0106 0006 ff72 4300 0000 6300  .........rC...c.
-00001ea0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-00001eb0: 0000 0000 0000 0073 6600 0000 6500 5a01  .......sf...e.Z.
-00001ec0: 6400 5a02 6401 5a03 6411 6504 6505 6506  d.Z.d.Z.d.e.e.e.
-00001ed0: 6403 9c03 8700 6601 6404 6405 840d 5a07  d.....f.d.d...Z.
-00001ee0: 6505 6406 9c01 6407 6408 8404 5a08 6505  e.d...d.d...Z.e.
-00001ef0: 6406 9c01 6409 640a 8404 5a09 650a 640b  d...d.d...Z.e.d.
-00001f00: 640c 8400 8301 5a0b 6412 650c 650d 640e  d.....Z.d.e.e.d.
-00001f10: 9c02 640f 6410 8405 5a0e 8700 0400 5a0f  ..d.d...Z.....Z.
-00001f20: 5300 2913 da08 4356 4675 7475 7265 619b  S.)...CVFuturea.
-00001f30: 0200 000a 2020 2020 5468 6973 2063 6c61  ....    This cla
-00001f40: 7373 2068 656c 7073 2069 6e69 7469 6174  ss helps initiat
-00001f50: 696e 672c 2073 7562 6d69 7474 696e 672c  ing, submitting,
-00001f60: 2061 6e64 2072 6574 7269 6576 696e 6720   and retrieving 
-00001f70: 7468 650a 2020 2020 7265 7375 6c74 7320  the.    results 
-00001f80: 6f66 2061 2063 726f 7373 2d76 616c 6964  of a cross-valid
-00001f90: 6174 696f 6e20 6a6f 622e 0a0a 2020 2020  ation job...    
-00001fa0: 4174 7472 6962 7574 6573 0a20 2020 202d  Attributes.    -
-00001fb0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7365  ---------.    se
-00001fc0: 7373 696f 6e20 3a20 4150 4953 6573 7369  ssion : APISessi
-00001fd0: 6f6e 0a20 2020 2020 2020 2054 6865 2073  on.        The s
-00001fe0: 6573 7369 6f6e 206f 626a 6563 7420 746f  ession object to
-00001ff0: 2075 7365 2066 6f72 2041 5049 2063 6f6d   use for API com
-00002000: 6d75 6e69 6361 7469 6f6e 2e0a 2020 2020  munication..    
-00002010: 7472 6169 6e5f 6a6f 625f 6964 203a 2073  train_job_id : s
-00002020: 7472 0a20 2020 2020 2020 2054 6865 2069  tr.        The i
-00002030: 6420 6f66 2074 6865 2074 7261 696e 696e  d of the trainin
-00002040: 6720 6a6f 6220 6173 736f 6369 6174 6564  g job associated
-00002050: 2077 6974 6820 7468 6973 2063 726f 7373   with this cross
-00002060: 2d76 616c 6964 6174 696f 6e20 6a6f 622e  -validation job.
-00002070: 0a20 2020 206a 6f62 203a 204a 6f62 0a20  .    job : Job. 
-00002080: 2020 2020 2020 2054 6865 204a 6f62 206f         The Job o
-00002090: 626a 6563 7420 666f 7220 7468 6973 2063  bject for this c
-000020a0: 726f 7373 2d76 616c 6964 6174 696f 6e20  ross-validation 
-000020b0: 6a6f 622e 0a20 2020 2070 6167 655f 7369  job..    page_si
-000020c0: 7a65 203a 2069 6e74 0a20 2020 2020 2020  ze : int.       
-000020d0: 2054 6865 206e 756d 6265 7220 6f66 2069   The number of i
-000020e0: 7465 6d73 2074 6f20 7265 7472 6965 7665  tems to retrieve
-000020f0: 2069 6e20 6120 7369 6e67 6c65 2072 6571   in a single req
-00002100: 7565 7374 2e0a 0a20 2020 204d 6574 686f  uest...    Metho
-00002110: 6473 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ds.    -------. 
-00002120: 2020 205f 5f73 7472 5f5f 2829 3a0a 2020     __str__():.  
-00002130: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
-00002140: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-00002150: 6174 696f 6e20 6f66 2074 6865 2063 726f  ation of the cro
-00002160: 7373 2d76 616c 6964 6174 696f 6e20 6a6f  ss-validation jo
-00002170: 622e 0a20 2020 205f 5f72 6570 725f 5f28  b..    __repr__(
-00002180: 293a 0a20 2020 2020 2020 2052 6574 7572  ):.        Retur
-00002190: 6e73 2061 2064 6574 6169 6c65 6420 7265  ns a detailed re
-000021a0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-000021b0: 7468 6520 6372 6f73 732d 7661 6c69 6461  the cross-valida
-000021c0: 7469 6f6e 206a 6f62 2e0a 2020 2020 4e29  tion job..    N)
-000021d0: 0372 1100 0000 721f 0000 0072 4400 0000  .r....r....rD...
-000021e0: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-000021f0: 0004 0000 0003 0000 0073 1e00 0000 7400  .........s....t.
-00002200: 8300 a001 7c01 7c03 a102 0100 7c02 7c00  ....|.|.....|.|.
-00002210: 5f02 6401 7c00 5f03 6402 5300 2903 6179  _.d.|._.d.S.).ay
-00002220: 0100 000a 2020 2020 2020 2020 436f 6e73  ....        Cons
-00002230: 7472 7563 7473 2061 206e 6577 2043 5646  tructs a new CVF
-00002240: 7574 7572 6520 696e 7374 616e 6365 2e0a  uture instance..
-00002250: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00002260: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00002270: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
-00002280: 6573 7369 6f6e 203a 2041 5049 5365 7373  ession : APISess
-00002290: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000022a0: 5468 6520 7365 7373 696f 6e20 6f62 6a65  The session obje
-000022b0: 6374 2074 6f20 7573 6520 666f 7220 4150  ct to use for AP
-000022c0: 4920 636f 6d6d 756e 6963 6174 696f 6e2e  I communication.
-000022d0: 0a20 2020 2020 2020 2074 7261 696e 5f6a  .        train_j
-000022e0: 6f62 5f69 6420 3a20 7374 720a 2020 2020  ob_id : str.    
-000022f0: 2020 2020 2020 2020 5468 6520 6964 206f          The id o
-00002300: 6620 7468 6520 7472 6169 6e69 6e67 206a  f the training j
-00002310: 6f62 2061 7373 6f63 6961 7465 6420 7769  ob associated wi
-00002320: 7468 2074 6869 7320 6372 6f73 732d 7661  th this cross-va
-00002330: 6c69 6461 7469 6f6e 206a 6f62 2e0a 2020  lidation job..  
-00002340: 2020 2020 2020 6a6f 6220 3a20 4a6f 622c        job : Job,
-00002350: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00002360: 2020 2020 2020 5468 6520 4a6f 6220 6f62        The Job ob
-00002370: 6a65 6374 2066 6f72 2074 6869 7320 6372  ject for this cr
-00002380: 6f73 732d 7661 6c69 6461 7469 6f6e 206a  oss-validation j
-00002390: 6f62 2e0a 2020 2020 2020 2020 69e8 0300  ob..        i...
-000023a0: 004e 2904 da05 7375 7065 72da 085f 5f69  .N)...super..__i
-000023b0: 6e69 745f 5f72 1f00 0000 7225 0000 0029  nit__r....r%...)
-000023c0: 0472 4600 0000 7211 0000 0072 1f00 0000  .rF...r....r....
-000023d0: 7244 0000 00a9 01da 095f 5f63 6c61 7373  rD.......__class
-000023e0: 5f5f 721b 0000 0072 1c00 0000 724f 0000  __r....r....rO..
-000023f0: 006c 0100 0073 0600 0000 000d 0e01 0601  .l...s..........
-00002400: 7a11 4356 4675 7475 7265 2e5f 5f69 6e69  z.CVFuture.__ini
-00002410: 745f 5fa9 0172 1300 0000 6301 0000 0000  t__..r....c.....
-00002420: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00002430: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00002440: 5300 a901 4ea9 0272 3300 0000 7244 0000  S...N..r3...rD..
-00002450: 0072 4500 0000 721b 0000 0072 1b00 0000  .rE...r....r....
-00002460: 721c 0000 00da 075f 5f73 7472 5f5f 7d01  r......__str__}.
-00002470: 0000 7302 0000 0000 017a 1043 5646 7574  ..s......z.CVFut
-00002480: 7572 652e 5f5f 7374 725f 5f63 0100 0000  ure.__str__c....
-00002490: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000024a0: 4300 0000 730a 0000 0074 007c 006a 0183  C...s....t.|.j..
-000024b0: 0153 0072 5300 0000 a902 da04 7265 7072  .S.rS.......repr
-000024c0: 7244 0000 0072 4500 0000 721b 0000 0072  rD...rE...r....r
-000024d0: 1b00 0000 721c 0000 00da 085f 5f72 6570  ....r......__rep
-000024e0: 725f 5f80 0100 0073 0200 0000 0001 7a11  r__....s......z.
-000024f0: 4356 4675 7475 7265 2e5f 5f72 6570 725f  CVFuture.__repr_
-00002500: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00002510: 0000 0100 0000 4300 0000 7308 0000 007c  ......C...s....|
-00002520: 006a 006a 0153 0072 5300 0000 a902 7244  .j.j.S.rS.....rD
-00002530: 0000 0072 1200 0000 7245 0000 0072 1b00  ...r....rE...r..
-00002540: 0000 721b 0000 0072 1c00 0000 7236 0000  ..r....r....r6..
-00002550: 0083 0100 0073 0200 0000 0002 7a0b 4356  .....s......z.CV
-00002560: 4675 7475 7265 2e69 6446 a902 da07 7665  Future.idF....ve
-00002570: 7262 6f73 6572 1300 0000 6302 0000 0000  rboser....c.....
-00002580: 0000 0000 0000 0008 0000 000a 0000 0043  ...............C
-00002590: 0000 0073 8c00 0000 7c00 6a00 7d02 6700  ...s....|.j.}.g.
-000025a0: 7d03 7c02 7d04 6401 7d05 7c04 7c02 6b05  }.|.}.d.}.|.|.k.
-000025b0: 7288 7a2e 7c00 6a01 7c05 7c02 6402 8d02  r.z.|.j.|.|.d...
-000025c0: 7d06 7c03 7c06 6a02 3700 7d03 7403 7c06  }.|.|.j.7.}.t.|.
-000025d0: 6a02 8301 7d04 7c05 7c04 3700 7d05 5700  j...}.|.|.7.}.W.
-000025e0: 7112 0400 7404 6b0a 7284 0100 7d07 0100  q...t.k.r...}...
-000025f0: 7a1e 7c01 726c 7405 6403 7c07 9b00 9d02  z.|.rlt.d.|.....
-00002600: 8301 0100 7c03 0600 5700 5900 a202 5300  ....|...W.Y...S.
-00002610: 6404 7d07 7e07 5800 5900 7112 5800 7112  d.}.~.X.Y.q.X.q.
-00002620: 7c03 5300 2905 6148 0100 000a 2020 2020  |.S.).aH....    
-00002630: 2020 2020 4765 7420 616c 6c20 7468 6520      Get all the 
-00002640: 7265 7375 6c74 7320 6f66 2074 6865 2043  results of the C
-00002650: 5620 6a6f 622e 0a0a 2020 2020 2020 2020  V job...        
-00002660: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00002670: 2020 7665 7262 6f73 6520 2862 6f6f 6c2c    verbose (bool,
-00002680: 206f 7074 696f 6e61 6c29 3a20 4966 2054   optional): If T
-00002690: 7275 652c 2070 7269 6e74 2076 6572 626f  rue, print verbo
-000026a0: 7365 206f 7574 7075 742e 2044 6566 6175  se output. Defau
-000026b0: 6c74 7320 4661 6c73 652e 0a0a 2020 2020  lts False...    
-000026c0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-000026d0: 2020 2020 2020 2020 4150 4945 7272 6f72          APIError
-000026e0: 3a20 4966 2074 6865 7265 2069 7320 616e  : If there is an
-000026f0: 2069 7373 7565 2077 6974 6820 7468 6520   issue with the 
-00002700: 4150 4920 7265 7175 6573 742e 0a0a 2020  API request...  
-00002710: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00002720: 2020 2020 2020 2020 2020 2050 7265 6469             Predi
-00002730: 6374 4a6f 623a 2041 206c 6973 7420 6f66  ctJob: A list of
-00002740: 2070 7265 6469 6374 206f 626a 6563 7473   predict objects
-00002750: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00002760: 6520 7265 7375 6c74 732e 0a20 2020 2020  e results..     
-00002770: 2020 2072 0100 0000 2902 7226 0000 0072     r....).r&...r
-00002780: 2500 0000 fa17 4661 696c 6564 2074 6f20  %.....Failed to 
-00002790: 6765 7420 7265 7375 6c74 733a 204e 2906  get results: N).
-000027a0: 7225 0000 0072 2900 0000 da06 7265 7375  r%...r).....resu
-000027b0: 6c74 da03 6c65 6e72 0d00 0000 da05 7072  lt..lenr......pr
-000027c0: 696e 7429 0872 4600 0000 725b 0000 00da  int).rF...r[....
-000027d0: 0473 7465 70da 0772 6573 756c 7473 da0c  .step..results..
-000027e0: 6e75 6d5f 7265 7475 726e 6564 da06 6f66  num_returned..of
-000027f0: 6673 6574 721a 0000 00da 0365 7863 721b  fsetr......excr.
-00002800: 0000 0072 1b00 0000 721c 0000 0072 1600  ...r....r....r..
-00002810: 0000 8701 0000 731e 0000 0000 0d06 0204  ......s.........
-00002820: 0104 0104 0208 0102 010e 010a 010a 010c  ................
-00002830: 0110 0104 010e 011c 017a 0c43 5646 7574  .........z.CVFut
-00002840: 7572 652e 6765 7429 014e 2901 4629 1072  ure.get).N).F).r
-00002850: 4700 0000 7248 0000 0072 4900 0000 724a  G...rH...rI...rJ
-00002860: 0000 0072 0500 0000 7233 0000 0072 0700  ...r....r3...r..
-00002870: 0000 724f 0000 0072 5500 0000 7258 0000  ..rO...rU...rX..
-00002880: 00da 0870 726f 7065 7274 7972 3600 0000  ...propertyr6...
-00002890: da04 626f 6f6c 720b 0000 0072 1600 0000  ..boolr....r....
-000028a0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-000028b0: 1b00 0000 721b 0000 0072 5000 0000 721c  ....r....rP...r.
-000028c0: 0000 0072 4d00 0000 5401 0000 730e 0000  ...rM...T...s...
-000028d0: 0008 0104 1718 110e 030e 0302 010a 0372  ...............r
-000028e0: 4d00 0000 6300 0000 0000 0000 0000 0000  M...c...........
-000028f0: 0000 0000 0003 0000 0040 0000 0073 5400  .........@...sT.
-00002900: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00002910: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
-00002920: 6404 5a07 6508 6505 6405 3c00 6509 6406  d.Z.e.e.d.<.e.d.
-00002930: 9c01 6407 6408 8404 5a0a 6409 640a 8400  ..d.d...Z.d.d...
-00002940: 5a0b 640b 640c 8400 5a0c 640d 640e 8400  Z.d.d...Z.d.d...
-00002950: 5a0d 6404 5300 290f da10 5472 6169 6e46  Z.d.S.)...TrainF
-00002960: 7574 7572 654d 6978 696e 614a 0200 000a  utureMixinaJ....
-00002970: 2020 2020 5468 6973 2063 6c61 7373 2070      This class p
-00002980: 726f 7669 6465 7320 6675 6e63 7469 6f6e  rovides function
-00002990: 616c 6974 7920 666f 7220 7265 7472 6965  ality for retrie
-000029a0: 7669 6e67 2074 6865 0a20 2020 2072 6573  ving the.    res
-000029b0: 756c 7473 206f 6620 6120 7472 6169 6e69  ults of a traini
-000029c0: 6e67 206a 6f62 2061 6e64 2069 6e69 7469  ng job and initi
-000029d0: 6174 696e 6720 6372 6f73 732d 7661 6c69  ating cross-vali
-000029e0: 6461 7469 6f6e 206a 6f62 732e 0a0a 2020  dation jobs...  
-000029f0: 2020 4174 7472 6962 7574 6573 0a20 2020    Attributes.   
-00002a00: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00002a10: 7365 7373 696f 6e20 3a20 4150 4953 6573  session : APISes
-00002a20: 7369 6f6e 0a20 2020 2020 2020 2054 6865  sion.        The
-00002a30: 2073 6573 7369 6f6e 206f 626a 6563 7420   session object 
-00002a40: 746f 2075 7365 2066 6f72 2041 5049 2063  to use for API c
-00002a50: 6f6d 6d75 6e69 6361 7469 6f6e 2e0a 2020  ommunication..  
-00002a60: 2020 6a6f 6220 3a20 4a6f 620a 2020 2020    job : Job.    
-00002a70: 2020 2020 5468 6520 4a6f 6220 6f62 6a65      The Job obje
-00002a80: 6374 2066 6f72 2074 6869 7320 7472 6169  ct for this trai
-00002a90: 6e69 6e67 206a 6f62 2e0a 2020 2020 6372  ning job..    cr
-00002aa0: 6f73 7376 616c 6964 6174 696f 6e20 3a20  ossvalidation : 
-00002ab0: 4356 4675 7475 7265 0a20 2020 2020 2020  CVFuture.       
-00002ac0: 2054 6865 2043 5646 7574 7572 6520 6f62   The CVFuture ob
-00002ad0: 6a65 6374 2066 6f72 2074 6865 2061 7373  ject for the ass
-00002ae0: 6f63 6961 7465 6420 6372 6f73 732d 7661  ociated cross-va
-00002af0: 6c69 6461 7469 6f6e 206a 6f62 2e0a 0a20  lidation job... 
-00002b00: 2020 204d 6574 686f 6473 0a20 2020 202d     Methods.    -
-00002b10: 2d2d 2d2d 2d2d 0a20 2020 2067 6574 5f72  ------.    get_r
-00002b20: 6573 756c 7473 2829 202d 3e20 5472 6169  esults() -> Trai
-00002b30: 6e47 7261 7068 3a0a 2020 2020 2020 2020  nGraph:.        
-00002b40: 5265 7475 726e 7320 7468 6520 7265 7375  Returns the resu
-00002b50: 6c74 7320 6f66 2074 6865 2074 7261 696e  lts of the train
-00002b60: 696e 6720 6a6f 622e 0a20 2020 2063 726f  ing job..    cro
-00002b70: 7373 7661 6c69 6461 7465 2829 3a0a 2020  ssvalidate():.  
-00002b80: 2020 2020 2020 5375 626d 6974 7320 6120        Submits a 
-00002b90: 6372 6f73 732d 7661 6c69 6461 7469 6f6e  cross-validation
-00002ba0: 206a 6f62 2061 6e64 2072 6574 7572 6e73   job and returns
-00002bb0: 2069 742e 0a20 2020 2072 1100 0000 7244   it..    r....rD
-00002bc0: 0000 004e da0f 6372 6f73 7376 616c 6964  ...N..crossvalid
-00002bd0: 6174 696f 6e72 5200 0000 6301 0000 0000  ationrR...c.....
-00002be0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00002bf0: 0000 0073 1000 0000 7400 7c00 6a01 7c00  ...s....t.|.j.|.
-00002c00: 6a02 6a03 8302 5300 2901 7a98 0a20 2020  j.j...S.).z..   
-00002c10: 2020 2020 2047 6574 7320 7468 6520 7265       Gets the re
-00002c20: 7375 6c74 7320 6f66 2074 6865 2074 7261  sults of the tra
-00002c30: 696e 696e 6720 6a6f 622e 0a0a 2020 2020  ining job...    
-00002c40: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00002c50: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00002c60: 2020 2020 5472 6169 6e47 7261 7068 0a20      TrainGraph. 
-00002c70: 2020 2020 2020 2020 2020 2054 6865 2072             The r
-00002c80: 6573 756c 7473 206f 6620 7468 6520 7472  esults of the tr
-00002c90: 6169 6e69 6e67 206a 6f62 2e0a 2020 2020  aining job..    
-00002ca0: 2020 2020 2904 7241 0000 0072 1100 0000      ).rA...r....
-00002cb0: 7244 0000 0072 1200 0000 7245 0000 0072  rD...r....rE...r
-00002cc0: 1b00 0000 721b 0000 0072 1c00 0000 da0b  ....r....r......
-00002cd0: 6765 745f 7265 7375 6c74 73c1 0100 0073  get_results....s
-00002ce0: 0200 0000 0009 7a1c 5472 6169 6e46 7574  ......z.TrainFut
-00002cf0: 7572 654d 6978 696e 2e67 6574 5f72 6573  ureMixin.get_res
-00002d00: 756c 7473 6301 0000 0000 0000 0000 0000  ultsc...........
-00002d10: 0001 0000 0003 0000 0043 0000 0073 2600  .........C...s&.
-00002d20: 0000 7c00 6a00 6401 6b08 721c 7401 7c00  ..|.j.d.k.r.t.|.
-00002d30: 6a02 7c00 6a03 6a04 8302 7c00 5f00 7c00  j.|.j.j...|._.|.
-00002d40: 6a00 a005 a100 5300 2902 6153 0100 000a  j.....S.).aS....
-00002d50: 2020 2020 2020 2020 5375 626d 6974 7320          Submits 
-00002d60: 6120 6372 6f73 732d 7661 6c69 6461 7469  a cross-validati
-00002d70: 6f6e 206a 6f62 2061 6e64 2062 696e 6473  on job and binds
-00002d80: 2069 742e 0a0a 2020 2020 2020 2020 4966   it...        If
-00002d90: 2061 2063 726f 7373 2d76 616c 6964 6174   a cross-validat
-00002da0: 696f 6e20 6a6f 6220 6861 7320 616c 7265  ion job has alre
-00002db0: 6164 7920 6265 656e 2063 7265 6174 6564  ady been created
-00002dc0: 2c20 6974 2072 6574 7572 6e73 2074 6861  , it returns tha
-00002dd0: 7420 6a6f 622e 0a20 2020 2020 2020 204f  t job..        O
-00002de0: 7468 6572 7769 7365 2c20 6974 2063 7265  therwise, it cre
-00002df0: 6174 6573 2061 206e 6577 2063 726f 7373  ates a new cross
-00002e00: 2d76 616c 6964 6174 696f 6e20 6a6f 6220  -validation job 
-00002e10: 616e 6420 7265 7475 726e 7320 6974 2e0a  and returns it..
-00002e20: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00002e30: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00002e40: 0a20 2020 2020 2020 2043 5646 7574 7572  .        CVFutur
-00002e50: 650a 2020 2020 2020 2020 2020 2020 5468  e.            Th
-00002e60: 6520 6372 6f73 732d 7661 6c69 6461 7469  e cross-validati
-00002e70: 6f6e 206a 6f62 2061 7373 6f63 6961 7465  on job associate
-00002e80: 6420 7769 7468 2074 6869 7320 7472 6169  d with this trai
-00002e90: 6e69 6e67 206a 6f62 2e0a 2020 2020 2020  ning job..      
-00002ea0: 2020 4e29 0672 6900 0000 724d 0000 0072    N).ri...rM...r
-00002eb0: 1100 0000 7244 0000 0072 1200 0000 7224  ....rD...r....r$
-00002ec0: 0000 0072 4500 0000 721b 0000 0072 1b00  ...rE...r....r..
-00002ed0: 0000 721c 0000 0072 2400 0000 cc01 0000  ..r....r$.......
-00002ee0: 7306 0000 0000 0c0a 0112 017a 1e54 7261  s..........z.Tra
-00002ef0: 696e 4675 7475 7265 4d69 7869 6e2e 6372  inFutureMixin.cr
-00002f00: 6f73 7376 616c 6964 6174 6563 0100 0000  ossvalidatec....
-00002f10: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00002f20: 4300 0000 730c 0000 0074 0064 0183 0182  C...s....t.d....
-00002f30: 0164 0253 0029 03fa 870a 2020 2020 2020  .d.S.)....      
-00002f40: 2020 4e4f 5420 494d 504c 454d 454e 5445    NOT IMPLEMENTE
-00002f50: 442e 0a0a 2020 2020 2020 2020 4765 7420  D...        Get 
-00002f60: 7468 6520 6173 7361 7920 6461 7461 2075  the assay data u
-00002f70: 7365 6420 666f 7220 7468 6520 7472 6169  sed for the trai
-00002f80: 6e69 6e67 206a 6f62 2e0a 0a20 2020 2020  ning job...     
-00002f90: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002fa0: 2020 2020 2020 2020 5468 6520 6173 7361          The assa
-00002fb0: 7920 6461 7461 2e0a 2020 2020 2020 2020  y data..        
-00002fc0: 7a20 6765 745f 6173 7361 795f 6461 7461  z get_assay_data
-00002fd0: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-00002fe0: 652e 4e29 01da 134e 6f74 496d 706c 656d  e.N)...NotImplem
-00002ff0: 656e 7465 6445 7272 6f72 7245 0000 0072  entedErrorrE...r
-00003000: 1b00 0000 721b 0000 0072 1c00 0000 da0e  ....r....r......
-00003010: 6765 745f 6173 7361 795f 6461 7461 dc01  get_assay_data..
-00003020: 0000 7302 0000 0000 097a 1f54 7261 696e  ..s......z.Train
-00003030: 4675 7475 7265 4d69 7869 6e2e 6765 745f  FutureMixin.get_
-00003040: 6173 7361 795f 6461 7461 6301 0000 0000  assay_datac.....
-00003050: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00003060: 0000 0073 1000 0000 7400 7c00 6a01 7c00  ...s....t.|.j.|.
-00003070: 6a02 6a03 8302 5300 2901 6118 0100 000a  j.j...S.).a.....
-00003080: 2020 2020 2020 2020 4c69 7374 206d 6f64          List mod
-00003090: 656c 7320 6173 736f 6963 6174 6564 2077  els assoicated w
-000030a0: 6974 6820 6a6f 620a 0a20 2020 2020 2020  ith job..       
-000030b0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000030c0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000030d0: 2020 2020 2020 2073 6573 7369 6f6e 203a         session :
-000030e0: 2041 5049 5365 7373 696f 6e0a 2020 2020   APISession.    
-000030f0: 2020 2020 2020 2020 5365 7373 696f 6e20          Session 
-00003100: 6f62 6a65 6374 2066 6f72 2041 5049 2063  object for API c
-00003110: 6f6d 6d75 6e69 6361 7469 6f6e 2e0a 2020  ommunication..  
-00003120: 2020 2020 2020 6a6f 625f 6964 203a 2073        job_id : s
-00003130: 7472 0a20 2020 2020 2020 2020 2020 206a  tr.            j
-00003140: 6f62 2049 440a 0a20 2020 2020 2020 2052  ob ID..        R
-00003150: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00003160: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204c  ------.        L
-00003170: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-00003180: 4c69 7374 206f 6620 6d6f 6465 6c73 0a20  List of models. 
-00003190: 2020 2020 2020 2029 0472 1d00 0000 7211         ).r....r.
-000031a0: 0000 0072 4400 0000 7212 0000 0072 4500  ...rD...r....rE.
-000031b0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000031c0: 0072 1d00 0000 e701 0000 7302 0000 0000  .r........s.....
-000031d0: 107a 1c54 7261 696e 4675 7475 7265 4d69  .z.TrainFutureMi
-000031e0: 7869 6e2e 6c69 7374 5f6d 6f64 656c 7329  xin.list_models)
-000031f0: 0e72 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
-00003200: 724a 0000 0072 0500 0000 724b 0000 0072  rJ...r....rK...r
-00003210: 0700 0000 7269 0000 0072 4d00 0000 7208  ....ri...rM...r.
-00003220: 0000 0072 6a00 0000 7224 0000 0072 6d00  ...rj...r$...rm.
-00003230: 0000 721d 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00003240: 0072 1b00 0000 721c 0000 0072 6800 0000  .r....r....rh...
-00003250: a701 0000 7310 0000 000a 0104 1508 0108  ....s...........
-00003260: 010c 020e 0b08 1008 0b72 6800 0000 6300  .........rh...c.
-00003270: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-00003280: 0000 0000 0000 0073 7200 0000 6500 5a01  .......sr...e.Z.
-00003290: 6400 5a02 6401 5a03 6413 6504 6505 6506  d.Z.d.Z.d.e.e.e.
-000032a0: 6507 1900 6403 9c03 8700 6601 6404 6405  e...d.....f.d.d.
-000032b0: 840d 5a08 6509 6406 9c01 6407 6408 8404  ..Z.e.d...d.d...
-000032c0: 5a0a 6509 6406 9c01 6409 640a 8404 5a0b  Z.e.d...d.d...Z.
-000032d0: 650c 640b 640c 8400 8301 5a0d 640d 640e  e.d.d.....Z.d.d.
-000032e0: 8400 5a0e 6414 650f 6510 6410 9c02 6411  ..Z.d.e.e.d...d.
-000032f0: 6412 8405 5a11 8700 0400 5a12 5300 2915  d...Z.....Z.S.).
-00003300: da0b 5472 6169 6e46 7574 7572 657a 2346  ..TrainFuturez#F
-00003310: 7574 7572 6520 4a6f 6220 666f 7220 6d61  uture Job for ma
-00003320: 6e69 7075 6c61 7469 6e67 2072 6573 756c  nipulating resul
-00003330: 7473 4e29 0372 1100 0000 7244 0000 00da  tsN).r....rD....
-00003340: 0d61 7373 6179 6d65 7461 6461 7461 6304  .assaymetadatac.
-00003350: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00003360: 0000 0003 0000 0073 2800 0000 7400 8300  .......s(...t...
-00003370: a001 7c01 7c02 a102 0100 7c03 7c00 5f02  ..|.|.....|.|._.
-00003380: 7403 7c01 7c02 6a04 6400 8303 7c00 5f05  t.|.|.j.d...|._.
-00003390: 6400 5300 7253 0000 0029 0672 4e00 0000  d.S.rS...).rN...
-000033a0: 724f 0000 0072 6f00 0000 724d 0000 0072  rO...ro...rM...r
-000033b0: 1200 0000 7269 0000 0029 0472 4600 0000  ....ri...).rF...
-000033c0: 7211 0000 0072 4400 0000 726f 0000 0072  r....rD...ro...r
-000033d0: 5000 0000 721b 0000 0072 1c00 0000 724f  P...r....r....rO
-000033e0: 0000 00fc 0100 0073 0600 0000 0006 0e01  .......s........
-000033f0: 0601 7a14 5472 6169 6e46 7574 7572 652e  ..z.TrainFuture.
-00003400: 5f5f 696e 6974 5f5f 7252 0000 0063 0100  __init__rR...c..
-00003410: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00003420: 0000 4300 0000 730a 0000 0074 007c 006a  ..C...s....t.|.j
-00003430: 0183 0153 0072 5300 0000 7254 0000 0072  ...S.rS...rT...r
-00003440: 4500 0000 721b 0000 0072 1b00 0000 721c  E...r....r....r.
-00003450: 0000 0072 5500 0000 0602 0000 7302 0000  ...rU.......s...
-00003460: 0000 017a 1354 7261 696e 4675 7475 7265  ...z.TrainFuture
-00003470: 2e5f 5f73 7472 5f5f 6301 0000 0000 0000  .__str__c.......
-00003480: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00003490: 0073 0a00 0000 7400 7c00 6a01 8301 5300  .s....t.|.j...S.
-000034a0: 7253 0000 0072 5600 0000 7245 0000 0072  rS...rV...rE...r
-000034b0: 1b00 0000 721b 0000 0072 1c00 0000 7258  ....r....r....rX
-000034c0: 0000 0009 0200 0073 0200 0000 0001 7a14  .......s......z.
-000034d0: 5472 6169 6e46 7574 7572 652e 5f5f 7265  TrainFuture.__re
-000034e0: 7072 5f5f 6301 0000 0000 0000 0000 0000  pr__c...........
-000034f0: 0001 0000 0001 0000 0043 0000 0073 0800  .........C...s..
-00003500: 0000 7c00 6a00 6a01 5300 7253 0000 0072  ..|.j.j.S.rS...r
-00003510: 5900 0000 7245 0000 0072 1b00 0000 721b  Y...rE...r....r.
-00003520: 0000 0072 1c00 0000 7236 0000 000c 0200  ...r....r6......
-00003530: 0073 0200 0000 0002 7a0e 5472 6169 6e46  .s......z.TrainF
-00003540: 7574 7572 652e 6964 6301 0000 0000 0000  uture.idc.......
-00003550: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00003560: 0073 0800 0000 7c00 a000 a100 5300 2901  .s....|.....S.).
-00003570: 726b 0000 0029 0172 6d00 0000 7245 0000  rk...).rm...rE..
-00003580: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00003590: 726d 0000 0010 0200 0073 0200 0000 0009  rm.......s......
-000035a0: 7a1a 5472 6169 6e46 7574 7572 652e 6765  z.TrainFuture.ge
-000035b0: 745f 6173 7361 795f 6461 7461 4672 5a00  t_assay_dataFrZ.
-000035c0: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
-000035d0: 0000 000a 0000 0043 0000 0073 4a00 0000  .......C...sJ...
-000035e0: 7a0c 7c00 a000 a100 7d02 5700 6e38 0400  z.|.....}.W.n8..
-000035f0: 7401 6b0a 7244 0100 7d03 0100 7a1a 7c01  t.k.rD..}...z.|.
-00003600: 7230 7402 6401 7c03 9b00 9d02 8301 0100  r0t.d.|.........
-00003610: 7c03 8201 5700 3500 6400 7d03 7e03 5800  |...W.5.d.}.~.X.
-00003620: 5900 6e02 5800 7c02 5300 2902 4e72 5c00  Y.n.X.|.S.).Nr\.
-00003630: 0000 2903 726a 0000 0072 0d00 0000 725f  ..).rj...r....r_
-00003640: 0000 0029 0472 4600 0000 725b 0000 0072  ...).rF...r[...r
-00003650: 6100 0000 7264 0000 0072 1b00 0000 721b  a...rd...r....r.
-00003660: 0000 0072 1c00 0000 7216 0000 001b 0200  ...r....r.......
-00003670: 0073 0e00 0000 0001 0201 0c01 1001 0401  .s..............
-00003680: 0e01 1601 7a0f 5472 6169 6e46 7574 7572  ....z.TrainFutur
-00003690: 652e 6765 7429 014e 2901 4629 1372 4700  e.get).N).F).rG.
-000036a0: 0000 7248 0000 0072 4900 0000 724a 0000  ..rH...rI...rJ..
-000036b0: 0072 0500 0000 7207 0000 0072 0200 0000  .r....r....r....
-000036c0: 7210 0000 0072 4f00 0000 7233 0000 0072  r....rO...r3...r
-000036d0: 5500 0000 7258 0000 0072 6500 0000 7236  U...rX...re...r6
-000036e0: 0000 0072 6d00 0000 7266 0000 0072 0800  ...rm...rf...r..
-000036f0: 0000 7216 0000 0072 6700 0000 721b 0000  ..r....rg...r...
-00003700: 0072 1b00 0000 7250 0000 0072 1c00 0000  .r....rP...r....
-00003710: 726e 0000 00fa 0100 0073 1a00 0000 0801  rn.......s......
-00003720: 0405 00fc 0202 0201 0201 06fc 100a 0e03  ................
-00003730: 0e03 0201 0a03 080b 726e 0000 0063 0000  ........rn...c..
-00003740: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-00003750: 0000 4000 0000 73b6 0000 0065 005a 0164  ..@...s....e.Z.d
-00003760: 005a 0264 015a 0365 0464 029c 0164 0364  .Z.d.Z.e.d...d.d
-00003770: 0484 045a 0564 1465 0665 0765 0865 0965  ...Z.d.e.e.e.e.e
-00003780: 0819 0066 0219 0065 0865 0a65 0b19 0065  ...f...e.e.e...e
-00003790: 0c64 079c 0564 0864 0984 055a 0d64 1565  .d...d.d...Z.d.e
-000037a0: 0665 0765 0865 0965 0819 0066 0219 0065  .e.e.e.e...f...e
-000037b0: 0865 0a65 0b19 0065 0c64 079c 0564 0a64  .e.e...e.d...d.d
-000037c0: 0b84 055a 0e64 1665 0665 0765 0865 0965  ...Z.d.e.e.e.e.e
-000037d0: 0819 0066 0219 0065 0865 0a65 0b19 0065  ...f...e.e.e...e
-000037e0: 0c64 079c 0564 0c64 0d84 055a 0f65 0865  .d...d.d...Z.e.e
-000037f0: 0c64 0e9c 0264 0f64 1084 045a 1065 0865  .d...d.d...Z.e.e
-00003800: 1164 0e9c 0264 1164 1284 045a 1264 1353  .d...d.d...Z.d.S
-00003810: 0029 17da 0b54 7261 696e 696e 6741 5049  .)...TrainingAPI
-00003820: 7a29 4150 4920 696e 7465 7266 6163 6520  z)API interface 
-00003830: 666f 7220 6361 6c6c 696e 6720 5472 6169  for calling Trai
-00003840: 6e20 656e 6470 6f69 6e74 7329 0172 1100  n endpoints).r..
-00003850: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00003860: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-00003870: 7c01 7c00 5f00 6400 7c00 5f01 6400 5300  |.|._.d.|._.d.S.
-00003880: 7253 0000 0029 0272 1100 0000 5a05 6173  rS...).r....Z.as
-00003890: 7361 7929 0272 4600 0000 7211 0000 0072  say).rF...r....r
-000038a0: 1b00 0000 721b 0000 0072 1c00 0000 724f  ....r....r....rO
-000038b0: 0000 0027 0200 0073 0400 0000 0004 0601  ...'...s........
-000038c0: 7a14 5472 6169 6e69 6e67 4150 492e 5f5f  z.TrainingAPI.__
-000038d0: 696e 6974 5f5f 722a 0000 0046 2905 722b  init__r*...F).r+
-000038e0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-000038f0: 0000 7213 0000 0063 0500 0000 0000 0000  ..r....c........
-00003900: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
-00003910: 7330 0000 0074 007c 0274 0183 0272 107c  s0...t.|.t...r.|
-00003920: 0267 017d 0274 027c 006a 037c 017c 027c  .g.}.t.|.j.|.|.|
-00003930: 037c 0483 057d 0574 047c 006a 037c 057c  .|...}.t.|.j.|.|
-00003940: 0183 0353 0029 0161 0004 0000 0a20 2020  ...S.).a.....   
-00003950: 2020 2020 2043 7265 6174 6520 6120 7472       Create a tr
-00003960: 6169 6e69 6e67 206a 6f62 206f 6e20 796f  aining job on yo
-00003970: 7572 2064 6174 612e 0a0a 2020 2020 2020  ur data...      
-00003980: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00003990: 7661 6c69 6461 7465 7320 7468 6520 696e  validates the in
-000039a0: 7075 7473 2c20 666f 726d 6174 7320 7468  puts, formats th
-000039b0: 6520 6461 7461 2c20 616e 6420 7365 6e64  e data, and send
-000039c0: 7320 7468 6520 6a6f 622e 0a0a 2020 2020  s the job...    
-000039d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000039e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000039f0: 2d0a 2020 2020 2020 2020 6173 7361 7964  -.        assayd
-00003a00: 6174 6173 6574 203a 2041 7373 6179 4461  ataset : AssayDa
-00003a10: 7461 7365 740a 2020 2020 2020 2020 2020  taset.          
-00003a20: 2020 416e 2041 7373 6179 4461 7461 7365    An AssayDatase
-00003a30: 7420 6f62 6a65 6374 2066 726f 6d20 7768  t object from wh
-00003a40: 6963 6820 7468 6520 6173 7361 795f 6964  ich the assay_id
-00003a50: 2069 7320 6578 7472 6163 7465 642e 0a20   is extracted.. 
-00003a60: 2020 2020 2020 206d 6561 7375 7265 6d65         measureme
-00003a70: 6e74 5f6e 616d 6520 3a20 7374 7220 6f72  nt_name : str or
-00003a80: 204c 6973 745b 7374 725d 0a20 2020 2020   List[str].     
-00003a90: 2020 2020 2020 2054 6865 206e 616d 6528         The name(
-00003aa0: 7329 206f 6620 7468 6520 6d65 6173 7572  s) of the measur
-00003ab0: 656d 656e 7428 7329 2074 6f20 6265 2075  ement(s) to be u
-00003ac0: 7365 6420 696e 2074 6865 2074 7261 696e  sed in the train
-00003ad0: 696e 6720 6a6f 622e 0a20 2020 2020 2020  ing job..       
-00003ae0: 206d 6f64 656c 5f6e 616d 6520 3a20 7374   model_name : st
-00003af0: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
-00003b00: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
-00003b10: 2074 6f20 6769 7665 2074 6865 206d 6f64   to give the mod
-00003b20: 656c 2e0a 2020 2020 2020 2020 666f 7263  el..        forc
-00003b30: 655f 7072 6570 726f 6365 7373 203a 2062  e_preprocess : b
-00003b40: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-00003b50: 2020 2020 2020 2020 2020 4966 2073 6574            If set
-00003b60: 2074 6f20 5472 7565 2c20 7072 6570 726f   to True, prepro
-00003b70: 6365 7373 696e 6720 6973 2066 6f72 6365  cessing is force
-00003b80: 6420 6576 656e 2069 6620 6461 7461 2061  d even if data a
-00003b90: 6c72 6561 6479 2065 7869 7374 732e 0a0a  lready exists...
-00003ba0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00003bb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00003bc0: 2020 2020 2020 2020 5472 6169 6e46 7574          TrainFut
-00003bd0: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
-00003be0: 4120 5472 6169 6e46 7574 7572 6520 4a6f  A TrainFuture Jo
-00003bf0: 620a 0a20 2020 2020 2020 2052 6169 7365  b..        Raise
-00003c00: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00003c10: 0a20 2020 2020 2020 2049 6e76 616c 6964  .        Invalid
-00003c20: 5061 7261 6d65 7465 7245 7272 6f72 0a20  ParameterError. 
-00003c30: 2020 2020 2020 2020 2020 2049 6620 7468             If th
-00003c40: 6520 6061 7373 6179 6461 7461 7365 7460  e `assaydataset`
-00003c50: 2069 7320 6e6f 7420 616e 2041 7373 6179   is not an Assay
-00003c60: 4461 7461 7365 7420 6f62 6a65 6374 2c0a  Dataset object,.
-00003c70: 2020 2020 2020 2020 2020 2020 4966 2061              If a
-00003c80: 6e79 206d 6561 7375 7265 6d65 6e74 206e  ny measurement n
-00003c90: 616d 6520 7072 6f76 6964 6564 2064 6f65  ame provided doe
-00003ca0: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
-00003cb0: 6865 2041 7373 6179 4461 7461 7365 742c  he AssayDataset,
-00003cc0: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
-00003cd0: 6966 2074 6865 2041 7373 6179 4461 7461  if the AssayData
-00003ce0: 7365 7420 6861 7320 6665 7765 7220 7468  set has fewer th
-00003cf0: 616e 2033 2064 6174 6120 706f 696e 7473  an 3 data points
-00003d00: 2e0a 2020 2020 2020 2020 4854 5450 4572  ..        HTTPEr
-00003d10: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-00003d20: 4966 2074 6865 2072 6571 7565 7374 2074  If the request t
-00003d30: 6f20 7468 6520 7365 7276 6572 2066 6169  o the server fai
-00003d40: 6c73 2e0a 2020 2020 2020 2020 2905 7232  ls..        ).r2
-00003d50: 0000 0072 3300 0000 723d 0000 0072 1100  ...r3...r=...r..
-00003d60: 0000 726e 0000 00a9 0672 4600 0000 722b  ..rn.....rF...r+
-00003d70: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00003d80: 0000 da0b 6a6f 625f 6465 7461 696c 7372  ....job_detailsr
-00003d90: 1b00 0000 721b 0000 0072 1c00 0000 da13  ....r....r......
-00003da0: 6372 6561 7465 5f74 7261 696e 696e 675f  create_training_
-00003db0: 6a6f 622e 0200 0073 1400 0000 0025 0a01  job....s.....%..
-00003dc0: 0601 0201 0400 0200 0200 0200 02ff 0403  ................
-00003dd0: 7a1f 5472 6169 6e69 6e67 4150 492e 6372  z.TrainingAPI.cr
-00003de0: 6561 7465 5f74 7261 696e 696e 675f 6a6f  eate_training_jo
-00003df0: 6263 0500 0000 0000 0000 0000 0000 0600  bc..............
-00003e00: 0000 0600 0000 4300 0000 7320 0000 0074  ......C...s ...t
-00003e10: 007c 006a 017c 017c 027c 037c 0483 057d  .|.j.|.|.|.|...}
-00003e20: 0574 027c 006a 017c 057c 0183 0353 00a9  .t.|.j.|.|...S..
-00003e30: 017a 1c53 616d 6520 6173 2063 7265 6174  .z.Same as creat
-00003e40: 655f 7472 6169 6e69 6e67 5f6a 6f62 2e29  e_training_job.)
-00003e50: 0372 3f00 0000 7211 0000 0072 6e00 0000  .r?...r....rn...
-00003e60: 7271 0000 0072 1b00 0000 721b 0000 0072  rq...r....r....r
-00003e70: 1c00 0000 da17 5f63 7265 6174 655f 7472  ......_create_tr
-00003e80: 6169 6e69 6e67 5f6a 6f62 5f62 725a 0200  aining_job_brZ..
-00003e90: 0073 1000 0000 0008 0201 0400 0200 0200  .s..............
-00003ea0: 0200 02ff 0403 7a23 5472 6169 6e69 6e67  ......z#Training
-00003eb0: 4150 492e 5f63 7265 6174 655f 7472 6169  API._create_trai
-00003ec0: 6e69 6e67 5f6a 6f62 5f62 7263 0500 0000  ning_job_brc....
-00003ed0: 0000 0000 0000 0000 0600 0000 0600 0000  ................
-00003ee0: 4300 0000 7320 0000 0074 007c 006a 017c  C...s ...t.|.j.|
-00003ef0: 017c 027c 037c 0483 057d 0574 027c 006a  .|.|.|...}.t.|.j
-00003f00: 017c 057c 0183 0353 0072 7400 0000 2903  .|.|...S.rt...).
-00003f10: 7240 0000 0072 1100 0000 726e 0000 0072  r@...r....rn...r
-00003f20: 7100 0000 721b 0000 0072 1b00 0000 721c  q...r....r....r.
-00003f30: 0000 00da 175f 6372 6561 7465 5f74 7261  ....._create_tra
-00003f40: 696e 696e 675f 6a6f 625f 6770 6702 0000  ining_job_gpg...
-00003f50: 7310 0000 0000 0802 0104 0002 0002 0002  s...............
-00003f60: 0002 ff04 037a 2354 7261 696e 696e 6741  .....z#TrainingA
-00003f70: 5049 2e5f 6372 6561 7465 5f74 7261 696e  PI._create_train
-00003f80: 696e 675f 6a6f 625f 6770 2902 7212 0000  ing_job_gp).r...
-00003f90: 0072 1300 0000 6302 0000 0000 0000 0000  .r....c.........
-00003fa0: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00003fb0: 1800 0000 7400 7c00 6a01 7c01 8302 7d02  ....t.|.j.|...}.
-00003fc0: 7402 7c00 6a01 7c02 8302 5300 2901 7ae1  t.|.j.|...S.).z.
-00003fd0: 0a20 2020 2020 2020 2047 6574 2074 7261  .        Get tra
-00003fe0: 696e 696e 6720 7265 7375 6c74 7320 2865  ining results (e
-00003ff0: 2e67 2e20 6c6f 7373 2065 7463 292e 0a0a  .g. loss etc)...
-00004000: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00004010: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00004020: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6a6f  -----.        jo
-00004030: 625f 6964 203a 2073 7472 0a20 2020 2020  b_id : str.     
-00004040: 2020 2020 2020 206a 6f62 5f69 6420 746f         job_id to
-00004050: 2067 6574 0a0a 0a20 2020 2020 2020 2052   get...        R
-00004060: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00004070: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
-00004080: 7261 696e 4675 7475 7265 0a20 2020 2020  rainFuture.     
-00004090: 2020 2020 2020 2041 2054 7261 696e 4675         A TrainFu
-000040a0: 7475 7265 204a 6f62 0a20 2020 2020 2020  ture Job.       
-000040b0: 2029 0372 4100 0000 7211 0000 0072 6e00   ).rA...r....rn.
-000040c0: 0000 2903 7246 0000 0072 1200 0000 7272  ..).rF...r....rr
-000040d0: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-000040e0: 0000 7241 0000 0074 0200 0073 0400 0000  ..rA...t...s....
-000040f0: 000f 0c01 7a20 5472 6169 6e69 6e67 4150  ....z TrainingAP
-00004100: 492e 6765 745f 7472 6169 6e69 6e67 5f72  I.get_training_r
-00004110: 6573 756c 7473 6302 0000 0000 0000 0000  esultsc.........
-00004120: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-00004130: 4000 0000 7400 7c00 6a01 7c01 8302 7d02  @...t.|.j.|...}.
-00004140: 6401 7d03 7c02 6a02 7403 6a04 6b03 7232  d.}.|.j.t.j.k.r2
-00004150: 7405 6402 7c01 9b00 6403 7403 6a04 9b00  t.d.|...d.t.j...
-00004160: 9d04 8301 8201 7406 7c00 6a01 7c02 7c03  ......t.|.j.|.|.
-00004170: 8303 5300 2904 61ac 0100 000a 2020 2020  ..S.).a.....    
-00004180: 2020 2020 5265 6c6f 6164 2061 2053 7562      Reload a Sub
-00004190: 6d69 7474 6564 206a 6f62 2074 6f20 7265  mitted job to re
-000041a0: 7375 6d65 2066 726f 6d20 7768 6572 6520  sume from where 
-000041b0: 796f 7520 6c65 6674 206f 6666 210a 0a0a  you left off!...
-000041c0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000041d0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000041e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6a6f  -----.        jo
-000041f0: 625f 6964 203a 2073 7472 0a20 2020 2020  b_id : str.     
-00004200: 2020 2020 2020 2054 6865 2069 6465 6e74         The ident
-00004210: 6966 6965 7220 6f66 2074 6865 206a 6f62  ifier of the job
-00004220: 2077 686f 7365 2064 6574 6169 6c73 2061   whose details a
-00004230: 7265 2074 6f20 6265 206c 6f61 6465 642e  re to be loaded.
-00004240: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00004250: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00004260: 2d0a 2020 2020 2020 2020 4a6f 620a 2020  -.        Job.  
-00004270: 2020 2020 2020 2020 2020 4a6f 620a 0a20            Job.. 
-00004280: 2020 2020 2020 2052 6169 7365 730a 2020         Raises.  
-00004290: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-000042a0: 2020 2020 2048 5454 5045 7272 6f72 0a20       HTTPError. 
-000042b0: 2020 2020 2020 2020 2020 2049 6620 7468             If th
-000042c0: 6520 7265 7175 6573 7420 746f 2074 6865  e request to the
-000042d0: 2073 6572 7665 7220 6661 696c 732e 0a20   server fails.. 
-000042e0: 2020 2020 2020 2049 6e76 616c 6964 4a6f         InvalidJo
-000042f0: 620a 2020 2020 2020 2020 2020 2020 4966  b.            If
-00004300: 2074 6865 204a 6f62 2069 7320 6f66 2074   the Job is of t
-00004310: 6865 2077 726f 6e67 2074 7970 650a 0a20  he wrong type.. 
-00004320: 2020 2020 2020 204e 7a04 4a6f 6220 7a10         Nz.Job z.
-00004330: 2069 7320 6e6f 7420 6f66 2074 7970 6520   is not of type 
-00004340: 2907 7242 0000 0072 1100 0000 da08 6a6f  ).rB...r......jo
-00004350: 625f 7479 7065 7209 0000 00da 0574 7261  b_typer......tra
-00004360: 696e 720e 0000 0072 6e00 0000 2904 7246  inr....rn...).rF
-00004370: 0000 0072 1200 0000 7272 0000 005a 0e61  ...r....rr...Z.a
-00004380: 7373 6179 5f6d 6574 6164 6174 6172 1b00  ssay_metadatar..
-00004390: 0000 721b 0000 0072 1c00 0000 7242 0000  ..r....r....rB..
-000043a0: 0086 0200 0073 0a00 0000 0017 0c01 0402  .....s..........
-000043b0: 0c01 1601 7a14 5472 6169 6e69 6e67 4150  ....z.TrainingAP
-000043c0: 492e 6c6f 6164 5f6a 6f62 4e29 0272 2a00  I.load_jobN).r*.
-000043d0: 0000 4629 0272 2a00 0000 4629 0272 2a00  ..F).r*...F).r*.
-000043e0: 0000 4629 1372 4700 0000 7248 0000 0072  ..F).rG...rH...r
-000043f0: 4900 0000 724a 0000 0072 0500 0000 724f  I...rJ...r....rO
-00004400: 0000 0072 0f00 0000 7204 0000 0072 3300  ...r....r....r3.
-00004410: 0000 7203 0000 0072 0200 0000 7266 0000  ..r....r....rf..
-00004420: 0072 6e00 0000 7273 0000 0072 7500 0000  .rn...rs...ru...
-00004430: 7276 0000 0072 4100 0000 720a 0000 0072  rv...rA...r....r
-00004440: 4200 0000 721b 0000 0072 1b00 0000 721b  B...r....r....r.
-00004450: 0000 0072 1c00 0000 7270 0000 0025 0200  ...r....rp...%..
-00004460: 0073 4000 0000 0801 0403 02fe 0c0b 0001  .s@.............
-00004470: 00fb 0202 0201 0e01 0201 0601 02fa 0c30  ...............0
-00004480: 0001 00fb 0202 0201 0e01 0201 0601 02fa  ................
-00004490: 0c11 0001 00fb 0202 0201 0e01 0201 0601  ................
-000044a0: 02fa 0c0d 1012 7270 0000 0029 0172 1e00  ......rp...).r..
-000044b0: 0000 2902 4e72 0100 0000 2902 722a 0000  ..).Nr....).r*..
-000044c0: 0046 2902 722a 0000 0046 2902 722a 0000  .F).r*...F).r*..
-000044d0: 0046 2902 722a 0000 0046 2927 da06 7479  .F).r*...F)'..ty
-000044e0: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
-000044f0: 0000 0072 2200 0000 da17 6f70 656e 7072  ...r".....openpr
-00004500: 6f74 6569 6e5f 7079 7468 6f6e 2e62 6173  otein_python.bas
-00004510: 6572 0500 0000 da1b 6f70 656e 7072 6f74  er......openprot
-00004520: 6569 6e5f 7079 7468 6f6e 2e61 7069 2e6a  ein_python.api.j
-00004530: 6f62 7372 0600 0000 7207 0000 00da 196f  obsr....r......o
-00004540: 7065 6e70 726f 7465 696e 5f70 7974 686f  penprotein_pytho
-00004550: 6e2e 6d6f 6465 6c73 7208 0000 0072 0900  n.modelsr....r..
-00004560: 0000 720a 0000 0072 0b00 0000 da19 6f70  ..r....r......op
-00004570: 656e 7072 6f74 6569 6e5f 7079 7468 6f6e  enprotein_python
-00004580: 2e65 7272 6f72 7372 0c00 0000 720d 0000  .errorsr....r...
-00004590: 0072 0e00 0000 da1b 6f70 656e 7072 6f74  .r......openprot
-000045a0: 6569 6e5f 7079 7468 6f6e 2e61 7069 2e64  ein_python.api.d
-000045b0: 6174 6172 0f00 0000 7210 0000 0072 3300  atar....r....r3.
-000045c0: 0000 721d 0000 0072 4c00 0000 7224 0000  ..r....rL...r$..
-000045d0: 0072 2900 0000 7266 0000 0072 3a00 0000  .r)...rf...r:...
-000045e0: 723d 0000 0072 3f00 0000 7240 0000 0072  r=...r?...r@...r
-000045f0: 4100 0000 7242 0000 0072 4300 0000 724d  A...rB...rC...rM
-00004600: 0000 0072 6800 0000 726e 0000 0072 7000  ...rh...rn...rp.
-00004610: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00004620: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00004630: 0100 0000 737c 0000 0014 0108 010c 0110  ....s|..........
-00004640: 0218 0114 0110 0312 1516 1600 0100 fc02  ................
-00004650: 0102 0102 0106 0106 0102 fb0c 1d00 0100  ................
-00004660: fa02 0102 0102 0102 010e 0102 0106 0102  ................
-00004670: f90c 4900 0100 fb02 0102 0102 010e 0102  ..I.............
-00004680: 0106 fb0c 3500 0100 fb02 0102 0102 010e  ....5...........
-00004690: 0102 0106 fb0c 1200 0100 fb02 0102 0102  ................
-000046a0: 010e 0102 0106 fb0c 0e12 0712 1c0e 5412  ..............T.
-000046b0: 530e 5312 2b                             S.S.+
+00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000010: 7274 204f 7074 696f 6e61 6c2c 204c 6973  rt Optional, Lis
+00000020: 742c 2055 6e69 6f6e 0a69 6d70 6f72 7420  t, Union.import 
+00000030: 7079 6461 6e74 6963 0a66 726f 6d20 6f70  pydantic.from op
+00000040: 656e 7072 6f74 6569 6e2e 6261 7365 2069  enprotein.base i
+00000050: 6d70 6f72 7420 4150 4953 6573 7369 6f6e  mport APISession
+00000060: 0a66 726f 6d20 6f70 656e 7072 6f74 6569  .from openprotei
+00000070: 6e2e 6170 692e 6a6f 6273 2069 6d70 6f72  n.api.jobs impor
+00000080: 7420 4173 796e 634a 6f62 4675 7475 7265  t AsyncJobFuture
+00000090: 2c20 4a6f 620a 0a66 726f 6d20 6f70 656e  , Job..from open
+000000a0: 7072 6f74 6569 6e2e 6d6f 6465 6c73 2069  protein.models i
+000000b0: 6d70 6f72 7420 5472 6169 6e47 7261 7068  mport TrainGraph
+000000c0: 2c20 4a6f 6254 7970 652c 204a 6f62 706c  , JobType, Jobpl
+000000d0: 7573 2c20 4356 5265 7375 6c74 730a 6672  us, CVResults.fr
+000000e0: 6f6d 206f 7065 6e70 726f 7465 696e 2e65  om openprotein.e
+000000f0: 7272 6f72 7320 696d 706f 7274 2049 6e76  rrors import Inv
+00000100: 616c 6964 5061 7261 6d65 7465 7245 7272  alidParameterErr
+00000110: 6f72 2c20 4150 4945 7272 6f72 2c20 496e  or, APIError, In
+00000120: 7661 6c69 644a 6f62 0a66 726f 6d20 6f70  validJob.from op
+00000130: 656e 7072 6f74 6569 6e2e 6170 692e 6461  enprotein.api.da
+00000140: 7461 2069 6d70 6f72 7420 4173 7361 7944  ta import AssayD
+00000150: 6174 6173 6574 2c20 4173 7361 794d 6574  ataset, AssayMet
+00000160: 6164 6174 610a 0a0a 6465 6620 6c69 7374  adata...def list
+00000170: 5f6d 6f64 656c 7328 7365 7373 696f 6e3a  _models(session:
+00000180: 2041 5049 5365 7373 696f 6e2c 206a 6f62   APISession, job
+00000190: 5f69 643a 2073 7472 2920 2d3e 204c 6973  _id: str) -> Lis
+000001a0: 743a 0a20 2020 2022 2222 0a20 2020 204c  t:.    """.    L
+000001b0: 6973 7420 6d6f 6465 6c73 2061 7373 6f69  ist models assoi
+000001c0: 6361 7465 6420 7769 7468 206a 6f62 0a0a  cated with job..
+000001d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000001e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000001f0: 2020 7365 7373 696f 6e20 3a20 4150 4953    session : APIS
+00000200: 6573 7369 6f6e 0a20 2020 2020 2020 2053  ession.        S
+00000210: 6573 7369 6f6e 206f 626a 6563 7420 666f  ession object fo
+00000220: 7220 4150 4920 636f 6d6d 756e 6963 6174  r API communicat
+00000230: 696f 6e2e 0a20 2020 206a 6f62 5f69 6420  ion..    job_id 
+00000240: 3a20 7374 720a 2020 2020 2020 2020 6a6f  : str.        jo
+00000250: 6220 4944 0a0a 2020 2020 5265 7475 726e  b ID..    Return
+00000260: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00000270: 2020 4c69 7374 0a20 2020 2020 2020 204c    List.        L
+00000280: 6973 7420 6f66 206d 6f64 656c 730a 2020  ist of models.  
+00000290: 2020 2222 220a 2020 2020 656e 6470 6f69    """.    endpoi
+000002a0: 6e74 203d 2022 7631 2f6d 6f64 656c 7322  nt = "v1/models"
+000002b0: 0a20 2020 2072 6573 706f 6e73 6520 3d20  .    response = 
+000002c0: 7365 7373 696f 6e2e 6765 7428 656e 6470  session.get(endp
+000002d0: 6f69 6e74 2c20 7061 7261 6d73 3d7b 226a  oint, params={"j
+000002e0: 6f62 5f69 6422 3a20 6a6f 625f 6964 7d29  ob_id": job_id})
+000002f0: 0a20 2020 2072 6574 7572 6e20 7265 7370  .    return resp
+00000300: 6f6e 7365 2e6a 736f 6e28 290a 0a0a 6465  onse.json()...de
+00000310: 6620 6372 6f73 7376 616c 6964 6174 6528  f crossvalidate(
+00000320: 7365 7373 696f 6e3a 2041 5049 5365 7373  session: APISess
+00000330: 696f 6e2c 2074 7261 696e 5f6a 6f62 5f69  ion, train_job_i
+00000340: 643a 2073 7472 2c20 6e5f 7370 6c69 7473  d: str, n_splits
+00000350: 3a20 696e 7420 3d20 3529 202d 3e20 4a6f  : int = 5) -> Jo
+00000360: 623a 0a20 2020 2022 2222 0a20 2020 2053  b:.    """.    S
+00000370: 7562 6d69 7420 6120 6372 6f73 732d 7661  ubmit a cross-va
+00000380: 6c69 6461 7469 6f6e 206a 6f62 2e0a 0a20  lidation job... 
+00000390: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000003a0: 2073 6573 7369 6f6e 2028 4150 4953 6573   session (APISes
+000003b0: 7369 6f6e 293a 2061 7574 6820 7365 7373  sion): auth sess
+000003c0: 696f 6e0a 2020 2020 2020 2020 6a6f 625f  ion.        job_
+000003d0: 6964 2028 7374 7229 3a20 6a6f 6220 6964  id (str): job id
+000003e0: 0a20 2020 2020 2020 206e 5f73 706c 6974  .        n_split
+000003f0: 7320 2869 6e74 2c20 6f70 7469 6f6e 616c  s (int, optional
+00000400: 293a 204e 206f 6620 4356 2073 706c 6974  ): N of CV split
+00000410: 732e 2044 6566 6175 6c74 7320 746f 2035  s. Defaults to 5
+00000420: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00000430: 2020 2020 2020 2020 4a6f 623a 0a20 2020          Job:.   
+00000440: 2022 2222 0a20 2020 2065 6e64 706f 696e   """.    endpoin
+00000450: 7420 3d20 2276 312f 776f 726b 666c 6f77  t = "v1/workflow
+00000460: 2f63 726f 7373 7661 6c69 6461 7465 220a  /crossvalidate".
+00000470: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00000480: 6573 7369 6f6e 2e70 6f73 7428 0a20 2020  ession.post(.   
+00000490: 2020 2020 2065 6e64 706f 696e 742c 206a       endpoint, j
+000004a0: 736f 6e3d 7b22 7472 6169 6e5f 6a6f 625f  son={"train_job_
+000004b0: 6964 223a 2074 7261 696e 5f6a 6f62 5f69  id": train_job_i
+000004c0: 642c 2022 6e5f 7370 6c69 7473 223a 206e  d, "n_splits": n
+000004d0: 5f73 706c 6974 737d 0a20 2020 2029 0a20  _splits}.    ). 
+000004e0: 2020 2072 6574 7572 6e20 7079 6461 6e74     return pydant
+000004f0: 6963 2e70 6172 7365 5f6f 626a 5f61 7328  ic.parse_obj_as(
+00000500: 4a6f 622c 2072 6573 706f 6e73 652e 6a73  Job, response.js
+00000510: 6f6e 2829 290a 0a0a 6465 6620 6765 745f  on())...def get_
+00000520: 6372 6f73 7376 616c 6964 6174 696f 6e28  crossvalidation(
+00000530: 0a20 2020 2073 6573 7369 6f6e 3a20 4150  .    session: AP
+00000540: 4953 6573 7369 6f6e 2c0a 2020 2020 6a6f  ISession,.    jo
+00000550: 625f 6964 3a20 7374 722c 0a20 2020 2070  b_id: str,.    p
+00000560: 6167 655f 7369 7a65 3a20 4f70 7469 6f6e  age_size: Option
+00000570: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+00000580: 2020 2020 7061 6765 5f6f 6666 7365 743a      page_offset:
+00000590: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+000005a0: 2030 2c0a 2920 2d3e 2043 5652 6573 756c   0,.) -> CVResul
+000005b0: 7473 3a0a 2020 2020 2222 220a 2020 2020  ts:.    """.    
+000005c0: 4765 7420 4356 2072 6573 756c 7473 0a0a  Get CV results..
+000005d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000005e0: 2020 7365 7373 696f 6e20 2841 5049 5365    session (APISe
+000005f0: 7373 696f 6e29 3a20 6175 7468 2764 2073  ssion): auth'd s
+00000600: 6573 7369 6f6e 0a20 2020 2020 2020 206a  ession.        j
+00000610: 6f62 5f69 6420 2873 7472 293a 204a 6f62  ob_id (str): Job
+00000620: 2069 640a 0a20 2020 2052 6574 7572 6e73   id..    Returns
+00000630: 3a0a 2020 2020 2020 2020 5f74 7970 655f  :.        _type_
+00000640: 3a20 5f64 6573 6372 6970 7469 6f6e 5f0a  : _description_.
+00000650: 2020 2020 2222 220a 2020 2020 656e 6470      """.    endp
+00000660: 6f69 6e74 203d 2066 2276 312f 776f 726b  oint = f"v1/work
+00000670: 666c 6f77 2f63 726f 7373 7661 6c69 6461  flow/crossvalida
+00000680: 7465 2f7b 6a6f 625f 6964 7d22 0a20 2020  te/{job_id}".   
+00000690: 2070 6172 616d 7320 3d20 7b22 7061 6765   params = {"page
+000006a0: 5f73 697a 6522 3a20 7061 6765 5f73 697a  _size": page_siz
+000006b0: 652c 2022 7061 6765 5f6f 6666 7365 7422  e, "page_offset"
+000006c0: 3a20 7061 6765 5f6f 6666 7365 747d 0a20  : page_offset}. 
+000006d0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
+000006e0: 7373 696f 6e2e 6765 7428 656e 6470 6f69  ssion.get(endpoi
+000006f0: 6e74 2c20 7061 7261 6d73 3d70 6172 616d  nt, params=param
+00000700: 7329 0a20 2020 2069 6620 7265 7370 6f6e  s).    if respon
+00000710: 7365 2e73 7461 7475 735f 636f 6465 203d  se.status_code =
+00000720: 3d20 3430 343a 0a20 2020 2020 2020 2072  = 404:.        r
+00000730: 6169 7365 2049 6e76 616c 6964 4a6f 6228  aise InvalidJob(
+00000740: 224e 6f20 4356 206a 6f62 2068 6173 2062  "No CV job has b
+00000750: 6565 6e20 7375 626d 6974 7465 6420 666f  een submitted fo
+00000760: 7220 7468 6973 206a 6f62 2122 290a 2020  r this job!").  
+00000770: 2020 7265 7475 726e 2070 7964 616e 7469    return pydanti
+00000780: 632e 7061 7273 655f 6f62 6a5f 6173 2843  c.parse_obj_as(C
+00000790: 5652 6573 756c 7473 2c20 7265 7370 6f6e  VResults, respon
+000007a0: 7365 2e6a 736f 6e28 2929 0a0a 0a64 6566  se.json())...def
+000007b0: 205f 7472 6169 6e5f 6a6f 6228 0a20 2020   _train_job(.   
+000007c0: 2073 6573 7369 6f6e 3a20 4150 4953 6573   session: APISes
+000007d0: 7369 6f6e 2c0a 2020 2020 656e 6470 6f69  sion,.    endpoi
+000007e0: 6e74 3a20 7374 722c 0a20 2020 2061 7373  nt: str,.    ass
+000007f0: 6179 6461 7461 7365 743a 2041 7373 6179  aydataset: Assay
+00000800: 4461 7461 7365 742c 0a20 2020 206d 6561  Dataset,.    mea
+00000810: 7375 7265 6d65 6e74 5f6e 616d 653a 2055  surement_name: U
+00000820: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
+00000830: 7472 5d5d 2c0a 2020 2020 6d6f 6465 6c5f  tr]],.    model_
+00000840: 6e61 6d65 3a20 7374 7220 3d20 2222 2c0a  name: str = "",.
+00000850: 2020 2020 666f 7263 655f 7072 6570 726f      force_prepro
+00000860: 6365 7373 3a20 4f70 7469 6f6e 616c 5b62  cess: Optional[b
+00000870: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2920  ool] = False,.) 
+00000880: 2d3e 204a 6f62 706c 7573 3a0a 2020 2020  -> Jobplus:.    
+00000890: 2222 220a 2020 2020 4372 6561 7465 2061  """.    Create a
+000008a0: 2074 7261 696e 696e 6720 6a6f 622e 0a0a   training job...
+000008b0: 2020 2020 5661 6c69 6461 7465 2069 6e70      Validate inp
+000008c0: 7574 732c 2066 6f72 6d61 7420 2064 6174  uts, format  dat
+000008d0: 612c 2073 656e 6473 2074 6865 206a 6f62  a, sends the job
+000008e0: 2074 7261 696e 696e 6720 7265 7175 6573   training reques
+000008f0: 7420 746f 2074 6865 2065 6e64 706f 696e  t to the endpoin
+00000900: 742c 0a0a 2020 2020 5061 7273 6573 2074  t,..    Parses t
+00000910: 6865 2072 6573 706f 6e73 6520 696e 746f  he response into
+00000920: 2061 2060 4a6f 6260 206f 626a 6563 742e   a `Job` object.
+00000930: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00000940: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000950: 2020 2020 7365 7373 696f 6e20 3a20 4150      session : AP
+00000960: 4953 6573 7369 6f6e 0a20 2020 2020 2020  ISession.       
+00000970: 2054 6865 2063 7572 7265 6e74 2041 5049   The current API
+00000980: 2073 6573 7369 6f6e 2066 6f72 2063 6f6d   session for com
+00000990: 6d75 6e69 6361 7469 6f6e 2077 6974 6820  munication with 
+000009a0: 7468 6520 7365 7276 6572 2e0a 2020 2020  the server..    
+000009b0: 656e 6470 6f69 6e74 203a 2073 7472 0a20  endpoint : str. 
+000009c0: 2020 2020 2020 2054 6865 2065 6e64 706f         The endpo
+000009d0: 696e 7420 746f 2077 6869 6368 2074 6865  int to which the
+000009e0: 206a 6f62 2074 7261 696e 696e 6720 7265   job training re
+000009f0: 7175 6573 7420 6973 2074 6f20 6265 2073  quest is to be s
+00000a00: 656e 742e 0a20 2020 2061 7373 6179 6461  ent..    assayda
+00000a10: 7461 7365 7420 3a20 4173 7361 7944 6174  taset : AssayDat
+00000a20: 6173 6574 0a20 2020 2020 2020 2041 6e20  aset.        An 
+00000a30: 4173 7361 7944 6174 6173 6574 206f 626a  AssayDataset obj
+00000a40: 6563 7420 6672 6f6d 2077 6869 6368 2074  ect from which t
+00000a50: 6865 2061 7373 6179 5f69 6420 6973 2065  he assay_id is e
+00000a60: 7874 7261 6374 6564 2e0a 2020 2020 6d65  xtracted..    me
+00000a70: 6173 7572 656d 656e 745f 6e61 6d65 203a  asurement_name :
+00000a80: 2073 7472 206f 7220 4c69 7374 5b73 7472   str or List[str
+00000a90: 5d0a 2020 2020 2020 2020 5468 6520 6e61  ].        The na
+00000aa0: 6d65 2873 2920 6f66 2074 6865 206d 6561  me(s) of the mea
+00000ab0: 7375 7265 6d65 6e74 2873 2920 746f 2062  surement(s) to b
+00000ac0: 6520 7573 6564 2069 6e20 7468 6520 7472  e used in the tr
+00000ad0: 6169 6e69 6e67 206a 6f62 2e0a 2020 2020  aining job..    
+00000ae0: 6d6f 6465 6c5f 6e61 6d65 203a 2073 7472  model_name : str
+00000af0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00000b00: 2020 2054 6865 206e 616d 6520 746f 2067     The name to g
+00000b10: 6976 6520 7468 6520 6d6f 6465 6c2e 0a20  ive the model.. 
+00000b20: 2020 2066 6f72 6365 5f70 7265 7072 6f63     force_preproc
+00000b30: 6573 7320 3a20 626f 6f6c 2c20 6f70 7469  ess : bool, opti
+00000b40: 6f6e 616c 0a20 2020 2020 2020 2049 6620  onal.        If 
+00000b50: 7365 7420 746f 2054 7275 652c 2070 7265  set to True, pre
+00000b60: 7072 6f63 6573 7369 6e67 2069 7320 666f  processing is fo
+00000b70: 7263 6564 2065 7665 6e20 6966 2070 7265  rced even if pre
+00000b80: 7072 6f63 6573 7365 6420 6461 7461 2061  processed data a
+00000b90: 6c72 6561 6479 2065 7869 7374 732e 0a0a  lready exists...
+00000ba0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000bb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 4a6f 620a  -------.    Job.
+00000bc0: 2020 2020 2020 2020 4120 4a6f 620a 0a20          A Job.. 
+00000bd0: 2020 2052 6169 7365 730a 2020 2020 2d2d     Raises.    --
+00000be0: 2d2d 2d2d 0a20 2020 2049 6e76 616c 6964  ----.    Invalid
+00000bf0: 5061 7261 6d65 7465 7245 7272 6f72 0a20  ParameterError. 
+00000c00: 2020 2020 2020 2049 6620 7468 6520 6061         If the `a
+00000c10: 7373 6179 6461 7461 7365 7460 2069 7320  ssaydataset` is 
+00000c20: 6e6f 7420 616e 2041 7373 6179 4461 7461  not an AssayData
+00000c30: 7365 7420 6f62 6a65 6374 2c0a 2020 2020  set object,.    
+00000c40: 2020 2020 4966 2061 6e79 206d 6561 7375      If any measu
+00000c50: 7265 6d65 6e74 206e 616d 6520 7072 6f76  rement name prov
+00000c60: 6964 6564 2064 6f65 7320 6e6f 7420 6578  ided does not ex
+00000c70: 6973 7420 696e 2074 6865 2041 7373 6179  ist in the Assay
+00000c80: 4461 7461 7365 742c 0a20 2020 2020 2020  Dataset,.       
+00000c90: 206f 7220 6966 2074 6865 2041 7373 6179   or if the Assay
+00000ca0: 4461 7461 7365 7420 6861 7320 6665 7765  Dataset has fewe
+00000cb0: 7220 7468 616e 2033 2064 6174 6120 706f  r than 3 data po
+00000cc0: 696e 7473 2e0a 2020 2020 4854 5450 4572  ints..    HTTPEr
+00000cd0: 726f 720a 2020 2020 2020 2020 4966 2074  ror.        If t
+00000ce0: 6865 2072 6571 7565 7374 2074 6f20 7468  he request to th
+00000cf0: 6520 7365 7276 6572 2066 6169 6c73 2e0a  e server fails..
+00000d00: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+00000d10: 6f74 2069 7369 6e73 7461 6e63 6528 6173  ot isinstance(as
+00000d20: 7361 7964 6174 6173 6574 2c20 4173 7361  saydataset, Assa
+00000d30: 7944 6174 6173 6574 293a 0a20 2020 2020  yDataset):.     
+00000d40: 2020 2072 6169 7365 2049 6e76 616c 6964     raise Invalid
+00000d50: 5061 7261 6d65 7465 7245 7272 6f72 2822  ParameterError("
+00000d60: 6173 7361 7964 6174 6173 6574 2073 686f  assaydataset sho
+00000d70: 756c 6420 6265 2061 6e20 6173 7361 7964  uld be an assayd
+00000d80: 6174 6120 4a6f 6220 7265 7375 6c74 2229  ata Job result")
+00000d90: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00000da0: 6365 286d 6561 7375 7265 6d65 6e74 5f6e  ce(measurement_n
+00000db0: 616d 652c 2073 7472 293a 0a20 2020 2020  ame, str):.     
+00000dc0: 2020 206d 6561 7375 7265 6d65 6e74 5f6e     measurement_n
+00000dd0: 616d 6520 3d20 5b6d 6561 7375 7265 6d65  ame = [measureme
+00000de0: 6e74 5f6e 616d 655d 0a0a 2020 2020 666f  nt_name]..    fo
+00000df0: 7220 6d65 6173 7572 656d 656e 7420 696e  r measurement in
+00000e00: 206d 6561 7375 7265 6d65 6e74 5f6e 616d   measurement_nam
+00000e10: 653a 0a20 2020 2020 2020 2069 6620 6d65  e:.        if me
+00000e20: 6173 7572 656d 656e 7420 6e6f 7420 696e  asurement not in
+00000e30: 2061 7373 6179 6461 7461 7365 742e 6d65   assaydataset.me
+00000e40: 6173 7572 656d 656e 745f 6e61 6d65 733a  asurement_names:
+00000e50: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00000e60: 7365 2049 6e76 616c 6964 5061 7261 6d65  se InvalidParame
+00000e70: 7465 7245 7272 6f72 2866 224e 6f20 7b6d  terError(f"No {m
+00000e80: 6561 7375 7265 6d65 6e74 7d20 696e 206d  easurement} in m
+00000e90: 6561 7375 7265 6d65 6e74 206e 616d 6573  easurement names
+00000ea0: 2229 0a20 2020 2069 6620 6173 7361 7964  ").    if assayd
+00000eb0: 6174 6173 6574 2e73 6861 7065 5b30 5d20  ataset.shape[0] 
+00000ec0: 3c20 333a 0a20 2020 2020 2020 2072 6169  < 3:.        rai
+00000ed0: 7365 2049 6e76 616c 6964 5061 7261 6d65  se InvalidParame
+00000ee0: 7465 7245 7272 6f72 2822 4173 7361 7964  terError("Assayd
+00000ef0: 6174 6120 6d75 7374 2068 6176 6520 3e3d  ata must have >=
+00000f00: 3320 6461 7461 2070 6f69 6e74 7320 666f  3 data points fo
+00000f10: 7220 7472 6169 6e69 6e67 2122 290a 2020  r training!").  
+00000f20: 2020 6966 206d 6f64 656c 5f6e 616d 6520    if model_name 
+00000f30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00000f40: 206d 6f64 656c 5f6e 616d 6520 3d20 2222   model_name = ""
+00000f50: 0a0a 2020 2020 6461 7461 203d 207b 0a20  ..    data = {. 
+00000f60: 2020 2020 2020 2022 6173 7361 795f 6964         "assay_id
+00000f70: 223a 2061 7373 6179 6461 7461 7365 742e  ": assaydataset.
+00000f80: 6964 2c0a 2020 2020 2020 2020 226d 6561  id,.        "mea
+00000f90: 7375 7265 6d65 6e74 5f6e 616d 6522 3a20  surement_name": 
+00000fa0: 6d65 6173 7572 656d 656e 745f 6e61 6d65  measurement_name
+00000fb0: 2c0a 2020 2020 2020 2020 226d 6f64 656c  ,.        "model
+00000fc0: 5f6e 616d 6522 3a20 6d6f 6465 6c5f 6e61  _name": model_na
+00000fd0: 6d65 2c0a 2020 2020 7d0a 2020 2020 7061  me,.    }.    pa
+00000fe0: 7261 6d73 203d 207b 2266 6f72 6365 5f70  rams = {"force_p
+00000ff0: 7265 7072 6f63 6573 7322 3a20 7374 7228  reprocess": str(
+00001000: 666f 7263 655f 7072 6570 726f 6365 7373  force_preprocess
+00001010: 292e 6c6f 7765 7228 297d 0a0a 2020 2020  ).lower()}..    
+00001020: 7265 7370 6f6e 7365 203d 2073 6573 7369  response = sessi
+00001030: 6f6e 2e70 6f73 7428 656e 6470 6f69 6e74  on.post(endpoint
+00001040: 2c20 7061 7261 6d73 3d70 6172 616d 732c  , params=params,
+00001050: 206a 736f 6e3d 6461 7461 290a 2020 2020   json=data).    
+00001060: 7265 7370 6f6e 7365 2e72 6169 7365 5f66  response.raise_f
+00001070: 6f72 5f73 7461 7475 7328 290a 2020 2020  or_status().    
+00001080: 7265 7475 726e 2070 7964 616e 7469 632e  return pydantic.
+00001090: 7061 7273 655f 6f62 6a5f 6173 284a 6f62  parse_obj_as(Job
+000010a0: 706c 7573 2c20 7265 7370 6f6e 7365 2e6a  plus, response.j
+000010b0: 736f 6e28 2929 0a0a 0a64 6566 2063 7265  son())...def cre
+000010c0: 6174 655f 7472 6169 6e5f 6a6f 6228 0a20  ate_train_job(. 
+000010d0: 2020 2073 6573 7369 6f6e 3a20 4150 4953     session: APIS
+000010e0: 6573 7369 6f6e 2c0a 2020 2020 6173 7361  ession,.    assa
+000010f0: 7964 6174 6173 6574 3a20 4173 7361 7944  ydataset: AssayD
+00001100: 6174 6173 6574 2c0a 2020 2020 6d65 6173  ataset,.    meas
+00001110: 7572 656d 656e 745f 6e61 6d65 3a20 556e  urement_name: Un
+00001120: 696f 6e5b 7374 722c 204c 6973 745b 7374  ion[str, List[st
+00001130: 725d 5d2c 0a20 2020 206d 6f64 656c 5f6e  r]],.    model_n
+00001140: 616d 653a 2073 7472 203d 2022 222c 0a20  ame: str = "",. 
+00001150: 2020 2066 6f72 6365 5f70 7265 7072 6f63     force_preproc
+00001160: 6573 733a 204f 7074 696f 6e61 6c5b 626f  ess: Optional[bo
+00001170: 6f6c 5d20 3d20 4661 6c73 652c 0a29 3a0a  ol] = False,.):.
+00001180: 2020 2020 2222 220a 2020 2020 4372 6561      """.    Crea
+00001190: 7465 2061 2074 7261 696e 696e 6720 6a6f  te a training jo
+000011a0: 622e 0a0a 2020 2020 5661 6c69 6461 7465  b...    Validate
+000011b0: 2069 6e70 7574 732c 2066 6f72 6d61 7420   inputs, format 
+000011c0: 2064 6174 612c 2073 656e 6473 2074 6865   data, sends the
+000011d0: 206a 6f62 2074 7261 696e 696e 6720 7265   job training re
+000011e0: 7175 6573 7420 746f 2074 6865 2065 6e64  quest to the end
+000011f0: 706f 696e 742c 0a0a 2020 2020 5061 7273  point,..    Pars
+00001200: 6573 2074 6865 2072 6573 706f 6e73 6520  es the response 
+00001210: 696e 746f 2061 2060 4a6f 6260 206f 626a  into a `Job` obj
+00001220: 6563 742e 0a0a 2020 2020 5061 7261 6d65  ect...    Parame
+00001230: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00001240: 2d2d 2d0a 2020 2020 7365 7373 696f 6e20  ---.    session 
+00001250: 3a20 4150 4953 6573 7369 6f6e 0a20 2020  : APISession.   
+00001260: 2020 2020 2054 6865 2063 7572 7265 6e74       The current
+00001270: 2041 5049 2073 6573 7369 6f6e 2066 6f72   API session for
+00001280: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2077   communication w
+00001290: 6974 6820 7468 6520 7365 7276 6572 2e0a  ith the server..
+000012a0: 2020 2020 656e 6470 6f69 6e74 203a 2073      endpoint : s
+000012b0: 7472 0a20 2020 2020 2020 2054 6865 2065  tr.        The e
+000012c0: 6e64 706f 696e 7420 746f 2077 6869 6368  ndpoint to which
+000012d0: 2074 6865 206a 6f62 2074 7261 696e 696e   the job trainin
+000012e0: 6720 7265 7175 6573 7420 6973 2074 6f20  g request is to 
+000012f0: 6265 2073 656e 742e 0a20 2020 2061 7373  be sent..    ass
+00001300: 6179 6461 7461 7365 7420 3a20 4173 7361  aydataset : Assa
+00001310: 7944 6174 6173 6574 0a20 2020 2020 2020  yDataset.       
+00001320: 2041 6e20 4173 7361 7944 6174 6173 6574   An AssayDataset
+00001330: 206f 626a 6563 7420 6672 6f6d 2077 6869   object from whi
+00001340: 6368 2074 6865 2061 7373 6179 5f69 6420  ch the assay_id 
+00001350: 6973 2065 7874 7261 6374 6564 2e0a 2020  is extracted..  
+00001360: 2020 6d65 6173 7572 656d 656e 745f 6e61    measurement_na
+00001370: 6d65 203a 2073 7472 206f 7220 4c69 7374  me : str or List
+00001380: 5b73 7472 5d0a 2020 2020 2020 2020 5468  [str].        Th
+00001390: 6520 6e61 6d65 2873 2920 6f66 2074 6865  e name(s) of the
+000013a0: 206d 6561 7375 7265 6d65 6e74 2873 2920   measurement(s) 
+000013b0: 746f 2062 6520 7573 6564 2069 6e20 7468  to be used in th
+000013c0: 6520 7472 6169 6e69 6e67 206a 6f62 2e0a  e training job..
+000013d0: 2020 2020 6d6f 6465 6c5f 6e61 6d65 203a      model_name :
+000013e0: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+000013f0: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
+00001400: 746f 2067 6976 6520 7468 6520 6d6f 6465  to give the mode
+00001410: 6c2e 0a20 2020 2066 6f72 6365 5f70 7265  l..    force_pre
+00001420: 7072 6f63 6573 7320 3a20 626f 6f6c 2c20  process : bool, 
+00001430: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00001440: 2049 6620 7365 7420 746f 2054 7275 652c   If set to True,
+00001450: 2070 7265 7072 6f63 6573 7369 6e67 2069   preprocessing i
+00001460: 7320 666f 7263 6564 2065 7665 6e20 6966  s forced even if
+00001470: 2070 7265 7072 6f63 6573 7365 6420 6461   preprocessed da
+00001480: 7461 2061 6c72 6561 6479 2065 7869 7374  ta already exist
+00001490: 732e 0a0a 2020 2020 5265 7475 726e 730a  s...    Returns.
+000014a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000014b0: 4a6f 620a 2020 2020 2020 2020 4120 4a6f  Job.        A Jo
+000014c0: 620a 0a20 2020 2052 6169 7365 730a 2020  b..    Raises.  
+000014d0: 2020 2d2d 2d2d 2d2d 0a20 2020 2049 6e76    ------.    Inv
+000014e0: 616c 6964 5061 7261 6d65 7465 7245 7272  alidParameterErr
+000014f0: 6f72 0a20 2020 2020 2020 2049 6620 7468  or.        If th
+00001500: 6520 6061 7373 6179 6461 7461 7365 7460  e `assaydataset`
+00001510: 2069 7320 6e6f 7420 616e 2041 7373 6179   is not an Assay
+00001520: 4461 7461 7365 7420 6f62 6a65 6374 2c0a  Dataset object,.
+00001530: 2020 2020 2020 2020 4966 2061 6e79 206d          If any m
+00001540: 6561 7375 7265 6d65 6e74 206e 616d 6520  easurement name 
+00001550: 7072 6f76 6964 6564 2064 6f65 7320 6e6f  provided does no
+00001560: 7420 6578 6973 7420 696e 2074 6865 2041  t exist in the A
+00001570: 7373 6179 4461 7461 7365 742c 0a20 2020  ssayDataset,.   
+00001580: 2020 2020 206f 7220 6966 2074 6865 2041       or if the A
+00001590: 7373 6179 4461 7461 7365 7420 6861 7320  ssayDataset has 
+000015a0: 6665 7765 7220 7468 616e 2033 2064 6174  fewer than 3 dat
+000015b0: 6120 706f 696e 7473 2e0a 2020 2020 4854  a points..    HT
+000015c0: 5450 4572 726f 720a 2020 2020 2020 2020  TPError.        
+000015d0: 4966 2074 6865 2072 6571 7565 7374 2074  If the request t
+000015e0: 6f20 7468 6520 7365 7276 6572 2066 6169  o the server fai
+000015f0: 6c73 2e0a 2020 2020 2222 220a 2020 2020  ls..    """.    
+00001600: 656e 6470 6f69 6e74 203d 2022 7631 2f77  endpoint = "v1/w
+00001610: 6f72 6b66 6c6f 772f 7472 6169 6e22 0a20  orkflow/train". 
+00001620: 2020 2072 6574 7572 6e20 5f74 7261 696e     return _train
+00001630: 5f6a 6f62 280a 2020 2020 2020 2020 7365  _job(.        se
+00001640: 7373 696f 6e2c 2065 6e64 706f 696e 742c  ssion, endpoint,
+00001650: 2061 7373 6179 6461 7461 7365 742c 206d   assaydataset, m
+00001660: 6561 7375 7265 6d65 6e74 5f6e 616d 652c  easurement_name,
+00001670: 206d 6f64 656c 5f6e 616d 652c 2066 6f72   model_name, for
+00001680: 6365 5f70 7265 7072 6f63 6573 730a 2020  ce_preprocess.  
+00001690: 2020 290a 0a0a 6465 6620 5f63 7265 6174    )...def _creat
+000016a0: 655f 7472 6169 6e5f 6a6f 625f 6272 280a  e_train_job_br(.
+000016b0: 2020 2020 7365 7373 696f 6e3a 2041 5049      session: API
+000016c0: 5365 7373 696f 6e2c 0a20 2020 2061 7373  Session,.    ass
+000016d0: 6179 6461 7461 7365 743a 2041 7373 6179  aydataset: Assay
+000016e0: 4461 7461 7365 742c 0a20 2020 206d 6561  Dataset,.    mea
+000016f0: 7375 7265 6d65 6e74 5f6e 616d 653a 2055  surement_name: U
+00001700: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
+00001710: 7472 5d5d 2c0a 2020 2020 6d6f 6465 6c5f  tr]],.    model_
+00001720: 6e61 6d65 3a20 7374 7220 3d20 2222 2c0a  name: str = "",.
+00001730: 2020 2020 666f 7263 655f 7072 6570 726f      force_prepro
+00001740: 6365 7373 3a20 4f70 7469 6f6e 616c 5b62  cess: Optional[b
+00001750: 6f6f 6c5d 203d 2046 616c 7365 2c0a 293a  ool] = False,.):
+00001760: 0a20 2020 2022 2222 416c 6961 7320 666f  .    """Alias fo
+00001770: 7220 6372 6561 7465 5f74 7261 696e 5f6a  r create_train_j
+00001780: 6f62 2222 220a 2020 2020 656e 6470 6f69  ob""".    endpoi
+00001790: 6e74 203d 2022 7631 2f77 6f72 6b66 6c6f  nt = "v1/workflo
+000017a0: 772f 7472 6169 6e2f 6272 220a 2020 2020  w/train/br".    
+000017b0: 7265 7475 726e 205f 7472 6169 6e5f 6a6f  return _train_jo
+000017c0: 6228 0a20 2020 2020 2020 2073 6573 7369  b(.        sessi
+000017d0: 6f6e 2c20 656e 6470 6f69 6e74 2c20 6173  on, endpoint, as
+000017e0: 7361 7964 6174 6173 6574 2c20 6d65 6173  saydataset, meas
+000017f0: 7572 656d 656e 745f 6e61 6d65 2c20 6d6f  urement_name, mo
+00001800: 6465 6c5f 6e61 6d65 2c20 666f 7263 655f  del_name, force_
+00001810: 7072 6570 726f 6365 7373 0a20 2020 2029  preprocess.    )
+00001820: 0a0a 0a64 6566 205f 6372 6561 7465 5f74  ...def _create_t
+00001830: 7261 696e 5f6a 6f62 5f67 7028 0a20 2020  rain_job_gp(.   
+00001840: 2073 6573 7369 6f6e 3a20 4150 4953 6573   session: APISes
+00001850: 7369 6f6e 2c0a 2020 2020 6173 7361 7964  sion,.    assayd
+00001860: 6174 6173 6574 3a20 4173 7361 7944 6174  ataset: AssayDat
+00001870: 6173 6574 2c0a 2020 2020 6d65 6173 7572  aset,.    measur
+00001880: 656d 656e 745f 6e61 6d65 3a20 556e 696f  ement_name: Unio
+00001890: 6e5b 7374 722c 204c 6973 745b 7374 725d  n[str, List[str]
+000018a0: 5d2c 0a20 2020 206d 6f64 656c 5f6e 616d  ],.    model_nam
+000018b0: 653a 2073 7472 203d 2022 222c 0a20 2020  e: str = "",.   
+000018c0: 2066 6f72 6365 5f70 7265 7072 6f63 6573   force_preproces
+000018d0: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
+000018e0: 5d20 3d20 4661 6c73 652c 0a29 3a0a 2020  ] = False,.):.  
+000018f0: 2020 2222 2241 6c69 6173 2066 6f72 2063    """Alias for c
+00001900: 7265 6174 655f 7472 6169 6e5f 6a6f 6222  reate_train_job"
+00001910: 2222 0a20 2020 2065 6e64 706f 696e 7420  "".    endpoint 
+00001920: 3d20 2276 312f 776f 726b 666c 6f77 2f74  = "v1/workflow/t
+00001930: 7261 696e 2f67 7022 0a20 2020 2072 6574  rain/gp".    ret
+00001940: 7572 6e20 5f74 7261 696e 5f6a 6f62 280a  urn _train_job(.
+00001950: 2020 2020 2020 2020 7365 7373 696f 6e2c          session,
+00001960: 2065 6e64 706f 696e 742c 2061 7373 6179   endpoint, assay
+00001970: 6461 7461 7365 742c 206d 6561 7375 7265  dataset, measure
+00001980: 6d65 6e74 5f6e 616d 652c 206d 6f64 656c  ment_name, model
+00001990: 5f6e 616d 652c 2066 6f72 6365 5f70 7265  _name, force_pre
+000019a0: 7072 6f63 6573 730a 2020 2020 290a 0a0a  process.    )...
+000019b0: 6465 6620 6765 745f 7472 6169 6e69 6e67  def get_training
+000019c0: 5f72 6573 756c 7473 2873 6573 7369 6f6e  _results(session
+000019d0: 3a20 4150 4953 6573 7369 6f6e 2c20 6a6f  : APISession, jo
+000019e0: 625f 6964 3a20 7374 7229 202d 3e20 5472  b_id: str) -> Tr
+000019f0: 6169 6e47 7261 7068 3a0a 2020 2020 2222  ainGraph:.    ""
+00001a00: 2247 6574 2054 7261 696e 696e 6720 7265  "Get Training re
+00001a10: 7375 6c74 7320 2865 2e67 2e20 6c6f 7373  sults (e.g. loss
+00001a20: 2065 7463 2920 6f66 206a 6f62 2e22 2222   etc) of job."""
+00001a30: 0a20 2020 2065 6e64 706f 696e 7420 3d20  .    endpoint = 
+00001a40: 6622 7631 2f77 6f72 6b66 6c6f 772f 7472  f"v1/workflow/tr
+00001a50: 6169 6e2f 7b6a 6f62 5f69 647d 220a 2020  ain/{job_id}".  
+00001a60: 2020 7265 7370 6f6e 7365 203d 2073 6573    response = ses
+00001a70: 7369 6f6e 2e67 6574 2865 6e64 706f 696e  sion.get(endpoin
+00001a80: 7429 0a20 2020 2072 6574 7572 6e20 5472  t).    return Tr
+00001a90: 6169 6e47 7261 7068 282a 2a72 6573 706f  ainGraph(**respo
+00001aa0: 6e73 652e 6a73 6f6e 2829 290a 0a0a 6465  nse.json())...de
+00001ab0: 6620 6c6f 6164 5f6a 6f62 2873 6573 7369  f load_job(sessi
+00001ac0: 6f6e 3a20 4150 4953 6573 7369 6f6e 2c20  on: APISession, 
+00001ad0: 6a6f 625f 6964 3a20 7374 7229 202d 3e20  job_id: str) -> 
+00001ae0: 4a6f 6270 6c75 733a 0a20 2020 2022 2222  Jobplus:.    """
+00001af0: 0a20 2020 2052 656c 6f61 6420 6120 5375  .    Reload a Su
+00001b00: 626d 6974 7465 6420 6a6f 6220 746f 2072  bmitted job to r
+00001b10: 6573 756d 6520 6672 6f6d 2077 6865 7265  esume from where
+00001b20: 2079 6f75 206c 6566 7420 6f66 6621 0a0a   you left off!..
+00001b30: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00001b40: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00001b50: 2020 2073 6573 7369 6f6e 203a 2041 5049     session : API
+00001b60: 5365 7373 696f 6e0a 2020 2020 2020 2020  Session.        
+00001b70: 5468 6520 6375 7272 656e 7420 4150 4920  The current API 
+00001b80: 7365 7373 696f 6e20 666f 7220 636f 6d6d  session for comm
+00001b90: 756e 6963 6174 696f 6e20 7769 7468 2074  unication with t
+00001ba0: 6865 2073 6572 7665 722e 0a20 2020 206a  he server..    j
+00001bb0: 6f62 5f69 6420 3a20 7374 720a 2020 2020  ob_id : str.    
+00001bc0: 2020 2020 5468 6520 6964 656e 7469 6669      The identifi
+00001bd0: 6572 206f 6620 7468 6520 6a6f 6220 7768  er of the job wh
+00001be0: 6f73 6520 6465 7461 696c 7320 6172 6520  ose details are 
+00001bf0: 746f 2062 6520 6c6f 6164 6564 2e0a 0a20  to be loaded... 
+00001c00: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00001c10: 2d2d 2d2d 2d2d 0a20 2020 204a 6f62 0a20  ------.    Job. 
+00001c20: 2020 2020 2020 204a 6f62 0a0a 2020 2020         Job..    
+00001c30: 5261 6973 6573 0a20 2020 202d 2d2d 2d2d  Raises.    -----
+00001c40: 2d0a 2020 2020 4854 5450 4572 726f 720a  -.    HTTPError.
+00001c50: 2020 2020 2020 2020 4966 2074 6865 2072          If the r
+00001c60: 6571 7565 7374 2074 6f20 7468 6520 7365  equest to the se
+00001c70: 7276 6572 2066 6169 6c73 2e0a 0a20 2020  rver fails...   
+00001c80: 2022 2222 0a20 2020 2065 6e64 706f 696e   """.    endpoin
+00001c90: 7420 3d20 6622 7631 2f77 6f72 6b66 6c6f  t = f"v1/workflo
+00001ca0: 772f 7472 6169 6e2f 6a6f 622f 7b6a 6f62  w/train/job/{job
+00001cb0: 5f69 647d 220a 2020 2020 7265 7370 6f6e  _id}".    respon
+00001cc0: 7365 203d 2073 6573 7369 6f6e 2e67 6574  se = session.get
+00001cd0: 2865 6e64 706f 696e 7429 0a20 2020 2072  (endpoint).    r
+00001ce0: 6574 7572 6e20 7079 6461 6e74 6963 2e70  eturn pydantic.p
+00001cf0: 6172 7365 5f6f 626a 5f61 7328 4a6f 6270  arse_obj_as(Jobp
+00001d00: 6c75 732c 2072 6573 706f 6e73 652e 6a73  lus, response.js
+00001d10: 6f6e 2829 290a 0a0a 636c 6173 7320 4356  on())...class CV
+00001d20: 4675 7475 7265 4d69 7869 6e3a 0a20 2020  FutureMixin:.   
+00001d30: 2022 2222 0a20 2020 2041 206d 6978 696e   """.    A mixin
+00001d40: 2063 6c61 7373 2074 6f20 7072 6f76 6964   class to provid
+00001d50: 6520 6372 6f73 732d 7661 6c69 6461 7469  e cross-validati
+00001d60: 6f6e 206a 6f62 2073 7562 6d69 7373 696f  on job submissio
+00001d70: 6e20 616e 6420 7265 7472 6965 7661 6c2e  n and retrieval.
+00001d80: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00001d90: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00001da0: 2020 2020 7365 7373 696f 6e20 3a20 4150      session : AP
+00001db0: 4953 6573 7369 6f6e 0a20 2020 2020 2020  ISession.       
+00001dc0: 2054 6865 2073 6573 7369 6f6e 206f 626a   The session obj
+00001dd0: 6563 7420 746f 2075 7365 2066 6f72 2041  ect to use for A
+00001de0: 5049 2063 6f6d 6d75 6e69 6361 7469 6f6e  PI communication
+00001df0: 2e0a 2020 2020 7472 6169 6e5f 6a6f 625f  ..    train_job_
+00001e00: 6964 203a 2073 7472 0a20 2020 2020 2020  id : str.       
+00001e10: 2054 6865 2069 6420 6f66 2074 6865 2074   The id of the t
+00001e20: 7261 696e 696e 6720 6a6f 6220 6173 736f  raining job asso
+00001e30: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
+00001e40: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+00001e50: 6e20 6a6f 622e 0a20 2020 206a 6f62 203a  n job..    job :
+00001e60: 204a 6f62 0a20 2020 2020 2020 2054 6865   Job.        The
+00001e70: 204a 6f62 206f 626a 6563 7420 666f 7220   Job object for 
+00001e80: 7468 6973 2063 726f 7373 2d76 616c 6964  this cross-valid
+00001e90: 6174 696f 6e20 6a6f 622e 0a0a 2020 2020  ation job...    
+00001ea0: 4d65 7468 6f64 730a 2020 2020 2d2d 2d2d  Methods.    ----
+00001eb0: 2d2d 2d0a 2020 2020 6372 6f73 7376 616c  ---.    crossval
+00001ec0: 6964 6174 6528 293a 0a20 2020 2020 2020  idate():.       
+00001ed0: 2053 7562 6d69 7473 2061 2063 726f 7373   Submits a cross
+00001ee0: 2d76 616c 6964 6174 696f 6e20 6a6f 6220  -validation job 
+00001ef0: 746f 2074 6865 2073 6572 7665 722e 0a20  to the server.. 
+00001f00: 2020 2067 6574 5f63 726f 7373 7661 6c69     get_crossvali
+00001f10: 6461 7469 6f6e 2870 6167 655f 7369 7a65  dation(page_size
+00001f20: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00001f30: 3d20 4e6f 6e65 2c20 7061 6765 5f6f 6666  = None, page_off
+00001f40: 7365 743a 204f 7074 696f 6e61 6c5b 696e  set: Optional[in
+00001f50: 745d 203d 2030 293a 0a20 2020 2020 2020  t] = 0):.       
+00001f60: 2052 6574 7269 6576 6573 2074 6865 2072   Retrieves the r
+00001f70: 6573 756c 7473 206f 6620 7468 6520 6372  esults of the cr
+00001f80: 6f73 732d 7661 6c69 6461 7469 6f6e 206a  oss-validation j
+00001f90: 6f62 2e0a 2020 2020 2222 220a 0a20 2020  ob..    """..   
+00001fa0: 2073 6573 7369 6f6e 3a20 4150 4953 6573   session: APISes
+00001fb0: 7369 6f6e 0a20 2020 2074 7261 696e 5f6a  sion.    train_j
+00001fc0: 6f62 5f69 643a 2073 7472 0a20 2020 206a  ob_id: str.    j
+00001fd0: 6f62 3a20 4a6f 620a 0a20 2020 2064 6566  ob: Job..    def
+00001fe0: 2063 726f 7373 7661 6c69 6461 7465 2873   crossvalidate(s
+00001ff0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00002000: 220a 2020 2020 2020 2020 5375 626d 6974  ".        Submit
+00002010: 2061 2063 726f 7373 2d76 616c 6964 6174   a cross-validat
+00002020: 696f 6e20 6a6f 6220 746f 2074 6865 2073  ion job to the s
+00002030: 6572 7665 722e 0a0a 2020 2020 2020 2020  erver...        
+00002040: 4966 2074 6865 206a 6f62 2068 6173 2061  If the job has a
+00002050: 6c72 6561 6479 2062 6565 6e20 7375 626d  lready been subm
+00002060: 6974 7465 642c 2061 6e20 496e 7661 6c69  itted, an Invali
+00002070: 644a 6f62 2065 7863 6570 7469 6f6e 2069  dJob exception i
+00002080: 7320 7261 6973 6564 2e0a 0a20 2020 2020  s raised...     
+00002090: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+000020a0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+000020b0: 2020 204a 6f62 0a20 2020 2020 2020 2020     Job.         
+000020c0: 2020 2054 6865 204a 6f62 206f 626a 6563     The Job objec
+000020d0: 7420 666f 7220 7468 6973 2063 726f 7373  t for this cross
+000020e0: 2d76 616c 6964 6174 696f 6e20 6a6f 622e  -validation job.
+000020f0: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00002100: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d0a  .        ------.
+00002110: 2020 2020 2020 2020 496e 7661 6c69 644a          InvalidJ
+00002120: 6f62 0a20 2020 2020 2020 2020 2020 2049  ob.            I
+00002130: 6620 7468 6520 6a6f 6220 6861 7320 616c  f the job has al
+00002140: 7265 6164 7920 6265 656e 2073 7562 6d69  ready been submi
+00002150: 7474 6564 2e0a 2020 2020 2020 2020 2222  tted..        ""
+00002160: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00002170: 662e 6a6f 6220 6973 204e 6f6e 653a 0a20  f.job is None:. 
+00002180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002190: 6a6f 6220 3d20 6372 6f73 7376 616c 6964  job = crossvalid
+000021a0: 6174 6528 7365 6c66 2e73 6573 7369 6f6e  ate(self.session
+000021b0: 2c20 7365 6c66 2e74 7261 696e 5f6a 6f62  , self.train_job
+000021c0: 5f69 6429 0a20 2020 2020 2020 2020 2020  _id).           
+000021d0: 2072 6574 7572 6e20 7365 6c66 2e6a 6f62   return self.job
+000021e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000021f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002200: 2049 6e76 616c 6964 4a6f 6228 0a20 2020   InvalidJob(.   
+00002210: 2020 2020 2020 2020 2020 2020 2022 4356               "CV
+00002220: 204a 6f62 2068 6173 2061 6c72 6561 6479   Job has already
+00002230: 2062 6565 6e20 7375 626d 6974 7465 642e   been submitted.
+00002240: 2055 7365 2067 6574 5f63 726f 7373 7661   Use get_crossva
+00002250: 6c69 6461 7469 6f6e 2829 2069 6e73 7465  lidation() inste
+00002260: 6164 2e22 0a20 2020 2020 2020 2020 2020  ad.".           
+00002270: 2029 0a0a 2020 2020 6465 6620 6765 745f   )..    def get_
+00002280: 6372 6f73 7376 616c 6964 6174 696f 6e28  crossvalidation(
+00002290: 0a20 2020 2020 2020 2073 656c 662c 2070  .        self, p
+000022a0: 6167 655f 7369 7a65 3a20 4f70 7469 6f6e  age_size: Option
+000022b0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c20  al[int] = None, 
+000022c0: 7061 6765 5f6f 6666 7365 743a 204f 7074  page_offset: Opt
+000022d0: 696f 6e61 6c5b 696e 745d 203d 2030 0a20  ional[int] = 0. 
+000022e0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+000022f0: 220a 2020 2020 2020 2020 5265 7472 6965  ".        Retrie
+00002300: 7665 7320 7468 6520 7265 7375 6c74 7320  ves the results 
+00002310: 6f66 2074 6865 2063 726f 7373 2d76 616c  of the cross-val
+00002320: 6964 6174 696f 6e20 6a6f 622e 0a0a 2020  idation job...  
+00002330: 2020 2020 2020 4966 206e 6f20 6a6f 6220        If no job 
+00002340: 6861 7320 6265 656e 2073 7562 6d69 7474  has been submitt
+00002350: 6564 2c20 616e 2049 6e76 616c 6964 4a6f  ed, an InvalidJo
+00002360: 6220 6578 6365 7074 696f 6e20 6973 2072  b exception is r
+00002370: 6169 7365 642e 0a0a 2020 2020 2020 2020  aised...        
+00002380: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00002390: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000023a0: 2020 2020 2020 7061 6765 5f73 697a 6520        page_size 
+000023b0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+000023c0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000023d0: 6e75 6d62 6572 206f 6620 6974 656d 7320  number of items 
+000023e0: 746f 2072 6574 7269 6576 6520 696e 2061  to retrieve in a
+000023f0: 2073 696e 676c 6520 7265 7175 6573 742e   single request.
+00002400: 2e0a 2020 2020 2020 2020 7061 6765 5f6f  ..        page_o
+00002410: 6666 7365 7420 3a20 696e 742c 206f 7074  ffset : int, opt
+00002420: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00002430: 2020 5468 6520 6f66 6673 6574 2074 6f20    The offset to 
+00002440: 7374 6172 7420 7265 7472 6965 7669 6e67  start retrieving
+00002450: 2069 7465 6d73 2066 726f 6d2e 2044 6566   items from. Def
+00002460: 6175 6c74 2069 7320 302e 0a0a 2020 2020  ault is 0...    
+00002470: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00002480: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00002490: 2020 2020 6469 6374 0a20 2020 2020 2020      dict.       
+000024a0: 2020 2020 2054 6865 2072 6573 756c 7473       The results
+000024b0: 206f 6620 7468 6520 6372 6f73 732d 7661   of the cross-va
+000024c0: 6c69 6461 7469 6f6e 206a 6f62 2e0a 0a20  lidation job... 
+000024d0: 2020 2020 2020 2052 6169 7365 730a 2020         Raises.  
+000024e0: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
+000024f0: 2020 2020 2049 6e76 616c 6964 4a6f 620a       InvalidJob.
+00002500: 2020 2020 2020 2020 2020 2020 4966 206e              If n
+00002510: 6f20 6a6f 6220 6861 7320 6265 656e 2073  o job has been s
+00002520: 7562 6d69 7474 6564 2e0a 2020 2020 2020  ubmitted..      
+00002530: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00002540: 2073 656c 662e 6a6f 6220 6973 206e 6f74   self.job is not
+00002550: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002560: 2020 2072 6574 7572 6e20 6765 745f 6372     return get_cr
+00002570: 6f73 7376 616c 6964 6174 696f 6e28 0a20  ossvalidation(. 
+00002580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002590: 656c 662e 7365 7373 696f 6e2c 2073 656c  elf.session, sel
+000025a0: 662e 6a6f 622e 6a6f 625f 6964 2c20 7061  f.job.job_id, pa
+000025b0: 6765 5f73 697a 652c 2070 6167 655f 6f66  ge_size, page_of
+000025c0: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
+000025d0: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+000025e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000025f0: 7365 2049 6e76 616c 6964 4a6f 6228 0a20  se InvalidJob(. 
+00002600: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002610: 4e6f 2043 5620 4a6f 6220 6861 7320 6265  No CV Job has be
+00002620: 656e 2073 7562 6d69 7474 6564 2120 4361  en submitted! Ca
+00002630: 6c6c 2063 726f 7373 7661 6c69 6461 7465  ll crossvalidate
+00002640: 2829 2061 6e64 2074 7279 2061 6761 696e  () and try again
+00002650: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+00002660: 0a0a 0a63 6c61 7373 2043 5646 7574 7572  ...class CVFutur
+00002670: 6528 4356 4675 7475 7265 4d69 7869 6e2c  e(CVFutureMixin,
+00002680: 2041 7379 6e63 4a6f 6246 7574 7572 6529   AsyncJobFuture)
+00002690: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+000026a0: 6973 2063 6c61 7373 2068 656c 7073 2069  is class helps i
+000026b0: 6e69 7469 6174 696e 672c 2073 7562 6d69  nitiating, submi
+000026c0: 7474 696e 672c 2061 6e64 2072 6574 7269  tting, and retri
+000026d0: 6576 696e 6720 7468 650a 2020 2020 7265  eving the.    re
+000026e0: 7375 6c74 7320 6f66 2061 2063 726f 7373  sults of a cross
+000026f0: 2d76 616c 6964 6174 696f 6e20 6a6f 622e  -validation job.
+00002700: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00002710: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00002720: 2020 2020 7365 7373 696f 6e20 3a20 4150      session : AP
+00002730: 4953 6573 7369 6f6e 0a20 2020 2020 2020  ISession.       
+00002740: 2054 6865 2073 6573 7369 6f6e 206f 626a   The session obj
+00002750: 6563 7420 746f 2075 7365 2066 6f72 2041  ect to use for A
+00002760: 5049 2063 6f6d 6d75 6e69 6361 7469 6f6e  PI communication
+00002770: 2e0a 2020 2020 7472 6169 6e5f 6a6f 625f  ..    train_job_
+00002780: 6964 203a 2073 7472 0a20 2020 2020 2020  id : str.       
+00002790: 2054 6865 2069 6420 6f66 2074 6865 2074   The id of the t
+000027a0: 7261 696e 696e 6720 6a6f 6220 6173 736f  raining job asso
+000027b0: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
+000027c0: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+000027d0: 6e20 6a6f 622e 0a20 2020 206a 6f62 203a  n job..    job :
+000027e0: 204a 6f62 0a20 2020 2020 2020 2054 6865   Job.        The
+000027f0: 204a 6f62 206f 626a 6563 7420 666f 7220   Job object for 
+00002800: 7468 6973 2063 726f 7373 2d76 616c 6964  this cross-valid
+00002810: 6174 696f 6e20 6a6f 622e 0a20 2020 2070  ation job..    p
+00002820: 6167 655f 7369 7a65 203a 2069 6e74 0a20  age_size : int. 
+00002830: 2020 2020 2020 2054 6865 206e 756d 6265         The numbe
+00002840: 7220 6f66 2069 7465 6d73 2074 6f20 7265  r of items to re
+00002850: 7472 6965 7665 2069 6e20 6120 7369 6e67  trieve in a sing
+00002860: 6c65 2072 6571 7565 7374 2e0a 0a20 2020  le request...   
+00002870: 204d 6574 686f 6473 0a20 2020 202d 2d2d   Methods.    ---
+00002880: 2d2d 2d2d 0a20 2020 205f 5f73 7472 5f5f  ----.    __str__
+00002890: 2829 3a0a 2020 2020 2020 2020 5265 7475  ():.        Retu
+000028a0: 726e 7320 6120 7374 7269 6e67 2072 6570  rns a string rep
+000028b0: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+000028c0: 6865 2063 726f 7373 2d76 616c 6964 6174  he cross-validat
+000028d0: 696f 6e20 6a6f 622e 0a20 2020 205f 5f72  ion job..    __r
+000028e0: 6570 725f 5f28 293a 0a20 2020 2020 2020  epr__():.       
+000028f0: 2052 6574 7572 6e73 2061 2064 6574 6169   Returns a detai
+00002900: 6c65 6420 7265 7072 6573 656e 7461 7469  led representati
+00002910: 6f6e 206f 6620 7468 6520 6372 6f73 732d  on of the cross-
+00002920: 7661 6c69 6461 7469 6f6e 206a 6f62 2e0a  validation job..
+00002930: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+00002940: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00002950: 7365 7373 696f 6e3a 2041 5049 5365 7373  session: APISess
+00002960: 696f 6e2c 2074 7261 696e 5f6a 6f62 5f69  ion, train_job_i
+00002970: 643a 2073 7472 2c20 6a6f 623a 204a 6f62  d: str, job: Job
+00002980: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00002990: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
+000029a0: 6e73 7472 7563 7473 2061 206e 6577 2043  nstructs a new C
+000029b0: 5646 7574 7572 6520 696e 7374 616e 6365  VFuture instance
+000029c0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+000029d0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+000029e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000029f0: 2073 6573 7369 6f6e 203a 2041 5049 5365   session : APISe
+00002a00: 7373 696f 6e0a 2020 2020 2020 2020 2020  ssion.          
+00002a10: 2020 5468 6520 7365 7373 696f 6e20 6f62    The session ob
+00002a20: 6a65 6374 2074 6f20 7573 6520 666f 7220  ject to use for 
+00002a30: 4150 4920 636f 6d6d 756e 6963 6174 696f  API communicatio
+00002a40: 6e2e 0a20 2020 2020 2020 2074 7261 696e  n..        train
+00002a50: 5f6a 6f62 5f69 6420 3a20 7374 720a 2020  _job_id : str.  
+00002a60: 2020 2020 2020 2020 2020 5468 6520 6964            The id
+00002a70: 206f 6620 7468 6520 7472 6169 6e69 6e67   of the training
+00002a80: 206a 6f62 2061 7373 6f63 6961 7465 6420   job associated 
+00002a90: 7769 7468 2074 6869 7320 6372 6f73 732d  with this cross-
+00002aa0: 7661 6c69 6461 7469 6f6e 206a 6f62 2e0a  validation job..
+00002ab0: 2020 2020 2020 2020 6a6f 6220 3a20 4a6f          job : Jo
+00002ac0: 622c 206f 7074 696f 6e61 6c0a 2020 2020  b, optional.    
+00002ad0: 2020 2020 2020 2020 5468 6520 4a6f 6220          The Job 
+00002ae0: 6f62 6a65 6374 2066 6f72 2074 6869 7320  object for this 
+00002af0: 6372 6f73 732d 7661 6c69 6461 7469 6f6e  cross-validation
+00002b00: 206a 6f62 2e0a 2020 2020 2020 2020 2222   job..        ""
+00002b10: 220a 2020 2020 2020 2020 7375 7065 7228  ".        super(
+00002b20: 292e 5f5f 696e 6974 5f5f 2873 6573 7369  ).__init__(sessi
+00002b30: 6f6e 2c20 6a6f 6229 0a20 2020 2020 2020  on, job).       
+00002b40: 2073 656c 662e 7472 6169 6e5f 6a6f 625f   self.train_job_
+00002b50: 6964 203d 2074 7261 696e 5f6a 6f62 5f69  id = train_job_i
+00002b60: 640a 2020 2020 2020 2020 7365 6c66 2e70  d.        self.p
+00002b70: 6167 655f 7369 7a65 203d 2031 3030 300a  age_size = 1000.
+00002b80: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+00002b90: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+00002ba0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00002bb0: 7228 7365 6c66 2e6a 6f62 290a 0a20 2020  r(self.job)..   
+00002bc0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+00002bd0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+00002be0: 2020 2020 7265 7475 726e 2072 6570 7228      return repr(
+00002bf0: 7365 6c66 2e6a 6f62 290a 0a20 2020 2040  self.job)..    @
+00002c00: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00002c10: 2069 6428 7365 6c66 293a 0a20 2020 2020   id(self):.     
+00002c20: 2020 2072 6574 7572 6e20 7365 6c66 2e6a     return self.j
+00002c30: 6f62 2e6a 6f62 5f69 640a 0a20 2020 2064  ob.job_id..    d
+00002c40: 6566 2067 6574 2873 656c 662c 2076 6572  ef get(self, ver
+00002c50: 626f 7365 3a20 626f 6f6c 203d 2046 616c  bose: bool = Fal
+00002c60: 7365 2920 2d3e 2043 5652 6573 756c 7473  se) -> CVResults
+00002c70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00002c80: 2020 2020 2020 4765 7420 616c 6c20 7468        Get all th
+00002c90: 6520 7265 7375 6c74 7320 6f66 2074 6865  e results of the
+00002ca0: 2043 5620 6a6f 622e 0a0a 2020 2020 2020   CV job...      
+00002cb0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00002cc0: 2020 2020 7665 7262 6f73 6520 2862 6f6f      verbose (boo
+00002cd0: 6c2c 206f 7074 696f 6e61 6c29 3a20 4966  l, optional): If
+00002ce0: 2054 7275 652c 2070 7269 6e74 2076 6572   True, print ver
+00002cf0: 626f 7365 206f 7574 7075 742e 2044 6566  bose output. Def
+00002d00: 6175 6c74 7320 4661 6c73 652e 0a0a 2020  aults False...  
+00002d10: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+00002d20: 2020 2020 2020 2020 2020 4150 4945 7272            APIErr
+00002d30: 6f72 3a20 4966 2074 6865 7265 2069 7320  or: If there is 
+00002d40: 616e 2069 7373 7565 2077 6974 6820 7468  an issue with th
+00002d50: 6520 4150 4920 7265 7175 6573 742e 0a0a  e API request...
+00002d60: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00002d70: 0a20 2020 2020 2020 2020 2020 2050 7265  .            Pre
+00002d80: 6469 6374 4a6f 623a 2041 206c 6973 7420  dictJob: A list 
+00002d90: 6f66 2070 7265 6469 6374 206f 626a 6563  of predict objec
+00002da0: 7473 2072 6570 7265 7365 6e74 696e 6720  ts representing 
+00002db0: 7468 6520 7265 7375 6c74 732e 0a20 2020  the results..   
+00002dc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002dd0: 2073 7465 7020 3d20 7365 6c66 2e70 6167   step = self.pag
+00002de0: 655f 7369 7a65 0a0a 2020 2020 2020 2020  e_size..        
+00002df0: 7265 7375 6c74 7320 3d20 5b5d 0a20 2020  results = [].   
+00002e00: 2020 2020 206e 756d 5f72 6574 7572 6e65       num_returne
+00002e10: 6420 3d20 7374 6570 0a20 2020 2020 2020  d = step.       
+00002e20: 206f 6666 7365 7420 3d20 300a 0a20 2020   offset = 0..   
+00002e30: 2020 2020 2077 6869 6c65 206e 756d 5f72       while num_r
+00002e40: 6574 7572 6e65 6420 3e3d 2073 7465 703a  eturned >= step:
+00002e50: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00002e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002e70: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00002e80: 662e 6765 745f 6372 6f73 7376 616c 6964  f.get_crossvalid
+00002e90: 6174 696f 6e28 7061 6765 5f6f 6666 7365  ation(page_offse
+00002ea0: 743d 6f66 6673 6574 2c20 7061 6765 5f73  t=offset, page_s
+00002eb0: 697a 653d 7374 6570 290a 2020 2020 2020  ize=step).      
+00002ec0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00002ed0: 7320 2b3d 2072 6573 706f 6e73 652e 7265  s += response.re
+00002ee0: 7375 6c74 0a20 2020 2020 2020 2020 2020  sult.           
+00002ef0: 2020 2020 206e 756d 5f72 6574 7572 6e65       num_returne
+00002f00: 6420 3d20 6c65 6e28 7265 7370 6f6e 7365  d = len(response
+00002f10: 2e72 6573 756c 7429 0a20 2020 2020 2020  .result).       
+00002f20: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
+00002f30: 2b3d 206e 756d 5f72 6574 7572 6e65 640a  += num_returned.
+00002f40: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002f50: 7074 2041 5049 4572 726f 7220 6173 2065  pt APIError as e
+00002f60: 7863 3a0a 2020 2020 2020 2020 2020 2020  xc:.            
+00002f70: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f90: 2020 2020 7072 696e 7428 6622 4661 696c      print(f"Fail
+00002fa0: 6564 2074 6f20 6765 7420 7265 7375 6c74  ed to get result
+00002fb0: 733a 207b 6578 637d 2229 0a20 2020 2020  s: {exc}").     
+00002fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002fd0: 6e20 7265 7375 6c74 730a 2020 2020 2020  n results.      
+00002fe0: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+00002ff0: 0a0a 0a63 6c61 7373 2054 7261 696e 4675  ...class TrainFu
+00003000: 7475 7265 4d69 7869 6e3a 0a20 2020 2022  tureMixin:.    "
+00003010: 2222 0a20 2020 2054 6869 7320 636c 6173  "".    This clas
+00003020: 7320 7072 6f76 6964 6573 2066 756e 6374  s provides funct
+00003030: 696f 6e61 6c69 7479 2066 6f72 2072 6574  ionality for ret
+00003040: 7269 6576 696e 6720 7468 650a 2020 2020  rieving the.    
+00003050: 7265 7375 6c74 7320 6f66 2061 2074 7261  results of a tra
+00003060: 696e 696e 6720 6a6f 6220 616e 6420 696e  ining job and in
+00003070: 6974 6961 7469 6e67 2063 726f 7373 2d76  itiating cross-v
+00003080: 616c 6964 6174 696f 6e20 6a6f 6273 2e0a  alidation jobs..
+00003090: 0a20 2020 2041 7474 7269 6275 7465 730a  .    Attributes.
+000030a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000030b0: 2020 2073 6573 7369 6f6e 203a 2041 5049     session : API
+000030c0: 5365 7373 696f 6e0a 2020 2020 2020 2020  Session.        
+000030d0: 5468 6520 7365 7373 696f 6e20 6f62 6a65  The session obje
+000030e0: 6374 2074 6f20 7573 6520 666f 7220 4150  ct to use for AP
+000030f0: 4920 636f 6d6d 756e 6963 6174 696f 6e2e  I communication.
+00003100: 0a20 2020 206a 6f62 203a 204a 6f62 0a20  .    job : Job. 
+00003110: 2020 2020 2020 2054 6865 204a 6f62 206f         The Job o
+00003120: 626a 6563 7420 666f 7220 7468 6973 2074  bject for this t
+00003130: 7261 696e 696e 6720 6a6f 622e 0a20 2020  raining job..   
+00003140: 2063 726f 7373 7661 6c69 6461 7469 6f6e   crossvalidation
+00003150: 203a 2043 5646 7574 7572 650a 2020 2020   : CVFuture.    
+00003160: 2020 2020 5468 6520 4356 4675 7475 7265      The CVFuture
+00003170: 206f 626a 6563 7420 666f 7220 7468 6520   object for the 
+00003180: 6173 736f 6369 6174 6564 2063 726f 7373  associated cross
+00003190: 2d76 616c 6964 6174 696f 6e20 6a6f 622e  -validation job.
+000031a0: 0a0a 2020 2020 4d65 7468 6f64 730a 2020  ..    Methods.  
+000031b0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6765    -------.    ge
+000031c0: 745f 7265 7375 6c74 7328 2920 2d3e 2054  t_results() -> T
+000031d0: 7261 696e 4772 6170 683a 0a20 2020 2020  rainGraph:.     
+000031e0: 2020 2052 6574 7572 6e73 2074 6865 2072     Returns the r
+000031f0: 6573 756c 7473 206f 6620 7468 6520 7472  esults of the tr
+00003200: 6169 6e69 6e67 206a 6f62 2e0a 2020 2020  aining job..    
+00003210: 6372 6f73 7376 616c 6964 6174 6528 293a  crossvalidate():
+00003220: 0a20 2020 2020 2020 2053 7562 6d69 7473  .        Submits
+00003230: 2061 2063 726f 7373 2d76 616c 6964 6174   a cross-validat
+00003240: 696f 6e20 6a6f 6220 616e 6420 7265 7475  ion job and retu
+00003250: 726e 7320 6974 2e0a 2020 2020 2222 220a  rns it..    """.
+00003260: 0a20 2020 2073 6573 7369 6f6e 3a20 4150  .    session: AP
+00003270: 4953 6573 7369 6f6e 0a20 2020 206a 6f62  ISession.    job
+00003280: 3a20 4a6f 620a 2020 2020 6372 6f73 7376  : Job.    crossv
+00003290: 616c 6964 6174 696f 6e3a 2043 5646 7574  alidation: CVFut
+000032a0: 7572 6520 3d20 4e6f 6e65 0a0a 2020 2020  ure = None..    
+000032b0: 6465 6620 6765 745f 7265 7375 6c74 7328  def get_results(
+000032c0: 7365 6c66 2920 2d3e 2054 7261 696e 4772  self) -> TrainGr
+000032d0: 6170 683a 0a20 2020 2020 2020 2022 2222  aph:.        """
+000032e0: 0a20 2020 2020 2020 2047 6574 7320 7468  .        Gets th
+000032f0: 6520 7265 7375 6c74 7320 6f66 2074 6865  e results of the
+00003300: 2074 7261 696e 696e 6720 6a6f 622e 0a0a   training job...
+00003310: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00003320: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00003330: 2020 2020 2020 2020 5472 6169 6e47 7261          TrainGra
+00003340: 7068 0a20 2020 2020 2020 2020 2020 2054  ph.            T
+00003350: 6865 2072 6573 756c 7473 206f 6620 7468  he results of th
+00003360: 6520 7472 6169 6e69 6e67 206a 6f62 2e0a  e training job..
+00003370: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003380: 2020 2020 7265 7475 726e 2067 6574 5f74      return get_t
+00003390: 7261 696e 696e 675f 7265 7375 6c74 7328  raining_results(
+000033a0: 7365 6c66 2e73 6573 7369 6f6e 2c20 7365  self.session, se
+000033b0: 6c66 2e6a 6f62 2e6a 6f62 5f69 6429 0a0a  lf.job.job_id)..
+000033c0: 2020 2020 6465 6620 6372 6f73 7376 616c      def crossval
+000033d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000033e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000033f0: 2053 7562 6d69 7473 2061 2063 726f 7373   Submits a cross
+00003400: 2d76 616c 6964 6174 696f 6e20 6a6f 6220  -validation job 
+00003410: 616e 6420 6269 6e64 7320 6974 2e0a 0a20  and binds it... 
+00003420: 2020 2020 2020 2049 6620 6120 6372 6f73         If a cros
+00003430: 732d 7661 6c69 6461 7469 6f6e 206a 6f62  s-validation job
+00003440: 2068 6173 2061 6c72 6561 6479 2062 6565   has already bee
+00003450: 6e20 6372 6561 7465 642c 2069 7420 7265  n created, it re
+00003460: 7475 726e 7320 7468 6174 206a 6f62 2e0a  turns that job..
+00003470: 2020 2020 2020 2020 4f74 6865 7277 6973          Otherwis
+00003480: 652c 2069 7420 6372 6561 7465 7320 6120  e, it creates a 
+00003490: 6e65 7720 6372 6f73 732d 7661 6c69 6461  new cross-valida
+000034a0: 7469 6f6e 206a 6f62 2061 6e64 2072 6574  tion job and ret
+000034b0: 7572 6e73 2069 742e 0a0a 2020 2020 2020  urns it...      
+000034c0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000034d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000034e0: 2020 4356 4675 7475 7265 0a20 2020 2020    CVFuture.     
+000034f0: 2020 2020 2020 2054 6865 2063 726f 7373         The cross
+00003500: 2d76 616c 6964 6174 696f 6e20 6a6f 6220  -validation job 
+00003510: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00003520: 7468 6973 2074 7261 696e 696e 6720 6a6f  this training jo
+00003530: 622e 0a20 2020 2020 2020 2022 2222 0a20  b..        """. 
+00003540: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00003550: 726f 7373 7661 6c69 6461 7469 6f6e 2069  rossvalidation i
+00003560: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00003570: 2020 2020 7365 6c66 2e63 726f 7373 7661      self.crossva
+00003580: 6c69 6461 7469 6f6e 203d 2043 5646 7574  lidation = CVFut
+00003590: 7572 6528 7365 6c66 2e73 6573 7369 6f6e  ure(self.session
+000035a0: 2c20 7365 6c66 2e6a 6f62 2e6a 6f62 5f69  , self.job.job_i
+000035b0: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
+000035c0: 6e20 7365 6c66 2e63 726f 7373 7661 6c69  n self.crossvali
+000035d0: 6461 7469 6f6e 2e63 726f 7373 7661 6c69  dation.crossvali
+000035e0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+000035f0: 6765 745f 6173 7361 795f 6461 7461 2873  get_assay_data(s
+00003600: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00003610: 220a 2020 2020 2020 2020 4e4f 5420 494d  ".        NOT IM
+00003620: 504c 454d 454e 5445 442e 0a0a 2020 2020  PLEMENTED...    
+00003630: 2020 2020 4765 7420 7468 6520 6173 7361      Get the assa
+00003640: 7920 6461 7461 2075 7365 6420 666f 7220  y data used for 
+00003650: 7468 6520 7472 6169 6e69 6e67 206a 6f62  the training job
+00003660: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00003670: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00003680: 5468 6520 6173 7361 7920 6461 7461 2e0a  The assay data..
+00003690: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000036a0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+000036b0: 6c65 6d65 6e74 6564 4572 726f 7228 2267  lementedError("g
+000036c0: 6574 5f61 7373 6179 5f64 6174 6120 6973  et_assay_data is
+000036d0: 206e 6f74 2061 7661 696c 6162 6c65 2e22   not available."
+000036e0: 290a 0a20 2020 2064 6566 206c 6973 745f  )..    def list_
+000036f0: 6d6f 6465 6c73 2873 656c 6629 3a0a 2020  models(self):.  
+00003700: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003710: 2020 4c69 7374 206d 6f64 656c 7320 6173    List models as
+00003720: 736f 6963 6174 6564 2077 6974 6820 6a6f  soicated with jo
+00003730: 620a 0a20 2020 2020 2020 2050 6172 616d  b..        Param
+00003740: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00003750: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00003760: 2073 6573 7369 6f6e 203a 2041 5049 5365   session : APISe
+00003770: 7373 696f 6e0a 2020 2020 2020 2020 2020  ssion.          
+00003780: 2020 5365 7373 696f 6e20 6f62 6a65 6374    Session object
+00003790: 2066 6f72 2041 5049 2063 6f6d 6d75 6e69   for API communi
+000037a0: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
+000037b0: 6a6f 625f 6964 203a 2073 7472 0a20 2020  job_id : str.   
+000037c0: 2020 2020 2020 2020 206a 6f62 2049 440a           job ID.
+000037d0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000037e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000037f0: 0a20 2020 2020 2020 204c 6973 740a 2020  .        List.  
+00003800: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
+00003810: 6620 6d6f 6465 6c73 0a20 2020 2020 2020  f models.       
+00003820: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00003830: 7572 6e20 6c69 7374 5f6d 6f64 656c 7328  urn list_models(
+00003840: 7365 6c66 2e73 6573 7369 6f6e 2c20 7365  self.session, se
+00003850: 6c66 2e6a 6f62 2e6a 6f62 5f69 6429 0a0a  lf.job.job_id)..
+00003860: 0a63 6c61 7373 2054 7261 696e 4675 7475  .class TrainFutu
+00003870: 7265 2854 7261 696e 4675 7475 7265 4d69  re(TrainFutureMi
+00003880: 7869 6e2c 2041 7379 6e63 4a6f 6246 7574  xin, AsyncJobFut
+00003890: 7572 6529 3a0a 2020 2020 2222 2246 7574  ure):.    """Fut
+000038a0: 7572 6520 4a6f 6220 666f 7220 6d61 6e69  ure Job for mani
+000038b0: 7075 6c61 7469 6e67 2072 6573 756c 7473  pulating results
+000038c0: 2222 220a 2020 2020 6465 6620 5f5f 696e  """.    def __in
+000038d0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000038e0: 6c66 2c0a 2020 2020 2020 2020 7365 7373  lf,.        sess
+000038f0: 696f 6e3a 2041 5049 5365 7373 696f 6e2c  ion: APISession,
+00003900: 0a20 2020 2020 2020 206a 6f62 3a20 4a6f  .        job: Jo
+00003910: 622c 0a20 2020 2020 2020 2061 7373 6179  b,.        assay
+00003920: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
+00003930: 616c 5b41 7373 6179 4d65 7461 6461 7461  al[AssayMetadata
+00003940: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00003950: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00003960: 2e5f 5f69 6e69 745f 5f28 7365 7373 696f  .__init__(sessio
+00003970: 6e2c 206a 6f62 290a 2020 2020 2020 2020  n, job).        
+00003980: 7365 6c66 2e61 7373 6179 6d65 7461 6461  self.assaymetada
+00003990: 7461 203d 2061 7373 6179 6d65 7461 6461  ta = assaymetada
+000039a0: 7461 0a20 2020 2020 2020 2073 656c 662e  ta.        self.
+000039b0: 6372 6f73 7376 616c 6964 6174 696f 6e3a  crossvalidation:
+000039c0: 204f 7074 696f 6e61 6c5b 4356 4675 7475   Optional[CVFutu
+000039d0: 7265 5d20 3d20 4356 4675 7475 7265 2873  re] = CVFuture(s
+000039e0: 6573 7369 6f6e 2c20 6a6f 622e 6a6f 625f  ession, job.job_
+000039f0: 6964 2c20 4e6f 6e65 290a 0a20 2020 2064  id, None)..    d
+00003a00: 6566 205f 5f73 7472 5f5f 2873 656c 6629  ef __str__(self)
+00003a10: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00003a20: 2072 6574 7572 6e20 7374 7228 7365 6c66   return str(self
+00003a30: 2e6a 6f62 290a 0a20 2020 2064 6566 205f  .job)..    def _
+00003a40: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+00003a50: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+00003a60: 7475 726e 2072 6570 7228 7365 6c66 2e6a  turn repr(self.j
+00003a70: 6f62 290a 0a20 2020 2040 7072 6f70 6572  ob)..    @proper
+00003a80: 7479 0a20 2020 2064 6566 2069 6428 7365  ty.    def id(se
+00003a90: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00003aa0: 7572 6e20 7365 6c66 2e6a 6f62 2e6a 6f62  urn self.job.job
+00003ab0: 5f69 640a 0a20 2020 2064 6566 2067 6574  _id..    def get
+00003ac0: 5f61 7373 6179 5f64 6174 6128 7365 6c66  _assay_data(self
+00003ad0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00003ae0: 2020 2020 2020 204e 4f54 2049 4d50 4c45         NOT IMPLE
+00003af0: 4d45 4e54 4544 2e0a 0a20 2020 2020 2020  MENTED...       
+00003b00: 2047 6574 2074 6865 2061 7373 6179 2064   Get the assay d
+00003b10: 6174 6120 7573 6564 2066 6f72 2074 6865  ata used for the
+00003b20: 2074 7261 696e 696e 6720 6a6f 622e 0a0a   training job...
+00003b30: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003b40: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00003b50: 2061 7373 6179 2064 6174 612e 0a20 2020   assay data..   
+00003b60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003b70: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+00003b80: 5f61 7373 6179 5f64 6174 6128 290a 0a20  _assay_data().. 
+00003b90: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
+00003ba0: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
+00003bb0: 2046 616c 7365 2920 2d3e 2054 7261 696e   False) -> Train
+00003bc0: 4772 6170 683a 0a20 2020 2020 2020 2074  Graph:.        t
+00003bd0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00003be0: 7265 7375 6c74 7320 3d20 7365 6c66 2e67  results = self.g
+00003bf0: 6574 5f72 6573 756c 7473 2829 0a20 2020  et_results().   
+00003c00: 2020 2020 2065 7863 6570 7420 4150 4945       except APIE
+00003c10: 7272 6f72 2061 7320 6578 633a 0a20 2020  rror as exc:.   
+00003c20: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
+00003c30: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00003c40: 2020 2020 2070 7269 6e74 2866 2246 6169       print(f"Fai
+00003c50: 6c65 6420 746f 2067 6574 2072 6573 756c  led to get resul
+00003c60: 7473 3a20 7b65 7863 7d22 290a 2020 2020  ts: {exc}").    
+00003c70: 2020 2020 2020 2020 7261 6973 6520 6578          raise ex
+00003c80: 630a 2020 2020 2020 2020 7265 7475 726e  c.        return
+00003c90: 2072 6573 756c 7473 0a0a 0a63 6c61 7373   results...class
+00003ca0: 2054 7261 696e 696e 6741 5049 3a0a 2020   TrainingAPI:.  
+00003cb0: 2020 2222 2241 5049 2069 6e74 6572 6661    """API interfa
+00003cc0: 6365 2066 6f72 2063 616c 6c69 6e67 2054  ce for calling T
+00003cd0: 7261 696e 2065 6e64 706f 696e 7473 2222  rain endpoints""
+00003ce0: 220a 2020 2020 6465 6620 5f5f 696e 6974  ".    def __init
+00003cf0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00003d00: 2c0a 2020 2020 2020 2020 7365 7373 696f  ,.        sessio
+00003d10: 6e3a 2041 5049 5365 7373 696f 6e2c 0a20  n: APISession,. 
+00003d20: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00003d30: 6c66 2e73 6573 7369 6f6e 203d 2073 6573  lf.session = ses
+00003d40: 7369 6f6e 0a20 2020 2020 2020 2073 656c  sion.        sel
+00003d50: 662e 6173 7361 7920 3d20 4e6f 6e65 0a0a  f.assay = None..
+00003d60: 2020 2020 6465 6620 6372 6561 7465 5f74      def create_t
+00003d70: 7261 696e 696e 675f 6a6f 6228 0a20 2020  raining_job(.   
+00003d80: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00003d90: 2020 2061 7373 6179 6461 7461 7365 743a     assaydataset:
+00003da0: 2041 7373 6179 4461 7461 7365 742c 0a20   AssayDataset,. 
+00003db0: 2020 2020 2020 206d 6561 7375 7265 6d65         measureme
+00003dc0: 6e74 5f6e 616d 653a 2055 6e69 6f6e 5b73  nt_name: Union[s
+00003dd0: 7472 2c20 4c69 7374 5b73 7472 5d5d 2c0a  tr, List[str]],.
+00003de0: 2020 2020 2020 2020 6d6f 6465 6c5f 6e61          model_na
+00003df0: 6d65 3a20 7374 7220 3d20 2222 2c0a 2020  me: str = "",.  
+00003e00: 2020 2020 2020 666f 7263 655f 7072 6570        force_prep
+00003e10: 726f 6365 7373 3a20 4f70 7469 6f6e 616c  rocess: Optional
+00003e20: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+00003e30: 2020 2020 2920 2d3e 2054 7261 696e 4675      ) -> TrainFu
+00003e40: 7475 7265 3a0a 2020 2020 2020 2020 2222  ture:.        ""
+00003e50: 220a 2020 2020 2020 2020 4372 6561 7465  ".        Create
+00003e60: 2061 2074 7261 696e 696e 6720 6a6f 6220   a training job 
+00003e70: 6f6e 2079 6f75 7220 6461 7461 2e0a 0a20  on your data... 
+00003e80: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
+00003e90: 7469 6f6e 2076 616c 6964 6174 6573 2074  tion validates t
+00003ea0: 6865 2069 6e70 7574 732c 2066 6f72 6d61  he inputs, forma
+00003eb0: 7473 2074 6865 2064 6174 612c 2061 6e64  ts the data, and
+00003ec0: 2073 656e 6473 2074 6865 206a 6f62 2e0a   sends the job..
+00003ed0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00003ee0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00003ef0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
+00003f00: 7373 6179 6461 7461 7365 7420 3a20 4173  ssaydataset : As
+00003f10: 7361 7944 6174 6173 6574 0a20 2020 2020  sayDataset.     
+00003f20: 2020 2020 2020 2041 6e20 4173 7361 7944         An AssayD
+00003f30: 6174 6173 6574 206f 626a 6563 7420 6672  ataset object fr
+00003f40: 6f6d 2077 6869 6368 2074 6865 2061 7373  om which the ass
+00003f50: 6179 5f69 6420 6973 2065 7874 7261 6374  ay_id is extract
+00003f60: 6564 2e0a 2020 2020 2020 2020 6d65 6173  ed..        meas
+00003f70: 7572 656d 656e 745f 6e61 6d65 203a 2073  urement_name : s
+00003f80: 7472 206f 7220 4c69 7374 5b73 7472 5d0a  tr or List[str].
+00003f90: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00003fa0: 6e61 6d65 2873 2920 6f66 2074 6865 206d  name(s) of the m
+00003fb0: 6561 7375 7265 6d65 6e74 2873 2920 746f  easurement(s) to
+00003fc0: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
+00003fd0: 7472 6169 6e69 6e67 206a 6f62 2e0a 2020  training job..  
+00003fe0: 2020 2020 2020 6d6f 6465 6c5f 6e61 6d65        model_name
+00003ff0: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+00004000: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00004010: 206e 616d 6520 746f 2067 6976 6520 7468   name to give th
+00004020: 6520 6d6f 6465 6c2e 0a20 2020 2020 2020  e model..       
+00004030: 2066 6f72 6365 5f70 7265 7072 6f63 6573   force_preproces
+00004040: 7320 3a20 626f 6f6c 2c20 6f70 7469 6f6e  s : bool, option
+00004050: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
+00004060: 6620 7365 7420 746f 2054 7275 652c 2070  f set to True, p
+00004070: 7265 7072 6f63 6573 7369 6e67 2069 7320  reprocessing is 
+00004080: 666f 7263 6564 2065 7665 6e20 6966 2064  forced even if d
+00004090: 6174 6120 616c 7265 6164 7920 6578 6973  ata already exis
+000040a0: 7473 2e0a 0a20 2020 2020 2020 2052 6574  ts...        Ret
+000040b0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000040c0: 2d2d 2d2d 0a20 2020 2020 2020 2054 7261  ----.        Tra
+000040d0: 696e 4675 7475 7265 0a20 2020 2020 2020  inFuture.       
+000040e0: 2020 2020 2041 2054 7261 696e 4675 7475       A TrainFutu
+000040f0: 7265 204a 6f62 0a0a 2020 2020 2020 2020  re Job..        
+00004100: 5261 6973 6573 0a20 2020 2020 2020 202d  Raises.        -
+00004110: 2d2d 2d2d 2d0a 2020 2020 2020 2020 496e  -----.        In
+00004120: 7661 6c69 6450 6172 616d 6574 6572 4572  validParameterEr
+00004130: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+00004140: 4966 2074 6865 2060 6173 7361 7964 6174  If the `assaydat
+00004150: 6173 6574 6020 6973 206e 6f74 2061 6e20  aset` is not an 
+00004160: 4173 7361 7944 6174 6173 6574 206f 626a  AssayDataset obj
+00004170: 6563 742c 0a20 2020 2020 2020 2020 2020  ect,.           
+00004180: 2049 6620 616e 7920 6d65 6173 7572 656d   If any measurem
+00004190: 656e 7420 6e61 6d65 2070 726f 7669 6465  ent name provide
+000041a0: 6420 646f 6573 206e 6f74 2065 7869 7374  d does not exist
+000041b0: 2069 6e20 7468 6520 4173 7361 7944 6174   in the AssayDat
+000041c0: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
+000041d0: 2020 6f72 2069 6620 7468 6520 4173 7361    or if the Assa
+000041e0: 7944 6174 6173 6574 2068 6173 2066 6577  yDataset has few
+000041f0: 6572 2074 6861 6e20 3320 6461 7461 2070  er than 3 data p
+00004200: 6f69 6e74 732e 0a20 2020 2020 2020 2048  oints..        H
+00004210: 5454 5045 7272 6f72 0a20 2020 2020 2020  TTPError.       
+00004220: 2020 2020 2049 6620 7468 6520 7265 7175       If the requ
+00004230: 6573 7420 746f 2074 6865 2073 6572 7665  est to the serve
+00004240: 7220 6661 696c 732e 0a20 2020 2020 2020  r fails..       
+00004250: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00004260: 6973 696e 7374 616e 6365 286d 6561 7375  isinstance(measu
+00004270: 7265 6d65 6e74 5f6e 616d 652c 2073 7472  rement_name, str
+00004280: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
+00004290: 6561 7375 7265 6d65 6e74 5f6e 616d 6520  easurement_name 
+000042a0: 3d20 5b6d 6561 7375 7265 6d65 6e74 5f6e  = [measurement_n
+000042b0: 616d 655d 0a20 2020 2020 2020 206a 6f62  ame].        job
+000042c0: 5f64 6574 6169 6c73 203d 2063 7265 6174  _details = creat
+000042d0: 655f 7472 6169 6e5f 6a6f 6228 0a20 2020  e_train_job(.   
+000042e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000042f0: 7373 696f 6e2c 2061 7373 6179 6461 7461  ssion, assaydata
+00004300: 7365 742c 206d 6561 7375 7265 6d65 6e74  set, measurement
+00004310: 5f6e 616d 652c 206d 6f64 656c 5f6e 616d  _name, model_nam
+00004320: 652c 2066 6f72 6365 5f70 7265 7072 6f63  e, force_preproc
+00004330: 6573 730a 2020 2020 2020 2020 290a 2020  ess.        ).  
+00004340: 2020 2020 2020 7265 7475 726e 2054 7261        return Tra
+00004350: 696e 4675 7475 7265 2873 656c 662e 7365  inFuture(self.se
+00004360: 7373 696f 6e2c 206a 6f62 5f64 6574 6169  ssion, job_detai
+00004370: 6c73 2c20 6173 7361 7964 6174 6173 6574  ls, assaydataset
+00004380: 290a 0a20 2020 2064 6566 205f 6372 6561  )..    def _crea
+00004390: 7465 5f74 7261 696e 696e 675f 6a6f 625f  te_training_job_
+000043a0: 6272 280a 2020 2020 2020 2020 7365 6c66  br(.        self
+000043b0: 2c0a 2020 2020 2020 2020 6173 7361 7964  ,.        assayd
+000043c0: 6174 6173 6574 3a20 4173 7361 7944 6174  ataset: AssayDat
+000043d0: 6173 6574 2c0a 2020 2020 2020 2020 6d65  aset,.        me
+000043e0: 6173 7572 656d 656e 745f 6e61 6d65 3a20  asurement_name: 
+000043f0: 556e 696f 6e5b 7374 722c 204c 6973 745b  Union[str, List[
+00004400: 7374 725d 5d2c 0a20 2020 2020 2020 206d  str]],.        m
+00004410: 6f64 656c 5f6e 616d 653a 2073 7472 203d  odel_name: str =
+00004420: 2022 222c 0a20 2020 2020 2020 2066 6f72   "",.        for
+00004430: 6365 5f70 7265 7072 6f63 6573 733a 204f  ce_preprocess: O
+00004440: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00004450: 4661 6c73 652c 0a20 2020 2029 202d 3e20  False,.    ) -> 
+00004460: 5472 6169 6e46 7574 7572 653a 0a20 2020  TrainFuture:.   
+00004470: 2020 2020 2022 2222 5361 6d65 2061 7320       """Same as 
+00004480: 6372 6561 7465 5f74 7261 696e 696e 675f  create_training_
+00004490: 6a6f 622e 2222 220a 2020 2020 2020 2020  job.""".        
+000044a0: 6a6f 625f 6465 7461 696c 7320 3d20 5f63  job_details = _c
+000044b0: 7265 6174 655f 7472 6169 6e5f 6a6f 625f  reate_train_job_
+000044c0: 6272 280a 2020 2020 2020 2020 2020 2020  br(.            
+000044d0: 7365 6c66 2e73 6573 7369 6f6e 2c20 6173  self.session, as
+000044e0: 7361 7964 6174 6173 6574 2c20 6d65 6173  saydataset, meas
+000044f0: 7572 656d 656e 745f 6e61 6d65 2c20 6d6f  urement_name, mo
+00004500: 6465 6c5f 6e61 6d65 2c20 666f 7263 655f  del_name, force_
+00004510: 7072 6570 726f 6365 7373 0a20 2020 2020  preprocess.     
+00004520: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00004530: 7572 6e20 5472 6169 6e46 7574 7572 6528  urn TrainFuture(
+00004540: 7365 6c66 2e73 6573 7369 6f6e 2c20 6a6f  self.session, jo
+00004550: 625f 6465 7461 696c 732c 2061 7373 6179  b_details, assay
+00004560: 6461 7461 7365 7429 0a0a 2020 2020 6465  dataset)..    de
+00004570: 6620 5f63 7265 6174 655f 7472 6169 6e69  f _create_traini
+00004580: 6e67 5f6a 6f62 5f67 7028 0a20 2020 2020  ng_job_gp(.     
+00004590: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000045a0: 2061 7373 6179 6461 7461 7365 743a 2041   assaydataset: A
+000045b0: 7373 6179 4461 7461 7365 742c 0a20 2020  ssayDataset,.   
+000045c0: 2020 2020 206d 6561 7375 7265 6d65 6e74       measurement
+000045d0: 5f6e 616d 653a 2055 6e69 6f6e 5b73 7472  _name: Union[str
+000045e0: 2c20 4c69 7374 5b73 7472 5d5d 2c0a 2020  , List[str]],.  
+000045f0: 2020 2020 2020 6d6f 6465 6c5f 6e61 6d65        model_name
+00004600: 3a20 7374 7220 3d20 2222 2c0a 2020 2020  : str = "",.    
+00004610: 2020 2020 666f 7263 655f 7072 6570 726f      force_prepro
+00004620: 6365 7373 3a20 4f70 7469 6f6e 616c 5b62  cess: Optional[b
+00004630: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
+00004640: 2020 2920 2d3e 2054 7261 696e 4675 7475    ) -> TrainFutu
+00004650: 7265 3a0a 2020 2020 2020 2020 2222 2253  re:.        """S
+00004660: 616d 6520 6173 2063 7265 6174 655f 7472  ame as create_tr
+00004670: 6169 6e69 6e67 5f6a 6f62 2e22 2222 0a20  aining_job.""". 
+00004680: 2020 2020 2020 206a 6f62 5f64 6574 6169         job_detai
+00004690: 6c73 203d 205f 6372 6561 7465 5f74 7261  ls = _create_tra
+000046a0: 696e 5f6a 6f62 5f67 7028 0a20 2020 2020  in_job_gp(.     
+000046b0: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+000046c0: 696f 6e2c 2061 7373 6179 6461 7461 7365  ion, assaydatase
+000046d0: 742c 206d 6561 7375 7265 6d65 6e74 5f6e  t, measurement_n
+000046e0: 616d 652c 206d 6f64 656c 5f6e 616d 652c  ame, model_name,
+000046f0: 2066 6f72 6365 5f70 7265 7072 6f63 6573   force_preproces
+00004700: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
+00004710: 2020 2020 7265 7475 726e 2054 7261 696e      return Train
+00004720: 4675 7475 7265 2873 656c 662e 7365 7373  Future(self.sess
+00004730: 696f 6e2c 206a 6f62 5f64 6574 6169 6c73  ion, job_details
+00004740: 2c20 6173 7361 7964 6174 6173 6574 290a  , assaydataset).
+00004750: 0a20 2020 2064 6566 2067 6574 5f74 7261  .    def get_tra
+00004760: 696e 696e 675f 7265 7375 6c74 7328 7365  ining_results(se
+00004770: 6c66 2c20 6a6f 625f 6964 3a20 7374 7229  lf, job_id: str)
+00004780: 202d 3e20 5472 6169 6e46 7574 7572 653a   -> TrainFuture:
+00004790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000047a0: 2020 2020 2047 6574 2074 7261 696e 696e       Get trainin
+000047b0: 6720 7265 7375 6c74 7320 2865 2e67 2e20  g results (e.g. 
+000047c0: 6c6f 7373 2065 7463 292e 0a0a 2020 2020  loss etc)...    
+000047d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000047e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000047f0: 2d0a 2020 2020 2020 2020 6a6f 625f 6964  -.        job_id
+00004800: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
+00004810: 2020 206a 6f62 5f69 6420 746f 2067 6574     job_id to get
+00004820: 0a0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00004830: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00004840: 2d2d 0a20 2020 2020 2020 2054 7261 696e  --.        Train
+00004850: 4675 7475 7265 0a20 2020 2020 2020 2020  Future.         
+00004860: 2020 2041 2054 7261 696e 4675 7475 7265     A TrainFuture
+00004870: 204a 6f62 0a20 2020 2020 2020 2022 2222   Job.        """
+00004880: 0a20 2020 2020 2020 206a 6f62 5f64 6574  .        job_det
+00004890: 6169 6c73 203d 2067 6574 5f74 7261 696e  ails = get_train
+000048a0: 696e 675f 7265 7375 6c74 7328 7365 6c66  ing_results(self
+000048b0: 2e73 6573 7369 6f6e 2c20 6a6f 625f 6964  .session, job_id
+000048c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000048d0: 2054 7261 696e 4675 7475 7265 2873 656c   TrainFuture(sel
+000048e0: 662e 7365 7373 696f 6e2c 206a 6f62 5f64  f.session, job_d
+000048f0: 6574 6169 6c73 290a 0a20 2020 2064 6566  etails)..    def
+00004900: 206c 6f61 645f 6a6f 6228 7365 6c66 2c20   load_job(self, 
+00004910: 6a6f 625f 6964 3a20 7374 7229 202d 3e20  job_id: str) -> 
+00004920: 4a6f 6270 6c75 733a 0a20 2020 2020 2020  Jobplus:.       
+00004930: 2022 2222 0a20 2020 2020 2020 2052 656c   """.        Rel
+00004940: 6f61 6420 6120 5375 626d 6974 7465 6420  oad a Submitted 
+00004950: 6a6f 6220 746f 2072 6573 756d 6520 6672  job to resume fr
+00004960: 6f6d 2077 6865 7265 2079 6f75 206c 6566  om where you lef
+00004970: 7420 6f66 6621 0a0a 0a20 2020 2020 2020  t off!...       
+00004980: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00004990: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000049a0: 2020 2020 2020 206a 6f62 5f69 6420 3a20         job_id : 
+000049b0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+000049c0: 5468 6520 6964 656e 7469 6669 6572 206f  The identifier o
+000049d0: 6620 7468 6520 6a6f 6220 7768 6f73 6520  f the job whose 
+000049e0: 6465 7461 696c 7320 6172 6520 746f 2062  details are to b
+000049f0: 6520 6c6f 6164 6564 2e0a 0a20 2020 2020  e loaded...     
+00004a00: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00004a10: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00004a20: 2020 204a 6f62 0a20 2020 2020 2020 2020     Job.         
+00004a30: 2020 204a 6f62 0a0a 2020 2020 2020 2020     Job..        
+00004a40: 5261 6973 6573 0a20 2020 2020 2020 202d  Raises.        -
+00004a50: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4854  -----.        HT
+00004a60: 5450 4572 726f 720a 2020 2020 2020 2020  TPError.        
+00004a70: 2020 2020 4966 2074 6865 2072 6571 7565      If the reque
+00004a80: 7374 2074 6f20 7468 6520 7365 7276 6572  st to the server
+00004a90: 2066 6169 6c73 2e0a 2020 2020 2020 2020   fails..        
+00004aa0: 496e 7661 6c69 644a 6f62 0a20 2020 2020  InvalidJob.     
+00004ab0: 2020 2020 2020 2049 6620 7468 6520 4a6f         If the Jo
+00004ac0: 6220 6973 206f 6620 7468 6520 7772 6f6e  b is of the wron
+00004ad0: 6720 7479 7065 0a0a 2020 2020 2020 2020  g type..        
+00004ae0: 2222 220a 2020 2020 2020 2020 6a6f 625f  """.        job_
+00004af0: 6465 7461 696c 7320 3d20 6c6f 6164 5f6a  details = load_j
+00004b00: 6f62 2873 656c 662e 7365 7373 696f 6e2c  ob(self.session,
+00004b10: 206a 6f62 5f69 6429 0a20 2020 2020 2020   job_id).       
+00004b20: 2061 7373 6179 5f6d 6574 6164 6174 6120   assay_metadata 
+00004b30: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+00004b40: 6966 206a 6f62 5f64 6574 6169 6c73 2e6a  if job_details.j
+00004b50: 6f62 5f74 7970 6520 213d 204a 6f62 5479  ob_type != JobTy
+00004b60: 7065 2e74 7261 696e 3a0a 2020 2020 2020  pe.train:.      
+00004b70: 2020 2020 2020 7261 6973 6520 496e 7661        raise Inva
+00004b80: 6c69 644a 6f62 2866 224a 6f62 207b 6a6f  lidJob(f"Job {jo
+00004b90: 625f 6964 7d20 6973 206e 6f74 206f 6620  b_id} is not of 
+00004ba0: 7479 7065 207b 4a6f 6254 7970 652e 7472  type {JobType.tr
+00004bb0: 6169 6e7d 2229 0a20 2020 2020 2020 2072  ain}").        r
+00004bc0: 6574 7572 6e20 5472 6169 6e46 7574 7572  eturn TrainFutur
+00004bd0: 6528 7365 6c66 2e73 6573 7369 6f6e 2c20  e(self.session, 
+00004be0: 6a6f 625f 6465 7461 696c 732c 2061 7373  job_details, ass
+00004bf0: 6179 5f6d 6574 6164 6174 6129 0a         ay_metadata).
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/data.py` & `openprotein_python-0.1.1b9/openprotein/api/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pydantic
 from typing import Optional, List
 from io import BytesIO
 
-from openprotein_python.models import AssayMetadata, AssayDataPage
-from openprotein_python.errors import APIError
-from openprotein_python.base import APISession
-import openprotein_python.config as config
+from openprotein.models import AssayMetadata, AssayDataPage
+from openprotein.errors import APIError
+from openprotein.base import APISession
+import openprotein.config as config
 
 
 def list_models(session: APISession, assay_id: str) -> List:
     """
     List models assoicated with assay.
 
     Parameters
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/design.py` & `openprotein_python-0.1.1b9/openprotein/api/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 import pydantic
 
-from openprotein_python.base import APISession
-from openprotein_python.api.jobs import AsyncJobFuture, Job
-import openprotein_python.config as config
-from openprotein_python.api.jobs import load_job
-from openprotein_python.models import DesignJobCreate, JobType, DesignResults
-from openprotein_python.errors import (
+from openprotein.base import APISession
+from openprotein.api.jobs import AsyncJobFuture, Job
+import openprotein.config as config
+from openprotein.api.jobs import load_job
+from openprotein.models import DesignJobCreate, JobType, DesignResults
+from openprotein.errors import (
     APIError,
     InvalidJob,
 )
 
 def create_design_job(session: APISession, design_job: DesignJobCreate) -> Job:
     """
     Send a POST request for protein design job.
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/embedding.py` & `openprotein_python-0.1.1b9/openprotein/api/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from openprotein_python.base import APISession
-from openprotein_python.api.jobs import (
+from openprotein.base import APISession
+from openprotein.api.jobs import (
     Job,
     MappedAsyncJobFuture,
     PagedAsyncJobFuture,
     job_get,
     JobStatus,
 )
-from openprotein_python.errors import InvalidJob
-import openprotein_python.config as config
-from openprotein_python.api.jobs import load_job
-from openprotein_python.models import (
+from openprotein.errors import InvalidJob
+import openprotein.config as config
+from openprotein.api.jobs import load_job
+from openprotein.models import (
     ModelDescription,
     TokenInfo,
     ModelMetadata,
     EmbeddedSequence,
     SVDMetadata,
     SVDJob,
     JobType,
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/jobs.py` & `openprotein_python-0.1.1b9/openprotein/api/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import time
 from enum import Enum
 
 import tqdm
 import pydantic
 from pydantic import BaseModel
 
-from openprotein_python.errors import TimeoutException
-from openprotein_python.base import APISession
-import openprotein_python.config as config
+from openprotein.errors import TimeoutException
+from openprotein.base import APISession
+import openprotein.config as config
 
 
 class JobStatus(str, Enum):
     PENDING: str = "PENDING"
     RUNNING: str = "RUNNING"
     SUCCESS: str = "SUCCESS"
     FAILURE: str = "FAILURE"
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/poet.py` & `openprotein_python-0.1.1b9/openprotein/api/poet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Optional, List, Union, BinaryIO, Iterator
 from io import BytesIO
 import random
 import csv
 import codecs
 import requests
 
-from openprotein_python.base import APISession
-from openprotein_python.api.jobs import (
+from openprotein.base import APISession
+from openprotein.api.jobs import (
     Job,
     AsyncJobFuture,
     StreamingAsyncJobFuture,
     job_get,
     job_args_get,
 )
-from openprotein_python.api.jobs import load_job #as base_load_job
-import openprotein_python.config as config
+from openprotein.api.jobs import load_job #as base_load_job
+import openprotein.config as config
 
-from openprotein_python.models import (
+from openprotein.models import (
     MSASamplingMethod,
     PoetInputType,
     PoetScoreJob,
     PoetScoreResult,
     PromptJob,
     MSAJob,
     JobType,
     PoetSSPJob,
     PoetSSPResult,
 )
-from openprotein_python.errors import (
+from openprotein.errors import (
     InvalidParameterError,
     MissingParameterError,
     APIError,
     InvalidJob,
 )
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/api/predict.py` & `openprotein_python-0.1.1b9/openprotein/api/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, List, Union
 import pydantic
 
-from openprotein_python.base import APISession
-from openprotein_python.api.jobs import AsyncJobFuture, Job
-from openprotein_python.models import (
+from openprotein.base import APISession
+from openprotein.api.jobs import AsyncJobFuture, Job
+from openprotein.models import (
     SequenceDataset,
     SequenceData,
     PredictJob,
     PredictSingleSiteJob,
     JobType,
 )
-from openprotein_python.errors import InvalidParameterError, APIError, InvalidJob
-from openprotein_python.api.train import TrainFuture
-from openprotein_python.api.jobs import load_job
+from openprotein.errors import InvalidParameterError, APIError, InvalidJob
+from openprotein.api.train import TrainFuture
+from openprotein.api.jobs import load_job
 
 
 def _create_predict_job(
     session: APISession,
     endpoint: str,
     payload: dict,
     model_ids: Optional[List[str]] = None,
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/base.py` & `openprotein_python-0.1.1b9/openprotein/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import openprotein_python.config as config
+import openprotein.config as config
 
 import requests
 from urllib.parse import urljoin
 from typing import Union
 
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
-from openprotein_python.errors import APIError, InvalidParameterError, MissingParameterError, AuthError
+from openprotein.errors import APIError, InvalidParameterError, MissingParameterError, AuthError
 
 class BearerAuth(requests.auth.AuthBase):
     """
     See https://stackoverflow.com/a/58055668
     """
 
     def __init__(self, token):
```

### Comparing `openprotein_python-0.1.1b8/openprotein_python/errors.py` & `openprotein_python-0.1.1b9/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b8/openprotein_python/fasta.py` & `openprotein_python-0.1.1b9/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b8/openprotein_python/models.py` & `openprotein_python-0.1.1b9/openprotein/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pydantic models
 from typing import Optional, List, Union, Dict, Literal
 from datetime import datetime
 from enum import Enum
 import numpy as np
 from pydantic import BaseModel, Field, validator
-from openprotein_python.api.jobs import Job, JobStatus
+from openprotein.api.jobs import Job, JobStatus
 
 class ModelDescription(BaseModel):
     citation_title: Optional[str] = None
     doi: Optional[str] = None
     summary: str
 
 class TokenInfo(BaseModel):
```

### Comparing `openprotein_python-0.1.1b8/PKG-INFO` & `openprotein_python-0.1.1b9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.1.1b8
+Version: 0.1.1b9
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,29 +18,32 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas (>=1)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: requests (>=2)
 Requires-Dist: tqdm (>=4)
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
+[![Coverage](./apidocs/source/coverage.svg)](https://pypi.org/project/openprotein-python/)
+
 # openprotein-python
 Python interface for the OpenProtein.AI REST API.
 
 ## Installation 
 
 You can install with pip: 
 
 ```
 pip install openprotein_python
 ```
 ## Getting started
 
 First, create a session using your login credentials.
 ```
-import openprotein
+import openprotein_python
 session = openprotein.connect(USERNAME, PASSWORD)
 ```
 
 Async calls return `AsyncJobFuture` objects that allow tracking the status of the job and retrieving the result when it's ready.
 
 Given a future, check its status and retrieve results
 ```
```

