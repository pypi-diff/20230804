# Comparing `tmp/payme-pkg-2.3.tar.gz` & `tmp/payme-pkg-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payme-pkg-2.3.tar", last modified: Mon Jul 31 07:04:07 2023, max compression
+gzip compressed data, was "dist/payme-pkg-2.4.tar", last modified: Fri Aug  4 07:33:59 2023, max compression
```

## Comparing `payme-pkg-2.3.tar` & `payme-pkg-2.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.223381 payme-pkg-2.3/
--rw-r--r--   0 thenight   (501) staff       (20)     1062 2023-07-29 22:54:03.000000 payme-pkg-2.3/LICENSE.txt
--rw-r--r--   0 thenight   (501) staff       (20)      338 2023-07-31 07:04:07.223698 payme-pkg-2.3/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)    19766 2023-07-29 22:54:03.000000 payme-pkg-2.3/README.md
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.177690 payme-pkg-2.3/lib/
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.187768 payme-pkg-2.3/lib/payme/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      287 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/admin.py
--rw-r--r--   0 thenight   (501) staff       (20)      264 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/apps.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.189913 payme-pkg-2.3/lib/payme/cards/
--rw-r--r--   0 thenight   (501) staff       (20)       29 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/cards/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     5071 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/cards/subscribe_cards.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.191569 payme-pkg-2.3/lib/payme/decorators/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/decorators/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      908 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/decorators/decorators.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.193338 payme-pkg-2.3/lib/payme/errors/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/errors/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     2241 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/errors/exceptions.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.201867 payme-pkg-2.3/lib/payme/methods/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1847 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/cancel_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)      708 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/check_perform_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1423 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/check_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     2302 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/create_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1954 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/generate_link.py
--rw-r--r--   0 thenight   (501) staff       (20)     2124 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/methods/get_statement.py
--rw-r--r--   0 thenight   (501) staff       (20)     1538 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/perform_transaction.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.204947 payme-pkg-2.3/lib/payme/migrations/
--rw-r--r--   0 thenight   (501) staff       (20)     2061 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/migrations/0001_initial.py
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/migrations/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1974 2023-07-31 07:00:59.000000 payme-pkg-2.3/lib/payme/models.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.207297 payme-pkg-2.3/lib/payme/receipts/
--rw-r--r--   0 thenight   (501) staff       (20)       32 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/receipts/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     6616 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/receipts/subscribe_receipts.py
--rw-r--r--   0 thenight   (501) staff       (20)     2755 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/serializers.py
--rw-r--r--   0 thenight   (501) staff       (20)      139 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/urls.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.217743 payme-pkg-2.3/lib/payme/utils/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      719 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/utils/get_params.py
--rw-r--r--   0 thenight   (501) staff       (20)      186 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/logging.py
--rw-r--r--   0 thenight   (501) staff       (20)      546 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/utils/make_aware_datetime.py
--rw-r--r--   0 thenight   (501) staff       (20)      209 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/support.py
--rw-r--r--   0 thenight   (501) staff       (20)      236 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/to_json.py
--rw-r--r--   0 thenight   (501) staff       (20)     4492 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/views.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.222764 payme-pkg-2.3/lib/payme_pkg.egg-info/
--rw-r--r--   0 thenight   (501) staff       (20)      338 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)     1183 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 thenight   (501) staff       (20)        1 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 thenight   (501) staff       (20)       59 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/requires.txt
--rw-r--r--   0 thenight   (501) staff       (20)        6 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/top_level.txt
--rw-r--r--   0 thenight   (501) staff       (20)      107 2023-07-31 07:04:07.224736 payme-pkg-2.3/setup.cfg
--rw-r--r--   0 thenight   (501) staff       (20)      538 2023-07-31 07:03:48.000000 payme-pkg-2.3/setup.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-08-04 07:33:59.000000 payme-pkg-2.4/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)    19385 2023-07-31 09:49:43.000000 payme-pkg-2.4/README.md
+-rw-r--r--   0 thenight   (501) staff       (20)      538 2023-08-04 07:29:55.000000 payme-pkg-2.4/setup.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)     1183 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 thenight   (501) staff       (20)       59 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/requires.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        6 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/top_level.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        1 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme_pkg.egg-info/dependency_links.txt
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/receipts/
+-rw-r--r--   0 thenight   (501) staff       (20)     6616 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/receipts/subscribe_receipts.py
+-rw-r--r--   0 thenight   (501) staff       (20)       32 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/receipts/__init__.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/migrations/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/migrations/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2060 2023-08-04 06:46:58.000000 payme-pkg-2.4/lib/payme/migrations/0001_initial.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/methods/
+-rw-r--r--   0 thenight   (501) staff       (20)      708 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/check_perform_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1847 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/cancel_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2302 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/create_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1538 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/perform_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1954 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/generate_link.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1423 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/methods/check_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2124 2023-07-31 06:55:26.000000 payme-pkg-2.4/lib/payme/methods/get_statement.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2208 2023-08-04 06:47:53.000000 payme-pkg-2.4/lib/payme/models.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/decorators/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/decorators/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      908 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/decorators/decorators.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/cards/
+-rw-r--r--   0 thenight   (501) staff       (20)     5071 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/cards/subscribe_cards.py
+-rw-r--r--   0 thenight   (501) staff       (20)       29 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/cards/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2755 2023-07-31 06:55:26.000000 payme-pkg-2.4/lib/payme/serializers.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/__init__.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/utils/
+-rw-r--r--   0 thenight   (501) staff       (20)      186 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/utils/logging.py
+-rw-r--r--   0 thenight   (501) staff       (20)      209 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/utils/support.py
+-rw-r--r--   0 thenight   (501) staff       (20)      546 2023-07-31 06:55:26.000000 payme-pkg-2.4/lib/payme/utils/make_aware_datetime.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/utils/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      236 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/utils/to_json.py
+-rw-r--r--   0 thenight   (501) staff       (20)      719 2023-07-31 06:55:26.000000 payme-pkg-2.4/lib/payme/utils/get_params.py
+-rw-r--r--   0 thenight   (501) staff       (20)      264 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/apps.py
+-rw-r--r--   0 thenight   (501) staff       (20)      287 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/admin.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-08-04 07:33:59.000000 payme-pkg-2.4/lib/payme/errors/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/errors/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2241 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/errors/exceptions.py
+-rw-r--r--   0 thenight   (501) staff       (20)      139 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/urls.py
+-rw-r--r--   0 thenight   (501) staff       (20)     4492 2023-07-29 22:54:03.000000 payme-pkg-2.4/lib/payme/views.py
+-rw-r--r--   0 thenight   (501) staff       (20)      107 2023-08-04 07:33:59.000000 payme-pkg-2.4/setup.cfg
+-rw-r--r--   0 thenight   (501) staff       (20)     1062 2023-07-29 22:54:03.000000 payme-pkg-2.4/LICENSE.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `payme-pkg-2.3/LICENSE.txt` & `payme-pkg-2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/README.md` & `payme-pkg-2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 ```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb"
+    paycom_id=$paycom_id
 )
 
 resp = client.cards_create(
     number="8600069195406311",
     expire="0399",
     save=True
 )
@@ -170,15 +170,15 @@
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb"
+    paycom_id=$paycom_id
 )
 
 resp = client.card_get_verify_code(
     token="630e5ffdd15d8d8d093b379b_2fsaoABWafecn20kofV4PFafFZjeGDWS9adM1PmboQaEZbbaxMcnaskctMbU9Iv8qgrOuKGz8SnjvZvYXDK64m1eS9gA5jZ7BBRaQybMXrDPtFPJ1fwek5B1KoIv5cMiCWYXj7ezpYEdJAKTIQw0Np9HsTXjqco4gQG3m8MOfeH9ovkdm66O6yj45oKXRmJyAK5i0SchXNNomACH3Oq80KyoRE1VoBRxvoKyMkOx0xcepXovxK9d3v26a8z7UtyokwY33N8MupviM3A5WHB5Xh35WZJJyFnxTSi1vvnYnG7uVd6Bb1GjV2yAHnimss8aEZGW5V7ZiPrhf8r6WJAeHciYDGK3msRKZJBQTfjgOdE9tGrEnMezVkxr1JXX0xSn5qqec2"
 )
 
 pprint(resp)
@@ -207,15 +207,15 @@
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb"
+    paycom_id=$paycom_id
 )
 
 resp = client.cards_verify(
     verify_code="666666",
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
@@ -250,15 +250,15 @@
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb"
+    paycom_id=$paycom_id
 )
 
 resp = client.cards_check(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
@@ -292,15 +292,15 @@
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb"
+    paycom_id=$paycom_id
 )
 
 resp = client.cards_remove(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
@@ -327,16 +327,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.receipts_create(
     amount=10000,
     order_id="1"
 )
 
@@ -409,16 +409,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.receipts_pay(
     invoice_id="631186b6c4420cbf2712a243",
     token="63118a5dd15d8d8d093b37b7_X2j34OIJPnROfsgzYZCZ0w7OcC50zzwiowTsotEVO1uUbxkzaDrvdOno6jicQTrcRmxvibxrye4vUS3AynTNPaPCTGpfk3RCKmT9NaOAyyTmctAjWsjwvqGR5XUzAP1Xcx12GkhuQi6VJ4BeaIXOokSRu06rRjaivmJQ8HTiJiR9b3OmZtrhkIRNcNXnnp9zYm1mFP4BuqGpS8BMnY0ASIE6ffxWykjgBcDTAfWBFt4mg7O9Dsvx0aj3IB8z3RIbZYtDZJnUVhCZrwW7ONVI9uEAdxNthorjO6PbV7TQ8XCjrztgGf6uCtOwwxasiIUVZN6tCVDk8A8NvVSUzUHXQHVkaPn5heJNa3K4WsffIckq7SwMbiw3UbawipeZKyD3iwk1Km",
     phone="998901304527"
 )
@@ -496,16 +496,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.receipts_send(
     invoice_id="631186b6c4420cbf2712a243",
     phone="998901304527"
 )
 
@@ -534,16 +534,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.receipts_cancel(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
@@ -620,16 +620,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.receipts_check(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
@@ -657,16 +657,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.reciepts_get(
     invoice_id="6311946bc4420cbf2712a247"
 )
 
 pprint(resp)
@@ -739,16 +739,16 @@
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
-    paycom_id="5e730e8e0b852a417aa49ceb",
-    paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
+    paycom_id=$paycom_id,
+    paycom_key=$paycom_key
 )
 
 resp = rclient.reciepts_get_all(
     count=2,
     _from=1636398000000,
     to=1636398000000,
     offset=0
```

### Comparing `payme-pkg-2.3/lib/payme/cards/subscribe_cards.py` & `payme-pkg-2.4/lib/payme/cards/subscribe_cards.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/decorators/decorators.py` & `payme-pkg-2.4/lib/payme/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/errors/exceptions.py` & `payme-pkg-2.4/lib/payme/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/cancel_transaction.py` & `payme-pkg-2.4/lib/payme/methods/cancel_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/check_perform_transaction.py` & `payme-pkg-2.4/lib/payme/methods/check_perform_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/check_transaction.py` & `payme-pkg-2.4/lib/payme/methods/check_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/create_transaction.py` & `payme-pkg-2.4/lib/payme/methods/create_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/generate_link.py` & `payme-pkg-2.4/lib/payme/methods/generate_link.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/get_statement.py` & `payme-pkg-2.4/lib/payme/methods/get_statement.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/methods/perform_transaction.py` & `payme-pkg-2.4/lib/payme/methods/perform_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/migrations/0001_initial.py` & `payme-pkg-2.4/lib/payme/migrations/0001_initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # pylint: disable=invalid-name
-from django.db import models
-from django.db import migrations
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    """
-    Migration class for Django Migrations.
-    """
+    # pylint: disable=missing-class-docstring
     initial = True
-
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
             name='MerchatTransactionsModel',
             fields=[
                 ('id', models.BigAutoField(
                     auto_created=True,
@@ -45,9 +40,10 @@
                     serialize=False,
                     verbose_name='ID')
                  ),
                 ('amount', models.IntegerField(blank=True, null=True)),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
             ],
+            options={'managed': False}
         ),
     ]
```

### Comparing `payme-pkg-2.3/lib/payme/models.py` & `payme-pkg-2.4/lib/payme/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.db import models
 from django.conf import settings
 from django.utils.module_loading import import_string
+from django.core.exceptions import FieldError
 
 from payme.utils.logging import logger
 
 
 class MerchatTransactionsModel(models.Model):
     """
     MerchatTransactionsModel class \
@@ -25,23 +26,28 @@
 
     def __str__(self):
         return str(self._id)
 
 
 try:
     CUSTOM_ORDER = import_string(settings.ORDER_MODEL)
-    if 'amount' in CUSTOM_ORDER.__doc__:
-        Order = CUSTOM_ORDER
-    else:
-        raise ImportError("amount field is not defined in your custom order model")
 
+    if not isinstance(CUSTOM_ORDER, models.base.ModelBase):
+        raise TypeError("The input must be an instance of models.Model class")
+
+    # pylint: disable=protected-access
+    if 'amount' not in [f.name for f in CUSTOM_ORDER._meta.fields]:
+        raise FieldError("Missing 'amount' field in your custom order model")
+
+    Order = CUSTOM_ORDER
 except (ImportError, AttributeError):
-    CUSTOM_ORDER = None
     logger.warning("You have no payme custom order model")
 
+    CUSTOM_ORDER = None
+
     class Order(models.Model):
         """
         Order class \
             That's used for managing order process
         """
         amount = models.IntegerField(null=True, blank=True)
         created_at = models.DateTimeField(auto_now_add=True)
```

### Comparing `payme-pkg-2.3/lib/payme/receipts/subscribe_receipts.py` & `payme-pkg-2.4/lib/payme/receipts/subscribe_receipts.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/serializers.py` & `payme-pkg-2.4/lib/payme/serializers.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/utils/get_params.py` & `payme-pkg-2.4/lib/payme/utils/get_params.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/utils/make_aware_datetime.py` & `payme-pkg-2.4/lib/payme/utils/make_aware_datetime.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme/views.py` & `payme-pkg-2.4/lib/payme/views.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/lib/payme_pkg.egg-info/SOURCES.txt` & `payme-pkg-2.4/lib/payme_pkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.3/setup.py` & `payme-pkg-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='payme-pkg',
-    version='2.3',
+    version='2.4',
     license='MIT',
     author="Muhammadali Akbarov",
     author_email='muhammadali17abc@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     url='https://github.com/Muhammadali-Akbarov/payme-pkg',
     keywords='paymeuz paycomuz payme-merchant merchant-api subscribe-api payme-pkg payme-api',
```

