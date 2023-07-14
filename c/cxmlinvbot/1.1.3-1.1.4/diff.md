# Comparing `tmp/cxmlinvbot-1.1.3.tar.gz` & `tmp/cxmlinvbot-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.1.3.tar", last modified: Fri Jul 14 13:40:09 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.1.4.tar", last modified: Fri Jul 14 15:38:45 2023, max compression
```

## Comparing `cxmlinvbot-1.1.3.tar` & `cxmlinvbot-1.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:08.550000 cxmlinvbot-1.1.3/
--rw-rw-rw-   0        0        0      166 2023-07-14 13:40:08.489600 cxmlinvbot-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:03.600000 cxmlinvbot-1.1.3/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.440000 cxmlinvbot-1.1.3/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.3/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-07-14 13:31:53.000000 cxmlinvbot-1.1.3/cxmlinvbot/config/base.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.640000 cxmlinvbot-1.1.3/cxmlinvbot/errors/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.3/cxmlinvbot/errors/__init__.py
--rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.3/cxmlinvbot/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.880000 cxmlinvbot-1.1.3/cxmlinvbot/filing/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.3/cxmlinvbot/filing/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/filing/filing.py
--rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.3/cxmlinvbot/kill.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:05.120000 cxmlinvbot-1.1.3/cxmlinvbot/mail/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.3/cxmlinvbot/mail/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.3/cxmlinvbot/mail/mail.py
--rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:06.010000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/__init__.py
--rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/action.py
--rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/headermapping.py
--rw-rw-rw-   0        0        0    14227 2023-07-14 13:24:45.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestmapping.py
--rw-rw-rw-   0        0        0    13938 2023-07-14 13:24:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
--rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/mapping.py
--rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/profilerequestmapping.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:06.570000 cxmlinvbot-1.1.3/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5479 2023-07-14 12:22:32.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:08.180000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     3025 2023-07-14 12:24:26.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_main.py
--rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.140000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-14 13:40:01.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1207 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 13:40:08.666697 cxmlinvbot-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:45.070000 cxmlinvbot-1.1.4/
+-rw-rw-rw-   0        0        0      166 2023-07-14 15:38:45.071084 cxmlinvbot-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:40.530000 cxmlinvbot-1.1.4/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.4/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:41.340000 cxmlinvbot-1.1.4/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.4/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1641 2023-07-14 15:37:03.000000 cxmlinvbot-1.1.4/cxmlinvbot/config/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:41.540000 cxmlinvbot-1.1.4/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.4/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.4/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:42.010000 cxmlinvbot-1.1.4/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.4/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.4/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.4/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:42.320000 cxmlinvbot-1.1.4/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.4/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.4/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     9292 2023-07-14 15:29:48.000000 cxmlinvbot-1.1.4/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:43.260000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    15982 2023-07-14 15:30:12.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0    15690 2023-07-14 15:20:56.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
+-rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.4/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:43.680000 cxmlinvbot-1.1.4/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.4/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5479 2023-07-14 12:22:32.000000 cxmlinvbot-1.1.4/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.4/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.4/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:44.490000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     3025 2023-07-14 12:24:26.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_main.py
+-rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:38:41.150000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-14 15:38:39.000000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1207 2023-07-14 15:38:39.000000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:38:39.000000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-14 15:38:39.000000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 15:38:39.000000 cxmlinvbot-1.1.4/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:38:45.100997 cxmlinvbot-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.4/setup.py
```

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/config/base.py` & `cxmlinvbot-1.1.4/cxmlinvbot/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PROD_COUPA_END_POINT    = 'https://cbre.coupahost.com/cxml/'
     TEST_COUPA_END_POINT    = 'https://cbre-test.coupahost.com/cxml/'
     PROD_INVOICE_END_POINT  = '%sinvoices/' % PROD_COUPA_END_POINT
     TEST_INVOICE_END_POINT  = '%sinvoices/' % TEST_COUPA_END_POINT
 
     # Miscellania...
     MAIL_PREAMBLE           = 'Pro Door Invoice Bot - '
-    VERSION                 = '1.1.3'
+    VERSION                 = '1.1.4'
 
     # Testing widgets...
     SAMPLE_PATH             = '%sResources\\cXML\\1.2.057\\Samples\\' % EnvConfig.PROJECT_ROOT
     XML_SAMPLES             = {
         'ProfileResponse'           : '%sprofileresponse.xml' % SAMPLE_PATH,
         'ProfileResponseNoDTD'      : '%sprofileresponsenodtd.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
```

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/filing/filing.py` & `cxmlinvbot-1.1.4/cxmlinvbot/filing/filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mail/mail.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mail/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/main.py` & `cxmlinvbot-1.1.4/cxmlinvbot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     invoice = row.get('InvoiceNumber', '')
     if not (type(invoice) == str and len(invoice)):
         return {'UNKNOWN' : 'There are rows in the CSV file without an InvoiceNumber field.'}
     
     logger.info('Processing invoice - %s' % invoice)
     if not cxmlArchive.exists(invoice):
         cxml = CXMLObject()
-        req = InvoiceDetailRequestMapping() if row.get('Quantity', True) else InvoiceDetailRequestServiceMapping()
+        req = InvoiceDetailRequestMapping() if row.get('Quantity', False) else InvoiceDetailRequestServiceMapping()
         try:
             cxml.fromPathValueMap(req.perform(row, catchAll=True))
             cxml.validate(req.getDTD_URL())
         except MapActionError as e1:
             logger.error('CSV mapping failed, please correct CSV for missing fields below...')
             logger.error(e1)
             return {invoice : e1}
```

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mapping/action.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mapping/action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mapping/headermapping.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mapping/headermapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestmapping.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,103 +2,107 @@
 import cxmlinvbot.mapping.action
 
 from   cxmlinvbot.config.base import BaseConfig
 from   cxmlinvbot.mapping.headermapping import HeaderMapping
 from   cxmlinvbot.mapping.mapping import Mapping
 from   local.config.env import EnvConfig
 
-class InvoiceDetailRequestMapping(Mapping):
+class InvoiceDetailRequestServiceMapping(Mapping):
   
   VAT_RE = re.compile('(?P<rate>[0-9]*)%.*')
 
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money',
-    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxRegime',
-    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money',
-    #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxRegime',
-    #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357108'),
+    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '1663'),
     SAAddressName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'Pro Door (UK) Limited'),
+    SAAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', 'Academy House'),
+    SAAddressLine2=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '241 Chertsey Road'),
+    SAAddressLine3=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'Addlestone'),
+    SAAddressLine4=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/State','Surrey'),
+    SAPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'KT15 2EW'),
+    SACountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@addressID', '437805'),
     ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),    
+    POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
+    POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/City', 'London'),
+    POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
+    POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
     #DueDate=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm/Extrinsic'),
     PlannedDate=cxmlinvbot.mapping.action.Ignore(),
-    TaxableAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
+    TaxableAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money')),
-    Total=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money',
+    Total=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money')),
     TaxTotal=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountPaid=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountDue=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money'),
     InventoryItemCode=cxmlinvbot.mapping.action.Ignore(),
-    Description=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description'),      
-    Quantity=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@quantity'),
-    UnitAmount=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money'),
-    UoM=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure', lambda m : {'Each':'EA'}.get(m, 'M4'), ('UoM',)),      
+    Description=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference/Description'),      
+    Quantity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem@quantity', ''),
+    #UnitAmount=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitPrice/Money'),
+    #UoM=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitOfMeasure', lambda m : {'Each':'EA'}.get(m, 'M4'), ('UoM',)),      
     Discount=cxmlinvbot.mapping.action.Ignore(),
     LineAmount=cxmlinvbot.mapping.action.Ignore(),
-    TaxType=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description',
+    TaxType=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description')),
-    #TaxCode=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxRegime',
+    #TaxCode=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxRegime',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxRegime'),
     #                                'Standard'),
-    TaxAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
-                                        'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money',
+    TaxAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money',
+                                        'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money',
                                         'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money',
                                         'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money')),
     TrackingName1=cxmlinvbot.mapping.action.Ignore(),
     TrackingOption1=cxmlinvbot.mapping.action.Ignore(),
     TrackingName2=cxmlinvbot.mapping.action.Ignore(),
     TrackingOption2=cxmlinvbot.mapping.action.Ignore(),
-    Currency=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money@currency',
+    Currency=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money@currency',
+                                    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitPrice/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money@currency'),
                                     'GBP'),
@@ -108,35 +112,35 @@
 
     # The following set of fields are additional requirements of the CXML document, they are not present in the CSV
     DeploymentMode=cxmlinvbot.mapping.action.Default('Request@deploymentMode', EnvConfig.DEPLOYMENT_MODE), # 'production' or 'test'
     #ExtrinsicDueDate=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm/Extrinsic@name', 'DueDate'),
     #ExtrinsicVatNo=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic@name',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic@name'),
     #                                      'ProdoorVatRegNO'),
-    InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@invoiceLineNumber',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference@lineNumber'),
+    InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem@invoiceLineNumber',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference@lineNumber'),
                                           '1'), # There is only ever 1 PO per Invoice hence defaulting to 1
     InvoiceOp=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@operation', 'new'),
     InvoiceOrigin=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceOrigin', 'supplier'),
     IPRoleSupplier=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
     IPRoleBuyer=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@role', 'billTo'),
-    Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description@xml:lang',
+    Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference/Description@xml:lang',
+                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang', 
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'),                                       
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang',
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'), 
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
-    #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
-    #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
+    #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
     #                                        lambda x, y : str(x * y), ('UnitAmount', 'Quantity')), # we never expect a Quantity > 1 currently            
-    TaxCat=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@category',
+    TaxCat=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail@category',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@category'),
                                               'vat'),
     TaxInline=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator@isTaxInLine', 'yes'),
-    TaxRate=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@percentageRate',
+    TaxRate=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail@percentageRate',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@percentageRate'),
-                                              lambda s : InvoiceDetailRequestMapping.VAT_RE.fullmatch(s).group('rate'), ('TaxType',)),
+                                              lambda s : InvoiceDetailRequestServiceMapping.VAT_RE.fullmatch(s).group('rate'), ('TaxType',)),
 )]
```

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mapping/invoicedetailrequestmapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,97 +2,113 @@
 import cxmlinvbot.mapping.action
 
 from   cxmlinvbot.config.base import BaseConfig
 from   cxmlinvbot.mapping.headermapping import HeaderMapping
 from   cxmlinvbot.mapping.mapping import Mapping
 from   local.config.env import EnvConfig
 
-class InvoiceDetailRequestServiceMapping(Mapping):
+class InvoiceDetailRequestMapping(Mapping):
   
   VAT_RE = re.compile('(?P<rate>[0-9]*)%.*')
 
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money',
-    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money',
+    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxRegime',
+    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
+    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money',
+    #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxRegime',
+    #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357108'),
+    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '1663'),
     SAAddressName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'Pro Door (UK) Limited'),
+    SAAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', 'Academy House'),
+    SAAddressLine2=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '241 Chertsey Road'),
+    SAAddressLine3=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'Addlestone'),
+    SAAddressLine4=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/State','Surrey'),
+    SAPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'KT15 2EW'),
+    SACountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@addressID', '437805'),
-    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),    
+    ContactName=cxmlinvbot.mapping.action.Default(   'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),    
+    POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
+    POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/City', 'London'),
+    POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
+    POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
     #DueDate=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm/Extrinsic'),
     PlannedDate=cxmlinvbot.mapping.action.Ignore(),
-    TaxableAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
+    TaxableAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money')),
-    Total=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money',
+    Total=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money')),
     TaxTotal=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountPaid=cxmlinvbot.mapping.action.Ignore(),
     InvoiceAmountDue=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money'),
     InventoryItemCode=cxmlinvbot.mapping.action.Ignore(),
-    Description=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference/Description'),      
-    Quantity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem@quantity', ''),
-    #UnitAmount=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitPrice/Money'),
-    #UoM=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitOfMeasure', lambda m : {'Each':'EA'}.get(m, 'M4'), ('UoM',)),      
+    Description=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description'),      
+    Quantity=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@quantity'),
+    UnitAmount=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money'),
+    UoM=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure', lambda m : {'Each':'EA'}.get(m, 'M4'), ('UoM',)),      
     Discount=cxmlinvbot.mapping.action.Ignore(),
     LineAmount=cxmlinvbot.mapping.action.Ignore(),
-    TaxType=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description',
+    TaxType=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description')),
-    #TaxCode=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxRegime',
+    #TaxCode=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxRegime',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxRegime'),
     #                                'Standard'),
-    TaxAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money',
-                                        'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money',
+    TaxAmount=cxmlinvbot.mapping.action.Required(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
+                                        'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money',
                                         'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money',
                                         'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money')),
     TrackingName1=cxmlinvbot.mapping.action.Ignore(),
     TrackingOption1=cxmlinvbot.mapping.action.Ignore(),
     TrackingName2=cxmlinvbot.mapping.action.Ignore(),
     TrackingOption2=cxmlinvbot.mapping.action.Ignore(),
-    Currency=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money@currency',
+    Currency=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxAmount/Money@currency',
-                                    #'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/UnitPrice/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money@currency',
-                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/GrossAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money@currency',
+                                    'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/GrossAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money@currency',
                                     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money@currency'),
                                     'GBP'),
@@ -102,35 +118,35 @@
 
     # The following set of fields are additional requirements of the CXML document, they are not present in the CSV
     DeploymentMode=cxmlinvbot.mapping.action.Default('Request@deploymentMode', EnvConfig.DEPLOYMENT_MODE), # 'production' or 'test'
     #ExtrinsicDueDate=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm/Extrinsic@name', 'DueDate'),
     #ExtrinsicVatNo=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic@name',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic@name'),
     #                                      'ProdoorVatRegNO'),
-    InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem@invoiceLineNumber',
-                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference@lineNumber'),
+    InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@invoiceLineNumber',
+                                          'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference@lineNumber'),
                                           '1'), # There is only ever 1 PO per Invoice hence defaulting to 1
     InvoiceOp=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@operation', 'new'),
     InvoiceOrigin=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceOrigin', 'supplier'),
     IPRoleSupplier=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
     IPRoleBuyer=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@role', 'billTo'),
-    Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description@xml:lang',
+    Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description@xml:lang',
+                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'), 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang', 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'),                                       
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
-    #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
-    #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
+    #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
+    #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
     #                                        lambda x, y : str(x * y), ('UnitAmount', 'Quantity')), # we never expect a Quantity > 1 currently            
-    TaxCat=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail@category',
+    TaxCat=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@category',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@category'),
                                               'vat'),
     TaxInline=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator@isTaxInLine', 'yes'),
-    TaxRate=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail@percentageRate',
+    TaxRate=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail@percentageRate',
                                               'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail@percentageRate'),
-                                              lambda s : InvoiceDetailRequestServiceMapping.VAT_RE.fullmatch(s).group('rate'), ('TaxType',)),
+                                              lambda s : InvoiceDetailRequestMapping.VAT_RE.fullmatch(s).group('rate'), ('TaxType',)),
 )]
```

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/mapping/mapping.py` & `cxmlinvbot-1.1.4/cxmlinvbot/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.1.4/cxmlinvbot/objects/cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.1.4/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.1.4/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_main.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.1.4/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/cxmlinvbot.egg-info/SOURCES.txt` & `cxmlinvbot-1.1.4/cxmlinvbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.3/setup.py` & `cxmlinvbot-1.1.4/setup.py`

 * *Files identical despite different names*

