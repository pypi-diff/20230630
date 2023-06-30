# Comparing `tmp/documentdataextraction-0.0.8-py3-none-any.whl.zip` & `tmp/documentdataextraction-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4950 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    10538 b- defN 22-Jul-19 10:14 documentdataextraction/__init__.py
--rw-rw-rw-  2.0 fat     1073 b- defN 22-Jul-19 11:40 documentdataextraction-0.0.8.dist-info/LICENCE.txt
--rw-rw-rw-  2.0 fat      779 b- defN 22-Jul-19 11:40 documentdataextraction-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-19 11:40 documentdataextraction-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 22-Jul-19 11:40 documentdataextraction-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      556 b- defN 22-Jul-19 11:40 documentdataextraction-0.0.8.dist-info/RECORD
-6 files, 13061 bytes uncompressed, 3928 bytes compressed:  69.9%
+Zip file size: 5006 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    10973 b- defN 22-Nov-22 05:13 documentdataextraction/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Nov-22 06:02 documentdataextraction-0.0.9.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      724 b- defN 22-Nov-22 06:02 documentdataextraction-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Nov-22 06:02 documentdataextraction-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       23 b- defN 22-Nov-22 06:02 documentdataextraction-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      556 b- defN 22-Nov-22 06:02 documentdataextraction-0.0.9.dist-info/RECORD
+6 files, 13441 bytes uncompressed, 3984 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: documentdataextraction/__init__.py
 Comment: 
 
-Filename: documentdataextraction-0.0.8.dist-info/LICENCE.txt
+Filename: documentdataextraction-0.0.9.dist-info/LICENCE.txt
 Comment: 
 
-Filename: documentdataextraction-0.0.8.dist-info/METADATA
+Filename: documentdataextraction-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: documentdataextraction-0.0.8.dist-info/WHEEL
+Filename: documentdataextraction-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: documentdataextraction-0.0.8.dist-info/top_level.txt
+Filename: documentdataextraction-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: documentdataextraction-0.0.8.dist-info/RECORD
+Filename: documentdataextraction-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## documentdataextraction/__init__.py

```diff
@@ -2,74 +2,73 @@
 from pathlib import Path
 # import cv2 as cv
 # import pytesseract as ts
 
 from visitingcard import extract
 import pdfkit
 from flask import request, make_response
-
+import loggerutility as logger
 
 class DataExtractor:
     """
     A resource for extracting invoice data using invoice2data library
     """
 
     def __init__(self):
         self.file_storage_path = os.environ.get('de_storage_path', '/flask_downloads')
-        self.template_folder = os.environ.get('de_templates_path',
-                                              '/DocDataExtraction')  # Changed by Pravin K on 9-JUNE-21 [As per K B sir suggestion changed root folder inv2data_templates to DocDataExtraction ]
+        self.template_folder = os.environ.get('de_templates_path', '/DocDataExtraction') # Changed by Pravin K on 9-JUNE-21 [As per K B sir suggestion changed root folder inv2data_templates to DocDataExtraction ] 
 
     def get(self):
         final_result = {}
 
         try:
             invoice_file_part = request.files.get('file_0', None)
 
             if not invoice_file_part:
                 raise Exception('Invoice file not found in request payload')
 
-            # Added By Prain K on 26-APR-21 START
-            print("inside get", invoice_file_part)
+            #Added By Prain K on 26-APR-21 START
+            logger.log(f"inside get  {invoice_file_part}","0")
             given_temp_path = request.args.get('extract_templ', None)
-            print("inside get:extract_templ:given_temp_path[", given_temp_path, "]")
+            logger.log(f"inside get:extract_templ:given_temp_path[{given_temp_path}]","0")
             if given_temp_path:
-                if given_temp_path != 'DocDataExtraction':  # Changed by Pravin K on 9-JUNE-21 [As per K B sir suggestion changed root folder inv2data_templates to DocDataExtraction ]
-                    self.template_folder = self.template_folder + '/' + given_temp_path + '/'
+                if given_temp_path != 'DocDataExtraction': # Changed by Pravin K on 9-JUNE-21 [As per K B sir suggestion changed root folder inv2data_templates to DocDataExtraction ] 
+                    self.template_folder =  self.template_folder +'/'+given_temp_path+'/'
 
-            print("inside get template_folder[", self.template_folder, "]")
-            # Added By Prain K on 26-APR-21 END
+            logger.log(f"inside get template_folder[{self.template_folder}]","0")
+            #Added By Prain K on 26-APR-21 END
 
             filename = invoice_file_part.filename
             file_path = os.path.join(self.file_storage_path, invoice_file_part.filename)
-            print("inside file_path", file_path)
-
+            logger.log(f"inside file_path  {file_path}","0")
+            
             if '.TXT' in filename or '.txt' in filename or '.PDF' in filename or '.pdf' in filename or '.xls' in filename or '.xlsx' in filename:
                 input_reader = request.args.get('input_reader', 'pdftotext')
 
             if '.png' in filename or '.PNG' in filename or '.jpg' in filename or '.JPG' in filename or '.jpeg' in filename or '.JPEG' in filename:
                 input_reader = request.args.get('input_reader', 'tesseract')
 
-                print("Read::image:", file_path)
-                # custom_oem_psm_config = r' --oem 2, --psm 3 '
-                # print("Read::file_path:",file_path)
+                logger.log(f"Read::image:{file_path}","0")
+                #custom_oem_psm_config = r' --oem 2, --psm 3 '
+                # logger.log("Read::file_path:",file_path)
                 # img = cv.imread(file_path,0)
                 # image_text = ts.image_to_string(img,config = custom_oem_psm_config)
-                # print("Read::image_text:",image_text)
-                print("Read Image  file using tesseract::input_reader:", input_reader)
+                # logger.log("Read::image_text:",image_text)
+                logger.log(f"Read Image  file using tesseract::input_reader:{input_reader}","0")
 
             Path(self.file_storage_path).mkdir(parents=True, exist_ok=True)
-
+            
             invoice_file_part.save(file_path)
 
             if '.TXT' in filename or '.txt' in filename:
-                print("Read Text file")
+                logger.log(f"Read Text file","0")
                 dot_ind = filename.rindex('.')
-                print('dot index' + str(dot_ind))
+                logger.log(f"dot index {str(dot_ind)}","0")
                 only_name = filename[:dot_ind]
-                print('only_name' + only_name)
+                logger.log(f"only_name {only_name}","0")
 
                 html_file_name = self.file_storage_path + "/" + only_name + ".html"
                 output_file_name = self.file_storage_path + "/" + only_name + ".pdf"
                 with open(file_path) as file:
                     with open(html_file_name, "w") as output:
                         file = file.read()
                         file = file.replace("\n", "<br>")
@@ -77,77 +76,80 @@
 
                 pdfkit.from_file(html_file_name, output_file_name)
                 try:
                     os.remove(file_path)
                     file_path = os.path.join(html_file_name)
                     os.remove(file_path)
                 except Exception as ex:
-                    print("DataExtractor: Exception while removing file", ex)
+                    logger.log(f"DataExtractor: Exception while removing file {ex}","0")
 
                 file_path = os.path.join(self.file_storage_path, output_file_name)
             if '.PDF' in filename or '.pdf' in filename and not given_temp_path == 'Visiting_Card':
-                print("Read pdf file")
+                logger.log(f"Read pdf file","0")
                 # Added by Akshay S on 07-MAY-21 [To extract Images inside PDF] START
                 import fitz
                 # from PIL import Image
                 from pdf2image import convert_from_path
                 # import ocrmypdf
                 file_path = os.path.join(self.file_storage_path, invoice_file_part.filename)
                 pdf_file = fitz.open(file_path)
                 for page_index in range(len(pdf_file)):
                     page = pdf_file[page_index]
                     image_list = page.getImageList()
-                print(page.getImageList())
-
-                if image_list:
-                    print(f"[+] Found a total of {len(image_list)} images in page {page_index}")
+                logger.log(f"{page.getImageList()}","0")
+                
+                if image_list: 
+                    logger.log(f"[+] Found a total of {len(image_list)} images in page {page_index}","0")
                     input_reader = request.args.get('input_reader', 'tesseract')
                     new_img_file_path = os.path.join(self.file_storage_path, 'out.jpg')
-                    print("file_path--[" + file_path + "],new_img_file_path[" + new_img_file_path + "]")
+                    logger.log(f"file_path--[{file_path}],new_img_file_path[{new_img_file_path}]","0")
                     images = convert_from_path(file_path, 200)
-
-                    for page in images:
+                 
+                    for page in images: 
                         page.save(new_img_file_path, 'JPEG')
-                    # file_path = new_img_file_path #Changed by Pravin K on 6-june-21
-
+                       #file_path = new_img_file_path #Changed by Pravin K on 6-june-21
+                    
 
                 else:
-                    print("[!] No images found on page", page_index)
-                    # Added by Akshay S on 07-MAY-21 [To extract Images inside PDF] END
+                    logger.log(f"[!] No images found on page {page_index}","0")  
+                # Added by Akshay S on 07-MAY-21 [To extract Images inside PDF] END  
 
             if '.xls' in filename or '.xlsx' in filename:
-                print("Read Excel file")
+                logger.log("Read Excel file","0")
 
             from invoice2data import extract_data
             from invoice2data.extract.loader import read_templates
 
             # Added by Aniket G on 28-JUNE-22 [To extract Data From Visiting card] START
-            print("template_Name [" + given_temp_path + "]")
+            logger.log(f"template_Name [{given_temp_path}]","0")
             if not given_temp_path == 'Visiting_Card':
-                print("Read::self.template_folder:", self.template_folder)
+                logger.log(f"Read::self.template_folder: {self.template_folder}","0")
                 if os.path.exists(self.template_folder):
                     templates = read_templates(self.template_folder)
-                print("Read::self.template_folder:", templates)
+                logger.log(f"Read::self.template_folder: {templates}","0")
                 input_reader_module = self.get_input_reader_module(input_reader)
-                print("input_reader_module :", input_reader_module)
+                logger.log(f"input_reader_module :{input_reader_module}","0")
             # Added by Aniket G END
+            
             # Added by Pravin START
             input_document_type = request.args.get('input_document_type', '')
-            print("input_document_type [" + input_document_type + "]")
+            # -----------------logger syntax error solve kar yaha se ------------
+            logger.log(f"input_document_type [ {input_document_type} ]","0")
             if input_document_type == 'cheque':
                 from proteus_services.resources.read_cheque import ReadCheque
                 read_cheque = ReadCheque()
                 result = read_cheque.read_cheque_details(file_path, templates, input_reader_module)
             # Added by Pravin END
+            
             # Added by Aniket G on 28-JUNE-22 [To extract Data From Visiting card] START
             elif given_temp_path == 'Visiting_Card':
                 result = extract(file_path)
             # Added by Aniket G END
             else:
-                print("extracting data start::", file_path)
+                logger.log(f"extracting data start::{file_path}","0")
                 result = extract_data(invoicefile=file_path,
                                       templates=templates,
                                       input_module=input_reader_module)
                 # Added by SwapnilB [12-07-22] [START] for filterng json of supplier bill 
                 try:
                     if 'customer_name' in result.keys():
                         result['customer_name'] = result['customer_name'].split(':')[1].strip()
@@ -162,43 +164,44 @@
                     if 'Bill_number' in result.keys():
                         result['Bill_number'] = result['Bill_number'].split(' ')[1].strip()
                         
                     if 'Bill_date' in result.keys():
                         result['Bill_date'] = result['Bill_date'].date()
                         
                 except Exception as e:
-                    print("Issue: ", e)
+                    logger.log(f"Issue:::  {e}","0")
                 # Added by SwapnilB [12-07-22] [END] for filterng json of supplier bill 
             try:
                 os.remove(file_path)
             except Exception as ex:
-                print("DataExtractor: Exception while removing file", ex)
-            
+                logger.log(f"DataExtractor: Exception while removing file  {ex}","0")
+
             # Added by Aniket G. Start
-            print('result'+str(result))  
+            logger.log(f"result  {str(result)}" ,"0" )  
             for key, value in result.items():
                 if key == "year_of_birth":
                     if value:
-                        print(value)
+                        logger.log(f"{value}","0")
                         values = "1/1/"+str(value)
                         result["dob"] = values
             
             # Added by Aniket G. END
-            print('result' + str(result))
+
+            logger.log(f"result::{str(result)}","0")    
             if not isinstance(result, bool):
                 result = self._reform_result(result)
 
             final_result['status'] = 1
             final_result['result'] = result
         except Exception as ex:
             final_result['status'] = 0
             final_result['error'] = str(ex)
 
-        return final_result  # Changed by Pravin k on 27-JAN-20 START
-        # return make_response(str(final_result))
+        return final_result # Changed by Pravin k on 27-JAN-20 START
+        #return make_response(str(final_result))
 
     @staticmethod
     def get_input_reader_module(input_reader):
         if input_reader == 'pdftotext':
             from invoice2data.input import pdftotext
             return pdftotext
         elif input_reader == 'pdfminer':
```

## Comparing `documentdataextraction-0.0.8.dist-info/LICENCE.txt` & `documentdataextraction-0.0.9.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `documentdataextraction-0.0.8.dist-info/METADATA` & `documentdataextraction-0.0.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: documentdataextraction
-Version: 0.0.8
+Version: 0.0.9
 Summary: Proteus data extractor File
-Home-page: UNKNOWN
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
-License: UNKNOWN
 Keywords: python,first package
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENCE.txt
@@ -20,8 +17,7 @@
 Requires-Dist: readchequeutility
 Requires-Dist: fitz
 Requires-Dist: pathlib
 Requires-Dist: pdfkit
 Requires-Dist: flask
 
 Proteus data extractor File
-
```

## Comparing `documentdataextraction-0.0.8.dist-info/RECORD` & `documentdataextraction-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-documentdataextraction/__init__.py,sha256=TJvszsQaydFLP08kjLwQO_R5SqJXKWL5Qm7eJl0mbG8,10538
-documentdataextraction-0.0.8.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
-documentdataextraction-0.0.8.dist-info/METADATA,sha256=dlrH7X-Hax3FRAI5DJQuVEW7MeMqwCnRwj2uuIl00sA,779
-documentdataextraction-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-documentdataextraction-0.0.8.dist-info/top_level.txt,sha256=taEbXAAJc3t8awOVwH0T27Og25LLFSGtCTpHTIwa7e0,23
-documentdataextraction-0.0.8.dist-info/RECORD,,
+documentdataextraction/__init__.py,sha256=GN42L5jQ7z4gvvh666O1Yh-Nw4IvIu8AMY2KN1JXskA,10973
+documentdataextraction-0.0.9.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
+documentdataextraction-0.0.9.dist-info/METADATA,sha256=WO8oMrAqPXza9QqujHuwSrSCxul7k1bOHqY48XgRHdg,724
+documentdataextraction-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+documentdataextraction-0.0.9.dist-info/top_level.txt,sha256=taEbXAAJc3t8awOVwH0T27Og25LLFSGtCTpHTIwa7e0,23
+documentdataextraction-0.0.9.dist-info/RECORD,,
```

