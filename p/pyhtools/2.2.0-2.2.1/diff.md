# Comparing `tmp/pyhtools-2.2.0.tar.gz` & `tmp/pyhtools-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.2.0.tar", max compression
+gzip compressed data, was "pyhtools-2.2.1.tar", max compression
```

## Comparing `pyhtools-2.2.0.tar` & `pyhtools-2.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1092 2023-04-25 17:42:54.251011 pyhtools-2.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-25 18:13:37.104832 pyhtools-2.2.0/pyhtools/__init__.py
--rw-r--r--   0        0        0      107 2023-04-25 17:59:09.458258 pyhtools-2.2.0/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/forensics/data_harvestor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     5037 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      422 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0     4784 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.262980 pyhtools-2.2.0/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     5151 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4404 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3591 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     4730 2023-04-25 17:42:54.263977 pyhtools-2.2.0/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     3921 2023-04-25 17:42:54.264974 pyhtools-2.2.0/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2290 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     2068 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2680 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     5501 2023-04-25 17:42:54.265563 pyhtools-2.2.0/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.0/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     5177 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     2280 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     1984 2023-04-25 17:42:54.267559 pyhtools-2.2.0/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1123 2023-04-25 17:42:54.268556 pyhtools-2.2.0/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     2843 2023-04-25 17:42:54.268556 pyhtools-2.2.0/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     3279 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     6440 2023-04-25 17:42:54.269299 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2174 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0     2888 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     1737 2023-04-25 17:42:54.270298 pyhtools-2.2.0/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     1856 2023-04-25 17:42:54.271295 pyhtools-2.2.0/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.271295 pyhtools-2.2.0/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3454 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2347 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1908 2023-04-25 17:42:54.272293 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1681 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     5013 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2295 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.273290 pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-25 17:42:54.274287 pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1189 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.277282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5175 2023-04-25 17:42:54.277282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5408 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5939 2023-04-25 17:42:54.276282 pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     4503 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0     2681 2023-04-25 17:42:54.278284 pyhtools-2.2.0/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2203 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2306 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0     1105 2023-04-25 17:42:54.279274 pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3993 2023-04-25 17:42:54.280272 pyhtools-2.2.0/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.259994 pyhtools-2.2.0/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      292 2023-04-25 17:42:54.260985 pyhtools-2.2.0/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     5725 2023-04-25 18:13:37.104832 pyhtools-2.2.0/pyhtools/UI/functions.py
--rw-r--r--   0        0        0      549 2023-04-25 17:42:54.281464 pyhtools-2.2.0/pyhtools/utils.py
--rw-r--r--   0        0        0     1570 2023-04-29 07:47:45.586523 pyhtools-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6828 2023-04-25 17:42:54.252008 pyhtools-2.2.0/README.md
--rw-r--r--   0        0        0     8627 1970-01-01 00:00:00.000000 pyhtools-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-25 17:42:54.251011 pyhtools-2.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-25 18:13:37.104832 pyhtools-2.2.1/pyhtools/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-29 09:33:06.558539 pyhtools-2.2.1/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0     2815 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/forensics/data_harvestor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     5037 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      422 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0     4820 2023-04-29 09:55:07.229175 pyhtools-2.2.1/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     5151 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4404 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3591 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     4730 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     3921 2023-04-25 17:42:54.264974 pyhtools-2.2.1/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2290 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     2068 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2680 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     5501 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     5177 2023-04-25 17:42:54.267559 pyhtools-2.2.1/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     2280 2023-04-29 09:41:26.943813 pyhtools-2.2.1/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     1984 2023-04-25 17:42:54.267559 pyhtools-2.2.1/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1123 2023-04-25 17:42:54.268556 pyhtools-2.2.1/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     2843 2023-04-25 17:42:54.268556 pyhtools-2.2.1/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     3279 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     6440 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2174 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0     2888 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     1737 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     2139 2023-04-29 13:02:00.887409 pyhtools-2.2.1/pyhtools/evil_files/exec_generator.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.271295 pyhtools-2.2.1/pyhtools/evil_files/malwares/__init__.py
+-rw-r--r--   0        0        0     3454 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     2347 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
+-rw-r--r--   0        0        0     1908 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
+-rw-r--r--   0        0        0     1681 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
+-rw-r--r--   0        0        0     5013 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
+-rw-r--r--   0        0        0     2295 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/__init__.py
+-rw-r--r--   0        0        0     1619 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/cert.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/keylogger/__init__.py
+-rw-r--r--   0        0        0     2700 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/keylogger/keylogger.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
+-rw-r--r--   0        0        0     1189 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.277282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
+-rw-r--r--   0        0        0     5175 2023-04-25 17:42:54.277282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
+-rw-r--r--   0        0        0     5408 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
+-rw-r--r--   0        0        0     5939 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
+-rw-r--r--   0        0        0     4503 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
+-rw-r--r--   0        0        0     2681 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/__init__.py
+-rw-r--r--   0        0        0     2203 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
+-rw-r--r--   0        0        0     2306 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
+-rw-r--r--   0        0        0     1105 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/worms/__init__.py
+-rw-r--r--   0        0        0     3993 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/worms/dir_cloner.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:42:54.259994 pyhtools-2.2.1/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-25 17:42:54.260985 pyhtools-2.2.1/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     5812 2023-04-29 09:55:07.228177 pyhtools-2.2.1/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0      549 2023-04-25 17:42:54.281464 pyhtools-2.2.1/pyhtools/utils.py
+-rw-r--r--   0        0        0     1570 2023-04-29 13:02:00.887409 pyhtools-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7022 2023-04-29 13:02:00.886433 pyhtools-2.2.1/README.md
+-rw-r--r--   0        0        0     8813 1970-01-01 00:00:00.000000 pyhtools-2.2.1/PKG-INFO
```

### Comparing `pyhtools-2.2.0/LICENSE` & `pyhtools-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Android/forensics/data_harvestor.py` & `pyhtools-2.2.1/pyhtools/attackers/Android/forensics/data_harvestor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.2.1/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/attackers.py` & `pyhtools-2.2.1/pyhtools/attackers/attackers.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,44 +108,44 @@
         login_post_values = json.loads(login_post_values)
 
         vuln_scanner.session.post(login_link, data=login_post_values)
 
     vuln_scanner.run()
 
 
-def webspider():
+async def webspider():
     '''
     description: maps all the links related to the root url
     params: None
     returns: None
     '''
     target_url = input('[+] TARGET URL : ')
     spider = Spider()
 
     print(f'{BRIGHT_YELLOW}[*] Starting Spider... Press Ctrl+C to interrupt')
-    discovered_links = spider.start(
+    discovered_links = await spider.start(
         target_url=target_url,
         print_links=True
     )
     print(f'[*] Total Links Found: {len(discovered_links)}')
 
 
-def webcrawldirs():
+async def webcrawldirs():
     '''
     description: find valid directories of the website using a wordlist
     params: None
     returns: None
     '''
     domain = input('[+] DOMAIN (duckduckgo.com): ')
     wordlist_path = input('[+] WORDLIST PATH: ')
-    run(discoverer.check_dirs(domain=domain, wordlist=wordlist_path))
+    await discoverer.check_dirs(domain=domain, wordlist_path=wordlist_path)
 
 
-def webcrawlsubdom():
+async def webcrawlsubdom():
     '''
     description: find valid subdomains of the website using a wordlist
     params: None
     returns: None
     '''
     domain = input('[+] DOMAIN (duckduckgo.com) : ')
     wordlist_path = input('[+] WORDLIST PATH : ')
-    run(discoverer.check_subdomains(domain=domain, wordlist=wordlist_path))
+    await discoverer.check_subdomains(domain=domain, wordlist_path=wordlist_path)
```

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/arpspoofer.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/code_injector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/dnsspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/downloads_replacer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/machngr.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/machngr.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/network_jammer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/nwscan.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/Network/tcp_proxy.py` & `pyhtools-2.2.1/pyhtools/attackers/Network/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/api/discover.py` & `pyhtools-2.2.1/pyhtools/attackers/web/api/discover.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.2.1/pyhtools/attackers/web/enumerate.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.2.1/pyhtools/attackers/web/get_forms.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.2.1/pyhtools/attackers/web/login_guesser.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/spider.py` & `pyhtools-2.2.1/pyhtools/attackers/web/spider.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/utils.py` & `pyhtools-2.2.1/pyhtools/attackers/web/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py` & `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.2.1/pyhtools/detectors/arp_spoof_detector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/exec_generator.py` & `pyhtools-2.2.1/pyhtools/evil_files/exec_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 '''
 module: generator.py
 description: generates evil file executable
 '''
+from enum import Enum
 from subprocess import call
 from os import name as os_name
-from enum import Enum
 
 
 class Compilers(Enum):
     DEFAULT = 0
     MINGW = 1
     CLANG = 2
 
 
 class ExecutableGenerator:
     '''
-    creates executable
+    creates executable from python script.
     '''
 
     def __init__(self, file_path: str, output_dir: str = None, icon: str = None, compiler: Compilers = Compilers.DEFAULT, onefile: bool = True, remove_output: bool = True,) -> None:
         # file options
         self.__file = file_path
 
         # set options
         self.__options = {
             'onefile': onefile,
             'standalone': True,
-            'onefile': True,
             'remove-output': remove_output,
             'output-dir': output_dir,
         }
 
         # os based options
         if os_name == 'nt':
             self.__options['icon'] = icon
@@ -40,15 +39,22 @@
         # compiler based options
         if compiler == Compilers.CLANG:
             self.__options['clang'] = True
         elif compiler == Compilers.MINGW:
             self.__options['mingw'] = True
 
     def __generate_command(self):
-        command = 'nuitka '
+        '''
+        generates nuitka command
+        '''
+        if os_name == 'nt':
+            command = 'python -m nuitka '
+        else:
+            command = 'python3 -m nuitka '
+
         for key in self.__options:
             cmd = ''
             value = self.__options[key]
             value_type = type(self.__options[key])
 
             # generate option
             if value_type is bool and value:
@@ -60,9 +66,13 @@
             command += cmd
 
         # add file name and return
         command += f'{self.__file}'
         return command
 
     def generate_executable(self):
+        # linux devices requires patchelf to be installed
+        # sudo apt install patchelf 
         command = self.__generate_command()
-        return call(command.split(), shell=True)
+
+        # vuln: os command injection
+        return call(command, shell=True)
```

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/backdoor/ssh/handler.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/handler.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/installer/cert.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/cert.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/keylogger/keylogger.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/keylogger/keylogger.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/malwares/utils.py` & `pyhtools-2.2.1/pyhtools/evil_files/malwares/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/decrypter.py` & `pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/encrypter.py` & `pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/encrypter.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md` & `pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/evil_files/worms/dir_cloner.py` & `pyhtools-2.2.1/pyhtools/evil_files/worms/dir_cloner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyhtools/UI/functions.py` & `pyhtools-2.2.1/pyhtools/UI/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from asyncio.exceptions import CancelledError
 from prettytable import PrettyTable
 from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, BACK_RED_BRIGHT_YELLOW, RESET_COLORS
 from pyhtools.evil_files.malwares.utils import send_mail
 
 
 import pyfiglet
 import os
@@ -118,15 +119,15 @@
     '''
     print(BRIGHT_YELLOW +
           '[-] Currently this feature is under test... Will update soon...')
     print(BRIGHT_WHITE +
           '[*] You can use scripts from malwares to manually generate evil files...')
 
 
-def run():
+async def run():
     '''
     start PyHTools
     '''
     try:
         while True:
             cmd = input(BACK_RED_BRIGHT_YELLOW + 'pyhtools >>' +
                         RESET_COLORS + ' ').lower().strip()
@@ -159,33 +160,33 @@
                 attacker.arpspoofer()
 
             elif cmd == 'nwscan':
                 attacker.nw_scan()
 
             # WEB ATTACKERS
             elif cmd == 'webspider':
-                attacker.webspider()
+                await attacker.webspider()
 
             elif cmd == 'webcrawldirs':
-                attacker.webcrawldirs()
+                await attacker.webcrawldirs()
 
             elif cmd == 'webcrawlsubdom':
-                attacker.webcrawlsubdom()
+                await attacker.webcrawlsubdom()
 
             elif cmd == 'weblogin':
                 attacker.brute_login()
 
             elif cmd == 'webvulnscan':
                 attacker.webvulnscan()
 
             else:
                 print(BRIGHT_RED +
                       '[-] Unknown command, use help to view valid commands')
 
-    except (EOFError, KeyboardInterrupt):
+    except (EOFError, KeyboardInterrupt, CancelledError):
         print()
         print(BRIGHT_YELLOW +
               "[\U0001f604] WE ARE NEVER RESPONSIBLE FOR YOUR ACTIONS!")
         print(BRIGHT_RED + '[-] Closing PHT....')
         sys.exit(0)
```

### Comparing `pyhtools-2.2.0/pyhtools/utils.py` & `pyhtools-2.2.1/pyhtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.0/pyproject.toml` & `pyhtools-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhtools"
-version = "2.2.0"
+version = "2.2.1"
 description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
 authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyhtools-2.2.0/README.md` & `pyhtools-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,22 @@
 
 ## How to Package a Evil Files
 
 - [Example Script](./examples/EvilFiles)
 - [View How to create a Trojan](./HowTo/Malwares/CreateTrojanPackage.md)
 - [Generator Script](./examples/EvilFiles/generatorScript.py)
 
+`Note`: On linux host machines, user needs to install `patchelf` package. Install using below command.
+
+```bash
+apt/dnf/yum install patchelf
+```
+
+> Above command needs root privileges.
+
 ## Have any Ideas 💡 or issue
 
 - Create an issue
 - Fork the repo, update script and create a Pull Request
 
 ## Contributing
```

### Comparing `pyhtools-2.2.0/PKG-INFO` & `pyhtools-2.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtools
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
 License: MIT
 Author: Dhrumil Mistry
 Author-email: contact@dmdhrumilmistry.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -204,14 +204,22 @@
 
 ## How to Package a Evil Files
 
 - [Example Script](./examples/EvilFiles)
 - [View How to create a Trojan](./HowTo/Malwares/CreateTrojanPackage.md)
 - [Generator Script](./examples/EvilFiles/generatorScript.py)
 
+`Note`: On linux host machines, user needs to install `patchelf` package. Install using below command.
+
+```bash
+apt/dnf/yum install patchelf
+```
+
+> Above command needs root privileges.
+
 ## Have any Ideas 💡 or issue
 
 - Create an issue
 - Fork the repo, update script and create a Pull Request
 
 ## Contributing
```

