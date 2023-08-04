# Comparing `tmp/nonebot_plugin_mystool-1.2.0.tar.gz` & `tmp/nonebot_plugin_mystool-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-1.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-1.2.0b1.tar", max compression
```

## Comparing `nonebot_plugin_mystool-1.2.0.tar` & `nonebot_plugin_mystool-1.2.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/LICENSE
--rw-r--r--   0        0        0     4964 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/README.md
--rw-r--r--   0        0        0     1443 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2139 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     4180 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    14918 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/data_model.py
--rw-r--r--   0        0        0    22933 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    11963 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/game_sign_api.py
--rw-r--r--   0        0        0     5463 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/good_image.py
--rw-r--r--   0        0        0     2154 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    10934 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    21935 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/myb_missions_api.py
--rw-r--r--   0        0        0    27107 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0    15046 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/plugin_data.py
--rw-r--r--   0        0        0    11801 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    70833 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/simple_api.py
--rw-r--r--   0        0        0    11057 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/user_check.py
--rw-r--r--   0        0        0    12948 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/user_data.py
--rw-r--r--   0        0        0    14370 2023-08-04 10:13:47.764027 nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     6492 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/LICENSE
+-rw-r--r--   0        0        0     4630 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/README.md
+-rw-r--r--   0        0        0     1382 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2139 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     4168 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    14918 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/data_model.py
+-rw-r--r--   0        0        0    22981 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    11963 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/game_sign_api.py
+-rw-r--r--   0        0        0     5463 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/good_image.py
+-rw-r--r--   0        0        0     2154 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    10355 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    21935 2023-07-27 19:15:44.169772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/myb_missions_api.py
+-rw-r--r--   0        0        0    25577 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0    15022 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plugin_data.py
+-rw-r--r--   0        0        0    11698 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    70833 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/simple_api.py
+-rw-r--r--   0        0        0    10022 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_check.py
+-rw-r--r--   0        0        0    12863 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_data.py
+-rw-r--r--   0        0        0    14402 2023-07-27 19:15:44.173772 nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     6101 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.2.0b1/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-1.2.0/LICENSE` & `nonebot_plugin_mystool-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/README.md` & `nonebot_plugin_mystool-1.2.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -48,264 +48,243 @@
 000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
 00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
 00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
 00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
 00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
 00000340: b60a 0a23 2320 f09f 93a3 20e6 9bb4 e696  ...## .... .....
 00000350: b0e5 8685 e5ae b90a 2323 2320 3230 3233  ........### 2023
-00000360: 2e38 2e34 202d 2076 312e 322e 300a 2d20  .8.4 - v1.2.0.- 
-00000370: e4bf aee5 a48d e58e 9fe7 a59e e7ad bee5  ................
-00000380: 88b0 e8bf 94e5 9b9e 4453 e697 a0e6 9588  ........DS......
-00000390: e79a 84e9 97ae e9a2 9820 2331 3530 2023  ......... #150 #
-000003a0: 3133 340a 2d20 e4bf aee5 a48d e5b4 a9e5  134.- ..........
-000003b0: 9d8f e4b8 89e7 adbe e588 b0e8 bf94 e59b  ................
-000003c0: 9e20 e280 9ce7 adbe e588 b0e5 8a9f e883  . ..............
-000003d0: bde7 bbb4 e68a a4e4 b8ad efbc 8ce8 afb7  ................
-000003e0: e880 90e5 bf83 e7ad 89e5 be85 e280 9d20  ............... 
-000003f0: e79a 84e9 97ae e9a2 9820 2331 3339 2023  ......... #139 #
-00000400: 3133 3120 2331 3330 0a2d 20e4 bfae e5a4  131 #130.- .....
-00000410: 8de4 bdbf e794 a851 51e9 a291 e981 93e9  .......QQ.......
-00000420: 8082 e985 8de5 99a8 e79a 84e6 8385 e586  ................
-00000430: b5e4 b88b e58f afe8 83bd e59b a0e4 b8ba  ................
-00000440: e58f 91e9 8081 e6b6 88e6 81af e5a4 b1e8  ................
-00000450: b4a5 e880 8ce6 97a0 e6b3 95e7 bba7 e7bb  ................
-00000460: ade7 9a84 e997 aee9 a298 200a 2d20 e58f  .......... .- ..
-00000470: 96e6 b688 e4ba 86e8 87aa e58a a8e5 88a0  ................
-00000480: e999 a4e9 9d9e e5a5 bde5 8f8b e79a 84e7  ................
-00000490: 94a8 e688 b7e6 95b0 e68d aee7 9a84 e58a  ................
-000004a0: 9fe8 83bd 0a0a 2323 2320 3230 3233 2e37  ......### 2023.7
-000004b0: 2e32 3820 2d20 7631 2e32 2e30 2d62 6574  .28 - v1.2.0-bet
-000004c0: 612e 310a 2d20 e5a2 9ee5 8aa0 e5af b951  a.1.- .........Q
-000004d0: 51e9 a291 e981 93e7 9a84 e694 afe6 8c81  Q...............
-000004e0: 2023 3132 380a 2020 3e20 e8af b4e6 988e   #128.  > ......
-000004f0: e696 87e6 a1a3 efbc 9a5b f09f 9497 5151  .........[....QQ
-00000500: 4775 696c 6420 e980 82e9 858d e599 a85d  Guild .........]
-00000510: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000520: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-00000530: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000540: 6f6f 6c2f 7769 6b69 2f49 6e73 7461 6c6c  ool/wiki/Install
-00000550: 6174 696f 6e23 5151 4775 696c 642d e980  ation#QQGuild-..
-00000560: 82e9 858d e599 a829 0a2d 20e5 a29e e58a  .......).- .....
-00000570: a0e7 94a8 e688 b7e6 95b0 e68d aee7 bb91  ................
-00000580: e5ae 9ae5 85b3 e881 94e5 8a9f e883 bdef  ................
-00000590: bc88 e5a6 8251 51e9 a291 e981 93e8 b4a6  .....QQ.........
-000005a0: e58f b7e4 b88e 5151 e881 8ae5 a4a9 e8b4  ......QQ........
-000005b0: a6e5 8fb7 e79a 84e6 95b0 e68d aee7 bb91  ................
-000005c0: e5ae 9aef bc89 0a20 203e 20e8 afb4 e698  .......  > .....
-000005d0: 8ee6 9687 e6a1 a3ef bc9a 5bf0 9f94 97e7  ..........[.....
-000005e0: 94a8 e688 b7e6 95b0 e68d aee7 bb91 e5ae  ................
-000005f0: 9ae5 85b3 e881 945d 2868 7474 7073 3a2f  .......](https:/
-00000600: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-00000610: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-00000620: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
-00000630: 2f49 6e66 6f72 6d61 7469 6f6e 2d55 7365  /Information-Use
-00000640: 7242 696e 6429 0a2d 20e5 a29e e58a a0e5  rBind).- .......
-00000650: 8e9f e7a5 9ee4 bebf e7ac bae6 a091 e884  ................
-00000660: 82e6 8f90 e986 92e9 9888 e580 bce7 9a84  ................
-00000670: e8ae bee7 bdae e980 89e9 a1b9 2023 3135  ............ #15
-00000680: 3120 6279 2040 4a6f 7365 616e 646c 7575  1 by @Joseandluu
-00000690: 650a 2020 3e20 e8af b4e6 988e e696 87e6  e.  > ..........
-000006a0: a1a3 efbc 9a5b f09f 9497 e5af b9e7 bb91  .....[..........
-000006b0: e5ae 9ae7 9a84 e69f 90e4 b8aa e7b1 b3e5  ................
-000006c0: 9388 e6b8 b8e8 b4a6 e688 b7e8 bf9b e8a1  ................
-000006d0: 8ce8 aebe e7bd ae5d 2868 7474 7073 3a2f  .......](https:/
-000006e0: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-000006f0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-00000700: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
-00000710: 2f49 6e66 6f72 6d61 7469 6f6e 2d53 6574  /Information-Set
-00000720: 7469 6e67 2325 4535 2541 4625 4239 2545  ting#%E5%AF%B9%E
-00000730: 3725 4242 2539 3125 4535 2541 4525 3941  7%BB%91%E5%AE%9A
-00000740: 2545 3725 3941 2538 3425 4536 2539 4625  %E7%9A%84%E6%9F%
-00000750: 3930 2545 3425 4238 2541 4125 4537 2542  90%E4%B8%AA%E7%B
-00000760: 3125 4233 2545 3525 3933 2538 3825 4536  1%B3%E5%93%88%E6
-00000770: 2542 3825 4238 2545 3825 4234 2541 3625  %B8%B8%E8%B4%A6%
-00000780: 4536 2538 3825 4237 2545 3825 4246 2539  E6%88%B7%E8%BF%9
-00000790: 4225 4538 2541 3125 3843 2545 3825 4145  B%E8%A1%8C%E8%AE
-000007a0: 2542 4525 4537 2542 4425 4145 290a 2d20  %BE%E7%BD%AE).- 
-000007b0: e4bf aee5 a48d 2060 7072 6566 6572 656e  ...... `preferen
-000007c0: 6365 2e6f 7665 7272 6964 655f 6465 7669  ce.override_devi
-000007d0: 6365 5f61 6e64 5f73 616c 7460 20e5 85b3  ce_and_salt` ...
-000007e0: e997 ade6 97a0 e695 88e7 9a84 e997 aee9  ................
-000007f0: a298 0a0a 2323 2320 3230 3233 2e37 2e32  ....### 2023.7.2
-00000800: 3320 2d20 7631 2e31 2e30 0a2d 20e5 a29e  3 - v1.1.0.- ...
-00000810: e58a a0e5 b4a9 e59d 8fef bc9a e698 9fe7  ................
-00000820: a9b9 e993 81e9 8193 e79a 84e4 bebf e7ac  ................
-00000830: bae5 8a9f e883 bd20 2331 3430 2023 3134  ....... #140 #14
-00000840: 3320 6279 2040 4a6f 7365 616e 646c 7575  3 by @Joseandluu
-00000850: 6520 4052 656d 6944 7265 0a20 2020 203e  e @RemiDre.    >
-00000860: 20e8 afb4 e698 8ee6 9687 e6a1 a3ef bc9a   ...............
-00000870: 5bf0 9f94 97e6 989f e7a9 b9e9 9381 e981  [...............
-00000880: 93e5 ae9e e697 b6e4 bebf e7ac ba5d 2868  .............](h
-00000890: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000008a0: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-000008b0: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-000008c0: 6c2f 7769 6b69 2f49 6e66 6f72 6d61 7469  l/wiki/Informati
-000008d0: 6f6e 2d53 7461 7252 6169 6c53 7461 7475  on-StarRailStatu
-000008e0: 7329 0a2d 20e4 bfae e5a4 8de6 af8f e5b0  s).- ...........
-000008f0: 8fe6 97b6 e983 bde5 8f91 e980 81e4 bebf  ................
-00000900: e7ac bae9 809a e79f a5e7 9a84 4275 6720  ............Bug 
-00000910: 2331 3335 0a2d 20e4 baba e69c bae9 aa8c  #135.- .........
-00000920: e8af 81e6 8993 e7a0 81e5 b9b3 e58f b0e6  ................
-00000930: 94af e68c 81e8 87aa e5ae 9ae4 b989 4a53  ..............JS
-00000940: 4f4e e586 85e5 aeb9 2023 3133 330a 2020  ON...... #133.  
-00000950: 2020 3e20 e8af b4e6 988e e696 87e6 a1a3    > ............
-00000960: efbc 9a5b f09f 9497 6765 6574 6573 745f  ...[....geetest_
-00000970: 6a73 6f6e 5d28 6874 7470 733a 2f2f 6769  json](https://gi
-00000980: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
-00000990: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
-000009a0: 2d6d 7973 746f 6f6c 2f77 696b 692f 436f  -mystool/wiki/Co
-000009b0: 6e66 6967 7572 6174 696f 6e2d 5072 6566  nfiguration-Pref
-000009c0: 6572 656e 6365 2367 6565 7465 7374 5f6a  erence#geetest_j
-000009d0: 736f 6e29 0a2d 20e4 bfae e5a4 8de5 9586  son).- .........
-000009e0: e593 81e5 8591 e68d a241 5049 2023 3131  .........API #11
-000009f0: 300a 2d20 e4b8 8de5 9ca8 e5a5 bde5 8f8b  0.- ............
-00000a00: e588 97e8 a1a8 e79a 84e7 94a8 e688 b7e6  ................
-00000a10: 95b0 e68d aee5 9ca8 e588 a0e9 99a4 e589  ................
-00000a20: 8de5 b086 e8bf 9be8 a18c e5a4 87e4 bbbd  ................
-00000a30: 2023 3132 390a 2020 2020 3e20 e5a4 87e4   #129.    > ....
-00000a40: bbbd e79b aee5 bd95 efbc 9a60 6461 7461  ...........`data
-00000a50: 2f6e 6f6e 6562 6f74 5f70 6c75 6769 6e5f  /nonebot_plugin_
-00000a60: 6d79 7374 6f6f 6c2f 6465 6c65 7465 6455  mystool/deletedU
-00000a70: 7365 7273 600a 2d20 e998 b2e6 ada2 e59b  sers`.- ........
-00000a80: a0e6 8f92 e4bb b6e6 95b0 e68d aee6 9687  ................
-00000a90: e4bb b6e4 b8ad e9bb 98e8 aea4 e5ad 98e5  ................
-00000aa0: 9ca8 2060 6465 7669 6365 5f63 6f6e 6669  .. `device_confi
-00000ab0: 6760 2c20 6073 616c 745f 636f 6e66 6967  g`, `salt_config
-00000ac0: 6020 e880 8ce5 afbc e887 b4e6 9bb4 e696  ` ..............
-00000ad0: b0e5 908e e9bb 98e8 aea4 e985 8de7 bdae  ................
-00000ae0: e8a2 abe5 8e9f e985 8de7 bdae e8a6 86e7  ................
-00000af0: 9b96 e79a 84e9 97ae e9a2 980a 2d20 e88b  ............- ..
-00000b00: a5e9 9c80 e8a6 81e4 bfae e694 b920 6064  ............. `d
-00000b10: 6576 6963 655f 636f 6e66 6967 6020 e985  evice_config` ..
-00000b20: 8de7 bdae efbc 8ce4 bfae e694 b9e5 908e  ................
-00000b30: e8bf 98e8 aebe e7bd aee6 8f92 e4bb b6e6  ................
-00000b40: 95b0 e68d aee6 9687 e4bb b6e4 b8ad 2060  .............. `
-00000b50: 7072 6566 6572 656e 6365 2e6f 7665 7272  preference.overr
-00000b60: 6964 655f 6465 7669 6365 5f61 6e64 5f73  ide_device_and_s
-00000b70: 616c 7460 20e4 b8ba 2074 7275 6520 e4bb  alt` ... true ..
-00000b80: a5e8 a686 e79b 96e9 bb98 e8ae a4e5 80bc  ................
-00000b90: 0a20 2020 203e 20e8 afb4 e698 8ee6 9687  .    > .........
-00000ba0: e6a1 a3ef bc9a 0a20 2020 203e 202d 205b  .......    > - [
-00000bb0: f09f 9497 e7bd 91e7 bb9c e8af b7e6 b182  ................
-00000bc0: e8ae bee5 a487 e4bf a1e6 81af 2060 636c  ............ `cl
-00000bd0: 6173 7320 4465 7669 6365 436f 6e66 6967  ass DeviceConfig
-00000be0: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
-00000bf0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000c00: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000c10: 7374 6f6f 6c2f 7769 6b69 2f43 6f6e 6669  stool/wiki/Confi
-00000c20: 6775 7261 7469 6f6e 2d44 6576 6963 6543  guration-DeviceC
-00000c30: 6f6e 6669 6729 0a20 2020 203e 202d 205b  onfig).    > - [
-00000c40: f09f 9497 6f76 6572 7269 6465 5f64 6576  ....override_dev
-00000c50: 6963 655f 616e 645f 7361 6c74 5d28 6874  ice_and_salt](ht
-00000c60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c70: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
-00000c80: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000c90: 2f77 696b 692f 436f 6e66 6967 7572 6174  /wiki/Configurat
-00000ca0: 696f 6e2d 5072 6566 6572 656e 6365 236f  ion-Preference#o
-00000cb0: 7665 7272 6964 655f 6465 7669 6365 5f61  verride_device_a
-00000cc0: 6e64 5f73 616c 7429 0a2d 20e5 a29e e58a  nd_salt).- .....
-00000cd0: a0e4 ba86 e698 afe5 90a6 e4bd bfe7 94a8  ................
-00000ce0: e5a4 9ae8 bf9b e7a8 8be7 949f e688 90e5  ................
-00000cf0: 9586 e593 81e5 9bbe e789 87e7 9a84 e985  ................
-00000d00: 8de7 bdae e9a1 b920 6067 6f6f 645f 6c69  ....... `good_li
-00000d10: 7374 5f69 6d61 6765 5f63 6f6e 6669 6760  st_image_config`
-00000d20: 2e60 4d55 4c54 495f 5052 4f43 4553 5360  .`MULTI_PROCESS`
-00000d30: efbc 8ce5 a682 e69e 9ce9 8187 e588 b0e7  ................
-00000d40: 949f e688 90e5 9bbe e789 87e5 a4b1 e8b4  ................
-00000d50: a5e5 8faf e4bb a5e5 b09d e8af 95e5 85b3  ................
-00000d60: e997 ade8 afa5 e9a1 b90a 2d20 e59c a8e5  ..........- ....
-00000d70: 8591 e68d a2e5 bc80 e5a7 8be5 908e e79a  ................
-00000d80: 84e4 b880 e6ae b5e6 97b6 e997 b4e5 8685  ................
-00000d90: e4b8 8de6 96ad e5b0 9de8 af95 e585 91e6  ................
-00000da0: 8da2 efbc 8ce7 9bb4 e588 b0e6 8890 e58a  ................
-00000db0: 9f20 2331 3130 0a2d 20e5 8591 e68d a2e5  . #110.- .......
-00000dc0: bc80 e5a7 8be5 908e e5b0 86e4 b88d e4bc  ................
-00000dd0: 9ae5 bbb6 e8bf 9fe5 8591 e68d a2ef bc8c  ................
-00000de0: e794 a8e6 88b7 e695 b0e6 8dae e696 87e4  ................
-00000df0: bbb6 e4b8 ad20 6070 7265 6665 7265 6e63  ..... `preferenc
-00000e00: 652e 6578 6368 616e 6765 5f6c 6174 656e  e.exchange_laten
-00000e10: 6379 6020 e5b0 86e4 bd9c e4b8 bae5 908c  cy` ............
-00000e20: e4b8 80e7 babf e7a8 8be4 b88b e6af 8fe4  ................
-00000e30: b8aa e585 91e6 8da2 e8af b7e6 b182 e4b9  ................
-00000e40: 8be9 97b4 e79a 84e6 97b6 e997 b4e9 97b4  ................
-00000e50: e99a 9420 2331 3130 0a2d 20e5 8591 e68d  ... #110.- .....
-00000e60: a2e8 afb7 e6b1 82e6 97a5 e5bf 97e5 8685  ................
-00000e70: e5ae b9e5 a29e e58a a0e4 ba86 e58f 91e9  ................
-00000e80: 8081 e8af b7e6 b182 e697 b6e7 9a84 e697  ................
-00000e90: b6e9 97b4 e688 b30a 0a23 2320 e58a 9fe8  .........## ....
-00000ea0: 83bd e592 8ce7 89b9 e680 a70a 0a2d 20e6  .............- .
-00000eb0: 94af e68c 8151 51e8 818a e5a4 a9e5 928c  .....QQ.........
-00000ec0: 5151 e9a2 91e9 8193 0a2d 20e7 9fad e4bf  QQ.......- .....
-00000ed0: a1e9 aa8c e8af 81e7 99bb e5bd 95ef bc8c  ................
-00000ee0: e585 8de6 8a93 e58c 85e8 8eb7 e58f 9620  ............... 
-00000ef0: 436f 6f6b 6965 0a2d 20e8 87aa e58a a8e5  Cookie.- .......
-00000f00: ae8c e688 90e6 af8f e697 a5e7 b1b3 e6b8  ................
-00000f10: b8e5 b881 e4bb bbe5 8aa1 0a2d 20e8 87aa  ...........- ...
-00000f20: e58a a8e8 bf9b e8a1 8ce6 b8b8 e688 8fe7  ................
-00000f30: adbe e588 b00a 2d20 e58f afe5 88b6 e5ae  ......- ........
-00000f40: 9ae7 b1b3 e6b8 b8e5 b881 e595 86e5 9381  ................
-00000f50: e585 91e6 8da2 e8ae a1e5 8892 efbc 8ce5  ................
-00000f60: 88b0 e782 b9e5 8591 e68d a2ef bc88 e59b  ................
-00000f70: a0e5 8aa0 e585 a5e4 ba86 e4ba bae6 9cba  ................
-00000f80: e9aa 8ce8 af81 efbc 8ce6 8890 e58a 9fe7  ................
-00000f90: 8e87 e8be 83e4 bd8e efbc 890a 2d20 e58f  ............- ..
-00000fa0: afe6 94af e68c 81e5 a49a e4b8 aa20 5151  ............. QQ
-00000fb0: 20e8 b4a6 e58f b7ef bc8c e6af 8fe4 b8aa   ...............
-00000fc0: 2051 5120 e8b4 a6e5 8fb7 e58f afe7 bb91   QQ ............
-00000fd0: e5ae 9ae5 a49a e4b8 aae7 b1b3 e593 88e6  ................
-00000fe0: b8b8 e8b4 a6e6 88b7 0a2d 2051 5120 e68e  .........- QQ ..
-00000ff0: a8e9 8081 e689 a7e8 a18c e7bb 93e6 9e9c  ................
-00001000: e980 9ae7 9fa5 0a2d 20e5 8e9f e7a5 9ee3  .......- .......
-00001010: 8081 e5b4 a9e5 9d8f efbc 9ae6 989f e7a9  ................
-00001020: b9e9 9381 e981 93e7 8ab6 e680 81e4 bebf  ................
-00001030: e7ac bae9 809a e79f a50a 0a23 2320 e4bd  ...........## ..
-00001040: bfe7 94a8 e8af b4e6 988e 0a0a 2323 2320  ............### 
-00001050: f09f 9ba0 efb8 8f20 4e6f 6e65 426f 7432  ....... NoneBot2
-00001060: 20e6 9cba e599 a8e4 baba e983 a8e7 bdb2   ...............
-00001070: e592 8ce6 8f92 e4bb b6e5 ae89 e8a3 850a  ................
-00001080: 0ae8 afb7 e69f a5e7 9c8b 202d 3e20 5bf0  .......... -> [.
-00001090: 9f94 9749 6e73 7461 6c6c 6174 696f 6e5d  ...Installation]
-000010a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000010b0: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-000010c0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-000010d0: 6f6f 6c2f 7769 6b69 2f49 6e73 7461 6c6c  ool/wiki/Install
-000010e0: 6174 696f 6e29 0a0a 2323 2320 f09f 9396  ation)..### ....
-000010f0: 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4 bdbf   ...............
-00001100: e794 a8e8 afb4 e698 8e0a 0ae8 afb7 e69f  ................
-00001110: a5e7 9c8b 202d 3e20 5bf0 9f94 9757 696b  .... -> [....Wik
-00001120: 6920 e696 87e6 a1a3 5d28 6874 7470 733a  i ......](https:
-00001130: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-00001140: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00001150: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-00001160: 6929 0a0a 2323 2320 e29d 9320 e88e b7e5  i)..### ... ....
-00001170: 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9 e4bf  ................
-00001180: a1e6 81af 0a0a 2323 2323 20e6 8f92 e4bb  ......#### .....
-00001190: b6e5 91bd e4bb a40a 0a60 6060 0a2f e5b8  .........```./..
-000011a0: aee5 8aa9 0a60 6060 0a0a 3e20 e29a a0ef  .....```..> ....
-000011b0: b88f 20e6 b3a8 e684 8f20 e6ad a4e5 a484  .. ...... ......
-000011c0: e6b2 a1e6 9c89 e4bd bfe7 94a8 205b f09f  ............ [..
-000011d0: 9497 20e6 8f92 e4bb b6e5 91bd e4bb a4e5  .. .............
-000011e0: a4b4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-000011f0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00001200: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00001210: 7973 746f 6f6c 2f77 696b 692f 436f 6e66  ystool/wiki/Conf
-00001220: 6967 7572 6174 696f 6e2d 436f 6e66 6967  iguration-Config
-00001230: 2363 6f6d 6d61 6e64 7374 6172 7429 0a0a  #commandstart)..
-00001240: 2323 20e5 85b6 e4bb 960a 0a23 2323 205b  ## ........### [
-00001250: f09f 9383 e6ba 90e7 a081 e8af b4e6 988e  ................
-00001260: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001270: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00001280: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00001290: 746f 6f6c 2f77 696b 692f 536f 7572 6365  tool/wiki/Source
-000012a0: 2d53 7472 7563 7475 7265 290a 2323 2320  -Structure).### 
-000012b0: e980 82e9 858d 205b e7bb aae5 b1b1 e79c  ...... [........
-000012c0: 9fe5 afbb 426f 745d 2868 7474 7073 3a2f  ....Bot](https:/
-000012d0: 2f67 6974 6875 622e 636f 6d2f 4869 6269  /github.com/Hibi
-000012e0: 4b69 6572 2f7a 6865 6e78 756e 5f62 6f74  Kier/zhenxun_bot
-000012f0: 2920 e79a 84e5 8886 e694 af0a 2d20 6874  ) ..........- ht
-00001300: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001310: 2f4d 5754 4a43 2f7a 6865 6e78 756e 2d70  /MWTJC/zhenxun-p
-00001320: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a 2d20  lugin-mystool.- 
-00001330: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001340: 6f6d 2f61 7961 6b61 7375 6b69 2f6e 6f6e  om/ayakasuki/non
-00001350: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00001360: 6f6f 6c0a                                ool.
+00000360: 2e37 2e32 3820 2d20 7631 2e32 2e30 2d62  .7.28 - v1.2.0-b
+00000370: 6574 612e 310a 2d20 e5a2 9ee5 8aa0 e5af  eta.1.- ........
+00000380: b951 51e9 a291 e981 93e7 9a84 e694 afe6  .QQ.............
+00000390: 8c81 2023 3132 380a 2020 3e20 e8af b4e6  .. #128.  > ....
+000003a0: 988e e696 87e6 a1a3 efbc 9a5b f09f 9497  ...........[....
+000003b0: 5151 4775 696c 6420 e980 82e9 858d e599  QQGuild ........
+000003c0: a85d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+000003d0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000003e0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+000003f0: 7374 6f6f 6c2f 7769 6b69 2f49 6e73 7461  stool/wiki/Insta
+00000400: 6c6c 6174 696f 6e23 5151 4775 696c 642d  llation#QQGuild-
+00000410: e980 82e9 858d e599 a829 0a2d 20e5 a29e  .........).- ...
+00000420: e58a a0e7 94a8 e688 b7e6 95b0 e68d aee7  ................
+00000430: bb91 e5ae 9ae5 85b3 e881 94e5 8a9f e883  ................
+00000440: bdef bc88 e5a6 8251 51e9 a291 e981 93e8  .......QQ.......
+00000450: b4a6 e58f b7e4 b88e 5151 e881 8ae5 a4a9  ........QQ......
+00000460: e8b4 a6e5 8fb7 e79a 84e6 95b0 e68d aee7  ................
+00000470: bb91 e5ae 9aef bc89 0a20 203e 20e8 afb4  .........  > ...
+00000480: e698 8ee6 9687 e6a1 a3ef bc9a 5bf0 9f94  ............[...
+00000490: 97e7 94a8 e688 b7e6 95b0 e68d aee7 bb91  ................
+000004a0: e5ae 9ae5 85b3 e881 945d 2868 7474 7073  .........](https
+000004b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+000004c0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+000004d0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+000004e0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d55  ki/Information-U
+000004f0: 7365 7242 696e 6429 0a2d 20e5 a29e e58a  serBind).- .....
+00000500: a0e5 8e9f e7a5 9ee4 bebf e7ac bae6 a091  ................
+00000510: e884 82e6 8f90 e986 92e9 9888 e580 bce7  ................
+00000520: 9a84 e8ae bee7 bdae e980 89e9 a1b9 2023  .............. #
+00000530: 3135 3120 6279 2040 4a6f 7365 616e 646c  151 by @Joseandl
+00000540: 7575 650a 2020 3e20 e8af b4e6 988e e696  uue.  > ........
+00000550: 87e6 a1a3 efbc 9a5b f09f 9497 e5af b9e7  .......[........
+00000560: bb91 e5ae 9ae7 9a84 e69f 90e4 b8aa e7b1  ................
+00000570: b3e5 9388 e6b8 b8e8 b4a6 e688 b7e8 bf9b  ................
+00000580: e8a1 8ce8 aebe e7bd ae5d 2868 7474 7073  .........](https
+00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
+000005a0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
+000005b0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
+000005c0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d53  ki/Information-S
+000005d0: 6574 7469 6e67 2325 4535 2541 4625 4239  etting#%E5%AF%B9
+000005e0: 2545 3725 4242 2539 3125 4535 2541 4525  %E7%BB%91%E5%AE%
+000005f0: 3941 2545 3725 3941 2538 3425 4536 2539  9A%E7%9A%84%E6%9
+00000600: 4625 3930 2545 3425 4238 2541 4125 4537  F%90%E4%B8%AA%E7
+00000610: 2542 3125 4233 2545 3525 3933 2538 3825  %B1%B3%E5%93%88%
+00000620: 4536 2542 3825 4238 2545 3825 4234 2541  E6%B8%B8%E8%B4%A
+00000630: 3625 4536 2538 3825 4237 2545 3825 4246  6%E6%88%B7%E8%BF
+00000640: 2539 4225 4538 2541 3125 3843 2545 3825  %9B%E8%A1%8C%E8%
+00000650: 4145 2542 4525 4537 2542 4425 4145 290a  AE%BE%E7%BD%AE).
+00000660: 2d20 e4bf aee5 a48d 2060 7072 6566 6572  - ...... `prefer
+00000670: 656e 6365 2e6f 7665 7272 6964 655f 6465  ence.override_de
+00000680: 7669 6365 5f61 6e64 5f73 616c 7460 20e5  vice_and_salt` .
+00000690: 85b3 e997 ade6 97a0 e695 88e7 9a84 e997  ................
+000006a0: aee9 a298 0a0a 2323 2320 3230 3233 2e37  ......### 2023.7
+000006b0: 2e32 3320 2d20 7631 2e31 2e30 0a2d 20e5  .23 - v1.1.0.- .
+000006c0: a29e e58a a0e5 b4a9 e59d 8fef bc9a e698  ................
+000006d0: 9fe7 a9b9 e993 81e9 8193 e79a 84e4 bebf  ................
+000006e0: e7ac bae5 8a9f e883 bd20 2331 3430 2023  ......... #140 #
+000006f0: 3134 3320 6279 2040 4a6f 7365 616e 646c  143 by @Joseandl
+00000700: 7575 6520 4052 656d 6944 7265 0a20 2020  uue @RemiDre.   
+00000710: 203e 20e8 afb4 e698 8ee6 9687 e6a1 a3ef   > .............
+00000720: bc9a 5bf0 9f94 97e6 989f e7a9 b9e9 9381  ..[.............
+00000730: e981 93e5 ae9e e697 b6e4 bebf e7ac ba5d  ...............]
+00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000750: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000760: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000770: 6f6f 6c2f 7769 6b69 2f49 6e66 6f72 6d61  ool/wiki/Informa
+00000780: 7469 6f6e 2d53 7461 7252 6169 6c53 7461  tion-StarRailSta
+00000790: 7475 7329 0a2d 20e4 bfae e5a4 8de6 af8f  tus).- .........
+000007a0: e5b0 8fe6 97b6 e983 bde5 8f91 e980 81e4  ................
+000007b0: bebf e7ac bae9 809a e79f a5e7 9a84 4275  ..............Bu
+000007c0: 6720 2331 3335 0a2d 20e4 baba e69c bae9  g #135.- .......
+000007d0: aa8c e8af 81e6 8993 e7a0 81e5 b9b3 e58f  ................
+000007e0: b0e6 94af e68c 81e8 87aa e5ae 9ae4 b989  ................
+000007f0: 4a53 4f4e e586 85e5 aeb9 2023 3133 330a  JSON...... #133.
+00000800: 2020 2020 3e20 e8af b4e6 988e e696 87e6      > ..........
+00000810: a1a3 efbc 9a5b f09f 9497 6765 6574 6573  .....[....geetes
+00000820: 745f 6a73 6f6e 5d28 6874 7470 733a 2f2f  t_json](https://
+00000830: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000840: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000850: 696e 2d6d 7973 746f 6f6c 2f77 696b 692f  in-mystool/wiki/
+00000860: 436f 6e66 6967 7572 6174 696f 6e2d 5072  Configuration-Pr
+00000870: 6566 6572 656e 6365 2367 6565 7465 7374  eference#geetest
+00000880: 5f6a 736f 6e29 0a2d 20e4 bfae e5a4 8de5  _json).- .......
+00000890: 9586 e593 81e5 8591 e68d a241 5049 2023  ...........API #
+000008a0: 3131 300a 2d20 e4b8 8de5 9ca8 e5a5 bde5  110.- ..........
+000008b0: 8f8b e588 97e8 a1a8 e79a 84e7 94a8 e688  ................
+000008c0: b7e6 95b0 e68d aee5 9ca8 e588 a0e9 99a4  ................
+000008d0: e589 8de5 b086 e8bf 9be8 a18c e5a4 87e4  ................
+000008e0: bbbd 2023 3132 390a 2020 2020 3e20 e5a4  .. #129.    > ..
+000008f0: 87e4 bbbd e79b aee5 bd95 efbc 9a60 6461  .............`da
+00000900: 7461 2f6e 6f6e 6562 6f74 5f70 6c75 6769  ta/nonebot_plugi
+00000910: 6e5f 6d79 7374 6f6f 6c2f 6465 6c65 7465  n_mystool/delete
+00000920: 6455 7365 7273 600a 2d20 e998 b2e6 ada2  dUsers`.- ......
+00000930: e59b a0e6 8f92 e4bb b6e6 95b0 e68d aee6  ................
+00000940: 9687 e4bb b6e4 b8ad e9bb 98e8 aea4 e5ad  ................
+00000950: 98e5 9ca8 2060 6465 7669 6365 5f63 6f6e  .... `device_con
+00000960: 6669 6760 2c20 6073 616c 745f 636f 6e66  fig`, `salt_conf
+00000970: 6967 6020 e880 8ce5 afbc e887 b4e6 9bb4  ig` ............
+00000980: e696 b0e5 908e e9bb 98e8 aea4 e985 8de7  ................
+00000990: bdae e8a2 abe5 8e9f e985 8de7 bdae e8a6  ................
+000009a0: 86e7 9b96 e79a 84e9 97ae e9a2 980a 2d20  ..............- 
+000009b0: e88b a5e9 9c80 e8a6 81e4 bfae e694 b920  ............... 
+000009c0: 6064 6576 6963 655f 636f 6e66 6967 6020  `device_config` 
+000009d0: e985 8de7 bdae efbc 8ce4 bfae e694 b9e5  ................
+000009e0: 908e e8bf 98e8 aebe e7bd aee6 8f92 e4bb  ................
+000009f0: b6e6 95b0 e68d aee6 9687 e4bb b6e4 b8ad  ................
+00000a00: 2060 7072 6566 6572 656e 6365 2e6f 7665   `preference.ove
+00000a10: 7272 6964 655f 6465 7669 6365 5f61 6e64  rride_device_and
+00000a20: 5f73 616c 7460 20e4 b8ba 2074 7275 6520  _salt` ... true 
+00000a30: e4bb a5e8 a686 e79b 96e9 bb98 e8ae a4e5  ................
+00000a40: 80bc 0a20 2020 203e 20e8 afb4 e698 8ee6  ...    > .......
+00000a50: 9687 e6a1 a3ef bc9a 0a20 2020 203e 202d  .........    > -
+00000a60: 205b f09f 9497 e7bd 91e7 bb9c e8af b7e6   [..............
+00000a70: b182 e8ae bee5 a487 e4bf a1e6 81af 2060  .............. `
+00000a80: 636c 6173 7320 4465 7669 6365 436f 6e66  class DeviceConf
+00000a90: 6967 605d 2868 7474 7073 3a2f 2f67 6974  ig`](https://git
+00000aa0: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
+00000ab0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000ac0: 6d79 7374 6f6f 6c2f 7769 6b69 2f43 6f6e  mystool/wiki/Con
+00000ad0: 6669 6775 7261 7469 6f6e 2d44 6576 6963  figuration-Devic
+00000ae0: 6543 6f6e 6669 6729 0a20 2020 203e 202d  eConfig).    > -
+00000af0: 205b f09f 9497 6f76 6572 7269 6465 5f64   [....override_d
+00000b00: 6576 6963 655f 616e 645f 7361 6c74 5d28  evice_and_salt](
+00000b10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b20: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000b30: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000b40: 6f6c 2f77 696b 692f 436f 6e66 6967 7572  ol/wiki/Configur
+00000b50: 6174 696f 6e2d 5072 6566 6572 656e 6365  ation-Preference
+00000b60: 236f 7665 7272 6964 655f 6465 7669 6365  #override_device
+00000b70: 5f61 6e64 5f73 616c 7429 0a2d 20e5 a29e  _and_salt).- ...
+00000b80: e58a a0e4 ba86 e698 afe5 90a6 e4bd bfe7  ................
+00000b90: 94a8 e5a4 9ae8 bf9b e7a8 8be7 949f e688  ................
+00000ba0: 90e5 9586 e593 81e5 9bbe e789 87e7 9a84  ................
+00000bb0: e985 8de7 bdae e9a1 b920 6067 6f6f 645f  ......... `good_
+00000bc0: 6c69 7374 5f69 6d61 6765 5f63 6f6e 6669  list_image_confi
+00000bd0: 6760 2e60 4d55 4c54 495f 5052 4f43 4553  g`.`MULTI_PROCES
+00000be0: 5360 efbc 8ce5 a682 e69e 9ce9 8187 e588  S`..............
+00000bf0: b0e7 949f e688 90e5 9bbe e789 87e5 a4b1  ................
+00000c00: e8b4 a5e5 8faf e4bb a5e5 b09d e8af 95e5  ................
+00000c10: 85b3 e997 ade8 afa5 e9a1 b90a 2d20 e59c  ............- ..
+00000c20: a8e5 8591 e68d a2e5 bc80 e5a7 8be5 908e  ................
+00000c30: e79a 84e4 b880 e6ae b5e6 97b6 e997 b4e5  ................
+00000c40: 8685 e4b8 8de6 96ad e5b0 9de8 af95 e585  ................
+00000c50: 91e6 8da2 efbc 8ce7 9bb4 e588 b0e6 8890  ................
+00000c60: e58a 9f20 2331 3130 0a2d 20e5 8591 e68d  ... #110.- .....
+00000c70: a2e5 bc80 e5a7 8be5 908e e5b0 86e4 b88d  ................
+00000c80: e4bc 9ae5 bbb6 e8bf 9fe5 8591 e68d a2ef  ................
+00000c90: bc8c e794 a8e6 88b7 e695 b0e6 8dae e696  ................
+00000ca0: 87e4 bbb6 e4b8 ad20 6070 7265 6665 7265  ....... `prefere
+00000cb0: 6e63 652e 6578 6368 616e 6765 5f6c 6174  nce.exchange_lat
+00000cc0: 656e 6379 6020 e5b0 86e4 bd9c e4b8 bae5  ency` ..........
+00000cd0: 908c e4b8 80e7 babf e7a8 8be4 b88b e6af  ................
+00000ce0: 8fe4 b8aa e585 91e6 8da2 e8af b7e6 b182  ................
+00000cf0: e4b9 8be9 97b4 e79a 84e6 97b6 e997 b4e9  ................
+00000d00: 97b4 e99a 9420 2331 3130 0a2d 20e5 8591  ..... #110.- ...
+00000d10: e68d a2e8 afb7 e6b1 82e6 97a5 e5bf 97e5  ................
+00000d20: 8685 e5ae b9e5 a29e e58a a0e4 ba86 e58f  ................
+00000d30: 91e9 8081 e8af b7e6 b182 e697 b6e7 9a84  ................
+00000d40: e697 b6e9 97b4 e688 b30a 0a23 2320 e58a  ...........## ..
+00000d50: 9fe8 83bd e592 8ce7 89b9 e680 a70a 0a2d  ...............-
+00000d60: 20e6 94af e68c 8151 51e8 818a e5a4 a9e5   ......QQ.......
+00000d70: 928c 5151 e9a2 91e9 8193 0a2d 20e7 9fad  ..QQ.......- ...
+00000d80: e4bf a1e9 aa8c e8af 81e7 99bb e5bd 95ef  ................
+00000d90: bc8c e585 8de6 8a93 e58c 85e8 8eb7 e58f  ................
+00000da0: 9620 436f 6f6b 6965 0a2d 20e8 87aa e58a  . Cookie.- .....
+00000db0: a8e5 ae8c e688 90e6 af8f e697 a5e7 b1b3  ................
+00000dc0: e6b8 b8e5 b881 e4bb bbe5 8aa1 0a2d 20e8  .............- .
+00000dd0: 87aa e58a a8e8 bf9b e8a1 8ce6 b8b8 e688  ................
+00000de0: 8fe7 adbe e588 b00a 2d20 e58f afe5 88b6  ........- ......
+00000df0: e5ae 9ae7 b1b3 e6b8 b8e5 b881 e595 86e5  ................
+00000e00: 9381 e585 91e6 8da2 e8ae a1e5 8892 efbc  ................
+00000e10: 8ce5 88b0 e782 b9e5 8591 e68d a2ef bc88  ................
+00000e20: e59b a0e5 8aa0 e585 a5e4 ba86 e4ba bae6  ................
+00000e30: 9cba e9aa 8ce8 af81 efbc 8ce6 8890 e58a  ................
+00000e40: 9fe7 8e87 e8be 83e4 bd8e efbc 890a 2d20  ..............- 
+00000e50: e58f afe6 94af e68c 81e5 a49a e4b8 aa20  ............... 
+00000e60: 5151 20e8 b4a6 e58f b7ef bc8c e6af 8fe4  QQ .............
+00000e70: b8aa 2051 5120 e8b4 a6e5 8fb7 e58f afe7  .. QQ ..........
+00000e80: bb91 e5ae 9ae5 a49a e4b8 aae7 b1b3 e593  ................
+00000e90: 88e6 b8b8 e8b4 a6e6 88b7 0a2d 2051 5120  ...........- QQ 
+00000ea0: e68e a8e9 8081 e689 a7e8 a18c e7bb 93e6  ................
+00000eb0: 9e9c e980 9ae7 9fa5 0a2d 20e5 8e9f e7a5  .........- .....
+00000ec0: 9ee3 8081 e5b4 a9e5 9d8f efbc 9ae6 989f  ................
+00000ed0: e7a9 b9e9 9381 e981 93e7 8ab6 e680 81e4  ................
+00000ee0: bebf e7ac bae9 809a e79f a50a 0a23 2320  .............## 
+00000ef0: e4bd bfe7 94a8 e8af b4e6 988e 0a0a 2323  ..............##
+00000f00: 2320 f09f 9ba0 efb8 8f20 4e6f 6e65 426f  # ....... NoneBo
+00000f10: 7432 20e6 9cba e599 a8e4 baba e983 a8e7  t2 .............
+00000f20: bdb2 e592 8ce6 8f92 e4bb b6e5 ae89 e8a3  ................
+00000f30: 850a 0ae8 afb7 e69f a5e7 9c8b 202d 3e20  ............ -> 
+00000f40: 5bf0 9f94 9749 6e73 7461 6c6c 6174 696f  [....Installatio
+00000f50: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+00000f60: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000f70: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000f80: 7374 6f6f 6c2f 7769 6b69 2f49 6e73 7461  stool/wiki/Insta
+00000f90: 6c6c 6174 696f 6e29 0a0a 2323 2320 f09f  llation)..### ..
+00000fa0: 9396 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4  .. .............
+00000fb0: bdbf e794 a8e8 afb4 e698 8e0a 0ae8 afb7  ................
+00000fc0: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9757  ...... -> [....W
+00000fd0: 696b 6920 e696 87e6 a1a3 5d28 6874 7470  iki ......](http
+00000fe0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+00000ff0: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
+00001000: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
+00001010: 696b 6929 0a0a 2323 2320 e29d 9320 e88e  iki)..### ... ..
+00001020: b7e5 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9  ................
+00001030: e4bf a1e6 81af 0a0a 2323 2323 20e6 8f92  ........#### ...
+00001040: e4bb b6e5 91bd e4bb a40a 0a60 6060 0a2f  ...........```./
+00001050: e5b8 aee5 8aa9 0a60 6060 0a0a 3e20 e29a  .......```..> ..
+00001060: a0ef b88f 20e6 b3a8 e684 8f20 e6ad a4e5  .... ...... ....
+00001070: a484 e6b2 a1e6 9c89 e4bd bfe7 94a8 205b  .............. [
+00001080: f09f 9497 20e6 8f92 e4bb b6e5 91bd e4bb  .... ...........
+00001090: a4e5 a4b4 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+000010a0: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
+000010b0: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
+000010c0: 2d6d 7973 746f 6f6c 2f77 696b 692f 436f  -mystool/wiki/Co
+000010d0: 6e66 6967 7572 6174 696f 6e2d 436f 6e66  nfiguration-Conf
+000010e0: 6967 2363 6f6d 6d61 6e64 7374 6172 7429  ig#commandstart)
+000010f0: 0a0a 2323 20e5 85b6 e4bb 960a 0a23 2323  ..## ........###
+00001100: 205b f09f 9383 e6ba 90e7 a081 e8af b4e6   [..............
+00001110: 988e 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
+00001120: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+00001130: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00001140: 7973 746f 6f6c 2f77 696b 692f 536f 7572  ystool/wiki/Sour
+00001150: 6365 2d53 7472 7563 7475 7265 290a 2323  ce-Structure).##
+00001160: 2320 e980 82e9 858d 205b e7bb aae5 b1b1  # ...... [......
+00001170: e79c 9fe5 afbb 426f 745d 2868 7474 7073  ......Bot](https
+00001180: 3a2f 2f67 6974 6875 622e 636f 6d2f 4869  ://github.com/Hi
+00001190: 6269 4b69 6572 2f7a 6865 6e78 756e 5f62  biKier/zhenxun_b
+000011a0: 6f74 2920 e79a 84e5 8886 e694 af0a 2d20  ot) ..........- 
+000011b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000011c0: 6f6d 2f4d 5754 4a43 2f7a 6865 6e78 756e  om/MWTJC/zhenxun
+000011d0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c0a  -plugin-mystool.
+000011e0: 2d20 6874 7470 733a 2f2f 6769 7468 7562  - https://github
+000011f0: 2e63 6f6d 2f61 7961 6b61 7375 6b69 2f6e  .com/ayakasuki/n
+00001200: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00001210: 7374 6f6f 6c0a                           stool.
```

### Comparing `nonebot_plugin_mystool-1.2.0/pyproject.toml` & `nonebot_plugin_mystool-1.2.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v1.2.0"
-description = "QQ聊天、频道机器人插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神崩铁便笺提醒"
+version = "v1.2.0-beta.1"
+description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool"
 repository = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool"
 documentation = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki"
-keywords = ["bot", "qq", "qqbot", "onebotv11", "onebot", "nonebot2", "nonebot", "mihoyo", "mihoyobbs", "qqguild", "star-rail", "genshin-impact"]
+keywords = ["bot", "qq", "qqbot", "onebotv11", "onebot", "nonebot2", "nonebot", "mihoyo", "mihoyobbs"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable"
 ]
 packages = [
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 address_matcher.usage = '跟随指引，获取地址ID，用于兑换米游币商品。在获取地址ID前，如果你还没有设置米游社收获地址，请前往官网或App设置'
 
 
 @address_matcher.handle()
 async def _(event: GeneralMessageEvent, matcher: Matcher, state: T_State):
     if isinstance(event, GeneralGroupMessageEvent):
         await address_matcher.finish("⚠️为了保护您的隐私，请私聊进行地址设置。")
-    user = _conf.users.get(event.get_user_id())
+    user = _conf.users.get(event.user_id)
     user_account = user.accounts if user else None
     if not user_account:
         await address_matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     else:
         await address_matcher.send(
             "请跟随指引设置收货地址ID，如果你还没有设置米游社收获地址，请前往官网或App设置。\n🚪过程中发送“退出”即可退出")
     if len(user_account) == 1:
@@ -42,15 +42,15 @@
 
 
 @address_matcher.got('bbs_uid')
 async def _(event: GeneralPrivateMessageEvent, state: T_State, bbs_uid=ArgStr()):
     if bbs_uid == '退出':
         await address_matcher.finish('🚪已成功退出')
 
-    user_account = _conf.users[event.get_user_id()].accounts
+    user_account = _conf.users[event.user_id].accounts
     if bbs_uid not in user_account:
         await address_matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
     account = user_account[bbs_uid]
     state['account'] = account
 
     address_status, address_list = await get_address(account)
     state['address_list'] = address_list
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/data_model.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/data_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from multiprocessing.pool import Pool
 from multiprocessing.synchronize import Lock
 from typing import List, Callable, Any, Tuple, Optional, Dict
 
 import nonebot
 from apscheduler.events import JobExecutionEvent, EVENT_JOB_EXECUTED
 from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageEvent as OneBotV11MessageEvent, MessageSegment as OneBotV11MessageSegment
+from nonebot.adapters.onebot.v11 import MessageEvent as OnebotV11MessageEvent, MessageSegment as OnebotV11MessageSegment
 from nonebot.adapters.qqguild import MessageEvent as QQGuildMessageEvent, MessageSegment as QQGuildMessageSegment
 from nonebot.internal.params import ArgStr
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, T_State, CommandArg, Command
 from nonebot_plugin_apscheduler import scheduler
 
 from .data_model import Good, GameRecord, ExchangeStatus
@@ -326,20 +326,20 @@
         await get_good_image.reject('⚠️您的输入有误，请重新输入')
 
     img_path = time.strftime(
         f'{_conf.good_list_image_config.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
     if os.path.exists(img_path):
         with open(img_path, 'rb') as f:
             image_bytes = io.BytesIO(f.read())
-        msg = None
-        if isinstance(event, OneBotV11MessageEvent):
-            msg = OneBotV11MessageSegment.image(image_bytes)
+        message_segment = None
+        if isinstance(event, OnebotV11MessageEvent):
+            message_segment = OnebotV11MessageSegment.image(image_bytes)
         elif isinstance(event, QQGuildMessageEvent):
-            msg = QQGuildMessageSegment.file_image(image_bytes)
-        await get_good_image.finish(msg)
+            message_segment = QQGuildMessageSegment.file_image(image_bytes)
+        await get_good_image.finish(message_segment)
     else:
         await get_good_image.finish(
             f'{arg[1]} 分区暂时没有可兑换的限时商品。如果这与实际不符，你可以尝试用『{COMMAND_BEGIN}商品 更新』进行更新。')
 
 
 lock = threading.Lock()
 finished: Dict[ExchangePlan, List[bool]] = {}
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/game_sign_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/game_sign_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
 
 class HonkaiImpact3Sign(BaseGameSign):
     """
     崩坏3 游戏签到
     """
     NAME = "崩坏3"
-    ACT_ID = "e202306201626331"
+    ACT_ID = "e202207181446311"
     GAME_ID = 1
 
 
 class HoukaiGakuen2Sign(BaseGameSign):
     """
     崩坏学园2 游戏签到
     """
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/good_image.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/good_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 ### 米游社登录获取Cookie相关
 """
 import json
 
 from nonebot import on_command
-from nonebot.adapters.qqguild import MessageSegment as QQGuildMessageSegment, DirectMessageCreateEvent
-from nonebot.adapters.qqguild.exception import AuditException
-from nonebot.exception import ActionFailed
+from nonebot.adapters.qqguild import MessageEvent as QQGuildMessageEvent, \
+    MessageSegment as QQGuildMessageSegment, DirectMessageCreateEvent
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import ArgStr
 from nonebot.params import ArgPlainText, T_State
 
 from .plugin_data import PluginDataManager, write_plugin_data
 from .simple_api import get_login_ticket_by_captcha, get_multi_token_by_login_ticket, get_stoken_v2_by_v1, \
     get_ltoken_by_stoken, get_cookie_token_by_stoken, get_device_fp
@@ -26,35 +25,27 @@
 
 
 @get_cookie.handle()
 async def handle_first_receive(event: GeneralMessageEvent):
     if isinstance(event, GeneralGroupMessageEvent):
         await get_cookie.finish("⚠️为了保护您的隐私，请私聊进行登录。")
     user_num = len(_conf.users)
-    if user_num <= _conf.preference.max_user or _conf.preference.max_user in [-1, 0]:
+    if user_num < _conf.preference.max_user or _conf.preference.max_user in [-1, 0]:
         # QQ频道可能无法发送链接，需要发送二维码
         login_url = "https://user.mihoyo.com/#/login/captcha"
-        msg_text = "登录过程概览：\n" \
-                   "1.发送手机号\n" \
-                   "2.{browse_way}，输入手机号并获取验证码（不要在网页上登录）\n" \
-                   "3.发送验证码给QQ机器人，完成登录\n" \
-                   "🚪过程中发送“退出”即可退出"
-        try:
-            await get_cookie.send(msg_text.format(browse_way=f"前往 {login_url}"))
-        except ActionFailed:
-            logger.exception("发送包含URL链接的登录消息失败")
-            msg_img = QQGuildMessageSegment.file_image(generate_qr_img(login_url))
-            try:
-                await get_cookie.send(msg_img)
-                await get_cookie.send(msg_text.format(browse_way="扫描二维码，进入米哈游官方登录页"))
-            except (ActionFailed, AuditException) as e:
-                if isinstance(e, ActionFailed):
-                    logger.exception("发送包含二维码的登录消息失败")
-                    await get_cookie.send(msg_text.format(
-                        browse_way="前往米哈游官方登录页") + "\n\n⚠️发送二维码失败，请自行搜索米哈游通行证登录页")
+        msg = "登录过程概览：\n" \
+              "1.发送手机号\n" \
+              "2.扫描二维码，进入米哈游官方登录页，输入手机号并获取验证码（网页上不要登录）\n" \
+            if isinstance(event, QQGuildMessageEvent) else \
+            f"2.前往 {login_url}，输入手机号并获取验证码（网页上不要登录）\n" \
+            "3.发送验证码给QQ机器人，完成登录\n" \
+            "🚪过程中发送“退出”即可退出"
+        if isinstance(event, QQGuildMessageEvent):
+            msg += QQGuildMessageSegment.file_image(generate_qr_img(login_url))
+        await get_cookie.send(msg)
     else:
         await get_cookie.finish('⚠️目前可支持使用用户数已经满啦~')
 
 
 @get_cookie.got('phone', prompt='1.请发送您的手机号：')
 async def _(_: GeneralPrivateMessageEvent, state: T_State, phone: str = ArgPlainText('phone')):
     if phone == '退出':
@@ -65,15 +56,15 @@
         await get_cookie.reject("⚠️手机号应为11位数字，请重新输入")
     else:
         state['phone'] = phone
 
 
 @get_cookie.handle()
 async def _(_: GeneralPrivateMessageEvent):
-    await get_cookie.send('2.前往米哈游官方登录页，获取验证码（不要登录！）')
+    await get_cookie.send('2.前往 https://user.mihoyo.com/#/login/captcha，获取验证码（不要登录！）')
 
 
 @get_cookie.got("captcha", prompt='3.请发送验证码：')
 async def _(event: GeneralPrivateMessageEvent, state: T_State, captcha: str = ArgPlainText('captcha')):
     phone_number: str = state['phone']
     if captcha == '退出':
         await get_cookie.finish("🚪已成功退出")
@@ -99,48 +90,48 @@
                 })
                 account = user.accounts[cookies.bbs_uid]
             else:
                 account.cookies.update(cookies)
             if not account.device_id_ios:
                 fp_status, account.device_fp = await get_device_fp(account.device_id_ios)
                 if fp_status:
-                    logger.success(f"用户 {cookies.bbs_uid} 成功获取 device_fp: {account.device_fp}")
+                    logger.info(f"用户 {cookies.bbs_uid} 成功获取 device_fp: {account.device_fp}")
             write_plugin_data()
 
             # 2. 通过 login_ticket 获取 stoken 和 ltoken
             if login_status or account:
                 login_status, cookies = await get_multi_token_by_login_ticket(account.cookies)
                 if login_status:
-                    logger.success(f"用户 {phone_number} 成功获取 stoken: {cookies.stoken}")
+                    logger.info(f"用户 {phone_number} 成功获取 stoken: {cookies.stoken}")
                     account.cookies.update(cookies)
                     write_plugin_data()
 
                     # 3. 通过 stoken_v1 获取 stoken_v2 和 mid
                     login_status, cookies = await get_stoken_v2_by_v1(account.cookies, account.device_id_ios)
                     if login_status:
-                        logger.success(f"用户 {phone_number} 成功获取 stoken_v2: {cookies.stoken_v2}")
+                        logger.info(f"用户 {phone_number} 成功获取 stoken_v2: {cookies.stoken_v2}")
                         account.cookies.update(cookies)
                         write_plugin_data()
 
                         # 4. 通过 stoken_v2 获取 ltoken
                         login_status, cookies = await get_ltoken_by_stoken(account.cookies, account.device_id_ios)
                         if login_status:
-                            logger.success(f"用户 {phone_number} 成功获取 ltoken: {cookies.ltoken}")
+                            logger.info(f"用户 {phone_number} 成功获取 ltoken: {cookies.ltoken}")
                             account.cookies.update(cookies)
                             write_plugin_data()
 
                             # 5. 通过 stoken_v2 获取 cookie_token
                             login_status, cookies = await get_cookie_token_by_stoken(account.cookies,
                                                                                      account.device_id_ios)
                             if login_status:
-                                logger.success(f"用户 {phone_number} 成功获取 cookie_token: {cookies.cookie_token}")
+                                logger.info(f"用户 {phone_number} 成功获取 cookie_token: {cookies.cookie_token}")
                                 account.cookies.update(cookies)
                                 write_plugin_data()
 
-                                logger.success(f"{_conf.preference.log_head}米游社账户 {phone_number} 绑定成功")
+                                logger.info(f"{_conf.preference.log_head}米游社账户 {phone_number} 绑定成功")
                                 await get_cookie.finish(f"🎉米游社账户 {phone_number} 绑定成功")
 
         if not login_status:
             notice_text = "⚠️登录失败："
             if login_status.incorrect_captcha:
                 notice_text += "验证码错误！"
             elif login_status.login_expired:
@@ -195,15 +186,15 @@
         msg = "您有多个账号，您要导出哪个账号的Cookies数据？\n"
         msg += "\n".join(map(lambda x: f"🆔{x}", user_account))
         msg += "\n🚪发送“退出”即可退出"
         await output_cookies.send(msg)
 
 
 @output_cookies.got('bbs_uid')
-async def _(event: GeneralPrivateMessageEvent, matcher: Matcher, bbs_uid=ArgStr()):
+async def _(event: GeneralPrivateMessageEvent, matcher: Matcher, state: T_State, bbs_uid=ArgStr()):
     """
     根据手机号设置导出相应的账户的Cookies
     """
     if bbs_uid == '退出':
         await matcher.finish('🚪已成功退出')
     user_account = _conf.users[event.get_user_id()].accounts
     if bbs_uid in user_account:
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/myb_missions_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/myb_missions_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """
 ### 计划任务相关
 """
 import asyncio
 import random
 import threading
 
-from nonebot import on_command, get_adapters
-from nonebot.adapters.onebot.v11 import MessageSegment as OneBotV11MessageSegment, Adapter as OneBotV11Adapter, \
-    MessageEvent as OneBotV11MessageEvent
-from nonebot.adapters.qqguild import MessageSegment as QQGuildMessageSegment, Adapter as QQGuildAdapter, \
-    MessageEvent as QQGuildMessageEvent
-from nonebot.adapters.qqguild.exception import AuditException
-from nonebot.exception import ActionFailed
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import (MessageSegment)
 from nonebot.internal.matcher import Matcher
 from nonebot_plugin_apscheduler import scheduler
 
 from .exchange import generate_image
 from .game_sign_api import BaseGameSign
 from .myb_missions_api import BaseMission, get_missions_state
 from .plugin_data import PluginDataManager, write_plugin_data
@@ -34,15 +29,15 @@
     """
     手动游戏签到函数
     """
     user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await manually_game_sign.send("⏳开始游戏签到...")
-    await perform_game_sign(user_id=event.get_user_id(), matcher=matcher, event=event)
+    await perform_game_sign(user_id=event.get_user_id(), matcher=matcher)
 
 
 manually_bbs_sign = on_command(_conf.preference.command_start + '任务', priority=5, block=True)
 manually_bbs_sign.name = '任务'
 manually_bbs_sign.usage = '手动执行米游币每日任务，可以查看米游币任务完成情况'
 
 
@@ -115,21 +110,20 @@
     """
     user = _conf.users.get(event.get_user_id())
     if not user or not user.accounts:
         await manually_game_sign.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
     await resin_check_sr(user_id=event.get_user_id(), matcher=matcher)
 
 
-async def perform_game_sign(user_id: str, matcher: Matcher = None, event: GeneralMessageEvent = None):
+async def perform_game_sign(user_id: str, matcher: Matcher = None):
     """
     执行游戏签到函数，并发送给用户签到消息。
 
     :param user_id: 用户QQ号
     :param matcher: 事件响应器
-    :param event: 事件
     """
     failed_accounts = []
     user = _conf.users[user_id]
     for account in _conf.users.get(user_id).accounts.values():
         # 自动签到时，要求用户打开了签到功能；手动签到时都可以调用执行。
         if not matcher and not account.enable_game_sign:
             continue
@@ -165,20 +159,20 @@
                 signed = info.is_sign
 
             # 若没签到，则进行签到功能；若获取今日签到情况失败，仍可继续
             if (get_info_status and not info.is_sign) or not get_info_status:
                 if matcher:
                     sign_status = await signer.sign(
                         account.platform,
-                        lambda: matcher.send("⏳正在尝试完成人机验证，请稍后...")
+                        lambda: matcher.send(f"⏳正在尝试完成人机验证，请稍后...")
                     )
                 else:
                     sign_status = await signer.sign(
                         account.platform,
-                        lambda: send_private_msg(user_id=user_id, message="⏳正在尝试完成人机验证，请稍后...")
+                        lambda: send_private_msg(user_id=user_id, message=f"⏳正在尝试完成人机验证，请稍后...")
                     )
                 if not sign_status and (user.enable_notice or matcher):
                     if sign_status.login_expired:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时服务器返回登录失效，请尝试重新登录绑定账户"
                     elif sign_status.need_verify:
                         message = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到时可能遇到验证码拦截，请尝试使用命令『/账号设置』更改设备平台，若仍失败请手动前往米游社签到"
                     else:
@@ -190,15 +184,15 @@
                     await asyncio.sleep(_conf.preference.sleep_time)
                     continue
 
                 await asyncio.sleep(_conf.preference.sleep_time)
 
             # 用户打开通知或手动签到时，进行通知
             if user.enable_notice or matcher:
-                onebot_img_msg, qq_guild_img_msg = "", ""
+                img = ""
                 get_info_status, info = await signer.get_info(account.platform)
                 get_award_status, awards = await signer.get_rewards()
                 if not get_info_status or not get_award_status:
                     msg = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』获取签到结果失败！请手动前往米游社查看"
                 else:
                     award = awards[info.total_sign_day - 1]
                     if info.is_sign:
@@ -207,37 +201,21 @@
                               f"\n🎮『{signer.NAME}』" \
                               f"\n🎮状态: {status}" \
                               f"\n{signer.record.nickname}·{signer.record.level}" \
                               "\n\n🎁今日签到奖励：" \
                               f"\n{award.name} * {award.cnt}" \
                               f"\n\n📅本月签到次数：{info.total_sign_day}"
                         img_file = await get_file(award.icon)
-                        onebot_img_msg = OneBotV11MessageSegment.image(img_file)
-                        qq_guild_img_msg = QQGuildMessageSegment.file_image(img_file)
+                        img = MessageSegment.image(img_file)
                     else:
                         msg = f"⚠️账户 {account.bbs_uid} 🎮『{signer.NAME}』签到失败！请尝试重新签到，若多次失败请尝试重新登录绑定账户"
                 if matcher:
-                    try:
-                        if isinstance(event, OneBotV11MessageEvent):
-                            await matcher.send(msg + onebot_img_msg)
-                        elif isinstance(event, QQGuildMessageEvent):
-                            await matcher.send(msg)
-                            await matcher.send(qq_guild_img_msg)
-                    except (ActionFailed, AuditException):
-                        pass
-                else:
-                    for adapter in get_adapters().values():
-                        try:
-                            if isinstance(adapter, OneBotV11Adapter):
-                                await send_private_msg(use=adapter, user_id=user_id, message=msg + onebot_img_msg)
-                            elif isinstance(adapter, QQGuildAdapter):
-                                await send_private_msg(use=adapter, user_id=user_id, message=msg)
-                                await send_private_msg(use=adapter, user_id=user_id, message=qq_guild_img_msg)
-                        except (ActionFailed, AuditException):
-                            pass
+                    await matcher.send(msg + img)
+                else:
+                    await send_private_msg(user_id=user_id, message=msg + img)
             await asyncio.sleep(_conf.preference.sleep_time)
 
         if not games_has_record:
             if matcher:
                 await matcher.send(f"⚠️您的米游社账户 {account.bbs_uid} 下不存在任何游戏账号，已跳过签到")
             else:
                 await send_private_msg(user_id=user_id,
@@ -372,15 +350,15 @@
                     write_plugin_data()
                     continue
                 if matcher:
                     await matcher.send(f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
             if genshin_board_status.need_verify:
                 if matcher:
-                    await matcher.send('⚠️遇到验证码正在尝试绕过')
+                    await matcher.send(f'⚠️遇到验证码正在尝试绕过')
             msg = ''
             # 手动查询体力时，无需判断是否溢出
             if not matcher:
                 # 体力溢出提醒
                 if board.current_resin == 160:
                     # 防止重复提醒
                     if has_checked[account.bbs_uid]['resin']:
@@ -457,15 +435,15 @@
                     write_plugin_data()
                     continue
                 if matcher:
                     await matcher.send(f'⚠️账户 {account.bbs_uid} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
             if starrail_board_status.need_verify:
                 if matcher:
-                    await matcher.send('⚠️遇到验证码正在尝试绕过')
+                    await matcher.send(f'⚠️遇到验证码正在尝试绕过')
             msg = ''
             # 手动查询体力时，无需判断是否溢出
             if not matcher:
                 # 体力溢出提醒
                 if board.current_stamina == 180:
                     # 防止重复提醒
                     if has_checked[account.bbs_uid]['stamina']:
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/plugin_data.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/plugin_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from loguru import logger
 from pydantic import BaseModel, ValidationError, BaseSettings, validator, Extra
 
 from . import user_data
 from .user_data import UserData, UserAccount
 
-VERSION = "v1.2.0"
+VERSION = "v1.2.0-beta.1"
 """程序当前版本"""
 
 ROOT_PATH = Path(__name__).parent.absolute()
 '''NoneBot2 机器人根目录'''
 
 DATA_PATH = ROOT_PATH / "data" / "nonebot-plugin-mystool"
 '''插件数据保存目录'''
@@ -140,41 +140,40 @@
     '''是否使用多进程生成图片（如果生成图片时崩溃，可尝试关闭此选项）'''
 
 
 class SaltConfig(BaseSettings):
     """
     生成Headers - DS所用salt值，非必要请勿修改
     """
-    SALT_IOS: str = "F6tsiCZEIcL9Mor64OXVJEKRRQ6BpOZa"
-    '''LK2 - 生成Headers iOS DS所需的salt'''
+    SALT_IOS: str = "ulInCDohgEs557j0VsPDYnQaaz6KJcv5"
+    '''生成Headers iOS DS所需的salt'''
     SALT_ANDROID: str = "n0KjuIrKgLHh08LWSCYP0WXlVXaYvV64"
     '''生成Headers Android DS所需的salt'''
     SALT_DATA: str = "t0qEgfub6cvueAPgR5m9aQWWVciEer7v"
-    '''6X - Android 设备传入content生成 DS 所需的 salt'''
+    '''Android 设备传入content生成 DS 所需的 salt'''
     SALT_PARAMS: str = "xV8v4Qu54lUKrEYFZkJhB8cuOh9Asafs"
-    '''4X - Android 设备传入url参数生成 DS 所需的 salt'''
+    '''Android 设备传入url参数生成 DS 所需的 salt'''
     SALT_PROD: str = "JwYDpKvLj6MrMqqYU6jTKF17KNO2PXoS"
-    '''PROD'''
 
     class Config(Preference.Config):
         pass
 
 
 class DeviceConfig(BaseSettings):
     """
     设备信息
     Headers所用的各种数据，非必要请勿修改
     """
-    USER_AGENT_MOBILE: str = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) miHoYoBBS/2.55.1"
+    USER_AGENT_MOBILE: str = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) miHoYoBBS/2.54.1"
     '''移动端 User-Agent(Mozilla UA)'''
     USER_AGENT_PC: str = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.0 Safari/605.1.15"
     '''桌面端 User-Agent(Mozilla UA)'''
     USER_AGENT_OTHER: str = "Hyperion/275 CFNetwork/1402.0.8 Darwin/22.2.0"
     '''获取用户 ActionTicket 时Headers所用的 User-Agent'''
-    USER_AGENT_ANDROID: str = "Mozilla/5.0 (Linux; Android 11; MI 8 SE Build/RQ3A.211001.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/104.0.5112.97 Mobile Safari/537.36 miHoYoBBS/2.55.1"
+    USER_AGENT_ANDROID: str = "Mozilla/5.0 (Linux; Android 11; MI 8 SE Build/RQ3A.211001.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/104.0.5112.97 Mobile Safari/537.36 miHoYoBBS/2.54.1"
     '''安卓端 User-Agent(Mozilla UA)'''
     USER_AGENT_ANDROID_OTHER: str = "okhttp/4.9.3"
     '''安卓端 User-Agent(专用于米游币任务等)'''
     USER_AGENT_WIDGET: str = "WidgetExtension/231 CFNetwork/1390 Darwin/22.0.0"
     '''iOS 小组件 User-Agent(原神实时便笺)'''
 
     X_RPC_DEVICE_MODEL_MOBILE: str = "iPhone10,2"
@@ -187,25 +186,25 @@
     X_RPC_DEVICE_NAME_MOBILE: str = "iPhone"
     '''移动端 x-rpc-device_name'''
     X_RPC_DEVICE_NAME_PC: str = "Microsoft Edge 103.0.1264.62"
     '''桌面端 x-rpc-device_name'''
     X_RPC_DEVICE_NAME_ANDROID: str = "Xiaomi MI 8 SE"
     '''安卓端 x-rpc-device_name'''
 
-    X_RPC_SYS_VERSION: str = "16.2"
+    X_RPC_SYS_VERSION: str = "15.4"
     '''Headers所用的 x-rpc-sys_version'''
     X_RPC_SYS_VERSION_ANDROID: str = "11"
     '''安卓端 x-rpc-sys_version'''
 
     X_RPC_CHANNEL: str = "appstore"
     '''Headers所用的 x-rpc-channel'''
     X_RPC_CHANNEL_ANDROID: str = "miyousheluodi"
     '''安卓端 x-rpc-channel'''
 
-    X_RPC_APP_VERSION: str = "2.55.1"
+    X_RPC_APP_VERSION: str = "2.54.1"
     '''Headers所用的 x-rpc-app_version'''
     X_RPC_PLATFORM: str = "ios"
     '''Headers所用的 x-rpc-platform'''
     UA: str = "\".Not/A)Brand\";v=\"99\", \"Microsoft Edge\";v=\"103\", \"Chromium\";v=\"103\""
     '''Headers所用的 sec-ch-ua'''
     UA_PLATFORM: str = "\"macOS\""
     '''Headers所用的 sec-ch-ua-platform'''
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,103 +130,100 @@
     elif setting_id == '6':
         await account_setting.send(
             "请发送想要修改体力提醒阈值的游戏编号："
             "\n1. 原神"
             "\n2. 崩坏：星穹铁道"
             "\n\n🚪发送“退出”即可退出"
         )
-        state["setting_item"] = "setting_notice_value"
-        return
+        state["setting_item"] = "notice_value"
     elif setting_id == '7':
         state["prepare_to_delete"] = True
         await account_setting.reject(f"⚠️确认删除账号 {account.phone_number} ？发送 \"确认删除\" 以确定。")
     elif setting_id == '确认删除' and state["prepare_to_delete"]:
         user_account.pop(account.bbs_uid)
         write_plugin_data()
         await account_setting.finish(f"已删除账号 {account.phone_number} 的数据")
     else:
         await account_setting.reject("⚠️您的输入有误，请重新输入")
 
-    state["notice_game"] = ""
-
 
 @account_setting.got('notice_game')
 async def _(_: GeneralMessageEvent, state: T_State, notice_game=ArgStr()):
     if notice_game == '退出':
         await account_setting.finish('🚪已成功退出')
-    elif state["setting_item"] == "setting_notice_value":
+    if state["setting_item"] == "notice_value":
         if notice_game == "1":
             await account_setting.send(
                 "请输入想要所需通知阈值，树脂达到该值时将进行通知："
                 "可用范围 [0, 160]"
                 "\n\n🚪发送“退出”即可退出"
             )
-            state["setting_item"] = "setting_notice_value_op"
+            state["setting_item"] = "notice_value_op"
         elif notice_game == "2":
             await account_setting.send(
                 "请输入想要所需阈值数字，开拓力达到该值时将进行通知："
                 "可用范围 [0, 180]"
                 "\n\n🚪发送“退出”即可退出"
             )
-            state["setting_item"] = "setting_notice_value_sr"
+            state["setting_item"] = "notice_value_sr"
         else:
             await account_setting.reject("⚠️您的输入有误，请重新输入")
 
 
-@account_setting.got('setting_value')
-async def _(_: GeneralMessageEvent, state: T_State, setting_value=ArgStr()):
-    if setting_value == '退出':
+@account_setting.got('notice_value')
+async def _(_: GeneralMessageEvent, state: T_State, notice_value=ArgStr()):
+    if notice_value == '退出':
         await account_setting.finish('🚪已成功退出')
     account: UserAccount = state['account']
 
-    if state["setting_item"] == "setting_notice_value_op":
+    if state["setting_item"] == "notice_value_op":
         try:
-            resin_threshold = int(setting_value)
+            resin_threshold = int(notice_value)
         except ValueError:
             await account_setting.reject("⚠️请输入有效的数字。")
         else:
             if 0 <= resin_threshold <= 160:
                 # 输入有效的数字范围，将 resin_threshold 赋值为输入的整数
                 account.user_resin_threshold = resin_threshold
                 write_plugin_data()
-                await account_setting.finish("更改原神便笺树脂提醒阈值成功\n"
+                await account_setting.finish(f"更改原神便笺树脂提醒阈值成功\n"
                                              f"⏰当前提醒阈值：{resin_threshold}")
             else:
                 await account_setting.reject("⚠️输入的数字范围应在 0 到 160 之间。")
 
-    elif state["setting_item"] == "setting_notice_value_sr":
+    elif state["setting_item"] == "notice_value_sr":
         try:
-            stamina_threshold = int(setting_value)
+            stamina_threshold = int(notice_value)
         except ValueError:
             await account_setting.reject("⚠️请输入有效的数字。")
         else:
             if 0 <= stamina_threshold <= 180:
                 # 输入有效的数字范围，将 stamina_threshold 赋值为输入的整数
                 account.user_stamina_threshold = stamina_threshold
                 write_plugin_data()
-                await account_setting.finish("更改崩铁便笺开拓力提醒阈值成功\n"
+                await account_setting.finish(f"更改崩铁便笺开拓力提醒阈值成功\n"
                                              f"⏰当前提醒阈值：{stamina_threshold}")
             else:
                 await account_setting.reject("⚠️输入的数字范围应在 0 到 180 之间。")
 
     elif state["setting_item"] == "mission_games":
-        games_input = setting_value.split()
+        games_input = notice_value.split()
         mission_games = set()
         for game in games_input:
             game_filter = filter(lambda x: x.NAME == game, BaseMission.AVAILABLE_GAMES)
             game_obj = next(game_filter, None)
             if game_obj is None:
                 await account_setting.reject("⚠️您的输入有误，请重新输入")
             else:
                 mission_games.add(game_obj)
 
         account.mission_games = mission_games
         write_plugin_data()
-        setting_value = setting_value.replace(" ", "、")
-        await account_setting.finish(f"💬执行米游币任务的频道已更改为『{setting_value}』")
+        notice_value = notice_value.replace(" ", "、")
+        await account_setting.finish(f"💬执行米游币任务的频道已更改为『{notice_value}』")
 
 
 global_setting = on_command(_conf.preference.command_start + '通知设置', priority=5, block=True)
 global_setting.name = "通知设置"
 global_setting.usage = "设置每日签到后是否进行QQ通知"
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/simple_api.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/simple_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/user_check.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 ### QQ好友相关、用户绑定相关
 """
 import asyncio
 from uuid import uuid4
 
 from nonebot import get_driver, on_request, on_command, Bot
-from nonebot.adapters.onebot.v11 import FriendRequestEvent, GroupRequestEvent, RequestEvent, Bot as OneBotV11Bot, \
-    ActionFailed as OneBotV11ActionFailed
+from nonebot.adapters.onebot.v11 import FriendRequestEvent, GroupRequestEvent, RequestEvent, Bot as OneBotV11Bot
 from nonebot.adapters.qqguild import Bot as QQGuildBot
-from nonebot.adapters.qqguild.exception import ActionFailed as QQGuildActionFailed
 from nonebot.internal.matcher import Matcher
 from nonebot.params import CommandArg, Command
 
 from .plugin_data import PluginDataManager, write_plugin_data
 from .user_data import uuid4_validate
 from .utils import logger, GeneralMessageEvent, COMMAND_BEGIN, get_last_command_sep, GeneralGroupMessageEvent, PLUGIN, \
     send_private_msg
@@ -202,34 +200,22 @@
         f"{_conf.preference.command_start}私聊响应",
         f"{_conf.preference.command_start}请求响应"
     },
     priority=5,
     block=True
 )
 direct_msg_respond.name = '私信响应'
-direct_msg_respond.usage = '让机器人私信发送给您一条消息，防止因为发送了三条私信消息而机器人未回复导致无法继续私信。' \
-                           '需要注意每个机器人每天只能对一个用户发2条主动消息。'
+direct_msg_respond.usage = '让机器人私信发送给您一条消息，防止因为发送了三条私信消息而机器人未回复导致无法继续私信'
 
 
 @direct_msg_respond.handle()
 async def _(bot: Bot, event: GeneralGroupMessageEvent):
     msg_text = f"{PLUGIN.metadata.name}" \
                f"{PLUGIN.metadata.description}\n" \
                "具体用法：\n" \
                f"{PLUGIN.metadata.usage.format(HEAD=COMMAND_BEGIN)}"
-    try:
-        if await send_private_msg(
-                user_id=event.get_user_id(),
-                message=msg_text,
-                guild_id=event.guild_id,
-                use=bot
-        ):
-            await direct_msg_respond.send("✔已发送私信，请查看私信消息")
-        else:
-            await direct_msg_respond.send("⚠️发送私信失败，请检查后台日志")
-    except (QQGuildActionFailed, OneBotV11ActionFailed) as e:
-        if isinstance(e, QQGuildActionFailed):
-            if e.code == 304049:
-                await direct_msg_respond.finish(f"⚠️发送私信失败，达到了机器人每日主动私信次数限制。错误信息：{e!r}")
-            elif e.code == 304022:
-                await direct_msg_respond.finish(f"⚠️发送私信失败，请换一个时间再试。错误信息：{e!r}")
-        await direct_msg_respond.finish(f"⚠️发送私信失败，错误信息：{e!r}")
+    await send_private_msg(
+        user_id=event.get_user_id(),
+        message=msg_text,
+        guild_id=event.guild_id,
+        use=bot
+    )
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/user_data.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/user_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,16 @@
         cookie_type: 是否返回符合Cookie类型的字典（没有自定义的stoken_v1、stoken_v2键）
         """
         # 保证 stuid, ltuid 等字段存在
         self.bbs_uid = self.bbs_uid
         cookies_dict = super().dict(include=include, exclude=exclude, by_alias=by_alias, skip_defaults=skip_defaults,
                                     exclude_unset=exclude_unset, exclude_defaults=exclude_defaults,
                                     exclude_none=exclude_none)
-        if v2_stoken and self.stoken_v2:
+        if v2_stoken:
             cookies_dict["stoken"] = self.stoken_v2
-        else:
-            cookies_dict["stoken"] = self.stoken_v1
 
         if cookie_type:
             # 去除自定义的 stoken_v1, stoken_v2 字段
             cookies_dict.pop("stoken_v1")
             cookies_dict.pop("stoken_v2")
 
             # 去除空的字段
```

### Comparing `nonebot_plugin_mystool-1.2.0/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-1.2.0b1/src/nonebot_plugin_mystool/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import httpx
 import nonebot
 import nonebot.log
 import nonebot.plugin
 import tenacity
 from nonebot import Adapter, Bot
 from nonebot.adapters import Message
-from nonebot.adapters.onebot.v11 import MessageEvent as OneBotV11MessageEvent, PrivateMessageEvent, GroupMessageEvent, \
-    Adapter as OneBotV11Adapter, Bot as OneBotV11Bot
+from nonebot.adapters.onebot.v11 import MessageEvent as OnebotV11MessageEvent, PrivateMessageEvent, GroupMessageEvent, \
+    Adapter as OnebotV11Adapter, Bot as OnebotV11Bot
 from nonebot.adapters.qqguild import DirectMessageCreateEvent, MessageCreateEvent, \
     Adapter as QQGuildAdapter, Bot as QQGuildBot, MessageSegment as QQGuildMessageSegment, Message as QQGuildMessage
 from nonebot.adapters.qqguild.api import DMS
 from nonebot.adapters.qqguild.exception import ActionFailed
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 from qrcode import QRCode
@@ -33,15 +33,15 @@
 from .plugin_data import PluginDataManager, Preference
 
 if TYPE_CHECKING:
     from loguru import Logger
 
 _conf = PluginDataManager.plugin_data
 
-GeneralMessageEvent = Union[OneBotV11MessageEvent, MessageCreateEvent, DirectMessageCreateEvent]
+GeneralMessageEvent = Union[OnebotV11MessageEvent, MessageCreateEvent, DirectMessageCreateEvent]
 """消息事件类型"""
 GeneralPrivateMessageEvent = Union[PrivateMessageEvent, DirectMessageCreateEvent]
 """私聊消息事件类型"""
 GeneralGroupMessageEvent = Union[GroupMessageEvent, MessageCreateEvent]
 """群聊消息事件类型"""
 
 
@@ -83,24 +83,20 @@
 
 def set_logger(logger: "Logger"):
     """
     给日志记录器对象增加输出到文件的Handler
     """
     # 根据"name"筛选日志，如果在 plugins 目录加载，则通过 LOG_HEAD 识别
     # 如果不是插件输出的日志，但是与插件有关，则也进行保存
-    logger.add(
-        _conf.preference.log_path,
-        diagnose=False,
-        format=nonebot.log.default_format,
-        rotation=_conf.preference.log_rotation,
-        filter=lambda x: x["name"] == _conf.preference.plugin_name or (
-                _conf.preference.log_head != "" and x["message"].find(_conf.preference.log_head) == 0
-        ) or x["message"].find(f"plugins.{_conf.preference.plugin_name}") != -1
-    )
-
+    logger.add(_conf.preference.log_path, diagnose=False, format=nonebot.log.default_format,
+               filter=lambda record: record["name"] == _conf.preference.plugin_name or
+                                     (_conf.preference.log_head != "" and record["message"].find(
+                                         _conf.preference.log_head) == 0) or
+                                     record["message"].find(f"plugins.{_conf.preference.plugin_name}") != -1,
+               rotation=_conf.preference.log_rotation)
     return logger
 
 
 logger = set_logger(logger)
 """本插件所用日志记录器对象（包含输出到文件）"""
 
 PLUGIN = nonebot.plugin.get_plugin(_conf.preference.plugin_name)
@@ -322,32 +318,31 @@
 
 
 async def send_private_msg(
         user_id: str,
         message: Union[str, Message],
         use: Union[Bot, Adapter] = None,
         guild_id: int = None
-) -> Union[bool, ActionFailed]:
+):
     """
     主动发送私信消息
 
     :param user_id: 目标用户ID
     :param message: 消息内容
     :param use: 使用的Bot或Adapter，为None则使用所有Bot
     :param guild_id: 用户所在频道ID，为None则从用户数据中获取
     :return: 是否发送成功
-    :raise ActionFailed
     """
-    if isinstance(use, (OneBotV11Bot, QQGuildBot)):
+    if isinstance(use, (OnebotV11Bot, QQGuildBot)):
         bots = [use]
-    elif isinstance(use, (OneBotV11Adapter, QQGuildAdapter)):
+    elif isinstance(use, (OnebotV11Adapter, QQGuildAdapter)):
         bots = use.bots.values()
     else:
         bots = nonebot.get_bots().values()
-    if isinstance(use, (OneBotV11Bot, OneBotV11Adapter)):
+    if isinstance(use, (OnebotV11Bot, OnebotV11Adapter)):
         for bot in bots:
             await bot.send_private_msg(user_id=int(user_id), message=message)
         return True
     elif isinstance(use, (QQGuildBot, QQGuildAdapter)):
         message = QQGuildMessageSegment.text(message) if isinstance(message, str) else message
         message = message if isinstance(message, QQGuildMessage) else QQGuildMessage(message)
 
@@ -387,23 +382,23 @@
                         embed=embed,  # type: ignore
                         ark=ark,  # type: ignore
                         image=image,  # type: ignore
                         file_image=file_image,  # type: ignore
                         markdown=markdown,  # type: ignore
                         message_reference=reference,  # type: ignore
                     )
-            except ActionFailed as e:
+            except ActionFailed:
                 logger.exception(
                     f"{_conf.preference.log_head}尝试主动发送私信消息失败。"
                     f"频道ID：{guild_id}，用户ID：{user_id}，消息内容：\n"
                     f"{message}"
                 )
-                raise e
             else:
                 return True
+        return False
 
 
 # TODO: 一个用于构建on_command事件相应器的函数，
 #  将使用偏好设置里的priority优先级和block设置，
 #  可能可以作为装饰器使用
 #   （需要先等用户数据改用Pydantic作为数据模型）
 def command_matcher(command: str, priority: int = None, block: bool = None) -> Matcher:
```

### Comparing `nonebot_plugin_mystool-1.2.0/PKG-INFO` & `nonebot_plugin_mystool-1.2.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 1.2.0
-Summary: QQ聊天、频道机器人插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神崩铁便笺提醒
+Version: 1.2.0b1
+Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
-Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs,qqguild,star-rail,genshin-impact
+Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -42,20 +42,14 @@
   <img alt="最新发行版" src="https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge">
   <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
 </div>
 
 # mysTool - 米游社辅助工具插件
 
 ## 📣 更新内容
-### 2023.8.4 - v1.2.0
-- 修复原神签到返回DS无效的问题 #150 #134
-- 修复崩坏三签到返回 “签到功能维护中，请耐心等待” 的问题 #139 #131 #130
-- 修复使用QQ频道适配器的情况下可能因为发送消息失败而无法继续的问题 
-- 取消了自动删除非好友的用户数据的功能
-
 ### 2023.7.28 - v1.2.0-beta.1
 - 增加对QQ频道的支持 #128
   > 说明文档：[🔗QQGuild 适配器](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Installation#QQGuild-适配器)
 - 增加用户数据绑定关联功能（如QQ频道账号与QQ聊天账号的数据绑定）
   > 说明文档：[🔗用户数据绑定关联](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-UserBind)
 - 增加原神便笺树脂提醒阈值的设置选项 #151 by @Joseandluue
   > 说明文档：[🔗对绑定的某个米哈游账户进行设置](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-Setting#%E5%AF%B9%E7%BB%91%E5%AE%9A%E7%9A%84%E6%9F%90%E4%B8%AA%E7%B1%B3%E5%93%88%E6%B8%B8%E8%B4%A6%E6%88%B7%E8%BF%9B%E8%A1%8C%E8%AE%BE%E7%BD%AE)
```

