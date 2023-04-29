# Comparing `tmp/nebulae-0.6.4.tar.gz` & `tmp/nebulae-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nebulae-0.6.4.tar", last modified: Tue Feb 28 03:48:35 2023, max compression
+gzip compressed data, was "dist/nebulae-0.6.5.tar", last modified: Sat Apr 29 13:30:01 2023, max compression
```

## Comparing `nebulae-0.6.4.tar` & `nebulae-0.6.5.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/fuel/
--rw-r--r--   0 root         (0) staff       (20)     1005 2022-08-20 04:55:27.000000 nebulae-0.6.4/nebulae/fuel/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9783 2022-08-20 04:52:42.000000 nebulae-0.6.4/nebulae/fuel/generator.py
--rw-r--r--   0 root         (0) staff       (20)    37708 2023-01-30 13:19:41.000000 nebulae-0.6.4/nebulae/fuel/comburant.py
--rw-r--r--   0 root         (0) staff       (20)     7790 2022-11-01 09:29:19.000000 nebulae-0.6.4/nebulae/fuel/tank.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/law/
--rw-r--r--   0 root         (0) staff       (20)      698 2021-09-14 09:32:19.000000 nebulae-0.6.4/nebulae/law/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      928 2020-10-20 09:25:06.000000 nebulae-0.6.4/nebulae/law/constant.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/kit/
--rw-r--r--   0 root         (0) staff       (20)     1123 2022-08-14 15:13:02.000000 nebulae-0.6.4/nebulae/kit/decorator.py
--rw-r--r--   0 root         (0) staff       (20)    25772 2022-11-04 03:44:29.000000 nebulae-0.6.4/nebulae/kit/utility.py
--rw-r--r--   0 root         (0) staff       (20)     1096 2022-08-21 05:01:44.000000 nebulae-0.6.4/nebulae/kit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      862 2022-07-22 10:10:53.000000 nebulae-0.6.4/nebulae/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/cockpit/
--rw-r--r--   0 root         (0) staff       (20)     3516 2022-08-06 07:48:20.000000 nebulae-0.6.4/nebulae/cockpit/time_machine.py
--rw-r--r--   0 root         (0) staff       (20)     5219 2022-09-16 14:43:52.000000 nebulae-0.6.4/nebulae/cockpit/multiverse.py
--rw-r--r--   0 root         (0) staff       (20)      843 2022-08-06 09:24:38.000000 nebulae-0.6.4/nebulae/cockpit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4251 2022-09-06 15:10:12.000000 nebulae-0.6.4/nebulae/cockpit/engine.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae/aerolog/
--rw-r--r--   0 root         (0) staff       (20)     4845 2022-08-06 10:32:13.000000 nebulae-0.6.4/nebulae/aerolog/blueprint.py
--rw-r--r--   0 root         (0) staff       (20)     5137 2021-12-28 10:13:49.000000 nebulae-0.6.4/nebulae/aerolog/control_panel.py
--rw-r--r--   0 root         (0) staff       (20)      770 2020-10-22 02:51:13.000000 nebulae-0.6.4/nebulae/aerolog/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13726 2023-02-23 04:44:33.000000 nebulae-0.6.4/nebulae/aerolog/dashboard.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae/astro/
--rw-r--r--   0 root         (0) staff       (20)    70841 2023-02-23 07:26:15.000000 nebulae-0.6.4/nebulae/astro/craft.py
--rw-r--r--   0 root         (0) staff       (20)      714 2022-08-20 05:44:48.000000 nebulae-0.6.4/nebulae/astro/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2740 2023-02-22 10:00:25.000000 nebulae-0.6.4/nebulae/astro/dock.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae/astro/hangar/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/
--rw-r--r--   0 root         (0) staff       (20)     1330 2022-10-26 12:11:07.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/gan.py
--rw-r--r--   0 root         (0) staff       (20)     1489 2020-11-18 08:18:05.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/wgan.py
--rw-r--r--   0 root         (0) staff       (20)     3571 2020-12-08 10:05:34.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/infogan.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:52.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    27430 2022-11-19 06:49:17.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1838 2021-02-09 08:51:42.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/biggan.py
--rw-r--r--   0 root         (0) staff       (20)     1378 2022-10-26 12:57:19.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/dcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1914 2022-11-19 03:39:59.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/wgan_div.py
--rw-r--r--   0 root         (0) staff       (20)     1384 2020-11-18 08:16:31.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/fcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1912 2022-11-19 07:00:35.000000 nebulae-0.6.4/nebulae/astro/hangar/GAN/resgan.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae/astro/hangar/Classic/
--rw-r--r--   0 root         (0) staff       (20)     3916 2022-08-20 12:56:43.000000 nebulae-0.6.4/nebulae/astro/hangar/Classic/vgg.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:37.000000 nebulae-0.6.4/nebulae/astro/hangar/Classic/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4998 2022-11-03 08:01:22.000000 nebulae-0.6.4/nebulae/astro/hangar/Classic/resnet.py
--rw-r--r--   0 root         (0) staff       (20)     1267 2023-02-22 11:57:27.000000 nebulae-0.6.4/nebulae/astro/hangar/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/astro/hangar/Seq2Seq/
--rw-r--r--   0 root         (0) staff       (20)      667 2021-05-22 03:22:45.000000 nebulae-0.6.4/nebulae/astro/hangar/Seq2Seq/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6860 2021-06-28 07:36:00.000000 nebulae-0.6.4/nebulae/astro/hangar/Seq2Seq/architect.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:35.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/
--rw-r--r--   0 root         (0) staff       (20)     1077 2023-01-27 08:47:47.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/resvae.py
--rw-r--r--   0 root         (0) staff       (20)      666 2022-11-03 11:54:33.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1091 2022-11-08 12:17:50.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/dcvae.py
--rw-r--r--   0 root         (0) staff       (20)    21531 2023-02-23 04:46:05.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1178 2023-02-22 13:00:49.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/vqvae.py
--rw-r--r--   0 root         (0) staff       (20)     1070 2022-11-08 12:17:50.000000 nebulae-0.6.4/nebulae/astro/hangar/VAE/vae.py
--rw-r--r--   0 root         (0) staff       (20)    16730 2023-02-28 03:48:35.000000 nebulae-0.6.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1073 2018-11-04 13:15:50.000000 nebulae-0.6.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    15157 2023-02-23 07:26:15.000000 nebulae-0.6.4/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    16730 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1507 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)      114 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-02-28 03:48:34.000000 nebulae-0.6.4/nebulae.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-02-28 03:48:35.000000 nebulae-0.6.4/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/fuel/
+-rw-r--r--   0 root         (0) staff       (20)     1005 2022-08-20 04:55:27.000000 nebulae-0.6.5/nebulae/fuel/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9783 2022-08-20 04:52:42.000000 nebulae-0.6.5/nebulae/fuel/generator.py
+-rw-r--r--   0 root         (0) staff       (20)    37708 2023-01-30 13:19:41.000000 nebulae-0.6.5/nebulae/fuel/comburant.py
+-rw-r--r--   0 root         (0) staff       (20)     7790 2022-11-01 09:29:19.000000 nebulae-0.6.5/nebulae/fuel/tank.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/law/
+-rw-r--r--   0 root         (0) staff       (20)      698 2021-09-14 09:32:19.000000 nebulae-0.6.5/nebulae/law/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      928 2020-10-20 09:25:06.000000 nebulae-0.6.5/nebulae/law/constant.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/kit/
+-rw-r--r--   0 root         (0) staff       (20)     1362 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/kit/decorator.py
+-rw-r--r--   0 root         (0) staff       (20)    25772 2022-11-04 03:44:29.000000 nebulae-0.6.5/nebulae/kit/utility.py
+-rw-r--r--   0 root         (0) staff       (20)     1096 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/kit/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      862 2022-07-22 10:10:53.000000 nebulae-0.6.5/nebulae/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/cockpit/
+-rw-r--r--   0 root         (0) staff       (20)     3516 2022-08-06 07:48:20.000000 nebulae-0.6.5/nebulae/cockpit/time_machine.py
+-rw-r--r--   0 root         (0) staff       (20)     5219 2022-09-16 14:43:52.000000 nebulae-0.6.5/nebulae/cockpit/multiverse.py
+-rw-r--r--   0 root         (0) staff       (20)      843 2022-08-06 09:24:38.000000 nebulae-0.6.5/nebulae/cockpit/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4251 2022-09-06 15:10:12.000000 nebulae-0.6.5/nebulae/cockpit/engine.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/aerolog/
+-rw-r--r--   0 root         (0) staff       (20)     6383 2023-04-29 13:28:54.000000 nebulae-0.6.5/nebulae/aerolog/inspector.py
+-rw-r--r--   0 root         (0) staff       (20)      733 2023-04-21 11:05:32.000000 nebulae-0.6.5/nebulae/aerolog/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13935 2023-04-21 08:53:35.000000 nebulae-0.6.5/nebulae/aerolog/dashboard.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/
+-rw-r--r--   0 root         (0) staff       (20)    74885 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/astro/craft.py
+-rw-r--r--   0 root         (0) staff       (20)      735 2023-04-27 15:32:39.000000 nebulae-0.6.5/nebulae/astro/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3187 2023-04-27 15:32:39.000000 nebulae-0.6.5/nebulae/astro/dock.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/
+-rw-r--r--   0 root         (0) staff       (20)     1330 2022-10-26 12:11:07.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/gan.py
+-rw-r--r--   0 root         (0) staff       (20)     1489 2020-11-18 08:18:05.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan.py
+-rw-r--r--   0 root         (0) staff       (20)     3571 2020-12-08 10:05:34.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/infogan.py
+-rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:52.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    27430 2022-11-19 06:49:17.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/architect.py
+-rw-r--r--   0 root         (0) staff       (20)     1838 2021-02-09 08:51:42.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/biggan.py
+-rw-r--r--   0 root         (0) staff       (20)     1378 2022-10-26 12:57:19.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/dcgan.py
+-rw-r--r--   0 root         (0) staff       (20)     1914 2022-11-19 03:39:59.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan_div.py
+-rw-r--r--   0 root         (0) staff       (20)     1384 2020-11-18 08:16:31.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/fcgan.py
+-rw-r--r--   0 root         (0) staff       (20)     1912 2022-11-19 07:00:35.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/resgan.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/
+-rw-r--r--   0 root         (0) staff       (20)     3916 2022-08-20 12:56:43.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/vgg.py
+-rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:37.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4998 2022-11-03 08:01:22.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/resnet.py
+-rw-r--r--   0 root         (0) staff       (20)     1267 2023-02-22 11:57:27.000000 nebulae-0.6.5/nebulae/astro/hangar/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/
+-rw-r--r--   0 root         (0) staff       (20)      667 2021-05-22 03:22:45.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6860 2021-06-28 07:36:00.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/architect.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/
+-rw-r--r--   0 root         (0) staff       (20)     1077 2023-01-27 08:47:47.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/resvae.py
+-rw-r--r--   0 root         (0) staff       (20)      666 2022-11-03 11:54:33.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1091 2022-11-08 12:17:50.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/dcvae.py
+-rw-r--r--   0 root         (0) staff       (20)    21531 2023-02-23 04:46:05.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/architect.py
+-rw-r--r--   0 root         (0) staff       (20)     1813 2023-04-29 13:26:32.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/vqvae.py
+-rw-r--r--   0 root         (0) staff       (20)     1070 2022-11-08 12:17:50.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/vae.py
+-rw-r--r--   0 root         (0) staff       (20)    16716 2023-04-29 13:30:01.000000 nebulae-0.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1073 2018-11-04 13:15:50.000000 nebulae-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    15344 2023-04-21 08:54:51.000000 nebulae-0.6.5/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    16716 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1474 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)      114 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-29 13:30:01.000000 nebulae-0.6.5/setup.cfg
```

### Comparing `nebulae-0.6.4/nebulae/fuel/__init__.py` & `nebulae-0.6.5/nebulae/fuel/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/fuel/generator.py` & `nebulae-0.6.5/nebulae/fuel/generator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/fuel/comburant.py` & `nebulae-0.6.5/nebulae/fuel/comburant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/fuel/tank.py` & `nebulae-0.6.5/nebulae/fuel/tank.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/law/__init__.py` & `nebulae-0.6.5/nebulae/law/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/law/constant.py` & `nebulae-0.6.5/nebulae/law/constant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/kit/decorator.py` & `nebulae-0.6.5/nebulae/kit/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,26 @@
         if not isinstance(ret, tuple):
             ret = (ret,)
         return (_t - t_,) + ret
 
     return _wrapper
 
 
+# def Formula(fn):
+#     def _decorator(func):
+#         def _wrapper(*args, **kwargs):
+#             ret = func(*args, **kwargs)
+#             ret.pods = fn
+#             return ret
+#
+#         return _wrapper
+#
+#     return _decorator
+
+
 def SPST(func):
     def _wrapper(*args, **kwargs):
         cv2.setNumThreads(0)
         cv2.ocl.setUseOpenCL(False)
         return func(*args, **kwargs)
 
     return _wrapper
```

### Comparing `nebulae-0.6.4/nebulae/kit/utility.py` & `nebulae-0.6.5/nebulae/kit/utility.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/kit/__init__.py` & `nebulae-0.6.5/nebulae/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/__init__.py` & `nebulae-0.6.5/nebulae/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/cockpit/time_machine.py` & `nebulae-0.6.5/nebulae/cockpit/time_machine.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/cockpit/multiverse.py` & `nebulae-0.6.5/nebulae/cockpit/multiverse.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/cockpit/__init__.py` & `nebulae-0.6.5/nebulae/cockpit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/cockpit/engine.py` & `nebulae-0.6.5/nebulae/cockpit/engine.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/aerolog/__init__.py` & `nebulae-0.6.5/nebulae/astro/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 '''
 __init__
-Created by Seria at 30/11/2018 6:00 PM
+Created by Seria at 23/11/2018 10:30 AM
 Email: zzqsummerai@yeah.net
 
                     _ooOoo_
                   o888888888o
                  o88`_ . _`88o
                  (|  0   0  |)
                  O \   。   / O
@@ -18,10 +18,10 @@
          ,--- /   ___\<|>/___   \ ---,
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
-from .blueprint import BluePrint
-from .dashboard import DashBoard
-from .control_panel import CtrlPanel
+from .craft import Craft
+from .dock import fn
+from . import hangar
```

### Comparing `nebulae-0.6.4/nebulae/aerolog/dashboard.py` & `nebulae-0.6.5/nebulae/aerolog/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     def __init__(self, log_path='./aerolog', window=1, divisor=10, span=30, format=None):
         '''
         :param config:
         :param window: the window length of moving average
         :param format: a list of which the element is format and mode, e.g. ['3f', 'raw']
         '''
         self.rank = int(os.environ.get('RANK', -1))
-        assert len(format)<8, 'NEBULAE ERROR ⨷ there are at most 7 panels to monitor.'
         if not os.path.exists(log_path):
             os.mkdir(log_path)
         self.log_path = log_path
         self.window = window
         self.divisor = divisor
         self.span = span
         self.format = format
@@ -57,15 +56,15 @@
         self.win_mile = {}
         self.gauge_mile = {}
         self.gauge_epoch = {}
         self.trail_mile = {}
         self.trail_epoch = {}
         self.is_global = None
         self.is_elastic = None
-        self.panel = 0
+        self.ptr = 0
 
     def _getOridinal(self, number):
         remainder = number % 10
         if remainder == 1:
             ordinal = 'st'
         elif remainder == 2:
             ordinal = 'nd'
@@ -88,23 +87,25 @@
             return ''
         elif mode == 'tailor':
             string = form(value)
             return ' %s ➠ \033[1;36m%s\033[0m |' % (abbr, string)
         else:
             raise KeyError('%s is an illegal format option.' % mode)
 
-    def gauge(self, entry, mile, epoch, mpe, stage, interval=1, duration=None,
-              plot=True, flush=0, is_global=True, is_elastic=False):
+    def gauge(self, entry, mile, epoch, mpe, stage, interval=1, duration=None, plot=True, flush=0,
+              is_global=True, is_elastic=False, in_loop=(-1,), last_for=1):
         if self.rank>0:
             return
         epoch += 1
         mile += 1
         string_mile = ''
         flag_display = False
         flag_epoch_end = False
+        len_loop = len(in_loop)
+        assert in_loop[0]<0 or len_loop>1, 'NEBULAE ERROR ⨷ the dashboard should loop through more than one curve.'
         if mile % interval == 0:
             flag_display = True
         if mile % mpe == 0:
             flag_epoch_end = True
             if epoch > self.max_epoch:
                 self.max_epoch = epoch
             string_epoch = ''
@@ -163,19 +164,21 @@
 
         if flag_display:
             if len(self.gauge_mile) > 0 and len(entry)>0 and plot:
                 curve_exists = True
             else:
                 curve_exists = False
             if curve_exists:
-                data = np.array(self.gauge_mile[items[self.panel]])
+                if mile % (interval*last_for) == 0:
+                    self.ptr = (self.ptr + 1) % len_loop
+                data = np.array(self.gauge_mile[items[in_loop[self.ptr]]])
                 is_global = is_global if self.is_global is None else self.is_global
                 is_elastic = is_elastic if self.is_elastic is None else self.is_elastic
                 curve = curve2str(data, self.divisor, self.span, is_global, is_elastic,
-                                  x_title='step', y_title=items[self.panel] + 10*' ')
+                                  x_title='step', y_title=items[in_loop[self.ptr]] + 10*' ')
                 print(curve)
                 print(w * ' ', end='\r')
 
             ordinal = self._getOridinal(epoch)
             progress = int((mile - 1) / mpe * 20 + 0.4)
             yellow_bar = progress * ' '
             space_bar = (20 - progress) * ' '
```

### Comparing `nebulae-0.6.4/nebulae/astro/craft.py` & `nebulae-0.6.5/nebulae/astro/craft.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
 
 '''
 # -*- coding:utf-8 -*-
 from math import ceil, sqrt
 from functools import partial
-import os
 import sys
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ptflops.pytorch_engine import add_flops_counting_methods
 from ..cockpit.engine import Engine
 from ..cockpit import CPU, GPU
@@ -43,20 +42,20 @@
            'Mean', 'Max', 'Min', 'Argmax', 'Argmin', 'Maxele', 'Minele', 'Sum', 'Dot', 'Scatter', 'Gather', 'Grad',
            'QR', 'Eigen', 'MaxEigen', 'FFT', 'IFFT',
            'Roll', 'Reshape', 'Permute', 'Expand', 'Squash', 'Tile', 'Zoom', 'SubPix', 'SurPix', 'MaxPool', 'AvgPool',
            'EMA', 'Retroact',
            'Sqrt', 'Exp', 'Log', 'Sin', 'Cos',
            'Concat', 'Stack',
            'D2S', 'S2D', 'SpDot',
-           'Clip', 'Dropout', 'BN', 'CBN', 'IN', 'CIN', 'LN', 'SN',
+           'Clip', 'Dropout', 'BN', 'CBN', 'IN', 'CIN', 'LN', 'GN', 'SN',
            'Relu', 'LRelu', 'PRelu', 'Gelu', 'Tanh', 'Sigm', 'Sftm', 'Sftp',
            'MAE', 'MSE', 'Huber', 'Charbon', 'SigmXE', 'SftmXE', 'OHEM',
            'AccCls', 'PSNR', 'SSIM',
            'StepLR', 'PolyLR', 'CosLR', 'ExpLR', 'WavyLR',
-           'Momentum', 'Nesterov', 'RMSProp', 'Adam', 'AdamW', 'Lion')
+           'Momentum', 'Nesterov', 'RMSProp', 'Adam', 'AdamW', 'Lion', 'Lamb')
 
 
 
 NEAREST = 0
 LINEAR = 1
 CUBIC = 2
 AREA = 3
@@ -94,17 +93,16 @@
 
 
 
 class Craft(nn.Module):
     def __init__(self, scope):
         super(Craft, self).__init__()
         self.scope = scope
-        self.__pods = []
+        self.__fns = []
         self.__dict = {}
-        self.__formulated = False
 
     def run(self, *args, **kwargs):
         raise NotImplementedError
 
     def forward(self, *args, **kwargs):
         # assert all([isinstance(a, Tensor) for a in args])
         return self.run(*args, **kwargs)
@@ -143,81 +141,31 @@
         _ = flops_model(*dummy_args, **dummy_kwargs)
 
         flops_count, params_count = flops_model.compute_average_flops_cost()
         flops_model.stop_flops_count()
 
         return flops_count
 
-    def dissect(self, *dummy_args, **dummy_kwargs):
-        rank = int(os.environ.get('RANK', -1))
-        if rank > 0:
-            return
-        # TODO: draw architectures
-        if 'export_path' in dummy_kwargs.keys():
-            export_path = dummy_kwargs['export_path']
-            dummy_kwargs.pop('export_path')
-        else:
-            export_path = ''
-        if 'onnx_version' in dummy_kwargs.keys():
-            onnx_version = dummy_kwargs['onnx_version']
-            dummy_kwargs.pop('onnx_version')
-        else:
-            onnx_version = 9
-
-        nbytes = {torch.int8: 1, torch.int64: 8, torch.float16: 2, torch.float32: 4, torch.float64: 8}
-        parambytes = sum([p.numel() * nbytes[p.dtype] for p in self.vars()])
-        if parambytes<1024:
-            parambytes = '%6d B  ' % parambytes
-        elif parambytes<1048576:
-            parambytes = '%6.2f KB ' % (parambytes / 1024)
-        elif parambytes<1073741824:
-            parambytes = '%6.2f MiB' % (parambytes / 1048576)
-        else:
-            parambytes = '%6.2f GB ' % (parambytes / 1073741824)
-
-        flops = self._get_flops(*dummy_args, **dummy_kwargs)
-
-        if flops<1024:
-            flops = '%6d  ' % flops
-        elif flops<1048576:
-            flops = '%6.2f K' % (flops / 1024)
-        elif flops<1073741824:
-            flops = '%6.2f M' % (flops / 1048576)
-        elif flops<1099511627776:
-            flops = '%6.2f G' % (flops / 1073741824)
-        else:
-            flops = '%6.2f T' % (flops / 1099511627776)
-        print('+' + (len(self.scope) + 46) * '-' + '+')
-        print('| Craft-%s weighs \033[1;32m%s\033[0m with \033[1;32m%s\033[0m FLOPS |' % (self.scope, parambytes, flops))
-        print('+' + (len(self.scope) + 46) * '-' + '+')
-
-        # convert to onnx
-        if export_path:
-            dummies = dummy_args + tuple(dummy_kwargs.values())
-            torch.onnx.export(self, dummies, export_path, opset_version=onnx_version)
+    def formulate(self, *fns):
+        for f in fns:
+            self.__fns.append(f)
 
     @property
-    def pods(self):
-        return self.__pods
-
-    @pods.setter
-    def pods(self, pods):
-        if not self.__formulated:
-            self.__pods = pods
-            self.__formulated = True
+    def fns(self):
+        return self.__fns
 
     def __getitem__(self, key):
         paths = key.split('/')
         craft = self
         for p in paths[:-1]:
             craft = getattr(craft, p)
         if paths[-1] == '':
             return craft
         else:
-            return craft.__dict[paths[-1]]
+            return craft.__dict.get(paths[-1])
 
     def __setitem__(self, key, value):
         self.__dict[key] = value
 
 
 
 class Rudder(object):
@@ -1640,14 +1588,28 @@
 
     def run(self, x):
         y = self.norm(x)
         return y
 
 
 
+class GN(Craft):
+    def __init__(self, out_chs, ngroup, resilient=True, scope='GN'):
+        super(GN, self).__init__(scope)
+        self.norm = nn.GroupNorm(ngroup, out_chs, affine=resilient, eps=1e-5)
+
+    def weights(self):
+        return self.norm.weight
+
+    def run(self, x):
+        y = self.norm(x)
+        return y
+
+
+
 class SN(Craft):
     def __init__(self, craft, niters=3, eps=1e-12, pname='weight', scope='SN'):
         super(SN, self).__init__(scope)
         if isinstance(craft, (Conv, TransConv)):
             self.key = 'conv/'
             self.hull = craft[self.key]
         elif isinstance(craft, Dense):
@@ -2339,14 +2301,155 @@
         if lr_decay is None:
             self.lr_decay = None
             if warmup>0:
                 self.lr_decay = WarmUpWrapper(warmup, self.optz)
         else:
             self.lr_decay = lr_decay(self.optz)
             if warmup>0:
+                self.lr_decay = WarmUpWrapper(warmup, self.lr_decay)
+
+    def run(self, target):
+        self.optz.zero_grad()
+        target.backward()
+        self.cnt += 1
+        if self.cnt == self.grad_accum:
+            self.cnt = 0
+            self.optz.step()
+            if self.lr_decay is not None:
+                self.lr_decay.step()
+
+
+
+class _Lamb(torch.optim.Optimizer):
+    r"""Implements Lamb algorithm.
+    It has been proposed in `Large Batch Optimization for Deep Learning: Training BERT in 76 minutes`_.
+    Arguments:
+        params (iterable): iterable of parameters to optimize or dicts defining
+            parameter groups
+        lr (float, optional): learning rate (default: 1e-3)
+        betas (Tuple[float, float], optional): coefficients used for computing
+            running averages of gradient and its square (default: (0.9, 0.999))
+        eps (float, optional): term added to the denominator to improve
+            numerical stability (default: 1e-8)
+        weight_decay (float, optional): weight decay (L2 penalty) (default: 0)
+        adam (bool, optional): always use trust ratio = 1, which turns this into
+            Adam. Useful for comparison purposes.
+    .. _Large Batch Optimization for Deep Learning: Training BERT in 76 minutes:
+        https://arxiv.org/abs/1904.00962
+    """
+
+    def __init__(self, params, lr=1e-3, betas=(0.9, 0.999), eps=1e-6, weight_decay=0):
+        if not 0.0 <= lr:
+            raise ValueError("Invalid learning rate: {}".format(lr))
+        if not 0.0 <= eps:
+            raise ValueError("Invalid epsilon value: {}".format(eps))
+        if not 0.0 <= betas[0] < 1.0:
+            raise ValueError("Invalid beta parameter at index 0: {}".format(betas[0]))
+        if not 0.0 <= betas[1] < 1.0:
+            raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
+        defaults = dict(lr=lr, betas=betas, eps=eps,
+                        weight_decay=weight_decay)
+        super(_Lamb, self).__init__(params, defaults)
+
+    def step(self, closure=None):
+        """Performs a single optimization step.
+        Arguments:
+            closure (callable, optional): A closure that reevaluates the model
+                and returns the loss.
+        """
+        loss = None
+        if closure is not None:
+            loss = closure()
+
+        for group in self.param_groups:
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+                grad = p.grad.data
+                if grad.is_sparse:
+                    raise RuntimeError('Lamb does not support sparse gradients, consider SparseAdam instad.')
+
+                state = self.state[p]
+
+                # State initialization
+                if len(state) == 0:
+                    state['step'] = 0
+                    # Exponential moving average of gradient values
+                    state['exp_avg'] = torch.zeros_like(p.data)
+                    # Exponential moving average of squared gradient values
+                    state['exp_avg_sq'] = torch.zeros_like(p.data)
+
+                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
+                beta1, beta2 = group['betas']
+
+                state['step'] += 1
+
+                # Decay the first and second moment running average coefficient
+                # m_t
+                exp_avg.mul_(beta1).add_(grad, alpha=1 - beta1)
+                # v_t
+                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1 - beta2)
+
+                # Paper v3 does not use debiasing.
+                # bias_correction1 = 1 - beta1 ** state['step']
+                # bias_correction2 = 1 - beta2 ** state['step']
+                # Apply bias to lr to avoid broadcast.
+                step_size = group['lr'] # * math.sqrt(bias_correction2) / bias_correction1
+
+                weight_norm = p.data.pow(2).sum().sqrt().clamp(0, 10)
+
+                adam_step = exp_avg / exp_avg_sq.sqrt().add(group['eps'])
+                if group['weight_decay'] != 0:
+                    adam_step.add_(p.data, alpha=group['weight_decay'])
+
+                adam_norm = adam_step.pow(2).sum().sqrt()
+                if weight_norm == 0 or adam_norm == 0:
+                    trust_ratio = 1
+                else:
+                    trust_ratio = weight_norm / adam_norm
+                state['weight_norm'] = weight_norm
+                state['adam_norm'] = adam_norm
+                state['trust_ratio'] = trust_ratio
+
+                p.data.add_(adam_step, alpha=-step_size * trust_ratio)
+
+        return loss
+
+
+
+class Lamb(Craft):
+    def __init__(self, hull, lr, mmnt1=0.9, mmnt2=0.999, wd=0, lr_decay=None, warmup=0,
+                 grad_limit=-1, grad_accum=1, update_scope=None, scope='LION'):
+        super(Lamb, self).__init__(scope)
+        # select parameters await updating
+        if update_scope is None:
+            update_var = hull.parameters()
+        else:
+            if isinstance(update_scope, str):
+                update_scope = [update_scope]
+            update_var = []
+            for us in update_scope:
+                paths = us.split('/')
+                craft = hull
+                for p in paths:
+                    craft = getattr(craft, p)
+                update_var.append(craft.parameters())
+
+        self.grad_accum = grad_accum
+        self.cnt = 0
+        if grad_limit > 0:
+            nn.utils.clip_grad_value_(update_var, grad_limit)
+        self.optz = _Lamb(update_var, lr=lr, betas=(mmnt1, mmnt2), weight_decay=wd)
+        if lr_decay is None:
+            self.lr_decay = None
+            if warmup>0:
+                self.lr_decay = WarmUpWrapper(warmup, self.optz)
+        else:
+            self.lr_decay = lr_decay(self.optz)
+            if warmup>0:
                 self.lr_decay = WarmUpWrapper(warmup, self.lr_decay)
 
     def run(self, target):
         self.optz.zero_grad()
         target.backward()
         self.cnt += 1
         if self.cnt == self.grad_accum:
```

### Comparing `nebulae-0.6.4/nebulae/astro/__init__.py` & `nebulae-0.6.5/nebulae/aerolog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 '''
 __init__
-Created by Seria at 23/11/2018 10:30 AM
+Created by Seria at 30/11/2018 6:00 PM
 Email: zzqsummerai@yeah.net
 
                     _ooOoo_
                   o888888888o
                  o88`_ . _`88o
                  (|  0   0  |)
                  O \   。   / O
@@ -18,9 +18,9 @@
          ,--- /   ___\<|>/___   \ ---,
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
-from .craft import Craft
-from . import hangar
+from .inspector import Inspector
+from .dashboard import DashBoard
```

### Comparing `nebulae-0.6.4/nebulae/astro/dock.py` & `nebulae-0.6.5/nebulae/astro/dock.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,78 +18,87 @@
          ,--- /   ___\<|>/___   \ ---,
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
-from ..kit.utility import cap, autopad
-from collections import namedtuple
+from ..kit.utility import autopad, cap
 
-__all__ = ('Pod', 'Tensor', 'coat', 'shell', 'autopad')
+__all__ = ('coat', 'shell', 'autopad')
 
 from .craft import *
 from . import craft
 __all__ += craft.__all__
 
 
-Tensor = namedtuple('tensor', ('key', 'val'))
 def coat(datum, as_const=True, sync=True):
     raise NotImplementedError('NEBULAE ERROR ⨷ coat function becomes valid only after setting up an Engine.')
 
 def shell(datum, as_np=True, sync=False):
     raise NotImplementedError('NEBULAE ERROR ⨷ shell function becomes valid only after setting up an Engine.')
 
 
-class Pod():
-    def __init__(self, name, comp=[], symbol=''):
+class fn():
+    def __init__(self, name, comp=None, symbol=''):
         self.name = name
-        if len(comp)==0: # atomic pod
-            self.comp = comp
+        if comp is None: # atomic fn
+            self.comp = []
         else:
             assert len(comp)==2
             left_sym = comp[0].symbol
             right_sym = comp[1].symbol
             if left_sym == right_sym:
                 if right_sym=='':
                     self.comp = comp
                 else:
                     self.comp = comp[0].comp + comp[1].comp
             else:
                 if left_sym=='':
-                    self.comp = [comp[0]] + comp[1].comp
+                    if symbol==right_sym:
+                        self.comp = [comp[0]] + comp[1].comp
+                    else:
+                        self.comp = [comp[0], comp[1]]
                 elif right_sym=='':
-                    self.comp = comp[0].comp + [comp[1]]
+                    if symbol == left_sym:
+                        self.comp = comp[0].comp + [comp[1]]
+                    else:
+                        self.comp = [comp[0], comp[1]]
                 else:
-                    self.comp = comp
+                    if symbol == left_sym:
+                        self.comp = comp[0].comp + [comp[1]]
+                    elif symbol == right_sym:
+                        self.comp = [comp[0]] + comp[1].comp
+                    else:
+                        self.comp = comp
         self.symbol = symbol
 
 
-    def __gt__(self, other):
-        return Pod('', [self, other], '>')
+    def __rshift__(self, other): # cascade
+        return fn('', [self, other], '>')
 
-    def __add__(self, other):
-        return Pod('', [self, other], '+')
+    def __add__(self, other): # add
+        return fn('', [self, other], '+')
 
-    def __sub__(self, other):
-        return Pod('', [self, other], '-')
+    def __sub__(self, other): # sub
+        return fn('', [self, other], '-')
 
-    def __mul__(self, other):
-        return Pod('', [self, other], '*')
+    def __mul__(self, other): # multiply
+        return fn('', [self, other], '*')
 
-    def __matmul__(self, other):
-        return Pod('', [self, other], '@')
+    def __matmul__(self, other): # dot
+        return fn('', [self, other], '@')
 
-    def __and__(self, other):
-        return Pod('', [self, other], '&')
+    def __and__(self, other): # concat
+        return fn('', [self, other], '&')
 
     def __or__(self, other):
-        return Pod('', [self, other], '|')
+        return fn('', [self, other], '|')
 
-    def __xor__(self, other):
-        return Pod('', [self, other], '^')
+    def __xor__(self, other): # with
+        return fn('', [self, other], '^')
 
     def _cap(self, scope):
         if '/' not in self.name:
             self.name = cap(self.name, scope)
         for c in self.comp:
             c._cap(scope)
```

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/gan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/gan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/wgan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/infogan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/infogan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/__init__.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/architect.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/biggan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/biggan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/dcgan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/dcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/wgan_div.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan_div.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/fcgan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/fcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/GAN/resgan.py` & `nebulae-0.6.5/nebulae/astro/hangar/GAN/resgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/Classic/vgg.py` & `nebulae-0.6.5/nebulae/astro/hangar/Classic/vgg.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/Classic/__init__.py` & `nebulae-0.6.5/nebulae/astro/hangar/Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/Classic/resnet.py` & `nebulae-0.6.5/nebulae/astro/hangar/Classic/resnet.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/__init__.py` & `nebulae-0.6.5/nebulae/astro/hangar/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/Seq2Seq/__init__.py` & `nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/Seq2Seq/architect.py` & `nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/VAE/resvae.py` & `nebulae-0.6.5/nebulae/astro/hangar/VAE/resvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/VAE/__init__.py` & `nebulae-0.6.5/nebulae/astro/hangar/VAE/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/VAE/dcvae.py` & `nebulae-0.6.5/nebulae/astro/hangar/VAE/dcvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/VAE/architect.py` & `nebulae-0.6.5/nebulae/astro/hangar/VAE/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/nebulae/astro/hangar/VAE/vqvae.py` & `nebulae-0.6.5/nebulae/astro/hangar/VAE/vae.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,24 +19,23 @@
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 from ... import dock, Craft
-from .architect import ResVQE, ResVQD, VecQuant
+from .architect import MLPE, MLPD
 
 
 
-class VQVAE(Craft):
-    def __init__(self, in_shape, hidden_dim, ncodes, scope='VQVAE'):
-        super(VQVAE, self).__init__(scope)
-        self.E = ResVQE(in_shape, hidden_dim, ncodes)
-        self.D = ResVQD(in_shape, hidden_dim)
-        self.Q = VecQuant(ncodes, self.E.ochs[-1])
+
+
+class VAE(Craft):
+    def __init__(self, in_shape, hidden_dim, latent_dim, scope='VAE'):
+        super(VAE, self).__init__(scope)
+        self.E = MLPE(in_shape, hidden_dim, latent_dim)
+        self.D = MLPD(in_shape, hidden_dim, latent_dim)
 
     def run(self, x):
-        z = self.E(x)
-        q = self.Q(z)
-        s = dock.shell(q-z, as_np=False)
-        y = self.D(z+s)
-        return z, q, y
+        mu, lv, z = self.E(x)
+        y = self.D(z)
+        return mu, lv, y
```

### Comparing `nebulae-0.6.4/PKG-INFO` & `nebulae-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.4
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.4: DashBoard.log() now plots curves only by metrics; add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.
+Version: 0.6.5
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge; add Lamb optimizer; replace BluePrint module with Inspector.
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.4/LICENSE` & `nebulae-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.4/setup.py` & `nebulae-0.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 import setuptools
 
 with open("Nebulae_Brochure.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nebulae",
-    version="0.6.4",
+    version="0.6.5",
     author="Seria",
     author_email="zzqsummerai@yeah.net",
     description="A novel and simple framework based on prevalent DL frameworks and other image processing libs."
-                + " v0.6.4: DashBoard.log() now plots curves only by metrics;"
-                + " add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.",
+                + " v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge;"
+                + " add Lamb optimizer; replace BluePrint module with Inspector.",
+                # + " v0.6.4: DashBoard.log() now plots curves only by metrics;"
+                # + " add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.",
                 # + " v0.6.3: OHEM loss supports an additional mask as input.",
                 # + " v0.6.2: change plot tools from matplotlib to seaborn;"
                 # + " make Pooling modules compatible with symmetric padding;"
                 # + " add dock.Roll module.",
                 # + " v0.6.1: fix a bug of specifying cpu_prefetch in Tank unexpectedly;"
                 # + " add transmit argument in Depot.mount().",
                 # + " v0.6.0: support PyTorch only from now on and remove many redundant arguments and methods"
```

### Comparing `nebulae-0.6.4/nebulae.egg-info/PKG-INFO` & `nebulae-0.6.5/nebulae.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.4
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.4: DashBoard.log() now plots curves only by metrics; add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.
+Version: 0.6.5
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge; add Lamb optimizer; replace BluePrint module with Inspector.
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.4/nebulae.egg-info/SOURCES.txt` & `nebulae-0.6.5/nebulae.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 nebulae/__init__.py
 nebulae.egg-info/PKG-INFO
 nebulae.egg-info/SOURCES.txt
 nebulae.egg-info/dependency_links.txt
 nebulae.egg-info/requires.txt
 nebulae.egg-info/top_level.txt
 nebulae/aerolog/__init__.py
-nebulae/aerolog/blueprint.py
-nebulae/aerolog/control_panel.py
 nebulae/aerolog/dashboard.py
+nebulae/aerolog/inspector.py
 nebulae/astro/__init__.py
 nebulae/astro/craft.py
 nebulae/astro/dock.py
 nebulae/astro/hangar/__init__.py
 nebulae/astro/hangar/Classic/__init__.py
 nebulae/astro/hangar/Classic/resnet.py
 nebulae/astro/hangar/Classic/vgg.py
```

