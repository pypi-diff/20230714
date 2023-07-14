# Comparing `tmp/kingsoftcloud-sdk-python-1.1.1.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.1.tar", last modified: Thu Jul 13 02:23:00 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.2.tar", last modified: Fri Jul 14 06:37:11 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.1.tar` & `kingsoftcloud-sdk-python-1.1.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 02:23:00.000000 kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.233834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.237834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.241834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   122915 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.245834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:23:00.249834 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 02:23:00.253834 kingsoftcloud-sdk-python-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 02:22:48.000000 kingsoftcloud-sdk-python-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 06:37:11.000000 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-14 06:37:11.000000 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:37:11.000000 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 06:37:11.000000 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 06:37:11.000000 kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.144559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.148559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.152559 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 06:37:11.156559 kingsoftcloud-sdk-python-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-14 06:36:56.000000 kingsoftcloud-sdk-python-1.1.2/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.1/LICENSE` & `kingsoftcloud-sdk-python-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.1/README.rst` & `kingsoftcloud-sdk-python-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.1/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.2/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
```

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/kec/v20160304/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,20 @@
         :type PathPrefix: Filter
         :param Userdata: 用户自定义数据
         :type PathPrefix: String
         :param SystemDisk.DiskType: 系统盘类型
         :type PathPrefix: String
         :param SystemDisk.DiskSize: 系统盘大小
         :type PathPrefix: Int
+        :param ModelId: 实例启动模版ID，如填写了此项，则RunInstances其他参数只有MaxCount、MinCount生效，其他不生效，如果批量创建，实例名称后缀依然存在。【传modelId，使用默认版本。传modelId和modelVersion，使用传递的版本】
+        :type PathPrefix: String
+        :param ModelVersion: 实例启动模板版本号。如不指定，则采用默认版本号
+        :type PathPrefix: Int
+        :param AssembledImageDataDiskType: 整机镜像所开云盘数据盘的类型
+        :type PathPrefix: String
         """
         self.ImageId = None
         self.DedicatedHostId = None
         self.InstanceConfigure.VCPU = None
         self.InstanceConfigure.MemoryGb = None
         self.InstanceType = None
         self.DataDiskGb = None
@@ -125,14 +131,17 @@
         self.InstanceNameSuffix = None
         self.ProjectId = None
         self.DataDisk = None
         self.NetworkInterface = None
         self.Userdata = None
         self.SystemDisk.DiskType = None
         self.SystemDisk.DiskSize = None
+        self.ModelId = None
+        self.ModelVersion = None
+        self.AssembledImageDataDiskType = None
 
     def _deserialize(self, params):
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("DedicatedHostId"):
             self.DedicatedHostId = params.get("DedicatedHostId")
         if params.get("InstanceConfigure.VCPU"):
@@ -171,14 +180,20 @@
             self.NetworkInterface = params.get("NetworkInterface")
         if params.get("Userdata"):
             self.Userdata = params.get("Userdata")
         if params.get("SystemDisk.DiskType"):
             self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
         if params.get("SystemDisk.DiskSize"):
             self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
+        if params.get("ModelId"):
+            self.ModelId = params.get("ModelId")
+        if params.get("ModelVersion"):
+            self.ModelVersion = params.get("ModelVersion")
+        if params.get("AssembledImageDataDiskType"):
+            self.AssembledImageDataDiskType = params.get("AssembledImageDataDiskType")
 
 
 class StartInstancesRequest(AbstractModel):
     """StartInstances请求参数结构体
     """
 
     def __init__(self):
@@ -459,23 +474,26 @@
         :param KeepImageLogin: 保留镜像设置登录。该参数只对使用自定义镜像有效。当该值填写为true，默认InstancePassword参数无效。该参数与InstancePassword必须填写一个。
 true/false,默认false
         :type PathPrefix: Boolean
         :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
         :type PathPrefix: String
         :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
         :type PathPrefix: String
+        :param UserData: 用户自定义数据，必须是base64编码
+        :type PathPrefix: String
         """
         self.InstanceId = None
         self.ImageId = None
         self.SystemDisk.DiskSize = None
         self.InstancePassword = None
         self.KeyId = None
         self.KeepImageLogin = None
         self.SystemDisk.DiskType = None
         self.SystemDisk.ResizeType = None
+        self.UserData = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("SystemDisk.DiskSize"):
@@ -486,14 +504,16 @@
             self.KeyId = params.get("KeyId")
         if params.get("KeepImageLogin"):
             self.KeepImageLogin = params.get("KeepImageLogin")
         if params.get("SystemDisk.DiskType"):
             self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
         if params.get("SystemDisk.ResizeType"):
             self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
+        if params.get("UserData"):
+            self.UserData = params.get("UserData")
 
 
 class CreateImageRequest(AbstractModel):
     """CreateImage请求参数结构体
     """
 
     def __init__(self):
@@ -2456,14 +2476,16 @@
         :param ModelName: 实例启动模版名称，不允许重复
 ModelTest001
         :type PathPrefix: String
         :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
         :type PathPrefix: String
         :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
         :type PathPrefix: String
+        :param VersionDetail: 模板描述
+        :type PathPrefix: String
         """
         self.ImageId = None
         self.InstanceType = None
         self.SystemDisk.DiskSize = None
         self.DataDiskGb = None
         self.SubnetId = None
         self.DataDisk = None
@@ -2482,14 +2504,15 @@
         self.LineId = None
         self.AddressChargeType = None
         self.AddressPurchaseTime = None
         self.AddressProjectId = None
         self.ModelName = None
         self.SystemDisk.DiskType = None
         self.SystemDisk.ResizeType = None
+        self.VersionDetail = None
 
     def _deserialize(self, params):
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("InstanceType"):
             self.InstanceType = params.get("InstanceType")
         if params.get("SystemDisk.DiskSize"):
@@ -2534,30 +2557,37 @@
             self.AddressProjectId = params.get("AddressProjectId")
         if params.get("ModelName"):
             self.ModelName = params.get("ModelName")
         if params.get("SystemDisk.DiskType"):
             self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
         if params.get("SystemDisk.ResizeType"):
             self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
+        if params.get("VersionDetail"):
+            self.VersionDetail = params.get("VersionDetail")
 
 
 class TerminateModelsRequest(AbstractModel):
     """TerminateModels请求参数结构体
     """
 
     def __init__(self):
         r"""删除实例启动模版
-        :param ModelId: 预删除的实例启动模板ID
-        :type PathPrefix: Filter
+        :param ModelId: 只传ModelId删除模板以及模板下对应的版本
+        :type PathPrefix: String
+        :param ModelVersion: 传ModelId和ModelVersion，删除某个模板下的版本
+        :type PathPrefix: Int
         """
         self.ModelId = None
+        self.ModelVersion = None
 
     def _deserialize(self, params):
         if params.get("ModelId"):
             self.ModelId = params.get("ModelId")
+        if params.get("ModelVersion"):
+            self.ModelVersion = params.get("ModelVersion")
 
 
 class DescribeModelsRequest(AbstractModel):
     """DescribeModels请求参数结构体
     """
 
     def __init__(self):
```

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.2/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.1/setup.py` & `kingsoftcloud-sdk-python-1.1.2/setup.py`

 * *Files identical despite different names*

