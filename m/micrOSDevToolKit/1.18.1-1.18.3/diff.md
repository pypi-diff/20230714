# Comparing `tmp/micrOSDevToolKit-1.18.1.tar.gz` & `tmp/micrOSDevToolKit-1.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.18.1.tar", last modified: Thu Jul  6 11:16:36 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.18.3.tar", last modified: Fri Jul 14 17:47:50 2023, max compression
```

## Comparing `micrOSDevToolKit-1.18.1.tar` & `micrOSDevToolKit-1.18.3.tar`

### file list

```diff
@@ -1,268 +1,269 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.110810 micrOSDevToolKit-1.18.1/
--rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.18.1/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-06 11:16:36.110112 micrOSDevToolKit-1.18.1/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.18.1/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.18.1/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:35.898726 micrOSDevToolKit-1.18.1/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:35.903118 micrOSDevToolKit-1.18.1/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.1/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.1/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:35.904756 micrOSDevToolKit-1.18.1/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:35.932583 micrOSDevToolKit-1.18.1/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:35.994508 micrOSDevToolKit-1.18.1/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.18.1/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6442 2023-07-06 10:43:08.000000 micrOSDevToolKit-1.18.1/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.18.1/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6345 2023-07-05 20:09:42.000000 micrOSDevToolKit-1.18.1/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2047 2023-07-06 09:27:38.000000 micrOSDevToolKit-1.18.1/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-06-28 17:39:05.000000 micrOSDevToolKit-1.18.1/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-06 10:27:16.000000 micrOSDevToolKit-1.18.1/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.18.1/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1592 2023-07-06 11:13:16.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.1/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.18.1/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.18.1/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.18.1/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-03-04 23:34:06.000000 micrOSDevToolKit-1.18.1/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-06-19 16:03:31.000000 micrOSDevToolKit-1.18.1/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-04 18:31:06.000000 micrOSDevToolKit-1.18.1/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.18.1/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/source/TinyPLed.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.008051 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     6020 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Common.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5582 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5406 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Debug.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2010 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Hooks.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5232 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterConnect.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8402 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4715 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1705 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1901 2023-07-01 19:35:59.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8842 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_system.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4265 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6294 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8881 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/SocketServer.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)    15255 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/TaskManager.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5912 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Time.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      833 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2139 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/micrOS.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3684 2023-07-01 19:15:09.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3355 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/urequests.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.1/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.18.1/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-06 11:13:33.000000 micrOSDevToolKit-1.18.1/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.18.1/micrOS/source/pycallgraph.png
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.18.1/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.18.1/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.010573 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-06 11:16:35.000000 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     9740 2023-07-06 11:16:35.000000 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-06 11:16:35.000000 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-06 11:16:35.000000 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-06 11:16:35.000000 micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-06 11:16:36.110962 micrOSDevToolKit-1.18.1/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-06 11:16:15.000000 micrOSDevToolKit-1.18.1/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.015169 micrOSDevToolKit-1.18.1/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.18.1/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.18.1/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31335 2023-07-05 12:50:59.000000 micrOSDevToolKit-1.18.1/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.18.1/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.025220 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.028129 micrOSDevToolKit-1.18.1/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.18.1/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.18.1/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.18.1/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.18.1/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.037926 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.059545 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-04 22:40:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6512 2023-07-04 22:40:18.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.18.1/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.060178 micrOSDevToolKit-1.18.1/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-06 11:16:36.108607 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1835 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3072 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1947 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      780 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2058 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4183 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2155 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4282 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3632 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3412 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3807 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5485 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2742 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1250 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1742 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-06 11:14:00.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1450 2023-07-06 11:14:01.000000 micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.459323 micrOSDevToolKit-1.18.3/
+-rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.18.3/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-14 17:47:50.458766 micrOSDevToolKit-1.18.3/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.18.3/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.18.3/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.155562 micrOSDevToolKit-1.18.3/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.182551 micrOSDevToolKit-1.18.3/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.3/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.3/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.185479 micrOSDevToolKit-1.18.3/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.18.3/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.244980 micrOSDevToolKit-1.18.3/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.318768 micrOSDevToolKit-1.18.3/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.18.3/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6442 2023-07-06 10:43:08.000000 micrOSDevToolKit-1.18.3/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6345 2023-07-05 20:09:42.000000 micrOSDevToolKit-1.18.3/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2047 2023-07-06 09:27:38.000000 micrOSDevToolKit-1.18.3/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7073 2023-07-14 17:40:17.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-14 17:20:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.18.3/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.18.3/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.18.3/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-07-12 17:38:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-14 17:39:42.000000 micrOSDevToolKit-1.18.3/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.18.3/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/TinyPLed.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.335583 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     6020 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Common.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5582 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5406 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Debug.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2010 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Hooks.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5232 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterConnect.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8402 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4715 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1705 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1901 2023-07-01 19:35:59.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8842 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_system.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4265 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6294 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4498 2023-07-13 18:33:20.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Scheduler.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8881 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/SocketServer.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)    15234 2023-07-13 18:33:20.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TaskManager.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5912 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Time.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      833 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2139 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOS.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     3684 2023-07-01 19:15:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     3355 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/urequests.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.18.3/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-06 11:13:33.000000 micrOSDevToolKit-1.18.3/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/pycallgraph.png
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.18.3/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.18.3/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.338931 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     9782 2023-07-14 17:47:50.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-14 17:47:50.459508 micrOSDevToolKit-1.18.3/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-14 17:36:01.000000 micrOSDevToolKit-1.18.3/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.348049 micrOSDevToolKit-1.18.3/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.18.3/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.367305 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.373632 micrOSDevToolKit-1.18.3/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.18.3/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.18.3/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.18.3/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.18.3/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.387964 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.421403 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-04 22:40:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6512 2023-07-04 22:40:18.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.18.3/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.422417 micrOSDevToolKit-1.18.3/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.457111 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1835 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3072 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1947 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      780 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2225 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4183 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2155 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4282 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3632 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3412 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3807 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5485 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2742 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1250 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1742 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1450 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.18.1/PKG-INFO` & `micrOSDevToolKit-1.18.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.18.1
+Version: 1.18.3
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.18.1/README.md` & `micrOSDevToolKit-1.18.3/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/devToolKit.py` & `micrOSDevToolKit-1.18.3/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/media/dnd.png` & `micrOSDevToolKit-1.18.3/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/media/logo.png` & `micrOSDevToolKit-1.18.3/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/media/logo_mini.png` & `micrOSDevToolKit-1.18.3/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.18.3/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.3/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.18.3/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Common.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.18.3/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Debug.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.18.3/micrOS/source/InterConnect.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from socket import getaddrinfo, AF_INET, SOCK_STREAM
 from re import match
 from Debug import errlog_add
 from ConfigHandler import cfgget
 from SocketServer import SocketServer
 from TaskManager import Task
 
+try:
+    from gc import collect
+except:
+    console_write("[SIMULATOR MODE GC IMPORT]")
+    from simgc import collect
+
 
 class InterCon:
     CONN_MAP = {}
     PORT = cfgget('socport')
 
     def __init__(self):
         self.reader = None
@@ -63,30 +69,30 @@
                     self.writer.close()
                     await self.writer.wait_closed()
 
             # Cache successful connection data (hostname:IP)
             if hostname is not None:
                 # In case of valid communication, store device IP; otherwise, set IP to None
                 InterCon.CONN_MAP[hostname] = None if output is None else host
-            # Successful communication: list of received lines / Failed communication: None
-            return '' if output is None else output
+            # None: ServerBusy(or \0) or Prompt mismatch (auto delete cached IP), STR: valid comm. output
+            return output
         else:
             errlog_add("[intercon][ERR] Invalid host: {}".format(host))
         return ''
 
     async def __run_command(self, cmd, hostname):
         """
         Implements receive data on open connection, command query and result collection
         :param cmd: command string to server socket shell
         :param hostname: hostname for prompt checking
+        Return None here will trigger retry mechanism... + deletes cached IP
         """
         cmd = str.encode(cmd)
         data, prompt = await self.__receive_data()
         if "Connection is busy. Bye!" in prompt:
-            SocketServer().reply_message("Try later...")
             return None
         # Compare prompt |node01 $| with hostname 'node01.local'
         if hostname is None or prompt is None or str(prompt).replace('$', '').strip() == str(hostname).split('.')[0]:
             # Run command on validated device
             self.writer.write(cmd)
             await self.writer.drain()
             data, _ = await self.__receive_data(prompt=prompt)
@@ -128,15 +134,22 @@
     Async send command wrapper for further async task integration and sync send_cmd usage (main)
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     :param com_obj: InterCon object to utilize send_cmd method and task status updates
     """
     # Send command
     with com_obj.task:
-        com_obj.task.out = await com_obj.send_cmd(host, cmd)
+        # Command send retry mechanism (retry: 3)
+        for _ in range(0, 3):
+            out = await com_obj.send_cmd(host, cmd)
+            if out is not None:
+                com_obj.task.out = out
+                break
+            await asyncio.sleep_ms(150)
+    collect()       # GC collect
     return com_obj.task.out
 
 
 def send_cmd(host, cmd):
     """
     Main wrapper of InterCon.send_cmd with
     - Intercon object creation
@@ -144,20 +157,22 @@
     - task creation
     - task creation verdict generation
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     """
     def _tagify():
         nonlocal host
+        nonlocal cmd
+        mod = cmd.split(' ')[0].strip()
         if InterCon.validate_ipv4(host):
-            return '.'.join(host.split('.')[-2:])
-        return host.replace('.local', '')
+            return f"{'.'.join(host.split('.')[-2:])}.{mod}"
+        return f"{host.replace('.local', '')}.{mod}"
 
     com_obj = InterCon()
-    tag = f"intercon.{_tagify()}"
+    tag = f"con.{_tagify()}"
     started = com_obj.task.create(callback=_send_cmd(host, cmd, com_obj), tag=tag)
     if started:
         result = {"verdict": f"Task started {host}:{cmd} -> task show {tag}", "tag": tag}
     else:
         result = {"verdict": "Task is Busy", "tag": tag}
     return result
```

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.18.3/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.18.1-0'
+    MICROS_VERSION = '1.18.2-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply_message('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.18.3/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_light_sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def illuminance():
     """
     Measure light illuminance in flux
     """
     volts = __init_tempt6000().get()['volt']
-    amps = volts / 10000.0                    # across 10,000 Ohms
+    amps = volts / 10000.0                    # across 10,000 Ohms (voltage divider circuit)
     microamps = amps * 1000000
     lux = '{:.2f}'.format(microamps * 2.0)
     return {'illuminance [lux]': lux}
 
 
 #######################
 # LM helper functions #
```

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.18.3/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Network.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Notify.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.18.3/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.18.3/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/Time.py` & `micrOSDevToolKit-1.18.3/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.18.3/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Common.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Debug.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Debug.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Hooks.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Hooks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterConnect.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterConnect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LM_system.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_system.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Network.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/SocketServer.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/SocketServer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/TaskManager.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TaskManager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 29 10:08:58 2023 UTC, .py size: 19197 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3a58 9d64 fd4a 0000  a.......:X.d.J..
+00000000: 610d 0d0a 0000 0000 6a65 a464 c94a 0000  a.......je.d.J..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6406 6c09 6d0a 5a0a 6d0b 5a0b 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6401 6408 6c0e  d.l.m.Z...d.d.l.
@@ -37,918 +37,917 @@
 00000240: 0664 0564 0684 005a 0764 0764 0884 005a  .d.d...Z.d.d...Z
 00000250: 0864 0964 0a84 005a 0964 1864 0c64 0d84  .d.d...Z.d.d.d..
 00000260: 015a 0a64 1964 0e64 0f84 015a 0b64 1064  .Z.d.d.d...Z.d.d
 00000270: 1184 005a 0c64 1264 1384 005a 0d64 1464  ...Z.d.d...Z.d.d
 00000280: 1584 005a 0e64 1664 1784 005a 0f64 0b53  ...Z.d.d...Z.d.S
 00000290: 0029 1ada 0454 6173 6b63 0100 0000 0000  .)...Taskc......
 000002a0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-000002b0: 0000 7338 0000 0074 00a0 01a1 007c 005f  ..s8...t.....|._
-000002c0: 0264 007c 005f 0364 017c 005f 0464 027c  .d.|._.d.|._.d.|
-000002d0: 005f 0564 007c 005f 0664 037c 005f 0764  ._.d.|._.d.|._.d
-000002e0: 047c 005f 0864 007c 005f 0964 0053 0029  .|._.d.|._.d.S.)
-000002f0: 054e 46e9 1400 0000 54da 0029 0ada 0761  .NF.....T..)...a
-00000300: 7379 6e63 696f da0e 6765 745f 6576 656e  syncio..get_even
-00000310: 745f 6c6f 6f70 da0b 5f54 6173 6b5f 5f6c  t_loop.._Task__l
-00000320: 6f6f 70da 0f5f 5461 736b 5f5f 6361 6c6c  oop.._Task__call
-00000330: 6261 636b da0d 5f54 6173 6b5f 5f69 6e6c  back.._Task__inl
-00000340: 6f6f 70da 0c5f 5461 736b 5f5f 736c 6565  oop.._Task__slee
-00000350: 70da 0474 6173 6bda 0464 6f6e 65da 036f  p..task..done..o
-00000360: 7574 da03 7461 67a9 01da 0473 656c 66a9  ut..tag....self.
-00000370: 0072 1900 0000 fa35 2f55 7365 7273 2f62  .r.....5/Users/b
-00000380: 6e6d 2f6d 6963 724f 532f 6d69 6372 4f53  nm/micrOS/micrOS
-00000390: 2f6d 6963 724f 532f 736f 7572 6365 2f54  /micrOS/source/T
-000003a0: 6173 6b4d 616e 6167 6572 2e70 79da 085f  askManager.py.._
-000003b0: 5f69 6e69 745f 5f20 0000 0073 1000 0000  _init__ ...s....
-000003c0: 0001 0a01 0601 0601 0601 0601 0601 0601  ................
-000003d0: 7a0d 5461 736b 2e5f 5f69 6e69 745f 5f63  z.Task.__init__c
-000003e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000003f0: 0400 0000 4300 0000 7324 0000 0074 006a  ....C...s$...t.j
-00000400: 01a0 027c 0064 01a1 027d 017c 0164 0175  ...|.d...}.|.d.u
-00000410: 0172 207c 016a 0373 2064 0253 0064 0353  .r |.j.s d.S.d.S
-00000420: 0029 047a 560a 2020 2020 2020 2020 4368  .).zV.        Ch
-00000430: 6563 6b20 7461 736b 2069 7320 6275 7379  eck task is busy
-00000440: 2062 7920 7461 6720 696e 2054 4153 4b53   by tag in TASKS
-00000450: 0a20 2020 2020 2020 202d 2065 7869 7374  .        - exist
-00000460: 7320 2b20 7275 6e6e 696e 6720 3d20 6275  s + running = bu
-00000470: 7379 0a20 2020 2020 2020 204e 5446 2904  sy.        NTF).
-00000480: 720a 0000 00da 0554 4153 4b53 da03 6765  r......TASKS..ge
-00000490: 7472 1400 0000 2902 7216 0000 0072 1300  tr....).r....r..
-000004a0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000004b0: 00da 0769 735f 6275 7379 2a00 0000 7308  ...is_busy*...s.
-000004c0: 0000 0000 060e 010e 0204 027a 0c54 6173  ...........z.Tas
-000004d0: 6b2e 6973 5f62 7573 7963 0100 0000 0000  k.is_busyc......
-000004e0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000004f0: 0000 7324 0000 0064 017c 005f 007c 006a  ..s$...d.|._.|.j
-00000500: 0174 026a 03a0 04a1 0076 0072 2074 026a  .t.j.....v.r t.j
-00000510: 037c 006a 013d 0064 0253 0029 037a 280a  .|.j.=.d.S.).z(.
-00000520: 2020 2020 2020 2020 4465 6c65 7465 2074          Delete t
-00000530: 6173 6b20 6672 6f6d 2054 4153 4b53 0a20  ask from TASKS. 
-00000540: 2020 2020 2020 2054 4e29 0572 1400 0000         TN).r....
-00000550: 7216 0000 0072 0a00 0000 721c 0000 00da  r....r....r.....
-00000560: 046b 6579 7372 1700 0000 7219 0000 0072  .keysr....r....r
-00000570: 1900 0000 721a 0000 005a 0a5f 5f74 6173  ....r....Z.__tas
-00000580: 6b5f 6465 6c37 0000 0073 0600 0000 0004  k_del7...s......
-00000590: 0601 1001 7a0f 5461 736b 2e5f 5f74 6173  ....z.Task.__tas
-000005a0: 6b5f 6465 6c63 0100 0000 0000 0000 0000  k_delc..........
-000005b0: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-000005c0: 0000 0064 017c 005f 007c 0053 0029 027a  ...d.|._.|.S.).z
-000005d0: 9a0a 2020 2020 2020 2020 5354 4152 5420  ..        START 
-000005e0: 434f 4e44 4954 494f 4e0a 2020 2020 2020  CONDITION.      
-000005f0: 2020 4865 6c70 6572 2066 756e 6374 696f    Helper functio
-00000600: 6e20 666f 7220 5461 736b 2063 7265 6174  n for Task creat
-00000610: 696f 6e20 696e 204c 6f61 6420 4d6f 6475  ion in Load Modu
-00000620: 6c65 730a 2020 2020 2020 2020 5b48 494e  les.        [HIN
-00000630: 545d 2055 7365 2070 7974 686f 6e20 7769  T] Use python wi
-00000640: 7468 2066 6561 7475 7265 2074 6f20 7574  th feature to ut
-00000650: 696c 697a 6520 7468 6973 2066 6561 7475  ilize this featu
-00000660: 7265 0a20 2020 2020 2020 2046 a901 7214  re.        F..r.
-00000670: 0000 0072 1700 0000 7219 0000 0072 1900  ...r....r....r..
-00000680: 0000 721a 0000 00da 095f 5f65 6e74 6572  ..r......__enter
-00000690: 5f5f 3f00 0000 7304 0000 0000 0606 017a  __?...s........z
-000006a0: 0e54 6173 6b2e 5f5f 656e 7465 725f 5f63  .Task.__enter__c
-000006b0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-000006c0: 0200 0000 4300 0000 730a 0000 0064 017c  ....C...s....d.|
-000006d0: 005f 0064 0253 0029 037a a30a 2020 2020  ._.d.S.).z..    
-000006e0: 2020 2020 4155 544f 4d41 5449 4320 5354      AUTOMATIC ST
-000006f0: 4f50 2043 4f4e 4449 5449 4f4e 0a20 2020  OP CONDITION.   
-00000700: 2020 2020 2048 656c 7065 7220 6675 6e63       Helper func
-00000710: 7469 6f6e 2066 6f72 2054 6173 6b20 6372  tion for Task cr
-00000720: 6561 7469 6f6e 2069 6e20 4c6f 6164 204d  eation in Load M
-00000730: 6f64 756c 6573 0a20 2020 2020 2020 205b  odules.        [
-00000740: 4849 4e54 5d20 5573 6520 7079 7468 6f6e  HINT] Use python
-00000750: 2077 6974 6820 6665 6174 7572 6520 746f   with feature to
-00000760: 2075 7469 6c69 7a65 2074 6869 7320 6665   utilize this fe
-00000770: 6174 7572 650a 2020 2020 2020 2020 544e  ature.        TN
-00000780: 7220 0000 0029 0472 1800 0000 da08 6578  r ...).r......ex
-00000790: 635f 7479 7065 da09 6578 635f 7661 6c75  c_type..exc_valu
-000007a0: 65da 0974 7261 6365 6261 636b 7219 0000  e..tracebackr...
-000007b0: 0072 1900 0000 721a 0000 00da 085f 5f65  .r....r......__e
-000007c0: 7869 745f 5f48 0000 0073 0200 0000 0006  xit__H...s......
-000007d0: 7a0d 5461 736b 2e5f 5f65 7869 745f 5f4e  z.Task.__exit__N
-000007e0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000007f0: 0003 0000 0043 0000 0073 5000 0000 7c02  .....C...sP...|.
-00000800: 6401 7500 7218 6402 7400 7401 6a02 8301  d.u.r.d.t.t.j...
-00000810: 9b00 9d02 6e02 7c02 7c00 5f03 7401 a004  ....n.|.|._.t...
-00000820: 7c00 6a03 a101 722e 6403 5300 6403 7c00  |.j...r.d.S.d.|.
-00000830: 5f05 7c00 6a06 a007 7c01 a101 7c00 5f08  _.|.j...|...|._.
-00000840: 7c00 7401 6a02 7c02 3c00 6404 5300 2905  |.t.j.|.<.d.S.).
-00000850: 7a8d 0a20 2020 2020 2020 2043 7265 6174  z..        Creat
-00000860: 6520 6173 796e 6320 7461 736b 2077 6974  e async task wit
-00000870: 6820 636f 726f 7574 696e 6520 6361 6c6c  h coroutine call
-00000880: 6261 636b 2028 6e6f 2071 7565 7565 206c  back (no queue l
-00000890: 696d 6974 2063 6865 636b 2129 0a20 2020  imit check!).   
-000008a0: 2020 2020 202d 2061 7379 6e63 2073 6f63       - async soc
-000008b0: 6b65 7420 7365 7276 6572 2074 6173 6b20  ket server task 
-000008c0: 7374 6172 740a 2020 2020 2020 2020 2d20  start.        - 
-000008d0: 6f74 6865 723f 0a20 2020 2020 2020 204e  other?.        N
-000008e0: 5a03 6169 6f46 5429 09da 036c 656e 720a  Z.aioFT)...lenr.
-000008f0: 0000 0072 1c00 0000 7216 0000 0072 1e00  ...r....r....r..
-00000900: 0000 7214 0000 0072 0f00 0000 da0b 6372  ..r....r......cr
-00000910: 6561 7465 5f74 6173 6b72 1300 0000 2903  eate_taskr....).
-00000920: 7218 0000 00da 0863 616c 6c62 6163 6b72  r......callbackr
-00000930: 1600 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000940: 0000 00da 0663 7265 6174 6550 0000 0073  .....createP...s
-00000950: 0e00 0000 0007 1e01 0c02 0403 0601 0e02  ................
-00000960: 0a01 7a0b 5461 736b 2e63 7265 6174 6563  ..z.Task.createc
-00000970: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-00000980: 0500 0000 4300 0000 7388 0000 0064 01a0  ....C...s....d..
-00000990: 007c 0164 0264 0385 0219 00a1 017c 005f  .|.d.d.......|._
-000009a0: 0174 02a0 037c 006a 01a1 0172 2464 0453  .t...|.j...r$d.S
-000009b0: 007c 017c 005f 047c 0264 0575 0072 387c  .|.|._.|.d.u.r8|
-000009c0: 006a 056e 027c 027c 005f 057c 0364 0575  .j.n.|.|._.|.d.u
-000009d0: 0072 4c7c 006a 066e 107c 0364 066b 0472  .rL|.j.n.|.d.k.r
-000009e0: 587c 036e 047c 006a 067c 005f 0664 047c  X|.n.|.j.|._.d.|
-000009f0: 005f 077c 006a 08a0 097c 00a0 0aa1 00a1  ._.|.j...|......
-00000a00: 017c 005f 0b7c 0074 026a 0c7c 006a 013c  .|._.|.t.j.|.j.<
-00000a10: 0064 0753 0029 087a fa0a 2020 2020 2020  .d.S.).z..      
-00000a20: 2020 4372 6561 7465 2061 7379 6e63 2074    Create async t
-00000a30: 6173 6b20 7769 7468 2066 756e 6374 696f  ask with functio
-00000a40: 6e20 6361 6c6c 6261 636b 2028 7769 7468  n callback (with
-00000a50: 2071 7565 7565 206c 696d 6974 2063 6865   queue limit che
-00000a60: 636b 290a 2020 2020 2020 2020 2d20 7772  ck).        - wr
-00000a70: 6170 2028 7379 6e63 2920 6675 6e63 7469  ap (sync) functi
-00000a80: 6f6e 2069 6e74 6f20 6173 796e 6320 7461  on into async ta
-00000a90: 736b 2028 7461 736b 5f77 7261 7070 6572  sk (task_wrapper
-00000aa0: 290a 2020 2020 2020 2020 2d20 6361 6c6c  ).        - call
-00000ab0: 6261 636b 3a20 3c6c 6f61 645f 6d6f 6475  back: <load_modu
-00000ac0: 6c65 3e20 3c66 756e 6374 696f 6e3e 203c  le> <function> <
-00000ad0: 7061 7261 6d3e 203c 7061 7261 6d32 3e0a  param> <param2>.
-00000ae0: 2020 2020 2020 2020 2d20 6c6f 6f70 3a20          - loop: 
-00000af0: 626f 6f6c 0a20 2020 2020 2020 202d 2073  bool.        - s
-00000b00: 6c65 6570 3a20 5b6d 735d 0a20 2020 2020  leep: [ms].     
-00000b10: 2020 20da 012e 7201 0000 00e9 0200 0000     ...r.........
-00000b20: 464e e913 0000 0054 290d da04 6a6f 696e  FN.....T)...join
-00000b30: 7216 0000 0072 0a00 0000 721e 0000 0072  r....r....r....r
-00000b40: 1000 0000 7211 0000 0072 1200 0000 7214  ....r....r....r.
-00000b50: 0000 0072 0f00 0000 7227 0000 00da 0c74  ...r....r'.....t
-00000b60: 6173 6b5f 7772 6170 7065 7272 1300 0000  ask_wrapperr....
-00000b70: 721c 0000 0029 0472 1800 0000 7228 0000  r....).r....r(..
-00000b80: 00da 046c 6f6f 70da 0573 6c65 6570 7219  ...loop..sleepr.
-00000b90: 0000 0072 1900 0000 721a 0000 00da 0963  ...r....r......c
-00000ba0: 7265 6174 655f 6c6d 6300 0000 7314 0000  reate_lmc...s...
-00000bb0: 0000 0914 010c 0204 0306 0114 0222 0206  ............."..
-00000bc0: 0212 020c 017a 0e54 6173 6b2e 6372 6561  .....z.Task.crea
-00000bd0: 7465 5f6c 6d63 0100 0000 0000 0000 0000  te_lmc..........
-00000be0: 0000 0200 0000 0a00 0000 4300 0000 73ac  ..........C...s.
-00000bf0: 0000 007a 727c 006a 0064 0175 0172 6a64  ...zr|.j.d.u.rjd
-00000c00: 027c 005f 017a 0e7c 006a 00a0 02a1 0001  .|._.z.|.j......
-00000c10: 0057 006e 3e04 0074 0379 5e01 007d 0101  .W.n>..t.y^..}..
-00000c20: 007a 2664 0374 047c 0183 016b 0372 4a74  .z&d.t.|...k.rJt
-00000c30: 0564 047c 019b 009d 0283 0101 0057 0059  .d.|.........W.Y
-00000c40: 0064 017d 017e 016e 0a64 017d 017e 0130  .d.}.~.n.d.}.~.0
-00000c50: 0030 007c 00a0 06a1 0001 006e 0657 0064  .0.|.......n.W.d
-00000c60: 0253 0057 006e 3404 0074 0379 a601 007d  .S.W.n4..t.y...}
-00000c70: 0101 007a 1c74 0564 057c 019b 009d 0283  ...z.t.d.|......
-00000c80: 0101 0057 0059 0064 017d 017e 0164 0253  ...W.Y.d.}.~.d.S
-00000c90: 0064 017d 017e 0130 0030 0064 0653 0029  .d.}.~.0.0.d.S.)
-00000ca0: 077a 280a 2020 2020 2020 2020 4361 6e63  .z(.        Canc
-00000cb0: 656c 2074 6173 6b20 282b 636c 6561 6e75  el task (+cleanu
-00000cc0: 7029 0a20 2020 2020 2020 204e 467a 1163  p).        NFz.c
-00000cd0: 616e 2774 2063 616e 6365 6c20 7365 6c66  an't cancel self
-00000ce0: 7a24 5b49 5251 206c 696d 6974 6174 696f  z$[IRQ limitatio
-00000cf0: 6e5d 2054 6173 6b20 6361 6e63 656c 2065  n] Task cancel e
-00000d00: 7272 6f72 3a20 7a17 5b45 5252 5d20 5461  rror: z.[ERR] Ta
-00000d10: 736b 206b 696c 6c20 6572 726f 723a 2054  sk kill error: T
-00000d20: 2907 7213 0000 0072 1100 0000 da06 6361  ).r....r......ca
-00000d30: 6e63 656c da09 4578 6365 7074 696f 6eda  ncel..Exception.
-00000d40: 0373 7472 7206 0000 00da 0f5f 5461 736b  .strr......_Task
-00000d50: 5f5f 7461 736b 5f64 656c 2902 7218 0000  __task_del).r...
-00000d60: 00da 0165 7219 0000 0072 1900 0000 721a  ...er....r....r.
-00000d70: 0000 0072 3200 0000 7e00 0000 731c 0000  ...r2...~...s...
-00000d80: 0000 0402 010a 0106 0102 010e 010e 010c  ................
-00000d90: 0124 010a 020a 010e 010e 0118 017a 0b54  .$...........z.T
-00000da0: 6173 6b2e 6361 6e63 656c 6301 0000 0000  ask.cancelc.....
-00000db0: 0000 0000 0000 0001 0000 0004 0000 00c3  ................
-00000dc0: 0000 0073 3600 0000 7400 a001 7c00 6a02  ...s6...t...|.j.
-00000dd0: a101 4900 6401 4800 0100 7403 7c00 6a04  ..I.d.H...t.|.j.
-00000de0: 7c00 6a05 6402 8d02 0100 7c00 6a06 7300  |.j.d.....|.j.s.
-00000df0: 712c 7100 6403 7c00 5f07 6401 5300 2904  q,q.d.|._.d.S.).
-00000e00: 6145 0100 000a 2020 2020 2020 2020 496d  aE....        Im
-00000e10: 706c 656d 656e 7473 2061 7379 6e63 2077  plements async w
-00000e20: 7261 7070 6572 2061 726f 756e 6420 4c6f  rapper around Lo
-00000e30: 6164 204d 6f64 756c 6520 6361 6c6c 0a20  ad Module call. 
-00000e40: 2020 2020 2020 202d 2073 656c 662e 5f5f         - self.__
-00000e50: 6361 6c6c 6261 636b 3a20 6c69 7374 202d  callback: list -
-00000e60: 2063 6f6e 7461 696e 7320 4c4d 2063 6f6d   contains LM com
-00000e70: 6d61 6e64 2073 7472 696e 6773 0a20 2020  mand strings.   
-00000e80: 2020 2020 202d 2073 656c 662e 5f5f 736c       - self.__sl
-00000e90: 6565 703a 206d 6169 6e20 6576 656e 7420  eep: main event 
-00000ea0: 6c6f 6f70 2066 6565 640a 2020 2020 2020  loop feed.      
-00000eb0: 2020 2d20 7365 6c66 2e5f 5f69 6e6c 6f6f    - self.__inloo
-00000ec0: 703a 206c 6d20 6361 6c6c 2074 7970 6520  p: lm call type 
-00000ed0: 2d20 6f6e 652d 7368 6f74 2028 4661 6c73  - one-shot (Fals
-00000ee0: 6529 202f 206c 6f6f 7065 6420 2854 7275  e) / looped (Tru
-00000ef0: 6529 0a20 2020 2020 2020 202d 2073 656c  e).        - sel
-00000f00: 662e 5f5f 6d73 675f 6275 663a 206c 6d20  f.__msg_buf: lm 
-00000f10: 6d73 6720 6f62 6a65 6374 2072 6564 6972  msg object redir
-00000f20: 6563 7420 746f 2076 6172 6961 626c 6520  ect to variable 
-00000f30: 2d20 7374 6f72 6520 6c6d 206f 7574 7075  - store lm outpu
-00000f40: 740a 2020 2020 2020 2020 4e29 01da 066d  t.        N)...m
-00000f50: 7367 6f62 6a54 2908 720d 0000 00da 0873  sgobjT).r......s
-00000f60: 6c65 6570 5f6d 7372 1200 0000 da0d 5f65  leep_msr......_e
-00000f70: 7865 635f 6c6d 5f63 6f72 6572 1000 0000  xec_lm_corer....
-00000f80: da0f 5f54 6173 6b5f 5f6d 7367 5f62 7566  .._Task__msg_buf
-00000f90: 6672 1100 0000 7214 0000 0072 1700 0000  fr....r....r....
-00000fa0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000fb0: 2e00 0000 9200 0000 730a 0000 0000 0912  ........s.......
-00000fc0: 0110 0106 0104 017a 1154 6173 6b2e 7461  .......z.Task.ta
-00000fd0: 736b 5f77 7261 7070 6572 6302 0000 0000  sk_wrapperc.....
-00000fe0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000ff0: 0000 0073 0a00 0000 7c01 7c00 5f00 6401  ...s....|.|._.d.
-00001000: 5300 2902 7a38 0a20 2020 2020 2020 2044  S.).z8.        D
-00001010: 756d 6d79 206d 7367 206f 626a 6563 7420  ummy msg object 
-00001020: 746f 2073 746f 7265 206f 7574 7075 7420  to store output 
-00001030: 7661 6c75 650a 2020 2020 2020 2020 4e29  value.        N)
-00001040: 0172 1500 0000 2902 7218 0000 00da 036d  .r....).r......m
-00001050: 7367 7219 0000 0072 1900 0000 721a 0000  sgr....r....r...
-00001060: 005a 0a5f 5f6d 7367 5f62 7566 66a1 0000  .Z.__msg_buff...
-00001070: 0073 0200 0000 0004 7a0f 5461 736b 2e5f  .s......z.Task._
-00001080: 5f6d 7367 5f62 7566 6663 0100 0000 0000  _msg_buffc......
-00001090: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-000010a0: 0000 730e 0000 0064 017c 005f 007c 0060  ..s....d.|._.|.`
-000010b0: 0164 0053 0029 024e 5429 0272 1400 0000  .d.S.).NT).r....
-000010c0: 7213 0000 0072 1700 0000 7219 0000 0072  r....r....r....r
-000010d0: 1900 0000 721a 0000 00da 075f 5f64 656c  ....r......__del
-000010e0: 5f5f a700 0000 7304 0000 0000 0106 017a  __....s........z
-000010f0: 0c54 6173 6b2e 5f5f 6465 6c5f 5f29 024e  .Task.__del__).N
-00001100: 4e29 034e 4e4e 2910 da08 5f5f 6e61 6d65  N).NNN)...__name
-00001110: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001120: 5f5f 7175 616c 6e61 6d65 5f5f 721c 0000  __qualname__r...
-00001130: 0072 1b00 0000 da0c 7374 6174 6963 6d65  .r......staticme
-00001140: 7468 6f64 721e 0000 0072 3500 0000 7221  thodr....r5...r!
-00001150: 0000 0072 2500 0000 7229 0000 0072 3100  ...r%...r)...r1.
-00001160: 0000 7232 0000 0072 2e00 0000 723a 0000  ..r2...r....r:..
-00001170: 0072 3c00 0000 7219 0000 0072 1900 0000  .r<...r....r....
-00001180: 7219 0000 0072 1a00 0000 720a 0000 001d  r....r....r.....
-00001190: 0000 0073 1a00 0000 0801 0402 080a 0201  ...s............
-000011a0: 0a0c 0808 0809 0808 0a13 0a1b 0814 080f  ................
-000011b0: 0806 720a 0000 0063 0000 0000 0000 0000  ..r....c........
-000011c0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-000011d0: 73ac 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000011e0: 0365 0464 0283 015a 0564 035a 0687 0066  .e.d...Z.d.Z...f
-000011f0: 0164 0464 0584 085a 0765 0864 1d64 0664  .d.d...Z.e.d.d.d
-00001200: 0784 0183 015a 0965 0864 0864 0984 0083  .....Z.e.d.d....
-00001210: 015a 0a65 0864 0a64 0b84 0083 015a 0b65  .Z.e.d.d.....Z.e
-00001220: 0864 0c64 0d84 0083 015a 0c64 1e64 0f64  .d.d.....Z.d.d.d
-00001230: 1084 015a 0d65 0864 1164 1284 0083 015a  ...Z.e.d.d.....Z
-00001240: 0e65 0864 1364 1484 0083 015a 0f65 0864  .e.d.d.....Z.e.d
-00001250: 1564 1684 0083 015a 1065 0864 1764 1884  .d.....Z.e.d.d..
-00001260: 0083 015a 1164 1964 1a84 005a 1265 0864  ...Z.d.d...Z.e.d
-00001270: 1b64 1c84 0083 015a 1387 0004 005a 1453  .d.....Z.....Z.S
-00001280: 0029 1fda 074d 616e 6167 6572 4e5a 0861  .)...ManagerNZ.a
-00001290: 696f 7175 6575 6572 0100 0000 6301 0000  ioqueuer....c...
-000012a0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000012b0: 0003 0000 0073 4e00 0000 7400 6a01 6401  .....sN...t.j.d.
-000012c0: 7500 7248 7402 8300 a003 7c00 a101 7400  u.rHt.....|...t.
-000012d0: 5f01 7404 a005 a100 7400 6a01 5f06 7400  _.t.....t.j._.t.
-000012e0: 6a01 6a06 a007 7c00 6a08 a101 0100 7400  j.j...|.j.....t.
-000012f0: 6a01 6a09 7400 a00a a100 6402 6403 8d02  j.j.t.....d.d...
-00001300: 0100 7400 6a01 5300 2904 7a74 0a20 2020  ..t.j.S.).zt.   
-00001310: 2020 2020 2053 696e 676c 6574 6f6e 2064       Singleton d
-00001320: 6573 6967 6e20 7061 7474 6572 6e0a 2020  esign pattern.  
-00001330: 2020 2020 2020 5f5f 6e65 775f 5f20 2d20        __new__ - 
-00001340: 4375 7374 6f6d 697a 6520 7468 6520 696e  Customize the in
-00001350: 7374 616e 6365 2063 7265 6174 696f 6e0a  stance creation.
-00001360: 2020 2020 2020 2020 636c 7320 2020 2020          cls     
-00001370: 2d20 636c 6173 730a 2020 2020 2020 2020  - class.        
-00001380: 4eda 0469 646c 65a9 0272 2800 0000 7216  N..idle..r(...r.
-00001390: 0000 0029 0b72 4100 0000 da12 5f4d 616e  ...).rA....._Man
-000013a0: 6167 6572 5f5f 696e 7374 616e 6365 da05  ager__instance..
-000013b0: 7375 7065 72da 075f 5f6e 6577 5f5f 720d  super..__new__r.
-000013c0: 0000 0072 0e00 0000 722f 0000 005a 1573  ...r....r/...Z.s
-000013d0: 6574 5f65 7863 6570 7469 6f6e 5f68 616e  et_exception_han
-000013e0: 646c 6572 da06 6178 6365 7074 7227 0000  dler..axceptr'..
-000013f0: 00da 0969 646c 655f 7461 736b 2901 da03  ...idle_task)...
-00001400: 636c 73a9 01da 095f 5f63 6c61 7373 5f5f  cls....__class__
-00001410: 7219 0000 0072 1a00 0000 7246 0000 00b6  r....r....rF....
-00001420: 0000 0073 0c00 0000 0006 0a02 0e02 0c01  ...s............
-00001430: 1001 1403 7a0f 4d61 6e61 6765 722e 5f5f  ....z.Manager.__
-00001440: 6e65 775f 5f63 0200 0000 0000 0000 0000  new__c..........
-00001450: 0000 0200 0000 0500 0000 4300 0000 7318  ..........C...s.
-00001460: 0000 0074 0064 017c 009b 0064 027c 019b  ...t.d.|...d.|..
-00001470: 009d 0483 0101 0064 0353 0029 047a 300a  .......d.S.).z0.
-00001480: 2020 2020 2020 2020 5365 7420 6173 2061          Set as a
-00001490: 7379 6e63 2065 7863 6570 7469 6f6e 2068  sync exception h
-000014a0: 616e 646c 6572 0a20 2020 2020 2020 207a  andler.        z
-000014b0: 115b 6169 6f5d 2065 7863 6570 7469 6f6e  .[aio] exception
-000014c0: 3a20 fa01 3a4e 2901 7206 0000 0029 0272  : ..:N).r....).r
-000014d0: 2f00 0000 da07 636f 6e74 6578 7472 1900  /.....contextr..
-000014e0: 0000 7219 0000 0072 1a00 0000 7247 0000  ..r....r....rG..
-000014f0: 00c7 0000 0073 0200 0000 0005 7a0e 4d61  .....s......z.Ma
-00001500: 6e61 6765 722e 6178 6365 7074 6300 0000  nager.axceptc...
-00001510: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00001520: 0043 0000 0073 1800 0000 7400 6401 6402  .C...s....t.d.d.
-00001530: 8400 7401 6a02 a003 a100 4400 8301 8301  ..t.j.....D.....
-00001540: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00001550: 0000 0300 0000 0400 0000 5300 0000 7322  ..........S...s"
-00001560: 0000 0067 007c 005d 1a5c 027d 017d 027c  ...g.|.].\.}.}.|
-00001570: 026a 0073 0464 007c 0176 0072 0464 0191  .j.s.d.|.v.r.d..
-00001580: 0271 0453 0029 0272 2a00 0000 e901 0000  .q.S.).r*.......
-00001590: 0072 2000 0000 2903 da02 2e30 7216 0000  .r ...)....0r...
-000015a0: 0072 1300 0000 7219 0000 0072 1900 0000  .r....r....r....
-000015b0: 721a 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-000015c0: 3ed1 0000 00f3 0000 0000 7a27 4d61 6e61  >.........z'Mana
-000015d0: 6765 722e 5f71 7565 7565 5f66 7265 652e  ger._queue_free.
-000015e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000015f0: 6d70 3e29 04da 0373 756d 720a 0000 0072  mp>)...sumr....r
-00001600: 1c00 0000 da05 6974 656d 7372 1900 0000  ......itemsr....
-00001610: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00001620: 0b5f 7175 6575 655f 6672 6565 ce00 0000  ._queue_free....
-00001630: 7302 0000 0000 037a 134d 616e 6167 6572  s......z.Manager
-00001640: 2e5f 7175 6575 655f 6672 6565 6300 0000  ._queue_freec...
-00001650: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00001660: 0043 0000 0073 2e00 0000 7400 a001 a100  .C...s....t.....
-00001670: 7400 6a02 6b05 722a 6401 7400 6a02 9b00  t.j.k.r*d.t.j...
-00001680: 9d02 7d00 7403 7c00 8301 0100 7404 7c00  ..}.t.|.....t.|.
-00001690: 8301 8201 6402 5300 2903 7a87 0a20 2020  ....d.S.).z..   
-000016a0: 2020 2020 2043 6865 636b 2074 6173 6b20       Check task 
-000016b0: 7175 6575 6520 6c69 6d69 740a 2020 2020  queue limit.    
-000016c0: 2020 2020 2d20 636f 6d70 6172 6520 7769      - compare wi
-000016d0: 7468 2061 6374 6976 6520 7275 6e6e 696e  th active runnin
-000016e0: 6720 7461 736b 7320 636f 756e 740a 2020  g tasks count.  
-000016f0: 2020 2020 2020 2d20 7768 656e 2071 7565        - when que
-00001700: 7565 2066 756c 6c20 7261 6973 6520 4578  ue full raise Ex
-00001710: 6365 7074 696f 6e21 2121 0a20 2020 2020  ception!!!.     
-00001720: 2020 207a 175b 6169 6f5d 2054 6173 6b20     z.[aio] Task 
-00001730: 7175 6575 6520 6675 6c6c 3a20 4e29 0572  queue full: N).r
-00001740: 4100 0000 7254 0000 00da 0a51 5545 5545  A...rT.....QUEUE
-00001750: 5f53 495a 4572 0600 0000 7233 0000 00a9  _SIZEr....r3....
-00001760: 0172 3b00 0000 7219 0000 0072 1900 0000  .r;...r....r....
-00001770: 721a 0000 00da 0e5f 7175 6575 655f 6c69  r......_queue_li
-00001780: 6d69 7465 72d3 0000 0073 0800 0000 0007  miter....s......
-00001790: 0e01 0c01 0801 7a16 4d61 6e61 6765 722e  ......z.Manager.
-000017a0: 5f71 7565 7565 5f6c 696d 6974 6572 6300  _queue_limiterc.
-000017b0: 0000 0000 0000 0000 0000 0007 0000 000a  ................
-000017c0: 0000 00c3 0000 0073 ce00 0000 6401 7d00  .......s....d.}.
-000017d0: 6402 7d01 7400 6a01 a002 6403 a101 7d02  d.}.t.j...d...}.
-000017e0: 6404 7c00 9b00 6405 9d03 7c02 5f03 7a6e  d.|...d...|._.zn
-000017f0: 7404 6406 7c01 8302 4400 5d16 7d03 7405  t.d.|...D.].}.t.
-00001800: a006 7c00 a101 4900 6407 4800 0100 712e  ..|...I.d.H...q.
-00001810: 712e 7407 8300 7d04 7405 a006 7c00 a101  q.t...}.t...|...
-00001820: 4900 6407 4800 0100 7408 7409 7407 8300  I.d.H...t.t.t...
-00001830: 7c04 8302 7c00 1b00 6408 1800 6409 1400  |...|...d...d...
-00001840: 8301 7d05 7408 740a 6a0b 7c05 1700 640a  ..}.t.t.j.|...d.
-00001850: 1b00 8301 740a 5f0b 7124 5700 6e32 0400  ....t._.q$W.n2..
-00001860: 740c 79c2 0100 7d06 0100 7a1a 740d 640b  t.y...}...z.t.d.
-00001870: 7c06 9b00 9d02 8301 0100 5700 5900 6407  |.........W.Y.d.
-00001880: 7d06 7e06 6e0a 6407 7d06 7e06 3000 3000  }.~.n.d.}.~.0.0.
-00001890: 640c 7c02 5f0e 6407 5300 290d 7a79 0a20  d.|._.d.S.).zy. 
-000018a0: 2020 2020 2020 2043 7265 6174 6520 4944         Create ID
-000018b0: 4c45 2074 6173 6b20 2d20 6669 7820 4952  LE task - fix IR
-000018c0: 5120 7461 736b 2073 7461 7274 0a20 2020  Q task start.   
-000018d0: 2020 2020 202d 2054 7279 2074 6f20 6d65       - Try to me
-000018e0: 6173 7572 6520 7379 7374 656d 206c 6f61  asure system loa
-000018f0: 6420 2d20 6261 7365 6420 6f6e 2069 646c  d - based on idl
-00001900: 6520 7461 736b 206c 6174 656e 6379 0a20  e task latency. 
-00001910: 2020 2020 2020 20e9 9600 0000 e906 0000         .........
-00001920: 0072 4200 0000 7a09 692e 642e 6c2e 653a  .rB...z.i.d.l.e:
-00001930: 20da 026d 7372 0100 0000 4e72 4e00 0000   ..msr....NrN...
-00001940: e964 0000 0072 2b00 0000 7a18 5b45 5252  .d...r+...z.[ERR
-00001950: 5d20 4964 6c65 2074 6173 6b20 6578 6973  ] Idle task exis
-00001960: 7473 3a20 5429 0f72 0a00 0000 721c 0000  ts: T).r....r...
-00001970: 0072 1d00 0000 7215 0000 00da 0572 616e  .r....r......ran
-00001980: 6765 720d 0000 0072 3800 0000 7208 0000  ger....r8...r...
-00001990: 00da 0369 6e74 7209 0000 0072 4100 0000  ...intr....rA...
-000019a0: da05 4f4c 4f41 4472 3300 0000 7206 0000  ..OLOADr3...r...
-000019b0: 0072 1400 0000 2907 5a09 7065 7269 6f64  .r....).Z.period
-000019c0: 5f6d 73da 0473 6b69 705a 076d 795f 7461  _ms..skipZ.my_ta
-000019d0: 736b da01 5fda 0174 5a0a 6465 6c74 615f  sk.._..tZ.delta_
-000019e0: 7261 7465 7236 0000 0072 1900 0000 7219  rater6...r....r.
-000019f0: 0000 0072 1a00 0000 7248 0000 00df 0000  ...r....rH......
-00001a00: 0073 1e00 0000 0007 0401 0401 0c01 0e01  .s..............
-00001a10: 0202 0e02 1001 0401 0601 1002 1c01 1a01  ................
-00001a20: 0e01 2401 7a11 4d61 6e61 6765 722e 6964  ..$.z.Manager.id
-00001a30: 6c65 5f74 6173 6b46 6305 0000 0000 0000  le_taskFc.......
-00001a40: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00001a50: 0073 3400 0000 7400 7c01 7401 8302 7224  .s4...t.|.t...r$
-00001a60: 7402 a003 a100 0100 7404 8300 6a05 7c01  t.......t...j.|.
-00001a70: 7c03 7c04 6401 8d03 5300 7404 8300 6a06  |.|.d...S.t...j.
-00001a80: 7c01 7c02 6402 8d02 5300 2903 7a8b 0a20  |.|.d...S.).z.. 
-00001a90: 2020 2020 2020 2050 7269 6d61 7279 2069         Primary i
-00001aa0: 6e74 6572 6661 6365 0a20 2020 2020 2020  nterface.       
-00001ab0: 2047 656e 6572 6963 2074 6173 6b20 6372   Generic task cr
-00001ac0: 6561 746f 7220 6d65 7468 6f64 0a20 2020  eator method.   
-00001ad0: 2020 2020 2020 2020 2043 7265 6174 6520           Create 
-00001ae0: 6173 796e 6320 5461 736b 2077 6974 6820  async Task with 
-00001af0: 636f 726f 7574 696e 652f 6c69 7374 286c  coroutine/list(l
-00001b00: 6d20 6361 6c6c 2920 6361 6c6c 6261 636b  m call) callback
-00001b10: 0a20 2020 2020 2020 2029 0372 2800 0000  .        ).r(...
-00001b20: 722f 0000 0072 3000 0000 7243 0000 0029  r/...r0...rC...)
-00001b30: 07da 0a69 7369 6e73 7461 6e63 65da 046c  ...isinstance..l
-00001b40: 6973 7472 4100 0000 7257 0000 0072 0a00  istrA...rW...r..
-00001b50: 0000 7231 0000 0072 2900 0000 2905 7249  ..r1...r)...).rI
-00001b60: 0000 0072 2800 0000 7216 0000 0072 2f00  ...r(...r....r/.
-00001b70: 0000 da05 6465 6c61 7972 1900 0000 7219  ....delayr....r.
-00001b80: 0000 0072 1a00 0000 7227 0000 00f9 0000  ...r....r'......
-00001b90: 0073 0800 0000 0006 0a01 0801 1201 7a13  .s............z.
-00001ba0: 4d61 6e61 6765 722e 6372 6561 7465 5f74  Manager.create_t
-00001bb0: 6173 6b63 0000 0000 0000 0000 0000 0000  askc............
-00001bc0: 0700 0000 0600 0000 4300 0000 737c 0000  ........C...s|..
-00001bd0: 0074 006a 0174 00a0 02a1 0018 007d 0064  .t.j.t.......}.d
-00001be0: 0164 027c 009b 0064 0374 006a 039b 0064  .d.|...d.t.j...d
-00001bf0: 049d 0564 0567 037d 0174 046a 05a0 06a1  ...d.g.}.t.j....
-00001c00: 0044 005d 405c 027d 027d 037c 036a 0772  .D.]@\.}.}.|.j.r
-00001c10: 4464 066e 0264 077d 0464 0864 0974 087c  Dd.n.d.}.d.d.t.|
-00001c20: 0483 0118 0014 007d 057c 049b 007c 059b  .......}.|...|..
-00001c30: 007c 029b 009d 037d 067c 01a0 097c 06a1  .|.....}.|...|..
-00001c40: 0101 0071 3274 0a7c 0183 0153 0029 0a7a  ...q2t.|...S.).z
-00001c50: 4a0a 2020 2020 2020 2020 5072 696d 6172  J.        Primar
-00001c60: 7920 696e 7465 7266 6163 650a 2020 2020  y interface.    
-00001c70: 2020 2020 2020 2020 4c69 7374 2074 6173          List tas
-00001c80: 6b73 202d 206d 6963 724f 5320 746f 7020  ks - micrOS top 
-00001c90: 3a44 0a20 2020 2020 2020 207a 152d 2d2d  :D.        z.---
-00001ca0: 2d20 6d69 6372 4f53 2020 746f 7020 2d2d  - micrOS  top --
-00001cb0: 2d2d 7a08 2371 7565 7565 3a20 7a08 2023  --z.#queue: z. #
-00001cc0: 6c6f 6164 3a20 7a02 250a 7a11 2341 6374  load: z.%.z.#Act
-00001cd0: 6976 6520 2020 2374 6173 6b49 445a 024e  ive   #taskIDZ.N
-00001ce0: 6f5a 0359 6573 fa01 20e9 0a00 0000 290b  oZ.Yes.. .....).
-00001cf0: 7241 0000 0072 5500 0000 7254 0000 0072  rA...rU...rT...r
-00001d00: 5e00 0000 720a 0000 0072 1c00 0000 7253  ^...r....r....rS
-00001d10: 0000 0072 1400 0000 7226 0000 00da 0661  ...r....r&.....a
-00001d20: 7070 656e 64da 0574 7570 6c65 2907 da01  ppend..tuple)...
-00001d30: 71da 066f 7574 7075 7472 1600 0000 7213  q..outputr....r.
-00001d40: 0000 005a 0a69 735f 7275 6e6e 696e 675a  ...Z.is_runningZ
-00001d50: 0473 7063 725a 0974 6173 6b5f 7669 6577  .spcrZ.task_view
-00001d60: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00001d70: 0a6c 6973 745f 7461 736b 7304 0100 0073  .list_tasks....s
-00001d80: 1000 0000 0006 0e01 1a01 1201 0e01 1001  ................
-00001d90: 1001 0c01 7a12 4d61 6e61 6765 722e 6c69  ....z.Manager.li
-00001da0: 7374 5f74 6173 6b73 6301 0000 0000 0000  st_tasksc.......
-00001db0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00001dc0: 0073 7e00 0000 7400 6a01 a002 7c00 6401  .s~...t.j...|.d.
-00001dd0: a102 7d01 7c01 6401 7500 7278 6700 7d02  ..}.|.d.u.rxg.}.
-00001de0: 7c00 a003 6402 a101 7d03 7400 6a01 a004  |...d...}.t.j...
-00001df0: a100 4400 5d34 7d04 7c04 a005 7c03 6403  ..D.]4}.|...|.d.
-00001e00: 1900 a101 722e 7406 7c03 8301 6404 6b04  ....r.t.|...d.k.
-00001e10: 722e 7c03 6404 1900 6405 6b02 722e 7c02  r.|.d...d.k.r.|.
-00001e20: a007 7c04 a101 0100 712e 7406 7c02 8301  ..|.....q.t.|...
-00001e30: 6403 6b02 7274 6700 5300 7c02 5300 7c00  d.k.rtg.S.|.S.|.
-00001e40: 6701 5300 2906 7a2c 4745 5420 5441 534b  g.S.).z,GET TASK
-00001e50: 2873 2920 4259 2054 4147 202d 206d 6f64  (s) BY TAG - mod
-00001e60: 756c 652e 6675 6e63 206f 7220 6d6f 6475  ule.func or modu
-00001e70: 6c65 2e2a 4e72 2a00 0000 7201 0000 0072  le.*Nr*...r....r
-00001e80: 4e00 0000 da01 2a29 0872 0a00 0000 721c  N.....*).r....r.
-00001e90: 0000 0072 1d00 0000 da05 7370 6c69 7472  ...r......splitr
-00001ea0: 1f00 0000 da0a 7374 6172 7473 7769 7468  ......startswith
-00001eb0: 7226 0000 0072 6700 0000 2905 7216 0000  r&...rg...).r...
-00001ec0: 0072 1300 0000 5a06 5f74 6173 6b73 5a09  .r....Z._tasksZ.
-00001ed0: 7461 675f 7061 7274 7372 6100 0000 7219  tag_partsra...r.
-00001ee0: 0000 0072 1900 0000 721a 0000 00da 0a5f  ...r....r......_
-00001ef0: 7061 7273 655f 7461 6713 0100 0073 1600  parse_tag....s..
-00001f00: 0000 0003 0e01 0801 0401 0a01 0e01 2601  ..............&.
-00001f10: 0c01 0c01 0401 0401 7a12 4d61 6e61 6765  ........z.Manage
-00001f20: 722e 5f70 6172 7365 5f74 6167 6301 0000  r._parse_tagc...
-00001f30: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00001f40: 0043 0000 0073 7000 0000 7400 a001 7c00  .C...sp...t...|.
-00001f50: a101 7d01 7402 7c01 8301 6401 6b02 7220  ..}.t.|...d.k.r 
-00001f60: 6402 7c00 9b00 9d02 5300 7402 7c01 8301  d.|.....S.t.|...
-00001f70: 6403 6b02 723c 7403 6a04 7c01 6401 1900  d.k.r<t.j.|.d...
-00001f80: 1900 6a05 5300 6700 7d02 7c01 4400 5d20  ..j.S.g.}.|.D.] 
-00001f90: 7d03 7c02 a006 7c03 9b00 6404 7403 6a04  }.|...|...d.t.j.
-00001fa0: 7c03 1900 6a05 9b00 9d03 a101 0100 7144  |...j.........qD
-00001fb0: 6405 a007 7c02 a101 5300 2906 7a49 0a20  d...|...S.).zI. 
-00001fc0: 2020 2020 2020 2050 7269 6d61 7279 2069         Primary i
-00001fd0: 6e74 6572 6661 6365 0a20 2020 2020 2020  nterface.       
-00001fe0: 2020 2020 2053 686f 7720 6275 6666 6572       Show buffer
-00001ff0: 6564 2074 6173 6b20 6f75 7470 7574 0a20  ed task output. 
-00002000: 2020 2020 2020 2072 0100 0000 fa0f 4e6f         r......No
-00002010: 2074 6173 6b20 666f 756e 643a 2072 4e00   task found: rN.
-00002020: 0000 fa02 3a20 da01 0a29 0872 4100 0000  ....: ...).rA...
-00002030: 726f 0000 0072 2600 0000 720a 0000 0072  ro...r&...r....r
-00002040: 1c00 0000 7215 0000 0072 6700 0000 722d  ....r....rg...r-
-00002050: 0000 0029 0472 1600 0000 da05 7461 736b  ...).r......task
-00002060: 7372 6a00 0000 7261 0000 0072 1900 0000  srj...ra...r....
-00002070: 7219 0000 0072 1a00 0000 da04 7368 6f77  r....r......show
-00002080: 2201 0000 7312 0000 0000 060a 010c 010a  "...s...........
-00002090: 010c 0110 0104 0108 011e 017a 0c4d 616e  ...........z.Man
-000020a0: 6167 6572 2e73 686f 7763 0100 0000 0000  ager.showc......
-000020b0: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
-000020c0: 0000 73a6 0000 0064 0164 0284 007d 0174  ..s....d.d...}.t
-000020d0: 00a0 017c 00a1 017d 0264 037d 0374 027c  ...|...}.d.}.t.|
-000020e0: 0283 0164 046b 0272 307c 0364 057c 009b  ...d.k.r0|.d.|..
-000020f0: 009d 0266 0253 0074 027c 0283 0164 066b  ...f.S.t.|...d.k
-00002100: 0272 6064 077c 0264 0419 009b 0064 087c  .r`d.|.d.....d.|
-00002110: 039b 009d 047d 047c 017c 0264 0419 0083  .....}.|.|.d....
-00002120: 017c 0466 0253 0067 007d 057c 0244 005d  .|.f.S.g.}.|.D.]
-00002130: 247d 067c 037c 017c 0683 014d 007d 037c  $}.|.|.|...M.}.|
-00002140: 05a0 037c 069b 0064 087c 039b 009d 03a1  ...|...d.|......
-00002150: 0101 0071 6864 0764 09a0 047c 05a1 019b  ...qhd.d...|....
-00002160: 009d 027d 047c 037c 0466 0253 0029 0a7a  ...}.|.|.f.S.).z
-00002170: 920a 2020 2020 2020 2020 5072 696d 6172  ..        Primar
-00002180: 7920 696e 7465 7266 6163 650a 2020 2020  y interface.    
-00002190: 2020 2020 4b69 6c6c 2f74 6572 6d69 6e61      Kill/termina
-000021a0: 7465 2061 7379 6e63 2074 6173 6b0a 2020  te async task.  
-000021b0: 2020 2020 2020 2d20 6279 2074 6167 3a20        - by tag: 
-000021c0: 6d6f 6475 6c65 2e66 756e 6374 696f 6e0a  module.function.
-000021d0: 2020 2020 2020 2020 2d20 6279 206b 696c          - by kil
-000021e0: 6c61 6c6c 2c20 6d6f 6475 6c65 2d74 6167  lall, module-tag
-000021f0: 3a20 6d6f 6475 6c65 2e2a 0a20 2020 2020  : module.*.     
-00002200: 2020 2063 0100 0000 0000 0000 0000 0000     c............
-00002210: 0300 0000 0a00 0000 5300 0000 735e 0000  ........S...s^..
-00002220: 0074 006a 01a0 027c 0064 00a1 027d 017a  .t.j...|.d...}.z
-00002230: 167c 0164 0075 0072 1c64 016e 067c 01a0  .|.d.u.r.d.n.|..
-00002240: 03a1 0057 0053 0004 0074 0479 5801 007d  ...W.S...t.yX..}
-00002250: 0201 007a 1c74 0564 027c 029b 009d 0283  ...z.t.d.|......
-00002260: 0101 0057 0059 0064 007d 027e 0264 0153  ...W.Y.d.}.~.d.S
-00002270: 0064 007d 027e 0230 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-00002280: 034e 467a 115b 4552 525d 2054 6173 6b20  .NFz.[ERR] Task 
-00002290: 6b69 6c6c 3a20 2906 720a 0000 0072 1c00  kill: ).r....r..
-000022a0: 0000 721d 0000 0072 3200 0000 7233 0000  ..r....r2...r3..
-000022b0: 0072 0600 0000 2903 5a04 5f74 6167 5a07  .r....).Z._tagZ.
-000022c0: 746f 5f6b 696c 6c72 3600 0000 7219 0000  to_killr6...r...
-000022d0: 0072 1900 0000 721a 0000 00da 0974 6572  .r....r......ter
-000022e0: 6d69 6e61 7465 3b01 0000 730c 0000 0000  minate;...s.....
-000022f0: 010e 0102 0116 010e 010e 017a 1f4d 616e  ...........z.Man
-00002300: 6167 6572 2e6b 696c 6c2e 3c6c 6f63 616c  ager.kill.<local
-00002310: 733e 2e74 6572 6d69 6e61 7465 5472 0100  s>.terminateTr..
-00002320: 0000 7270 0000 0072 4e00 0000 7a06 4b69  ..rp...rN...z.Ki
-00002330: 6c6c 3a20 fa01 7cfa 022c 2029 0572 4100  ll: ..|.., ).rA.
-00002340: 0000 726f 0000 0072 2600 0000 7267 0000  ..ro...r&...rg..
-00002350: 0072 2d00 0000 2907 7216 0000 0072 7500  .r-...).r....ru.
-00002360: 0000 7273 0000 00da 0573 7461 7465 723b  ..rs.....stater;
-00002370: 0000 0072 6a00 0000 da01 6b72 1900 0000  ...rj.....kr....
-00002380: 7219 0000 0072 1a00 0000 da04 6b69 6c6c  r....r......kill
-00002390: 3201 0000 731c 0000 0000 0908 090a 0104  2...s...........
-000023a0: 010c 010e 010c 0114 0110 0104 0108 010c  ................
-000023b0: 0116 0110 017a 0c4d 616e 6167 6572 2e6b  .....z.Manager.k
-000023c0: 696c 6c63 0100 0000 0000 0000 0000 0000  illc............
-000023d0: 0200 0000 0a00 0000 4300 0000 7350 0000  ........C...sP..
-000023e0: 007a 0e7c 006a 00a0 01a1 0001 0057 006e  .z.|.j.......W.n
-000023f0: 3c04 0074 0279 4a01 007d 0101 007a 2474  <..t.yJ..}...z$t
-00002400: 0364 017c 019b 009d 0283 0101 007c 006a  .d.|.........|.j
-00002410: 00a0 04a1 0001 0057 0059 0064 027d 017e  .......W.Y.d.}.~
-00002420: 016e 0a64 027d 017e 0130 0030 0064 0253  .n.d.}.~.0.0.d.S
-00002430: 0029 037a 260a 2020 2020 2020 2020 5275  .).z&.        Ru
-00002440: 6e20 6173 796e 6320 6576 656e 7420 6c6f  n async event lo
-00002450: 6f70 0a20 2020 2020 2020 207a 145b 6169  op.        z.[ai
-00002460: 6f5d 206c 6f6f 7020 7374 6f70 7065 643a  o] loop stopped:
-00002470: 204e 2905 722f 0000 00da 0b72 756e 5f66   N).r/.....run_f
-00002480: 6f72 6576 6572 7233 0000 0072 0600 0000  oreverr3...r....
-00002490: da05 636c 6f73 6529 0272 4900 0000 7236  ..close).rI...r6
-000024a0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-000024b0: 0000 727b 0000 0052 0100 0073 0a00 0000  ..r{...R...s....
-000024c0: 0004 0201 0e01 0e01 0e01 7a13 4d61 6e61  ..........z.Mana
-000024d0: 6765 722e 7275 6e5f 666f 7265 7665 7263  ger.run_foreverc
-000024e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000024f0: 0400 0000 4300 0000 7324 0000 0074 006a  ....C...s$...t.j
-00002500: 01a0 0264 0164 00a1 027d 017c 0164 0075  ...d.d...}.|.d.u
-00002510: 0072 1a64 0053 007c 007c 015f 0364 0053  .r.d.S.|.|._.d.S
-00002520: 0029 024e da06 7365 7276 6572 2904 720a  .).N..server).r.
-00002530: 0000 0072 1c00 0000 721d 0000 0072 1500  ...r....r....r..
-00002540: 0000 2902 723b 0000 005a 0b73 6572 7665  ..).r;...Z.serve
-00002550: 725f 7461 736b 7219 0000 0072 1900 0000  r_taskr....r....
-00002560: 721a 0000 00da 0f73 6572 7665 725f 7461  r......server_ta
-00002570: 736b 5f6d 7367 5c01 0000 7308 0000 0000  sk_msg\...s.....
-00002580: 020e 0108 0104 017a 174d 616e 6167 6572  .......z.Manager
-00002590: 2e73 6572 7665 725f 7461 736b 5f6d 7367  .server_task_msg
-000025a0: 2902 4e4e 2903 4e46 4e29 1572 3d00 0000  ).NN).NFN).r=...
-000025b0: 723e 0000 0072 3f00 0000 7244 0000 0072  r>...r?...rD...r
-000025c0: 0700 0000 7255 0000 0072 5e00 0000 7246  ....rU...r^...rF
-000025d0: 0000 0072 4000 0000 7247 0000 0072 5400  ...r@...rG...rT.
-000025e0: 0000 7257 0000 0072 4800 0000 7227 0000  ..rW...rH...r'..
-000025f0: 0072 6b00 0000 726f 0000 0072 7400 0000  .rk...ro...rt...
-00002600: 727a 0000 0072 7b00 0000 727e 0000 00da  rz...r{...r~....
-00002610: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7219  .__classcell__r.
-00002620: 0000 0072 1900 0000 724a 0000 0072 1a00  ...r....rJ...r..
-00002630: 0000 7241 0000 00b1 0000 0073 3000 0000  ..rA.......s0...
-00002640: 0801 0401 0801 0402 0c11 0201 0c06 0201  ................
-00002650: 0a04 0201 0a0b 0201 0a19 0a0b 0201 0a0e  ................
-00002660: 0201 0a0e 0201 0a0f 0201 0a1f 080a 0201  ................
-00002670: 7241 0000 0063 0100 0000 0000 0000 0000  rA...c..........
-00002680: 0000 0300 0000 0a00 0000 4300 0000 7392  ..........C...s.
-00002690: 0000 007a 447c 00a0 0064 01a1 0172 1257  ...zD|...d...r.W
-000026a0: 0064 0253 0064 0364 0484 007c 00a0 0164  .d.S.d.d...|...d
-000026b0: 05a1 0144 0083 0144 005d 1a7d 0174 027c  ...D...D.].}.t.|
-000026c0: 0183 0173 2674 0364 067c 019b 009d 0283  ...s&t.d.|......
-000026d0: 0101 0071 2657 006e 4804 0074 0479 8c01  ...q&W.nH..t.y..
-000026e0: 007d 0201 007a 3074 0364 077c 009b 0064  .}...z0t.d.|...d
-000026f0: 087c 029b 009d 0483 0101 0074 0564 097c  .|.........t.d.|
-00002700: 029b 009d 0283 0101 0057 0059 0064 0a7d  .........W.Y.d.}
-00002710: 027e 0264 0b53 0064 0a7d 027e 0230 0030  .~.d.S.d.}.~.0.0
-00002720: 0064 0253 0029 0c7a 790a 2020 2020 496e  .d.S.).zy.    In
-00002730: 7075 743a 2074 6173 6b73 7472 2063 6f6e  put: taskstr con
-00002740: 7461 696e 7320 4c4d 2063 616c 6c73 2073  tains LM calls s
-00002750: 6570 6172 6174 6564 2062 7920 3b0a 2020  eparated by ;.  
-00002760: 2020 5573 6564 2066 6f72 2065 7865 6375    Used for execu
-00002770: 7465 2063 6f6e 6669 6720 6361 6c6c 6261  te config callba
-00002780: 636b 2070 6172 616d 6574 6572 7320 2842  ck parameters (B
-00002790: 6f6f 7448 6f6f 6b2c 202e 2e2e 290a 2020  ootHook, ...).  
-000027a0: 2020 7a03 6e2f 6154 6301 0000 0000 0000    z.n/aTc.......
-000027b0: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
-000027c0: 0073 2600 0000 7c00 5d1e 7d01 7400 7c01  .s&...|.].}.t.|.
-000027d0: 8301 6400 6b04 7202 7c01 a001 a100 a002  ..d.k.r.|.......
-000027e0: a100 5600 0100 7102 6401 5300 2902 7201  ..V...q.d.S.).r.
-000027f0: 0000 004e 2903 7226 0000 00da 0573 7472  ...N).r&.....str
-00002800: 6970 726d 0000 0029 0272 4f00 0000 da03  iprm...).rO.....
-00002810: 636d 6472 1900 0000 7219 0000 0072 1a00  cmdr....r....r..
-00002820: 0000 da09 3c67 656e 6578 7072 3e72 0100  ....<genexpr>r..
-00002830: 0072 5100 0000 7a1f 6578 6563 5f6c 6d5f  .rQ...z.exec_lm_
-00002840: 7069 7065 2e3c 6c6f 6361 6c73 3e2e 3c67  pipe.<locals>.<g
-00002850: 656e 6578 7072 3efa 013b 7a18 7c2d 5b4c  enexpr>..;z.|-[L
-00002860: 4d2d 5049 5045 5d20 7461 736b 2065 7272  M-PIPE] task err
-00002870: 6f72 3a20 7a12 5b49 5251 2d50 4950 455d  or: z.[IRQ-PIPE]
-00002880: 2065 7272 6f72 3a20 7272 0000 007a 1a5b   error: rr...z.[
-00002890: 4552 525d 2065 7865 635f 6c6d 5f70 6970  ERR] exec_lm_pip
-000028a0: 6520 6572 726f 723a 204e 4629 0672 6e00  e error: NF).rn.
-000028b0: 0000 726d 0000 00da 0c65 7865 635f 6c6d  ..rm.....exec_lm
-000028c0: 5f63 6f72 6572 0500 0000 7233 0000 0072  _corer....r3...r
-000028d0: 0600 0000 2903 da07 7461 736b 7374 7272  ....)...taskstrr
-000028e0: 8100 0000 7236 0000 0072 1900 0000 7219  ....r6...r....r.
-000028f0: 0000 0072 1a00 0000 da0c 6578 6563 5f6c  ...r......exec_l
-00002900: 6d5f 7069 7065 6801 0000 7316 0000 0000  m_pipeh...s.....
-00002910: 0502 020a 0106 0218 0108 0114 010e 0114  ................
-00002920: 010e 0118 0172 8600 0000 6301 0000 0000  .....r....c.....
-00002930: 0000 0000 0000 0002 0000 000a 0000 0043  ...............C
-00002940: 0000 0073 4a00 0000 7a10 7400 7401 7c00  ...sJ...z.t.t.|.
-00002950: 8302 0100 5700 6401 5300 0400 7402 7944  ....W.d.S...t.yD
-00002960: 0100 7d01 0100 7a1c 7403 6402 7c01 9b00  ..}...z.t.d.|...
-00002970: 9d02 8301 0100 5700 5900 6403 7d01 7e01  ......W.Y.d.}.~.
-00002980: 6404 5300 6403 7d01 7e01 3000 3000 6403  d.S.d.}.~.0.0.d.
-00002990: 5300 2905 7a5a 0a20 2020 2057 7261 7070  S.).zZ.    Wrapp
-000029a0: 6572 2066 6f72 2065 7865 635f 6c6d 5f70  er for exec_lm_p
-000029b0: 6970 650a 2020 2020 2d20 5363 6865 6475  ipe.    - Schedu
-000029c0: 6c65 204c 4d20 6578 6563 7574 696f 6e73  le LM executions
-000029d0: 2066 726f 6d20 4952 5173 2028 6578 7449   from IRQs (extI
-000029e0: 5251 2c20 7469 6d49 5251 290a 2020 2020  RQ, timIRQ).    
-000029f0: 547a 1d65 7865 635f 6c6d 5f70 6970 655f  Tz.exec_lm_pipe_
-00002a00: 7363 6865 6475 6c65 2065 7272 6f72 3a20  schedule error: 
-00002a10: 4e46 2904 7204 0000 0072 8600 0000 7233  NF).r....r....r3
-00002a20: 0000 0072 0600 0000 2902 7285 0000 0072  ...r....).r....r
-00002a30: 3600 0000 7219 0000 0072 1900 0000 721a  6...r....r....r.
-00002a40: 0000 00da 1565 7865 635f 6c6d 5f70 6970  .....exec_lm_pip
-00002a50: 655f 7363 6865 6475 6c65 7c01 0000 730c  e_schedule|...s.
-00002a60: 0000 0000 0502 010a 0106 010e 010e 0172  ...............r
-00002a70: 8700 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00002a80: 0003 0000 0003 0000 0003 0000 0073 3400  .............s4.
-00002a90: 0000 8801 6401 7500 7210 6402 6403 8400  ....d.u.r.d.d...
-00002aa0: 8901 8700 8701 6602 6404 6405 8408 7d02  ......f.d.d...}.
-00002ab0: 7c02 8800 8301 722a 6406 5300 7400 8800  |.....r*d.S.t...
-00002ac0: 8801 8302 5300 2907 7a8b 0a20 2020 204d  ....S.).z..    M
-00002ad0: 6169 6e20 4c4d 2065 7865 6375 746f 7220  ain LM executor 
-00002ae0: 6675 6e63 7469 6f6e 2077 7261 7070 6572  function wrapper
-00002af0: 0a20 2020 202d 2068 616e 646c 6520 6173  .    - handle as
-00002b00: 796e 6320 2862 6163 6b67 726f 756e 6429  ync (background)
-00002b10: 2074 6173 6b20 6578 6563 7574 696f 6e0a   task execution.
-00002b20: 2020 2020 2d20 6861 6e64 6c65 2073 796e      - handle syn
-00002b30: 6320 7461 736b 2065 7865 6375 7469 6f6e  c task execution
-00002b40: 2028 5f65 7865 635f 6c6d 5f63 6f72 6529   (_exec_lm_core)
-00002b50: 0a20 2020 204e 6301 0000 0000 0000 0000  .    Nc.........
-00002b60: 0000 0001 0000 0001 0000 0053 0000 0073  ...........S...s
-00002b70: 0400 0000 6400 5300 2901 4e72 1900 0000  ....d.S.).Nr....
-00002b80: 7256 0000 0072 1900 0000 7219 0000 0072  rV...r....r....r
-00002b90: 1a00 0000 da08 3c6c 616d 6264 613e 9201  ......<lambda>..
-00002ba0: 0000 7251 0000 007a 1e65 7865 635f 6c6d  ..rQ...z.exec_lm
-00002bb0: 5f63 6f72 652e 3c6c 6f63 616c 733e 2e3c  _core.<locals>.<
-00002bc0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
-00002bd0: 0000 0000 0a00 0000 0a00 0000 1300 0000  ................
-00002be0: 739a 0100 0074 007c 0083 017d 0164 017c  s....t.|...}.d.|
-00002bf0: 0064 0219 006b 0272 b67c 0164 036b 0272  .d...k.r.|.d.k.r
-00002c00: 4e64 047c 0064 0519 006b 0272 4e64 06a0  Nd.|.d...k.rNd..
-00002c10: 0174 0283 00a0 03a1 00a1 017d 027c 029b  .t.........}.|..
-00002c20: 0064 069d 027d 0288 017c 0283 0101 0064  .d...}...|.....d
-00002c30: 0753 007c 0164 036b 0472 aa64 087c 0064  .S.|.d.k.r.d.|.d
-00002c40: 0519 006b 0272 8474 0283 006a 047c 0064  ...k.r.t...j.|.d
-00002c50: 0319 0064 098d 015c 027d 037d 0488 017c  ...d...\.}.}...|
-00002c60: 0483 0101 0064 0753 0064 0a7c 0064 0519  .....d.S.d.|.d..
-00002c70: 006b 0272 aa88 0174 0283 006a 057c 0064  .k.r...t...j.|.d
-00002c80: 0319 0064 098d 0183 0101 0064 0753 0088  ...d.......d.S..
-00002c90: 0164 0b83 0101 0064 0753 007c 0164 036b  .d.....d.S.|.d.k
-00002ca0: 0490 0172 9664 0c88 0064 0d19 0076 0090  ...r.d...d...v..
-00002cb0: 0172 9688 00a0 0664 0da1 017d 057c 05a0  .r.....d...}.|..
-00002cc0: 0764 0ca1 0164 036b 0272 ea64 076e 0264  .d...d.k.r.d.n.d
-00002cd0: 0e7d 067c 05a0 0864 0c64 0fa1 02a0 09a1  .}.|...d.d......
-00002ce0: 007d 077c 07a0 0aa1 0090 0172 1074 0b7c  .}.|.......r.t.|
-00002cf0: 0783 016e 0264 007d 077a 1674 0283 006a  ...n.d.}.z.t...j
-00002d00: 0c88 007c 067c 0764 108d 037d 0357 006e  ...|.|.d...}.W.n
-00002d10: 3004 0074 0d90 0179 5a01 007d 0801 007a  0..t...yZ..}...z
-00002d20: 1688 017c 0883 0101 0057 0059 0064 007d  ...|.....W.Y.d.}
-00002d30: 087e 0864 0753 0064 007d 087e 0830 0030  .~.d.S.d.}.~.0.0
-00002d40: 0064 11a0 0188 0064 0264 0385 0219 00a1  .d.....d.d......
-00002d50: 017d 097c 0390 0172 8488 0164 127c 099b  .}.|...r...d.|..
-00002d60: 009d 0283 0101 006e 0e88 017c 099b 0064  .......n...|...d
-00002d70: 139d 0283 0101 0064 0753 0064 0e53 0029  .......d.S.d.S.)
-00002d80: 144e 7213 0000 0072 0100 0000 722b 0000  .Nr....r....r+..
-00002d90: 0072 6300 0000 724e 0000 0072 7200 0000  .rc...rN...rr...
-00002da0: 5472 7a00 0000 2901 7216 0000 0072 7400  Trz...).r....rt.
-00002db0: 0000 7a41 496e 7661 6c69 6420 7461 736b  ..zAInvalid task
-00002dc0: 2063 6d64 2120 4865 6c70 3a20 7461 736b   cmd! Help: task
-00002dd0: 206c 6973 7420 2f20 6b69 6c6c 203c 7461   list / kill <ta
-00002de0: 736b 4944 3e20 2f20 7368 6f77 203c 7461  skID> / show <ta
-00002df0: 736b 4944 3efa 0126 e9ff ffff ff46 720c  skID>..&.....Fr.
-00002e00: 0000 0029 0272 2f00 0000 7264 0000 0072  ...).r/...rd...r
-00002e10: 2a00 0000 7a06 5374 6172 7420 7a08 2069  *...z.Start z. i
-00002e20: 7320 4275 7379 290e 7226 0000 0072 2d00  s Busy).r&...r-.
-00002e30: 0000 7241 0000 0072 6b00 0000 727a 0000  ..rA...rk...rz..
-00002e40: 0072 7400 0000 da03 706f 70da 0563 6f75  .rt.....pop..cou
-00002e50: 6e74 da07 7265 706c 6163 6572 8000 0000  nt..replacer....
-00002e60: da07 6973 6469 6769 7472 5d00 0000 7227  ..isdigitr]...r'
-00002e70: 0000 0072 3300 0000 290a 5a08 6d73 675f  ...r3...).Z.msg_
-00002e80: 6c69 7374 5a07 6d73 675f 6c65 6e72 7300  listZ.msg_lenrs.
-00002e90: 0000 7278 0000 0072 3b00 0000 da04 6d6f  ..rx...r;.....mo
-00002ea0: 6465 722f 0000 0072 6400 0000 7236 0000  der/...rd...r6..
-00002eb0: 0072 1600 0000 a902 da08 6172 675f 6c69  .r........arg_li
-00002ec0: 7374 7237 0000 0072 1900 0000 721a 0000  str7...r....r...
-00002ed0: 00da 0c74 6173 6b5f 6d61 6e61 6765 7294  ...task_manager.
-00002ee0: 0100 0073 4200 0000 0001 0802 0c02 1401  ...sB...........
-00002ef0: 1001 0a01 0801 0402 0801 0c01 1601 0801  ................
-00002f00: 0401 0c01 1601 0401 0801 0402 1802 0a01  ................
-00002f10: 1601 1001 1602 0201 1601 1001 0802 1801  ................
-00002f20: 1201 0601 1002 0e02 0402 7a22 6578 6563  ..........z"exec
-00002f30: 5f6c 6d5f 636f 7265 2e3c 6c6f 6361 6c73  _lm_core.<locals
-00002f40: 3e2e 7461 736b 5f6d 616e 6167 6572 5429  >.task_managerT)
-00002f50: 0172 3900 0000 2903 7291 0000 0072 3700  .r9...).r....r7.
-00002f60: 0000 7292 0000 0072 1900 0000 7290 0000  ..r....r....r...
-00002f70: 0072 1a00 0000 7284 0000 0089 0100 0073  .r....r........s
-00002f80: 0c00 0000 0008 0801 0802 0e2f 0801 0402  .........../....
-00002f90: 7284 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00002fa0: 0000 0a00 0000 0a00 0000 0300 0000 73d0  ..............s.
-00002fb0: 0100 0064 0164 0284 007d 0287 0066 0164  ...d.d...}...f.d
-00002fc0: 0364 0484 087d 037c 0064 0519 0064 066b  .d...}.|.d...d.k
-00002fd0: 027d 047c 0472 307c 0064 0764 0585 0219  .}.|.r0|.d.d....
-00002fe0: 006e 027c 007d 0574 007c 0583 0164 086b  .n.|.}.t.|...d.k
-00002ff0: 0590 0172 bc64 097c 0564 0719 009b 009d  ...r.d.|.d......
-00003000: 027c 0564 0a19 007c 0264 0ba0 017c 0564  .|.d...|.d...|.d
-00003010: 0864 0c85 0219 00a1 0183 0103 0002 007d  .d.............}
-00003020: 067d 077d 087a ca7c 0674 0276 0172 8a74  .}.}.z.|.t.v.r.t
-00003030: 0364 0d7c 069b 009d 0283 0101 007a 1e74  .d.|.........z.t
-00003040: 047c 069b 0064 0e7c 079b 0064 0f7c 089b  .|...d.|...d.|..
-00003050: 0064 109d 0683 0189 0057 006e 7604 0074  .d.......W.nv..t
-00003060: 0590 0179 1e01 007d 0901 007a 5c7c 0674  ...y...}...z\|.t
-00003070: 067c 0983 0176 0090 0172 0274 0764 117c  .|...v...r.t.d.|
-00003080: 069b 0064 129d 0383 0101 0074 0364 0d7c  ...d.......t.d.|
-00003090: 069b 009d 0283 0101 0074 047c 069b 0064  .........t.|...d
-000030a0: 0e7c 079b 0064 0f7c 089b 0064 109d 0683  .|...d.|...d....
-000030b0: 0189 006e 0874 057c 0983 0182 0157 0059  ...n.t.|.....W.Y
-000030c0: 0064 0c7d 097e 096e 0a64 0c7d 097e 0930  .d.}.~.n.d.}.~.0
-000030d0: 0030 007c 037c 047c 0788 0083 0389 007c  .0.|.|.|.......|
-000030e0: 0174 0688 0083 0183 0101 0057 0064 1353  .t.........W.d.S
-000030f0: 0004 0074 0590 0179 ba01 007d 0901 007a  ...t...y...}...z
-00003100: 647c 0164 147c 069b 0064 157c 079b 0064  d|.d.|...d.|...d
-00003110: 167c 099b 009d 0683 0101 0064 1774 067c  .|.........d.t.|
-00003120: 0983 0176 0090 0173 8464 1874 067c 0983  ...v...s.d.t.|..
-00003130: 0176 0090 0172 a67c 0674 02a0 08a1 0076  .v...r.|.t.....v
-00003140: 0090 0172 9874 027c 063d 0057 0059 0064  ...r.t.|.=.W.Y.d
-00003150: 0c7d 097e 0964 1953 0057 0059 0064 0c7d  .}.~.d.S.W.Y.d.}
-00003160: 097e 096e 0a64 0c7d 097e 0930 0030 007c  .~.n.d.}.~.0.0.|
-00003170: 0164 1a83 0101 007c 0164 1b83 0101 0064  .d.....|.d.....d
-00003180: 1353 0029 1c7a e30a 2020 2020 4d41 494e  .S.).z..    MAIN
-00003190: 2046 554e 4354 494f 4e20 544f 2052 554e   FUNCTION TO RUN
-000031a0: 2053 5452 494e 4720 4d4f 4455 4c45 2e46   STRING MODULE.F
-000031b0: 554e 4354 494f 4e20 4558 4543 5554 494f  UNCTION EXECUTIO
-000031c0: 4e53 0a20 2020 205b 315d 206d 6f64 756c  NS.    [1] modul
-000031d0: 6520 6e61 6d65 2028 4c4d 290a 2020 2020  e name (LM).    
-000031e0: 5b32 5d20 6675 6e63 7469 6f6e 0a20 2020  [2] function.   
-000031f0: 205b 332e 2e2e 5d20 7061 7261 6d65 7465   [3...] paramete
-00003200: 7273 2028 7365 7061 7261 746f 723a 2073  rs (separator: s
-00003210: 7061 6365 290a 2020 2020 4e4f 5445 3a20  pace).    NOTE: 
-00003220: 6d73 676f 626a 202d 206d 7573 7420 6265  msgobj - must be
-00003230: 2061 2066 756e 6374 696f 6e20 7769 7468   a function with
-00003240: 206f 6e65 2069 6e70 7574 2070 6172 616d   one input param
-00003250: 2028 7374 646f 7574 2f66 696c 652f 7374   (stdout/file/st
-00003260: 7265 616d 290a 2020 2020 6301 0000 0000  ream).    c.....
-00003270: 0000 0000 0000 0003 0000 0005 0000 0013  ................
-00003280: 0000 0073 8000 0000 6400 7d01 6401 8800  ...s....d.}.d...
-00003290: 7600 7314 6402 8800 7600 725c 6403 6404  v.s.d...v.r\d.d.
-000032a0: 8400 7400 8800 8301 4400 8301 8901 8700  ..t.....D.......
-000032b0: 8701 6602 6405 6404 8408 7401 6406 7402  ..f.d.d...t.d.t.
-000032c0: 8801 8301 6407 8303 4400 8301 7d01 7c01  ....d...D...}.|.
-000032d0: 4400 5d10 7d02 8800 a003 7c02 6408 a102  D.].}.....|.d...
-000032e0: 8900 714a 8800 a003 6409 640a a102 8900  ..qJ....d.d.....
-000032f0: 7404 7c01 7405 8302 727c 8800 6a06 7c01  t.|.t...r|..j.|.
-00003300: 8e00 8900 8800 5300 290b 4efa 0127 fa01  ......S.).N..'..
-00003310: 2263 0100 0000 0000 0000 0000 0000 0300  "c..............
-00003320: 0000 0400 0000 5300 0000 7324 0000 0067  ......S...s$...g
-00003330: 007c 005d 1c5c 027d 017d 027c 0264 006b  .|.].\.}.}.|.d.k
-00003340: 0273 1c7c 0264 016b 0272 047c 0191 0271  .s.|.d.k.r.|...q
-00003350: 0453 0029 0272 9400 0000 7293 0000 0072  .S.).r....r....r
-00003360: 1900 0000 2903 724f 0000 00da 0169 da01  ....).rO.....i..
-00003370: 6372 1900 0000 7219 0000 0072 1a00 0000  cr....r....r....
-00003380: 7250 0000 00d5 0100 0072 5100 0000 7a3d  rP.......rQ...z=
-00003390: 5f65 7865 635f 6c6d 5f63 6f72 652e 3c6c  _exec_lm_core.<l
-000033a0: 6f63 616c 733e 2e5f 5f63 6f6e 765f 6675  ocals>.__conv_fu
-000033b0: 6e63 5f70 6172 616d 732e 3c6c 6f63 616c  nc_params.<local
-000033c0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-000033d0: 0000 0000 0000 0000 0000 0200 0000 0700  ................
-000033e0: 0000 1300 0000 7328 0000 0067 007c 005d  ......s(...g.|.]
-000033f0: 207d 0188 0088 017c 0119 0088 017c 0164   }.....|.....|.d
-00003400: 0017 0019 0064 0017 0085 0219 0091 0271  .....d.........q
-00003410: 0453 0029 0172 4e00 0000 7219 0000 0029  .S.).rN...r....)
-00003420: 0272 4f00 0000 5a05 7374 725f 69a9 02da  .rO...Z.str_i...
-00003430: 0570 6172 616d 5a09 7374 725f 696e 6465  .paramZ.str_inde
-00003440: 7872 1900 0000 721a 0000 0072 5000 0000  xr....r....rP...
-00003450: d601 0000 7251 0000 0072 0100 0000 722b  ....rQ...r....r+
-00003460: 0000 007a 027b 7d72 6500 0000 7277 0000  ...z.{}re...rw..
-00003470: 0029 07da 0965 6e75 6d65 7261 7465 725c  .)...enumerater\
-00003480: 0000 0072 2600 0000 728d 0000 0072 6200  ...r&...r....rb.
-00003490: 0000 7263 0000 00da 0666 6f72 6d61 7429  ..rc.....format)
-000034a0: 0372 9800 0000 da03 6275 665a 0673 7562  .r......bufZ.sub
-000034b0: 7374 7272 1900 0000 7297 0000 0072 1a00  strr....r....r..
-000034c0: 0000 da12 5f5f 636f 6e76 5f66 756e 635f  ....__conv_func_
-000034d0: 7061 7261 6d73 d201 0000 7314 0000 0000  params....s.....
-000034e0: 0104 0110 0112 0120 0108 010e 010c 010a  ....... ........
-000034f0: 010a 017a 295f 6578 6563 5f6c 6d5f 636f  ...z)_exec_lm_co
-00003500: 7265 2e3c 6c6f 6361 6c73 3e2e 5f5f 636f  re.<locals>.__co
-00003510: 6e76 5f66 756e 635f 7061 7261 6d73 6303  nv_func_paramsc.
-00003520: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00003530: 0000 0013 0000 0073 5a00 0000 7400 7c02  .......sZ...t.|.
-00003540: 7401 8302 722e 7c00 7216 7402 7c02 8301  t...r.|.r.t.|...
-00003550: 5300 6401 a003 6402 6403 8400 8800 a004  S.d...d.d.......
-00003560: a100 4400 8301 a101 5300 7c01 6404 6b02  ..D.....S.|.d.k.
-00003570: 7256 7c00 7242 7402 7c02 8301 5300 6401  rV|.rBt.|...S.d.
-00003580: a003 6405 6403 8400 7c02 4400 8301 a101  ..d.d...|.D.....
-00003590: 5300 7c02 5300 2906 4e72 7200 0000 6301  S.|.S.).Nrr...c.
-000035a0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-000035b0: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
-000035c0: 5d18 5c02 7d01 7d02 6400 7c01 9b00 6401  ].\.}.}.d.|...d.
-000035d0: 7c02 9b00 9d04 9102 7104 5300 2902 7265  |.......q.S.).re
-000035e0: 0000 0072 7100 0000 7219 0000 0029 0372  ...rq...r....).r
-000035f0: 4f00 0000 da03 6b65 79da 0576 616c 7565  O.....key..value
-00003600: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00003610: 5000 0000 e401 0000 7251 0000 007a 375f  P.......rQ...z7_
-00003620: 6578 6563 5f6c 6d5f 636f 7265 2e3c 6c6f  exec_lm_core.<lo
-00003630: 6361 6c73 3e2e 5f5f 666f 726d 6174 5f6f  cals>.__format_o
-00003640: 7574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ut.<locals>.<lis
-00003650: 7463 6f6d 703e da04 6865 6c70 6301 0000  tcomp>..helpc...
-00003660: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00003670: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-00003680: 7d01 6400 7c01 9b00 6401 9d03 9102 7104  }.d.|...d.....q.
-00003690: 5300 2902 7265 0000 00fa 012c 7219 0000  S.).re.....,r...
-000036a0: 0029 0272 4f00 0000 7215 0000 0072 1900  .).rO...r....r..
-000036b0: 0000 7219 0000 0072 1a00 0000 7250 0000  ..r....r....rP..
-000036c0: 00ea 0100 0072 5100 0000 2905 7262 0000  .....rQ...).rb..
-000036d0: 00da 0464 6963 7472 0300 0000 722d 0000  ...dictr....r-..
-000036e0: 0072 5300 0000 2903 da09 6a73 6f6e 5f6d  .rS...)...json_m
-000036f0: 6f64 65da 076c 6d5f 6675 6e63 726a 0000  ode..lm_funcrj..
-00003700: 00a9 015a 096c 6d5f 6f75 7470 7574 7219  ...Z.lm_outputr.
-00003710: 0000 0072 1a00 0000 da0c 5f5f 666f 726d  ...r......__form
-00003720: 6174 5f6f 7574 df01 0000 7312 0000 0000  at_out....s.....
-00003730: 010a 0104 0108 0218 0208 0104 0108 0214  ................
-00003740: 017a 235f 6578 6563 5f6c 6d5f 636f 7265  .z#_exec_lm_core
-00003750: 2e3c 6c6f 6361 6c73 3e2e 5f5f 666f 726d  .<locals>.__form
-00003760: 6174 5f6f 7574 728a 0000 007a 053e 6a73  at_outr....z.>js
-00003770: 6f6e 7201 0000 0072 2b00 0000 5a03 4c4d  onr....r+...Z.LM
-00003780: 5f72 4e00 0000 7265 0000 004e 7a07 696d  _rN...re...Nz.im
-00003790: 706f 7274 2072 2a00 0000 fa01 28fa 0129  port r*.....(..)
-000037a0: 7a18 5f65 7865 635f 6c6d 5f63 6f72 6520  z._exec_lm_core 
-000037b0: 7265 2d69 6d70 6f72 7420 fa01 2154 7a0d  re-import ..!Tz.
-000037c0: 6578 6563 5f6c 6d5f 636f 7265 207a 022d  exec_lm_core z.-
-000037d0: 3e72 7100 0000 7a18 6d65 6d6f 7279 2061  >rq...z.memory a
-000037e0: 6c6c 6f63 6174 696f 6e20 6661 696c 6564  llocation failed
-000037f0: 7a0e 6973 206e 6f74 2064 6566 696e 6564  z.is not defined
-00003800: 467a 3453 4845 4c4c 3a20 7479 7065 2068  Fz4SHELL: type h
-00003810: 656c 7020 666f 7220 7369 6e67 6c65 2077  elp for single w
-00003820: 6f72 6420 636f 6d6d 616e 6473 2028 6275  ord commands (bu
-00003830: 696c 742d 696e 297a 4353 4845 4c4c 3a20  ilt-in)zCSHELL: 
-00003840: 666f 7220 4c4d 2065 7865 633a 205b 315d  for LM exec: [1]
-00003850: 284c 4d29 6d6f 6475 6c65 205b 325d 6675  (LM)module [2]fu
-00003860: 6e63 7469 6f6e 205b 332e 2e2e 5d6f 7074  nction [3...]opt
-00003870: 696f 6e61 6c20 7061 7261 6d73 2909 7226  ional params).r&
-00003880: 0000 0072 2d00 0000 7202 0000 00da 0465  ...r-...r......e
-00003890: 7865 63da 0465 7661 6c72 3300 0000 7234  xec..evalr3...r4
-000038a0: 0000 0072 0600 0000 721f 0000 0029 0a72  ...r....r....).r
-000038b0: 9100 0000 7237 0000 0072 9c00 0000 72a5  ....r7...r....r.
-000038c0: 0000 0072 a200 0000 5a08 636d 645f 6c69  ...r....Z.cmd_li
-000038d0: 7374 5a06 6c6d 5f6d 6f64 72a3 0000 005a  stZ.lm_modr....Z
-000038e0: 096c 6d5f 7061 7261 6d73 7236 0000 0072  .lm_paramsr6...r
-000038f0: 1900 0000 72a4 0000 0072 1a00 0000 7239  ....r....r....r9
-00003900: 0000 00c9 0100 0073 3a00 0000 0009 080d  .......s:.......
-00003910: 0c0f 0c01 1402 0e01 3001 0203 0801 0e01  ........0.......
-00003920: 0202 1e01 1002 0e01 1002 0e02 1c02 1e03  ................
-00003930: 0c02 0c01 0602 1001 1a01 1c02 0e01 0602  ................
-00003940: 2401 0801 0802 7239 0000 0063 0100 0000  $.....r9...c....
-00003950: 0000 0000 0000 0000 0200 0000 0a00 0000  ................
-00003960: 4300 0000 7350 0000 007a 1074 0074 017c  C...sP...z.t.t.|
-00003970: 0083 0201 0057 0064 0153 0004 0074 0279  .....W.d.S...t.y
-00003980: 4a01 007d 0101 007a 2274 0364 027c 009b  J..}...z"t.d.|..
-00003990: 0064 037c 019b 009d 0483 0101 0057 0059  .d.|.........W.Y
-000039a0: 0064 047d 017e 0164 0553 0064 047d 017e  .d.}.~.d.S.d.}.~
-000039b0: 0130 0030 0064 0453 0029 067a 740a 2020  .0.0.d.S.).zt.  
-000039c0: 2020 5772 6170 7065 7220 666f 7220 6578    Wrapper for ex
-000039d0: 6563 5f6c 6d5f 636f 7265 2066 6f72 2053  ec_lm_core for S
-000039e0: 6368 6564 756c 6572 0a20 2020 202d 206d  cheduler.    - m
-000039f0: 6963 726f 7079 7468 6f6e 2073 6368 6564  icropython sched
-00003a00: 756c 696e 670a 2020 2020 2020 2020 2d20  uling.        - 
-00003a10: 6578 6563 2070 726f 7465 6374 696f 6e20  exec protection 
-00003a20: 666f 7220 6372 6f6e 2049 5251 0a20 2020  for cron IRQ.   
-00003a30: 2054 7a11 7363 6865 6475 6c65 5f6c 6d5f   Tz.schedule_lm_
-00003a40: 6578 6563 207a 0820 6572 726f 723a 204e  exec z. error: N
-00003a50: 4629 0472 0400 0000 7284 0000 0072 3300  F).r....r....r3.
-00003a60: 0000 7206 0000 0029 0272 9100 0000 7236  ..r....).r....r6
-00003a70: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00003a80: 0000 da15 6578 6563 5f6c 6d5f 636f 7265  ....exec_lm_core
-00003a90: 5f73 6368 6564 756c 651a 0200 0073 0c00  _schedule....s..
-00003aa0: 0000 0006 0201 0a01 0601 0e01 1401 72ab  ..............r.
-00003ab0: 0000 0029 014e 2918 da07 5f5f 646f 635f  ...).N)...__doc_
-00003ac0: 5fda 0373 7973 7202 0000 005a 046a 736f  _..sysr....Z.jso
-00003ad0: 6e72 0300 0000 5a0b 6d69 6372 6f70 7974  nr....Z.micropyt
-00003ae0: 686f 6e72 0400 0000 5a08 7561 7379 6e63  honr....Z.uasync
-00003af0: 696f 720d 0000 00da 0544 6562 7567 7205  ior......Debugr.
-00003b00: 0000 0072 0600 0000 da0d 436f 6e66 6967  ...r......Config
-00003b10: 4861 6e64 6c65 7272 0700 0000 da05 7574  Handlerr......ut
-00003b20: 696d 6572 0800 0000 7209 0000 0072 0a00  imer....r....r..
-00003b30: 0000 7241 0000 0072 8600 0000 7287 0000  ..rA...r....r...
-00003b40: 0072 8400 0000 7239 0000 0072 ab00 0000  .r....r9...r....
-00003b50: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00003b60: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00003b70: 0000 7320 0000 0004 0e0c 010c 010c 0108  ..s ............
-00003b80: 0110 010c 0110 080e 7f00 150e 7f00 3808  ..............8.
-00003b90: 1408 0d0a 4008 51                        ....@.Q
+000002b0: 0000 732e 0000 0064 007c 005f 0064 017c  ..s....d.|._.d.|
+000002c0: 005f 0164 027c 005f 0264 007c 005f 0364  ._.d.|._.d.|._.d
+000002d0: 037c 005f 0464 047c 005f 0564 007c 005f  .|._.d.|._.d.|._
+000002e0: 0664 0053 0029 054e 46e9 1400 0000 54da  .d.S.).NF.....T.
+000002f0: 0029 07da 0f5f 5461 736b 5f5f 6361 6c6c  .)..._Task__call
+00000300: 6261 636b da0d 5f54 6173 6b5f 5f69 6e6c  back.._Task__inl
+00000310: 6f6f 70da 0c5f 5461 736b 5f5f 736c 6565  oop.._Task__slee
+00000320: 70da 0474 6173 6bda 0464 6f6e 65da 036f  p..task..done..o
+00000330: 7574 da03 7461 67a9 01da 0473 656c 66a9  ut..tag....self.
+00000340: 0072 1600 0000 fa35 2f55 7365 7273 2f62  .r.....5/Users/b
+00000350: 6e6d 2f6d 6963 724f 532f 6d69 6372 4f53  nm/micrOS/micrOS
+00000360: 2f6d 6963 724f 532f 736f 7572 6365 2f54  /micrOS/source/T
+00000370: 6173 6b4d 616e 6167 6572 2e70 79da 085f  askManager.py.._
+00000380: 5f69 6e69 745f 5f20 0000 0073 0e00 0000  _init__ ...s....
+00000390: 0001 0601 0601 0601 0601 0601 0601 7a0d  ..............z.
+000003a0: 5461 736b 2e5f 5f69 6e69 745f 5f63 0100  Task.__init__c..
+000003b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000003c0: 0000 4300 0000 7324 0000 0074 006a 01a0  ..C...s$...t.j..
+000003d0: 027c 0064 01a1 027d 017c 0164 0175 0172  .|.d...}.|.d.u.r
+000003e0: 207c 016a 0373 2064 0253 0064 0353 0029   |.j.s d.S.d.S.)
+000003f0: 047a 560a 2020 2020 2020 2020 4368 6563  .zV.        Chec
+00000400: 6b20 7461 736b 2069 7320 6275 7379 2062  k task is busy b
+00000410: 7920 7461 6720 696e 2054 4153 4b53 0a20  y tag in TASKS. 
+00000420: 2020 2020 2020 202d 2065 7869 7374 7320         - exists 
+00000430: 2b20 7275 6e6e 696e 6720 3d20 6275 7379  + running = busy
+00000440: 0a20 2020 2020 2020 204e 5446 2904 720a  .        NTF).r.
+00000450: 0000 00da 0554 4153 4b53 da03 6765 7472  .....TASKS..getr
+00000460: 1100 0000 2902 7213 0000 0072 1000 0000  ....).r....r....
+00000470: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00000480: 0769 735f 6275 7379 2900 0000 7308 0000  .is_busy)...s...
+00000490: 0000 060e 010e 0204 027a 0c54 6173 6b2e  .........z.Task.
+000004a0: 6973 5f62 7573 7963 0100 0000 0000 0000  is_busyc........
+000004b0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000004c0: 7324 0000 0064 017c 005f 007c 006a 0174  s$...d.|._.|.j.t
+000004d0: 026a 03a0 04a1 0076 0072 2074 026a 037c  .j.....v.r t.j.|
+000004e0: 006a 013d 0064 0253 0029 037a 280a 2020  .j.=.d.S.).z(.  
+000004f0: 2020 2020 2020 4465 6c65 7465 2074 6173        Delete tas
+00000500: 6b20 6672 6f6d 2054 4153 4b53 0a20 2020  k from TASKS.   
+00000510: 2020 2020 2054 4e29 0572 1100 0000 7213       TN).r....r.
+00000520: 0000 0072 0a00 0000 7219 0000 00da 046b  ...r....r......k
+00000530: 6579 7372 1400 0000 7216 0000 0072 1600  eysr....r....r..
+00000540: 0000 7217 0000 005a 0a5f 5f74 6173 6b5f  ..r....Z.__task_
+00000550: 6465 6c36 0000 0073 0600 0000 0004 0601  del6...s........
+00000560: 1001 7a0f 5461 736b 2e5f 5f74 6173 6b5f  ..z.Task.__task_
+00000570: 6465 6c63 0100 0000 0000 0000 0000 0000  delc............
+00000580: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00000590: 0064 017c 005f 007c 0053 0029 027a 9a0a  .d.|._.|.S.).z..
+000005a0: 2020 2020 2020 2020 5354 4152 5420 434f          START CO
+000005b0: 4e44 4954 494f 4e0a 2020 2020 2020 2020  NDITION.        
+000005c0: 4865 6c70 6572 2066 756e 6374 696f 6e20  Helper function 
+000005d0: 666f 7220 5461 736b 2063 7265 6174 696f  for Task creatio
+000005e0: 6e20 696e 204c 6f61 6420 4d6f 6475 6c65  n in Load Module
+000005f0: 730a 2020 2020 2020 2020 5b48 494e 545d  s.        [HINT]
+00000600: 2055 7365 2070 7974 686f 6e20 7769 7468   Use python with
+00000610: 2066 6561 7475 7265 2074 6f20 7574 696c   feature to util
+00000620: 697a 6520 7468 6973 2066 6561 7475 7265  ize this feature
+00000630: 0a20 2020 2020 2020 2046 a901 7211 0000  .        F..r...
+00000640: 0072 1400 0000 7216 0000 0072 1600 0000  .r....r....r....
+00000650: 7217 0000 00da 095f 5f65 6e74 6572 5f5f  r......__enter__
+00000660: 3e00 0000 7304 0000 0000 0606 017a 0e54  >...s........z.T
+00000670: 6173 6b2e 5f5f 656e 7465 725f 5f63 0400  ask.__enter__c..
+00000680: 0000 0000 0000 0000 0000 0400 0000 0200  ................
+00000690: 0000 4300 0000 730a 0000 0064 017c 005f  ..C...s....d.|._
+000006a0: 0064 0253 0029 037a a30a 2020 2020 2020  .d.S.).z..      
+000006b0: 2020 4155 544f 4d41 5449 4320 5354 4f50    AUTOMATIC STOP
+000006c0: 2043 4f4e 4449 5449 4f4e 0a20 2020 2020   CONDITION.     
+000006d0: 2020 2048 656c 7065 7220 6675 6e63 7469     Helper functi
+000006e0: 6f6e 2066 6f72 2054 6173 6b20 6372 6561  on for Task crea
+000006f0: 7469 6f6e 2069 6e20 4c6f 6164 204d 6f64  tion in Load Mod
+00000700: 756c 6573 0a20 2020 2020 2020 205b 4849  ules.        [HI
+00000710: 4e54 5d20 5573 6520 7079 7468 6f6e 2077  NT] Use python w
+00000720: 6974 6820 6665 6174 7572 6520 746f 2075  ith feature to u
+00000730: 7469 6c69 7a65 2074 6869 7320 6665 6174  tilize this feat
+00000740: 7572 650a 2020 2020 2020 2020 544e 721d  ure.        TNr.
+00000750: 0000 0029 0472 1500 0000 da08 6578 635f  ...).r......exc_
+00000760: 7479 7065 da09 6578 635f 7661 6c75 65da  type..exc_value.
+00000770: 0974 7261 6365 6261 636b 7216 0000 0072  .tracebackr....r
+00000780: 1600 0000 7217 0000 00da 085f 5f65 7869  ....r......__exi
+00000790: 745f 5f47 0000 0073 0200 0000 0006 7a0d  t__G...s......z.
+000007a0: 5461 736b 2e5f 5f65 7869 745f 5f4e 6303  Task.__exit__Nc.
+000007b0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000007c0: 0000 0043 0000 0073 5200 0000 7c02 6401  ...C...sR...|.d.
+000007d0: 7500 7218 6402 7400 7401 6a02 8301 9b00  u.r.d.t.t.j.....
+000007e0: 9d02 6e02 7c02 7c00 5f03 7401 a004 7c00  ..n.|.|._.t...|.
+000007f0: 6a03 a101 722e 6403 5300 6403 7c00 5f05  j...r.d.S.d.|._.
+00000800: 7406 a007 a100 a008 7c01 a101 7c00 5f09  t.......|...|._.
+00000810: 7c00 7401 6a02 7c02 3c00 6404 5300 2905  |.t.j.|.<.d.S.).
+00000820: 7a8d 0a20 2020 2020 2020 2043 7265 6174  z..        Creat
+00000830: 6520 6173 796e 6320 7461 736b 2077 6974  e async task wit
+00000840: 6820 636f 726f 7574 696e 6520 6361 6c6c  h coroutine call
+00000850: 6261 636b 2028 6e6f 2071 7565 7565 206c  back (no queue l
+00000860: 696d 6974 2063 6865 636b 2129 0a20 2020  imit check!).   
+00000870: 2020 2020 202d 2061 7379 6e63 2073 6f63       - async soc
+00000880: 6b65 7420 7365 7276 6572 2074 6173 6b20  ket server task 
+00000890: 7374 6172 740a 2020 2020 2020 2020 2d20  start.        - 
+000008a0: 6f74 6865 723f 0a20 2020 2020 2020 204e  other?.        N
+000008b0: 5a03 6169 6f46 5429 0ada 036c 656e 720a  Z.aioFT)...lenr.
+000008c0: 0000 0072 1900 0000 7213 0000 0072 1b00  ...r....r....r..
+000008d0: 0000 7211 0000 00da 0761 7379 6e63 696f  ..r......asyncio
+000008e0: da0e 6765 745f 6576 656e 745f 6c6f 6f70  ..get_event_loop
+000008f0: da0b 6372 6561 7465 5f74 6173 6b72 1000  ..create_taskr..
+00000900: 0000 2903 7215 0000 00da 0863 616c 6c62  ..).r......callb
+00000910: 6163 6b72 1300 0000 7216 0000 0072 1600  ackr....r....r..
+00000920: 0000 7217 0000 00da 0663 7265 6174 654f  ..r......createO
+00000930: 0000 0073 0e00 0000 0007 1e01 0c02 0403  ...s............
+00000940: 0601 1002 0a01 7a0b 5461 736b 2e63 7265  ......z.Task.cre
+00000950: 6174 6563 0400 0000 0000 0000 0000 0000  atec............
+00000960: 0400 0000 0500 0000 4300 0000 738a 0000  ........C...s...
+00000970: 0064 01a0 007c 0164 0264 0385 0219 00a1  .d...|.d.d......
+00000980: 017c 005f 0174 02a0 037c 006a 01a1 0172  .|._.t...|.j...r
+00000990: 2464 0453 007c 017c 005f 047c 0264 0575  $d.S.|.|._.|.d.u
+000009a0: 0072 387c 006a 056e 027c 027c 005f 057c  .r8|.j.n.|.|._.|
+000009b0: 0364 0575 0072 4c7c 006a 066e 107c 0364  .d.u.rL|.j.n.|.d
+000009c0: 066b 0472 587c 036e 047c 006a 067c 005f  .k.rX|.n.|.j.|._
+000009d0: 0664 047c 005f 0774 08a0 09a1 00a0 0a7c  .d.|._.t.......|
+000009e0: 00a0 0ba1 00a1 017c 005f 0c7c 0074 026a  .......|._.|.t.j
+000009f0: 0d7c 006a 013c 0064 0753 0029 087a fa0a  .|.j.<.d.S.).z..
+00000a00: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
+00000a10: 7379 6e63 2074 6173 6b20 7769 7468 2066  sync task with f
+00000a20: 756e 6374 696f 6e20 6361 6c6c 6261 636b  unction callback
+00000a30: 2028 7769 7468 2071 7565 7565 206c 696d   (with queue lim
+00000a40: 6974 2063 6865 636b 290a 2020 2020 2020  it check).      
+00000a50: 2020 2d20 7772 6170 2028 7379 6e63 2920    - wrap (sync) 
+00000a60: 6675 6e63 7469 6f6e 2069 6e74 6f20 6173  function into as
+00000a70: 796e 6320 7461 736b 2028 7461 736b 5f77  ync task (task_w
+00000a80: 7261 7070 6572 290a 2020 2020 2020 2020  rapper).        
+00000a90: 2d20 6361 6c6c 6261 636b 3a20 3c6c 6f61  - callback: <loa
+00000aa0: 645f 6d6f 6475 6c65 3e20 3c66 756e 6374  d_module> <funct
+00000ab0: 696f 6e3e 203c 7061 7261 6d3e 203c 7061  ion> <param> <pa
+00000ac0: 7261 6d32 3e0a 2020 2020 2020 2020 2d20  ram2>.        - 
+00000ad0: 6c6f 6f70 3a20 626f 6f6c 0a20 2020 2020  loop: bool.     
+00000ae0: 2020 202d 2073 6c65 6570 3a20 5b6d 735d     - sleep: [ms]
+00000af0: 0a20 2020 2020 2020 20da 012e 7201 0000  .        ...r...
+00000b00: 00e9 0200 0000 464e e913 0000 0054 290e  ......FN.....T).
+00000b10: da04 6a6f 696e 7213 0000 0072 0a00 0000  ..joinr....r....
+00000b20: 721b 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000b30: 0f00 0000 7211 0000 0072 2400 0000 7225  ....r....r$...r%
+00000b40: 0000 0072 2600 0000 da0c 7461 736b 5f77  ...r&.....task_w
+00000b50: 7261 7070 6572 7210 0000 0072 1900 0000  rapperr....r....
+00000b60: 2904 7215 0000 0072 2700 0000 da04 6c6f  ).r....r'.....lo
+00000b70: 6f70 da05 736c 6565 7072 1600 0000 7216  op..sleepr....r.
+00000b80: 0000 0072 1700 0000 da09 6372 6561 7465  ...r......create
+00000b90: 5f6c 6d62 0000 0073 1400 0000 0009 1401  _lmb...s........
+00000ba0: 0c02 0403 0601 1402 2202 0602 1402 0c01  ........".......
+00000bb0: 7a0e 5461 736b 2e63 7265 6174 655f 6c6d  z.Task.create_lm
+00000bc0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000bd0: 000a 0000 0043 0000 0073 ac00 0000 7a72  .....C...s....zr
+00000be0: 7c00 6a00 6401 7501 726a 6402 7c00 5f01  |.j.d.u.rjd.|._.
+00000bf0: 7a0e 7c00 6a00 a002 a100 0100 5700 6e3e  z.|.j.......W.n>
+00000c00: 0400 7403 795e 0100 7d01 0100 7a26 6403  ..t.y^..}...z&d.
+00000c10: 7404 7c01 8301 6b03 724a 7405 6404 7c01  t.|...k.rJt.d.|.
+00000c20: 9b00 9d02 8301 0100 5700 5900 6401 7d01  ........W.Y.d.}.
+00000c30: 7e01 6e0a 6401 7d01 7e01 3000 3000 7c00  ~.n.d.}.~.0.0.|.
+00000c40: a006 a100 0100 6e06 5700 6402 5300 5700  ......n.W.d.S.W.
+00000c50: 6e34 0400 7403 79a6 0100 7d01 0100 7a1c  n4..t.y...}...z.
+00000c60: 7405 6405 7c01 9b00 9d02 8301 0100 5700  t.d.|.........W.
+00000c70: 5900 6401 7d01 7e01 6402 5300 6401 7d01  Y.d.}.~.d.S.d.}.
+00000c80: 7e01 3000 3000 6406 5300 2907 7a28 0a20  ~.0.0.d.S.).z(. 
+00000c90: 2020 2020 2020 2043 616e 6365 6c20 7461         Cancel ta
+00000ca0: 736b 2028 2b63 6c65 616e 7570 290a 2020  sk (+cleanup).  
+00000cb0: 2020 2020 2020 4e46 7a11 6361 6e27 7420        NFz.can't 
+00000cc0: 6361 6e63 656c 2073 656c 667a 245b 4952  cancel selfz$[IR
+00000cd0: 5120 6c69 6d69 7461 7469 6f6e 5d20 5461  Q limitation] Ta
+00000ce0: 736b 2063 616e 6365 6c20 6572 726f 723a  sk cancel error:
+00000cf0: 207a 175b 4552 525d 2054 6173 6b20 6b69   z.[ERR] Task ki
+00000d00: 6c6c 2065 7272 6f72 3a20 5429 0772 1000  ll error: T).r..
+00000d10: 0000 720e 0000 00da 0663 616e 6365 6cda  ..r......cancel.
+00000d20: 0945 7863 6570 7469 6f6e da03 7374 7272  .Exception..strr
+00000d30: 0600 0000 da0f 5f54 6173 6b5f 5f74 6173  ......_Task__tas
+00000d40: 6b5f 6465 6c29 0272 1500 0000 da01 6572  k_del).r......er
+00000d50: 1600 0000 7216 0000 0072 1700 0000 7231  ....r....r....r1
+00000d60: 0000 007d 0000 0073 1c00 0000 0004 0201  ...}...s........
+00000d70: 0a01 0601 0201 0e01 0e01 0c01 2401 0a02  ............$...
+00000d80: 0a01 0e01 0e01 1801 7a0b 5461 736b 2e63  ........z.Task.c
+00000d90: 616e 6365 6c63 0100 0000 0000 0000 0000  ancelc..........
+00000da0: 0000 0100 0000 0400 0000 c300 0000 7336  ..............s6
+00000db0: 0000 0074 00a0 017c 006a 02a1 0149 0064  ...t...|.j...I.d
+00000dc0: 0148 0001 0074 037c 006a 047c 006a 0564  .H...t.|.j.|.j.d
+00000dd0: 028d 0201 007c 006a 0673 0071 2c71 0064  .....|.j.s.q,q.d
+00000de0: 037c 005f 0764 0153 0029 0461 4501 0000  .|._.d.S.).aE...
+00000df0: 0a20 2020 2020 2020 2049 6d70 6c65 6d65  .        Impleme
+00000e00: 6e74 7320 6173 796e 6320 7772 6170 7065  nts async wrappe
+00000e10: 7220 6172 6f75 6e64 204c 6f61 6420 4d6f  r around Load Mo
+00000e20: 6475 6c65 2063 616c 6c0a 2020 2020 2020  dule call.      
+00000e30: 2020 2d20 7365 6c66 2e5f 5f63 616c 6c62    - self.__callb
+00000e40: 6163 6b3a 206c 6973 7420 2d20 636f 6e74  ack: list - cont
+00000e50: 6169 6e73 204c 4d20 636f 6d6d 616e 6420  ains LM command 
+00000e60: 7374 7269 6e67 730a 2020 2020 2020 2020  strings.        
+00000e70: 2d20 7365 6c66 2e5f 5f73 6c65 6570 3a20  - self.__sleep: 
+00000e80: 6d61 696e 2065 7665 6e74 206c 6f6f 7020  main event loop 
+00000e90: 6665 6564 0a20 2020 2020 2020 202d 2073  feed.        - s
+00000ea0: 656c 662e 5f5f 696e 6c6f 6f70 3a20 6c6d  elf.__inloop: lm
+00000eb0: 2063 616c 6c20 7479 7065 202d 206f 6e65   call type - one
+00000ec0: 2d73 686f 7420 2846 616c 7365 2920 2f20  -shot (False) / 
+00000ed0: 6c6f 6f70 6564 2028 5472 7565 290a 2020  looped (True).  
+00000ee0: 2020 2020 2020 2d20 7365 6c66 2e5f 5f6d        - self.__m
+00000ef0: 7367 5f62 7566 3a20 6c6d 206d 7367 206f  sg_buf: lm msg o
+00000f00: 626a 6563 7420 7265 6469 7265 6374 2074  bject redirect t
+00000f10: 6f20 7661 7269 6162 6c65 202d 2073 746f  o variable - sto
+00000f20: 7265 206c 6d20 6f75 7470 7574 0a20 2020  re lm output.   
+00000f30: 2020 2020 204e 2901 da06 6d73 676f 626a       N)...msgobj
+00000f40: 5429 0872 2400 0000 da08 736c 6565 705f  T).r$.....sleep_
+00000f50: 6d73 720f 0000 00da 0d5f 6578 6563 5f6c  msr......_exec_l
+00000f60: 6d5f 636f 7265 720d 0000 00da 0f5f 5461  m_corer......_Ta
+00000f70: 736b 5f5f 6d73 675f 6275 6666 720e 0000  sk__msg_buffr...
+00000f80: 0072 1100 0000 7214 0000 0072 1600 0000  .r....r....r....
+00000f90: 7216 0000 0072 1700 0000 722d 0000 0091  r....r....r-....
+00000fa0: 0000 0073 0a00 0000 0009 1201 1001 0601  ...s............
+00000fb0: 0401 7a11 5461 736b 2e74 6173 6b5f 7772  ..z.Task.task_wr
+00000fc0: 6170 7065 7263 0200 0000 0000 0000 0000  apperc..........
+00000fd0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000fe0: 0000 007c 017c 005f 0064 0153 0029 027a  ...|.|._.d.S.).z
+00000ff0: 380a 2020 2020 2020 2020 4475 6d6d 7920  8.        Dummy 
+00001000: 6d73 6720 6f62 6a65 6374 2074 6f20 7374  msg object to st
+00001010: 6f72 6520 6f75 7470 7574 2076 616c 7565  ore output value
+00001020: 0a20 2020 2020 2020 204e 2901 7212 0000  .        N).r...
+00001030: 0029 0272 1500 0000 da03 6d73 6772 1600  .).r......msgr..
+00001040: 0000 7216 0000 0072 1700 0000 5a0a 5f5f  ..r....r....Z.__
+00001050: 6d73 675f 6275 6666 a000 0000 7302 0000  msg_buff....s...
+00001060: 0000 047a 0f54 6173 6b2e 5f5f 6d73 675f  ...z.Task.__msg_
+00001070: 6275 6666 6301 0000 0000 0000 0000 0000  buffc...........
+00001080: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
+00001090: 0000 6401 7c00 5f00 7c00 6001 6400 5300  ..d.|._.|.`.d.S.
+000010a0: 2902 4e54 2902 7211 0000 0072 1000 0000  ).NT).r....r....
+000010b0: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000010c0: 1700 0000 da07 5f5f 6465 6c5f 5fa6 0000  ......__del__...
+000010d0: 0073 0400 0000 0001 0601 7a0c 5461 736b  .s........z.Task
+000010e0: 2e5f 5f64 656c 5f5f 2902 4e4e 2903 4e4e  .__del__).NN).NN
+000010f0: 4e29 10da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00001100: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001110: 6c6e 616d 655f 5f72 1900 0000 7218 0000  lname__r....r...
+00001120: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
+00001130: 1b00 0000 7234 0000 0072 1e00 0000 7222  ....r4...r....r"
+00001140: 0000 0072 2800 0000 7230 0000 0072 3100  ...r(...r0...r1.
+00001150: 0000 722d 0000 0072 3900 0000 723b 0000  ..r-...r9...r;..
+00001160: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
+00001170: 7217 0000 0072 0a00 0000 1d00 0000 731a  r....r........s.
+00001180: 0000 0008 0104 0208 0902 010a 0c08 0808  ................
+00001190: 0908 080a 130a 1b08 1408 0f08 0672 0a00  .............r..
+000011a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000011b0: 0000 0004 0000 0000 0000 0073 ac00 0000  ...........s....
+000011c0: 6500 5a01 6400 5a02 6401 5a03 6504 6402  e.Z.d.Z.d.Z.e.d.
+000011d0: 8301 5a05 6403 5a06 8700 6601 6404 6405  ..Z.d.Z...f.d.d.
+000011e0: 8408 5a07 6508 641d 6406 6407 8401 8301  ..Z.e.d.d.d.....
+000011f0: 5a09 6508 6408 6409 8400 8301 5a0a 6508  Z.e.d.d.....Z.e.
+00001200: 640a 640b 8400 8301 5a0b 6508 640c 640d  d.d.....Z.e.d.d.
+00001210: 8400 8301 5a0c 641e 640f 6410 8401 5a0d  ....Z.d.d.d...Z.
+00001220: 6508 6411 6412 8400 8301 5a0e 6508 6413  e.d.d.....Z.e.d.
+00001230: 6414 8400 8301 5a0f 6508 6415 6416 8400  d.....Z.e.d.d...
+00001240: 8301 5a10 6508 6417 6418 8400 8301 5a11  ..Z.e.d.d.....Z.
+00001250: 6419 641a 8400 5a12 6508 641b 641c 8400  d.d...Z.e.d.d...
+00001260: 8301 5a13 8700 0400 5a14 5300 291f da07  ..Z.....Z.S.)...
+00001270: 4d61 6e61 6765 724e 5a08 6169 6f71 7565  ManagerNZ.aioque
+00001280: 7565 7201 0000 0063 0100 0000 0000 0000  uer....c........
+00001290: 0000 0000 0100 0000 0400 0000 0300 0000  ................
+000012a0: 734e 0000 0074 006a 0164 0175 0072 4874  sN...t.j.d.u.rHt
+000012b0: 0283 00a0 037c 00a1 0174 005f 0174 04a0  .....|...t._.t..
+000012c0: 05a1 0074 006a 015f 0674 006a 016a 06a0  ...t.j._.t.j.j..
+000012d0: 077c 006a 08a1 0101 0074 006a 016a 0974  .|.j.....t.j.j.t
+000012e0: 00a0 0aa1 0064 0264 038d 0201 0074 006a  .....d.d.....t.j
+000012f0: 0153 0029 047a 740a 2020 2020 2020 2020  .S.).zt.        
+00001300: 5369 6e67 6c65 746f 6e20 6465 7369 676e  Singleton design
+00001310: 2070 6174 7465 726e 0a20 2020 2020 2020   pattern.       
+00001320: 205f 5f6e 6577 5f5f 202d 2043 7573 746f   __new__ - Custo
+00001330: 6d69 7a65 2074 6865 2069 6e73 7461 6e63  mize the instanc
+00001340: 6520 6372 6561 7469 6f6e 0a20 2020 2020  e creation.     
+00001350: 2020 2063 6c73 2020 2020 202d 2063 6c61     cls     - cla
+00001360: 7373 0a20 2020 2020 2020 204e da04 6964  ss.        N..id
+00001370: 6c65 a902 7227 0000 0072 1300 0000 290b  le..r'...r....).
+00001380: 7240 0000 00da 125f 4d61 6e61 6765 725f  r@....._Manager_
+00001390: 5f69 6e73 7461 6e63 65da 0573 7570 6572  _instance..super
+000013a0: da07 5f5f 6e65 775f 5f72 2400 0000 7225  ..__new__r$...r%
+000013b0: 0000 0072 2e00 0000 da15 7365 745f 6578  ...r......set_ex
+000013c0: 6365 7074 696f 6e5f 6861 6e64 6c65 72da  ception_handler.
+000013d0: 0661 7863 6570 7472 2600 0000 da09 6964  .axceptr&.....id
+000013e0: 6c65 5f74 6173 6b29 01da 0363 6c73 a901  le_task)...cls..
+000013f0: da09 5f5f 636c 6173 735f 5f72 1600 0000  ..__class__r....
+00001400: 7217 0000 0072 4500 0000 b500 0000 730c  r....rE.......s.
+00001410: 0000 0000 060a 020e 020c 0110 0114 037a  ...............z
+00001420: 0f4d 616e 6167 6572 2e5f 5f6e 6577 5f5f  .Manager.__new__
+00001430: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001440: 0005 0000 0043 0000 0073 1800 0000 7400  .....C...s....t.
+00001450: 6401 7c00 9b00 6402 7c01 9b00 9d04 8301  d.|...d.|.......
+00001460: 0100 6403 5300 2904 7a30 0a20 2020 2020  ..d.S.).z0.     
+00001470: 2020 2053 6574 2061 7320 6173 796e 6320     Set as async 
+00001480: 6578 6365 7074 696f 6e20 6861 6e64 6c65  exception handle
+00001490: 720a 2020 2020 2020 2020 7a11 5b61 696f  r.        z.[aio
+000014a0: 5d20 6578 6365 7074 696f 6e3a 20fa 013a  ] exception: ..:
+000014b0: 4e29 0172 0600 0000 2902 722e 0000 00da  N).r....).r.....
+000014c0: 0763 6f6e 7465 7874 7216 0000 0072 1600  .contextr....r..
+000014d0: 0000 7217 0000 0072 4700 0000 c600 0000  ..r....rG.......
+000014e0: 7302 0000 0000 057a 0e4d 616e 6167 6572  s......z.Manager
+000014f0: 2e61 7863 6570 7463 0000 0000 0000 0000  .axceptc........
+00001500: 0000 0000 0000 0000 0400 0000 4300 0000  ............C...
+00001510: 7318 0000 0074 0064 0164 0284 0074 016a  s....t.d.d...t.j
+00001520: 02a0 03a1 0044 0083 0183 0153 0029 034e  .....D.....S.).N
+00001530: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00001540: 0004 0000 0053 0000 0073 2200 0000 6700  .....S...s"...g.
+00001550: 7c00 5d1a 5c02 7d01 7d02 7c02 6a00 7304  |.].\.}.}.|.j.s.
+00001560: 6400 7c01 7600 7204 6401 9102 7104 5300  d.|.v.r.d...q.S.
+00001570: 2902 7229 0000 00e9 0100 0000 721d 0000  ).r)........r...
+00001580: 0029 03da 022e 3072 1300 0000 7210 0000  .)....0r....r...
+00001590: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+000015a0: da0a 3c6c 6973 7463 6f6d 703e d000 0000  ..<listcomp>....
+000015b0: f300 0000 007a 274d 616e 6167 6572 2e5f  .....z'Manager._
+000015c0: 7175 6575 655f 6672 6565 2e3c 6c6f 6361  queue_free.<loca
+000015d0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2904  ls>.<listcomp>).
+000015e0: da03 7375 6d72 0a00 0000 7219 0000 00da  ..sumr....r.....
+000015f0: 0569 7465 6d73 7216 0000 0072 1600 0000  .itemsr....r....
+00001600: 7216 0000 0072 1700 0000 da0b 5f71 7565  r....r......_que
+00001610: 7565 5f66 7265 65cd 0000 0073 0200 0000  ue_free....s....
+00001620: 0003 7a13 4d61 6e61 6765 722e 5f71 7565  ..z.Manager._que
+00001630: 7565 5f66 7265 6563 0000 0000 0000 0000  ue_freec........
+00001640: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001650: 732e 0000 0074 00a0 01a1 0074 006a 026b  s....t.....t.j.k
+00001660: 0572 2a64 0174 006a 029b 009d 027d 0074  .r*d.t.j.....}.t
+00001670: 037c 0083 0101 0074 047c 0083 0182 0164  .|.....t.|.....d
+00001680: 0253 0029 037a 870a 2020 2020 2020 2020  .S.).z..        
+00001690: 4368 6563 6b20 7461 736b 2071 7565 7565  Check task queue
+000016a0: 206c 696d 6974 0a20 2020 2020 2020 202d   limit.        -
+000016b0: 2063 6f6d 7061 7265 2077 6974 6820 6163   compare with ac
+000016c0: 7469 7665 2072 756e 6e69 6e67 2074 6173  tive running tas
+000016d0: 6b73 2063 6f75 6e74 0a20 2020 2020 2020  ks count.       
+000016e0: 202d 2077 6865 6e20 7175 6575 6520 6675   - when queue fu
+000016f0: 6c6c 2072 6169 7365 2045 7863 6570 7469  ll raise Excepti
+00001700: 6f6e 2121 210a 2020 2020 2020 2020 7a17  on!!!.        z.
+00001710: 5b61 696f 5d20 5461 736b 2071 7565 7565  [aio] Task queue
+00001720: 2066 756c 6c3a 204e 2905 7240 0000 0072   full: N).r@...r
+00001730: 5400 0000 da0a 5155 4555 455f 5349 5a45  T.....QUEUE_SIZE
+00001740: 7206 0000 0072 3200 0000 a901 723a 0000  r....r2.....r:..
+00001750: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001760: da0e 5f71 7565 7565 5f6c 696d 6974 6572  .._queue_limiter
+00001770: d200 0000 7308 0000 0000 070e 010c 0108  ....s...........
+00001780: 017a 164d 616e 6167 6572 2e5f 7175 6575  .z.Manager._queu
+00001790: 655f 6c69 6d69 7465 7263 0000 0000 0000  e_limiterc......
+000017a0: 0000 0000 0000 0700 0000 0a00 0000 c300  ................
+000017b0: 0000 73ce 0000 0064 017d 0064 027d 0174  ..s....d.}.d.}.t
+000017c0: 006a 01a0 0264 03a1 017d 0264 047c 009b  .j...d...}.d.|..
+000017d0: 0064 059d 037c 025f 037a 6e74 0464 067c  .d...|._.znt.d.|
+000017e0: 0183 0244 005d 167d 0374 05a0 067c 00a1  ...D.].}.t...|..
+000017f0: 0149 0064 0748 0001 0071 2e71 2e74 0783  .I.d.H...q.q.t..
+00001800: 007d 0474 05a0 067c 00a1 0149 0064 0748  .}.t...|...I.d.H
+00001810: 0001 0074 0874 0974 0783 007c 0483 027c  ...t.t.t...|...|
+00001820: 001b 0064 0818 0064 0914 0083 017d 0574  ...d...d.....}.t
+00001830: 0874 0a6a 0b7c 0517 0064 0a1b 0083 0174  .t.j.|...d.....t
+00001840: 0a5f 0b71 2457 006e 3204 0074 0c79 c201  ._.q$W.n2..t.y..
+00001850: 007d 0601 007a 1a74 0d64 0b7c 069b 009d  .}...z.t.d.|....
+00001860: 0283 0101 0057 0059 0064 077d 067e 066e  .....W.Y.d.}.~.n
+00001870: 0a64 077d 067e 0630 0030 0064 0c7c 025f  .d.}.~.0.0.d.|._
+00001880: 0e64 0753 0029 0d7a 790a 2020 2020 2020  .d.S.).zy.      
+00001890: 2020 4372 6561 7465 2049 444c 4520 7461    Create IDLE ta
+000018a0: 736b 202d 2066 6978 2049 5251 2074 6173  sk - fix IRQ tas
+000018b0: 6b20 7374 6172 740a 2020 2020 2020 2020  k start.        
+000018c0: 2d20 5472 7920 746f 206d 6561 7375 7265  - Try to measure
+000018d0: 2073 7973 7465 6d20 6c6f 6164 202d 2062   system load - b
+000018e0: 6173 6564 206f 6e20 6964 6c65 2074 6173  ased on idle tas
+000018f0: 6b20 6c61 7465 6e63 790a 2020 2020 2020  k latency.      
+00001900: 2020 e996 0000 00e9 0600 0000 7241 0000    ..........rA..
+00001910: 007a 0969 2e64 2e6c 2e65 3a20 5a02 6d73  .z.i.d.l.e: Z.ms
+00001920: 7201 0000 004e 724e 0000 00e9 6400 0000  r....NrN....d...
+00001930: 722a 0000 007a 185b 4552 525d 2049 646c  r*...z.[ERR] Idl
+00001940: 6520 7461 736b 2065 7869 7374 733a 2054  e task exists: T
+00001950: 290f 720a 0000 0072 1900 0000 721a 0000  ).r....r....r...
+00001960: 0072 1200 0000 da05 7261 6e67 6572 2400  .r......ranger$.
+00001970: 0000 7237 0000 0072 0800 0000 da03 696e  ..r7...r......in
+00001980: 7472 0900 0000 7240 0000 00da 054f 4c4f  tr....r@.....OLO
+00001990: 4144 7232 0000 0072 0600 0000 7211 0000  ADr2...r....r...
+000019a0: 0029 075a 0970 6572 696f 645f 6d73 da04  .).Z.period_ms..
+000019b0: 736b 6970 5a07 6d79 5f74 6173 6bda 015f  skipZ.my_task.._
+000019c0: da01 745a 0a64 656c 7461 5f72 6174 6572  ..tZ.delta_rater
+000019d0: 3500 0000 7216 0000 0072 1600 0000 7217  5...r....r....r.
+000019e0: 0000 0072 4800 0000 de00 0000 731e 0000  ...rH.......s...
+000019f0: 0000 0704 0104 010c 010e 0102 020e 0210  ................
+00001a00: 0104 0106 0110 021c 011a 010e 0124 017a  .............$.z
+00001a10: 114d 616e 6167 6572 2e69 646c 655f 7461  .Manager.idle_ta
+00001a20: 736b 4663 0500 0000 0000 0000 0000 0000  skFc............
+00001a30: 0500 0000 0500 0000 4300 0000 7334 0000  ........C...s4..
+00001a40: 0074 007c 0174 0183 0272 2474 02a0 03a1  .t.|.t...r$t....
+00001a50: 0001 0074 0483 006a 057c 017c 037c 0464  ...t...j.|.|.|.d
+00001a60: 018d 0353 0074 0483 006a 067c 017c 0264  ...S.t...j.|.|.d
+00001a70: 028d 0253 0029 037a 8b0a 2020 2020 2020  ...S.).z..      
+00001a80: 2020 5072 696d 6172 7920 696e 7465 7266    Primary interf
+00001a90: 6163 650a 2020 2020 2020 2020 4765 6e65  ace.        Gene
+00001aa0: 7269 6320 7461 736b 2063 7265 6174 6f72  ric task creator
+00001ab0: 206d 6574 686f 640a 2020 2020 2020 2020   method.        
+00001ac0: 2020 2020 4372 6561 7465 2061 7379 6e63      Create async
+00001ad0: 2054 6173 6b20 7769 7468 2063 6f72 6f75   Task with corou
+00001ae0: 7469 6e65 2f6c 6973 7428 6c6d 2063 616c  tine/list(lm cal
+00001af0: 6c29 2063 616c 6c62 6163 6b0a 2020 2020  l) callback.    
+00001b00: 2020 2020 2903 7227 0000 0072 2e00 0000      ).r'...r....
+00001b10: 722f 0000 0072 4200 0000 2907 da0a 6973  r/...rB...)...is
+00001b20: 696e 7374 616e 6365 da04 6c69 7374 7240  instance..listr@
+00001b30: 0000 0072 5700 0000 720a 0000 0072 3000  ...rW...r....r0.
+00001b40: 0000 7228 0000 0029 0572 4900 0000 7227  ..r(...).rI...r'
+00001b50: 0000 0072 1300 0000 722e 0000 00da 0564  ...r....r......d
+00001b60: 656c 6179 7216 0000 0072 1600 0000 7217  elayr....r....r.
+00001b70: 0000 0072 2600 0000 f800 0000 7308 0000  ...r&.......s...
+00001b80: 0000 060a 0108 0112 017a 134d 616e 6167  .........z.Manag
+00001b90: 6572 2e63 7265 6174 655f 7461 736b 6300  er.create_taskc.
+00001ba0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00001bb0: 0000 0043 0000 0073 7c00 0000 7400 6a01  ...C...s|...t.j.
+00001bc0: 7400 a002 a100 1800 7d00 6401 6402 7c00  t.......}.d.d.|.
+00001bd0: 9b00 6403 7400 6a03 9b00 6404 9d05 6405  ..d.t.j...d...d.
+00001be0: 6703 7d01 7404 6a05 a006 a100 4400 5d40  g.}.t.j.....D.]@
+00001bf0: 5c02 7d02 7d03 7c03 6a07 7244 6406 6e02  \.}.}.|.j.rDd.n.
+00001c00: 6407 7d04 6408 6409 7408 7c04 8301 1800  d.}.d.d.t.|.....
+00001c10: 1400 7d05 7c04 9b00 7c05 9b00 7c02 9b00  ..}.|...|...|...
+00001c20: 9d03 7d06 7c01 a009 7c06 a101 0100 7132  ..}.|...|.....q2
+00001c30: 740a 7c01 8301 5300 290a 7a4a 0a20 2020  t.|...S.).zJ.   
+00001c40: 2020 2020 2050 7269 6d61 7279 2069 6e74       Primary int
+00001c50: 6572 6661 6365 0a20 2020 2020 2020 2020  erface.         
+00001c60: 2020 204c 6973 7420 7461 736b 7320 2d20     List tasks - 
+00001c70: 6d69 6372 4f53 2074 6f70 203a 440a 2020  micrOS top :D.  
+00001c80: 2020 2020 2020 7a15 2d2d 2d2d 206d 6963        z.---- mic
+00001c90: 724f 5320 2074 6f70 202d 2d2d 2d7a 0823  rOS  top ----z.#
+00001ca0: 7175 6575 653a 207a 0820 236c 6f61 643a  queue: z. #load:
+00001cb0: 207a 0225 0a7a 1123 4163 7469 7665 2020   z.%.z.#Active  
+00001cc0: 2023 7461 736b 4944 5a02 4e6f 5a03 5965   #taskIDZ.NoZ.Ye
+00001cd0: 73fa 0120 e90a 0000 0029 0b72 4000 0000  s.. .....).r@...
+00001ce0: 7255 0000 0072 5400 0000 725d 0000 0072  rU...rT...r]...r
+00001cf0: 0a00 0000 7219 0000 0072 5300 0000 7211  ....r....rS...r.
+00001d00: 0000 0072 2300 0000 da06 6170 7065 6e64  ...r#.....append
+00001d10: da05 7475 706c 6529 07da 0171 da06 6f75  ..tuple)...q..ou
+00001d20: 7470 7574 7213 0000 0072 1000 0000 da0a  tputr....r......
+00001d30: 6973 5f72 756e 6e69 6e67 5a04 7370 6372  is_runningZ.spcr
+00001d40: 5a09 7461 736b 5f76 6965 7772 1600 0000  Z.task_viewr....
+00001d50: 7216 0000 0072 1700 0000 da0a 6c69 7374  r....r......list
+00001d60: 5f74 6173 6b73 0301 0000 7310 0000 0000  _tasks....s.....
+00001d70: 060e 011a 0112 010e 0110 0110 010c 017a  ...............z
+00001d80: 124d 616e 6167 6572 2e6c 6973 745f 7461  .Manager.list_ta
+00001d90: 736b 7363 0100 0000 0000 0000 0000 0000  sksc............
+00001da0: 0500 0000 0500 0000 4300 0000 737e 0000  ........C...s~..
+00001db0: 0074 006a 01a0 027c 0064 01a1 027d 017c  .t.j...|.d...}.|
+00001dc0: 0164 0175 0072 7867 007d 027c 00a0 0364  .d.u.rxg.}.|...d
+00001dd0: 02a1 017d 0374 006a 01a0 04a1 0044 005d  ...}.t.j.....D.]
+00001de0: 347d 047c 04a0 057c 0364 0319 00a1 0172  4}.|...|.d.....r
+00001df0: 2e74 067c 0383 0164 046b 0472 2e7c 0364  .t.|...d.k.r.|.d
+00001e00: 0419 0064 056b 0272 2e7c 02a0 077c 04a1  ...d.k.r.|...|..
+00001e10: 0101 0071 2e74 067c 0283 0164 036b 0272  ...q.t.|...d.k.r
+00001e20: 7467 0053 007c 0253 007c 0067 0153 0029  tg.S.|.S.|.g.S.)
+00001e30: 067a 2c47 4554 2054 4153 4b28 7329 2042  .z,GET TASK(s) B
+00001e40: 5920 5441 4720 2d20 6d6f 6475 6c65 2e66  Y TAG - module.f
+00001e50: 756e 6320 6f72 206d 6f64 756c 652e 2a4e  unc or module.*N
+00001e60: 7229 0000 0072 0100 0000 724e 0000 00da  r)...r....rN....
+00001e70: 012a 2908 720a 0000 0072 1900 0000 721a  .*).r....r....r.
+00001e80: 0000 00da 0573 706c 6974 721c 0000 00da  .....splitr.....
+00001e90: 0a73 7461 7274 7377 6974 6872 2300 0000  .startswithr#...
+00001ea0: 7266 0000 0029 0572 1300 0000 7210 0000  rf...).r....r...
+00001eb0: 005a 065f 7461 736b 735a 0974 6167 5f70  .Z._tasksZ.tag_p
+00001ec0: 6172 7473 7260 0000 0072 1600 0000 7216  artsr`...r....r.
+00001ed0: 0000 0072 1700 0000 da0a 5f70 6172 7365  ...r......_parse
+00001ee0: 5f74 6167 1201 0000 7316 0000 0000 030e  _tag....s.......
+00001ef0: 0108 0104 010a 010e 0126 010c 010c 0104  .........&......
+00001f00: 0104 017a 124d 616e 6167 6572 2e5f 7061  ...z.Manager._pa
+00001f10: 7273 655f 7461 6763 0100 0000 0000 0000  rse_tagc........
+00001f20: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00001f30: 7370 0000 0074 00a0 017c 00a1 017d 0174  sp...t...|...}.t
+00001f40: 027c 0183 0164 016b 0272 2064 027c 009b  .|...d.k.r d.|..
+00001f50: 009d 0253 0074 027c 0183 0164 036b 0272  ...S.t.|...d.k.r
+00001f60: 3c74 036a 047c 0164 0119 0019 006a 0553  <t.j.|.d.....j.S
+00001f70: 0067 007d 027c 0144 005d 207d 037c 02a0  .g.}.|.D.] }.|..
+00001f80: 067c 039b 0064 0474 036a 047c 0319 006a  .|...d.t.j.|...j
+00001f90: 059b 009d 03a1 0101 0071 4464 05a0 077c  .........qDd...|
+00001fa0: 02a1 0153 0029 067a 490a 2020 2020 2020  ...S.).zI.      
+00001fb0: 2020 5072 696d 6172 7920 696e 7465 7266    Primary interf
+00001fc0: 6163 650a 2020 2020 2020 2020 2020 2020  ace.            
+00001fd0: 5368 6f77 2062 7566 6665 7265 6420 7461  Show buffered ta
+00001fe0: 736b 206f 7574 7075 740a 2020 2020 2020  sk output.      
+00001ff0: 2020 7201 0000 00fa 0f4e 6f20 7461 736b    r......No task
+00002000: 2066 6f75 6e64 3a20 724e 0000 00fa 023a   found: rN.....:
+00002010: 20da 010a 2908 7240 0000 0072 6f00 0000   ...).r@...ro...
+00002020: 7223 0000 0072 0a00 0000 7219 0000 0072  r#...r....r....r
+00002030: 1200 0000 7266 0000 0072 2c00 0000 2904  ....rf...r,...).
+00002040: 7213 0000 00da 0574 6173 6b73 7269 0000  r......tasksri..
+00002050: 0072 6000 0000 7216 0000 0072 1600 0000  .r`...r....r....
+00002060: 7217 0000 00da 0473 686f 7721 0100 0073  r......show!...s
+00002070: 1200 0000 0006 0a01 0c01 0a01 0c01 1001  ................
+00002080: 0401 0801 1e01 7a0c 4d61 6e61 6765 722e  ......z.Manager.
+00002090: 7368 6f77 6301 0000 0000 0000 0000 0000  showc...........
+000020a0: 0007 0000 0006 0000 0043 0000 0073 a600  .........C...s..
+000020b0: 0000 6401 6402 8400 7d01 7400 a001 7c00  ..d.d...}.t...|.
+000020c0: a101 7d02 6403 7d03 7402 7c02 8301 6404  ..}.d.}.t.|...d.
+000020d0: 6b02 7230 7c03 6405 7c00 9b00 9d02 6602  k.r0|.d.|.....f.
+000020e0: 5300 7402 7c02 8301 6406 6b02 7260 6407  S.t.|...d.k.r`d.
+000020f0: 7c02 6404 1900 9b00 6408 7c03 9b00 9d04  |.d.....d.|.....
+00002100: 7d04 7c01 7c02 6404 1900 8301 7c04 6602  }.|.|.d.....|.f.
+00002110: 5300 6700 7d05 7c02 4400 5d24 7d06 7c03  S.g.}.|.D.]$}.|.
+00002120: 7c01 7c06 8301 4d00 7d03 7c05 a003 7c06  |.|...M.}.|...|.
+00002130: 9b00 6408 7c03 9b00 9d03 a101 0100 7168  ..d.|.........qh
+00002140: 6407 6409 a004 7c05 a101 9b00 9d02 7d04  d.d...|.......}.
+00002150: 7c03 7c04 6602 5300 290a 7a92 0a20 2020  |.|.f.S.).z..   
+00002160: 2020 2020 2050 7269 6d61 7279 2069 6e74       Primary int
+00002170: 6572 6661 6365 0a20 2020 2020 2020 204b  erface.        K
+00002180: 696c 6c2f 7465 726d 696e 6174 6520 6173  ill/terminate as
+00002190: 796e 6320 7461 736b 0a20 2020 2020 2020  ync task.       
+000021a0: 202d 2062 7920 7461 673a 206d 6f64 756c   - by tag: modul
+000021b0: 652e 6675 6e63 7469 6f6e 0a20 2020 2020  e.function.     
+000021c0: 2020 202d 2062 7920 6b69 6c6c 616c 6c2c     - by killall,
+000021d0: 206d 6f64 756c 652d 7461 673a 206d 6f64   module-tag: mod
+000021e0: 756c 652e 2a0a 2020 2020 2020 2020 6301  ule.*.        c.
+000021f0: 0000 0000 0000 0000 0000 0003 0000 000a  ................
+00002200: 0000 0053 0000 0073 5e00 0000 7400 6a01  ...S...s^...t.j.
+00002210: a002 7c00 6400 a102 7d01 7a16 7c01 6400  ..|.d...}.z.|.d.
+00002220: 7500 721c 6401 6e06 7c01 a003 a100 5700  u.r.d.n.|.....W.
+00002230: 5300 0400 7404 7958 0100 7d02 0100 7a1c  S...t.yX..}...z.
+00002240: 7405 6402 7c02 9b00 9d02 8301 0100 5700  t.d.|.........W.
+00002250: 5900 6400 7d02 7e02 6401 5300 6400 7d02  Y.d.}.~.d.S.d.}.
+00002260: 7e02 3000 3000 6400 5300 2903 4e46 7a11  ~.0.0.d.S.).NFz.
+00002270: 5b45 5252 5d20 5461 736b 206b 696c 6c3a  [ERR] Task kill:
+00002280: 2029 0672 0a00 0000 7219 0000 0072 1a00   ).r....r....r..
+00002290: 0000 7231 0000 0072 3200 0000 7206 0000  ..r1...r2...r...
+000022a0: 0029 035a 045f 7461 675a 0774 6f5f 6b69  .).Z._tagZ.to_ki
+000022b0: 6c6c 7235 0000 0072 1600 0000 7216 0000  llr5...r....r...
+000022c0: 0072 1700 0000 da09 7465 726d 696e 6174  .r......terminat
+000022d0: 653a 0100 0073 0c00 0000 0001 0e01 0201  e:...s..........
+000022e0: 1601 0e01 0e01 7a1f 4d61 6e61 6765 722e  ......z.Manager.
+000022f0: 6b69 6c6c 2e3c 6c6f 6361 6c73 3e2e 7465  kill.<locals>.te
+00002300: 726d 696e 6174 6554 7201 0000 0072 7000  rminateTr....rp.
+00002310: 0000 724e 0000 007a 064b 696c 6c3a 20fa  ..rN...z.Kill: .
+00002320: 017c fa02 2c20 2905 7240 0000 0072 6f00  .|.., ).r@...ro.
+00002330: 0000 7223 0000 0072 6600 0000 722c 0000  ..r#...rf...r,..
+00002340: 0029 0772 1300 0000 7275 0000 0072 7300  .).r....ru...rs.
+00002350: 0000 da05 7374 6174 6572 3a00 0000 7269  ....stater:...ri
+00002360: 0000 00da 016b 7216 0000 0072 1600 0000  .....kr....r....
+00002370: 7217 0000 00da 046b 696c 6c31 0100 0073  r......kill1...s
+00002380: 1c00 0000 0009 0809 0a01 0401 0c01 0e01  ................
+00002390: 0c01 1401 1001 0401 0801 0c01 1601 1001  ................
+000023a0: 7a0c 4d61 6e61 6765 722e 6b69 6c6c 6301  z.Manager.killc.
+000023b0: 0000 0000 0000 0000 0000 0002 0000 000a  ................
+000023c0: 0000 0043 0000 0073 5000 0000 7a0e 7c00  ...C...sP...z.|.
+000023d0: 6a00 a001 a100 0100 5700 6e3c 0400 7402  j.......W.n<..t.
+000023e0: 794a 0100 7d01 0100 7a24 7403 6401 7c01  yJ..}...z$t.d.|.
+000023f0: 9b00 9d02 8301 0100 7c00 6a00 a004 a100  ........|.j.....
+00002400: 0100 5700 5900 6402 7d01 7e01 6e0a 6402  ..W.Y.d.}.~.n.d.
+00002410: 7d01 7e01 3000 3000 6402 5300 2903 7a26  }.~.0.0.d.S.).z&
+00002420: 0a20 2020 2020 2020 2052 756e 2061 7379  .        Run asy
+00002430: 6e63 2065 7665 6e74 206c 6f6f 700a 2020  nc event loop.  
+00002440: 2020 2020 2020 7a14 5b61 696f 5d20 6c6f        z.[aio] lo
+00002450: 6f70 2073 746f 7070 6564 3a20 4e29 0572  op stopped: N).r
+00002460: 2e00 0000 da0b 7275 6e5f 666f 7265 7665  ......run_foreve
+00002470: 7272 3200 0000 7206 0000 00da 0563 6c6f  rr2...r......clo
+00002480: 7365 2902 7249 0000 0072 3500 0000 7216  se).rI...r5...r.
+00002490: 0000 0072 1600 0000 7217 0000 0072 7b00  ...r....r....r{.
+000024a0: 0000 5101 0000 730a 0000 0000 0402 010e  ..Q...s.........
+000024b0: 010e 010e 017a 134d 616e 6167 6572 2e72  .....z.Manager.r
+000024c0: 756e 5f66 6f72 6576 6572 6301 0000 0000  un_foreverc.....
+000024d0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000024e0: 0000 0073 2400 0000 7400 6a01 a002 6401  ...s$...t.j...d.
+000024f0: 6400 a102 7d01 7c01 6400 7500 721a 6400  d...}.|.d.u.r.d.
+00002500: 5300 7c00 7c01 5f03 6400 5300 2902 4eda  S.|.|._.d.S.).N.
+00002510: 0673 6572 7665 7229 0472 0a00 0000 7219  .server).r....r.
+00002520: 0000 0072 1a00 0000 7212 0000 0029 0272  ...r....r....).r
+00002530: 3a00 0000 5a0b 7365 7276 6572 5f74 6173  :...Z.server_tas
+00002540: 6b72 1600 0000 7216 0000 0072 1700 0000  kr....r....r....
+00002550: da0f 7365 7276 6572 5f74 6173 6b5f 6d73  ..server_task_ms
+00002560: 675b 0100 0073 0800 0000 0002 0e01 0801  g[...s..........
+00002570: 0401 7a17 4d61 6e61 6765 722e 7365 7276  ..z.Manager.serv
+00002580: 6572 5f74 6173 6b5f 6d73 6729 024e 4e29  er_task_msg).NN)
+00002590: 034e 464e 2915 723c 0000 0072 3d00 0000  .NFN).r<...r=...
+000025a0: 723e 0000 0072 4300 0000 7207 0000 0072  r>...rC...r....r
+000025b0: 5500 0000 725d 0000 0072 4500 0000 723f  U...r]...rE...r?
+000025c0: 0000 0072 4700 0000 7254 0000 0072 5700  ...rG...rT...rW.
+000025d0: 0000 7248 0000 0072 2600 0000 726b 0000  ..rH...r&...rk..
+000025e0: 0072 6f00 0000 7274 0000 0072 7a00 0000  .ro...rt...rz...
+000025f0: 727b 0000 0072 7e00 0000 da0d 5f5f 636c  r{...r~.....__cl
+00002600: 6173 7363 656c 6c5f 5f72 1600 0000 7216  asscell__r....r.
+00002610: 0000 0072 4a00 0000 7217 0000 0072 4000  ...rJ...r....r@.
+00002620: 0000 b000 0000 7330 0000 0008 0104 0108  ......s0........
+00002630: 0104 020c 1102 010c 0602 010a 0402 010a  ................
+00002640: 0b02 010a 190a 0b02 010a 0e02 010a 0e02  ................
+00002650: 010a 0f02 010a 1f08 0a02 0172 4000 0000  ...........r@...
+00002660: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002670: 000a 0000 0043 0000 0073 9200 0000 7a44  .....C...s....zD
+00002680: 7c00 a000 6401 a101 7212 5700 6402 5300  |...d...r.W.d.S.
+00002690: 6403 6404 8400 7c00 a001 6405 a101 4400  d.d...|...d...D.
+000026a0: 8301 4400 5d1a 7d01 7402 7c01 8301 7326  ..D.].}.t.|...s&
+000026b0: 7403 6406 7c01 9b00 9d02 8301 0100 7126  t.d.|.........q&
+000026c0: 5700 6e48 0400 7404 798c 0100 7d02 0100  W.nH..t.y...}...
+000026d0: 7a30 7403 6407 7c00 9b00 6408 7c02 9b00  z0t.d.|...d.|...
+000026e0: 9d04 8301 0100 7405 6409 7c02 9b00 9d02  ......t.d.|.....
+000026f0: 8301 0100 5700 5900 640a 7d02 7e02 640b  ....W.Y.d.}.~.d.
+00002700: 5300 640a 7d02 7e02 3000 3000 6402 5300  S.d.}.~.0.0.d.S.
+00002710: 290c 7a79 0a20 2020 2049 6e70 7574 3a20  ).zy.    Input: 
+00002720: 7461 736b 7374 7220 636f 6e74 6169 6e73  taskstr contains
+00002730: 204c 4d20 6361 6c6c 7320 7365 7061 7261   LM calls separa
+00002740: 7465 6420 6279 203b 0a20 2020 2055 7365  ted by ;.    Use
+00002750: 6420 666f 7220 6578 6563 7574 6520 636f  d for execute co
+00002760: 6e66 6967 2063 616c 6c62 6163 6b20 7061  nfig callback pa
+00002770: 7261 6d65 7465 7273 2028 426f 6f74 486f  rameters (BootHo
+00002780: 6f6b 2c20 2e2e 2e29 0a20 2020 207a 036e  ok, ...).    z.n
+00002790: 2f61 5463 0100 0000 0000 0000 0000 0000  /aTc............
+000027a0: 0200 0000 0300 0000 7300 0000 7326 0000  ........s...s&..
+000027b0: 007c 005d 1e7d 0174 007c 0183 0164 006b  .|.].}.t.|...d.k
+000027c0: 0472 027c 01a0 01a1 00a0 02a1 0056 0001  .r.|.........V..
+000027d0: 0071 0264 0153 0029 0272 0100 0000 4e29  .q.d.S.).r....N)
+000027e0: 0372 2300 0000 da05 7374 7269 7072 6d00  .r#.....striprm.
+000027f0: 0000 2902 724f 0000 00da 0363 6d64 7216  ..).rO.....cmdr.
+00002800: 0000 0072 1600 0000 7217 0000 00da 093c  ...r....r......<
+00002810: 6765 6e65 7870 723e 7101 0000 7251 0000  genexpr>q...rQ..
+00002820: 007a 1f65 7865 635f 6c6d 5f70 6970 652e  .z.exec_lm_pipe.
+00002830: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00002840: 723e fa01 3b7a 187c 2d5b 4c4d 2d50 4950  r>..;z.|-[LM-PIP
+00002850: 455d 2074 6173 6b20 6572 726f 723a 207a  E] task error: z
+00002860: 125b 4952 512d 5049 5045 5d20 6572 726f  .[IRQ-PIPE] erro
+00002870: 723a 2072 7200 0000 7a1a 5b45 5252 5d20  r: rr...z.[ERR] 
+00002880: 6578 6563 5f6c 6d5f 7069 7065 2065 7272  exec_lm_pipe err
+00002890: 6f72 3a20 4e46 2906 726e 0000 0072 6d00  or: NF).rn...rm.
+000028a0: 0000 da0c 6578 6563 5f6c 6d5f 636f 7265  ....exec_lm_core
+000028b0: 7205 0000 0072 3200 0000 7206 0000 0029  r....r2...r....)
+000028c0: 03da 0774 6173 6b73 7472 7281 0000 0072  ...taskstrr....r
+000028d0: 3500 0000 7216 0000 0072 1600 0000 7217  5...r....r....r.
+000028e0: 0000 00da 0c65 7865 635f 6c6d 5f70 6970  .....exec_lm_pip
+000028f0: 6567 0100 0073 1600 0000 0005 0202 0a01  eg...s..........
+00002900: 0602 1801 0801 1401 0e01 1401 0e01 1801  ................
+00002910: 7286 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002920: 0000 0200 0000 0a00 0000 4300 0000 734a  ..........C...sJ
+00002930: 0000 007a 1074 0074 017c 0083 0201 0057  ...z.t.t.|.....W
+00002940: 0064 0153 0004 0074 0279 4401 007d 0101  .d.S...t.yD..}..
+00002950: 007a 1c74 0364 027c 019b 009d 0283 0101  .z.t.d.|........
+00002960: 0057 0059 0064 037d 017e 0164 0453 0064  .W.Y.d.}.~.d.S.d
+00002970: 037d 017e 0130 0030 0064 0353 0029 057a  .}.~.0.0.d.S.).z
+00002980: 5a0a 2020 2020 5772 6170 7065 7220 666f  Z.    Wrapper fo
+00002990: 7220 6578 6563 5f6c 6d5f 7069 7065 0a20  r exec_lm_pipe. 
+000029a0: 2020 202d 2053 6368 6564 756c 6520 4c4d     - Schedule LM
+000029b0: 2065 7865 6375 7469 6f6e 7320 6672 6f6d   executions from
+000029c0: 2049 5251 7320 2865 7874 4952 512c 2074   IRQs (extIRQ, t
+000029d0: 696d 4952 5129 0a20 2020 2054 7a1d 6578  imIRQ).    Tz.ex
+000029e0: 6563 5f6c 6d5f 7069 7065 5f73 6368 6564  ec_lm_pipe_sched
+000029f0: 756c 6520 6572 726f 723a 204e 4629 0472  ule error: NF).r
+00002a00: 0400 0000 7286 0000 0072 3200 0000 7206  ....r....r2...r.
+00002a10: 0000 0029 0272 8500 0000 7235 0000 0072  ...).r....r5...r
+00002a20: 1600 0000 7216 0000 0072 1700 0000 da15  ....r....r......
+00002a30: 6578 6563 5f6c 6d5f 7069 7065 5f73 6368  exec_lm_pipe_sch
+00002a40: 6564 756c 657b 0100 0073 0c00 0000 0005  edule{...s......
+00002a50: 0201 0a01 0601 0e01 0e01 7287 0000 0063  ..........r....c
+00002a60: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00002a70: 0300 0000 0300 0000 7334 0000 0088 0164  ........s4.....d
+00002a80: 0175 0072 1064 0264 0384 0089 0187 0087  .u.r.d.d........
+00002a90: 0166 0264 0464 0584 087d 027c 0288 0083  .f.d.d...}.|....
+00002aa0: 0172 2a64 0653 0074 0088 0088 0183 0253  .r*d.S.t.......S
+00002ab0: 0029 077a 8b0a 2020 2020 4d61 696e 204c  .).z..    Main L
+00002ac0: 4d20 6578 6563 7574 6f72 2066 756e 6374  M executor funct
+00002ad0: 696f 6e20 7772 6170 7065 720a 2020 2020  ion wrapper.    
+00002ae0: 2d20 6861 6e64 6c65 2061 7379 6e63 2028  - handle async (
+00002af0: 6261 636b 6772 6f75 6e64 2920 7461 736b  background) task
+00002b00: 2065 7865 6375 7469 6f6e 0a20 2020 202d   execution.    -
+00002b10: 2068 616e 646c 6520 7379 6e63 2074 6173   handle sync tas
+00002b20: 6b20 6578 6563 7574 696f 6e20 285f 6578  k execution (_ex
+00002b30: 6563 5f6c 6d5f 636f 7265 290a 2020 2020  ec_lm_core).    
+00002b40: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
+00002b50: 0000 0100 0000 5300 0000 7304 0000 0064  ......S...s....d
+00002b60: 0053 0029 014e 7216 0000 0072 5600 0000  .S.).Nr....rV...
+00002b70: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00002b80: 083c 6c61 6d62 6461 3e91 0100 0072 5100  .<lambda>....rQ.
+00002b90: 0000 7a1e 6578 6563 5f6c 6d5f 636f 7265  ..z.exec_lm_core
+00002ba0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00002bb0: 613e 6301 0000 0000 0000 0000 0000 000a  a>c.............
+00002bc0: 0000 000a 0000 0013 0000 0073 9a01 0000  ...........s....
+00002bd0: 7400 7c00 8301 7d01 6401 7c00 6402 1900  t.|...}.d.|.d...
+00002be0: 6b02 72b6 7c01 6403 6b02 724e 6404 7c00  k.r.|.d.k.rNd.|.
+00002bf0: 6405 1900 6b02 724e 6406 a001 7402 8300  d...k.rNd...t...
+00002c00: a003 a100 a101 7d02 7c02 9b00 6406 9d02  ......}.|...d...
+00002c10: 7d02 8801 7c02 8301 0100 6407 5300 7c01  }...|.....d.S.|.
+00002c20: 6403 6b04 72aa 6408 7c00 6405 1900 6b02  d.k.r.d.|.d...k.
+00002c30: 7284 7402 8300 6a04 7c00 6403 1900 6409  r.t...j.|.d...d.
+00002c40: 8d01 5c02 7d03 7d04 8801 7c04 8301 0100  ..\.}.}...|.....
+00002c50: 6407 5300 640a 7c00 6405 1900 6b02 72aa  d.S.d.|.d...k.r.
+00002c60: 8801 7402 8300 6a05 7c00 6403 1900 6409  ..t...j.|.d...d.
+00002c70: 8d01 8301 0100 6407 5300 8801 640b 8301  ......d.S...d...
+00002c80: 0100 6407 5300 7c01 6403 6b04 9001 7296  ..d.S.|.d.k...r.
+00002c90: 640c 8800 640d 1900 7600 9001 7296 8800  d...d...v...r...
+00002ca0: a006 640d a101 7d05 7c05 a007 640c a101  ..d...}.|...d...
+00002cb0: 6403 6b02 72ea 6407 6e02 640e 7d06 7c05  d.k.r.d.n.d.}.|.
+00002cc0: a008 640c 640f a102 a009 a100 7d07 7c07  ..d.d.......}.|.
+00002cd0: a00a a100 9001 7210 740b 7c07 8301 6e02  ......r.t.|...n.
+00002ce0: 6400 7d07 7a16 7402 8300 6a0c 8800 7c06  d.}.z.t...j...|.
+00002cf0: 7c07 6410 8d03 7d03 5700 6e30 0400 740d  |.d...}.W.n0..t.
+00002d00: 9001 795a 0100 7d08 0100 7a16 8801 7c08  ..yZ..}...z...|.
+00002d10: 8301 0100 5700 5900 6400 7d08 7e08 6407  ....W.Y.d.}.~.d.
+00002d20: 5300 6400 7d08 7e08 3000 3000 6411 a001  S.d.}.~.0.0.d...
+00002d30: 8800 6402 6403 8502 1900 a101 7d09 7c03  ..d.d.......}.|.
+00002d40: 9001 7284 8801 6412 7c09 9b00 9d02 8301  ..r...d.|.......
+00002d50: 0100 6e0e 8801 7c09 9b00 6413 9d02 8301  ..n...|...d.....
+00002d60: 0100 6407 5300 640e 5300 2914 4e72 1000  ..d.S.d.S.).Nr..
+00002d70: 0000 7201 0000 0072 2a00 0000 7262 0000  ..r....r*...rb..
+00002d80: 0072 4e00 0000 7272 0000 0054 727a 0000  .rN...rr...Trz..
+00002d90: 0029 0172 1300 0000 7274 0000 007a 4149  .).r....rt...zAI
+00002da0: 6e76 616c 6964 2074 6173 6b20 636d 6421  nvalid task cmd!
+00002db0: 2048 656c 703a 2074 6173 6b20 6c69 7374   Help: task list
+00002dc0: 202f 206b 696c 6c20 3c74 6173 6b49 443e   / kill <taskID>
+00002dd0: 202f 2073 686f 7720 3c74 6173 6b49 443e   / show <taskID>
+00002de0: fa01 26e9 ffff ffff 4672 0c00 0000 2902  ..&.....Fr....).
+00002df0: 722e 0000 0072 6300 0000 7229 0000 007a  r....rc...r)...z
+00002e00: 0653 7461 7274 207a 0820 6973 2042 7573  .Start z. is Bus
+00002e10: 7929 0e72 2300 0000 722c 0000 0072 4000  y).r#...r,...r@.
+00002e20: 0000 726b 0000 0072 7a00 0000 7274 0000  ..rk...rz...rt..
+00002e30: 00da 0370 6f70 da05 636f 756e 74da 0772  ...pop..count..r
+00002e40: 6570 6c61 6365 7280 0000 00da 0769 7364  eplacer......isd
+00002e50: 6967 6974 725c 0000 0072 2600 0000 7232  igitr\...r&...r2
+00002e60: 0000 0029 0a5a 086d 7367 5f6c 6973 745a  ...).Z.msg_listZ
+00002e70: 076d 7367 5f6c 656e 7273 0000 0072 7800  .msg_lenrs...rx.
+00002e80: 0000 723a 0000 00da 046d 6f64 6572 2e00  ..r:.....moder..
+00002e90: 0000 7263 0000 0072 3500 0000 7213 0000  ..rc...r5...r...
+00002ea0: 00a9 02da 0861 7267 5f6c 6973 7472 3600  .....arg_listr6.
+00002eb0: 0000 7216 0000 0072 1700 0000 da0c 7461  ..r....r......ta
+00002ec0: 736b 5f6d 616e 6167 6572 9301 0000 7342  sk_manager....sB
+00002ed0: 0000 0000 0108 020c 0214 0110 010a 0108  ................
+00002ee0: 0104 0208 010c 0116 0108 0104 010c 0116  ................
+00002ef0: 0104 0108 0104 0218 020a 0116 0110 0116  ................
+00002f00: 0202 0116 0110 0108 0218 0112 0106 0110  ................
+00002f10: 020e 0204 027a 2265 7865 635f 6c6d 5f63  .....z"exec_lm_c
+00002f20: 6f72 652e 3c6c 6f63 616c 733e 2e74 6173  ore.<locals>.tas
+00002f30: 6b5f 6d61 6e61 6765 7254 2901 7238 0000  k_managerT).r8..
+00002f40: 0029 0372 9100 0000 7236 0000 0072 9200  .).r....r6...r..
+00002f50: 0000 7216 0000 0072 9000 0000 7217 0000  ..r....r....r...
+00002f60: 0072 8400 0000 8801 0000 730c 0000 0000  .r........s.....
+00002f70: 0808 0108 020e 2f08 0104 0272 8400 0000  ....../....r....
+00002f80: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
+00002f90: 000a 0000 0003 0000 0073 d001 0000 6401  .........s....d.
+00002fa0: 6402 8400 7d02 8700 6601 6403 6404 8408  d...}...f.d.d...
+00002fb0: 7d03 7c00 6405 1900 6406 6b02 7d04 7c04  }.|.d...d.k.}.|.
+00002fc0: 7230 7c00 6407 6405 8502 1900 6e02 7c00  r0|.d.d.....n.|.
+00002fd0: 7d05 7400 7c05 8301 6408 6b05 9001 72bc  }.t.|...d.k...r.
+00002fe0: 6409 7c05 6407 1900 9b00 9d02 7c05 640a  d.|.d.......|.d.
+00002ff0: 1900 7c02 640b a001 7c05 6408 640c 8502  ..|.d...|.d.d...
+00003000: 1900 a101 8301 0300 0200 7d06 7d07 7d08  ..........}.}.}.
+00003010: 7aca 7c06 7402 7601 728a 7403 640d 7c06  z.|.t.v.r.t.d.|.
+00003020: 9b00 9d02 8301 0100 7a1e 7404 7c06 9b00  ........z.t.|...
+00003030: 640e 7c07 9b00 640f 7c08 9b00 6410 9d06  d.|...d.|...d...
+00003040: 8301 8900 5700 6e76 0400 7405 9001 791e  ....W.nv..t...y.
+00003050: 0100 7d09 0100 7a5c 7c06 7406 7c09 8301  ..}...z\|.t.|...
+00003060: 7600 9001 7202 7407 6411 7c06 9b00 6412  v...r.t.d.|...d.
+00003070: 9d03 8301 0100 7403 640d 7c06 9b00 9d02  ......t.d.|.....
+00003080: 8301 0100 7404 7c06 9b00 640e 7c07 9b00  ....t.|...d.|...
+00003090: 640f 7c08 9b00 6410 9d06 8301 8900 6e08  d.|...d.......n.
+000030a0: 7405 7c09 8301 8201 5700 5900 640c 7d09  t.|.....W.Y.d.}.
+000030b0: 7e09 6e0a 640c 7d09 7e09 3000 3000 7c03  ~.n.d.}.~.0.0.|.
+000030c0: 7c04 7c07 8800 8303 8900 7c01 7406 8800  |.|.......|.t...
+000030d0: 8301 8301 0100 5700 6413 5300 0400 7405  ......W.d.S...t.
+000030e0: 9001 79ba 0100 7d09 0100 7a64 7c01 6414  ..y...}...zd|.d.
+000030f0: 7c06 9b00 6415 7c07 9b00 6416 7c09 9b00  |...d.|...d.|...
+00003100: 9d06 8301 0100 6417 7406 7c09 8301 7600  ......d.t.|...v.
+00003110: 9001 7384 6418 7406 7c09 8301 7600 9001  ..s.d.t.|...v...
+00003120: 72a6 7c06 7402 a008 a100 7600 9001 7298  r.|.t.....v...r.
+00003130: 7402 7c06 3d00 5700 5900 640c 7d09 7e09  t.|.=.W.Y.d.}.~.
+00003140: 6419 5300 5700 5900 640c 7d09 7e09 6e0a  d.S.W.Y.d.}.~.n.
+00003150: 640c 7d09 7e09 3000 3000 7c01 641a 8301  d.}.~.0.0.|.d...
+00003160: 0100 7c01 641b 8301 0100 6413 5300 291c  ..|.d.....d.S.).
+00003170: 7ae3 0a20 2020 204d 4149 4e20 4655 4e43  z..    MAIN FUNC
+00003180: 5449 4f4e 2054 4f20 5255 4e20 5354 5249  TION TO RUN STRI
+00003190: 4e47 204d 4f44 554c 452e 4655 4e43 5449  NG MODULE.FUNCTI
+000031a0: 4f4e 2045 5845 4355 5449 4f4e 530a 2020  ON EXECUTIONS.  
+000031b0: 2020 5b31 5d20 6d6f 6475 6c65 206e 616d    [1] module nam
+000031c0: 6520 284c 4d29 0a20 2020 205b 325d 2066  e (LM).    [2] f
+000031d0: 756e 6374 696f 6e0a 2020 2020 5b33 2e2e  unction.    [3..
+000031e0: 2e5d 2070 6172 616d 6574 6572 7320 2873  .] parameters (s
+000031f0: 6570 6172 6174 6f72 3a20 7370 6163 6529  eparator: space)
+00003200: 0a20 2020 204e 4f54 453a 206d 7367 6f62  .    NOTE: msgob
+00003210: 6a20 2d20 6d75 7374 2062 6520 6120 6675  j - must be a fu
+00003220: 6e63 7469 6f6e 2077 6974 6820 6f6e 6520  nction with one 
+00003230: 696e 7075 7420 7061 7261 6d20 2873 7464  input param (std
+00003240: 6f75 742f 6669 6c65 2f73 7472 6561 6d29  out/file/stream)
+00003250: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
+00003260: 0000 0300 0000 0500 0000 1300 0000 7380  ..............s.
+00003270: 0000 0064 007d 0164 0188 0076 0073 1464  ...d.}.d...v.s.d
+00003280: 0288 0076 0072 5c64 0364 0484 0074 0088  ...v.r\d.d...t..
+00003290: 0083 0144 0083 0189 0187 0087 0166 0264  ...D.........f.d
+000032a0: 0564 0484 0874 0164 0674 0288 0183 0164  .d...t.d.t.....d
+000032b0: 0783 0344 0083 017d 017c 0144 005d 107d  ...D...}.|.D.].}
+000032c0: 0288 00a0 037c 0264 08a1 0289 0071 4a88  .....|.d.....qJ.
+000032d0: 00a0 0364 0964 0aa1 0289 0074 047c 0174  ...d.d.....t.|.t
+000032e0: 0583 0272 7c88 006a 067c 018e 0089 0088  ...r|..j.|......
+000032f0: 0053 0029 0b4e fa01 27fa 0122 6301 0000  .S.).N..'.."c...
+00003300: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00003310: 0053 0000 0073 2400 0000 6700 7c00 5d1c  .S...s$...g.|.].
+00003320: 5c02 7d01 7d02 7c02 6400 6b02 731c 7c02  \.}.}.|.d.k.s.|.
+00003330: 6401 6b02 7204 7c01 9102 7104 5300 2902  d.k.r.|...q.S.).
+00003340: 7294 0000 0072 9300 0000 7216 0000 0029  r....r....r....)
+00003350: 0372 4f00 0000 da01 69da 0163 7216 0000  .rO.....i..cr...
+00003360: 0072 1600 0000 7217 0000 0072 5000 0000  .r....r....rP...
+00003370: d401 0000 7251 0000 007a 3d5f 6578 6563  ....rQ...z=_exec
+00003380: 5f6c 6d5f 636f 7265 2e3c 6c6f 6361 6c73  _lm_core.<locals
+00003390: 3e2e 5f5f 636f 6e76 5f66 756e 635f 7061  >.__conv_func_pa
+000033a0: 7261 6d73 2e3c 6c6f 6361 6c73 3e2e 3c6c  rams.<locals>.<l
+000033b0: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+000033c0: 0000 0000 0002 0000 0007 0000 0013 0000  ................
+000033d0: 0073 2800 0000 6700 7c00 5d20 7d01 8800  .s(...g.|.] }...
+000033e0: 8801 7c01 1900 8801 7c01 6400 1700 1900  ..|.....|.d.....
+000033f0: 6400 1700 8502 1900 9102 7104 5300 2901  d.........q.S.).
+00003400: 724e 0000 0072 1600 0000 2902 724f 0000  rN...r....).rO..
+00003410: 005a 0573 7472 5f69 a902 da05 7061 7261  .Z.str_i....para
+00003420: 6d5a 0973 7472 5f69 6e64 6578 7216 0000  mZ.str_indexr...
+00003430: 0072 1700 0000 7250 0000 00d5 0100 0072  .r....rP.......r
+00003440: 5100 0000 7201 0000 0072 2a00 0000 7a02  Q...r....r*...z.
+00003450: 7b7d 7264 0000 0072 7700 0000 2907 da09  {}rd...rw...)...
+00003460: 656e 756d 6572 6174 6572 5b00 0000 7223  enumerater[...r#
+00003470: 0000 0072 8d00 0000 7261 0000 0072 6200  ...r....ra...rb.
+00003480: 0000 da06 666f 726d 6174 2903 7298 0000  ....format).r...
+00003490: 00da 0362 7566 da06 7375 6273 7472 7216  ...buf..substrr.
+000034a0: 0000 0072 9700 0000 7217 0000 00da 125f  ...r....r......_
+000034b0: 5f63 6f6e 765f 6675 6e63 5f70 6172 616d  _conv_func_param
+000034c0: 73d1 0100 0073 1400 0000 0001 0401 1001  s....s..........
+000034d0: 1201 2001 0801 0e01 0c01 0a01 0a01 7a29  .. ...........z)
+000034e0: 5f65 7865 635f 6c6d 5f63 6f72 652e 3c6c  _exec_lm_core.<l
+000034f0: 6f63 616c 733e 2e5f 5f63 6f6e 765f 6675  ocals>.__conv_fu
+00003500: 6e63 5f70 6172 616d 7363 0300 0000 0000  nc_paramsc......
+00003510: 0000 0000 0000 0300 0000 0500 0000 1300  ................
+00003520: 0000 735a 0000 0074 007c 0274 0183 0272  ..sZ...t.|.t...r
+00003530: 2e7c 0072 1674 027c 0283 0153 0064 01a0  .|.r.t.|...S.d..
+00003540: 0364 0264 0384 0088 00a0 04a1 0044 0083  .d.d.........D..
+00003550: 01a1 0153 007c 0164 046b 0272 567c 0072  ...S.|.d.k.rV|.r
+00003560: 4274 027c 0283 0153 0064 01a0 0364 0564  Bt.|...S.d...d.d
+00003570: 0384 007c 0244 0083 01a1 0153 007c 0253  ...|.D.....S.|.S
+00003580: 0029 064e 7272 0000 0063 0100 0000 0000  .).Nrr...c......
+00003590: 0000 0000 0000 0300 0000 0600 0000 5300  ..............S.
+000035a0: 0000 7320 0000 0067 007c 005d 185c 027d  ..s ...g.|.].\.}
+000035b0: 017d 0264 007c 019b 0064 017c 029b 009d  .}.d.|...d.|....
+000035c0: 0491 0271 0453 0029 0272 6400 0000 7271  ...q.S.).rd...rq
+000035d0: 0000 0072 1600 0000 2903 724f 0000 00da  ...r....).rO....
+000035e0: 036b 6579 da05 7661 6c75 6572 1600 0000  .key..valuer....
+000035f0: 7216 0000 0072 1700 0000 7250 0000 00e3  r....r....rP....
+00003600: 0100 0072 5100 0000 7a37 5f65 7865 635f  ...rQ...z7_exec_
+00003610: 6c6d 5f63 6f72 652e 3c6c 6f63 616c 733e  lm_core.<locals>
+00003620: 2e5f 5f66 6f72 6d61 745f 6f75 742e 3c6c  .__format_out.<l
+00003630: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00003640: 3eda 0468 656c 7063 0100 0000 0000 0000  >..helpc........
+00003650: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00003660: 7318 0000 0067 007c 005d 107d 0164 007c  s....g.|.].}.d.|
+00003670: 019b 0064 019d 0391 0271 0453 0029 0272  ...d.....q.S.).r
+00003680: 6400 0000 fa01 2c72 1600 0000 2902 724f  d.....,r....).rO
+00003690: 0000 0072 1200 0000 7216 0000 0072 1600  ...r....r....r..
+000036a0: 0000 7217 0000 0072 5000 0000 e901 0000  ..r....rP.......
+000036b0: 7251 0000 0029 0572 6100 0000 da04 6469  rQ...).ra.....di
+000036c0: 6374 7203 0000 0072 2c00 0000 7253 0000  ctr....r,...rS..
+000036d0: 0029 03da 096a 736f 6e5f 6d6f 6465 da07  .)...json_mode..
+000036e0: 6c6d 5f66 756e 6372 6900 0000 a901 5a09  lm_funcri.....Z.
+000036f0: 6c6d 5f6f 7574 7075 7472 1600 0000 7217  lm_outputr....r.
+00003700: 0000 00da 0c5f 5f66 6f72 6d61 745f 6f75  .....__format_ou
+00003710: 74de 0100 0073 1200 0000 0001 0a01 0401  t....s..........
+00003720: 0802 1802 0801 0401 0802 1401 7a23 5f65  ............z#_e
+00003730: 7865 635f 6c6d 5f63 6f72 652e 3c6c 6f63  xec_lm_core.<loc
+00003740: 616c 733e 2e5f 5f66 6f72 6d61 745f 6f75  als>.__format_ou
+00003750: 7472 8a00 0000 7a05 3e6a 736f 6e72 0100  tr....z.>jsonr..
+00003760: 0000 722a 0000 005a 034c 4d5f 724e 0000  ..r*...Z.LM_rN..
+00003770: 0072 6400 0000 4e7a 0769 6d70 6f72 7420  .rd...Nz.import 
+00003780: 7229 0000 00fa 0128 fa01 297a 185f 6578  r).....(..)z._ex
+00003790: 6563 5f6c 6d5f 636f 7265 2072 652d 696d  ec_lm_core re-im
+000037a0: 706f 7274 20fa 0121 547a 0d65 7865 635f  port ..!Tz.exec_
+000037b0: 6c6d 5f63 6f72 6520 7a02 2d3e 7271 0000  lm_core z.->rq..
+000037c0: 007a 186d 656d 6f72 7920 616c 6c6f 6361  .z.memory alloca
+000037d0: 7469 6f6e 2066 6169 6c65 647a 0e69 7320  tion failedz.is 
+000037e0: 6e6f 7420 6465 6669 6e65 6446 7a34 5348  not definedFz4SH
+000037f0: 454c 4c3a 2074 7970 6520 6865 6c70 2066  ELL: type help f
+00003800: 6f72 2073 696e 676c 6520 776f 7264 2063  or single word c
+00003810: 6f6d 6d61 6e64 7320 2862 7569 6c74 2d69  ommands (built-i
+00003820: 6e29 7a43 5348 454c 4c3a 2066 6f72 204c  n)zCSHELL: for L
+00003830: 4d20 6578 6563 3a20 5b31 5d28 4c4d 296d  M exec: [1](LM)m
+00003840: 6f64 756c 6520 5b32 5d66 756e 6374 696f  odule [2]functio
+00003850: 6e20 5b33 2e2e 2e5d 6f70 7469 6f6e 616c  n [3...]optional
+00003860: 2070 6172 616d 7329 0972 2300 0000 722c   params).r#...r,
+00003870: 0000 0072 0200 0000 da04 6578 6563 da04  ...r......exec..
+00003880: 6576 616c 7232 0000 0072 3300 0000 7206  evalr2...r3...r.
+00003890: 0000 0072 1c00 0000 290a 7291 0000 0072  ...r....).r....r
+000038a0: 3600 0000 729d 0000 0072 a600 0000 72a3  6...r....r....r.
+000038b0: 0000 005a 0863 6d64 5f6c 6973 745a 066c  ...Z.cmd_listZ.l
+000038c0: 6d5f 6d6f 6472 a400 0000 5a09 6c6d 5f70  m_modr....Z.lm_p
+000038d0: 6172 616d 7372 3500 0000 7216 0000 0072  aramsr5...r....r
+000038e0: a500 0000 7217 0000 0072 3800 0000 c801  ....r....r8.....
+000038f0: 0000 733a 0000 0000 0908 0d0c 0f0c 0114  ..s:............
+00003900: 020e 0130 0102 0308 010e 0102 021e 0110  ...0............
+00003910: 020e 0110 020e 021c 021e 030c 020c 0106  ................
+00003920: 0210 011a 011c 020e 0106 0224 0108 0108  ...........$....
+00003930: 0272 3800 0000 6301 0000 0000 0000 0000  .r8...c.........
+00003940: 0000 0002 0000 000a 0000 0043 0000 0073  ...........C...s
+00003950: 5000 0000 7a10 7400 7401 7c00 8302 0100  P...z.t.t.|.....
+00003960: 5700 6401 5300 0400 7402 794a 0100 7d01  W.d.S...t.yJ..}.
+00003970: 0100 7a22 7403 6402 7c00 9b00 6403 7c01  ..z"t.d.|...d.|.
+00003980: 9b00 9d04 8301 0100 5700 5900 6404 7d01  ........W.Y.d.}.
+00003990: 7e01 6405 5300 6404 7d01 7e01 3000 3000  ~.d.S.d.}.~.0.0.
+000039a0: 6404 5300 2906 7a74 0a20 2020 2057 7261  d.S.).zt.    Wra
+000039b0: 7070 6572 2066 6f72 2065 7865 635f 6c6d  pper for exec_lm
+000039c0: 5f63 6f72 6520 666f 7220 5363 6865 6475  _core for Schedu
+000039d0: 6c65 720a 2020 2020 2d20 6d69 6372 6f70  ler.    - microp
+000039e0: 7974 686f 6e20 7363 6865 6475 6c69 6e67  ython scheduling
+000039f0: 0a20 2020 2020 2020 202d 2065 7865 6320  .        - exec 
+00003a00: 7072 6f74 6563 7469 6f6e 2066 6f72 2063  protection for c
+00003a10: 726f 6e20 4952 510a 2020 2020 547a 1173  ron IRQ.    Tz.s
+00003a20: 6368 6564 756c 655f 6c6d 5f65 7865 6320  chedule_lm_exec 
+00003a30: 7a08 2065 7272 6f72 3a20 4e46 2904 7204  z. error: NF).r.
+00003a40: 0000 0072 8400 0000 7232 0000 0072 0600  ...r....r2...r..
+00003a50: 0000 2902 7291 0000 0072 3500 0000 7216  ..).r....r5...r.
+00003a60: 0000 0072 1600 0000 7217 0000 00da 1565  ...r....r......e
+00003a70: 7865 635f 6c6d 5f63 6f72 655f 7363 6865  xec_lm_core_sche
+00003a80: 6475 6c65 1902 0000 730c 0000 0000 0602  dule....s.......
+00003a90: 010a 0106 010e 0114 0172 ac00 0000 2901  .........r....).
+00003aa0: 4e29 18da 075f 5f64 6f63 5f5f da03 7379  N)...__doc__..sy
+00003ab0: 7372 0200 0000 5a04 6a73 6f6e 7203 0000  sr....Z.jsonr...
+00003ac0: 005a 0b6d 6963 726f 7079 7468 6f6e 7204  .Z.micropythonr.
+00003ad0: 0000 005a 0875 6173 796e 6369 6f72 2400  ...Z.uasyncior$.
+00003ae0: 0000 da05 4465 6275 6772 0500 0000 7206  ....Debugr....r.
+00003af0: 0000 005a 0d43 6f6e 6669 6748 616e 646c  ...Z.ConfigHandl
+00003b00: 6572 7207 0000 00da 0575 7469 6d65 7208  err......utimer.
+00003b10: 0000 0072 0900 0000 720a 0000 0072 4000  ...r....r....r@.
+00003b20: 0000 7286 0000 0072 8700 0000 7284 0000  ..r....r....r...
+00003b30: 0072 3800 0000 72ac 0000 0072 1600 0000  .r8...r....r....
+00003b40: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00003b50: 083c 6d6f 6475 6c65 3e01 0000 0073 2000  .<module>....s .
+00003b60: 0000 040e 0c01 0c01 0c01 0801 1001 0c01  ................
+00003b70: 1008 0e7f 0014 0e7f 0038 0814 080d 0a40  .........8.....@
+00003b80: 0851                                     .Q
```

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/Time.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Time.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/micrOS.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/__pycache__/urequests.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/urequests.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.18.3/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.18.3/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/pycallgraph.png` & `micrOSDevToolKit-1.18.3/micrOS/source/pycallgraph.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOS/source/urequests.py` & `micrOSDevToolKit-1.18.3/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.18.1
+Version: 1.18.3
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.18.1/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 devToolKit.py
 setup.py
 env/__init__.py
 media/__init__.py
 media/dnd.png
 media/logo.png
 media/logo_mini.png
+micrOS/SchedulerUT.py
 micrOS/__init__.py
-micrOS/micropython/__init__.py
 micrOS/micropython/esp32-20220618-v1.19.1.bin
 micrOS/micropython/esp32s2-20220618-v1.19.1.bin
 micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
 micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
 micrOS/micropython/tinypico-20220618-v1.19.1.bin
 micrOS/source/.DS_Store
 micrOS/source/Common.py
@@ -86,14 +86,15 @@
 micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
 micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
 micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
 micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
 micrOS/source/__pycache__/LM_system.cpython-39.pyc
 micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
 micrOS/source/__pycache__/Network.cpython-39.pyc
+micrOS/source/__pycache__/Scheduler.cpython-39.pyc
 micrOS/source/__pycache__/SocketServer.cpython-39.pyc
 micrOS/source/__pycache__/TaskManager.cpython-39.pyc
 micrOS/source/__pycache__/Time.cpython-39.pyc
 micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
 micrOS/source/__pycache__/micrOS.cpython-39.pyc
 micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
 micrOS/source/__pycache__/urequests.cpython-39.pyc
```

### Comparing `micrOSDevToolKit-1.18.1/setup.py` & `micrOSDevToolKit-1.18.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.18.1',
+    version='1.18.3',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.18.1/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.18.3/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.18.3/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.18.3/toolkit/DevEnvUSB.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,16 @@
                         micros_devices.append(dev_abs_path)
                         self.console("Device was found: {}".format(dev_abs_path), state="imp")
                         break
         else:
             # List USB devices on Windows
             ports = list(serial_port_list.comports())
             for item in ports:
-                if "CP210" in str(item.description):
+                self.console(f'[Win] Com device: {item.description}')
+                if "CP210" in str(item.description) or "CH340" in str(item.description):
                     micros_devices.append(item.device)
                     self.console("Device was found: {}".format(item.device, state="imp"))
         # Eval device list, return with devices
         if len(micros_devices) > 0:
             self.console("Device was found. :)", state="ok")
         else:
             self.console("No device was connected. :(", state="err")
```

### Comparing `micrOSDevToolKit-1.18.1/toolkit/Gateway.py` & `micrOSDevToolKit-1.18.3/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.18.3/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.18.3/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.18.3/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.18.3/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.18.3/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.18.3/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.18.3/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/socketClient.py` & `micrOSDevToolKit-1.18.3/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files 21% similar despite different names*

```diff
@@ -1,129 +1,140 @@
-00000000: 4d06 001f 4c0b 1e49 6e74 6572 436f 6e6e  M...L..InterConn
+00000000: 4d06 001f 530a 1e49 6e74 6572 436f 6e6e  M...S..InterConn
 00000010: 6563 742e 7079 000f 1075 6173 796e 6369  ect.py...uasynci
 00000020: 6f00 1667 6574 6164 6472 696e 666f 000e  o..getaddrinfo..
 00000030: 4146 5f49 4e45 5400 1653 4f43 4b5f 5354  AF_INET..SOCK_ST
 00000040: 5245 414d 000c 736f 636b 6574 000a 6d61  REAM..socket..ma
 00000050: 7463 6800 0472 6500 1465 7272 6c6f 675f  tch..re..errlog_
 00000060: 6164 6400 0a44 6562 7567 000c 6366 6767  add..Debug..cfgg
 00000070: 6574 001a 436f 6e66 6967 4861 6e64 6c65  et..ConfigHandle
 00000080: 7200 1853 6f63 6b65 7453 6572 7665 7200  r..SocketServer.
 00000090: 0854 6173 6b00 1654 6173 6b4d 616e 6167  .Task..TaskManag
-000000a0: 6572 0010 496e 7465 7243 6f6e 000e 736f  er..InterCon..so
-000000b0: 6370 6f72 7400 125f 7365 6e64 5f63 6d64  cport.._send_cmd
-000000c0: 0008 7461 736b 0010 7365 6e64 5f63 6d64  ..task..send_cmd
-000000d0: 0006 6f75 7400 8129 0c63 7265 6174 6500  ..out..).create.
-000000e0: 1063 616c 6c62 6163 6b00 0674 6167 000e  .callback..tag..
-000000f0: 7665 7264 6963 7400 1464 756d 705f 6361  verdict..dump_ca
-00000100: 6368 6500 1043 4f4e 4e5f 4d41 5000 230c  che..CONN_MAP.#.
-00000110: 7265 6164 6572 000c 7772 6974 6572 001a  reader..writer..
-00000120: 7661 6c69 6461 7465 5f69 7076 3400 812d  validate_ipv4..-
-00000130: 0850 4f52 5400 1a72 6570 6c79 5f6d 6573  .PORT..reply_mes
-00000140: 7361 6765 0003 1e6f 7065 6e5f 636f 6e6e  sage...open_conn
-00000150: 6563 7469 6f6e 001a 5f5f 7275 6e5f 636f  ection..__run_co
-00000160: 6d6d 616e 6400 810f 1677 6169 745f 636c  mmand....wait_cl
-00000170: 6f73 6564 000c 656e 636f 6465 001c 5f5f  osed..encode..__
-00000180: 7265 6365 6976 655f 6461 7461 0082 0302  receive_data....
-00000190: 2400 8231 8223 022e 0082 490a 6472 6169  $..1.#....I.drai
-000001a0: 6e00 0c70 726f 6d70 7400 0200 0081 7b0c  n..prompt.....{.
-000001b0: 6465 636f 6465 0082 4308 4279 6521 0007  decode..C.Bye!..
-000001c0: 090e 5f74 6167 6966 7900 8151 0c2e 6c6f  .._tagify..Q..lo
-000001d0: 6361 6c00 0e61 7379 6e63 696f 002f 2d35  cal..asyncio./-5
-000001e0: 8229 0868 6f73 7400 0663 6d64 000e 636f  .).host..cmd..co
-000001f0: 6d5f 6f62 6a00 8213 0c73 7472 5f69 6e00  m_obj....str_in.
-00000200: 7d61 1068 6f73 746e 616d 6500 822f 0b05  }a.hostname../..
-00000210: 0b69 6e74 6572 636f 6e2e 7b7d 0005 2254  .intercon.{}.."T
-00000220: 6173 6b20 7374 6172 7465 6420 7b7d 3a7b  ask started {}:{
-00000230: 7d20 2d3e 2074 6173 6b20 7368 6f77 207b  } -> task show {
-00000240: 7d00 050c 5461 736b 2069 7320 4275 7379  }...Task is Busy
-00000250: 0005 8114 5e28 5c64 7c5b 312d 395d 5c64  ....^(\d|[1-9]\d
-00000260: 7c31 5c64 5c64 7c32 5b30 2d34 5d5c 647c  |1\d\d|2[0-4]\d|
-00000270: 3235 5b30 2d35 5d29 5c2e 285c 647c 5b31  25[0-5])\.(\d|[1
-00000280: 2d39 5d5c 647c 315c 645c 647c 325b 302d  -9]\d|1\d\d|2[0-
-00000290: 345d 5c64 7c32 355b 302d 355d 295c 2e28  4]\d|25[0-5])\.(
-000002a0: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
-000002b0: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
-000002c0: 5d29 5c2e 285c 647c 5b31 2d39 5d5c 647c  ])\.(\d|[1-9]\d|
-000002d0: 315c 645c 647c 325b 302d 345d 5c64 7c32  1\d\d|2[0-4]\d|2
-000002e0: 355b 302d 355d 2924 0005 155b 696e 7465  5[0-5])$...[inte
-000002f0: 7263 6f6e 5d20 4e6f 486f 7374 3a20 7b7d  rcon] NoHost: {}
-00000300: 0005 205b 696e 7465 7263 6f6e 5d20 7365  .. [intercon] se
-00000310: 6e64 5f63 6d64 207b 7d20 6f73 6572 723a  nd_cmd {} oserr:
-00000320: 207b 7d00 0520 5b69 6e74 6572 636f 6e5d   {}.. [intercon]
-00000330: 5b45 5252 5d20 496e 7661 6c69 6420 686f  [ERR] Invalid ho
-00000340: 7374 3a20 7b7d 0005 1843 6f6e 6e65 6374  st: {}...Connect
-00000350: 696f 6e20 6973 2062 7573 792e 2042 7965  ion is busy. Bye
-00000360: 2100 050c 5472 7920 6c61 7465 722e 2e2e  !...Try later...
-00000370: 0005 345b 696e 7465 7263 6f6e 5d20 7072  ..4[intercon] pr
-00000380: 6f6d 7074 206d 6973 6d61 7463 682c 2068  ompt mismatch, h
-00000390: 6f73 746e 616d 653a 207b 7d20 7072 6f6d  ostname: {} prom
-000003a0: 7074 3a20 7b7d 2000 050b 5b63 6f6e 6669  pt: {} ...[confi
-000003b0: 6775 7265 5d00 880c 181c 0126 382c 2c2c  gure]......&8,,,
-000003c0: 2c6c 8974 840d 841a 8051 1b02 163d 8010  ,l.t.....Q...=..
-000003d0: 0310 0410 052a 031b 061c 0316 031c 0416  .....*..........
-000003e0: 041c 0516 0559 8010 072a 011b 081c 0716  .....Y...*......
-000003f0: 0759 8010 092a 011b 0a1c 0916 0959 8010  .Y...*.......Y..
-00000400: 0b2a 011b 0c1c 0b16 0b59 8010 0d2a 011b  .*.......Y...*..
-00000410: 0d1c 0d16 0d59 8010 0e2a 011b 0f1c 0e16  .....Y...*......
-00000420: 0e59 5432 0010 1034 0216 1032 0116 1232  .YT2...4...2...2
-00000430: 0216 1432 0316 1b51 6304 840c 081a 1088  ...2...Qc.......
-00000440: 0a24 4864 4088 0784 3284 1911 3e16 3f10  .$Hd@...2...>.?.
-00000450: 1016 402c 0016 1c11 0b10 1134 0116 2232  ..@,.......4.."2
-00000460: 0016 1d11 4132 0134 0116 2032 0216 1432  ....A2.4.. 2...2
-00000470: 0316 2651 2a01 5333 0416 2a51 6305 8148  ..&Q*.S3..*Qc..H
-00000480: 110c 1d45 800e 2424 51b0 181e 51b0 181f  ...E..$$Q...Q...
-00000490: 120e 3400 b018 1351 6381 6029 0e20 4680  ..4....Qc.`). F.
-000004a0: 1423 2c22 2303 c112 4712 07b1 b034 0234  .#,"#...G....4.4
-000004b0: 0144 4252 6350 6393 78f7 4242 1445 4243  .DBRcPc.x.BB.EBC
-000004c0: 801a 8007 422a 422f 222d 5330 2d6e 472a  ....B*B/"-S0-nG*
-000004d0: 4456 5630 2d4c 2528 6c46 4f4a 2c51 c312  DVV0-L%(lFOJ,Q..
-000004e0: 1014 20b1 3601 43e5 80b1 c312 1013 1c14  .. .6.C.........
-000004f0: 21b3 5136 0251 de44 cd80 4817 1203 b112  !.Q6.Q.D..H.....
-00000500: 1013 2280 1205 3404 c4b4 7f55 8455 8055  .."...4....U.U.U
-00000510: c14a 3257 1248 df44 6bc5 4921 120d 3400  .J2W.H.Dk.I!..4.
-00000520: 1423 2304 1416 b536 0136 0159 1209 2305  .##....6.6.Y..#.
-00000530: 1416 b1b5 3602 3401 5910 2463 5151 c528  ....6.4.Y.$cQQ.(
-00000540: 055d 4a01 5d42 4712 1013 1cb3 55c1 1210  .]J.]BG.....U...
-00000550: 1420 b136 0144 9181 4957 4823 123d 1425  . .6.D..IWH#.=.%
-00000560: b112 1013 2236 025e 5168 3002 b018 1eb0  ...."6.^Qh0.....
-00000570: 181f b014 26b2 b336 025e 5168 c64a 3157  ....&..6.^Qh.J1W
-00000580: 1248 df44 6ac5 4920 120d 3400 1423 2304  .H.Dj.I ..4..##.
-00000590: 1416 b536 0136 0159 1209 2305 1416 b1b5  ...6.6.Y..#.....
-000005a0: 3602 3401 5951 c651 51c5 2805 5d4a 015d  6.4.YQ.QQ.(.]J.]
-000005b0: 51b0 131f 4453 b013 1f14 2736 0059 b013  Q...DS....'6.Y..
-000005c0: 1f14 2836 005e 5168 595d b351 ded3 444f  ..(6.^QhY].Q..DO
-000005d0: b651 de44 4351 4241 b112 1013 1cb3 56b6  .Q.DCQBA......V.
-000005e0: 51de 4443 1024 63b6 6312 0923 0614 16b1  Q.DC.$c.c..#....
-000005f0: 3601 3401 5910 2463 8a60 db40 2c26 4543  6.4.Y.$c.`.@,&EC
-00000600: 4980 4c60 4028 2c26 2b42 1f4c 292b 3026  I.L`@(,&+B.L)+0&
-00000610: 4242 3112 4a14 29b1 3601 c1b0 142a 3600  BB1.J.).6....*6.
-00000620: 5e51 6830 02c3 c423 07b4 dd44 4d12 0d34  ^Qh0...#...DM..4
-00000630: 0014 2323 0836 0159 5163 b251 de43 66b4  ..##.6.YQc.Q.Cf.
-00000640: 51de 4361 124a b434 0114 2b10 2c10 2436  Q.Ca.J.4..+.,.$6
-00000650: 0214 2d36 0012 4ab2 3401 142e 102f 3601  ..-6..J.4..../6.
-00000660: 8055 d944 6eb0 131f 1430 b136 0159 b013  .U.Dn....0.6.Y..
-00000670: 1f14 3136 005e 5168 59b0 142a 1032 b436  ..16.^QhY..*.2.6
-00000680: 8200 5e51 6830 02c3 c5b3 1033 d944 4251  ..^Qh0.....3.DBQ
-00000690: 63b3 6312 0d34 0014 2323 0914 16b2 b436  c.c..4..##.....6
-000006a0: 0236 0159 5163 8878 ce41 282a 4532 8065  .6.YQc.x.A(*E2.e
-000006b0: 6020 4320 222e 2324 4c2e 4435 4c29 3110  ` C ".#$L.D5L)1.
-000006c0: 24c2 484d b013 1e14 3422 8200 3601 5e51  $.HM....4"..6.^Q
-000006d0: 68c3 b343 4440 c980 01b3 1435 1036 3601  h..CD@.....5.66.
-000006e0: 142d 3600 c3b1 51de 4447 b314 2d36 0042  .-6...Q.DG..-6.B
-000006f0: 41b1 c1b2 b3e5 c2b1 b214 2d36 00dd 434c  A.........-6..CL
-00000700: 230a b2dd 4346 1037 b3dd 4443 4053 014a  #...CF.7..DC@S.J
-00000710: 0d57 1248 df44 4659 4047 014a 015d 42a1  .W.H.DFY@G.J.]B.
-00000720: 7fb2 142b b110 2436 0214 2b10 3810 3936  ...+..$6..+.8.96
-00000730: 02c2 b2b1 2a02 6382 58c7 4014 1242 4344  ....*.c.X.@..BCD
-00000740: 807e 8007 2632 b213 1347 1159 b214 14b0  .~..&2...G.Y....
-00000750: b136 025e 5168 b213 1318 1551 5c5d b213  .6.^Qh.....Q\]..
-00000760: 1313 1563 861c 6a1f 1442 4380 8b80 0965  ...c..j..BC....e
-00000770: 6025 2a36 2356 2c00 b020 0001 c212 1034  `%*6#V,.. .....4
-00000780: 00c3 2300 1416 b234 0036 01c4 b313 1314  ..#....4.6......
-00000790: 1710 1812 1225 00b1 b334 0310 19b4 3684  .....%...4....6.
-000007a0: 00c5 b544 562c 0223 0114 1625 00b1 b436  ...DV,.#...%...6
-000007b0: 0310 1a62 b410 1962 c642 4c2c 0223 0210  ...b...b.BL,.#..
-000007c0: 1a62 b410 1962 c6b6 6301 8310 290e 3a4b  .b...b..c...).:K
-000007d0: 8095 202a 3412 1014 2025 0036 0144 5410  .. *4... %.6.DT.
-000007e0: 2f14 3b25 0014 2e10 2f36 017e 512e 0255  /.;%..../6.~Q..U
-000007f0: 3601 6325 0014 2b10 3c10 2436 0263 5800  6.c%..+.<.$6.cX.
-00000800: 081b 80a5 6012 1013 1c63                 ....`....c
+000000a0: 6572 000e 636f 6c6c 6563 7400 0467 6300  er..collect..gc.
+000000b0: 0a73 696d 6763 0010 496e 7465 7243 6f6e  .simgc..InterCon
+000000c0: 000e 736f 6370 6f72 7400 125f 7365 6e64  ..socport.._send
+000000d0: 5f63 6d64 0008 7461 736b 0010 7365 6e64  _cmd..task..send
+000000e0: 5f63 6d64 0006 6f75 7400 1073 6c65 6570  _cmd..out..sleep
+000000f0: 5f6d 7300 0c63 6f6e 2e7b 7d00 8129 0c63  _ms..con.{}..).c
+00000100: 7265 6174 6500 1063 616c 6c62 6163 6b00  reate..callback.
+00000110: 0674 6167 000e 7665 7264 6963 7400 1464  .tag..verdict..d
+00000120: 756d 705f 6361 6368 6500 1043 4f4e 4e5f  ump_cache..CONN_
+00000130: 4d41 5000 230c 7265 6164 6572 000c 7772  MAP.#.reader..wr
+00000140: 6974 6572 001a 7661 6c69 6461 7465 5f69  iter..validate_i
+00000150: 7076 3400 812d 0850 4f52 5400 1a72 6570  pv4..-.PORT..rep
+00000160: 6c79 5f6d 6573 7361 6765 0003 1e6f 7065  ly_message...ope
+00000170: 6e5f 636f 6e6e 6563 7469 6f6e 001a 5f5f  n_connection..__
+00000180: 7275 6e5f 636f 6d6d 616e 6400 810f 1677  run_command....w
+00000190: 6169 745f 636c 6f73 6564 000c 656e 636f  ait_closed..enco
+000001a0: 6465 001c 5f5f 7265 6365 6976 655f 6461  de..__receive_da
+000001b0: 7461 0082 0302 2400 8231 8223 022e 0082  ta....$..1.#....
+000001c0: 490a 6472 6169 6e00 0c70 726f 6d70 7400  I.drain..prompt.
+000001d0: 0200 0081 7b0c 6465 636f 6465 0082 4308  ....{.decode..C.
+000001e0: 4279 6521 0007 090e 5f74 6167 6966 7900  Bye!...._tagify.
+000001f0: 0a7b 7d2e 7b7d 0081 510c 2e6c 6f63 616c  .{}.{}..Q..local
+00000200: 000e 6173 796e 6369 6f00 1a63 6f6e 736f  ..asyncio..conso
+00000210: 6c65 5f77 7269 7465 002f 2d35 8229 0868  le_write./-5.).h
+00000220: 6f73 7400 0663 6d64 000e 636f 6d5f 6f62  ost..cmd..com_ob
+00000230: 6a00 8213 0c73 7472 5f69 6e00 7d61 1068  j....str_in.}a.h
+00000240: 6f73 746e 616d 6500 822f 0b05 1a5b 5349  ostname../...[SI
+00000250: 4d55 4c41 544f 5220 4d4f 4445 2047 4320  MULATOR MODE GC 
+00000260: 494d 504f 5254 5d00 0522 5461 736b 2073  IMPORT].."Task s
+00000270: 7461 7274 6564 207b 7d3a 7b7d 202d 3e20  tarted {}:{} -> 
+00000280: 7461 736b 2073 686f 7720 7b7d 0005 0c54  task show {}...T
+00000290: 6173 6b20 6973 2042 7573 7900 0581 145e  ask is Busy....^
+000002a0: 285c 647c 5b31 2d39 5d5c 647c 315c 645c  (\d|[1-9]\d|1\d\
+000002b0: 647c 325b 302d 345d 5c64 7c32 355b 302d  d|2[0-4]\d|25[0-
+000002c0: 355d 295c 2e28 5c64 7c5b 312d 395d 5c64  5])\.(\d|[1-9]\d
+000002d0: 7c31 5c64 5c64 7c32 5b30 2d34 5d5c 647c  |1\d\d|2[0-4]\d|
+000002e0: 3235 5b30 2d35 5d29 5c2e 285c 647c 5b31  25[0-5])\.(\d|[1
+000002f0: 2d39 5d5c 647c 315c 645c 647c 325b 302d  -9]\d|1\d\d|2[0-
+00000300: 345d 5c64 7c32 355b 302d 355d 295c 2e28  4]\d|25[0-5])\.(
+00000310: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
+00000320: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
+00000330: 5d29 2400 0515 5b69 6e74 6572 636f 6e5d  ])$...[intercon]
+00000340: 204e 6f48 6f73 743a 207b 7d00 0520 5b69   NoHost: {}.. [i
+00000350: 6e74 6572 636f 6e5d 2073 656e 645f 636d  ntercon] send_cm
+00000360: 6420 7b7d 206f 7365 7272 3a20 7b7d 0005  d {} oserr: {}..
+00000370: 205b 696e 7465 7263 6f6e 5d5b 4552 525d   [intercon][ERR]
+00000380: 2049 6e76 616c 6964 2068 6f73 743a 207b   Invalid host: {
+00000390: 7d00 0518 436f 6e6e 6563 7469 6f6e 2069  }...Connection i
+000003a0: 7320 6275 7379 2e20 4279 6521 0005 345b  s busy. Bye!..4[
+000003b0: 696e 7465 7263 6f6e 5d20 7072 6f6d 7074  intercon] prompt
+000003c0: 206d 6973 6d61 7463 682c 2068 6f73 746e   mismatch, hostn
+000003d0: 616d 653a 207b 7d20 7072 6f6d 7074 3a20  ame: {} prompt: 
+000003e0: 7b7d 2000 050b 5b63 6f6e 6669 6775 7265  {} ...[configure
+000003f0: 5d00 8a64 2424 0126 382c 2c2c 2c4c 224f  ]..d$$.&8,,,,L"O
+00000400: 276f 8974 8414 841c 8051 1b02 1643 8010  'o.t.....Q...C..
+00000410: 0310 0410 052a 031b 061c 0316 031c 0416  .....*..........
+00000420: 041c 0516 0559 8010 072a 011b 081c 0716  .....Y...*......
+00000430: 0759 8010 092a 011b 0a1c 0916 0959 8010  .Y...*.......Y..
+00000440: 0b2a 011b 0c1c 0b16 0b59 8010 0d2a 011b  .*.......Y...*..
+00000450: 0d1c 0d16 0d59 8010 0e2a 011b 0f1c 0e16  .....Y...*......
+00000460: 0e59 480e 8010 102a 011b 111c 1016 1059  .YH....*.......Y
+00000470: 4a17 5911 4423 0034 0159 8010 102a 011b  J.Y.D#.4.Y...*..
+00000480: 121c 1016 1059 4a01 5d54 3200 1013 3402  .....YJ.]T2...4.
+00000490: 1613 3201 1615 3202 1617 3203 1620 5163  ..2...2...2.. Qc
+000004a0: 0484 0c08 1a13 8810 2448 6440 8807 8432  ........$Hd@...2
+000004b0: 8419 1145 1646 1013 1647 2c00 1621 110b  ...E.F...G,..!..
+000004c0: 1014 3401 1627 3200 1622 1148 3201 3401  ..4..'2..".H2.4.
+000004d0: 1625 3202 1617 3203 162b 512a 0153 3304  .%2...2..+Q*.S3.
+000004e0: 162f 5163 0581 4811 0c22 4c80 1424 2451  ./Qc..H.."L..$$Q
+000004f0: b018 2351 b018 2412 0e34 00b0 1816 5163  ..#Q..$..4....Qc
+00000500: 8160 290e 254d 801a 232c 2223 03c1 124e  .`).%M..#,"#...N
+00000510: 1207 b1b0 3402 3401 4442 5263 5063 9338  ....4.4.DBRcPc.8
+00000520: f742 4217 4c49 4a80 2080 0742 2a42 2f22  .BB.LIJ. ..B*B/"
+00000530: 2d53 302d 6e47 2a44 5656 302d 4c25 286c  -S0-nG*DVV0-L%(l
+00000540: 464f 422c 51c3 1213 1425 b136 0143 e580  FOB,Q....%.6.C..
+00000550: b1c3 1213 1321 1426 b351 3602 51de 44cd  .....!.&.Q6.Q.D.
+00000560: 8048 1712 03b1 1213 1327 8012 0534 04c4  .H.......'...4..
+00000570: b47f 5584 5580 55c1 4a32 5712 4fdf 446b  ..U.U.U.J2W.O.Dk
+00000580: c549 2112 0d34 0014 2823 0414 1bb5 3601  .I!..4..(#....6.
+00000590: 3601 5912 0923 0514 1bb1 b536 0234 0159  6.Y..#.....6.4.Y
+000005a0: 1029 6351 51c5 2805 5d4a 015d 4247 1213  .)cQQ.(.]J.]BG..
+000005b0: 1321 b355 c112 1314 25b1 3601 4489 8149  .!.U....%.6.D..I
+000005c0: 5748 2312 4314 2ab1 1213 1327 3602 5e51  WH#.C.*....'6.^Q
+000005d0: 6830 02b0 1823 b018 24b0 142b b2b3 3602  h0...#..$..+..6.
+000005e0: 5e51 68c6 4a31 5712 4fdf 446a c549 2012  ^Qh.J1W.O.Dj.I .
+000005f0: 0d34 0014 2823 0414 1bb5 3601 3601 5912  .4..(#....6.6.Y.
+00000600: 0923 0514 1bb1 b536 0234 0159 51c6 5151  .#.....6.4.YQ.QQ
+00000610: c528 055d 4a01 5d51 b013 2444 53b0 1324  .(.]J.]Q..$DS..$
+00000620: 142c 3600 59b0 1324 142d 3600 5e51 6859  .,6.Y..$.-6.^QhY
+00000630: 5db3 51de d344 4fb6 51de 4443 5142 41b1  ].Q..DO.Q.DCQBA.
+00000640: 1213 1321 b356 b663 1209 2306 141b b136  ...!.V.c..#....6
+00000650: 0134 0159 1029 638a 00db 402a 2b4c 4a50  .4.Y.)c...@*+LJP
+00000660: 8052 6060 282c 2642 1f4c 292b 3026 4242  .R``(,&B.L)+0&BB
+00000670: 3112 5114 2eb1 3601 c1b0 142f 3600 5e51  1.Q...6..../6.^Q
+00000680: 6830 02c3 c423 07b4 dd44 4251 63b2 51de  h0...#...DBQc.Q.
+00000690: 4366 b451 de43 6112 51b4 3401 1430 1031  Cf.Q.Ca.Q.4..0.1
+000006a0: 1029 3602 1432 3600 1251 b234 0114 3310  .)6..26..Q.4..3.
+000006b0: 3436 0180 55d9 446e b013 2414 35b1 3601  46..U.Dn..$.5.6.
+000006c0: 59b0 1324 1436 3600 5e51 6859 b014 2f10  Y..$.66.^QhY../.
+000006d0: 37b4 3682 005e 5168 3002 c3c5 b310 38d9  7.6..^Qh0.....8.
+000006e0: 4442 5163 b363 120d 3400 1428 2308 141b  DBQc.c..4..(#...
+000006f0: b2b4 3602 3601 5951 6388 78ce 4128 2f4c  ..6.6.YQc.x.A(/L
+00000700: 3780 6b60 2043 2022 2e23 244c 2e44 354c  7.k` C ".#$L.D5L
+00000710: 2931 1029 c248 4db0 1323 1439 2282 0036  )1.).HM..#.9"..6
+00000720: 015e 5168 c3b3 4344 40c9 8001 b314 3a10  .^Qh..CD@.....:.
+00000730: 3b36 0114 3236 00c3 b151 de44 47b3 1432  ;6..26...Q.DG..2
+00000740: 3600 4241 b1c1 b2b3 e5c2 b1b2 1432 3600  6.BA.........26.
+00000750: dd43 4c23 09b2 dd43 4610 3cb3 dd44 4340  .CL#...CF.<..DC@
+00000760: 5301 4a0d 5712 4fdf 4446 5940 4701 4a01  S.J.W.O.DFY@G.J.
+00000770: 5d42 a17f b214 30b1 1029 3602 1430 103d  ]B....0..)6..0.=
+00000780: 103e 3602 c2b2 b12a 0263 8550 df40 2015  .>6....*.c.P.@ .
+00000790: 494a 4b80 8480 0746 252b 2626 2238 25b2  IJK....F%+&&"8%.
+000007a0: 1316 4735 5980 426a 57c3 b214 17b0 b136  ..G5Y.BjW......6
+000007b0: 025e 5168 c4b4 51de d344 48b4 b213 1618  .^Qh..Q..DH.....
+000007c0: 1842 5412 4314 1922 8116 3601 5e51 6859  .BT.C.."..6.^QhY
+000007d0: 81e5 5783 d743 1159 515c 5d12 1034 0059  ..W..C.YQ\]..4.Y
+000007e0: b213 1613 1863 8644 6a9e 0117 494a 8098  .....c.Dj...IJ..
+000007f0: 8009 8608 252a 3723 572c 0001 b0b1 2000  ....%*7#W,.... .
+00000800: 02c2 1213 3400 c310 1a14 1bb2 3400 3601  ....4.......4.6.
+00000810: c4b3 1316 141c 101d 1215 2500 2501 b334  ..........%.%..4
+00000820: 0310 1eb4 3684 00c5 b544 572c 0223 0114  ....6....DW,.#..
+00000830: 1b25 0025 01b4 3603 101f 62b4 101e 62c6  .%.%..6...b...b.
+00000840: 424c 2c02 2302 101f 62b4 101e 62c6 b663  BL,.#...b...b..c
+00000850: 0185 104a 143f 5252 80a2 2020 2f2a 3b25  ...J.?RR..  /*;%
+00000860: 0114 3310 3e36 0180 5514 3236 00c2 1213  ..3.>6..U.26....
+00000870: 1425 2500 3601 445b 1040 141b 1034 1441  .%%.6.D[.@...4.A
+00000880: 2500 1433 1034 3601 7e51 2e02 5536 01b2  %..3.46.~Q..U6..
+00000890: 3602 6310 4014 1b25 0014 3010 4210 2936  6.c.@..%..0.B.)6
+000008a0: 02b2 3602 6358 0008 2080 b460 1213 1321  ..6.cX.. ..`...!
+000008b0: 63                                       c
```

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 0e6d 6163 6869  ug..reset..machi
 000000a0: 6e65 000a 5368 656c 6c00 1031 2e31 382e  ne..Shell..1.18.
-000000b0: 312d 3000 230e 6d73 675f 6f62 6a00 0c64  1-0.#.msg_obj..d
+000000b0: 322d 3000 230e 6d73 675f 6f62 6a00 0c64  2-0.#.msg_obj..d
 000000c0: 6576 6669 6400 105f 5f64 6576 6669 6400  evfid..__devfid.
 000000d0: 0861 7574 6800 165f 5f61 7574 685f 6d6f  .auth..__auth_mo
 000000e0: 6465 000a 6877 7569 6400 0e5f 5f68 7775  de..hwuid..__hwu
 000000f0: 6964 0012 5f5f 6175 7468 5f6f 6b00 165f  id..__auth_ok.._
 00000100: 5f63 6f6e 665f 6d6f 6465 000e 7665 7273  _conf_mode..vers
 00000110: 696f 6e00 1c4d 4943 524f 535f 5645 5253  ion..MICROS_VERS
 00000120: 494f 4e00 8129 066d 7367 000c 7265 626f  ION..).msg..rebo
```

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.1/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

