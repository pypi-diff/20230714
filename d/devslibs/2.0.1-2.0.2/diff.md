# Comparing `tmp/devslibs-2.0.1.tar.gz` & `tmp/devslibs-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devslibs-2.0.1.tar", last modified: Thu Jul 13 15:37:44 2023, max compression
+gzip compressed data, was "devslibs-2.0.2.tar", last modified: Fri Jul 14 07:33:39 2023, max compression
```

## Comparing `devslibs-2.0.1.tar` & `devslibs-2.0.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.695675 devslibs-2.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.683674 devslibs-2.0.1/Ayra/
--rw-r--r--   0 root         (0) root         (0)     2991 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.683674 devslibs-2.0.1/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12360 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.687675 devslibs-2.0.1/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1910 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.691675 devslibs-2.0.1/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28822 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.695675 devslibs-2.0.1/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8629 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18539 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-13 15:37:25.000000 devslibs-2.0.1/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-07-13 15:37:25.000000 devslibs-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3490 2023-07-13 15:37:44.695675 devslibs-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-13 15:37:25.000000 devslibs-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:37:44.695675 devslibs-2.0.1/devslibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3490 2023-07-13 15:37:44.000000 devslibs-2.0.1/devslibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-13 15:37:44.000000 devslibs-2.0.1/devslibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 15:37:44.000000 devslibs-2.0.1/devslibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 15:37:44.000000 devslibs-2.0.1/devslibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-13 15:37:44.000000 devslibs-2.0.1/devslibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 15:37:44.695675 devslibs-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1589 2023-07-13 15:37:25.000000 devslibs-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.722960 devslibs-2.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.714959 devslibs-2.0.2/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.718959 devslibs-2.0.2/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12360 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.718959 devslibs-2.0.2/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.722960 devslibs-2.0.2/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28822 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.722960 devslibs-2.0.2/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18543 2023-07-14 07:33:20.000000 devslibs-2.0.2/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-13 15:37:25.000000 devslibs-2.0.2/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-14 07:33:20.000000 devslibs-2.0.2/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-07-13 15:37:25.000000 devslibs-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-14 07:33:39.722960 devslibs-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-13 15:37:25.000000 devslibs-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:33:39.722960 devslibs-2.0.2/devslibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-14 07:33:39.000000 devslibs-2.0.2/devslibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-14 07:33:39.000000 devslibs-2.0.2/devslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 07:33:39.000000 devslibs-2.0.2/devslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 07:33:39.000000 devslibs-2.0.2/devslibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-14 07:33:39.000000 devslibs-2.0.2/devslibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 07:33:39.722960 devslibs-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-07-13 15:37:25.000000 devslibs-2.0.2/setup.py
```

### Comparing `devslibs-2.0.1/Ayra/__init__.py` & `devslibs-2.0.2/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/__main__.py` & `devslibs-2.0.2/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/_misc/__init__.py` & `devslibs-2.0.2/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/_misc/_assistant.py` & `devslibs-2.0.2/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/_misc/_decorators.py` & `devslibs-2.0.2/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/_misc/_supporter.py` & `devslibs-2.0.2/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/_misc/_wrappers.py` & `devslibs-2.0.2/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/configs.py` & `devslibs-2.0.2/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/__init__.py` & `devslibs-2.0.2/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/afk_db.py` & `devslibs-2.0.2/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/antiflood_db.py` & `devslibs-2.0.2/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/asst_fns.py` & `devslibs-2.0.2/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/asstcmd_db.py` & `devslibs-2.0.2/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/autoban_db.py` & `devslibs-2.0.2/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/blacklist_db.py` & `devslibs-2.0.2/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/botchat_db.py` & `devslibs-2.0.2/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/broadcast_db.py` & `devslibs-2.0.2/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/ch_db.py` & `devslibs-2.0.2/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/dnd_db.py` & `devslibs-2.0.2/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/echo_db.py` & `devslibs-2.0.2/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/filestore_db.py` & `devslibs-2.0.2/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/filter_db.py` & `devslibs-2.0.2/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/forcesub_db.py` & `devslibs-2.0.2/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/gban_mute_db.py` & `devslibs-2.0.2/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/gcast_blacklist_db.py` & `devslibs-2.0.2/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/greetings_db.py` & `devslibs-2.0.2/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/logusers_db.py` & `devslibs-2.0.2/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/mute_db.py` & `devslibs-2.0.2/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/night_db.py` & `devslibs-2.0.2/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/notes_db.py` & `devslibs-2.0.2/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/nsfw_db.py` & `devslibs-2.0.2/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/pmpermit_db.py` & `devslibs-2.0.2/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/snips_db.py` & `devslibs-2.0.2/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/vc_sudos.py` & `devslibs-2.0.2/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/dB/warn_db.py` & `devslibs-2.0.2/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/FastTelethon.py` & `devslibs-2.0.2/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/__init__.py` & `devslibs-2.0.2/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/admins.py` & `devslibs-2.0.2/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/executor.py` & `devslibs-2.0.2/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/gDrive.py` & `devslibs-2.0.2/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/google_image.py` & `devslibs-2.0.2/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/helper.py` & `devslibs-2.0.2/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/info.py` & `devslibs-2.0.2/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/misc.py` & `devslibs-2.0.2/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/tools.py` & `devslibs-2.0.2/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/fns/ytdl.py` & `devslibs-2.0.2/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/kynan.py` & `devslibs-2.0.2/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/loader.py` & `devslibs-2.0.2/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/BaseClient.py` & `devslibs-2.0.2/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/__init__.py` & `devslibs-2.0.2/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/_database.py` & `devslibs-2.0.2/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/_extra.py` & `devslibs-2.0.2/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/connections.py` & `devslibs-2.0.2/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/funcs.py` & `devslibs-2.0.2/Ayra/startup/funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,16 +341,16 @@
         UL = f"@{asst.me.username}"
         if not ayra_bot.me.username:
             sir = ayra_bot.me.first_name
         else:
             sir = f"@{ayra_bot.me.username}"
         file = random.choice(
             [
-                "resources/extras/logo.jpg",
-                "resources/extras/logo.jpg",
+                "./resources/extras/logo.jpg",
+                "./resources/extras/logo.jpg",
             ]
         )
         if not os.path.exists(file):
             file = await download_file(file, "profile.jpg")
             rem = True
         msg = await asst.send_message(
             chat_id, "**Penyesuaian Otomatis** Dimulai @Botfather"
```

### Comparing `devslibs-2.0.1/Ayra/startup/loader.py` & `devslibs-2.0.2/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/Ayra/startup/utils.py` & `devslibs-2.0.2/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/LICENSE` & `devslibs-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/PKG-INFO` & `devslibs-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devslibs
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `devslibs-2.0.1/README.md` & `devslibs-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/devslibs.egg-info/PKG-INFO` & `devslibs-2.0.2/devslibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devslibs
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `devslibs-2.0.1/devslibs.egg-info/SOURCES.txt` & `devslibs-2.0.2/devslibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devslibs-2.0.1/setup.py` & `devslibs-2.0.2/setup.py`

 * *Files identical despite different names*

