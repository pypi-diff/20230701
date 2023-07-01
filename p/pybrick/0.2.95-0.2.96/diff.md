# Comparing `tmp/pybrick-0.2.95-py3-none-any.whl.zip` & `tmp/pybrick-0.2.96-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6400 bytes, number of entries: 7
+Zip file size: 6398 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
 -rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-29 01:19 pybrick/ptest.csv
--rw-rw-rw-  2.0 fat    14578 b- defN 23-Jun-30 18:15 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      521 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/RECORD
-7 files, 15609 bytes uncompressed, 5474 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat    14580 b- defN 23-Jul-01 02:11 pybrick/pybrick.py
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      521 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/RECORD
+7 files, 15611 bytes uncompressed, 5472 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pybrick/ptest.csv
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.95.dist-info/METADATA
+Filename: pybrick-0.2.96.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.95.dist-info/WHEEL
+Filename: pybrick-0.2.96.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.95.dist-info/top_level.txt
+Filename: pybrick-0.2.96.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.95.dist-info/RECORD
+Filename: pybrick-0.2.96.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/pybrick.py

```diff
@@ -1,8 +1,8 @@
-__version__="0.2.95"
+__version__="0.2.96"
 __doc__="""
 pybrick uses sqlalchemy to provide a convenient connection to Yellowbrick.
 """
 import pdb
 import os
 import sys
 import subprocess
@@ -131,15 +131,15 @@
         )
         
         try:
             self.engine=sa.create_engine(connection_url,pool_pre_ping=True)
             conn=self.engine.connect().execution_options(isolation_level="AUTOCOMMIT")
             return conn
         except Exception as e:
-            raise RuntimeError("Error connecting to Yellowbrick:\n{e}")
+            raise RuntimeError(f"Error connecting to Yellowbrick:\n{e}")
     
     
     def disconnect(self):
         """ """
         if self.connection:
             self.connection.close()
         return
@@ -177,15 +177,15 @@
         #print the details, and always close the connection.
         try:
             if withData:
                 df=pd.read_sql(sa.text(query_to_run),self.getEngine())
             else:
                 self.connection.execute(sa.text(query_to_run))
         except Exception as e:
-            raise RuntimeError("There was an error while executing the SQL:\n{e}")
+            raise RuntimeError(f"There was an error while executing the SQL:\n{e}")
         
         return df
     
     def tableExists(self,table):
         """ """
         (db,tbl)=table.split(".")
         q=f"""
```

