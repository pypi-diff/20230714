# Comparing `tmp/AshCrypt-1.3.5.tar.gz` & `tmp/AshCrypt-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.3.5.tar", last modified: Sun Jul  9 22:31:08 2023, max compression
+gzip compressed data, was "AshCrypt-1.3.6.tar", last modified: Wed Jul 12 12:31:29 2023, max compression
```

## Comparing `AshCrypt-1.3.5.tar` & `AshCrypt-1.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.122261 AshCrypt-1.3.5/
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.086271 AshCrypt-1.3.5/AshCrypt/
--rw-rw-rw-   0        0        0     5209 2023-07-09 22:22:00.000000 AshCrypt-1.3.5/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    39532 2023-07-09 22:23:47.000000 AshCrypt-1.3.5/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6704 2023-07-09 22:26:42.000000 AshCrypt-1.3.5/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8993 2023-07-09 22:27:03.000000 AshCrypt-1.3.5/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     4019 2023-07-09 22:27:54.000000 AshCrypt-1.3.5/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.5/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1801 2023-07-09 22:29:17.000000 AshCrypt-1.3.5/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.5/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.110628 AshCrypt-1.3.5/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6384 2023-07-09 22:24:31.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.5/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-09 22:29:03.000000 AshCrypt-1.3.5/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.114964 AshCrypt-1.3.5/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.5/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.119046 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.5/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-09 22:31:08.095877 AshCrypt-1.3.5/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-09 22:31:07.000000 AshCrypt-1.3.5/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.5/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-09 22:31:08.122261 AshCrypt-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    21825 2023-07-09 20:32:48.000000 AshCrypt-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 22:31:08.123261 AshCrypt-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-09 20:20:19.000000 AshCrypt-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.913721 AshCrypt-1.3.6/
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.858448 AshCrypt-1.3.6/AshCrypt/
+-rw-rw-rw-   0        0        0     5207 2023-07-11 22:44:20.000000 AshCrypt-1.3.6/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    39423 2023-07-11 23:08:17.000000 AshCrypt-1.3.6/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6789 2023-07-12 12:30:45.000000 AshCrypt-1.3.6/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8993 2023-07-09 22:27:03.000000 AshCrypt-1.3.6/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     4017 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0      288 2023-07-11 22:11:01.000000 AshCrypt-1.3.6/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1799 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.6/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.895726 AshCrypt-1.3.6/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6384 2023-07-11 22:44:21.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7369 2023-07-10 11:21:27.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3292 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2430 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      738 2023-07-10 11:21:27.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-09 22:29:03.000000 AshCrypt-1.3.6/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.901722 AshCrypt-1.3.6/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.6/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.907719 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5719 2023-07-11 22:42:13.000000 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3348 2023-07-11 22:42:13.000000 AshCrypt-1.3.6/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.872127 AshCrypt-1.3.6/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0     1315 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     1315 2023-07-12 12:31:29.911726 AshCrypt-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21689 2023-07-11 22:57:53.000000 AshCrypt-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:31:29.913721 AshCrypt-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-12 12:30:49.000000 AshCrypt-1.3.6/setup.py
```

### Comparing `AshCrypt-1.3.5/AshCrypt/Ash.py` & `AshCrypt-1.3.6/AshCrypt/Ash.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             password=mainkey.encode('UTF-8'),
             salt=salt_pepper,
             desired_key_bytes=32,
             rounds=iterations)
 
     @staticmethod
     def genMainkey() -> str:
-        return os.urandom(64).hex()
+        return os.urandom(32).hex()
 
     def mode(self):
         return modes.CBC(self.iv)
 
     def cipher(self):
         return Cipher(
             algorithms.AES(
@@ -144,8 +144,8 @@
         unpadder = padding.PKCS7(128).unpadder()
         return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
 
     def decToBytes(self) -> bytes:
         return self.unpadded_m()
 
     def decToStr(self) -> str:
-        return (self.unpadded_m().decode('UTF-8'))
+        return (self.unpadded_m().decode('UTF-8'))
```

### Comparing `AshCrypt-1.3.5/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.3.6/AshCrypt/AshCryptGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os.path
 import string
 import atexit
 import json
 import re
 
 
-'''--------------------------------------FRAMING STARTED-------------------------------------------------------------'''
+'''------------------------FRAMING STARTED-------------------'''
 
 object = tk.Window(themename='vapor')
 object.resizable(False, False)
 object.title('AshCrypt')
 object.geometry('1500x800')
 
 
@@ -34,44 +34,49 @@
 
 textFrame2 = tk.Frame(master=object, width=500, height=250)
 textFrame2.place(x=1000, y=250)
 
 lowerFrame = tk.Frame(master=object, width=1000, height=260)
 lowerFrame.place(x=500, y=540)
 
-'''--------------------------------------DATABASE FRAME STARTED------------------------------------------------'''
+'''---------------DATABASE FRAME STARTED-----------------------'''
 
 
 databaseFrame = tk.Frame(master=object, height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
-console_label = tk.Label(
-    master=databaseFrame,
-    text='DATABASE OUTPUT CONSOLE',
-    font='Calibre 15 bold')
-console_label.place(relx=0.09, rely=0.04)
-
 if platform.system() == 'Windows':
-    db_display_text = tk.Text(
-        width=38,
-        height=18,
-        font='Calibre 13 bold',
+    console_label = tk.Label(
+        master=databaseFrame,
+        text='DATABASE OUTPUT CONSOLE',
+        font='Terminal 15 bold')
+    console_label.place(relx=0.09, rely=0.04)
+
+    db_display_text = tk.ScrolledText(
+        width=43,
+        height=27,
+        font='terminal 13',
         wrap='word')
-    db_display_text.place(relx=0.015, rely=0.105)
+    db_display_text.place(relx=0.016, rely=0.105)
     db_display_text.insert(tk.END, 'Waiting to fetch..')
 else:
+    console_label = tk.Label(
+        master=databaseFrame,
+        text='DATABASE OUTPUT CONSOLE',
+        font='Calibre 15 bold')
+    console_label.place(relx=0.09, rely=0.04)
+
     db_display_text = tk.Text(
         width=38,
         height=22,
         font='Calibre 13 bold',
         wrap='word')
     db_display_text.place(relx=0.015, rely=0.105)
     db_display_text.insert(tk.END, 'Waiting to fetch..')
 
-
 def show_all_content():
     global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn, db_display_text, keys_db_conn
     if db_enable_blocker != 0:
         db_display_text.delete('1.0', tk.END)
         db_display_text.insert(
             tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
         json_path = os.path.join(usable_real_path, 'output.json')
@@ -287,15 +292,15 @@
     master=databaseFrame,
     text='SHOW CONTENT BY ID',
     command=show_content_by_id,
     bootstyle='warning outline')
 show_content_by_id_button.place(relx=0.562, rely=0.93)
 
 
-'''----------------------------------------LOWER FRAME STARTED----------------------------------'''
+'''----------------------LOWER FRAME STARTED------------------'''
 
 
 lowerFrame = tk.Frame(master=object, width=1000, height=260)
 lowerFrame.place(x=500, y=540)
 
 
 db_path_blocker = 0
@@ -604,15 +609,15 @@
                                  command=swich_db)
 swich_db_toggle.state(['disabled'])
 
 
 swich_db_toggle.place(relx=0.47, rely=0.413)
 
 
-'''-------------------------------TEXT DECRYPTION/ENCRYPTION STARTED---------------------------------------------------'''
+'''------------TEXT DECRYPTION/ENCRYPTION STARTED--------------'''
 
 
 def encryption():
     m = inputfield1_1.get()
     if AF.CryptFile.keyverify(
             mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if len(m) > 200:
@@ -748,15 +753,15 @@
     mode='indeterminate',
     style='secondary',
     length=100,
 )
 progressbar2.place(relx=0.05, rely=0.42)
 
 
-'''-------------------------------FILE ENCRYPTION/DECRYPTION STARTED--------------------------------------------'''
+'''---------FILE ENCRYPTION/DECRYPTION STARTED-------------'''
 
 
 filepathlabel = tk.Label(master=frameFile1,
                          text='FILE PATH',
                          font='Calibre 20 bold',
                          )
 filepathlabel.place(relx=0.335, rely=0.10)
@@ -1069,24 +1074,24 @@
 
 keyButton = tk.Button(master=frameFile2,
                       text='GENERATE',
                       command=genMainKey,
                       bootstyle='success outline').place(relx=0.671, rely=0.7)
 
 
-'''---------------------------------------STAMP STARTED -------------------------------------------------------'''
+'''----------------------------STAMP STARTED ------------------------------'''
 
 
 latest_ID_key_label = tk.Label(
     master=lowerFrame,
     text='GitHub.com/AshGw/AES-256',
     font='Calibre 6')
 latest_ID_key_label.place(relx=0.84, rely=0.92)
 
-'''---------------------------------------STAMP ENDED-------------------------------------------------------'''
+'''------------------------------STAMP ENDED------------------------------'''
 
 
 def rm_json():
     global usable_real_path
     file = os.path.join(usable_real_path, 'output.json')
     if os.path.exists(file):
         os.remove(file)
```

### Comparing `AshCrypt-1.3.5/AshCrypt/CliCrypt.py` & `AshCrypt-1.3.6/AshCrypt/CliCrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 from AshCrypt import TextCrypt as A
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
-commands = 'Commands : \n\tq: to quit the program \n\tc : view commands\n\te: for encryption\n\td : for decryption\n' \
-           '\tef : to encrypt a file\n\tdf : to decrypt a file\n'
+commands = 'Commands : \n' \
+           '\tq: to quit the program \n' \
+           '\tc : view commands\n' \
+           '\te: for encryption\n' \
+           '\td : for decryption\n' \
+           '\tef : to encrypt a file\n' \
+           '\tdf : to decrypt a file\n'
 
 global key
 
 
 def input_selection(q=None, c=None, e=None, d=None, ef=None, df=None):
     global encflag, decFlag, file_decFlag, file_encFlag
     if q == 1:
@@ -179,15 +184,15 @@
             if a == 0:
                 print(
                     'Error in the decryption process. Check if the the file is distorted or it might just be '
                     'decrypted already')
             if a == 4:
                 print('Unknown Error has occurred\n')
             if a == 5:
-                print('ERROR : Key is Not 512-bit')
+                print('ERROR : Key is Not 256-bit')
             if a == 6:
                 print('ERROR : File is already decrypted')
             elif a == 7:
                 print('ERROR : Given a directory instead of a file')
 
 
 def file_enc():
@@ -214,15 +219,15 @@
                     f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
                 print(
                     'Error in the encryption process. Check if the the file is distorted')
             elif a == 4:
                 print('Unknown Error has occurred\n')
             if a == 5:
-                print('ERROR : Key is Not 512-bit')
+                print('ERROR : Key is Not 256-bit')
             if a == 6:
                 print('ERROR : File is already encrypted')
             elif a == 7:
                 print('ERROR : Given a directory instead of a file')
 
 
 if __name__ == '__main__':
```

### Comparing `AshCrypt-1.3.5/AshCrypt/Database.py` & `AshCrypt-1.3.6/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.5/AshCrypt/FileCrypt.py` & `AshCrypt-1.3.6/AshCrypt/FileCrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from AshCrypt import Ash
 import os
 
 
 class KeyError(Exception):
     def __init__(self):
-        self.display = 'Key must be 512 Bit long !'
+        self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class CryptFile():
     def __init__(self, filename, key):
         self.filename = filename
-        self.not_512_bit_key = 0
+        self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
-            self.not_512_bit_key = 1  # Raise KeyError()
+            self.not_256_bit_key = 1  # Raise KeyError()
 
     @staticmethod
     def genkey() -> str:
         return Ash.Enc.genMainkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         try:
             if isinstance(key, str):
                 a = bytes.fromhex(key.strip())
-                if len(a) == 64:
+                if len(a) == 32:
                     return 1
                 else:
                     return 0
         except BaseException:
             return 2
 
     def encrypt(self) -> int:
         if os.path.isdir(self.filename):
             return 7
-        if self.not_512_bit_key == 1:
+        if self.not_256_bit_key == 1:
             return 5
         try:
             go_ahead_rename_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
                 if os.path.splitext(self.filename)[1] == '.crypt':
@@ -67,15 +67,15 @@
                         return 1
         except Exception:
             return 4
 
     def decrypt(self) -> int:
         if os.path.isdir(self.filename):
             return 7
-        if self.not_512_bit_key == 1:
+        if self.not_256_bit_key == 1:
             return 5
         try:
             go_ahead_remove_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
                 if os.path.splitext(self.filename)[1] != '.crypt':
@@ -105,8 +105,8 @@
         except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
+        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `AshCrypt-1.3.5/AshCrypt/README.md` & `AshCrypt-1.3.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,137 @@
-# Cryptography App &  Library : AES-256
+# Cryptography App & Library w/ AES-256
 ##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
+## Reason Behind It
+In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
+
+This led me to develop a set of tools in Python that leverages the AES-256 algorithm to make it easier for individuals to safeguard their data without blindly relying on third parties to do it for them. 
+
+My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
-**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
-<br>The library incorporates a base cryptography mdoule called **Ash** 
+![alt text](important/GUI.png)
+The project incorporates an App & a library called **AshCrypt** : 
 
-<br>A simple, secure, and developer-oriented module for
-encryption and decryption with AES-256 (CBC) . It offers an intuitive
-interface, seamless integration with precompiled 
+**App :** 
+<br>Fully-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
+<br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
+
+**Library :** 
+<br>A simple, secure, and developer-oriented library for
+encryption and decryption with AES-256 (CBC) . 
+<br>The core of the library is the module `Ash`
+It offers an intuitive interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
-<br>View **Features** Header for more details.
+<br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
-The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check `GUI` header for more info.
-
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for `FileCrypt` and `TextCrypt` to learn more.
+view the headers for [FileCrypt](https://github.com/AshGw/AES-256#filecrypt) and [TextCrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
-safe and simple manner, you can use whichever you see fit.
+safe and simple manner.
+
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [Database](https://github.com/AshGw/AES-256#database-1) header to learn more.
+
+## Installation ##
+There are many ways to go by this : 
+### If you want to use it as a library ###
+You can simply use **pip**
+<br>First upgrade the package installer 
+```bash
+pip install --upgrade pip 
+```
+Then install the Library 
+```bash
+pip install AshCrypt
+```
+This will install the latest version of `AshCrypt`.
+You can start using it in your code by importing its modules : 
+```python
+from AshCrypt.Ash import *
+```
+That's it.
+### Ready-to-go Executable files:
+If you want to use the App right away : 
+<br>**For Windows** : Download this repo as a ZIP file, extract the content
+<br>then click on `Executables > AshCryptGUI.exe` This will automatically run the GUI
+
+### Whole repo installation 
+Now if you want to get the whole repo with no manual configurations
+<br>Run this command in the Terminal
+```bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
+```
+This will run the commands in [setup.sh](important/setup.sh).
+<br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
+
+you can use this command to automate the environment setup process if you haven't done it  already
+```bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/Docker-build/env-setup.sh | bash
+```
+<details>
+<summary>Got Errors ?</summary>
+
+<h5>For Debian based systems</h5>
 
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
-Check `Database` header to learn more.
+1) Install `curl` if you don't have it already 
+```bash
+sudo apt-get install curl
+```
+2) If you're running a lightweight python version it might not include `tkinter` in the standard library so run
+```bash
+sudo apt-get update
+sudo apt-get install python3-tk 
+```
+3) If you're running `python 3.6` or older then you might need to install `dataclasses`
+```
+pip install dataclasses
+```
+<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
+</details>
 
-**After the library is installed**
-<br>to run the GUI 
+**After the library is installed** 
+<br>To run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
-To run the CLI
+
+**NOTE**:
+You  can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
+
+
+To run the CLI 
 ```shell
 python -m AshCrypt.CliCrypt
 ```
 
-
 ## Ash Module ##
-The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+The `Ash.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
-<br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
-<br>You can check **Features** tag below to learn more about the security features.
+<br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
+<br>You can check the [unittesting file](AshCrypt/unittests/unittestAsh.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
 <br>Set the correct mainkey ( 64 byte long key ) 
 ```python
-mainkey = 'd5d717f57933ad21725888d3451a9cd7a565dfda677fe92fd8ff9e9c3a36d1496af58c17de2b77d4d3ea6d8791b27350fea0af3ad2610d38c8cb12a29fda4bcf'
+mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
 The message can be of type string or bytes.
 <br>Normal string message :  
 ```python 
 message = 'Hello There'
 ```
 or a normal bytes message 
@@ -95,45 +165,45 @@
 That simple, that's it.
 
 
 
 
 ## Features ## 
 - AES 256 CBC mode 
-- Generates a randomly secure 512 Bit mainkey 
+- Generates a randomly secure 256 Bit main key 
 - Derives the HMAC and the AES key from the mainkey using bcrypt's KDFs with a configurable number of iterations with :
     - Salt : Random 128 bit value is generated  each time and passed to the KDF to generate the AES key
     - Pepper : Random 128 bit value is generated  each time and passed to the KDF to generate the HMAC
 - AES Key : 256 bit
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 512 bit long key )
+- In Ash module the key is flexible it doesn't have to be 256 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 256 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
-
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
-
-
-
+<br>You can check how it works by checking this [Jupyter Notebook](demo/demo.ipynb) demo file
+<br>Note that im using a 512 bit long key to demonstrate the process although as I mentioned earlier you can use any key length with `Ash`.
 ## AshCryptGUI ##
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
 - Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+<br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
+
 #### Files
 - Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
 - The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extention you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
 #### Database
 - Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
 1) Specify the actual path where you want your database to be 
 2) Give it a name, it must be a valid file name that ends with `.db` .<br>
@@ -145,19 +215,19 @@
 <br>If anyone gets hold of your main database they would only see some encrypted content and some key refrence that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
 That's why I made two different databases not two tables within a single database. 
 <br> So you keep your keys database safe and secure.
 
 
 **Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
 `Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
-<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 512 bit long encryption key.
+<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 256 bit long encryption key.
 <br>`Key` in  both db's that holds the `KeyRef` or key reference value
 #### Usage 
 The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
-<br>Just click buttons and check the result in the output console, it will guide you the process.
+<br>Just click buttons and check the result in the output console, it will guide you through the process.
 
 <br>To run the GUI anywhere
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 
@@ -194,24 +264,21 @@
 <br> 1 : File successfully encrypted/decrypted + added/removed .crypt extension 
 <br> 2 : File is empty
 <br> 3 : File doesn't exist
 <br> 4 : Unknown Error usually a system related one 
 <br> 5 : Key is denied for cryptographic use
 <br> 6 : File is already encrypted/decrypted
 <br> 7 : File is not a file it's a directory
-<br> 0 : Error in enc/dec probable file distortion or tampering or wrong key
+<br> 0 : Error in enc/dec probable file distortion, tampering or wrong key
 ```python
 instance1.encrypt()
 ```
 ```python
 instance1.decrypt()
 ```
-**Note** : 
-<br>Sometimes you might forget that you've applied  `encrypt()` more than one time , so when you try to `decrypt()` the file ,  the output is 1 but the file content is still in binary, just apply the function `decrypt()` the same number of times you applied `encrypt()`.
-
 
 That's it, if you follow the steps above then everything should work just fine.
 ## TextCrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
 instance1 = Crypt('Hello Wold !',key)
 ```
```

### Comparing `AshCrypt-1.3.5/AshCrypt/TextCrypt.py` & `AshCrypt-1.3.6/AshCrypt/TextCrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 from AshCrypt import Ash
 
 
 class KeyError(Exception):
     def __init__(self):
-        self.display = 'Key must be 512 Bit long !'
+        self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class Crypt():
     def __init__(self, text: Union[str, bytes], key: str):
         self.text = text
         if self.keyverify(key) == 1:
@@ -21,15 +21,15 @@
         return Ash.Enc.genMainkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         if isinstance(key, str):
             try:
                 a = bytes.fromhex(key.strip())
-                if len(a) == 64:
+                if len(a) == 32:
                     return 1
             except Exception:
                 return 0
 
         else:
             return 2
 
@@ -58,8 +58,8 @@
         else:
             return 0.0, 0.0
 
     def __str__(self):
         return f'Encrypting/Decrypting Text {(self.text)[:8]}.. With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({(self.text)[:8]},{self.key})'
+        return f'{self.__class__.__name__}({(self.text)[:8]},{self.key})'
```

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jul  9 22:22:00 2023 UTC, .py size: 5209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0833 ab64 5914 0000  a........3.dY...
+00000000: 610d 0d0a 0000 0000 44db ad64 5714 0000  a.......D..dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c09 5a0c 6400  m.Z...d.d.l.Z.d.
@@ -28,29 +28,29 @@
 000001b0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
 000001c0: 0000 0073 2000 0000 6401 7c01 9b00 6402  ...s ...d.|...d.
 000001d0: 9d03 7c00 5f00 7401 8300 a002 7c00 6a00  ..|._.t.....|.j.
 000001e0: a101 0100 6400 5300 2903 4e7a 3549 7465  ....d.S.).Nz5Ite
 000001f0: 7261 7469 6f6e 7320 6d75 7374 2062 6520  rations must be 
 00000200: 6265 7477 6565 6e20 3530 2061 6e64 2031  between 50 and 1
 00000210: 3030 3030 302e 2052 4543 4549 5645 4420  00000. RECEIVED 
-00000220: 3a20 fa01 20a9 03da 0764 6973 706c 6179  : .. ....display
+00000220: 3a20 fa01 20a9 035a 0764 6973 706c 6179  : .. ..Z.display
 00000230: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
 00000240: 5f29 02da 0473 656c 6672 0b00 0000 a901  _)...selfr......
 00000250: da09 5f5f 636c 6173 735f 5fa9 00fa 2a43  ..__class__...*C
 00000260: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
 00000270: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
-00000280: 7074 5c41 7368 2e70 7972 1100 0000 0e00  pt\Ash.pyr......
+00000280: 7074 5c41 7368 2e70 7972 1000 0000 0e00  pt\Ash.pyr......
 00000290: 0000 7304 0000 0000 010e 017a 2349 7465  ..s........z#Ite
 000002a0: 7261 7469 6f6e 734f 7574 6f66 6152 616e  rationsOutofaRan
 000002b0: 6765 4572 726f 722e 5f5f 696e 6974 5f5f  geError.__init__
 000002c0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000002d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000002e0: 6e61 6d65 5f5f da03 616e 7972 1100 0000  name__..anyr....
+000002e0: 6e61 6d65 5f5f da03 616e 7972 1000 0000  name__..anyr....
 000002f0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000300: 1500 0000 7215 0000 0072 1300 0000 7216  ....r....r....r.
+00000300: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
 00000310: 0000 0072 0a00 0000 0d00 0000 7302 0000  ...r........s...
 00000320: 0008 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
 00000330: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
 00000340: 0073 bc00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
 00000350: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
 00000360: 6403 6404 8404 5a06 6507 6504 6505 6508  d.d...Z.e.e.e.e.
 00000370: 6505 6405 9c04 6406 6407 8404 8301 5a09  e.d...d.d.....Z.
@@ -75,185 +75,185 @@
 000004a0: 6a7c 006a 0b64 036b 0472 7474 0c7c 006a  j|.j.d.k.rtt.|.j
 000004b0: 0b83 0182 017c 00a0 0d7c 006a 057c 006a  .....|...|.j.|.j
 000004c0: 097c 006a 0ba1 037c 005f 0e7c 00a0 0d7c  .|.j...|._.|...|
 000004d0: 006a 057c 006a 0a7c 006a 0ba1 037c 005f  .j.|.j.|.j...|._
 000004e0: 0f64 0053 0029 044e e910 0000 00e9 3200  .d.S.).N......2.
 000004f0: 0000 e9a0 8601 0029 10da 0a69 7369 6e73  .......)...isins
 00000500: 7461 6e63 65da 0373 7472 da06 656e 636f  tance..str..enco
-00000510: 6465 721e 0000 00da 0562 7974 6573 721f  der......bytesr.
+00000510: 6465 721d 0000 00da 0562 7974 6573 721e  der......bytesr.
 00000520: 0000 00da 026f 73da 0775 7261 6e64 6f6d  .....os..urandom
 00000530: da02 6976 da04 7361 6c74 da06 7065 7070  ..iv..salt..pepp
 00000540: 6572 da0a 6974 6572 6174 696f 6e73 720a  er..iterationsr.
 00000550: 0000 00da 0664 6572 6b65 79da 0665 6e63  .....derkey..enc
 00000560: 4b65 79da 0868 6d61 635f 6b65 7929 0372  Key..hmac_key).r
-00000570: 1200 0000 721e 0000 0072 1f00 0000 7215  ....r....r....r.
-00000580: 0000 0072 1500 0000 7216 0000 0072 1100  ...r....r....r..
+00000570: 1100 0000 721d 0000 0072 1e00 0000 7214  ....r....r....r.
+00000580: 0000 0072 1400 0000 7215 0000 0072 1000  ...r....r....r..
 00000590: 0000 1400 0000 731a 0000 0000 010a 010c  ......s.........
 000005a0: 010a 0106 0206 010c 010c 010c 0106 0114  ................
 000005b0: 010a 0116 017a 0c45 6e63 2e5f 5f69 6e69  .....z.Enc.__ini
-000005c0: 745f 5f29 0472 1f00 0000 da0b 7361 6c74  t__).r......salt
-000005d0: 5f70 6570 7065 7272 2c00 0000 720c 0000  _pepperr,...r...
+000005c0: 745f 5f29 0472 1e00 0000 da0b 7361 6c74  t__).r......salt
+000005d0: 5f70 6570 7065 7272 2b00 0000 720c 0000  _pepperr+...r...
 000005e0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
 000005f0: 0000 0600 0000 4300 0000 7318 0000 0074  ......C...s....t
 00000600: 006a 017c 00a0 0264 01a1 017c 0164 027c  .j.|...d...|.d.|
 00000610: 0264 038d 0453 0029 044e fa05 5554 462d  .d...S.).N..UTF-
 00000620: 38e9 2000 0000 2904 5a08 7061 7373 776f  8. ...).Z.passwo
-00000630: 7264 722a 0000 005a 1164 6573 6972 6564  rdr*...Z.desired
+00000630: 7264 7229 0000 005a 1164 6573 6972 6564  rdr)...Z.desired
 00000640: 5f6b 6579 5f62 7974 6573 da06 726f 756e  _key_bytes..roun
 00000650: 6473 2903 da06 6263 7279 7074 5a03 6b64  ds)...bcryptZ.kd
-00000660: 6672 2500 0000 2903 721f 0000 0072 3000  fr%...).r....r0.
-00000670: 0000 722c 0000 0072 1500 0000 7215 0000  ..r,...r....r...
-00000680: 0072 1600 0000 722d 0000 0024 0000 0073  .r....r-...$...s
+00000660: 6672 2400 0000 2903 721e 0000 0072 2f00  fr$...).r....r/.
+00000670: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
+00000680: 0072 1500 0000 722c 0000 0024 0000 0073  .r....r,...$...s
 00000690: 0c00 0000 0002 0401 0801 0201 0201 02fc  ................
 000006a0: 7a0a 456e 632e 6465 726b 6579 a901 720c  z.Enc.derkey..r.
 000006b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 000006c0: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
 000006d0: 0074 00a0 0164 01a1 01a0 02a1 0053 0029  .t...d.......S.)
-000006e0: 024e e940 0000 0029 0372 2700 0000 7228  .N.@...).r'...r(
-000006f0: 0000 00da 0368 6578 7215 0000 0072 1500  .....hexr....r..
-00000700: 0000 7215 0000 0072 1600 0000 da0a 6765  ..r....r......ge
+000006e0: 024e 7231 0000 0029 0372 2600 0000 7227  .Nr1...).r&...r'
+000006f0: 0000 00da 0368 6578 7214 0000 0072 1400  .....hexr....r..
+00000700: 0000 7214 0000 0072 1500 0000 da0a 6765  ..r....r......ge
 00000710: 6e4d 6169 6e6b 6579 2c00 0000 7302 0000  nMainkey,...s...
 00000720: 0000 027a 0e45 6e63 2e67 656e 4d61 696e  ...z.Enc.genMain
 00000730: 6b65 7963 0100 0000 0000 0000 0000 0000  keyc............
 00000740: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
 00000750: 0074 00a0 017c 006a 02a1 0153 00a9 014e  .t...|.j...S...N
-00000760: 2903 7204 0000 00da 0343 4243 7229 0000  ).r......CBCr)..
-00000770: 00a9 0172 1200 0000 7215 0000 0072 1500  ...r....r....r..
-00000780: 0000 7216 0000 00da 046d 6f64 6530 0000  ..r......mode0..
+00000760: 2903 7204 0000 00da 0343 4243 7228 0000  ).r......CBCr(..
+00000770: 00a9 0172 1100 0000 7214 0000 0072 1400  ...r....r....r..
+00000780: 0000 7215 0000 00da 046d 6f64 6530 0000  ..r......mode0..
 00000790: 0073 0200 0000 0001 7a08 456e 632e 6d6f  .s......z.Enc.mo
 000007a0: 6465 6301 0000 0000 0000 0000 0000 0001  dec.............
 000007b0: 0000 0005 0000 0043 0000 0073 1e00 0000  .......C...s....
 000007c0: 7400 7401 6a02 7c00 6a03 6401 8d01 7c00  t.t.j.|.j.d...|.
 000007d0: a004 a100 7405 8300 6402 8d03 5300 a903  ....t...d...S...
-000007e0: 4e29 01da 036b 6579 2902 723c 0000 005a  N)...key).r<...Z
+000007e0: 4e29 01da 036b 6579 2902 723a 0000 005a  N)...key).r:...Z
 000007f0: 0762 6163 6b65 6e64 2906 7202 0000 0072  .backend).r....r
-00000800: 0300 0000 da03 4145 5372 2e00 0000 723c  ......AESr....r<
-00000810: 0000 0072 0600 0000 723b 0000 0072 1500  ...r....r;...r..
-00000820: 0000 7215 0000 0072 1600 0000 da06 6369  ..r....r......ci
+00000800: 0300 0000 da03 4145 5372 2d00 0000 723a  ......AESr-...r:
+00000810: 0000 0072 0600 0000 7239 0000 0072 1400  ...r....r9...r..
+00000820: 0000 7214 0000 0072 1500 0000 da06 6369  ..r....r......ci
 00000830: 7068 6572 3300 0000 730e 0000 0000 0102  pher3...s.......
 00000840: 0104 0104 ff04 0206 0104 fc7a 0a45 6e63  ...........z.Enc
 00000850: 2e63 6970 6865 7263 0100 0000 0000 0000  .cipherc........
 00000860: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
 00000870: 730c 0000 007c 00a0 00a1 00a0 01a1 0053  s....|.........S
-00000880: 0072 3900 0000 2902 7240 0000 005a 0965  .r9...).r@...Z.e
-00000890: 6e63 7279 7074 6f72 723b 0000 0072 1500  ncryptorr;...r..
-000008a0: 0000 7215 0000 0072 1600 0000 da10 6369  ..r....r......ci
+00000880: 0072 3700 0000 2902 723e 0000 005a 0965  .r7...).r>...Z.e
+00000890: 6e63 7279 7074 6f72 7239 0000 0072 1400  ncryptorr9...r..
+000008a0: 0000 7214 0000 0072 1500 0000 da10 6369  ..r....r......ci
 000008b0: 7068 6572 5f65 6e63 7279 7074 6f72 3a00  pher_encryptor:.
 000008c0: 0000 7302 0000 0000 017a 1445 6e63 2e63  ..s......z.Enc.c
 000008d0: 6970 6865 725f 656e 6372 7970 746f 7263  ipher_encryptorc
 000008e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 000008f0: 0300 0000 4300 0000 7322 0000 0074 00a0  ....C...s"...t..
 00000900: 0164 01a1 01a0 02a1 007d 017c 01a0 037c  .d.......}.|...|
 00000910: 006a 04a1 017c 01a0 05a1 0017 0053 00a9  .j...|.......S..
 00000920: 024e e980 0000 0029 0672 0500 0000 da05  .N.....).r......
 00000930: 504b 4353 37da 0670 6164 6465 72da 0675  PKCS7..padder..u
-00000940: 7064 6174 6572 1e00 0000 da08 6669 6e61  pdater......fina
-00000950: 6c69 7a65 2902 7212 0000 0072 4500 0000  lize).r....rE...
-00000960: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000940: 7064 6174 6572 1d00 0000 da08 6669 6e61  pdater......fina
+00000950: 6c69 7a65 2902 7211 0000 0072 4300 0000  lize).r....rC...
+00000960: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
 00000970: 0e70 6164 6465 645f 6d65 7373 6167 653d  .padded_message=
 00000980: 0000 0073 0400 0000 0001 0e01 7a12 456e  ...s........z.En
 00000990: 632e 7061 6464 6564 5f6d 6573 7361 6765  c.padded_message
 000009a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 000009b0: 0004 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
 000009c0: a000 a100 a001 7c00 a002 a100 a101 7c00  ......|.......|.
-000009d0: a000 a100 a003 a100 1700 5300 7239 0000  ..........S.r9..
-000009e0: 0029 0472 4100 0000 7246 0000 0072 4800  .).rA...rF...rH.
-000009f0: 0000 7247 0000 0072 3b00 0000 7215 0000  ..rG...r;...r...
-00000a00: 0072 1500 0000 7216 0000 00da 0a63 6970  .r....r......cip
+000009d0: a000 a100 a003 a100 1700 5300 7237 0000  ..........S.r7..
+000009e0: 0029 0472 3f00 0000 7244 0000 0072 4600  .).r?...rD...rF.
+000009f0: 0000 7245 0000 0072 3900 0000 7214 0000  ..rE...r9...r...
+00000a00: 0072 1400 0000 7215 0000 00da 0a63 6970  .r....r......cip
 00000a10: 6865 7274 6578 7441 0000 0073 0600 0000  hertextA...s....
 00000a20: 0001 1001 0aff 7a0e 456e 632e 6369 7068  ......z.Enc.ciph
 00000a30: 6572 7465 7874 6301 0000 0000 0000 0000  ertextc.........
 00000a40: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
 00000a50: 2c00 0000 7c00 6a00 7d01 7401 a002 7c01  ,...|.j.}.t...|.
 00000a60: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
 00000a70: a006 a100 a101 0100 7c01 a007 a100 5300  ........|.....S.
-00000a80: 7239 0000 0029 0872 2f00 0000 7208 0000  r9...).r/...r...
+00000a80: 7237 0000 0029 0872 2e00 0000 7208 0000  r7...).r....r...
 00000a90: 00da 0448 4d41 4372 0700 0000 da06 5348  ...HMACr......SH
-00000aa0: 4135 3132 7246 0000 0072 4900 0000 7247  A512rF...rI...rG
-00000ab0: 0000 00a9 0272 1200 0000 da01 6872 1500  .....r......hr..
-00000ac0: 0000 7215 0000 0072 1600 0000 724a 0000  ..r....r....rJ..
+00000aa0: 4135 3132 7244 0000 0072 4700 0000 7245  A512rD...rG...rE
+00000ab0: 0000 00a9 0272 1100 0000 da01 6872 1400  .....r......hr..
+00000ac0: 0000 7214 0000 0072 1500 0000 7248 0000  ..r....r....rH..
 00000ad0: 0045 0000 0073 0800 0000 0001 0601 1001  .E...s..........
 00000ae0: 0e01 7a08 456e 632e 484d 4143 6301 0000  ..z.Enc.HMACc...
 00000af0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 00000b00: 0043 0000 0073 1200 0000 7400 a001 6401  .C...s....t...d.
 00000b10: 7c00 6a02 a102 7d01 7c01 5300 2902 4efa  |.j...}.|.S.).N.
-00000b20: 0221 4929 03da 0673 7472 7563 745a 0470  .!I)...structZ.p
-00000b30: 6163 6b72 2c00 0000 2902 7212 0000 005a  ackr,...).r....Z
-00000b40: 0b69 7465 7273 5f62 7974 6573 7215 0000  .iters_bytesr...
-00000b50: 0072 1500 0000 7216 0000 00da 0f73 6574  .r....r......set
+00000b20: 0221 4929 03da 0673 7472 7563 74da 0470  .!I)...struct..p
+00000b30: 6163 6b72 2b00 0000 2902 7211 0000 005a  ackr+...).r....Z
+00000b40: 0b69 7465 7273 5f62 7974 6573 7214 0000  .iters_bytesr...
+00000b50: 0072 1400 0000 7215 0000 00da 0f73 6574  .r....r......set
 00000b60: 7570 4974 6572 6174 696f 6e73 4b00 0000  upIterationsK...
 00000b70: 7304 0000 0000 010e 017a 1345 6e63 2e73  s........z.Enc.s
 00000b80: 6574 7570 4974 6572 6174 696f 6e73 6301  etupIterationsc.
 00000b90: 0000 0000 0000 0000 0000 0001 0000 0003  ................
 00000ba0: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
 00000bb0: a100 7c00 6a01 1700 7c00 6a02 1700 7c00  ..|.j...|.j...|.
 00000bc0: 6a03 1700 7c00 a004 a100 1700 7c00 a005  j...|.......|...
-00000bd0: a100 1700 5300 7239 0000 0029 0672 4a00  ....S.r9...).rJ.
-00000be0: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
-00000bf0: 0072 5000 0000 7249 0000 0072 3b00 0000  .rP...rI...r;...
-00000c00: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000bd0: a100 1700 5300 7237 0000 0029 0672 4800  ....S.r7...).rH.
+00000be0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00000bf0: 0072 4f00 0000 7247 0000 0072 3900 0000  .rO...rG...r9...
+00000c00: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
 00000c10: 0a65 6e63 546f 4279 7465 734f 0000 0073  .encToBytesO...s
 00000c20: 0a00 0000 0001 1801 06ff 0201 06ff 7a0e  ..............z.
 00000c30: 456e 632e 656e 6354 6f42 7974 6573 6301  Enc.encToBytesc.
 00000c40: 0000 0000 0000 0000 0000 0001 0000 0004  ................
 00000c50: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
 00000c60: 7c00 a002 a100 a101 a003 6401 a101 5300  |.........d...S.
-00000c70: a902 4e72 3100 0000 2904 da06 6261 7365  ..Nr1...)...base
+00000c70: a902 4e72 3000 0000 2904 da06 6261 7365  ..Nr0...)...base
 00000c80: 3634 5a11 7572 6c73 6166 655f 6236 3465  64Z.urlsafe_b64e
-00000c90: 6e63 6f64 6572 5100 0000 da06 6465 636f  ncoderQ.....deco
-00000ca0: 6465 723b 0000 0072 1500 0000 7215 0000  der;...r....r...
-00000cb0: 0072 1600 0000 da08 656e 6354 6f53 7472  .r......encToStr
+00000c90: 6e63 6f64 6572 5000 0000 da06 6465 636f  ncoderP.....deco
+00000ca0: 6465 7239 0000 0072 1400 0000 7214 0000  der9...r....r...
+00000cb0: 0072 1500 0000 da08 656e 6354 6f53 7472  .r......encToStr
 00000cc0: 5300 0000 7302 0000 0000 017a 0c45 6e63  S...s......z.Enc
-00000cd0: 2e65 6e63 546f 5374 7229 1472 1700 0000  .encToStr).r....
-00000ce0: 7218 0000 0072 1900 0000 7209 0000 0072  r....r....r....r
-00000cf0: 2400 0000 7226 0000 0072 1100 0000 da0c  $...r&...r......
+00000cd0: 2e65 6e63 546f 5374 7229 1472 1600 0000  .encToStr).r....
+00000ce0: 7217 0000 0072 1800 0000 7209 0000 0072  r....r....r....r
+00000cf0: 2300 0000 7225 0000 0072 1000 0000 da0c  #...r%...r......
 00000d00: 7374 6174 6963 6d65 7468 6f64 da03 696e  staticmethod..in
-00000d10: 7472 2d00 0000 7238 0000 0072 3c00 0000  tr-...r8...r<...
-00000d20: 7240 0000 0072 4100 0000 7248 0000 0072  r@...rA...rH...r
-00000d30: 4900 0000 724a 0000 0072 5000 0000 7251  I...rJ...rP...rQ
-00000d40: 0000 0072 5500 0000 7215 0000 0072 1500  ...rU...r....r..
-00000d50: 0000 7215 0000 0072 1600 0000 721c 0000  ..r....r....r...
+00000d10: 7472 2c00 0000 7236 0000 0072 3a00 0000  tr,...r6...r:...
+00000d20: 723e 0000 0072 3f00 0000 7246 0000 0072  r>...r?...rF...r
+00000d30: 4700 0000 7248 0000 0072 4f00 0000 7250  G...rH...rO...rP
+00000d40: 0000 0072 5400 0000 7214 0000 0072 1400  ...rT...r....r..
+00000d50: 0000 7214 0000 0072 1500 0000 721b 0000  ..r....r....r...
 00000d60: 0013 0000 0073 1c00 0000 0801 1a10 0201  .....s..........
 00000d70: 1607 0201 1003 0803 0807 0803 0e04 0e04  ................
-00000d80: 0e06 0e04 0e04 721c 0000 0063 0000 0000  ......r....c....
+00000d80: 0e06 0e04 0e04 721b 0000 0063 0000 0000  ......r....c....
 00000d90: 0000 0000 0000 0000 0000 0000 0400 0000  ................
 00000da0: 0000 0000 7322 0000 0065 005a 0164 005a  ....s"...e.Z.d.Z
 00000db0: 0264 0164 029c 0187 0066 0164 0364 0484  .d.d.....f.d.d..
 00000dc0: 0c5a 0387 0004 005a 0453 0029 05da 154d  .Z.....Z.S.)...M
 00000dd0: 6573 7361 6765 5461 6d70 6572 696e 6745  essageTamperingE
-00000de0: 7272 6f72 4e72 3500 0000 6301 0000 0000  rrorNr5...c.....
+00000de0: 7272 6f72 4e72 3400 0000 6301 0000 0000  rrorNr4...c.....
 00000df0: 0000 0000 0000 0001 0000 0003 0000 0003  ................
 00000e00: 0000 0073 1800 0000 6401 7c00 5f00 7401  ...s....d.|._.t.
 00000e10: 8300 a002 7c00 6a00 a101 0100 6400 5300  ....|.j.....d.S.
 00000e20: 2902 4e7a 4c48 4d41 4320 6d69 736d 6174  ).NzLHMAC mismat
 00000e30: 6368 2021 204d 6573 7361 6765 2068 6173  ch ! Message has
 00000e40: 2062 6565 6e20 5441 4d50 4552 4544 2077   been TAMPERED w
 00000e50: 6974 6820 2c0a 206f 7220 506f 7373 6962  ith ,. or Possib
 00000e60: 6c65 206b 6579 2064 6966 6665 7265 6e63  le key differenc
-00000e70: 6572 0e00 0000 723b 0000 0072 1300 0000  er....r;...r....
-00000e80: 7215 0000 0072 1600 0000 7211 0000 0058  r....r....r....X
+00000e70: 6572 0e00 0000 7239 0000 0072 1200 0000  er....r9...r....
+00000e80: 7214 0000 0072 1500 0000 7210 0000 0058  r....r....r....X
 00000e90: 0000 0073 0400 0000 0001 0601 7a1e 4d65  ...s........z.Me
 00000ea0: 7373 6167 6554 616d 7065 7269 6e67 4572  ssageTamperingEr
-00000eb0: 726f 722e 5f5f 696e 6974 5f5f 2905 7217  ror.__init__).r.
-00000ec0: 0000 0072 1800 0000 7219 0000 0072 1100  ...r....r....r..
-00000ed0: 0000 721b 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000ee0: 0072 1300 0000 7216 0000 0072 5800 0000  .r....r....rX...
-00000ef0: 5700 0000 7302 0000 0008 0172 5800 0000  W...s......rX...
+00000eb0: 726f 722e 5f5f 696e 6974 5f5f 2905 7216  ror.__init__).r.
+00000ec0: 0000 0072 1700 0000 7218 0000 0072 1000  ...r....r....r..
+00000ed0: 0000 721a 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00000ee0: 0072 1200 0000 7215 0000 0072 5700 0000  .r....r....rW...
+00000ef0: 5700 0000 7302 0000 0008 0172 5700 0000  W...s......rW...
 00000f00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000f10: 0004 0000 0040 0000 0073 9200 0000 6500  .....@...s....e.
 00000f20: 5a01 6400 5a02 6503 6504 6505 6602 1900  Z.d.Z.e.e.e.f...
 00000f30: 6504 6401 6402 9c03 6403 6404 8404 5a06  e.d.d...d.d...Z.
 00000f40: 6505 6405 9c01 6406 6407 8404 5a07 6508  e.d...d.d...Z.e.
 00000f50: 6405 9c01 6408 6409 8404 5a09 640a 640b  d...d.d...Z.d.d.
 00000f60: 8400 5a0a 640c 640d 8400 5a0b 640e 640f  ..Z.d.d...Z.d.d.
 00000f70: 8400 5a0c 6505 6405 9c01 6410 6411 8404  ..Z.e.d...d.d...
 00000f80: 5a0d 6505 6405 9c01 6412 6413 8404 5a0e  Z.e.d...d.d...Z.
 00000f90: 6505 6405 9c01 6414 6415 8404 5a0f 6504  e.d...d.d...Z.e.
 00000fa0: 6405 9c01 6416 6417 8404 5a10 6401 5300  d...d.d...Z.d.S.
-00000fb0: 2918 da03 4465 634e 721d 0000 0063 0300  )...DecNr....c..
+00000fb0: 2918 da03 4465 634e 721c 0000 0063 0300  )...DecNr....c..
 00000fc0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
 00000fd0: 0000 4300 0000 7306 0100 0074 007c 0174  ..C...s....t.|.t
 00000fe0: 0183 0272 227c 01a0 0264 01a1 017d 0374  ...r"|...d...}.t
 00000ff0: 03a0 047c 03a1 017c 005f 056e 1074 007c  ...|...|._.n.t.|
 00001000: 0174 0683 0272 327c 017c 005f 057c 027c  .t...r2|.|._.|.|
 00001010: 005f 077c 006a 0564 0064 0285 0219 007c  ._.|.j.d.d.....|
 00001020: 005f 087c 006a 0564 0264 0385 0219 007c  ._.|.j.d.d.....|
@@ -264,136 +264,136 @@
 00001070: 006a 0e64 096b 0073 a87c 006a 0e64 0a6b  .j.d.k.s.|.j.d.k
 00001080: 0472 b274 0f7c 006a 0e83 0182 017c 006a  .r.t.|.j.....|.j
 00001090: 0564 0764 0085 0219 007c 005f 1074 11a0  .d.d.....|._.t..
 000010a0: 127c 006a 077c 006a 0a7c 006a 0ea1 037c  .|.j.|.j.|.j...|
 000010b0: 005f 1374 11a0 127c 006a 077c 006a 0b7c  ._.t...|.j.|.j.|
 000010c0: 006a 0ea1 037c 005f 147c 00a0 15a1 0064  .j...|._.|.....d
 000010d0: 0b75 0090 0172 0274 1683 0082 0164 0053  .u...r.t.....d.S
-000010e0: 0029 0c4e 7231 0000 0072 3600 0000 e950  .).Nr1...r6....P
-000010f0: 0000 00e9 6000 0000 e970 0000 0072 4e00  ....`....p...rN.
-00001100: 0000 e974 0000 0072 0100 0000 7221 0000  ...t...r....r!..
-00001110: 0072 2200 0000 4629 1772 2300 0000 7224  .r"...F).r#...r$
-00001120: 0000 0072 2500 0000 7253 0000 005a 1175  ...r%...rS...Z.u
+000010e0: 0029 0c4e 7230 0000 00e9 4000 0000 e950  .).Nr0....@....P
+000010f0: 0000 00e9 6000 0000 e970 0000 0072 4c00  ....`....p...rL.
+00001100: 0000 e974 0000 0072 0100 0000 7220 0000  ...t...r....r ..
+00001110: 0072 2100 0000 4629 1772 2200 0000 7223  .r!...F).r"...r#
+00001120: 0000 0072 2400 0000 7252 0000 005a 1175  ...r$...rR...Z.u
 00001130: 726c 7361 6665 5f62 3634 6465 636f 6465  rlsafe_b64decode
-00001140: 721e 0000 0072 2600 0000 723e 0000 00da  r....r&...r>....
+00001140: 721d 0000 0072 2500 0000 723c 0000 00da  r....r%...r<....
 00001150: 0872 6563 5f68 6d61 63da 0672 6563 5f69  .rec_hmac..rec_i
-00001160: 765a 0872 6563 5f73 616c 745a 0a72 6563  vZ.rec_saltZ.rec
-00001170: 5f70 6570 7065 7272 4f00 0000 5a06 756e  _pepperrO...Z.un
-00001180: 7061 636b 5a0e 7265 635f 6974 6572 6174  packZ.rec_iterat
+00001160: 76da 0872 6563 5f73 616c 74da 0a72 6563  v..rec_salt..rec
+00001170: 5f70 6570 7065 7272 4d00 0000 da06 756e  _pepperrM.....un
+00001180: 7061 636b da0e 7265 635f 6974 6572 6174  pack..rec_iterat
 00001190: 696f 6e73 720a 0000 00da 0e72 6563 5f63  ionsr......rec_c
-000011a0: 6970 6865 7274 6578 7472 1c00 0000 722d  iphertextr....r-
+000011a0: 6970 6865 7274 6578 7472 1b00 0000 722c  iphertextr....r,
 000011b0: 0000 00da 0664 6563 4b65 79da 0668 6d61  .....decKey..hma
 000011c0: 635f 6bda 0a76 6572 6966 7948 4d41 4372  c_k..verifyHMACr
-000011d0: 5800 0000 2904 7212 0000 0072 1e00 0000  X...).r....r....
-000011e0: 721f 0000 00da 016d 7215 0000 0072 1500  r......mr....r..
-000011f0: 0000 7216 0000 0072 1100 0000 5e00 0000  ..r....r....^...
+000011d0: 5700 0000 2904 7211 0000 0072 1d00 0000  W...).r....r....
+000011e0: 721e 0000 00da 016d 7214 0000 0072 1400  r......mr....r..
+000011f0: 0000 7215 0000 0072 1000 0000 5e00 0000  ..r....r....^...
 00001200: 732c 0000 0000 010a 010a 010e 010a 0106  s,..............
 00001210: 0106 0110 0110 0110 0110 011c 0114 010a  ................
 00001220: 0110 0116 0104 0104 0104 0104 fd06 040e  ................
 00001230: 017a 0c44 6563 2e5f 5f69 6e69 745f 5f72  .z.Dec.__init__r
-00001240: 3500 0000 6301 0000 0000 0000 0000 0000  5...c...........
+00001240: 3400 0000 6301 0000 0000 0000 0000 0000  4...c...........
 00001250: 0002 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
 00001260: 0000 7c00 6a00 7d01 7401 a002 7c01 7403  ..|.j.}.t...|.t.
 00001270: a004 a100 a102 7d01 7c01 a005 7c00 6a06  ......}.|...|.j.
-00001280: a101 0100 7c01 a007 a100 5300 7239 0000  ....|.....S.r9..
-00001290: 0029 0872 6200 0000 7208 0000 0072 4a00  .).rb...r....rJ.
-000012a0: 0000 7207 0000 0072 4b00 0000 7246 0000  ..r....rK...rF..
-000012b0: 0072 6000 0000 7247 0000 0072 4c00 0000  .r`...rG...rL...
-000012c0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00001280: a101 0100 7c01 a007 a100 5300 7237 0000  ....|.....S.r7..
+00001290: 0029 0872 6600 0000 7208 0000 0072 4800  .).rf...r....rH.
+000012a0: 0000 7207 0000 0072 4900 0000 7244 0000  ..r....rI...rD..
+000012b0: 0072 6400 0000 7245 0000 0072 4a00 0000  .rd...rE...rJ...
+000012c0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
 000012d0: 0a61 6374 7561 6c48 4d41 4375 0000 0073  .actualHMACu...s
 000012e0: 0800 0000 0001 0601 1001 0c01 7a0e 4465  ............z.De
 000012f0: 632e 6163 7475 616c 484d 4143 6301 0000  c.actualHMACc...
 00001300: 0000 0000 0000 0000 0001 0000 0004 0000  ................
 00001310: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
-00001320: a002 a100 7c00 6a03 a102 5300 7239 0000  ....|.j...S.r9..
+00001320: a002 a100 7c00 6a03 a102 5300 7237 0000  ....|.j...S.r7..
 00001330: 0029 04da 0368 6d63 5a0e 636f 6d70 6172  .)...hmcZ.compar
-00001340: 655f 6469 6765 7374 7265 0000 0072 5e00  e_digestre...r^.
-00001350: 0000 723b 0000 0072 1500 0000 7215 0000  ..r;...r....r...
-00001360: 0072 1600 0000 7263 0000 007b 0000 0073  .r....rc...{...s
+00001340: 655f 6469 6765 7374 7269 0000 0072 5e00  e_digestri...r^.
+00001350: 0000 7239 0000 0072 1400 0000 7214 0000  ..r9...r....r...
+00001360: 0072 1500 0000 7267 0000 007b 0000 0073  .r....rg...{...s
 00001370: 0200 0000 0001 7a0e 4465 632e 7665 7269  ......z.Dec.veri
 00001380: 6679 484d 4143 6301 0000 0000 0000 0000  fyHMACc.........
 00001390: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
 000013a0: 0c00 0000 7400 a001 7c00 6a02 a101 5300  ....t...|.j...S.
-000013b0: 7239 0000 0029 0372 0400 0000 723a 0000  r9...).r....r:..
-000013c0: 0072 5f00 0000 723b 0000 0072 1500 0000  .r_...r;...r....
-000013d0: 7215 0000 0072 1600 0000 723c 0000 007e  r....r....r<...~
+000013b0: 7237 0000 0029 0372 0400 0000 7238 0000  r7...).r....r8..
+000013c0: 0072 5f00 0000 7239 0000 0072 1400 0000  .r_...r9...r....
+000013d0: 7214 0000 0072 1500 0000 723a 0000 007e  r....r....r:...~
 000013e0: 0000 0073 0200 0000 0001 7a08 4465 632e  ...s......z.Dec.
 000013f0: 6d6f 6465 6301 0000 0000 0000 0000 0000  modec...........
 00001400: 0001 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
 00001410: 0000 7400 7401 6a02 7c00 6a03 6401 8d01  ..t.t.j.|.j.d...
 00001420: 7c00 a004 a100 7405 8300 6402 8d03 5300  |.....t...d...S.
-00001430: 723d 0000 0029 0672 0200 0000 7203 0000  r=...).r....r...
-00001440: 0072 3f00 0000 7261 0000 0072 3c00 0000  .r?...ra...r<...
-00001450: 7206 0000 0072 3b00 0000 7215 0000 0072  r....r;...r....r
-00001460: 1500 0000 7216 0000 0072 4000 0000 8100  ....r....r@.....
+00001430: 723b 0000 0029 0672 0200 0000 7203 0000  r;...).r....r...
+00001440: 0072 3d00 0000 7265 0000 0072 3a00 0000  .r=...re...r:...
+00001450: 7206 0000 0072 3900 0000 7214 0000 0072  r....r9...r....r
+00001460: 1400 0000 7215 0000 0072 3e00 0000 8100  ....r....r>.....
 00001470: 0000 730e 0000 0000 0102 0104 0104 ff04  ..s.............
 00001480: 0206 0104 fc7a 0a44 6563 2e63 6970 6865  .....z.Dec.ciphe
 00001490: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
 000014a0: 0000 0200 0000 4300 0000 730c 0000 007c  ......C...s....|
-000014b0: 00a0 00a1 00a0 01a1 0053 0072 3900 0000  .........S.r9...
-000014c0: 2902 7240 0000 005a 0964 6563 7279 7074  ).r@...Z.decrypt
-000014d0: 6f72 723b 0000 0072 1500 0000 7215 0000  orr;...r....r...
-000014e0: 0072 1600 0000 da10 6369 7068 6572 5f64  .r......cipher_d
+000014b0: 00a0 00a1 00a0 01a1 0053 0072 3700 0000  .........S.r7...
+000014c0: 2902 723e 0000 005a 0964 6563 7279 7074  ).r>...Z.decrypt
+000014d0: 6f72 7239 0000 0072 1400 0000 7214 0000  orr9...r....r...
+000014e0: 0072 1500 0000 da10 6369 7068 6572 5f64  .r......cipher_d
 000014f0: 6563 7279 7074 6f72 8800 0000 7302 0000  ecryptor....s...
 00001500: 0000 017a 1444 6563 2e63 6970 6865 725f  ...z.Dec.cipher_
 00001510: 6465 6372 7970 746f 7263 0100 0000 0000  decryptorc......
 00001520: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
 00001530: 0000 731c 0000 007c 00a0 00a1 00a0 017c  ..s....|.......|
 00001540: 006a 02a1 017c 00a0 00a1 00a0 03a1 0017  .j...|..........
-00001550: 0053 0072 3900 0000 2904 7267 0000 0072  .S.r9...).rg...r
-00001560: 4600 0000 7260 0000 0072 4700 0000 723b  F...r`...rG...r;
-00001570: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00001550: 0053 0072 3700 0000 2904 726b 0000 0072  .S.r7...).rk...r
+00001560: 4400 0000 7264 0000 0072 4500 0000 7239  D...rd...rE...r9
+00001570: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
 00001580: 0000 da11 7072 655f 756e 7061 6464 696e  ....pre_unpaddin
 00001590: 675f 6465 638b 0000 0073 0600 0000 0001  g_dec....s......
 000015a0: 0e01 0aff 7a15 4465 632e 7072 655f 756e  ....z.Dec.pre_un
 000015b0: 7061 6464 696e 675f 6465 6363 0100 0000  padding_decc....
 000015c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 000015d0: 4300 0000 7324 0000 0074 00a0 0164 01a1  C...s$...t...d..
 000015e0: 01a0 02a1 007d 017c 01a0 037c 00a0 04a1  .....}.|...|....
-000015f0: 00a1 017c 01a0 05a1 0017 0053 0072 4200  ...|.......S.rB.
-00001600: 0000 2906 7205 0000 0072 4400 0000 da08  ..).r....rD.....
-00001610: 756e 7061 6464 6572 7246 0000 0072 6800  unpadderrF...rh.
-00001620: 0000 7247 0000 0029 0272 1200 0000 7269  ..rG...).r....ri
-00001630: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000015f0: 00a1 017c 01a0 05a1 0017 0053 0072 4000  ...|.......S.r@.
+00001600: 0000 2906 7205 0000 0072 4200 0000 da08  ..).r....rB.....
+00001610: 756e 7061 6464 6572 7244 0000 0072 6c00  unpadderrD...rl.
+00001620: 0000 7245 0000 0029 0272 1100 0000 726d  ..rE...).r....rm
+00001630: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
 00001640: 0000 da0a 756e 7061 6464 6564 5f6d 8f00  ....unpadded_m..
 00001650: 0000 7304 0000 0000 010e 017a 0e44 6563  ..s........z.Dec
 00001660: 2e75 6e70 6164 6465 645f 6d63 0100 0000  .unpadded_mc....
 00001670: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00001680: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
-00001690: 0072 3900 0000 2901 726a 0000 0072 3b00  .r9...).rj...r;.
-000016a0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00001690: 0072 3700 0000 2901 726e 0000 0072 3900  .r7...).rn...r9.
+000016a0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
 000016b0: 00da 0a64 6563 546f 4279 7465 7393 0000  ...decToBytes...
 000016c0: 0073 0200 0000 0001 7a0e 4465 632e 6465  .s......z.Dec.de
 000016d0: 6354 6f42 7974 6573 6301 0000 0000 0000  cToBytesc.......
 000016e0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
 000016f0: 0073 0e00 0000 7c00 a000 a100 a001 6401  .s....|.......d.
-00001700: a101 5300 7252 0000 0029 0272 6a00 0000  ..S.rR...).rj...
-00001710: 7254 0000 0072 3b00 0000 7215 0000 0072  rT...r;...r....r
-00001720: 1500 0000 7216 0000 00da 0864 6563 546f  ....r......decTo
+00001700: a101 5300 7251 0000 0029 0272 6e00 0000  ..S.rQ...).rn...
+00001710: 7253 0000 0072 3900 0000 7214 0000 0072  rS...r9...r....r
+00001720: 1400 0000 7215 0000 00da 0864 6563 546f  ....r......decTo
 00001730: 5374 7296 0000 0073 0200 0000 0001 7a0c  Str....s......z.
-00001740: 4465 632e 6465 6354 6f53 7472 2911 7217  Dec.decToStr).r.
-00001750: 0000 0072 1800 0000 7219 0000 0072 0900  ...r....r....r..
-00001760: 0000 7224 0000 0072 2600 0000 7211 0000  ..r$...r&...r...
-00001770: 0072 6500 0000 da04 626f 6f6c 7263 0000  .re.....boolrc..
-00001780: 0072 3c00 0000 7240 0000 0072 6700 0000  .r<...r@...rg...
-00001790: 7268 0000 0072 6a00 0000 726b 0000 0072  rh...rj...rk...r
-000017a0: 6c00 0000 7215 0000 0072 1500 0000 7215  l...r....r....r.
-000017b0: 0000 0072 1600 0000 7259 0000 005d 0000  ...r....rY...]..
+00001740: 4465 632e 6465 6354 6f53 7472 2911 7216  Dec.decToStr).r.
+00001750: 0000 0072 1700 0000 7218 0000 0072 0900  ...r....r....r..
+00001760: 0000 7223 0000 0072 2500 0000 7210 0000  ..r#...r%...r...
+00001770: 0072 6900 0000 da04 626f 6f6c 7267 0000  .ri.....boolrg..
+00001780: 0072 3a00 0000 723e 0000 0072 6b00 0000  .r:...r>...rk...
+00001790: 726c 0000 0072 6e00 0000 726f 0000 0072  rl...rn...ro...r
+000017a0: 7000 0000 7214 0000 0072 1400 0000 7214  p...r....r....r.
+000017b0: 0000 0072 1500 0000 7258 0000 005d 0000  ...r....rX...]..
 000017c0: 0073 1400 0000 0801 1a17 0e06 0e03 0803  .s..............
-000017d0: 0807 0803 0e04 0e04 0e03 7259 0000 0029  ..........rY...)
+000017d0: 0807 0803 0e04 0e04 0e03 7258 0000 0029  ..........rX...)
 000017e0: 165a 2663 7279 7074 6f67 7261 7068 792e  .Z&cryptography.
 000017f0: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
 00001800: 732e 6369 7068 6572 7372 0200 0000 7203  s.ciphersr....r.
 00001810: 0000 0072 0400 0000 5a1e 6372 7970 746f  ...r....Z.crypto
 00001820: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
 00001830: 696d 6974 6976 6573 7205 0000 005a 1c63  imitivesr....Z.c
 00001840: 7279 7074 6f67 7261 7068 792e 6861 7a6d  ryptography.hazm
 00001850: 6174 2e62 6163 6b65 6e64 7372 0600 0000  at.backendsr....
 00001860: 7207 0000 0072 0800 0000 da06 7479 7069  r....r......typi
-00001870: 6e67 7209 0000 0072 6600 0000 7234 0000  ngr....rf...r4..
-00001880: 0072 5300 0000 724f 0000 0072 2700 0000  .rS...rO...r'...
+00001870: 6e67 7209 0000 0072 6a00 0000 7233 0000  ngr....rj...r3..
+00001880: 0072 5200 0000 724d 0000 0072 2600 0000  .rR...rM...r&...
 00001890: da09 4578 6365 7074 696f 6e72 0a00 0000  ..Exceptionr....
-000018a0: 721c 0000 0072 5800 0000 7259 0000 0072  r....rX...rY...r
-000018b0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000018a0: 721b 0000 0072 5700 0000 7258 0000 0072  r....rW...rX...r
+000018b0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
 000018c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 000018d0: 0073 1a00 0000 1401 0c01 0c01 1001 0c01  .s..............
 000018e0: 0801 0801 0801 0801 0803 1006 0e44 1006  .............D..
```

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Jul  3 21:05:38 2023 UTC, .py size: 8450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2238 a364 0221 0000  a......."8.d.!..
+00000000: 610d 0d0a 0000 0000 3734 ab64 2123 0000  a.......74.d!#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 5a06 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c07 5a07 6501 4700 6405 6406 8400  d.l.Z.e.G.d.d...
 00000070: 6406 8302 8301 5a08 6404 5300 2907 e900  d.....Z.d.S.)...
@@ -40,15 +40,15 @@
 00000270: da07 7371 6c69 7465 33da 0763 6f6e 6e65  ..sqlite3..conne
 00000280: 6374 7207 0000 0072 0c00 0000 5a06 6375  ctr....r....Z.cu
 00000290: 7273 6f72 720d 0000 00a9 01da 0473 656c  rsorr........sel
 000002a0: 66a9 0072 1200 0000 fa2f 433a 5c57 6f72  f..r...../C:\Wor
 000002b0: 6b5c 4769 7448 7562 576f 726b 5c41 4553  k\GitHubWork\AES
 000002c0: 2d32 3536 5c41 7368 4372 7970 745c 4461  -256\AshCrypt\Da
 000002d0: 7461 6261 7365 2e70 79da 0d5f 5f70 6f73  tabase.py..__pos
-000002e0: 745f 696e 6974 5f5f 0e00 0000 7304 0000  t_init__....s...
+000002e0: 745f 696e 6974 5f5f 0f00 0000 7304 0000  t_init__....s...
 000002f0: 0000 010e 017a 1644 6174 6162 6173 652e  .....z.Database.
 00000300: 5f5f 706f 7374 5f69 6e69 745f 5f63 0100  __post_init__c..
 00000310: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
 00000320: 0000 4300 0000 738a 0000 007a 567c 006a  ..C...s....zV|.j
 00000330: 008f 3c01 007c 006a 01a0 0264 01a1 0101  ..<..|.j...d....
 00000340: 007c 006a 01a0 03a1 007d 017c 0164 0219  .|.j.....}.|.d..
 00000350: 0064 031b 0064 031b 007d 027c 0257 0002  .d...d...}.|.W..
@@ -64,393 +64,398 @@
 000003f0: 202c 2070 7261 676d 615f 7061 6765 5f73   , pragma_page_s
 00000400: 697a 6572 0100 0000 6900 0400 0029 0672  izer....i....).r
 00000410: 0c00 0000 720d 0000 00da 0765 7865 6375  ....r......execu
 00000420: 7465 da08 6665 7463 686f 6e65 720e 0000  te..fetchoner...
 00000430: 00da 0545 7272 6f72 2904 7211 0000 005a  ...Error).r....Z
 00000440: 0973 697a 655f 696e 666f da04 7369 7a65  .size_info..size
 00000450: da01 6572 1200 0000 7212 0000 0072 1300  ..er....r....r..
-00000460: 0000 7218 0000 0012 0000 0073 1000 0000  ..r........s....
-00000470: 0002 0201 0801 0c01 0a01 1001 2801 1001  ............(...
-00000480: 7a0d 4461 7461 6261 7365 2e73 697a 6529  z.Database.size)
-00000490: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
-000004a0: 0000 0000 0000 0300 0000 0a00 0000 4300  ..............C.
-000004b0: 0000 734c 0000 007a 1a74 00a0 0174 02a0  ..sL...z.t...t..
-000004c0: 037c 006a 04a1 016a 05a1 017d 017c 0157  .|.j...j...}.|.W
-000004d0: 0053 0004 0074 0679 4601 007d 0201 007a  .S...t.yF..}...z
-000004e0: 1464 017c 0266 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
-000004f0: 027e 0253 0064 007d 027e 0230 0030 0064  .~.S.d.}.~.0.0.d
-00000500: 0053 0029 024e 7201 0000 0029 0772 0400  .S.).Nr....).r..
-00000510: 0000 da0d 6672 6f6d 7469 6d65 7374 616d  ....fromtimestam
-00000520: 70da 026f 73da 0473 7461 7472 0700 0000  p..os..statr....
-00000530: da08 7374 5f6d 7469 6d65 da07 4f53 4572  ..st_mtime..OSEr
-00000540: 726f 7229 0372 1100 0000 5a09 7469 6d65  ror).r....Z.time
-00000550: 5f73 7461 7472 1900 0000 7212 0000 0072  _statr....r....r
-00000560: 1200 0000 7213 0000 00da 086c 6173 745f  ....r......last_
-00000570: 6d6f 641d 0000 0073 0a00 0000 0002 0201  mod....s........
-00000580: 1401 0602 0e01 7a11 4461 7461 6261 7365  ......z.Database
-00000590: 2e6c 6173 745f 6d6f 6463 0100 0000 0000  .last_modc......
-000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000005b0: 0000 730e 0000 0064 017c 006a 009b 0064  ..s....d.|.j...d
-000005c0: 029d 0353 0029 034e 7a20 4445 4641 554c  ...S.).Nz DEFAUL
-000005d0: 5420 524f 5554 494e 4720 414c 4c20 4d45  T ROUTING ALL ME
-000005e0: 5448 4f44 5320 544f 2022 fa01 2229 0172  THODS TO "..").r
-000005f0: 0900 0000 7210 0000 0072 1200 0000 7212  ....r....r....r.
-00000600: 0000 0072 1300 0000 da0f 6465 6661 756c  ...r......defaul
-00000610: 745f 726f 7574 696e 6726 0000 0073 0200  t_routing&...s..
-00000620: 0000 0002 7a18 4461 7461 6261 7365 2e64  ....z.Database.d
-00000630: 6566 6175 6c74 5f72 6f75 7469 6e67 2902  efault_routing).
-00000640: da06 7175 6572 7973 721a 0000 0063 0100  ..querysr....c..
-00000650: 0000 0000 0000 0000 0000 0600 0000 0b00  ................
-00000660: 0000 4700 0000 7300 0100 0067 007d 0274  ..G...s....g.}.t
-00000670: 007c 0183 0144 005d ee5c 027d 037d 0474  .|...D.].\.}.}.t
-00000680: 017c 0474 0283 0273 367c 02a0 0364 017c  .|.t...s6|...d.|
-00000690: 039b 009d 0264 0274 0466 0269 01a1 0101  .....d.t.f.i....
-000006a0: 007a 807c 006a 058f 6601 007c 006a 06a0  .z.|.j..f..|.j..
-000006b0: 077c 04a1 0101 007c 006a 066a 0864 036b  .|.....|.j.j.d.k
-000006c0: 0272 787c 02a0 0364 017c 039b 009d 0264  .rx|...d.|.....d
-000006d0: 047c 006a 06a0 09a1 0067 0269 01a1 0101  .|.j.....g.i....
-000006e0: 006e 1e7c 02a0 0364 017c 039b 009d 0264  .n.|...d.|.....d
-000006f0: 047c 006a 06a0 0aa1 0067 0269 01a1 0101  .|.j.....g.i....
-00000700: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00000710: 0073 aa30 0001 0001 0001 0059 0001 0057  .s.0.......Y...W
-00000720: 0071 0c04 0074 0b6a 0c79 f801 007d 0501  .q...t.j.y...}..
-00000730: 007a 287c 02a0 0364 017c 039b 009d 0264  .z(|...d.|.....d
-00000740: 057c 05a0 0da1 0066 0269 01a1 0101 0057  .|.....f.i.....W
-00000750: 0059 0064 007d 057e 0571 0c64 007d 057e  .Y.d.}.~.q.d.}.~
-00000760: 0530 0030 0071 0c7c 0253 0029 064e 7a06  .0.0.q.|.S.).Nz.
-00000770: 7175 6572 7920 e700 0000 0000 0000 00e9  query ..........
-00000780: 0100 0000 da07 5355 4343 4553 53da 0746  ......SUCCESS..F
-00000790: 4149 4c55 5245 290e da09 656e 756d 6572  AILURE)...enumer
-000007a0: 6174 65da 0a69 7369 6e73 7461 6e63 65da  ate..isinstance.
-000007b0: 0373 7472 da06 6170 7065 6e64 da09 5479  .str..append..Ty
-000007c0: 7065 4572 726f 7272 0c00 0000 720d 0000  peErrorr....r...
-000007d0: 0072 1500 0000 5a08 726f 7763 6f75 6e74  .r....Z.rowcount
-000007e0: 7216 0000 00da 0866 6574 6368 616c 6c72  r......fetchallr
-000007f0: 0e00 0000 7217 0000 00da 075f 5f73 7472  ....r......__str
-00000800: 5f5f 2906 7211 0000 0072 2300 0000 da06  __).r....r#.....
-00000810: 7265 7375 6c74 da01 69da 0571 7565 7279  result..i..query
-00000820: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000830: 1300 0000 7231 0000 002a 0000 0073 1a00  ....r1...*...s..
-00000840: 0000 0001 0401 1001 0a01 1801 0201 0801  ................
-00000850: 0c01 0c01 2002 4002 1001 3401 7a0e 4461  .... .@...4.z.Da
-00000860: 7461 6261 7365 2e71 7565 7279 4e63 0200  tabase.queryNc..
-00000870: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
-00000880: 0000 4300 0000 73f8 0000 007c 0164 0075  ..C...s....|.d.u
-00000890: 0072 7c7a 427c 006a 008f 2601 007c 006a  .r|zB|.j..&..|.j
-000008a0: 01a0 0264 017c 006a 039b 0064 029d 03a1  ...d.|.j...d....
-000008b0: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000008c0: 1031 0073 3c30 0001 0001 0001 0059 0001  .1.s<0.......Y..
-000008d0: 0057 0064 0353 0004 0074 046a 0579 7801  .W.d.S...t.j.yx.
-000008e0: 007d 0201 007a 1464 047c 0266 0257 0006  .}...z.d.|.f.W..
-000008f0: 0059 0064 007d 027e 0253 0064 007d 027e  .Y.d.}.~.S.d.}.~
-00000900: 0230 0030 006e 787a 467c 006a 008f 2a01  .0.0.nxzF|.j..*.
-00000910: 007c 006a 01a0 0264 017c 019b 0064 059d  .|.j...d.|...d..
-00000920: 03a1 0101 007c 017c 005f 0357 0064 0004  .....|.|._.W.d..
-00000930: 0004 0083 0301 006e 1031 0073 b430 0001  .......n.1.s.0..
-00000940: 0001 0001 0059 0001 0057 0064 0653 0004  .....Y...W.d.S..
-00000950: 0074 046a 0590 0079 f201 007d 0201 007a  .t.j...y...}...z
-00000960: 1464 077c 0266 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
-00000970: 027e 0253 0064 007d 027e 0230 0030 0064  .~.S.d.}.~.0.0.d
-00000980: 0053 0029 084e 7a1b 4352 4541 5445 2054  .S.).Nz.CREATE T
-00000990: 4142 4c45 2049 4620 4e4f 5420 4558 4953  ABLE IF NOT EXIS
-000009a0: 5453 207a 3e20 2849 4420 494e 5445 4745  TS z> (ID INTEGE
-000009b0: 5220 5052 494d 4152 5920 4b45 592c 204e  R PRIMARY KEY, N
-000009c0: 616d 6520 5465 7874 202c 2043 6f6e 7465  ame Text , Conte
-000009d0: 6e74 2042 4c4f 4220 2c4b 6579 2054 4558  nt BLOB ,Key TEX
-000009e0: 5420 29e9 0b00 0000 7224 0000 007a 3c20  T ).....r$...z< 
-000009f0: 2849 4420 494e 5445 4745 5220 5052 494d  (ID INTEGER PRIM
-00000a00: 4152 5920 4b45 592c 4e61 6d65 2054 4558  ARY KEY,Name TEX
-00000a10: 5420 2c43 6f6e 7465 6e74 2042 4c4f 4220  T ,Content BLOB 
-00000a20: 2c4b 6579 2054 4558 5420 2972 2500 0000  ,Key TEXT )r%...
-00000a30: 7201 0000 00a9 0672 0c00 0000 720d 0000  r......r....r...
-00000a40: 0072 1500 0000 7209 0000 0072 0e00 0000  .r....r....r....
-00000a50: 7217 0000 0029 0372 1100 0000 da12 6f70  r....).r......op
-00000a60: 7469 6f6e 616c 5f74 6162 6c65 6e61 6d65  tional_tablename
-00000a70: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000a80: 1300 0000 da08 6164 6474 6162 6c65 3b00  ......addtable;.
-00000a90: 0000 731c 0000 0000 0108 0102 0108 0134  ..s............4
-00000aa0: 0206 0110 0120 0302 0108 0114 0524 0106  ..... .......$..
-00000ab0: 0212 017a 1144 6174 6162 6173 652e 6164  ...z.Database.ad
-00000ac0: 6474 6162 6c65 6305 0000 0000 0000 0000  dtablec.........
-00000ad0: 0000 0006 0000 000a 0000 0043 0000 0073  ...........C...s
-00000ae0: 0201 0000 7c04 6400 7500 7284 7a4a 7c00  ....|.d.u.r.zJ|.
-00000af0: 6a00 8f2e 0100 7c00 6a01 a002 6401 7c00  j.....|.j...d.|.
-00000b00: 6a03 9b00 6402 9d03 7c01 7c02 7c03 6603  j...d...|.|.|.f.
-00000b10: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000b20: 6e10 3100 7344 3000 0100 0100 0100 5900  n.1.sD0.......Y.
-00000b30: 0100 5700 6403 5300 0400 7404 6a05 7980  ..W.d.S...t.j.y.
-00000b40: 0100 7d05 0100 7a14 6404 7c05 6602 5700  ..}...z.d.|.f.W.
-00000b50: 0600 5900 6400 7d05 7e05 5300 6400 7d05  ..Y.d.}.~.S.d.}.
-00000b60: 7e05 3000 3000 6e7a 7a48 7c00 6a00 8f2c  ~.0.0.nzzH|.j..,
-00000b70: 0100 7c00 6a01 a002 6401 7c04 9b00 6405  ..|.j...d.|...d.
-00000b80: 9d03 7c01 7c02 7c03 6603 a102 0100 5700  ..|.|.|.f.....W.
-00000b90: 6400 0400 0400 8303 0100 6e10 3100 73be  d.........n.1.s.
-00000ba0: 3000 0100 0100 0100 5900 0100 5700 6406  0.......Y...W.d.
-00000bb0: 5300 0400 7404 6a05 9000 79fc 0100 7d05  S...t.j...y...}.
-00000bc0: 0100 7a14 6407 7c05 6602 5700 0600 5900  ..z.d.|.f.W...Y.
-00000bd0: 6400 7d05 7e05 5300 6400 7d05 7e05 3000  d.}.~.S.d.}.~.0.
-00000be0: 3000 6400 5300 2908 4e7a 0c49 4e53 4552  0.d.S.).Nz.INSER
-00000bf0: 5420 494e 544f 207a 2a20 284e 616d 6520  T INTO z* (Name 
-00000c00: 2c20 436f 6e74 656e 7420 2c4b 6579 2920  , Content ,Key) 
-00000c10: 5641 4c55 4553 2028 3f20 2c20 3f20 2c20  VALUES (? , ? , 
-00000c20: 3f29 2072 3200 0000 7224 0000 007a 2920  ?) r2...r$...z) 
-00000c30: 284e 616d 652c 2043 6f6e 7465 6e74 202c  (Name, Content ,
-00000c40: 4b65 7929 2056 414c 5545 5320 283f 202c  Key) VALUES (? ,
-00000c50: 203f 202c 203f 2920 7225 0000 0072 0100   ? , ?) r%...r..
-00000c60: 0000 7233 0000 0029 0672 1100 0000 da04  ..r3...).r......
-00000c70: 6e61 6d65 da07 636f 6e74 656e 74da 036b  name..content..k
-00000c80: 6579 da13 6f70 7469 6f6e 616c 5f74 6162  ey..optional_tab
-00000c90: 6c65 5f6e 616d 6572 1900 0000 7212 0000  le_namer....r...
-00000ca0: 0072 1200 0000 7213 0000 00da 0669 6e73  .r....r......ins
-00000cb0: 6572 7453 0000 0073 2200 0000 0001 0801  ertS...s".......
-00000cc0: 0201 0801 1201 08ff 2203 0601 1001 2003  ........"..... .
-00000cd0: 0201 0801 1001 08ff 2202 0601 1201 7a0f  ........".....z.
-00000ce0: 4461 7461 6261 7365 2e69 6e73 6572 7429  Database.insert)
-00000cf0: 03da 0b63 6f6c 756d 6e5f 6e61 6d65 da0e  ...column_name..
-00000d00: 6e65 775f 636f 6c75 6d6e 5f76 616c da02  new_column_val..
-00000d10: 4944 6305 0000 0000 0000 0000 0000 0006  IDc.............
-00000d20: 0000 000a 0000 0043 0000 0073 0a01 0000  .......C...s....
-00000d30: 7c04 6400 7500 728a 7a50 7c00 6a00 8f36  |.d.u.r.zP|.j..6
-00000d40: 0100 7c00 6a01 a002 6401 7c00 6a03 9b00  ..|.j...d.|.j...
-00000d50: 6402 7c01 9b00 6403 9d05 7c02 7c03 6602  d.|...d...|.|.f.
-00000d60: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000d70: 5700 6404 5300 3100 734c 3000 0100 0100  W.d.S.1.sL0.....
-00000d80: 0100 5900 0100 5700 6e2e 0400 7404 6a05  ..Y...W.n...t.j.
-00000d90: 7986 0100 7d05 0100 7a14 6405 7c05 6602  y...}...z.d.|.f.
-00000da0: 5700 0600 5900 6400 7d05 7e05 5300 6400  W...Y.d.}.~.S.d.
-00000db0: 7d05 7e05 3000 3000 6e7c 7a4a 7c00 6a00  }.~.0.0.n|zJ|.j.
-00000dc0: 8f30 0100 7c00 6a01 a002 6401 7c04 9b00  .0..|.j...d.|...
-00000dd0: 6406 9d03 7c01 7c02 7c03 6603 a102 0100  d...|.|.|.f.....
-00000de0: 5700 6400 0400 0400 8303 0100 5700 6407  W.d.........W.d.
-00000df0: 5300 3100 73c8 3000 0100 0100 0100 5900  S.1.s.0.......Y.
-00000e00: 0100 5700 6e30 0400 7404 6a05 9001 7904  ..W.n0..t.j...y.
-00000e10: 0100 7d05 0100 7a14 6408 7c05 6602 5700  ..}...z.d.|.f.W.
-00000e20: 0600 5900 6400 7d05 7e05 5300 6400 7d05  ..Y.d.}.~.S.d.}.
-00000e30: 7e05 3000 3000 6400 5300 2909 4e7a 0755  ~.0.0.d.S.).Nz.U
-00000e40: 5044 4154 4520 7a05 2053 4554 207a 1220  PDATE z. SET z. 
-00000e50: 3d20 3f20 5748 4552 4520 4944 203d 203f  = ? WHERE ID = ?
-00000e60: 2072 3200 0000 7224 0000 007a 1820 5345   r2...r$...z. SE
-00000e70: 5420 3f20 3d20 3f20 5748 4552 4520 4944  T ? = ? WHERE ID
-00000e80: 203d 203f 2072 2500 0000 7201 0000 0072   = ? r%...r....r
-00000e90: 3300 0000 2906 7211 0000 0072 3b00 0000  3...).r....r;...
-00000ea0: 723c 0000 0072 3d00 0000 7239 0000 0072  r<...r=...r9...r
-00000eb0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000ec0: 0000 00da 0675 7064 6174 6567 0000 0073  .....updateg...s
-00000ed0: 2200 0000 0001 0801 0201 0801 1801 06ff  "...............
-00000ee0: 0402 2602 1001 2003 0201 0801 1001 08ff  ..&... .........
-00000ef0: 0402 2602 1201 7a0f 4461 7461 6261 7365  ..&...z.Database
-00000f00: 2e75 7064 6174 6563 0200 0000 0000 0000  .updatec........
-00000f10: 0000 0000 0400 0000 0a00 0000 6300 0000  ............c...
-00000f20: 731a 0100 007c 0164 0075 0072 907a 567c  s....|.d.u.r.zV|
-00000f30: 006a 008f 3c01 007c 006a 01a0 0264 017c  .j..<..|.j...d.|
-00000f40: 006a 039b 0064 029d 03a1 0101 007c 006a  .j...d.......|.j
-00000f50: 01a0 04a1 0044 005d 0a7d 027c 0256 0001  .....D.].}.|.V..
-00000f60: 0071 3257 0064 0004 0004 0083 0301 006e  .q2W.d.........n
-00000f70: 1031 0073 5230 0001 0001 0001 0059 0001  .1.sR0.......Y..
-00000f80: 0057 006e 2e04 0074 056a 0679 8c01 007d  .W.n...t.j.y...}
-00000f90: 0301 007a 1464 037c 0366 0257 0006 0059  ...z.d.|.f.W...Y
-00000fa0: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
-00000fb0: 0030 006e 867a 547c 006a 008f 3a01 007c  .0.n.zT|.j..:..|
-00000fc0: 006a 01a0 0264 017c 019b 0064 029d 03a1  .j...d.|...d....
-00000fd0: 0101 007c 006a 01a0 04a1 0044 005d 0a7d  ...|.j.....D.].}
-00000fe0: 027c 0256 0001 0071 b857 0064 0004 0004  .|.V...q.W.d....
-00000ff0: 0083 0301 006e 1031 0073 d830 0001 0001  .....n.1.s.0....
-00001000: 0001 0059 0001 0057 006e 3004 0074 056a  ...Y...W.n0..t.j
-00001010: 0690 0179 1401 007d 0301 007a 1464 047c  ...y...}...z.d.|
-00001020: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
-00001030: 0064 007d 037e 0330 0030 0064 0053 00a9  .d.}.~.0.0.d.S..
-00001040: 054e fa0e 5345 4c45 4354 202a 2046 524f  .N..SELECT * FRO
-00001050: 4d20 fa01 2072 2400 0000 7201 0000 00a9  M .. r$...r.....
-00001060: 0772 0c00 0000 720d 0000 0072 1500 0000  .r....r....r....
-00001070: 7209 0000 0072 2d00 0000 720e 0000 0072  r....r-...r....r
-00001080: 1700 0000 2904 7211 0000 0072 3400 0000  ....).r....r4...
-00001090: da03 726f 7772 1900 0000 7212 0000 0072  ..rowr....r....r
-000010a0: 1200 0000 7213 0000 0072 3700 0000 7c00  ....r....r7...|.
-000010b0: 0000 731e 0000 0000 0108 0102 0108 0116  ..s.............
-000010c0: 010e 012a 0210 0120 0302 0108 0114 010e  ...*... ........
-000010d0: 012a 0212 017a 1044 6174 6162 6173 652e  .*...z.Database.
-000010e0: 636f 6e74 656e 7429 01da 0269 6463 0300  content)...idc..
-000010f0: 0000 0000 0000 0000 0000 0500 0000 0a00  ................
-00001100: 0000 6300 0000 7322 0100 007c 0264 0075  ..c...s"...|.d.u
-00001110: 0072 947a 5a7c 006a 008f 4001 007c 006a  .r.zZ|.j..@..|.j
-00001120: 01a0 0264 017c 006a 039b 0064 029d 037c  ...d.|.j...d...|
-00001130: 0166 01a1 0201 007c 006a 01a0 04a1 0044  .f.....|.j.....D
-00001140: 005d 0a7d 037c 0356 0001 0071 3657 0064  .].}.|.V...q6W.d
-00001150: 0004 0004 0083 0301 006e 1031 0073 5630  .........n.1.sV0
-00001160: 0001 0001 0001 0059 0001 0057 006e 2e04  .......Y...W.n..
-00001170: 0074 056a 0679 9001 007d 0401 007a 1464  .t.j.y...}...z.d
-00001180: 037c 0466 0257 0006 0059 0064 007d 047e  .|.f.W...Y.d.}.~
-00001190: 0453 0064 007d 047e 0430 0030 006e 8a7a  .S.d.}.~.0.0.n.z
-000011a0: 587c 006a 008f 3e01 007c 006a 01a0 0264  X|.j..>..|.j...d
-000011b0: 017c 029b 0064 029d 037c 0166 01a1 0201  .|...d...|.f....
-000011c0: 007c 006a 01a0 04a1 0044 005d 0a7d 037c  .|.j.....D.].}.|
-000011d0: 0356 0001 0071 c057 0064 0004 0004 0083  .V...q.W.d......
-000011e0: 0301 006e 1031 0073 e030 0001 0001 0001  ...n.1.s.0......
-000011f0: 0059 0001 0057 006e 3004 0074 056a 0690  .Y...W.n0..t.j..
-00001200: 0179 1c01 007d 0401 007a 1464 047c 0466  .y...}...z.d.|.f
-00001210: 0257 0006 0059 0064 007d 047e 0453 0064  .W...Y.d.}.~.S.d
-00001220: 007d 047e 0430 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
-00001230: 7240 0000 007a 0e20 5748 4552 4520 4944  r@...z. WHERE ID
-00001240: 203d 203f 2072 2400 0000 7201 0000 0072   = ? r$...r....r
-00001250: 4200 0000 2905 7211 0000 0072 4400 0000  B...).r....rD...
-00001260: 7234 0000 0072 4300 0000 7219 0000 0072  r4...rC...r....r
-00001270: 1200 0000 7212 0000 0072 1300 0000 da0d  ....r....r......
-00001280: 636f 6e74 656e 745f 6279 5f69 6491 0000  content_by_id...
-00001290: 0073 1e00 0000 0001 0801 0201 0801 1a01  .s..............
-000012a0: 0e01 2a02 1001 2003 0201 0801 1801 0e01  ..*... .........
-000012b0: 2a02 1201 7a16 4461 7461 6261 7365 2e63  *...z.Database.c
-000012c0: 6f6e 7465 6e74 5f62 795f 6964 6301 0000  ontent_by_idc...
-000012d0: 0000 0000 0000 0000 0005 0000 000a 0000  ................
-000012e0: 0067 0000 0073 2a01 0000 7c01 7298 7a62  .g...s*...|.r.zb
-000012f0: 7c01 4400 5d58 7d02 7c00 6a00 8f3e 0100  |.D.]X}.|.j..>..
-00001300: 7c00 6a01 a002 6401 7c02 9b00 6402 9d03  |.j...d.|...d...
-00001310: a101 0100 7c00 6a01 a003 a100 4400 5d0e  ....|.j.....D.].
-00001320: 7d03 7c02 7c03 6901 5600 0100 7134 5700  }.|.|.i.V...q4W.
-00001330: 6400 0400 0400 8303 0100 710a 3100 7358  d.........q.1.sX
-00001340: 3000 0100 0100 0100 5900 0100 710a 5700  0.......Y...q.W.
-00001350: 6e2e 0400 7404 6a05 7994 0100 7d04 0100  n...t.j.y...}...
-00001360: 7a14 6403 7c04 6602 5700 0600 5900 6400  z.d.|.f.W...Y.d.
-00001370: 7d04 7e04 5300 6400 7d04 7e04 3000 3000  }.~.S.d.}.~.0.0.
-00001380: 6e8e 7a5c 7c00 6a00 8f42 0100 7c00 6a01  n.z\|.j..B..|.j.
-00001390: a002 6401 7c00 6a06 9b00 6402 9d03 a101  ..d.|.j...d.....
-000013a0: 0100 7c00 6a01 a003 a100 4400 5d10 7d03  ..|.j.....D.].}.
-000013b0: 7c00 6a06 7c03 6901 5600 0100 71c2 5700  |.j.|.i.V...q.W.
-000013c0: 6400 0400 0400 8303 0100 6e10 3100 73e8  d.........n.1.s.
-000013d0: 3000 0100 0100 0100 5900 0100 5700 6e30  0.......Y...W.n0
-000013e0: 0400 7404 6a05 9001 7924 0100 7d04 0100  ..t.j...y$..}...
-000013f0: 7a14 6404 7c04 6602 5700 0600 5900 6400  z.d.|.f.W...Y.d.
-00001400: 7d04 7e04 5300 6400 7d04 7e04 3000 3000  }.~.S.d.}.~.0.0.
-00001410: 6400 5300 723f 0000 0029 0772 0c00 0000  d.S.r?...).r....
-00001420: 720d 0000 0072 1500 0000 722d 0000 0072  r....r....r-...r
-00001430: 0e00 0000 7217 0000 0072 0900 0000 2905  ....r....r....).
-00001440: 7211 0000 005a 136f 7074 696f 6e61 6c5f  r....Z.optional_
-00001450: 7461 626c 656e 616d 6573 da03 6172 6772  tablenames..argr
-00001460: 4300 0000 7219 0000 0072 1200 0000 7212  C...r....r....r.
-00001470: 0000 0072 1300 0000 da0d 7368 6f77 5f63  ...r......show_c
-00001480: 6f6e 7465 6e74 73a6 0000 0073 2000 0000  ontents....s ...
-00001490: 0001 0401 0201 0801 0801 1401 0e01 3002  ..............0.
-000014a0: 1001 2003 0201 0801 1601 0e01 3002 1201  .. .........0...
-000014b0: 7a16 4461 7461 6261 7365 2e73 686f 775f  z.Database.show_
-000014c0: 636f 6e74 656e 7473 6301 0000 0000 0000  contentsc.......
-000014d0: 0000 0000 0003 0000 000a 0000 0063 0000  .............c..
-000014e0: 0073 8000 0000 7a4c 7c00 6a00 8f32 0100  .s....zL|.j..2..
-000014f0: 7c00 6a01 a002 6401 a101 0100 7c00 6a01  |.j...d.....|.j.
-00001500: a003 a100 4400 5d0a 7d01 7c01 5600 0100  ....D.].}.|.V...
-00001510: 7120 5700 6400 0400 0400 8303 0100 6e10  q W.d.........n.
-00001520: 3100 7340 3000 0100 0100 0100 5900 0100  1.s@0.......Y...
-00001530: 5700 6e2e 0400 7404 6a05 797a 0100 7d02  W.n...t.j.yz..}.
-00001540: 0100 7a14 6402 7c02 6602 5700 0600 5900  ..z.d.|.f.W...Y.
-00001550: 6400 7d02 7e02 5300 6400 7d02 7e02 3000  d.}.~.S.d.}.~.0.
-00001560: 3000 6400 5300 2903 4efa 3353 454c 4543  0.d.S.).N.3SELEC
-00001570: 5420 6e61 6d65 2046 524f 4d20 7371 6c69  T name FROM sqli
-00001580: 7465 5f6d 6173 7465 7220 5748 4552 4520  te_master WHERE 
-00001590: 7479 7065 3d20 2774 6162 6c65 2720 7201  type= 'table' r.
-000015a0: 0000 00a9 0672 0c00 0000 720d 0000 0072  .....r....r....r
-000015b0: 1500 0000 722d 0000 0072 0e00 0000 7217  ....r-...r....r.
-000015c0: 0000 0029 0372 1100 0000 7243 0000 0072  ...).r....rC...r
-000015d0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000015e0: 0000 00da 0b73 686f 775f 7461 626c 6573  .....show_tables
-000015f0: bc00 0000 730e 0000 0000 0102 0108 010c  ....s...........
-00001600: 010e 012a 0210 017a 1444 6174 6162 6173  ...*...z.Databas
-00001610: 652e 7368 6f77 5f74 6162 6c65 7363 0100  e.show_tablesc..
-00001620: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
-00001630: 0000 4300 0000 7394 0000 007a 607c 006a  ..C...s....z`|.j
-00001640: 008f 4601 007c 006a 01a0 0264 01a1 0101  ..F..|.j...d....
-00001650: 007c 006a 01a0 03a1 0044 005d 1a7d 017c  .|.j.....D.].}.|
-00001660: 006a 01a0 0264 027c 0164 0319 009b 009d  .j...d.|.d......
-00001670: 02a1 0101 0071 2057 0064 0004 0004 0083  .....q W.d......
-00001680: 0301 0057 0064 0453 0031 0073 5430 0001  ...W.d.S.1.sT0..
-00001690: 0001 0001 0059 0001 0057 006e 2e04 0074  .....Y...W.n...t
-000016a0: 046a 0579 8e01 007d 0201 007a 1464 037c  .j.y...}...z.d.|
-000016b0: 0266 0257 0006 0059 0064 007d 027e 0253  .f.W...Y.d.}.~.S
-000016c0: 0064 007d 027e 0230 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-000016d0: 054e 7248 0000 00fa 0b44 524f 5020 5441  .NrH.....DROP TA
-000016e0: 424c 4520 7201 0000 0072 2500 0000 7249  BLE r....r%...rI
-000016f0: 0000 0029 0372 1100 0000 da05 7461 626c  ...).r......tabl
-00001700: 6572 1900 0000 7212 0000 0072 1200 0000  er....r....r....
-00001710: 7213 0000 00da 0764 726f 7061 6c6c c600  r......dropall..
-00001720: 0000 7310 0000 0000 0102 0108 010c 010e  ..s.............
-00001730: 0118 0126 0210 017a 1044 6174 6162 6173  ...&...z.Databas
-00001740: 652e 6472 6f70 616c 6c63 0100 0000 0000  e.dropallc......
-00001750: 0000 0000 0000 0400 0000 0a00 0000 4700  ..............G.
-00001760: 0000 73f6 0000 007c 0172 7e7a 487c 0144  ..s....|.r~zH|.D
-00001770: 005d 3c7d 027c 006a 008f 2201 007c 006a  .]<}.|.j.."..|.j
-00001780: 01a0 0264 017c 029b 009d 02a1 0101 0057  ...d.|.........W
-00001790: 0064 0004 0004 0083 0301 0071 0a31 0073  .d.........q.1.s
-000017a0: 3c30 0001 0001 0001 0059 0001 0071 0a57  <0.......Y...q.W
-000017b0: 0064 0253 0004 0074 036a 0479 7a01 007d  .d.S...t.j.yz..}
-000017c0: 0301 007a 1464 037c 0366 0257 0006 0059  ...z.d.|.f.W...Y
-000017d0: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
-000017e0: 0030 006e 747a 427c 006a 008f 2801 007c  .0.ntzB|.j..(..|
-000017f0: 006a 01a0 0264 017c 006a 059b 009d 02a1  .j...d.|.j......
-00001800: 0101 0057 0064 0004 0004 0083 0301 0057  ...W.d.........W
-00001810: 0064 0253 0031 0073 b430 0001 0001 0001  .d.S.1.s.0......
-00001820: 0059 0001 0057 006e 3004 0074 036a 0490  .Y...W.n0..t.j..
-00001830: 0079 f001 007d 0301 007a 1464 047c 0366  .y...}...z.d.|.f
-00001840: 0257 0006 0059 0064 007d 037e 0353 0064  .W...Y.d.}.~.S.d
-00001850: 007d 037e 0330 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
-00001860: 724b 0000 0072 2500 0000 7224 0000 0072  rK...r%...r$...r
-00001870: 0100 0000 2906 720c 0000 0072 0d00 0000  ....).r....r....
-00001880: 7215 0000 0072 0e00 0000 7217 0000 0072  r....r....r....r
-00001890: 0900 0000 2904 7211 0000 005a 0b74 6162  ....).r....Z.tab
-000018a0: 6c65 5f6e 616d 6573 7246 0000 0072 1900  le_namesrF...r..
-000018b0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000018c0: 00da 0a64 726f 705f 7461 626c 65d1 0000  ...drop_table...
-000018d0: 0073 1c00 0000 0001 0401 0201 0801 0801  .s..............
-000018e0: 3201 0601 1001 2003 0201 0801 1401 2602  2..... .......&.
-000018f0: 1201 7a13 4461 7461 6261 7365 2e64 726f  ..z.Database.dro
-00001900: 705f 7461 626c 6563 0300 0000 0000 0000  p_tablec........
-00001910: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
-00001920: 73fa 0000 007c 0264 0075 0072 807a 467c  s....|.d.u.r.zF|
-00001930: 006a 008f 2a01 007c 006a 01a0 0264 017c  .j..*..|.j...d.|
-00001940: 006a 039b 0064 027c 019b 009d 04a1 0101  .j...d.|........
-00001950: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001960: 0073 4030 0001 0001 0001 0059 0001 0057  .s@0.......Y...W
-00001970: 0064 0353 0004 0074 046a 0579 7c01 007d  .d.S...t.j.y|..}
-00001980: 0301 007a 1464 047c 0366 0257 0006 0059  ...z.d.|.f.W...Y
-00001990: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
-000019a0: 0030 006e 767a 447c 006a 008f 2801 007c  .0.nvzD|.j..(..|
-000019b0: 006a 01a0 0264 017c 029b 0064 027c 019b  .j...d.|...d.|..
-000019c0: 009d 04a1 0101 0057 0064 0004 0004 0083  .......W.d......
-000019d0: 0301 006e 1031 0073 b630 0001 0001 0001  ...n.1.s.0......
-000019e0: 0059 0001 0057 0064 0553 0004 0074 046a  .Y...W.d.S...t.j
-000019f0: 0590 0079 f401 007d 0301 007a 1464 067c  ...y...}...z.d.|
-00001a00: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
-00001a10: 0064 007d 037e 0330 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-00001a20: 074e 7a0c 4445 4c45 5445 2046 524f 4d20  .Nz.DELETE FROM 
-00001a30: 7a0c 2057 4845 5245 2049 4420 3d20 7232  z. WHERE ID = r2
-00001a40: 0000 0072 2400 0000 7225 0000 0072 0100  ...r$...r%...r..
-00001a50: 0000 7233 0000 0029 0472 1100 0000 723d  ..r3...).r....r=
-00001a60: 0000 0072 3900 0000 7219 0000 0072 1200  ...r9...r....r..
-00001a70: 0000 7212 0000 0072 1300 0000 da0c 6472  ..r....r......dr
-00001a80: 6f70 5f63 6f6e 7465 6e74 e400 0000 731a  op_content....s.
-00001a90: 0000 0000 0108 0102 0108 0138 0106 0210  ...........8....
-00001aa0: 0120 0302 0108 0136 0106 0212 017a 1544  . .....6.....z.D
-00001ab0: 6174 6162 6173 652e 6472 6f70 5f63 6f6e  atabase.drop_con
-00001ac0: 7465 6e74 2901 4e29 014e 2901 4e29 014e  tent).N).N).N).N
-00001ad0: 2901 4e29 014e 2922 da08 5f5f 6e61 6d65  ).N).N)"..__name
-00001ae0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001af0: 5f5f 7175 616c 6e61 6d65 5f5f 7203 0000  __qualname__r...
-00001b00: 0072 0700 0000 722a 0000 00da 0f5f 5f61  .r....r*.....__a
-00001b10: 6e6e 6f74 6174 696f 6e73 5f5f 7209 0000  nnotations__r...
-00001b20: 0072 0c00 0000 720e 0000 005a 0a43 6f6e  .r....r....Z.Con
-00001b30: 6e65 6374 696f 6e72 0d00 0000 5a06 4375  nectionr....Z.Cu
-00001b40: 7273 6f72 7214 0000 00da 0870 726f 7065  rsorr......prope
-00001b50: 7274 7972 1800 0000 7205 0000 0072 0400  rtyr....r....r..
-00001b60: 0000 da05 7475 706c 6572 2000 0000 7222  ....tupler ...r"
-00001b70: 0000 00da 046c 6973 7472 3100 0000 7235  .....listr1...r5
-00001b80: 0000 0072 3a00 0000 da03 696e 7472 3e00  ...r:.....intr>.
-00001b90: 0000 7237 0000 0072 4500 0000 7247 0000  ..r7...rE...rG..
-00001ba0: 0072 4a00 0000 724d 0000 0072 4e00 0000  .rJ...rM...rN...
-00001bb0: 724f 0000 0072 1200 0000 7212 0000 0072  rO...r....r....r
-00001bc0: 1200 0000 7213 0000 0072 0600 0000 0700  ....r....r......
-00001bd0: 0000 732c 0000 000a 020e 0112 0116 0116  ..s,............
-00001be0: 0208 0402 010a 0a02 0118 0802 010a 0310  ................
-00001bf0: 110a 180a 1414 150a 1510 1508 160e 0a08  ................
-00001c00: 0b08 1372 0600 0000 2909 5a0b 6461 7461  ...r....).Z.data
-00001c10: 636c 6173 7365 7372 0200 0000 7203 0000  classesr....r...
-00001c20: 0072 0400 0000 da06 7479 7069 6e67 7205  .r......typingr.
-00001c30: 0000 0072 0e00 0000 721c 0000 0072 0600  ...r....r....r..
-00001c40: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00001c50: 0072 1300 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001c60: 0100 0000 730c 0000 0010 010c 010c 0108  ....s...........
-00001c70: 0108 0202 01                             .....
+00000460: 0000 7218 0000 0013 0000 0073 1400 0000  ..r........s....
+00000470: 0002 0201 0801 0601 02ff 0402 0a01 1001  ................
+00000480: 2801 1001 7a0d 4461 7461 6261 7365 2e73  (...z.Database.s
+00000490: 697a 6529 01da 0672 6574 7572 6e63 0100  ize)...returnc..
+000004a0: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+000004b0: 0000 4300 0000 734c 0000 007a 1a74 00a0  ..C...sL...z.t..
+000004c0: 0174 02a0 037c 006a 04a1 016a 05a1 017d  .t...|.j...j...}
+000004d0: 017c 0157 0053 0004 0074 0679 4601 007d  .|.W.S...t.yF..}
+000004e0: 0201 007a 1464 017c 0266 0257 0006 0059  ...z.d.|.f.W...Y
+000004f0: 0064 007d 027e 0253 0064 007d 027e 0230  .d.}.~.S.d.}.~.0
+00000500: 0030 0064 0053 0029 024e 7201 0000 0029  .0.d.S.).Nr....)
+00000510: 0772 0400 0000 da0d 6672 6f6d 7469 6d65  .r......fromtime
+00000520: 7374 616d 70da 026f 73da 0473 7461 7472  stamp..os..statr
+00000530: 0700 0000 da08 7374 5f6d 7469 6d65 da07  ......st_mtime..
+00000540: 4f53 4572 726f 7229 0372 1100 0000 5a09  OSError).r....Z.
+00000550: 7469 6d65 5f73 7461 7472 1900 0000 7212  time_statr....r.
+00000560: 0000 0072 1200 0000 7213 0000 00da 086c  ...r....r......l
+00000570: 6173 745f 6d6f 641f 0000 0073 0a00 0000  ast_mod....s....
+00000580: 0002 0201 1401 0602 0e01 7a11 4461 7461  ..........z.Data
+00000590: 6261 7365 2e6c 6173 745f 6d6f 6463 0100  base.last_modc..
+000005a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000005b0: 0000 4300 0000 730e 0000 0064 017c 006a  ..C...s....d.|.j
+000005c0: 009b 0064 029d 0353 0029 034e 7a20 4445  ...d...S.).Nz DE
+000005d0: 4641 554c 5420 524f 5554 494e 4720 414c  FAULT ROUTING AL
+000005e0: 4c20 4d45 5448 4f44 5320 544f 2022 fa01  L METHODS TO "..
+000005f0: 2229 0172 0900 0000 7210 0000 0072 1200  ").r....r....r..
+00000600: 0000 7212 0000 0072 1300 0000 da0f 6465  ..r....r......de
+00000610: 6661 756c 745f 726f 7574 696e 6728 0000  fault_routing(..
+00000620: 0073 0200 0000 0002 7a18 4461 7461 6261  .s......z.Databa
+00000630: 7365 2e64 6566 6175 6c74 5f72 6f75 7469  se.default_routi
+00000640: 6e67 2902 da06 7175 6572 7973 721a 0000  ng)...querysr...
+00000650: 0063 0100 0000 0000 0000 0000 0000 0600  .c..............
+00000660: 0000 0b00 0000 4700 0000 7300 0100 0067  ......G...s....g
+00000670: 007d 0274 007c 0183 0144 005d ee5c 027d  .}.t.|...D.].\.}
+00000680: 037d 0474 017c 0474 0283 0273 367c 02a0  .}.t.|.t...s6|..
+00000690: 0364 017c 039b 009d 0264 0274 0466 0269  .d.|.....d.t.f.i
+000006a0: 01a1 0101 007a 807c 006a 058f 6601 007c  .....z.|.j..f..|
+000006b0: 006a 06a0 077c 04a1 0101 007c 006a 066a  .j...|.....|.j.j
+000006c0: 0864 036b 0272 787c 02a0 0364 017c 039b  .d.k.rx|...d.|..
+000006d0: 009d 0264 047c 006a 06a0 09a1 0067 0269  ...d.|.j.....g.i
+000006e0: 01a1 0101 006e 1e7c 02a0 0364 017c 039b  .....n.|...d.|..
+000006f0: 009d 0264 047c 006a 06a0 0aa1 0067 0269  ...d.|.j.....g.i
+00000700: 01a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00000710: 006e 1031 0073 aa30 0001 0001 0001 0059  .n.1.s.0.......Y
+00000720: 0001 0057 0071 0c04 0074 0b6a 0c79 f801  ...W.q...t.j.y..
+00000730: 007d 0501 007a 287c 02a0 0364 017c 039b  .}...z(|...d.|..
+00000740: 009d 0264 057c 05a0 0da1 0066 0269 01a1  ...d.|.....f.i..
+00000750: 0101 0057 0059 0064 007d 057e 0571 0c64  ...W.Y.d.}.~.q.d
+00000760: 007d 057e 0530 0030 0071 0c7c 0253 0029  .}.~.0.0.q.|.S.)
+00000770: 064e 7a06 7175 6572 7920 e700 0000 0000  .Nz.query ......
+00000780: 0000 00e9 0100 0000 da07 5355 4343 4553  ..........SUCCES
+00000790: 53da 0746 4149 4c55 5245 290e da09 656e  S..FAILURE)...en
+000007a0: 756d 6572 6174 65da 0a69 7369 6e73 7461  umerate..isinsta
+000007b0: 6e63 65da 0373 7472 da06 6170 7065 6e64  nce..str..append
+000007c0: da09 5479 7065 4572 726f 7272 0c00 0000  ..TypeErrorr....
+000007d0: 720d 0000 0072 1500 0000 5a08 726f 7763  r....r....Z.rowc
+000007e0: 6f75 6e74 7216 0000 00da 0866 6574 6368  ountr......fetch
+000007f0: 616c 6c72 0e00 0000 7217 0000 00da 075f  allr....r......_
+00000800: 5f73 7472 5f5f 2906 7211 0000 0072 2300  _str__).r....r#.
+00000810: 0000 da06 7265 7375 6c74 da01 69da 0571  ....result..i..q
+00000820: 7565 7279 7219 0000 0072 1200 0000 7212  ueryr....r....r.
+00000830: 0000 0072 1300 0000 7231 0000 002c 0000  ...r....r1...,..
+00000840: 0073 2200 0000 0001 0401 1001 0a01 1801  .s".............
+00000850: 0201 0801 0c01 0c01 0401 16ff 0603 0401  ................
+00000860: 16ff 2603 1001 3401 7a0e 4461 7461 6261  ..&...4.z.Databa
+00000870: 7365 2e71 7565 7279 4e63 0200 0000 0000  se.queryNc......
+00000880: 0000 0000 0000 0300 0000 0a00 0000 4300  ..............C.
+00000890: 0000 73f8 0000 007c 0164 0075 0072 7c7a  ..s....|.d.u.r|z
+000008a0: 427c 006a 008f 2601 007c 006a 01a0 0264  B|.j..&..|.j...d
+000008b0: 017c 006a 039b 0064 029d 03a1 0101 0057  .|.j...d.......W
+000008c0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+000008d0: 3c30 0001 0001 0001 0059 0001 0057 0064  <0.......Y...W.d
+000008e0: 0353 0004 0074 046a 0579 7801 007d 0201  .S...t.j.yx..}..
+000008f0: 007a 1464 047c 0266 0257 0006 0059 0064  .z.d.|.f.W...Y.d
+00000900: 007d 027e 0253 0064 007d 027e 0230 0030  .}.~.S.d.}.~.0.0
+00000910: 006e 787a 467c 006a 008f 2a01 007c 006a  .nxzF|.j..*..|.j
+00000920: 01a0 0264 017c 019b 0064 059d 03a1 0101  ...d.|...d......
+00000930: 007c 017c 005f 0357 0064 0004 0004 0083  .|.|._.W.d......
+00000940: 0301 006e 1031 0073 b430 0001 0001 0001  ...n.1.s.0......
+00000950: 0059 0001 0057 0064 0653 0004 0074 046a  .Y...W.d.S...t.j
+00000960: 0590 0079 f201 007d 0201 007a 1464 077c  ...y...}...z.d.|
+00000970: 0266 0257 0006 0059 0064 007d 027e 0253  .f.W...Y.d.}.~.S
+00000980: 0064 007d 027e 0230 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00000990: 084e 7a1b 4352 4541 5445 2054 4142 4c45  .Nz.CREATE TABLE
+000009a0: 2049 4620 4e4f 5420 4558 4953 5453 207a   IF NOT EXISTS z
+000009b0: 3e20 2849 4420 494e 5445 4745 5220 5052  > (ID INTEGER PR
+000009c0: 494d 4152 5920 4b45 592c 204e 616d 6520  IMARY KEY, Name 
+000009d0: 5465 7874 202c 2043 6f6e 7465 6e74 2042  Text , Content B
+000009e0: 4c4f 4220 2c4b 6579 2054 4558 5420 29e9  LOB ,Key TEXT ).
+000009f0: 0b00 0000 7224 0000 007a 3c20 2849 4420  ....r$...z< (ID 
+00000a00: 494e 5445 4745 5220 5052 494d 4152 5920  INTEGER PRIMARY 
+00000a10: 4b45 592c 4e61 6d65 2054 4558 5420 2c43  KEY,Name TEXT ,C
+00000a20: 6f6e 7465 6e74 2042 4c4f 4220 2c4b 6579  ontent BLOB ,Key
+00000a30: 2054 4558 5420 2972 2500 0000 7201 0000   TEXT )r%...r...
+00000a40: 00a9 0672 0c00 0000 720d 0000 0072 1500  ...r....r....r..
+00000a50: 0000 7209 0000 0072 0e00 0000 7217 0000  ..r....r....r...
+00000a60: 0029 0372 1100 0000 da12 6f70 7469 6f6e  .).r......option
+00000a70: 616c 5f74 6162 6c65 6e61 6d65 7219 0000  al_tablenamer...
+00000a80: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000a90: da08 6164 6474 6162 6c65 3f00 0000 7324  ..addtable?...s$
+00000aa0: 0000 0000 0108 0102 0108 0106 010c ff22  ..............."
+00000ab0: 0306 0110 0120 0302 0108 0106 010a ff04  ..... ..........
+00000ac0: 0624 0106 0212 017a 1144 6174 6162 6173  .$.....z.Databas
+00000ad0: 652e 6164 6474 6162 6c65 6305 0000 0000  e.addtablec.....
+00000ae0: 0000 0000 0000 0006 0000 000a 0000 0043  ...............C
+00000af0: 0000 0073 0201 0000 7c04 6400 7500 7284  ...s....|.d.u.r.
+00000b00: 7a4a 7c00 6a00 8f2e 0100 7c00 6a01 a002  zJ|.j.....|.j...
+00000b10: 6401 7c00 6a03 9b00 6402 9d03 7c01 7c02  d.|.j...d...|.|.
+00000b20: 7c03 6603 a102 0100 5700 6400 0400 0400  |.f.....W.d.....
+00000b30: 8303 0100 6e10 3100 7344 3000 0100 0100  ....n.1.sD0.....
+00000b40: 0100 5900 0100 5700 6403 5300 0400 7404  ..Y...W.d.S...t.
+00000b50: 6a05 7980 0100 7d05 0100 7a14 6404 7c05  j.y...}...z.d.|.
+00000b60: 6602 5700 0600 5900 6400 7d05 7e05 5300  f.W...Y.d.}.~.S.
+00000b70: 6400 7d05 7e05 3000 3000 6e7a 7a48 7c00  d.}.~.0.0.nzzH|.
+00000b80: 6a00 8f2c 0100 7c00 6a01 a002 6401 7c04  j..,..|.j...d.|.
+00000b90: 9b00 6405 9d03 7c01 7c02 7c03 6603 a102  ..d...|.|.|.f...
+00000ba0: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
+00000bb0: 3100 73be 3000 0100 0100 0100 5900 0100  1.s.0.......Y...
+00000bc0: 5700 6406 5300 0400 7404 6a05 9000 79fc  W.d.S...t.j...y.
+00000bd0: 0100 7d05 0100 7a14 6407 7c05 6602 5700  ..}...z.d.|.f.W.
+00000be0: 0600 5900 6400 7d05 7e05 5300 6400 7d05  ..Y.d.}.~.S.d.}.
+00000bf0: 7e05 3000 3000 6400 5300 2908 4e7a 0c49  ~.0.0.d.S.).Nz.I
+00000c00: 4e53 4552 5420 494e 544f 207a 2a20 284e  NSERT INTO z* (N
+00000c10: 616d 6520 2c20 436f 6e74 656e 7420 2c4b  ame , Content ,K
+00000c20: 6579 2920 5641 4c55 4553 2028 3f20 2c20  ey) VALUES (? , 
+00000c30: 3f20 2c20 3f29 2072 3200 0000 7224 0000  ? , ?) r2...r$..
+00000c40: 007a 2920 284e 616d 652c 2043 6f6e 7465  .z) (Name, Conte
+00000c50: 6e74 202c 4b65 7929 2056 414c 5545 5320  nt ,Key) VALUES 
+00000c60: 283f 202c 203f 202c 203f 2920 7225 0000  (? , ? , ?) r%..
+00000c70: 0072 0100 0000 7233 0000 0029 0672 1100  .r....r3...).r..
+00000c80: 0000 da04 6e61 6d65 da07 636f 6e74 656e  ....name..conten
+00000c90: 74da 036b 6579 da13 6f70 7469 6f6e 616c  t..key..optional
+00000ca0: 5f74 6162 6c65 5f6e 616d 6572 1900 0000  _table_namer....
+00000cb0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000cc0: 0669 6e73 6572 7459 0000 0073 3200 0000  .insertY...s2...
+00000cd0: 0001 0801 0201 0801 0601 0c01 0201 0201  ................
+00000ce0: 02fe 02fe 2206 0601 1001 2003 0201 0801  ...."..... .....
+00000cf0: 0601 0a01 0201 0201 02fe 02fe 2205 0601  ............"...
+00000d00: 1201 7a0f 4461 7461 6261 7365 2e69 6e73  ..z.Database.ins
+00000d10: 6572 7429 03da 0b63 6f6c 756d 6e5f 6e61  ert)...column_na
+00000d20: 6d65 da0e 6e65 775f 636f 6c75 6d6e 5f76  me..new_column_v
+00000d30: 616c da02 4944 6305 0000 0000 0000 0000  al..IDc.........
+00000d40: 0000 0006 0000 000a 0000 0043 0000 0073  ...........C...s
+00000d50: 0a01 0000 7c04 6400 7500 728a 7a50 7c00  ....|.d.u.r.zP|.
+00000d60: 6a00 8f36 0100 7c00 6a01 a002 6401 7c00  j..6..|.j...d.|.
+00000d70: 6a03 9b00 6402 7c01 9b00 6403 9d05 7c02  j...d.|...d...|.
+00000d80: 7c03 6602 a102 0100 5700 6400 0400 0400  |.f.....W.d.....
+00000d90: 8303 0100 5700 6404 5300 3100 734c 3000  ....W.d.S.1.sL0.
+00000da0: 0100 0100 0100 5900 0100 5700 6e2e 0400  ......Y...W.n...
+00000db0: 7404 6a05 7986 0100 7d05 0100 7a14 6405  t.j.y...}...z.d.
+00000dc0: 7c05 6602 5700 0600 5900 6400 7d05 7e05  |.f.W...Y.d.}.~.
+00000dd0: 5300 6400 7d05 7e05 3000 3000 6e7c 7a4a  S.d.}.~.0.0.n|zJ
+00000de0: 7c00 6a00 8f30 0100 7c00 6a01 a002 6401  |.j..0..|.j...d.
+00000df0: 7c04 9b00 6406 9d03 7c01 7c02 7c03 6603  |...d...|.|.|.f.
+00000e00: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00000e10: 5700 6407 5300 3100 73c8 3000 0100 0100  W.d.S.1.s.0.....
+00000e20: 0100 5900 0100 5700 6e30 0400 7404 6a05  ..Y...W.n0..t.j.
+00000e30: 9001 7904 0100 7d05 0100 7a14 6408 7c05  ..y...}...z.d.|.
+00000e40: 6602 5700 0600 5900 6400 7d05 7e05 5300  f.W...Y.d.}.~.S.
+00000e50: 6400 7d05 7e05 3000 3000 6400 5300 2909  d.}.~.0.0.d.S.).
+00000e60: 4e7a 0755 5044 4154 4520 7a05 2053 4554  Nz.UPDATE z. SET
+00000e70: 207a 1220 3d20 3f20 5748 4552 4520 4944   z. = ? WHERE ID
+00000e80: 203d 203f 2072 3200 0000 7224 0000 007a   = ? r2...r$...z
+00000e90: 1820 5345 5420 3f20 3d20 3f20 5748 4552  . SET ? = ? WHER
+00000ea0: 4520 4944 203d 203f 2072 2500 0000 7201  E ID = ? r%...r.
+00000eb0: 0000 0072 3300 0000 2906 7211 0000 0072  ...r3...).r....r
+00000ec0: 3b00 0000 723c 0000 0072 3d00 0000 7239  ;...r<...r=...r9
+00000ed0: 0000 0072 1900 0000 7212 0000 0072 1200  ...r....r....r..
+00000ee0: 0000 7213 0000 00da 0675 7064 6174 6573  ..r......updates
+00000ef0: 0000 0073 3000 0000 0006 0801 0201 0801  ...s0...........
+00000f00: 0601 1201 0201 02ff 02fe 0404 2602 1001  ............&...
+00000f10: 2003 0201 0801 0601 0a01 0201 0201 02fe   ...............
+00000f20: 02fe 0405 2602 1201 7a0f 4461 7461 6261  ....&...z.Databa
+00000f30: 7365 2e75 7064 6174 6563 0200 0000 0000  se.updatec......
+00000f40: 0000 0000 0000 0400 0000 0a00 0000 6300  ..............c.
+00000f50: 0000 731a 0100 007c 0164 0075 0072 907a  ..s....|.d.u.r.z
+00000f60: 567c 006a 008f 3c01 007c 006a 01a0 0264  V|.j..<..|.j...d
+00000f70: 017c 006a 039b 0064 029d 03a1 0101 007c  .|.j...d.......|
+00000f80: 006a 01a0 04a1 0044 005d 0a7d 027c 0256  .j.....D.].}.|.V
+00000f90: 0001 0071 3257 0064 0004 0004 0083 0301  ...q2W.d........
+00000fa0: 006e 1031 0073 5230 0001 0001 0001 0059  .n.1.sR0.......Y
+00000fb0: 0001 0057 006e 2e04 0074 056a 0679 8c01  ...W.n...t.j.y..
+00000fc0: 007d 0301 007a 1464 037c 0366 0257 0006  .}...z.d.|.f.W..
+00000fd0: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
+00000fe0: 0330 0030 006e 867a 547c 006a 008f 3a01  .0.0.n.zT|.j..:.
+00000ff0: 007c 006a 01a0 0264 017c 019b 0064 029d  .|.j...d.|...d..
+00001000: 03a1 0101 007c 006a 01a0 04a1 0044 005d  .....|.j.....D.]
+00001010: 0a7d 027c 0256 0001 0071 b857 0064 0004  .}.|.V...q.W.d..
+00001020: 0004 0083 0301 006e 1031 0073 d830 0001  .......n.1.s.0..
+00001030: 0001 0001 0059 0001 0057 006e 3004 0074  .....Y...W.n0..t
+00001040: 056a 0690 0179 1401 007d 0301 007a 1464  .j...y...}...z.d
+00001050: 047c 0366 0257 0006 0059 0064 007d 037e  .|.f.W...Y.d.}.~
+00001060: 0353 0064 007d 037e 0330 0030 0064 0053  .S.d.}.~.0.0.d.S
+00001070: 00a9 054e fa0e 5345 4c45 4354 202a 2046  ...N..SELECT * F
+00001080: 524f 4d20 fa01 2072 2400 0000 7201 0000  ROM .. r$...r...
+00001090: 00a9 0772 0c00 0000 720d 0000 0072 1500  ...r....r....r..
+000010a0: 0000 7209 0000 0072 2d00 0000 720e 0000  ..r....r-...r...
+000010b0: 0072 1700 0000 2904 7211 0000 0072 3400  .r....).r....r4.
+000010c0: 0000 da03 726f 7772 1900 0000 7212 0000  ....rowr....r...
+000010d0: 0072 1200 0000 7213 0000 0072 3700 0000  .r....r....r7...
+000010e0: 9200 0000 731e 0000 0000 0108 0102 0108  ....s...........
+000010f0: 0116 010e 012a 0210 0120 0302 0108 0114  .....*... ......
+00001100: 010e 012a 0212 017a 1044 6174 6162 6173  ...*...z.Databas
+00001110: 652e 636f 6e74 656e 7429 01da 0269 6463  e.content)...idc
+00001120: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00001130: 0a00 0000 6300 0000 7322 0100 007c 0264  ....c...s"...|.d
+00001140: 0075 0072 947a 5a7c 006a 008f 4001 007c  .u.r.zZ|.j..@..|
+00001150: 006a 01a0 0264 017c 006a 039b 0064 029d  .j...d.|.j...d..
+00001160: 037c 0166 01a1 0201 007c 006a 01a0 04a1  .|.f.....|.j....
+00001170: 0044 005d 0a7d 037c 0356 0001 0071 3657  .D.].}.|.V...q6W
+00001180: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00001190: 5630 0001 0001 0001 0059 0001 0057 006e  V0.......Y...W.n
+000011a0: 2e04 0074 056a 0679 9001 007d 0401 007a  ...t.j.y...}...z
+000011b0: 1464 037c 0466 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
+000011c0: 047e 0453 0064 007d 047e 0430 0030 006e  .~.S.d.}.~.0.0.n
+000011d0: 8a7a 587c 006a 008f 3e01 007c 006a 01a0  .zX|.j..>..|.j..
+000011e0: 0264 017c 029b 0064 029d 037c 0166 01a1  .d.|...d...|.f..
+000011f0: 0201 007c 006a 01a0 04a1 0044 005d 0a7d  ...|.j.....D.].}
+00001200: 037c 0356 0001 0071 c057 0064 0004 0004  .|.V...q.W.d....
+00001210: 0083 0301 006e 1031 0073 e030 0001 0001  .....n.1.s.0....
+00001220: 0001 0059 0001 0057 006e 3004 0074 056a  ...Y...W.n0..t.j
+00001230: 0690 0179 1c01 007d 0401 007a 1464 047c  ...y...}...z.d.|
+00001240: 0466 0257 0006 0059 0064 007d 047e 0453  .f.W...Y.d.}.~.S
+00001250: 0064 007d 047e 0430 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00001260: 054e 7240 0000 007a 0e20 5748 4552 4520  .Nr@...z. WHERE 
+00001270: 4944 203d 203f 2072 2400 0000 7201 0000  ID = ? r$...r...
+00001280: 0072 4200 0000 2905 7211 0000 0072 4400  .rB...).r....rD.
+00001290: 0000 7234 0000 0072 4300 0000 7219 0000  ..r4...rC...r...
+000012a0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+000012b0: da0d 636f 6e74 656e 745f 6279 5f69 64a7  ..content_by_id.
+000012c0: 0000 0073 2600 0000 0001 0801 0201 0801  ...s&...........
+000012d0: 0601 10ff 0402 0e01 2a02 1001 2003 0201  ........*... ...
+000012e0: 0801 0601 0eff 0402 0e01 2a02 1201 7a16  ..........*...z.
+000012f0: 4461 7461 6261 7365 2e63 6f6e 7465 6e74  Database.content
+00001300: 5f62 795f 6964 6301 0000 0000 0000 0000  _by_idc.........
+00001310: 0000 0005 0000 000a 0000 0067 0000 0073  ...........g...s
+00001320: 2a01 0000 7c01 7298 7a62 7c01 4400 5d58  *...|.r.zb|.D.]X
+00001330: 7d02 7c00 6a00 8f3e 0100 7c00 6a01 a002  }.|.j..>..|.j...
+00001340: 6401 7c02 9b00 6402 9d03 a101 0100 7c00  d.|...d.......|.
+00001350: 6a01 a003 a100 4400 5d0e 7d03 7c02 7c03  j.....D.].}.|.|.
+00001360: 6901 5600 0100 7134 5700 6400 0400 0400  i.V...q4W.d.....
+00001370: 8303 0100 710a 3100 7358 3000 0100 0100  ....q.1.sX0.....
+00001380: 0100 5900 0100 710a 5700 6e2e 0400 7404  ..Y...q.W.n...t.
+00001390: 6a05 7994 0100 7d04 0100 7a14 6403 7c04  j.y...}...z.d.|.
+000013a0: 6602 5700 0600 5900 6400 7d04 7e04 5300  f.W...Y.d.}.~.S.
+000013b0: 6400 7d04 7e04 3000 3000 6e8e 7a5c 7c00  d.}.~.0.0.n.z\|.
+000013c0: 6a00 8f42 0100 7c00 6a01 a002 6401 7c00  j..B..|.j...d.|.
+000013d0: 6a06 9b00 6402 9d03 a101 0100 7c00 6a01  j...d.......|.j.
+000013e0: a003 a100 4400 5d10 7d03 7c00 6a06 7c03  ....D.].}.|.j.|.
+000013f0: 6901 5600 0100 71c2 5700 6400 0400 0400  i.V...q.W.d.....
+00001400: 8303 0100 6e10 3100 73e8 3000 0100 0100  ....n.1.s.0.....
+00001410: 0100 5900 0100 5700 6e30 0400 7404 6a05  ..Y...W.n0..t.j.
+00001420: 9001 7924 0100 7d04 0100 7a14 6404 7c04  ..y$..}...z.d.|.
+00001430: 6602 5700 0600 5900 6400 7d04 7e04 5300  f.W...Y.d.}.~.S.
+00001440: 6400 7d04 7e04 3000 3000 6400 5300 723f  d.}.~.0.0.d.S.r?
+00001450: 0000 0029 0772 0c00 0000 720d 0000 0072  ...).r....r....r
+00001460: 1500 0000 722d 0000 0072 0e00 0000 7217  ....r-...r....r.
+00001470: 0000 0072 0900 0000 2905 7211 0000 005a  ...r....).r....Z
+00001480: 136f 7074 696f 6e61 6c5f 7461 626c 656e  .optional_tablen
+00001490: 616d 6573 da03 6172 6772 4300 0000 7219  ames..argrC...r.
+000014a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+000014b0: 0000 da0d 7368 6f77 5f63 6f6e 7465 6e74  ....show_content
+000014c0: 73be 0000 0073 2000 0000 0001 0401 0201  s....s .........
+000014d0: 0801 0801 1401 0e01 3002 1001 2003 0201  ........0... ...
+000014e0: 0801 1601 0e01 3002 1201 7a16 4461 7461  ......0...z.Data
+000014f0: 6261 7365 2e73 686f 775f 636f 6e74 656e  base.show_conten
+00001500: 7473 6301 0000 0000 0000 0000 0000 0003  tsc.............
+00001510: 0000 000a 0000 0063 0000 0073 8000 0000  .......c...s....
+00001520: 7a4c 7c00 6a00 8f32 0100 7c00 6a01 a002  zL|.j..2..|.j...
+00001530: 6401 a101 0100 7c00 6a01 a003 a100 4400  d.....|.j.....D.
+00001540: 5d0a 7d01 7c01 5600 0100 7120 5700 6400  ].}.|.V...q W.d.
+00001550: 0400 0400 8303 0100 6e10 3100 7340 3000  ........n.1.s@0.
+00001560: 0100 0100 0100 5900 0100 5700 6e2e 0400  ......Y...W.n...
+00001570: 7404 6a05 797a 0100 7d02 0100 7a14 6402  t.j.yz..}...z.d.
+00001580: 7c02 6602 5700 0600 5900 6400 7d02 7e02  |.f.W...Y.d.}.~.
+00001590: 5300 6400 7d02 7e02 3000 3000 6400 5300  S.d.}.~.0.0.d.S.
+000015a0: 2903 4efa 3353 454c 4543 5420 6e61 6d65  ).N.3SELECT name
+000015b0: 2046 524f 4d20 7371 6c69 7465 5f6d 6173   FROM sqlite_mas
+000015c0: 7465 7220 5748 4552 4520 7479 7065 3d20  ter WHERE type= 
+000015d0: 2774 6162 6c65 2720 7201 0000 00a9 0672  'table' r......r
+000015e0: 0c00 0000 720d 0000 0072 1500 0000 722d  ....r....r....r-
+000015f0: 0000 0072 0e00 0000 7217 0000 0029 0372  ...r....r....).r
+00001600: 1100 0000 7243 0000 0072 1900 0000 7212  ....rC...r....r.
+00001610: 0000 0072 1200 0000 7213 0000 00da 0b73  ...r....r......s
+00001620: 686f 775f 7461 626c 6573 d400 0000 7312  how_tables....s.
+00001630: 0000 0000 0102 0108 0106 0102 ff04 020e  ................
+00001640: 012a 0210 017a 1444 6174 6162 6173 652e  .*...z.Database.
+00001650: 7368 6f77 5f74 6162 6c65 7363 0100 0000  show_tablesc....
+00001660: 0000 0000 0000 0000 0300 0000 0a00 0000  ................
+00001670: 4300 0000 7394 0000 007a 607c 006a 008f  C...s....z`|.j..
+00001680: 4601 007c 006a 01a0 0264 01a1 0101 007c  F..|.j...d.....|
+00001690: 006a 01a0 03a1 0044 005d 1a7d 017c 006a  .j.....D.].}.|.j
+000016a0: 01a0 0264 027c 0164 0319 009b 009d 02a1  ...d.|.d........
+000016b0: 0101 0071 2057 0064 0004 0004 0083 0301  ...q W.d........
+000016c0: 0057 0064 0453 0031 0073 5430 0001 0001  .W.d.S.1.sT0....
+000016d0: 0001 0059 0001 0057 006e 2e04 0074 046a  ...Y...W.n...t.j
+000016e0: 0579 8e01 007d 0201 007a 1464 037c 0266  .y...}...z.d.|.f
+000016f0: 0257 0006 0059 0064 007d 027e 0253 0064  .W...Y.d.}.~.S.d
+00001700: 007d 027e 0230 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
+00001710: 7248 0000 00fa 0b44 524f 5020 5441 424c  rH.....DROP TABL
+00001720: 4520 7201 0000 0072 2500 0000 7249 0000  E r....r%...rI..
+00001730: 0029 0372 1100 0000 da05 7461 626c 6572  .).r......tabler
+00001740: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00001750: 0000 00da 0764 726f 7061 6c6c df00 0000  .....dropall....
+00001760: 7314 0000 0000 0102 0108 0106 0102 ff04  s...............
+00001770: 020e 0118 0126 0210 017a 1044 6174 6162  .....&...z.Datab
+00001780: 6173 652e 6472 6f70 616c 6c63 0100 0000  ase.dropallc....
+00001790: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
+000017a0: 4700 0000 73f6 0000 007c 0172 7e7a 487c  G...s....|.r~zH|
+000017b0: 0144 005d 3c7d 027c 006a 008f 2201 007c  .D.]<}.|.j.."..|
+000017c0: 006a 01a0 0264 017c 029b 009d 02a1 0101  .j...d.|........
+000017d0: 0057 0064 0004 0004 0083 0301 0071 0a31  .W.d.........q.1
+000017e0: 0073 3c30 0001 0001 0001 0059 0001 0071  .s<0.......Y...q
+000017f0: 0a57 0064 0253 0004 0074 036a 0479 7a01  .W.d.S...t.j.yz.
+00001800: 007d 0301 007a 1464 037c 0366 0257 0006  .}...z.d.|.f.W..
+00001810: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
+00001820: 0330 0030 006e 747a 427c 006a 008f 2801  .0.0.ntzB|.j..(.
+00001830: 007c 006a 01a0 0264 017c 006a 059b 009d  .|.j...d.|.j....
+00001840: 02a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00001850: 0057 0064 0253 0031 0073 b430 0001 0001  .W.d.S.1.s.0....
+00001860: 0001 0059 0001 0057 006e 3004 0074 036a  ...Y...W.n0..t.j
+00001870: 0490 0079 f001 007d 0301 007a 1464 047c  ...y...}...z.d.|
+00001880: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
+00001890: 0064 007d 037e 0330 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+000018a0: 054e 724b 0000 0072 2500 0000 7224 0000  .NrK...r%...r$..
+000018b0: 0072 0100 0000 2906 720c 0000 0072 0d00  .r....).r....r..
+000018c0: 0000 7215 0000 0072 0e00 0000 7217 0000  ..r....r....r...
+000018d0: 0072 0900 0000 2904 7211 0000 005a 0b74  .r....).r....Z.t
+000018e0: 6162 6c65 5f6e 616d 6573 7246 0000 0072  able_namesrF...r
+000018f0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00001900: 0000 00da 0a64 726f 705f 7461 626c 65eb  .....drop_table.
+00001910: 0000 0073 1c00 0000 0001 0401 0201 0801  ...s............
+00001920: 0801 3201 0601 1001 2003 0201 0801 1401  ..2..... .......
+00001930: 2602 1201 7a13 4461 7461 6261 7365 2e64  &...z.Database.d
+00001940: 726f 705f 7461 626c 6563 0300 0000 0000  rop_tablec......
+00001950: 0000 0000 0000 0400 0000 0a00 0000 4300  ..............C.
+00001960: 0000 73fa 0000 007c 0264 0075 0072 807a  ..s....|.d.u.r.z
+00001970: 467c 006a 008f 2a01 007c 006a 01a0 0264  F|.j..*..|.j...d
+00001980: 017c 006a 039b 0064 027c 019b 009d 04a1  .|.j...d.|......
+00001990: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+000019a0: 1031 0073 4030 0001 0001 0001 0059 0001  .1.s@0.......Y..
+000019b0: 0057 0064 0353 0004 0074 046a 0579 7c01  .W.d.S...t.j.y|.
+000019c0: 007d 0301 007a 1464 047c 0366 0257 0006  .}...z.d.|.f.W..
+000019d0: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
+000019e0: 0330 0030 006e 767a 447c 006a 008f 2801  .0.0.nvzD|.j..(.
+000019f0: 007c 006a 01a0 0264 017c 029b 0064 027c  .|.j...d.|...d.|
+00001a00: 019b 009d 04a1 0101 0057 0064 0004 0004  .........W.d....
+00001a10: 0083 0301 006e 1031 0073 b630 0001 0001  .....n.1.s.0....
+00001a20: 0001 0059 0001 0057 0064 0553 0004 0074  ...Y...W.d.S...t
+00001a30: 046a 0590 0079 f401 007d 0301 007a 1464  .j...y...}...z.d
+00001a40: 067c 0366 0257 0006 0059 0064 007d 037e  .|.f.W...Y.d.}.~
+00001a50: 0353 0064 007d 037e 0330 0030 0064 0053  .S.d.}.~.0.0.d.S
+00001a60: 0029 074e 7a0c 4445 4c45 5445 2046 524f  .).Nz.DELETE FRO
+00001a70: 4d20 7a0c 2057 4845 5245 2049 4420 3d20  M z. WHERE ID = 
+00001a80: 7232 0000 0072 2400 0000 7225 0000 0072  r2...r$...r%...r
+00001a90: 0100 0000 7233 0000 0029 0472 1100 0000  ....r3...).r....
+00001aa0: 723d 0000 0072 3900 0000 7219 0000 0072  r=...r9...r....r
+00001ab0: 1200 0000 7212 0000 0072 1300 0000 da0c  ....r....r......
+00001ac0: 6472 6f70 5f63 6f6e 7465 6e74 fe00 0000  drop_content....
+00001ad0: 7322 0000 0000 0108 0102 0108 0106 0110  s"..............
+00001ae0: ff22 0206 0210 0120 0302 0108 0106 010e  ."..... ........
+00001af0: ff22 0206 0212 017a 1544 6174 6162 6173  .".....z.Databas
+00001b00: 652e 6472 6f70 5f63 6f6e 7465 6e74 2901  e.drop_content).
+00001b10: 4e29 014e 2901 4e29 014e 2901 4e29 014e  N).N).N).N).N).N
+00001b20: 2922 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )"..__name__..__
+00001b30: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001b40: 6e61 6d65 5f5f 7203 0000 0072 0700 0000  name__r....r....
+00001b50: 722a 0000 00da 0f5f 5f61 6e6e 6f74 6174  r*.....__annotat
+00001b60: 696f 6e73 5f5f 7209 0000 0072 0c00 0000  ions__r....r....
+00001b70: 720e 0000 005a 0a43 6f6e 6e65 6374 696f  r....Z.Connectio
+00001b80: 6e72 0d00 0000 5a06 4375 7273 6f72 7214  nr....Z.Cursorr.
+00001b90: 0000 00da 0870 726f 7065 7274 7972 1800  .....propertyr..
+00001ba0: 0000 7205 0000 0072 0400 0000 da05 7475  ..r....r......tu
+00001bb0: 706c 6572 2000 0000 7222 0000 00da 046c  pler ...r".....l
+00001bc0: 6973 7472 3100 0000 7235 0000 0072 3a00  istr1...r5...r:.
+00001bd0: 0000 da03 696e 7472 3e00 0000 7237 0000  ....intr>...r7..
+00001be0: 0072 4500 0000 7247 0000 0072 4a00 0000  .rE...rG...rJ...
+00001bf0: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
+00001c00: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00001c10: 0000 0072 0600 0000 0800 0000 7336 0000  ...r........s6..
+00001c20: 000a 020e 0112 0116 0116 0208 0402 010a  ................
+00001c30: 0b02 0118 0802 010a 0310 130a 1a0a 1f00  ................
+00001c40: fb02 0202 0102 0102 fc0c 1f0a 1510 1708  ................
+00001c50: 160e 0b08 0c08 1372 0600 0000 2909 5a0b  .......r....).Z.
+00001c60: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
+00001c70: 7203 0000 0072 0400 0000 da06 7479 7069  r....r......typi
+00001c80: 6e67 7205 0000 0072 0e00 0000 721c 0000  ngr....r....r...
+00001c90: 0072 0600 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001ca0: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
+00001cb0: 756c 653e 0100 0000 730c 0000 0010 010c  ule>....s.......
+00001cc0: 010c 0108 0108 0302 01                   .........
```

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Jul  1 02:35:10 2023 UTC, .py size: 3849 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 de90 9f64 090f 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 f8db ad64 b10f 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000050: 5a04 4700 6405 6406 8400 6406 8302 5a05  Z.G.d.d...d...Z.
 00000060: 6402 5300 2907 e900 0000 0029 01da 0341  d.S.)......)...A
 00000070: 7368 4e63 0000 0000 0000 0000 0000 0000  shNc............
@@ -10,29 +10,29 @@
 00000090: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
 000000a0: 0284 085a 0387 0004 005a 0453 0029 03da  ...Z.....Z.S.)..
 000000b0: 084b 6579 4572 726f 7263 0100 0000 0000  .KeyErrorc......
 000000c0: 0000 0000 0000 0100 0000 0300 0000 0300  ................
 000000d0: 0000 7318 0000 0064 017c 005f 0074 0183  ..s....d.|._.t..
 000000e0: 00a0 027c 006a 00a1 0101 0064 0053 0029  ...|.j.....d.S.)
 000000f0: 024e 7a1a 4b65 7920 6d75 7374 2062 6520  .Nz.Key must be 
-00000100: 3531 3220 4269 7420 6c6f 6e67 2021 2903  512 Bit long !).
+00000100: 3235 3620 4269 7420 6c6f 6e67 2021 2903  256 Bit long !).
 00000110: 5a07 6469 7370 6c61 79da 0573 7570 6572  Z.display..super
 00000120: da08 5f5f 696e 6974 5f5f a901 da04 7365  ..__init__....se
 00000130: 6c66 a901 da09 5f5f 636c 6173 735f 5fa9  lf....__class__.
 00000140: 00fa 3043 3a5c 576f 726b 5c47 6974 4875  ..0C:\Work\GitHu
 00000150: 6257 6f72 6b5c 4145 532d 3235 365c 4173  bWork\AES-256\As
 00000160: 6843 7279 7074 5c46 696c 6543 7279 7074  hCrypt\FileCrypt
-00000170: 2e70 7972 0500 0000 0500 0000 7304 0000  .pyr........s...
+00000170: 2e70 7972 0500 0000 0600 0000 7304 0000  .pyr........s...
 00000180: 0000 0106 017a 114b 6579 4572 726f 722e  .....z.KeyError.
 00000190: 5f5f 696e 6974 5f5f 2905 da08 5f5f 6e61  __init__)...__na
 000001a0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000001b0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7205  ..__qualname__r.
 000001c0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
 000001d0: 5f5f 720a 0000 0072 0a00 0000 7208 0000  __r....r....r...
-000001e0: 0072 0b00 0000 7203 0000 0004 0000 0073  .r....r........s
+000001e0: 0072 0b00 0000 7203 0000 0005 0000 0073  .r....r........s
 000001f0: 0200 0000 0801 7203 0000 0063 0000 0000  ......r....c....
 00000200: 0000 0000 0000 0000 0000 0000 0400 0000  ................
 00000210: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
 00000220: 0264 0164 0284 005a 0365 0465 0564 039c  .d.d...Z.e.e.d..
 00000230: 0164 0464 0584 0483 015a 0665 0465 0565  .d.d.....Z.e.e.e
 00000240: 0764 069c 0264 0764 0884 0483 015a 0865  .d...d.d.....Z.e
 00000250: 0764 039c 0164 0964 0a84 045a 0965 0764  .d...d.d...Z.e.d
@@ -41,163 +41,166 @@
 00000280: 12da 0943 7279 7074 4669 6c65 6303 0000  ...CryptFilec...
 00000290: 0000 0000 0000 0000 0003 0000 0003 0000  ................
 000002a0: 0043 0000 0073 2c00 0000 7c01 7c00 5f00  .C...s,...|.|._.
 000002b0: 6401 7c00 5f01 7c00 a002 7c02 a101 6402  d.|._.|...|...d.
 000002c0: 6b02 7222 7c02 7c00 5f03 6e06 6402 7c00  k.r"|.|._.n.d.|.
 000002d0: 5f01 6400 5300 2903 4e72 0100 0000 e901  _.d.S.).Nr......
 000002e0: 0000 0029 04da 0866 696c 656e 616d 65da  ...)...filename.
-000002f0: 0f6e 6f74 5f35 3132 5f62 6974 5f6b 6579  .not_512_bit_key
+000002f0: 0f6e 6f74 5f32 3536 5f62 6974 5f6b 6579  .not_256_bit_key
 00000300: da09 6b65 7976 6572 6966 79da 036b 6579  ..keyverify..key
 00000310: 2903 7207 0000 0072 1200 0000 7215 0000  ).r....r....r...
 00000320: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000330: 7205 0000 000a 0000 0073 0a00 0000 0001  r........s......
+00000330: 7205 0000 000c 0000 0073 0a00 0000 0001  r........s......
 00000340: 0601 0601 0e01 0802 7a12 4372 7970 7446  ........z.CryptF
 00000350: 696c 652e 5f5f 696e 6974 5f5f 2901 da06  ile.__init__)...
 00000360: 7265 7475 726e 6300 0000 0000 0000 0000  returnc.........
 00000370: 0000 0000 0000 0002 0000 0043 0000 0073  ...........C...s
 00000380: 0a00 0000 7400 6a01 a002 a100 5300 2901  ....t.j.....S.).
 00000390: 4e29 0372 0200 0000 da03 456e 635a 0a67  N).r......EncZ.g
 000003a0: 656e 4d61 696e 6b65 7972 0a00 0000 720a  enMainkeyr....r.
 000003b0: 0000 0072 0a00 0000 720b 0000 00da 0667  ...r....r......g
-000003c0: 656e 6b65 7912 0000 0073 0200 0000 0002  enkey....s......
+000003c0: 656e 6b65 7914 0000 0073 0200 0000 0002  enkey....s......
 000003d0: 7a10 4372 7970 7446 696c 652e 6765 6e6b  z.CryptFile.genk
 000003e0: 6579 2902 7215 0000 0072 1600 0000 6301  ey).r....r....c.
-000003f0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000400: 0000 0043 0000 0073 4800 0000 7a34 7400  ...C...sH...z4t.
+000003f0: 0000 0000 0000 0000 0000 0002 0000 0008  ................
+00000400: 0000 0043 0000 0073 4e00 0000 7a34 7400  ...C...sN...z4t.
 00000410: 7c00 7401 8302 7232 7402 a003 7c00 a004  |.t...r2t...|...
 00000420: a100 a101 7d01 7405 7c01 8301 6401 6b02  ....}.t.|...d.k.
 00000430: 722c 5700 6402 5300 5700 6403 5300 5700  r,W.d.S.W.d.S.W.
-00000440: 6e0e 0100 0100 0100 5900 6404 5300 3000  n.......Y.d.S.0.
-00000450: 6400 5300 2905 4ee9 4000 0000 7211 0000  d.S.).N.@...r...
-00000460: 0072 0100 0000 e902 0000 0029 06da 0a69  .r.........)...i
-00000470: 7369 6e73 7461 6e63 65da 0373 7472 da05  sinstance..str..
-00000480: 6279 7465 73da 0766 726f 6d68 6578 da05  bytes..fromhex..
-00000490: 7374 7269 70da 036c 656e 2902 7215 0000  strip..len).r...
-000004a0: 00da 0161 720a 0000 0072 0a00 0000 720b  ...ar....r....r.
-000004b0: 0000 0072 1400 0000 1600 0000 7310 0000  ...r........s...
-000004c0: 0000 0202 010a 010e 010c 0106 020a 0106  ................
-000004d0: 017a 1343 7279 7074 4669 6c65 2e6b 6579  .z.CryptFile.key
-000004e0: 7665 7269 6679 6301 0000 0000 0000 0000  verifyc.........
-000004f0: 0000 0006 0000 0008 0000 0043 0000 0073  ...........C...s
-00000500: 7001 0000 7400 6a01 a002 7c00 6a03 a101  p...t.j...|.j...
-00000510: 7212 6401 5300 7c00 6a04 6402 6b02 7220  r.d.S.|.j.d.k.r 
-00000520: 6403 5300 9001 7a32 6404 7d01 7400 6a01  d.S...z2d.}.t.j.
-00000530: a005 7c00 6a03 a101 733c 5700 6405 5300  ..|.j...s<W.d.S.
-00000540: 7400 6a01 a006 7c00 6a03 a101 6402 1900  t.j...|.j...d...
-00000550: 6406 6b02 7258 5700 6407 5300 7407 7c00  d.k.rXW.d.S.t.|.
-00000560: 6a03 6408 8302 8f18 7d02 7c02 a008 a100  j.d.....}.|.....
-00000570: 7d03 5700 6400 0400 0400 8303 0100 6e10  }.W.d.........n.
-00000580: 3100 7382 3000 0100 0100 0100 5900 0100  1.s.0.......Y...
-00000590: 7407 7c00 6a03 6409 8302 8f84 7d02 7c03  t.|.j.d.....}.|.
-000005a0: 72f2 7a2a 7409 6a0a 7c03 7c00 6a0b 640a  r.z*t.j.|.|.j.d.
-000005b0: 8d02 7d04 7c04 a00c a100 7d05 7c02 a00d  ..}.|.....}.|...
-000005c0: 7c05 a101 0100 6402 7d01 5700 6e26 0100  |.....d.}.W.n&..
-000005d0: 0100 0100 7c02 a00d 7c03 a101 0100 5900  ....|...|.....Y.
-000005e0: 5700 6400 0400 0400 8303 0100 5700 6404  W.d.........W.d.
-000005f0: 5300 3000 6e1c 7c02 a00d 7c03 a101 0100  S.0.n.|...|.....
-00000600: 5700 6400 0400 0400 8303 0100 5700 640b  W.d.........W.d.
-00000610: 5300 5700 6400 0400 0400 8303 0100 6e12  S.W.d.........n.
-00000620: 3100 9001 7324 3000 0100 0100 0100 5900  1...s$0.......Y.
-00000630: 0100 7c01 6402 6b02 9001 7252 7400 a00e  ..|.d.k...rRt...
-00000640: 7c00 6a03 7c00 6a03 6406 1700 a102 0100  |.j.|.j.d.......
-00000650: 5700 6402 5300 5700 6e16 0400 740f 9001  W.d.S.W.n...t...
-00000660: 796a 0100 0100 0100 5900 640c 5300 3000  yj......Y.d.S.0.
-00000670: 6400 5300 a90d 4ee9 0700 0000 7211 0000  d.S...N.....r...
-00000680: 00e9 0500 0000 7201 0000 00e9 0300 0000  ......r.........
-00000690: 7a06 2e63 7279 7074 e906 0000 005a 0272  z..crypt.....Z.r
-000006a0: 62da 0277 6229 02da 076d 6573 7361 6765  b..wb)...message
-000006b0: 5a07 6d61 696e 6b65 7972 1a00 0000 e904  Z.mainkeyr......
-000006c0: 0000 0029 10da 026f 73da 0470 6174 68da  ...)...os..path.
-000006d0: 0569 7364 6972 7212 0000 0072 1300 0000  .isdirr....r....
-000006e0: da06 6578 6973 7473 da08 7370 6c69 7465  ..exists..splite
-000006f0: 7874 da04 6f70 656e da04 7265 6164 7202  xt..open..readr.
-00000700: 0000 0072 1700 0000 7215 0000 005a 0a65  ...r....r....Z.e
-00000710: 6e63 546f 4279 7465 73da 0577 7269 7465  ncToBytes..write
-00000720: da06 7265 6e61 6d65 da09 4578 6365 7074  ..rename..Except
-00000730: 696f 6e29 0672 0700 0000 5a15 676f 5f61  ion).r....Z.go_a
-00000740: 6865 6164 5f72 656e 616d 655f 6372 7970  head_rename_cryp
-00000750: 74da 0166 5a0b 6669 6c65 636f 6e74 656e  t..fZ.fileconten
-00000760: 74da 0369 6e73 5a0b 6e65 775f 636f 6e74  t..insZ.new_cont
-00000770: 656e 7472 0a00 0000 720a 0000 0072 0b00  entr....r....r..
-00000780: 0000 da07 656e 6372 7970 7422 0000 0073  ....encrypt"...s
-00000790: 3a00 0000 0001 0e01 0401 0a01 0401 0401  :...............
-000007a0: 0401 0e01 0602 1601 0602 0e01 2601 0e01  ............&...
-000007b0: 0401 0201 1001 0801 0a01 0801 0601 0a01  ................
-000007c0: 1802 0a01 3201 0a01 1401 0a01 0e01 7a11  ....2.........z.
-000007d0: 4372 7970 7446 696c 652e 656e 6372 7970  CryptFile.encryp
-000007e0: 7463 0100 0000 0000 0000 0000 0000 0600  tc..............
-000007f0: 0000 0900 0000 4300 0000 7382 0100 0074  ......C...s....t
-00000800: 006a 01a0 027c 006a 03a1 0172 1264 0153  .j...|.j...r.d.S
-00000810: 007c 006a 0464 026b 0272 2064 0353 0090  .|.j.d.k.r d.S..
-00000820: 017a 4464 047d 0174 006a 01a0 057c 006a  .zDd.}.t.j...|.j
-00000830: 03a1 0173 3c57 0064 0553 0074 006a 01a0  ...s<W.d.S.t.j..
-00000840: 067c 006a 03a1 0164 0219 0064 066b 0372  .|.j...d...d.k.r
-00000850: 5857 0064 0753 0074 077c 006a 0364 0883  XW.d.S.t.|.j.d..
-00000860: 028f 187d 027c 02a0 08a1 007d 0357 0064  ...}.|.....}.W.d
-00000870: 0004 0004 0083 0301 006e 1031 0073 8230  .........n.1.s.0
-00000880: 0001 0001 0001 0059 0001 0074 077c 006a  .......Y...t.|.j
-00000890: 0364 0983 028f 8e7d 027c 0390 0072 fc7a  .d.....}.|...r.z
-000008a0: 2a74 096a 0a7c 037c 006a 0b64 0a8d 027d  *t.j.|.|.j.d...}
-000008b0: 047c 04a0 0ca1 007d 057c 02a0 0d7c 05a1  .|.....}.|...|..
-000008c0: 0101 0064 027d 0157 006e 2e04 0074 0e90  ...d.}.W.n...t..
-000008d0: 0079 f801 0001 0001 007c 02a0 0d7c 03a1  .y.......|...|..
-000008e0: 0101 0059 0057 0064 0004 0004 0083 0301  ...Y.W.d........
-000008f0: 0057 0064 0453 0030 006e 1c7c 02a0 0d7c  .W.d.S.0.n.|...|
-00000900: 03a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00000910: 0057 0064 0b53 0057 0064 0004 0004 0083  .W.d.S.W.d......
-00000920: 0301 006e 1231 0090 0173 2e30 0001 0001  ...n.1...s.0....
-00000930: 0001 0059 0001 007c 0164 026b 0290 0172  ...Y...|.d.k...r
-00000940: 6474 00a0 0f7c 006a 0374 006a 01a0 067c  dt...|.j.t.j...|
-00000950: 006a 03a1 0164 0419 00a1 0201 0057 0064  .j...d.......W.d
-00000960: 0253 0057 006e 1604 0074 0e90 0179 7c01  .S.W.n...t...y|.
-00000970: 0001 0001 0059 0064 0c53 0030 0064 0053  .....Y.d.S.0.d.S
-00000980: 0072 2200 0000 2910 722a 0000 0072 2b00  .r"...).r*...r+.
-00000990: 0000 722c 0000 0072 1200 0000 7213 0000  ..r,...r....r...
-000009a0: 0072 2d00 0000 722e 0000 0072 2f00 0000  .r-...r....r/...
-000009b0: 7230 0000 0072 0200 0000 5a03 4465 6372  r0...r....Z.Decr
-000009c0: 1500 0000 5a0a 6465 6354 6f42 7974 6573  ....Z.decToBytes
-000009d0: 7231 0000 0072 3300 0000 7232 0000 0029  r1...r3...r2...)
-000009e0: 0672 0700 0000 5a15 676f 5f61 6865 6164  .r....Z.go_ahead
-000009f0: 5f72 656d 6f76 655f 6372 7970 7472 3400  _remove_cryptr4.
-00000a00: 0000 5a0b 656e 635f 636f 6e74 656e 7472  ..Z.enc_contentr
-00000a10: 3500 0000 7221 0000 0072 0a00 0000 720a  5...r!...r....r.
-00000a20: 0000 0072 0b00 0000 da07 6465 6372 7970  ...r......decryp
-00000a30: 7444 0000 0073 3a00 0000 0001 0e01 0401  tD...s:.........
-00000a40: 0a01 0401 0401 0401 0e01 0602 1601 0602  ................
-00000a50: 0e01 2601 0e01 0601 0201 1001 0801 0a01  ..&.............
-00000a60: 0801 0e01 0a01 1802 0a01 3201 0a01 1c01  ..........2.....
-00000a70: 0a01 0e01 7a11 4372 7970 7446 696c 652e  ....z.CryptFile.
-00000a80: 6465 6372 7970 7463 0100 0000 0000 0000  decryptc........
-00000a90: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00000aa0: 7316 0000 0064 017c 006a 009b 0064 027c  s....d.|.j...d.|
-00000ab0: 006a 019b 0064 039d 0553 0029 044e 7a1b  .j...d...S.).Nz.
-00000ac0: 456e 6372 7970 7469 6e67 2f44 6563 7279  Encrypting/Decry
-00000ad0: 7074 696e 6720 4669 6c65 207a 0620 5769  pting File z. Wi
-00000ae0: 7468 207a 0520 4b65 7920 2902 7212 0000  th z. Key ).r...
-00000af0: 0072 1500 0000 7206 0000 0072 0a00 0000  .r....r....r....
-00000b00: 720a 0000 0072 0b00 0000 da07 5f5f 7374  r....r......__st
-00000b10: 725f 5f66 0000 0073 0200 0000 0001 7a11  r__f...s......z.
-00000b20: 4372 7970 7446 696c 652e 5f5f 7374 725f  CryptFile.__str_
-00000b30: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000b40: 0000 0600 0000 4300 0000 731e 0000 007c  ......C...s....|
-00000b50: 006a 006a 019b 0064 017c 006a 029b 0064  .j.j...d.|.j...d
-00000b60: 027c 006a 039b 0064 039d 0653 0029 044e  .|.j...d...S.).N
-00000b70: fa01 28fa 012c fa01 2929 0472 0900 0000  ..(..,..)).r....
-00000b80: 720c 0000 0072 1200 0000 7215 0000 0072  r....r....r....r
-00000b90: 0600 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-00000ba0: 0000 00da 085f 5f72 6570 725f 5f68 0000  .....__repr__h..
-00000bb0: 0073 0200 0000 0001 7a12 4372 7970 7446  .s......z.CryptF
-00000bc0: 696c 652e 5f5f 7265 7072 5f5f 4e29 0d72  ile.__repr__N).r
-00000bd0: 0c00 0000 720d 0000 0072 0e00 0000 7205  ....r....r....r.
-00000be0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
-00000bf0: 6472 1c00 0000 7218 0000 00da 0369 6e74  dr....r......int
-00000c00: 7214 0000 0072 3600 0000 7237 0000 0072  r....r6...r7...r
-00000c10: 3800 0000 723c 0000 0072 0a00 0000 720a  8...r<...r....r.
-00000c20: 0000 0072 0a00 0000 720b 0000 0072 1000  ...r....r....r..
-00000c30: 0000 0900 0000 7312 0000 0008 0108 0802  ......s.........
-00000c40: 0110 0302 0112 0b0e 220e 2208 0272 1000  ........"."..r..
-00000c50: 0000 2906 da08 4173 6843 7279 7074 7202  ..)...AshCryptr.
-00000c60: 0000 0072 2a00 0000 7233 0000 0072 0300  ...r*...r3...r..
-00000c70: 0000 7210 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000c80: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
-00000c90: 6475 6c65 3e01 0000 0073 0600 0000 0c01  dule>....s......
-00000ca0: 0802 1005                                ....
+00000440: 6e14 0400 7406 7948 0100 0100 0100 5900  n...t.yH......Y.
+00000450: 6404 5300 3000 6400 5300 2905 4ee9 2000  d.S.0.d.S.).N. .
+00000460: 0000 7211 0000 0072 0100 0000 e902 0000  ..r....r........
+00000470: 0029 07da 0a69 7369 6e73 7461 6e63 65da  .)...isinstance.
+00000480: 0373 7472 da05 6279 7465 73da 0766 726f  .str..bytes..fro
+00000490: 6d68 6578 da05 7374 7269 70da 036c 656e  mhex..strip..len
+000004a0: da0d 4261 7365 4578 6365 7074 696f 6e29  ..BaseException)
+000004b0: 0272 1500 0000 da01 6172 0a00 0000 720a  .r......ar....r.
+000004c0: 0000 0072 0b00 0000 7214 0000 0018 0000  ...r....r.......
+000004d0: 0073 1000 0000 0002 0201 0a01 0e01 0c01  .s..............
+000004e0: 0602 0a01 0c01 7a13 4372 7970 7446 696c  ......z.CryptFil
+000004f0: 652e 6b65 7976 6572 6966 7963 0100 0000  e.keyverifyc....
+00000500: 0000 0000 0000 0000 0600 0000 0900 0000  ................
+00000510: 4300 0000 737a 0100 0074 006a 01a0 027c  C...sz...t.j...|
+00000520: 006a 03a1 0172 1264 0153 007c 006a 0464  .j...r.d.S.|.j.d
+00000530: 026b 0272 2064 0353 0090 017a 3c64 047d  .k.r d.S...z<d.}
+00000540: 0174 006a 01a0 057c 006a 03a1 0173 3c57  .t.j...|.j...s<W
+00000550: 0064 0553 0074 006a 01a0 067c 006a 03a1  .d.S.t.j...|.j..
+00000560: 0164 0219 0064 066b 0272 5857 0064 0753  .d...d.k.rXW.d.S
+00000570: 0074 077c 006a 0364 0883 028f 187d 027c  .t.|.j.d.....}.|
+00000580: 02a0 08a1 007d 0357 0064 0004 0004 0083  .....}.W.d......
+00000590: 0301 006e 1031 0073 8230 0001 0001 0001  ...n.1.s.0......
+000005a0: 0059 0001 0074 077c 006a 0364 0983 028f  .Y...t.|.j.d....
+000005b0: 8e7d 027c 0390 0072 fc7a 2a74 096a 0a7c  .}.|...r.z*t.j.|
+000005c0: 037c 006a 0b64 0a8d 027d 047c 04a0 0ca1  .|.j.d...}.|....
+000005d0: 007d 057c 02a0 0d7c 05a1 0101 0064 027d  .}.|...|.....d.}
+000005e0: 0157 006e 2e04 0074 0e90 0079 f801 0001  .W.n...t...y....
+000005f0: 0001 007c 02a0 0d7c 03a1 0101 0059 0057  ...|...|.....Y.W
+00000600: 0064 0004 0004 0083 0301 0057 0064 0453  .d.........W.d.S
+00000610: 0030 006e 1c7c 02a0 0d7c 03a1 0101 0057  .0.n.|...|.....W
+00000620: 0064 0004 0004 0083 0301 0057 0064 0b53  .d.........W.d.S
+00000630: 0057 0064 0004 0004 0083 0301 006e 1231  .W.d.........n.1
+00000640: 0090 0173 2e30 0001 0001 0001 0059 0001  ...s.0.......Y..
+00000650: 007c 0164 026b 0290 0172 5c74 00a0 0f7c  .|.d.k...r\t...|
+00000660: 006a 037c 006a 0364 0617 00a1 0201 0057  .j.|.j.d.......W
+00000670: 0064 0253 0057 006e 1604 0074 1090 0179  .d.S.W.n...t...y
+00000680: 7401 0001 0001 0059 0064 0c53 0030 0064  t......Y.d.S.0.d
+00000690: 0053 00a9 0d4e e907 0000 0072 1100 0000  .S...N.....r....
+000006a0: e905 0000 0072 0100 0000 e903 0000 007a  .....r.........z
+000006b0: 062e 6372 7970 74e9 0600 0000 5a02 7262  ..crypt.....Z.rb
+000006c0: da02 7762 2902 da07 6d65 7373 6167 655a  ..wb)...messageZ
+000006d0: 076d 6169 6e6b 6579 721a 0000 00e9 0400  .mainkeyr.......
+000006e0: 0000 2911 da02 6f73 da04 7061 7468 da05  ..)...os..path..
+000006f0: 6973 6469 7272 1200 0000 7213 0000 00da  isdirr....r.....
+00000700: 0665 7869 7374 73da 0873 706c 6974 6578  .exists..splitex
+00000710: 74da 046f 7065 6eda 0472 6561 6472 0200  t..open..readr..
+00000720: 0000 7217 0000 0072 1500 0000 5a0a 656e  ..r....r....Z.en
+00000730: 6354 6f42 7974 6573 da05 7772 6974 6572  cToBytes..writer
+00000740: 2100 0000 da06 7265 6e61 6d65 da09 4578  !.....rename..Ex
+00000750: 6365 7074 696f 6e29 0672 0700 0000 5a15  ception).r....Z.
+00000760: 676f 5f61 6865 6164 5f72 656e 616d 655f  go_ahead_rename_
+00000770: 6372 7970 74da 0166 5a0b 6669 6c65 636f  crypt..fZ.fileco
+00000780: 6e74 656e 74da 0369 6e73 5a0b 6e65 775f  ntent..insZ.new_
+00000790: 636f 6e74 656e 7472 0a00 0000 720a 0000  contentr....r...
+000007a0: 0072 0b00 0000 da07 656e 6372 7970 7424  .r......encrypt$
+000007b0: 0000 0073 3e00 0000 0001 0e01 0401 0a01  ...s>...........
+000007c0: 0401 0401 0401 0e01 0602 1601 0602 0e01  ................
+000007d0: 2601 0e01 0601 0201 0401 06ff 0602 0801  &...............
+000007e0: 0a01 0801 0e01 0a01 1802 0a01 3201 0a01  ............2...
+000007f0: 1401 0a01 0e01 7a11 4372 7970 7446 696c  ......z.CryptFil
+00000800: 652e 656e 6372 7970 7463 0100 0000 0000  e.encryptc......
+00000810: 0000 0000 0000 0600 0000 0900 0000 4300  ..............C.
+00000820: 0000 7382 0100 0074 006a 01a0 027c 006a  ..s....t.j...|.j
+00000830: 03a1 0172 1264 0153 007c 006a 0464 026b  ...r.d.S.|.j.d.k
+00000840: 0272 2064 0353 0090 017a 4464 047d 0174  .r d.S...zDd.}.t
+00000850: 006a 01a0 057c 006a 03a1 0173 3c57 0064  .j...|.j...s<W.d
+00000860: 0553 0074 006a 01a0 067c 006a 03a1 0164  .S.t.j...|.j...d
+00000870: 0219 0064 066b 0372 5857 0064 0753 0074  ...d.k.rXW.d.S.t
+00000880: 077c 006a 0364 0883 028f 187d 027c 02a0  .|.j.d.....}.|..
+00000890: 08a1 007d 0357 0064 0004 0004 0083 0301  ...}.W.d........
+000008a0: 006e 1031 0073 8230 0001 0001 0001 0059  .n.1.s.0.......Y
+000008b0: 0001 0074 077c 006a 0364 0983 028f 8e7d  ...t.|.j.d.....}
+000008c0: 027c 0390 0072 fc7a 2a74 096a 0a7c 037c  .|...r.z*t.j.|.|
+000008d0: 006a 0b64 0a8d 027d 047c 04a0 0ca1 007d  .j.d...}.|.....}
+000008e0: 057c 02a0 0d7c 05a1 0101 0064 027d 0157  .|...|.....d.}.W
+000008f0: 006e 2e04 0074 0e90 0079 f801 0001 0001  .n...t...y......
+00000900: 007c 02a0 0d7c 03a1 0101 0059 0057 0064  .|...|.....Y.W.d
+00000910: 0004 0004 0083 0301 0057 0064 0453 0030  .........W.d.S.0
+00000920: 006e 1c7c 02a0 0d7c 03a1 0101 0057 0064  .n.|...|.....W.d
+00000930: 0004 0004 0083 0301 0057 0064 0b53 0057  .........W.d.S.W
+00000940: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
+00000950: 0173 2e30 0001 0001 0001 0059 0001 007c  .s.0.......Y...|
+00000960: 0164 026b 0290 0172 6474 00a0 0f7c 006a  .d.k...rdt...|.j
+00000970: 0374 006a 01a0 067c 006a 03a1 0164 0419  .t.j...|.j...d..
+00000980: 00a1 0201 0057 0064 0253 0057 006e 1604  .....W.d.S.W.n..
+00000990: 0074 0e90 0179 7c01 0001 0001 0059 0064  .t...y|......Y.d
+000009a0: 0c53 0030 0064 0053 0072 2300 0000 2910  .S.0.d.S.r#...).
+000009b0: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+000009c0: 1200 0000 7213 0000 0072 2e00 0000 722f  ....r....r....r/
+000009d0: 0000 0072 3000 0000 7231 0000 0072 0200  ...r0...r1...r..
+000009e0: 0000 5a03 4465 6372 1500 0000 5a0a 6465  ..Z.Decr....Z.de
+000009f0: 6354 6f42 7974 6573 7232 0000 0072 3400  cToBytesr2...r4.
+00000a00: 0000 7233 0000 0029 0672 0700 0000 5a15  ..r3...).r....Z.
+00000a10: 676f 5f61 6865 6164 5f72 656d 6f76 655f  go_ahead_remove_
+00000a20: 6372 7970 7472 3500 0000 5a0b 656e 635f  cryptr5...Z.enc_
+00000a30: 636f 6e74 656e 7472 3600 0000 7222 0000  contentr6...r"..
+00000a40: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000a50: da07 6465 6372 7970 7447 0000 0073 4a00  ..decryptG...sJ.
+00000a60: 0000 0001 0e01 0401 0a01 0401 0401 0401  ................
+00000a70: 0e01 0602 1601 0602 0e01 2601 0e01 0601  ..........&.....
+00000a80: 0201 0401 06ff 0602 0801 0a01 0801 0e01  ................
+00000a90: 0a01 1802 0a01 3201 0a01 0401 0a01 04ff  ......2.........
+00000aa0: 0201 02ff 02ff 0403 0a01 0e01 7a11 4372  ............z.Cr
+00000ab0: 7970 7446 696c 652e 6465 6372 7970 7463  yptFile.decryptc
+00000ac0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000ad0: 0500 0000 4300 0000 7316 0000 0064 017c  ....C...s....d.|
+00000ae0: 006a 009b 0064 027c 006a 019b 0064 039d  .j...d.|.j...d..
+00000af0: 0553 0029 044e 7a1b 456e 6372 7970 7469  .S.).Nz.Encrypti
+00000b00: 6e67 2f44 6563 7279 7074 696e 6720 4669  ng/Decrypting Fi
+00000b10: 6c65 207a 0620 5769 7468 207a 0520 4b65  le z. With z. Ke
+00000b20: 7920 2902 7212 0000 0072 1500 0000 7206  y ).r....r....r.
+00000b30: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+00000b40: 0000 da07 5f5f 7374 725f 5f6c 0000 0073  ....__str__l...s
+00000b50: 0200 0000 0001 7a11 4372 7970 7446 696c  ......z.CryptFil
+00000b60: 652e 5f5f 7374 725f 5f63 0100 0000 0000  e.__str__c......
+00000b70: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
+00000b80: 0000 731e 0000 007c 006a 006a 019b 0064  ..s....|.j.j...d
+00000b90: 017c 006a 029b 0064 027c 006a 039b 0064  .|.j...d.|.j...d
+00000ba0: 039d 0653 0029 044e fa01 28fa 012c fa01  ...S.).N..(..,..
+00000bb0: 2929 0472 0900 0000 720c 0000 0072 1200  )).r....r....r..
+00000bc0: 0000 7215 0000 0072 0600 0000 720a 0000  ..r....r....r...
+00000bd0: 0072 0a00 0000 720b 0000 00da 085f 5f72  .r....r......__r
+00000be0: 6570 725f 5f6f 0000 0073 0200 0000 0001  epr__o...s......
+00000bf0: 7a12 4372 7970 7446 696c 652e 5f5f 7265  z.CryptFile.__re
+00000c00: 7072 5f5f 4e29 0d72 0c00 0000 720d 0000  pr__N).r....r...
+00000c10: 0072 0e00 0000 7205 0000 00da 0c73 7461  .r....r......sta
+00000c20: 7469 636d 6574 686f 6472 1c00 0000 7218  ticmethodr....r.
+00000c30: 0000 00da 0369 6e74 7214 0000 0072 3700  .....intr....r7.
+00000c40: 0000 7238 0000 0072 3900 0000 723d 0000  ..r8...r9...r=..
+00000c50: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000c60: 720b 0000 0072 1000 0000 0b00 0000 7312  r....r........s.
+00000c70: 0000 0008 0108 0802 0110 0302 0112 0b0e  ................
+00000c80: 230e 2508 0372 1000 0000 2906 da08 4173  #.%..r....)...As
+00000c90: 6843 7279 7074 7202 0000 0072 2b00 0000  hCryptr....r+...
+00000ca0: 7234 0000 0072 0300 0000 7210 0000 0072  r4...r....r....r
+00000cb0: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000cc0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000cd0: 0073 0600 0000 0c01 0803 1006            .s..........
```

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Jul  1 02:35:10 2023 UTC, .py size: 1852 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 de90 9f64 3c07 0000  a..........d<...
+00000000: 610d 0d0a 0000 0000 f8db ad64 0707 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 8303 5a05 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
 00000060: 8302 5a06 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0555 6e69 6f6e 2901 da03 4173 6863  ...Union)...Ashc
@@ -10,15 +10,15 @@
 00000090: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
 000000a0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
 000000b0: 0387 0004 005a 0453 0029 03da 084b 6579  .....Z.S.)...Key
 000000c0: 4572 726f 7263 0100 0000 0000 0000 0000  Errorc..........
 000000d0: 0000 0100 0000 0300 0000 0300 0000 7318  ..............s.
 000000e0: 0000 0064 017c 005f 0074 0183 00a0 027c  ...d.|._.t.....|
 000000f0: 006a 00a1 0101 0064 0053 0029 024e 7a1a  .j.....d.S.).Nz.
-00000100: 4b65 7920 6d75 7374 2062 6520 3531 3220  Key must be 512 
+00000100: 4b65 7920 6d75 7374 2062 6520 3235 3620  Key must be 256 
 00000110: 4269 7420 6c6f 6e67 2021 2903 da07 6469  Bit long !)...di
 00000120: 7370 6c61 79da 0573 7570 6572 da08 5f5f  splay..super..__
 00000130: 696e 6974 5f5f a901 da04 7365 6c66 a901  init__....self..
 00000140: da09 5f5f 636c 6173 735f 5fa9 00fa 3043  ..__class__...0C
 00000150: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
 00000160: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
 00000170: 7074 5c54 6578 7443 7279 7074 2e70 7972  pt\TextCrypt.pyr
@@ -45,107 +45,108 @@
 000002c0: 0000 0300 0000 4300 0000 7326 0000 007c  ......C...s&...|
 000002d0: 017c 005f 007c 00a0 017c 02a1 0164 016b  .|._.|...|...d.k
 000002e0: 0272 1c7c 027c 005f 026e 0674 0383 0082  .r.|.|._.n.t....
 000002f0: 0164 0053 0029 024e e901 0000 0029 0472  .d.S.).N.....).r
 00000300: 1400 0000 da09 6b65 7976 6572 6966 7972  ......keyverifyr
 00000310: 1500 0000 7204 0000 0029 0372 0900 0000  ....r....).r....
 00000320: 7214 0000 0072 1500 0000 720c 0000 0072  r....r....r....r
-00000330: 0c00 0000 720d 0000 0072 0700 0000 0b00  ....r....r......
+00000330: 0c00 0000 720d 0000 0072 0700 0000 0c00  ....r....r......
 00000340: 0000 7308 0000 0000 0106 010e 0108 027a  ..s............z
 00000350: 0e43 7279 7074 2e5f 5f69 6e69 745f 5f29  .Crypt.__init__)
 00000360: 01da 0672 6574 7572 6e63 0000 0000 0000  ...returnc......
 00000370: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
 00000380: 0000 730a 0000 0074 006a 01a0 02a1 0053  ..s....t.j.....S
 00000390: 0029 014e 2903 7203 0000 00da 0345 6e63  .).N).r......Enc
 000003a0: da0a 6765 6e4d 6169 6e6b 6579 720c 0000  ..genMainkeyr...
 000003b0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000003c0: da06 6765 6e6b 6579 1200 0000 7302 0000  ..genkey....s...
+000003c0: da06 6765 6e6b 6579 1300 0000 7302 0000  ..genkey....s...
 000003d0: 0000 027a 0c43 7279 7074 2e67 656e 6b65  ...z.Crypt.genke
 000003e0: 7929 0272 1500 0000 7218 0000 0063 0100  y).r....r....c..
 000003f0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
 00000400: 0000 4300 0000 734e 0000 0074 007c 0074  ..C...sN...t.|.t
 00000410: 0183 0272 467a 2474 02a0 037c 00a0 04a1  ...rFz$t...|....
 00000420: 00a1 017d 0174 057c 0183 0164 016b 0272  ...}.t.|...d.k.r
 00000430: 2c57 0064 0253 0057 0071 4a04 0074 0679  ,W.d.S.W.qJ..t.y
 00000440: 4201 0001 0001 0059 0064 0353 0030 006e  B......Y.d.S.0.n
-00000450: 0464 0453 0064 0053 0029 054e e940 0000  .d.S.d.S.).N.@..
+00000450: 0464 0453 0064 0053 0029 054e e920 0000  .d.S.d.S.).N. ..
 00000460: 0072 1600 0000 7201 0000 00e9 0200 0000  .r....r.........
 00000470: 2907 da0a 6973 696e 7374 616e 6365 da03  )...isinstance..
 00000480: 7374 72da 0562 7974 6573 da07 6672 6f6d  str..bytes..from
 00000490: 6865 78da 0573 7472 6970 da03 6c65 6eda  hex..strip..len.
 000004a0: 0945 7863 6570 7469 6f6e 2902 7215 0000  .Exception).r...
 000004b0: 00da 0161 720c 0000 0072 0c00 0000 720d  ...ar....r....r.
-000004c0: 0000 0072 1700 0000 1600 0000 7310 0000  ...r........s...
+000004c0: 0000 0072 1700 0000 1700 0000 7310 0000  ...r........s...
 000004d0: 0000 020a 0102 010e 010c 010a 010c 010a  ................
 000004e0: 037a 0f43 7279 7074 2e6b 6579 7665 7269  .z.Crypt.keyveri
 000004f0: 6679 6301 0000 0000 0000 0000 0000 0004  fyc.............
-00000500: 0000 0006 0000 0043 0000 0073 4c00 0000  .......C...sL...
-00000510: 7c00 6a00 7244 7a22 7401 a002 7c00 6a00  |.j.rDz"t...|.j.
+00000500: 0000 0008 0000 0043 0000 0073 5200 0000  .......C...sR...
+00000510: 7c00 6a00 724a 7a22 7401 a002 7c00 6a00  |.j.rJz"t...|.j.
 00000520: 7c00 6a03 a102 7d01 7c01 a004 a100 7d02  |.j...}.|.....}.
-00000530: 6401 7c02 6602 5700 5300 0100 0100 0100  d.|.f.W.S.......
-00000540: 6402 7d03 6403 7c03 6602 0600 5900 5300  d.}.d.|.f...Y.S.
-00000550: 3000 6e04 6404 5300 6400 5300 2905 4e72  0.n.d.S.d.S.).Nr
-00000560: 1600 0000 da01 4572 0100 0000 a902 e700  ......Er........
-00000570: 0000 0000 0000 0072 2800 0000 2905 7214  .......r(...).r.
-00000580: 0000 0072 0300 0000 7219 0000 0072 1500  ...r....r....r..
-00000590: 0000 da08 656e 6354 6f53 7472 2904 7209  ....encToStr).r.
-000005a0: 0000 00da 0369 6e73 da0b 6e65 775f 636f  .....ins..new_co
-000005b0: 6e74 656e 74da 066f 7574 7075 7472 0c00  ntent..outputr..
-000005c0: 0000 720c 0000 0072 0d00 0000 da07 656e  ..r....r......en
-000005d0: 6372 7970 7423 0000 0073 1200 0000 0001  crypt#...s......
-000005e0: 0601 0201 1001 0801 0a01 0601 0401 1002  ................
-000005f0: 7a0d 4372 7970 742e 656e 6372 7970 7463  z.Crypt.encryptc
-00000600: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00000610: 0800 0000 4300 0000 735a 0000 007c 006a  ....C...sZ...|.j
-00000620: 0072 527a 2874 016a 027c 006a 007c 006a  .rRz(t.j.|.j.|.j
-00000630: 0364 018d 027d 017c 01a0 04a1 007d 027c  .d...}.|.....}.|
-00000640: 027d 0364 027c 0366 0257 0053 0004 0074  .}.d.|.f.W.S...t
-00000650: 0579 4e01 0001 0001 007c 006a 007d 0364  .yN......|.j.}.d
-00000660: 037c 0366 0206 0059 0053 0030 006e 0464  .|.f...Y.S.0.n.d
-00000670: 0453 0064 0053 0029 054e 2902 da07 6d65  .S.d.S.).N)...me
-00000680: 7373 6167 65da 076d 6169 6e6b 6579 7216  ssage..mainkeyr.
-00000690: 0000 0072 0100 0000 7227 0000 0029 0672  ...r....r'...).r
-000006a0: 1400 0000 7203 0000 00da 0344 6563 7215  ....r......Decr.
-000006b0: 0000 00da 0864 6563 546f 5374 7272 2400  .....decToStrr$.
-000006c0: 0000 2904 7209 0000 005a 0c64 6563 5f69  ..).r....Z.dec_i
-000006d0: 6e73 7461 6e63 6572 2500 0000 722c 0000  nstancer%...r,..
-000006e0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000006f0: da07 6465 6372 7970 742f 0000 0073 1400  ..decrypt/...s..
-00000700: 0000 0001 0601 0201 1201 0801 0401 0a01  ................
-00000710: 0c01 0601 1002 7a0d 4372 7970 742e 6465  ......z.Crypt.de
-00000720: 6372 7970 7463 0100 0000 0000 0000 0000  cryptc..........
-00000730: 0000 0100 0000 0500 0000 4300 0000 731e  ..........C...s.
-00000740: 0000 0064 017c 006a 0064 0064 0285 0219  ...d.|.j.d.d....
-00000750: 009b 0064 037c 006a 019b 0064 049d 0553  ...d.|.j...d...S
-00000760: 0029 054e 7a1b 456e 6372 7970 7469 6e67  .).Nz.Encrypting
-00000770: 2f44 6563 7279 7074 696e 6720 5465 7874  /Decrypting Text
-00000780: 20e9 0800 0000 7a08 2e2e 2057 6974 6820   .....z... With 
-00000790: 7a05 204b 6579 2072 1300 0000 7208 0000  z. Key r....r...
-000007a0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000007b0: da07 5f5f 7374 725f 5f3c 0000 0073 0200  ..__str__<...s..
-000007c0: 0000 0001 7a0d 4372 7970 742e 5f5f 7374  ....z.Crypt.__st
-000007d0: 725f 5f63 0100 0000 0000 0000 0000 0000  r__c............
-000007e0: 0100 0000 0600 0000 4300 0000 7326 0000  ........C...s&..
-000007f0: 007c 006a 006a 019b 0064 017c 006a 0264  .|.j.j...d.|.j.d
-00000800: 0064 0285 0219 009b 0064 037c 006a 039b  .d.......d.|.j..
-00000810: 0064 049d 0653 0029 054e fa01 2872 3300  .d...S.).N..(r3.
-00000820: 0000 fa01 2cfa 0129 2904 720b 0000 0072  ....,..)).r....r
-00000830: 0e00 0000 7214 0000 0072 1500 0000 7208  ....r....r....r.
-00000840: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000850: 0000 da08 5f5f 7265 7072 5f5f 3e00 0000  ....__repr__>...
-00000860: 7302 0000 0000 017a 0e43 7279 7074 2e5f  s......z.Crypt._
-00000870: 5f72 6570 725f 5f4e 2910 720e 0000 0072  _repr__N).r....r
-00000880: 0f00 0000 7210 0000 0072 0200 0000 721f  ....r....r....r.
-00000890: 0000 0072 2000 0000 7207 0000 00da 0c73  ...r ...r......s
-000008a0: 7461 7469 636d 6574 686f 6472 1b00 0000  taticmethodr....
-000008b0: da03 696e 7472 1700 0000 da05 7475 706c  ..intr......tupl
-000008c0: 6572 2d00 0000 7232 0000 0072 3400 0000  er-...r2...r4...
-000008d0: 7238 0000 0072 0c00 0000 720c 0000 0072  r8...r....r....r
-000008e0: 0c00 0000 720d 0000 0072 1200 0000 0a00  ....r....r......
-000008f0: 0000 7312 0000 0008 0118 0702 0110 0302  ..s.............
-00000900: 0112 0c0e 0c0e 0d08 0272 1200 0000 4e29  .........r....N)
-00000910: 07da 0674 7970 696e 6772 0200 0000 da08  ...typingr......
-00000920: 4173 6843 7279 7074 7203 0000 0072 2400  AshCryptr....r$.
-00000930: 0000 7204 0000 0072 1200 0000 720c 0000  ..r....r....r...
-00000940: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000950: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
-00000960: 0000 000c 010c 0310 05                   .........
+00000530: 6401 7c02 6602 5700 5300 0400 7405 7946  d.|.f.W.S...t.yF
+00000540: 0100 0100 0100 6402 7d03 6403 7c03 6602  ......d.}.d.|.f.
+00000550: 0600 5900 5300 3000 6e04 6404 5300 6400  ..Y.S.0.n.d.S.d.
+00000560: 5300 2905 4e72 1600 0000 da01 4572 0100  S.).Nr......Er..
+00000570: 0000 a902 e700 0000 0000 0000 0072 2800  .............r(.
+00000580: 0000 2906 7214 0000 0072 0300 0000 7219  ..).r....r....r.
+00000590: 0000 0072 1500 0000 da08 656e 6354 6f53  ...r......encToS
+000005a0: 7472 da0d 4261 7365 4578 6365 7074 696f  tr..BaseExceptio
+000005b0: 6e29 0472 0900 0000 da03 696e 73da 0b6e  n).r......ins..n
+000005c0: 6577 5f63 6f6e 7465 6e74 da06 6f75 7470  ew_content..outp
+000005d0: 7574 720c 0000 0072 0c00 0000 720d 0000  utr....r....r...
+000005e0: 00da 0765 6e63 7279 7074 2400 0000 7312  ...encrypt$...s.
+000005f0: 0000 0000 0106 0102 0110 0108 010a 010c  ................
+00000600: 0104 0110 027a 0d43 7279 7074 2e65 6e63  .....z.Crypt.enc
+00000610: 7279 7074 6301 0000 0000 0000 0000 0000  ryptc...........
+00000620: 0004 0000 0008 0000 0043 0000 0073 5a00  .........C...sZ.
+00000630: 0000 7c00 6a00 7252 7a28 7401 6a02 7c00  ..|.j.rRz(t.j.|.
+00000640: 6a00 7c00 6a03 6401 8d02 7d01 7c01 a004  j.|.j.d...}.|...
+00000650: a100 7d02 7c02 7d03 6402 7c03 6602 5700  ..}.|.}.d.|.f.W.
+00000660: 5300 0400 7405 794e 0100 0100 0100 7c00  S...t.yN......|.
+00000670: 6a00 7d03 6403 7c03 6602 0600 5900 5300  j.}.d.|.f...Y.S.
+00000680: 3000 6e04 6404 5300 6400 5300 2905 4e29  0.n.d.S.d.S.).N)
+00000690: 02da 076d 6573 7361 6765 da07 6d61 696e  ...message..main
+000006a0: 6b65 7972 1600 0000 7201 0000 0072 2700  keyr....r....r'.
+000006b0: 0000 2906 7214 0000 0072 0300 0000 da03  ..).r....r......
+000006c0: 4465 6372 1500 0000 da08 6465 6354 6f53  Decr......decToS
+000006d0: 7472 7224 0000 0029 0472 0900 0000 5a0c  trr$...).r....Z.
+000006e0: 6465 635f 696e 7374 616e 6365 7225 0000  dec_instancer%..
+000006f0: 0072 2d00 0000 720c 0000 0072 0c00 0000  .r-...r....r....
+00000700: 720d 0000 00da 0764 6563 7279 7074 3000  r......decrypt0.
+00000710: 0000 7314 0000 0000 0106 0102 0112 0108  ..s.............
+00000720: 0104 010a 010c 0106 0110 027a 0d43 7279  ...........z.Cry
+00000730: 7074 2e64 6563 7279 7074 6301 0000 0000  pt.decryptc.....
+00000740: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00000750: 0000 0073 1e00 0000 6401 7c00 6a00 6400  ...s....d.|.j.d.
+00000760: 6402 8502 1900 9b00 6403 7c00 6a01 9b00  d.......d.|.j...
+00000770: 6404 9d05 5300 2905 4e7a 1b45 6e63 7279  d...S.).Nz.Encry
+00000780: 7074 696e 672f 4465 6372 7970 7469 6e67  pting/Decrypting
+00000790: 2054 6578 7420 e908 0000 007a 082e 2e20   Text .....z... 
+000007a0: 5769 7468 207a 0520 4b65 7920 7213 0000  With z. Key r...
+000007b0: 0072 0800 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000007c0: 720d 0000 00da 075f 5f73 7472 5f5f 3d00  r......__str__=.
+000007d0: 0000 7302 0000 0000 017a 0d43 7279 7074  ..s......z.Crypt
+000007e0: 2e5f 5f73 7472 5f5f 6301 0000 0000 0000  .__str__c.......
+000007f0: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
+00000800: 0073 2600 0000 7c00 6a00 6a01 9b00 6401  .s&...|.j.j...d.
+00000810: 7c00 6a02 6400 6402 8502 1900 9b00 6403  |.j.d.d.......d.
+00000820: 7c00 6a03 9b00 6404 9d06 5300 2905 4efa  |.j...d...S.).N.
+00000830: 0128 7234 0000 00fa 012c fa01 2929 0472  .(r4.....,..)).r
+00000840: 0b00 0000 720e 0000 0072 1400 0000 7215  ....r....r....r.
+00000850: 0000 0072 0800 0000 720c 0000 0072 0c00  ...r....r....r..
+00000860: 0000 720d 0000 00da 085f 5f72 6570 725f  ..r......__repr_
+00000870: 5f40 0000 0073 0200 0000 0001 7a0e 4372  _@...s......z.Cr
+00000880: 7970 742e 5f5f 7265 7072 5f5f 4e29 1072  ypt.__repr__N).r
+00000890: 0e00 0000 720f 0000 0072 1000 0000 7202  ....r....r....r.
+000008a0: 0000 0072 1f00 0000 7220 0000 0072 0700  ...r....r ...r..
+000008b0: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+000008c0: 721b 0000 00da 0369 6e74 7217 0000 00da  r......intr.....
+000008d0: 0574 7570 6c65 722e 0000 0072 3300 0000  .tupler....r3...
+000008e0: 7235 0000 0072 3900 0000 720c 0000 0072  r5...r9...r....r
+000008f0: 0c00 0000 720c 0000 0072 0d00 0000 7212  ....r....r....r.
+00000900: 0000 000b 0000 0073 1200 0000 0801 1807  .......s........
+00000910: 0201 1003 0201 120c 0e0c 0e0d 0803 7212  ..............r.
+00000920: 0000 004e 2907 da06 7479 7069 6e67 7202  ...N)...typingr.
+00000930: 0000 00da 0841 7368 4372 7970 7472 0300  .....AshCryptr..
+00000940: 0000 7224 0000 0072 0400 0000 7212 0000  ..r$...r....r...
+00000950: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000960: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000970: 0000 0073 0600 0000 0c01 0c03 1006       ...s..........
```

### Comparing `AshCrypt-1.3.5/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jul  7 12:45:35 2023 UTC, .py size: 536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-00000000: 610d 0d0a 0000 0000 ef08 a864 1802 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 af34 ab64 1802 0000  a........4.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6503 6502 6504 6505 6602 1900 6403  ..e.e.e.e.f...d.
-00000050: 9c02 6404 6405 8404 5a06 6507 6406 6b02  ..d.d...Z.e.d.k.
-00000060: 723c 6506 6407 8301 0100 6401 5300 2908  r<e.d.....d.S.).
-00000070: e900 0000 004e 2901 da05 556e 696f 6e29  .....N)...Union)
-00000080: 02da 0474 6578 74da 0672 6574 7572 6e63  ...text..returnc
-00000090: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-000000a0: 0a00 0000 4300 0000 738c 0000 007a 5a7c  ....C...s....zZ|
-000000b0: 00a0 00a1 007d 0174 016a 0264 0174 016a  .....}.t.j.d.t.j
-000000c0: 036a 0464 0264 0364 048d 047d 027c 02a0  .j.d.d.d...}.|..
-000000d0: 057c 01a1 0101 007c 026a 0664 0564 068d  .|.....|.j.d.d..
-000000e0: 0101 007c 026a 0764 0764 0864 098d 027d  ...|.j.d.d.d...}
-000000f0: 037c 03a0 0864 0aa1 0101 007c 03a0 09a1  .|...d.....|....
-00000100: 0001 0057 0064 0353 0004 0074 0a79 8601  ...W.d.S...t.y..
-00000110: 007d 0401 007a 1464 0b7c 0466 0257 0006  .}...z.d.|.f.W..
-00000120: 0059 0064 007d 047e 0453 0064 007d 047e  .Y.d.}.~.S.d.}.~
-00000130: 0430 0030 0064 0053 0029 0c4e e90a 0000  .0.0.d.S.).N....
-00000140: 00e9 1400 0000 e901 0000 0029 04da 0776  ...........)...v
-00000150: 6572 7369 6f6e 5a10 6572 726f 725f 636f  ersionZ.error_co
-00000160: 7272 6563 7469 6f6e 5a08 626f 785f 7369  rrectionZ.box_si
-00000170: 7a65 da06 626f 7264 6572 5429 015a 0366  ze..borderT).Z.f
-00000180: 6974 da05 626c 6163 6bda 0577 6869 7465  it..black..white
-00000190: 2902 5a0a 6669 6c6c 5f63 6f6c 6f72 5a0a  ).Z.fill_colorZ.
-000001a0: 6261 636b 5f63 6f6c 6f72 7a09 7172 7631  back_colorz.qrv1
-000001b0: 302e 706e 6772 0100 0000 290b da05 7374  0.pngr....)...st
-000001c0: 7269 70da 0671 7263 6f64 655a 0651 5243  rip..qrcodeZ.QRC
-000001d0: 6f64 65da 0963 6f6e 7374 616e 7473 5a0f  ode..constantsZ.
-000001e0: 4552 524f 525f 434f 5252 4543 545f 4c5a  ERROR_CORRECT_LZ
-000001f0: 0861 6464 5f64 6174 615a 046d 616b 655a  .add_dataZ.makeZ
-00000200: 0a6d 616b 655f 696d 6167 65da 0473 6176  .make_image..sav
-00000210: 65da 0473 686f 77da 0945 7863 6570 7469  e..show..Excepti
-00000220: 6f6e 2905 7203 0000 00da 0178 da02 7172  on).r......x..qr
-00000230: da03 696d 67da 0165 a900 7216 0000 00fa  ..img..e..r.....
-00000240: 2943 3a5c 576f 726b 5c47 6974 4875 6257  )C:\Work\GitHubW
-00000250: 6f72 6b5c 4145 532d 3235 365c 4173 6843  ork\AES-256\AshC
-00000260: 7279 7074 5c71 722e 7079 da03 7471 7204  rypt\qr.py..tqr.
-00000270: 0000 0073 1600 0000 0001 0201 0801 1601  ...s............
-00000280: 0a01 0c01 0e01 0a01 0801 0602 0e01 7218  ..............r.
-00000290: 0000 00da 085f 5f6d 6169 6e5f 5f7a 0954  .....__main__z.T
-000002a0: 6578 7420 6865 7265 2908 720d 0000 00da  ext here).r.....
-000002b0: 0674 7970 696e 6772 0200 0000 da03 7374  .typingr......st
-000002c0: 72da 0369 6e74 da05 7475 706c 6572 1800  r..int..tupler..
-000002d0: 0000 da08 5f5f 6e61 6d65 5f5f 7216 0000  ....__name__r...
-000002e0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000002f0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-00000300: 0000 0008 010c 0218 0f08 01              ...........
+00000050: 9c02 6404 6405 8404 5a06 6401 5300 2906  ..d.d...Z.d.S.).
+00000060: e900 0000 004e 2901 da05 556e 696f 6e29  .....N)...Union)
+00000070: 02da 0474 6578 74da 0672 6574 7572 6e63  ...text..returnc
+00000080: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00000090: 0a00 0000 4300 0000 738c 0000 007a 5a7c  ....C...s....zZ|
+000000a0: 00a0 00a1 007d 0174 016a 0264 0174 016a  .....}.t.j.d.t.j
+000000b0: 036a 0464 0264 0364 048d 047d 027c 02a0  .j.d.d.d...}.|..
+000000c0: 057c 01a1 0101 007c 026a 0664 0564 068d  .|.....|.j.d.d..
+000000d0: 0101 007c 026a 0764 0764 0864 098d 027d  ...|.j.d.d.d...}
+000000e0: 037c 03a0 0864 0aa1 0101 007c 03a0 09a1  .|...d.....|....
+000000f0: 0001 0057 0064 0353 0004 0074 0a79 8601  ...W.d.S...t.y..
+00000100: 007d 0401 007a 1464 0b7c 0466 0257 0006  .}...z.d.|.f.W..
+00000110: 0059 0064 007d 047e 0453 0064 007d 047e  .Y.d.}.~.S.d.}.~
+00000120: 0430 0030 0064 0053 0029 0c4e e90a 0000  .0.0.d.S.).N....
+00000130: 00e9 1400 0000 e901 0000 0029 04da 0776  ...........)...v
+00000140: 6572 7369 6f6e 5a10 6572 726f 725f 636f  ersionZ.error_co
+00000150: 7272 6563 7469 6f6e 5a08 626f 785f 7369  rrectionZ.box_si
+00000160: 7a65 da06 626f 7264 6572 5429 015a 0366  ze..borderT).Z.f
+00000170: 6974 da05 626c 6163 6bda 0577 6869 7465  it..black..white
+00000180: 2902 5a0a 6669 6c6c 5f63 6f6c 6f72 5a0a  ).Z.fill_colorZ.
+00000190: 6261 636b 5f63 6f6c 6f72 7a09 7172 7631  back_colorz.qrv1
+000001a0: 302e 706e 6772 0100 0000 290b da05 7374  0.pngr....)...st
+000001b0: 7269 70da 0671 7263 6f64 655a 0651 5243  rip..qrcodeZ.QRC
+000001c0: 6f64 65da 0963 6f6e 7374 616e 7473 5a0f  ode..constantsZ.
+000001d0: 4552 524f 525f 434f 5252 4543 545f 4c5a  ERROR_CORRECT_LZ
+000001e0: 0861 6464 5f64 6174 615a 046d 616b 655a  .add_dataZ.makeZ
+000001f0: 0a6d 616b 655f 696d 6167 65da 0473 6176  .make_image..sav
+00000200: 65da 0473 686f 77da 0945 7863 6570 7469  e..show..Excepti
+00000210: 6f6e 2905 7203 0000 00da 0178 da02 7172  on).r......x..qr
+00000220: da03 696d 67da 0165 a900 7216 0000 00fa  ..img..e..r.....
+00000230: 2943 3a5c 576f 726b 5c47 6974 4875 6257  )C:\Work\GitHubW
+00000240: 6f72 6b5c 4145 532d 3235 365c 4173 6843  ork\AES-256\AshC
+00000250: 7279 7074 5c71 722e 7079 da03 7471 7205  rypt\qr.py..tqr.
+00000260: 0000 0073 2000 0000 0001 0201 0801 0401  ...s ...........
+00000270: 0201 0601 0201 02fc 0605 0a01 0c01 0e01  ................
+00000280: 0a01 0801 0602 0e01 7218 0000 0029 0772  ........r....).r
+00000290: 0d00 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
+000002a0: 00da 0373 7472 da03 696e 74da 0574 7570  ...str..int..tup
+000002b0: 6c65 7218 0000 0072 1600 0000 7216 0000  ler....r....r...
+000002c0: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+000002d0: 6475 6c65 3e01 0000 0073 0400 0000 0801  dule>....s......
+000002e0: 0c03                                     ..
```

### Comparing `AshCrypt-1.3.5/AshCrypt/qr.py` & `AshCrypt-1.3.6/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.5/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Jul  3 12:24:38 2023 UTC, .py size: 3401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 06be a264 490d 0000  a..........dI...
+00000000: 610d 0d0a 0000 0000 c5da ad64 140d 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 6d03 5a03 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000050: 8400 6403 6500 6a04 8303 5a05 6506 6404  ..d.e.j...Z.e.d.
 00000060: 6b02 723e 6500 a007 a100 0100 6401 5300  k.r>e.......d.S.
 00000070: 2905 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
@@ -28,335 +28,331 @@
 000001b0: 0064 027c 005f 0164 037c 005f 0274 036a  .d.|._.d.|._.t.j
 000001c0: 047c 006a 007c 006a 0264 048d 027c 005f  .|.j.|.j.d...|._
 000001d0: 057c 006a 05a0 06a1 007c 005f 077c 006a  .|.j.....|._.|.j
 000001e0: 05a0 08a1 007c 005f 0974 036a 0a7c 006a  .....|._.t.j.|.j
 000001f0: 097c 006a 0264 048d 027c 005f 0b64 0053  .|.j.d...|._.d.S
 00000200: 0029 054e 7a1f 4865 6c6c 6f20 7468 6572  .).Nz.Hello ther
 00000210: 6520 7465 7374 696e 6720 6966 2069 7420  e testing if it 
-00000220: 776f 726b 7373 1700 0000 4865 6c6c 6f20  workss....Hello 
-00000230: 7468 6973 2069 7320 6279 7465 7320 6e6f  this is bytes no
-00000240: 775a 8063 3330 3636 6534 3634 3335 3065  wZ.c3066e464350e
-00000250: 3638 6131 3434 6436 6265 3365 3335 6338  68a144d6be3e35c8
-00000260: 3739 6561 6331 6239 6633 3630 3133 3934  79eac1b9f3601394
-00000270: 3433 6565 3364 3965 3139 3630 3732 3564  43ee3d9e1960725d
-00000280: 3661 3464 3333 3739 6166 3061 3335 6236  6a4d3379af0a35b6
-00000290: 6130 3764 3038 3365 6363 3239 6334 6261  a07d083ecc29c4ba
-000002a0: 3033 3736 3761 6436 6434 3862 3865 3963  03767ad6d48b8e9c
-000002b0: 3230 6433 3139 6464 3435 3964 6135 3261  20d319dd459da52a
-000002c0: 3931 61a9 02da 076d 6573 7361 6765 da07  91a....message..
-000002d0: 6d61 696e 6b65 7929 0c5a 086d 6573 7361  mainkey).Z.messa
-000002e0: 6765 315a 086d 6573 7361 6765 3272 0600  ge1Z.message2r..
-000002f0: 0000 da03 4173 68da 0345 6e63 da04 696e  ....Ash..Enc..in
-00000300: 7331 da08 656e 6354 6f53 7472 5a0e 7374  s1..encToStrZ.st
-00000310: 7269 6e67 5f6d 6573 7361 6765 da0a 656e  ring_message..en
-00000320: 6354 6f42 7974 6573 da0d 6279 7465 735f  cToBytes..bytes_
-00000330: 6d65 7373 6167 65da 0344 6563 da04 696e  message..Dec..in
-00000340: 7332 a901 da04 7365 6c66 a900 7211 0000  s2....self..r...
-00000350: 00fa 3c43 3a5c 576f 726b 5c47 6974 4875  ..<C:\Work\GitHu
-00000360: 6257 6f72 6b5c 4145 532d 3235 365c 4173  bWork\AES-256\As
-00000370: 6843 7279 7074 5c75 6e69 7474 6573 7473  hCrypt\unittests
-00000380: 5c75 6e69 7474 6573 7441 7368 2e70 79da  \unittestAsh.py.
-00000390: 0573 6574 5570 0600 0000 730e 0000 0000  .setUp....s.....
-000003a0: 0106 0106 0106 0114 010c 010c 017a 1641  .............z.A
-000003b0: 7368 4d6f 6475 6c65 5465 7374 696e 672e  shModuleTesting.
-000003c0: 7365 7455 7063 0100 0000 0000 0000 0000  setUpc..........
-000003d0: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-000003e0: 0000 0064 0053 00a9 014e 7211 0000 0072  ...d.S...Nr....r
-000003f0: 0f00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000400: 0000 00da 0874 6561 7244 6f77 6e0f 0000  .....tearDown...
-00000410: 0073 0200 0000 0001 7a19 4173 684d 6f64  .s......z.AshMod
-00000420: 756c 6554 6573 7469 6e67 2e74 6561 7244  uleTesting.tearD
-00000430: 6f77 6e63 0100 0000 0000 0000 0000 0000  ownc............
-00000440: 0100 0000 0700 0000 4300 0000 7320 0000  ........C...s ..
-00000450: 007c 00a0 0064 0174 01a0 0274 036a 04a0  .|...d.t...t.j..
-00000460: 05a1 00a1 01a0 06a1 00a1 0201 0064 0053  .............d.S
-00000470: 00a9 024e e940 0000 0029 07da 0b61 7373  ...N.@...)...ass
-00000480: 6572 7445 7175 616c da05 6279 7465 73da  ertEqual..bytes.
-00000490: 0766 726f 6d68 6578 7207 0000 0072 0800  .fromhexr....r..
-000004a0: 0000 da0a 6765 6e4d 6169 6e6b 6579 da07  ....genMainkey..
-000004b0: 5f5f 6c65 6e5f 5f72 0f00 0000 7211 0000  __len__r....r...
-000004c0: 0072 1100 0000 7212 0000 00da 0e74 6573  .r....r......tes
-000004d0: 745f 4b65 794c 656e 6774 6812 0000 0073  t_KeyLength....s
-000004e0: 0200 0000 0001 7a1f 4173 684d 6f64 756c  ......z.AshModul
-000004f0: 6554 6573 7469 6e67 2e74 6573 745f 4b65  eTesting.test_Ke
-00000500: 794c 656e 6774 6863 0100 0000 0000 0000  yLengthc........
-00000510: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-00000520: 731a 0000 007c 00a0 0074 0174 0274 036a  s....|...t.t.t.j
-00000530: 04a0 05a1 0083 01a1 0201 0064 0053 0072  ...........d.S.r
-00000540: 1400 0000 2906 da08 6173 7365 7274 4973  ....)...assertIs
-00000550: da03 7374 72da 0474 7970 6572 0700 0000  ..str..typer....
-00000560: 7208 0000 0072 1b00 0000 720f 0000 0072  r....r....r....r
-00000570: 1100 0000 7211 0000 0072 1200 0000 da0c  ....r....r......
-00000580: 7465 7374 5f4b 6579 5479 7065 1500 0000  test_KeyType....
-00000590: 7302 0000 0000 017a 1d41 7368 4d6f 6475  s......z.AshModu
-000005a0: 6c65 5465 7374 696e 672e 7465 7374 5f4b  leTesting.test_K
-000005b0: 6579 5479 7065 6301 0000 0000 0000 0000  eyTypec.........
-000005c0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-000005d0: 2200 0000 7c00 a000 7c00 6a01 6400 6401  "...|...|.j.d.d.
-000005e0: 8502 1900 7c00 6a02 a003 a100 6b02 a101  ....|.j.....k...
-000005f0: 0100 6400 5300 7216 0000 0029 04da 0a61  ..d.S.r....)...a
-00000600: 7373 6572 7454 7275 6572 0c00 0000 7209  ssertTruer....r.
-00000610: 0000 00da 0448 4d41 4372 0f00 0000 7211  .....HMACr....r.
-00000620: 0000 0072 1100 0000 7212 0000 00da 0974  ...r....r......t
-00000630: 6573 745f 484d 4143 1800 0000 7302 0000  est_HMAC....s...
-00000640: 0000 017a 1a41 7368 4d6f 6475 6c65 5465  ...z.AshModuleTe
-00000650: 7374 696e 672e 7465 7374 5f48 4d41 4363  sting.test_HMACc
-00000660: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000670: 0500 0000 4300 0000 7320 0000 007c 00a0  ....C...s ...|..
-00000680: 007c 006a 0164 0164 0285 0219 007c 006a  .|.j.d.d.....|.j
-00000690: 026a 036b 02a1 0101 0064 0053 0029 034e  .j.k.....d.S.).N
-000006a0: 7217 0000 00e9 5000 0000 2904 7222 0000  r.....P...).r"..
-000006b0: 0072 0c00 0000 7209 0000 00da 0269 7672  .r....r......ivr
-000006c0: 0f00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-000006d0: 0000 00da 0774 6573 745f 4956 1b00 0000  .....test_IV....
-000006e0: 7302 0000 0000 017a 1841 7368 4d6f 6475  s......z.AshModu
-000006f0: 6c65 5465 7374 696e 672e 7465 7374 5f49  leTesting.test_I
-00000700: 5663 0100 0000 0000 0000 0000 0000 0100  Vc..............
-00000710: 0000 0500 0000 4300 0000 7320 0000 007c  ......C...s ...|
-00000720: 00a0 007c 006a 0164 0164 0285 0219 007c  ...|.j.d.d.....|
-00000730: 006a 026a 036b 02a1 0101 0064 0053 0029  .j.j.k.....d.S.)
-00000740: 034e 7225 0000 00e9 6000 0000 2904 7222  .Nr%....`...).r"
-00000750: 0000 0072 0c00 0000 7209 0000 00da 0473  ...r....r......s
-00000760: 616c 7472 0f00 0000 7211 0000 0072 1100  altr....r....r..
-00000770: 0000 7212 0000 00da 0974 6573 745f 5361  ..r......test_Sa
-00000780: 6c74 1e00 0000 7302 0000 0000 017a 1a41  lt....s......z.A
-00000790: 7368 4d6f 6475 6c65 5465 7374 696e 672e  shModuleTesting.
-000007a0: 7465 7374 5f53 616c 7463 0100 0000 0000  test_Saltc......
-000007b0: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
-000007c0: 0000 7320 0000 007c 00a0 007c 006a 0164  ..s ...|...|.j.d
-000007d0: 0164 0285 0219 007c 006a 026a 036b 02a1  .d.....|.j.j.k..
-000007e0: 0101 0064 0053 0029 034e 7228 0000 00e9  ...d.S.).Nr(....
-000007f0: 7000 0000 2904 7222 0000 0072 0c00 0000  p...).r"...r....
-00000800: 7209 0000 00da 0670 6570 7065 7272 0f00  r......pepperr..
-00000810: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000820: 00da 0b74 6573 745f 5065 7070 6572 2100  ...test_Pepper!.
-00000830: 0000 7302 0000 0000 017a 1c41 7368 4d6f  ..s......z.AshMo
-00000840: 6475 6c65 5465 7374 696e 672e 7465 7374  duleTesting.test
-00000850: 5f50 6570 7065 7263 0100 0000 0000 0000  _Pepperc........
-00000860: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00000870: 7322 0000 007c 00a0 007c 006a 0164 0164  s"...|...|.j.d.d
-00000880: 0285 0219 007c 006a 02a0 03a1 006b 02a1  .....|.j.....k..
-00000890: 0101 0064 0053 0029 034e 722b 0000 00e9  ...d.S.).Nr+....
-000008a0: 7400 0000 2904 7222 0000 0072 0c00 0000  t...).r"...r....
-000008b0: 7209 0000 00da 0f73 6574 7570 4974 6572  r......setupIter
-000008c0: 6174 696f 6e73 720f 0000 0072 1100 0000  ationsr....r....
-000008d0: 7211 0000 0072 1200 0000 da0f 7465 7374  r....r......test
-000008e0: 5f49 7465 7261 7469 6f6e 7324 0000 0073  _Iterations$...s
-000008f0: 0200 0000 0001 7a20 4173 684d 6f64 756c  ......z AshModul
-00000900: 6554 6573 7469 6e67 2e74 6573 745f 4974  eTesting.test_It
-00000910: 6572 6174 696f 6e73 6301 0000 0000 0000  erationsc.......
-00000920: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00000930: 0073 2200 0000 7c00 a000 7c00 6a01 6401  .s"...|...|.j.d.
-00000940: 6400 8502 1900 7c00 6a02 a003 a100 6b02  d.....|.j.....k.
-00000950: a101 0100 6400 5300 2902 4e72 2e00 0000  ....d.S.).Nr....
-00000960: 2904 7222 0000 0072 0c00 0000 7209 0000  ).r"...r....r...
-00000970: 00da 0a63 6970 6865 7274 6578 7472 0f00  ...ciphertextr..
-00000980: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000990: 00da 0f74 6573 745f 4369 7068 6572 7465  ...test_Cipherte
-000009a0: 7874 2700 0000 7302 0000 0000 017a 2041  xt'...s......z A
-000009b0: 7368 4d6f 6475 6c65 5465 7374 696e 672e  shModuleTesting.
-000009c0: 7465 7374 5f43 6970 6865 7274 6578 7463  test_Ciphertextc
-000009d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000009e0: 0600 0000 4300 0000 731a 0000 007c 00a0  ....C...s....|..
-000009f0: 0074 0174 027c 006a 03a0 04a1 0083 01a1  .t.t.|.j........
-00000a00: 0201 0064 0053 0072 1400 0000 2905 721e  ...d.S.r....).r.
-00000a10: 0000 0072 1900 0000 7220 0000 0072 0900  ...r....r ...r..
-00000a20: 0000 722f 0000 0072 0f00 0000 7211 0000  ..r/...r....r...
-00000a30: 0072 1100 0000 7212 0000 00da 1374 6573  .r....r......tes
-00000a40: 745f 5479 7065 4974 6572 6174 696f 6e73  t_TypeIterations
-00000a50: 2a00 0000 7302 0000 0000 017a 2441 7368  *...s......z$Ash
-00000a60: 4d6f 6475 6c65 5465 7374 696e 672e 7465  ModuleTesting.te
-00000a70: 7374 5f54 7970 6549 7465 7261 7469 6f6e  st_TypeIteration
-00000a80: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00000a90: 0000 0500 0000 4300 0000 731a 0000 007c  ......C...s....|
-00000aa0: 00a0 0064 017c 006a 01a0 02a1 00a0 03a1  ...d.|.j........
-00000ab0: 00a1 0201 0064 0053 0029 024e e904 0000  .....d.S.).N....
-00000ac0: 0029 0472 1800 0000 7209 0000 0072 2f00  .).r....r....r/.
-00000ad0: 0000 721c 0000 0072 0f00 0000 7211 0000  ..r....r....r...
-00000ae0: 0072 1100 0000 7212 0000 00da 1974 6573  .r....r......tes
-00000af0: 745f 4974 6572 6174 696f 6e73 4669 7865  t_IterationsFixe
-00000b00: 645f 7369 7a65 2d00 0000 7302 0000 0000  d_size-...s.....
-00000b10: 017a 2a41 7368 4d6f 6475 6c65 5465 7374  .z*AshModuleTest
-00000b20: 696e 672e 7465 7374 5f49 7465 7261 7469  ing.test_Iterati
-00000b30: 6f6e 7346 6978 6564 5f73 697a 6563 0100  onsFixed_sizec..
-00000b40: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000b50: 0000 4300 0000 731a 0000 007c 00a0 0074  ..C...s....|...t
-00000b60: 0174 027c 006a 03a0 04a1 0083 01a1 0201  .t.|.j..........
-00000b70: 0064 0053 0072 1400 0000 2905 721e 0000  .d.S.r....).r...
-00000b80: 0072 1900 0000 7220 0000 0072 0900 0000  .r....r ...r....
-00000b90: 720b 0000 0072 0f00 0000 7211 0000 0072  r....r....r....r
-00000ba0: 1100 0000 7212 0000 00da 1374 6573 745f  ....r......test_
-00000bb0: 456e 634f 7574 7075 7442 7974 6573 3000  EncOutputBytes0.
-00000bc0: 0000 7302 0000 0000 017a 2441 7368 4d6f  ..s......z$AshMo
-00000bd0: 6475 6c65 5465 7374 696e 672e 7465 7374  duleTesting.test
-00000be0: 5f45 6e63 4f75 7470 7574 4279 7465 7363  _EncOutputBytesc
-00000bf0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000c00: 0600 0000 4300 0000 731a 0000 007c 00a0  ....C...s....|..
-00000c10: 0074 0174 027c 006a 03a0 04a1 0083 01a1  .t.t.|.j........
-00000c20: 0201 0064 0053 0072 1400 0000 2905 721e  ...d.S.r....).r.
-00000c30: 0000 0072 1f00 0000 7220 0000 0072 0900  ...r....r ...r..
-00000c40: 0000 720a 0000 0072 0f00 0000 7211 0000  ..r....r....r...
-00000c50: 0072 1100 0000 7212 0000 00da 1474 6573  .r....r......tes
-00000c60: 745f 456e 634f 7574 7075 7453 7472 696e  t_EncOutputStrin
-00000c70: 6733 0000 0073 0200 0000 0001 7a25 4173  g3...s......z%As
-00000c80: 684d 6f64 756c 6554 6573 7469 6e67 2e74  hModuleTesting.t
-00000c90: 6573 745f 456e 634f 7574 7075 7453 7472  est_EncOutputStr
-00000ca0: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
-00000cb0: 0100 0000 0400 0000 4300 0000 731a 0000  ........C...s...
-00000cc0: 007c 00a0 007c 006a 01a0 02a1 007c 006a  .|...|.j.....|.j
-00000cd0: 036a 04a1 0201 0064 0053 0072 1400 0000  .j.....d.S.r....
-00000ce0: 2905 7218 0000 0072 0900 0000 7223 0000  ).r....r....r#..
-00000cf0: 0072 0e00 0000 5a08 7265 635f 686d 6163  .r....Z.rec_hmac
-00000d00: 720f 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000d10: 1200 0000 da0e 7465 7374 5f48 4d41 435f  ......test_HMAC_
-00000d20: 436f 6d70 3600 0000 7302 0000 0000 017a  Comp6...s......z
-00000d30: 1f41 7368 4d6f 6475 6c65 5465 7374 696e  .AshModuleTestin
-00000d40: 672e 7465 7374 5f48 4d41 435f 436f 6d70  g.test_HMAC_Comp
-00000d50: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000d60: 0004 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00000d70: a000 7c00 6a01 6a02 7c00 6a03 6a04 a102  ..|.j.j.|.j.j...
-00000d80: 0100 6400 5300 7214 0000 0029 0572 1800  ..d.S.r....).r..
-00000d90: 0000 7209 0000 0072 2600 0000 720e 0000  ..r....r&...r...
-00000da0: 005a 0672 6563 5f69 7672 0f00 0000 7211  .Z.rec_ivr....r.
-00000db0: 0000 0072 1100 0000 7212 0000 00da 0c74  ...r....r......t
-00000dc0: 6573 745f 4956 5f43 6f6d 7039 0000 0073  est_IV_Comp9...s
-00000dd0: 0200 0000 0001 7a1d 4173 684d 6f64 756c  ......z.AshModul
-00000de0: 6554 6573 7469 6e67 2e74 6573 745f 4956  eTesting.test_IV
-00000df0: 5f43 6f6d 7063 0100 0000 0000 0000 0000  _Compc..........
-00000e00: 0000 0100 0000 0400 0000 4300 0000 7318  ..........C...s.
-00000e10: 0000 007c 00a0 007c 006a 016a 027c 006a  ...|...|.j.j.|.j
-00000e20: 036a 04a1 0201 0064 0053 0072 1400 0000  .j.....d.S.r....
-00000e30: 2905 7218 0000 0072 0900 0000 7229 0000  ).r....r....r)..
-00000e40: 0072 0e00 0000 5a08 7265 635f 7361 6c74  .r....Z.rec_salt
-00000e50: 720f 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000e60: 1200 0000 da0e 7465 7374 5f53 616c 745f  ......test_Salt_
-00000e70: 436f 6d70 3c00 0000 7302 0000 0000 017a  Comp<...s......z
-00000e80: 1f41 7368 4d6f 6475 6c65 5465 7374 696e  .AshModuleTestin
-00000e90: 672e 7465 7374 5f53 616c 745f 436f 6d70  g.test_Salt_Comp
-00000ea0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000eb0: 0004 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00000ec0: a000 7c00 6a01 6a02 7c00 6a03 6a04 a102  ..|.j.j.|.j.j...
-00000ed0: 0100 6400 5300 7214 0000 0029 0572 1800  ..d.S.r....).r..
-00000ee0: 0000 7209 0000 0072 2c00 0000 720e 0000  ..r....r,...r...
-00000ef0: 005a 0a72 6563 5f70 6570 7065 7272 0f00  .Z.rec_pepperr..
-00000f00: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000f10: 00da 1074 6573 745f 5065 7070 6572 5f43  ...test_Pepper_C
-00000f20: 6f6d 703f 0000 0073 0200 0000 0001 7a21  omp?...s......z!
-00000f30: 4173 684d 6f64 756c 6554 6573 7469 6e67  AshModuleTesting
-00000f40: 2e74 6573 745f 5065 7070 6572 5f43 6f6d  .test_Pepper_Com
-00000f50: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
-00000f60: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
-00000f70: 00a0 007c 006a 016a 027c 006a 036a 04a1  ...|.j.j.|.j.j..
-00000f80: 0201 0064 0053 0072 1400 0000 2905 7218  ...d.S.r....).r.
-00000f90: 0000 0072 0900 0000 5a0a 6974 6572 6174  ...r....Z.iterat
-00000fa0: 696f 6e73 720e 0000 005a 0e72 6563 5f69  ionsr....Z.rec_i
-00000fb0: 7465 7261 7469 6f6e 7372 0f00 0000 7211  terationsr....r.
-00000fc0: 0000 0072 1100 0000 7212 0000 00da 1474  ...r....r......t
-00000fd0: 6573 745f 4974 6572 6174 696f 6e73 5f43  est_Iterations_C
-00000fe0: 6f6d 7042 0000 0073 0200 0000 0001 7a25  ompB...s......z%
-00000ff0: 4173 684d 6f64 756c 6554 6573 7469 6e67  AshModuleTesting
-00001000: 2e74 6573 745f 4974 6572 6174 696f 6e73  .test_Iterations
-00001010: 5f43 6f6d 7063 0100 0000 0000 0000 0000  _Compc..........
-00001020: 0000 0100 0000 0400 0000 4300 0000 731a  ..........C...s.
-00001030: 0000 007c 00a0 007c 006a 01a0 02a1 007c  ...|...|.j.....|
-00001040: 006a 036a 04a1 0201 0064 0053 0072 1400  .j.j.....d.S.r..
-00001050: 0000 2905 7218 0000 0072 0900 0000 7231  ..).r....r....r1
-00001060: 0000 0072 0e00 0000 5a0e 7265 635f 6369  ...r....Z.rec_ci
-00001070: 7068 6572 7465 7874 720f 0000 0072 1100  phertextr....r..
-00001080: 0000 7211 0000 0072 1200 0000 da14 7465  ..r....r......te
-00001090: 7374 5f43 6970 6865 7274 6578 745f 436f  st_Ciphertext_Co
-000010a0: 6d70 4500 0000 7302 0000 0000 017a 2541  mpE...s......z%A
-000010b0: 7368 4d6f 6475 6c65 5465 7374 696e 672e  shModuleTesting.
-000010c0: 7465 7374 5f43 6970 6865 7274 6578 745f  test_Ciphertext_
-000010d0: 436f 6d70 6301 0000 0000 0000 0000 0000  Compc...........
-000010e0: 0003 0000 0008 0000 0043 0000 0073 6c00  .........C...sl.
-000010f0: 0000 7c00 6a00 a001 a100 6400 6401 8502  ..|.j.....d.d...
-00001100: 1900 6402 1700 7d01 7c01 7c00 6a00 a001  ..d...}.|.|.j...
-00001110: a100 6403 6400 8502 1900 1700 7d02 7c00  ..d.d.......}.|.
-00001120: a002 7403 6a04 a101 8f20 0100 7403 6a05  ..t.j.... ..t.j.
-00001130: 7c02 7c00 6a06 6404 8d02 0100 5700 6400  |.|.j.d.....W.d.
-00001140: 0400 0400 8303 0100 6e10 3100 735e 3000  ........n.1.s^0.
-00001150: 0100 0100 0100 5900 0100 6400 5300 2905  ......Y...d.S.).
-00001160: 4ee9 3f00 0000 f301 0000 0031 7217 0000  N.?........1r...
-00001170: 0072 0400 0000 2907 7209 0000 0072 0b00  .r....).r....r..
-00001180: 0000 da0c 6173 7365 7274 5261 6973 6573  ....assertRaises
-00001190: 7207 0000 005a 154d 6573 7361 6765 5461  r....Z.MessageTa
-000011a0: 6d70 6572 696e 6745 7272 6f72 720d 0000  mperingErrorr...
-000011b0: 0072 0600 0000 2903 7210 0000 005a 0d74  .r....).r....Z.t
-000011c0: 616d 7065 7265 645f 484d 4143 da10 7461  ampered_HMAC..ta
-000011d0: 6d70 6572 6564 5f6d 6573 7361 6765 7211  mpered_messager.
-000011e0: 0000 0072 1100 0000 7212 0000 00da 1774  ...r....r......t
-000011f0: 6573 745f 484d 4143 5f4d 6973 6d61 7463  est_HMAC_Mismatc
-00001200: 6845 7272 6f72 4800 0000 7308 0000 0000  hErrorH...s.....
-00001210: 0116 0116 010e 017a 2841 7368 4d6f 6475  .......z(AshModu
-00001220: 6c65 5465 7374 696e 672e 7465 7374 5f48  leTesting.test_H
-00001230: 4d41 435f 4d69 736d 6174 6368 4572 726f  MAC_MismatchErro
-00001240: 7263 0100 0000 0000 0000 0000 0000 0300  rc..............
-00001250: 0000 0800 0000 4300 0000 736e 0000 007c  ......C...sn...|
-00001260: 006a 00a0 01a1 007d 017c 0164 0064 0185  .j.....}.|.d.d..
-00001270: 0219 0074 02a0 0364 0264 03a1 0217 007c  ...t...d.d.....|
-00001280: 0164 0464 0085 0219 0017 007d 027c 00a0  .d.d.......}.|..
-00001290: 0474 056a 06a1 018f 2001 0074 056a 077c  .t.j.... ..t.j.|
-000012a0: 027c 006a 0864 058d 0201 0057 0064 0004  .|.j.d.....W.d..
-000012b0: 0004 0083 0301 006e 1031 0073 6030 0001  .......n.1.s`0..
-000012c0: 0001 0001 0059 0001 0064 0053 0029 064e  .....Y...d.S.).N
-000012d0: 722b 0000 007a 0221 4969 a186 0100 722e  r+...z.!Ii....r.
-000012e0: 0000 0072 0400 0000 2909 7209 0000 0072  ...r....).r....r
-000012f0: 0b00 0000 da06 7374 7275 6374 5a04 7061  ......structZ.pa
-00001300: 636b 7240 0000 0072 0700 0000 5a1a 4974  ckr@...r....Z.It
-00001310: 6572 6174 696f 6e73 4f75 746f 6661 5261  erationsOutofaRa
-00001320: 6e67 6545 7272 6f72 720d 0000 0072 0600  ngeErrorr....r..
-00001330: 0000 2903 7210 0000 005a 0365 6e62 7241  ..).r....Z.enbrA
-00001340: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001350: 0000 da1f 7465 7374 5f49 7465 7261 7469  ....test_Iterati
-00001360: 6f6e 734f 7574 4f66 5261 6e67 6545 7272  onsOutOfRangeErr
-00001370: 6f72 324e 0000 0073 0800 0000 0001 0a01  or2N...s........
-00001380: 2401 0e01 7a30 4173 684d 6f64 756c 6554  $...z0AshModuleT
-00001390: 6573 7469 6e67 2e74 6573 745f 4974 6572  esting.test_Iter
-000013a0: 6174 696f 6e73 4f75 744f 6652 616e 6765  ationsOutOfRange
-000013b0: 4572 726f 7232 6301 0000 0000 0000 0000  Error2c.........
-000013c0: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
-000013d0: 1a00 0000 7c00 a000 7401 7402 7c00 6a03  ....|...t.t.|.j.
-000013e0: a004 a100 8301 a102 0100 6400 5300 7214  ..........d.S.r.
-000013f0: 0000 0029 0572 1800 0000 7219 0000 0072  ...).r....r....r
-00001400: 2000 0000 720e 0000 005a 0a64 6563 546f   ...r....Z.decTo
-00001410: 4279 7465 7372 0f00 0000 7211 0000 0072  Bytesr....r....r
-00001420: 1100 0000 7212 0000 00da 1374 6573 745f  ....r......test_
-00001430: 4465 634f 7574 7075 7442 7974 6573 5400  DecOutputBytesT.
-00001440: 0000 7302 0000 0000 017a 2441 7368 4d6f  ..s......z$AshMo
-00001450: 6475 6c65 5465 7374 696e 672e 7465 7374  duleTesting.test
-00001460: 5f44 6563 4f75 7470 7574 4279 7465 7363  _DecOutputBytesc
-00001470: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001480: 0600 0000 4300 0000 731a 0000 007c 00a0  ....C...s....|..
-00001490: 0074 0174 027c 006a 03a0 04a1 0083 01a1  .t.t.|.j........
-000014a0: 0201 0064 0053 0072 1400 0000 2905 7218  ...d.S.r....).r.
-000014b0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
-000014c0: 0000 5a08 6465 6354 6f53 7472 720f 0000  ..Z.decToStrr...
-000014d0: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-000014e0: da14 7465 7374 5f44 6563 4f75 7470 7574  ..test_DecOutput
-000014f0: 5374 7269 6e67 5700 0000 7302 0000 0000  StringW...s.....
-00001500: 017a 2541 7368 4d6f 6475 6c65 5465 7374  .z%AshModuleTest
-00001510: 696e 672e 7465 7374 5f44 6563 4f75 7470  ing.test_DecOutp
-00001520: 7574 5374 7269 6e67 291b da08 5f5f 6e61  utString)...__na
-00001530: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001540: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7213  ..__qualname__r.
-00001550: 0000 0072 1500 0000 721d 0000 0072 2100  ...r....r....r!.
-00001560: 0000 7224 0000 0072 2700 0000 722a 0000  ..r$...r'...r*..
-00001570: 0072 2d00 0000 7230 0000 0072 3200 0000  .r-...r0...r2...
-00001580: 7233 0000 0072 3500 0000 7236 0000 0072  r3...r5...r6...r
-00001590: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
-000015a0: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
-000015b0: 0000 7242 0000 0072 4400 0000 7245 0000  ..rB...rD...rE..
-000015c0: 0072 4600 0000 7211 0000 0072 1100 0000  .rF...r....r....
-000015d0: 7211 0000 0072 1200 0000 7202 0000 0005  r....r....r.....
-000015e0: 0000 0073 3000 0000 0801 0e09 0e03 0803  ...s0...........
-000015f0: 0803 0803 0803 0803 0803 0803 0803 0803  ................
-00001600: 0803 0803 0803 0803 0803 0803 0803 0803  ................
-00001610: 0803 0806 0806 0803 7202 0000 00da 085f  ........r......_
-00001620: 5f6d 6169 6e5f 5f29 08da 0875 6e69 7474  _main__)...unitt
-00001630: 6573 7472 4300 0000 5a0c 4173 6843 7279  estrC...Z.AshCry
-00001640: 7074 2e41 7368 7207 0000 00da 0854 6573  pt.Ashr......Tes
-00001650: 7443 6173 6572 0200 0000 7247 0000 00da  tCaser....rG....
-00001660: 046d 6169 6e72 1100 0000 7211 0000 0072  .mainr....r....r
-00001670: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
-00001680: 6c65 3e01 0000 0073 0a00 0000 0801 0801  le>....s........
-00001690: 0c02 1258 0801                           ...X..
+00000220: 776f 726b 7373 1100 0000 7468 6973 2069  workss....this i
+00000230: 7320 6279 7465 7320 6e6f 775a 4036 6365  s bytes nowZ@6ce
+00000240: 3131 3362 6531 3965 3839 3863 3262 3938  113be19e898c2b98
+00000250: 6466 3832 6237 6661 3865 6662 3136 3639  df82b7fa8efb1669
+00000260: 3238 3932 3566 6330 3535 3734 6135 3465  28925fc05574a54e
+00000270: 6231 3131 3463 3334 3130 3930 30a9 02da  b1114c3410900...
+00000280: 076d 6573 7361 6765 da07 6d61 696e 6b65  .message..mainke
+00000290: 7929 0c5a 086d 6573 7361 6765 315a 086d  y).Z.message1Z.m
+000002a0: 6573 7361 6765 3272 0600 0000 da03 4173  essage2r......As
+000002b0: 68da 0345 6e63 da04 696e 7331 da08 656e  h..Enc..ins1..en
+000002c0: 6354 6f53 7472 5a0e 7374 7269 6e67 5f6d  cToStrZ.string_m
+000002d0: 6573 7361 6765 da0a 656e 6354 6f42 7974  essage..encToByt
+000002e0: 6573 da0d 6279 7465 735f 6d65 7373 6167  es..bytes_messag
+000002f0: 65da 0344 6563 da04 696e 7332 a901 da04  e..Dec..ins2....
+00000300: 7365 6c66 a900 7211 0000 00fa 3c43 3a5c  self..r.....<C:\
+00000310: 576f 726b 5c47 6974 4875 6257 6f72 6b5c  Work\GitHubWork\
+00000320: 4145 532d 3235 365c 4173 6843 7279 7074  AES-256\AshCrypt
+00000330: 5c75 6e69 7474 6573 7473 5c75 6e69 7474  \unittests\unitt
+00000340: 6573 7441 7368 2e70 79da 0573 6574 5570  estAsh.py..setUp
+00000350: 0700 0000 730e 0000 0000 0106 0106 0106  ....s...........
+00000360: 0114 010c 010c 017a 1641 7368 4d6f 6475  .......z.AshModu
+00000370: 6c65 5465 7374 696e 672e 7365 7455 7063  leTesting.setUpc
+00000380: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000390: 0100 0000 4300 0000 7304 0000 0064 0053  ....C...s....d.S
+000003a0: 00a9 014e 7211 0000 0072 0f00 0000 7211  ...Nr....r....r.
+000003b0: 0000 0072 1100 0000 7212 0000 00da 0874  ...r....r......t
+000003c0: 6561 7244 6f77 6e10 0000 0073 0200 0000  earDown....s....
+000003d0: 0001 7a19 4173 684d 6f64 756c 6554 6573  ..z.AshModuleTes
+000003e0: 7469 6e67 2e74 6561 7244 6f77 6e63 0100  ting.tearDownc..
+000003f0: 0000 0000 0000 0000 0000 0100 0000 0700  ................
+00000400: 0000 4300 0000 7320 0000 007c 00a0 0064  ..C...s ...|...d
+00000410: 0174 01a0 0274 036a 04a0 05a1 00a1 01a0  .t...t.j........
+00000420: 06a1 00a1 0201 0064 0053 0029 024e e920  .......d.S.).N. 
+00000430: 0000 0029 07da 0b61 7373 6572 7445 7175  ...)...assertEqu
+00000440: 616c da05 6279 7465 73da 0766 726f 6d68  al..bytes..fromh
+00000450: 6578 7207 0000 0072 0800 0000 da0a 6765  exr....r......ge
+00000460: 6e4d 6169 6e6b 6579 da07 5f5f 6c65 6e5f  nMainkey..__len_
+00000470: 5f72 0f00 0000 7211 0000 0072 1100 0000  _r....r....r....
+00000480: 7212 0000 00da 0e74 6573 745f 4b65 794c  r......test_KeyL
+00000490: 656e 6774 6813 0000 0073 0200 0000 0001  ength....s......
+000004a0: 7a1f 4173 684d 6f64 756c 6554 6573 7469  z.AshModuleTesti
+000004b0: 6e67 2e74 6573 745f 4b65 794c 656e 6774  ng.test_KeyLengt
+000004c0: 6863 0100 0000 0000 0000 0000 0000 0100  hc..............
+000004d0: 0000 0600 0000 4300 0000 731a 0000 007c  ......C...s....|
+000004e0: 00a0 0074 0174 0274 036a 04a0 05a1 0083  ...t.t.t.j......
+000004f0: 01a1 0201 0064 0053 0072 1400 0000 2906  .....d.S.r....).
+00000500: da08 6173 7365 7274 4973 da03 7374 72da  ..assertIs..str.
+00000510: 0474 7970 6572 0700 0000 7208 0000 0072  .typer....r....r
+00000520: 1a00 0000 720f 0000 0072 1100 0000 7211  ....r....r....r.
+00000530: 0000 0072 1200 0000 da0c 7465 7374 5f4b  ...r......test_K
+00000540: 6579 5479 7065 1600 0000 7302 0000 0000  eyType....s.....
+00000550: 017a 1d41 7368 4d6f 6475 6c65 5465 7374  .z.AshModuleTest
+00000560: 696e 672e 7465 7374 5f4b 6579 5479 7065  ing.test_KeyType
+00000570: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000580: 0005 0000 0043 0000 0073 2200 0000 7c00  .....C...s"...|.
+00000590: a000 7c00 6a01 6400 6401 8502 1900 7c00  ..|.j.d.d.....|.
+000005a0: 6a02 a003 a100 6b02 a101 0100 6400 5300  j.....k.....d.S.
+000005b0: 2902 4ee9 4000 0000 2904 da0a 6173 7365  ).N.@...)...asse
+000005c0: 7274 5472 7565 720c 0000 0072 0900 0000  rtTruer....r....
+000005d0: da04 484d 4143 720f 0000 0072 1100 0000  ..HMACr....r....
+000005e0: 7211 0000 0072 1200 0000 da09 7465 7374  r....r......test
+000005f0: 5f48 4d41 4319 0000 0073 0200 0000 0001  _HMAC....s......
+00000600: 7a1a 4173 684d 6f64 756c 6554 6573 7469  z.AshModuleTesti
+00000610: 6e67 2e74 6573 745f 484d 4143 6301 0000  ng.test_HMACc...
+00000620: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00000630: 0043 0000 0073 2000 0000 7c00 a000 7c00  .C...s ...|...|.
+00000640: 6a01 6401 6402 8502 1900 7c00 6a02 6a03  j.d.d.....|.j.j.
+00000650: 6b02 a101 0100 6400 5300 2903 4e72 2100  k.....d.S.).Nr!.
+00000660: 0000 e950 0000 0029 0472 2200 0000 720c  ...P...).r"...r.
+00000670: 0000 0072 0900 0000 da02 6976 720f 0000  ...r......ivr...
+00000680: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000690: da07 7465 7374 5f49 561c 0000 0073 0200  ..test_IV....s..
+000006a0: 0000 0001 7a18 4173 684d 6f64 756c 6554  ....z.AshModuleT
+000006b0: 6573 7469 6e67 2e74 6573 745f 4956 6301  esting.test_IVc.
+000006c0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+000006d0: 0000 0043 0000 0073 2000 0000 7c00 a000  ...C...s ...|...
+000006e0: 7c00 6a01 6401 6402 8502 1900 7c00 6a02  |.j.d.d.....|.j.
+000006f0: 6a03 6b02 a101 0100 6400 5300 2903 4e72  j.k.....d.S.).Nr
+00000700: 2500 0000 e960 0000 0029 0472 2200 0000  %....`...).r"...
+00000710: 720c 0000 0072 0900 0000 da04 7361 6c74  r....r......salt
+00000720: 720f 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000730: 1200 0000 da09 7465 7374 5f53 616c 741f  ......test_Salt.
+00000740: 0000 0073 0200 0000 0001 7a1a 4173 684d  ...s......z.AshM
+00000750: 6f64 756c 6554 6573 7469 6e67 2e74 6573  oduleTesting.tes
+00000760: 745f 5361 6c74 6301 0000 0000 0000 0000  t_Saltc.........
+00000770: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00000780: 2000 0000 7c00 a000 7c00 6a01 6401 6402   ...|...|.j.d.d.
+00000790: 8502 1900 7c00 6a02 6a03 6b02 a101 0100  ....|.j.j.k.....
+000007a0: 6400 5300 2903 4e72 2800 0000 e970 0000  d.S.).Nr(....p..
+000007b0: 0029 0472 2200 0000 720c 0000 0072 0900  .).r"...r....r..
+000007c0: 0000 da06 7065 7070 6572 720f 0000 0072  ....pepperr....r
+000007d0: 1100 0000 7211 0000 0072 1200 0000 da0b  ....r....r......
+000007e0: 7465 7374 5f50 6570 7065 7222 0000 0073  test_Pepper"...s
+000007f0: 0200 0000 0001 7a1c 4173 684d 6f64 756c  ......z.AshModul
+00000800: 6554 6573 7469 6e67 2e74 6573 745f 5065  eTesting.test_Pe
+00000810: 7070 6572 6301 0000 0000 0000 0000 0000  pperc...........
+00000820: 0001 0000 0005 0000 0043 0000 0073 2200  .........C...s".
+00000830: 0000 7c00 a000 7c00 6a01 6401 6402 8502  ..|...|.j.d.d...
+00000840: 1900 7c00 6a02 a003 a100 6b02 a101 0100  ..|.j.....k.....
+00000850: 6400 5300 2903 4e72 2b00 0000 e974 0000  d.S.).Nr+....t..
+00000860: 0029 0472 2200 0000 720c 0000 0072 0900  .).r"...r....r..
+00000870: 0000 da0f 7365 7475 7049 7465 7261 7469  ....setupIterati
+00000880: 6f6e 7372 0f00 0000 7211 0000 0072 1100  onsr....r....r..
+00000890: 0000 7212 0000 00da 0f74 6573 745f 4974  ..r......test_It
+000008a0: 6572 6174 696f 6e73 2500 0000 7306 0000  erations%...s...
+000008b0: 0000 0104 0116 ff7a 2041 7368 4d6f 6475  .......z AshModu
+000008c0: 6c65 5465 7374 696e 672e 7465 7374 5f49  leTesting.test_I
+000008d0: 7465 7261 7469 6f6e 7363 0100 0000 0000  terationsc......
+000008e0: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+000008f0: 0000 7322 0000 007c 00a0 007c 006a 0164  ..s"...|...|.j.d
+00000900: 0164 0085 0219 007c 006a 02a0 03a1 006b  .d.....|.j.....k
+00000910: 02a1 0101 0064 0053 0029 024e 722e 0000  .....d.S.).Nr...
+00000920: 0029 0472 2200 0000 720c 0000 0072 0900  .).r"...r....r..
+00000930: 0000 da0a 6369 7068 6572 7465 7874 720f  ....ciphertextr.
+00000940: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000950: 0000 da0f 7465 7374 5f43 6970 6865 7274  ....test_Ciphert
+00000960: 6578 7429 0000 0073 0200 0000 0001 7a20  ext)...s......z 
+00000970: 4173 684d 6f64 756c 6554 6573 7469 6e67  AshModuleTesting
+00000980: 2e74 6573 745f 4369 7068 6572 7465 7874  .test_Ciphertext
+00000990: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000009a0: 0006 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+000009b0: a000 7401 7402 7c00 6a03 a004 a100 8301  ..t.t.|.j.......
+000009c0: a102 0100 6400 5300 7214 0000 0029 0572  ....d.S.r....).r
+000009d0: 1d00 0000 7218 0000 0072 1f00 0000 7209  ....r....r....r.
+000009e0: 0000 0072 2f00 0000 720f 0000 0072 1100  ...r/...r....r..
+000009f0: 0000 7211 0000 0072 1200 0000 da13 7465  ..r....r......te
+00000a00: 7374 5f54 7970 6549 7465 7261 7469 6f6e  st_TypeIteration
+00000a10: 732c 0000 0073 0200 0000 0001 7a24 4173  s,...s......z$As
+00000a20: 684d 6f64 756c 6554 6573 7469 6e67 2e74  hModuleTesting.t
+00000a30: 6573 745f 5479 7065 4974 6572 6174 696f  est_TypeIteratio
+00000a40: 6e73 6301 0000 0000 0000 0000 0000 0001  nsc.............
+00000a50: 0000 0005 0000 0043 0000 0073 1a00 0000  .......C...s....
+00000a60: 7c00 a000 6401 7c00 6a01 a002 a100 a003  |...d.|.j.......
+00000a70: a100 a102 0100 6400 5300 2902 4ee9 0400  ......d.S.).N...
+00000a80: 0000 2904 7217 0000 0072 0900 0000 722f  ..).r....r....r/
+00000a90: 0000 0072 1b00 0000 720f 0000 0072 1100  ...r....r....r..
+00000aa0: 0000 7211 0000 0072 1200 0000 da19 7465  ..r....r......te
+00000ab0: 7374 5f49 7465 7261 7469 6f6e 7346 6978  st_IterationsFix
+00000ac0: 6564 5f73 697a 652f 0000 0073 0200 0000  ed_size/...s....
+00000ad0: 0001 7a2a 4173 684d 6f64 756c 6554 6573  ..z*AshModuleTes
+00000ae0: 7469 6e67 2e74 6573 745f 4974 6572 6174  ting.test_Iterat
+00000af0: 696f 6e73 4669 7865 645f 7369 7a65 6301  ionsFixed_sizec.
+00000b00: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00000b10: 0000 0043 0000 0073 1a00 0000 7c00 a000  ...C...s....|...
+00000b20: 7401 7402 7c00 6a03 a004 a100 8301 a102  t.t.|.j.........
+00000b30: 0100 6400 5300 7214 0000 0029 0572 1d00  ..d.S.r....).r..
+00000b40: 0000 7218 0000 0072 1f00 0000 7209 0000  ..r....r....r...
+00000b50: 0072 0b00 0000 720f 0000 0072 1100 0000  .r....r....r....
+00000b60: 7211 0000 0072 1200 0000 da13 7465 7374  r....r......test
+00000b70: 5f45 6e63 4f75 7470 7574 4279 7465 7332  _EncOutputBytes2
+00000b80: 0000 0073 0200 0000 0001 7a24 4173 684d  ...s......z$AshM
+00000b90: 6f64 756c 6554 6573 7469 6e67 2e74 6573  oduleTesting.tes
+00000ba0: 745f 456e 634f 7574 7075 7442 7974 6573  t_EncOutputBytes
+00000bb0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000bc0: 0006 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+00000bd0: a000 7401 7402 7c00 6a03 a004 a100 8301  ..t.t.|.j.......
+00000be0: a102 0100 6400 5300 7214 0000 0029 0572  ....d.S.r....).r
+00000bf0: 1d00 0000 721e 0000 0072 1f00 0000 7209  ....r....r....r.
+00000c00: 0000 0072 0a00 0000 720f 0000 0072 1100  ...r....r....r..
+00000c10: 0000 7211 0000 0072 1200 0000 da14 7465  ..r....r......te
+00000c20: 7374 5f45 6e63 4f75 7470 7574 5374 7269  st_EncOutputStri
+00000c30: 6e67 3500 0000 7302 0000 0000 017a 2541  ng5...s......z%A
+00000c40: 7368 4d6f 6475 6c65 5465 7374 696e 672e  shModuleTesting.
+00000c50: 7465 7374 5f45 6e63 4f75 7470 7574 5374  test_EncOutputSt
+00000c60: 7269 6e67 6301 0000 0000 0000 0000 0000  ringc...........
+00000c70: 0001 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
+00000c80: 0000 7c00 a000 7c00 6a01 a002 a100 7c00  ..|...|.j.....|.
+00000c90: 6a03 6a04 a102 0100 6400 5300 7214 0000  j.j.....d.S.r...
+00000ca0: 0029 0572 1700 0000 7209 0000 0072 2300  .).r....r....r#.
+00000cb0: 0000 720e 0000 005a 0872 6563 5f68 6d61  ..r....Z.rec_hma
+00000cc0: 6372 0f00 0000 7211 0000 0072 1100 0000  cr....r....r....
+00000cd0: 7212 0000 00da 0e74 6573 745f 484d 4143  r......test_HMAC
+00000ce0: 5f43 6f6d 7038 0000 0073 0200 0000 0001  _Comp8...s......
+00000cf0: 7a1f 4173 684d 6f64 756c 6554 6573 7469  z.AshModuleTesti
+00000d00: 6e67 2e74 6573 745f 484d 4143 5f43 6f6d  ng.test_HMAC_Com
+00000d10: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
+00000d20: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000d30: 00a0 007c 006a 016a 027c 006a 036a 04a1  ...|.j.j.|.j.j..
+00000d40: 0201 0064 0053 0072 1400 0000 2905 7217  ...d.S.r....).r.
+00000d50: 0000 0072 0900 0000 7226 0000 0072 0e00  ...r....r&...r..
+00000d60: 0000 5a06 7265 635f 6976 720f 0000 0072  ..Z.rec_ivr....r
+00000d70: 1100 0000 7211 0000 0072 1200 0000 da0c  ....r....r......
+00000d80: 7465 7374 5f49 565f 436f 6d70 3b00 0000  test_IV_Comp;...
+00000d90: 7302 0000 0000 017a 1d41 7368 4d6f 6475  s......z.AshModu
+00000da0: 6c65 5465 7374 696e 672e 7465 7374 5f49  leTesting.test_I
+00000db0: 565f 436f 6d70 6301 0000 0000 0000 0000  V_Compc.........
+00000dc0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000dd0: 1800 0000 7c00 a000 7c00 6a01 6a02 7c00  ....|...|.j.j.|.
+00000de0: 6a03 6a04 a102 0100 6400 5300 7214 0000  j.j.....d.S.r...
+00000df0: 0029 0572 1700 0000 7209 0000 0072 2900  .).r....r....r).
+00000e00: 0000 720e 0000 005a 0872 6563 5f73 616c  ..r....Z.rec_sal
+00000e10: 7472 0f00 0000 7211 0000 0072 1100 0000  tr....r....r....
+00000e20: 7212 0000 00da 0e74 6573 745f 5361 6c74  r......test_Salt
+00000e30: 5f43 6f6d 703e 0000 0073 0200 0000 0001  _Comp>...s......
+00000e40: 7a1f 4173 684d 6f64 756c 6554 6573 7469  z.AshModuleTesti
+00000e50: 6e67 2e74 6573 745f 5361 6c74 5f43 6f6d  ng.test_Salt_Com
+00000e60: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
+00000e70: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000e80: 00a0 007c 006a 016a 027c 006a 036a 04a1  ...|.j.j.|.j.j..
+00000e90: 0201 0064 0053 0072 1400 0000 2905 7217  ...d.S.r....).r.
+00000ea0: 0000 0072 0900 0000 722c 0000 0072 0e00  ...r....r,...r..
+00000eb0: 0000 5a0a 7265 635f 7065 7070 6572 720f  ..Z.rec_pepperr.
+00000ec0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000ed0: 0000 da10 7465 7374 5f50 6570 7065 725f  ....test_Pepper_
+00000ee0: 436f 6d70 4100 0000 7302 0000 0000 017a  CompA...s......z
+00000ef0: 2141 7368 4d6f 6475 6c65 5465 7374 696e  !AshModuleTestin
+00000f00: 672e 7465 7374 5f50 6570 7065 725f 436f  g.test_Pepper_Co
+00000f10: 6d70 6301 0000 0000 0000 0000 0000 0001  mpc.............
+00000f20: 0000 0004 0000 0043 0000 0073 1800 0000  .......C...s....
+00000f30: 7c00 a000 7c00 6a01 6a02 7c00 6a03 6a04  |...|.j.j.|.j.j.
+00000f40: a102 0100 6400 5300 7214 0000 0029 0572  ....d.S.r....).r
+00000f50: 1700 0000 7209 0000 005a 0a69 7465 7261  ....r....Z.itera
+00000f60: 7469 6f6e 7372 0e00 0000 5a0e 7265 635f  tionsr....Z.rec_
+00000f70: 6974 6572 6174 696f 6e73 720f 0000 0072  iterationsr....r
+00000f80: 1100 0000 7211 0000 0072 1200 0000 da14  ....r....r......
+00000f90: 7465 7374 5f49 7465 7261 7469 6f6e 735f  test_Iterations_
+00000fa0: 436f 6d70 4400 0000 7302 0000 0000 017a  CompD...s......z
+00000fb0: 2541 7368 4d6f 6475 6c65 5465 7374 696e  %AshModuleTestin
+00000fc0: 672e 7465 7374 5f49 7465 7261 7469 6f6e  g.test_Iteration
+00000fd0: 735f 436f 6d70 6301 0000 0000 0000 0000  s_Compc.........
+00000fe0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000ff0: 1a00 0000 7c00 a000 7c00 6a01 a002 a100  ....|...|.j.....
+00001000: 7c00 6a03 6a04 a102 0100 6400 5300 7214  |.j.j.....d.S.r.
+00001010: 0000 0029 0572 1700 0000 7209 0000 0072  ...).r....r....r
+00001020: 3100 0000 720e 0000 005a 0e72 6563 5f63  1...r....Z.rec_c
+00001030: 6970 6865 7274 6578 7472 0f00 0000 7211  iphertextr....r.
+00001040: 0000 0072 1100 0000 7212 0000 00da 1474  ...r....r......t
+00001050: 6573 745f 4369 7068 6572 7465 7874 5f43  est_Ciphertext_C
+00001060: 6f6d 7047 0000 0073 0200 0000 0001 7a25  ompG...s......z%
+00001070: 4173 684d 6f64 756c 6554 6573 7469 6e67  AshModuleTesting
+00001080: 2e74 6573 745f 4369 7068 6572 7465 7874  .test_Ciphertext
+00001090: 5f43 6f6d 7063 0100 0000 0000 0000 0000  _Compc..........
+000010a0: 0000 0300 0000 0800 0000 4300 0000 736c  ..........C...sl
+000010b0: 0000 007c 006a 00a0 01a1 0064 0064 0185  ...|.j.....d.d..
+000010c0: 0219 0064 0217 007d 017c 017c 006a 00a0  ...d...}.|.|.j..
+000010d0: 01a1 0064 0364 0085 0219 0017 007d 027c  ...d.d.......}.|
+000010e0: 00a0 0274 036a 04a1 018f 2001 0074 036a  ...t.j.... ..t.j
+000010f0: 057c 027c 006a 0664 048d 0201 0057 0064  .|.|.j.d.....W.d
+00001100: 0004 0004 0083 0301 006e 1031 0073 5e30  .........n.1.s^0
+00001110: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00001120: 054e e93f 0000 00f3 0100 0000 3172 2100  .N.?........1r!.
+00001130: 0000 7204 0000 0029 0772 0900 0000 720b  ..r....).r....r.
+00001140: 0000 00da 0c61 7373 6572 7452 6169 7365  .....assertRaise
+00001150: 7372 0700 0000 5a15 4d65 7373 6167 6554  sr....Z.MessageT
+00001160: 616d 7065 7269 6e67 4572 726f 7272 0d00  amperingErrorr..
+00001170: 0000 7206 0000 0029 0372 1000 0000 5a0d  ..r....).r....Z.
+00001180: 7461 6d70 6572 6564 5f48 4d41 43da 1074  tampered_HMAC..t
+00001190: 616d 7065 7265 645f 6d65 7373 6167 6572  ampered_messager
+000011a0: 1100 0000 7211 0000 0072 1200 0000 da17  ....r....r......
+000011b0: 7465 7374 5f48 4d41 435f 4d69 736d 6174  test_HMAC_Mismat
+000011c0: 6368 4572 726f 724a 0000 0073 0800 0000  chErrorJ...s....
+000011d0: 0001 1601 1601 0e01 7a28 4173 684d 6f64  ........z(AshMod
+000011e0: 756c 6554 6573 7469 6e67 2e74 6573 745f  uleTesting.test_
+000011f0: 484d 4143 5f4d 6973 6d61 7463 6845 7272  HMAC_MismatchErr
+00001200: 6f72 6301 0000 0000 0000 0000 0000 0003  orc.............
+00001210: 0000 0008 0000 0043 0000 0073 6e00 0000  .......C...sn...
+00001220: 7c00 6a00 a001 a100 7d01 7c01 6400 6401  |.j.....}.|.d.d.
+00001230: 8502 1900 7402 a003 6402 6403 a102 1700  ....t...d.d.....
+00001240: 7c01 6404 6400 8502 1900 1700 7d02 7c00  |.d.d.......}.|.
+00001250: a004 7405 6a06 a101 8f20 0100 7405 6a07  ..t.j.... ..t.j.
+00001260: 7c02 7c00 6a08 6405 8d02 0100 5700 6400  |.|.j.d.....W.d.
+00001270: 0400 0400 8303 0100 6e10 3100 7360 3000  ........n.1.s`0.
+00001280: 0100 0100 0100 5900 0100 6400 5300 2906  ......Y...d.S.).
+00001290: 4e72 2b00 0000 7a02 2149 69a1 8601 0072  Nr+...z.!Ii....r
+000012a0: 2e00 0000 7204 0000 0029 0972 0900 0000  ....r....).r....
+000012b0: 720b 0000 00da 0673 7472 7563 745a 0470  r......structZ.p
+000012c0: 6163 6b72 4000 0000 7207 0000 005a 1a49  ackr@...r....Z.I
+000012d0: 7465 7261 7469 6f6e 734f 7574 6f66 6152  terationsOutofaR
+000012e0: 616e 6765 4572 726f 7272 0d00 0000 7206  angeErrorr....r.
+000012f0: 0000 0029 0372 1000 0000 5a03 656e 6272  ...).r....Z.enbr
+00001300: 4100 0000 7211 0000 0072 1100 0000 7212  A...r....r....r.
+00001310: 0000 00da 1f74 6573 745f 4974 6572 6174  .....test_Iterat
+00001320: 696f 6e73 4f75 744f 6652 616e 6765 4572  ionsOutOfRangeEr
+00001330: 726f 7232 5000 0000 7308 0000 0000 010a  ror2P...s.......
+00001340: 0124 010e 017a 3041 7368 4d6f 6475 6c65  .$...z0AshModule
+00001350: 5465 7374 696e 672e 7465 7374 5f49 7465  Testing.test_Ite
+00001360: 7261 7469 6f6e 734f 7574 4f66 5261 6e67  rationsOutOfRang
+00001370: 6545 7272 6f72 3263 0100 0000 0000 0000  eError2c........
+00001380: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+00001390: 731a 0000 007c 00a0 0074 0174 027c 006a  s....|...t.t.|.j
+000013a0: 03a0 04a1 0083 01a1 0201 0064 0053 0072  ...........d.S.r
+000013b0: 1400 0000 2905 7217 0000 0072 1800 0000  ....).r....r....
+000013c0: 721f 0000 0072 0e00 0000 5a0a 6465 6354  r....r....Z.decT
+000013d0: 6f42 7974 6573 720f 0000 0072 1100 0000  oBytesr....r....
+000013e0: 7211 0000 0072 1200 0000 da13 7465 7374  r....r......test
+000013f0: 5f44 6563 4f75 7470 7574 4279 7465 7356  _DecOutputBytesV
+00001400: 0000 0073 0200 0000 0001 7a24 4173 684d  ...s......z$AshM
+00001410: 6f64 756c 6554 6573 7469 6e67 2e74 6573  oduleTesting.tes
+00001420: 745f 4465 634f 7574 7075 7442 7974 6573  t_DecOutputBytes
+00001430: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001440: 0006 0000 0043 0000 0073 1a00 0000 7c00  .....C...s....|.
+00001450: a000 7401 7402 7c00 6a03 a004 a100 8301  ..t.t.|.j.......
+00001460: a102 0100 6400 5300 7214 0000 0029 0572  ....d.S.r....).r
+00001470: 1700 0000 721e 0000 0072 1f00 0000 720e  ....r....r....r.
+00001480: 0000 005a 0864 6563 546f 5374 7272 0f00  ...Z.decToStrr..
+00001490: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000014a0: 00da 1474 6573 745f 4465 634f 7574 7075  ...test_DecOutpu
+000014b0: 7453 7472 696e 6759 0000 0073 0200 0000  tStringY...s....
+000014c0: 0001 7a25 4173 684d 6f64 756c 6554 6573  ..z%AshModuleTes
+000014d0: 7469 6e67 2e74 6573 745f 4465 634f 7574  ting.test_DecOut
+000014e0: 7075 7453 7472 696e 6729 1bda 085f 5f6e  putString)...__n
+000014f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00001500: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00001510: 1300 0000 7215 0000 0072 1c00 0000 7220  ....r....r....r 
+00001520: 0000 0072 2400 0000 7227 0000 0072 2a00  ...r$...r'...r*.
+00001530: 0000 722d 0000 0072 3000 0000 7232 0000  ..r-...r0...r2..
+00001540: 0072 3300 0000 7235 0000 0072 3600 0000  .r3...r5...r6...
+00001550: 7237 0000 0072 3800 0000 7239 0000 0072  r7...r8...r9...r
+00001560: 3a00 0000 723b 0000 0072 3c00 0000 723d  :...r;...r<...r=
+00001570: 0000 0072 4200 0000 7244 0000 0072 4500  ...rB...rD...rE.
+00001580: 0000 7246 0000 0072 1100 0000 7211 0000  ..rF...r....r...
+00001590: 0072 1100 0000 7212 0000 0072 0200 0000  .r....r....r....
+000015a0: 0600 0000 7330 0000 0008 010e 090e 0308  ....s0..........
+000015b0: 0308 0308 0308 0308 0308 0308 0408 0308  ................
+000015c0: 0308 0308 0308 0308 0308 0308 0308 0308  ................
+000015d0: 0308 0308 0608 0608 0372 0200 0000 da08  .........r......
+000015e0: 5f5f 6d61 696e 5f5f 2908 da08 756e 6974  __main__)...unit
+000015f0: 7465 7374 7243 0000 005a 0c41 7368 4372  testrC...Z.AshCr
+00001600: 7970 742e 4173 6872 0700 0000 da08 5465  ypt.Ashr......Te
+00001610: 7374 4361 7365 7202 0000 0072 4700 0000  stCaser....rG...
+00001620: da04 6d61 696e 7211 0000 0072 1100 0000  ..mainr....r....
+00001630: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+00001640: 756c 653e 0100 0000 730a 0000 0008 0108  ule>....s.......
+00001650: 010c 0312 5708 01                        ....W..
```

### Comparing `AshCrypt-1.3.5/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.3.6/AshCrypt/unittests/unittestAsh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import unittest
 import struct
 import AshCrypt.Ash as Ash
 
+
 class AshModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
         self.message2 = b'this is bytes now'
-        self.mainkey = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
+        self.mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
         self.ins1 = Ash.Enc(message=self.message1, mainkey=self.mainkey)
         self.string_message = self.ins1.encToStr()
         self.bytes_message = self.ins1.encToBytes()
-        self.ins2 = Ash.Dec(message=self.bytes_message,mainkey=self.mainkey)
+        self.ins2 = Ash.Dec(message=self.bytes_message, mainkey=self.mainkey)
 
     def tearDown(self) -> None:
         pass
 
     def test_KeyLength(self):
-        self.assertEqual(64, bytes.fromhex(Ash.Enc.genMainkey()).__len__())
+        self.assertEqual(32, bytes.fromhex(Ash.Enc.genMainkey()).__len__())
 
     def test_KeyType(self):
-        self.assertIs(str,type(Ash.Enc.genMainkey()))
+        self.assertIs(str, type(Ash.Enc.genMainkey()))
 
     def test_HMAC(self):
         self.assertTrue(self.bytes_message[:64] == self.ins1.HMAC())
 
     def test_IV(self):
         self.assertTrue(self.bytes_message[64:80] == self.ins1.iv)
 
     def test_Salt(self):
         self.assertTrue(self.bytes_message[80:96] == self.ins1.salt)
 
     def test_Pepper(self):
         self.assertTrue(self.bytes_message[96:112] == self.ins1.pepper)
 
     def test_Iterations(self):
-        self.assertTrue(self.bytes_message[112:116] == self.ins1.setupIterations())
+        self.assertTrue(
+            self.bytes_message[112:116] == self.ins1.setupIterations())
 
     def test_Ciphertext(self):
         self.assertTrue(self.bytes_message[116:] == self.ins1.ciphertext())
 
     def test_TypeIterations(self):
-        self.assertIs(bytes,type(self.ins1.setupIterations()))
+        self.assertIs(bytes, type(self.ins1.setupIterations()))
 
     def test_IterationsFixed_size(self):
-        self.assertEqual(4,self.ins1.setupIterations().__len__())
+        self.assertEqual(4, self.ins1.setupIterations().__len__())
 
     def test_EncOutputBytes(self):
-        self.assertIs(bytes,type(self.ins1.encToBytes()))
+        self.assertIs(bytes, type(self.ins1.encToBytes()))
 
     def test_EncOutputString(self):
-        self.assertIs(str,type(self.ins1.encToStr()))
+        self.assertIs(str, type(self.ins1.encToStr()))
 
     def test_HMAC_Comp(self):
         self.assertEqual(self.ins1.HMAC(), self.ins2.rec_hmac)
 
     def test_IV_Comp(self):
         self.assertEqual(self.ins1.iv, self.ins2.rec_iv)
 
@@ -63,32 +65,30 @@
     def test_Pepper_Comp(self):
         self.assertEqual(self.ins1.pepper, self.ins2.rec_pepper)
 
     def test_Iterations_Comp(self):
         self.assertEqual(self.ins1.iterations, self.ins2.rec_iterations)
 
     def test_Ciphertext_Comp(self):
-        self.assertEqual(self.ins1.ciphertext(),self.ins2.rec_ciphertext)
+        self.assertEqual(self.ins1.ciphertext(), self.ins2.rec_ciphertext)
 
     def test_HMAC_MismatchError(self):
         tampered_HMAC = self.ins1.encToBytes()[:63] + b'1'
         tampered_message = tampered_HMAC + self.ins1.encToBytes()[64:]
         with self.assertRaises(Ash.MessageTamperingError):
-            Ash.Dec(message = tampered_message, mainkey = self.mainkey)
+            Ash.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
         enb = self.ins1.encToBytes()
-        tampered_message = enb[:112] + struct.pack('!I',100001) + enb[116:]
+        tampered_message = enb[:112] + struct.pack('!I', 100001) + enb[116:]
         with self.assertRaises(Ash.IterationsOutofaRangeError):
-            Ash.Dec(message=tampered_message,mainkey=self.mainkey)
+            Ash.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_DecOutputBytes(self):
         self.assertEqual(bytes, type(self.ins2.decToBytes()))
 
     def test_DecOutputString(self):
         self.assertEqual(str, type(self.ins2.decToStr()))
 
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `AshCrypt-1.3.5/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.3.6/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.5/LICENSE` & `AshCrypt-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.5/setup.py` & `AshCrypt-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.3.5',
+    version='1.3.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

