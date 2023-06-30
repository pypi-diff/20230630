# Comparing `tmp/pybrick-0.2.93-py3-none-any.whl.zip` & `tmp/pybrick-0.2.94-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6391 bytes, number of entries: 7
+Zip file size: 6380 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
 -rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-29 01:19 pybrick/ptest.csv
--rw-rw-rw-  2.0 fat    14560 b- defN 23-Jun-30 17:31 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-30 17:32 pybrick-0.2.93.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 17:32 pybrick-0.2.93.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 17:32 pybrick-0.2.93.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      521 b- defN 23-Jun-30 17:32 pybrick-0.2.93.dist-info/RECORD
-7 files, 15591 bytes uncompressed, 5465 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat    14527 b- defN 23-Jun-30 17:41 pybrick/pybrick.py
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      521 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/RECORD
+7 files, 15558 bytes uncompressed, 5454 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pybrick/ptest.csv
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.93.dist-info/METADATA
+Filename: pybrick-0.2.94.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.93.dist-info/WHEEL
+Filename: pybrick-0.2.94.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.93.dist-info/top_level.txt
+Filename: pybrick-0.2.94.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.93.dist-info/RECORD
+Filename: pybrick-0.2.94.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/pybrick.py

```diff
@@ -111,15 +111,15 @@
         """ """
         self._checkConnection()
         return self.engine
     
     def getConnection(self):
         """ """
         if not self.host:
-            raise RuntimeError("Failed to reach",self.host)
+            raise RuntimeError(f"Failed to reach {self.orig_host}")
         
         psql_vinfo=tuple([int(x) for x in self.psql_compatible_version.split(".")])
         PGDialect._get_server_version_info = lambda *args:psql_vinfo
         
         connection_url = sa.engine.URL.create(
             drivername="postgresql+psycopg2",
             username=self.user,
@@ -128,16 +128,16 @@
             database=self.db,
         )
         
         try:
             self.engine=sa.create_engine(connection_url,pool_pre_ping=True)
             conn=self.engine.connect().execution_options(isolation_level="AUTOCOMMIT")
             return conn
-        except Exception as details:
-            raise RuntimeError("Error connecting using:",(self.host,self.db,self.user,self.pw))
+        except Exception as e:
+            raise RuntimeError("Error connecting to Yellowbrick:\n{e}")
     
     
     def disconnect(self):
         """ """
         if self.connection:
             self.connection.close()
         return
@@ -174,16 +174,16 @@
         #Connect and execute, with or without returning results.  If there's a problem
         #print the details, and always close the connection.
         try:
             if withData:
                 df=pd.read_sql(sa.text(query_to_run),self.getEngine())
             else:
                 self.connection.execute(sa.text(query_to_run))
-        except Exception as d:
-            raise RuntimeError("There was an error while executing the SQL:\n",d)
+        except Exception as e:
+            raise RuntimeError("There was an error while executing the SQL:\n{e}")
         
         return df
     
     def tableExists(self,table):
         """ """
         (db,tbl)=table.split(".")
         q=f"""
@@ -312,16 +312,16 @@
                  '--table',target,
                  dump
             ]
             vprint(f"Running this now ===> {' '.join(cmd)}")
             
             try:
                 res=subprocess.run(cmd,capture_output=True,check=True)
-            except Exception as details:
-                raise RuntimeError(f"There was a problem running ybload.  Make sure it's installed, is on your PATH, and that Java is installed:\n{details}")
+            except Exception as e:
+                raise RuntimeError(f"There was a problem running ybload.  Make sure it's installed, is on your PATH, and that Java is installed:\n{e}")
             
             lrows = self.tableRowCount(target)
             if len(src)==lrows or clobber==False:
                 print("YBload successful")
                 vprint(f"Dumped {len(src)} rows, and then loaded {lrows} rows.")
             else:
                 print("WARNING: The number of rows in {target} doesn't match the size of {src}.")
```

