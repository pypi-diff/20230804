# Comparing `tmp/lexisnexisapi-3.0.tar.gz` & `tmp/lexisnexisapi-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-3.0.tar", last modified: Thu Aug  3 15:32:45 2023, max compression
+gzip compressed data, was "lexisnexisapi-3.0.1.tar", last modified: Fri Aug  4 20:31:44 2023, max compression
```

## Comparing `lexisnexisapi-3.0.tar` & `lexisnexisapi-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.731744 lexisnexisapi-3.0/
--rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0/LICENSE.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6031 2023-08-03 15:32:45.731488 lexisnexisapi-3.0/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0/README.md
--rw-r--r--   0 rwcuffney   (501) staff       (20)      616 2023-08-03 15:21:57.000000 lexisnexisapi-3.0/pyproject.toml
--rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-03 15:32:45.731817 lexisnexisapi-3.0/setup.cfg
--rw-r--r--   0 rwcuffney   (501) staff       (20)      765 2023-08-03 15:21:25.000000 lexisnexisapi-3.0/setup.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.727594 lexisnexisapi-3.0/src/
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.729909 lexisnexisapi-3.0/src/lexisnexisapi/
--rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0/src/lexisnexisapi/__init__.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0/src/lexisnexisapi/credentials.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)    10144 2023-08-02 20:20:42.000000 lexisnexisapi-3.0/src/lexisnexisapi/metabase.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-03 15:32:45.731132 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6031 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)      302 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-03 15:32:45.000000 lexisnexisapi-3.0/src/lexisnexisapi.egg-info/top_level.txt
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.505852 lexisnexisapi-3.0.1/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.1/LICENSE.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-04 20:31:44.505639 lexisnexisapi-3.0.1/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0.1/README.md
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      618 2023-08-04 20:30:10.000000 lexisnexisapi-3.0.1/pyproject.toml
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-04 20:31:44.505918 lexisnexisapi-3.0.1/setup.cfg
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      767 2023-08-04 20:29:23.000000 lexisnexisapi-3.0.1/setup.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.499226 lexisnexisapi-3.0.1/src/
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.502993 lexisnexisapi-3.0.1/src/lexisnexisapi/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/__init__.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/credentials.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     9718 2023-08-04 19:52:06.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/metabase.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     2963 2023-08-04 20:27:36.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/webservices.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.505197 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6148 2023-08-04 20:10:21.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/.DS_Store
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      372 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-3.0/PKG-INFO` & `lexisnexisapi-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 3.0
+Version: 3.0.1
 Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lexisnexisapi-3.0/README.md` & `lexisnexisapi-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0/pyproject.toml` & `lexisnexisapi-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "3.0"
+version = "3.0.1"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
 description = "A module to support the lexisnexis metabase search api"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lexisnexisapi-3.0/setup.py` & `lexisnexisapi-3.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lexisnexisapi",
-    version='3.0',
+    version='3.0.1',
     license='MIT',
     author="Robert Cuffney",
     author_email='robert.cuffney@lexisnexis.com',
     description = 'a module to support the lexisnexis metabase search api',
     long_description = ' module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `lexisnexisapi-3.0/src/lexisnexisapi/credentials.py` & `lexisnexisapi-3.0.1/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0/src/lexisnexisapi/metabase.py` & `lexisnexisapi-3.0.1/src/lexisnexisapi/metabase.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,116 +16,114 @@
 #url = 'http://metabase.moreover.com/api/v10/searchArticles?'
 
 METABASE_SEARCH_URL = 'http://metabase.moreover.com/api/v10/searchArticles?'
 METABASE_RATE_CHECK_URL = 'https://metabase.moreover.com/api/v10/rateLimits?key='
 
 ##Function names should be lowercase, with words separated by underscores as necessary to improve readability.
 ##Class names should normally use the CapWords convention.  CapitalizedWords 
+
+
 class Search:
     '''
     mbSearch class
     returns API response as a python class
     accepts either a string query, or a dictionary of all metabase parameters
     full_dataset = True -- activates the option to create a full dataset of total results 
     '''
+    @error_handler
     def __init__(self,  full_dataset = False,**kwargs):
-        try:
-            self.parameters = self.set_parameters(kwargs)
-            if full_dataset:
-                data = self.get_fulldataset()
-                print(data['totalResults'])
-            else:
-                data = http_request(self.parameters)
-            if type(data)==dict:
-                self.__dict__.update(data)
-            else:
-                print("Something went wrong, No data was returned")
-        except Exception as e:
-            print(f"Error occurred: {e}")
+        self.parameters = self.set_parameters(kwargs)
+        if full_dataset:
+            data = self.get_fulldataset()
+            print(data['totalResults'])
+        else:
+            data = http_request(self.parameters)
+        if type(data)==dict:
+            self.__dict__.update(data)
+        else:
+            print("Something went wrong, No data was returned")
+
+    @error_handler
     def set_parameters(self,p):
-        try:
-            p.setdefault('key', cred.get_Key("Metabase_Search_Key"))
-            p.setdefault('limit','10000')
-            p['format']='json'
-            return p
-        except Exception as e:
-            print(f"Error occurred: {e}")
+        p.setdefault('key', cred.get_Key("Metabase_Search_Key"))
+        p.setdefault('limit','10000')
+        p['format']='json'
+        return p
+
+    @error_handler   
     def articles_dataframe(self,*args):
         '''
         returns a data frame of the articles
         optional parameter fields, is a list of desired fields to return
         '''
-        try:
-            df = pd.DataFrame.from_records(self.articles)
-            ## Filter dataframe, if *args are provided
-            if args:
-                series = list(args)
-                df = df[series]
-            return df
-        except Exception as e:
-            print(f"Error occurred: {e}")
+        df = pd.DataFrame.from_records(self.articles)
+        ## Filter dataframe, if *args are provided
+        if args:
+            series = list(args)
+            df = df[series]
+        return df
+    
+    @error_handler 
     def create_file(self,file='articles.json'):
         '''
         creates a json file
         '''
-        try:
-            if self.totalResults != 0:
-                with open(file, "w") as my_file:
-                    my_file.write(json.dumps(self.articles, indent=4))
-                    print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
-            else:
-                print("no articles to write to file!") 
-        except Exception as e:
-            print(f"Error occurred: {e}")
+        if self.totalResults != 0:
+            with open(file, "w") as my_file:
+                my_file.write(json.dumps(self.articles, indent=4))
+                print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
+        else:
+            print("no articles to write to file!") =
 
 #### Below Functions, within this class, used only for FullDataSet
+    @error_handler 
     def get_fulldataset(self):
         self.parameters.pop('sequence_id',"")                 #get rid of 'sequence_id' if it's there
         #self.parameters['limit']='1000'                       #This will set the limit to the maximum allowed per their key  
         t_lst =[]                                             #this will be the list of all articles
         x=1                                                   #this will represent the number of articles left
-        try:
-            i=1                                               #i counts the number of loops occurring
-            mc = Streamline(self.parameters['key'])
-            while x > 0:                                      #run while x (number of articles remaining)
-                #self.set_calls()                               #use set_calls object to determine calls left in minute
-                mc.track_calls()
-                myData = http_request(self.parameters)             #call API
-                t_lst = t_lst + myData['articles']            #add articles to t_lst  
-                s_id = myData['articles'][-1]['sequenceId']   #find the last sequence id available
-                self.parameters['sequence_id'] = s_id         #set sequence within parameters for next API call
-                t = myData['totalResults']
-                print(f'\rRemaining Results: {t} / sequence_id: {s_id} / number: {i}', end ="              ")   # print progress
-                x = int(myData['totalResults'])-len(myData['articles'])  #update number of articles left to pull
-                i += 1
-            #End of 'while' loop   
-            print("all done")                                 #print to notify user of completion  
-            #total = len(t_lst)                               #total of all articles pulled, should equal original 'totalResults'
-            myData['articles']= t_lst                         #set the total list of articles as the value in the key 'articles'
-            myData['totalResults']= len(t_lst)                #make sure the 'totalResults' key is set to the original 'totalResults'
-            return myData
-        #error handling:
-        except Exception as e:
-            print(f"Error occurred: {e}")
+
+        i=1                                               #i counts the number of loops occurring
+        mc = Streamline(self.parameters['key'])
+        while x > 0:                                      #run while x (number of articles remaining)
+            #self.set_calls()                               #use set_calls object to determine calls left in minute
+            mc.track_calls()
+            myData = http_request(self.parameters)             #call API
+            t_lst = t_lst + myData['articles']            #add articles to t_lst  
+            s_id = myData['articles'][-1]['sequenceId']   #find the last sequence id available
+            self.parameters['sequence_id'] = s_id         #set sequence within parameters for next API call
+            t = myData['totalResults']
+            print(f'\rRemaining Results: {t} / sequence_id: {s_id} / number: {i}', end ="              ")   # print progress
+            x = int(myData['totalResults'])-len(myData['articles'])  #update number of articles left to pull
+            i += 1
+        #End of 'while' loop   
+        print("all done")                                 #print to notify user of completion  
+        #total = len(t_lst)                               #total of all articles pulled, should equal original 'totalResults'
+        myData['articles']= t_lst                         #set the total list of articles as the value in the key 'articles'
+        myData['totalResults']= len(t_lst)                #make sure the 'totalResults' key is set to the original 'totalResults'
+        return myData
 
 class Streamline:
     '''
     This is a class object to maximize metabase search calls without going over the
     calls per minute limit.  Class is used as a counter
     Upon instantiation the rate limit API is called. 
     The Streamline object will reset it's calls_remaining to the minute_limit at the beginning of every new minute.
     '''
+    @error_handler
     def __init__(self,key):
         self.key = key
         self.start_minute =  self.get_current_minute()
         lst = rate_check(self.key)
         for l in  lst:
             if l['unit']=='MINUTE':
                 self.minute_limit = int(l['limit'])
         self.calls_remaining = self.minute_limit
+    
+    @error_handler
     def track_calls(self):
         current_minute = self.get_current_minute() 
         same_minute = (self.start_minute==current_minute)
         if same_minute:
             self.calls_remaining -=1
         else:
             self.calls_remaining = self.minute_limit-1
@@ -143,44 +141,56 @@
             current_minute = self.get_current_minute()
         self.start_minute = current_minute
         self.calls_remaining= self.minute_limit -1
     def get_current_minute(self):
         return datetime.now().minute
         
     
+def error_handler(func):
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            print(f"Error occurred in function: '{func.__name__}'")
+            print("error: {e}")
+            print(f"args:{args}")
+            print(f"kwargs:{kwargs}")
+            raise  # Re-raise the exception to propagate it further
+    return wrapper
+
+@error_handler
 def http_request(p):
-    try:
-        url = METABASE_SEARCH_URL 
-        r = requests.get(url, params=p) 
-        data = r.__dict__.copy()
-        data.pop('_content', None)
-        data.update(r.json())
-        if r.status_code != 200:
-            print(r.text)
-            print('An error occurred while attempting to retrieve data from the API.')   
-        return data
-    except Exception as e:
-        print(f"Error occurred: {e}")
+    url = METABASE_SEARCH_URL 
+    r = requests.get(url, params=p) 
+    data = r.__dict__.copy()
+    data.pop('_content', None)
+    data.update(r.json())
+    if r.status_code != 200:
+        print(r.text)
+        print('An error occurred while attempting to retrieve data from the API.')   
+    return data
+
+
+@error_handler
 def rate_check(key):
     '''
     Calls the Metabase rate limit API and returns the results as a list of dictionaries
     '''
-    try:
-        if not key:
-            key = cred.get_Key('Metabase_Search_Key')
-        rateCheckUrl = METABASE_RATE_CHECK_URL + key
-        r = requests.get(rateCheckUrl)
-        if r.status_code == 200:
-            data = r.json()
-        return data['rateLimits']
-    except Exception as e:
-        print(f"Error occurred: {e}")
-        
-def set_Metabase_Search_Key(v):
+    if not key:
+        key = cred.get_Key('Metabase_Search_Key')
+    rateCheckUrl = METABASE_RATE_CHECK_URL + key
+    r = requests.get(rateCheckUrl)
+    if r.status_code == 200:
+        data = r.json()
+    return data['rateLimits']
+
+    
+def set_metabase_search_key(v):
     cred.set_Key(Metabase_Search_Key=v)
+
 def get_time():
     '''
     returns the current minute
     '''
     return datetime.now().minute 
 class Article:
     '''
@@ -192,47 +202,45 @@
     def __init__(self, myArticle):
         '''
         Takes each key from the article dictionary and sets it as an attribute of the class
         '''
         self.__dict__.update(myArticle)
 
     
+@error_handler
 def indexTerms(obj,*args):
     '''
     returns a dataframe of index terms
     accepts either an instance of Search, or an instance of Article.
     if Search is sent, df return is an aggregate count of the terms
     if Article is sent, df return is a dataframe of all index terms
     '''
-    try:
-        if isinstance(obj, Search):
-            if obj.articles:
-                df=  pd.concat(
-                    [
-                        pd.DataFrame.from_dict(article["indexTerms"], orient="columns")
-                        for article in obj.articles
-                    ]
-                )
-                df['count'] = df.groupby(['name'])['domains'].transform('count')
-                df= df.drop(columns=['score','code'])
-                df = df.dropna()
-                df = df.drop_duplicates(['name'])
-                df = df.sort_values('count', ascending=False)
-            else:
-                print("no indexTerms to show!")
-        if isinstance(obj, Article):
-            indexterms_lst = obj.indexTerms
-            for x in indexterms_lst:
-                if not 'domains' in x:
-                    x.remove(x)
-            df = pd.DataFrame.from_records(indexterms_lst)
-        ## Filter dataframe, if *args are provided
-        if args:
-            lst =[x.upper() for x in args]
-            df["INCLUDE"] = df["domains"].apply(lambda v: len(list(set(v).intersection(lst)) )!=0 )
-            df =  df[df['INCLUDE']].reset_index(drop=True)
-            del df['INCLUDE']
-            df
-        return df
-    except Exception as e:
-        print(f"Error occurred: {e}")
-  
+    if isinstance(obj, Search):
+        if obj.articles:
+            df=  pd.concat(
+                [
+                    pd.DataFrame.from_dict(article["indexTerms"], orient="columns")
+                    for article in obj.articles
+                ]
+            )
+            df['count'] = df.groupby(['name'])['domains'].transform('count')
+            df= df.drop(columns=['score','code'])
+            df = df.dropna()
+            df = df.drop_duplicates(['name'])
+            df = df.sort_values('count', ascending=False)
+        else:
+            print("no indexTerms to show!")
+    if isinstance(obj, Article):
+        indexterms_lst = obj.indexTerms
+        for x in indexterms_lst:
+            if not 'domains' in x:
+                x.remove(x)
+        df = pd.DataFrame.from_records(indexterms_lst)
+    ## Filter dataframe, if *args are provided
+    if args:
+        lst =[x.upper() for x in args]
+        df["INCLUDE"] = df["domains"].apply(lambda v: len(list(set(v).intersection(lst)) )!=0 )
+        df =  df[df['INCLUDE']].reset_index(drop=True)
+        del df['INCLUDE']
+        df
+    return df
+
```

### Comparing `lexisnexisapi-3.0/src/lexisnexisapi.egg-info/PKG-INFO` & `lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 3.0
+Version: 3.0.1
 Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

