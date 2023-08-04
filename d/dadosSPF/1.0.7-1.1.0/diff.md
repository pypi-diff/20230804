# Comparing `tmp/dadosSPF-1.0.7.tar.gz` & `tmp/dadosSPF-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.7.tar", last modified: Wed Jul 12 18:42:28 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.1.0.tar", last modified: Fri Aug  4 19:26:18 2023, max compression
```

## Comparing `dadosSPF-1.0.7.tar` & `dadosSPF-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      773 2023-07-11 22:32:57.000000 dadosSPF-1.0.7/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.7/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    41131 2023-07-12 18:42:00.000000 dadosSPF-1.0.7/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF.egg-info/
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:20.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        8 2023-07-12 17:57:17.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      548 2023-07-12 18:42:09.000000 dadosSPF-1.0.7/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-08-04 19:26:18.000000 dadosSPF-1.1.0/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-08-04 19:26:18.000000 dadosSPF-1.1.0/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      773 2023-07-11 22:32:57.000000 dadosSPF-1.1.0/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-08-04 19:26:17.000000 dadosSPF-1.1.0/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.1.0/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    55681 2023-08-04 19:23:22.000000 dadosSPF-1.1.0/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-08-04 19:26:17.000000 dadosSPF-1.1.0/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-08-04 19:26:18.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-08-04 19:24:41.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        8 2023-07-12 17:57:17.000000 dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-08-04 19:26:16.000000 dadosSPF-1.1.0/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-08-04 19:26:16.000000 dadosSPF-1.1.0/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-08-04 19:26:16.000000 dadosSPF-1.1.0/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-08-04 19:26:16.000000 dadosSPF-1.1.0/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-08-04 19:26:16.000000 dadosSPF-1.1.0/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-08-04 19:26:18.000000 dadosSPF-1.1.0/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      548 2023-08-04 19:25:12.000000 dadosSPF-1.1.0/setup.py
```

### Comparing `dadosSPF-1.0.7/PKG-INFO` & `dadosSPF-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.7
+Version: 1.1.0
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.7/README.md` & `dadosSPF-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.7/dadosSPF/dadosSPF.py` & `dadosSPF-1.1.0/dadosSPF/dadosSPF.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 __author__ =     "CARLOS PIVETA"
-__collaborators__ = "CARLOS PIVETA"
+__collaborators__ = "CARLOS PIVETA, LEONARDO BOTELHO"
 __license__ =    "DADOS"
-__version__ =    "1.0.7"
+__version__ =    "1.1.0"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
+import time
 import shutil
 import zipfile
 import logging
 import warnings
 import holidays
 import pandas as pd
 from unidecode import unidecode
+from pyspark import HiveContext
 from impala.dbapi import connect
 from impala.util import as_pandas
 from pyspark.sql import SQLContext
 from pyspark.sql import SparkSession
-from pyspark.sql.types import StringType
+from pyspark.sql.functions import col, lit
 from datetime import date,datetime,timedelta
 from pyspark.sql import Row, functions as spf
 from dateutil.relativedelta import relativedelta
+from pyspark.sql.types import IntegerType, StringType, StructType, StructField
 warnings.filterwarnings("ignore")
 
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS CONN
 # -------------------------------------------------------------------------------------------------------------------------------
 class conn():   
     
@@ -57,14 +60,27 @@
                     self.pswd = None
                     self.environment = 'DEV'
                     print('Criar variaveis de ambiente !!!!')
             else:
                 self.sandbox = None
                 self.pswd = None
                 self.environment = 'PROD'
+        
+        strPasta="./";
+        strfile = '/app/mount/'+strPasta;
+        self.qtEtapas = 0;
+        if os.path.exists(strfile):
+            path = strfile;
+        else:
+            path = strPasta;
+        try:
+            with open(path+"CONTROLE.txt", 'r') as f:
+                self.dbControle = f.readline().strip();
+        except:
+            self.dbControle = self.sandbox;
                 
         #conexções
         self.spark = None
         self.impala = None
         self.hive = None
         self.tpConn = None
         
@@ -190,14 +206,17 @@
         Função de conexão para consulta/execução de comandos SQL via Impala        
         Parameters
         ----------
         dPrint : bool (optional)
             Define se será impresso a menssagem de retorno
             
         """
+        if self.impala != None:
+            if self.impala.ping == False:
+                self.impala = None
         if self.impala == None:
             try:
                 IMPALA_HOST='coordinator-impala-users-prod-1.env-8gtbx9.dw.lg50-5lsa.cloudera.site'
                 IMPALA_PORT='443'
                 impala_conn = connect(host=IMPALA_HOST,
                                port=IMPALA_PORT,
                                auth_mechanism='LDAP',
@@ -351,15 +370,42 @@
                     return df
                 except Exception as e:
                     df = self.tpConn.sql('select * from {}.{} {}'.format(strSchema,strTable,strLimit))
                     return df
         except Exception as e:
             if dPrint == True: print('Tabela {} não possui partição'.format(strTable))
             print(e)
-            
+    def getMaxPartitionTable(self,strSchema=None,strTable="",strPartition="dt_ingest"):
+        """
+        [dtPartition] = getMaxPartitionTable(strSchema = 'abc',strTable ='tabela',strPartition='dt_ingest')
+        Função para pegar a maior partição
+        Parameters
+        ----------
+        strSchema: str
+            Nome do database aonde a tabela esta localizada
+        strTable : str
+            Nome da tabela a ser deletada do ambiente sandbox
+        strPartition : str
+            Nome da partição
+        Returns Valor da partição com maior valor    
+        """;
+        if((strSchema is None)|(strSchema=="")):
+            strTableName = strTable if(len(strTable.split("."))>1) else strTable;
+        else:
+            strTableName = strSchema+"."+strTable.split(".")[1] if(len(strTable.split("."))>1) else strSchema +"."+ strTable;
+        strNmPartition = strPartition.upper();
+        dfListPartition = self.tpConn.sql("SHOW PARTITIONS {0}".format(strTableName));
+        vMaxPartition = dfListPartition \
+        .withColumn("posPartition",spf.expr(f"instr(upper(partition),'{strNmPartition}')+length('{strNmPartition}')+1")) \
+        .withColumn("vStr",spf.expr(f"substring(partition,posPartition)")) \
+        .withColumn("findP",spf.expr(f"ifnull(nullif(instr(vStr,'/')-1,-1),length(vStr))")) \
+        .withColumn("valuePartition",spf.expr(f"substring(vStr,1,findP)")) \
+        .agg({"valuePartition": "max"}).collect()[0][0];
+        return vMaxPartition;
+    
     def toSandBox(self,strSchema,strTable,ultimaParticao = False,intLimit = None,CampoDocumento = None,tpDocumento = None):
         """
         toSandBox(strSchema = 'abc',strTable = 'tabela',[ultimaParticao = False],[intLimit = 100],[CampoDocumento = None],[tpDocumento = None])
         Função para salvar uma tabela do ambiente produtivo no ambiente sandbox com id unico caso seja necessário
         Parameters
         ----------
         strTable : str
@@ -690,14 +736,29 @@
         df dataframe
             dataframe o qual será convertido
 
         """
         ##Converte todos os campos em String e nome das colunas tudo em CAIXA ALTA
         df = df.select([spf.when(spf.col(x).cast(StringType()).isNull(),spf.lit("")).otherwise(spf.concat(spf.lit('"'),spf.col(x), spf.lit('"')).cast(StringType())).alias(x.upper()) for x in df.columns])
         return df
+    
+    def SaveFileProcess(self,DF_INSERT,pathFile):
+        DF_INSERT\
+         .write\
+         .format("parquet")\
+         .mode("overwrite")\
+         .save(pathFile)
+        print(f"Arquivo salvo em: {pathFile}");
+    
+    def CheckPoint(self,df,table):
+        pathTable = "{0}/temp/{1}/".format(paths3,table)
+        spark.sparkContext.setCheckpointDir(pathTable)
+        df = df.checkpoint()
+        df.createOrReplaceTempView(table)
+        return df
 
     def csvToSandbox(self,pasta = './arquivos/',delimiter = None,header = 'true' ):
         """
         s.csvToSandbox(self,pasta = './arquivos/',delimiter = None,header = 'true' )
         
         Função para carregar arquivos de texte em um dataframe no sandbox
         
@@ -784,57 +845,193 @@
 
                     if resp != []:
                         files = resp
 
             files = sorted(files)
             for fls in range(len(files)):
                 if files[fls].endswith(".txt"):
+                    arquivo = files[fls].replace('.txt','')
+                    print(f'==== Rodando processo {arquivo} ====')
                     proc = files[fls].replace('.txt','')
                     with open(path+r'/'+files[fls], 'r') as file:
                         query = file.read()
-                        try:
-                            query = query.format(**str_where)
-                        except Exception as e:
-                            print(e)
-                        table = files[fls].replace('.txt','')
+                        #query = query.format(**str_where)
                         tmpTxt = query.replace(';','')
-                        arquivo = files[fls].replace('.txt','')
                         tmptables = re.findall(r'FROM(.*?)(\S+)',tmpTxt.upper())
                         tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
                         tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
                         tables = list(set(tmptables))
                         tmpTxt = None
 
-                for tt in range(len(tables)):
-                    if tables[tt][1].replace('(','').replace(')','') == '':
-                        pass
-                    else:
-                        schema = tables[tt][1].lower().split('.')[0]
-                        tabela = tables[tt][1].lower().split('.')[1]
-                        self.getSpark()
-                        lp = self.getLastPartition(schema,tabela,dPrint = False)
-                        if lp != None:
-                            str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
-
-                executionPlan = query.format(**str_where).split(';')
-
-                impala = self.getImpala()
-                for i in range(len(executionPlan)):
-                    try:
-                        val = executionPlan[i].replace('\n',' ')
-                        print(f'Executando : {val}')
-                        impala.execute(executionPlan[i])
-                        print(f'-----FINALIZADO -----')
-                    except Exception as e:
-                        print(f'-----!!! ERRO !!!-----')
-                        print(e)   
-                        pass
+                    for tt in range(len(tables)):
+                        if tables[tt][1].replace('(','').replace(')','') == '':
+                            pass
+                        else:
+                            schema = tables[tt][1].lower().split('.')[0]
+                            tabela = tables[tt][1].lower().split('.')[1]
+                            s.getSpark()
+                            print(schema,tabela)
+                            lp = s.getLastPartition(schema,tabela, dPrint=False)
+                            if lp != None:
+                                str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
 
+                    executionPlan = query.format(**str_where).split(';')
+
+                    impala = s.getImpala()
+                    for i in range(len(executionPlan)):
+                        try:
+                            val = executionPlan[i].replace('\n',' ')
+                            print(f'Executando : {val}')
+                            impala.execute(executionPlan[i])
+                            print(f'-----FINALIZADO -----')
+                        except Exception as e:
+                            print(f'-----!!! ERRO !!!-----')
+                            print(e)   
+                            pass
         except Exception as e:
             print(e)
+
+    def switchDB(self,vQuery,dbTo):
+        newDB = dbTo;
+        if(self.dbControle=="SYS_DB"):
+            newDB = "SYS_" + dbTo.replace("_produtivo","").replace("_PRODUTIVO","");
+        if(self.dbControle.lower()==self.sandbox):
+            newDB = self.dbControle;
+        vQuery = vQuery.replace(dbTo,newDB);
+            
+        return vQuery;
+    
+    def switchListTable(self,vQuery,vTabelas):
+        list_tables = vTabelas.upper().split(",");
+            
+        for tb in list_tables:
+            nmTb = tb.split(".")[1]
+            dbTable=self.switchDB(tb.split(".")[0],tb.split(".")[0]);
+            tbName = dbTable+"."+tb.split(".")[1];
+            vQuery = vQuery.replace(tb.lower(),tbName.lower());  
+            vQuery = vQuery.replace(tb,tbName);
+        return vQuery;
+    
+    def getTimeSrv(self):
+        return self.tpConn.sql("SELECT current_timestamp() - interval 3 hours as dt_processamento").collect()[0][0];
+
+    def runProcesso(self,vArquivo):
+        vDtProcessamento = datetime.strftime(self.getTimeSrv(), '%d/%m/%Y %H:%M:%S')
+        S3_TIMESTAMP = vDtProcessamento
+        self.qtEtapas  = self.qtEtapas+1;
+        dsEtapa = f'\nEtapa {self.qtEtapas}({vArquivo}): {S3_TIMESTAMP} \n'
+        print(dsEtapa)
+        arquivoPy = __import__(vArquivo);
+
+    def runPy(self,vPrint,vArquivo):
+        if(vPrint==1):
+            print(vArquivo);
+        else:
+            self.runProcesso(vArquivo);
+            
+    def orquestradorFiles(self,vPasta,vNmProcesso,vOrdemAvulso=0,vPrintOnly=1):
+        """
+        Executa todos os arquivos de 1 pasta em ordem crescente.
+        Os arquivos dentro da pasta devem seguir o seguinte formato: XXX_NOME_ARQUIVO
+        XXX = Deve ser numerico de 000 à 999.
+        
+        vPasta = Subpasta onde estão localizados os scripts .py
+        vNmProcesso = Nome do Processo(necessário para execuções Avulsas, selecionar apenas alguns arquivos para execução)
+        vOrdemAvulso = Valor que representa a sequência de arquivos à ser executada
+        vPrintOnly = 1 (Apenas printar os arquivos do path). 0 (Executa os scrtips)
+        ----------
+        """
+        strPasta=vPasta;
+        strfile = '/app/mount/'+strPasta;
+        if os.path.exists(strfile):
+            path = strfile;
+        else:
+            path = strPasta;
+
+        arquivosPy ="";
+        print(f"\nArquivos listdir:{path} \n")
+        files = os.listdir(path)
+        files.sort();
+
+        for arq in files:
+            if ((arq[-3:].lower() == '.py')):
+                filePy = "".join([strPasta,".",arq.replace(".py","")]);
+                arquivosPy = arquivosPy+","+filePy;
+                ordem = str(int(filePy.split(".")[1].split("_")[0]));
+        arquivosPy = arquivosPy[1:];
+        print(arquivosPy);
+
+        dfConfigJob = self.tpConn.sql(f"""
+        select arquivo
+        from sandbox_crm.config_processos_crm
+        where PROCESSO ='{vNmProcesso}'
+        AND dt_processamento = current_date()
+        """);
+        dfConfigJob = dfConfigJob.dropDuplicates();
+        
+        listJobs = [row.arquivo for row in dfConfigJob.collect()];
+        my_data =arquivosPy.split(",");
+        R = Row('filename',"ordem");
+        printOnly = vPrintOnly;
+        print("\nJobs Avulsos:",listJobs);
+        DF_FILES = self.spark.createDataFrame([R(x,int(str(x.split(".")[1].split("_")[0]))) for  x in (my_data)]);
+        for arquivo in DF_FILES.sort(col("ordem")).collect():
+            arquivoPy = arquivo.filename.split(".")[1];
+            try:
+                jobAvulso = [jobFind for i, jobFind in enumerate(listJobs) if jobFind == arquivoPy];
+            except:
+                jobAvulso = "";
+            if((len(listJobs)>0)&(len(jobAvulso)>0)&(arquivo.ordem>=0)):
+                self.runPy(printOnly,arquivo.filename);
+            else:
+                if((arquivo.ordem>=vOrdemAvulso)&(len(listJobs)==0)):
+                    self.runPy(printOnly,arquivo.filename);
+    
+    def finLastFileElegiveis(self,strEtapa,strPasta,strPath):
+        arquivoAnterior = "".join(["0",str(int(strEtapa)-1)])[-2:];
+        
+        EtapaManual = self.spark.sql(f"""
+        select 
+          coalesce(max(b.nu_etapa),max(a.nu_etapa),'0') as ETAPA
+        from sandbox_crm.config_job_nbo  a
+        left join sandbox_crm.config_job_nbo b
+        on (a.dt_processamento = b.dt_processamento and b.nu_etapa < '{strEtapa}')
+        where (a.dt_processamento = current_date()
+        AND a.nm_arquivo not like '%NBO_ELEGIVEIS_FINAL')
+        """).collect()[0][0];
+        
+        strfile = '/app/mount/'+strPasta;
+
+        if os.path.exists(strfile):
+            path = strfile;
+        else:
+            path = strPasta;
+
+        files = os.listdir(path)
+        files.sort();
+
+        arquivosPy="";
+        for arq in files:
+            if ((arq[-3:].lower() == '.py')):
+                filePy = "".join([strPasta,".",arq.replace(".py","")]);
+                if((filePy.split(".")[1].split("_")[1].upper()=="NBO") & (filePy.split(".")[1].split("_")[2].upper()=="ELEGIVEIS") &(filePy.split(".")[1].split("_")[0]!="99")):
+                    ultEtapa = str(filePy.split(".")[1].split("_")[0]);
+
+        pathFile = "{0}/parquet_tmp/{1}/".format(strPath,ultEtapa);
+        pathAnterior = "{0}/parquet_tmp/{1}/".format(strPath,arquivoAnterior);
+
+        if(EtapaManual>=strEtapa):
+            pathElegiveis = pathFile;
+            print(f"\nLoad manual, arquivo da etapa {ultEtapa}!!!");
+        elif(int(EtapaManual)>0):
+            pathElegiveis = "{0}/parquet_tmp/{1}/".format(strPath,EtapaManual);
+        else:
+            pathElegiveis = pathAnterior;
+        print(f"\nLoad Path:{pathElegiveis}");
+        return pathElegiveis;
             
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS TOOLS
 # -------------------------------------------------------------------------------------------------------------------------------
 
 class tool():
     """
@@ -987,14 +1184,169 @@
             pasta = pasta + '/'
         try:
             with zipfile.ZipFile(arquivo,"r") as zip_ref:
                 zip_ref.extractall(pasta)
         except Exception as e:
             print('ERRO! AO EXTRAIR O ARQUIVO')
             print(e)
+            
+class DtIngestValidation(object):    
+
+    def __init__(self, sql_context):
+        self.db_name = ""
+        self.table_name = ""
+        self.sqlc = sql_context
+        self._current_date = datetime.now().date()
+
+    def get_dt_ingest(self):
+        max_dt_ingest=self.sqlc.sql(f"SHOW PARTITIONS {self.db_name}.{self.table_name}").collect()
+        last_partition = max_dt_ingest[len(max_dt_ingest)-1]["partition"][10:20]
+
+        return last_partition
+    
+    def is_dt_ingest_valid(self):      
+        date_var = datetime.strptime(self.get_dt_ingest(),'%Y-%m-%d').date()
+
+        print('INFO: current_date {0}'.format(self._current_date))
+        print(f'INFO: last dt_ingest from {self.db_name}.{self.table_name}: {date_var}')
+
+        if (self._current_date > date_var):
+            return False
+        
+        return True 
     
-                                
+    def check_ingest(self, db_name, table_name):
+
+        self.db_name = db_name
+        self.table_name = table_name
+        attempts = 1
+        success = False
+        time_count = 1800
+
+        while((attempts <= 4) & (success == False)):
+            if attempts == 4:
+                print(f"ERROR: Não foi possível realizar a operação devido a falta de ingestão na tabela {self.db_name}.{self.table_name}")
+
+                raise Exception
+            
+            print(f"INFO: Tentativa de execução {attempts}")
+
+            try:                
+                isValid = self.is_dt_ingest_valid()
+
+                if(isValid):
+                    print("INFO: A ingestão foi realizada hoje!")
+
+                    success = True
+                    break
+                else:
+                    print("INFO: A ingestão ainda não ocorreu")
+
+                    success = False
+                    attempts = attempts + 1
+                    time.sleep(time_count)
+
+            except:
+                print('ERROR: Falha na verificação da ingestão. Uma nova tentativa será feita!')
+                attempts = attempts + 1
+                time.sleep(time_count);
+
+    def ckpLay1(self,dfCkp,pathSave,tbFile=None, tbFileWhere=None,data_ref=datetime.today().date().strftime("%Y-%m-%d")):
+
+        # verificar se ja existe o campo COD_CRM, se nao existir precisa adicionar o UUID
+        if "cod_crm" not in list(map(lambda x: x.lower(),dfCkp.columns)):
+            # GERAR UUID
+            unique_id_column = "unique_id_to_merge"
+
+            all_uuids = [(str(uuid.uuid4()),) for x in range(0,dfCkp.count())]
+            df_tmp_uuids = self.spark.createDataFrame(all_uuids, ['COD_CRM'])
+
+            # monotonically_increasing_id nao esta gerando ids consecutivos.
+            df_tmp_uuids = df_tmp_uuids.withColumn(unique_id_column, F.monotonically_increasing_id())
+
+            dfCkp_with_id = dfCkp.withColumn(unique_id_column, F.monotonically_increasing_id())
+
+            windowSpec = W.orderBy(unique_id_column)
+            dfCkp_with_id = dfCkp_with_id.withColumn(unique_id_column, F.row_number().over(windowSpec))
+            df_tmp_uuids = df_tmp_uuids.withColumn(unique_id_column, F.row_number().over(windowSpec))
+            final_df = dfCkp_with_id.join(df_tmp_uuids, dfCkp_with_id[unique_id_column] == df_tmp_uuids[unique_id_column]).\
+                         drop(unique_id_column)
+        else: 
+            final_df = dfCkp;
+
+
+        first_row=data_ref[8:]+data_ref[5:7]+data_ref[:4]+"|1"
+        print(f"primeira linha gerada - data\n")
+        print(first_row)
+
+        final_df_columns_list = final_df.columns
+        second_row = "|".join(final_df_columns_list)
+        print(f"segunda linha gerada - colunas:\n")
+        print(second_row)
+
+        # third_row_dfTb = DataFrame para salvar dados em tabelas Hive(Não pode fazer o tratamento do [n]
+        third_row_dfTb = final_df.withColumn("ARQ_VALUES", spf.concat_ws("|",*final_df_columns_list));
+        third_row_df = final_df.withColumn("A", spf.concat_ws("|",*final_df_columns_list));
+        third_row_df = third_row_df.withColumn("ExpCkpValues",spf.expr("""replace(A,'[n]',concat(decode(unhex(hex(92)), 'US-ASCII'),'n'))"""));
+        third_row = list(zip(third_row_df.select("ExpCkpValues").rdd.flatMap(lambda x: x).collect())); 
+
+
+
+        # verificar se existe condicao - tbFileWhere
+        if tbFileWhere is not None and tbFileWhere!="":
+            print(f"condicao tbFileWhere: {tbFileWhere}")
+            third_row_df = third_row_df.where(tbFileWhere);
+            third_row_dfTb= third_row_dfTb.where(tbFileWhere);
+        third_row = list(zip(third_row_df.select("ExpCkpValues").rdd.flatMap(lambda x: x).collect()));
+        third_row_dfTb = list(zip(third_row_dfTb.select("ARQ_VALUES").rdd.flatMap(lambda x: x).collect()));
+        print(f"terceira (ate n) linha gerada:\n")
+        print(third_row[-5:])
+
+        last_row = third_row_df.count()
+        last_row = str(last_row)
+        print(f"ultima linha gerada:{last_row}")
+
+        # Salvar resultado com o nome especificado na variavel tbFile
+        spark_log_table_columns = StructType([
+        StructField("A",StringType(),True)])
+
+        spark_row = [
+            tuple([first_row]),
+            tuple([second_row]),
+            *third_row,
+            tuple([last_row])];
+
+        spark_rowTb = [
+            tuple([first_row]),
+            tuple([second_row]),
+            *third_row_dfTb,
+            tuple([last_row])];
+
+        arqCkp = self.spark.createDataFrame(spark_row, spark_log_table_columns);
+        print(f"generating {tbFile}");
+
+        arqCkp.coalesce(1) \
+        .write\
+        .format("csv") \
+        .option("header", "false") \
+        .option("encoding", "cp1252") \
+        .option("escapeQuotes","false") \
+        .option("quoteAll","false") \
+        .option("escape","") \
+        .option("quote", "\u0000") \
+        .mode("overwrite") \
+        .save(pathSave)
+
+        print("\nArquivo salvo com sucesso em: {}".format(pathSave));
+        
+        if((tbFile is not None ) & (tbFile !="")):
+            try:
+                arqCkpTb = self.spark.createDataFrame(spark_rowTb, spark_log_table_columns);
+                arqCkpTb.write.format('hive').mode('overwrite').saveAsTable(tbFile);
+                print(f"\nPúblico salvo na tabela [{tbFile}]");
+            except:
+                print(f"\nErro ao salvar tabela [{tbFile}]");
 # -------------------------------------------------------------------------------------------------------------------------------
 # | EASY IMPORTS
 # -------------------------------------------------------------------------------------------------------------------------------                                
 sqlConn =  conn()
 tools = tool()
```

### Comparing `dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `dadosSPF-1.1.0/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.7
+Version: 1.1.0
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.7/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.1.0/dadosSPF.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.7
+Version: 1.1.0
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.7/dadosSPF.egg-info/SOURCES.txt` & `dadosSPF-1.1.0/dadosSPF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.7/setup.py` & `dadosSPF-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.7',
+    version='1.1.0',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
```

