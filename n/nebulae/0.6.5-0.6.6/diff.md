# Comparing `tmp/nebulae-0.6.5.tar.gz` & `tmp/nebulae-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nebulae-0.6.5.tar", last modified: Sat Apr 29 13:30:01 2023, max compression
+gzip compressed data, was "dist/nebulae-0.6.6.tar", last modified: Sat Apr 29 14:57:00 2023, max compression
```

## Comparing `nebulae-0.6.5.tar` & `nebulae-0.6.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/fuel/
--rw-r--r--   0 root         (0) staff       (20)     1005 2022-08-20 04:55:27.000000 nebulae-0.6.5/nebulae/fuel/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9783 2022-08-20 04:52:42.000000 nebulae-0.6.5/nebulae/fuel/generator.py
--rw-r--r--   0 root         (0) staff       (20)    37708 2023-01-30 13:19:41.000000 nebulae-0.6.5/nebulae/fuel/comburant.py
--rw-r--r--   0 root         (0) staff       (20)     7790 2022-11-01 09:29:19.000000 nebulae-0.6.5/nebulae/fuel/tank.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/law/
--rw-r--r--   0 root         (0) staff       (20)      698 2021-09-14 09:32:19.000000 nebulae-0.6.5/nebulae/law/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      928 2020-10-20 09:25:06.000000 nebulae-0.6.5/nebulae/law/constant.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/kit/
--rw-r--r--   0 root         (0) staff       (20)     1362 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/kit/decorator.py
--rw-r--r--   0 root         (0) staff       (20)    25772 2022-11-04 03:44:29.000000 nebulae-0.6.5/nebulae/kit/utility.py
--rw-r--r--   0 root         (0) staff       (20)     1096 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/kit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      862 2022-07-22 10:10:53.000000 nebulae-0.6.5/nebulae/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/cockpit/
--rw-r--r--   0 root         (0) staff       (20)     3516 2022-08-06 07:48:20.000000 nebulae-0.6.5/nebulae/cockpit/time_machine.py
--rw-r--r--   0 root         (0) staff       (20)     5219 2022-09-16 14:43:52.000000 nebulae-0.6.5/nebulae/cockpit/multiverse.py
--rw-r--r--   0 root         (0) staff       (20)      843 2022-08-06 09:24:38.000000 nebulae-0.6.5/nebulae/cockpit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4251 2022-09-06 15:10:12.000000 nebulae-0.6.5/nebulae/cockpit/engine.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/aerolog/
--rw-r--r--   0 root         (0) staff       (20)     6383 2023-04-29 13:28:54.000000 nebulae-0.6.5/nebulae/aerolog/inspector.py
--rw-r--r--   0 root         (0) staff       (20)      733 2023-04-21 11:05:32.000000 nebulae-0.6.5/nebulae/aerolog/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13935 2023-04-21 08:53:35.000000 nebulae-0.6.5/nebulae/aerolog/dashboard.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/
--rw-r--r--   0 root         (0) staff       (20)    74885 2023-04-29 13:24:36.000000 nebulae-0.6.5/nebulae/astro/craft.py
--rw-r--r--   0 root         (0) staff       (20)      735 2023-04-27 15:32:39.000000 nebulae-0.6.5/nebulae/astro/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3187 2023-04-27 15:32:39.000000 nebulae-0.6.5/nebulae/astro/dock.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/
--rw-r--r--   0 root         (0) staff       (20)     1330 2022-10-26 12:11:07.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/gan.py
--rw-r--r--   0 root         (0) staff       (20)     1489 2020-11-18 08:18:05.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan.py
--rw-r--r--   0 root         (0) staff       (20)     3571 2020-12-08 10:05:34.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/infogan.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:52.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    27430 2022-11-19 06:49:17.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1838 2021-02-09 08:51:42.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/biggan.py
--rw-r--r--   0 root         (0) staff       (20)     1378 2022-10-26 12:57:19.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/dcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1914 2022-11-19 03:39:59.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan_div.py
--rw-r--r--   0 root         (0) staff       (20)     1384 2020-11-18 08:16:31.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/fcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1912 2022-11-19 07:00:35.000000 nebulae-0.6.5/nebulae/astro/hangar/GAN/resgan.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/
--rw-r--r--   0 root         (0) staff       (20)     3916 2022-08-20 12:56:43.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/vgg.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:37.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4998 2022-11-03 08:01:22.000000 nebulae-0.6.5/nebulae/astro/hangar/Classic/resnet.py
--rw-r--r--   0 root         (0) staff       (20)     1267 2023-02-22 11:57:27.000000 nebulae-0.6.5/nebulae/astro/hangar/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/
--rw-r--r--   0 root         (0) staff       (20)      667 2021-05-22 03:22:45.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6860 2021-06-28 07:36:00.000000 nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/architect.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/
--rw-r--r--   0 root         (0) staff       (20)     1077 2023-01-27 08:47:47.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/resvae.py
--rw-r--r--   0 root         (0) staff       (20)      666 2022-11-03 11:54:33.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1091 2022-11-08 12:17:50.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/dcvae.py
--rw-r--r--   0 root         (0) staff       (20)    21531 2023-02-23 04:46:05.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1813 2023-04-29 13:26:32.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/vqvae.py
--rw-r--r--   0 root         (0) staff       (20)     1070 2022-11-08 12:17:50.000000 nebulae-0.6.5/nebulae/astro/hangar/VAE/vae.py
--rw-r--r--   0 root         (0) staff       (20)    16716 2023-04-29 13:30:01.000000 nebulae-0.6.5/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1073 2018-11-04 13:15:50.000000 nebulae-0.6.5/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    15344 2023-04-21 08:54:51.000000 nebulae-0.6.5/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    16716 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1474 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)      114 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-29 13:30:01.000000 nebulae-0.6.5/nebulae.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-29 13:30:01.000000 nebulae-0.6.5/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/fuel/
+-rw-r--r--   0 root         (0) staff       (20)     1005 2022-08-20 04:55:27.000000 nebulae-0.6.6/nebulae/fuel/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9783 2022-08-20 04:52:42.000000 nebulae-0.6.6/nebulae/fuel/generator.py
+-rw-r--r--   0 root         (0) staff       (20)    37708 2023-01-30 13:19:41.000000 nebulae-0.6.6/nebulae/fuel/comburant.py
+-rw-r--r--   0 root         (0) staff       (20)     7790 2022-11-01 09:29:19.000000 nebulae-0.6.6/nebulae/fuel/tank.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/law/
+-rw-r--r--   0 root         (0) staff       (20)      698 2021-09-14 09:32:19.000000 nebulae-0.6.6/nebulae/law/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      928 2020-10-20 09:25:06.000000 nebulae-0.6.6/nebulae/law/constant.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/kit/
+-rw-r--r--   0 root         (0) staff       (20)     1362 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/kit/decorator.py
+-rw-r--r--   0 root         (0) staff       (20)    25772 2022-11-04 03:44:29.000000 nebulae-0.6.6/nebulae/kit/utility.py
+-rw-r--r--   0 root         (0) staff       (20)     1096 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/kit/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      862 2022-07-22 10:10:53.000000 nebulae-0.6.6/nebulae/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/cockpit/
+-rw-r--r--   0 root         (0) staff       (20)     3516 2022-08-06 07:48:20.000000 nebulae-0.6.6/nebulae/cockpit/time_machine.py
+-rw-r--r--   0 root         (0) staff       (20)     5219 2022-09-16 14:43:52.000000 nebulae-0.6.6/nebulae/cockpit/multiverse.py
+-rw-r--r--   0 root         (0) staff       (20)      843 2022-08-06 09:24:38.000000 nebulae-0.6.6/nebulae/cockpit/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4251 2022-09-06 15:10:12.000000 nebulae-0.6.6/nebulae/cockpit/engine.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/aerolog/
+-rw-r--r--   0 root         (0) staff       (20)     6383 2023-04-29 13:28:54.000000 nebulae-0.6.6/nebulae/aerolog/inspector.py
+-rw-r--r--   0 root         (0) staff       (20)      733 2023-04-21 11:05:32.000000 nebulae-0.6.6/nebulae/aerolog/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    14070 2023-04-29 14:54:27.000000 nebulae-0.6.6/nebulae/aerolog/dashboard.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/
+-rw-r--r--   0 root         (0) staff       (20)    74885 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/astro/craft.py
+-rw-r--r--   0 root         (0) staff       (20)      735 2023-04-27 15:32:39.000000 nebulae-0.6.6/nebulae/astro/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3187 2023-04-27 15:32:39.000000 nebulae-0.6.6/nebulae/astro/dock.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/
+-rw-r--r--   0 root         (0) staff       (20)     1330 2022-10-26 12:11:07.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/gan.py
+-rw-r--r--   0 root         (0) staff       (20)     1489 2020-11-18 08:18:05.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan.py
+-rw-r--r--   0 root         (0) staff       (20)     3571 2020-12-08 10:05:34.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/infogan.py
+-rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:52.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    27430 2022-11-19 06:49:17.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/architect.py
+-rw-r--r--   0 root         (0) staff       (20)     1838 2021-02-09 08:51:42.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/biggan.py
+-rw-r--r--   0 root         (0) staff       (20)     1378 2022-10-26 12:57:19.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/dcgan.py
+-rw-r--r--   0 root         (0) staff       (20)     1914 2022-11-19 03:39:59.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan_div.py
+-rw-r--r--   0 root         (0) staff       (20)     1384 2020-11-18 08:16:31.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/fcgan.py
+-rw-r--r--   0 root         (0) staff       (20)     1912 2022-11-19 07:00:35.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/resgan.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/
+-rw-r--r--   0 root         (0) staff       (20)     3916 2022-08-20 12:56:43.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/vgg.py
+-rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:37.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4998 2022-11-03 08:01:22.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/resnet.py
+-rw-r--r--   0 root         (0) staff       (20)     1267 2023-02-22 11:57:27.000000 nebulae-0.6.6/nebulae/astro/hangar/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/
+-rw-r--r--   0 root         (0) staff       (20)      667 2021-05-22 03:22:45.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6860 2021-06-28 07:36:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/architect.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/
+-rw-r--r--   0 root         (0) staff       (20)     1077 2023-01-27 08:47:47.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/resvae.py
+-rw-r--r--   0 root         (0) staff       (20)      666 2022-11-03 11:54:33.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1091 2022-11-08 12:17:50.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/dcvae.py
+-rw-r--r--   0 root         (0) staff       (20)    21531 2023-02-23 04:46:05.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/architect.py
+-rw-r--r--   0 root         (0) staff       (20)     1813 2023-04-29 14:48:07.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/vqvae.py
+-rw-r--r--   0 root         (0) staff       (20)     1070 2022-11-08 12:17:50.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/vae.py
+-rw-r--r--   0 root         (0) staff       (20)    16636 2023-04-29 14:57:00.000000 nebulae-0.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1073 2018-11-04 13:15:50.000000 nebulae-0.6.6/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    15430 2023-04-29 14:56:45.000000 nebulae-0.6.6/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    16636 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1474 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)      114 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-29 14:57:00.000000 nebulae-0.6.6/setup.cfg
```

### Comparing `nebulae-0.6.5/nebulae/fuel/__init__.py` & `nebulae-0.6.6/nebulae/fuel/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/fuel/generator.py` & `nebulae-0.6.6/nebulae/fuel/generator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/fuel/comburant.py` & `nebulae-0.6.6/nebulae/fuel/comburant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/fuel/tank.py` & `nebulae-0.6.6/nebulae/fuel/tank.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/law/__init__.py` & `nebulae-0.6.6/nebulae/law/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/law/constant.py` & `nebulae-0.6.6/nebulae/law/constant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/kit/decorator.py` & `nebulae-0.6.6/nebulae/kit/decorator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/kit/utility.py` & `nebulae-0.6.6/nebulae/kit/utility.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/kit/__init__.py` & `nebulae-0.6.6/nebulae/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/__init__.py` & `nebulae-0.6.6/nebulae/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/cockpit/time_machine.py` & `nebulae-0.6.6/nebulae/cockpit/time_machine.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/cockpit/multiverse.py` & `nebulae-0.6.6/nebulae/cockpit/multiverse.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/cockpit/__init__.py` & `nebulae-0.6.6/nebulae/cockpit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/cockpit/engine.py` & `nebulae-0.6.6/nebulae/cockpit/engine.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/aerolog/inspector.py` & `nebulae-0.6.6/nebulae/aerolog/inspector.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/aerolog/__init__.py` & `nebulae-0.6.6/nebulae/aerolog/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/aerolog/dashboard.py` & `nebulae-0.6.6/nebulae/aerolog/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,21 +164,25 @@
 
         if flag_display:
             if len(self.gauge_mile) > 0 and len(entry)>0 and plot:
                 curve_exists = True
             else:
                 curve_exists = False
             if curve_exists:
-                if mile % (interval*last_for) == 0:
-                    self.ptr = (self.ptr + 1) % len_loop
-                data = np.array(self.gauge_mile[items[in_loop[self.ptr]]])
+                if len_loop > 1:
+                    if mile % (interval*last_for) == 0:
+                        self.ptr = (self.ptr + 1) % len_loop
+                    metric_idx = in_loop[self.ptr]
+                else:
+                    metric_idx = 0
+                data = np.array(self.gauge_mile[items[metric_idx]])
                 is_global = is_global if self.is_global is None else self.is_global
                 is_elastic = is_elastic if self.is_elastic is None else self.is_elastic
                 curve = curve2str(data, self.divisor, self.span, is_global, is_elastic,
-                                  x_title='step', y_title=items[in_loop[self.ptr]] + 10*' ')
+                                  x_title='step', y_title=items[metric_idx] + 10*' ')
                 print(curve)
                 print(w * ' ', end='\r')
 
             ordinal = self._getOridinal(epoch)
             progress = int((mile - 1) / mpe * 20 + 0.4)
             yellow_bar = progress * ' '
             space_bar = (20 - progress) * ' '
```

### Comparing `nebulae-0.6.5/nebulae/astro/craft.py` & `nebulae-0.6.6/nebulae/astro/craft.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/__init__.py` & `nebulae-0.6.6/nebulae/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/dock.py` & `nebulae-0.6.6/nebulae/astro/dock.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/gan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/gan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/infogan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/infogan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/__init__.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/architect.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/biggan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/biggan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/dcgan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/dcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/wgan_div.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan_div.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/fcgan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/fcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/GAN/resgan.py` & `nebulae-0.6.6/nebulae/astro/hangar/GAN/resgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/Classic/vgg.py` & `nebulae-0.6.6/nebulae/astro/hangar/Classic/vgg.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/Classic/__init__.py` & `nebulae-0.6.6/nebulae/astro/hangar/Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/Classic/resnet.py` & `nebulae-0.6.6/nebulae/astro/hangar/Classic/resnet.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/__init__.py` & `nebulae-0.6.6/nebulae/astro/hangar/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/__init__.py` & `nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/Seq2Seq/architect.py` & `nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/resvae.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/resvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/__init__.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/dcvae.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/dcvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/architect.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/vqvae.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/vqvae.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,14 @@
     def run(self, x):
         self['input'] = x
         self['encoded'] = self.E(self['input'])
         self['quantized'] = self.Q(self['encoded'])
         self['detached'] = dock.shell(self['quantized'] - self['encoded'], as_np=False)
         self['vector'] = self['encoded'] + self['detached']
         self['output'] = self.D(self['vector'])
-        return self['encoded'], self['quantized'], self['vector']
+        return self['encoded'], self['quantized'], self['output']
 
         # z = self.E(x)
         # q = self.Q(z)
         # s = dock.shell(q-z, as_np=False)
         # y = self.D(z+s)
         # return z, q, y
```

### Comparing `nebulae-0.6.5/nebulae/astro/hangar/VAE/vae.py` & `nebulae-0.6.6/nebulae/astro/hangar/VAE/vae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/PKG-INFO` & `nebulae-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.5
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge; add Lamb optimizer; replace BluePrint module with Inspector.
+Version: 0.6.6
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.6: add in_loop and last_for args in DashBoard.gauge().
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.5/LICENSE` & `nebulae-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.5/setup.py` & `nebulae-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 import setuptools
 
 with open("Nebulae_Brochure.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nebulae",
-    version="0.6.5",
+    version="0.6.6",
     author="Seria",
     author_email="zzqsummerai@yeah.net",
     description="A novel and simple framework based on prevalent DL frameworks and other image processing libs."
-                + " v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge;"
-                + " add Lamb optimizer; replace BluePrint module with Inspector.",
+                + " v0.6.6: add in_loop and last_for args in DashBoard.gauge().",
+                # + " v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge;"
+                # + " add Lamb optimizer; replace BluePrint module with Inspector.",
                 # + " v0.6.4: DashBoard.log() now plots curves only by metrics;"
                 # + " add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.",
                 # + " v0.6.3: OHEM loss supports an additional mask as input.",
                 # + " v0.6.2: change plot tools from matplotlib to seaborn;"
                 # + " make Pooling modules compatible with symmetric padding;"
                 # + " add dock.Roll module.",
                 # + " v0.6.1: fix a bug of specifying cpu_prefetch in Tank unexpectedly;"
```

### Comparing `nebulae-0.6.5/nebulae.egg-info/PKG-INFO` & `nebulae-0.6.6/nebulae.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.5
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge; add Lamb optimizer; replace BluePrint module with Inspector.
+Version: 0.6.6
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.6: add in_loop and last_for args in DashBoard.gauge().
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nebulae-0.6.5/nebulae.egg-info/SOURCES.txt` & `nebulae-0.6.6/nebulae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

