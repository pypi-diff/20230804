# Comparing `tmp/siat-2.4.8-py3-none-any.whl.zip` & `tmp/siat-2.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1723136 bytes, number of entries: 127
+Zip file size: 1723182 bytes, number of entries: 127
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2286 b- defN 23-Jul-17 01:30 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28808 b- defN 23-Jul-20 14:51 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    37055 b- defN 23-Jul-20 14:54 siat/beta_adjustment.py
@@ -100,15 +100,15 @@
 -rw-rw-rw-  2.0 fat     1294 b- defN 23-Jun-14 07:32 siat/stock_china_test.py
 -rw-rw-rw-  2.0 fat  1266744 b- defN 23-Jun-05 00:13 siat/stock_info.pickle
 -rw-rw-rw-  2.0 fat     6122 b- defN 23-Apr-10 11:29 siat/stock_info_test.py
 -rw-rw-rw-  2.0 fat     1014 b- defN 23-Apr-10 11:29 siat/stock_list_china_test.py
 -rw-rw-rw-  2.0 fat    36738 b- defN 23-Apr-10 11:29 siat/stock_prices_kneighbors.py
 -rw-rw-rw-  2.0 fat    13991 b- defN 23-Apr-10 11:29 siat/stock_prices_linear.py
 -rw-rw-rw-  2.0 fat    25092 b- defN 23-Jul-13 11:38 siat/stock_profile.py
--rw-rw-rw-  2.0 fat    72798 b- defN 23-Aug-04 12:16 siat/stock_technical.py
+-rw-rw-rw-  2.0 fat    72967 b- defN 23-Aug-04 13:17 siat/stock_technical.py
 -rw-rw-rw-  2.0 fat    19475 b- defN 23-Apr-10 11:29 siat/stock_test.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/temp.py
 -rw-rw-rw-  2.0 fat    16648 b- defN 23-Apr-18 09:06 siat/test2_graphviz.py
 -rw-rw-rw-  2.0 fat    16999 b- defN 23-Apr-14 14:38 siat/test_graphviz.py
 -rw-rw-rw-  2.0 fat     6122 b- defN 23-Jul-09 07:39 siat/test_markowitz_simple.py
 -rw-rw-rw-  2.0 fat     7407 b- defN 23-Jul-08 17:33 siat/test_markowitz_simple_revised.py
 -rw-rw-rw-  2.0 fat     7361 b- defN 23-Jul-09 11:15 siat/test_markowitz_simple_revised2.py
@@ -118,12 +118,12 @@
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
 -rw-rw-rw-  2.0 fat   135790 b- defN 23-Jul-28 20:52 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    52241 b- defN 23-Jul-19 12:01 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1276 b- defN 23-Aug-04 13:03 siat-2.4.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 13:03 siat-2.4.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-04 13:03 siat-2.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    10212 b- defN 23-Aug-04 13:03 siat-2.4.8.dist-info/RECORD
-127 files, 7849333 bytes uncompressed, 1707550 bytes compressed:  78.2%
+-rw-rw-rw-  2.0 fat     1277 b- defN 23-Aug-04 13:20 siat-2.4.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 13:20 siat-2.4.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-04 13:20 siat-2.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    10212 b- defN 23-Aug-04 13:20 siat-2.4.9.dist-info/RECORD
+127 files, 7849503 bytes uncompressed, 1707596 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -363,20 +363,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-2.4.8.dist-info/METADATA
+Filename: siat-2.4.9.dist-info/METADATA
 Comment: 
 
-Filename: siat-2.4.8.dist-info/WHEEL
+Filename: siat-2.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: siat-2.4.8.dist-info/top_level.txt
+Filename: siat-2.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-2.4.8.dist-info/RECORD
+Filename: siat-2.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/stock_technical.py

```diff
@@ -588,15 +588,16 @@
     MA，又称移动平均线，是借助统计处理方式将若干天的股票价格加以平均，然后连接成一条线，用以观察股价趋势。
     移动平均线通常有3日、6日、10日、12日、24日、30日、72日、200日、288日、13周、26周、52周等等，不一而足，
     其目的在取得某一段期间的平均成本，而以此平均成本的移动曲线配合每日收盘价的线路变化分析某一期间多空的优劣形势，
     以研判股价的可能变化。
     一般来说，现行价格在平均价之上，意味着市场买力（需求）较大，行情看好；
     反之，行情价在平均价之下，则意味着供过于求，卖压显然较重，行情看淡。    
     """
-    if ('MA' in graph) or ('ALL' in graph):
+    #if ('MA' in graph) or ('ALL' in graph):
+    if (graph in ['MA',['MA']]) or ('ALL' in graph):    
         MA_cols=[]
         for mad in MA_days:
             col='MA'+str(mad)+'简单移动均线'
             MA_cols=MA_cols+[col]
             df[col] = talib.MA(df['Close'],timeperiod=mad)
         
         # MA快慢线交叉
@@ -870,15 +871,15 @@
     smooth=True
     linewidth=1.5
     graph=['ALL']
     printout=True
     
 def stock_RSI(ticker,start,end, \
              RSI_days=[6,12,24],RSI_lines=[20,50,80], \
-             resample_freq='H',smooth=False,linewidth=1.5, \
+             resample_freq='H',smooth=True,linewidth=1.5, \
              loc1='lower left',loc2='lower right', \
              graph=['ALL'],printout=True):
     """
     功能：计算股票的技术分析指标RSI
     输入：df，四种股价Open/Close/High/Low，成交量Volume
     输出：df
     含有指标：
@@ -984,14 +985,15 @@
         ax.legend(loc=loc1,fontsize=legend_txt_size)
         
         # 绘制股价在右侧
         #绘证券2：建立第二y轴
         
         #插值平滑
         if smooth:
+            print("  Smoothening curves directly ...")
             try:
                 df5=df_smooth_manual(df4,resample_freq=resample_freq)
             except:
                 df5=df4
         else:
             df5=df4
         
@@ -1073,15 +1075,15 @@
     graph=['ALL']
     printout=True
     
     graph=False
     
 def stock_KDJ(ticker,start,end, \
              KDJ_days=[9,3,3],matypes=[0,0],KDJ_lines=[20,50,80], \
-             resample_freq='H',smooth=False,linewidth=1.5, \
+             resample_freq='H',smooth=True,linewidth=1.5, \
              loc1='lower left',loc2='lower right', \
              graph=['ALL'],printout=True):
     """
     功能：计算股票的技术分析指标KDJ
     输入：df，四种股价Open/Close/High/Low，成交量Volume
     输出：df
     含有指标：
@@ -1237,14 +1239,15 @@
         #ax.set_ylim(-5,105)
         
         # 绘制股价在右侧
         #绘证券2：建立第二y轴
         
         #插值平滑
         if smooth:
+            print("  Smoothening curves directly ...")
             try:
                 df5=df_smooth_manual(df4,resample_freq=resample_freq)
             except:
                 df5=df4
         else:
             df5=df4
```

## Comparing `siat-2.4.8.dist-info/METADATA` & `siat-2.4.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siat
-Version: 2.4.8
+Version: 2.4.9
 Summary: Securities Investment Analysis Tools (siat)
 Home-page: https://pypi.org/project/siat/
 Author: Prof. WANG Dehong, Business School, BFSU
 Author-email: wdehong2000@163.com
 License: Copyright (C) WANG Dehong, 2023. For educational purpose only!
 Requires-Dist: pandas-datareader
 Requires-Dist: yfinance
@@ -26,12 +26,12 @@
 Requires-Dist: pathlib
 Requires-Dist: ruamel-yaml
 Requires-Dist: prettytable
 
 
     This plug-in is designed to use with the author's textbooks on security investment, 
     where case studies can be replayed, updated and re-created in different securities, 
-    different time line and different measurements. 
+    different time lines and different measurements. 
     The plug-in is for teaching and learning purposes only, not for commercial use. 
-    The author is not responsible for the results of applying this plug-in in real 
+    The author is not responsible for any results of applying this plug-in in real 
     investment activities.
```

## Comparing `siat-2.4.8.dist-info/RECORD` & `siat-2.4.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 siat/stock_china_test.py,sha256=eO4HWsSvc6qezl0LndjtL24lViEyrBjH_sx2c2Y2Q2M,1294
 siat/stock_info.pickle,sha256=o4M-pcN8Sh8QiwZQAZWY1aelI4xgIGIxors7n2uHSJI,1266744
 siat/stock_info_test.py,sha256=gfG3DbhDACbtD8wnv_R6zhj0t11XaC8NX8uLD9Qv3Fo,6122
 siat/stock_list_china_test.py,sha256=gv14UwMMvkZqtb6G7DCTSuehIwVHuVwu7w60p6gyHoo,1014
 siat/stock_prices_kneighbors.py,sha256=WfZvo5EyeBsm-T37zDj7Sl9dPSRq5Bx4JxIJ9IUum6s,36738
 siat/stock_prices_linear.py,sha256=-OUKRr27L2aStQgJSlJOrJ4gay_G7P-m-7t7cU2Yoqk,13991
 siat/stock_profile.py,sha256=gr7abaTBpGcMBH5Qo8idQKKRTegr-GDll6iFWXK1DJw,25092
-siat/stock_technical.py,sha256=KY_d42wPSdoWlIquKX9Mdd9aLSS9eKsrRXppIYhue-A,72798
+siat/stock_technical.py,sha256=qLVaog6zn3Kl7AKBn0iYfbEtUmh9bSzfh4uDIazvKUs,72967
 siat/stock_test.py,sha256=E9YJAvOw1VEGJSDI4IZuEjl0tGoisOIlN-g9UqA_IZE,19475
 siat/temp.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/test2_graphviz.py,sha256=05w2YJuIBH0LsJjdA60EFn7rL0vCo-CA6EVJEQOXNE4,16648
 siat/test_graphviz.py,sha256=CETKpDL8PnysS-PD3fHkeAgagUxjaUl0CsXPiadQySg,16999
 siat/test_markowitz_simple.py,sha256=jAgwpkdMGxvjlfEg0I8qbyLQHDd5rErWqHgiqVvOJlY,6122
 siat/test_markowitz_simple_revised.py,sha256=Tq44VTIjc75RR4_AMEWmU3-EW7TH4ZNEC6Zcer3fbmk,7407
 siat/test_markowitz_simple_revised2.py,sha256=r0KzW9zvaP9BTdXyB2M3MhRKtzHDIituAflT9ZTR9bs,7361
@@ -117,11 +117,11 @@
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
 siat/translate.py,sha256=W8Kyb_7GVomX9hDgN1d0uCocQQU-5JRsYPJDah7bglQ,135790
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=SPJFU9J8WJhz_HOXgIAjoG8dZs1zSPS1BZxkjhA-D1w,52241
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-2.4.8.dist-info/METADATA,sha256=X8okNY2Q9Bl8PBR0up-ncJw13lVCM1mcI2RGBY8brfs,1276
-siat-2.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-siat-2.4.8.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-2.4.8.dist-info/RECORD,,
+siat-2.4.9.dist-info/METADATA,sha256=9w2XwXKCo3s3NoeRJnmbz7Q4ZxmmZfyr316wOr6o_18,1277
+siat-2.4.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+siat-2.4.9.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-2.4.9.dist-info/RECORD,,
```

