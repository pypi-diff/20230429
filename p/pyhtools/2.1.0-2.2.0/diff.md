# Comparing `tmp/pyhtools-2.1.0.tar.gz` & `tmp/pyhtools-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.1.0.tar", max compression
+gzip compressed data, was "pyhtools-2.2.0.tar", max compression
```

## Comparing `pyhtools-2.1.0.tar` & `pyhtools-2.2.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
--rw-r--r--   0        0        0     1092 2023-03-07 16:09:27.046239 pyhtools-2.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.062006 pyhtools-2.1.0/pyhtools/__init__.py
--rw-r--r--   0        0        0      107 2023-03-07 16:09:27.062006 pyhtools-2.1.0/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.069042 pyhtools-2.1.0/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.063003 pyhtools-2.1.0/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0     2815 2023-03-07 16:09:27.063003 pyhtools-2.1.0/pyhtools/attackers/Android/forensics/data_harvestor.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.064027 pyhtools-2.1.0/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     5037 2023-03-07 16:09:27.064685 pyhtools-2.1.0/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      422 2023-03-07 16:09:27.064685 pyhtools-2.1.0/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0     4784 2023-03-07 16:09:27.070042 pyhtools-2.1.0/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.065686 pyhtools-2.1.0/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     5114 2023-03-07 16:09:27.065686 pyhtools-2.1.0/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4404 2023-03-07 16:09:27.065686 pyhtools-2.1.0/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3591 2023-03-07 16:09:27.067036 pyhtools-2.1.0/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     4730 2023-03-07 16:09:27.067036 pyhtools-2.1.0/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     3921 2023-03-07 16:09:27.067036 pyhtools-2.1.0/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2290 2023-03-07 16:09:27.068136 pyhtools-2.1.0/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     2050 2023-03-07 16:09:27.068136 pyhtools-2.1.0/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2680 2023-03-07 16:09:27.069042 pyhtools-2.1.0/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     5501 2023-03-07 16:09:27.069042 pyhtools-2.1.0/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.070042 pyhtools-2.1.0/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.071039 pyhtools-2.1.0/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     5177 2023-03-07 16:09:27.071039 pyhtools-2.1.0/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     2280 2023-03-07 16:09:27.072037 pyhtools-2.1.0/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     1984 2023-03-07 16:09:27.072037 pyhtools-2.1.0/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1123 2023-03-07 16:09:27.072037 pyhtools-2.1.0/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     2843 2023-03-07 16:09:27.073034 pyhtools-2.1.0/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     3279 2023-03-07 16:09:27.074208 pyhtools-2.1.0/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.074795 pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     6440 2023-03-07 16:09:27.074795 pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2174 2023-03-07 16:09:27.074795 pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0     2888 2023-03-07 16:09:27.074795 pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.075794 pyhtools-2.1.0/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     1737 2023-03-07 16:09:27.075794 pyhtools-2.1.0/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     1856 2023-03-07 16:09:27.077024 pyhtools-2.1.0/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.077024 pyhtools-2.1.0/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3454 2023-03-07 16:09:27.078520 pyhtools-2.1.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2347 2023-03-07 16:09:27.078520 pyhtools-2.1.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1908 2023-03-07 16:09:27.079531 pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1681 2023-03-07 16:09:27.079531 pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     5013 2023-03-07 16:09:27.079531 pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2295 2023-03-07 16:09:27.080531 pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.080531 pyhtools-2.1.0/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1619 2023-03-07 16:09:27.080531 pyhtools-2.1.0/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.082254 pyhtools-2.1.0/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2700 2023-03-07 16:09:27.082254 pyhtools-2.1.0/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.085474 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.083260 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1387 2023-03-07 16:09:27.083260 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1189 2023-03-07 16:09:27.083260 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.086532 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5175 2023-03-07 16:09:27.086532 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.084692 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5431 2023-03-07 16:09:27.084692 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5939 2023-03-07 16:09:27.085474 pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.087965 pyhtools-2.1.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     4503 2023-03-07 16:09:27.087965 pyhtools-2.1.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0     2681 2023-03-07 16:09:27.087965 pyhtools-2.1.0/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.089037 pyhtools-2.1.0/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.089037 pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2203 2023-03-07 16:09:27.090107 pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2306 2023-03-07 16:09:27.090107 pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0     1105 2023-03-07 16:09:27.089037 pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.090107 pyhtools-2.1.0/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3993 2023-03-07 16:09:27.091218 pyhtools-2.1.0/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0        0 2023-03-07 16:09:27.060998 pyhtools-2.1.0/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      292 2023-03-07 16:09:27.060998 pyhtools-2.1.0/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     5618 2023-03-07 16:09:27.062006 pyhtools-2.1.0/pyhtools/UI/functions.py
--rw-r--r--   0        0        0      549 2023-03-07 16:09:27.091820 pyhtools-2.1.0/pyhtools/utils.py
--rw-r--r--   0        0        0     1588 2023-03-07 17:58:35.442492 pyhtools-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6989 2023-03-07 17:55:08.167343 pyhtools-2.1.0/README.md
--rw-r--r--   0        0        0     9567 1970-01-01 00:00:00.000000 pyhtools-2.1.0/setup.py
--rw-r--r--   0        0        0     8824 1970-01-01 00:00:00.000000 pyhtools-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-25 17:42:54.251011 pyhtools-2.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-25 18:13:37.104832 pyhtools-2.2.0/pyhtools/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-25 17:59:09.458258 pyhtools-2.2.0/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0     2815 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/forensics/data_harvestor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     5037 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      422 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0     4784 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     5151 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4404 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3591 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     4730 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     3921 2023-04-25 17:42:54.264974 pyhtools-2.2.0/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2290 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     2068 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2680 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     5501 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     5177 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     2280 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     1984 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1123 2023-04-25 17:42:54.268556 pyhtools-2.2.0/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     2843 2023-04-25 17:42:54.268556 pyhtools-2.2.0/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     3279 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     6440 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2174 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0     2888 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     1737 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     1856 2023-04-25 17:42:54.271295 pyhtools-2.2.0/pyhtools/evil_files/exec_generator.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.271295 pyhtools-2.2.0/pyhtools/evil_files/malwares/__init__.py
+-rw-r--r--   0        0        0     3454 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     2347 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
+-rw-r--r--   0        0        0     1908 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
+-rw-r--r--   0        0        0     1681 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
+-rw-r--r--   0        0        0     5013 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
+-rw-r--r--   0        0        0     2295 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/__init__.py
+-rw-r--r--   0        0        0     1619 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/cert.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/keylogger.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
+-rw-r--r--   0        0        0     1189 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.277282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
+-rw-r--r--   0        0        0     5175 2023-04-25 17:42:54.277282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
+-rw-r--r--   0        0        0     5408 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
+-rw-r--r--   0        0        0     5939 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
+-rw-r--r--   0        0        0     4503 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
+-rw-r--r--   0        0        0     2681 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/__init__.py
+-rw-r--r--   0        0        0     2203 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
+-rw-r--r--   0        0        0     2306 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
+-rw-r--r--   0        0        0     1105 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/worms/__init__.py
+-rw-r--r--   0        0        0     3993 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/worms/dir_cloner.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.259994 pyhtools-2.2.0/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-25 17:42:54.260985 pyhtools-2.2.0/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     5725 2023-04-25 18:13:37.104832 pyhtools-2.2.0/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0      549 2023-04-25 17:42:54.281464 pyhtools-2.2.0/pyhtools/utils.py
+-rw-r--r--   0        0        0     1570 2023-04-29 07:47:45.586523 pyhtools-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6828 2023-04-25 17:42:54.252008 pyhtools-2.2.0/README.md
+-rw-r--r--   0        0        0     8627 1970-01-01 00:00:00.000000 pyhtools-2.2.0/PKG-INFO
```

### Comparing `pyhtools-2.1.0/LICENSE` & `pyhtools-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Android/forensics/data_harvestor.py` & `pyhtools-2.2.0/pyhtools/attackers/Android/forensics/data_harvestor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.2.0/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/attackers.py` & `pyhtools-2.2.0/pyhtools/attackers/attackers.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/arpspoofer.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/arpspoofer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # how to forward port on linux
 # execute any of the commands below
 # 1. sudo sysctl -w net.ipv4.ip_forward = 1
 # 2. sudo echo 1 > /proc/sys/net/ipv4/ip_forward
 
 
-import kamene.all as sp
+import scapy.all as sp
 import argparse
 from time import sleep
-from pyhtools.UI.colors import *
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
 from sys import exit
 
 
 def get_args():
     '''
     get arguments from command line.
     '''
@@ -40,19 +40,19 @@
     elif not spoof_ip:
         exit(BRIGHT_RED +
              "[-] Please enter spoof ip as argument, use -h or --help for more info")
 
     return True
 
 
-def generate_packet(PDST, HWDST, PSRC):
+def generate_packet(pdst, hwdst, psrc):
     '''
     generates spoof packets.
     '''
-    packet = sp.ARP(op=2, pdst=PDST, hwdst=HWDST, psrc=PSRC)
+    packet = sp.ARP(op=2, pdst=pdst, hwdst=hwdst, psrc=psrc)
     return packet
 
 
 def get_mac(ip):
     '''
     retrieves mac address from the ip.
     '''
```

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/code_injector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/dnsspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/downloads_replacer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/machngr.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/machngr.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/network_jammer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/nwscan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-#!usr/bin/env python3
-import kamene.all as sp
+from pyhtools.UI.colors import BRIGHT_WHITE, BRIGHT_YELLOW, BRIGHT_RED
+
+
+import scapy.all as sp
 import argparse
-from pyhtools.UI.colors import *
 
 
 def get_args():
     '''
     description: get arguments from the command line.
     params: None
     returns: str
@@ -48,23 +49,23 @@
 
     for client in clients:
         print( BRIGHT_WHITE + client.get('ip') + '\t\t' + client.get('mac'))
     
     print(BRIGHT_YELLOW + '________________________________________________________\n')
     
 
-def run_nwscan(IP:str):
+def run_nwscan(ip:str):
     '''
     description: starts network scanner for specified ip range or ip.
     params: IP (str)
     returns: None
     '''
     try:
         print(BRIGHT_YELLOW + '[*] Starting Network Scanner....')
-        clients = scan(IP)
+        clients = scan(ip)
         print_clients(clients)
     except Exception as e:
         print(BRIGHT_RED + '[-] Exception : ', e)
 
 
 if __name__ == "__main__":
     IP = get_args()
```

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/Network/tcp_proxy.py` & `pyhtools-2.2.0/pyhtools/attackers/Network/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/api/discover.py` & `pyhtools-2.2.0/pyhtools/attackers/web/api/discover.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.2.0/pyhtools/attackers/web/enumerate.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.2.0/pyhtools/attackers/web/get_forms.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.2.0/pyhtools/attackers/web/login_guesser.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/spider.py` & `pyhtools-2.2.0/pyhtools/attackers/web/spider.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/utils.py` & `pyhtools-2.2.0/pyhtools/attackers/web/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py` & `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.2.0/pyhtools/detectors/arp_spoof_detector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/exec_generator.py` & `pyhtools-2.2.0/pyhtools/evil_files/exec_generator.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/installer/cert.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/cert.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/keylogger/keylogger.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/keylogger.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!usr/bin/env python3
 import base64
 import socket
 import sys
 import json
 
 class Listener:
```

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/malwares/utils.py` & `pyhtools-2.2.0/pyhtools/evil_files/malwares/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py` & `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py` & `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md` & `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/evil_files/worms/dir_cloner.py` & `pyhtools-2.2.0/pyhtools/evil_files/worms/dir_cloner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyhtools/UI/functions.py` & `pyhtools-2.2.0/pyhtools/UI/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from pyhtools.UI.colors import *
 from prettytable import PrettyTable
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, BACK_RED_BRIGHT_YELLOW, RESET_COLORS
 from pyhtools.evil_files.malwares.utils import send_mail
+
+
 import pyfiglet
 import os
 import sys
 import pyhtools.attackers.attackers as attacker
 import pyhtools.evil_files.malwares.reverse_backdoor.TCP.listener as listener
 
+__version = '2.1.0'
 
 def clrscr():
     if os.name == 'nt':
         os.system('cls')
     elif os.name == 'posix':
         os.system('clear')
 
@@ -18,16 +21,15 @@
 def banner():
     '''
     prints PyHTools Banner
     '''
     clrscr()
     print(BRIGHT_YELLOW + pyfiglet.figlet_format('PyHTools'))
     print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
-
-    print(BRIGHT_WHITE + '| written by Dhrumil Mistry\tpht v1.0.1 |')
+    print(BRIGHT_WHITE + f'| written by dmdhrumilmistry\tpht v{__version} |')
     print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
 
 
 def print_help():
     '''
     prints commands with their brief description.
     '''
```

### Comparing `pyhtools-2.1.0/pyhtools/utils.py` & `pyhtools-2.2.0/pyhtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.1.0/pyproject.toml` & `pyhtools-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "pyhtools"
-version = "2.1.0"
+version = "2.2.0"
 description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
 authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiodns = "^3.0.0"
 aiohttp = "^3.8.4"
 beautifulsoup4 = "^4.11.2"
 colorama = "^0.4.6"
 frida-tools = "^12.1.1"
-kamene = "^0.32"
 nuitka = "^1.4.8"
 paramiko = "^3.0.0"
 pure-python-adb = "^0.3.0.dev0"
 pyfiglet = "^0.8.post1"
 pynput = "^1.7.6"
 pytelegrambotapi = "^4.10.0"
 prettytable = "^3.6.0"
```

### Comparing `pyhtools-2.1.0/README.md` & `pyhtools-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 
 - to get all the commands use `help`
 
   ```bash
   pyhtools >> help
   ```
 
-> There may be chances that pyfiglet or kamene will not be installed through requirements.txt, you can install manually using `pip3 install pyfiglet kamene`.  
 > If you're using Termux or windows, then use `pip` instead of `pip3`.  
 > Few features are only for linux os, hence they might not work on windows and require admin priviliges.
 
 ### Open In Google Cloud Shell
 
 - Temporary Session  
   [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)
```

### Comparing `pyhtools-2.1.0/setup.py` & `pyhtools-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,230 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyhtools
+Version: 2.2.0
+Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
+License: MIT
+Author: Dhrumil Mistry
+Author-email: contact@dmdhrumilmistry.tech
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: linux
+Provides-Extra: windows
+Requires-Dist: aiodns (>=3.0.0,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: frida-tools (>=12.1.1,<13.0.0)
+Requires-Dist: netfilterqueue (>=1.1.0,<2.0.0) ; extra == "linux"
+Requires-Dist: nuitka (>=1.4.8,<2.0.0)
+Requires-Dist: paramiko (>=3.0.0,<4.0.0)
+Requires-Dist: prettytable (>=3.6.0,<4.0.0)
+Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: pure-python-adb (>=0.3.0.dev0,<0.4.0)
+Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
+Requires-Dist: pynput (>=1.7.6,<2.0.0)
+Requires-Dist: pytelegrambotapi (>=4.10.0,<5.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: scapy (>=2.5.0,<3.0.0)
+Requires-Dist: wmi (>=1.5.1,<2.0.0) ; extra == "windows"
+Requires-Dist: zstandard (>=0.20.0,<0.21.0)
+Project-URL: Bug Tracker, https://github.com/dmdhrumilmistry/pyhtools/issues
+Project-URL: Home, https://github.com/dmdhrumilmistry/pyhtools
+Project-URL: PayPal, https://paypal.me/dmdhrumilmistry
+Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
+Description-Content-Type: text/markdown
 
-packages = \
-['pyhtools',
- 'pyhtools.UI',
- 'pyhtools.attackers',
- 'pyhtools.attackers.Android',
- 'pyhtools.attackers.Android.forensics',
- 'pyhtools.attackers.Android.mitm',
- 'pyhtools.attackers.Network',
- 'pyhtools.attackers.web',
- 'pyhtools.attackers.web.api',
- 'pyhtools.attackers.web.vuln_scanner',
- 'pyhtools.detectors',
- 'pyhtools.evil_files',
- 'pyhtools.evil_files.malwares',
- 'pyhtools.evil_files.malwares.backdoor.ssh',
- 'pyhtools.evil_files.malwares.data_harvesters',
- 'pyhtools.evil_files.malwares.installer',
- 'pyhtools.evil_files.malwares.keylogger',
- 'pyhtools.evil_files.malwares.reverse_backdoor',
- 'pyhtools.evil_files.malwares.reverse_backdoor.HTTP',
- 'pyhtools.evil_files.malwares.reverse_backdoor.TCP',
- 'pyhtools.evil_files.malwares.reverse_backdoor.ssh',
- 'pyhtools.evil_files.malwares.telegram_remote_code_executor',
- 'pyhtools.evil_files.ransomwares',
- 'pyhtools.evil_files.ransomwares.dmsec',
- 'pyhtools.evil_files.worms']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiodns>=3.0.0,<4.0.0',
- 'aiohttp>=3.8.4,<4.0.0',
- 'beautifulsoup4>=4.11.2,<5.0.0',
- 'colorama>=0.4.6,<0.5.0',
- 'frida-tools>=12.1.1,<13.0.0',
- 'kamene>=0.32,<0.33',
- 'nuitka>=1.4.8,<2.0.0',
- 'paramiko>=3.0.0,<4.0.0',
- 'prettytable>=3.6.0,<4.0.0',
- 'psutil>=5.9.4,<6.0.0',
- 'pure-python-adb>=0.3.0.dev0,<0.4.0',
- 'pyfiglet>=0.8.post1,<0.9',
- 'pynput>=1.7.6,<2.0.0',
- 'pytelegrambotapi>=4.10.0,<5.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'scapy>=2.5.0,<3.0.0',
- 'zstandard>=0.20.0,<0.21.0']
-
-extras_require = \
-{'linux': ['netfilterqueue>=1.1.0,<2.0.0'], 'windows': ['wmi>=1.5.1,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'pyhtools',
-    'version': '2.1.0',
-    'description': 'Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.',
-    'long_description': "# PyHTools\n\n![PyHTools Logo](https://i.ibb.co/CtwVV5T/Py-HTools-without-bg-cropped.png)\n\n- Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.\n\n- These tools are written in python3, refer installation to install/download tools and its dependencies.\n\n- PyHTools comes with UI, but you can also use command line to use tools individually.\n\n**`NOTE` : The UI hasn't been updated yet with new tools, Refer examples for more information**\n\n\n## Disclaimer\n\nThe disclaimer advises users to use the open source project for ethical and legitimate purposes only and refrain from using it for any malicious activities. The creators and contributors of the project are not responsible for any illegal activities or damages that may arise from the misuse of the project. Users are solely responsible for their use of the project and should exercise caution and diligence when using it. Any unauthorized or malicious use of the project may result in legal action and other consequences.\n\n[Read More](./DISCLAIMER.md)\n\n\n## Join Our Discord Community\n\n[![Join our Discord server!](https://invidget.switchblade.xyz/DJrnAg4nv2)](http://discord.gg/DJrnAg4nv2)\n\n## How To Videos\n\n- Gain access to remote shell over the Internet using HTTP Backdoor\n\n  [![YT Thumbnail](https://img.youtube.com/vi/Wg-PiywAqyw/maxresdefault.jpg)](https://youtu.be/Wg-PiywAqyw)\n\n## Installation\n\n### Using pip\n\n- Install main branch using pip\n\n  ```bash\n  python3 -m pip install git+https://github.com/dmdhrumilmistry/pyhtools.git\n  ```\n\n- Install Release from PyPi\n\n  ```bash\n  # without options\n  python3 -m pip install pyhtools\n\n  # for windows\n  python3 -m pip install pyhtools[windows]\n\n  # for linux\n  python3 -m pip install pyhtools[linux]\n  ```\n\n### Manual Method\n\n- Open terminal\n\n- Install git package\n\n  ```bash\n  sudo apt install git python3 -y\n  ```\n\n- Install [Poetry](https://python-poetry.org/docs/master#installing-with-the-official-installer)\n\n- clone the repository to your machine\n\n  ```bash\n  git clone https://github.com/dmdhrumilmistry/pyhtools.git\n  ```\n\n- Change directory\n\n  ```bash\n  cd pyhtools\n  ```\n\n- install with poetry\n\n  ```bash\n  # without options\n  poetry install\n\n  # for windows\n  poetry install -E windows\n\n  # for linux\n  poetry install -E linux\n  ```\n\n## Start PyHTools\n\n- run pyhtools.py\n\n  ```bash\n  python3 -m pyhtools\n  ```\n\n- to get all the commands use `help`\n\n  ```bash\n  pyhtools >> help\n  ```\n\n> There may be chances that pyfiglet or kamene will not be installed through requirements.txt, you can install manually using `pip3 install pyfiglet kamene`.  \n> If you're using Termux or windows, then use `pip` instead of `pip3`.  \n> Few features are only for linux os, hence they might not work on windows and require admin priviliges.\n\n### Open In Google Cloud Shell\n\n- Temporary Session  \n  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)\n- Perisitent Session  \n  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=false&show=terminal&cloudshell_print=./DISCLAIMER.md)\n\n## Package Tools and Features\n\n### Attackers\n\n- `For Networks`\n\n  - Network Scanner\n  - Mac changer\n  - ARP Spoofing\n  - DNS spoofing\n  - Downloads Replacer\n  - Network Jammer\n  - Pkt Sniffer\n  - Code Injector\n\n- `For Websites`\n\n  - Login Guesser (Login Bruteforcer)\n  - Web Spider\n  - Web crawler (detects dirs | subdomains)\n  - Web Vulnerablity Scanner\n\n- `For Android`\n  - mitm\n    - Custom Certificate Pinner\n\n### Detectors\n\n- ARP Spoof Detector\n\n### Malwares/Trojans/Payloads/Ransomwares/Worms\n\n- Email Sender (reporter)\n- Downloader\n- Wireless Password Harvester\n- Credential Harvester\n- Keylogger (dlogs)\n- Reverse Backdoors\n  - TCP\n  - HTTP\n- Download and Execute\n- Telegram Data Harvester\n- DMSecRansomware\n- Telegram Remote Code Executor\n- DirCloner\n\n> **NOTE:** Do not upload/send/report malwares to anti virus services such as `VirusTotal`. This will make program detectable\n\n## Project Updates\n\n- [View](https://github.com/users/dmdhrumilmistry/projects/2/views/1)\n\n## How to Package a Evil Files\n\n- [Example Script](./examples/EvilFiles)\n- [View How to create a Trojan](./HowTo/Malwares/CreateTrojanPackage.md)\n- [Generator Script](./examples/EvilFiles/generatorScript.py)\n\n## Have any Ideas 💡 or issue\n\n- Create an issue\n- Fork the repo, update script and create a Pull Request\n\n## Contributing\n\nRefer [CONTRIBUTIONS.md](/.github/CONTRIBUTING.md) for contributing to the project.\n\n## LICENSE\n\nPyHTools is distributed under `MIT` License. Refer [License](/LICENSE) for more information.\n\n## Connect With Me\n\n|                                                                                                                       |                                                       Platforms                                                       |                                                                                                                                        |\n| :-------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------: |\n|       [![GitHub](https://img.shields.io/badge/Github-dmdhrumilmistry-333)](https://github.com/dmdhrumilmistry)        | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Dhrumil%20Mistry-4078c0)](https://linkedin.com/in/dmdhrumilmistry) |             [![Twitter](https://img.shields.io/badge/Twitter-dmdhrumilmistry-4078c0)](https://twitter.com/dmdhrumilmistry)             |\n| [![Instagram](https://img.shields.io/badge/Instagram-dmdhrumilmistry-833ab4)](https://instagram.com/dmdhrumilmistry/) |     [![Blog](https://img.shields.io/badge/Blog-Dhrumil%20Mistry-bd2c00)](https://dmdhrumilmistry.github.io/blog)      | [![Youtube](https://img.shields.io/badge/YouTube-Dhrumil%20Mistry-critical)](https://www.youtube.com/channel/UChbjrRvbzgY3BIomUI55XDQ) |\n",
-    'author': 'Dhrumil Mistry',
-    'author_email': 'contact@dmdhrumilmistry.tech',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
+# PyHTools
 
+![PyHTools Logo](https://i.ibb.co/CtwVV5T/Py-HTools-without-bg-cropped.png)
+
+- Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
+
+- These tools are written in python3, refer installation to install/download tools and its dependencies.
+
+- PyHTools comes with UI, but you can also use command line to use tools individually.
+
+**`NOTE` : The UI hasn't been updated yet with new tools, Refer examples for more information**
+
+
+## Disclaimer
+
+The disclaimer advises users to use the open source project for ethical and legitimate purposes only and refrain from using it for any malicious activities. The creators and contributors of the project are not responsible for any illegal activities or damages that may arise from the misuse of the project. Users are solely responsible for their use of the project and should exercise caution and diligence when using it. Any unauthorized or malicious use of the project may result in legal action and other consequences.
+
+[Read More](./DISCLAIMER.md)
+
+
+## Join Our Discord Community
+
+[![Join our Discord server!](https://invidget.switchblade.xyz/DJrnAg4nv2)](http://discord.gg/DJrnAg4nv2)
+
+## How To Videos
+
+- Gain access to remote shell over the Internet using HTTP Backdoor
+
+  [![YT Thumbnail](https://img.youtube.com/vi/Wg-PiywAqyw/maxresdefault.jpg)](https://youtu.be/Wg-PiywAqyw)
+
+## Installation
+
+### Using pip
+
+- Install main branch using pip
+
+  ```bash
+  python3 -m pip install git+https://github.com/dmdhrumilmistry/pyhtools.git
+  ```
+
+- Install Release from PyPi
+
+  ```bash
+  # without options
+  python3 -m pip install pyhtools
+
+  # for windows
+  python3 -m pip install pyhtools[windows]
+
+  # for linux
+  python3 -m pip install pyhtools[linux]
+  ```
+
+### Manual Method
+
+- Open terminal
+
+- Install git package
+
+  ```bash
+  sudo apt install git python3 -y
+  ```
+
+- Install [Poetry](https://python-poetry.org/docs/master#installing-with-the-official-installer)
+
+- clone the repository to your machine
+
+  ```bash
+  git clone https://github.com/dmdhrumilmistry/pyhtools.git
+  ```
+
+- Change directory
+
+  ```bash
+  cd pyhtools
+  ```
+
+- install with poetry
+
+  ```bash
+  # without options
+  poetry install
+
+  # for windows
+  poetry install -E windows
+
+  # for linux
+  poetry install -E linux
+  ```
+
+## Start PyHTools
+
+- run pyhtools.py
+
+  ```bash
+  python3 -m pyhtools
+  ```
+
+- to get all the commands use `help`
+
+  ```bash
+  pyhtools >> help
+  ```
+
+> If you're using Termux or windows, then use `pip` instead of `pip3`.  
+> Few features are only for linux os, hence they might not work on windows and require admin priviliges.
+
+### Open In Google Cloud Shell
+
+- Temporary Session  
+  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)
+- Perisitent Session  
+  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=false&show=terminal&cloudshell_print=./DISCLAIMER.md)
+
+## Package Tools and Features
+
+### Attackers
+
+- `For Networks`
+
+  - Network Scanner
+  - Mac changer
+  - ARP Spoofing
+  - DNS spoofing
+  - Downloads Replacer
+  - Network Jammer
+  - Pkt Sniffer
+  - Code Injector
+
+- `For Websites`
+
+  - Login Guesser (Login Bruteforcer)
+  - Web Spider
+  - Web crawler (detects dirs | subdomains)
+  - Web Vulnerablity Scanner
+
+- `For Android`
+  - mitm
+    - Custom Certificate Pinner
+
+### Detectors
+
+- ARP Spoof Detector
+
+### Malwares/Trojans/Payloads/Ransomwares/Worms
+
+- Email Sender (reporter)
+- Downloader
+- Wireless Password Harvester
+- Credential Harvester
+- Keylogger (dlogs)
+- Reverse Backdoors
+  - TCP
+  - HTTP
+- Download and Execute
+- Telegram Data Harvester
+- DMSecRansomware
+- Telegram Remote Code Executor
+- DirCloner
+
+> **NOTE:** Do not upload/send/report malwares to anti virus services such as `VirusTotal`. This will make program detectable
+
+## Project Updates
+
+- [View](https://github.com/users/dmdhrumilmistry/projects/2/views/1)
+
+## How to Package a Evil Files
+
+- [Example Script](./examples/EvilFiles)
+- [View How to create a Trojan](./HowTo/Malwares/CreateTrojanPackage.md)
+- [Generator Script](./examples/EvilFiles/generatorScript.py)
+
+## Have any Ideas 💡 or issue
+
+- Create an issue
+- Fork the repo, update script and create a Pull Request
+
+## Contributing
+
+Refer [CONTRIBUTIONS.md](/.github/CONTRIBUTING.md) for contributing to the project.
+
+## LICENSE
+
+PyHTools is distributed under `MIT` License. Refer [License](/LICENSE) for more information.
+
+## Connect With Me
+
+|                                                                                                                       |                                                       Platforms                                                       |                                                                                                                                        |
+| :-------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------: |
+|       [![GitHub](https://img.shields.io/badge/Github-dmdhrumilmistry-333)](https://github.com/dmdhrumilmistry)        | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Dhrumil%20Mistry-4078c0)](https://linkedin.com/in/dmdhrumilmistry) |             [![Twitter](https://img.shields.io/badge/Twitter-dmdhrumilmistry-4078c0)](https://twitter.com/dmdhrumilmistry)             |
+| [![Instagram](https://img.shields.io/badge/Instagram-dmdhrumilmistry-833ab4)](https://instagram.com/dmdhrumilmistry/) |     [![Blog](https://img.shields.io/badge/Blog-Dhrumil%20Mistry-bd2c00)](https://dmdhrumilmistry.github.io/blog)      | [![Youtube](https://img.shields.io/badge/YouTube-Dhrumil%20Mistry-critical)](https://www.youtube.com/channel/UChbjrRvbzgY3BIomUI55XDQ) |
 
-setup(**setup_kwargs)
```

