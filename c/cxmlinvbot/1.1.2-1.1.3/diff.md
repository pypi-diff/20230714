# Comparing `tmp/cxmlinvbot-1.1.2.tar.gz` & `tmp/cxmlinvbot-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.1.2.tar", last modified: Thu Jul 13 11:29:22 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.1.3.tar", last modified: Fri Jul 14 13:40:09 2023, max compression
```

## Comparing `cxmlinvbot-1.1.2.tar` & `cxmlinvbot-1.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:22.140000 cxmlinvbot-1.1.2/
--rw-rw-rw-   0        0        0      166 2023-07-13 11:29:22.120772 cxmlinvbot-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:07.190000 cxmlinvbot-1.1.2/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:12.970000 cxmlinvbot-1.1.2/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.2/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-07-13 11:23:30.000000 cxmlinvbot-1.1.2/cxmlinvbot/config/base.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:13.830000 cxmlinvbot-1.1.2/cxmlinvbot/errors/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.2/cxmlinvbot/errors/__init__.py
--rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.2/cxmlinvbot/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:14.270000 cxmlinvbot-1.1.2/cxmlinvbot/filing/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.2/cxmlinvbot/filing/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.2/cxmlinvbot/filing/filing.py
--rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.2/cxmlinvbot/kill.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:14.780000 cxmlinvbot-1.1.2/cxmlinvbot/mail/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.2/cxmlinvbot/mail/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.2/cxmlinvbot/mail/mail.py
--rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:17.830000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/__init__.py
--rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/action.py
--rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/headermapping.py
--rw-rw-rw-   0        0        0    14134 2023-06-30 13:25:39.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestmapping.py
--rw-rw-rw-   0        0        0    13884 2023-06-30 13:25:50.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
--rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/mapping.py
--rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/profilerequestmapping.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:18.890000 cxmlinvbot-1.1.2/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:21.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_main.py
--rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:29:11.780000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1207 2023-07-13 11:29:03.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:29:22.191465 cxmlinvbot-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:08.550000 cxmlinvbot-1.1.3/
+-rw-rw-rw-   0        0        0      166 2023-07-14 13:40:08.489600 cxmlinvbot-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:03.600000 cxmlinvbot-1.1.3/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.440000 cxmlinvbot-1.1.3/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.3/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1641 2023-07-14 13:31:53.000000 cxmlinvbot-1.1.3/cxmlinvbot/config/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.640000 cxmlinvbot-1.1.3/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.3/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.3/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.880000 cxmlinvbot-1.1.3/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.3/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.3/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:05.120000 cxmlinvbot-1.1.3/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.3/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.3/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:06.010000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    14227 2023-07-14 13:24:45.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0    13938 2023-07-14 13:24:19.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
+-rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.3/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:06.570000 cxmlinvbot-1.1.3/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5479 2023-07-14 12:22:32.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.3/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:08.180000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     3025 2023-07-14 12:24:26.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_main.py
+-rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:40:04.140000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-14 13:40:01.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1207 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 13:40:02.000000 cxmlinvbot-1.1.3/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:40:08.666697 cxmlinvbot-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.3/setup.py
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/config/base.py` & `cxmlinvbot-1.1.3/cxmlinvbot/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PROD_COUPA_END_POINT    = 'https://cbre.coupahost.com/cxml/'
     TEST_COUPA_END_POINT    = 'https://cbre-test.coupahost.com/cxml/'
     PROD_INVOICE_END_POINT  = '%sinvoices/' % PROD_COUPA_END_POINT
     TEST_INVOICE_END_POINT  = '%sinvoices/' % TEST_COUPA_END_POINT
 
     # Miscellania...
     MAIL_PREAMBLE           = 'Pro Door Invoice Bot - '
-    VERSION                 = '1.1.2'
+    VERSION                 = '1.1.3'
 
     # Testing widgets...
     SAMPLE_PATH             = '%sResources\\cXML\\1.2.057\\Samples\\' % EnvConfig.PROJECT_ROOT
     XML_SAMPLES             = {
         'ProfileResponse'           : '%sprofileresponse.xml' % SAMPLE_PATH,
         'ProfileResponseNoDTD'      : '%sprofileresponsenodtd.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/filing/filing.py` & `cxmlinvbot-1.1.3/cxmlinvbot/filing/filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mail/mail.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mail/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/main.py` & `cxmlinvbot-1.1.3/cxmlinvbot/main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mapping/action.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mapping/action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mapping/headermapping.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mapping/headermapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestmapping.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestmapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
-    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
@@ -40,20 +41,18 @@
     #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '437805'),
-    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),
-    POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
-    POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'London'),
-    POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
-    POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
+    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357108'),
+    SAAddressName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'Pro Door (UK) Limited'),
+    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@addressID', '437805'),
+    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),    
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
@@ -114,19 +113,21 @@
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic@name'),
     #                                      'ProdoorVatRegNO'),
     InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@invoiceLineNumber',
                                           'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference@lineNumber'),
                                           '1'), # There is only ever 1 PO per Invoice hence defaulting to 1
     InvoiceOp=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@operation', 'new'),
     InvoiceOrigin=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceOrigin', 'supplier'),
-    IPRole=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
+    IPRoleSupplier=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
+    IPRoleBuyer=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@role', 'billTo'),
     Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang'), 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang', 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'),                                       
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
     #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
-    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
@@ -34,20 +35,18 @@
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '437805'),
-    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),
-    POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
-    POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'London'),
-    POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
-    POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
+    RemitToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357108'),
+    SAAddressName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'Pro Door (UK) Limited'),
+    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@addressID', '437805'),
+    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),    
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
@@ -108,19 +107,21 @@
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic@name'),
     #                                      'ProdoorVatRegNO'),
     InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem@invoiceLineNumber',
                                           'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference@lineNumber'),
                                           '1'), # There is only ever 1 PO per Invoice hence defaulting to 1
     InvoiceOp=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@operation', 'new'),
     InvoiceOrigin=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceOrigin', 'supplier'),
-    IPRole=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
+    IPRoleSupplier=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
+    IPRoleBuyer=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact@role', 'billTo'),
     Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/InvoiceDetailServiceItemReference/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang'), 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang',
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner__seq2__/Contact/Name@xml:lang'), 
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
     #SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/SubtotalAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailServiceItem/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/mapping/mapping.py` & `cxmlinvbot-1.1.3/cxmlinvbot/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.1.3/cxmlinvbot/objects/cxmlobject.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 import urllib.request
 from   lxml import etree
 
 from   cxmlinvbot.config.base import BaseConfig
 from   cxmlinvbot.errors.errors import CXML_DTDError
 
 logger = logging.getLogger(__name__)
@@ -50,14 +51,15 @@
         self._dtdURL = BaseConfig.CXML_DTD_URL
         self._xmlNS = '{%s}' % BaseConfig.XML_NS
         self._parser = CXMLParser(self)  
         self._xml = etree.ElementTree(etree.XML('''\
 <?xml version="1.0"?>\
 <!DOCTYPE cXML SYSTEM "%s">\
 <cXML></cXML>''' % BaseConfig.CXML_DTD_URL))
+        self._seqPat = re.compile('__seq[0-9]*__')
 
     def parserElemCB(self, ancestor: str, elem: str, attrs: dict):
         '''
         ancestor: a string representing the last element processed
         elem: a string representing the current element to be processed
         attrs: a dict representing the attributes associated with this elem
 
@@ -72,16 +74,15 @@
         
         To be overridden in sub class
         '''        
         pass
 
     def _generateTree(self, pvMap: dict):
         '''
-        fv: a dictionary of fields->values to be mapped
-        m: a cxml mapping description
+        pvMap: a dictionary of paths->values to be mapped
         '''
 
         for p, v in pvMap.items():
             curEl = self._xml.getroot()
             els, attr = p.split('@')[:] if '@' in p else (p, None) 
             els = els.split('/')
             for e in els:
@@ -97,19 +98,27 @@
                 if ':' in attr:
                     curEl.set(self._xmlNS + attr.split(':')[1], v)
                 else:
                     curEl.set(attr, v)
             else:
                 curEl.text = v
             
+    def _removeSequenceIds(self):
+        # replace the sequence identifying element of any tag
+        for el in self._xml.getroot().getiterator():
+            m = self._seqPat.search(el.tag)
+            if m:
+                el.tag = el.tag.replace(m.group(), '')
+
     def fromPathValueMap(self, pvMap: dict):
         '''
         pvMap: a dictionary of xml paths->values to be mapped to cxml
         '''
         self._generateTree(pvMap)
+        self._removeSequenceIds()
 
     def fromXMLString(self, s):
         self._xml = etree.fromstring(s, parser=etree.XMLParser(target=self._parser))
 
     def fromXMLFile(self, f):
         '''
         f: filename or a file type object
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.1.3/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.1.3/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,18 +68,19 @@
         self.assertEqual(expectedRes, obj.asXMLString())
 
     def test_CXMLObjectFromPathValueMap(self):
         test = {
             'Foo/Bar': 'Hello',
             'Foo/Bar/Baa': 'World',
             'Foo/Bar@foo': 'bar',
+            'Foo/Bar__seq2__/Caa': 'Universe',
             'Foo/Bah': '!!'
         }
 
-        expectedRes = '<cXML><Foo><Bar foo="bar">Hello<Baa>World</Baa></Bar><Bah>!!</Bah></Foo></cXML>'
+        expectedRes = '<cXML><Foo><Bar foo="bar">Hello<Baa>World</Baa></Bar><Bar><Caa>Universe</Caa></Bar><Bah>!!</Bah></Foo></cXML>'
 
         obj = CXMLObject()
         obj.fromPathValueMap(test)
         self.assertTrue(expectedRes in obj.asXMLString())
 
 
 if __name__ == '__main__':
```

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_main.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.1.3/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/cxmlinvbot.egg-info/SOURCES.txt` & `cxmlinvbot-1.1.3/cxmlinvbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.2/setup.py` & `cxmlinvbot-1.1.3/setup.py`

 * *Files identical despite different names*

