# Comparing `tmp/npn-1.0.tar.gz` & `tmp/npn-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\npn-1.0.tar", last modified: Sat Jul  1 13:28:54 2023, max compression
+gzip compressed data, was "npn-1.1.tar", last modified: Fri Jul 14 01:21:45 2023, max compression
```

## Comparing `npn-1.0.tar` & `npn-1.1.tar`

### file list

```diff
@@ -1,8 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:28:54.000000 npn-1.0/
--rw-rw-rw-   0        0        0      384 2023-07-01 13:28:54.000000 npn-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 13:28:54.000000 npn-1.0/npn/
--rw-rw-rw-   0        0        0      154 2023-06-30 22:16:32.000000 npn-1.0/npn/__init__.py
--rw-rw-rw-   0        0        0     1792 2023-07-01 13:28:49.000000 npn-1.0/npn/api.py
--rw-rw-rw-   0        0        0    16632 2023-07-01 13:20:39.000000 npn-1.0/npn/libnpn.so
--rw-rw-rw-   0        0        0    12800 2023-07-01 13:12:43.000000 npn-1.0/npn/npn.dll
--rw-rw-rw-   0        0        0      458 2023-07-01 13:27:49.000000 npn-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.316379 npn-1.1/
+-rw-rw-rw-   0        0        0      325 2023-07-14 01:21:45.316379 npn-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2023-07-13 12:16:12.000000 npn-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.312379 npn-1.1/npn/
+-rw-rw-rw-   0        0        0      179 2023-07-13 18:02:13.000000 npn-1.1/npn/__init__.py
+-rw-rw-rw-   0        0        0     4471 2023-07-14 01:20:34.000000 npn-1.1/npn/api.py
+-rw-rw-rw-   0        0        0    16728 2023-07-14 00:26:42.000000 npn-1.1/npn/libnpn.so
+-rw-rw-rw-   0        0        0    13312 2023-07-13 19:51:46.000000 npn-1.1/npn/npn.dll
+drwxrwxrwx   0        0        0        0 2023-07-14 01:21:45.315379 npn-1.1/npn.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-14 01:21:45.000000 npn-1.1/npn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 01:21:45.316379 npn-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      458 2023-07-14 01:21:36.000000 npn-1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `npn-1.0/npn/libnpn.so` & `npn-1.1/npn/libnpn.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 12% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x10a0
+  Entry point address:               0x10c0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          14776 (bytes into file)
+  Start of section headers:          14872 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         29
   Section header string table index: 28
```

#### readelf --wide --program-header {}

```diff
@@ -1,25 +1,25 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x10a0
+Entry point 0x10c0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000820 0x000820 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000c95 0x000c95 R E 0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0001bc 0x0001bc R   0x1000
-  LOAD           0x002dc0 0x0000000000003dc0 0x0000000000003dc0 0x000278 0x07cf88 RW  0x1000
-  DYNAMIC        0x002dd8 0x0000000000003dd8 0x0000000000003dd8 0x0001d0 0x0001d0 RW  0x8
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0008d0 0x0008d0 R   0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000da9 0x000da9 R E 0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0001cc 0x0001cc R   0x1000
+  LOAD           0x002da8 0x0000000000003da8 0x0000000000003da8 0x000298 0x07cfc0 RW  0x1000
+  DYNAMIC        0x002dc0 0x0000000000003dc0 0x0000000000003dc0 0x0001e0 0x0001e0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   GNU_EH_FRAME   0x002000 0x0000000000002000 0x0000000000002000 0x000044 0x000044 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x002dc0 0x0000000000003dc0 0x0000000000003dc0 0x000240 0x000240 R   0x1
+  GNU_RELRO      0x002da8 0x0000000000003da8 0x0000000000003da8 0x000258 0x000258 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini 
    02     .eh_frame_hdr .eh_frame 
    03     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,38 +1,38 @@
-There are 29 section headers, starting at offset 0x39b8:
+There are 29 section headers, starting at offset 0x3a18:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
-  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000048 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000338 000338 000198 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          00000000000004d0 0004d0 00013c 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          000000000000060c 00060c 000022 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000000630 000630 000040 00   A  5   2  8
-  [ 8] .rela.dyn         RELA            0000000000000670 000670 000168 18   A  4   0  8
-  [ 9] .rela.plt         RELA            00000000000007d8 0007d8 000048 18  AI  4  22  8
+  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 00004c 00   A  4   0  8
+  [ 4] .dynsym           DYNSYM          0000000000000340 000340 0001c8 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          0000000000000508 000508 00016e 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          0000000000000676 000676 000026 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         00000000000006a0 0006a0 000050 00   A  5   2  8
+  [ 8] .rela.dyn         RELA            00000000000006f0 0006f0 000180 18   A  4   0  8
+  [ 9] .rela.plt         RELA            0000000000000870 000870 000060 18  AI  4  22  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
-  [11] .plt              PROGBITS        0000000000001020 001020 000040 10  AX  0   0 16
-  [12] .plt.got          PROGBITS        0000000000001060 001060 000010 10  AX  0   0 16
-  [13] .plt.sec          PROGBITS        0000000000001070 001070 000030 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000010a0 0010a0 000be5 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001c88 001c88 00000d 00  AX  0   0  4
+  [11] .plt              PROGBITS        0000000000001020 001020 000050 10  AX  0   0 16
+  [12] .plt.got          PROGBITS        0000000000001070 001070 000010 10  AX  0   0 16
+  [13] .plt.sec          PROGBITS        0000000000001080 001080 000040 10  AX  0   0 16
+  [14] .text             PROGBITS        00000000000010c0 0010c0 000cd9 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001d9c 001d9c 00000d 00  AX  0   0  4
   [16] .eh_frame_hdr     PROGBITS        0000000000002000 002000 000044 00   A  0   0  4
-  [17] .eh_frame         PROGBITS        0000000000002048 002048 000174 00   A  0   0  8
-  [18] .init_array       INIT_ARRAY      0000000000003dc0 002dc0 000010 08  WA  0   0  8
-  [19] .fini_array       FINI_ARRAY      0000000000003dd0 002dd0 000008 08  WA  0   0  8
-  [20] .dynamic          DYNAMIC         0000000000003dd8 002dd8 0001d0 10  WA  5   0  8
-  [21] .got              PROGBITS        0000000000003fa8 002fa8 000058 08  WA  0   0  8
-  [22] .got.plt          PROGBITS        0000000000004000 003000 000030 08  WA  0   0  8
-  [23] .data             PROGBITS        0000000000004030 003030 000008 00  WA  0   0  8
-  [24] .bss              NOBITS          0000000000004040 003038 07cd08 00  WA  0   0 32
-  [25] .comment          PROGBITS        0000000000000000 003038 00002a 01  MS  0   0  1
-  [26] .symtab           SYMTAB          0000000000000000 003068 0005e8 18     27  47  8
-  [27] .strtab           STRTAB          0000000000000000 003650 000261 00      0   0  1
-  [28] .shstrtab         STRTAB          0000000000000000 0038b1 000105 00      0   0  1
+  [17] .eh_frame         PROGBITS        0000000000002048 002048 000184 00   A  0   0  8
+  [18] .init_array       INIT_ARRAY      0000000000003da8 002da8 000010 08  WA  0   0  8
+  [19] .fini_array       FINI_ARRAY      0000000000003db8 002db8 000008 08  WA  0   0  8
+  [20] .dynamic          DYNAMIC         0000000000003dc0 002dc0 0001e0 10  WA  5   0  8
+  [21] .got              PROGBITS        0000000000003fa0 002fa0 000060 08  WA  0   0  8
+  [22] .got.plt          PROGBITS        0000000000004000 003000 000038 08  WA  0   0  8
+  [23] .data             PROGBITS        0000000000004038 003038 000008 00  WA  0   0  8
+  [24] .bss              NOBITS          0000000000004040 003040 07cd28 00  WA  0   0 32
+  [25] .comment          PROGBITS        0000000000000000 003040 00002a 01  MS  0   0  1
+  [26] .symtab           SYMTAB          0000000000000000 003070 000618 18     27  47  8
+  [27] .strtab           STRTAB          0000000000000000 003688 00028a 00      0   0  1
+  [28] .shstrtab         STRTAB          0000000000000000 003912 000105 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,86 +1,90 @@
 
-Symbol table '.dynsym' contains 17 entries:
+Symbol table '.dynsym' contains 19 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      2: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 (2)
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5 (3)
      4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 (2)
      5: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
      6: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
      7: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
-     8: 0000000000004060 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_next_
-     9: 0000000000074860  4320 OBJECT  GLOBAL DEFAULT   24 perm
-    10: 0000000000069460 46080 OBJECT  GLOBAL DEFAULT   24 phase_
-    11: 00000000000018b0   838 FUNC    GLOBAL DEFAULT   14 NpCanonicalRepresentative
-    12: 000000000005e060 46080 OBJECT  GLOBAL DEFAULT   24 phase_next_
-    13: 0000000000075940 46080 OBJECT  GLOBAL DEFAULT   24 pos
-    14: 0000000000031060 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_
-    15: 00000000000011a0  1800 FUNC    GLOBAL DEFAULT   14 GeneratePermutationTable
-    16: 0000000000001c00   133 FUNC    GLOBAL DEFAULT   14 NpnCanonicalRepresentative
+     8: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4 (4)
+     9: 0000000000004080 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_next_
+    10: 0000000000074880  4320 OBJECT  GLOBAL DEFAULT   24 perm
+    11: 0000000000004060     1 OBJECT  GLOBAL DEFAULT   24 c_num_inputs
+    12: 0000000000069480 46080 OBJECT  GLOBAL DEFAULT   24 phase_
+    13: 0000000000001900   872 FUNC    GLOBAL DEFAULT   14 NpCanonicalRepresentative
+    14: 000000000005e080 46080 OBJECT  GLOBAL DEFAULT   24 phase_next_
+    15: 0000000000075960 46080 OBJECT  GLOBAL DEFAULT   24 pos
+    16: 0000000000031080 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_
+    17: 00000000000011c0  1854 FUNC    GLOBAL DEFAULT   14 GeneratePermutationTable
+    18: 0000000000001c70   297 FUNC    GLOBAL DEFAULT   14 NpnCanonicalRepresentative
 
-Symbol table '.symtab' contains 63 entries:
+Symbol table '.symtab' contains 65 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 00000000000002a8     0 SECTION LOCAL  DEFAULT    1 .note.gnu.property
      2: 00000000000002c8     0 SECTION LOCAL  DEFAULT    2 .note.gnu.build-id
      3: 00000000000002f0     0 SECTION LOCAL  DEFAULT    3 .gnu.hash
-     4: 0000000000000338     0 SECTION LOCAL  DEFAULT    4 .dynsym
-     5: 00000000000004d0     0 SECTION LOCAL  DEFAULT    5 .dynstr
-     6: 000000000000060c     0 SECTION LOCAL  DEFAULT    6 .gnu.version
-     7: 0000000000000630     0 SECTION LOCAL  DEFAULT    7 .gnu.version_r
-     8: 0000000000000670     0 SECTION LOCAL  DEFAULT    8 .rela.dyn
-     9: 00000000000007d8     0 SECTION LOCAL  DEFAULT    9 .rela.plt
+     4: 0000000000000340     0 SECTION LOCAL  DEFAULT    4 .dynsym
+     5: 0000000000000508     0 SECTION LOCAL  DEFAULT    5 .dynstr
+     6: 0000000000000676     0 SECTION LOCAL  DEFAULT    6 .gnu.version
+     7: 00000000000006a0     0 SECTION LOCAL  DEFAULT    7 .gnu.version_r
+     8: 00000000000006f0     0 SECTION LOCAL  DEFAULT    8 .rela.dyn
+     9: 0000000000000870     0 SECTION LOCAL  DEFAULT    9 .rela.plt
     10: 0000000000001000     0 SECTION LOCAL  DEFAULT   10 .init
     11: 0000000000001020     0 SECTION LOCAL  DEFAULT   11 .plt
-    12: 0000000000001060     0 SECTION LOCAL  DEFAULT   12 .plt.got
-    13: 0000000000001070     0 SECTION LOCAL  DEFAULT   13 .plt.sec
-    14: 00000000000010a0     0 SECTION LOCAL  DEFAULT   14 .text
-    15: 0000000000001c88     0 SECTION LOCAL  DEFAULT   15 .fini
+    12: 0000000000001070     0 SECTION LOCAL  DEFAULT   12 .plt.got
+    13: 0000000000001080     0 SECTION LOCAL  DEFAULT   13 .plt.sec
+    14: 00000000000010c0     0 SECTION LOCAL  DEFAULT   14 .text
+    15: 0000000000001d9c     0 SECTION LOCAL  DEFAULT   15 .fini
     16: 0000000000002000     0 SECTION LOCAL  DEFAULT   16 .eh_frame_hdr
     17: 0000000000002048     0 SECTION LOCAL  DEFAULT   17 .eh_frame
-    18: 0000000000003dc0     0 SECTION LOCAL  DEFAULT   18 .init_array
-    19: 0000000000003dd0     0 SECTION LOCAL  DEFAULT   19 .fini_array
-    20: 0000000000003dd8     0 SECTION LOCAL  DEFAULT   20 .dynamic
-    21: 0000000000003fa8     0 SECTION LOCAL  DEFAULT   21 .got
+    18: 0000000000003da8     0 SECTION LOCAL  DEFAULT   18 .init_array
+    19: 0000000000003db8     0 SECTION LOCAL  DEFAULT   19 .fini_array
+    20: 0000000000003dc0     0 SECTION LOCAL  DEFAULT   20 .dynamic
+    21: 0000000000003fa0     0 SECTION LOCAL  DEFAULT   21 .got
     22: 0000000000004000     0 SECTION LOCAL  DEFAULT   22 .got.plt
-    23: 0000000000004030     0 SECTION LOCAL  DEFAULT   23 .data
+    23: 0000000000004038     0 SECTION LOCAL  DEFAULT   23 .data
     24: 0000000000004040     0 SECTION LOCAL  DEFAULT   24 .bss
     25: 0000000000000000     0 SECTION LOCAL  DEFAULT   25 .comment
     26: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS npn.cpp
-    27: 00000000000010a0    50 FUNC    LOCAL  DEFAULT   14 _GLOBAL__sub_I_npn.cpp
-    28: 0000000000080d40     1 OBJECT  LOCAL  DEFAULT   24 _ZStL8__ioinit
+    27: 00000000000010c0    50 FUNC    LOCAL  DEFAULT   14 _GLOBAL__sub_I_npn.cpp
+    28: 0000000000080d60     1 OBJECT  LOCAL  DEFAULT   24 _ZStL8__ioinit
     29: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    30: 00000000000010e0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
-    31: 0000000000001110     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
-    32: 0000000000001150     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
+    30: 0000000000001100     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
+    31: 0000000000001130     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
+    32: 0000000000001170     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
     33: 0000000000004040     1 OBJECT  LOCAL  DEFAULT   24 completed.8060
-    34: 0000000000003dd0     0 OBJECT  LOCAL  DEFAULT   19 __do_global_dtors_aux_fini_array_entry
-    35: 0000000000001190     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
-    36: 0000000000003dc0     0 OBJECT  LOCAL  DEFAULT   18 __frame_dummy_init_array_entry
+    34: 0000000000003db8     0 OBJECT  LOCAL  DEFAULT   19 __do_global_dtors_aux_fini_array_entry
+    35: 00000000000011b0     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
+    36: 0000000000003da8     0 OBJECT  LOCAL  DEFAULT   18 __frame_dummy_init_array_entry
     37: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    38: 00000000000021b8     0 OBJECT  LOCAL  DEFAULT   17 __FRAME_END__
+    38: 00000000000021c8     0 OBJECT  LOCAL  DEFAULT   17 __FRAME_END__
     39: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     40: 0000000000002000     0 NOTYPE  LOCAL  DEFAULT   16 __GNU_EH_FRAME_HDR
-    41: 0000000000001c88     0 FUNC    LOCAL  DEFAULT   15 _fini
+    41: 0000000000001d9c     0 FUNC    LOCAL  DEFAULT   15 _fini
     42: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   22 _GLOBAL_OFFSET_TABLE_
-    43: 0000000000004038     0 OBJECT  LOCAL  DEFAULT   23 __TMC_END__
-    44: 0000000000004030     0 OBJECT  LOCAL  DEFAULT   23 __dso_handle
-    45: 0000000000003dd8     0 OBJECT  LOCAL  DEFAULT   20 _DYNAMIC
+    43: 0000000000004040     0 OBJECT  LOCAL  DEFAULT   23 __TMC_END__
+    44: 0000000000004038     0 OBJECT  LOCAL  DEFAULT   23 __dso_handle
+    45: 0000000000003dc0     0 OBJECT  LOCAL  DEFAULT   20 _DYNAMIC
     46: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
-    47: 0000000000075940 46080 OBJECT  GLOBAL DEFAULT   24 pos
-    48: 0000000000004060 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_next_
+    47: 0000000000075960 46080 OBJECT  GLOBAL DEFAULT   24 pos
+    48: 0000000000004080 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_next_
     49: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4
     51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@@GLIBC_2.2.5
     52: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4
     53: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     54: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     55: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
-    56: 0000000000074860  4320 OBJECT  GLOBAL DEFAULT   24 perm
-    57: 0000000000069460 46080 OBJECT  GLOBAL DEFAULT   24 phase_
-    58: 00000000000018b0   838 FUNC    GLOBAL DEFAULT   14 NpCanonicalRepresentative
-    59: 000000000005e060 46080 OBJECT  GLOBAL DEFAULT   24 phase_next_
-    60: 00000000000011a0  1800 FUNC    GLOBAL DEFAULT   14 GeneratePermutationTable
-    61: 0000000000031060 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_
-    62: 0000000000001c00   133 FUNC    GLOBAL DEFAULT   14 NpnCanonicalRepresentative
+    56: 0000000000074880  4320 OBJECT  GLOBAL DEFAULT   24 perm
+    57: 0000000000004060     1 OBJECT  GLOBAL DEFAULT   24 c_num_inputs
+    58: 0000000000069480 46080 OBJECT  GLOBAL DEFAULT   24 phase_
+    59: 0000000000001900   872 FUNC    GLOBAL DEFAULT   14 NpCanonicalRepresentative
+    60: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@@GLIBC_2.4
+    61: 000000000005e080 46080 OBJECT  GLOBAL DEFAULT   24 phase_next_
+    62: 00000000000011c0  1854 FUNC    GLOBAL DEFAULT   14 GeneratePermutationTable
+    63: 0000000000031080 0x2d000 OBJECT  GLOBAL DEFAULT   24 ids_
+    64: 0000000000001c70   297 FUNC    GLOBAL DEFAULT   14 NpnCanonicalRepresentative
```

#### readelf --wide --relocs {}

```diff
@@ -1,24 +1,26 @@
 
-Relocation section '.rela.dyn' at offset 0x670 contains 15 entries:
+Relocation section '.rela.dyn' at offset 0x6f0 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000003dc0  0000000000000008 R_X86_64_RELATIVE                         1190
-0000000000003dc8  0000000000000008 R_X86_64_RELATIVE                         10a0
-0000000000003dd0  0000000000000008 R_X86_64_RELATIVE                         1150
-0000000000004030  0000000000000008 R_X86_64_RELATIVE                         4030
-0000000000003fa8  0000000d00000006 R_X86_64_GLOB_DAT      0000000000075940 pos + 0
-0000000000003fb0  0000000800000006 R_X86_64_GLOB_DAT      0000000000004060 ids_next_ + 0
-0000000000003fb8  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000003fc0  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
-0000000000003fc8  0000000500000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000003fd0  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000003fd8  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-0000000000003fe0  0000000900000006 R_X86_64_GLOB_DAT      0000000000074860 perm + 0
-0000000000003fe8  0000000a00000006 R_X86_64_GLOB_DAT      0000000000069460 phase_ + 0
-0000000000003ff0  0000000c00000006 R_X86_64_GLOB_DAT      000000000005e060 phase_next_ + 0
-0000000000003ff8  0000000e00000006 R_X86_64_GLOB_DAT      0000000000031060 ids_ + 0
+0000000000003da8  0000000000000008 R_X86_64_RELATIVE                         11b0
+0000000000003db0  0000000000000008 R_X86_64_RELATIVE                         10c0
+0000000000003db8  0000000000000008 R_X86_64_RELATIVE                         1170
+0000000000004038  0000000000000008 R_X86_64_RELATIVE                         4038
+0000000000003fa0  0000000f00000006 R_X86_64_GLOB_DAT      0000000000075960 pos + 0
+0000000000003fa8  0000000900000006 R_X86_64_GLOB_DAT      0000000000004080 ids_next_ + 0
+0000000000003fb0  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000003fb8  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
+0000000000003fc0  0000000500000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000003fc8  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000003fd0  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000003fd8  0000000a00000006 R_X86_64_GLOB_DAT      0000000000074880 perm + 0
+0000000000003fe0  0000000b00000006 R_X86_64_GLOB_DAT      0000000000004060 c_num_inputs + 0
+0000000000003fe8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000069480 phase_ + 0
+0000000000003ff0  0000000e00000006 R_X86_64_GLOB_DAT      000000000005e080 phase_next_ + 0
+0000000000003ff8  0000001000000006 R_X86_64_GLOB_DAT      0000000000031080 ids_ + 0
 
-Relocation section '.rela.plt' at offset 0x7d8 contains 3 entries:
+Relocation section '.rela.plt' at offset 0x870 contains 4 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000004018  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 + 0
 0000000000004020  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
-0000000000004028  0000000b00000007 R_X86_64_JUMP_SLOT     00000000000018b0 NpCanonicalRepresentative + 0
+0000000000004028  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000001900 NpCanonicalRepresentative + 0
+0000000000004030  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,29 @@
 
-Dynamic section at offset 0x2dd8 contains 25 entries:
+Dynamic section at offset 0x2dc0 contains 26 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
+ 0x000000000000000e (SONAME)             Library soname: [libnpn.so]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1c88
- 0x0000000000000019 (INIT_ARRAY)         0x3dc0
+ 0x000000000000000d (FINI)               0x1d9c
+ 0x0000000000000019 (INIT_ARRAY)         0x3da8
  0x000000000000001b (INIT_ARRAYSZ)       16 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x3dd0
+ 0x000000000000001a (FINI_ARRAY)         0x3db8
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0x4d0
- 0x0000000000000006 (SYMTAB)             0x338
- 0x000000000000000a (STRSZ)              316 (bytes)
+ 0x0000000000000005 (STRTAB)             0x508
+ 0x0000000000000006 (SYMTAB)             0x340
+ 0x000000000000000a (STRSZ)              366 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4000
- 0x0000000000000002 (PLTRELSZ)           72 (bytes)
+ 0x0000000000000002 (PLTRELSZ)           96 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x7d8
- 0x0000000000000007 (RELA)               0x670
- 0x0000000000000008 (RELASZ)             360 (bytes)
+ 0x0000000000000017 (JMPREL)             0x870
+ 0x0000000000000007 (RELA)               0x6f0
+ 0x0000000000000008 (RELASZ)             384 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x630
+ 0x000000006ffffffe (VERNEED)            0x6a0
  0x000000006fffffff (VERNEEDNUM)         2
- 0x000000006ffffff0 (VERSYM)             0x60c
+ 0x000000006ffffff0 (VERSYM)             0x676
  0x000000006ffffff9 (RELACOUNT)          4
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 58f623147ed87aa1432d90fd8823fb254112b44d
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0b152c8771dc4bbaaa3e54385165b586087b02f4
```

#### readelf --wide --version-info {}

```diff
@@ -1,15 +1,16 @@
 
-Version symbols section '.gnu.version' contains 17 entries:
- Addr: 0x000000000000060c  Offset: 0x0000060c  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 19 entries:
+ Addr: 0x0000000000000676  Offset: 0x00000676  Link: 4 (.dynsym)
   000:   0 (*local*)       0 (*local*)       2 (GLIBCXX_3.4)   3 (GLIBC_2.2.5)
   004:   2 (GLIBCXX_3.4)   0 (*local*)       0 (*local*)       3 (GLIBC_2.2.5)
-  008:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
+  008:   4 (GLIBC_2.4)     1 (*global*)      1 (*global*)      1 (*global*)   
   00c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  010:   1 (*global*)   
+  010:   1 (*global*)      1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 2 entries:
- Addr: 0x0000000000000630  Offset: 0x00000630  Link: 5 (.dynstr)
-  000000: Version: 1  File: libc.so.6  Cnt: 1
-  0x0010:   Name: GLIBC_2.2.5  Flags: none  Version: 3
-  0x0020: Version: 1  File: libstdc++.so.6  Cnt: 1
-  0x0030:   Name: GLIBCXX_3.4  Flags: none  Version: 2
+ Addr: 0x00000000000006a0  Offset: 0x000006a0  Link: 5 (.dynstr)
+  000000: Version: 1  File: libc.so.6  Cnt: 2
+  0x0010:   Name: GLIBC_2.4  Flags: none  Version: 4
+  0x0020:   Name: GLIBC_2.2.5  Flags: none  Version: 3
+  0x0030: Version: 1  File: libstdc++.so.6  Cnt: 1
+  0x0040:   Name: GLIBCXX_3.4  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,168 +9,178 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001020..0000000000001060
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001020..0000000000001070
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000001026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000001030
   DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000001060..0000000000001070
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000001070..0000000000001080
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000001070..00000000000010a0
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000001080..00000000000010c0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000070 000000000000004c 00000074 FDE cie=00000000 pc=00000000000011a0..00000000000018a8
-  DW_CFA_advance_loc: 6 to 00000000000011a6
+00000070 000000000000004c 00000074 FDE cie=00000000 pc=00000000000011c0..00000000000018fe
+  DW_CFA_advance_loc: 6 to 00000000000011c6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 9 to 00000000000011af
+  DW_CFA_advance_loc: 6 to 00000000000011cc
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 4 to 00000000000011b3
+  DW_CFA_advance_loc: 4 to 00000000000011d0
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000011b5
+  DW_CFA_advance_loc: 5 to 00000000000011d5
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000011b6
+  DW_CFA_advance_loc: 1 to 00000000000011d6
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000011b7
+  DW_CFA_advance_loc: 1 to 00000000000011d7
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 8 to 00000000000011bf
-  DW_CFA_def_cfa_offset: 136
-  DW_CFA_advance_loc2: 1722 to 0000000000001879
+  DW_CFA_advance_loc: 4 to 00000000000011db
+  DW_CFA_def_cfa_offset: 168
+  DW_CFA_advance_loc2: 1778 to 00000000000018cd
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000187a
+  DW_CFA_advance_loc: 4 to 00000000000018d1
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 000000000000187b
+  DW_CFA_advance_loc: 1 to 00000000000018d2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000187d
+  DW_CFA_advance_loc: 2 to 00000000000018d4
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000187f
+  DW_CFA_advance_loc: 2 to 00000000000018d6
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001881
+  DW_CFA_advance_loc: 2 to 00000000000018d8
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001883
+  DW_CFA_advance_loc: 2 to 00000000000018da
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001884
+  DW_CFA_advance_loc: 1 to 00000000000018db
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000c0 0000000000000058 000000c4 FDE cie=00000000 pc=00000000000018b0..0000000000001bf6
-  DW_CFA_advance_loc: 10 to 00000000000018ba
+000000c0 0000000000000058 000000c4 FDE cie=00000000 pc=0000000000001900..0000000000001c68
+  DW_CFA_advance_loc: 6 to 0000000000001906
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 5 to 00000000000018bf
+  DW_CFA_advance_loc: 5 to 000000000000190b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000018c1
+  DW_CFA_advance_loc: 2 to 000000000000190d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000018c3
+  DW_CFA_advance_loc: 2 to 000000000000190f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000018c4
+  DW_CFA_advance_loc: 1 to 0000000000001910
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 00000000000018c5
+  DW_CFA_advance_loc: 1 to 0000000000001911
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc2: 598 to 0000000000001b1b
+  DW_CFA_advance_loc2: 618 to 0000000000001b7b
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001b1c
+  DW_CFA_advance_loc: 1 to 0000000000001b7c
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 5 to 0000000000001b21
+  DW_CFA_advance_loc: 5 to 0000000000001b81
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001b23
+  DW_CFA_advance_loc: 2 to 0000000000001b83
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001b25
+  DW_CFA_advance_loc: 2 to 0000000000001b85
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001b27
+  DW_CFA_advance_loc: 2 to 0000000000001b87
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001b28
+  DW_CFA_advance_loc: 1 to 0000000000001b88
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 150 to 0000000000001bbe
+  DW_CFA_advance_loc1: 169 to 0000000000001c31
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 4 to 0000000000001bc2
+  DW_CFA_advance_loc: 1 to 0000000000001c32
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001bc4
+  DW_CFA_advance_loc: 2 to 0000000000001c34
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001bc6
+  DW_CFA_advance_loc: 2 to 0000000000001c36
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001bc8
+  DW_CFA_advance_loc: 2 to 0000000000001c38
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001bca
+  DW_CFA_advance_loc: 2 to 0000000000001c3a
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001bcb
+  DW_CFA_advance_loc: 1 to 0000000000001c3b
   DW_CFA_restore_state
 
-0000011c 0000000000000038 00000120 FDE cie=00000000 pc=0000000000001c00..0000000000001c85
-  DW_CFA_advance_loc: 6 to 0000000000001c06
+0000011c 0000000000000048 00000120 FDE cie=00000000 pc=0000000000001c70..0000000000001d99
+  DW_CFA_advance_loc: 6 to 0000000000001c76
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 6 to 0000000000001c0c
+  DW_CFA_offset: r15 (r15) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000001c78
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000001c10
+  DW_CFA_offset: r14 (r14) at cfa-24
+  DW_CFA_advance_loc: 8 to 0000000000001c80
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000001c14
+  DW_CFA_offset: r13 (r13) at cfa-32
+  DW_CFA_advance_loc: 5 to 0000000000001c85
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 9 to 0000000000001c1d
+  DW_CFA_offset: r12 (r12) at cfa-40
+  DW_CFA_advance_loc: 4 to 0000000000001c89
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc1: 81 to 0000000000001c6e
+  DW_CFA_offset: r6 (rbp) at cfa-48
+  DW_CFA_advance_loc: 4 to 0000000000001c8d
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_offset: r3 (rbx) at cfa-56
+  DW_CFA_advance_loc: 7 to 0000000000001c94
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc1: 192 to 0000000000001d54
   DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 1 to 0000000000001d55
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 0000000000001d56
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000001c6f
+  DW_CFA_advance_loc: 2 to 0000000000001d58
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000001c70
+  DW_CFA_advance_loc: 2 to 0000000000001d5a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001c72
+  DW_CFA_advance_loc: 2 to 0000000000001d5c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001c74
+  DW_CFA_advance_loc: 2 to 0000000000001d5e
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 0000000000001c78
+  DW_CFA_advance_loc: 2 to 0000000000001d60
   DW_CFA_restore_state
   DW_CFA_nop
 
-00000158 0000000000000014 0000015c FDE cie=00000000 pc=00000000000010a0..00000000000010d2
-  DW_CFA_advance_loc: 8 to 00000000000010a8
+00000168 0000000000000014 0000016c FDE cie=00000000 pc=00000000000010c0..00000000000010f2
+  DW_CFA_advance_loc: 8 to 00000000000010c8
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 23 to 00000000000010bf
+  DW_CFA_advance_loc: 23 to 00000000000010df
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000170 ZERO terminator
+00000180 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -1,30 +1,36 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 GeneratePermutationTable
+c_num_inputs
 NpCanonicalRepresentative
 ids_next_
 phase_next_
 NpnCanonicalRepresentative
+__stack_chk_fail
 _ZNSt8ios_base4InitC1Ev
 _ZNSt8ios_base4InitD1Ev
 __cxa_atexit
 libstdc++.so.6
 libc.so.6
+libnpn.so
+GLIBC_2.4
 GLIBC_2.2.5
 GLIBCXX_3.4
-@:|$D~ZHct$
-@:|$E~=Hct$ HcT$$A
-@:|$F~ Hct$(HcT$,A
-P[]A\A]A^A_
-AVAUATUS
+@:|$"~mHct$
+@:|$#~PHct$$HcT$(A
+@:|$d~3Hct$0HcT$4A
+Hct$8HcT$<A
+[]A\A]A^A_
+AVAUATUSH
 A\A]A^A_
-]A\A]A^A_
+[]A\A]A^A_
+8[]A\A]A^A_
 GCC: (Ubuntu 9.3.0-17ubuntu1~20.04) 9.3.0
 _GLOBAL__sub_I_npn.cpp
 _ZStL8__ioinit
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8060
@@ -41,15 +47,17 @@
 __gmon_start__
 _ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4
 __cxa_atexit@@GLIBC_2.2.5
 _ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize@@GLIBC_2.2.5
+c_num_inputs
 NpCanonicalRepresentative
+__stack_chk_fail@@GLIBC_2.4
 phase_next_
 GeneratePermutationTable
 NpnCanonicalRepresentative
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .gnu.hash
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,8 +1,8 @@
 
 Hex dump of section '.gnu.hash':
-  0x000002f0 03000000 08000000 01000000 06000000 ................
-  0x00000300 8014890c 14803053 08000000 0d000000 ......0S........
-  0x00000310 0f000000 e261e17c b8369c7c f4e6b114 .....a.|.6.|....
-  0x00000320 fc115941 937f5171 169e880b e55b987c ..YA..Qq.....[.|
-  0x00000330 101d428f 0b533a67                   ..B..S:g
+  0x000002f0 03000000 09000000 01000000 06000000 ................
+  0x00000300 8015890c 14803053 09000000 0f000000 ......0S........
+  0x00000310 11000000 e261e17c b8369c7c 38f268e3 .....a.|.6.|8.h.
+  0x00000320 f4e6b114 fc115941 937f5171 169e880b ......YA..Qq....
+  0x00000330 e55b987c 101d428f 0b533a67          .[.|..B..S:g
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,23 +1,26 @@
 
 Hex dump of section '.dynstr':
-  0x000004d0 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x000004e0 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x000004f0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000500 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000510 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000520 6c697a65 0047656e 65726174 65506572 lize.GeneratePer
-  0x00000530 6d757461 74696f6e 5461626c 6500706f mutationTable.po
-  0x00000540 73007065 726d004e 7043616e 6f6e6963 s.perm.NpCanonic
-  0x00000550 616c5265 70726573 656e7461 74697665 alRepresentative
-  0x00000560 00706861 73655f00 6964735f 00696473 .phase_.ids_.ids
-  0x00000570 5f6e6578 745f0070 68617365 5f6e6578 _next_.phase_nex
-  0x00000580 745f004e 706e4361 6e6f6e69 63616c52 t_.NpnCanonicalR
-  0x00000590 65707265 73656e74 61746976 65005f5a epresentative._Z
-  0x000005a0 4e537438 696f735f 62617365 34496e69 NSt8ios_base4Ini
-  0x000005b0 74433145 76005f5a 4e537438 696f735f tC1Ev._ZNSt8ios_
-  0x000005c0 62617365 34496e69 74443145 76005f5f base4InitD1Ev.__
-  0x000005d0 6378615f 61746578 6974006c 69627374 cxa_atexit.libst
-  0x000005e0 64632b2b 2e736f2e 36006c69 62632e73 dc++.so.6.libc.s
-  0x000005f0 6f2e3600 474c4942 435f322e 322e3500 o.6.GLIBC_2.2.5.
-  0x00000600 474c4942 4358585f 332e3400          GLIBCXX_3.4.
+  0x00000508 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x00000518 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x00000528 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x00000538 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x00000548 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000558 6c697a65 0047656e 65726174 65506572 lize.GeneratePer
+  0x00000568 6d757461 74696f6e 5461626c 6500706f mutationTable.po
+  0x00000578 73007065 726d0063 5f6e756d 5f696e70 s.perm.c_num_inp
+  0x00000588 75747300 4e704361 6e6f6e69 63616c52 uts.NpCanonicalR
+  0x00000598 65707265 73656e74 61746976 65006964 epresentative.id
+  0x000005a8 735f0070 68617365 5f006964 735f6e65 s_.phase_.ids_ne
+  0x000005b8 78745f00 70686173 655f6e65 78745f00 xt_.phase_next_.
+  0x000005c8 4e706e43 616e6f6e 6963616c 52657072 NpnCanonicalRepr
+  0x000005d8 6573656e 74617469 7665005f 5f737461 esentative.__sta
+  0x000005e8 636b5f63 686b5f66 61696c00 5f5a4e53 ck_chk_fail._ZNS
+  0x000005f8 7438696f 735f6261 73653449 6e697443 t8ios_base4InitC
+  0x00000608 31457600 5f5a4e53 7438696f 735f6261 1Ev._ZNSt8ios_ba
+  0x00000618 73653449 6e697444 31457600 5f5f6378 se4InitD1Ev.__cx
+  0x00000628 615f6174 65786974 006c6962 73746463 a_atexit.libstdc
+  0x00000638 2b2b2e73 6f2e3600 6c696263 2e736f2e ++.so.6.libc.so.
+  0x00000648 36006c69 626e706e 2e736f00 474c4942 6.libnpn.so.GLIB
+  0x00000658 435f322e 3400474c 4942435f 322e322e C_2.4.GLIBC_2.2.
+  0x00000668 3500474c 49424358 585f332e 3400     5.GLIBCXX_3.4.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -3,13 +3,13 @@
 
 Disassembly of section .init:
 
 0000000000001000 <_init>:
 _init():
 	endbr64
 	sub    $0x8,%rsp
-	mov    0x2fa9(%rip),%rax        
+	mov    0x2fa1(%rip),%rax        
 	test   %rax,%rax
 	je     1016 <_init+0x16>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -15,7 +15,11 @@
 	push   $0x1
 	bnd jmp 1020 <.plt>
 	nop
 	endbr64
 	push   $0x2
 	bnd jmp 1020 <.plt>
 	nop
+	endbr64
+	push   $0x3
+	bnd jmp 1020 <.plt>
+	nop
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,9 +1,9 @@
 
 
 
 Disassembly of section .plt.got:
 
-0000000000001060 <__cxa_finalize@plt>:
+0000000000001070 <__cxa_finalize@plt>:
 	endbr64
-	bnd jmp *0x2f6d(%rip)        
+	bnd jmp *0x2f55(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.sec {}

```diff
@@ -1,19 +1,24 @@
 
 
 
 Disassembly of section .plt.sec:
 
-0000000000001070 <std::ios_base::Init::Init()@plt>:
+0000000000001080 <std::ios_base::Init::Init()@plt>:
 	endbr64
-	bnd jmp *0x2f9d(%rip)        
+	bnd jmp *0x2f8d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001080 <__cxa_atexit@plt>:
+0000000000001090 <__cxa_atexit@plt>:
 	endbr64
-	bnd jmp *0x2f95(%rip)        
+	bnd jmp *0x2f85(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001090 <NpCanonicalRepresentative@plt>:
+00000000000010a0 <NpCanonicalRepresentative@plt>:
 	endbr64
-	bnd jmp *0x2f8d(%rip)        
+	bnd jmp *0x2f7d(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+00000000000010b0 <__stack_chk_fail@plt>:
+	endbr64
+	bnd jmp *0x2f75(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,819 +1,881 @@
 
 
 
 Disassembly of section .text:
 
-00000000000010a0 <_GLOBAL__sub_I_npn.cpp>:
+00000000000010c0 <_GLOBAL__sub_I_npn.cpp>:
 _GLOBAL__sub_I_npn.cpp():
 	endbr64
 	sub    $0x8,%rsp
 	lea    0x7fc91(%rip),%rdi        
-	call   1070 <std::ios_base::Init::Init()@plt>
-	mov    0x2f05(%rip),%rdi        
+	call   1080 <std::ios_base::Init::Init()@plt>
+	mov    0x2edd(%rip),%rdi        
 	add    $0x8,%rsp
-	lea    0x2f6a(%rip),%rdx        
+	lea    0x2f52(%rip),%rdx        
 	lea    0x7fc73(%rip),%rsi        
-	jmp    1080 <__cxa_atexit@plt>
+	jmp    1090 <__cxa_atexit@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
-00000000000010e0 <deregister_tm_clones>:
+0000000000001100 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x2f51(%rip),%rdi        
-	lea    0x2f4a(%rip),%rax        
+	lea    0x2f39(%rip),%rdi        
+	lea    0x2f32(%rip),%rax        
 	cmp    %rdi,%rax
-	je     1108 <deregister_tm_clones+0x28>
-	mov    0x2ece(%rip),%rax        
+	je     1128 <deregister_tm_clones+0x28>
+	mov    0x2ea6(%rip),%rax        
 	test   %rax,%rax
-	je     1108 <deregister_tm_clones+0x28>
+	je     1128 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000001110 <register_tm_clones>:
+0000000000001130 <register_tm_clones>:
 register_tm_clones():
-	lea    0x2f21(%rip),%rdi        
-	lea    0x2f1a(%rip),%rsi        
+	lea    0x2f09(%rip),%rdi        
+	lea    0x2f02(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    %rsi
-	je     1148 <register_tm_clones+0x38>
-	mov    0x2e95(%rip),%rax        
+	je     1168 <register_tm_clones+0x38>
+	mov    0x2e6d(%rip),%rax        
 	test   %rax,%rax
-	je     1148 <register_tm_clones+0x38>
+	je     1168 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
-0000000000001150 <__do_global_dtors_aux>:
+0000000000001170 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0x2ee5(%rip)        
-	jne    1188 <__do_global_dtors_aux+0x38>
+	cmpb   $0x0,0x2ec5(%rip)        
+	jne    11a8 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x2e72(%rip)        
+	cmpq   $0x0,0x2e4a(%rip)        
 	mov    %rsp,%rbp
-	je     1177 <__do_global_dtors_aux+0x27>
-	mov    0x2ebe(%rip),%rdi        
-	call   1060 <__cxa_finalize@plt>
-	call   10e0 <deregister_tm_clones>
-	movb   $0x1,0x2ebd(%rip)        
+	je     1197 <__do_global_dtors_aux+0x27>
+	mov    0x2ea6(%rip),%rdi        
+	call   1070 <__cxa_finalize@plt>
+	call   1100 <deregister_tm_clones>
+	movb   $0x1,0x2e9d(%rip)        
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000001190 <frame_dummy>:
+00000000000011b0 <frame_dummy>:
 frame_dummy():
 	endbr64
-	jmp    1110 <register_tm_clones>
+	jmp    1130 <register_tm_clones>
 	nopl   0x0(%rax)
 
-00000000000011a0 <GeneratePermutationTable>:
+00000000000011c0 <GeneratePermutationTable>:
 GeneratePermutationTable():
 	endbr64
 	push   %r15
 	movsbl %dil,%eax
-	mov    %edi,%r8d
 	push   %r14
 	mov    %eax,%edx
 	push   %r13
+	mov    %edi,%r13d
 	push   %r12
 	push   %rbp
 	push   %rbx
-	mov    %eax,%ebx
-	mov    %ebx,%ecx
-	sub    $0x50,%rsp
-	mov    %eax,0x3c(%rsp)
+	sub    $0x70,%rsp
+	mov    %edi,0x60(%rsp)
+	mov    %eax,%edi
+	mov    %eax,0x58(%rsp)
+	mov    %edi,%ecx
 	mov    $0x1,%eax
-	mov    %dil,-0x49(%rsp)
-	cmp    $0x1,%ebx
-	jbe    11e0 <GeneratePermutationTable+0x40>
+	cmp    $0x1,%edi
+	jbe    11ff <GeneratePermutationTable+0x3f>
 	imul   %eax,%ecx
 	add    $0x1,%eax
 	cmp    %eax,%edx
-	jne    11d2 <GeneratePermutationTable+0x32>
-	mov    %ecx,0x3c(%rsp)
-	mov    0x3c(%rsp),%esi
-	test   %esi,%esi
-	je     1295 <GeneratePermutationTable+0xf5>
-	mov    0x3c(%rsp),%eax
-	mov    0x2db1(%rip),%rcx        
-	mov    0x2de2(%rip),%rsi        
-	lea    -0x1(%rax),%r9d
-	movzbl -0x49(%rsp),%eax
-	lea    0x40(%rcx),%r10
-	shl    $0x6,%r9
-	lea    -0x1(%rax),%edx
-	add    %r10,%r9
-	movabs $0x101010101010101,%rax
+	jne    11f1 <GeneratePermutationTable+0x31>
+	mov    %ecx,0x58(%rsp)
+	mov    0x58(%rsp),%eax
+	test   %eax,%eax
+	je     18e7 <GeneratePermutationTable+0x727>
+	mov    0x58(%rsp),%eax
+	lea    -0x1(%r13),%edx
+	mov    0x2d86(%rip),%rcx        
+	movabs $0x101010101010101,%rdi
 	movzbl %dl,%edx
+	mov    0x2daa(%rip),%r14        
 	add    $0x1,%rdx
-	mov    %edx,%ebp
+	lea    -0x1(%rax),%r8d
+	lea    0x40(%rcx),%r9
+	movzbl %r13b,%eax
+	shl    $0x6,%r8
 	mov    %edx,%ebx
 	mov    %edx,%r11d
-	and    $0x4,%ebp
-	and    $0x2,%ebx
-	jmp    125c <GeneratePermutationTable+0xbc>
-	test   %ebp,%ebp
-	jne    1884 <GeneratePermutationTable+0x6e4>
-	test   %edx,%edx
-	je     124c <GeneratePermutationTable+0xac>
-	movb   $0x1,(%rsi)
+	mov    %r14,%rsi
+	imul   %rdi,%rax
+	add    %r9,%r8
+	mov    %edx,%r10d
+	and    $0x4,%ebx
+	and    $0x2,%r11d
+	jmp    1284 <GeneratePermutationTable+0xc4>
 	test   %ebx,%ebx
-	jne    1898 <GeneratePermutationTable+0x6f8>
-	mov    %r10,%rcx
+	jne    18db <GeneratePermutationTable+0x71b>
+	test   %edx,%edx
+	je     1274 <GeneratePermutationTable+0xb4>
+	mov    %al,(%rsi)
+	test   %r11d,%r11d
+	jne    18f3 <GeneratePermutationTable+0x733>
+	mov    %r9,%rcx
 	add    $0x6,%rsi
-	cmp    %r9,%r10
-	je     1295 <GeneratePermutationTable+0xf5>
-	add    $0x40,%r10
-	cmpb   $0x0,-0x49(%rsp)
+	cmp    %r8,%r9
+	je     12bb <GeneratePermutationTable+0xfb>
+	add    $0x40,%r9
 	movb   $0x0,(%rcx)
-	jle    124c <GeneratePermutationTable+0xac>
+	test   %r13b,%r13b
+	jle    1274 <GeneratePermutationTable+0xb4>
 	cmp    $0x8,%edx
-	jb     1235 <GeneratePermutationTable+0x95>
+	jb     125d <GeneratePermutationTable+0x9d>
 	lea    0x8(%rsi),%rdi
 	mov    %rsi,%rcx
 	mov    %rax,(%rsi)
 	add    $0x6,%rsi
 	and    $0xfffffffffffffff8,%rdi
-	mov    %rax,-0xe(%rsi,%r11,1)
+	mov    %rax,-0xe(%rsi,%r10,1)
 	sub    %rdi,%rcx
 	add    %edx,%ecx
 	shr    $0x3,%ecx
 	rep stos %rax,%es:(%rdi)
-	mov    %r10,%rcx
-	cmp    %r9,%r10
-	jne    1258 <GeneratePermutationTable+0xb8>
-	mov    %r8b,0x47(%rsp)
-	movl   $0x0,0x40(%rsp)
-	movl   $0x1,0x38(%rsp)
-	test   %r8b,%r8b
-	jle    1875 <GeneratePermutationTable+0x6d5>
-	mov    0x40(%rsp),%esi
+	mov    %r9,%rcx
+	cmp    %r8,%r9
+	jne    1280 <GeneratePermutationTable+0xc0>
+	mov    0x60(%rsp),%eax
+	movl   $0x0,0x5c(%rsp)
+	movl   $0x1,0x2c(%rsp)
+	mov    %al,0x67(%rsp)
+	test   %al,%al
+	jle    18ba <GeneratePermutationTable+0x6fa>
+	mov    0x5c(%rsp),%esi
 	mov    $0x1,%eax
-	mov    0x38(%rsp),%ebx
+	mov    0x2c(%rsp),%r15d
 	xor    %edx,%edx
 	mov    %esi,%ecx
+	mov    %esi,%ebx
 	shl    %cl,%eax
 	mov    %eax,%ecx
 	mov    %eax,%edi
-	mov    0x3c(%rsp),%eax
-	div    %ebx
-	movzbl 0x47(%rsp),%edx
+	mov    0x58(%rsp),%eax
+	div    %r15d
+	movzbl 0x67(%rsp),%edx
 	sub    %esi,%edx
 	movsbl %dl,%edx
 	mov    %edx,%esi
-	mov    %edx,-0x14(%rsp)
+	mov    %edx,-0x10(%rsp)
 	xor    %edx,%edx
-	mov    %eax,-0x10(%rsp)
-	mov    -0x10(%rsp),%eax
+	mov    %eax,-0xc(%rsp)
+	mov    -0xc(%rsp),%eax
 	div    %esi
-	test   %ebx,%ebx
-	je     1855 <GeneratePermutationTable+0x6b5>
+	test   %r15d,%r15d
+	je     189b <GeneratePermutationTable+0x6db>
 	movsbl %cl,%edx
-	mov    %ecx,%r14d
-	mov    %cl,-0x58(%rsp)
-	mov    %ecx,%ebx
+	mov    %ecx,%r15d
+	mov    %cl,-0x64(%rsp)
+	mov    %ecx,%ebp
 	lea    0xf(%rdx),%esi
 	cmp    $0x1e,%esi
 	lea    -0x1(%rcx),%esi
-	seta   %r13b
+	seta   %r8b
 	cmp    $0xe,%sil
 	seta   %sil
-	and    $0xfffffff0,%r14d
-	shr    $0x4,%bl
-	lea    0x2(%r14),%r11d
-	and    %esi,%r13d
-	lea    0x1(%r14),%esi
-	mov    %r14b,-0x57(%rsp)
-	mov    %r11b,-0x55(%rsp)
+	and    $0xfffffff0,%r15d
+	shr    $0x4,%bpl
+	lea    0x2(%r15),%r11d
+	and    %esi,%r8d
+	lea    0x1(%r15),%esi
+	mov    %r15b,-0x63(%rsp)
+	mov    %r11b,-0x61(%rsp)
 	movsbl %r11b,%r11d
-	movsbl %r14b,%ecx
-	mov    %r11d,-0x54(%rsp)
-	add    %edx,%r11d
-	lea    (%rcx,%rdx,1),%r8d
+	movsbl %r15b,%ecx
 	mov    %r11d,-0x50(%rsp)
-	lea    0x3(%r14),%r11d
-	mov    %r11b,-0x4a(%rsp)
+	add    %edx,%r11d
+	mov    %r11d,-0x4c(%rsp)
+	lea    0x3(%r15),%r11d
+	mov    %r11b,-0x2c(%rsp)
 	movsbl %r11b,%r11d
 	mov    %r11d,-0x48(%rsp)
 	add    %edx,%r11d
 	mov    %r11d,-0x44(%rsp)
-	lea    0x4(%r14),%r11d
-	mov    %r11b,-0x28(%rsp)
+	lea    0x4(%r15),%r11d
+	mov    %r11b,-0x2b(%rsp)
 	movsbl %r11b,%r11d
 	mov    %r11d,-0x40(%rsp)
 	add    %edx,%r11d
 	mov    %r11d,-0x3c(%rsp)
-	lea    0x5(%r14),%r11d
-	mov    %r11b,-0x27(%rsp)
+	lea    0x5(%r15),%r11d
+	mov    %r11b,-0x2a(%rsp)
 	movsbl %r11b,%r11d
-	mov    %r11d,-0x38(%rsp)
-	add    %edx,%r11d
 	mov    %r11d,-0x34(%rsp)
-	lea    0x6(%r14),%r11d
-	mov    %r11b,-0x26(%rsp)
-	movsbl %r11b,%r11d
-	mov    %r11d,-0x30(%rsp)
 	add    %edx,%r11d
-	mov    %r11d,-0x2c(%rsp)
-	lea    0x7(%r14),%r11d
-	mov    %r11b,-0x25(%rsp)
+	mov    %r11d,-0x30(%rsp)
+	lea    0x6(%r15),%r11d
+	mov    %r11b,-0x29(%rsp)
 	movsbl %r11b,%r11d
-	mov    %r11d,-0x24(%rsp)
+	mov    %r11d,-0x28(%rsp)
 	add    %edx,%r11d
-	mov    %r11d,-0x20(%rsp)
-	lea    0x8(%r14),%r11d
-	mov    %r11b,0xc(%rsp)
+	mov    %r11d,-0x24(%rsp)
+	lea    0x7(%r15),%r11d
+	mov    %r11b,(%rsp)
 	movsbl %r11b,%r11d
-	mov    %r11d,-0x1c(%rsp)
+	mov    %r11d,-0x20(%rsp)
 	add    %edx,%r11d
-	mov    %r11d,-0x18(%rsp)
-	lea    0x9(%r14),%r11d
-	mov    %r11b,0xd(%rsp)
+	mov    %r11d,-0x1c(%rsp)
+	lea    0x8(%r15),%r11d
+	mov    %r11b,0x1(%rsp)
 	movsbl %r11b,%r11d
-	mov    %r11d,-0xc(%rsp)
+	mov    %r11d,-0x18(%rsp)
 	add    %edx,%r11d
-	mov    %r11d,-0x8(%rsp)
-	lea    0xa(%r14),%r11d
-	mov    %r11b,0xe(%rsp)
+	mov    %r11d,-0x14(%rsp)
+	lea    0x9(%r15),%r11d
+	mov    %r11b,0x2(%rsp)
 	movsbl %r11b,%r11d
-	mov    %r11d,0x4(%rsp)
+	mov    %r11d,-0x8(%rsp)
 	add    %edx,%r11d
-	mov    %r11d,0x8(%rsp)
-	lea    0xb(%r14),%r11d
-	mov    %r11b,0xf(%rsp)
+	mov    %r11d,-0x4(%rsp)
+	lea    0xa(%r15),%r11d
+	mov    %r11b,0x3(%rsp)
 	movsbl %r11b,%r11d
 	mov    %r11d,0x10(%rsp)
 	add    %edx,%r11d
-	mov    %sil,-0x56(%rsp)
-	movsbl %sil,%esi
 	mov    %r11d,0x14(%rsp)
-	lea    0xc(%r14),%r11d
-	lea    (%rsi,%rdx,1),%r9d
-	mov    0x2b94(%rip),%rbp        
-	mov    %r11b,0x44(%rsp)
+	lea    0xb(%r15),%r11d
+	mov    %r11b,0x22(%rsp)
 	movsbl %r11b,%r11d
+	mov    %r8b,0x66(%rsp)
+	lea    (%rcx,%rdx,1),%r8d
+	mov    %sil,-0x62(%rsp)
+	movsbl %sil,%esi
 	mov    %r11d,0x18(%rsp)
 	add    %edx,%r11d
+	lea    (%rsi,%rdx,1),%r9d
 	mov    %r11d,0x1c(%rsp)
-	lea    0xd(%r14),%r11d
-	add    $0xe,%r14d
-	mov    %r11b,0x45(%rsp)
-	movsbl %r11b,%r11d
-	mov    %r14b,0x46(%rsp)
-	movsbl %r14b,%r14d
-	mov    %r11d,0x20(%rsp)
+	lea    0xc(%r15),%r11d
+	mov    %r11b,0x23(%rsp)
+	movsbl %r11b,%r11d
+	mov    %r11d,0x24(%rsp)
 	add    %edx,%r11d
-	add    %r14d,%edx
-	mov    %edx,0x2c(%rsp)
+	mov    %r11d,0x28(%rsp)
+	lea    0xd(%r15),%r11d
+	add    $0xe,%r15d
+	mov    %r11b,0x64(%rsp)
+	movsbl %r11b,%r11d
+	mov    %r15b,0x65(%rsp)
+	movsbl %r15b,%r15d
+	mov    %r11d,0x30(%rsp)
+	add    %edx,%r11d
+	add    %r15d,%edx
+	mov    %edx,0x3c(%rsp)
+	movsbq %dil,%rdx
+	mov    %rdx,0x40(%rsp)
 	movslq %r8d,%rdx
-	mov    %rdx,0x30(%rsp)
+	mov    %rdx,0x48(%rsp)
 	movslq %ecx,%rdx
-	mov    %rdx,-0x70(%rsp)
+	mov    %rdx,0x50(%rsp)
 	movslq %r9d,%rdx
-	mov    %rdx,-0x68(%rsp)
-	movslq %esi,%rdx
-	movl   $0x0,-0x4(%rsp)
 	mov    %rdx,-0x60(%rsp)
-	mov    %r11d,0x24(%rsp)
+	movslq %esi,%rdx
+	mov    %r15d,0x38(%rsp)
+	movl   $0x0,-0x38(%rsp)
+	mov    %rdx,-0x58(%rsp)
+	mov    %r11d,0x34(%rsp)
 	xor    %r11d,%r11d
-	mov    %r14d,0x28(%rsp)
-	movsbq %dil,%r14
+	nopl   0x0(%rax)
 	xor    %ecx,%ecx
-	jmp    14dd <GeneratePermutationTable+0x33d>
-	nopl   0x0(%rax,%rax,1)
+	jmp    150c <GeneratePermutationTable+0x34c>
+	nopl   0x0(%rax)
 	add    $0x1,%ecx
-	cmp    %cl,-0x49(%rsp)
-	jle    1842 <GeneratePermutationTable+0x6a2>
+	cmp    %cl,%r13b
+	jle    1888 <GeneratePermutationTable+0x6c8>
 	mov    %r11d,%edx
 	movslq %ecx,%rsi
 	lea    (%rdx,%rdx,2),%rdx
-	lea    0x0(%rbp,%rdx,2),%rdx
-	cmpb   $0x0,(%rdx,%rsi,1)
-	je     14d0 <GeneratePermutationTable+0x330>
-	mov    -0x14(%rsp),%r8d
-	cmp    %r8d,-0x10(%rsp)
-	jb     14d0 <GeneratePermutationTable+0x330>
+	lea    (%r14,%rdx,2),%rdx
+	cmp    %r13b,(%rdx,%rsi,1)
+	jne    1500 <GeneratePermutationTable+0x340>
+	mov    -0x10(%rsp),%r15d
+	cmp    %r15d,-0xc(%rsp)
+	jb     1500 <GeneratePermutationTable+0x340>
 	mov    $0x1,%edx
 	shl    %cl,%edx
 	mov    %edx,%r8d
 	xor    %edx,%edx
-	nopw   0x0(%rax,%rax,1)
+	nopl   0x0(%rax,%rax,1)
 	lea    (%rdx,%r11,1),%r9d
 	add    $0x1,%edx
 	lea    (%r9,%r9,2),%r9
-	lea    0x0(%rbp,%r9,2),%r9
-	movb   $0x0,(%r9,%rsi,1)
+	lea    (%r14,%r9,2),%r9
+	mov    %bl,(%r9,%rsi,1)
 	cmp    %edx,%eax
-	ja     1510 <GeneratePermutationTable+0x370>
+	ja     1540 <GeneratePermutationTable+0x380>
 	movd   %r8d,%xmm0
-	mov    0x30(%rsp),%rdx
-	mov    %ecx,(%rsp)
+	mov    0x48(%rsp),%rdx
+	mov    %bl,0x20(%rsp)
 	xor    %r9d,%r9d
 	punpcklbw %xmm0,%xmm0
+	mov    %r13b,0x21(%rsp)
+	movzbl 0x66(%rsp),%r15d
 	punpcklwd %xmm0,%xmm0
-	mov    %rdx,-0x78(%rsp)
+	mov    %r14,0x8(%rsp)
+	mov    0x40(%rsp),%r13
+	mov    %ecx,0x4(%rsp)
+	mov    0x50(%rsp),%r14
 	pshufd $0x0,%xmm0,%xmm0
-	jmp    17b9 <GeneratePermutationTable+0x619>
-	mov    0x2a51(%rip),%r10        
+	mov    %rdx,-0x70(%rsp)
+	jmp    17e9 <GeneratePermutationTable+0x629>
+	nopl   (%rax)
+	mov    0x29f9(%rip),%r10        
 	mov    %rdx,%rsi
 	shl    $0x6,%rsi
-	lea    (%r10,%rsi,1),%r12
-	add    %r14,%rsi
-	movdqa (%r12),%xmm1
+	lea    (%r10,%rsi,1),%rbx
+	add    %r13,%rsi
+	movdqa (%rbx),%xmm1
 	add    %r10,%rsi
 	paddb  %xmm0,%xmm1
 	movups %xmm1,(%rsi)
-	cmp    $0x1,%bl
-	jbe    15b1 <GeneratePermutationTable+0x411>
-	movdqa 0x10(%r12),%xmm1
+	cmp    $0x1,%bpl
+	jbe    15fc <GeneratePermutationTable+0x43c>
+	movdqa 0x10(%rbx),%xmm1
 	paddb  %xmm0,%xmm1
 	movups %xmm1,0x10(%rsi)
-	cmp    $0x2,%bl
-	je     15b1 <GeneratePermutationTable+0x411>
-	movdqa 0x20(%r12),%xmm1
+	cmp    $0x2,%bpl
+	je     15fc <GeneratePermutationTable+0x43c>
+	movdqa 0x20(%rbx),%xmm1
 	paddb  %xmm0,%xmm1
 	movups %xmm1,0x20(%rsi)
-	cmp    $0x3,%bl
-	je     15b1 <GeneratePermutationTable+0x411>
-	movdqa 0x30(%r12),%xmm1
+	cmp    $0x3,%bpl
+	je     15fc <GeneratePermutationTable+0x43c>
+	movdqa 0x30(%rbx),%xmm1
 	paddb  %xmm0,%xmm1
 	movups %xmm1,0x30(%rsi)
-	movzbl -0x57(%rsp),%esi
-	cmp    %sil,-0x58(%rsp)
-	je     17b0 <GeneratePermutationTable+0x610>
+	movzbl -0x63(%rsp),%ebx
+	cmp    %bl,-0x64(%rsp)
+	je     17e0 <GeneratePermutationTable+0x620>
 	mov    %rdx,%rsi
 	mov    -0x70(%rsp),%rcx
 	shl    $0x6,%rsi
 	add    %r10,%rsi
-	movzbl (%rsi,%rcx,1),%r12d
-	mov    -0x78(%rsp),%rcx
-	add    %r8d,%r12d
-	mov    %r12b,(%rsi,%rcx,1)
-	cmp    -0x56(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
+	movzbl (%rsi,%r14,1),%ebx
+	add    %r8d,%ebx
+	mov    %bl,(%rsi,%rcx,1)
+	cmp    -0x62(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	mov    -0x58(%rsp),%rcx
+	movzbl (%rsi,%rcx,1),%ebx
 	mov    -0x60(%rsp),%rcx
-	movzbl (%rsi,%rcx,1),%r12d
-	mov    -0x68(%rsp),%rcx
-	add    %r8d,%r12d
-	mov    %r12b,(%rsi,%rcx,1)
-	cmp    -0x55(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x54(%rsp),%r15
+	add    %r8d,%ebx
+	mov    %bl,(%rsi,%rcx,1)
+	cmp    -0x61(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq -0x50(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
+	movslq -0x4c(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
 	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    -0x4a(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x48(%rsp),%r15
-	movslq -0x44(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
-	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    -0x28(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x40(%rsp),%r15
-	movslq -0x3c(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
-	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    -0x27(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x38(%rsp),%r15
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    -0x2c(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq -0x48(%rsp),%r12
+	movslq -0x44(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
+	add    %r8d,%ecx
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    -0x2b(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq -0x40(%rsp),%r12
+	movslq -0x3c(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
+	add    %r8d,%ecx
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    -0x2a(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq -0x34(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
+	movslq -0x30(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
 	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    -0x26(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x30(%rsp),%r15
-	movslq -0x2c(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
-	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    -0x25(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x24(%rsp),%r15
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    -0x29(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq -0x28(%rsp),%r12
+	movslq -0x24(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
+	add    %r8d,%ecx
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    (%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq -0x20(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
+	movslq -0x1c(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
 	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    0xc(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq -0x1c(%rsp),%r15
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    0x1(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq -0x18(%rsp),%r12
-	movzbl (%rsi,%r15,1),%ecx
+	movslq -0x14(%rsp),%rbx
+	movzbl (%rsi,%r12,1),%ecx
 	add    %r8d,%ecx
-	mov    %cl,(%rsi,%r12,1)
-	cmp    0xd(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
+	mov    %cl,(%rsi,%rbx,1)
+	cmp    0x2(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	shl    $0x6,%rdx
-	movslq -0x8(%rsp),%rsi
+	movslq -0x4(%rsp),%rsi
 	add    %rdx,%r10
-	movslq -0xc(%rsp),%rdx
-	movzbl (%r10,%rdx,1),%ecx
-	add    %r8d,%ecx
-	mov    %cl,(%r10,%rsi,1)
-	cmp    0xe(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq 0x4(%rsp),%rsi
-	movslq 0x8(%rsp),%rdx
-	movzbl (%r10,%rsi,1),%ecx
-	add    %r8d,%ecx
-	mov    %cl,(%r10,%rdx,1)
-	cmp    0xf(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
+	movslq -0x8(%rsp),%rdx
+	movzbl (%r10,%rdx,1),%ebx
+	add    %r8d,%ebx
+	mov    %bl,(%r10,%rsi,1)
+	cmp    0x3(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq 0x10(%rsp),%rsi
 	movslq 0x14(%rsp),%rdx
 	movzbl (%r10,%rsi,1),%ecx
 	add    %r8d,%ecx
 	mov    %cl,(%r10,%rdx,1)
-	cmp    0x44(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
+	cmp    0x22(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
 	movslq 0x18(%rsp),%rsi
 	movslq 0x1c(%rsp),%rdx
 	movzbl (%r10,%rsi,1),%ecx
 	add    %r8d,%ecx
 	mov    %cl,(%r10,%rdx,1)
-	cmp    0x45(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq 0x20(%rsp),%rsi
-	movslq 0x24(%rsp),%rdx
+	cmp    0x23(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq 0x24(%rsp),%rsi
+	movslq 0x28(%rsp),%rdx
 	movzbl (%r10,%rsi,1),%ecx
 	add    %r8d,%ecx
 	mov    %cl,(%r10,%rdx,1)
-	cmp    0x46(%rsp),%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	movslq 0x28(%rsp),%rsi
-	movslq 0x2c(%rsp),%rdx
+	cmp    0x64(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq 0x30(%rsp),%rsi
+	movslq 0x34(%rsp),%rdx
+	movzbl (%r10,%rsi,1),%ecx
+	add    %r8d,%ecx
+	mov    %cl,(%r10,%rdx,1)
+	cmp    0x65(%rsp),%dil
+	jle    17e0 <GeneratePermutationTable+0x620>
+	movslq 0x38(%rsp),%rsi
+	movslq 0x3c(%rsp),%rdx
 	movzbl (%r10,%rsi,1),%ecx
 	add    %r8d,%ecx
 	mov    %cl,(%r10,%rdx,1)
-	cs nopw 0x0(%rax,%rax,1)
 	add    $0x1,%r9d
 	cmp    %r9d,%eax
-	jbe    1818 <GeneratePermutationTable+0x678>
+	jbe    1848 <GeneratePermutationTable+0x688>
 	lea    (%r11,%r9,1),%edx
 	test   %dil,%dil
-	jle    17b0 <GeneratePermutationTable+0x610>
-	test   %r13b,%r13b
-	jne    1550 <GeneratePermutationTable+0x3b0>
-	mov    0x27d6(%rip),%rsi        
+	jle    17e0 <GeneratePermutationTable+0x620>
+	test   %r15b,%r15b
+	jne    15a0 <GeneratePermutationTable+0x3e0>
+	mov    0x279e(%rip),%rsi        
 	shl    $0x6,%rdx
-	mov    -0x78(%rsp),%rcx
-	lea    (%rdx,%rsi,1),%r12
-	add    %r14,%rdx
+	mov    -0x70(%rsp),%rcx
+	lea    (%rdx,%rsi,1),%rbx
+	add    %r13,%rdx
 	add    %rsi,%rdx
 	xor    %esi,%esi
 	nopw   0x0(%rax,%rax,1)
-	movzbl (%r12,%rsi,1),%r10d
+	movzbl (%rbx,%rsi,1),%r10d
 	add    %r8d,%r10d
 	mov    %r10b,(%rdx,%rsi,1)
 	add    $0x1,%rsi
 	cmp    %sil,%dil
-	jg     17f0 <GeneratePermutationTable+0x650>
+	jg     1820 <GeneratePermutationTable+0x660>
 	add    $0x1,%r9d
-	mov    %rcx,-0x78(%rsp)
+	mov    %rcx,-0x70(%rsp)
 	cmp    %r9d,%eax
-	ja     17b9 <GeneratePermutationTable+0x619>
+	ja     17e9 <GeneratePermutationTable+0x629>
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x14(%rsp),%r8d
+	mov    0x4(%rsp),%ecx
+	mov    -0x10(%rsp),%r15d
 	lea    -0x1(%rax),%edx
 	mov    $0x0,%esi
-	mov    (%rsp),%ecx
-	cmp    %r8d,-0x10(%rsp)
+	cmp    %r15d,-0xc(%rsp)
+	movzbl 0x21(%rsp),%r13d
 	cmovb  %esi,%edx
 	add    $0x1,%ecx
+	movzbl 0x20(%rsp),%ebx
+	mov    0x8(%rsp),%r14
 	lea    0x1(%r11,%rdx,1),%r11d
-	cmp    %cl,-0x49(%rsp)
-	jg     14dd <GeneratePermutationTable+0x33d>
-	addl   $0x1,-0x4(%rsp)
-	mov    -0x4(%rsp),%edx
-	cmp    0x38(%rsp),%edx
-	jne    14c4 <GeneratePermutationTable+0x324>
-	mov    0x38(%rsp),%eax
-	imul   -0x14(%rsp),%eax
-	addl   $0x1,0x40(%rsp)
-	mov    %eax,0x38(%rsp)
-	mov    0x40(%rsp),%eax
-	cmp    %al,-0x49(%rsp)
-	jg     12b3 <GeneratePermutationTable+0x113>
-	add    $0x50,%rsp
+	cmp    %cl,%r13b
+	jg     150c <GeneratePermutationTable+0x34c>
+	nopw   0x0(%rax,%rax,1)
+	addl   $0x1,-0x38(%rsp)
+	mov    -0x38(%rsp),%edx
+	cmp    0x2c(%rsp),%edx
+	jne    14f8 <GeneratePermutationTable+0x338>
+	mov    0x2c(%rsp),%eax
+	imul   -0x10(%rsp),%eax
+	addl   $0x1,0x5c(%rsp)
+	mov    %eax,0x2c(%rsp)
+	mov    0x5c(%rsp),%eax
+	cmp    %al,%r13b
+	jg     12db <GeneratePermutationTable+0x11b>
+	mov    0x271f(%rip),%rax        
+	movzbl 0x60(%rsp),%edi
+	mov    %dil,(%rax)
+	add    $0x70,%rsp
+	mov    %r14,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	movl   $0x1010101,(%rsi)
-	movl   $0x1010101,-0x4(%rsi,%r11,1)
-	jmp    124c <GeneratePermutationTable+0xac>
-	mov    $0x101,%ecx
-	mov    %cx,-0x2(%rsi,%r11,1)
-	jmp    124c <GeneratePermutationTable+0xac>
-	nopl   0x0(%rax,%rax,1)
+	mov    %eax,(%rsi)
+	mov    %eax,-0x4(%rsi,%r10,1)
+	jmp    1274 <GeneratePermutationTable+0xb4>
+	mov    0x26ea(%rip),%r14        
+	jmp    12bb <GeneratePermutationTable+0xfb>
+	mov    %ax,-0x2(%rsi,%r10,1)
+	jmp    1274 <GeneratePermutationTable+0xb4>
+	xchg   %ax,%ax
 
-00000000000018b0 <NpCanonicalRepresentative>:
+0000000000001900 <NpCanonicalRepresentative>:
 NpCanonicalRepresentative():
 	endbr64
-	movsbl %sil,%ecx
 	push   %r15
 	mov    %rdi,%r10
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
+	mov    %rcx,-0x8(%rsp)
+	movsbl %sil,%ecx
+	mov    %rdx,-0x10(%rsp)
 	cmp    $0x1,%ecx
-	jbe    1bcb <NpCanonicalRepresentative+0x31b>
+	jbe    1c3b <NpCanonicalRepresentative+0x33b>
 	mov    %ecx,%edx
 	mov    $0x1,%eax
-	nopl   (%rax)
+	nop
 	imul   %eax,%edx
 	add    $0x1,%eax
 	cmp    %eax,%ecx
-	jne    18d8 <NpCanonicalRepresentative+0x28>
-	mov    %edx,-0x8(%rsp)
+	jne    1930 <NpCanonicalRepresentative+0x30>
+	mov    %edx,-0x18(%rsp)
 	mov    $0x1,%eax
 	shl    %cl,%eax
-	mov    %eax,-0x4(%rsp)
+	mov    %eax,-0x14(%rsp)
 	mov    %eax,%ecx
 	test   %eax,%eax
-	je     1b17 <NpCanonicalRepresentative+0x267>
+	je     1b77 <NpCanonicalRepresentative+0x277>
 	xor    %eax,%eax
-	jmp    190e <NpCanonicalRepresentative+0x5e>
-	nop
+	jmp    196e <NpCanonicalRepresentative+0x6e>
+	nopw   0x0(%rax,%rax,1)
 	add    $0x1,%eax
 	movsbl %al,%edx
 	cmp    %ecx,%edx
-	jae    1b17 <NpCanonicalRepresentative+0x267>
+	jae    1b77 <NpCanonicalRepresentative+0x277>
 	movsbq %al,%rdx
 	movzbl (%r10,%rdx,1),%edx
 	test   %dl,%dl
-	je     1900 <NpCanonicalRepresentative+0x50>
-	mov    %dl,-0x16(%rsp)
-	mov    0x26c2(%rip),%rcx        
+	je     1960 <NpCanonicalRepresentative+0x60>
+	mov    %dl,-0x26(%rsp)
+	mov    0x2672(%rip),%r8        
 	xor    %eax,%eax
 	xor    %edi,%edi
-	mov    0x26c7(%rip),%r8        
-	mov    -0x4(%rsp),%r9d
+	mov    0x2657(%rip),%rdx        
+	mov    -0x14(%rsp),%r9d
 	cs nopw 0x0(%rax,%rax,1)
-	movsbq %al,%rdx
-	cmpb   $0x0,(%r10,%rdx,1)
-	je     195b <NpCanonicalRepresentative+0xab>
-	mov    %edi,%edx
+	movsbq %al,%rcx
+	cmpb   $0x0,(%r10,%rcx,1)
+	je     19bb <NpCanonicalRepresentative+0xbb>
+	mov    %edi,%ecx
 	add    $0x1,%edi
-	mov    %al,(%rcx,%rdx,1)
-	movl   $0x0,(%r8,%rdx,4)
+	mov    %al,(%rdx,%rcx,1)
+	movl   $0x0,(%r8,%rcx,4)
 	add    $0x1,%eax
-	movsbl %al,%edx
-	cmp    %r9d,%edx
-	jb     1940 <NpCanonicalRepresentative+0x90>
+	movsbl %al,%ecx
+	cmp    %r9d,%ecx
+	jb     19a0 <NpCanonicalRepresentative+0xa0>
 	test   %sil,%sil
-	jle    1bd4 <NpCanonicalRepresentative+0x324>
+	jle    1c44 <NpCanonicalRepresentative+0x344>
 	lea    -0x1(%rsi),%eax
 	mov    %r8,%r15
-	mov    0x2634(%rip),%r9        
-	mov    %rcx,%r13
-	mov    %al,-0x15(%rsp)
-	mov    0x2666(%rip),%r8        
-	movl   $0x0,-0x10(%rsp)
-	mov    0x260f(%rip),%r14        
-	movl   $0x1,-0x14(%rsp)
+	mov    0x25cc(%rip),%r9        
+	mov    %rdx,%r14
+	mov    %al,-0x25(%rsp)
+	mov    0x2606(%rip),%r8        
+	movl   $0x0,-0x20(%rsp)
+	mov    0x25a7(%rip),%rbx        
+	movl   $0x1,-0x24(%rsp)
 	nopl   0x0(%rax)
-	movzbl -0x10(%rsp),%ecx
+	movzbl -0x20(%rsp),%ecx
+	movzbl -0x25(%rsp),%esi
 	mov    $0x1,%eax
 	xor    %edx,%edx
 	shl    %cl,%eax
-	movzbl -0x15(%rsp),%ecx
-	mov    %eax,-0x24(%rsp)
-	lea    0x1(%rcx),%eax
-	movzbl %al,%ebx
-	mov    -0x8(%rsp),%eax
-	mov    %ebx,-0xc(%rsp)
-	divl   -0x14(%rsp)
+	mov    %eax,-0x34(%rsp)
+	lea    0x1(%rsi),%eax
+	movzbl %al,%ecx
+	mov    -0x18(%rsp),%eax
+	mov    %ecx,-0x1c(%rsp)
+	divl   -0x24(%rsp)
 	xor    %edx,%edx
-	div    %ebx
+	div    %ecx
 	test   %edi,%edi
-	je     1a40 <NpCanonicalRepresentative+0x190>
+	je     1aa1 <NpCanonicalRepresentative+0x1a1>
 	lea    -0x1(%rdi),%edx
-	movzbl %cl,%r12d
-	mov    %r13,-0x20(%rsp)
-	mov    %r13,%rbp
-	lea    0x4(%r15,%rdx,4),%rsi
-	mov    %r15,%rbx
+	movzbl %sil,%r13d
+	mov    %r14,-0x30(%rsp)
+	mov    %r14,%r12
+	lea    0x4(%r15,%rdx,4),%rcx
+	mov    %r15,%rbp
 	xor    %edi,%edi
-	add    $0x1,%r12d
-	mov    %rsi,%r13
+	add    $0x1,%r13d
+	mov    %rcx,%r14
 	nopl   0x0(%rax)
 	mov    %edi,%edx
 	xor    %ecx,%ecx
-	add    %r12d,%edi
+	add    %r13d,%edi
 	nopw   0x0(%rax,%rax,1)
-	movzbl 0x0(%rbp),%r11d
+	movzbl (%r12),%r11d
 	mov    %edx,%esi
 	add    $0x1,%edx
 	mov    %r11b,(%r8,%rsi,1)
-	mov    (%rbx),%r11d
+	mov    0x0(%rbp),%r11d
 	add    %ecx,%r11d
 	add    %eax,%ecx
 	mov    %r11d,(%r9,%rsi,4)
 	cmp    %edi,%edx
-	jne    1a10 <NpCanonicalRepresentative+0x160>
-	add    $0x4,%rbx
-	add    $0x1,%rbp
-	cmp    %rbx,%r13
-	jne    1a00 <NpCanonicalRepresentative+0x150>
-	mov    -0x20(%rsp),%r13
-	cmpb   $0x0,-0x24(%rsp)
-	jle    1b28 <NpCanonicalRepresentative+0x278>
-	mov    -0x24(%rsp),%eax
+	jne    1a70 <NpCanonicalRepresentative+0x170>
+	add    $0x4,%rbp
+	add    $0x1,%r12
+	cmp    %rbp,%r14
+	jne    1a60 <NpCanonicalRepresentative+0x160>
+	mov    -0x30(%rsp),%r14
+	cmpb   $0x0,-0x34(%rsp)
+	jle    1b88 <NpCanonicalRepresentative+0x288>
+	mov    -0x34(%rsp),%eax
 	movsbq %al,%r11
 	sub    $0x1,%eax
-	lea    0x1(%r11),%ebx
+	lea    0x1(%r11),%ecx
 	movzbl %al,%eax
-	add    %ebx,%eax
-	mov    %ebx,-0x24(%rsp)
-	mov    %eax,-0x20(%rsp)
-	nopw   0x0(%rax,%rax,1)
+	add    %ecx,%eax
+	mov    %ecx,-0x34(%rsp)
+	mov    %eax,-0x30(%rsp)
+	nopl   0x0(%rax,%rax,1)
 	test   %edi,%edi
-	je     1ae8 <NpCanonicalRepresentative+0x238>
-	lea    -0x1(%rdi),%ebx
-	movzbl -0x16(%rsp),%esi
+	je     1b48 <NpCanonicalRepresentative+0x248>
+	lea    -0x1(%rdi),%ebp
+	movzbl -0x26(%rsp),%esi
 	xor    %eax,%eax
 	xor    %edi,%edi
-	jmp    1aa7 <NpCanonicalRepresentative+0x1f7>
+	jmp    1b07 <NpCanonicalRepresentative+0x207>
 	nopw   0x0(%rax,%rax,1)
 	mov    %r15,%rdx
-	mov    %r13,%r12
+	mov    %r14,%r13
 	mov    $0x1,%edi
 	xor    %esi,%esi
 	mov    %ecx,(%rdx)
 	lea    0x1(%rax),%rdx
-	mov    %bpl,(%r12)
-	cmp    %rax,%rbx
-	je     1ae8 <NpCanonicalRepresentative+0x238>
+	mov    %r12b,0x0(%r13)
+	cmp    %rax,%rbp
+	je     1b48 <NpCanonicalRepresentative+0x248>
 	mov    %rdx,%rax
 	mov    (%r9,%rax,4),%edx
-	movzbl (%r8,%rax,1),%ebp
+	movzbl (%r8,%rax,1),%r12d
 	mov    %rdx,%rcx
 	shl    $0x6,%rdx
-	add    %r14,%rdx
-	movzbl (%rdx,%r11,1),%r12d
-	xor    %ebp,%r12d
-	movsbq %r12b,%rdx
+	add    %rbx,%rdx
+	movzbl (%rdx,%r11,1),%r13d
+	xor    %r12d,%r13d
+	movsbq %r13b,%rdx
 	movzbl (%r10,%rdx,1),%edx
 	test   %dl,%dl
-	je     1ad4 <NpCanonicalRepresentative+0x224>
+	je     1b34 <NpCanonicalRepresentative+0x234>
 	test   %sil,%sil
-	jne    1a88 <NpCanonicalRepresentative+0x1d8>
+	jne    1ae8 <NpCanonicalRepresentative+0x1e8>
 	or     %sil,%dl
-	jne    1be3 <NpCanonicalRepresentative+0x333>
+	jne    1c56 <NpCanonicalRepresentative+0x356>
 	xor    %esi,%esi
 	lea    0x1(%rax),%rdx
-	cmp    %rax,%rbx
-	jne    1aa4 <NpCanonicalRepresentative+0x1f4>
-	mov    -0x24(%rsp),%eax
+	cmp    %rax,%rbp
+	jne    1b04 <NpCanonicalRepresentative+0x204>
+	mov    -0x34(%rsp),%eax
 	movslq %eax,%r11
-	cmp    %eax,-0x20(%rsp)
-	je     1b40 <NpCanonicalRepresentative+0x290>
+	cmp    %eax,-0x30(%rsp)
+	je     1ba0 <NpCanonicalRepresentative+0x2a0>
 	mov    %r9,%rax
 	mov    %r15,%r9
 	mov    %rax,%r15
 	mov    %r8,%rax
-	mov    %r13,%r8
-	mov    %rax,%r13
-	mov    -0x24(%rsp),%eax
+	mov    %r14,%r8
+	mov    %rax,%r14
+	mov    -0x34(%rsp),%eax
 	add    $0x1,%eax
-	mov    %eax,-0x24(%rsp)
-	jmp    1a70 <NpCanonicalRepresentative+0x1c0>
+	mov    %eax,-0x34(%rsp)
+	jmp    1ad0 <NpCanonicalRepresentative+0x1d0>
 	xor    %r8d,%r8d
 	pop    %rbx
 	pop    %rbp
 	mov    %r8,%rax
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	mov    %r15,%rax
 	mov    %r9,%r15
 	mov    %rax,%r9
-	mov    %r13,%rax
-	mov    %r8,%r13
+	mov    %r14,%rax
+	mov    %r8,%r14
 	mov    %rax,%r8
 	nopw   0x0(%rax,%rax,1)
-	mov    -0x14(%rsp),%eax
-	imul   -0xc(%rsp),%eax
-	subb   $0x1,-0x15(%rsp)
-	addl   $0x1,-0x10(%rsp)
-	mov    %eax,-0x14(%rsp)
-	movzbl -0x15(%rsp),%eax
+	mov    -0x24(%rsp),%eax
+	imul   -0x1c(%rsp),%eax
+	subb   $0x1,-0x25(%rsp)
+	addl   $0x1,-0x20(%rsp)
+	mov    %eax,-0x24(%rsp)
+	movzbl -0x25(%rsp),%eax
 	cmp    $0xff,%al
-	jne    19a8 <NpCanonicalRepresentative+0xf8>
-	mov    %r13,%rbx
-	mov    (%r15),%r9d
-	movzbl (%rbx),%edi
+	jne    1a08 <NpCanonicalRepresentative+0x108>
+	mov    (%r15),%edi
+	movzbl (%r14),%r9d
 	xor    %esi,%esi
 	xor    %r8d,%r8d
-	mov    -0x4(%rsp),%ebx
+	mov    -0x14(%rsp),%ebp
 	xor    %edx,%edx
 	xor    %eax,%eax
-	mov    $0x1,%r11d
-	shl    $0x6,%r9
-	add    %r14,%r9
+	mov    %rdi,%r11
+	shl    $0x6,%rdi
+	add    %rbx,%rdi
+	mov    $0x1,%ebx
 	nopw   0x0(%rax,%rax,1)
-	movzbl (%r9,%rax,1),%ecx
-	xor    %edi,%ecx
+	movzbl (%rdi,%rax,1),%ecx
+	xor    %r9d,%ecx
 	movsbq %cl,%rax
 	cmpb   $0x0,(%r10,%rax,1)
-	je     1bb0 <NpCanonicalRepresentative+0x300>
+	je     1c10 <NpCanonicalRepresentative+0x310>
 	not    %edx
-	mov    %r11,%rax
-	lea    (%rdx,%rbx,1),%ecx
+	mov    %rbx,%rax
+	lea    (%rdx,%rbp,1),%ecx
 	shl    %cl,%rax
 	add    %rax,%r8
 	add    $0x1,%esi
 	movsbq %sil,%rax
 	mov    %eax,%edx
-	cmp    %eax,%ebx
-	ja     1b90 <NpCanonicalRepresentative+0x2e0>
-	pop    %rbx
+	cmp    %eax,%ebp
+	ja     1bf0 <NpCanonicalRepresentative+0x2f0>
+	mov    -0x10(%rsp),%rax
+	mov    %r9b,(%rax)
+	mov    -0x8(%rsp),%rax
+	mov    %r11d,(%rax)
 	mov    %r8,%rax
+	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	mov    %ecx,-0x8(%rsp)
-	jmp    18e6 <NpCanonicalRepresentative+0x36>
-	mov    0x23cd(%rip),%r14        
+	mov    %ecx,-0x18(%rsp)
+	jmp    193e <NpCanonicalRepresentative+0x3e>
+	mov    0x2355(%rip),%rbx        
 	mov    %r8,%r15
-	mov    %rcx,%rbx
-	jmp    1b67 <NpCanonicalRepresentative+0x2b7>
+	mov    %rdx,%r14
+	jmp    1bc4 <NpCanonicalRepresentative+0x2c4>
 	mov    %edi,%edx
 	add    $0x1,%edi
-	lea    0x0(%r13,%rdx,1),%r12
+	lea    (%r14,%rdx,1),%r13
 	lea    (%r15,%rdx,4),%rdx
-	jmp    1a95 <NpCanonicalRepresentative+0x1e5>
-	cs nopw 0x0(%rax,%rax,1)
+	jmp    1af5 <NpCanonicalRepresentative+0x1f5>
+	nopl   0x0(%rax,%rax,1)
 
-0000000000001c00 <NpnCanonicalRepresentative>:
+0000000000001c70 <NpnCanonicalRepresentative>:
 NpnCanonicalRepresentative():
 	endbr64
+	push   %r15
+	push   %r14
+	mov    $0x1,%r14d
 	push   %r13
-	movsbl %sil,%r13d
+	mov    %r8,%r13
 	push   %r12
-	mov    %r13d,%esi
+	mov    %rcx,%r12
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
-	mov    $0x1,%ebx
-	sub    $0x8,%rsp
-	call   1090 <NpCanonicalRepresentative@plt>
-	mov    %r13d,%ecx
-	shl    %cl,%ebx
-	mov    %rax,%r12
-	test   %ebx,%ebx
-	jle    1c78 <NpnCanonicalRepresentative+0x78>
+	mov    %rdx,%rbx
+	sub    $0x38,%rsp
+	mov    %fs:0x28,%rax
+	mov    %rax,0x28(%rsp)
+	xor    %eax,%eax
+	mov    0x2335(%rip),%rax        
+	lea    0x20(%rsp),%rcx
+	lea    0x1e(%rsp),%rdx
+	mov    %sil,(%rax)
+	movsbl %sil,%esi
+	mov    %esi,0xc(%rsp)
+	call   10a0 <NpCanonicalRepresentative@plt>
+	mov    0xc(%rsp),%esi
+	mov    %rax,%r15
+	mov    %esi,%ecx
+	shl    %cl,%r14d
+	test   %r14d,%r14d
+	jle    1d80 <NpnCanonicalRepresentative+0x110>
 	xor    %eax,%eax
+	nopl   0x0(%rax)
 	movsbq %al,%rdx
 	add    $0x1,%eax
 	xorb   $0x1,0x0(%rbp,%rdx,1)
 	movsbl %al,%edx
-	cmp    %ebx,%edx
-	jl     1c30 <NpnCanonicalRepresentative+0x30>
-	mov    %r13d,%esi
+	cmp    %r14d,%edx
+	jl     1ce0 <NpnCanonicalRepresentative+0x70>
+	lea    0x1f(%rsp),%rdx
+	lea    0x24(%rsp),%rcx
 	mov    %rbp,%rdi
-	call   1090 <NpCanonicalRepresentative@plt>
+	call   10a0 <NpCanonicalRepresentative@plt>
 	xor    %edx,%edx
+	nopl   0x0(%rax,%rax,1)
 	movsbq %dl,%rcx
 	add    $0x1,%edx
 	xorb   $0x1,0x0(%rbp,%rcx,1)
 	movsbl %dl,%ecx
-	cmp    %ebx,%ecx
-	jl     1c50 <NpnCanonicalRepresentative+0x50>
-	cmp    %rax,%r12
-	cmovae %r12,%rax
-	add    $0x8,%rsp
+	cmp    %r14d,%ecx
+	jl     1d10 <NpnCanonicalRepresentative+0xa0>
+	cmp    %rax,%r15
+	jbe    1d60 <NpnCanonicalRepresentative+0xf0>
+	movzbl 0x1e(%rsp),%eax
+	mov    %al,(%rbx)
+	mov    0x20(%rsp),%eax
+	mov    %eax,(%r12)
+	mov    %r15,%rax
+	movb   $0x0,0x0(%r13)
+	mov    0x28(%rsp),%rbx
+	xor    %fs:0x28,%rbx
+	jne    1d94 <NpnCanonicalRepresentative+0x124>
+	add    $0x38,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
+	pop    %r14
+	pop    %r15
 	ret
-	nopl   (%rax)
-	mov    %r13d,%esi
+	nop
+	movzbl 0x1f(%rsp),%edx
+	mov    %dl,(%rbx)
+	mov    0x24(%rsp),%edx
+	mov    %edx,(%r12)
+	movb   $0x1,0x0(%r13)
+	jmp    1d40 <NpnCanonicalRepresentative+0xd0>
+	cs nopw 0x0(%rax,%rax,1)
+	lea    0x24(%rsp),%rcx
+	lea    0x1f(%rsp),%rdx
 	mov    %rbp,%rdi
-	call   1090 <NpCanonicalRepresentative@plt>
-	jmp    1c63 <NpnCanonicalRepresentative+0x63>
+	call   10a0 <NpCanonicalRepresentative@plt>
+	jmp    1d24 <NpnCanonicalRepresentative+0xb4>
+	call   10b0 <__stack_chk_fail@plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001c88 <_fini>:
+0000000000001d9c <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,8 +1,8 @@
 
 Hex dump of section '.eh_frame_hdr':
   0x00002000 011b033b 44000000 07000000 20f0ffff ...;D....... ...
-  0x00002010 60000000 60f0ffff 88000000 70f0ffff `...`.......p...
-  0x00002020 a0000000 a0f0ffff a0010000 a0f1ffff ................
-  0x00002030 b8000000 b0f8ffff 08010000 00fcffff ................
+  0x00002010 60000000 70f0ffff 88000000 80f0ffff `...p...........
+  0x00002020 a0000000 c0f0ffff b0010000 c0f1ffff ................
+  0x00002030 b8000000 00f9ffff 08010000 70fcffff ............p...
   0x00002040 64010000                            d...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,27 +1,28 @@
 
 Hex dump of section '.eh_frame':
   0x00002048 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00002058 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00002068 b8efffff 40000000 000e1046 0e184a0f ....@......F..J.
+  0x00002068 b8efffff 50000000 000e1046 0e184a0f ....P......F..J.
   0x00002078 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x00002088 14000000 44000000 d0efffff 10000000 ....D...........
+  0x00002088 14000000 44000000 e0efffff 10000000 ....D...........
   0x00002098 00000000 00000000 14000000 5c000000 ............\...
-  0x000020a8 c8efffff 30000000 00000000 00000000 ....0...........
-  0x000020b8 4c000000 74000000 e0f0ffff 08070000 L...t...........
-  0x000020c8 00460e10 8f02490e 188e0344 0e208d04 .F....I....D. ..
-  0x000020d8 420e288c 05410e30 8606410e 38830748 B.(..A.0..A.8..H
-  0x000020e8 0e880103 ba060a0e 38410e30 410e2842 ........8A.0A.(B
+  0x000020a8 d8efffff 40000000 00000000 00000000 ....@...........
+  0x000020b8 4c000000 74000000 00f1ffff 3e070000 L...t.......>...
+  0x000020c8 00460e10 8f02460e 188e0344 0e208d04 .F....F....D. ..
+  0x000020d8 450e288c 05410e30 8606410e 38830744 E.(..A.0..A.8..D
+  0x000020e8 0ea80103 f2060a0e 38440e30 410e2842 ........8D.0A.(B
   0x000020f8 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x00002108 58000000 c4000000 a0f7ffff 46030000 X...........F...
-  0x00002118 004a0e10 8f02450e 188e0342 0e208d04 .J....E....B. ..
+  0x00002108 58000000 c4000000 f0f7ffff 68030000 X...........h...
+  0x00002118 00460e10 8f02450e 188e0342 0e208d04 .F....E....B. ..
   0x00002128 420e288c 05410e30 8606410e 38830703 B.(..A.0..A.8...
-  0x00002138 56020a0e 30410e28 450e2042 0e18420e V...0A.(E. B..B.
-  0x00002148 10420e08 410b0296 0a0e3044 0e28420e .B..A.....0D.(B.
-  0x00002158 20420e18 420e1042 0e08410b 38000000  B..B..B..A.8...
-  0x00002168 20010000 94faffff 85000000 00460e10  ............F..
-  0x00002178 8d02460e 188c0344 0e208604 440e2883 ..F....D. ..D.(.
-  0x00002188 05490e30 02510a0e 28410e20 410e1842 .I.0.Q..(A. A..B
-  0x00002198 0e10420e 08440b00 14000000 5c010000 ..B..D......\...
-  0x000021a8 f8eeffff 32000000 00480e10 570e0800 ....2....H..W...
-  0x000021b8 00000000                            ....
+  0x00002138 6a020a0e 30410e28 450e2042 0e18420e j...0A.(E. B..B.
+  0x00002148 10420e08 410b02a9 0a0e3041 0e28420e .B..A.....0A.(B.
+  0x00002158 20420e18 420e1042 0e08410b 48000000  B..B..B..A.H...
+  0x00002168 20010000 04fbffff 29010000 00460e10  .......)....F..
+  0x00002178 8f02420e 188e0348 0e208d04 450e288c ..B....H. ..E.(.
+  0x00002188 05440e30 8606440e 38830747 0e7002c0 .D.0..D.8..G.p..
+  0x00002198 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
+  0x000021a8 0e10420e 08420b00 14000000 6c010000 ..B..B......l...
+  0x000021b8 08efffff 32000000 00480e10 570e0800 ....2....H..W...
+  0x000021c8 00000000                            ....
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00003dc0 90110000 00000000 a0100000 00000000 ................
+  0x00003da8 b0110000 00000000 c0100000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00003dd0 50110000 00000000                   P.......
+  0x00003db8 70110000 00000000                   p.......
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,9 +1,9 @@
 
 Hex dump of section '.got':
-  0x00003fa8 00000000 00000000 00000000 00000000 ................
-  0x00003fb8 00000000 00000000 00000000 00000000 ................
-  0x00003fc8 00000000 00000000 00000000 00000000 ................
-  0x00003fd8 00000000 00000000 00000000 00000000 ................
-  0x00003fe8 00000000 00000000 00000000 00000000 ................
-  0x00003ff8 00000000 00000000                   ........
+  0x00003fa0 00000000 00000000 00000000 00000000 ................
+  0x00003fb0 00000000 00000000 00000000 00000000 ................
+  0x00003fc0 00000000 00000000 00000000 00000000 ................
+  0x00003fd0 00000000 00000000 00000000 00000000 ................
+  0x00003fe0 00000000 00000000 00000000 00000000 ................
+  0x00003ff0 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,7 +1,8 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00004000 d83d0000 00000000 00000000 00000000 .=..............
+  0x00004000 c03d0000 00000000 00000000 00000000 .=..............
   0x00004010 00000000 00000000 30100000 00000000 ........0.......
   0x00004020 40100000 00000000 50100000 00000000 @.......P.......
+  0x00004030 60100000 00000000                   `.......
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00004030 30400000 00000000                   0@......
+  0x00004038 38400000 00000000                   8@......
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -27,16 +27,18 @@
   0x00000180 5a4e5374 38696f73 5f626173 6534496e ZNSt8ios_base4In
   0x00000190 69744431 45764040 474c4942 4358585f itD1Ev@@GLIBCXX_
   0x000001a0 332e3400 5f49544d 5f646572 65676973 3.4._ITM_deregis
   0x000001b0 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
   0x000001c0 5f49544d 5f726567 69737465 72544d43 _ITM_registerTMC
   0x000001d0 6c6f6e65 5461626c 65005f5f 6378615f loneTable.__cxa_
   0x000001e0 66696e61 6c697a65 4040474c 4942435f finalize@@GLIBC_
-  0x000001f0 322e322e 35007065 726d0070 68617365 2.2.5.perm.phase
-  0x00000200 5f004e70 43616e6f 6e696361 6c526570 _.NpCanonicalRep
-  0x00000210 72657365 6e746174 69766500 70686173 resentative.phas
-  0x00000220 655f6e65 78745f00 47656e65 72617465 e_next_.Generate
-  0x00000230 5065726d 75746174 696f6e54 61626c65 PermutationTable
-  0x00000240 00696473 5f004e70 6e43616e 6f6e6963 .ids_.NpnCanonic
-  0x00000250 616c5265 70726573 656e7461 74697665 alRepresentative
-  0x00000260 00                                  .
+  0x000001f0 322e322e 35007065 726d0063 5f6e756d 2.2.5.perm.c_num
+  0x00000200 5f696e70 75747300 70686173 655f004e _inputs.phase_.N
+  0x00000210 7043616e 6f6e6963 616c5265 70726573 pCanonicalRepres
+  0x00000220 656e7461 74697665 005f5f73 7461636b entative.__stack
+  0x00000230 5f63686b 5f666169 6c404047 4c494243 _chk_fail@@GLIBC
+  0x00000240 5f322e34 00706861 73655f6e 6578745f _2.4.phase_next_
+  0x00000250 0047656e 65726174 65506572 6d757461 .GeneratePermuta
+  0x00000260 74696f6e 5461626c 65006964 735f004e tionTable.ids_.N
+  0x00000270 706e4361 6e6f6e69 63616c52 65707265 pnCanonicalRepre
+  0x00000280 73656e74 61746976 6500              sentative.
```

### Comparing `npn-1.0/npn/npn.dll` & `npn-1.1/npn/npn.dll`

 * *Files 13% similar despite different names*

#### objdump

```diff
@@ -1,54 +1,54 @@
 
 architecture: i386:x86-64, flags 0x0000012f:
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
-start address 0x0000000180001c84
+start address 0x0000000180001cdc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jul  1 13:12:43 2023
+Time/Date		Thu Jul 13 19:51:46 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
-SizeOfCode		0000000000001600
+SizeOfCode		0000000000001800
 SizeOfInitializedData	0000000000001800
 SizeOfUninitializedData	0000000000000000
-AddressOfEntryPoint	0000000000001c84
+AddressOfEntryPoint	0000000000001cdc
 BaseOfCode		0000000000001000
 ImageBase		0000000180000000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	6
 MinorOSystemVersion	0
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00084000
 SizeOfHeaders		00000400
-CheckSum		00004f26
+CheckSum		00008c17
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
-Entry 0 0000000000003840 0000009c Export Directory [.edata (or where ever we found it)]
-Entry 1 00000000000038dc 00000050 Import Directory [parts of .idata]
+Entry 0 0000000000003850 0000009c Export Directory [.edata (or where ever we found it)]
+Entry 1 00000000000038ec 00000050 Import Directory [parts of .idata]
 Entry 2 0000000000082000 000001b4 Resource Directory [.rsrc]
 Entry 3 0000000000081000 00000234 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 0000000000083000 00000028 Base Relocation Directory [.reloc]
 Entry 6 00000000000032c0 0000001c Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
@@ -56,447 +56,454 @@
 Entry a 0000000000003180 00000140 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 0000000000003000 000000e0 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
-There is an import table in .rdata at 0x1800038dc
+There is an import table in .rdata at 0x1800038ec
 
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
- 000038dc	000039a0 00000000 00000000 00003a52 00003070
+ 000038ec	000039b0 00000000 00000000 00003a62 00003070
 
 	DLL Name: VCRUNTIME140.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	3c78	   60  memcpy
-	3a32	   37  __std_type_info_destroy_list
-	3a1a	    8  __C_specific_handler
-	3a10	   62  memset
+	3c88	   60  memcpy
+	3a42	   37  __std_type_info_destroy_list
+	3a2a	    8  __C_specific_handler
+	3a20	   62  memset
 
- 000038f0	000039c8 00000000 00000000 00003b0a 00003098
+ 00003900	000039d8 00000000 00000000 00003b1a 00003098
 
 	DLL Name: api-ms-win-crt-runtime-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	3b00	   22  _cexit
-	3ae8	   34  _execute_onexit_table
-	3acc	   52  _initialize_onexit_table
-	3aaa	   51  _initialize_narrow_environment
-	3a90	   24  _configure_narrow_argv
-	3a7e	   63  _seh_filter_dll
-	3a70	   55  _initterm_e
-	3a64	   54  _initterm
+	3b10	   22  _cexit
+	3af8	   34  _execute_onexit_table
+	3adc	   52  _initialize_onexit_table
+	3aba	   51  _initialize_narrow_environment
+	3aa0	   24  _configure_narrow_argv
+	3a8e	   63  _seh_filter_dll
+	3a80	   55  _initterm_e
+	3a74	   54  _initterm
 
- 00003904	00003930 00000000 00000000 00003c6a 00003000
+ 00003914	00003940 00000000 00000000 00003c7a 00003000
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	3c00	  919  IsDebuggerPresent
-	3b46	  555  GetCurrentProcessId
-	3b2c	 1124  QueryPerformanceCounter
-	3b72	  769  GetSystemTimeAsFileTime
-	3b8c	  300  DisableThreadLibraryCalls
-	3ba8	  897  InitializeSListHead
-	3c4e	  926  IsProcessorFeaturePresent
-	3c30	 1431  SetUnhandledExceptionFilter
-	3c14	 1496  UnhandledExceptionFilter
-	3b5c	  559  GetCurrentThreadId
-	3bec	 1272  RtlVirtualUnwind
-	3bd2	 1265  RtlLookupFunctionEntry
-	3bbe	 1257  RtlCaptureContext
+	3c10	  919  IsDebuggerPresent
+	3b56	  555  GetCurrentProcessId
+	3b3c	 1124  QueryPerformanceCounter
+	3b82	  769  GetSystemTimeAsFileTime
+	3b9c	  300  DisableThreadLibraryCalls
+	3bb8	  897  InitializeSListHead
+	3c5e	  926  IsProcessorFeaturePresent
+	3c40	 1431  SetUnhandledExceptionFilter
+	3c24	 1496  UnhandledExceptionFilter
+	3b6c	  559  GetCurrentThreadId
+	3bfc	 1272  RtlVirtualUnwind
+	3be2	 1265  RtlLookupFunctionEntry
+	3bce	 1257  RtlCaptureContext
 
- 00003918	00000000 00000000 00000000 00000000 00000000
+ 00003928	00000000 00000000 00000000 00000000 00000000
 
-There is an export table in .rdata at 0x180003840
+There is an export table in .rdata at 0x180003850
 
 The Export Tables (interpreted .rdata section contents)
 
 Export Flags 			0
 Time/Date stamp 		ffffffff
 Major/Minor 			0/0
-Name 				0000000000003886 npn.dll
+Name 				0000000000003896 npn.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000003
 	[Name Pointer/Ordinal] Table	00000003
 Table Addresses
-	Export Address Table 		0000000000003868
-	Name Pointer Table 		0000000000003874
-	Ordinal Table 			0000000000003880
+	Export Address Table 		0000000000003878
+	Name Pointer Table 		0000000000003884
+	Ordinal Table 			0000000000003890
 
 Export Address Table -- Ordinal Base 1
 	[   0] +base[   1] 1000 Export RVA
-	[   1] +base[   2] 1240 Export RVA
-	[   2] +base[   3] 1590 Export RVA
+	[   1] +base[   2] 1250 Export RVA
+	[   2] +base[   3] 15b0 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] GeneratePermutationTable
 	[   1] NpCanonicalRepresentative
 	[   2] NpnCanonicalRepresentative
 
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
- 0000000180081000:	0000000180001000 00000001800010bc 00000001800035a0
- 000000018008100c:	00000001800010bc 000000018000122f 00000001800035b0
- 0000000180081018:	000000018000122f 000000018000123f 00000001800035d4
- 0000000180081024:	0000000180001240 00000001800012b5 000000018000366c
- 0000000180081030:	00000001800012b5 0000000180001333 000000018000367c
- 000000018008103c:	0000000180001333 0000000180001514 000000018000369c
- 0000000180081048:	0000000180001514 0000000180001540 00000001800036b0
- 0000000180081054:	0000000180001540 000000018000158a 00000001800036c0
- 0000000180081060:	0000000180001590 00000001800015a4 00000001800035e4
- 000000018008106c:	00000001800015a4 0000000180001660 00000001800035f4
- 0000000180081078:	0000000180001660 000000018000168e 0000000180003608
- 0000000180081084:	000000018000168e 0000000180001713 0000000180003618
- 0000000180081090:	0000000180001713 00000001800018f1 0000000180003634
- 000000018008109c:	00000001800018f1 0000000180001920 0000000180003648
- 00000001800810a8:	0000000180001920 0000000180001964 0000000180003658
- 00000001800810b4:	0000000180001964 00000001800019b4 0000000180003768
- 00000001800810c0:	00000001800019b4 0000000180001aca 00000001800036d0
- 00000001800810cc:	0000000180001acc 0000000180001b50 0000000180003714
- 00000001800810d8:	0000000180001b50 0000000180001c81 0000000180003770
- 00000001800810e4:	0000000180001c84 0000000180001cc1 00000001800037a0
- 00000001800810f0:	0000000180001cc4 0000000180001d70 00000001800037b0
- 00000001800810fc:	0000000180001d70 0000000180001d93 0000000180003768
- 0000000180081108:	0000000180001dc0 0000000180001ddb 0000000180003768
- 0000000180081114:	0000000180001ddc 0000000180001e15 0000000180003768
- 0000000180081120:	0000000180001e18 0000000180001e4c 0000000180003768
- 000000018008112c:	0000000180001e4c 0000000180001e61 0000000180003768
- 0000000180081138:	0000000180001e64 0000000180001e8c 0000000180003768
- 0000000180081144:	0000000180001e8c 0000000180001ea1 0000000180003768
- 0000000180081150:	0000000180001ea4 0000000180001f04 00000001800037ec
- 000000018008115c:	0000000180001f04 0000000180001f34 0000000180003768
- 0000000180081168:	0000000180001f34 0000000180001f48 0000000180003768
- 0000000180081174:	0000000180001f48 0000000180001f91 00000001800037e4
- 0000000180081180:	0000000180001f94 000000018000201f 00000001800037e4
- 000000018008118c:	0000000180002020 00000001800020b8 00000001800037bc
- 0000000180081198:	00000001800020b8 00000001800020dc 00000001800037e4
- 00000001800811a4:	00000001800020dc 0000000180002105 00000001800037e4
- 00000001800811b0:	0000000180002118 0000000180002263 0000000180003800
- 00000001800811bc:	0000000180002264 00000001800022a0 0000000180003810
- 00000001800811c8:	00000001800022a0 00000001800022dc 0000000180003810
- 00000001800811d4:	00000001800022e0 000000018000248c 000000018000381c
- 00000001800811e0:	0000000180002510 0000000180002512 0000000180003830
- 00000001800811ec:	0000000180002530 0000000180002536 0000000180003838
- 00000001800811f8:	0000000180002536 000000018000254d 000000018000370c
- 0000000180081204:	000000018000254d 0000000180002566 000000018000370c
- 0000000180081210:	0000000180002566 000000018000257a 000000018000370c
- 000000018008121c:	000000018000257a 00000001800025b0 0000000180003798
- 0000000180081228:	00000001800025b0 00000001800025c8 00000001800037dc
+ 0000000180081000:	0000000180001000 00000001800010c2 00000001800035a0
+ 000000018008100c:	00000001800010c2 0000000180001222 00000001800035b4
+ 0000000180081018:	0000000180001222 0000000180001242 00000001800035d4
+ 0000000180081024:	0000000180001250 00000001800012d1 00000001800035e4
+ 0000000180081030:	00000001800012d1 0000000180001540 00000001800035f8
+ 000000018008103c:	0000000180001540 00000001800015a6 0000000180003618
+ 0000000180081048:	00000001800015b0 00000001800015cd 0000000180003628
+ 0000000180081054:	00000001800015cd 00000001800015d4 0000000180003638
+ 0000000180081060:	00000001800015d4 00000001800016b0 000000018000364c
+ 000000018008106c:	00000001800016b0 00000001800016de 0000000180003668
+ 0000000180081078:	00000001800016de 00000001800016ff 0000000180003680
+ 0000000180081084:	00000001800016ff 000000018000176e 0000000180003694
+ 0000000180081090:	000000018000176e 0000000180001921 00000001800036b4
+ 000000018008109c:	0000000180001921 0000000180001994 00000001800036c8
+ 00000001800810a8:	0000000180001994 00000001800019bb 0000000180003680
+ 00000001800810b4:	00000001800019bc 0000000180001a0c 0000000180003770
+ 00000001800810c0:	0000000180001a0c 0000000180001b22 00000001800036d8
+ 00000001800810cc:	0000000180001b24 0000000180001ba8 000000018000371c
+ 00000001800810d8:	0000000180001ba8 0000000180001cd9 0000000180003778
+ 00000001800810e4:	0000000180001cdc 0000000180001d19 00000001800037a8
+ 00000001800810f0:	0000000180001d1c 0000000180001dc8 00000001800037b8
+ 00000001800810fc:	0000000180001dc8 0000000180001deb 0000000180003770
+ 0000000180081108:	0000000180001e18 0000000180001e33 0000000180003770
+ 0000000180081114:	0000000180001e34 0000000180001e6d 0000000180003770
+ 0000000180081120:	0000000180001e70 0000000180001ea4 0000000180003770
+ 000000018008112c:	0000000180001ea4 0000000180001eb9 0000000180003770
+ 0000000180081138:	0000000180001ebc 0000000180001ee4 0000000180003770
+ 0000000180081144:	0000000180001ee4 0000000180001ef9 0000000180003770
+ 0000000180081150:	0000000180001efc 0000000180001f5c 00000001800037f4
+ 000000018008115c:	0000000180001f5c 0000000180001f8c 0000000180003770
+ 0000000180081168:	0000000180001f8c 0000000180001fa0 0000000180003770
+ 0000000180081174:	0000000180001fa0 0000000180001fe9 00000001800037ec
+ 0000000180081180:	0000000180001fec 0000000180002077 00000001800037ec
+ 000000018008118c:	0000000180002078 0000000180002110 00000001800037c4
+ 0000000180081198:	0000000180002110 0000000180002134 00000001800037ec
+ 00000001800811a4:	0000000180002134 000000018000215d 00000001800037ec
+ 00000001800811b0:	0000000180002170 00000001800022bb 0000000180003808
+ 00000001800811bc:	00000001800022bc 00000001800022f8 0000000180003818
+ 00000001800811c8:	00000001800022f8 0000000180002334 0000000180003818
+ 00000001800811d4:	0000000180002338 00000001800024e4 0000000180003824
+ 00000001800811e0:	0000000180002570 0000000180002572 0000000180003838
+ 00000001800811ec:	0000000180002590 0000000180002596 0000000180003840
+ 00000001800811f8:	0000000180002596 00000001800025ad 0000000180003714
+ 0000000180081204:	00000001800025ad 00000001800025c6 0000000180003714
+ 0000000180081210:	00000001800025c6 00000001800025da 0000000180003714
+ 000000018008121c:	00000001800025da 0000000180002610 00000001800037a0
+ 0000000180081228:	0000000180002610 0000000180002628 00000001800037e4
 
 Dump of .rdata
- 00000001800035a0 (rva: 000035a0): 0000000180001000 - 00000001800010bc
+ 00000001800035a0 (rva: 000035a0): 0000000180001000 - 00000001800010c2
 	Version: 1, Flags: none
-	Nbr codes: 6, Prologue size: 0x54, Frame offset: 0x0, Frame reg: none
-	  pc+0x54: save rsi at rsp + 0x58
-	  pc+0x3a: save rbx at rsp + 0x68
-	  pc+0x09: alloc small area: rsp = rsp - 0x70
-	  pc+0x05: push rdi
- 00000001800035b0 (rva: 000035b0): 00000001800010bc - 000000018000122f
+	Nbr codes: 8, Prologue size: 0x52, Frame offset: 0x0, Frame reg: none
+	  pc+0x52: save rdi at rsp + 0x50
+	  pc+0x46: save rsi at rsp + 0x58
+	  pc+0x3b: save rbx at rsp + 0x68
+	  pc+0x0a: alloc small area: rsp = rsp - 0x70
+	  pc+0x06: push r13
+ 00000001800035b4 (rva: 000035b4): 00000001800010c2 - 0000000180001222
 	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 10, Prologue size: 0x19, Frame offset: 0x0, Frame reg: none
-	  pc+0x19: save r15 at rsp + 0x38
-	  pc+0x14: save r14 at rsp + 0x40
-	  pc+0x0f: save r13 at rsp + 0x48
-	  pc+0x0a: save r12 at rsp + 0x50
+	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
+	  pc+0x14: save r15 at rsp + 0x38
+	  pc+0x0f: save r14 at rsp + 0x40
+	  pc+0x0a: save r12 at rsp + 0x48
 	  pc+0x05: save rbp at rsp + 0x60
-	Chain: start: 0000000000001000, end: 00000000000010bc
+	Chain: start: 0000000000001000, end: 00000000000010c2
 	 unwind data: 00000000000035a0.
- 00000001800035d4 (rva: 000035d4): 000000018000122f - 000000018000123f
+ 00000001800035d4 (rva: 000035d4): 0000000180001222 - 0000000180001242
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 0000000000001000, end: 00000000000010bc
+	Chain: start: 0000000000001000, end: 00000000000010c2
 	 unwind data: 00000000000035a0.
- 000000018000366c (rva: 0000366c): 0000000180001240 - 00000001800012b5
+ 00000001800035e4 (rva: 000035e4): 0000000180001250 - 00000001800012d1
 	Version: 1, Flags: none
-	Nbr codes: 5, Prologue size: 0x73, Frame offset: 0x0, Frame reg: none
-	  pc+0x73: save rbp at rsp + 0x60
-	  pc+0x10: alloc small area: rsp = rsp - 0x68
-	  pc+0x0c: push r15
-	  pc+0x0a: push rbx
- 000000018000367c (rva: 0000367c): 00000001800012b5 - 0000000180001333
+	Nbr codes: 7, Prologue size: 0x7f, Frame offset: 0x0, Frame reg: none
+	  pc+0x7f: save rbp at rsp + 0x58
+	  pc+0x7a: save rbx at rsp + 0x60
+	  pc+0x1b: alloc small area: rsp = rsp - 0x68
+	  pc+0x17: push r13
+	  pc+0x15: push r12
+ 00000001800035f8 (rva: 000035f8): 00000001800012d1 - 0000000180001540
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 8, Prologue size: 0x24, Frame offset: 0x0, Frame reg: none
-	  pc+0x24: save r14 at rsp + 0x38
-	  pc+0x18: save r13 at rsp + 0x40
-	  pc+0x0c: save rdi at rsp + 0x50
-	  pc+0x05: save rsi at rsp + 0x58
-	Chain: start: 0000000000001240, end: 00000000000012b5
-	 unwind data: 000000000000366c.
- 000000018000369c (rva: 0000369c): 0000000180001333 - 0000000180001514
-	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: save r12 at rsp + 0x48
-	Chain: start: 00000000000012b5, end: 0000000000001333
-	 unwind data: 000000000000367c.
- 00000001800036b0 (rva: 000036b0): 0000000180001514 - 0000000180001540
-	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 00000000000012b5, end: 0000000000001333
-	 unwind data: 000000000000367c.
- 00000001800036c0 (rva: 000036c0): 0000000180001540 - 000000018000158a
+	  pc+0x24: save r15 at rsp + 0x38
+	  pc+0x18: save r14 at rsp + 0x40
+	  pc+0x0c: save rdi at rsp + 0x48
+	  pc+0x05: save rsi at rsp + 0x50
+	Chain: start: 0000000000001250, end: 00000000000012d1
+	 unwind data: 00000000000035e4.
+ 0000000180003618 (rva: 00003618): 0000000180001540 - 00000001800015a6
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 0000000000001240, end: 00000000000012b5
-	 unwind data: 000000000000366c.
- 00000001800035e4 (rva: 000035e4): 0000000180001590 - 00000001800015a4
+	Chain: start: 0000000000001250, end: 00000000000012d1
+	 unwind data: 00000000000035e4.
+ 0000000180003628 (rva: 00003628): 00000001800015b0 - 00000001800015cd
 	Version: 1, Flags: none
-	Nbr codes: 5, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
-	  pc+0x14: alloc large area: rsp = rsp - 0x90
-	  pc+0x0d: push r15
-	  pc+0x0b: push rbp
-	  pc+0x0a: push rbx
- 00000001800035f4 (rva: 000035f4): 00000001800015a4 - 0000000180001660
+	Nbr codes: 5, Prologue size: 0x1d, Frame offset: 0x0, Frame reg: none
+	  pc+0x1d: alloc large area: rsp = rsp - 0x90
+	  pc+0x16: push r14
+	  pc+0x14: push rsi
+	  pc+0x13: push rbp
+ 0000000180003638 (rva: 00003638): 00000001800015cd - 00000001800015d4
 	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: save r12 at rsp + 0x78
-	Chain: start: 0000000000001590, end: 00000000000015a4
-	 unwind data: 00000000000035e4.
- 0000000180003608 (rva: 00003608): 0000000180001660 - 000000018000168e
+	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
+	  pc+0x04: save rdi at rsp + 0x80
+	Chain: start: 00000000000015b0, end: 00000000000015cd
+	 unwind data: 0000000000003628.
+ 000000018000364c (rva: 0000364c): 00000001800015d4 - 00000001800016b0
 	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 0000000000001590, end: 00000000000015a4
-	 unwind data: 00000000000035e4.
- 0000000180003618 (rva: 00003618): 000000018000168e - 0000000180001713
+	Nbr codes: 6, Prologue size: 0x96, Frame offset: 0x0, Frame reg: none
+	  pc+0x96: save rbx at rsp + 0x88
+	  pc+0x17: save r15 at rsp + 0x68
+	  pc+0x04: save r12 at rsp + 0x78
+	Chain: start: 00000000000015cd, end: 00000000000015d4
+	 unwind data: 0000000000003638.
+ 0000000180003668 (rva: 00003668): 00000001800016b0 - 00000001800016de
 	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 6, Prologue size: 0x25, Frame offset: 0x0, Frame reg: none
-	  pc+0x25: save r14 at rsp + 0x68
-	  pc+0x17: save rdi at rsp + 0x80
-	  pc+0x08: save rsi at rsp + 0x88
-	Chain: start: 0000000000001920, end: 0000000000001964
-	 unwind data: 0000000000003658.
- 0000000180003634 (rva: 00003634): 0000000180001713 - 00000001800018f1
+	Nbr codes: 4, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+	  pc+0x00: save r15 at rsp + 0x68
+	  pc+0x00: save rbx at rsp + 0x88
+	Chain: start: 00000000000015cd, end: 00000000000015d4
+	 unwind data: 0000000000003638.
+ 0000000180003680 (rva: 00003680): 00000001800016de - 00000001800016ff
+	Version: 1, Flags: UNW_FLAG_CHAININFO
+	Nbr codes: 2, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+	  pc+0x00: save rbx at rsp + 0x88
+	Chain: start: 00000000000015b0, end: 00000000000015cd
+	 unwind data: 0000000000003628.
+ 0000000180003694 (rva: 00003694): 00000001800016ff - 000000018000176e
+	Version: 1, Flags: UNW_FLAG_CHAININFO
+	Nbr codes: 8, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+	  pc+0x00: save r15 at rsp + 0x68
+	  pc+0x00: save r12 at rsp + 0x78
+	  pc+0x00: save rdi at rsp + 0x80
+	  pc+0x00: save rbx at rsp + 0x88
+	Chain: start: 00000000000015b0, end: 00000000000015cd
+	 unwind data: 0000000000003628.
+ 00000001800036b4 (rva: 000036b4): 000000018000176e - 0000000180001921
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: save r13 at rsp + 0x70
-	Chain: start: 000000000000168e, end: 0000000000001713
-	 unwind data: 0000000000003618.
- 0000000180003648 (rva: 00003648): 00000001800018f1 - 0000000180001920
+	Chain: start: 00000000000016ff, end: 000000000000176e
+	 unwind data: 0000000000003694.
+ 00000001800036c8 (rva: 000036c8): 0000000180001921 - 0000000180001994
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 000000000000168e, end: 0000000000001713
-	 unwind data: 0000000000003618.
- 0000000180003658 (rva: 00003658): 0000000180001920 - 0000000180001964
+	Chain: start: 00000000000016ff, end: 000000000000176e
+	 unwind data: 0000000000003694.
+ 0000000180003680 (rva: 00003680): 0000000180001994 - 00000001800019bb
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	  pc+0x00: save r12 at rsp + 0x78
-	Chain: start: 0000000000001590, end: 00000000000015a4
-	 unwind data: 00000000000035e4.
- 0000000180003768 (rva: 00003768): 0000000180001964 - 00000001800019b4
+	  pc+0x00: save rbx at rsp + 0x88
+	Chain: start: 00000000000015b0, end: 00000000000015cd
+	 unwind data: 0000000000003628.
+ 0000000180003770 (rva: 00003770): 00000001800019bc - 0000000180001a0c
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000001800036d0 (rva: 000036d0): 00000001800019b4 - 0000000180001aca
+ 00000001800036d8 (rva: 000036d8): 0000000180001a0c - 0000000180001b22
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rdi at rsp + 0x48
 	  pc+0x15: save rsi at rsp + 0x38
 	  pc+0x15: save rbx at rsp + 0x30
 	  pc+0x15: alloc small area: rsp = rsp - 0x20
 	  pc+0x11: push r14
-	Handler: 00000001800024a6.
+	Handler: 0000000180002506.
 	User data:
-	  000: 02 00 00 00 ec 19 00 00 5b 1a 00 00 36 25 00 00
-	  010: 00 00 00 00 be 1a 00 00 c9 1a 00 00 36 25 00 00
+	  000: 02 00 00 00 44 1a 00 00 b3 1a 00 00 96 25 00 00
+	  010: 00 00 00 00 16 1b 00 00 21 1b 00 00 96 25 00 00
 	  020: 00 00 00 00
- 0000000180003714 (rva: 00003714): 0000000180001acc - 0000000180001b50
+ 000000018000371c (rva: 0000371c): 0000000180001b24 - 0000000180001ba8
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x40
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rdi
-	Handler: 00000001800024a6.
+	Handler: 0000000180002506.
 	User data:
-	  000: 04 00 00 00 03 1b 00 00 22 1b 00 00 4d 25 00 00
-	  010: 00 00 00 00 f8 1a 00 00 3a 1b 00 00 66 25 00 00
-	  020: 00 00 00 00 43 1b 00 00 4e 1b 00 00 4d 25 00 00
-	  030: 00 00 00 00 43 1b 00 00 4f 1b 00 00 66 25 00 00
+	  000: 04 00 00 00 5b 1b 00 00 7a 1b 00 00 ad 25 00 00
+	  010: 00 00 00 00 50 1b 00 00 92 1b 00 00 c6 25 00 00
+	  020: 00 00 00 00 9b 1b 00 00 a6 1b 00 00 ad 25 00 00
+	  030: 00 00 00 00 9b 1b 00 00 a7 1b 00 00 c6 25 00 00
 	  040: 00 00 00 00
- 0000000180003770 (rva: 00003770): 0000000180001b50 - 0000000180001c81
+ 0000000180003778 (rva: 00003778): 0000000180001ba8 - 0000000180001cd9
 	Version: 1, Flags: UNW_FLAG_EHANDLER
 	Nbr codes: 6, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save rbx at rsp + 0x78
 	  pc+0x1a: alloc small area: rsp = rsp - 0x40
 	  pc+0x16: push r14
 	  pc+0x14: push rdi
 	  pc+0x13: push rsi
-	Handler: 00000001800024a6.
+	Handler: 0000000180002506.
 	User data:
-	  000: 01 00 00 00 85 1b 00 00 6b 1c 00 00 7a 25 00 00
-	  010: 6b 1c 00 00
- 00000001800037a0 (rva: 000037a0): 0000000180001c84 - 0000000180001cc1
+	  000: 01 00 00 00 dd 1b 00 00 c3 1c 00 00 da 25 00 00
+	  010: c3 1c 00 00
+ 00000001800037a8 (rva: 000037a8): 0000000180001cdc - 0000000180001d19
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x38
 	  pc+0x0f: save rbx at rsp + 0x30
 	  pc+0x0f: alloc small area: rsp = rsp - 0x20
 	  pc+0x0b: push rdi
- 00000001800037b0 (rva: 000037b0): 0000000180001cc4 - 0000000180001d70
+ 00000001800037b8 (rva: 000037b8): 0000000180001d1c - 0000000180001dc8
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0d, Frame offset: 0x0, Frame reg: none
 	  pc+0x0d: save rbx at rsp + 0x48
 	  pc+0x0d: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
- 0000000180003768 (rva: 00003768): 0000000180001d70 - 0000000180001d93
+ 0000000180003770 (rva: 00003770): 0000000180001dc8 - 0000000180001deb
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 0000000180003768 also used for function at 0000000180001dc0
- 0000000180003768 also used for function at 0000000180001ddc
- 0000000180003768 also used for function at 0000000180001e18
- 0000000180003768 also used for function at 0000000180001e4c
- 0000000180003768 also used for function at 0000000180001e64
- 0000000180003768 also used for function at 0000000180001e8c
- 00000001800037ec (rva: 000037ec): 0000000180001ea4 - 0000000180001f04
+ 0000000180003770 also used for function at 0000000180001e18
+ 0000000180003770 also used for function at 0000000180001e34
+ 0000000180003770 also used for function at 0000000180001e70
+ 0000000180003770 also used for function at 0000000180001ea4
+ 0000000180003770 also used for function at 0000000180001ebc
+ 0000000180003770 also used for function at 0000000180001ee4
+ 00000001800037f4 (rva: 000037f4): 0000000180001efc - 0000000180001f5c
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: save rsi at rsp + 0x40
 	  pc+0x14: save rbp at rsp + 0x38
 	  pc+0x14: save rbx at rsp + 0x30
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push rdi
- 0000000180003768 (rva: 00003768): 0000000180001f04 - 0000000180001f34
+ 0000000180003770 (rva: 00003770): 0000000180001f5c - 0000000180001f8c
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 0000000180003768 also used for function at 0000000180001f34
- 00000001800037e4 (rva: 000037e4): 0000000180001f48 - 0000000180001f91
+ 0000000180003770 also used for function at 0000000180001f8c
+ 00000001800037ec (rva: 000037ec): 0000000180001fa0 - 0000000180001fe9
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 00000001800037e4 also used for function at 0000000180001f94
- 00000001800037bc (rva: 000037bc): 0000000180002020 - 00000001800020b8
+ 00000001800037ec also used for function at 0000000180001fec
+ 00000001800037c4 (rva: 000037c4): 0000000180002078 - 0000000180002110
 	Version: 1, Flags: UNW_FLAG_EHANDLER
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
-	Handler: 00000001800024a6.
+	Handler: 0000000180002506.
 	User data:
-	  000: 01 00 00 00 27 20 00 00 b1 20 00 00 b0 25 00 00
-	  010: b1 20 00 00
- 00000001800037e4 (rva: 000037e4): 00000001800020b8 - 00000001800020dc
+	  000: 01 00 00 00 7f 20 00 00 09 21 00 00 10 26 00 00
+	  010: 09 21 00 00
+ 00000001800037ec (rva: 000037ec): 0000000180002110 - 0000000180002134
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 00000001800037e4 also used for function at 00000001800020dc
- 0000000180003800 (rva: 00003800): 0000000180002118 - 0000000180002263
+ 00000001800037ec also used for function at 0000000180002134
+ 0000000180003808 (rva: 00003808): 0000000180002170 - 00000001800022bb
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rbx at rsp + 0x5d0
 	  pc+0x15: alloc large area: rsp = rsp - 0x5c0
 	  pc+0x06: push rbp
- 0000000180003810 (rva: 00003810): 0000000180002264 - 00000001800022a0
+ 0000000180003818 (rva: 00003818): 00000001800022bc - 00000001800022f8
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x30
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
- 0000000180003810 also used for function at 00000001800022a0
- 000000018000381c (rva: 0000381c): 00000001800022e0 - 000000018000248c
+ 0000000180003818 also used for function at 00000001800022f8
+ 0000000180003824 (rva: 00003824): 0000000180002338 - 00000001800024e4
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x30
 	  pc+0x0f: save rbx at rsp + 0x28
 	  pc+0x0f: alloc small area: rsp = rsp - 0x10
 	  pc+0x0b: push rdi
 	User data:
 	  000: 00 00 00 00
- 0000000180003830 (rva: 00003830): 0000000180002510 - 0000000180002512
+ 0000000180003838 (rva: 00003838): 0000000180002570 - 0000000180002572
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	User data:
 	  000: 00 00 00 00
- 0000000180003838 (rva: 00003838): 0000000180002530 - 0000000180002536
+ 0000000180003840 (rva: 00003840): 0000000180002590 - 0000000180002596
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	User data:
-	  000: 00 00 00 00 00 00 00 00 ff ff ff ff 00 00 00 00
-	  010: 86 38 00 00 01 00 00 00 03 00 00 00 03 00 00 00
-	  020: 68 38 00 00 74 38 00 00 80 38 00 00 00 10 00 00
-	  030: 40 12 00 00 90 15 00 00 8e 38 00 00 a7 38 00 00
-	  040: c1 38 00 00 00 00 01 00 02 00 6e 70 6e 2e 64 6c
-	  050: 6c 00 47 65 6e 65 72 61 74 65 50 65 72 6d 75 74
-	  060: 61 74 69 6f 6e 54 61 62 6c 65 00 4e 70 43 61 6e
-	  070: 6f 6e 69 63 61 6c 52 65 70 72 65 73 65 6e 74 61
-	  080: 74 69 76 65 00 4e 70 6e 43 61 6e 6f 6e 69 63 61
-	  090: 6c 52 65 70 72 65 73 65 6e 74 61 74 69 76 65 00
-	  0a0: a0 39 00 00 00 00 00 00 00 00 00 00 52 3a 00 00
-	  0b0: 70 30 00 00 c8 39 00 00 00 00 00 00 00 00 00 00
-	  0c0: 0a 3b 00 00 98 30 00 00 30 39 00 00 00 00 00 00
-	  0d0: 00 00 00 00 6a 3c 00 00 00 30 00 00 00 00 00 00
-	  0e0: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  0f0: 00 00 00 00 00 3c 00 00 00 00 00 00 46 3b 00 00
-	  100: 00 00 00 00 2c 3b 00 00 00 00 00 00 72 3b 00 00
-	  110: 00 00 00 00 8c 3b 00 00 00 00 00 00 a8 3b 00 00
-	  120: 00 00 00 00 4e 3c 00 00 00 00 00 00 30 3c 00 00
-	  130: 00 00 00 00 14 3c 00 00 00 00 00 00 5c 3b 00 00
-	  140: 00 00 00 00 ec 3b 00 00 00 00 00 00 d2 3b 00 00
-	  150: 00 00 00 00 be 3b 00 00 00 00 00 00 00 00 00 00
-	  160: 00 00 00 00 78 3c 00 00 00 00 00 00 32 3a 00 00
-	  170: 00 00 00 00 1a 3a 00 00 00 00 00 00 10 3a 00 00
-	  180: 00 00 00 00 00 00 00 00 00 00 00 00 00 3b 00 00
-	  190: 00 00 00 00 e8 3a 00 00 00 00 00 00 cc 3a 00 00
-	  1a0: 00 00 00 00 aa 3a 00 00 00 00 00 00 90 3a 00 00
-	  1b0: 00 00 00 00 7e 3a 00 00 00 00 00 00 70 3a 00 00
-	  1c0: 00 00 00 00 64 3a 00 00 00 00 00 00 00 00 00 00
-	  1d0: 00 00 00 00 3e 00 6d 65 6d 73 65 74 00 00 08 00
-	  1e0: 5f 5f 43 5f 73 70 65 63 69 66 69 63 5f 68 61 6e
-	  1f0: 64 6c 65 72 00 00 25 00 5f 5f 73 74 64 5f 74 79
-	  200: 70 65 5f 69 6e 66 6f 5f 64 65 73 74 72 6f 79 5f
-	  210: 6c 69 73 74 00 00 56 43 52 55 4e 54 49 4d 45 31
-	  220: 34 30 2e 64 6c 6c 00 00 36 00 5f 69 6e 69 74 74
-	  230: 65 72 6d 00 37 00 5f 69 6e 69 74 74 65 72 6d 5f
-	  240: 65 00 3f 00 5f 73 65 68 5f 66 69 6c 74 65 72 5f
-	  250: 64 6c 6c 00 18 00 5f 63 6f 6e 66 69 67 75 72 65
-	  260: 5f 6e 61 72 72 6f 77 5f 61 72 67 76 00 00 33 00
-	  270: 5f 69 6e 69 74 69 61 6c 69 7a 65 5f 6e 61 72 72
-	  280: 6f 77 5f 65 6e 76 69 72 6f 6e 6d 65 6e 74 00 00
-	  290: 34 00 5f 69 6e 69 74 69 61 6c 69 7a 65 5f 6f 6e
-	  2a0: 65 78 69 74 5f 74 61 62 6c 65 00 00 22 00 5f 65
-	  2b0: 78 65 63 75 74 65 5f 6f 6e 65 78 69 74 5f 74 61
-	  2c0: 62 6c 65 00 16 00 5f 63 65 78 69 74 00 00 61 70
-	  2d0: 69 2d 6d 73 2d 77 69 6e 2d 63 72 74 2d 72 75 6e
-	  2e0: 74 69 6d 65 2d 6c 31 2d 31 2d 30 2e 64 6c 6c 00
-	  2f0: 64 04 51 75 65 72 79 50 65 72 66 6f 72 6d 61 6e
-	  300: 63 65 43 6f 75 6e 74 65 72 00 2b 02 47 65 74 43
-	  310: 75 72 72 65 6e 74 50 72 6f 63 65 73 73 49 64 00
-	  320: 2f 02 47 65 74 43 75 72 72 65 6e 74 54 68 72 65
-	  330: 61 64 49 64 00 00 01 03 47 65 74 53 79 73 74 65
-	  340: 6d 54 69 6d 65 41 73 46 69 6c 65 54 69 6d 65 00
-	  350: 2c 01 44 69 73 61 62 6c 65 54 68 72 65 61 64 4c
-	  360: 69 62 72 61 72 79 43 61 6c 6c 73 00 81 03 49 6e
-	  370: 69 74 69 61 6c 69 7a 65 53 4c 69 73 74 48 65 61
-	  380: 64 00 e9 04 52 74 6c 43 61 70 74 75 72 65 43 6f
-	  390: 6e 74 65 78 74 00 f1 04 52 74 6c 4c 6f 6f 6b 75
-	  3a0: 70 46 75 6e 63 74 69 6f 6e 45 6e 74 72 79 00 00
-	  3b0: f8 04 52 74 6c 56 69 72 74 75 61 6c 55 6e 77 69
-	  3c0: 6e 64 00 00 97 03 49 73 44 65 62 75 67 67 65 72
-	  3d0: 50 72 65 73 65 6e 74 00 d8 05 55 6e 68 61 6e 64
-	  3e0: 6c 65 64 45 78 63 65 70 74 69 6f 6e 46 69 6c 74
-	  3f0: 65 72 00 00 97 05 53 65 74 55 6e 68 61 6e 64 6c
-	  400: 65 64 45 78 63 65 70 74 69 6f 6e 46 69 6c 74 65
-	  410: 72 00 9e 03 49 73 50 72 6f 63 65 73 73 6f 72 46
-	  420: 65 61 74 75 72 65 50 72 65 73 65 6e 74 00 4b 45
-	  430: 52 4e 45 4c 33 32 2e 64 6c 6c 00 00 3c 00 6d 65
-	  440: 6d 63 70 79 00 00
- 000000018000370c (rva: 0000370c): 0000000180002536 - 000000018000254d
+	  000: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  010: ff ff ff ff 00 00 00 00 96 38 00 00 01 00 00 00
+	  020: 03 00 00 00 03 00 00 00 78 38 00 00 84 38 00 00
+	  030: 90 38 00 00 00 10 00 00 50 12 00 00 b0 15 00 00
+	  040: 9e 38 00 00 b7 38 00 00 d1 38 00 00 00 00 01 00
+	  050: 02 00 6e 70 6e 2e 64 6c 6c 00 47 65 6e 65 72 61
+	  060: 74 65 50 65 72 6d 75 74 61 74 69 6f 6e 54 61 62
+	  070: 6c 65 00 4e 70 43 61 6e 6f 6e 69 63 61 6c 52 65
+	  080: 70 72 65 73 65 6e 74 61 74 69 76 65 00 4e 70 6e
+	  090: 43 61 6e 6f 6e 69 63 61 6c 52 65 70 72 65 73 65
+	  0a0: 6e 74 61 74 69 76 65 00 b0 39 00 00 00 00 00 00
+	  0b0: 00 00 00 00 62 3a 00 00 70 30 00 00 d8 39 00 00
+	  0c0: 00 00 00 00 00 00 00 00 1a 3b 00 00 98 30 00 00
+	  0d0: 40 39 00 00 00 00 00 00 00 00 00 00 7a 3c 00 00
+	  0e0: 00 30 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  0f0: 00 00 00 00 00 00 00 00 00 00 00 00 10 3c 00 00
+	  100: 00 00 00 00 56 3b 00 00 00 00 00 00 3c 3b 00 00
+	  110: 00 00 00 00 82 3b 00 00 00 00 00 00 9c 3b 00 00
+	  120: 00 00 00 00 b8 3b 00 00 00 00 00 00 5e 3c 00 00
+	  130: 00 00 00 00 40 3c 00 00 00 00 00 00 24 3c 00 00
+	  140: 00 00 00 00 6c 3b 00 00 00 00 00 00 fc 3b 00 00
+	  150: 00 00 00 00 e2 3b 00 00 00 00 00 00 ce 3b 00 00
+	  160: 00 00 00 00 00 00 00 00 00 00 00 00 88 3c 00 00
+	  170: 00 00 00 00 42 3a 00 00 00 00 00 00 2a 3a 00 00
+	  180: 00 00 00 00 20 3a 00 00 00 00 00 00 00 00 00 00
+	  190: 00 00 00 00 10 3b 00 00 00 00 00 00 f8 3a 00 00
+	  1a0: 00 00 00 00 dc 3a 00 00 00 00 00 00 ba 3a 00 00
+	  1b0: 00 00 00 00 a0 3a 00 00 00 00 00 00 8e 3a 00 00
+	  1c0: 00 00 00 00 80 3a 00 00 00 00 00 00 74 3a 00 00
+	  1d0: 00 00 00 00 00 00 00 00 00 00 00 00 3e 00 6d 65
+	  1e0: 6d 73 65 74 00 00 08 00 5f 5f 43 5f 73 70 65 63
+	  1f0: 69 66 69 63 5f 68 61 6e 64 6c 65 72 00 00 25 00
+	  200: 5f 5f 73 74 64 5f 74 79 70 65 5f 69 6e 66 6f 5f
+	  210: 64 65 73 74 72 6f 79 5f 6c 69 73 74 00 00 56 43
+	  220: 52 55 4e 54 49 4d 45 31 34 30 2e 64 6c 6c 00 00
+	  230: 36 00 5f 69 6e 69 74 74 65 72 6d 00 37 00 5f 69
+	  240: 6e 69 74 74 65 72 6d 5f 65 00 3f 00 5f 73 65 68
+	  250: 5f 66 69 6c 74 65 72 5f 64 6c 6c 00 18 00 5f 63
+	  260: 6f 6e 66 69 67 75 72 65 5f 6e 61 72 72 6f 77 5f
+	  270: 61 72 67 76 00 00 33 00 5f 69 6e 69 74 69 61 6c
+	  280: 69 7a 65 5f 6e 61 72 72 6f 77 5f 65 6e 76 69 72
+	  290: 6f 6e 6d 65 6e 74 00 00 34 00 5f 69 6e 69 74 69
+	  2a0: 61 6c 69 7a 65 5f 6f 6e 65 78 69 74 5f 74 61 62
+	  2b0: 6c 65 00 00 22 00 5f 65 78 65 63 75 74 65 5f 6f
+	  2c0: 6e 65 78 69 74 5f 74 61 62 6c 65 00 16 00 5f 63
+	  2d0: 65 78 69 74 00 00 61 70 69 2d 6d 73 2d 77 69 6e
+	  2e0: 2d 63 72 74 2d 72 75 6e 74 69 6d 65 2d 6c 31 2d
+	  2f0: 31 2d 30 2e 64 6c 6c 00 64 04 51 75 65 72 79 50
+	  300: 65 72 66 6f 72 6d 61 6e 63 65 43 6f 75 6e 74 65
+	  310: 72 00 2b 02 47 65 74 43 75 72 72 65 6e 74 50 72
+	  320: 6f 63 65 73 73 49 64 00 2f 02 47 65 74 43 75 72
+	  330: 72 65 6e 74 54 68 72 65 61 64 49 64 00 00 01 03
+	  340: 47 65 74 53 79 73 74 65 6d 54 69 6d 65 41 73 46
+	  350: 69 6c 65 54 69 6d 65 00 2c 01 44 69 73 61 62 6c
+	  360: 65 54 68 72 65 61 64 4c 69 62 72 61 72 79 43 61
+	  370: 6c 6c 73 00 81 03 49 6e 69 74 69 61 6c 69 7a 65
+	  380: 53 4c 69 73 74 48 65 61 64 00 e9 04 52 74 6c 43
+	  390: 61 70 74 75 72 65 43 6f 6e 74 65 78 74 00 f1 04
+	  3a0: 52 74 6c 4c 6f 6f 6b 75 70 46 75 6e 63 74 69 6f
+	  3b0: 6e 45 6e 74 72 79 00 00 f8 04 52 74 6c 56 69 72
+	  3c0: 74 75 61 6c 55 6e 77 69 6e 64 00 00 97 03 49 73
+	  3d0: 44 65 62 75 67 67 65 72 50 72 65 73 65 6e 74 00
+	  3e0: d8 05 55 6e 68 61 6e 64 6c 65 64 45 78 63 65 70
+	  3f0: 74 69 6f 6e 46 69 6c 74 65 72 00 00 97 05 53 65
+	  400: 74 55 6e 68 61 6e 64 6c 65 64 45 78 63 65 70 74
+	  410: 69 6f 6e 46 69 6c 74 65 72 00 9e 03 49 73 50 72
+	  420: 6f 63 65 73 73 6f 72 46 65 61 74 75 72 65 50 72
+	  430: 65 73 65 6e 74 00 4b 45 52 4e 45 4c 33 32 2e 64
+	  440: 6c 6c 00 00 3c 00 6d 65 6d 63 70 79 00 00
+ 0000000180003714 (rva: 00003714): 0000000180002596 - 00000001800025ad
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000370c also used for function at 000000018000254d
- 000000018000370c also used for function at 0000000180002566
- 0000000180003798 (rva: 00003798): 000000018000257a - 00000001800025b0
+ 0000000180003714 also used for function at 00000001800025ad
+ 0000000180003714 also used for function at 00000001800025c6
+ 00000001800037a0 (rva: 000037a0): 00000001800025da - 0000000180002610
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x30
 	  pc+0x02: push rbp
- 00000001800037dc (rva: 000037dc): 00000001800025b0 - 00000001800025c8
+ 00000001800037e4 (rva: 000037e4): 0000000180002610 - 0000000180002628
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x02, Frame offset: 0x0, Frame reg: none
 	  pc+0x02: push rbp
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
@@ -517,132 +524,133 @@
 	reloc   13 offset  2b0 [32b0] DIR64
 	reloc   14 offset  2b8 [32b8] DIR64
 	reloc   15 offset    0 [3000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800032c0
 
 Type                Size     Rva      Offset
- 13         CoffGrp 00000230 00003350 00001d50
+ 13         CoffGrp 00000230 00003350 00001f50
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
 018    Name Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 028     Entry: ID: 0x000002, Value: 0x80000030
 030      Language Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 040       Entry: ID: 0x000409, Value: 0x000048
 048        Leaf: Addr: 0x082058, Size: 0x00015a, Codepage: 1252
  Resources start at offset: 0x58
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         000015c8  0000000180001000  0000000180001000  00000400  2**4
+  0 .text         00001628  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
-  1 .rdata        00000c82  0000000180003000  0000000180003000  00001a00  2**4
+  1 .rdata        00000c92  0000000180003000  0000000180003000  00001c00  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  2 .data         00000200  0000000180004000  0000000180004000  00002800  2**4
+  2 .data         00000200  0000000180004000  0000000180004000  00002a00  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  3 .pdata        00000234  0000000180081000  0000000180081000  00002a00  2**2
+  3 .pdata        00000234  0000000180081000  0000000180081000  00002c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .rsrc         000001b4  0000000180082000  0000000180082000  00002e00  2**2
+  4 .rsrc         000001b4  0000000180082000  0000000180082000  00003000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  5 .reloc        00000028  0000000180083000  0000000180083000  00003000  2**2
+  5 .reloc        00000028  0000000180083000  0000000180083000  00003200  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
 SYMBOL TABLE:
 no symbols
 
 
 
 Disassembly of section .text:
 
 0000000180001000 <.text>:
    180001000:	mov    %cl,0x8(%rsp)
-   180001004:	push   %rdi
-   180001005:	sub    $0x70,%rsp
-   180001009:	movsbl %cl,%r8d
-   18000100d:	mov    $0x1,%eax
-   180001012:	mov    %r8d,0x90(%rsp)
-   18000101a:	mov    %r8d,%r10d
-   18000101d:	cmp    %eax,%r8d
-   180001020:	jbe    0x180001035
-   180001022:	imul   %eax,%r10d
-   180001026:	inc    %eax
-   180001028:	cmp    %r8d,%eax
-   18000102b:	jb     0x180001022
-   18000102d:	mov    %r10d,0x90(%rsp)
-   180001035:	mov    %rbx,0x68(%rsp)
-   18000103a:	mov    $0x1,%r9d
-   180001040:	mov    %r9d,0x98(%rsp)
-   180001048:	lea    0xe3f1(%rip),%rdi        # 0x18000f440
-   18000104f:	mov    %rsi,0x58(%rsp)
-   180001054:	lea    0x2fe5(%rip),%rax        # 0x180004040
-   18000105b:	test   %r10d,%r10d
-   18000105e:	je     0x1800010aa
-   180001060:	mov    %rax,%rbx
-   180001063:	mov    %r10d,%esi
-   180001066:	movb   $0x0,(%rbx)
-   180001069:	test   %r8b,%r8b
-   18000106c:	jle    0x180001085
-   18000106e:	movzbl %r8b,%r8d
-   180001072:	mov    $0x1,%dl
-   180001074:	mov    %rdi,%rcx
-   180001077:	call   0x1800024a0
-   18000107c:	movzbl 0x80(%rsp),%r8d
-   180001085:	add    $0x40,%rbx
-   180001089:	add    $0x6,%rdi
-   18000108d:	sub    $0x1,%rsi
-   180001091:	jne    0x180001066
-   180001093:	mov    0x98(%rsp),%r9d
-   18000109b:	lea    0xe39e(%rip),%rdi        # 0x18000f440
-   1800010a2:	mov    0x90(%rsp),%r10d
-   1800010aa:	xor    %cl,%cl
-   1800010ac:	mov    %cl,0x88(%rsp)
-   1800010b3:	test   %r8b,%r8b
-   1800010b6:	jle    0x18000122f
-   1800010bc:	mov    %rbp,0x60(%rsp)
-   1800010c1:	mov    %r12,0x50(%rsp)
-   1800010c6:	mov    %r13,0x48(%rsp)
-   1800010cb:	mov    %r14,0x40(%rsp)
-   1800010d0:	mov    %r15,0x38(%rsp)
-   1800010d5:	data16 data16 nopw 0x0(%rax,%rax,1)
+   180001004:	push   %r13
+   180001006:	sub    $0x70,%rsp
+   18000100a:	movsbl %cl,%r9d
+   18000100e:	mov    $0x1,%eax
+   180001013:	mov    %r9d,0x88(%rsp)
+   18000101b:	mov    %r9d,%r10d
+   18000101e:	cmp    %eax,%r9d
+   180001021:	jbe    0x180001036
+   180001023:	imul   %eax,%r10d
+   180001027:	inc    %eax
+   180001029:	cmp    %r9d,%eax
+   18000102c:	jb     0x180001023
+   18000102e:	mov    %r10d,0x88(%rsp)
+   180001036:	mov    %rbx,0x68(%rsp)
+   18000103b:	mov    $0x1,%r8d
+   180001041:	mov    %rsi,0x58(%rsp)
+   180001046:	lea    0xe3f3(%rip),%r11        # 0x18000f440
+   18000104d:	mov    %rdi,0x50(%rsp)
+   180001052:	lea    0x2fe7(%rip),%rax        # 0x180004040
+   180001059:	mov    %r8d,0x90(%rsp)
+   180001061:	test   %r10d,%r10d
+   180001064:	je     0x1800010b6
+   180001066:	mov    %r11,%rdi
+   180001069:	mov    %r10d,%esi
+   18000106c:	mov    %rax,%rbx
+   18000106f:	nop
+   180001070:	movb   $0x0,(%rbx)
+   180001073:	test   %r9b,%r9b
+   180001076:	jle    0x180001091
+   180001078:	movzbl %r9b,%r8d
+   18000107c:	movzbl %r9b,%edx
+   180001080:	mov    %rdi,%rcx
+   180001083:	call   0x180002500
+   180001088:	movzbl 0x80(%rsp),%r9d
+   180001091:	add    $0x40,%rbx
+   180001095:	add    $0x6,%rdi
+   180001099:	sub    $0x1,%rsi
+   18000109d:	jne    0x180001070
+   18000109f:	mov    0x90(%rsp),%r8d
+   1800010a7:	lea    0xe392(%rip),%r11        # 0x18000f440
+   1800010ae:	mov    0x88(%rsp),%r10d
+   1800010b6:	xor    %r13b,%r13b
+   1800010b9:	test   %r9b,%r9b
+   1800010bc:	jle    0x180001222
+   1800010c2:	mov    %rbp,0x60(%rsp)
+   1800010c7:	mov    %r12,0x48(%rsp)
+   1800010cc:	mov    %r14,0x40(%rsp)
+   1800010d1:	mov    %r15,0x38(%rsp)
+   1800010d6:	data16 nopw 0x0(%rax,%rax,1)
    1800010e0:	xor    %edx,%edx
-   1800010e2:	movzbl %r8b,%eax
-   1800010e6:	sub    %cl,%al
-   1800010e8:	mov    $0x1,%ebx
-   1800010ed:	movsbl %al,%r11d
-   1800010f1:	xor    %esi,%esi
-   1800010f3:	mov    %r10d,%eax
-   1800010f6:	shl    %cl,%bl
-   1800010f8:	div    %r9d
-   1800010fb:	xor    %edx,%edx
-   1800010fd:	mov    %r11d,0x20(%rsp)
-   180001102:	div    %r11d
-   180001105:	mov    %eax,%r13d
-   180001108:	test   %r9d,%r9d
-   18000110b:	je     0x1800011f8
-   180001111:	mov    %r9d,%eax
-   180001114:	mov    %rax,0x28(%rsp)
-   180001119:	nopl   0x0(%rax)
-   180001120:	xor    %r15b,%r15b
-   180001123:	xor    %r14d,%r14d
-   180001126:	data16 nopw 0x0(%rax,%rax,1)
+   1800010e2:	movzbl %r9b,%eax
+   1800010e6:	sub    %r13b,%al
+   1800010e9:	movzbl %r13b,%ecx
+   1800010ed:	mov    $0x1,%ebx
+   1800010f2:	xor    %esi,%esi
+   1800010f4:	shl    %cl,%bl
+   1800010f6:	movsbl %al,%ecx
+   1800010f9:	mov    %r10d,%eax
+   1800010fc:	div    %r8d
+   1800010ff:	xor    %edx,%edx
+   180001101:	mov    %ecx,0x20(%rsp)
+   180001105:	div    %ecx
+   180001107:	mov    %eax,0x98(%rsp)
+   18000110e:	mov    %eax,%edx
+   180001110:	test   %r8d,%r8d
+   180001113:	je     0x1800011f6
+   180001119:	mov    %r8d,%eax
+   18000111c:	mov    %rax,0x28(%rsp)
+   180001121:	xor    %r15b,%r15b
+   180001124:	xor    %r14d,%r14d
+   180001127:	nopw   0x0(%rax,%rax,1)
    180001130:	lea    (%rsi,%rsi,2),%rax
    180001134:	lea    (%r14,%rax,2),%rcx
-   180001138:	cmpb   $0x0,(%rcx,%rdi,1)
-   18000113c:	je     0x1800011c0
-   180001142:	test   %r13d,%r13d
-   180001145:	je     0x1800011c0
-   180001147:	movsbl %r15b,%r12d
-   18000114b:	mov    %r13,%rbp
-   18000114e:	xchg   %ax,%ax
+   180001138:	cmp    %r9b,(%rcx,%r11,1)
+   18000113c:	jne    0x1800011c7
+   180001142:	test   %edx,%edx
+   180001144:	je     0x1800011c7
+   18000114a:	movsbl %r15b,%r12d
+   18000114e:	mov    %edx,%ebp
    180001150:	lea    (%rsi,%rsi,2),%rax
    180001154:	mov    %esi,%r10d
    180001157:	lea    (%r14,%rax,2),%rcx
    18000115b:	xor    %al,%al
-   18000115d:	movb   $0x0,(%rcx,%rdi,1)
+   18000115d:	mov    %r13b,(%rcx,%r11,1)
    180001161:	test   %bl,%bl
    180001163:	jle    0x1800011af
    180001165:	mov    %r12d,%ecx
    180001168:	movsbl %bl,%edi
    18000116b:	mov    $0x1,%r11d
    180001171:	lea    0x2ec8(%rip),%r12        # 0x180004040
    180001178:	shl    %cl,%r11b
@@ -656,1564 +664,1612 @@
    180001194:	inc    %al
    180001196:	movslq %ecx,%rdx
    180001199:	add    %r10,%rdx
    18000119c:	mov    %r8b,(%rdx,%r12,1)
    1800011a0:	cmp    %bl,%al
    1800011a2:	jl     0x180001183
    1800011a4:	movsbl %r15b,%r12d
-   1800011a8:	lea    0xe291(%rip),%rdi        # 0x18000f440
+   1800011a8:	lea    0xe291(%rip),%r11        # 0x18000f440
    1800011af:	inc    %esi
    1800011b1:	sub    $0x1,%rbp
    1800011b5:	jne    0x180001150
-   1800011b7:	movzbl 0x80(%rsp),%r8d
-   1800011c0:	inc    %r15b
-   1800011c3:	inc    %r14
-   1800011c6:	cmp    %r8b,%r15b
-   1800011c9:	jl     0x180001130
-   1800011cf:	subq   $0x1,0x28(%rsp)
-   1800011d5:	jne    0x180001120
-   1800011db:	movzbl 0x88(%rsp),%ecx
-   1800011e3:	mov    0x98(%rsp),%r9d
-   1800011eb:	mov    0x90(%rsp),%r10d
-   1800011f3:	mov    0x20(%rsp),%r11d
-   1800011f8:	imul   %r11d,%r9d
-   1800011fc:	inc    %cl
-   1800011fe:	mov    %cl,0x88(%rsp)
-   180001205:	mov    %r9d,0x98(%rsp)
-   18000120d:	cmp    %r8b,%cl
-   180001210:	jl     0x1800010e0
-   180001216:	mov    0x38(%rsp),%r15
-   18000121b:	mov    0x40(%rsp),%r14
-   180001220:	mov    0x48(%rsp),%r13
-   180001225:	mov    0x50(%rsp),%r12
-   18000122a:	mov    0x60(%rsp),%rbp
-   18000122f:	mov    0x58(%rsp),%rsi
-   180001234:	mov    0x68(%rsp),%rbx
-   180001239:	add    $0x70,%rsp
-   18000123d:	pop    %rdi
-   18000123e:	ret
-   18000123f:	int3
-   180001240:	mov    %dl,0x10(%rsp)
-   180001244:	mov    %rcx,0x8(%rsp)
-   180001249:	push   %rbx
-   18000124a:	push   %r15
-   18000124c:	sub    $0x68,%rsp
-   180001250:	mov    %rcx,%rbx
-   180001253:	mov    $0x1,%eax
-   180001258:	movsbl %dl,%ecx
-   18000125b:	mov    %ecx,0xc(%rsp)
-   18000125f:	mov    %ecx,%r8d
-   180001262:	cmp    %eax,%ecx
-   180001264:	jbe    0x180001275
-   180001266:	imul   %eax,%r8d
-   18000126a:	inc    %eax
-   18000126c:	cmp    %ecx,%eax
-   18000126e:	jb     0x180001266
-   180001270:	mov    %r8d,0xc(%rsp)
-   180001275:	mov    $0x1,%r15d
-   18000127b:	shl    %cl,%r15d
-   18000127e:	xor    %cl,%cl
-   180001280:	mov    %r15d,0x18(%rsp)
-   180001285:	test   %r15d,%r15d
-   180001288:	je     0x1800012a4
-   18000128a:	nopw   0x0(%rax,%rax,1)
-   180001290:	movsbq %cl,%rax
-   180001294:	cmpb   $0x0,(%rax,%rbx,1)
-   180001298:	jne    0x1800012ae
-   18000129a:	inc    %cl
-   18000129c:	movsbl %cl,%eax
-   18000129f:	cmp    %r15d,%eax
-   1800012a2:	jb     0x180001290
-   1800012a4:	xor    %eax,%eax
-   1800012a6:	add    $0x68,%rsp
-   1800012aa:	pop    %r15
-   1800012ac:	pop    %rbx
-   1800012ad:	ret
-   1800012ae:	mov    %rbp,0x60(%rsp)
-   1800012b3:	xor    %ebp,%ebp
-   1800012b5:	mov    %rsi,0x58(%rsp)
-   1800012ba:	xor    %cl,%cl
-   1800012bc:	mov    %rdi,0x50(%rsp)
-   1800012c1:	lea    0x1a658(%rip),%rsi        # 0x18001b920
-   1800012c8:	mov    %r13,0x40(%rsp)
-   1800012cd:	lea    0xf24c(%rip),%rdi        # 0x180010520
-   1800012d4:	mov    %r14,0x38(%rsp)
-   1800012d9:	lea    0x25a40(%rip),%r13        # 0x180026d20
-   1800012e0:	lea    0x52a39(%rip),%r14        # 0x180053d20
-   1800012e7:	mov    %ebp,%r11d
-   1800012ea:	nopw   0x0(%rax,%rax,1)
-   1800012f0:	movsbq %cl,%rax
-   1800012f4:	cmp    %bpl,(%rax,%rbx,1)
-   1800012f8:	je     0x180001306
-   1800012fa:	mov    %cl,(%r11,%rdi,1)
-   1800012fe:	mov    %ebp,0x0(%r13,%r11,4)
-   180001303:	inc    %r11d
-   180001306:	inc    %cl
-   180001308:	movsbl %cl,%eax
-   18000130b:	cmp    %r15d,%eax
-   18000130e:	jb     0x1800012f0
-   180001310:	xor    %al,%al
-   180001312:	lea    0x2d27(%rip),%rcx        # 0x180004040
-   180001319:	mov    %al,0x98(%rsp)
-   180001320:	mov    $0x1,%r10d
-   180001326:	mov    %r10d,0x4(%rsp)
-   18000132b:	test   %dl,%dl
-   18000132d:	jle    0x180001514
-   180001333:	mov    %r12,0x48(%rsp)
-   180001338:	movzbl %dl,%r15d
-   18000133c:	mov    %dl,(%rsp)
-   18000133f:	nop
-   180001340:	movzbl %al,%ecx
-   180001343:	xor    %edx,%edx
-   180001345:	mov    %r8d,%eax
-   180001348:	mov    $0x1,%r9d
-   18000134e:	div    %r10d
-   180001351:	shl    %cl,%r9b
-   180001354:	xor    %edx,%edx
-   180001356:	movsbl %r15b,%ecx
-   18000135a:	mov    %ebp,%r8d
-   18000135d:	div    %ecx
-   18000135f:	mov    %r9d,0x8(%rsp)
-   180001364:	mov    %eax,%ebx
-   180001366:	test   %r11d,%r11d
-   180001369:	je     0x1800013b8
-   18000136b:	mov    %rdi,%r9
-   18000136e:	mov    %r13,%r10
-   180001371:	xor    %dl,%dl
-   180001373:	test   %r15b,%r15b
-   180001376:	jle    0x1800013a1
-   180001378:	nopl   0x0(%rax,%rax,1)
-   180001380:	movzbl (%r9),%eax
-   180001384:	mov    %r8d,%ecx
-   180001387:	inc    %r8d
-   18000138a:	mov    %al,(%rcx,%rsi,1)
-   18000138d:	movzbl %dl,%eax
-   180001390:	inc    %dl
-   180001392:	imul   %ebx,%eax
-   180001395:	add    (%r10),%eax
-   180001398:	mov    %eax,(%r14,%rcx,4)
-   18000139c:	cmp    %r15b,%dl
-   18000139f:	jl     0x180001380
-   1800013a1:	inc    %r9
-   1800013a4:	add    $0x4,%r10
-   1800013a8:	sub    $0x1,%r11
-   1800013ac:	jne    0x180001371
-   1800013ae:	mov    0x8(%rsp),%r9d
-   1800013b3:	mov    0x4(%rsp),%r10d
-   1800013b8:	mov    %r13,%rax
-   1800013bb:	mov    %r14,0x10(%rsp)
-   1800013c0:	xor    %r12b,%r12b
-   1800013c3:	mov    %rsi,0x20(%rsp)
-   1800013c8:	mov    %r8d,%r11d
-   1800013cb:	mov    %r14,%r13
-   1800013ce:	mov    %r12b,0x90(%rsp)
-   1800013d6:	mov    %rax,%r14
-   1800013d9:	mov    %rdi,%rax
-   1800013dc:	mov    %rsi,%rdi
-   1800013df:	mov    %rax,%rsi
-   1800013e2:	test   %r9b,%r9b
-   1800013e5:	jle    0x1800014c4
-   1800013eb:	mov    %r13,%r15
-   1800013ee:	xchg   %ax,%ax
-   1800013f0:	mov    %ebp,%eax
-   1800013f2:	mov    $0x1,%r8b
-   1800013f5:	test   %r11d,%r11d
-   1800013f8:	je     0x180001482
-   1800013fe:	movzbl %r12b,%edx
-   180001402:	mov    %r15,%r10
-   180001405:	mov    0x80(%rsp),%r15
-   18000140d:	lea    0x2c2c(%rip),%r12        # 0x180004040
-   180001414:	movsbl %r9b,%ecx
-   180001418:	mov    %rdi,%r9
-   18000141b:	add    %ecx,%edx
-   18000141d:	movslq %edx,%r13
-   180001420:	mov    (%r10),%ebx
-   180001423:	movsbq (%r9),%rdi
-   180001427:	mov    %ebx,%ecx
-   180001429:	shl    $0x6,%rcx
-   18000142d:	add    %r13,%rcx
-   180001430:	movsbq (%rcx,%r12,1),%rdx
-   180001435:	xor    %rdi,%rdx
-   180001438:	movzbl (%rdx,%r15,1),%ecx
-   18000143d:	test   %r8b,%r8b
-   180001440:	je     0x18000144d
-   180001442:	test   %cl,%cl
-   180001444:	je     0x180001451
-   180001446:	xor    %r8b,%r8b
-   180001449:	mov    %ebp,%eax
-   18000144b:	jmp    0x180001451
-   18000144d:	test   %cl,%cl
-   18000144f:	je     0x18000145d
-   180001451:	mov    %eax,%ecx
-   180001453:	inc    %eax
-   180001455:	mov    %dil,(%rcx,%rsi,1)
-   180001459:	mov    %ebx,(%r14,%rcx,4)
-   18000145d:	add    $0x4,%r10
-   180001461:	inc    %r9
-   180001464:	sub    $0x1,%r11
-   180001468:	jne    0x180001420
-   18000146a:	movzbl 0x90(%rsp),%r12d
-   180001473:	mov    0x20(%rsp),%rdi
-   180001478:	mov    0x10(%rsp),%r15
-   18000147d:	mov    0x8(%rsp),%r9d
-   180001482:	mov    %r15,%rcx
-   180001485:	mov    %r14,0x10(%rsp)
-   18000148a:	inc    %r12b
-   18000148d:	mov    %rsi,0x20(%rsp)
-   180001492:	mov    %eax,%r11d
-   180001495:	mov    %r14,%r15
-   180001498:	mov    %r12b,0x90(%rsp)
-   1800014a0:	mov    %rcx,%r14
-   1800014a3:	mov    %rdi,%rcx
-   1800014a6:	mov    %rsi,%rdi
-   1800014a9:	mov    %rcx,%rsi
-   1800014ac:	cmp    %r9b,%r12b
-   1800014af:	jl     0x1800013f0
-   1800014b5:	movzbl (%rsp),%r15d
-   1800014ba:	mov    0x10(%rsp),%r13
-   1800014bf:	mov    0x4(%rsp),%r10d
-   1800014c4:	mov    0xc(%rsp),%r8d
-   1800014c9:	movsbl %r15b,%eax
-   1800014cd:	dec    %r15b
-   1800014d0:	imul   %eax,%r10d
-   1800014d4:	movzbl 0x98(%rsp),%eax
-   1800014dc:	inc    %al
-   1800014de:	mov    %r15b,(%rsp)
-   1800014e2:	mov    %al,0x98(%rsp)
-   1800014e9:	mov    %r10d,0x4(%rsp)
-   1800014ee:	cmp    0x88(%rsp),%al
-   1800014f5:	jl     0x180001340
-   1800014fb:	mov    0x80(%rsp),%rbx
-   180001503:	lea    0x2b36(%rip),%rcx        # 0x180004040
-   18000150a:	mov    0x18(%rsp),%r15d
-   18000150f:	mov    0x48(%rsp),%r12
-   180001514:	mov    0x0(%r13),%r9d
-   180001518:	xor    %r8b,%r8b
-   18000151b:	movsbq (%rdi),%r10
-   18000151f:	mov    %ebp,%edx
-   180001521:	mov    0x38(%rsp),%r14
-   180001526:	mov    0x40(%rsp),%r13
-   18000152b:	mov    0x50(%rsp),%rdi
-   180001530:	mov    0x58(%rsp),%rsi
-   180001535:	shl    $0x6,%r9
-   180001539:	nopl   0x0(%rax)
+   1800011b7:	movzbl 0x80(%rsp),%r9d
+   1800011c0:	mov    0x98(%rsp),%edx
+   1800011c7:	inc    %r15b
+   1800011ca:	inc    %r14
+   1800011cd:	cmp    %r9b,%r15b
+   1800011d0:	jl     0x180001130
+   1800011d6:	subq   $0x1,0x28(%rsp)
+   1800011dc:	jne    0x180001121
+   1800011e2:	mov    0x90(%rsp),%r8d
+   1800011ea:	mov    0x88(%rsp),%r10d
+   1800011f2:	mov    0x20(%rsp),%ecx
+   1800011f6:	imul   %ecx,%r8d
+   1800011fa:	inc    %r13b
+   1800011fd:	mov    %r8d,0x90(%rsp)
+   180001205:	cmp    %r9b,%r13b
+   180001208:	jl     0x1800010e0
+   18000120e:	mov    0x38(%rsp),%r15
+   180001213:	mov    0x40(%rsp),%r14
+   180001218:	mov    0x48(%rsp),%r12
+   18000121d:	mov    0x60(%rsp),%rbp
+   180001222:	mov    0x50(%rsp),%rdi
+   180001227:	mov    %r11,%rax
+   18000122a:	mov    0x58(%rsp),%rsi
+   18000122f:	mov    0x68(%rsp),%rbx
+   180001234:	mov    %r9b,0x7fae5(%rip)        # 0x180080d20
+   18000123b:	add    $0x70,%rsp
+   18000123f:	pop    %r13
+   180001241:	ret
+   180001242:	int3
+   180001243:	int3
+   180001244:	int3
+   180001245:	int3
+   180001246:	int3
+   180001247:	int3
+   180001248:	int3
+   180001249:	int3
+   18000124a:	int3
+   18000124b:	int3
+   18000124c:	int3
+   18000124d:	int3
+   18000124e:	int3
+   18000124f:	int3
+   180001250:	mov    %r9,0x20(%rsp)
+   180001255:	mov    %r8,0x18(%rsp)
+   18000125a:	mov    %dl,0x10(%rsp)
+   18000125e:	mov    %rcx,0x8(%rsp)
+   180001263:	push   %r12
+   180001265:	push   %r13
+   180001267:	sub    $0x68,%rsp
+   18000126b:	mov    %rcx,%r12
+   18000126e:	mov    $0x1,%eax
+   180001273:	movsbl %dl,%ecx
+   180001276:	mov    %ecx,0xc(%rsp)
+   18000127a:	mov    %ecx,%r8d
+   18000127d:	cmp    %eax,%ecx
+   18000127f:	jbe    0x180001290
+   180001281:	imul   %eax,%r8d
+   180001285:	inc    %eax
+   180001287:	cmp    %ecx,%eax
+   180001289:	jb     0x180001281
+   18000128b:	mov    %r8d,0xc(%rsp)
+   180001290:	mov    $0x1,%r13d
+   180001296:	shl    %cl,%r13d
+   180001299:	xor    %cl,%cl
+   18000129b:	mov    %r13d,0x18(%rsp)
+   1800012a0:	test   %r13d,%r13d
+   1800012a3:	je     0x1800012ba
+   1800012a5:	movsbq %cl,%rax
+   1800012a9:	cmpb   $0x0,(%rax,%r12,1)
+   1800012ae:	jne    0x1800012c5
+   1800012b0:	inc    %cl
+   1800012b2:	movsbl %cl,%eax
+   1800012b5:	cmp    %r13d,%eax
+   1800012b8:	jb     0x1800012a5
+   1800012ba:	xor    %eax,%eax
+   1800012bc:	add    $0x68,%rsp
+   1800012c0:	pop    %r13
+   1800012c2:	pop    %r12
+   1800012c4:	ret
+   1800012c5:	mov    %rbx,0x60(%rsp)
+   1800012ca:	mov    %rbp,0x58(%rsp)
+   1800012cf:	xor    %ebp,%ebp
+   1800012d1:	mov    %rsi,0x50(%rsp)
+   1800012d6:	xor    %cl,%cl
+   1800012d8:	mov    %rdi,0x48(%rsp)
+   1800012dd:	lea    0x1a63c(%rip),%rsi        # 0x18001b920
+   1800012e4:	mov    %r14,0x40(%rsp)
+   1800012e9:	lea    0xf230(%rip),%rdi        # 0x180010520
+   1800012f0:	mov    %r15,0x38(%rsp)
+   1800012f5:	lea    0x52a24(%rip),%r14        # 0x180053d20
+   1800012fc:	lea    0x25a1d(%rip),%r15        # 0x180026d20
+   180001303:	mov    %ebp,%r11d
+   180001306:	movsbq %cl,%rax
+   18000130a:	cmp    %bpl,(%rax,%r12,1)
+   18000130e:	je     0x18000131b
+   180001310:	mov    %cl,(%r11,%rdi,1)
+   180001314:	mov    %ebp,(%r15,%r11,4)
+   180001318:	inc    %r11d
+   18000131b:	inc    %cl
+   18000131d:	movsbl %cl,%eax
+   180001320:	cmp    %r13d,%eax
+   180001323:	jb     0x180001306
+   180001325:	xor    %al,%al
+   180001327:	lea    0x2d12(%rip),%rcx        # 0x180004040
+   18000132e:	mov    %al,0x1(%rsp)
+   180001332:	mov    $0x1,%r10d
+   180001338:	mov    %r10d,0x4(%rsp)
+   18000133d:	test   %dl,%dl
+   18000133f:	jle    0x180001513
+   180001345:	movzbl %dl,%r13d
+   180001349:	mov    %dl,0x2(%rsp)
+   18000134d:	nopl   (%rax)
+   180001350:	movzbl %al,%ecx
+   180001353:	xor    %edx,%edx
+   180001355:	mov    %r8d,%eax
+   180001358:	mov    $0x1,%r9d
+   18000135e:	div    %r10d
+   180001361:	shl    %cl,%r9b
+   180001364:	xor    %edx,%edx
+   180001366:	movsbl %r13b,%ecx
+   18000136a:	mov    %ebp,%r8d
+   18000136d:	div    %ecx
+   18000136f:	mov    %r9d,0x8(%rsp)
+   180001374:	mov    %eax,%ebx
+   180001376:	test   %r11d,%r11d
+   180001379:	je     0x1800013c8
+   18000137b:	mov    %rdi,%r9
+   18000137e:	mov    %r15,%r10
+   180001381:	xor    %dl,%dl
+   180001383:	test   %r13b,%r13b
+   180001386:	jle    0x1800013b1
+   180001388:	nopl   0x0(%rax,%rax,1)
+   180001390:	movzbl (%r9),%eax
+   180001394:	mov    %r8d,%ecx
+   180001397:	inc    %r8d
+   18000139a:	mov    %al,(%rcx,%rsi,1)
+   18000139d:	movzbl %dl,%eax
+   1800013a0:	inc    %dl
+   1800013a2:	imul   %ebx,%eax
+   1800013a5:	add    (%r10),%eax
+   1800013a8:	mov    %eax,(%r14,%rcx,4)
+   1800013ac:	cmp    %r13b,%dl
+   1800013af:	jl     0x180001390
+   1800013b1:	inc    %r9
+   1800013b4:	add    $0x4,%r10
+   1800013b8:	sub    $0x1,%r11
+   1800013bc:	jne    0x180001381
+   1800013be:	mov    0x8(%rsp),%r9d
+   1800013c3:	mov    0x4(%rsp),%r10d
+   1800013c8:	mov    %r15,%rax
+   1800013cb:	mov    %r14,0x10(%rsp)
+   1800013d0:	xor    %r12b,%r12b
+   1800013d3:	mov    %rsi,0x20(%rsp)
+   1800013d8:	mov    %r8d,%r11d
+   1800013db:	mov    %r14,%r15
+   1800013de:	mov    %r12b,(%rsp)
+   1800013e2:	mov    %rax,%r14
+   1800013e5:	mov    %rdi,%rax
+   1800013e8:	mov    %rsi,%rdi
+   1800013eb:	mov    %rax,%rsi
+   1800013ee:	test   %r9b,%r9b
+   1800013f1:	jle    0x1800014cd
+   1800013f7:	mov    %r15,%r13
+   1800013fa:	nopw   0x0(%rax,%rax,1)
+   180001400:	mov    %ebp,%eax
+   180001402:	mov    $0x1,%r8b
+   180001405:	test   %r11d,%r11d
+   180001408:	je     0x18000148e
+   18000140e:	movzbl %r12b,%edx
+   180001412:	mov    %r13,%r10
+   180001415:	mov    0x80(%rsp),%r13
+   18000141d:	lea    0x2c1c(%rip),%r12        # 0x180004040
+   180001424:	movsbl %r9b,%ecx
+   180001428:	mov    %rdi,%r9
+   18000142b:	add    %ecx,%edx
+   18000142d:	movslq %edx,%r15
+   180001430:	mov    (%r10),%ebx
+   180001433:	movsbq (%r9),%rdi
+   180001437:	mov    %ebx,%ecx
+   180001439:	shl    $0x6,%rcx
+   18000143d:	add    %r15,%rcx
+   180001440:	movsbq (%rcx,%r12,1),%rdx
+   180001445:	xor    %rdi,%rdx
+   180001448:	movzbl (%rdx,%r13,1),%ecx
+   18000144d:	test   %r8b,%r8b
+   180001450:	je     0x18000145d
+   180001452:	test   %cl,%cl
+   180001454:	je     0x180001461
+   180001456:	xor    %r8b,%r8b
+   180001459:	mov    %ebp,%eax
+   18000145b:	jmp    0x180001461
+   18000145d:	test   %cl,%cl
+   18000145f:	je     0x18000146d
+   180001461:	mov    %eax,%ecx
+   180001463:	inc    %eax
+   180001465:	mov    %dil,(%rcx,%rsi,1)
+   180001469:	mov    %ebx,(%r14,%rcx,4)
+   18000146d:	add    $0x4,%r10
+   180001471:	inc    %r9
+   180001474:	sub    $0x1,%r11
+   180001478:	jne    0x180001430
+   18000147a:	movzbl (%rsp),%r12d
+   18000147f:	mov    0x20(%rsp),%rdi
+   180001484:	mov    0x10(%rsp),%r13
+   180001489:	mov    0x8(%rsp),%r9d
+   18000148e:	mov    %r13,%rcx
+   180001491:	mov    %r14,0x10(%rsp)
+   180001496:	inc    %r12b
+   180001499:	mov    %rsi,0x20(%rsp)
+   18000149e:	mov    %eax,%r11d
+   1800014a1:	mov    %r14,%r13
+   1800014a4:	mov    %r12b,(%rsp)
+   1800014a8:	mov    %rcx,%r14
+   1800014ab:	mov    %rdi,%rcx
+   1800014ae:	mov    %rsi,%rdi
+   1800014b1:	mov    %rcx,%rsi
+   1800014b4:	cmp    %r9b,%r12b
+   1800014b7:	jl     0x180001400
+   1800014bd:	movzbl 0x2(%rsp),%r13d
+   1800014c3:	mov    0x10(%rsp),%r15
+   1800014c8:	mov    0x4(%rsp),%r10d
+   1800014cd:	mov    0xc(%rsp),%r8d
+   1800014d2:	movsbl %r13b,%eax
+   1800014d6:	dec    %r13b
+   1800014d9:	imul   %eax,%r10d
+   1800014dd:	movzbl 0x1(%rsp),%eax
+   1800014e2:	inc    %al
+   1800014e4:	mov    %r13b,0x2(%rsp)
+   1800014e9:	mov    %al,0x1(%rsp)
+   1800014ed:	mov    %r10d,0x4(%rsp)
+   1800014f2:	cmp    0x88(%rsp),%al
+   1800014f9:	jl     0x180001350
+   1800014ff:	mov    0x80(%rsp),%r12
+   180001507:	lea    0x2b32(%rip),%rcx        # 0x180004040
+   18000150e:	mov    0x18(%rsp),%r13d
+   180001513:	mov    (%r15),%ebx
+   180001516:	xor    %r8b,%r8b
+   180001519:	movsbq (%rdi),%r11
+   18000151d:	mov    %ebx,%r9d
+   180001520:	mov    0x38(%rsp),%r15
+   180001525:	mov    %ebp,%edx
+   180001527:	mov    0x40(%rsp),%r14
+   18000152c:	mov    0x48(%rsp),%rdi
+   180001531:	mov    0x50(%rsp),%rsi
+   180001536:	shl    $0x6,%r9
+   18000153a:	nopw   0x0(%rax,%rax,1)
    180001540:	movsbq %r8b,%rax
    180001544:	add    %r9,%rax
    180001547:	movsbq (%rax,%rcx,1),%rax
-   18000154c:	xor    %r10,%rax
-   18000154f:	cmpb   $0x0,(%rax,%rbx,1)
-   180001553:	je     0x18000156e
-   180001555:	mov    %r15d,%ecx
-   180001558:	sub    %edx,%ecx
-   18000155a:	mov    $0x1,%edx
-   18000155f:	dec    %ecx
-   180001561:	shl    %cl,%rdx
-   180001564:	lea    0x2ad5(%rip),%rcx        # 0x180004040
-   18000156b:	add    %rdx,%rbp
-   18000156e:	inc    %r8b
-   180001571:	movsbl %r8b,%edx
-   180001575:	cmp    %r15d,%edx
-   180001578:	jb     0x180001540
-   18000157a:	mov    %rbp,%rax
-   18000157d:	mov    0x60(%rsp),%rbp
-   180001582:	add    $0x68,%rsp
-   180001586:	pop    %r15
-   180001588:	pop    %rbx
-   180001589:	ret
-   18000158a:	int3
-   18000158b:	int3
-   18000158c:	int3
-   18000158d:	int3
-   18000158e:	int3
-   18000158f:	int3
-   180001590:	mov    %dl,0x10(%rsp)
-   180001594:	mov    %rcx,0x8(%rsp)
-   180001599:	push   %rbx
-   18000159a:	push   %rbp
-   18000159b:	push   %r15
-   18000159d:	sub    $0x90,%rsp
-   1800015a4:	mov    %r12,0x78(%rsp)
-   1800015a9:	mov    %rcx,%rbx
-   1800015ac:	movsbl %dl,%r12d
-   1800015b0:	movzbl %r12b,%edx
-   1800015b4:	call   0x180001240
-   1800015b9:	mov    %r12d,%ecx
-   1800015bc:	mov    %rax,0x50(%rsp)
-   1800015c1:	mov    $0x1,%r15d
-   1800015c7:	xor    %dl,%dl
-   1800015c9:	shl    %cl,%r15d
-   1800015cc:	mov    %rax,%r10
-   1800015cf:	mov    %r15d,0x3c(%rsp)
-   1800015d4:	test   %r15d,%r15d
-   1800015d7:	jle    0x1800015f8
-   1800015d9:	nopl   0x0(%rax)
-   1800015e0:	movsbq %dl,%rcx
-   1800015e4:	cmpb   $0x0,(%rcx,%rbx,1)
-   1800015e8:	sete   %al
-   1800015eb:	inc    %dl
-   1800015ed:	mov    %al,(%rcx,%rbx,1)
-   1800015f0:	movsbl %dl,%eax
-   1800015f3:	cmp    %r15d,%eax
-   1800015f6:	jl     0x1800015e0
-   1800015f8:	mov    $0x1,%eax
-   1800015fd:	mov    %r12d,0x28(%rsp)
-   180001602:	mov    %r12d,%r9d
-   180001605:	cmp    %eax,%r12d
-   180001608:	jbe    0x180001620
-   18000160a:	nopw   0x0(%rax,%rax,1)
-   180001610:	imul   %eax,%r9d
-   180001614:	inc    %eax
-   180001616:	cmp    %r12d,%eax
-   180001619:	jb     0x180001610
-   18000161b:	mov    %r9d,0x28(%rsp)
-   180001620:	xor    %cl,%cl
-   180001622:	test   %r15d,%r15d
-   180001625:	je     0x180001644
-   180001627:	nopw   0x0(%rax,%rax,1)
-   180001630:	movsbq %cl,%rax
-   180001634:	cmpb   $0x0,(%rax,%rbx,1)
-   180001638:	jne    0x18000168e
-   18000163a:	inc    %cl
-   18000163c:	movsbl %cl,%eax
-   18000163f:	cmp    %r15d,%eax
-   180001642:	jb     0x180001630
-   180001644:	xor    %ebp,%ebp
-   180001646:	mov    0x78(%rsp),%r12
-   18000164b:	xor    %dl,%dl
-   18000164d:	test   %r15d,%r15d
-   180001650:	jle    0x180001678
-   180001652:	nopl   0x0(%rax)
-   180001656:	data16 nopw 0x0(%rax,%rax,1)
-   180001660:	movsbq %dl,%rax
-   180001664:	cmpb   $0x0,(%rax,%rbx,1)
-   180001668:	sete   %cl
-   18000166b:	inc    %dl
-   18000166d:	mov    %cl,(%rax,%rbx,1)
-   180001670:	movsbl %dl,%ecx
-   180001673:	cmp    %r15d,%ecx
-   180001676:	jl     0x180001660
-   180001678:	cmp    %rbp,%r10
-   18000167b:	cmova  %r10,%rbp
-   18000167f:	mov    %rbp,%rax
-   180001682:	add    $0x90,%rsp
-   180001689:	pop    %r15
-   18000168b:	pop    %rbp
-   18000168c:	pop    %rbx
-   18000168d:	ret
-   18000168e:	mov    %rsi,0x88(%rsp)
-   180001696:	lea    0x25683(%rip),%r10        # 0x180026d20
-   18000169d:	mov    %rdi,0x80(%rsp)
-   1800016a5:	lea    0x1a274(%rip),%rsi        # 0x18001b920
-   1800016ac:	xor    %ebp,%ebp
-   1800016ae:	mov    %r14,0x68(%rsp)
-   1800016b3:	lea    0x52666(%rip),%r14        # 0x180053d20
-   1800016ba:	mov    %r10,0x30(%rsp)
-   1800016bf:	lea    0xee5a(%rip),%rdi        # 0x180010520
-   1800016c6:	mov    %ebp,%r11d
-   1800016c9:	xor    %cl,%cl
-   1800016cb:	nopl   0x0(%rax,%rax,1)
-   1800016d0:	movsbq %cl,%rax
-   1800016d4:	cmp    %bpl,(%rax,%rbx,1)
-   1800016d8:	je     0x1800016e5
-   1800016da:	mov    %cl,(%r11,%rdi,1)
-   1800016de:	mov    %ebp,(%r10,%r11,4)
-   1800016e2:	inc    %r11d
-   1800016e5:	inc    %cl
-   1800016e7:	movsbl %cl,%eax
-   1800016ea:	cmp    %r15d,%eax
-   1800016ed:	jb     0x1800016d0
-   1800016ef:	xor    %al,%al
-   1800016f1:	lea    0x2948(%rip),%rcx        # 0x180004040
-   1800016f8:	mov    %al,0xc8(%rsp)
-   1800016ff:	mov    $0x1,%r8d
-   180001705:	mov    %r8d,0x24(%rsp)
-   18000170a:	test   %r12b,%r12b
-   18000170d:	jle    0x1800018f1
-   180001713:	mov    %r13,0x70(%rsp)
-   180001718:	movzbl %r12b,%r13d
-   18000171c:	mov    %r12b,0x20(%rsp)
-   180001721:	movzbl %al,%ecx
-   180001724:	xor    %edx,%edx
-   180001726:	mov    %r9d,%eax
-   180001729:	mov    $0x1,%r15d
-   18000172f:	div    %r8d
-   180001732:	shl    %cl,%r15b
-   180001735:	xor    %edx,%edx
-   180001737:	movsbl %r13b,%ecx
-   18000173b:	mov    %ebp,%r8d
-   18000173e:	div    %ecx
-   180001740:	mov    %r15d,0x38(%rsp)
-   180001745:	mov    %eax,%ebx
-   180001747:	test   %r11d,%r11d
-   18000174a:	je     0x180001793
-   18000174c:	mov    %rdi,%r9
-   18000174f:	nop
-   180001750:	xor    %dl,%dl
-   180001752:	test   %r13b,%r13b
-   180001755:	jle    0x180001781
-   180001757:	nopw   0x0(%rax,%rax,1)
-   180001760:	movzbl (%r9),%eax
-   180001764:	mov    %r8d,%ecx
-   180001767:	inc    %r8d
-   18000176a:	mov    %al,(%rcx,%rsi,1)
-   18000176d:	movzbl %dl,%eax
-   180001770:	inc    %dl
-   180001772:	imul   %ebx,%eax
-   180001775:	add    (%r10),%eax
-   180001778:	mov    %eax,(%r14,%rcx,4)
-   18000177c:	cmp    %r13b,%dl
-   18000177f:	jl     0x180001760
-   180001781:	inc    %r9
-   180001784:	add    $0x4,%r10
-   180001788:	sub    $0x1,%r11
-   18000178c:	jne    0x180001750
-   18000178e:	mov    0x30(%rsp),%r10
-   180001793:	mov    %r10,%rax
-   180001796:	mov    %r14,0x30(%rsp)
-   18000179b:	xor    %r12b,%r12b
-   18000179e:	mov    %rsi,0x40(%rsp)
-   1800017a3:	mov    %r8d,%r11d
-   1800017a6:	mov    %r14,%r10
-   1800017a9:	mov    %r12b,0xc0(%rsp)
-   1800017b1:	mov    %rax,%r14
-   1800017b4:	mov    %rdi,%rax
-   1800017b7:	mov    %rsi,%rdi
-   1800017ba:	mov    %rax,%rsi
-   1800017bd:	test   %r15b,%r15b
-   1800017c0:	jle    0x18000189b
-   1800017c6:	mov    0xb0(%rsp),%r13
-   1800017ce:	xchg   %ax,%ax
-   1800017d0:	mov    %ebp,%eax
-   1800017d2:	mov    $0x1,%r8b
-   1800017d5:	test   %r11d,%r11d
-   1800017d8:	je     0x180001862
-   1800017de:	movzbl %r12b,%edx
-   1800017e2:	mov    %rdi,%r9
-   1800017e5:	movsbl %r15b,%ecx
-   1800017e9:	lea    0x2850(%rip),%r12        # 0x180004040
-   1800017f0:	add    %ecx,%edx
-   1800017f2:	movslq %edx,%r15
-   1800017f5:	data16 data16 nopw 0x0(%rax,%rax,1)
-   180001800:	mov    (%r10),%ebx
-   180001803:	movsbq (%r9),%rdi
-   180001807:	mov    %ebx,%ecx
-   180001809:	shl    $0x6,%rcx
-   18000180d:	add    %r15,%rcx
-   180001810:	movsbq (%rcx,%r12,1),%rdx
-   180001815:	xor    %rdi,%rdx
-   180001818:	movzbl (%rdx,%r13,1),%ecx
-   18000181d:	test   %r8b,%r8b
-   180001820:	je     0x18000182d
-   180001822:	test   %cl,%cl
-   180001824:	je     0x180001831
-   180001826:	xor    %r8b,%r8b
-   180001829:	mov    %ebp,%eax
-   18000182b:	jmp    0x180001831
-   18000182d:	test   %cl,%cl
-   18000182f:	je     0x18000183d
-   180001831:	mov    %eax,%ecx
-   180001833:	inc    %eax
-   180001835:	mov    %dil,(%rcx,%rsi,1)
-   180001839:	mov    %ebx,(%r14,%rcx,4)
-   18000183d:	add    $0x4,%r10
-   180001841:	inc    %r9
-   180001844:	sub    $0x1,%r11
-   180001848:	jne    0x180001800
-   18000184a:	movzbl 0xc0(%rsp),%r12d
-   180001853:	mov    0x40(%rsp),%rdi
-   180001858:	mov    0x30(%rsp),%r10
-   18000185d:	mov    0x38(%rsp),%r15d
-   180001862:	mov    %r10,%rcx
-   180001865:	mov    %r14,0x30(%rsp)
-   18000186a:	inc    %r12b
-   18000186d:	mov    %rsi,0x40(%rsp)
-   180001872:	mov    %eax,%r11d
-   180001875:	mov    %r14,%r10
-   180001878:	mov    %r12b,0xc0(%rsp)
-   180001880:	mov    %rcx,%r14
-   180001883:	mov    %rdi,%rcx
-   180001886:	mov    %rsi,%rdi
-   180001889:	mov    %rcx,%rsi
-   18000188c:	cmp    %r15b,%r12b
-   18000188f:	jl     0x1800017d0
-   180001895:	movzbl 0x20(%rsp),%r13d
-   18000189b:	mov    0x24(%rsp),%r8d
-   1800018a0:	mov    0x28(%rsp),%r9d
-   1800018a5:	movsbl %r13b,%eax
-   1800018a9:	dec    %r13b
-   1800018ac:	imul   %eax,%r8d
-   1800018b0:	movzbl 0xc8(%rsp),%eax
-   1800018b8:	inc    %al
-   1800018ba:	mov    %r13b,0x20(%rsp)
-   1800018bf:	mov    %al,0xc8(%rsp)
-   1800018c6:	mov    %r8d,0x24(%rsp)
-   1800018cb:	cmp    0xb8(%rsp),%al
-   1800018d2:	jl     0x180001721
-   1800018d8:	mov    0xb0(%rsp),%rbx
-   1800018e0:	lea    0x2759(%rip),%rcx        # 0x180004040
-   1800018e7:	mov    0x3c(%rsp),%r15d
-   1800018ec:	mov    0x70(%rsp),%r13
-   1800018f1:	mov    (%r10),%r9d
-   1800018f4:	xor    %dl,%dl
-   1800018f6:	movsbq (%rdi),%r10
-   1800018fa:	mov    %ebp,%r8d
-   1800018fd:	mov    0x80(%rsp),%rdi
-   180001905:	mov    0x68(%rsp),%r14
-   18000190a:	mov    0x88(%rsp),%rsi
-   180001912:	shl    $0x6,%r9
-   180001916:	data16 nopw 0x0(%rax,%rax,1)
-   180001920:	movsbq %dl,%rax
-   180001924:	add    %r9,%rax
-   180001927:	movsbq (%rax,%rcx,1),%rax
-   18000192c:	xor    %r10,%rax
-   18000192f:	cmpb   $0x0,(%rax,%rbx,1)
-   180001933:	je     0x18000194f
-   180001935:	mov    %r15d,%ecx
-   180001938:	mov    $0x1,%eax
-   18000193d:	sub    %r8d,%ecx
-   180001940:	dec    %ecx
-   180001942:	shl    %cl,%rax
-   180001945:	lea    0x26f4(%rip),%rcx        # 0x180004040
-   18000194c:	add    %rax,%rbp
-   18000194f:	inc    %dl
-   180001951:	movsbl %dl,%r8d
-   180001955:	cmp    %r15d,%r8d
-   180001958:	jb     0x180001920
-   18000195a:	mov    0x50(%rsp),%r10
-   18000195f:	jmp    0x180001646
-   180001964:	sub    $0x28,%rsp
-   180001968:	test   %edx,%edx
-   18000196a:	je     0x1800019a5
-   18000196c:	sub    $0x1,%edx
-   18000196f:	je     0x180001999
-   180001971:	sub    $0x1,%edx
-   180001974:	je     0x18000198c
-   180001976:	cmp    $0x1,%edx
-   180001979:	je     0x180001985
-   18000197b:	mov    $0x1,%eax
-   180001980:	add    $0x28,%rsp
-   180001984:	ret
-   180001985:	call   0x180001e8c
-   18000198a:	jmp    0x180001991
-   18000198c:	call   0x180001e64
-   180001991:	movzbl %al,%eax
-   180001994:	add    $0x28,%rsp
-   180001998:	ret
-   180001999:	mov    %r8,%rdx
-   18000199c:	add    $0x28,%rsp
-   1800019a0:	jmp    0x1800019b4
-   1800019a5:	test   %r8,%r8
-   1800019a8:	setne  %cl
-   1800019ab:	add    $0x28,%rsp
-   1800019af:	jmp    0x180001acc
-   1800019b4:	mov    %rbx,0x8(%rsp)
-   1800019b9:	mov    %rsi,0x10(%rsp)
-   1800019be:	mov    %rdi,0x20(%rsp)
-   1800019c3:	push   %r14
-   1800019c5:	sub    $0x20,%rsp
-   1800019c9:	mov    %rdx,%rsi
-   1800019cc:	mov    %rcx,%r14
-   1800019cf:	xor    %ecx,%ecx
-   1800019d1:	call   0x180001f48
-   1800019d6:	test   %al,%al
-   1800019d8:	je     0x180001aa6
-   1800019de:	call   0x180001ddc
-   1800019e3:	mov    %al,%bl
-   1800019e5:	mov    %al,0x40(%rsp)
-   1800019e9:	mov    $0x1,%dil
-   1800019ec:	cmpl   $0x0,0x7f35d(%rip)        # 0x180080d50
-   1800019f3:	jne    0x180001abe
-   1800019f9:	movl   $0x1,0x7f34d(%rip)        # 0x180080d50
-   180001a03:	call   0x180001e4c
-   180001a08:	test   %al,%al
-   180001a0a:	je     0x180001a5b
-   180001a0c:	call   0x180002264
-   180001a11:	call   0x180001d94
-   180001a16:	call   0x180001dc0
-   180001a1b:	lea    0x170e(%rip),%rdx        # 0x180003130
-   180001a22:	lea    0x16ff(%rip),%rcx        # 0x180003128
-   180001a29:	call   0x1800024b8
-   180001a2e:	test   %eax,%eax
-   180001a30:	jne    0x180001a5b
-   180001a32:	call   0x180001e18
-   180001a37:	test   %al,%al
-   180001a39:	je     0x180001a5b
-   180001a3b:	lea    0x16de(%rip),%rdx        # 0x180003120
-   180001a42:	lea    0x16cf(%rip),%rcx        # 0x180003118
-   180001a49:	call   0x1800024b2
-   180001a4e:	movl   $0x2,0x7f2f8(%rip)        # 0x180080d50
-   180001a58:	xor    %dil,%dil
-   180001a5b:	mov    %bl,%cl
-   180001a5d:	call   0x1800020b8
-   180001a62:	test   %dil,%dil
-   180001a65:	jne    0x180001aa6
-   180001a67:	call   0x180002108
-   180001a6c:	mov    %rax,%rbx
-   180001a6f:	cmpq   $0x0,(%rax)
-   180001a73:	je     0x180001a99
-   180001a75:	mov    %rax,%rcx
-   180001a78:	call   0x180002020
-   180001a7d:	test   %al,%al
-   180001a7f:	je     0x180001a99
-   180001a81:	mov    %rsi,%r8
-   180001a84:	mov    $0x2,%edx
-   180001a89:	mov    %r14,%rcx
-   180001a8c:	mov    (%rbx),%rax
-   180001a8f:	mov    0x165a(%rip),%r9        # 0x1800030f0
-   180001a96:	call   *%r9
-   180001a99:	incl   0x7f281(%rip)        # 0x180080d20
-   180001a9f:	mov    $0x1,%eax
-   180001aa4:	jmp    0x180001aa8
-   180001aa6:	xor    %eax,%eax
-   180001aa8:	mov    0x30(%rsp),%rbx
-   180001aad:	mov    0x38(%rsp),%rsi
-   180001ab2:	mov    0x48(%rsp),%rdi
-   180001ab7:	add    $0x20,%rsp
-   180001abb:	pop    %r14
-   180001abd:	ret
-   180001abe:	mov    $0x7,%ecx
-   180001ac3:	call   0x180002118
-   180001ac8:	nop
-   180001ac9:	int3
-   180001aca:	int3
-   180001acb:	int3
-   180001acc:	mov    %rbx,0x8(%rsp)
-   180001ad1:	push   %rdi
-   180001ad2:	sub    $0x30,%rsp
-   180001ad6:	mov    %cl,%dil
-   180001ad9:	mov    0x7f241(%rip),%eax        # 0x180080d20
-   180001adf:	test   %eax,%eax
-   180001ae1:	jg     0x180001af0
-   180001ae3:	xor    %eax,%eax
-   180001ae5:	mov    0x40(%rsp),%rbx
-   180001aea:	add    $0x30,%rsp
-   180001aee:	pop    %rdi
-   180001aef:	ret
-   180001af0:	dec    %eax
-   180001af2:	mov    %eax,0x7f228(%rip)        # 0x180080d20
-   180001af8:	call   0x180001ddc
-   180001afd:	mov    %al,%bl
-   180001aff:	mov    %al,0x20(%rsp)
-   180001b03:	cmpl   $0x2,0x7f246(%rip)        # 0x180080d50
-   180001b0a:	jne    0x180001b43
-   180001b0c:	call   0x180001f04
-   180001b11:	call   0x180001da4
-   180001b16:	call   0x1800022a0
-   180001b1b:	andl   $0x0,0x7f22e(%rip)        # 0x180080d50
-   180001b22:	mov    %bl,%cl
-   180001b24:	call   0x1800020b8
-   180001b29:	xor    %edx,%edx
-   180001b2b:	mov    %dil,%cl
-   180001b2e:	call   0x1800020dc
-   180001b33:	neg    %al
-   180001b35:	sbb    %ebx,%ebx
-   180001b37:	and    $0x1,%ebx
-   180001b3a:	call   0x180001f34
-   180001b3f:	mov    %ebx,%eax
-   180001b41:	jmp    0x180001ae5
-   180001b43:	mov    $0x7,%ecx
-   180001b48:	call   0x180002118
-   180001b4d:	nop
-   180001b4e:	nop
-   180001b4f:	int3
-   180001b50:	mov    %rsp,%rax
-   180001b53:	mov    %rbx,0x20(%rax)
-   180001b57:	mov    %r8,0x18(%rax)
-   180001b5b:	mov    %edx,0x10(%rax)
-   180001b5e:	mov    %rcx,0x8(%rax)
-   180001b62:	push   %rsi
-   180001b63:	push   %rdi
-   180001b64:	push   %r14
-   180001b66:	sub    $0x40,%rsp
-   180001b6a:	mov    %r8,%rsi
-   180001b6d:	mov    %edx,%edi
-   180001b6f:	mov    %rcx,%r14
-   180001b72:	test   %edx,%edx
-   180001b74:	jne    0x180001b85
-   180001b76:	cmp    %edx,0x7f1a4(%rip)        # 0x180080d20
-   180001b7c:	jg     0x180001b85
-   180001b7e:	xor    %eax,%eax
-   180001b80:	jmp    0x180001c73
-   180001b85:	lea    -0x1(%rdx),%eax
-   180001b88:	cmp    $0x1,%eax
-   180001b8b:	ja     0x180001bd2
-   180001b8d:	mov    0x15d4(%rip),%rax        # 0x180003168
-   180001b94:	test   %rax,%rax
-   180001b97:	jne    0x180001ba3
-   180001b99:	movl   $0x1,0x30(%rsp)
-   180001ba1:	jmp    0x180001bb7
-   180001ba3:	call   *0x1547(%rip)        # 0x1800030f0
-   180001ba9:	mov    %eax,%ebx
-   180001bab:	mov    %eax,0x30(%rsp)
-   180001baf:	test   %eax,%eax
-   180001bb1:	je     0x180001c69
-   180001bb7:	mov    %rsi,%r8
-   180001bba:	mov    %edi,%edx
-   180001bbc:	mov    %r14,%rcx
-   180001bbf:	call   0x180001964
-   180001bc4:	mov    %eax,%ebx
-   180001bc6:	mov    %eax,0x30(%rsp)
-   180001bca:	test   %eax,%eax
-   180001bcc:	je     0x180001c69
-   180001bd2:	mov    %rsi,%r8
-   180001bd5:	mov    %edi,%edx
-   180001bd7:	mov    %r14,%rcx
-   180001bda:	call   0x180001d70
-   180001bdf:	mov    %eax,%ebx
-   180001be1:	mov    %eax,0x30(%rsp)
-   180001be5:	cmp    $0x1,%edi
-   180001be8:	jne    0x180001c20
-   180001bea:	test   %eax,%eax
-   180001bec:	jne    0x180001c20
-   180001bee:	mov    %rsi,%r8
-   180001bf1:	xor    %edx,%edx
-   180001bf3:	mov    %r14,%rcx
-   180001bf6:	call   0x180001d70
-   180001bfb:	test   %rsi,%rsi
-   180001bfe:	setne  %cl
-   180001c01:	call   0x180001acc
-   180001c06:	mov    0x155b(%rip),%rax        # 0x180003168
-   180001c0d:	test   %rax,%rax
-   180001c10:	je     0x180001c20
-   180001c12:	mov    %rsi,%r8
-   180001c15:	xor    %edx,%edx
-   180001c17:	mov    %r14,%rcx
-   180001c1a:	call   *0x14d0(%rip)        # 0x1800030f0
-   180001c20:	test   %edi,%edi
-   180001c22:	je     0x180001c29
-   180001c24:	cmp    $0x3,%edi
-   180001c27:	jne    0x180001c69
-   180001c29:	mov    %rsi,%r8
-   180001c2c:	mov    %edi,%edx
-   180001c2e:	mov    %r14,%rcx
-   180001c31:	call   0x180001964
-   180001c36:	mov    %eax,%ebx
-   180001c38:	mov    %eax,0x30(%rsp)
-   180001c3c:	test   %eax,%eax
-   180001c3e:	je     0x180001c69
-   180001c40:	mov    0x1521(%rip),%rax        # 0x180003168
-   180001c47:	test   %rax,%rax
-   180001c4a:	jne    0x180001c55
-   180001c4c:	lea    0x1(%rax),%ebx
-   180001c4f:	mov    %ebx,0x30(%rsp)
-   180001c53:	jmp    0x180001c69
-   180001c55:	mov    %rsi,%r8
-   180001c58:	mov    %edi,%edx
-   180001c5a:	mov    %r14,%rcx
-   180001c5d:	call   *0x148d(%rip)        # 0x1800030f0
-   180001c63:	mov    %eax,%ebx
-   180001c65:	mov    %eax,0x30(%rsp)
-   180001c69:	jmp    0x180001c71
-   180001c6b:	xor    %ebx,%ebx
-   180001c6d:	mov    %ebx,0x30(%rsp)
-   180001c71:	mov    %ebx,%eax
-   180001c73:	mov    0x78(%rsp),%rbx
-   180001c78:	add    $0x40,%rsp
-   180001c7c:	pop    %r14
-   180001c7e:	pop    %rdi
-   180001c7f:	pop    %rsi
-   180001c80:	ret
-   180001c81:	int3
-   180001c82:	int3
-   180001c83:	int3
-   180001c84:	mov    %rbx,0x8(%rsp)
-   180001c89:	mov    %rsi,0x10(%rsp)
-   180001c8e:	push   %rdi
-   180001c8f:	sub    $0x20,%rsp
-   180001c93:	mov    %r8,%rdi
-   180001c96:	mov    %edx,%ebx
-   180001c98:	mov    %rcx,%rsi
-   180001c9b:	cmp    $0x1,%edx
-   180001c9e:	jne    0x180001ca5
-   180001ca0:	call   0x180001cc4
-   180001ca5:	mov    %rdi,%r8
-   180001ca8:	mov    %ebx,%edx
-   180001caa:	mov    %rsi,%rcx
-   180001cad:	mov    0x30(%rsp),%rbx
-   180001cb2:	mov    0x38(%rsp),%rsi
-   180001cb7:	add    $0x20,%rsp
-   180001cbb:	pop    %rdi
-   180001cbc:	jmp    0x180001b50
-   180001cc1:	int3
-   180001cc2:	int3
-   180001cc3:	int3
-   180001cc4:	mov    %rbx,0x20(%rsp)
-   180001cc9:	push   %rbp
-   180001cca:	mov    %rsp,%rbp
-   180001ccd:	sub    $0x20,%rsp
-   180001cd1:	mov    0x2338(%rip),%rax        # 0x180004010
-   180001cd8:	movabs $0x2b992ddfa232,%rbx
-   180001ce2:	cmp    %rbx,%rax
-   180001ce5:	jne    0x180001d5b
-   180001ce7:	andq   $0x0,0x18(%rbp)
-   180001cec:	lea    0x18(%rbp),%rcx
-   180001cf0:	call   *0x1322(%rip)        # 0x180003018
-   180001cf6:	mov    0x18(%rbp),%rax
-   180001cfa:	mov    %rax,0x10(%rbp)
-   180001cfe:	call   *0x1344(%rip)        # 0x180003048
-   180001d04:	mov    %eax,%eax
-   180001d06:	xor    %rax,0x10(%rbp)
-   180001d0a:	call   *0x12f8(%rip)        # 0x180003008
-   180001d10:	mov    %eax,%eax
-   180001d12:	lea    0x20(%rbp),%rcx
-   180001d16:	xor    %rax,0x10(%rbp)
-   180001d1a:	call   *0x12f0(%rip)        # 0x180003010
-   180001d20:	mov    0x20(%rbp),%eax
-   180001d23:	lea    0x10(%rbp),%rcx
-   180001d27:	shl    $0x20,%rax
-   180001d2b:	xor    0x20(%rbp),%rax
-   180001d2f:	xor    0x10(%rbp),%rax
-   180001d33:	xor    %rcx,%rax
-   180001d36:	movabs $0xffffffffffff,%rcx
-   180001d40:	and    %rcx,%rax
-   180001d43:	movabs $0x2b992ddfa233,%rcx
-   180001d4d:	cmp    %rbx,%rax
-   180001d50:	cmove  %rcx,%rax
-   180001d54:	mov    %rax,0x22b5(%rip)        # 0x180004010
-   180001d5b:	mov    0x48(%rsp),%rbx
-   180001d60:	not    %rax
-   180001d63:	mov    %rax,0x229e(%rip)        # 0x180004008
-   180001d6a:	add    $0x20,%rsp
-   180001d6e:	pop    %rbp
-   180001d6f:	ret
-   180001d70:	sub    $0x28,%rsp
-   180001d74:	cmp    $0x1,%edx
-   180001d77:	jne    0x180001d89
-   180001d79:	cmpq   $0x0,0x13e7(%rip)        # 0x180003168
-   180001d81:	jne    0x180001d89
-   180001d83:	call   *0x1297(%rip)        # 0x180003020
-   180001d89:	mov    $0x1,%eax
-   180001d8e:	add    $0x28,%rsp
-   180001d92:	ret
-   180001d93:	int3
-   180001d94:	lea    0x7ef95(%rip),%rcx        # 0x180080d30
-   180001d9b:	rex.W jmp *0x1286(%rip)        # 0x180003028
-   180001da2:	int3
-   180001da3:	int3
-   180001da4:	lea    0x7ef85(%rip),%rcx        # 0x180080d30
-   180001dab:	jmp    0x1800024ac
-   180001db0:	lea    0x7ef89(%rip),%rax        # 0x180080d40
-   180001db7:	ret
-   180001db8:	lea    0x7ef89(%rip),%rax        # 0x180080d48
-   180001dbf:	ret
-   180001dc0:	sub    $0x28,%rsp
-   180001dc4:	call   0x180001db0
-   180001dc9:	orq    $0x24,(%rax)
-   180001dcd:	call   0x180001db8
-   180001dd2:	orq    $0x2,(%rax)
-   180001dd6:	add    $0x28,%rsp
-   180001dda:	ret
-   180001ddb:	int3
-   180001ddc:	sub    $0x28,%rsp
-   180001de0:	call   0x180002494
-   180001de5:	test   %eax,%eax
-   180001de7:	je     0x180001e0a
-   180001de9:	mov    %gs:0x30,%rax
-   180001df2:	mov    0x8(%rax),%rcx
-   180001df6:	jmp    0x180001dfd
-   180001df8:	cmp    %rax,%rcx
-   180001dfb:	je     0x180001e11
-   180001dfd:	xor    %eax,%eax
-   180001dff:	lock cmpxchg %rcx,0x7ef50(%rip)        # 0x180080d58
-   180001e08:	jne    0x180001df8
-   180001e0a:	xor    %al,%al
-   180001e0c:	add    $0x28,%rsp
-   180001e10:	ret
-   180001e11:	mov    $0x1,%al
-   180001e13:	jmp    0x180001e0c
-   180001e15:	int3
-   180001e16:	int3
-   180001e17:	int3
+   18000154c:	xor    %r11,%rax
+   18000154f:	cmpb   $0x0,(%rax,%r12,1)
+   180001554:	je     0x18000156f
+   180001556:	mov    %r13d,%ecx
+   180001559:	sub    %edx,%ecx
+   18000155b:	mov    $0x1,%edx
+   180001560:	dec    %ecx
+   180001562:	shl    %cl,%rdx
+   180001565:	lea    0x2ad4(%rip),%rcx        # 0x180004040
+   18000156c:	add    %rdx,%rbp
+   18000156f:	inc    %r8b
+   180001572:	movsbl %r8b,%edx
+   180001576:	cmp    %r13d,%edx
+   180001579:	jb     0x180001540
+   18000157b:	mov    0x90(%rsp),%rax
+   180001583:	mov    %r11b,(%rax)
+   180001586:	mov    0x98(%rsp),%rax
+   18000158e:	mov    %ebx,(%rax)
+   180001590:	mov    %rbp,%rax
+   180001593:	mov    0x58(%rsp),%rbp
+   180001598:	mov    0x60(%rsp),%rbx
+   18000159d:	add    $0x68,%rsp
+   1800015a1:	pop    %r13
+   1800015a3:	pop    %r12
+   1800015a5:	ret
+   1800015a6:	int3
+   1800015a7:	int3
+   1800015a8:	int3
+   1800015a9:	int3
+   1800015aa:	int3
+   1800015ab:	int3
+   1800015ac:	int3
+   1800015ad:	int3
+   1800015ae:	int3
+   1800015af:	int3
+   1800015b0:	mov    %rsp,%rax
+   1800015b3:	mov    %r9,0x20(%rax)
+   1800015b7:	mov    %r8,0x18(%rax)
+   1800015bb:	mov    %dl,0x10(%rax)
+   1800015be:	mov    %rcx,0x8(%rax)
+   1800015c2:	push   %rbp
+   1800015c3:	push   %rsi
+   1800015c4:	push   %r14
+   1800015c6:	sub    $0x90,%rsp
+   1800015cd:	mov    %rdi,-0x28(%rax)
+   1800015d1:	mov    %r9,%rsi
+   1800015d4:	mov    %r12,-0x30(%rax)
+   1800015d8:	lea    -0x60(%rax),%r9
+   1800015dc:	movsbl %dl,%r12d
+   1800015e0:	mov    %r8,%r14
+   1800015e3:	movzbl %r12b,%edx
+   1800015e7:	mov    %r15,-0x40(%rax)
+   1800015eb:	lea    0x23(%rsp),%r8
+   1800015f0:	mov    %r12b,0x7f729(%rip)        # 0x180080d20
+   1800015f7:	mov    %rcx,%rdi
+   1800015fa:	call   0x180001250
+   1800015ff:	mov    %r12d,%ecx
+   180001602:	mov    %rax,0x50(%rsp)
+   180001607:	mov    $0x1,%r15d
+   18000160d:	xor    %dl,%dl
+   18000160f:	shl    %cl,%r15d
+   180001612:	mov    %rax,%r9
+   180001615:	mov    %r15d,0x44(%rsp)
+   18000161a:	test   %r15d,%r15d
+   18000161d:	jle    0x180001638
+   18000161f:	nop
+   180001620:	movsbq %dl,%rcx
+   180001624:	cmpb   $0x0,(%rcx,%rdi,1)
+   180001628:	sete   %al
+   18000162b:	inc    %dl
+   18000162d:	mov    %al,(%rcx,%rdi,1)
+   180001630:	movsbl %dl,%eax
+   180001633:	cmp    %r15d,%eax
+   180001636:	jl     0x180001620
+   180001638:	mov    $0x1,%eax
+   18000163d:	mov    %r12d,0x2c(%rsp)
+   180001642:	mov    %r12d,%r8d
+   180001645:	cmp    %eax,%r12d
+   180001648:	jbe    0x180001660
+   18000164a:	nopw   0x0(%rax,%rax,1)
+   180001650:	imul   %eax,%r8d
+   180001654:	inc    %eax
+   180001656:	cmp    %r12d,%eax
+   180001659:	jb     0x180001650
+   18000165b:	mov    %r8d,0x2c(%rsp)
+   180001660:	xor    %cl,%cl
+   180001662:	mov    %rbx,0x88(%rsp)
+   18000166a:	test   %r15d,%r15d
+   18000166d:	je     0x180001688
+   18000166f:	nop
+   180001670:	movsbq %cl,%rax
+   180001674:	cmpb   $0x0,(%rax,%rdi,1)
+   180001678:	jne    0x1800016ff
+   18000167e:	inc    %cl
+   180001680:	movsbl %cl,%eax
+   180001683:	cmp    %r15d,%eax
+   180001686:	jb     0x180001670
+   180001688:	mov    0xb8(%rsp),%ebx
+   18000168f:	xor    %ebp,%ebp
+   180001691:	movzbl 0xb8(%rsp),%r11d
+   18000169a:	mov    0x78(%rsp),%r12
+   18000169f:	xor    %dl,%dl
+   1800016a1:	test   %r15d,%r15d
+   1800016a4:	jle    0x1800016c8
+   1800016a6:	data16 nopw 0x0(%rax,%rax,1)
+   1800016b0:	movsbq %dl,%rcx
+   1800016b4:	cmpb   $0x0,(%rcx,%rdi,1)
+   1800016b8:	sete   %al
+   1800016bb:	inc    %dl
+   1800016bd:	mov    %al,(%rcx,%rdi,1)
+   1800016c0:	movsbl %dl,%eax
+   1800016c3:	cmp    %r15d,%eax
+   1800016c6:	jl     0x1800016b0
+   1800016c8:	mov    0x68(%rsp),%r15
+   1800016cd:	mov    0x80(%rsp),%rdi
+   1800016d5:	cmp    %rbp,%r9
+   1800016d8:	jbe    0x180001994
+   1800016de:	movzbl 0x23(%rsp),%eax
+   1800016e3:	mov    %al,(%r14)
+   1800016e6:	mov    0x48(%rsp),%eax
+   1800016ea:	mov    %eax,(%rsi)
+   1800016ec:	mov    0xd0(%rsp),%rax
+   1800016f4:	movb   $0x0,(%rax)
+   1800016f7:	mov    %r9,%rax
+   1800016fa:	jmp    0x1800019a7
+   1800016ff:	xor    %ebp,%ebp
+   180001701:	lea    0xee18(%rip),%r9        # 0x180010520
+   180001708:	lea    0x25611(%rip),%r10        # 0x180026d20
+   18000170f:	mov    %r9,0x38(%rsp)
+   180001714:	mov    %r10,0x30(%rsp)
+   180001719:	lea    0x1a200(%rip),%rsi        # 0x18001b920
+   180001720:	mov    %ebp,%r11d
+   180001723:	lea    0x525f6(%rip),%r14        # 0x180053d20
+   18000172a:	xor    %cl,%cl
+   18000172c:	nopl   0x0(%rax)
+   180001730:	movsbq %cl,%rax
+   180001734:	cmp    %bpl,(%rax,%rdi,1)
+   180001738:	je     0x180001745
+   18000173a:	mov    %cl,(%r11,%r9,1)
+   18000173e:	mov    %ebp,(%r10,%r11,4)
+   180001742:	inc    %r11d
+   180001745:	inc    %cl
+   180001747:	movsbl %cl,%eax
+   18000174a:	cmp    %r15d,%eax
+   18000174d:	jb     0x180001730
+   18000174f:	xor    %al,%al
+   180001751:	lea    0x28e8(%rip),%rcx        # 0x180004040
+   180001758:	mov    %al,0x21(%rsp)
+   18000175c:	mov    $0x1,%ebx
+   180001761:	mov    %ebx,0x28(%rsp)
+   180001765:	test   %r12b,%r12b
+   180001768:	jle    0x180001921
+   18000176e:	mov    %r13,0x70(%rsp)
+   180001773:	movzbl %r12b,%r13d
+   180001777:	mov    %r12b,0x22(%rsp)
+   18000177c:	nopl   0x0(%rax)
+   180001780:	movzbl %al,%ecx
+   180001783:	xor    %edx,%edx
+   180001785:	mov    %r8d,%eax
+   180001788:	mov    $0x1,%edi
+   18000178d:	div    %ebx
+   18000178f:	shl    %cl,%dil
+   180001792:	xor    %edx,%edx
+   180001794:	movsbl %r13b,%ecx
+   180001798:	mov    %ebp,%r8d
+   18000179b:	div    %ecx
+   18000179d:	mov    %edi,0x40(%rsp)
+   1800017a1:	mov    %eax,%ebx
+   1800017a3:	test   %r11d,%r11d
+   1800017a6:	je     0x1800017e8
+   1800017a8:	xor    %dl,%dl
+   1800017aa:	test   %r13b,%r13b
+   1800017ad:	jle    0x1800017d1
+   1800017af:	nop
+   1800017b0:	movzbl (%r9),%eax
+   1800017b4:	mov    %r8d,%ecx
+   1800017b7:	inc    %r8d
+   1800017ba:	mov    %al,(%rcx,%rsi,1)
+   1800017bd:	movzbl %dl,%eax
+   1800017c0:	inc    %dl
+   1800017c2:	imul   %ebx,%eax
+   1800017c5:	add    (%r10),%eax
+   1800017c8:	mov    %eax,(%r14,%rcx,4)
+   1800017cc:	cmp    %r13b,%dl
+   1800017cf:	jl     0x1800017b0
+   1800017d1:	inc    %r9
+   1800017d4:	add    $0x4,%r10
+   1800017d8:	sub    $0x1,%r11
+   1800017dc:	jne    0x1800017a8
+   1800017de:	mov    0x38(%rsp),%r9
+   1800017e3:	mov    0x30(%rsp),%r10
+   1800017e8:	mov    %r10,%rax
+   1800017eb:	mov    %r14,0x30(%rsp)
+   1800017f0:	xor    %r12b,%r12b
+   1800017f3:	mov    %rsi,0x38(%rsp)
+   1800017f8:	mov    %r8d,%r11d
+   1800017fb:	mov    %r14,%r10
+   1800017fe:	mov    %r12b,0x20(%rsp)
+   180001803:	mov    %rax,%r14
+   180001806:	mov    %r9,%rax
+   180001809:	mov    %rsi,%r9
+   18000180c:	mov    %rax,%rsi
+   18000180f:	test   %dil,%dil
+   180001812:	jle    0x1800018d4
+   180001818:	mov    0xb0(%rsp),%r13
+   180001820:	mov    %ebp,%eax
+   180001822:	mov    $0x1,%r8b
+   180001825:	test   %r11d,%r11d
+   180001828:	je     0x18000189e
+   18000182a:	movzbl %r12b,%edx
+   18000182e:	lea    0x280b(%rip),%r12        # 0x180004040
+   180001835:	movsbl %dil,%ecx
+   180001839:	add    %ecx,%edx
+   18000183b:	movslq %edx,%r15
+   18000183e:	xchg   %ax,%ax
+   180001840:	mov    (%r10),%ebx
+   180001843:	movsbq (%r9),%rdi
+   180001847:	mov    %ebx,%ecx
+   180001849:	shl    $0x6,%rcx
+   18000184d:	add    %r15,%rcx
+   180001850:	movsbq (%rcx,%r12,1),%rdx
+   180001855:	xor    %rdi,%rdx
+   180001858:	movzbl (%rdx,%r13,1),%ecx
+   18000185d:	test   %r8b,%r8b
+   180001860:	je     0x18000186d
+   180001862:	test   %cl,%cl
+   180001864:	je     0x180001871
+   180001866:	xor    %r8b,%r8b
+   180001869:	mov    %ebp,%eax
+   18000186b:	jmp    0x180001871
+   18000186d:	test   %cl,%cl
+   18000186f:	je     0x18000187d
+   180001871:	mov    %eax,%ecx
+   180001873:	inc    %eax
+   180001875:	mov    %dil,(%rcx,%rsi,1)
+   180001879:	mov    %ebx,(%r14,%rcx,4)
+   18000187d:	add    $0x4,%r10
+   180001881:	inc    %r9
+   180001884:	sub    $0x1,%r11
+   180001888:	jne    0x180001840
+   18000188a:	movzbl 0x20(%rsp),%r12d
+   180001890:	mov    0x38(%rsp),%r9
+   180001895:	mov    0x30(%rsp),%r10
+   18000189a:	mov    0x40(%rsp),%edi
+   18000189e:	mov    %r10,%rcx
+   1800018a1:	mov    %r14,0x30(%rsp)
+   1800018a6:	inc    %r12b
+   1800018a9:	mov    %rsi,0x38(%rsp)
+   1800018ae:	mov    %eax,%r11d
+   1800018b1:	mov    %r14,%r10
+   1800018b4:	mov    %r12b,0x20(%rsp)
+   1800018b9:	mov    %rcx,%r14
+   1800018bc:	mov    %r9,%rcx
+   1800018bf:	mov    %rsi,%r9
+   1800018c2:	mov    %rcx,%rsi
+   1800018c5:	cmp    %dil,%r12b
+   1800018c8:	jl     0x180001820
+   1800018ce:	movzbl 0x22(%rsp),%r13d
+   1800018d4:	mov    0x28(%rsp),%ebx
+   1800018d8:	mov    0x2c(%rsp),%r8d
+   1800018dd:	movsbl %r13b,%eax
+   1800018e1:	dec    %r13b
+   1800018e4:	imul   %eax,%ebx
+   1800018e7:	movzbl 0x21(%rsp),%eax
+   1800018ec:	inc    %al
+   1800018ee:	mov    %r13b,0x22(%rsp)
+   1800018f3:	mov    %al,0x21(%rsp)
+   1800018f7:	mov    %ebx,0x28(%rsp)
+   1800018fb:	cmp    0xb8(%rsp),%al
+   180001902:	jl     0x180001780
+   180001908:	mov    0xb0(%rsp),%rdi
+   180001910:	lea    0x2729(%rip),%rcx        # 0x180004040
+   180001917:	mov    0x44(%rsp),%r15d
+   18000191c:	mov    0x70(%rsp),%r13
+   180001921:	movsbq (%r9),%r11
+   180001925:	xor    %dl,%dl
+   180001927:	mov    (%r10),%ebx
+   18000192a:	mov    %ebp,%r8d
+   18000192d:	mov    %ebx,%r9d
+   180001930:	shl    $0x6,%r9
+   180001934:	nopl   0x0(%rax)
+   180001938:	nopl   0x0(%rax,%rax,1)
+   180001940:	movsbq %dl,%rax
+   180001944:	add    %r9,%rax
+   180001947:	movsbq (%rax,%rcx,1),%rax
+   18000194c:	xor    %r11,%rax
+   18000194f:	cmpb   $0x0,(%rax,%rdi,1)
+   180001953:	je     0x18000196f
+   180001955:	mov    %r15d,%ecx
+   180001958:	mov    $0x1,%eax
+   18000195d:	sub    %r8d,%ecx
+   180001960:	dec    %ecx
+   180001962:	shl    %cl,%rax
+   180001965:	lea    0x26d4(%rip),%rcx        # 0x180004040
+   18000196c:	add    %rax,%rbp
+   18000196f:	inc    %dl
+   180001971:	movsbl %dl,%r8d
+   180001975:	cmp    %r15d,%r8d
+   180001978:	jb     0x180001940
+   18000197a:	mov    0x50(%rsp),%r9
+   18000197f:	mov    0xc8(%rsp),%rsi
+   180001987:	mov    0xc0(%rsp),%r14
+   18000198f:	jmp    0x18000169a
+   180001994:	mov    0xd0(%rsp),%rcx
+   18000199c:	mov    %rbp,%rax
+   18000199f:	mov    %r11b,(%r14)
+   1800019a2:	mov    %ebx,(%rsi)
+   1800019a4:	movb   $0x1,(%rcx)
+   1800019a7:	mov    0x88(%rsp),%rbx
+   1800019af:	add    $0x90,%rsp
+   1800019b6:	pop    %r14
+   1800019b8:	pop    %rsi
+   1800019b9:	pop    %rbp
+   1800019ba:	ret
+   1800019bb:	int3
+   1800019bc:	sub    $0x28,%rsp
+   1800019c0:	test   %edx,%edx
+   1800019c2:	je     0x1800019fd
+   1800019c4:	sub    $0x1,%edx
+   1800019c7:	je     0x1800019f1
+   1800019c9:	sub    $0x1,%edx
+   1800019cc:	je     0x1800019e4
+   1800019ce:	cmp    $0x1,%edx
+   1800019d1:	je     0x1800019dd
+   1800019d3:	mov    $0x1,%eax
+   1800019d8:	add    $0x28,%rsp
+   1800019dc:	ret
+   1800019dd:	call   0x180001ee4
+   1800019e2:	jmp    0x1800019e9
+   1800019e4:	call   0x180001ebc
+   1800019e9:	movzbl %al,%eax
+   1800019ec:	add    $0x28,%rsp
+   1800019f0:	ret
+   1800019f1:	mov    %r8,%rdx
+   1800019f4:	add    $0x28,%rsp
+   1800019f8:	jmp    0x180001a0c
+   1800019fd:	test   %r8,%r8
+   180001a00:	setne  %cl
+   180001a03:	add    $0x28,%rsp
+   180001a07:	jmp    0x180001b24
+   180001a0c:	mov    %rbx,0x8(%rsp)
+   180001a11:	mov    %rsi,0x10(%rsp)
+   180001a16:	mov    %rdi,0x20(%rsp)
+   180001a1b:	push   %r14
+   180001a1d:	sub    $0x20,%rsp
+   180001a21:	mov    %rdx,%rsi
+   180001a24:	mov    %rcx,%r14
+   180001a27:	xor    %ecx,%ecx
+   180001a29:	call   0x180001fa0
+   180001a2e:	test   %al,%al
+   180001a30:	je     0x180001afe
+   180001a36:	call   0x180001e34
+   180001a3b:	mov    %al,%bl
+   180001a3d:	mov    %al,0x40(%rsp)
+   180001a41:	mov    $0x1,%dil
+   180001a44:	cmpl   $0x0,0x7f305(%rip)        # 0x180080d50
+   180001a4b:	jne    0x180001b16
+   180001a51:	movl   $0x1,0x7f2f5(%rip)        # 0x180080d50
+   180001a5b:	call   0x180001ea4
+   180001a60:	test   %al,%al
+   180001a62:	je     0x180001ab3
+   180001a64:	call   0x1800022bc
+   180001a69:	call   0x180001dec
+   180001a6e:	call   0x180001e18
+   180001a73:	lea    0x16b6(%rip),%rdx        # 0x180003130
+   180001a7a:	lea    0x16a7(%rip),%rcx        # 0x180003128
+   180001a81:	call   0x180002518
+   180001a86:	test   %eax,%eax
+   180001a88:	jne    0x180001ab3
+   180001a8a:	call   0x180001e70
+   180001a8f:	test   %al,%al
+   180001a91:	je     0x180001ab3
+   180001a93:	lea    0x1686(%rip),%rdx        # 0x180003120
+   180001a9a:	lea    0x1677(%rip),%rcx        # 0x180003118
+   180001aa1:	call   0x180002512
+   180001aa6:	movl   $0x2,0x7f2a0(%rip)        # 0x180080d50
+   180001ab0:	xor    %dil,%dil
+   180001ab3:	mov    %bl,%cl
+   180001ab5:	call   0x180002110
+   180001aba:	test   %dil,%dil
+   180001abd:	jne    0x180001afe
+   180001abf:	call   0x180002160
+   180001ac4:	mov    %rax,%rbx
+   180001ac7:	cmpq   $0x0,(%rax)
+   180001acb:	je     0x180001af1
+   180001acd:	mov    %rax,%rcx
+   180001ad0:	call   0x180002078
+   180001ad5:	test   %al,%al
+   180001ad7:	je     0x180001af1
+   180001ad9:	mov    %rsi,%r8
+   180001adc:	mov    $0x2,%edx
+   180001ae1:	mov    %r14,%rcx
+   180001ae4:	mov    (%rbx),%rax
+   180001ae7:	mov    0x1602(%rip),%r9        # 0x1800030f0
+   180001aee:	call   *%r9
+   180001af1:	incl   0x7f22d(%rip)        # 0x180080d24
+   180001af7:	mov    $0x1,%eax
+   180001afc:	jmp    0x180001b00
+   180001afe:	xor    %eax,%eax
+   180001b00:	mov    0x30(%rsp),%rbx
+   180001b05:	mov    0x38(%rsp),%rsi
+   180001b0a:	mov    0x48(%rsp),%rdi
+   180001b0f:	add    $0x20,%rsp
+   180001b13:	pop    %r14
+   180001b15:	ret
+   180001b16:	mov    $0x7,%ecx
+   180001b1b:	call   0x180002170
+   180001b20:	nop
+   180001b21:	int3
+   180001b22:	int3
+   180001b23:	int3
+   180001b24:	mov    %rbx,0x8(%rsp)
+   180001b29:	push   %rdi
+   180001b2a:	sub    $0x30,%rsp
+   180001b2e:	mov    %cl,%dil
+   180001b31:	mov    0x7f1ed(%rip),%eax        # 0x180080d24
+   180001b37:	test   %eax,%eax
+   180001b39:	jg     0x180001b48
+   180001b3b:	xor    %eax,%eax
+   180001b3d:	mov    0x40(%rsp),%rbx
+   180001b42:	add    $0x30,%rsp
+   180001b46:	pop    %rdi
+   180001b47:	ret
+   180001b48:	dec    %eax
+   180001b4a:	mov    %eax,0x7f1d4(%rip)        # 0x180080d24
+   180001b50:	call   0x180001e34
+   180001b55:	mov    %al,%bl
+   180001b57:	mov    %al,0x20(%rsp)
+   180001b5b:	cmpl   $0x2,0x7f1ee(%rip)        # 0x180080d50
+   180001b62:	jne    0x180001b9b
+   180001b64:	call   0x180001f5c
+   180001b69:	call   0x180001dfc
+   180001b6e:	call   0x1800022f8
+   180001b73:	andl   $0x0,0x7f1d6(%rip)        # 0x180080d50
+   180001b7a:	mov    %bl,%cl
+   180001b7c:	call   0x180002110
+   180001b81:	xor    %edx,%edx
+   180001b83:	mov    %dil,%cl
+   180001b86:	call   0x180002134
+   180001b8b:	neg    %al
+   180001b8d:	sbb    %ebx,%ebx
+   180001b8f:	and    $0x1,%ebx
+   180001b92:	call   0x180001f8c
+   180001b97:	mov    %ebx,%eax
+   180001b99:	jmp    0x180001b3d
+   180001b9b:	mov    $0x7,%ecx
+   180001ba0:	call   0x180002170
+   180001ba5:	nop
+   180001ba6:	nop
+   180001ba7:	int3
+   180001ba8:	mov    %rsp,%rax
+   180001bab:	mov    %rbx,0x20(%rax)
+   180001baf:	mov    %r8,0x18(%rax)
+   180001bb3:	mov    %edx,0x10(%rax)
+   180001bb6:	mov    %rcx,0x8(%rax)
+   180001bba:	push   %rsi
+   180001bbb:	push   %rdi
+   180001bbc:	push   %r14
+   180001bbe:	sub    $0x40,%rsp
+   180001bc2:	mov    %r8,%rsi
+   180001bc5:	mov    %edx,%edi
+   180001bc7:	mov    %rcx,%r14
+   180001bca:	test   %edx,%edx
+   180001bcc:	jne    0x180001bdd
+   180001bce:	cmp    %edx,0x7f150(%rip)        # 0x180080d24
+   180001bd4:	jg     0x180001bdd
+   180001bd6:	xor    %eax,%eax
+   180001bd8:	jmp    0x180001ccb
+   180001bdd:	lea    -0x1(%rdx),%eax
+   180001be0:	cmp    $0x1,%eax
+   180001be3:	ja     0x180001c2a
+   180001be5:	mov    0x157c(%rip),%rax        # 0x180003168
+   180001bec:	test   %rax,%rax
+   180001bef:	jne    0x180001bfb
+   180001bf1:	movl   $0x1,0x30(%rsp)
+   180001bf9:	jmp    0x180001c0f
+   180001bfb:	call   *0x14ef(%rip)        # 0x1800030f0
+   180001c01:	mov    %eax,%ebx
+   180001c03:	mov    %eax,0x30(%rsp)
+   180001c07:	test   %eax,%eax
+   180001c09:	je     0x180001cc1
+   180001c0f:	mov    %rsi,%r8
+   180001c12:	mov    %edi,%edx
+   180001c14:	mov    %r14,%rcx
+   180001c17:	call   0x1800019bc
+   180001c1c:	mov    %eax,%ebx
+   180001c1e:	mov    %eax,0x30(%rsp)
+   180001c22:	test   %eax,%eax
+   180001c24:	je     0x180001cc1
+   180001c2a:	mov    %rsi,%r8
+   180001c2d:	mov    %edi,%edx
+   180001c2f:	mov    %r14,%rcx
+   180001c32:	call   0x180001dc8
+   180001c37:	mov    %eax,%ebx
+   180001c39:	mov    %eax,0x30(%rsp)
+   180001c3d:	cmp    $0x1,%edi
+   180001c40:	jne    0x180001c78
+   180001c42:	test   %eax,%eax
+   180001c44:	jne    0x180001c78
+   180001c46:	mov    %rsi,%r8
+   180001c49:	xor    %edx,%edx
+   180001c4b:	mov    %r14,%rcx
+   180001c4e:	call   0x180001dc8
+   180001c53:	test   %rsi,%rsi
+   180001c56:	setne  %cl
+   180001c59:	call   0x180001b24
+   180001c5e:	mov    0x1503(%rip),%rax        # 0x180003168
+   180001c65:	test   %rax,%rax
+   180001c68:	je     0x180001c78
+   180001c6a:	mov    %rsi,%r8
+   180001c6d:	xor    %edx,%edx
+   180001c6f:	mov    %r14,%rcx
+   180001c72:	call   *0x1478(%rip)        # 0x1800030f0
+   180001c78:	test   %edi,%edi
+   180001c7a:	je     0x180001c81
+   180001c7c:	cmp    $0x3,%edi
+   180001c7f:	jne    0x180001cc1
+   180001c81:	mov    %rsi,%r8
+   180001c84:	mov    %edi,%edx
+   180001c86:	mov    %r14,%rcx
+   180001c89:	call   0x1800019bc
+   180001c8e:	mov    %eax,%ebx
+   180001c90:	mov    %eax,0x30(%rsp)
+   180001c94:	test   %eax,%eax
+   180001c96:	je     0x180001cc1
+   180001c98:	mov    0x14c9(%rip),%rax        # 0x180003168
+   180001c9f:	test   %rax,%rax
+   180001ca2:	jne    0x180001cad
+   180001ca4:	lea    0x1(%rax),%ebx
+   180001ca7:	mov    %ebx,0x30(%rsp)
+   180001cab:	jmp    0x180001cc1
+   180001cad:	mov    %rsi,%r8
+   180001cb0:	mov    %edi,%edx
+   180001cb2:	mov    %r14,%rcx
+   180001cb5:	call   *0x1435(%rip)        # 0x1800030f0
+   180001cbb:	mov    %eax,%ebx
+   180001cbd:	mov    %eax,0x30(%rsp)
+   180001cc1:	jmp    0x180001cc9
+   180001cc3:	xor    %ebx,%ebx
+   180001cc5:	mov    %ebx,0x30(%rsp)
+   180001cc9:	mov    %ebx,%eax
+   180001ccb:	mov    0x78(%rsp),%rbx
+   180001cd0:	add    $0x40,%rsp
+   180001cd4:	pop    %r14
+   180001cd6:	pop    %rdi
+   180001cd7:	pop    %rsi
+   180001cd8:	ret
+   180001cd9:	int3
+   180001cda:	int3
+   180001cdb:	int3
+   180001cdc:	mov    %rbx,0x8(%rsp)
+   180001ce1:	mov    %rsi,0x10(%rsp)
+   180001ce6:	push   %rdi
+   180001ce7:	sub    $0x20,%rsp
+   180001ceb:	mov    %r8,%rdi
+   180001cee:	mov    %edx,%ebx
+   180001cf0:	mov    %rcx,%rsi
+   180001cf3:	cmp    $0x1,%edx
+   180001cf6:	jne    0x180001cfd
+   180001cf8:	call   0x180001d1c
+   180001cfd:	mov    %rdi,%r8
+   180001d00:	mov    %ebx,%edx
+   180001d02:	mov    %rsi,%rcx
+   180001d05:	mov    0x30(%rsp),%rbx
+   180001d0a:	mov    0x38(%rsp),%rsi
+   180001d0f:	add    $0x20,%rsp
+   180001d13:	pop    %rdi
+   180001d14:	jmp    0x180001ba8
+   180001d19:	int3
+   180001d1a:	int3
+   180001d1b:	int3
+   180001d1c:	mov    %rbx,0x20(%rsp)
+   180001d21:	push   %rbp
+   180001d22:	mov    %rsp,%rbp
+   180001d25:	sub    $0x20,%rsp
+   180001d29:	mov    0x22e0(%rip),%rax        # 0x180004010
+   180001d30:	movabs $0x2b992ddfa232,%rbx
+   180001d3a:	cmp    %rbx,%rax
+   180001d3d:	jne    0x180001db3
+   180001d3f:	andq   $0x0,0x18(%rbp)
+   180001d44:	lea    0x18(%rbp),%rcx
+   180001d48:	call   *0x12ca(%rip)        # 0x180003018
+   180001d4e:	mov    0x18(%rbp),%rax
+   180001d52:	mov    %rax,0x10(%rbp)
+   180001d56:	call   *0x12ec(%rip)        # 0x180003048
+   180001d5c:	mov    %eax,%eax
+   180001d5e:	xor    %rax,0x10(%rbp)
+   180001d62:	call   *0x12a0(%rip)        # 0x180003008
+   180001d68:	mov    %eax,%eax
+   180001d6a:	lea    0x20(%rbp),%rcx
+   180001d6e:	xor    %rax,0x10(%rbp)
+   180001d72:	call   *0x1298(%rip)        # 0x180003010
+   180001d78:	mov    0x20(%rbp),%eax
+   180001d7b:	lea    0x10(%rbp),%rcx
+   180001d7f:	shl    $0x20,%rax
+   180001d83:	xor    0x20(%rbp),%rax
+   180001d87:	xor    0x10(%rbp),%rax
+   180001d8b:	xor    %rcx,%rax
+   180001d8e:	movabs $0xffffffffffff,%rcx
+   180001d98:	and    %rcx,%rax
+   180001d9b:	movabs $0x2b992ddfa233,%rcx
+   180001da5:	cmp    %rbx,%rax
+   180001da8:	cmove  %rcx,%rax
+   180001dac:	mov    %rax,0x225d(%rip)        # 0x180004010
+   180001db3:	mov    0x48(%rsp),%rbx
+   180001db8:	not    %rax
+   180001dbb:	mov    %rax,0x2246(%rip)        # 0x180004008
+   180001dc2:	add    $0x20,%rsp
+   180001dc6:	pop    %rbp
+   180001dc7:	ret
+   180001dc8:	sub    $0x28,%rsp
+   180001dcc:	cmp    $0x1,%edx
+   180001dcf:	jne    0x180001de1
+   180001dd1:	cmpq   $0x0,0x138f(%rip)        # 0x180003168
+   180001dd9:	jne    0x180001de1
+   180001ddb:	call   *0x123f(%rip)        # 0x180003020
+   180001de1:	mov    $0x1,%eax
+   180001de6:	add    $0x28,%rsp
+   180001dea:	ret
+   180001deb:	int3
+   180001dec:	lea    0x7ef3d(%rip),%rcx        # 0x180080d30
+   180001df3:	rex.W jmp *0x122e(%rip)        # 0x180003028
+   180001dfa:	int3
+   180001dfb:	int3
+   180001dfc:	lea    0x7ef2d(%rip),%rcx        # 0x180080d30
+   180001e03:	jmp    0x18000250c
+   180001e08:	lea    0x7ef31(%rip),%rax        # 0x180080d40
+   180001e0f:	ret
+   180001e10:	lea    0x7ef31(%rip),%rax        # 0x180080d48
+   180001e17:	ret
    180001e18:	sub    $0x28,%rsp
-   180001e1c:	call   0x180002494
-   180001e21:	test   %eax,%eax
-   180001e23:	je     0x180001e2c
-   180001e25:	call   0x1800022e0
-   180001e2a:	jmp    0x180001e45
-   180001e2c:	call   0x18000248c
-   180001e31:	mov    %eax,%ecx
-   180001e33:	call   0x1800024c4
-   180001e38:	test   %eax,%eax
-   180001e3a:	je     0x180001e40
-   180001e3c:	xor    %al,%al
-   180001e3e:	jmp    0x180001e47
-   180001e40:	call   0x1800024ca
-   180001e45:	mov    $0x1,%al
-   180001e47:	add    $0x28,%rsp
-   180001e4b:	ret
-   180001e4c:	sub    $0x28,%rsp
-   180001e50:	xor    %ecx,%ecx
-   180001e52:	call   0x180001f94
-   180001e57:	test   %al,%al
-   180001e59:	setne  %al
-   180001e5c:	add    $0x28,%rsp
-   180001e60:	ret
-   180001e61:	int3
-   180001e62:	int3
-   180001e63:	int3
-   180001e64:	sub    $0x28,%rsp
-   180001e68:	call   0x1800024e4
-   180001e6d:	test   %al,%al
-   180001e6f:	jne    0x180001e75
-   180001e71:	xor    %al,%al
-   180001e73:	jmp    0x180001e87
-   180001e75:	call   0x1800024e4
-   180001e7a:	test   %al,%al
-   180001e7c:	jne    0x180001e85
-   180001e7e:	call   0x1800024e4
-   180001e83:	jmp    0x180001e71
-   180001e85:	mov    $0x1,%al
-   180001e87:	add    $0x28,%rsp
-   180001e8b:	ret
-   180001e8c:	sub    $0x28,%rsp
-   180001e90:	call   0x1800024e4
-   180001e95:	call   0x1800024e4
-   180001e9a:	mov    $0x1,%al
-   180001e9c:	add    $0x28,%rsp
-   180001ea0:	ret
-   180001ea1:	int3
-   180001ea2:	int3
-   180001ea3:	int3
-   180001ea4:	mov    %rbx,0x8(%rsp)
-   180001ea9:	mov    %rbp,0x10(%rsp)
-   180001eae:	mov    %rsi,0x18(%rsp)
-   180001eb3:	push   %rdi
-   180001eb4:	sub    $0x20,%rsp
-   180001eb8:	mov    %r9,%rdi
-   180001ebb:	mov    %r8,%rsi
-   180001ebe:	mov    %edx,%ebx
-   180001ec0:	mov    %rcx,%rbp
-   180001ec3:	call   0x180002494
-   180001ec8:	test   %eax,%eax
-   180001eca:	jne    0x180001ee2
-   180001ecc:	cmp    $0x1,%ebx
-   180001ecf:	jne    0x180001ee2
-   180001ed1:	mov    %rsi,%r8
-   180001ed4:	xor    %edx,%edx
-   180001ed6:	mov    %rbp,%rcx
-   180001ed9:	mov    %rdi,%rax
-   180001edc:	call   *0x120e(%rip)        # 0x1800030f0
-   180001ee2:	mov    0x58(%rsp),%rdx
-   180001ee7:	mov    0x50(%rsp),%ecx
-   180001eeb:	mov    0x30(%rsp),%rbx
-   180001ef0:	mov    0x38(%rsp),%rbp
-   180001ef5:	mov    0x40(%rsp),%rsi
-   180001efa:	add    $0x20,%rsp
-   180001efe:	pop    %rdi
-   180001eff:	jmp    0x1800024be
-   180001f04:	sub    $0x28,%rsp
-   180001f08:	call   0x180002494
-   180001f0d:	test   %eax,%eax
-   180001f0f:	je     0x180001f21
-   180001f11:	lea    0x7ee50(%rip),%rcx        # 0x180080d68
-   180001f18:	add    $0x28,%rsp
-   180001f1c:	jmp    0x1800024d6
-   180001f21:	call   0x1800024e8
-   180001f26:	test   %eax,%eax
-   180001f28:	jne    0x180001f2f
-   180001f2a:	call   0x1800024dc
-   180001f2f:	add    $0x28,%rsp
-   180001f33:	ret
-   180001f34:	sub    $0x28,%rsp
-   180001f38:	xor    %ecx,%ecx
-   180001f3a:	call   0x1800024e4
-   180001f3f:	add    $0x28,%rsp
-   180001f43:	jmp    0x1800024e4
-   180001f48:	rex push %rbx
-   180001f4a:	sub    $0x20,%rsp
-   180001f4e:	movzbl 0x7ee0b(%rip),%eax        # 0x180080d60
-   180001f55:	test   %ecx,%ecx
-   180001f57:	mov    $0x1,%ebx
-   180001f5c:	cmove  %ebx,%eax
-   180001f5f:	mov    %al,0x7edfb(%rip)        # 0x180080d60
-   180001f65:	call   0x1800022e0
-   180001f6a:	call   0x1800024e4
-   180001f6f:	test   %al,%al
-   180001f71:	jne    0x180001f77
-   180001f73:	xor    %al,%al
-   180001f75:	jmp    0x180001f8b
-   180001f77:	call   0x1800024e4
-   180001f7c:	test   %al,%al
-   180001f7e:	jne    0x180001f89
-   180001f80:	xor    %ecx,%ecx
-   180001f82:	call   0x1800024e4
-   180001f87:	jmp    0x180001f73
-   180001f89:	mov    %bl,%al
-   180001f8b:	add    $0x20,%rsp
-   180001f8f:	pop    %rbx
-   180001f90:	ret
-   180001f91:	int3
-   180001f92:	int3
-   180001f93:	int3
-   180001f94:	rex push %rbx
-   180001f96:	sub    $0x20,%rsp
-   180001f9a:	cmpb   $0x0,0x7edc0(%rip)        # 0x180080d61
-   180001fa1:	mov    %ecx,%ebx
-   180001fa3:	jne    0x18000200c
-   180001fa5:	cmp    $0x1,%ecx
-   180001fa8:	ja     0x180002014
-   180001faa:	call   0x180002494
-   180001faf:	test   %eax,%eax
-   180001fb1:	je     0x180001fdb
-   180001fb3:	test   %ebx,%ebx
-   180001fb5:	jne    0x180001fdb
-   180001fb7:	lea    0x7edaa(%rip),%rcx        # 0x180080d68
-   180001fbe:	call   0x1800024d0
-   180001fc3:	test   %eax,%eax
-   180001fc5:	jne    0x180001fd7
-   180001fc7:	lea    0x7edb2(%rip),%rcx        # 0x180080d80
-   180001fce:	call   0x1800024d0
-   180001fd3:	test   %eax,%eax
-   180001fd5:	je     0x180002005
-   180001fd7:	xor    %al,%al
-   180001fd9:	jmp    0x18000200e
-   180001fdb:	movdqa 0x118d(%rip),%xmm0        # 0x180003170
-   180001fe3:	or     $0xffffffffffffffff,%rax
-   180001fe7:	movdqu %xmm0,0x7ed79(%rip)        # 0x180080d68
-   180001fef:	mov    %rax,0x7ed82(%rip)        # 0x180080d78
-   180001ff6:	movdqu %xmm0,0x7ed82(%rip)        # 0x180080d80
-   180001ffe:	mov    %rax,0x7ed8b(%rip)        # 0x180080d90
-   180002005:	movb   $0x1,0x7ed55(%rip)        # 0x180080d61
-   18000200c:	mov    $0x1,%al
-   18000200e:	add    $0x20,%rsp
-   180002012:	pop    %rbx
-   180002013:	ret
-   180002014:	mov    $0x5,%ecx
-   180002019:	call   0x180002118
-   18000201e:	int3
-   18000201f:	int3
-   180002020:	sub    $0x18,%rsp
-   180002024:	mov    %rcx,%r8
-   180002027:	mov    $0x5a4d,%eax
-   18000202c:	cmp    %ax,-0x2033(%rip)        # 0x180000000
-   180002033:	jne    0x1800020ad
-   180002035:	movslq -0x2000(%rip),%rcx        # 0x18000003c
-   18000203c:	lea    -0x2043(%rip),%rdx        # 0x180000000
-   180002043:	add    %rdx,%rcx
-   180002046:	cmpl   $0x4550,(%rcx)
-   18000204c:	jne    0x1800020ad
-   18000204e:	mov    $0x20b,%eax
-   180002053:	cmp    %ax,0x18(%rcx)
-   180002057:	jne    0x1800020ad
-   180002059:	sub    %rdx,%r8
-   18000205c:	movzwl 0x14(%rcx),%edx
-   180002060:	add    $0x18,%rdx
-   180002064:	add    %rcx,%rdx
-   180002067:	movzwl 0x6(%rcx),%eax
-   18000206b:	lea    (%rax,%rax,4),%rcx
-   18000206f:	lea    (%rdx,%rcx,8),%r9
-   180002073:	mov    %rdx,(%rsp)
-   180002077:	cmp    %r9,%rdx
-   18000207a:	je     0x180002094
-   18000207c:	mov    0xc(%rdx),%ecx
-   18000207f:	cmp    %rcx,%r8
-   180002082:	jb     0x18000208e
-   180002084:	mov    0x8(%rdx),%eax
-   180002087:	add    %ecx,%eax
-   180002089:	cmp    %rax,%r8
-   18000208c:	jb     0x180002096
-   18000208e:	add    $0x28,%rdx
-   180002092:	jmp    0x180002073
-   180002094:	xor    %edx,%edx
-   180002096:	test   %rdx,%rdx
-   180002099:	jne    0x18000209f
-   18000209b:	xor    %al,%al
-   18000209d:	jmp    0x1800020b3
-   18000209f:	cmpl   $0x0,0x24(%rdx)
-   1800020a3:	jge    0x1800020a9
-   1800020a5:	xor    %al,%al
-   1800020a7:	jmp    0x1800020b3
-   1800020a9:	mov    $0x1,%al
-   1800020ab:	jmp    0x1800020b3
-   1800020ad:	xor    %al,%al
-   1800020af:	jmp    0x1800020b3
-   1800020b1:	xor    %al,%al
-   1800020b3:	add    $0x18,%rsp
-   1800020b7:	ret
-   1800020b8:	rex push %rbx
-   1800020ba:	sub    $0x20,%rsp
-   1800020be:	mov    %cl,%bl
-   1800020c0:	call   0x180002494
-   1800020c5:	xor    %edx,%edx
-   1800020c7:	test   %eax,%eax
-   1800020c9:	je     0x1800020d6
-   1800020cb:	test   %bl,%bl
-   1800020cd:	jne    0x1800020d6
-   1800020cf:	xchg   %rdx,0x7ec82(%rip)        # 0x180080d58
-   1800020d6:	add    $0x20,%rsp
-   1800020da:	pop    %rbx
-   1800020db:	ret
-   1800020dc:	rex push %rbx
-   1800020de:	sub    $0x20,%rsp
-   1800020e2:	cmpb   $0x0,0x7ec77(%rip)        # 0x180080d60
-   1800020e9:	mov    %cl,%bl
-   1800020eb:	je     0x1800020f1
-   1800020ed:	test   %dl,%dl
-   1800020ef:	jne    0x1800020fd
-   1800020f1:	call   0x1800024e4
-   1800020f6:	mov    %bl,%cl
-   1800020f8:	call   0x1800024e4
-   1800020fd:	mov    $0x1,%al
-   1800020ff:	add    $0x20,%rsp
-   180002103:	pop    %rbx
-   180002104:	ret
-   180002105:	int3
-   180002106:	int3
-   180002107:	int3
-   180002108:	lea    0x7ec91(%rip),%rax        # 0x180080da0
+   180001e1c:	call   0x180001e08
+   180001e21:	orq    $0x24,(%rax)
+   180001e25:	call   0x180001e10
+   180001e2a:	orq    $0x2,(%rax)
+   180001e2e:	add    $0x28,%rsp
+   180001e32:	ret
+   180001e33:	int3
+   180001e34:	sub    $0x28,%rsp
+   180001e38:	call   0x1800024ec
+   180001e3d:	test   %eax,%eax
+   180001e3f:	je     0x180001e62
+   180001e41:	mov    %gs:0x30,%rax
+   180001e4a:	mov    0x8(%rax),%rcx
+   180001e4e:	jmp    0x180001e55
+   180001e50:	cmp    %rax,%rcx
+   180001e53:	je     0x180001e69
+   180001e55:	xor    %eax,%eax
+   180001e57:	lock cmpxchg %rcx,0x7eef8(%rip)        # 0x180080d58
+   180001e60:	jne    0x180001e50
+   180001e62:	xor    %al,%al
+   180001e64:	add    $0x28,%rsp
+   180001e68:	ret
+   180001e69:	mov    $0x1,%al
+   180001e6b:	jmp    0x180001e64
+   180001e6d:	int3
+   180001e6e:	int3
+   180001e6f:	int3
+   180001e70:	sub    $0x28,%rsp
+   180001e74:	call   0x1800024ec
+   180001e79:	test   %eax,%eax
+   180001e7b:	je     0x180001e84
+   180001e7d:	call   0x180002338
+   180001e82:	jmp    0x180001e9d
+   180001e84:	call   0x1800024e4
+   180001e89:	mov    %eax,%ecx
+   180001e8b:	call   0x180002524
+   180001e90:	test   %eax,%eax
+   180001e92:	je     0x180001e98
+   180001e94:	xor    %al,%al
+   180001e96:	jmp    0x180001e9f
+   180001e98:	call   0x18000252a
+   180001e9d:	mov    $0x1,%al
+   180001e9f:	add    $0x28,%rsp
+   180001ea3:	ret
+   180001ea4:	sub    $0x28,%rsp
+   180001ea8:	xor    %ecx,%ecx
+   180001eaa:	call   0x180001fec
+   180001eaf:	test   %al,%al
+   180001eb1:	setne  %al
+   180001eb4:	add    $0x28,%rsp
+   180001eb8:	ret
+   180001eb9:	int3
+   180001eba:	int3
+   180001ebb:	int3
+   180001ebc:	sub    $0x28,%rsp
+   180001ec0:	call   0x180002544
+   180001ec5:	test   %al,%al
+   180001ec7:	jne    0x180001ecd
+   180001ec9:	xor    %al,%al
+   180001ecb:	jmp    0x180001edf
+   180001ecd:	call   0x180002544
+   180001ed2:	test   %al,%al
+   180001ed4:	jne    0x180001edd
+   180001ed6:	call   0x180002544
+   180001edb:	jmp    0x180001ec9
+   180001edd:	mov    $0x1,%al
+   180001edf:	add    $0x28,%rsp
+   180001ee3:	ret
+   180001ee4:	sub    $0x28,%rsp
+   180001ee8:	call   0x180002544
+   180001eed:	call   0x180002544
+   180001ef2:	mov    $0x1,%al
+   180001ef4:	add    $0x28,%rsp
+   180001ef8:	ret
+   180001ef9:	int3
+   180001efa:	int3
+   180001efb:	int3
+   180001efc:	mov    %rbx,0x8(%rsp)
+   180001f01:	mov    %rbp,0x10(%rsp)
+   180001f06:	mov    %rsi,0x18(%rsp)
+   180001f0b:	push   %rdi
+   180001f0c:	sub    $0x20,%rsp
+   180001f10:	mov    %r9,%rdi
+   180001f13:	mov    %r8,%rsi
+   180001f16:	mov    %edx,%ebx
+   180001f18:	mov    %rcx,%rbp
+   180001f1b:	call   0x1800024ec
+   180001f20:	test   %eax,%eax
+   180001f22:	jne    0x180001f3a
+   180001f24:	cmp    $0x1,%ebx
+   180001f27:	jne    0x180001f3a
+   180001f29:	mov    %rsi,%r8
+   180001f2c:	xor    %edx,%edx
+   180001f2e:	mov    %rbp,%rcx
+   180001f31:	mov    %rdi,%rax
+   180001f34:	call   *0x11b6(%rip)        # 0x1800030f0
+   180001f3a:	mov    0x58(%rsp),%rdx
+   180001f3f:	mov    0x50(%rsp),%ecx
+   180001f43:	mov    0x30(%rsp),%rbx
+   180001f48:	mov    0x38(%rsp),%rbp
+   180001f4d:	mov    0x40(%rsp),%rsi
+   180001f52:	add    $0x20,%rsp
+   180001f56:	pop    %rdi
+   180001f57:	jmp    0x18000251e
+   180001f5c:	sub    $0x28,%rsp
+   180001f60:	call   0x1800024ec
+   180001f65:	test   %eax,%eax
+   180001f67:	je     0x180001f79
+   180001f69:	lea    0x7edf8(%rip),%rcx        # 0x180080d68
+   180001f70:	add    $0x28,%rsp
+   180001f74:	jmp    0x180002536
+   180001f79:	call   0x180002548
+   180001f7e:	test   %eax,%eax
+   180001f80:	jne    0x180001f87
+   180001f82:	call   0x18000253c
+   180001f87:	add    $0x28,%rsp
+   180001f8b:	ret
+   180001f8c:	sub    $0x28,%rsp
+   180001f90:	xor    %ecx,%ecx
+   180001f92:	call   0x180002544
+   180001f97:	add    $0x28,%rsp
+   180001f9b:	jmp    0x180002544
+   180001fa0:	rex push %rbx
+   180001fa2:	sub    $0x20,%rsp
+   180001fa6:	movzbl 0x7edb3(%rip),%eax        # 0x180080d60
+   180001fad:	test   %ecx,%ecx
+   180001faf:	mov    $0x1,%ebx
+   180001fb4:	cmove  %ebx,%eax
+   180001fb7:	mov    %al,0x7eda3(%rip)        # 0x180080d60
+   180001fbd:	call   0x180002338
+   180001fc2:	call   0x180002544
+   180001fc7:	test   %al,%al
+   180001fc9:	jne    0x180001fcf
+   180001fcb:	xor    %al,%al
+   180001fcd:	jmp    0x180001fe3
+   180001fcf:	call   0x180002544
+   180001fd4:	test   %al,%al
+   180001fd6:	jne    0x180001fe1
+   180001fd8:	xor    %ecx,%ecx
+   180001fda:	call   0x180002544
+   180001fdf:	jmp    0x180001fcb
+   180001fe1:	mov    %bl,%al
+   180001fe3:	add    $0x20,%rsp
+   180001fe7:	pop    %rbx
+   180001fe8:	ret
+   180001fe9:	int3
+   180001fea:	int3
+   180001feb:	int3
+   180001fec:	rex push %rbx
+   180001fee:	sub    $0x20,%rsp
+   180001ff2:	cmpb   $0x0,0x7ed68(%rip)        # 0x180080d61
+   180001ff9:	mov    %ecx,%ebx
+   180001ffb:	jne    0x180002064
+   180001ffd:	cmp    $0x1,%ecx
+   180002000:	ja     0x18000206c
+   180002002:	call   0x1800024ec
+   180002007:	test   %eax,%eax
+   180002009:	je     0x180002033
+   18000200b:	test   %ebx,%ebx
+   18000200d:	jne    0x180002033
+   18000200f:	lea    0x7ed52(%rip),%rcx        # 0x180080d68
+   180002016:	call   0x180002530
+   18000201b:	test   %eax,%eax
+   18000201d:	jne    0x18000202f
+   18000201f:	lea    0x7ed5a(%rip),%rcx        # 0x180080d80
+   180002026:	call   0x180002530
+   18000202b:	test   %eax,%eax
+   18000202d:	je     0x18000205d
+   18000202f:	xor    %al,%al
+   180002031:	jmp    0x180002066
+   180002033:	movdqa 0x1135(%rip),%xmm0        # 0x180003170
+   18000203b:	or     $0xffffffffffffffff,%rax
+   18000203f:	movdqu %xmm0,0x7ed21(%rip)        # 0x180080d68
+   180002047:	mov    %rax,0x7ed2a(%rip)        # 0x180080d78
+   18000204e:	movdqu %xmm0,0x7ed2a(%rip)        # 0x180080d80
+   180002056:	mov    %rax,0x7ed33(%rip)        # 0x180080d90
+   18000205d:	movb   $0x1,0x7ecfd(%rip)        # 0x180080d61
+   180002064:	mov    $0x1,%al
+   180002066:	add    $0x20,%rsp
+   18000206a:	pop    %rbx
+   18000206b:	ret
+   18000206c:	mov    $0x5,%ecx
+   180002071:	call   0x180002170
+   180002076:	int3
+   180002077:	int3
+   180002078:	sub    $0x18,%rsp
+   18000207c:	mov    %rcx,%r8
+   18000207f:	mov    $0x5a4d,%eax
+   180002084:	cmp    %ax,-0x208b(%rip)        # 0x180000000
+   18000208b:	jne    0x180002105
+   18000208d:	movslq -0x2058(%rip),%rcx        # 0x18000003c
+   180002094:	lea    -0x209b(%rip),%rdx        # 0x180000000
+   18000209b:	add    %rdx,%rcx
+   18000209e:	cmpl   $0x4550,(%rcx)
+   1800020a4:	jne    0x180002105
+   1800020a6:	mov    $0x20b,%eax
+   1800020ab:	cmp    %ax,0x18(%rcx)
+   1800020af:	jne    0x180002105
+   1800020b1:	sub    %rdx,%r8
+   1800020b4:	movzwl 0x14(%rcx),%edx
+   1800020b8:	add    $0x18,%rdx
+   1800020bc:	add    %rcx,%rdx
+   1800020bf:	movzwl 0x6(%rcx),%eax
+   1800020c3:	lea    (%rax,%rax,4),%rcx
+   1800020c7:	lea    (%rdx,%rcx,8),%r9
+   1800020cb:	mov    %rdx,(%rsp)
+   1800020cf:	cmp    %r9,%rdx
+   1800020d2:	je     0x1800020ec
+   1800020d4:	mov    0xc(%rdx),%ecx
+   1800020d7:	cmp    %rcx,%r8
+   1800020da:	jb     0x1800020e6
+   1800020dc:	mov    0x8(%rdx),%eax
+   1800020df:	add    %ecx,%eax
+   1800020e1:	cmp    %rax,%r8
+   1800020e4:	jb     0x1800020ee
+   1800020e6:	add    $0x28,%rdx
+   1800020ea:	jmp    0x1800020cb
+   1800020ec:	xor    %edx,%edx
+   1800020ee:	test   %rdx,%rdx
+   1800020f1:	jne    0x1800020f7
+   1800020f3:	xor    %al,%al
+   1800020f5:	jmp    0x18000210b
+   1800020f7:	cmpl   $0x0,0x24(%rdx)
+   1800020fb:	jge    0x180002101
+   1800020fd:	xor    %al,%al
+   1800020ff:	jmp    0x18000210b
+   180002101:	mov    $0x1,%al
+   180002103:	jmp    0x18000210b
+   180002105:	xor    %al,%al
+   180002107:	jmp    0x18000210b
+   180002109:	xor    %al,%al
+   18000210b:	add    $0x18,%rsp
    18000210f:	ret
-   180002110:	andl   $0x0,0x7ec81(%rip)        # 0x180080d98
-   180002117:	ret
-   180002118:	mov    %rbx,0x8(%rsp)
-   18000211d:	push   %rbp
-   18000211e:	lea    -0x4c0(%rsp),%rbp
-   180002126:	sub    $0x5c0,%rsp
-   18000212d:	mov    %ecx,%ebx
-   18000212f:	mov    $0x17,%ecx
-   180002134:	call   *0xef6(%rip)        # 0x180003030
-   18000213a:	test   %eax,%eax
-   18000213c:	je     0x180002142
-   18000213e:	mov    %ebx,%ecx
-   180002140:	int    $0x29
-   180002142:	mov    $0x3,%ecx
-   180002147:	call   0x180002110
-   18000214c:	xor    %edx,%edx
-   18000214e:	lea    -0x10(%rbp),%rcx
-   180002152:	mov    $0x4d0,%r8d
-   180002158:	call   0x1800024a0
-   18000215d:	lea    -0x10(%rbp),%rcx
-   180002161:	call   *0xef9(%rip)        # 0x180003060
-   180002167:	mov    0xe8(%rbp),%rbx
-   18000216e:	lea    0x4d8(%rbp),%rdx
-   180002175:	mov    %rbx,%rcx
-   180002178:	xor    %r8d,%r8d
-   18000217b:	call   *0xed7(%rip)        # 0x180003058
-   180002181:	test   %rax,%rax
-   180002184:	je     0x1800021c2
-   180002186:	andq   $0x0,0x38(%rsp)
-   18000218c:	lea    0x4e0(%rbp),%rcx
-   180002193:	mov    0x4d8(%rbp),%rdx
-   18000219a:	mov    %rax,%r9
-   18000219d:	mov    %rcx,0x30(%rsp)
-   1800021a2:	mov    %rbx,%r8
-   1800021a5:	lea    0x4e8(%rbp),%rcx
-   1800021ac:	mov    %rcx,0x28(%rsp)
-   1800021b1:	lea    -0x10(%rbp),%rcx
-   1800021b5:	mov    %rcx,0x20(%rsp)
-   1800021ba:	xor    %ecx,%ecx
-   1800021bc:	call   *0xe8e(%rip)        # 0x180003050
-   1800021c2:	mov    0x4c8(%rbp),%rax
-   1800021c9:	lea    0x50(%rsp),%rcx
-   1800021ce:	mov    %rax,0xe8(%rbp)
-   1800021d5:	xor    %edx,%edx
-   1800021d7:	lea    0x4c8(%rbp),%rax
-   1800021de:	mov    $0x98,%r8d
-   1800021e4:	add    $0x8,%rax
-   1800021e8:	mov    %rax,0x88(%rbp)
-   1800021ef:	call   0x1800024a0
-   1800021f4:	mov    0x4c8(%rbp),%rax
-   1800021fb:	mov    %rax,0x60(%rsp)
-   180002200:	movl   $0x40000015,0x50(%rsp)
-   180002208:	movl   $0x1,0x54(%rsp)
-   180002210:	call   *0xdea(%rip)        # 0x180003000
-   180002216:	cmp    $0x1,%eax
-   180002219:	lea    0x50(%rsp),%rax
-   18000221e:	mov    %rax,0x40(%rsp)
-   180002223:	lea    -0x10(%rbp),%rax
-   180002227:	sete   %bl
-   18000222a:	mov    %rax,0x48(%rsp)
-   18000222f:	xor    %ecx,%ecx
-   180002231:	call   *0xe01(%rip)        # 0x180003038
-   180002237:	lea    0x40(%rsp),%rcx
-   18000223c:	call   *0xdfe(%rip)        # 0x180003040
-   180002242:	test   %eax,%eax
-   180002244:	jne    0x180002252
-   180002246:	test   %bl,%bl
-   180002248:	jne    0x180002252
-   18000224a:	lea    0x3(%rax),%ecx
-   18000224d:	call   0x180002110
-   180002252:	mov    0x5d0(%rsp),%rbx
-   18000225a:	add    $0x5c0,%rsp
-   180002261:	pop    %rbp
-   180002262:	ret
-   180002263:	int3
-   180002264:	mov    %rbx,0x8(%rsp)
-   180002269:	push   %rdi
-   18000226a:	sub    $0x20,%rsp
-   18000226e:	lea    0x1313(%rip),%rbx        # 0x180003588
-   180002275:	lea    0x130c(%rip),%rdi        # 0x180003588
-   18000227c:	jmp    0x180002290
-   18000227e:	mov    (%rbx),%rax
-   180002281:	test   %rax,%rax
-   180002284:	je     0x18000228c
-   180002286:	call   *0xe64(%rip)        # 0x1800030f0
-   18000228c:	add    $0x8,%rbx
-   180002290:	cmp    %rdi,%rbx
-   180002293:	jb     0x18000227e
-   180002295:	mov    0x30(%rsp),%rbx
-   18000229a:	add    $0x20,%rsp
-   18000229e:	pop    %rdi
-   18000229f:	ret
-   1800022a0:	mov    %rbx,0x8(%rsp)
-   1800022a5:	push   %rdi
-   1800022a6:	sub    $0x20,%rsp
-   1800022aa:	lea    0x12e7(%rip),%rbx        # 0x180003598
-   1800022b1:	lea    0x12e0(%rip),%rdi        # 0x180003598
-   1800022b8:	jmp    0x1800022cc
-   1800022ba:	mov    (%rbx),%rax
-   1800022bd:	test   %rax,%rax
-   1800022c0:	je     0x1800022c8
-   1800022c2:	call   *0xe28(%rip)        # 0x1800030f0
-   1800022c8:	add    $0x8,%rbx
-   1800022cc:	cmp    %rdi,%rbx
-   1800022cf:	jb     0x1800022ba
-   1800022d1:	mov    0x30(%rsp),%rbx
-   1800022d6:	add    $0x20,%rsp
-   1800022da:	pop    %rdi
-   1800022db:	ret
-   1800022dc:	ret    $0x0
-   1800022df:	int3
-   1800022e0:	mov    %rbx,0x10(%rsp)
-   1800022e5:	mov    %rsi,0x18(%rsp)
-   1800022ea:	push   %rdi
-   1800022eb:	sub    $0x10,%rsp
-   1800022ef:	xor    %eax,%eax
-   1800022f1:	xor    %ecx,%ecx
-   1800022f3:	cpuid
-   1800022f5:	mov    %ecx,%r8d
-   1800022f8:	xor    %r11d,%r11d
-   1800022fb:	mov    %edx,%r10d
-   1800022fe:	xor    $0x6c65746e,%r8d
-   180002305:	xor    $0x49656e69,%r10d
-   18000230c:	mov    %ebx,%r9d
-   18000230f:	mov    %eax,%esi
-   180002311:	xor    %ecx,%ecx
-   180002313:	lea    0x1(%r11),%eax
-   180002317:	or     %r8d,%r10d
-   18000231a:	cpuid
-   18000231c:	xor    $0x756e6547,%r9d
-   180002323:	mov    %eax,(%rsp)
-   180002326:	or     %r9d,%r10d
-   180002329:	mov    %ebx,0x4(%rsp)
-   18000232d:	mov    %ecx,%edi
-   18000232f:	mov    %ecx,0x8(%rsp)
-   180002333:	mov    %edx,0xc(%rsp)
-   180002337:	jne    0x180002394
-   180002339:	orq    $0xffffffffffffffff,0x1ce7(%rip)        # 0x180004028
-   180002341:	and    $0xfff3ff0,%eax
-   180002346:	movq   $0x8000,0x1ccf(%rip)        # 0x180004020
-   180002351:	cmp    $0x106c0,%eax
-   180002356:	je     0x180002380
-   180002358:	cmp    $0x20660,%eax
-   18000235d:	je     0x180002380
-   18000235f:	cmp    $0x20670,%eax
-   180002364:	je     0x180002380
-   180002366:	add    $0xfffcf9b0,%eax
-   18000236b:	cmp    $0x20,%eax
-   18000236e:	ja     0x180002394
-   180002370:	movabs $0x100010001,%rcx
-   18000237a:	bt     %rax,%rcx
-   18000237e:	jae    0x180002394
-   180002380:	mov    0x7ea15(%rip),%r8d        # 0x180080d9c
-   180002387:	or     $0x1,%r8d
-   18000238b:	mov    %r8d,0x7ea0a(%rip)        # 0x180080d9c
-   180002392:	jmp    0x18000239b
-   180002394:	mov    0x7ea01(%rip),%r8d        # 0x180080d9c
-   18000239b:	mov    $0x7,%eax
-   1800023a0:	lea    -0x5(%rax),%r9d
-   1800023a4:	cmp    %eax,%esi
-   1800023a6:	jl     0x1800023ce
-   1800023a8:	xor    %ecx,%ecx
-   1800023aa:	cpuid
-   1800023ac:	mov    %eax,(%rsp)
-   1800023af:	mov    %ebx,%r11d
-   1800023b2:	mov    %ebx,0x4(%rsp)
-   1800023b6:	mov    %ecx,0x8(%rsp)
-   1800023ba:	mov    %edx,0xc(%rsp)
-   1800023be:	bt     $0x9,%ebx
-   1800023c2:	jae    0x1800023ce
-   1800023c4:	or     %r9d,%r8d
-   1800023c7:	mov    %r8d,0x7e9ce(%rip)        # 0x180080d9c
-   1800023ce:	movl   $0x1,0x1c40(%rip)        # 0x180004018
-   1800023d8:	mov    %r9d,0x1c3d(%rip)        # 0x18000401c
-   1800023df:	bt     $0x14,%edi
-   1800023e3:	jae    0x18000247a
-   1800023e9:	mov    %r9d,0x1c28(%rip)        # 0x180004018
-   1800023f0:	mov    $0x6,%ebx
-   1800023f5:	mov    %ebx,0x1c21(%rip)        # 0x18000401c
-   1800023fb:	bt     $0x1b,%edi
-   1800023ff:	jae    0x18000247a
-   180002401:	bt     $0x1c,%edi
-   180002405:	jae    0x18000247a
-   180002407:	xor    %ecx,%ecx
-   180002409:	xgetbv
-   18000240c:	shl    $0x20,%rdx
-   180002410:	or     %rax,%rdx
-   180002413:	mov    %rdx,0x20(%rsp)
-   180002418:	mov    0x20(%rsp),%rax
-   18000241d:	and    %bl,%al
-   18000241f:	cmp    %bl,%al
-   180002421:	jne    0x18000247a
-   180002423:	mov    0x1bf3(%rip),%eax        # 0x18000401c
-   180002429:	or     $0x8,%eax
-   18000242c:	movl   $0x3,0x1be2(%rip)        # 0x180004018
-   180002436:	mov    %eax,0x1be0(%rip)        # 0x18000401c
-   18000243c:	test   $0x20,%r11b
-   180002440:	je     0x18000247a
-   180002442:	or     $0x20,%eax
-   180002445:	movl   $0x5,0x1bc9(%rip)        # 0x180004018
-   18000244f:	mov    %eax,0x1bc7(%rip)        # 0x18000401c
-   180002455:	mov    $0xd0030000,%eax
-   18000245a:	and    %eax,%r11d
-   18000245d:	cmp    %eax,%r11d
-   180002460:	jne    0x18000247a
-   180002462:	mov    0x20(%rsp),%rax
-   180002467:	and    $0xe0,%al
-   180002469:	cmp    $0xe0,%al
-   18000246b:	jne    0x18000247a
-   18000246d:	orl    $0x40,0x1ba8(%rip)        # 0x18000401c
-   180002474:	mov    %ebx,0x1b9e(%rip)        # 0x180004018
-   18000247a:	mov    0x28(%rsp),%rbx
-   18000247f:	xor    %eax,%eax
-   180002481:	mov    0x30(%rsp),%rsi
-   180002486:	add    $0x10,%rsp
-   18000248a:	pop    %rdi
-   18000248b:	ret
-   18000248c:	mov    $0x1,%eax
-   180002491:	ret
-   180002492:	int3
-   180002493:	int3
-   180002494:	xor    %eax,%eax
-   180002496:	cmp    %eax,0x1b94(%rip)        # 0x180004030
-   18000249c:	setne  %al
-   18000249f:	ret
-   1800024a0:	jmp    *0xbe2(%rip)        # 0x180003088
-   1800024a6:	jmp    *0xbd4(%rip)        # 0x180003080
-   1800024ac:	jmp    *0xbc6(%rip)        # 0x180003078
-   1800024b2:	jmp    *0xc18(%rip)        # 0x1800030d0
-   1800024b8:	jmp    *0xc0a(%rip)        # 0x1800030c8
-   1800024be:	jmp    *0xbfc(%rip)        # 0x1800030c0
-   1800024c4:	jmp    *0xbee(%rip)        # 0x1800030b8
-   1800024ca:	jmp    *0xbe0(%rip)        # 0x1800030b0
-   1800024d0:	jmp    *0xbd2(%rip)        # 0x1800030a8
-   1800024d6:	jmp    *0xbc4(%rip)        # 0x1800030a0
-   1800024dc:	jmp    *0xbb6(%rip)        # 0x180003098
-   1800024e2:	int3
-   1800024e3:	int3
-   1800024e4:	mov    $0x1,%al
-   1800024e6:	ret
-   1800024e7:	int3
-   1800024e8:	xor    %eax,%eax
-   1800024ea:	ret
-   1800024eb:	jmp    *0xb7f(%rip)        # 0x180003070
-   1800024f1:	int3
-   1800024f2:	int3
-   1800024f3:	int3
-   1800024f4:	int3
-   1800024f5:	int3
-   1800024f6:	int3
-   1800024f7:	int3
+   180002110:	rex push %rbx
+   180002112:	sub    $0x20,%rsp
+   180002116:	mov    %cl,%bl
+   180002118:	call   0x1800024ec
+   18000211d:	xor    %edx,%edx
+   18000211f:	test   %eax,%eax
+   180002121:	je     0x18000212e
+   180002123:	test   %bl,%bl
+   180002125:	jne    0x18000212e
+   180002127:	xchg   %rdx,0x7ec2a(%rip)        # 0x180080d58
+   18000212e:	add    $0x20,%rsp
+   180002132:	pop    %rbx
+   180002133:	ret
+   180002134:	rex push %rbx
+   180002136:	sub    $0x20,%rsp
+   18000213a:	cmpb   $0x0,0x7ec1f(%rip)        # 0x180080d60
+   180002141:	mov    %cl,%bl
+   180002143:	je     0x180002149
+   180002145:	test   %dl,%dl
+   180002147:	jne    0x180002155
+   180002149:	call   0x180002544
+   18000214e:	mov    %bl,%cl
+   180002150:	call   0x180002544
+   180002155:	mov    $0x1,%al
+   180002157:	add    $0x20,%rsp
+   18000215b:	pop    %rbx
+   18000215c:	ret
+   18000215d:	int3
+   18000215e:	int3
+   18000215f:	int3
+   180002160:	lea    0x7ec39(%rip),%rax        # 0x180080da0
+   180002167:	ret
+   180002168:	andl   $0x0,0x7ec29(%rip)        # 0x180080d98
+   18000216f:	ret
+   180002170:	mov    %rbx,0x8(%rsp)
+   180002175:	push   %rbp
+   180002176:	lea    -0x4c0(%rsp),%rbp
+   18000217e:	sub    $0x5c0,%rsp
+   180002185:	mov    %ecx,%ebx
+   180002187:	mov    $0x17,%ecx
+   18000218c:	call   *0xe9e(%rip)        # 0x180003030
+   180002192:	test   %eax,%eax
+   180002194:	je     0x18000219a
+   180002196:	mov    %ebx,%ecx
+   180002198:	int    $0x29
+   18000219a:	mov    $0x3,%ecx
+   18000219f:	call   0x180002168
+   1800021a4:	xor    %edx,%edx
+   1800021a6:	lea    -0x10(%rbp),%rcx
+   1800021aa:	mov    $0x4d0,%r8d
+   1800021b0:	call   0x180002500
+   1800021b5:	lea    -0x10(%rbp),%rcx
+   1800021b9:	call   *0xea1(%rip)        # 0x180003060
+   1800021bf:	mov    0xe8(%rbp),%rbx
+   1800021c6:	lea    0x4d8(%rbp),%rdx
+   1800021cd:	mov    %rbx,%rcx
+   1800021d0:	xor    %r8d,%r8d
+   1800021d3:	call   *0xe7f(%rip)        # 0x180003058
+   1800021d9:	test   %rax,%rax
+   1800021dc:	je     0x18000221a
+   1800021de:	andq   $0x0,0x38(%rsp)
+   1800021e4:	lea    0x4e0(%rbp),%rcx
+   1800021eb:	mov    0x4d8(%rbp),%rdx
+   1800021f2:	mov    %rax,%r9
+   1800021f5:	mov    %rcx,0x30(%rsp)
+   1800021fa:	mov    %rbx,%r8
+   1800021fd:	lea    0x4e8(%rbp),%rcx
+   180002204:	mov    %rcx,0x28(%rsp)
+   180002209:	lea    -0x10(%rbp),%rcx
+   18000220d:	mov    %rcx,0x20(%rsp)
+   180002212:	xor    %ecx,%ecx
+   180002214:	call   *0xe36(%rip)        # 0x180003050
+   18000221a:	mov    0x4c8(%rbp),%rax
+   180002221:	lea    0x50(%rsp),%rcx
+   180002226:	mov    %rax,0xe8(%rbp)
+   18000222d:	xor    %edx,%edx
+   18000222f:	lea    0x4c8(%rbp),%rax
+   180002236:	mov    $0x98,%r8d
+   18000223c:	add    $0x8,%rax
+   180002240:	mov    %rax,0x88(%rbp)
+   180002247:	call   0x180002500
+   18000224c:	mov    0x4c8(%rbp),%rax
+   180002253:	mov    %rax,0x60(%rsp)
+   180002258:	movl   $0x40000015,0x50(%rsp)
+   180002260:	movl   $0x1,0x54(%rsp)
+   180002268:	call   *0xd92(%rip)        # 0x180003000
+   18000226e:	cmp    $0x1,%eax
+   180002271:	lea    0x50(%rsp),%rax
+   180002276:	mov    %rax,0x40(%rsp)
+   18000227b:	lea    -0x10(%rbp),%rax
+   18000227f:	sete   %bl
+   180002282:	mov    %rax,0x48(%rsp)
+   180002287:	xor    %ecx,%ecx
+   180002289:	call   *0xda9(%rip)        # 0x180003038
+   18000228f:	lea    0x40(%rsp),%rcx
+   180002294:	call   *0xda6(%rip)        # 0x180003040
+   18000229a:	test   %eax,%eax
+   18000229c:	jne    0x1800022aa
+   18000229e:	test   %bl,%bl
+   1800022a0:	jne    0x1800022aa
+   1800022a2:	lea    0x3(%rax),%ecx
+   1800022a5:	call   0x180002168
+   1800022aa:	mov    0x5d0(%rsp),%rbx
+   1800022b2:	add    $0x5c0,%rsp
+   1800022b9:	pop    %rbp
+   1800022ba:	ret
+   1800022bb:	int3
+   1800022bc:	mov    %rbx,0x8(%rsp)
+   1800022c1:	push   %rdi
+   1800022c2:	sub    $0x20,%rsp
+   1800022c6:	lea    0x12bb(%rip),%rbx        # 0x180003588
+   1800022cd:	lea    0x12b4(%rip),%rdi        # 0x180003588
+   1800022d4:	jmp    0x1800022e8
+   1800022d6:	mov    (%rbx),%rax
+   1800022d9:	test   %rax,%rax
+   1800022dc:	je     0x1800022e4
+   1800022de:	call   *0xe0c(%rip)        # 0x1800030f0
+   1800022e4:	add    $0x8,%rbx
+   1800022e8:	cmp    %rdi,%rbx
+   1800022eb:	jb     0x1800022d6
+   1800022ed:	mov    0x30(%rsp),%rbx
+   1800022f2:	add    $0x20,%rsp
+   1800022f6:	pop    %rdi
+   1800022f7:	ret
+   1800022f8:	mov    %rbx,0x8(%rsp)
+   1800022fd:	push   %rdi
+   1800022fe:	sub    $0x20,%rsp
+   180002302:	lea    0x128f(%rip),%rbx        # 0x180003598
+   180002309:	lea    0x1288(%rip),%rdi        # 0x180003598
+   180002310:	jmp    0x180002324
+   180002312:	mov    (%rbx),%rax
+   180002315:	test   %rax,%rax
+   180002318:	je     0x180002320
+   18000231a:	call   *0xdd0(%rip)        # 0x1800030f0
+   180002320:	add    $0x8,%rbx
+   180002324:	cmp    %rdi,%rbx
+   180002327:	jb     0x180002312
+   180002329:	mov    0x30(%rsp),%rbx
+   18000232e:	add    $0x20,%rsp
+   180002332:	pop    %rdi
+   180002333:	ret
+   180002334:	ret    $0x0
+   180002337:	int3
+   180002338:	mov    %rbx,0x10(%rsp)
+   18000233d:	mov    %rsi,0x18(%rsp)
+   180002342:	push   %rdi
+   180002343:	sub    $0x10,%rsp
+   180002347:	xor    %eax,%eax
+   180002349:	xor    %ecx,%ecx
+   18000234b:	cpuid
+   18000234d:	mov    %ecx,%r8d
+   180002350:	xor    %r11d,%r11d
+   180002353:	mov    %edx,%r10d
+   180002356:	xor    $0x6c65746e,%r8d
+   18000235d:	xor    $0x49656e69,%r10d
+   180002364:	mov    %ebx,%r9d
+   180002367:	mov    %eax,%esi
+   180002369:	xor    %ecx,%ecx
+   18000236b:	lea    0x1(%r11),%eax
+   18000236f:	or     %r8d,%r10d
+   180002372:	cpuid
+   180002374:	xor    $0x756e6547,%r9d
+   18000237b:	mov    %eax,(%rsp)
+   18000237e:	or     %r9d,%r10d
+   180002381:	mov    %ebx,0x4(%rsp)
+   180002385:	mov    %ecx,%edi
+   180002387:	mov    %ecx,0x8(%rsp)
+   18000238b:	mov    %edx,0xc(%rsp)
+   18000238f:	jne    0x1800023ec
+   180002391:	orq    $0xffffffffffffffff,0x1c8f(%rip)        # 0x180004028
+   180002399:	and    $0xfff3ff0,%eax
+   18000239e:	movq   $0x8000,0x1c77(%rip)        # 0x180004020
+   1800023a9:	cmp    $0x106c0,%eax
+   1800023ae:	je     0x1800023d8
+   1800023b0:	cmp    $0x20660,%eax
+   1800023b5:	je     0x1800023d8
+   1800023b7:	cmp    $0x20670,%eax
+   1800023bc:	je     0x1800023d8
+   1800023be:	add    $0xfffcf9b0,%eax
+   1800023c3:	cmp    $0x20,%eax
+   1800023c6:	ja     0x1800023ec
+   1800023c8:	movabs $0x100010001,%rcx
+   1800023d2:	bt     %rax,%rcx
+   1800023d6:	jae    0x1800023ec
+   1800023d8:	mov    0x7e9bd(%rip),%r8d        # 0x180080d9c
+   1800023df:	or     $0x1,%r8d
+   1800023e3:	mov    %r8d,0x7e9b2(%rip)        # 0x180080d9c
+   1800023ea:	jmp    0x1800023f3
+   1800023ec:	mov    0x7e9a9(%rip),%r8d        # 0x180080d9c
+   1800023f3:	mov    $0x7,%eax
+   1800023f8:	lea    -0x5(%rax),%r9d
+   1800023fc:	cmp    %eax,%esi
+   1800023fe:	jl     0x180002426
+   180002400:	xor    %ecx,%ecx
+   180002402:	cpuid
+   180002404:	mov    %eax,(%rsp)
+   180002407:	mov    %ebx,%r11d
+   18000240a:	mov    %ebx,0x4(%rsp)
+   18000240e:	mov    %ecx,0x8(%rsp)
+   180002412:	mov    %edx,0xc(%rsp)
+   180002416:	bt     $0x9,%ebx
+   18000241a:	jae    0x180002426
+   18000241c:	or     %r9d,%r8d
+   18000241f:	mov    %r8d,0x7e976(%rip)        # 0x180080d9c
+   180002426:	movl   $0x1,0x1be8(%rip)        # 0x180004018
+   180002430:	mov    %r9d,0x1be5(%rip)        # 0x18000401c
+   180002437:	bt     $0x14,%edi
+   18000243b:	jae    0x1800024d2
+   180002441:	mov    %r9d,0x1bd0(%rip)        # 0x180004018
+   180002448:	mov    $0x6,%ebx
+   18000244d:	mov    %ebx,0x1bc9(%rip)        # 0x18000401c
+   180002453:	bt     $0x1b,%edi
+   180002457:	jae    0x1800024d2
+   180002459:	bt     $0x1c,%edi
+   18000245d:	jae    0x1800024d2
+   18000245f:	xor    %ecx,%ecx
+   180002461:	xgetbv
+   180002464:	shl    $0x20,%rdx
+   180002468:	or     %rax,%rdx
+   18000246b:	mov    %rdx,0x20(%rsp)
+   180002470:	mov    0x20(%rsp),%rax
+   180002475:	and    %bl,%al
+   180002477:	cmp    %bl,%al
+   180002479:	jne    0x1800024d2
+   18000247b:	mov    0x1b9b(%rip),%eax        # 0x18000401c
+   180002481:	or     $0x8,%eax
+   180002484:	movl   $0x3,0x1b8a(%rip)        # 0x180004018
+   18000248e:	mov    %eax,0x1b88(%rip)        # 0x18000401c
+   180002494:	test   $0x20,%r11b
+   180002498:	je     0x1800024d2
+   18000249a:	or     $0x20,%eax
+   18000249d:	movl   $0x5,0x1b71(%rip)        # 0x180004018
+   1800024a7:	mov    %eax,0x1b6f(%rip)        # 0x18000401c
+   1800024ad:	mov    $0xd0030000,%eax
+   1800024b2:	and    %eax,%r11d
+   1800024b5:	cmp    %eax,%r11d
+   1800024b8:	jne    0x1800024d2
+   1800024ba:	mov    0x20(%rsp),%rax
+   1800024bf:	and    $0xe0,%al
+   1800024c1:	cmp    $0xe0,%al
+   1800024c3:	jne    0x1800024d2
+   1800024c5:	orl    $0x40,0x1b50(%rip)        # 0x18000401c
+   1800024cc:	mov    %ebx,0x1b46(%rip)        # 0x180004018
+   1800024d2:	mov    0x28(%rsp),%rbx
+   1800024d7:	xor    %eax,%eax
+   1800024d9:	mov    0x30(%rsp),%rsi
+   1800024de:	add    $0x10,%rsp
+   1800024e2:	pop    %rdi
+   1800024e3:	ret
+   1800024e4:	mov    $0x1,%eax
+   1800024e9:	ret
+   1800024ea:	int3
+   1800024eb:	int3
+   1800024ec:	xor    %eax,%eax
+   1800024ee:	cmp    %eax,0x1b3c(%rip)        # 0x180004030
+   1800024f4:	setne  %al
+   1800024f7:	ret
    1800024f8:	int3
    1800024f9:	int3
    1800024fa:	int3
    1800024fb:	int3
    1800024fc:	int3
    1800024fd:	int3
    1800024fe:	int3
    1800024ff:	int3
-   180002500:	int3
-   180002501:	int3
-   180002502:	int3
-   180002503:	int3
-   180002504:	int3
-   180002505:	int3
-   180002506:	data16 nopw 0x0(%rax,%rax,1)
-   180002510:	jmp    *%rax
-   180002512:	int3
-   180002513:	int3
-   180002514:	int3
-   180002515:	int3
-   180002516:	int3
-   180002517:	int3
-   180002518:	int3
-   180002519:	int3
-   18000251a:	int3
-   18000251b:	int3
-   18000251c:	int3
-   18000251d:	int3
-   18000251e:	int3
-   18000251f:	int3
-   180002520:	int3
-   180002521:	int3
-   180002522:	int3
-   180002523:	int3
-   180002524:	int3
-   180002525:	int3
-   180002526:	data16 nopw 0x0(%rax,%rax,1)
-   180002530:	jmp    *0xbba(%rip)        # 0x1800030f0
-   180002536:	rex push %rbp
-   180002538:	sub    $0x20,%rsp
-   18000253c:	mov    %rdx,%rbp
-   18000253f:	mov    0x40(%rbp),%cl
-   180002542:	add    $0x20,%rsp
-   180002546:	pop    %rbp
-   180002547:	jmp    0x1800020b8
-   18000254c:	int3
-   18000254d:	rex push %rbp
-   18000254f:	sub    $0x20,%rsp
-   180002553:	mov    %rdx,%rbp
-   180002556:	mov    0x20(%rbp),%cl
-   180002559:	call   0x1800020b8
-   18000255e:	nop
-   18000255f:	add    $0x20,%rsp
-   180002563:	pop    %rbp
-   180002564:	ret
+   180002500:	jmp    *0xb82(%rip)        # 0x180003088
+   180002506:	jmp    *0xb74(%rip)        # 0x180003080
+   18000250c:	jmp    *0xb66(%rip)        # 0x180003078
+   180002512:	jmp    *0xbb8(%rip)        # 0x1800030d0
+   180002518:	jmp    *0xbaa(%rip)        # 0x1800030c8
+   18000251e:	jmp    *0xb9c(%rip)        # 0x1800030c0
+   180002524:	jmp    *0xb8e(%rip)        # 0x1800030b8
+   18000252a:	jmp    *0xb80(%rip)        # 0x1800030b0
+   180002530:	jmp    *0xb72(%rip)        # 0x1800030a8
+   180002536:	jmp    *0xb64(%rip)        # 0x1800030a0
+   18000253c:	jmp    *0xb56(%rip)        # 0x180003098
+   180002542:	int3
+   180002543:	int3
+   180002544:	mov    $0x1,%al
+   180002546:	ret
+   180002547:	int3
+   180002548:	xor    %eax,%eax
+   18000254a:	ret
+   18000254b:	jmp    *0xb1f(%rip)        # 0x180003070
+   180002551:	int3
+   180002552:	int3
+   180002553:	int3
+   180002554:	int3
+   180002555:	int3
+   180002556:	int3
+   180002557:	int3
+   180002558:	int3
+   180002559:	int3
+   18000255a:	int3
+   18000255b:	int3
+   18000255c:	int3
+   18000255d:	int3
+   18000255e:	int3
+   18000255f:	int3
+   180002560:	int3
+   180002561:	int3
+   180002562:	int3
+   180002563:	int3
+   180002564:	int3
    180002565:	int3
-   180002566:	rex push %rbp
-   180002568:	sub    $0x20,%rsp
-   18000256c:	mov    %rdx,%rbp
-   18000256f:	add    $0x20,%rsp
-   180002573:	pop    %rbp
-   180002574:	jmp    0x180001f34
+   180002566:	data16 nopw 0x0(%rax,%rax,1)
+   180002570:	jmp    *%rax
+   180002572:	int3
+   180002573:	int3
+   180002574:	int3
+   180002575:	int3
+   180002576:	int3
+   180002577:	int3
+   180002578:	int3
    180002579:	int3
-   18000257a:	rex push %rbp
-   18000257c:	sub    $0x30,%rsp
-   180002580:	mov    %rdx,%rbp
-   180002583:	mov    (%rcx),%rax
-   180002586:	mov    (%rax),%edx
-   180002588:	mov    %rcx,0x28(%rsp)
-   18000258d:	mov    %edx,0x20(%rsp)
-   180002591:	lea    -0xc34(%rip),%r9        # 0x180001964
-   180002598:	mov    0x70(%rbp),%r8
-   18000259c:	mov    0x68(%rbp),%edx
-   18000259f:	mov    0x60(%rbp),%rcx
-   1800025a3:	call   0x180001ea4
-   1800025a8:	nop
-   1800025a9:	add    $0x30,%rsp
-   1800025ad:	pop    %rbp
-   1800025ae:	ret
-   1800025af:	int3
-   1800025b0:	rex push %rbp
-   1800025b2:	mov    %rdx,%rbp
-   1800025b5:	mov    (%rcx),%rax
-   1800025b8:	xor    %ecx,%ecx
-   1800025ba:	cmpl   $0xc0000005,(%rax)
-   1800025c0:	sete   %cl
-   1800025c3:	mov    %ecx,%eax
-   1800025c5:	pop    %rbp
-   1800025c6:	ret
-   1800025c7:	int3
+   18000257a:	int3
+   18000257b:	int3
+   18000257c:	int3
+   18000257d:	int3
+   18000257e:	int3
+   18000257f:	int3
+   180002580:	int3
+   180002581:	int3
+   180002582:	int3
+   180002583:	int3
+   180002584:	int3
+   180002585:	int3
+   180002586:	data16 nopw 0x0(%rax,%rax,1)
+   180002590:	jmp    *0xb5a(%rip)        # 0x1800030f0
+   180002596:	rex push %rbp
+   180002598:	sub    $0x20,%rsp
+   18000259c:	mov    %rdx,%rbp
+   18000259f:	mov    0x40(%rbp),%cl
+   1800025a2:	add    $0x20,%rsp
+   1800025a6:	pop    %rbp
+   1800025a7:	jmp    0x180002110
+   1800025ac:	int3
+   1800025ad:	rex push %rbp
+   1800025af:	sub    $0x20,%rsp
+   1800025b3:	mov    %rdx,%rbp
+   1800025b6:	mov    0x20(%rbp),%cl
+   1800025b9:	call   0x180002110
+   1800025be:	nop
+   1800025bf:	add    $0x20,%rsp
+   1800025c3:	pop    %rbp
+   1800025c4:	ret
+   1800025c5:	int3
+   1800025c6:	rex push %rbp
+   1800025c8:	sub    $0x20,%rsp
+   1800025cc:	mov    %rdx,%rbp
+   1800025cf:	add    $0x20,%rsp
+   1800025d3:	pop    %rbp
+   1800025d4:	jmp    0x180001f8c
+   1800025d9:	int3
+   1800025da:	rex push %rbp
+   1800025dc:	sub    $0x30,%rsp
+   1800025e0:	mov    %rdx,%rbp
+   1800025e3:	mov    (%rcx),%rax
+   1800025e6:	mov    (%rax),%edx
+   1800025e8:	mov    %rcx,0x28(%rsp)
+   1800025ed:	mov    %edx,0x20(%rsp)
+   1800025f1:	lea    -0xc3c(%rip),%r9        # 0x1800019bc
+   1800025f8:	mov    0x70(%rbp),%r8
+   1800025fc:	mov    0x68(%rbp),%edx
+   1800025ff:	mov    0x60(%rbp),%rcx
+   180002603:	call   0x180001efc
+   180002608:	nop
+   180002609:	add    $0x30,%rsp
+   18000260d:	pop    %rbp
+   18000260e:	ret
+   18000260f:	int3
+   180002610:	rex push %rbp
+   180002612:	mov    %rdx,%rbp
+   180002615:	mov    (%rcx),%rax
+   180002618:	xor    %ecx,%ecx
+   18000261a:	cmpl   $0xc0000005,(%rax)
+   180002620:	sete   %cl
+   180002623:	mov    %ecx,%eax
+   180002625:	pop    %rbp
+   180002626:	ret
+   180002627:	int3
 
 Disassembly of section .rdata:
 
 0000000180003000 <.rdata>:
-   180003000:	add    %bh,(%rax,%rax,1)
+   180003000:	adc    %bh,(%rax,%rax,1)
    180003003:	add    %al,(%rax)
    180003005:	add    %al,(%rax)
-   180003007:	add    %al,0x3b(%rsi)
+   180003007:	add    %dl,0x3b(%rsi)
    18000300a:	add    %al,(%rax)
    18000300c:	add    %al,(%rax)
    18000300e:	add    %al,(%rax)
-   180003010:	sub    $0x3b,%al
+   180003010:	cmp    $0x3b,%al
    180003012:	add    %al,(%rax)
    180003014:	add    %al,(%rax)
    180003016:	add    %al,(%rax)
-   180003018:	jb     0x180003055
-   18000301a:	add    %al,(%rax)
-   18000301c:	add    %al,(%rax)
-   18000301e:	add    %al,(%rax)
-   180003020:	mov    %?,(%rbx)
-   180003022:	add    %al,(%rax)
-   180003024:	add    %al,(%rax)
+   180003018:	(bad)
+   180003019:	cmp    (%rax),%eax
+   18000301b:	add    %al,(%rax)
+   18000301d:	add    %al,(%rax)
+   18000301f:	add    %bl,0x0(%rbx,%rdi,1)
    180003026:	add    %al,(%rax)
-   180003028:	test   $0x3b,%al
-   18000302a:	add    %al,(%rax)
-   18000302c:	add    %al,(%rax)
-   18000302e:	add    %al,(%rax)
-   180003030:	rex.WRX cmp $0x0,%al
-   180003033:	add    %al,(%rax)
-   180003035:	add    %al,(%rax)
-   180003037:	add    %dh,(%rax)
-   180003039:	cmp    $0x0,%al
+   180003028:	mov    $0x3b,%eax
+   18000302d:	add    %al,(%rax)
+   18000302f:	add    %bl,0x3c(%rsi)
+   180003032:	add    %al,(%rax)
+   180003034:	add    %al,(%rax)
+   180003036:	add    %al,(%rax)
+   180003038:	rex cmp $0x0,%al
    18000303b:	add    %al,(%rax)
    18000303d:	add    %al,(%rax)
-   18000303f:	add    %dl,(%rsp,%rdi,1)
+   18000303f:	add    %ah,(%rsp,%rdi,1)
    180003042:	add    %al,(%rax)
    180003044:	add    %al,(%rax)
    180003046:	add    %al,(%rax)
-   180003048:	pop    %rsp
+   180003048:	insb   (%dx),%es:(%rdi)
    180003049:	cmp    (%rax),%eax
    18000304b:	add    %al,(%rax)
    18000304d:	add    %al,(%rax)
-   18000304f:	add    %ch,%ah
+   18000304f:	add    %bh,%ah
    180003051:	cmp    (%rax),%eax
    180003053:	add    %al,(%rax)
    180003055:	add    %al,(%rax)
-   180003057:	add    %dl,%dl
+   180003057:	add    %ah,%dl
    180003059:	cmp    (%rax),%eax
    18000305b:	add    %al,(%rax)
    18000305d:	add    %al,(%rax)
-   18000305f:	add    %bh,0x3b(%rsi)
+   18000305f:	add    %cl,%dh
+   180003061:	cmp    (%rax),%eax
 	...
-   18000306d:	add    %al,(%rax)
-   18000306f:	add    %bh,0x3c(%rax)
-   180003072:	add    %al,(%rax)
-   180003074:	add    %al,(%rax)
-   180003076:	add    %al,(%rax)
-   180003078:	xor    (%rdx),%bh
+   18000306f:	add    %cl,0x3c(%rax)
+   180003075:	add    %al,(%rax)
+   180003077:	add    %al,0x3a(%rdx)
    18000307a:	add    %al,(%rax)
    18000307c:	add    %al,(%rax)
    18000307e:	add    %al,(%rax)
-   180003080:	sbb    (%rdx),%bh
+   180003080:	sub    (%rdx),%bh
    180003082:	add    %al,(%rax)
    180003084:	add    %al,(%rax)
    180003086:	add    %al,(%rax)
-   180003088:	adc    %bh,(%rdx)
+   180003088:	and    %bh,(%rdx)
 	...
    180003096:	add    %al,(%rax)
-   180003098:	add    %bh,(%rbx)
+   180003098:	adc    %bh,(%rbx)
    18000309a:	add    %al,(%rax)
    18000309c:	add    %al,(%rax)
    18000309e:	add    %al,(%rax)
-   1800030a0:	call   0x1800030df
+   1800030a0:	clc
+   1800030a1:	cmp    (%rax),%al
+   1800030a3:	add    %al,(%rax)
    1800030a5:	add    %al,(%rax)
-   1800030a7:	add    %cl,%ah
+   1800030a7:	add    %bl,%ah
    1800030a9:	cmp    (%rax),%al
    1800030ab:	add    %al,(%rax)
    1800030ad:	add    %al,(%rax)
-   1800030af:	add    %ch,0x3a(%rdx)
+   1800030af:	add    %bh,0x3a(%rdx)
    1800030b5:	add    %al,(%rax)
-   1800030b7:	add    %dl,0x3a(%rax)
+   1800030b7:	add    %ah,0x3a(%rax)
    1800030bd:	add    %al,(%rax)
-   1800030bf:	add    %bh,0x3a(%rsi)
-   1800030c2:	add    %al,(%rax)
-   1800030c4:	add    %al,(%rax)
-   1800030c6:	add    %al,(%rax)
-   1800030c8:	jo     0x180003104
-   1800030ca:	add    %al,(%rax)
-   1800030cc:	add    %al,(%rax)
-   1800030ce:	add    %al,(%rax)
-   1800030d0:	cmp    %fs:(%rax),%al
-	...
-   1800030df:	add    %bl,%ah
-   1800030e1:	and    (%rax),%al
-   1800030e3:	addb   $0x0,(%rcx)
-   1800030e6:	add    %al,(%rax)
-   1800030e8:	fsubl  (%rdx)
+   1800030bf:	add    %cl,0x3a(%rsi)
+   1800030c5:	add    %al,(%rax)
+   1800030c7:	add    %al,0x3a(%rax)
+   1800030cd:	add    %al,(%rax)
+   1800030cf:	add    %dh,0x0(%rdx,%rdi,1)
+	...
+   1800030df:	add    %dh,(%rbx,%riz,1)
+   1800030e2:	add    %al,0x1(%rax)
+   1800030e8:	xor    $0x23,%al
    1800030ea:	add    %al,0x1(%rax)
-   1800030f0:	adc    %ah,0x18000(%rip)        # 0x18001b0f6
-   1800030f6:	add    %al,(%rax)
-   1800030f8:	xor    %ah,0x18000(%rip)        # 0x18001b0fe
+   1800030f0:	jo     0x180003117
+   1800030f2:	add    %al,0x1(%rax)
+   1800030f8:	nop
+   1800030f9:	and    $0x18000,%eax
    1800030fe:	add    %al,(%rax)
-   180003100:	xor    %ah,0x18000(%rip)        # 0x18001b106
+   180003100:	nop
+   180003101:	and    $0x18000,%eax
 	...
    18000310e:	add    %al,(%rax)
-   180003110:	jmp    0x180003136
-   180003112:	add    %al,0x1(%rax)
+   180003110:	rex.WXB and $0x18000,%rax
 	...
+   18000316e:	add    %al,(%rax)
    180003170:	(bad)
    180003171:	(bad)
    180003172:	(bad)
    180003173:	(bad)
    180003174:	(bad)
    180003175:	(bad)
    180003176:	(bad)
@@ -2254,72 +2310,78 @@
    1800032aa:	add    %al,0x1(%rax)
    1800032b0:	or     %dh,(%rcx)
    1800032b2:	add    %al,0x1(%rax)
    1800032b8:	adc    %dh,(%rcx)
    1800032ba:	add    %al,0x1(%rax)
    1800032c0:	add    %al,(%rax)
    1800032c2:	add    %al,(%rax)
-   1800032c4:	rex.WXB
-   1800032c5:	es movabs 0xd0000000064,%al
-   1800032cf:	add    %dh,(%rax)
+   1800032c4:	rclb   %cl,-0x50(%rbp)
+   1800032c7:	add    %al,%fs:(%rax)
+   1800032ca:	add    %al,(%rax)
+   1800032cc:	or     $0x30000000,%eax
    1800032d1:	add    (%rax),%al
    1800032d3:	add    %dl,0x33(%rax)
    1800032d6:	add    %al,(%rax)
    1800032d8:	push   %rax
-   1800032d9:	sbb    $0x0,%eax
+   1800032d9:	(bad)
 	...
    1800032fe:	add    %al,(%rax)
    180003300:	sbb    %al,(%rax)
    180003302:	add    %al,(%rax)
    180003304:	add    0x33188002(%rax),%al
    18000330a:	add    %al,(%rax)
    18000330c:	and    %al,(%rax)
    18000330e:	add    %al,(%rax)
    180003310:	cmp    %dh,(%rbx)
    180003312:	add    %al,(%rax)
    180003314:	sbb    %al,(%rax)
    180003316:	add    %al,(%rax)
-   180003318:	jmp    0x17f00333a
-   18000331d:	sbb    $0x20cf0000,%eax
-   180003322:	add    %al,(%rax)
-   180003324:	ret    $0x21
-   180003327:	add    %dh,%ah
-   180003329:	and    %eax,(%rax)
-   18000332b:	add    %dl,(%rbx)
-   18000332d:	and    $0x0,%al
-   18000332f:	add    %bl,(%rax)
-   180003331:	and    $0x0,%al
-   180003333:	add    %ah,0x24(%rdx)
-   180003336:	add    %al,(%rax)
-   180003338:	add    %dl,(%rax)
-   18000333a:	add    %al,(%rax)
-   18000333c:	movabs 0x7000024e4000014,%al
+   180003318:	rex.B (bad)
+   18000331a:	add    %al,(%rax)
+   18000331c:	push   %rdi
+   18000331d:	(bad)
+   18000331e:	add    %al,(%rax)
+   180003320:	(bad)
+   180003321:	and    %eax,(%rax)
+   180003323:	add    %bl,(%rdx)
+   180003325:	and    (%rax),%al
+   180003327:	add    %cl,0x0(%rdx,%riz,1)
+   18000332b:	add    %ch,0x24(%rbx)
+   18000332e:	add    %al,(%rax)
+   180003330:	jo     0x180003356
+   180003332:	add    %al,(%rax)
+   180003334:	mov    $0x24,%edx
+   180003339:	adc    %al,(%rax)
+   18000333b:	add    %al,(%rax)
+   18000333d:	adc    $0x25440000,%eax
+   180003342:	add    %al,(%rax)
+   180003344:	(bad)
    180003345:	add    %al,(%rax)
-   180003347:	add    %dh,(%rsi)
-   180003349:	and    $0x920000,%eax
-   18000334e:	add    %al,(%rax)
-   180003350:	add    %al,(%rax)
-   180003352:	add    %al,(%rax)
-   180003354:	add    %dl,(%rax)
-   180003356:	add    %al,(%rax)
-   180003358:	add    %dl,0x742e0000(%rip)        # 0x1f42e335e
-   18000335e:	gs js  0x1800033d5
+   180003347:	add    %dl,-0x6dffffdb(%rsi)
+	...
+   180003355:	adc    %al,(%rax)
+   180003357:	add    %ah,0x15(%rax)
+   18000335a:	add    %al,(%rax)
+   18000335c:	je,pn  0x1800033c4
+   18000335f:	js     0x1800033d5
    180003361:	and    $0x6d,%al
    180003363:	outsb  %ds:(%rsi),(%dx)
    180003364:	add    %al,(%rax)
    180003366:	add    %al,(%rax)
-   180003368:	add    %ah,0x360000(%rip)        # 0x18036336e
+   180003368:	(bad)
+   180003369:	and    $0x360000,%eax
    18000336e:	add    %al,(%rax)
    180003370:	je,pn  0x1800033d8
    180003373:	js     0x1800033e9
    180003375:	and    $0x6d,%al
    180003377:	outsb  %ds:(%rsi),(%dx)
    180003378:	and    $0x30,%al
    18000337a:	xor    %al,(%rax)
-   18000337c:	ss and $0x920000,%eax
+   18000337c:	xchg   %eax,%esi
+   18000337d:	and    $0x920000,%eax
    180003382:	add    %al,(%rax)
    180003384:	je,pn  0x1800033ec
    180003387:	js     0x1800033fd
    180003389:	and    $0x78,%al
    18000338b:	add    %al,(%rax)
    18000338d:	xor    %al,(%rax)
    18000338f:	add    %ah,%al
@@ -2478,45 +2540,45 @@
    1800034d2:	add    %al,(%rax)
    1800034d4:	jb,pn  0x18000354b
    1800034d7:	movsxd (%rsp,%rdx,2),%esp
    1800034da:	pop    %rdx
    1800034db:	pop    %rdx
    1800034dc:	add    %al,(%rax)
    1800034de:	add    %al,(%rax)
-   1800034e0:	movabs 0x2e000002a0000035,%al
+   1800034e0:	movabs 0x2e000002b0000035,%al
    1800034e9:	js     0x18000354f
    1800034eb:	(bad)
    1800034ec:	je     0x18000354f
    1800034ee:	add    %al,(%rax)
-   1800034f0:	rex cmp %al,(%rax)
+   1800034f0:	push   %rax
+   1800034f1:	cmp    %al,(%rax)
    1800034f3:	add    %bl,0x652e0000(%rax,%rax,1)
    1800034fa:	fs (bad)
    1800034fc:	je     0x18000355f
    1800034fe:	add    %al,(%rax)
-   180003500:	fdivrl (%rax)
-   180003502:	add    %al,(%rax)
-   180003504:	cmp    $0x0,%al
+   180003500:	in     (%dx),%al
+   180003501:	cmp    %al,(%rax)
+   180003503:	add    %bh,(%rax,%rax,1)
    180003506:	add    %al,(%rax)
    180003508:	cs imul $0x322461,0x74(%rcx,%riz,2),%esp
    180003511:	add    %al,(%rax)
-   180003513:	add    %bl,(%rax)
+   180003513:	add    %ch,(%rax)
    180003515:	cmp    %eax,(%rax)
    180003517:	add    %bl,(%rax)
    180003519:	add    %al,(%rax)
    18000351b:	add    %ch,(%rsi)
    18000351d:	imul   $0x332461,0x74(%rcx,%riz,2),%esp
    180003525:	add    %al,(%rax)
-   180003527:	add    %dh,(%rax)
-   180003529:	cmp    %eax,(%rax)
-   18000352b:	add    %ah,%al
-   18000352d:	add    %al,(%rax)
-   18000352f:	add    %ch,(%rsi)
-   180003531:	imul   $0x342461,0x74(%rcx,%riz,2),%esp
+   180003527:	add    %al,0x39(%rax)
+   18000352a:	add    %al,(%rax)
+   18000352c:	loopne 0x18000352e
+   18000352e:	add    %al,(%rax)
+   180003530:	cs imul $0x342461,0x74(%rcx,%riz,2),%esp
    180003539:	add    %al,(%rax)
-   18000353b:	add    %dl,(%rax)
+   18000353b:	add    %ah,(%rax)
    18000353d:	cmp    (%rax),%al
    18000353f:	add    %dh,0x2(%rdx)
    180003542:	add    %al,(%rax)
    180003544:	cs imul $0x362461,0x74(%rcx,%riz,2),%esp
    18000354d:	add    %al,(%rax)
    18000354f:	add    %al,(%rax)
    180003551:	rex add %al,(%rax)
@@ -2536,709 +2598,714 @@
    180003573:	add    %dh,(%rdx,%rax,1)
    180003576:	add    %al,(%rax)
    180003578:	jo,pn  0x1800035df
    18000357b:	(bad)
    18000357c:	je     0x1800035df
 	...
    18000359e:	add    %al,(%rax)
-   1800035a0:	add    %edx,0x0(%rsi,%rax,1)
-   1800035a4:	push   %rsp
-   1800035a5:	or     %fs:(%rax),%eax
-   1800035a8:	cmp    0x5d20900(,%rcx,1),%dh
-   1800035af:	jo     0x1800035d2
-   1800035b1:	sbb    %ecx,(%rdx)
-   1800035b3:	add    %bl,(%rcx)
-   1800035b5:	hlt
-   1800035b6:	(bad)
-   1800035b7:	add    %dl,(%rsp,%riz,8)
-   1800035ba:	or     %al,(%rax)
-   1800035bc:	paddq  (%rcx),%mm1
+   1800035a0:	add    %edx,0x8(%rdx)
+   1800035a3:	add    %dl,0x74(%rdx)
+   1800035a6:	or     (%rax),%al
+   1800035a8:	rex.RX
+   1800035a9:	or     %fs:(%rax),%eax
+   1800035ac:	cmp    0x6d20a00(,%rcx,1),%esi
+   1800035b3:	shlb   (%rcx)
+   1800035b5:	adc    $0x8,%al
+   1800035b7:	add    %dl,(%rsp,%rsi,8)
+   1800035ba:	(bad)
+   1800035bb:	add    %cl,(%rdi)
+   1800035bd:	in     $0x8,%al
    1800035bf:	add    %cl,(%rdx)
    1800035c1:	(bad)
-   1800035c2:	or     (%rax),%al
+   1800035c2:	or     %eax,(%rax)
    1800035c4:	add    $0xc54,%eax
    1800035c9:	adc    %al,(%rax)
-   1800035cb:	add    %bh,0x35a00000(%rax,%rdx,1)
-   1800035d2:	add    %al,(%rax)
-   1800035d4:	and    %eax,(%rax)
-   1800035d6:	add    %al,(%rax)
-   1800035d8:	add    %dl,(%rax)
-   1800035da:	add    %al,(%rax)
-   1800035dc:	mov    $0xa0000010,%esp
-   1800035e1:	xor    $0x14010000,%eax
-   1800035e6:	add    $0x12011400,%eax
-   1800035eb:	add    %cl,0xa500bf0(%rip)        # 0x18a5041e1
-   1800035f1:	xor    %al,(%rax)
-   1800035f3:	add    %ah,(%rcx)
-   1800035f5:	add    $0xc4050002,%eax
-   1800035fa:	lldt   -0x5bffffeb(%rax)
-   180003601:	adc    $0x35e40000,%eax
-   180003606:	add    %al,(%rax)
-   180003608:	and    %eax,(%rax)
-   18000360a:	add    %al,(%rax)
-   18000360c:	nop
-   18000360d:	adc    $0x15a40000,%eax
-   180003612:	add    %al,(%rax)
-   180003614:	in     $0x35,%al
-   180003616:	add    %al,(%rax)
-   180003618:	and    %esp,-0x1bdafffa(%rip)        # 0x164253624
-   18000361e:	or     $0x10741700,%eax
-   180003623:	add    %cl,(%rax)
-   180003625:	adc    %eax,%fs:(%rax)
-   180003628:	and    %bl,(%rcx)
-   18000362a:	add    %al,(%rax)
-   18000362c:	sbb    %eax,%fs:(%rax)
-   18000362f:	add    %bl,0x36(%rax)
-   180003632:	add    %al,(%rax)
-   180003634:	and    %eax,-0x2bfafffe(%rip)        # 0x15405363c
-   18000363a:	(bad)
-   18000363b:	add    %cl,0x13000016(%rsi)
-   180003641:	(bad)
+   1800035cb:	add    %al,%dl
+   1800035cd:	adc    %al,(%rax)
+   1800035cf:	add    %ah,0x21000035(%rax)
+   1800035d5:	add    %al,(%rax)
+   1800035d7:	add    %al,(%rax)
+   1800035d9:	adc    %al,(%rax)
+   1800035db:	add    %al,%dl
+   1800035dd:	adc    %al,(%rax)
+   1800035df:	add    %ah,0x1000035(%rax)
+   1800035e5:	jg     0x1800035ee
+   1800035e7:	add    %bh,0x54(%rdi)
+   1800035ea:	or     (%rax),%eax
+   1800035ec:	jp     0x180003622
+   1800035ee:	or     $0x0,%al
+   1800035f0:	sbb    %edx,%eax
+   1800035f2:	(bad)
+   1800035f3:	rclb   0x210000c0(%rip)        # 0x1a10036b9
+   1800035f9:	and    $0x8,%al
+   1800035fb:	add    %ah,(%rsp,%rsi,8)
+   1800035fe:	(bad)
+   1800035ff:	add    %bl,(%rax)
+   180003601:	in     $0x8,%al
+   180003603:	add    %cl,(%rsp,%rsi,2)
+   180003606:	or     %eax,(%rax)
+   180003608:	add    $0x50000a64,%eax
+   18000360d:	adc    (%rax),%al
+   18000360f:	add    %dl,%cl
+   180003611:	adc    (%rax),%al
+   180003613:	add    %ah,%ah
+   180003615:	xor    $0x210000,%eax
+   18000361a:	add    %al,(%rax)
+   18000361c:	push   %rax
+   18000361d:	adc    (%rax),%al
+   18000361f:	add    %dl,%cl
+   180003621:	adc    (%rax),%al
+   180003623:	add    %ah,%ah
+   180003625:	xor    $0x1d010000,%eax
+   18000362a:	add    $0x12011d00,%eax
+   18000362f:	add    %dl,(%rsi)
+   180003631:	loopne 0x180003647
+   180003633:	(bad)
+   180003634:	adc    0x0(%rax),%edx
+   180003637:	add    %ah,(%rcx)
+   180003639:	add    $0x2,%al
+   18000363b:	add    %al,(%rsp,%rsi,2)
+   18000363e:	adc    %al,(%rax)
+   180003640:	mov    $0x15,%al
    180003642:	add    %al,(%rax)
-   180003644:	sbb    %dh,(%rsi)
+   180003644:	int    $0x15
    180003646:	add    %al,(%rax)
-   180003648:	and    %eax,(%rax)
+   180003648:	sub    %dh,(%rsi)
    18000364a:	add    %al,(%rax)
-   18000364c:	mov    (%rsi),%ss
-   18000364e:	add    %al,(%rax)
-   180003650:	adc    (%rdi),%edx
-   180003652:	add    %al,(%rax)
-   180003654:	sbb    %dh,(%rsi)
-   180003656:	add    %al,(%rax)
-   180003658:	and    %eax,(%rax)
-   18000365a:	add    (%rax),%al
-   18000365c:	add    %al,%ah
-   18000365e:	lldt   -0x5bffffeb(%rax)
-   180003665:	adc    $0x35e40000,%eax
-   18000366a:	add    %al,(%rax)
-   18000366c:	add    %esi,0x5(%rbx)
-   18000366f:	add    %dh,0x54(%rbx)
-   180003672:	or     $0x0,%al
-   180003674:	adc    %al,%dl
-   180003676:	or     $0xf0,%al
-   180003678:	or     (%rax),%dh
+   18000364c:	and    %edx,0x34960006(%rsi)
+   180003652:	adc    %eax,(%rax)
+   180003654:	(bad)
+   180003655:	hlt
+   180003656:	or     $0xfc40400,%eax
+   18000365b:	add    %cl,%ch
+   18000365d:	adc    $0x15d40000,%eax
+   180003662:	add    %al,(%rax)
+   180003664:	cmp    %dh,(%rsi)
+   180003666:	add    %al,(%rax)
+   180003668:	and    %eax,(%rax)
+   18000366a:	add    $0x0,%al
+   18000366c:	add    %dh,%ah
+   18000366e:	or     $0x11340000,%eax
+   180003673:	add    %cl,%ch
+   180003675:	adc    $0x15d40000,%eax
    18000367a:	add    %al,(%rax)
-   18000367c:	and    %esp,(%rax,%rcx,1)
-   18000367f:	add    %ah,(%rsp,%riz,8)
-   180003682:	(bad)
-   180003683:	add    %bl,(%rax)
-   180003685:	(bad)
-   180003686:	or     %al,(%rax)
-   180003688:	or     $0x74,%al
-   18000368a:	or     (%rax),%al
-   18000368c:	add    $0x40000b64,%eax
-   180003691:	adc    (%rax),%al
-   180003693:	add    %dh,0x6c000012(%rbp)
-   180003699:	ss add %al,(%rax)
-   18000369c:	and    %eax,-0x3bfafffe(%rip)        # 0x1440536a4
-   1800036a2:	or     %eax,(%rax)
-   1800036a4:	mov    $0x12,%ch
-   1800036a6:	add    %al,(%rax)
-   1800036a8:	xor    (%rbx),%edx
-   1800036aa:	add    %al,(%rax)
-   1800036ac:	jl     0x1800036e4
-   1800036ae:	add    %al,(%rax)
-   1800036b0:	and    %eax,(%rax)
+   18000367c:	cmp    %dh,(%rsi)
+   18000367e:	add    %al,(%rax)
+   180003680:	and    %eax,(%rax)
+   180003682:	add    (%rax),%al
+   180003684:	add    %dh,(%rcx,%rdx,1)
+   180003687:	add    %dh,-0x32ffffeb(%rax)
+   18000368d:	adc    $0x36280000,%eax
+   180003692:	add    %al,(%rax)
+   180003694:	and    %eax,(%rax)
+   180003696:	or     %al,(%rax)
+   180003698:	add    %dh,%ah
+   18000369a:	or     $0xfc40000,%eax
+   18000369f:	add    %al,(%rax)
+   1800036a1:	je     0x1800036b3
+   1800036a3:	add    %al,(%rax)
+   1800036a5:	xor    $0x11,%al
+   1800036a7:	add    %dh,-0x32ffffeb(%rax)
+   1800036ad:	adc    $0x36280000,%eax
    1800036b2:	add    %al,(%rax)
-   1800036b4:	mov    $0x12,%ch
-   1800036b6:	add    %al,(%rax)
-   1800036b8:	xor    (%rbx),%edx
-   1800036ba:	add    %al,(%rax)
-   1800036bc:	jl     0x1800036f4
+   1800036b4:	and    %eax,-0x2bfafffe(%rip)        # 0x1540536bc
+   1800036ba:	(bad)
+   1800036bb:	add    %bh,%bh
+   1800036bd:	(bad)
    1800036be:	add    %al,(%rax)
-   1800036c0:	and    %eax,(%rax)
+   1800036c0:	outsb  %ds:(%rsi),(%dx)
+   1800036c1:	(bad)
    1800036c2:	add    %al,(%rax)
-   1800036c4:	rex adc (%rax),%al
-   1800036c7:	add    %dh,0x6c000012(%rbp)
-   1800036cd:	ss add %al,(%rax)
-   1800036d0:	adc    %edx,0x74150008(%rip)        # 0x1f41536de
-   1800036d6:	or     %eax,(%rax)
-   1800036d8:	adc    $0x15000764,%eax
-   1800036dd:	xor    $0x6,%al
-   1800036df:	add    %dl,-0x591feece(%rip)        # 0x126e04817
-   1800036e5:	and    $0x0,%al
-   1800036e7:	add    %al,(%rdx)
-   1800036e9:	add    %al,(%rax)
-   1800036eb:	add    %ch,%ah
-   1800036ed:	sbb    %eax,(%rax)
-   1800036ef:	add    %bl,0x1a(%rbx)
+   1800036c4:	xchg   %eax,%esp
+   1800036c5:	ss add %al,(%rax)
+   1800036c8:	and    %eax,(%rax)
+   1800036ca:	add    %al,(%rax)
+   1800036cc:	call   *(%rsi)
+   1800036ce:	add    %al,(%rax)
+   1800036d0:	outsb  %ds:(%rsi),(%dx)
+   1800036d1:	(bad)
+   1800036d2:	add    %al,(%rax)
+   1800036d4:	xchg   %eax,%esp
+   1800036d5:	ss add %al,(%rax)
+   1800036d8:	adc    %edx,0x74150008(%rip)        # 0x1f41536e6
+   1800036de:	or     %eax,(%rax)
+   1800036e0:	adc    $0x15000764,%eax
+   1800036e5:	xor    $0x6,%al
+   1800036e7:	add    %dl,0x6e01132(%rip)        # 0x186e0481f
+   1800036ed:	and    $0x20000,%eax
    1800036f2:	add    %al,(%rax)
-   1800036f4:	ss and $0x0,%eax
-   1800036fa:	add    %al,(%rax)
-   1800036fc:	mov    $0xc900001a,%esi
-   180003701:	sbb    (%rax),%al
-   180003703:	add    %dh,(%rsi)
-   180003705:	and    $0x0,%eax
-   18000370a:	add    %al,(%rax)
-   18000370c:	add    %eax,(%rsi)
-   18000370e:	add    (%rax),%al
-   180003710:	(bad)
-   180003711:	xor    (%rdx),%al
-   180003713:	push   %rax
-   180003714:	adc    %ecx,(%rdx)
-   180003716:	add    $0x0,%al
-   180003718:	or     (%rax,%rcx,1),%dh
-   18000371b:	add    %cl,(%rdx)
-   18000371d:	push   %rdx
-   18000371e:	(bad)
-   18000371f:	jo     0x1800036c7
-   180003721:	and    $0x0,%al
-   180003723:	add    %al,(%rax,%rax,1)
-   180003726:	add    %al,(%rax)
-   180003728:	add    (%rbx),%ebx
-   18000372a:	add    %al,(%rax)
-   18000372c:	and    (%rbx),%bl
+   1800036f4:	sbb    (%rax),%r8b
+   1800036f7:	add    %dh,-0x69ffffe6(%rbx)
+   1800036fd:	and    $0x0,%eax
+   180003702:	add    %al,(%rax)
+   180003704:	(bad)
+   180003705:	sbb    (%rax),%eax
+   180003707:	add    %ah,(%rcx)
+   180003709:	sbb    (%rax),%eax
+   18000370b:	add    %dl,0x25(%rsi)
+   180003711:	add    %al,(%rax)
+   180003713:	add    %al,(%rcx)
+   180003715:	(bad)
+   180003716:	add    (%rax),%al
+   180003718:	(bad)
+   180003719:	xor    (%rdx),%al
+   18000371b:	push   %rax
+   18000371c:	adc    %ecx,(%rdx)
+   18000371e:	add    $0x0,%al
+   180003720:	or     (%rax,%rcx,1),%dh
+   180003723:	add    %cl,(%rdx)
+   180003725:	push   %rdx
+   180003726:	(bad)
+   180003727:	jo     0x18000372f
+   180003729:	and    $0x40000,%eax
    18000372e:	add    %al,(%rax)
-   180003730:	rex.WRB and $0x0,%rax
+   180003730:	pop    %rbx
+   180003731:	sbb    (%rax),%eax
+   180003733:	add    %bh,0x1b(%rdx)
    180003736:	add    %al,(%rax)
-   180003738:	clc
-   180003739:	sbb    (%rax),%al
-   18000373b:	add    %bh,(%rdx)
-   18000373d:	sbb    (%rax),%eax
-   18000373f:	add    %ah,0x25(%rsi)
-   180003742:	add    %al,(%rax)
-   180003744:	add    %al,(%rax)
-   180003746:	add    %al,(%rax)
-   180003748:	rex.XB sbb (%r8),%eax
-   18000374b:	add    %cl,0x1b(%rsi)
+   180003738:	lods   %ds:(%rsi),%eax
+   180003739:	and    $0x0,%eax
+   18000373e:	add    %al,(%rax)
+   180003740:	push   %rax
+   180003741:	sbb    (%rax),%eax
+   180003743:	add    %dl,-0x39ffffe5(%rdx)
+   180003749:	and    $0x0,%eax
    18000374e:	add    %al,(%rax)
-   180003750:	rex.WRB and $0x0,%rax
-   180003756:	add    %al,(%rax)
-   180003758:	rex.XB sbb (%r8),%eax
-   18000375b:	add    %cl,0x1b(%rdi)
+   180003750:	fwait
+   180003751:	sbb    (%rax),%eax
+   180003753:	add    %ah,-0x52ffffe5(%rsi)
+   180003759:	and    $0x0,%eax
    18000375e:	add    %al,(%rax)
-   180003760:	and    $0x0,%ax
-   180003764:	add    %al,(%rax)
-   180003766:	add    %al,(%rax)
-   180003768:	add    %eax,(%rcx,%rax,1)
-   18000376b:	add    %al,(%rdx,%rax,2)
+   180003760:	fwait
+   180003761:	sbb    (%rax),%eax
+   180003763:	add    %ah,-0x39ffffe5(%rdi)
+   180003769:	and    $0x0,%eax
    18000376e:	add    %al,(%rax)
-   180003770:	or     %ebx,(%rdx)
-   180003772:	(bad)
-   180003773:	add    %bl,(%rdx)
-   180003775:	xor    $0xf,%al
-   180003777:	add    %bl,(%rdx)
-   180003779:	jb     0x180003791
-   18000377b:	loopne 0x180003791
-   18000377d:	jo     0x180003792
-   18000377f:	(bad)
-   180003780:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180003781:	and    $0x0,%al
-   180003783:	add    %al,(%rcx)
-   180003785:	add    %al,(%rax)
-   180003787:	add    %al,0x6b00001b(%rbp)
-   18000378d:	sbb    $0x0,%al
-   18000378f:	add    %bh,0x25(%rdx)
+   180003770:	add    %eax,(%rcx,%rax,1)
+   180003773:	add    %al,(%rdx,%rax,2)
+   180003776:	add    %al,(%rax)
+   180003778:	or     %ebx,(%rdx)
+   18000377a:	(bad)
+   18000377b:	add    %bl,(%rdx)
+   18000377d:	xor    $0xf,%al
+   18000377f:	add    %bl,(%rdx)
+   180003781:	jb     0x180003799
+   180003783:	loopne 0x180003799
+   180003785:	jo     0x18000379a
+   180003787:	(bad)
+   180003788:	(bad)
+   180003789:	and    $0x10000,%eax
+   18000378e:	add    %al,(%rax)
+   180003790:	fstpl  (%rbx)
    180003792:	add    %al,(%rax)
-   180003794:	imul   $0x0,(%rax,%rax,1),%ebx
-   180003798:	add    %eax,(%rsi)
-   18000379a:	add    (%rax),%al
-   18000379c:	(bad)
-   18000379d:	push   %rdx
-   18000379e:	add    0x1(%rax),%dl
-   1800037a1:	clts
-   1800037a3:	add    %cl,(%rdi)
-   1800037a5:	fs (bad)
-   1800037a7:	add    %cl,(%rdi)
-   1800037a9:	xor    $0x6,%al
+   180003794:	ret
+   180003795:	sbb    $0x0,%al
+   180003797:	add    %bl,%dl
+   180003799:	and    $0x1cc30000,%eax
+   18000379e:	add    %al,(%rax)
+   1800037a0:	add    %eax,(%rsi)
+   1800037a2:	add    (%rax),%al
+   1800037a4:	(bad)
+   1800037a5:	push   %rdx
+   1800037a6:	add    0x1(%rax),%dl
+   1800037a9:	clts
    1800037ab:	add    %cl,(%rdi)
-   1800037ad:	xor    (%rbx),%cl
-   1800037af:	jo     0x1800037b2
-   1800037b1:	or     $0x340d0004,%eax
-   1800037b6:	or     %eax,(%rax)
-   1800037b8:	or     $0x9500632,%eax
-   1800037bd:	add    $0x1,%al
-   1800037bf:	add    %al,(%rdx,%riz,1)
-   1800037c2:	add    %al,(%rax)
-   1800037c4:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   1800037c5:	and    $0x0,%al
-   1800037c7:	add    %al,(%rcx)
-   1800037c9:	add    %al,(%rax)
-   1800037cb:	add    %ah,(%rdi)
-   1800037cd:	and    %al,(%rax)
-   1800037cf:	add    %dh,-0x4fffffe0(%rcx)
-   1800037d5:	and    $0x20b10000,%eax
+   1800037ad:	fs (bad)
+   1800037af:	add    %cl,(%rdi)
+   1800037b1:	xor    $0x6,%al
+   1800037b3:	add    %cl,(%rdi)
+   1800037b5:	xor    (%rbx),%cl
+   1800037b7:	jo     0x1800037ba
+   1800037b9:	or     $0x340d0004,%eax
+   1800037be:	or     %eax,(%rax)
+   1800037c0:	or     $0x9500632,%eax
+   1800037c5:	add    $0x1,%al
+   1800037c7:	add    %al,(%rdx,%riz,1)
+   1800037ca:	add    %al,(%rax)
+   1800037cc:	(bad)
+   1800037cd:	and    $0x10000,%eax
+   1800037d2:	add    %al,(%rax)
+   1800037d4:	jg     0x1800037f6
+   1800037d6:	add    %al,(%rax)
+   1800037d8:	or     %esp,(%rcx)
    1800037da:	add    %al,(%rax)
-   1800037dc:	add    %eax,(%rdx)
-   1800037de:	add    %eax,(%rax)
-   1800037e0:	add    0x0(%rax),%dl
-   1800037e3:	add    %al,(%rcx)
-   1800037e5:	(bad)
-   1800037e6:	add    (%rax),%al
-   1800037e8:	(bad)
-   1800037e9:	xor    (%rdx),%al
-   1800037eb:	xor    %al,(%rcx)
-   1800037ed:	adc    $0x8,%al
-   1800037ef:	add    %dl,(%rsp,%riz,2)
-   1800037f2:	or     %al,(%rax)
-   1800037f4:	adc    $0x54,%al
-   1800037f6:	(bad)
-   1800037f7:	add    %dl,(%rsp,%rsi,1)
-   1800037fa:	(bad)
-   1800037fb:	add    %dl,(%rdx,%rsi,1)
-   1800037fe:	adc    %dh,0x1(%rax)
-   180003801:	adc    $0x34150005,%eax
-   180003806:	mov    $0xb8011500,%edx
-   18000380b:	add    %al,(%rsi)
-   18000380d:	push   %rax
-   18000380e:	add    %al,(%rax)
-   180003810:	add    %ecx,(%rdx)
-   180003812:	add    $0x0,%al
-   180003814:	or     (%rsi,%rax,1),%dh
-   180003817:	add    %cl,(%rdx)
-   180003819:	xor    (%rsi),%al
-   18000381b:	jo     0x18000381e
-   18000381d:	clts
-   18000381f:	add    %cl,(%rdi)
-   180003821:	fs (bad)
-   180003823:	add    %cl,(%rdi)
-   180003825:	xor    $0x5,%al
+   1800037dc:	adc    %ah,(%rsi)
+   1800037de:	add    %al,(%rax)
+   1800037e0:	or     %esp,(%rcx)
+   1800037e2:	add    %al,(%rax)
+   1800037e4:	add    %eax,(%rdx)
+   1800037e6:	add    %eax,(%rax)
+   1800037e8:	add    0x0(%rax),%dl
+   1800037eb:	add    %al,(%rcx)
+   1800037ed:	(bad)
+   1800037ee:	add    (%rax),%al
+   1800037f0:	(bad)
+   1800037f1:	xor    (%rdx),%al
+   1800037f3:	xor    %al,(%rcx)
+   1800037f5:	adc    $0x8,%al
+   1800037f7:	add    %dl,(%rsp,%riz,2)
+   1800037fa:	or     %al,(%rax)
+   1800037fc:	adc    $0x54,%al
+   1800037fe:	(bad)
+   1800037ff:	add    %dl,(%rsp,%rsi,1)
+   180003802:	(bad)
+   180003803:	add    %dl,(%rdx,%rsi,1)
+   180003806:	adc    %dh,0x1(%rax)
+   180003809:	adc    $0x34150005,%eax
+   18000380e:	mov    $0xb8011500,%edx
+   180003813:	add    %al,(%rsi)
+   180003815:	push   %rax
+   180003816:	add    %al,(%rax)
+   180003818:	add    %ecx,(%rdx)
+   18000381a:	add    $0x0,%al
+   18000381c:	or     (%rsi,%rax,1),%dh
+   18000381f:	add    %cl,(%rdx)
+   180003821:	xor    (%rsi),%al
+   180003823:	jo     0x180003826
+   180003825:	clts
    180003827:	add    %cl,(%rdi)
-   180003829:	adc    (%rbx),%cl
-   18000382b:	jo     0x18000382d
-   18000382d:	add    %al,(%rax)
-   18000382f:	add    %al,(%rcx)
-   180003831:	add    %al,(%rax)
-   180003833:	add    %al,(%rax)
+   180003829:	fs (bad)
+   18000382b:	add    %cl,(%rdi)
+   18000382d:	xor    $0x5,%al
+   18000382f:	add    %cl,(%rdi)
+   180003831:	adc    (%rbx),%cl
+   180003833:	jo     0x180003835
    180003835:	add    %al,(%rax)
    180003837:	add    %al,(%rcx)
+   180003839:	add    %al,(%rax)
+   18000383b:	add    %al,(%rax)
+   18000383d:	add    %al,(%rax)
+   18000383f:	add    %al,(%rcx)
 	...
-   180003841:	add    %al,(%rax)
-   180003843:	add    %bh,%bh
-   180003845:	(bad)
-   180003846:	(bad)
-   180003847:	incl   (%rax)
-   180003849:	add    %al,(%rax)
-   18000384b:	add    %al,0x1000038(%rsi)
    180003851:	add    %al,(%rax)
-   180003853:	add    %al,(%rbx)
-   180003855:	add    %al,(%rax)
-   180003857:	add    %al,(%rbx)
+   180003853:	add    %bh,%bh
+   180003855:	(bad)
+   180003856:	(bad)
+   180003857:	incl   (%rax)
    180003859:	add    %al,(%rax)
-   18000385b:	add    %ch,0x38(%rax)
-   18000385e:	add    %al,(%rax)
-   180003860:	je     0x18000389a
-   180003862:	add    %al,(%rax)
-   180003864:	cmpb   $0x0,(%rax)
-   180003867:	add    %al,(%rax)
-   180003869:	adc    %al,(%rax)
-   18000386b:	add    %al,0x12(%rax)
+   18000385b:	add    %dl,0x1000038(%rsi)
+   180003861:	add    %al,(%rax)
+   180003863:	add    %al,(%rbx)
+   180003865:	add    %al,(%rax)
+   180003867:	add    %al,(%rbx)
+   180003869:	add    %al,(%rax)
+   18000386b:	add    %bh,0x38(%rax)
    18000386e:	add    %al,(%rax)
-   180003870:	nop
-   180003871:	adc    $0x388e0000,%eax
-   180003876:	add    %al,(%rax)
-   180003878:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   180003879:	cmp    %al,(%rax)
-   18000387b:	add    %al,%cl
-   18000387d:	cmp    %al,(%rax)
-   18000387f:	add    %al,(%rax)
-   180003881:	add    %al,(%rcx)
-   180003883:	add    %al,(%rdx)
-   180003885:	add    %ch,0x70(%rsi)
-   180003888:	outsb  %ds:(%rsi),(%dx)
-   180003889:	cs fs insb (%dx),%es:(%rdi)
-   18000388c:	insb   (%dx),%es:(%rdi)
-   18000388d:	add    %al,0x65(%rdi)
-   180003890:	outsb  %ds:(%rsi),(%dx)
-   180003891:	gs jb  0x1800038f5
-   180003894:	je     0x1800038fb
-   180003896:	push   %rax
-   180003897:	gs jb  0x180003907
-   18000389a:	jne    0x180003910
-   18000389c:	(bad)
-   18000389d:	je     0x180003908
-   18000389f:	outsl  %ds:(%rsi),(%dx)
+   180003870:	test   %bh,(%rax)
+   180003872:	add    %al,(%rax)
+   180003874:	nop
+   180003875:	cmp    %al,(%rax)
+   180003877:	add    %al,(%rax)
+   180003879:	adc    %al,(%rax)
+   18000387b:	add    %dl,0x12(%rax)
+   18000387e:	add    %al,(%rax)
+   180003880:	mov    $0x15,%al
+   180003882:	add    %al,(%rax)
+   180003884:	sahf
+   180003885:	cmp    %al,(%rax)
+   180003887:	add    %dh,-0x2effffc8(%rdi)
+   18000388d:	cmp    %al,(%rax)
+   18000388f:	add    %al,(%rax)
+   180003891:	add    %al,(%rcx)
+   180003893:	add    %al,(%rdx)
+   180003895:	add    %ch,0x70(%rsi)
+   180003898:	outsb  %ds:(%rsi),(%dx)
+   180003899:	cs fs insb (%dx),%es:(%rdi)
+   18000389c:	insb   (%dx),%es:(%rdi)
+   18000389d:	add    %al,0x65(%rdi)
    1800038a0:	outsb  %ds:(%rsi),(%dx)
-   1800038a1:	push   %rsp
-   1800038a2:	(bad)
-   1800038a3:	(bad)
-   1800038a4:	insb   (%dx),%es:(%rdi)
-   1800038a5:	add    %cl,%gs:0x70(%rsi)
-   1800038a9:	rex.XB (bad)
-   1800038ab:	outsb  %ds:(%rsi),(%dx)
-   1800038ac:	outsl  %ds:(%rsi),(%dx)
-   1800038ad:	outsb  %ds:(%rsi),(%dx)
-   1800038ae:	imul   $0x7065526c,0x61(%rbx),%esp
-   1800038b5:	jb     0x18000391c
-   1800038b7:	jae    0x18000391e
-   1800038b9:	outsb  %ds:(%rsi),(%dx)
-   1800038ba:	je     0x18000391d
-   1800038bc:	je     0x180003927
-   1800038be:	jbe    0x180003925
-   1800038c0:	add    %cl,0x70(%rsi)
-   1800038c3:	outsb  %ds:(%rsi),(%dx)
-   1800038c4:	rex.XB (bad)
-   1800038c6:	outsb  %ds:(%rsi),(%dx)
-   1800038c7:	outsl  %ds:(%rsi),(%dx)
-   1800038c8:	outsb  %ds:(%rsi),(%dx)
-   1800038c9:	imul   $0x7065526c,0x61(%rbx),%esp
-   1800038d0:	jb     0x180003937
-   1800038d2:	jae    0x180003939
-   1800038d4:	outsb  %ds:(%rsi),(%dx)
-   1800038d5:	je     0x180003938
-   1800038d7:	je     0x180003942
-   1800038d9:	jbe    0x180003940
-   1800038db:	add    %ah,0x39(%rax)
-   1800038e1:	add    %al,(%rax)
-   1800038e3:	add    %al,(%rax)
-   1800038e5:	add    %al,(%rax)
-   1800038e7:	add    %dl,0x3a(%rdx)
-   1800038ea:	add    %al,(%rax)
-   1800038ec:	jo     0x18000391e
-   1800038ee:	add    %al,(%rax)
-   1800038f0:	enter  $0x39,$0x0
-	...
-   1800038fc:	or     (%rbx),%bh
+   1800038a1:	gs jb  0x180003905
+   1800038a4:	je     0x18000390b
+   1800038a6:	push   %rax
+   1800038a7:	gs jb  0x180003917
+   1800038aa:	jne    0x180003920
+   1800038ac:	(bad)
+   1800038ad:	je     0x180003918
+   1800038af:	outsl  %ds:(%rsi),(%dx)
+   1800038b0:	outsb  %ds:(%rsi),(%dx)
+   1800038b1:	push   %rsp
+   1800038b2:	(bad)
+   1800038b3:	(bad)
+   1800038b4:	insb   (%dx),%es:(%rdi)
+   1800038b5:	add    %cl,%gs:0x70(%rsi)
+   1800038b9:	rex.XB (bad)
+   1800038bb:	outsb  %ds:(%rsi),(%dx)
+   1800038bc:	outsl  %ds:(%rsi),(%dx)
+   1800038bd:	outsb  %ds:(%rsi),(%dx)
+   1800038be:	imul   $0x7065526c,0x61(%rbx),%esp
+   1800038c5:	jb     0x18000392c
+   1800038c7:	jae    0x18000392e
+   1800038c9:	outsb  %ds:(%rsi),(%dx)
+   1800038ca:	je     0x18000392d
+   1800038cc:	je     0x180003937
+   1800038ce:	jbe    0x180003935
+   1800038d0:	add    %cl,0x70(%rsi)
+   1800038d3:	outsb  %ds:(%rsi),(%dx)
+   1800038d4:	rex.XB (bad)
+   1800038d6:	outsb  %ds:(%rsi),(%dx)
+   1800038d7:	outsl  %ds:(%rsi),(%dx)
+   1800038d8:	outsb  %ds:(%rsi),(%dx)
+   1800038d9:	imul   $0x7065526c,0x61(%rbx),%esp
+   1800038e0:	jb     0x180003947
+   1800038e2:	jae    0x180003949
+   1800038e4:	outsb  %ds:(%rsi),(%dx)
+   1800038e5:	je     0x180003948
+   1800038e7:	je     0x180003952
+   1800038e9:	jbe    0x180003950
+   1800038eb:	add    %dh,0x39(%rax)
+   1800038f1:	add    %al,(%rax)
+   1800038f3:	add    %al,(%rax)
+   1800038f5:	add    %al,(%rax)
+   1800038f7:	add    %ah,0x3a(%rdx)
+   1800038fa:	add    %al,(%rax)
+   1800038fc:	jo     0x18000392e
    1800038fe:	add    %al,(%rax)
-   180003900:	cwtl
-   180003901:	xor    %al,(%rax)
-   180003903:	add    %dh,(%rax)
-   180003905:	cmp    %eax,(%rax)
-	...
-   18000390f:	add    %ch,0x3c(%rdx)
-   180003912:	add    %al,(%rax)
-   180003914:	add    %dh,(%rax)
-	...
-   18000392e:	add    %al,(%rax)
-   180003930:	add    %bh,(%rax,%rax,1)
-   180003933:	add    %al,(%rax)
-   180003935:	add    %al,(%rax)
-   180003937:	add    %al,0x3b(%rsi)
-   18000393a:	add    %al,(%rax)
-   18000393c:	add    %al,(%rax)
+   180003900:	fdivrs (%rcx)
+	...
+   18000390a:	add    %al,(%rax)
+   18000390c:	sbb    (%rbx),%bh
+   18000390e:	add    %al,(%rax)
+   180003910:	cwtl
+   180003911:	xor    %al,(%rax)
+   180003913:	add    %al,0x39(%rax)
+	...
+   18000391e:	add    %al,(%rax)
+   180003920:	jp     0x18000395e
+   180003922:	add    %al,(%rax)
+   180003924:	add    %dh,(%rax)
+	...
    18000393e:	add    %al,(%rax)
-   180003940:	sub    $0x3b,%al
-   180003942:	add    %al,(%rax)
-   180003944:	add    %al,(%rax)
-   180003946:	add    %al,(%rax)
-   180003948:	jb     0x180003985
+   180003940:	adc    %bh,(%rax,%rax,1)
+   180003943:	add    %al,(%rax)
+   180003945:	add    %al,(%rax)
+   180003947:	add    %dl,0x3b(%rsi)
    18000394a:	add    %al,(%rax)
    18000394c:	add    %al,(%rax)
    18000394e:	add    %al,(%rax)
-   180003950:	mov    %?,(%rbx)
+   180003950:	cmp    $0x3b,%al
    180003952:	add    %al,(%rax)
    180003954:	add    %al,(%rax)
    180003956:	add    %al,(%rax)
-   180003958:	test   $0x3b,%al
-   18000395a:	add    %al,(%rax)
-   18000395c:	add    %al,(%rax)
-   18000395e:	add    %al,(%rax)
-   180003960:	rex.WRX cmp $0x0,%al
-   180003963:	add    %al,(%rax)
-   180003965:	add    %al,(%rax)
-   180003967:	add    %dh,(%rax)
-   180003969:	cmp    $0x0,%al
-   18000396b:	add    %al,(%rax)
+   180003958:	(bad)
+   180003959:	cmp    (%rax),%eax
+   18000395b:	add    %al,(%rax)
+   18000395d:	add    %al,(%rax)
+   18000395f:	add    %bl,0x0(%rbx,%rdi,1)
+   180003966:	add    %al,(%rax)
+   180003968:	mov    $0x3b,%eax
    18000396d:	add    %al,(%rax)
-   18000396f:	add    %dl,(%rsp,%rdi,1)
+   18000396f:	add    %bl,0x3c(%rsi)
    180003972:	add    %al,(%rax)
    180003974:	add    %al,(%rax)
    180003976:	add    %al,(%rax)
-   180003978:	pop    %rsp
-   180003979:	cmp    (%rax),%eax
+   180003978:	rex cmp $0x0,%al
    18000397b:	add    %al,(%rax)
    18000397d:	add    %al,(%rax)
-   18000397f:	add    %ch,%ah
-   180003981:	cmp    (%rax),%eax
-   180003983:	add    %al,(%rax)
-   180003985:	add    %al,(%rax)
-   180003987:	add    %dl,%dl
+   18000397f:	add    %ah,(%rsp,%rdi,1)
+   180003982:	add    %al,(%rax)
+   180003984:	add    %al,(%rax)
+   180003986:	add    %al,(%rax)
+   180003988:	insb   (%dx),%es:(%rdi)
    180003989:	cmp    (%rax),%eax
    18000398b:	add    %al,(%rax)
    18000398d:	add    %al,(%rax)
-   18000398f:	add    %bh,0x3b(%rsi)
-	...
+   18000398f:	add    %bh,%ah
+   180003991:	cmp    (%rax),%eax
+   180003993:	add    %al,(%rax)
+   180003995:	add    %al,(%rax)
+   180003997:	add    %ah,%dl
+   180003999:	cmp    (%rax),%eax
+   18000399b:	add    %al,(%rax)
    18000399d:	add    %al,(%rax)
-   18000399f:	add    %bh,0x3c(%rax)
-   1800039a2:	add    %al,(%rax)
-   1800039a4:	add    %al,(%rax)
-   1800039a6:	add    %al,(%rax)
-   1800039a8:	xor    (%rdx),%bh
-   1800039aa:	add    %al,(%rax)
-   1800039ac:	add    %al,(%rax)
-   1800039ae:	add    %al,(%rax)
-   1800039b0:	sbb    (%rdx),%bh
-   1800039b2:	add    %al,(%rax)
-   1800039b4:	add    %al,(%rax)
-   1800039b6:	add    %al,(%rax)
-   1800039b8:	adc    %bh,(%rdx)
+   18000399f:	add    %cl,%dh
+   1800039a1:	cmp    (%rax),%eax
 	...
+   1800039af:	add    %cl,0x3c(%rax)
+   1800039b5:	add    %al,(%rax)
+   1800039b7:	add    %al,0x3a(%rdx)
+   1800039ba:	add    %al,(%rax)
+   1800039bc:	add    %al,(%rax)
+   1800039be:	add    %al,(%rax)
+   1800039c0:	sub    (%rdx),%bh
+   1800039c2:	add    %al,(%rax)
+   1800039c4:	add    %al,(%rax)
    1800039c6:	add    %al,(%rax)
-   1800039c8:	add    %bh,(%rbx)
-   1800039ca:	add    %al,(%rax)
-   1800039cc:	add    %al,(%rax)
-   1800039ce:	add    %al,(%rax)
-   1800039d0:	call   0x180003a0f
-   1800039d5:	add    %al,(%rax)
-   1800039d7:	add    %cl,%ah
-   1800039d9:	cmp    (%rax),%al
-   1800039db:	add    %al,(%rax)
-   1800039dd:	add    %al,(%rax)
-   1800039df:	add    %ch,0x3a(%rdx)
+   1800039c8:	and    %bh,(%rdx)
+	...
+   1800039d6:	add    %al,(%rax)
+   1800039d8:	adc    %bh,(%rbx)
+   1800039da:	add    %al,(%rax)
+   1800039dc:	add    %al,(%rax)
+   1800039de:	add    %al,(%rax)
+   1800039e0:	clc
+   1800039e1:	cmp    (%rax),%al
+   1800039e3:	add    %al,(%rax)
    1800039e5:	add    %al,(%rax)
-   1800039e7:	add    %dl,0x3a(%rax)
+   1800039e7:	add    %bl,%ah
+   1800039e9:	cmp    (%rax),%al
+   1800039eb:	add    %al,(%rax)
    1800039ed:	add    %al,(%rax)
-   1800039ef:	add    %bh,0x3a(%rsi)
-   1800039f2:	add    %al,(%rax)
-   1800039f4:	add    %al,(%rax)
-   1800039f6:	add    %al,(%rax)
-   1800039f8:	jo     0x180003a34
-   1800039fa:	add    %al,(%rax)
-   1800039fc:	add    %al,(%rax)
-   1800039fe:	add    %al,(%rax)
-   180003a00:	cmp    %fs:(%rax),%al
-	...
-   180003a0f:	add    %bh,(%rsi)
-   180003a11:	add    %ch,0x65(%rbp)
-   180003a14:	insl   (%dx),%es:(%rdi)
-   180003a15:	jae    0x180003a7c
-   180003a17:	je     0x180003a19
-   180003a19:	add    %cl,(%rax)
-   180003a1b:	add    %bl,0x5f(%rdi)
-   180003a1e:	rex.XB pop %r15
-   180003a20:	jae    0x180003a92
-   180003a22:	movsxd %gs:0x66(%rcx),%ebp
-   180003a26:	imul   $0x646e6168,0x5f(%rbx),%esp
-   180003a2d:	insb   (%dx),%es:(%rdi)
-   180003a2e:	gs jb  0x180003a31
-   180003a31:	add    %ah,0x735f5f00(%rip)        # 0x1f35f9937
-   180003a37:	je     0x180003a9d
-   180003a39:	pop    %rdi
-   180003a3a:	je     0x180003ab5
-   180003a3c:	jo     0x180003aa3
-   180003a3e:	pop    %rdi
-   180003a3f:	imul   $0x65645f6f,0x66(%rsi),%ebp
-   180003a46:	jae    0x180003abc
-   180003a48:	jb     0x180003ab9
-   180003a4a:	jns    0x180003aab
-   180003a4c:	insb   (%dx),%es:(%rdi)
-   180003a4d:	imul   $0x43560000,0x74(%rbx),%esi
-   180003a54:	push   %rdx
-   180003a55:	push   %rbp
-   180003a56:	rex.WRX push %rsp
-   180003a58:	rex.WB
-   180003a59:	rex.WRB
-   180003a5a:	xor    %r14d,(%r8,%rsi,1)
-   180003a5e:	cs fs insb (%dx),%es:(%rdi)
-   180003a61:	insb   (%dx),%es:(%rdi)
-   180003a62:	add    %al,(%rax)
-   180003a64:	ss add %bl,0x69(%rdi)
-   180003a68:	outsb  %ds:(%rsi),(%dx)
-   180003a69:	imul   $0x37006d72,0x65(%rsp,%rsi,2),%esi
-   180003a71:	add    %bl,0x69(%rdi)
-   180003a74:	outsb  %ds:(%rsi),(%dx)
-   180003a75:	imul   $0x655f6d72,0x65(%rsp,%rsi,2),%esi
-   180003a7d:	add    %bh,(%rdi)
-   180003a7f:	add    %bl,0x73(%rdi)
-   180003a82:	gs push $0x6c69665f
-   180003a88:	je     0x180003aef
-   180003a8a:	jb     0x180003aeb
-   180003a8c:	fs insb (%dx),%es:(%rdi)
-   180003a8e:	insb   (%dx),%es:(%rdi)
-   180003a8f:	add    %bl,(%rax)
-   180003a91:	add    %bl,0x63(%rdi)
-   180003a94:	outsl  %ds:(%rsi),(%dx)
-   180003a95:	outsb  %ds:(%rsi),(%dx)
-   180003a96:	imul   $0x6572,0x75(%rdi),%sp
-   180003a9c:	pop    %rdi
-   180003a9d:	outsb  %ds:(%rsi),(%dx)
-   180003a9e:	(bad)
-   180003a9f:	jb     0x180003b13
-   180003aa1:	outsl  %ds:(%rsi),(%dx)
-   180003aa2:	ja     0x180003b03
-   180003aa4:	(bad)
-   180003aa5:	jb     0x180003b0e
-   180003aa7:	jbe    0x180003aa9
-   180003aa9:	add    %dh,(%rbx)
-   180003aab:	add    %bl,0x69(%rdi)
-   180003aae:	outsb  %ds:(%rsi),(%dx)
-   180003aaf:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   180003ab7:	pop    %rdi
-   180003ab8:	outsb  %ds:(%rsi),(%dx)
-   180003ab9:	(bad)
-   180003aba:	jb     0x180003b2e
-   180003abc:	outsl  %ds:(%rsi),(%dx)
-   180003abd:	ja     0x180003b1e
-   180003abf:	outsb  %gs:(%rsi),(%dx)
-   180003ac1:	jbe    0x180003b2c
-   180003ac3:	jb     0x180003b34
-   180003ac5:	outsb  %ds:(%rsi),(%dx)
-   180003ac6:	insl   (%dx),%es:(%rdi)
-   180003ac7:	outsb  %gs:(%rsi),(%dx)
-   180003ac9:	je     0x180003acb
-   180003acb:	add    %dh,(%rax,%rax,1)
-   180003ace:	pop    %rdi
-   180003acf:	imul   $0x6c616974,0x69(%rsi),%ebp
-   180003ad6:	imul   $0x656e6f5f,0x65(%rdx),%edi
-   180003add:	js     0x180003b48
-   180003adf:	je     0x180003b40
-   180003ae1:	je     0x180003b44
-   180003ae3:	(bad)
-   180003ae4:	insb   (%dx),%es:(%rdi)
-   180003ae5:	add    %al,%gs:(%rax)
-   180003ae8:	and    (%rax),%al
-   180003aea:	pop    %rdi
-   180003aeb:	gs js  0x180003b53
-   180003aee:	movsxd 0x74(%rbp),%esi
-   180003af1:	gs pop %rdi
-   180003af3:	outsl  %ds:(%rsi),(%dx)
-   180003af4:	outsb  %ds:(%rsi),(%dx)
-   180003af5:	gs js  0x180003b61
-   180003af8:	je     0x180003b59
-   180003afa:	je     0x180003b5d
-   180003afc:	(bad)
-   180003afd:	insb   (%dx),%es:(%rdi)
-   180003afe:	add    %dl,%gs:(%rsi)
-   180003b01:	add    %bl,0x63(%rdi)
-   180003b04:	gs js  0x180003b70
-   180003b07:	je     0x180003b09
-   180003b09:	add    %ah,0x70(%rcx)
-   180003b0c:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72dae83
-   180003b16:	jb     0x180003b8c
-   180003b18:	sub    $0x746e7572,%eax
-   180003b1d:	imul   $0x2d316c2d,0x65(%rbp),%ebp
-   180003b24:	xor    %ebp,0x6c642e30(%rip)        # 0x1ec64695a
-   180003b2a:	insb   (%dx),%es:(%rdi)
-   180003b2b:	add    %ah,0x51(%rsp,%rax,1)
-   180003b2f:	jne    0x180003b96
-   180003b31:	jb     0x180003bac
-   180003b33:	push   %rax
-   180003b34:	gs jb  0x180003b9d
-   180003b37:	outsl  %ds:(%rsi),(%dx)
-   180003b38:	jb     0x180003ba7
-   180003b3a:	(bad)
-   180003b3b:	outsb  %ds:(%rsi),(%dx)
-   180003b3c:	movsxd 0x43(%rbp),%esp
-   180003b3f:	outsl  %ds:(%rsi),(%dx)
-   180003b40:	jne    0x180003bb0
-   180003b42:	je     0x180003ba9
-   180003b44:	jb     0x180003b46
-   180003b46:	sub    (%rdx),%eax
-   180003b48:	rex.RXB
-   180003b49:	gs je  0x180003b8f
-   180003b4c:	jne    0x180003bc0
-   180003b4e:	jb     0x180003bb5
-   180003b50:	outsb  %ds:(%rsi),(%dx)
-   180003b51:	je     0x180003ba3
-   180003b53:	jb     0x180003bc4
-   180003b55:	movsxd 0x73(%rbp),%esp
-   180003b58:	jae    0x180003ba3
-   180003b5a:	add    %ch,%fs:(%rdi)
-   180003b5d:	add    0x65(%rdi),%al
-   180003b60:	je     0x180003ba5
-   180003b62:	jne    0x180003bd6
-   180003b64:	jb     0x180003bcb
-   180003b66:	outsb  %ds:(%rsi),(%dx)
-   180003b67:	je     0x180003bbd
-   180003b69:	push   $0x64616572
-   180003b6e:	rex.WB
-   180003b6f:	add    %al,%fs:(%rax)
-   180003b72:	add    %eax,(%rbx)
-   180003b74:	rex.RXB
-   180003b75:	gs je  0x180003bcb
-   180003b78:	jns    0x180003bed
-   180003b7a:	je     0x180003be1
-   180003b7c:	insl   (%dx),%es:(%rdi)
-   180003b7d:	push   %rsp
-   180003b7e:	imul   $0x69467341,0x65(%rbp),%ebp
-   180003b85:	insb   (%dx),%es:(%rdi)
-   180003b86:	gs push %rsp
-   180003b88:	imul   $0x44012c00,0x65(%rbp),%ebp
-   180003b8f:	imul   $0x54656c62,0x61(%rbx),%esi
-   180003b96:	push   $0x64616572
-   180003b9b:	imul   $0x43797261,0x72(%rdx),%r12
-   180003ba3:	(bad)
-   180003ba4:	insb   (%dx),%es:(%rdi)
-   180003ba5:	insb   (%dx),%es:(%rdi)
-   180003ba6:	jae    0x180003ba8
-   180003ba8:	addl   $0x74696e49,(%rbx)
-   180003bae:	imul   $0x53657a69,0x6c(%rcx),%esp
-   180003bb5:	imul   $0x64616548,0x74(%rbx),%r14
-   180003bbd:	add    %ch,%cl
-   180003bbf:	add    $0x52,%al
-   180003bc1:	je     0x180003c2f
-   180003bc3:	rex.XB (bad)
-   180003bc5:	jo     0x180003c3b
-   180003bc7:	jne    0x180003c3b
-   180003bc9:	rex.XB outsl %gs:(%rsi),(%dx)
-   180003bcc:	outsb  %ds:(%rsi),(%dx)
-   180003bcd:	je     0x180003c34
-   180003bcf:	js     0x180003c45
-   180003bd1:	add    %dh,%cl
-   180003bd3:	add    $0x52,%al
-   180003bd5:	je     0x180003c43
-   180003bd7:	rex.WR outsl %ds:(%rsi),(%dx)
-   180003bd9:	outsl  %ds:(%rsi),(%dx)
-   180003bda:	imul   $0x46,0x70(%rbp),%esi
-   180003bde:	jne    0x180003c4e
-   180003be0:	movsxd 0x6f(%rcx,%rbp,2),%esi
-   180003be4:	outsb  %ds:(%rsi),(%dx)
-   180003be5:	rex.RB outsb %ds:(%rsi),(%dx)
-   180003be7:	je     0x180003c5b
-   180003be9:	jns    0x180003beb
-   180003beb:	add    %bh,%al
-   180003bed:	add    $0x52,%al
-   180003bef:	je     0x180003c5d
-   180003bf1:	push   %rsi
-   180003bf2:	imul   $0x556c6175,0x74(%rdx),%esi
-   180003bf9:	outsb  %ds:(%rsi),(%dx)
-   180003bfa:	ja     0x180003c65
-   180003bfc:	outsb  %ds:(%rsi),(%dx)
-   180003bfd:	add    %al,%fs:(%rax)
-   180003c00:	xchg   %eax,%edi
-   180003c01:	add    0x73(%rcx),%ecx
-   180003c04:	rex.R
-   180003c05:	(bad)
-   180003c0b:	jb     0x180003c5d
-   180003c0d:	jb     0x180003c74
-   180003c0f:	jae    0x180003c76
-   180003c11:	outsb  %ds:(%rsi),(%dx)
-   180003c12:	je     0x180003c14
-   180003c14:	fadds  0x61686e55(%rip)        # 0x1e168aa6f
-   180003c1a:	outsb  %ds:(%rsi),(%dx)
-   180003c1b:	fs insb (%dx),%es:(%rdi)
-   180003c1d:	gs fs rex.RB js 0x180003c85
-   180003c22:	gs jo  0x180003c99
-   180003c25:	imul   $0x746c6946,0x6e(%rdi),%ebp
-   180003c2c:	gs jb  0x180003c2f
-   180003c2f:	add    %dl,0x74655305(%rdi)
-   180003c35:	push   %rbp
-   180003c36:	outsb  %ds:(%rsi),(%dx)
-   180003c37:	push   $0x6c646e61
-   180003c3c:	gs fs rex.RB js 0x180003ca4
-   180003c41:	gs jo  0x180003cb8
-   180003c44:	imul   $0x746c6946,0x6e(%rdi),%ebp
-   180003c4b:	gs jb  0x180003c4e
-   180003c4e:	sahf
-   180003c4f:	add    0x73(%rcx),%ecx
-   180003c52:	push   %rax
-   180003c53:	jb     0x180003cc4
-   180003c55:	movsxd 0x73(%rbp),%esp
-   180003c58:	jae    0x180003cc9
-   180003c5a:	jb     0x180003ca2
-   180003c5c:	gs (bad)
-   180003c5e:	je     0x180003cd5
-   180003c60:	jb     0x180003cc7
+   1800039ef:	add    %bh,0x3a(%rdx)
+   1800039f5:	add    %al,(%rax)
+   1800039f7:	add    %ah,0x3a(%rax)
+   1800039fd:	add    %al,(%rax)
+   1800039ff:	add    %cl,0x3a(%rsi)
+   180003a05:	add    %al,(%rax)
+   180003a07:	add    %al,0x3a(%rax)
+   180003a0d:	add    %al,(%rax)
+   180003a0f:	add    %dh,0x0(%rdx,%rdi,1)
+	...
+   180003a1f:	add    %bh,(%rsi)
+   180003a21:	add    %ch,0x65(%rbp)
+   180003a24:	insl   (%dx),%es:(%rdi)
+   180003a25:	jae    0x180003a8c
+   180003a27:	je     0x180003a29
+   180003a29:	add    %cl,(%rax)
+   180003a2b:	add    %bl,0x5f(%rdi)
+   180003a2e:	rex.XB pop %r15
+   180003a30:	jae    0x180003aa2
+   180003a32:	movsxd %gs:0x66(%rcx),%ebp
+   180003a36:	imul   $0x646e6168,0x5f(%rbx),%esp
+   180003a3d:	insb   (%dx),%es:(%rdi)
+   180003a3e:	gs jb  0x180003a41
+   180003a41:	add    %ah,0x735f5f00(%rip)        # 0x1f35f9947
+   180003a47:	je     0x180003aad
+   180003a49:	pop    %rdi
+   180003a4a:	je     0x180003ac5
+   180003a4c:	jo     0x180003ab3
+   180003a4e:	pop    %rdi
+   180003a4f:	imul   $0x65645f6f,0x66(%rsi),%ebp
+   180003a56:	jae    0x180003acc
+   180003a58:	jb     0x180003ac9
+   180003a5a:	jns    0x180003abb
+   180003a5c:	insb   (%dx),%es:(%rdi)
+   180003a5d:	imul   $0x43560000,0x74(%rbx),%esi
+   180003a64:	push   %rdx
+   180003a65:	push   %rbp
+   180003a66:	rex.WRX push %rsp
+   180003a68:	rex.WB
+   180003a69:	rex.WRB
+   180003a6a:	xor    %r14d,(%r8,%rsi,1)
+   180003a6e:	cs fs insb (%dx),%es:(%rdi)
+   180003a71:	insb   (%dx),%es:(%rdi)
+   180003a72:	add    %al,(%rax)
+   180003a74:	ss add %bl,0x69(%rdi)
+   180003a78:	outsb  %ds:(%rsi),(%dx)
+   180003a79:	imul   $0x37006d72,0x65(%rsp,%rsi,2),%esi
+   180003a81:	add    %bl,0x69(%rdi)
+   180003a84:	outsb  %ds:(%rsi),(%dx)
+   180003a85:	imul   $0x655f6d72,0x65(%rsp,%rsi,2),%esi
+   180003a8d:	add    %bh,(%rdi)
+   180003a8f:	add    %bl,0x73(%rdi)
+   180003a92:	gs push $0x6c69665f
+   180003a98:	je     0x180003aff
+   180003a9a:	jb     0x180003afb
+   180003a9c:	fs insb (%dx),%es:(%rdi)
+   180003a9e:	insb   (%dx),%es:(%rdi)
+   180003a9f:	add    %bl,(%rax)
+   180003aa1:	add    %bl,0x63(%rdi)
+   180003aa4:	outsl  %ds:(%rsi),(%dx)
+   180003aa5:	outsb  %ds:(%rsi),(%dx)
+   180003aa6:	imul   $0x6572,0x75(%rdi),%sp
+   180003aac:	pop    %rdi
+   180003aad:	outsb  %ds:(%rsi),(%dx)
+   180003aae:	(bad)
+   180003aaf:	jb     0x180003b23
+   180003ab1:	outsl  %ds:(%rsi),(%dx)
+   180003ab2:	ja     0x180003b13
+   180003ab4:	(bad)
+   180003ab5:	jb     0x180003b1e
+   180003ab7:	jbe    0x180003ab9
+   180003ab9:	add    %dh,(%rbx)
+   180003abb:	add    %bl,0x69(%rdi)
+   180003abe:	outsb  %ds:(%rsi),(%dx)
+   180003abf:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   180003ac7:	pop    %rdi
+   180003ac8:	outsb  %ds:(%rsi),(%dx)
+   180003ac9:	(bad)
+   180003aca:	jb     0x180003b3e
+   180003acc:	outsl  %ds:(%rsi),(%dx)
+   180003acd:	ja     0x180003b2e
+   180003acf:	outsb  %gs:(%rsi),(%dx)
+   180003ad1:	jbe    0x180003b3c
+   180003ad3:	jb     0x180003b44
+   180003ad5:	outsb  %ds:(%rsi),(%dx)
+   180003ad6:	insl   (%dx),%es:(%rdi)
+   180003ad7:	outsb  %gs:(%rsi),(%dx)
+   180003ad9:	je     0x180003adb
+   180003adb:	add    %dh,(%rax,%rax,1)
+   180003ade:	pop    %rdi
+   180003adf:	imul   $0x6c616974,0x69(%rsi),%ebp
+   180003ae6:	imul   $0x656e6f5f,0x65(%rdx),%edi
+   180003aed:	js     0x180003b58
+   180003aef:	je     0x180003b50
+   180003af1:	je     0x180003b54
+   180003af3:	(bad)
+   180003af4:	insb   (%dx),%es:(%rdi)
+   180003af5:	add    %al,%gs:(%rax)
+   180003af8:	and    (%rax),%al
+   180003afa:	pop    %rdi
+   180003afb:	gs js  0x180003b63
+   180003afe:	movsxd 0x74(%rbp),%esi
+   180003b01:	gs pop %rdi
+   180003b03:	outsl  %ds:(%rsi),(%dx)
+   180003b04:	outsb  %ds:(%rsi),(%dx)
+   180003b05:	gs js  0x180003b71
+   180003b08:	je     0x180003b69
+   180003b0a:	je     0x180003b6d
+   180003b0c:	(bad)
+   180003b0d:	insb   (%dx),%es:(%rdi)
+   180003b0e:	add    %dl,%gs:(%rsi)
+   180003b11:	add    %bl,0x63(%rdi)
+   180003b14:	gs js  0x180003b80
+   180003b17:	je     0x180003b19
+   180003b19:	add    %ah,0x70(%rcx)
+   180003b1c:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72dae93
+   180003b26:	jb     0x180003b9c
+   180003b28:	sub    $0x746e7572,%eax
+   180003b2d:	imul   $0x2d316c2d,0x65(%rbp),%ebp
+   180003b34:	xor    %ebp,0x6c642e30(%rip)        # 0x1ec64696a
+   180003b3a:	insb   (%dx),%es:(%rdi)
+   180003b3b:	add    %ah,0x51(%rsp,%rax,1)
+   180003b3f:	jne    0x180003ba6
+   180003b41:	jb     0x180003bbc
+   180003b43:	push   %rax
+   180003b44:	gs jb  0x180003bad
+   180003b47:	outsl  %ds:(%rsi),(%dx)
+   180003b48:	jb     0x180003bb7
+   180003b4a:	(bad)
+   180003b4b:	outsb  %ds:(%rsi),(%dx)
+   180003b4c:	movsxd 0x43(%rbp),%esp
+   180003b4f:	outsl  %ds:(%rsi),(%dx)
+   180003b50:	jne    0x180003bc0
+   180003b52:	je     0x180003bb9
+   180003b54:	jb     0x180003b56
+   180003b56:	sub    (%rdx),%eax
+   180003b58:	rex.RXB
+   180003b59:	gs je  0x180003b9f
+   180003b5c:	jne    0x180003bd0
+   180003b5e:	jb     0x180003bc5
+   180003b60:	outsb  %ds:(%rsi),(%dx)
+   180003b61:	je     0x180003bb3
+   180003b63:	jb     0x180003bd4
+   180003b65:	movsxd 0x73(%rbp),%esp
+   180003b68:	jae    0x180003bb3
+   180003b6a:	add    %ch,%fs:(%rdi)
+   180003b6d:	add    0x65(%rdi),%al
+   180003b70:	je     0x180003bb5
+   180003b72:	jne    0x180003be6
+   180003b74:	jb     0x180003bdb
+   180003b76:	outsb  %ds:(%rsi),(%dx)
+   180003b77:	je     0x180003bcd
+   180003b79:	push   $0x64616572
+   180003b7e:	rex.WB
+   180003b7f:	add    %al,%fs:(%rax)
+   180003b82:	add    %eax,(%rbx)
+   180003b84:	rex.RXB
+   180003b85:	gs je  0x180003bdb
+   180003b88:	jns    0x180003bfd
+   180003b8a:	je     0x180003bf1
+   180003b8c:	insl   (%dx),%es:(%rdi)
+   180003b8d:	push   %rsp
+   180003b8e:	imul   $0x69467341,0x65(%rbp),%ebp
+   180003b95:	insb   (%dx),%es:(%rdi)
+   180003b96:	gs push %rsp
+   180003b98:	imul   $0x44012c00,0x65(%rbp),%ebp
+   180003b9f:	imul   $0x54656c62,0x61(%rbx),%esi
+   180003ba6:	push   $0x64616572
+   180003bab:	imul   $0x43797261,0x72(%rdx),%r12
+   180003bb3:	(bad)
+   180003bb4:	insb   (%dx),%es:(%rdi)
+   180003bb5:	insb   (%dx),%es:(%rdi)
+   180003bb6:	jae    0x180003bb8
+   180003bb8:	addl   $0x74696e49,(%rbx)
+   180003bbe:	imul   $0x53657a69,0x6c(%rcx),%esp
+   180003bc5:	imul   $0x64616548,0x74(%rbx),%r14
+   180003bcd:	add    %ch,%cl
+   180003bcf:	add    $0x52,%al
+   180003bd1:	je     0x180003c3f
+   180003bd3:	rex.XB (bad)
+   180003bd5:	jo     0x180003c4b
+   180003bd7:	jne    0x180003c4b
+   180003bd9:	rex.XB outsl %gs:(%rsi),(%dx)
+   180003bdc:	outsb  %ds:(%rsi),(%dx)
+   180003bdd:	je     0x180003c44
+   180003bdf:	js     0x180003c55
+   180003be1:	add    %dh,%cl
+   180003be3:	add    $0x52,%al
+   180003be5:	je     0x180003c53
+   180003be7:	rex.WR outsl %ds:(%rsi),(%dx)
+   180003be9:	outsl  %ds:(%rsi),(%dx)
+   180003bea:	imul   $0x46,0x70(%rbp),%esi
+   180003bee:	jne    0x180003c5e
+   180003bf0:	movsxd 0x6f(%rcx,%rbp,2),%esi
+   180003bf4:	outsb  %ds:(%rsi),(%dx)
+   180003bf5:	rex.RB outsb %ds:(%rsi),(%dx)
+   180003bf7:	je     0x180003c6b
+   180003bf9:	jns    0x180003bfb
+   180003bfb:	add    %bh,%al
+   180003bfd:	add    $0x52,%al
+   180003bff:	je     0x180003c6d
+   180003c01:	push   %rsi
+   180003c02:	imul   $0x556c6175,0x74(%rdx),%esi
+   180003c09:	outsb  %ds:(%rsi),(%dx)
+   180003c0a:	ja     0x180003c75
+   180003c0c:	outsb  %ds:(%rsi),(%dx)
+   180003c0d:	add    %al,%fs:(%rax)
+   180003c10:	xchg   %eax,%edi
+   180003c11:	add    0x73(%rcx),%ecx
+   180003c14:	rex.R
+   180003c15:	(bad)
+   180003c1b:	jb     0x180003c6d
+   180003c1d:	jb     0x180003c84
+   180003c1f:	jae    0x180003c86
+   180003c21:	outsb  %ds:(%rsi),(%dx)
+   180003c22:	je     0x180003c24
+   180003c24:	fadds  0x61686e55(%rip)        # 0x1e168aa7f
+   180003c2a:	outsb  %ds:(%rsi),(%dx)
+   180003c2b:	fs insb (%dx),%es:(%rdi)
+   180003c2d:	gs fs rex.RB js 0x180003c95
+   180003c32:	gs jo  0x180003ca9
+   180003c35:	imul   $0x746c6946,0x6e(%rdi),%ebp
+   180003c3c:	gs jb  0x180003c3f
+   180003c3f:	add    %dl,0x74655305(%rdi)
+   180003c45:	push   %rbp
+   180003c46:	outsb  %ds:(%rsi),(%dx)
+   180003c47:	push   $0x6c646e61
+   180003c4c:	gs fs rex.RB js 0x180003cb4
+   180003c51:	gs jo  0x180003cc8
+   180003c54:	imul   $0x746c6946,0x6e(%rdi),%ebp
+   180003c5b:	gs jb  0x180003c5e
+   180003c5e:	sahf
+   180003c5f:	add    0x73(%rcx),%ecx
    180003c62:	push   %rax
-   180003c63:	jb     0x180003cca
-   180003c65:	jae    0x180003ccc
-   180003c67:	outsb  %ds:(%rsi),(%dx)
-   180003c68:	je     0x180003c6a
-   180003c6a:	rex.WXB
-   180003c6b:	rex.RB push %r10
-   180003c6d:	rex.WRX
-   180003c6e:	rex.RB
-   180003c6f:	xor    (%rdx),%r14
-   180003c72:	cs fs insb (%dx),%es:(%rdi)
-   180003c75:	insb   (%dx),%es:(%rdi)
-   180003c76:	add    %al,(%rax)
-   180003c78:	cmp    $0x0,%al
-   180003c7a:	insl   (%dx),%es:(%rdi)
-   180003c7b:	gs insl (%dx),%es:(%rdi)
-   180003c7d:	movsxd 0x79(%rax),%esi
+   180003c63:	jb     0x180003cd4
+   180003c65:	movsxd 0x73(%rbp),%esp
+   180003c68:	jae    0x180003cd9
+   180003c6a:	jb     0x180003cb2
+   180003c6c:	gs (bad)
+   180003c6e:	je     0x180003ce5
+   180003c70:	jb     0x180003cd7
+   180003c72:	push   %rax
+   180003c73:	jb     0x180003cda
+   180003c75:	jae    0x180003cdc
+   180003c77:	outsb  %ds:(%rsi),(%dx)
+   180003c78:	je     0x180003c7a
+   180003c7a:	rex.WXB
+   180003c7b:	rex.RB push %r10
+   180003c7d:	rex.WRX
+   180003c7e:	rex.RB
+   180003c7f:	xor    (%rdx),%r14
+   180003c82:	cs fs insb (%dx),%es:(%rdi)
+   180003c85:	insb   (%dx),%es:(%rdi)
+   180003c86:	add    %al,(%rax)
+   180003c88:	cmp    $0x0,%al
+   180003c8a:	insl   (%dx),%es:(%rdi)
+   180003c8b:	gs insl (%dx),%es:(%rdi)
+   180003c8d:	movsxd 0x79(%rax),%esi
 	...
 
 Disassembly of section .data:
 
 0000000180004000 <.data>:
    180004000:	(bad)
    180004001:	(bad)
@@ -3267,239 +3334,260 @@
 	...
 
 Disassembly of section .pdata:
 
 0000000180081000 <.pdata>:
    180081000:	add    %dl,(%rax)
    180081002:	add    %al,(%rax)
-   180081004:	mov    $0xa0000010,%esp
-   180081009:	xor    $0x10bc0000,%eax
-   18008100e:	add    %al,(%rax)
-   180081010:	(bad)
+   180081004:	ret    $0x10
+   180081007:	add    %ah,-0x3dffffcb(%rax)
+   18008100d:	adc    %al,(%rax)
+   18008100f:	add    %ah,(%rdx)
    180081011:	adc    (%rax),%al
-   180081013:	add    %dh,0x2f000035(%rax)
-   180081019:	adc    (%rax),%al
-   18008101b:	add    %bh,(%rdi)
-   18008101d:	adc    (%rax),%al
+   180081013:	add    %dh,0x12220000(%rbp,%rsi,1)
+   18008101a:	add    %al,(%rax)
+   18008101c:	rex.X adc (%rax),%al
    18008101f:	add    %dl,%ah
-   180081021:	xor    $0x12400000,%eax
+   180081021:	xor    $0x12500000,%eax
    180081026:	add    %al,(%rax)
-   180081028:	mov    $0x12,%ch
+   180081028:	rcll   (%rdx)
    18008102a:	add    %al,(%rax)
-   18008102c:	insb   (%dx),%es:(%rdi)
-   18008102d:	ss add %al,(%rax)
-   180081030:	mov    $0x12,%ch
+   18008102c:	in     $0x35,%al
+   18008102e:	add    %al,(%rax)
+   180081030:	rcll   (%rdx)
    180081032:	add    %al,(%rax)
-   180081034:	xor    (%rbx),%edx
-   180081036:	add    %al,(%rax)
-   180081038:	jl     0x180081070
+   180081034:	rex adc $0x35f80000,%eax
    18008103a:	add    %al,(%rax)
-   18008103c:	xor    (%rbx),%edx
-   18008103e:	add    %al,(%rax)
-   180081040:	adc    $0x15,%al
+   18008103c:	rex adc $0x15a60000,%eax
    180081042:	add    %al,(%rax)
-   180081044:	pushf
-   180081045:	ss add %al,(%rax)
-   180081048:	adc    $0x15,%al
+   180081044:	sbb    %dh,(%rsi)
+   180081046:	add    %al,(%rax)
+   180081048:	mov    $0x15,%al
    18008104a:	add    %al,(%rax)
-   18008104c:	rex adc $0x36b00000,%eax
+   18008104c:	int    $0x15
+   18008104e:	add    %al,(%rax)
+   180081050:	sub    %dh,(%rsi)
    180081052:	add    %al,(%rax)
-   180081054:	rex adc $0x158a0000,%eax
-   18008105a:	add    %al,(%rax)
-   18008105c:	shlb   $0x0,(%rsi)
-   18008105f:	add    %dl,-0x5bffffeb(%rax)
-   180081065:	adc    $0x35e40000,%eax
-   18008106a:	add    %al,(%rax)
-   18008106c:	movsb  %ds:(%rsi),%es:(%rdi)
-   18008106d:	adc    $0x16600000,%eax
+   180081054:	int    $0x15
+   180081056:	add    %al,(%rax)
+   180081058:	(bad)
+   180081059:	adc    $0x36380000,%eax
+   18008105e:	add    %al,(%rax)
+   180081060:	(bad)
+   180081061:	adc    $0x16b00000,%eax
+   180081066:	add    %al,(%rax)
+   180081068:	rex.WR
+   180081069:	ss add %al,(%rax)
+   18008106c:	mov    $0x16,%al
+   18008106e:	add    %al,(%rax)
+   180081070:	ficoms (%rsi)
    180081072:	add    %al,(%rax)
-   180081074:	hlt
-   180081075:	xor    $0x16600000,%eax
+   180081074:	push   $0xffffffffde000036
+   180081079:	(bad)
    18008107a:	add    %al,(%rax)
-   18008107c:	mov    (%rsi),%ss
+   18008107c:	call   *(%rsi)
    18008107e:	add    %al,(%rax)
-   180081080:	or     %dh,(%rsi)
-   180081082:	add    %al,(%rax)
-   180081084:	mov    (%rsi),%ss
+   180081080:	xorb   $0x0,(%rsi)
+   180081083:	add    %bh,%bh
+   180081085:	(bad)
    180081086:	add    %al,(%rax)
-   180081088:	adc    (%rdi),%edx
+   180081088:	outsb  %ds:(%rsi),(%dx)
+   180081089:	(bad)
    18008108a:	add    %al,(%rax)
-   18008108c:	sbb    %dh,(%rsi)
-   18008108e:	add    %al,(%rax)
-   180081090:	adc    (%rdi),%edx
+   18008108c:	xchg   %eax,%esp
+   18008108d:	ss add %al,(%rax)
+   180081090:	outsb  %ds:(%rsi),(%dx)
+   180081091:	(bad)
    180081092:	add    %al,(%rax)
-   180081094:	int1
-   180081095:	sbb    %al,(%rax)
-   180081097:	add    %dh,(%rsi,%rsi,1)
+   180081094:	and    %ebx,(%rcx)
+   180081096:	add    %al,(%rax)
+   180081098:	mov    $0x36,%ah
    18008109a:	add    %al,(%rax)
-   18008109c:	int1
-   18008109d:	sbb    %al,(%rax)
-   18008109f:	add    %ah,(%rax)
+   18008109c:	and    %ebx,(%rcx)
+   18008109e:	add    %al,(%rax)
+   1800810a0:	xchg   %eax,%esp
    1800810a1:	sbb    %eax,(%rax)
-   1800810a3:	add    %cl,0x36(%rax)
-   1800810a6:	add    %al,(%rax)
-   1800810a8:	and    %bl,(%rcx)
-   1800810aa:	add    %al,(%rax)
-   1800810ac:	sbb    %eax,%fs:(%rax)
-   1800810af:	add    %bl,0x36(%rax)
-   1800810b2:	add    %al,(%rax)
-   1800810b4:	sbb    %eax,%fs:(%rax)
-   1800810b7:	add    %dh,0x37680000(%rcx,%rbx,1)
+   1800810a3:	add    %cl,%al
+   1800810a5:	ss add %al,(%rax)
+   1800810a8:	xchg   %eax,%esp
+   1800810a9:	sbb    %eax,(%rax)
+   1800810ab:	add    %bh,-0x7fffffe7(%rbx)
+   1800810b1:	ss add %al,(%rax)
+   1800810b4:	mov    $0xc000019,%esp
+   1800810b9:	sbb    (%rax),%al
+   1800810bb:	add    %dh,0x37(%rax)
    1800810be:	add    %al,(%rax)
-   1800810c0:	mov    $0x19,%ah
+   1800810c0:	or     $0x1a,%al
    1800810c2:	add    %al,(%rax)
-   1800810c4:	lret   $0x1a
-   1800810c7:	add    %dl,%al
-   1800810c9:	ss add %al,(%rax)
-   1800810cc:	int3
-   1800810cd:	sbb    (%rax),%al
-   1800810cf:	add    %dl,0x1b(%rax)
+   1800810c4:	and    (%rbx),%bl
+   1800810c6:	add    %al,(%rax)
+   1800810c8:	fdivs  (%rsi)
+   1800810ca:	add    %al,(%rax)
+   1800810cc:	and    $0x1b,%al
+   1800810ce:	add    %al,(%rax)
+   1800810d0:	test   $0x1b,%al
    1800810d2:	add    %al,(%rax)
-   1800810d4:	adc    $0x37,%al
+   1800810d4:	sbb    $0x37,%al
    1800810d6:	add    %al,(%rax)
-   1800810d8:	push   %rax
-   1800810d9:	sbb    (%rax),%eax
-   1800810db:	add    %al,0x7000001c(%rcx)
-   1800810e1:	(bad)
+   1800810d8:	test   $0x1b,%al
+   1800810da:	add    %al,(%rax)
+   1800810dc:	fstps  (%rax,%rax,1)
+   1800810df:	add    %bh,0x37(%rax)
    1800810e2:	add    %al,(%rax)
-   1800810e4:	test   %bl,(%rax,%rax,1)
-   1800810e7:	add    %al,%cl
-   1800810e9:	sbb    $0x0,%al
-   1800810eb:	add    %ah,-0x3bffffc9(%rax)
-   1800810f1:	sbb    $0x0,%al
-   1800810f3:	add    %dh,0x1d(%rax)
-   1800810f6:	add    %al,(%rax)
-   1800810f8:	mov    $0x37,%al
-   1800810fa:	add    %al,(%rax)
-   1800810fc:	jo     0x18008111b
-   1800810fe:	add    %al,(%rax)
-   180081100:	xchg   %eax,%ebx
-   180081101:	sbb    $0x37680000,%eax
+   1800810e4:	fcompl (%rax,%rax,1)
+   1800810e7:	add    %bl,(%rcx)
+   1800810e9:	sbb    $0x37a80000,%eax
+   1800810ee:	add    %al,(%rax)
+   1800810f0:	sbb    $0x1d,%al
+   1800810f2:	add    %al,(%rax)
+   1800810f4:	enter  $0x1d,$0x0
+   1800810f8:	mov    $0xc8000037,%eax
+   1800810fd:	sbb    $0x1deb0000,%eax
+   180081102:	add    %al,(%rax)
+   180081104:	jo     0x18008113d
    180081106:	add    %al,(%rax)
-   180081108:	rcrb   $0x0,0x1ddb0000(%rip)        # 0x19de3110f
-   18008110f:	add    %ch,0x37(%rax)
+   180081108:	sbb    %bl,(%rsi)
+   18008110a:	add    %al,(%rax)
+   18008110c:	xor    (%rsi),%ebx
+   18008110e:	add    %al,(%rax)
+   180081110:	jo     0x180081149
    180081112:	add    %al,(%rax)
-   180081114:	fcompl 0x1e150000(%rip)        # 0x19e1d111a
+   180081114:	xor    $0x1e,%al
+   180081116:	add    %al,(%rax)
+   180081118:	insl   (%dx),%es:(%rdi)
+   180081119:	(bad)
    18008111a:	add    %al,(%rax)
-   18008111c:	push   $0x18000037
-   180081121:	(bad)
+   18008111c:	jo     0x180081155
+   18008111e:	add    %al,(%rax)
+   180081120:	jo     0x180081140
    180081122:	add    %al,(%rax)
-   180081124:	rex.WR (bad)
+   180081124:	movsb  %ds:(%rsi),%es:(%rdi)
+   180081125:	(bad)
    180081126:	add    %al,(%rax)
-   180081128:	push   $0x4c000037
+   180081128:	jo     0x180081161
+   18008112a:	add    %al,(%rax)
+   18008112c:	movsb  %ds:(%rsi),%es:(%rdi)
    18008112d:	(bad)
    18008112e:	add    %al,(%rax)
-   180081130:	(bad)
-   180081131:	(bad)
-   180081132:	add    %al,(%rax)
-   180081134:	push   $0x64000037
-   180081139:	(bad)
-   18008113a:	add    %al,(%rax)
-   18008113c:	mov    %ds,(%rsi)
+   180081130:	mov    $0x7000001e,%ecx
+   180081135:	(bad)
+   180081136:	add    %al,(%rax)
+   180081138:	mov    $0xe400001e,%esp
+   18008113d:	(bad)
    18008113e:	add    %al,(%rax)
-   180081140:	push   $0xffffffff8c000037
-   180081145:	(bad)
+   180081140:	jo     0x180081179
+   180081142:	add    %al,(%rax)
+   180081144:	in     $0x1e,%al
    180081146:	add    %al,(%rax)
-   180081148:	movabs 0xa40000376800001e,%eax
+   180081148:	stc
+   180081149:	(bad)
+   18008114a:	add    %al,(%rax)
+   18008114c:	jo     0x180081185
+   18008114e:	add    %al,(%rax)
+   180081150:	cld
    180081151:	(bad)
    180081152:	add    %al,(%rax)
-   180081154:	add    $0x1f,%al
+   180081154:	pop    %rsp
+   180081155:	(bad)
    180081156:	add    %al,(%rax)
-   180081158:	in     (%dx),%al
+   180081158:	hlt
    180081159:	(bad)
    18008115a:	add    %al,(%rax)
-   18008115c:	add    $0x1f,%al
+   18008115c:	pop    %rsp
+   18008115d:	(bad)
    18008115e:	add    %al,(%rax)
-   180081160:	xor    $0x1f,%al
+   180081160:	mov    %ds,(%rdi)
    180081162:	add    %al,(%rax)
-   180081164:	push   $0x34000037
-   180081169:	(bad)
+   180081164:	jo     0x18008119d
+   180081166:	add    %al,(%rax)
+   180081168:	mov    %ds,(%rdi)
    18008116a:	add    %al,(%rax)
-   18008116c:	rex.W (bad)
-   18008116e:	add    %al,(%rax)
-   180081170:	push   $0x48000037
+   18008116c:	movabs 0xa00000377000001f,%al
    180081175:	(bad)
    180081176:	add    %al,(%rax)
-   180081178:	xchg   %eax,%ecx
-   180081179:	(bad)
-   18008117a:	add    %al,(%rax)
-   18008117c:	in     $0x37,%al
+   180081178:	jmp    0x16c08119c
+   18008117d:	(bad)
    18008117e:	add    %al,(%rax)
-   180081180:	xchg   %eax,%esp
+   180081180:	in     (%dx),%al
    180081181:	(bad)
    180081182:	add    %al,(%rax)
-   180081184:	(bad)
-   180081185:	and    %al,(%rax)
-   180081187:	add    %ah,%ah
+   180081184:	ja     0x1800811a6
+   180081186:	add    %al,(%rax)
+   180081188:	in     (%dx),%al
    180081189:	(bad)
    18008118a:	add    %al,(%rax)
-   18008118c:	and    %ah,(%rax)
+   18008118c:	js     0x1800811ae
    18008118e:	add    %al,(%rax)
-   180081190:	mov    $0xbc000020,%eax
+   180081190:	adc    %ah,(%rcx)
+   180081192:	add    %al,(%rax)
+   180081194:	(bad)
    180081195:	(bad)
    180081196:	add    %al,(%rax)
-   180081198:	mov    $0xdc000020,%eax
-   18008119d:	and    %al,(%rax)
-   18008119f:	add    %ah,%ah
+   180081198:	adc    %ah,(%rcx)
+   18008119a:	add    %al,(%rax)
+   18008119c:	xor    $0x21,%al
+   18008119e:	add    %al,(%rax)
+   1800811a0:	in     (%dx),%al
    1800811a1:	(bad)
    1800811a2:	add    %al,(%rax)
-   1800811a4:	fsubl  (%rax)
+   1800811a4:	xor    $0x21,%al
    1800811a6:	add    %al,(%rax)
-   1800811a8:	add    $0xe4000021,%eax
+   1800811a8:	pop    %rbp
+   1800811a9:	and    %eax,(%rax)
+   1800811ab:	add    %ch,%ah
    1800811ad:	(bad)
    1800811ae:	add    %al,(%rax)
-   1800811b0:	sbb    %ah,(%rcx)
+   1800811b0:	jo     0x1800811d3
    1800811b2:	add    %al,(%rax)
-   1800811b4:	movsxd (%rdx),%esp
-   1800811b6:	add    %al,(%rax)
-   1800811b8:	add    %bh,(%rax)
-   1800811ba:	add    %al,(%rax)
-   1800811bc:	and    %fs:(%rax),%al
-   1800811bf:	add    %ah,0x10000022(%rax)
-   1800811c5:	cmp    %al,(%rax)
-   1800811c7:	add    %ah,-0x23ffffde(%rax)
-   1800811cd:	and    (%rax),%al
-   1800811cf:	add    %dl,(%rax)
-   1800811d1:	cmp    %al,(%rax)
-   1800811d3:	add    %ah,%al
-   1800811d5:	and    (%rax),%al
-   1800811d7:	add    %cl,0x381c0000(%rsp)
+   1800811b4:	mov    $0x8000022,%ebx
+   1800811b9:	cmp    %al,(%rax)
+   1800811bb:	add    %bh,0x22f80000(%rdx,%riz,1)
+   1800811c2:	add    %al,(%rax)
+   1800811c4:	sbb    %bh,(%rax)
+   1800811c6:	add    %al,(%rax)
+   1800811c8:	clc
+   1800811c9:	and    (%rax),%al
+   1800811cb:	add    %dh,(%rbx,%riz,1)
+   1800811ce:	add    %al,(%rax)
+   1800811d0:	sbb    %bh,(%rax)
+   1800811d2:	add    %al,(%rax)
+   1800811d4:	cmp    %ah,(%rbx)
+   1800811d6:	add    %al,(%rax)
+   1800811d8:	in     $0x24,%al
+   1800811da:	add    %al,(%rax)
+   1800811dc:	and    $0x38,%al
    1800811de:	add    %al,(%rax)
-   1800811e0:	adc    %ah,0x25120000(%rip)        # 0x1a51a11e6
+   1800811e0:	jo     0x180081207
+   1800811e2:	add    %al,(%rax)
+   1800811e4:	jb     0x18008120b
    1800811e6:	add    %al,(%rax)
-   1800811e8:	xor    %bh,(%rax)
+   1800811e8:	cmp    %bh,(%rax)
    1800811ea:	add    %al,(%rax)
-   1800811ec:	xor    %ah,0x25360000(%rip)        # 0x1a53e11f2
+   1800811ec:	nop
+   1800811ed:	and    $0x25960000,%eax
    1800811f2:	add    %al,(%rax)
-   1800811f4:	cmp    %bh,(%rax)
-   1800811f6:	add    %al,(%rax)
-   1800811f8:	ss and $0x254d0000,%eax
-   1800811fe:	add    %al,(%rax)
-   180081200:	or     $0x37,%al
+   1800811f4:	rex cmp %al,(%rax)
+   1800811f7:	add    %dl,-0x52ffffdb(%rsi)
+   1800811fd:	and    $0x37140000,%eax
    180081202:	add    %al,(%rax)
-   180081204:	rex.WRB and $0x25660000,%rax
+   180081204:	lods   %ds:(%rsi),%eax
+   180081205:	and    $0x25c60000,%eax
    18008120a:	add    %al,(%rax)
-   18008120c:	or     $0x37,%al
+   18008120c:	adc    $0x37,%al
    18008120e:	add    %al,(%rax)
-   180081210:	and    $0x0,%ax
-   180081214:	jp     0x18008123b
+   180081210:	(bad)
+   180081211:	and    $0x25da0000,%eax
    180081216:	add    %al,(%rax)
-   180081218:	or     $0x37,%al
+   180081218:	adc    $0x37,%al
    18008121a:	add    %al,(%rax)
-   18008121c:	jp     0x180081243
-   18008121e:	add    %al,(%rax)
-   180081220:	mov    $0x25,%al
+   18008121c:	fisubl 0x26100000(%rip)        # 0x1a6181222
    180081222:	add    %al,(%rax)
-   180081224:	cwtl
-   180081225:	(bad)
-   180081226:	add    %al,(%rax)
-   180081228:	mov    $0x25,%al
-   18008122a:	add    %al,(%rax)
-   18008122c:	enter  $0x25,$0x0
-   180081230:	fdivl  (%rdi)
+   180081224:	movabs 0x2800002610000037,%al
+   18008122d:	es add %al,(%rax)
+   180081230:	in     $0x37,%al
 	...
 
 Disassembly of section .rsrc:
 
 0000000180082000 <.rsrc>:
 	...
    180082008:	add    $0x0,%al
```

