# Comparing `tmp/nicknames-0.1.5.tar.gz` & `tmp/nicknames-0.1.6.tar.gz`

## Comparing `nicknames-0.1.5.tar` & `nicknames-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.5/test_package.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/_compat.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/_version.py
--rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/names.csv
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.5/.gitignore
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.5/hatch_build.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 nicknames-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.5/../README.md
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nicknames-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.6/test_package.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.6/src/nicknames/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.6/src/nicknames/_compat.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.6/src/nicknames/_version.py
+-rw-r--r--   0        0        0    22943 2020-02-02 00:00:00.000000 nicknames-0.1.6/src/nicknames/names.csv
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.6/hatch_build.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 nicknames-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.6/../README.md
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nicknames-0.1.6/PKG-INFO
```

### Comparing `nicknames-0.1.5/test_package.py` & `nicknames-0.1.6/test_package.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/src/nicknames/__init__.py` & `nicknames-0.1.6/src/nicknames/__init__.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/src/nicknames/_compat.py` & `nicknames-0.1.6/src/nicknames/_compat.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/src/nicknames/names.csv` & `nicknames-0.1.6/src/nicknames/names.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 aaron,erin,ronnie,ron
-abbigail,nabby,abby,gail,abbi,abbey
+abbigail,nabby,abby,gail,abbe,abbi,abbey
+abbigale,nabby,abby,gail,abbe,abbi,abbey
 abednego,bedney
 abel,ebbie,ab,abe,eb
 abiel,ab
-abigail,nabby,abby,gail
+abigail,nabby,abby,gail,abbe,abbi,abbey
+abigale,nabby,abby,gail,abbe,abbi,abbey
 abijah,ab,bige
 abner,ab
 abraham,ab,abe
 abram,ab,abe
 absalom,app,ab,abbie
-ada,addy
-adaline,delia,lena,dell,addy,ada
+ada,addy,adie
+adaline,delia,lena,dell,addy,ada,adie
 addison,addie,addy
-adela,della
-adelaide,heidi,adele,dell,addy,della
+adela,della,adie
+adelaide,heidi,adele,dell,addy,della,adie
 adelbert,del,albert,delbert,bert
 adele,addy,dell
 adeline,delia,lena,dell,addy,ada
 adelphia,philly,delphia,adele,dell,addy
 adolphus,dolph,ado,adolph
 adrian,rian
 adriane,riane
@@ -34,32 +36,32 @@
 aldo,al
 aldrich,riche,rich
 aleksandr,alex,alek
 aleva,levy,leve
 alex,al
 alexander,alex,al,sandy,alec
 alexandra,alex,sandy,alla,sandra
-alexandria,drina,alexander,alla,sandra
-alexis,lexi
+alexandria,drina,alexander,alla,sandra,alex
+alexis,lexi,alex
 alfonse,al
 alfred,freddy,al,fred
 alfreda,freddy,alfy,freda,frieda
 algernon,algy
 alice,lisa,elsie,allie
 alicia,lisa,elsie,allie
 aline,adeline
 alison,ali,allie
 alixandra,alix
 allan,al
 allen,al
-allisandra,allie
-allison,ali,allie
-allyson,ally,allie
-allyssa,ally,allie
-almena,mena,allie
+allisandra,ali,ally,allie
+allison,ali,ally,allie
+allyson,ali,ally,allie
+allyssa,ali,ally,allie
+almena,mena,ali,ally,allie
 almina,minnie
 almira,myra
 alonzo,lon,al,lonzo
 alphinias,alphus
 althea,ally
 alverta,virdie,vert
 alyssa,lissia,al,ally
@@ -345,35 +347,35 @@
 elijah,lige,eli
 eliphalel,life
 eliphalet,left
 elisa,lisa
 elisha,lish,eli
 eliza,elizabeth
 elizabeth,libby,lisa,lib,lizzy,lizzie,eliza,betsy,liza,betty,bessie,bess,beth,liz
-ella,ellen
+ella,ellen,el
 ellen,nellie,nell,helen
 ellender,nellie,ellen,helen
 ellie,elly
 ellswood,elsey
 elminie,minnie
 elmira,ellie,elly,mira
 elnora,nora
 eloise,heloise,louise
 elouise,louise
 elsie,elsey
 elswood,elsey
 elvira,elvie
 elwood,woody
-elysia,lisa
+elysia,lisa,lissa
 elze,elsey
 emanuel,manuel,manny
 emeline,em,emmy,emma,milly,emily
-emil,emily
-emily,emmy,millie,emma,mel
-emma,emmy
+emil,emily,em
+emily,emmy,millie,emma,mel,em
+emma,emmy,em
 epaphroditius,dite,ditus,eppa,dyche,dyce
 ephraim,eph
 erasmus,raze,rasmus
 eric,rick,ricky
 ernest,ernie
 ernestine,teeny,ernest,tina,erna
 erwin,irwin
@@ -401,27 +403,25 @@
 faith,fay
 felicia,fel,felix,feli
 felicity,flick,tick
 feltie,felty
 ferdinand,freddie,freddy,ferdie,fred
 ferdinando,nando,ferdie,fred
 fidelia,delia
-flo,florence
 flora,florence
 florence,flossy,flora,flo
 floyd,lloyd
 fran,frannie
 frances,sis,cissy,frankie,franniey,fran,francie,frannie,fanny
 francie,francine
 francine,franniey,fran,frannie,francie
 francis,fran,frankie,frank
-frank,franklin
 frankie,frank,francis
 franklin,fran,frank
-franklind,frank
+franklind,fran,frank
 freda,frieda
 frederica,frederick,freddy
 frederick,freddie,freddy,fritz,fred
 fredericka,freddy,ricka,freda,frieda
 frieda,freddie,freddy,fred
 gabriel,gabe,gabby
 gabriella,ella,gabby
@@ -590,15 +590,14 @@
 kendra,kenj,kenji,kay,kenny
 kendrick,ken,kenny
 kendrik,ken,kenny
 kenneth,ken,kenny,kendrick
 kenny,ken,kenneth
 kent,ken,kenny,kendrick
 keziah,kizza,kizzie
-kim,kimberly,kimberley
 kimberley,kim
 kimberly,kim
 kingsley,king
 kingston,king
 kit,kittie
 kris,chris
 kristel,kris
@@ -823,15 +822,15 @@
 oswald,ozzy,waldo,ossy
 otis,ode,ote
 pamela,pam
 pandora,dora
 parmelia,amelia,milly,melia
 parthenia,teeny,parsuny,pasoonie,phenie
 patience,pat,patty
-patricia,tricia,pat,patsy,patty,patti
+patricia,tricia,pat,patsy,patty,patti,trish
 patrick,pate,peter,pat,patsy,paddy
 patsy,patty
 patty,patricia
 paul,polly
 paula,polly,lina
 paulina,polly,lina
 pauline,polly
@@ -886,15 +885,15 @@
 rhyna,rhynie
 ricardo,rick,ricky
 rich,dick,rick
 richard,dick,dickon,dickie,dicky,rick,rich,ricky,richie
 rick,ricky
 ricky,dick,rich
 robert,hob,hobkin,dob,rob,bobby,dobbin,bob
-roberta,robbie,bert,bobbie,birdie,bertie
+roberta,robbie,bert,bobbie,birdie,bertie,roby
 roderick,rod,erick,rickie,roddy
 rodger,roge,bobby,hodge,rod,robby,rupert,robin
 rodney,rod
 roger,roge,bobby,hodge,rod,robby,rupert,robin
 roland,rollo,lanny,orlando,rolly
 ron,ronnie,ronny
 ronald,naldo,ron,ronny,ronnie
```

### Comparing `nicknames-0.1.5/hatch_build.py` & `nicknames-0.1.6/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/pyproject.toml` & `nicknames-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/../README.md` & `nicknames-0.1.6/../README.md`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.5/PKG-INFO` & `nicknames-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicknames
-Version: 0.1.5
+Version: 0.1.6
 Summary: Hand-curated dataset of English given names and nicknames
 Project-URL: Homepage, https://github.com/carltonnorthern/nicknames
 Project-URL: Bug Tracker, https://github.com/carltonnorthern/nicknames/issues
 Author-email: Carlton Northern <carlton.northern@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

