# Comparing `tmp/cbra-2.0.0a91.tar.gz` & `tmp/cbra-3.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbra-2.0.0a91.tar", last modified: Sat Apr 29 03:28:08 2023, max compression
+gzip compressed data, was "cbra-3.0.0a7.tar", last modified: Wed Mar  1 11:11:23 2023, max compression
```

## Comparing `cbra-2.0.0a91.tar` & `cbra-3.0.0a7.tar`

### file list

```diff
@@ -1,614 +1,284 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.156847 cbra-2.0.0a91/
--rw-r--r--   0 cochise    (501) staff       (20)      348 2023-03-26 17:07:04.000000 cbra-2.0.0a91/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)     1692 2023-04-29 03:28:08.156676 cbra-2.0.0a91/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      727 2023-04-15 23:44:57.000000 cbra-2.0.0a91/README.md
--rw-r--r--   0 cochise    (501) staff       (20)       13 2023-04-29 02:34:49.000000 cbra-2.0.0a91/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.896504 cbra-2.0.0a91/cbra/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.901631 cbra-2.0.0a91/cbra/core/
--rw-r--r--   0 cochise    (501) staff       (20)     5694 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      993 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/apiroute.py
--rw-r--r--   0 cochise    (501) staff       (20)     4614 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/application.py
--rw-r--r--   0 cochise    (501) staff       (20)    15083 2023-04-18 01:17:10.000000 cbra-2.0.0a91/cbra/core/conf.py
--rw-r--r--   0 cochise    (501) staff       (20)     2508 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     4301 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/endpointprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)     3677 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/endpointtype.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.904205 cbra-2.0.0a91/cbra/core/iam/
--rw-r--r--   0 cochise    (501) staff       (20)     5342 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/authenticatedcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)     2899 2023-04-11 00:00:19.000000 cbra-2.0.0a91/cbra/core/iam/authenticationservice.py
--rw-r--r--   0 cochise    (501) staff       (20)     5337 2023-03-13 14:28:50.000000 cbra-2.0.0a91/cbra/core/iam/authorizationcontextfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)     1164 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/isubjectrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)      824 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/memorysubjectrepository.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.906857 cbra-2.0.0a91/cbra/core/iam/models/
--rw-r--r--   0 cochise    (501) staff       (20)      731 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      913 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/models/accesscontrollist.py
--rw-r--r--   0 cochise    (501) staff       (20)      877 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/models/basesubject.py
--rw-r--r--   0 cochise    (501) staff       (20)     1039 2023-04-16 14:38:14.000000 cbra-2.0.0a91/cbra/core/iam/models/emailprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1233 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/models/externalprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      545 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/models/persistedsubject.py
--rw-r--r--   0 cochise    (501) staff       (20)     2056 2023-04-16 14:37:34.000000 cbra-2.0.0a91/cbra/core/iam/models/principal.py
--rw-r--r--   0 cochise    (501) staff       (20)      564 2023-04-16 14:36:59.000000 cbra-2.0.0a91/cbra/core/iam/models/principalmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     1117 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/models/publicidentifierprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     5563 2023-04-16 15:00:19.000000 cbra-2.0.0a91/cbra/core/iam/models/subject.py
--rw-r--r--   0 cochise    (501) staff       (20)     6095 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/models/subjectclaimset.py
--rw-r--r--   0 cochise    (501) staff       (20)     1021 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/nullauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)      728 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/nullsubjectesolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     2599 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/principalhasher.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.907348 cbra-2.0.0a91/cbra/core/iam/services/
--rw-r--r--   0 cochise    (501) staff       (20)      669 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/iam/services/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     6661 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/services/useronboarding.py
--rw-r--r--   0 cochise    (501) staff       (20)     1314 2023-02-26 14:42:54.000000 cbra-2.0.0a91/cbra/core/iam/subject.py
--rw-r--r--   0 cochise    (501) staff       (20)     2688 2023-03-20 20:13:29.000000 cbra-2.0.0a91/cbra/core/iam/subjectresolver.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.908993 cbra-2.0.0a91/cbra/core/iam/types/
--rw-r--r--   0 cochise    (501) staff       (20)      847 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1015 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/iam/types/isubjectrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     1777 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/types/iuseronboardingservice.py
--rw-r--r--   0 cochise    (501) staff       (20)      495 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/types/principal.py
--rw-r--r--   0 cochise    (501) staff       (20)      294 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/types/principaltype.py
--rw-r--r--   0 cochise    (501) staff       (20)      656 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/iam/types/publicidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1483 2023-04-16 15:00:19.000000 cbra-2.0.0a91/cbra/core/iam/types/subject.py
--rw-r--r--   0 cochise    (501) staff       (20)      498 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/iam/types/subjectlifecycletype.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.911019 cbra-2.0.0a91/cbra/core/ioc/
--rw-r--r--   0 cochise    (501) staff       (20)     1318 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/config.py
--rw-r--r--   0 cochise    (501) staff       (20)     1978 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/ioc/container.py
--rw-r--r--   0 cochise    (501) staff       (20)     1169 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/ioc/dependency.py
--rw-r--r--   0 cochise    (501) staff       (20)      476 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/dependencynotsatisfied.py
--rw-r--r--   0 cochise    (501) staff       (20)     1528 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/inheriteddependencydecorator.py
--rw-r--r--   0 cochise    (501) staff       (20)     1245 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/ioc/injected.py
--rw-r--r--   0 cochise    (501) staff       (20)      808 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/ioc/instance.py
--rw-r--r--   0 cochise    (501) staff       (20)     2225 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/loader.py
--rw-r--r--   0 cochise    (501) staff       (20)     1585 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/ioc/requirement.py
--rw-r--r--   0 cochise    (501) staff       (20)     1532 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/setting_.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.911329 cbra-2.0.0a91/cbra/core/ioc/test/
--rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/ioc/test/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1065 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/localmessagetransport.py
--rw-r--r--   0 cochise    (501) staff       (20)     1383 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/messagepublisher.py
--rw-r--r--   0 cochise    (501) staff       (20)     2964 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/messagerunner.py
--rw-r--r--   0 cochise    (501) staff       (20)     1139 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/metricreporter.py
--rw-r--r--   0 cochise    (501) staff       (20)     1237 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/optionsrequesthandler.py
--rw-r--r--   0 cochise    (501) staff       (20)     1967 2023-04-16 15:06:25.000000 cbra-2.0.0a91/cbra/core/package.json
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.911789 cbra-2.0.0a91/cbra/core/params/
--rw-r--r--   0 cochise    (501) staff       (20)     2490 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/params/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      696 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/params/applicationemailsender.py
--rw-r--r--   0 cochise    (501) staff       (20)     1145 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/params/applicationkeychain.py
--rw-r--r--   0 cochise    (501) staff       (20)    18208 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/requesthandler.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.918731 cbra-2.0.0a91/cbra/core/resource/
--rw-r--r--   0 cochise    (501) staff       (20)     1170 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2566 2023-04-15 22:29:43.000000 cbra-2.0.0a91/cbra/core/resource/collection.py
--rw-r--r--   0 cochise    (501) staff       (20)      701 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/collectionaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      430 2023-04-15 22:29:43.000000 cbra-2.0.0a91/cbra/core/resource/const.py
--rw-r--r--   0 cochise    (501) staff       (20)     1321 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/create.py
--rw-r--r--   0 cochise    (501) staff       (20)     2285 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/createaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1898 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/customaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1486 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/delete.py
--rw-r--r--   0 cochise    (501) staff       (20)     1574 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/deleteaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/detail.py
--rw-r--r--   0 cochise    (501) staff       (20)     2562 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/detailaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      981 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/iresource.py
--rw-r--r--   0 cochise    (501) staff       (20)      875 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/listaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      711 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/persister.py
--rw-r--r--   0 cochise    (501) staff       (20)      740 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/queryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)      684 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/replace.py
--rw-r--r--   0 cochise    (501) staff       (20)     1152 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/replaceaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     3104 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)     7086 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/resourceaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/resourceidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      670 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/resourcelist.py
--rw-r--r--   0 cochise    (501) staff       (20)     1252 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/resourcelistmetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     1304 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/resourcemodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     5901 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/resourcemodeltype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1222 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/resourceoptionsrequesthandler.py
--rw-r--r--   0 cochise    (501) staff       (20)      506 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/resourceprotocol.py
--rw-r--r--   0 cochise    (501) staff       (20)     5038 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/resourcetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      742 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/retrieve.py
--rw-r--r--   0 cochise    (501) staff       (20)      967 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/retrieveaction.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.919414 cbra-2.0.0a91/cbra/core/resource/test/
--rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/test/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      698 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/test/book.py
--rw-r--r--   0 cochise    (501) staff       (20)      528 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/test/bookpublication.py
--rw-r--r--   0 cochise    (501) staff       (20)     1711 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/test/bookresource.py
--rw-r--r--   0 cochise    (501) staff       (20)     1524 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/resource/update.py
--rw-r--r--   0 cochise    (501) staff       (20)     1149 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/updateaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      529 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/core/resource/versioned.py
--rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/resource/viewer.py
--rw-r--r--   0 cochise    (501) staff       (20)     2642 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/router.py
--rw-r--r--   0 cochise    (501) staff       (20)     2730 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/core/secretkey.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.919838 cbra-2.0.0a91/cbra/core/sessions/
--rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/sessions/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     5767 2023-04-29 02:20:30.000000 cbra-2.0.0a91/cbra/core/sessions/requestsession.py
--rw-r--r--   0 cochise    (501) staff       (20)     1107 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/core/utils.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.894514 cbra-2.0.0a91/cbra/ext/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.921046 cbra-2.0.0a91/cbra/ext/bff/
--rw-r--r--   0 cochise    (501) staff       (20)      562 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1454 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/frontendauthenticationcontextfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)      743 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/frontendendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)      755 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/frontendresource.py
--rw-r--r--   0 cochise    (501) staff       (20)     2461 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/frontendsubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     1463 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/oidcrequestsubject.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.921375 cbra-2.0.0a91/cbra/ext/bff/params/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/params/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      555 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/params/currentresourceserver.py
--rw-r--r--   0 cochise    (501) staff       (20)      543 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/bff/resourceserverclient.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.921935 cbra-2.0.0a91/cbra/ext/cache/
--rw-r--r--   0 cochise    (501) staff       (20)      838 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/cache/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1254 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/cache/cacheconfiguration.py
--rw-r--r--   0 cochise    (501) staff       (20)      887 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/cache/memorycache.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.923236 cbra-2.0.0a91/cbra/ext/email/
--rw-r--r--   0 cochise    (501) staff       (20)      784 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      568 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/accesscodeextension.py
--rw-r--r--   0 cochise    (501) staff       (20)     2286 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/baseemailsender.py
--rw-r--r--   0 cochise    (501) staff       (20)     2274 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/basewrapextension.py
--rw-r--r--   0 cochise    (501) staff       (20)      556 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/buttonextension.py
--rw-r--r--   0 cochise    (501) staff       (20)      565 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/paragraphextension.py
--rw-r--r--   0 cochise    (501) staff       (20)      559 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/sectionextension.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.924113 cbra-2.0.0a91/cbra/ext/email/templates/
--rw-r--r--   0 cochise    (501) staff       (20)      360 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/templates/accesscode.html.j2
--rw-r--r--   0 cochise    (501) staff       (20)     1162 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/templates/button.html.j2
--rw-r--r--   0 cochise    (501) staff       (20)     8850 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/templates/email.html.j2
--rw-r--r--   0 cochise    (501) staff       (20)       56 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/templates/paragraph.html.j2
--rw-r--r--   0 cochise    (501) staff       (20)      612 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/email/templates/section.html.j2
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.929841 cbra-2.0.0a91/cbra/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)     3994 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      818 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/aortadebugendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1326 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/aortaendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     3598 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/basedatastorerepository.py
--rw-r--r--   0 cochise    (501) staff       (20)      504 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/datastorecursor.py
--rw-r--r--   0 cochise    (501) staff       (20)      726 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/datastorequeryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)     7242 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/datastorerepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     6321 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/datastoresubjectrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     1660 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/datastoresubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)      453 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/debugcommand.py
--rw-r--r--   0 cochise    (501) staff       (20)      449 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/debugevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      767 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/environ.py
--rw-r--r--   0 cochise    (501) staff       (20)     1689 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/eventarcendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1837 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/googleendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1986 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/googlepubsubtransport.py
--rw-r--r--   0 cochise    (501) staff       (20)     1158 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/googlesecret.py
--rw-r--r--   0 cochise    (501) staff       (20)      591 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/googleserviceaccountprincipal.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.892831 cbra-2.0.0a91/cbra/ext/google/impl/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.930580 cbra-2.0.0a91/cbra/ext/google/impl/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)      526 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/impl/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1945 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/impl/oauth2/basemodelstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     2843 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/impl/oauth2/clientstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     8756 2023-04-16 14:28:19.000000 cbra-2.0.0a91/cbra/ext/google/impl/oauth2/storage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1218 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/logging.py
--rw-r--r--   0 cochise    (501) staff       (20)      496 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/messagediscarded.py
--rw-r--r--   0 cochise    (501) staff       (20)     1130 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/messagepublished.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.931177 cbra-2.0.0a91/cbra/ext/google/params/
--rw-r--r--   0 cochise    (501) staff       (20)      610 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/params/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1718 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/params/applicationstoragebucket.py
--rw-r--r--   0 cochise    (501) staff       (20)      702 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/params/applicationstorageclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1719 2023-04-15 22:47:24.000000 cbra-2.0.0a91/cbra/ext/google/polymoprhicdatastorecursor.py
--rw-r--r--   0 cochise    (501) staff       (20)     5488 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/polymorphicdatastorerepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     3262 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/pubsubmessage.py
--rw-r--r--   0 cochise    (501) staff       (20)      917 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/resourcemetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)      729 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/google/runner.py
--rw-r--r--   0 cochise    (501) staff       (20)     2521 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/service.py
--rw-r--r--   0 cochise    (501) staff       (20)     5394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/sheet.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.931969 cbra-2.0.0a91/cbra/ext/google/types/
--rw-r--r--   0 cochise    (501) staff       (20)      693 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      638 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/types/idatastorecursor.py
--rw-r--r--   0 cochise    (501) staff       (20)      877 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/types/idatastoreentity.py
--rw-r--r--   0 cochise    (501) staff       (20)      527 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/google/types/idatastorekey.py
--rw-r--r--   0 cochise    (501) staff       (20)      717 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/google/types/idatastorequery.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.937299 cbra-2.0.0a91/cbra/ext/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)     2558 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2764 2023-04-16 14:24:44.000000 cbra-2.0.0a91/cbra/ext/oauth2/applicationstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     4018 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/authorizationcodecallbackendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     4506 2023-04-29 02:34:06.000000 cbra-2.0.0a91/cbra/ext/oauth2/authorizationrequestendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     5419 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/authorizationserver.py
--rw-r--r--   0 cochise    (501) staff       (20)     2115 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/authorizationserverstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     3135 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/basefrontendstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     6936 2023-04-16 14:23:51.000000 cbra-2.0.0a91/cbra/ext/oauth2/basestorage.py
--rw-r--r--   0 cochise    (501) staff       (20)    12424 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/callbackendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.937710 cbra-2.0.0a91/cbra/ext/oauth2/client/
--rw-r--r--   0 cochise    (501) staff       (20)      497 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/client/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1299 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/client/accesstokenfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)      914 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/clientkeysendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)      810 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/const.py
--rw-r--r--   0 cochise    (501) staff       (20)     1246 2023-04-16 01:25:52.000000 cbra-2.0.0a91/cbra/ext/oauth2/currentsubjectendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1389 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/danceinitiationmixin.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.938511 cbra-2.0.0a91/cbra/ext/oauth2/endpoints/
--rw-r--r--   0 cochise    (501) staff       (20)      650 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/endpoints/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     9920 2023-04-16 15:00:19.000000 cbra-2.0.0a91/cbra/ext/oauth2/endpoints/authorizationendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     3205 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/endpoints/base.py
--rw-r--r--   0 cochise    (501) staff       (20)     2021 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/endpoints/userinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)     3020 2023-04-20 01:38:44.000000 cbra-2.0.0a91/cbra/ext/oauth2/frontendloginendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1781 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/frontendproxyendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     2514 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/frontendredirectionendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1757 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/frontenduserendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)      947 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/jwksendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     4883 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/loginendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     3871 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/memorystorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1157 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/metadataendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.949138 cbra-2.0.0a91/cbra/ext/oauth2/models/
--rw-r--r--   0 cochise    (501) staff       (20)     2356 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2473 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/accountregistration.py
--rw-r--r--   0 cochise    (501) staff       (20)     7311 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/applicationclient.py
--rw-r--r--   0 cochise    (501) staff       (20)      985 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorization.py
--rw-r--r--   0 cochise    (501) staff       (20)      652 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationcode.py
--rw-r--r--   0 cochise    (501) staff       (20)     5362 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationcodegrant.py
--rw-r--r--   0 cochise    (501) staff       (20)    19337 2023-04-29 02:26:28.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)     3374 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequestclient.py
--rw-r--r--   0 cochise    (501) staff       (20)      671 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequestobject.py
--rw-r--r--   0 cochise    (501) staff       (20)     4358 2023-04-29 02:28:11.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequestparameters.py
--rw-r--r--   0 cochise    (501) staff       (20)     1198 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequestreference.py
--rw-r--r--   0 cochise    (501) staff       (20)     1327 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      589 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/baseclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1209 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/basetokenrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      521 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/beginonboardrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      482 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/beginonboardresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     3853 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/client.py
--rw-r--r--   0 cochise    (501) staff       (20)     2307 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/clientcredentialsgrant.py
--rw-r--r--   0 cochise    (501) staff       (20)      876 2023-04-16 12:14:27.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/currentauthorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      564 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/downstreamproviderconfig.py
--rw-r--r--   0 cochise    (501) staff       (20)      513 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/emailchallenge.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.949965 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/
--rw-r--r--   0 cochise    (501) staff       (20)     3684 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1154 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/baseauthorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      590 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/downstreamauthorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      575 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/loginauthorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      592 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/recoveryauthorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      616 2023-04-20 01:37:30.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/frontendloginrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      482 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/frontendloginresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     1083 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/grant.py
--rw-r--r--   0 cochise    (501) staff       (20)     3437 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/managedgrant.py
--rw-r--r--   0 cochise    (501) staff       (20)      542 2023-04-29 02:13:25.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/patchauthorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      480 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/patchauthorizationresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     2900 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/refreshtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     2768 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/refreshtokengrant.py
--rw-r--r--   0 cochise    (501) staff       (20)     1200 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/resourceowner.py
--rw-r--r--   0 cochise    (501) staff       (20)      473 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/models/sector.py
--rw-r--r--   0 cochise    (501) staff       (20)     2163 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/oauth2/oidcregistrationendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     2985 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/onboardingendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.962677 cbra-2.0.0a91/cbra/ext/oauth2/params/
--rw-r--r--   0 cochise    (501) staff       (20)     2133 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2203 2023-04-18 01:28:24.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/applicationclient.py
--rw-r--r--   0 cochise    (501) staff       (20)      706 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/clientstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)      604 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/cookieclientidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     2011 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/cookiestoredauthorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      711 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/currentissuer.py
--rw-r--r--   0 cochise    (501) staff       (20)     2447 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/downstreamerror.py
--rw-r--r--   0 cochise    (501) staff       (20)     2878 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/downstreamtokentesponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     1673 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/frontenderror.py
--rw-r--r--   0 cochise    (501) staff       (20)      942 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/frontendredirecturi.py
--rw-r--r--   0 cochise    (501) staff       (20)     5140 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/frontendtokenresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     1919 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/localauthorizationrequeststate.py
--rw-r--r--   0 cochise    (501) staff       (20)      926 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/localclientprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)     1636 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/localopenidprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)     1345 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/localstorageauthorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)     6033 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/requestaccesstoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     5159 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/requestedgrant.py
--rw-r--r--   0 cochise    (501) staff       (20)     5839 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/requestingclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1189 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/requestresourceowner.py
--rw-r--r--   0 cochise    (501) staff       (20)     1969 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/resourceserverclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1021 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/serverkeychain.py
--rw-r--r--   0 cochise    (501) staff       (20)     4849 2023-04-16 00:43:19.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/tokenbuilder.py
--rw-r--r--   0 cochise    (501) staff       (20)     1491 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/params/tokensigner.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.963261 cbra-2.0.0a91/cbra/ext/oauth2/resource/
--rw-r--r--   0 cochise    (501) staff       (20)      761 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      978 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/resourceserverauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)     2509 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/resourceserverendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     2565 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/resourceserverresource.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.963801 cbra-2.0.0a91/cbra/ext/oauth2/resource/types/
--rw-r--r--   0 cochise    (501) staff       (20)      526 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      902 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/types/scope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1050 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resource/types/userinfosubject.py
--rw-r--r--   0 cochise    (501) staff       (20)     1440 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/resourceserversubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     2958 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/tokenendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1296 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/tokenhandlerendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.984611 cbra-2.0.0a91/cbra/ext/oauth2/types/
--rw-r--r--   0 cochise    (501) staff       (20)     5520 2023-04-16 14:19:14.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      488 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/accesstype.py
--rw-r--r--   0 cochise    (501) staff       (20)      635 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/authorizationcode.py
--rw-r--r--   0 cochise    (501) staff       (20)     1420 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/authorizationexception.py
--rw-r--r--   0 cochise    (501) staff       (20)      694 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/authorizationlifecycle.py
--rw-r--r--   0 cochise    (501) staff       (20)      652 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/authorizationrequestidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      911 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/basescope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1223 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/bearertoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     1237 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/bearertokencredential.py
--rw-r--r--   0 cochise    (501) staff       (20)     1567 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/bearertokenexception.py
--rw-r--r--   0 cochise    (501) staff       (20)      720 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/clientauthenticationmethod.py
--rw-r--r--   0 cochise    (501) staff       (20)      595 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/clientidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      774 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/clientinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      849 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/clientsecret.py
--rw-r--r--   0 cochise    (501) staff       (20)      636 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/compositeobjectidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/consentrequired.py
--rw-r--r--   0 cochise    (501) staff       (20)     1002 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/emailscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      663 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/extauthorizationrequeststate.py
--rw-r--r--   0 cochise    (501) staff       (20)      888 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/fatalauthorizationexception.py
--rw-r--r--   0 cochise    (501) staff       (20)     1032 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/fatalclientexception.py
--rw-r--r--   0 cochise    (501) staff       (20)     1230 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/frontendexception.py
--rw-r--r--   0 cochise    (501) staff       (20)      549 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/frontendobjecttype.py
--rw-r--r--   0 cochise    (501) staff       (20)      839 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/genericscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      977 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/grantedscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      539 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iaccesstoken.py
--rw-r--r--   0 cochise    (501) staff       (20)      627 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iaccesstokenobtainer.py
--rw-r--r--   0 cochise    (501) staff       (20)      590 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iauthorizationflowstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      844 2023-04-16 00:43:51.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iauthorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1130 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iauthorizationserverstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)      974 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1128 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iexternalauthorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      836 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/ifrontendstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1169 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/imanagedgrant.py
--rw-r--r--   0 cochise    (501) staff       (20)      809 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      638 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidclient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1262 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidgrant.py
--rw-r--r--   0 cochise    (501) staff       (20)      915 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      743 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidresponsetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      608 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      638 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/invalidtarget.py
--rw-r--r--   0 cochise    (501) staff       (20)      901 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/irefreshtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)      537 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iresourceowner.py
--rw-r--r--   0 cochise    (501) staff       (20)      672 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/iresourceserverstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1538 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/issuedaccesstoken.py
--rw-r--r--   0 cochise    (501) staff       (20)      812 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/issuedaccesstokenidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     2114 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/itokenbuilder.py
--rw-r--r--   0 cochise    (501) staff       (20)      699 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/itokensigner.py
--rw-r--r--   0 cochise    (501) staff       (20)      685 2023-02-25 23:04:12.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/jarmauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      702 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/loginresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      618 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/managedgrantidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      651 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/missingresponsetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      559 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/objectidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      498 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/oidcclaimset.py
--rw-r--r--   0 cochise    (501) staff       (20)     2962 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/oidcprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)      654 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/oidctokensubjectidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      939 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/openidscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      599 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/pairwiseidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      617 2023-04-16 14:18:56.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/principalidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1517 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/profilescope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1067 2023-02-25 23:16:14.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/queryauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     4139 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/redirectparameters.py
--rw-r--r--   0 cochise    (501) staff       (20)     3206 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/redirecturi.py
--rw-r--r--   0 cochise    (501) staff       (20)      626 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/refreshtokenidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      618 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/refreshtokenpolicytype.py
--rw-r--r--   0 cochise    (501) staff       (20)      511 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/refreshtokentype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1932 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/requestedscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      745 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/resourceaccesstokenidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      581 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/resourceowneridentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1949 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/resourceserveraccesstoken.py
--rw-r--r--   0 cochise    (501) staff       (20)      820 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/responsemodenotsupported.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/responsevalidationfailure.py
--rw-r--r--   0 cochise    (501) staff       (20)     5277 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/rfc9068accesstoken.py
--rw-r--r--   0 cochise    (501) staff       (20)      624 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/signable.py
--rw-r--r--   0 cochise    (501) staff       (20)     2143 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/signableoidctoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     1131 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/subjectclaimscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      948 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/subscope.py
--rw-r--r--   0 cochise    (501) staff       (20)      966 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/tokenendpointexception.py
--rw-r--r--   0 cochise    (501) staff       (20)      752 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     1052 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/useragentfingerprintscope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1273 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/oauth2/types/usererror.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.984776 cbra-2.0.0a91/cbra/ext/origin/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/origin/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.985304 cbra-2.0.0a91/cbra/ext/origin/types/
--rw-r--r--   0 cochise    (501) staff       (20)      485 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/origin/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      822 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/origin/types/ioriginstorage.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.986262 cbra-2.0.0a91/cbra/ext/picqer/
--rw-r--r--   0 cochise    (501) staff       (20)     1048 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4065 2023-04-14 17:07:39.000000 cbra-2.0.0a91/cbra/ext/picqer/picqerwebhookendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.988488 cbra-2.0.0a91/cbra/ext/picqer/v1/
--rw-r--r--   0 cochise    (501) staff       (20)      989 2023-04-14 13:26:11.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/event.py
--rw-r--r--   0 cochise    (501) staff       (20)      700 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/orderevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      717 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/picklistevent.py
--rw-r--r--   0 cochise    (501) staff       (20)     1079 2023-04-14 17:08:08.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/picklistshipment.py
--rw-r--r--   0 cochise    (501) staff       (20)      610 2023-04-14 13:26:11.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/picklistshipmentevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      710 2023-04-14 10:31:53.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/productevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/v1/purchaseorderevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      951 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/webhookresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      901 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/webhooksecret.py
--rw-r--r--   0 cochise    (501) staff       (20)     1622 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/picqer/webhooksignature.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.988646 cbra-2.0.0a91/cbra/ext/rbac/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.989333 cbra-2.0.0a91/cbra/ext/rbac/models/
--rw-r--r--   0 cochise    (501) staff       (20)      547 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1143 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/models/binding.py
--rw-r--r--   0 cochise    (501) staff       (20)      906 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/models/member.py
--rw-r--r--   0 cochise    (501) staff       (20)      682 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/models/policy.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.989936 cbra-2.0.0a91/cbra/ext/rbac/types/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      620 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/types/ipermissionsfinder.py
--rw-r--r--   0 cochise    (501) staff       (20)      493 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/types/ipolicy.py
--rw-r--r--   0 cochise    (501) staff       (20)      589 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/rbac/types/ipolicyfinder.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.990551 cbra-2.0.0a91/cbra/ext/secrets/
--rw-r--r--   0 cochise    (501) staff       (20)     1715 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/secrets/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      459 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/secrets/basesecret.py
--rw-r--r--   0 cochise    (501) staff       (20)      549 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/secrets/memorysecret.py
--rw-r--r--   0 cochise    (501) staff       (20)      542 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/secrets/secret.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.991056 cbra-2.0.0a91/cbra/ext/security/
--rw-r--r--   0 cochise    (501) staff       (20)      505 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/security/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3832 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/security/applicationkeychain.py
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/security/wrappedkey.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.991320 cbra-2.0.0a91/cbra/ext/sendgrid/
--rw-r--r--   0 cochise    (501) staff       (20)      500 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/sendgrid/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4688 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/ext/sendgrid/sendgridemailsender.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.992597 cbra-2.0.0a91/cbra/ext/shopify/
--rw-r--r--   0 cochise    (501) staff       (20)      598 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/shopify/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1772 2023-03-10 18:45:08.000000 cbra-2.0.0a91/cbra/ext/shopify/shopifywebhookendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     2408 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/shopify/shopifywebhookenvelope.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.993620 cbra-2.0.0a91/cbra/ext/shopify/v2023_01/
--rw-r--r--   0 cochise    (501) staff       (20)      480 2023-03-10 18:45:08.000000 cbra-2.0.0a91/cbra/ext/shopify/v2023_01/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.999432 cbra-2.0.0a91/cbra/ext/webhooks/
--rw-r--r--   0 cochise    (501) staff       (20)     1223 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4588 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/basewebhookendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1193 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/hmacwebhookverifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      837 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/incomingwebhook.py
--rw-r--r--   0 cochise    (501) staff       (20)      635 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/notimplementedenvelope.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.001131 cbra-2.0.0a91/cbra/ext/webhooks/types/
--rw-r--r--   0 cochise    (501) staff       (20)      707 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      788 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/types/iwebhookenvelope.py
--rw-r--r--   0 cochise    (501) staff       (20)      647 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/types/malformedsignature.py
--rw-r--r--   0 cochise    (501) staff       (20)      980 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/types/webhookexception.py
--rw-r--r--   0 cochise    (501) staff       (20)     1102 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/types/webhookresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      535 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/webhookendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1748 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/webhookendpointtype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1175 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/ext/webhooks/webhookenvelope.py
--rw-r--r--   0 cochise    (501) staff       (20)     1000 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/package.json
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.110611 cbra-2.0.0a91/cbra/types/
--rw-r--r--   0 cochise    (501) staff       (20)     4886 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1104 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/abortable.py
--rw-r--r--   0 cochise    (501) staff       (20)     4163 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/basemodel.py
--rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/conflict.py
--rw-r--r--   0 cochise    (501) staff       (20)     1206 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/etagset.py
--rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/forbidden.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/hints.py
--rw-r--r--   0 cochise    (501) staff       (20)      787 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/hmacsignature.py
--rw-r--r--   0 cochise    (501) staff       (20)     1666 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/httpheaderprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     2338 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)     1155 2023-04-08 21:27:20.000000 cbra-2.0.0a91/cbra/types/iauthorizationcontextfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)      482 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iblob.py
--rw-r--r--   0 cochise    (501) staff       (20)      690 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/icache.py
--rw-r--r--   0 cochise    (501) staff       (20)      699 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/icredential.py
--rw-r--r--   0 cochise    (501) staff       (20)      877 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/icredentialverifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      446 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/icursor.py
--rw-r--r--   0 cochise    (501) staff       (20)     1423 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/ideferred.py
--rw-r--r--   0 cochise    (501) staff       (20)     1414 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/idependant.py
--rw-r--r--   0 cochise    (501) staff       (20)     1933 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iemailsender.py
--rw-r--r--   0 cochise    (501) staff       (20)     6922 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1792 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/ihashable.py
--rw-r--r--   0 cochise    (501) staff       (20)     1360 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/imodelrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)      755 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/integerpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      562 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/ipersister.py
--rw-r--r--   0 cochise    (501) staff       (20)      634 2023-04-15 22:47:47.000000 cbra-2.0.0a91/cbra/types/ipolymorphiccursor.py
--rw-r--r--   0 cochise    (501) staff       (20)      715 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/ipolymorphicquery.py
--rw-r--r--   0 cochise    (501) staff       (20)     1690 2023-04-15 22:47:24.000000 cbra-2.0.0a91/cbra/types/ipolymorphicrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)      487 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      581 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/iqueryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)     3406 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/irequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/irequestprincipalintrospecter.py
--rw-r--r--   0 cochise    (501) staff       (20)      697 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/iroutable.py
--rw-r--r--   0 cochise    (501) staff       (20)     1522 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/isessiondata.py
--rw-r--r--   0 cochise    (501) staff       (20)      608 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/isessionfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)     1689 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/isessionmanager.py
--rw-r--r--   0 cochise    (501) staff       (20)      813 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/istoragebucket.py
--rw-r--r--   0 cochise    (501) staff       (20)     1242 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/isubject.py
--rw-r--r--   0 cochise    (501) staff       (20)      833 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/isubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)      649 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/iverifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      675 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/jsonwebtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     1473 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/jsonwebtokenprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1512 2023-03-13 21:30:22.000000 cbra-2.0.0a91/cbra/types/modelautoassignedidentity.py
--rw-r--r--   0 cochise    (501) staff       (20)     1529 2023-03-13 21:30:22.000000 cbra-2.0.0a91/cbra/types/modelidentity.py
--rw-r--r--   0 cochise    (501) staff       (20)     3193 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/modelinspector.py
--rw-r--r--   0 cochise    (501) staff       (20)     1051 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/modelmetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     1600 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/mutablesignature.py
--rw-r--r--   0 cochise    (501) staff       (20)      523 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/notauthorized.py
--rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/notfound.py
--rw-r--r--   0 cochise    (501) staff       (20)      702 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/nullemailsender.py
--rw-r--r--   0 cochise    (501) staff       (20)      735 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/nullrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1036 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/nullsubject.py
--rw-r--r--   0 cochise    (501) staff       (20)      713 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/nullsubjectesolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     1806 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/oidcrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/opaquebearertokenprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/operation.py
--rw-r--r--   0 cochise    (501) staff       (20)     1133 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/pathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)     1013 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/persistedmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     1974 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/policyprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      864 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/request.py
--rw-r--r--   0 cochise    (501) staff       (20)     1717 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/requestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1768 2023-03-14 13:31:12.000000 cbra-2.0.0a91/cbra/types/rfc9068requestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      529 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/servicenotavailable.py
--rw-r--r--   0 cochise    (501) staff       (20)     2534 2023-04-29 02:19:31.000000 cbra-2.0.0a91/cbra/types/session.py
--rw-r--r--   0 cochise    (501) staff       (20)      760 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/sessionclaims.py
--rw-r--r--   0 cochise    (501) staff       (20)     1509 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/sessionmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     2090 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/sessionrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      753 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/stringpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      782 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/subjectidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1023 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/unauthenticatedauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)      800 2023-02-23 23:31:32.000000 cbra-2.0.0a91/cbra/types/uuidpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      564 2023-03-10 18:44:55.000000 cbra-2.0.0a91/cbra/types/verifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      465 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/versionconflict.py
--rw-r--r--   0 cochise    (501) staff       (20)     1494 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/versionedciphertext.py
--rw-r--r--   0 cochise    (501) staff       (20)      727 2023-04-15 23:44:57.000000 cbra-2.0.0a91/cbra/types/versionedhmac.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.897767 cbra-2.0.0a91/cbra.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)     1692 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)    20284 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)      117 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/entry_points.txt
--rw-r--r--   0 cochise    (501) staff       (20)      602 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       54 2023-04-29 03:28:07.000000 cbra-2.0.0a91/cbra.egg-info/top_level.txt
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:07.894781 cbra-2.0.0a91/docs/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.113643 cbra-2.0.0a91/docs/source/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.113881 cbra-2.0.0a91/docs/source/_ext/
--rw-r--r--   0 cochise    (501) staff       (20)    15901 2023-02-23 23:31:32.000000 cbra-2.0.0a91/docs/source/_ext/djangodocs.py
--rw-r--r--   0 cochise    (501) staff       (20)     2934 2023-03-10 18:44:55.000000 cbra-2.0.0a91/docs/source/conf.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.144887 cbra-2.0.0a91/examples/
--rw-r--r--   0 cochise    (501) staff       (20)      904 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)     1631 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/dependency-injection.py
--rw-r--r--   0 cochise    (501) staff       (20)      754 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1029 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/fastapi-authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)      318 2023-04-15 23:44:57.000000 cbra-2.0.0a91/examples/google-ancestor.py
--rw-r--r--   0 cochise    (501) staff       (20)      557 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/google-cloud-platform.py
--rw-r--r--   0 cochise    (501) staff       (20)     1673 2023-04-15 23:44:57.000000 cbra-2.0.0a91/examples/oauth2-callback-google.py
--rw-r--r--   0 cochise    (501) staff       (20)     3050 2023-04-15 23:44:57.000000 cbra-2.0.0a91/examples/oauth2-server.py
--rw-r--r--   0 cochise    (501) staff       (20)     1387 2023-04-15 23:44:57.000000 cbra-2.0.0a91/examples/picqer-webhook.py
--rw-r--r--   0 cochise    (501) staff       (20)     2128 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)      899 2023-02-23 23:31:32.000000 cbra-2.0.0a91/examples/session.py
--rw-r--r--   0 cochise    (501) staff       (20)      739 2023-04-15 23:44:57.000000 cbra-2.0.0a91/examples/webhook.py
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-04-29 03:28:08.156885 cbra-2.0.0a91/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-03-10 18:44:55.000000 cbra-2.0.0a91/setup.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.147929 cbra-2.0.0a91/tests/
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      961 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.149315 cbra-2.0.0a91/tests/core/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/core/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.149508 cbra-2.0.0a91/tests/core/iam/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/core/iam/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.149716 cbra-2.0.0a91/tests/core/iam/models/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/core/iam/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2695 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/core/iam/models/test_unit_subject.py
--rw-r--r--   0 cochise    (501) staff       (20)     1275 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/core/test_unit_allow_explicit_none.py
--rw-r--r--   0 cochise    (501) staff       (20)     1616 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/core/test_unit_endpoint_etag.py
--rw-r--r--   0 cochise    (501) staff       (20)      752 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/core/test_unit_messagerunner_sends_to_sewer.py
--rw-r--r--   0 cochise    (501) staff       (20)     1853 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/core/test_unit_response_model_with_aliases.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.150074 cbra-2.0.0a91/tests/ext/
--rw-r--r--   0 cochise    (501) staff       (20)      400 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      521 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.150486 cbra-2.0.0a91/tests/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/ext/google/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.150970 cbra-2.0.0a91/tests/ext/google/system/
--rw-r--r--   0 cochise    (501) staff       (20)     1339 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/google/system/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1924 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/google/system/test_system_basedatastorerepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     2397 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/google/system/test_system_googleendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1928 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/google/test_integration_aorta.py
--rw-r--r--   0 cochise    (501) staff       (20)     2007 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/google/test_unit_messagepublisher.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.152719 cbra-2.0.0a91/tests/ext/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/ext/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3923 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     3165 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_integration_authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)     1659 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_integration_authorization.py
--rw-r--r--   0 cochise    (501) staff       (20)     2232 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_integration_authorization_request_requires_response_type.py
--rw-r--r--   0 cochise    (501) staff       (20)     2365 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_integration_authorization_request_requires_valid_redirect_uri.py
--rw-r--r--   0 cochise    (501) staff       (20)     1289 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_integration_authorization_requires_valid_client.py
--rw-r--r--   0 cochise    (501) staff       (20)     2267 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/oauth2/test_unit_redirecturi.py
--rw-r--r--   0 cochise    (501) staff       (20)     2219 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/oauth2/test_unit_refreshtoken.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.152996 cbra-2.0.0a91/tests/ext/picqer/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/picqer/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3877 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/picqer/test_unit_signature.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.153312 cbra-2.0.0a91/tests/ext/rbac/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/rbac/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      395 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/rbac/test_unit_policybinding.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.154573 cbra-2.0.0a91/tests/ext/security/
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/security/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1545 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/security/test_unit_applicationkeychain.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.154719 cbra-2.0.0a91/tests/ext/shopify/
--rw-r--r--   0 cochise    (501) staff       (20)     2398 2023-04-15 23:44:57.000000 cbra-2.0.0a91/tests/ext/shopify/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.155518 cbra-2.0.0a91/tests/ext/webhooks/
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/webhooks/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1758 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/webhooks/base.py
--rw-r--r--   0 cochise    (501) staff       (20)     3829 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/webhooks/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)      419 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/webhooks/test_unit_webhookendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1190 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/ext/webhooks/test_unit_webhookendpoint_authenticated.py
--rw-r--r--   0 cochise    (501) staff       (20)     3599 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/test_unit_endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1465 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/test_unit_endpoint_authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/test_unit_ioc.py
--rw-r--r--   0 cochise    (501) staff       (20)     4480 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/test_unit_principal.py
--rw-r--r--   0 cochise    (501) staff       (20)     3162 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/test_unit_resource.py
--rw-r--r--   0 cochise    (501) staff       (20)     4380 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/test_unit_session.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.155927 cbra-2.0.0a91/tests/types/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/types/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-04-29 03:28:08.156441 cbra-2.0.0a91/tests/types/persistedmodel/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/types/persistedmodel/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      750 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/types/persistedmodel/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1019 2023-03-10 18:44:55.000000 cbra-2.0.0a91/tests/types/persistedmodel/test_unit_metadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     4378 2023-02-23 23:31:32.000000 cbra-2.0.0a91/tests/types/test_unit_basemodel_identity.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.128428 cbra-3.0.0a7/
+-rw-r--r--   0 cochise    (501) staff       (20)      348 2023-02-23 23:31:32.000000 cbra-3.0.0a7/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 11:11:23.128244 cbra-3.0.0a7/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)      667 2023-02-23 23:31:32.000000 cbra-3.0.0a7/README.md
+-rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-01 11:11:07.000000 cbra-3.0.0a7/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.097025 cbra-3.0.0a7/cbra/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.099274 cbra-3.0.0a7/cbra/core/
+-rw-r--r--   0 cochise    (501) staff       (20)     3494 2023-02-28 17:21:37.000000 cbra-3.0.0a7/cbra/core/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5199 2023-02-28 17:24:16.000000 cbra-3.0.0a7/cbra/core/application.py
+-rw-r--r--   0 cochise    (501) staff       (20)     9725 2023-02-27 00:14:50.000000 cbra-3.0.0a7/cbra/core/conf.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2104 2023-02-28 17:15:47.000000 cbra-3.0.0a7/cbra/core/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3293 2023-02-26 16:38:33.000000 cbra-3.0.0a7/cbra/core/endpointtype.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.100169 cbra-3.0.0a7/cbra/core/iam/
+-rw-r--r--   0 cochise    (501) staff       (20)     5076 2023-02-26 14:40:20.000000 cbra-3.0.0a7/cbra/core/iam/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/authenticatedcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2899 2023-02-27 00:53:49.000000 cbra-3.0.0a7/cbra/core/iam/authenticationservice.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5337 2023-02-26 14:30:31.000000 cbra-3.0.0a7/cbra/core/iam/authorizationcontextfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1164 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/isubjectrepository.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.100995 cbra-3.0.0a7/cbra/core/iam/models/
+-rw-r--r--   0 cochise    (501) staff       (20)      588 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      978 2023-02-24 09:14:37.000000 cbra-3.0.0a7/cbra/core/iam/models/emailprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1233 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/externalprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1996 2023-02-24 11:02:31.000000 cbra-3.0.0a7/cbra/core/iam/models/principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      499 2023-02-24 09:14:50.000000 cbra-3.0.0a7/cbra/core/iam/models/principalmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1117 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/publicidentifierprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2235 2023-02-24 11:35:17.000000 cbra-3.0.0a7/cbra/core/iam/models/subject.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2597 2023-02-25 11:57:16.000000 cbra-3.0.0a7/cbra/core/iam/principalhasher.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.101245 cbra-3.0.0a7/cbra/core/iam/services/
+-rw-r--r--   0 cochise    (501) staff       (20)      669 2023-02-24 09:33:47.000000 cbra-3.0.0a7/cbra/core/iam/services/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5165 2023-02-24 13:36:08.000000 cbra-3.0.0a7/cbra/core/iam/services/useronboarding.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1314 2023-02-26 14:42:54.000000 cbra-3.0.0a7/cbra/core/iam/subject.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2688 2023-02-26 14:28:24.000000 cbra-3.0.0a7/cbra/core/iam/subjectresolver.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.102096 cbra-3.0.0a7/cbra/core/iam/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      764 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1015 2023-02-24 10:08:16.000000 cbra-3.0.0a7/cbra/core/iam/types/isubjectrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1065 2023-02-24 10:06:00.000000 cbra-3.0.0a7/cbra/core/iam/types/iuseronboardingservice.py
+-rw-r--r--   0 cochise    (501) staff       (20)      495 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      294 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/principaltype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      656 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/publicidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      880 2023-02-24 11:10:55.000000 cbra-3.0.0a7/cbra/core/iam/types/subject.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103277 cbra-3.0.0a7/cbra/core/ioc/
+-rw-r--r--   0 cochise    (501) staff       (20)     1318 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/config.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1972 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/container.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/dependency.py
+-rw-r--r--   0 cochise    (501) staff       (20)      476 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/dependencynotsatisfied.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1528 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/inheriteddependencydecorator.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1246 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/injected.py
+-rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/instance.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2225 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/loader.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1527 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/requirement.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1532 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/setting_.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103383 cbra-3.0.0a7/cbra/core/ioc/test/
+-rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/test/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-28 17:24:40.000000 cbra-3.0.0a7/cbra/core/messagepublisher.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1237 2023-02-24 00:54:18.000000 cbra-3.0.0a7/cbra/core/optionsrequesthandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1527 2023-02-28 18:16:08.000000 cbra-3.0.0a7/cbra/core/package.json
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103588 cbra-3.0.0a7/cbra/core/params/
+-rw-r--r--   0 cochise    (501) staff       (20)      790 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/params/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)    16189 2023-03-01 11:06:07.000000 cbra-3.0.0a7/cbra/core/requesthandler.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.107881 cbra-3.0.0a7/cbra/core/resource/
+-rw-r--r--   0 cochise    (501) staff       (20)     1120 2023-02-26 16:22:34.000000 cbra-3.0.0a7/cbra/core/resource/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1309 2023-02-26 16:27:20.000000 cbra-3.0.0a7/cbra/core/resource/collection.py
+-rw-r--r--   0 cochise    (501) staff       (20)      701 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/collectionaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1321 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/create.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2169 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/createaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1655 2023-02-26 18:45:57.000000 cbra-3.0.0a7/cbra/core/resource/customaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1486 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/delete.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1506 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/deleteaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/detail.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2448 2023-02-26 18:43:37.000000 cbra-3.0.0a7/cbra/core/resource/detailaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      832 2023-02-26 16:34:31.000000 cbra-3.0.0a7/cbra/core/resource/iresource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      875 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/listaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      711 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/persister.py
+-rw-r--r--   0 cochise    (501) staff       (20)      740 2023-02-26 16:22:20.000000 cbra-3.0.0a7/cbra/core/resource/queryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)      684 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/replace.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1093 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/replaceaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1687 2023-02-26 18:39:53.000000 cbra-3.0.0a7/cbra/core/resource/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6201 2023-02-26 18:50:19.000000 cbra-3.0.0a7/cbra/core/resource/resourceaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourceidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      670 2023-02-26 15:33:10.000000 cbra-3.0.0a7/cbra/core/resource/resourcelist.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1252 2023-02-26 15:23:44.000000 cbra-3.0.0a7/cbra/core/resource/resourcelistmetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1304 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourcemodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5732 2023-02-26 15:17:35.000000 cbra-3.0.0a7/cbra/core/resource/resourcemodeltype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1222 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourceoptionsrequesthandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)      506 2023-02-26 15:43:35.000000 cbra-3.0.0a7/cbra/core/resource/resourceprotocol.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4552 2023-02-26 18:40:03.000000 cbra-3.0.0a7/cbra/core/resource/resourcetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      715 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/retrieve.py
+-rw-r--r--   0 cochise    (501) staff       (20)      967 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/retrieveaction.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.108457 cbra-3.0.0a7/cbra/core/resource/test/
+-rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      698 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/book.py
+-rw-r--r--   0 cochise    (501) staff       (20)      528 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/bookpublication.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1711 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/bookresource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1512 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/update.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1090 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/updateaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/viewer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2729 2023-02-27 00:53:17.000000 cbra-3.0.0a7/cbra/core/secretkey.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.109571 cbra-3.0.0a7/cbra/core/sessions/
+-rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/sessions/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3275 2023-02-27 00:24:50.000000 cbra-3.0.0a7/cbra/core/sessions/requestsession.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1107 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/utils.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095348 cbra-3.0.0a7/cbra/ext/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.112506 cbra-3.0.0a7/cbra/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)     3653 2023-02-28 17:26:30.000000 cbra-3.0.0a7/cbra/ext/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1695 2023-02-28 17:36:58.000000 cbra-3.0.0a7/cbra/ext/google/aortaendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)      504 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/datastorecursor.py
+-rw-r--r--   0 cochise    (501) staff       (20)      726 2023-02-26 16:25:00.000000 cbra-3.0.0a7/cbra/ext/google/datastorequeryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7030 2023-02-26 16:51:13.000000 cbra-3.0.0a7/cbra/ext/google/datastorerepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4746 2023-02-26 14:42:12.000000 cbra-3.0.0a7/cbra/ext/google/datastoresubjectrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1658 2023-02-26 14:44:09.000000 cbra-3.0.0a7/cbra/ext/google/datastoresubjectresolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)      666 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/environ.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1689 2023-02-28 17:59:59.000000 cbra-3.0.0a7/cbra/ext/google/eventarcendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1837 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/googleendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1294 2023-02-28 16:12:25.000000 cbra-3.0.0a7/cbra/ext/google/googlepubsubtransport.py
+-rw-r--r--   0 cochise    (501) staff       (20)      591 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/googleserviceaccountprincipal.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095097 cbra-3.0.0a7/cbra/ext/google/impl/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.112767 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)      464 2023-02-25 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1026 2023-02-25 23:47:40.000000 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/storage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      496 2023-02-28 17:35:28.000000 cbra-3.0.0a7/cbra/ext/google/messagediscarded.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1130 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/messagepublished.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2852 2023-02-28 18:12:33.000000 cbra-3.0.0a7/cbra/ext/google/messagerunner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3262 2023-02-28 15:37:54.000000 cbra-3.0.0a7/cbra/ext/google/pubsubmessage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      917 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/resourcemetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)      729 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/runner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1547 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/service.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.113675 cbra-3.0.0a7/cbra/ext/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)     1157 2023-02-25 22:48:42.000000 cbra-3.0.0a7/cbra/ext/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4017 2023-02-25 23:48:33.000000 cbra-3.0.0a7/cbra/ext/oauth2/authorizationcodecallbackendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1551 2023-02-24 01:22:55.000000 cbra-3.0.0a7/cbra/ext/oauth2/authorizationendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1238 2023-02-25 23:46:59.000000 cbra-3.0.0a7/cbra/ext/oauth2/basestorage.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1459 2023-02-25 22:50:10.000000 cbra-3.0.0a7/cbra/ext/oauth2/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4852 2023-02-26 13:22:04.000000 cbra-3.0.0a7/cbra/ext/oauth2/loginendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1511 2023-02-25 23:51:05.000000 cbra-3.0.0a7/cbra/ext/oauth2/memorystorage.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.114099 cbra-3.0.0a7/cbra/ext/oauth2/models/
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-25 23:27:34.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      985 2023-02-24 02:23:22.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/authorization.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1327 2023-02-25 23:34:52.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/authorizationstate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      473 2023-02-25 23:27:21.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/sector.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2163 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/oidcregistrationendpoint.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.115811 cbra-3.0.0a7/cbra/ext/oauth2/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1379 2023-02-25 22:44:57.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      694 2023-02-24 01:40:14.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationlifecycle.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5357 2023-02-24 00:44:41.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-24 00:31:50.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequestobject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-24 00:06:09.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequestreference.py
+-rw-r--r--   0 cochise    (501) staff       (20)      590 2023-02-25 23:18:46.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationflowstate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      867 2023-02-25 23:46:40.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationserverstorage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      763 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/invalidauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      685 2023-02-25 23:04:12.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/jarmauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      702 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/loginresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1067 2023-02-25 23:16:14.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/queryauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4139 2023-02-25 23:15:11.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/redirectparameters.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3014 2023-02-24 00:04:27.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/redirecturi.py
+-rw-r--r--   0 cochise    (501) staff       (20)      774 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/responsemodenotsupported.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/responsevalidationfailure.py
+-rw-r--r--   0 cochise    (501) staff       (20)      752 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.116325 cbra-3.0.0a7/cbra/ext/picqer/
+-rw-r--r--   0 cochise    (501) staff       (20)     1048 2023-02-25 04:58:32.000000 cbra-3.0.0a7/cbra/ext/picqer/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4065 2023-02-25 11:25:08.000000 cbra-3.0.0a7/cbra/ext/picqer/picqerwebhookendpoint.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.116856 cbra-3.0.0a7/cbra/ext/picqer/v1/
+-rw-r--r--   0 cochise    (501) staff       (20)      799 2023-02-28 19:39:45.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-25 04:17:59.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/event.py
+-rw-r--r--   0 cochise    (501) staff       (20)      700 2023-02-25 09:56:51.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/orderevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      717 2023-02-25 09:56:58.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/picklistevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-28 19:39:23.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/purchaseorderevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      951 2023-02-25 01:54:30.000000 cbra-3.0.0a7/cbra/ext/picqer/webhookresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-25 04:56:47.000000 cbra-3.0.0a7/cbra/ext/picqer/webhooksecret.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1622 2023-02-25 04:57:09.000000 cbra-3.0.0a7/cbra/ext/picqer/webhooksignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1000 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/package.json
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124122 cbra-3.0.0a7/cbra/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     3660 2023-02-27 00:47:33.000000 cbra-3.0.0a7/cbra/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      911 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/abortable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4141 2023-02-25 23:42:27.000000 cbra-3.0.0a7/cbra/types/basemodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/conflict.py
+-rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/forbidden.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/hints.py
+-rw-r--r--   0 cochise    (501) staff       (20)      787 2023-02-27 00:52:53.000000 cbra-3.0.0a7/cbra/types/hmacsignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1666 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/httpheaderprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1973 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/iauthorizationcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1155 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/iauthorizationcontextfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)      699 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icredential.py
+-rw-r--r--   0 cochise    (501) staff       (20)      877 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icredentialverifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      446 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icursor.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1423 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/ideferred.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1414 2023-02-28 16:57:21.000000 cbra-3.0.0a7/cbra/types/idependant.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5642 2023-03-01 11:05:07.000000 cbra-3.0.0a7/cbra/types/iendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1792 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/ihashable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1360 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/imodelrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)      755 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/integerpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      581 2023-02-26 15:28:16.000000 cbra-3.0.0a7/cbra/types/iqueryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3046 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/irequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/irequestprincipalintrospecter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-26 16:35:24.000000 cbra-3.0.0a7/cbra/types/iroutable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1522 2023-02-27 00:35:48.000000 cbra-3.0.0a7/cbra/types/isessiondata.py
+-rw-r--r--   0 cochise    (501) staff       (20)      608 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isessionfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1495 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isessionmanager.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-26 19:12:06.000000 cbra-3.0.0a7/cbra/types/isubject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      785 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isubjectresolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)      675 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/jsonwebtoken.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1473 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/jsonwebtokenprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1508 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/modelautoassignedidentity.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1525 2023-02-25 22:43:16.000000 cbra-3.0.0a7/cbra/types/modelidentity.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1600 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/mutablesignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)      523 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/notauthorized.py
+-rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/notfound.py
+-rw-r--r--   0 cochise    (501) staff       (20)      644 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1036 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullsubject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      713 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullsubjectesolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1806 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/oidcrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/opaquebearertokenprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/operation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1133 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/pathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-25 23:40:52.000000 cbra-3.0.0a7/cbra/types/persistedmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1717 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/requestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1768 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/rfc9068requestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2380 2023-02-27 00:36:50.000000 cbra-3.0.0a7/cbra/types/session.py
+-rw-r--r--   0 cochise    (501) staff       (20)      618 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/sessionclaims.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1134 2023-02-27 00:36:57.000000 cbra-3.0.0a7/cbra/types/sessionmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2090 2023-02-27 00:49:22.000000 cbra-3.0.0a7/cbra/types/sessionrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      753 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/stringpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/subjectidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1023 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/unauthenticatedauthorizationcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)      800 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/uuidpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      564 2023-02-27 00:52:11.000000 cbra-3.0.0a7/cbra/types/verifier.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.098090 cbra-3.0.0a7/cbra.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)     8035 2023-03-01 11:11:23.000000 cbra-3.0.0a7/cbra.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      117 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/entry_points.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      299 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       54 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/top_level.txt
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095579 cbra-3.0.0a7/docs/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124237 cbra-3.0.0a7/docs/source/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124348 cbra-3.0.0a7/docs/source/_ext/
+-rw-r--r--   0 cochise    (501) staff       (20)    15901 2023-02-23 23:31:32.000000 cbra-3.0.0a7/docs/source/_ext/djangodocs.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2934 2023-02-23 23:31:32.000000 cbra-3.0.0a7/docs/source/conf.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.125435 cbra-3.0.0a7/examples/
+-rw-r--r--   0 cochise    (501) staff       (20)      904 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1631 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/dependency-injection.py
+-rw-r--r--   0 cochise    (501) staff       (20)      754 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1029 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/fastapi-authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)      557 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/google-cloud-platform.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1673 2023-02-23 18:20:54.000000 cbra-3.0.0a7/examples/oauth2-callback-google.py
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-24 00:39:57.000000 cbra-3.0.0a7/examples/oauth2-server.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1387 2023-02-25 05:00:28.000000 cbra-3.0.0a7/examples/picqer-webhook.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2128 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      899 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/session.py
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-01 11:11:23.128466 cbra-3.0.0a7/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-3.0.0a7/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126401 cbra-3.0.0a7/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      550 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126520 cbra-3.0.0a7/tests/core/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126618 cbra-3.0.0a7/tests/core/iam/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/iam/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126808 cbra-3.0.0a7/tests/core/iam/models/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/iam/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2695 2023-02-24 11:07:32.000000 cbra-3.0.0a7/tests/core/iam/models/test_unit_subject.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126939 cbra-3.0.0a7/tests/ext/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127125 cbra-3.0.0a7/tests/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/google/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127374 cbra-3.0.0a7/tests/ext/google/system/
+-rw-r--r--   0 cochise    (501) staff       (20)     1339 2023-02-25 04:00:03.000000 cbra-3.0.0a7/tests/ext/google/system/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2387 2023-02-28 17:14:16.000000 cbra-3.0.0a7/tests/ext/google/system/test_system_googleendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1928 2023-02-28 18:14:15.000000 cbra-3.0.0a7/tests/ext/google/test_integration_aorta.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127572 cbra-3.0.0a7/tests/ext/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2267 2023-02-23 23:48:41.000000 cbra-3.0.0a7/tests/ext/oauth2/test_unit_redirecturi.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127773 cbra-3.0.0a7/tests/ext/picqer/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-25 03:36:34.000000 cbra-3.0.0a7/tests/ext/picqer/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3876 2023-02-25 04:58:38.000000 cbra-3.0.0a7/tests/ext/picqer/test_unit_signature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3599 2023-03-01 11:10:13.000000 cbra-3.0.0a7/tests/test_unit_endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1465 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_endpoint_authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_ioc.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4480 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3162 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4380 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_session.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127993 cbra-3.0.0a7/tests/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4378 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/types/test_unit_basemodel_identity.py
```

### Comparing `cbra-2.0.0a91/PKG-INFO` & `cbra-3.0.0a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbra
-Version: 2.0.0a91
+Version: 3.0.0a7
 Summary: A class-based REStful API framework built on FastAPI
 Home-page: https://docs.cochise.io/python/cbra/latest
 Author: Cochise Ruhulessin
 Author-email: cochiseruhulessin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -18,23 +18,18 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: google
 Provides-Extra: gunicorn
-Provides-Extra: sendgrid
 
 
 
 
-# OAuth 2.x
-
-- https://www.rfc-editor.org/rfc/rfc8707.html
-
 # Resources
 
 - https://tyk.io/blog/your-data-model-is-not-an-api/
 - https://shekhargulati.com/2021/10/15/web-api-design-anti-pattern-exposing-your-database-model
 - https://cloud.google.com/blog/products/api-management/why-your-web-apis-should-be-entity-oriented
 - https://cloud.google.com/blog/products/application-development/api-design-why-you-should-use-links-not-keys-to-represent-relationships-in-apis
 - https://tools.ietf.org/html/rfc7807
```

### Comparing `cbra-2.0.0a91/README.md` & `cbra-3.0.0a7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 
 
 
-# OAuth 2.x
-
-- https://www.rfc-editor.org/rfc/rfc8707.html
-
 # Resources
 
 - https://tyk.io/blog/your-data-model-is-not-an-api/
 - https://shekhargulati.com/2021/10/15/web-api-design-anti-pattern-exposing-your-database-model
 - https://cloud.google.com/blog/products/api-management/why-your-web-apis-should-be-entity-oriented
 - https://cloud.google.com/blog/products/application-development/api-design-why-you-should-use-links-not-keys-to-represent-relationships-in-apis
 - https://tools.ietf.org/html/rfc7807
```

### Comparing `cbra-2.0.0a91/cbra/core/__init__.py` & `cbra-3.0.0a7/cbra/core/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,90 +2,64 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# type: ignore
-import importlib
-import inspect
-import pathlib
-import os
-from typing import cast
-from typing import Any
 from typing import Callable
 from typing import TypeVar
 
-import aorta
-import unimatrix.runtime
-import yaml
 from pydantic import Field
 
-from cbra.types import Request
-from .router import APIRouter
 from .application import Application
 from .endpoint import Endpoint
-from .endpointtype import EndpointType
 from . import ioc
-from . import utils
-from .localmessagetransport import LocalMessageTransport
 from .messagepublisher import MessagePublisher
-from .messagerunner import MessageRunner
-from .metricreporter import MetricReporter
 from .params import *
 from .resource import Collection
 from .resource import Create
 from .resource import Delete
 from .resource import Mutable
 from .resource import QueryResult
 from .resource import Replace
 from .resource import Resource
 from .resource import ResourceModel
 from .resource import ResourceType
 from .resource import Retrieve
 from .resource import Update
-from .resource import Versioned
 from .secretkey import SecretKey
 
 
 T = TypeVar('T')
 
 
 __all__: list[str] = [
     'describe',
     'inject',
     'instance',
     'ioc',
     'permission',
-    'utils',
-    'APIRouter',
     'Application',
     'ApplicationSecretKey',
     'Collection',
     'Create',
     'Delete',
     'Endpoint',
-    'EndpointType',
     'Field',
-    'LocalMessageTransport',
     'MessagePublisher',
-    'MessageRunner',
-    'MetricReporter',
     'Mutable',
     'QueryResult',
-    'Request',
     'Replace',
     'Resource',
     'ResourceModel',
     'ResourceType',
     'Retrieve',
     'SecretKey',
-    'Update',
-    'Versioned',
+    'Update'
 ]
 
 inject = ioc.inject
 instance = ioc.instance
 permission = Endpoint.require_permission
 
 
@@ -165,61 +139,8 @@
     ) -> Callable[..., T]:
         if not hasattr(func, 'responses'):
             func.responses = {} # type: ignore
         func.responses[self.status_code] = { # type: ignore
             k: v for k, v in self.__dict__.items()
             if v is not None and k != 'status_code'
         }
-        return func
-    
-
-def autodiscover(
-    qualname: str, cls: type[T] | None  = None
-) -> T:
-    os.environ.setdefault(
-        'PYTHON_SETTINGS_MODULE',
-        unimatrix.runtime.get_settings_module(__name__)
-    )
-    parent = qualname.rsplit('.', 1)[0]
-    modules: list[str] = [
-        'endpoints',
-        'handlers',
-        'listeners',
-        'resources',
-    ]
-    asgi = importlib.import_module(qualname)
-    params: dict[str, Any] = {
-        'docs_url'  : '/ui',
-        'redoc_url' : '/'
-    }
-    base = pathlib.Path(asgi.__file__).parent
-    meta = base.joinpath('asgi.yml')
-    if meta.exists():
-        params.update(yaml.safe_load(meta.read_text()))
-    cls = cls or Application
-    app = cast(Application, cls(**params))
-    addables: tuple[type] = (
-        Resource,
-        aorta.CommandHandler,
-        aorta.Sewer,
-        aorta.EventListener,
-    )
-    for name in modules:
-        try:
-            module = importlib.import_module(f'{parent}.{name}')
-        except ImportError:
-            # Raise the error if the module exists because then it
-            # was something in the module that raised it.
-            if any([
-                base.joinpath(name).exists(),
-                base.joinpath(f'{name}.py').exists()
-            ]):
-                raise
-            continue
-        for _, member in inspect.getmembers(module):
-            if not inspect.isclass(member) or not issubclass(member, addables):
-                continue
-            if not getattr(member, 'autodiscover', False):
-                continue
-            app.add(member)
-
-    return app
+        return func
```

### Comparing `cbra-2.0.0a91/cbra/core/apiroute.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-# Copyright (C) 2022 Cochise Ruhulessin
+# Copyright (C) 2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
-from typing import Callable
-from typing import Coroutine
+from typing import TypeAlias
+from typing import Union
 
-import fastapi
-import fastapi.exceptions
-import fastapi.routing
-
-from cbra.types import Request
-
-
-class APIRoute(fastapi.routing.APIRoute):
-
-    def get_route_handler(
-        self
-    ) -> Callable[[fastapi.Request], Coroutine[Any, Any, fastapi.Response]]:
-        super_handler = super().get_route_handler()
-
-        async def handler(request: fastapi.Request) -> fastapi.Response:
-            return await super_handler(
-                Request(request.scope, request.receive)
-            )
-
-        return handler
+from .orderevent import OrderEvent
+from .picklistevent import PicklistEvent
+from .purchaseorderevent import PurchaseOrderEvent
+
+
+__all__: list[str] = [
+    'OrderEvent',
+    'PicklistEvent',
+    'PicqerWebhookMessage',
+    'PurchaseOrderEvent',
+]
+
+
+PicqerWebhookMessage: TypeAlias = Union[
+    OrderEvent,
+    PicklistEvent,
+    PurchaseOrderEvent
+]
```

### Comparing `cbra-2.0.0a91/cbra/core/application.py` & `cbra-3.0.0a7/cbra/core/application.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,79 +2,64 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import asyncio
-import copy
-import logging.config
+import inspect
 from typing import Any
-from typing import Awaitable
 from typing import Callable
 
+import aorta
 import fastapi
 from fastapi import FastAPI
+from fastapi.routing import DecoratedCallable
 from fastapi.params import Depends
 
 from cbra.types import Abortable
-from cbra.types import NullEmailSender
-from .apiroute import APIRoute
 from .conf import settings
-from .endpointprovider import EndpointProvider
+from .endpoint import Endpoint
+from .resource import Resource
+from .ioc import Container
 from .ioc import Requirement
-from .localmessagetransport import LocalMessageTransport
 from .messagepublisher import MessagePublisher
 from .utils import parent_signature
 
 
-class Application(FastAPI, EndpointProvider):
+class Application(FastAPI):
     __module__: str = 'cbra'
     _injectables: tuple[type, ...] = (
         Depends,
         Requirement
     )
 
     @parent_signature(FastAPI.__init__)
-    def __init__(self, **kwargs: Any):
-        EndpointProvider.__init__(self)
+    def __init__(self, *args: Any, **kwargs: Any):
+        self.container = Container.fromsettings()
+
         handlers: dict[type, Any] = kwargs.setdefault('exception_handlers', {})
         handlers[Abortable] = self.on_aborted
 
         kwargs.setdefault('root_path', settings.ASGI_ROOT_PATH)
         self.inject('MessagePublisher', MessagePublisher)
-        if not self.container.has('MessageTransport'):
-            self.inject('MessageTransport', LocalMessageTransport)
-        if not self.container.has('EmailSender'):
-            self.container.provide('EmailSender', {
-                'qualname': '_',
-                'symbol': NullEmailSender
-            })
-        FastAPI.__init__(self, **kwargs)
-        self.router.route_class = APIRoute
-        self.add_event_handler('startup', self.setup_logging) # type: ignore
-        if settings.DEBUG_RESPONSE_TIME is not None:
-            self.middleware('http')(self.delay_response)
+        self.inject('MessageTransport', aorta.NullTransport())
+        super().__init__(*args, **kwargs)
+
+    def add(
+        self,
+        routable: type[Endpoint | Resource],
+        *args: Any, **kwargs: Any
+    ) -> None:
+        routable.add_to_router(self, *args, **kwargs)
 
     def inject(self, name: str, value: Any) -> None:
         """Inject a value into the dependencies container."""
         self.container.inject(name, value)
 
-    def logging_config(self):
-        config = copy.deepcopy(settings.LOGGING)
-        if not settings.DEBUG:
-            # Remove console handler when not running in debug mode and its
-            # not explicitely enabled in the settings.
-            config['handlers']['console'] = {'class': 'logging.NullHandler'}
-        return config
-
-    def setup_logging(self) -> None:
-        logging.config.dictConfig(self.logging_config())
-
     async def on_aborted(
         self,
         request: fastapi.Request,
         exc: Abortable
     ) -> fastapi.Response:
         return await exc.as_response()
 
@@ -115,16 +100,46 @@
     @parent_signature(FastAPI.options)
     def options(self, *a: Any, **k: Any):
         return self.discover_requirements(FastAPI.options, *a, **k)
 
     @parent_signature(FastAPI.delete)
     def delete(self, *a: Any, **k: Any):
         return self.discover_requirements(FastAPI.delete, *a, **k)
-    
-    async def delay_response(
+
+    def discover_requirements(
         self,
-        request: fastapi.Request,
-        call_next: Callable[[fastapi.Request], Awaitable[fastapi.Response]]
-    ) -> fastapi.Response:
-        if isinstance(settings.DEBUG_RESPONSE_TIME, int):
-            await asyncio.sleep(settings.DEBUG_RESPONSE_TIME/1000)
-        return await call_next(request)
+        decorator_factory: Callable[..., DecoratedCallable],
+        *args: Any,
+        **kwargs: Any
+    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        def decorator(func: DecoratedCallable) -> DecoratedCallable:
+            self.update_requirements(func)
+            return decorator_factory(self, *args, **kwargs)(func)
+        return decorator
+
+    def update_requirements(self, func: Callable[..., Any] | Depends | Any) -> None:
+        """Traverse the signature tree of the given function to find
+        all :class:`Requirement` instances.
+        """
+        # TODO: this will completely mess up if multiple Application instances
+        # are spawned.
+        if not callable(func): return None
+        if isinstance(func, Depends):
+            return self.update_requirements(func.dependency)
+        if isinstance(func, Requirement):
+            func.add_to_container(self.container)
+        signature = inspect.signature(func) # type: ignore
+        for param in signature.parameters.values():
+            if not isinstance(param.default, self._injectables):
+                continue
+            if isinstance(param.default, Requirement):
+                param.default.add_to_container(self.container)
+                if param.default.callable():
+                    self.update_requirements(param.default.factory) # type: ignore
+                continue
+
+            if isinstance(param.default, Depends):
+                injectable = param.default.dependency
+                if injectable is None:
+                    # Was declared as f(dependency: Callable = fastapi.Depends())
+                    injectable = param.annotation
+                self.update_requirements(injectable)
```

### Comparing `cbra-2.0.0a91/cbra/core/endpoint.py` & `cbra-3.0.0a7/cbra/core/endpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,55 +10,47 @@
 from datetime import timezone
 from typing import Any
 from typing import TypeVar
 
 import fastapi
 
 from cbra.types import IAuthorizationContext
-from cbra.types import IAuthorizationContextFactory
-from cbra.types import IEmailSender
 from cbra.types import IEndpoint
 from cbra.types import RequestPrincipal
-from cbra.types import NullRequestPrincipal
 from .iam import AuthorizationContextFactory
-from .ioc import instance
 from .endpointtype import EndpointType
-from .messagepublisher import MessagePublisher
-from .params import ApplicationEmailSender
 from .sessions import RequestSession
 
 
 T = TypeVar('T')
 
 
 class Endpoint(IEndpoint, metaclass=EndpointType):
     __abstract__: bool = True
     __module__: str = 'cbra'
     allowed_http_methods: list[str]
-    email: IEmailSender = ApplicationEmailSender
     include_in_schema: bool = True
-    principal: RequestPrincipal | NullRequestPrincipal = RequestPrincipal.depends()
+    principal: RequestPrincipal = RequestPrincipal.depends()
     ctx: IAuthorizationContext
-    context_factory: IAuthorizationContextFactory = AuthorizationContextFactory.depends()
-    publisher: MessagePublisher = instance('MessagePublisher')
+    context_factory: AuthorizationContextFactory = AuthorizationContextFactory.depends()
     session: RequestSession = RequestSession.depends()
     timestamp: datetime
 
     def __init__(self, **kwargs: Any):
         """Constructor. Called in the router; can contain helpful extra
         keyword arguments, and other things.
         """
         # Go through keyword arguments, and either save their values to our
         # instance, or raise an error.
         for key, value in kwargs.items():
             setattr(self, key, value)
         self.timestamp = datetime.now(timezone.utc)
 
     @classmethod
-    def add_to_router(cls, router: fastapi.FastAPI | fastapi.APIRouter, **kwargs: Any) -> None:
+    def add_to_router(cls, router: fastapi.FastAPI, **kwargs: Any) -> None:
         kwargs.setdefault('path', '/')
         kwargs.setdefault('response_model_by_alias', cls.response_model_by_alias)
         kwargs.setdefault('status_code', cls.status_code)
         kwargs.setdefault('summary', cls.summary)
         kwargs.setdefault('tags', cls.tags)
         for handler in cls.handlers:
             handler.add_to_router(cls, router, **kwargs)
```

### Comparing `cbra-2.0.0a91/cbra/core/endpointtype.py` & `cbra-3.0.0a7/cbra/core/endpointtype.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import collections
-import inspect
 import itertools
 import types
 from typing import Any
 
-from cbra.types import IDependant
 from cbra.types import IEndpoint
 from cbra.types import IRequestPrincipal
 from cbra.types import RequestPrincipal
 from .requesthandler import RequestHandler
 from .optionsrequesthandler import OptionsRequestHandler
 
 
@@ -38,23 +36,14 @@
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **params: Any
     ) -> type[IEndpoint]:
         annotations = namespace.get('__annotations__') or {}
         is_abstract = namespace.pop('__abstract__', False)
         handlers: dict[str, RequestHandler[Any]] = collections.OrderedDict()
-
-        # Inspect annotations for injectables.
-        for attname, hint in annotations.items():
-            if not inspect.isclass(hint)\
-            or not issubclass(hint, IDependant)\
-            or attname in namespace:
-                continue
-            namespace[attname] = hint.depends()
-
         if not is_abstract:
             for h in itertools.chain(*[getattr(x, 'handlers', {}) for x in bases]):
                 handlers[h.attname] = h.clone() # type: ignore
 
             for attname, func in list(namespace.items()):
                 if attname not in cls.http_methods:
                     continue
@@ -69,15 +58,15 @@
             namespace.update({
                 'allowed_http_methods': [x.method for x in handlers.values()],
                 'handlers': handlers.values()
             })
 
         # Create a concrete Principal subclass. This is to allow
         # thing like principal: RFC9068RequestPrincipal | OIDCRequestPrincipal.
-        if annotations.get('principal') and not namespace.get('principal'):
+        if annotations.get('principal'):
             EndpointPrincipal: type[RequestPrincipal]
             principal: types.UnionType | IRequestPrincipal = annotations['principal']
             if isinstance(principal, types.UnionType):
                 EndpointPrincipal = annotations['principal'] = type(
                     f'{name}Principal',
                     (RequestPrincipal,),
                     {'__annotations__': {'__root__': principal}}
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,27 +127,21 @@
         headers = {'Authorization': f'bearer {id_token}'}
         print(id_token)
 """
 from .authenticatedcontext import AuthenticatedContext
 from .authenticationservice import AuthenticationService
 from .authorizationcontextfactory import AuthorizationContextFactory
 from .isubjectrepository import ISubjectRepository
-from .memorysubjectrepository import MemorySubjectRepository
-from .nullauthorizationcontext import NullAuthorizationContext
-from .nullsubjectesolver import NullSubjectResolver
 from .subject import Subject as RequestSubject
 from .subjectresolver import SubjectResolver
 from .types import IUserOnboardingService
 
 
 __all__: list[str] = [
     'AuthenticatedContext',
     'AuthenticationService',
     'AuthorizationContextFactory',
     'ISubjectRepository',
     'IUserOnboardingService',
-    'MemorySubjectRepository',
-    'NullAuthorizationContext',
-    'NullSubjectResolver',
     'RequestSubject',
     'SubjectResolver',
 ]
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/authenticatedcontext.py` & `cbra-3.0.0a7/cbra/core/iam/authenticatedcontext.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/authenticationservice.py` & `cbra-3.0.0a7/cbra/core/iam/authenticationservice.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/authorizationcontextfactory.py` & `cbra-3.0.0a7/cbra/core/iam/authorizationcontextfactory.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/isubjectrepository.py` & `cbra-3.0.0a7/cbra/core/iam/isubjectrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .accesscontrollist import AccessControlList
 from .externalprincipal import ExternalPrincipal
 from .principal import Principal
 from .subject import Subject
-from .subjectclaimset import SubjectClaimSet
 
 
 __all__: list[str] = [
-    'AccessControlList',
     'ExternalPrincipal',
     'Principal',
-    'Subject',
-    'SubjectClaimSet',
+    'Subject'
 ]
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/accesscontrollist.py` & `cbra-3.0.0a7/cbra/types/abortable.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
+import fastapi
 
-import pydantic
 
-from cbra.types import PolicyPrincipal
+class Abortable(Exception):
+    """An exception class that is detected by the framework and
+    can be converted for a corresponding HTTP response.
+
+    Be aware that any part of the code that catches an :class:`Abortable`
+    is allowed to abort the operation in progress and return a response
+    to the client.
+    """
+    __module__: str = 'cbra.types'
+    status_code: int = 500
 
-
-class AccessControlList(pydantic.BaseModel):
-    enabled: bool = True
-    members: list[PolicyPrincipal] = []
-
-    def is_enabled(self) -> bool:
-        """Return a boolean indicating if the ACL is enabled."""
-        return self.enabled
-
-    def is_member(self, obj: Any) -> bool:
-        """Return a boolean indicating if the object is a member of the
-        ACL.
-        """
-        return any([x.match(obj) for x in self.members])
+    async def as_response(self) -> fastapi.Response:
+        return fastapi.Response(status_code=self.status_code)
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/basesubject.py` & `cbra-3.0.0a7/cbra/ext/google/datastorequeryresult.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from datetime import datetime
-from typing import Literal
+from typing import Generic
+from typing import TypeVar
 
-import pydantic
 
-from cbra.types import PersistedModel
-from ..types import SubjectLifecycleType
+T = TypeVar('T')
 
 
-class BaseSubject(PersistedModel):
-    kind: Literal['User']
-    uid: int | None = pydantic.Field(
-        default=None,
-        auto_assign=True
-    )
-    created: datetime
-    seen: datetime
-    status: SubjectLifecycleType = SubjectLifecycleType.pending
+class DatastoreQueryResult(Generic[T]):
+    __module__: str = 'cbra.ext.google'
+    token: str | None
+    items: list[T]
 
-    def is_encypted(self) -> bool:
-        raise NotImplementedError
+    def __init__(self, token: str | None, entities: list[T]) -> None:
+        self.token = token or None
+        self.items = entities
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/emailprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/emailprincipal.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,10 +24,7 @@
         cls,
         values: dict[str, Any]
     ) -> dict[str, Any]:
         value: EmailAddress | None = values.pop('principal', None)
         if isinstance(value, EmailAddress):
             values['email'] = value
         return values
-
-    def __str__(self) -> str:
-        return str(self.email)
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/externalprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/externalprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/persistedsubject.py` & `cbra-3.0.0a7/cbra/types/iqueryresult.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,13 +2,19 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from cbra.types import VersionedCipherText
-from .basesubject import BaseSubject
+from typing import Generic
+from typing import Protocol
 
+from typing import TypeVar
 
-class PersistedSubject(BaseSubject):
-    claims: VersionedCipherText
+
+T = TypeVar('T')
+
+
+class IQueryResult(Protocol, Generic[T]):
+    token: str | None
+    items: list[T]
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/principal.py` & `cbra-3.0.0a7/cbra/core/iam/models/principal.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     PublicIdentifierPrincipal
 ]
 
 hasher: PrincipalHasher = PrincipalHasher()
 
 
 class Principal(PersistedModel):
+    id: int | None = pydantic.Field(
+        default=None,
+        auto_assign=True
+    )
     spec: PrincipalSpecType
     subject: int
     asserted: datetime
     suspended: bool = False
 
     #: A hash value created from the spec. For internal use only.
     key: str = pydantic.Field(..., primary_key=True)
@@ -59,14 +63,8 @@
             'trust': trust,
             'key': hasher.hash(principal),
             'spec': {
                 'iss': issuer,
                 'kind': type(principal).__name__,
                 'principal': principal,
             }
-        })
-    
-    def is_owned_by(self, uid: int) -> bool:
-        return uid == self.subject
-    
-    def __str__(self) -> str:
-        return str(self.spec)
+        })
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/principalmodel.py` & `cbra-3.0.0a7/cbra/core/resource/detail.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from cbra.types import PersistedModel
+from typing import Any
 
 
-class PrincipalModel(PersistedModel):
-    kind: str
-    iss: str
+class Detail:
+    __module__: str = 'cbra.core'
 
-    def __str__(self) -> str:
+    async def get_object(self) -> Any:
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/publicidentifierprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/publicidentifierprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/subject.py` & `cbra-3.0.0a7/cbra/ext/google/datastoresubjectrepository.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,157 +2,123 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from datetime import datetime
+import functools
 from typing import Any
-from typing import Literal
+from typing import AsyncGenerator
 
-import pydantic
-from canonical import DomainName
 from canonical import EmailAddress
-from headless.ext.oauth2.models import OIDCToken
+from google.cloud.datastore import Query
+from headless.ext.oauth2.models import SubjectIdentifier
 
-from cbra.ext.security import ApplicationKeychain
-from cbra.types import ISessionManager
-from cbra.types import PersistedModel
-from cbra.types import VersionedCipherText
-from ..types import PrincipalType
-from ..types import SubjectLifecycleType
-from .principal import Principal
-from .subjectclaimset import SubjectClaimSet
-
-
-class Subject(PersistedModel):
-    kind: Literal['User']
-    uid: int | None = pydantic.Field(
-        default=None,
-        auto_assign=True
-    )
-    created: datetime
-    seen: datetime
-    status: SubjectLifecycleType = SubjectLifecycleType.pending
-
-    claims: VersionedCipherText | SubjectClaimSet = pydantic.Field(
-        default_factory=SubjectClaimSet
-    )
-
-    principals: set[Principal] = set()
-
-    #: TODO: The PeristedModel must be refactored to register attribute mutations
-    #: so that the storage backend can detect if it needs to delete something.
-    _removed_principals: list[Principal] = pydantic.PrivateAttr([])
+from cbra.types import IModelRepository
+from cbra.core.iam import ISubjectRepository
+from cbra.core.iam.models import Principal
+from cbra.core.iam.models import Subject
+from .datastorerepository import DatastoreRepository
+
+
+class DatastoreSubjectRepository(
+    DatastoreRepository,
+    ISubjectRepository,
+    IModelRepository[Subject]
+):
+    __module__: str = 'cbra.ext.google'
+
+    @functools.singledispatchmethod # type: ignore
+    async def get(self, principal: Any) -> Subject | None:
+        if principal is None: return None
+        raise NotImplementedError(f'{principal.__module__}.{type(principal).__name__}')
+
+    @get.register
+    async def get_by_email(self, principal: EmailAddress) -> Subject | None:
+        query = self.query('Principal')
+        query.add_filter('spec.kind', '=', 'EmailAddress') # type: ignore
+        query.add_filter('spec.email', '=', str(principal)) # type: ignore
+        dao = await self.one(Principal, query)
+        if dao is None:
+            return None
+        return await self.get(dao.subject)
+
+    @get.register
+    async def get_by_identifier(self, principal: SubjectIdentifier) -> Subject | None:
+        query = self.query('Principal')
+        query.add_filter('spec.kind', '=', 'SubjectIdentifier') # type: ignore
+        query.add_filter('spec.iss', '=', principal.iss) # type: ignore
+        query.add_filter('spec.sub', '=', principal.sub) # type: ignore
+        dao = await self.one(Principal, query)
+        if dao is None:
+            return None
+        return await self.get(dao.subject)
+
+    @get.register
+    async def get_by_uid(self, uid: int) -> Subject | None:
+        assert isinstance(uid, int), repr(uid)
+        obj = await self.get_model_by_key(Subject, uid)
+        if obj is None:
+            return None
+        assert obj.uid is not None
+        async for principal in self.get_principals(obj.uid):
+            obj.principals.add(principal)
+        return obj
+
+    async def get_principals(self, subject_id: int) -> AsyncGenerator[Principal, None]:
+        query = self.query(Principal)
+        query.add_filter('subject', '=', subject_id) # type: ignore
+        for entity in await self.run_in_executor(query.fetch): # type: ignore
+            yield self.restore(Principal, entity)
+
+    async def resolve(self, identity: int | str) -> Subject | None:
+        """Resolve a principal to a global subject identifier."""
+        return await self.get(int(identity))
 
-    def activate(self) -> None:
-        self.status = SubjectLifecycleType.active
+    async def find_by_principals(
+        self,
+        principals: list[Any]
+    ) -> set[int]:
+        subjects: set[int] = set()
+        for principal in principals:
+            query = self.query(Principal)
+            self.filter_principal(principal, query)
+            subjects.update([
+                int(x['subject']) async for x in self.execute(query, dict[str, int])
+            ])
+        return subjects
+
+    async def persist(self, instance: Subject) -> Subject:
+        await self.put(instance, exclude={'principals', 'uid'})
+        assert instance.uid is not None
+        await self.delete([self.model_key(x) for x in instance._removed_principals]) # type: ignore
+        for principal in instance.principals:
+            await self.put(principal, exclude={'id'})
+        return instance
+
+    @functools.singledispatchmethod
+    def filter_principal(
+        self,
+        principal: EmailAddress | SubjectIdentifier,
+        query: Query
+    ) -> None:
+        raise NotImplementedError(type(principal).__name__)
+
+    @filter_principal.register
+    def filter_emailaddress(
+        self,
+        principal: EmailAddress,
+        query: Query
+    ) -> None:
+        query.add_filter('spec.kind', '=', 'EmailAddress') # type: ignore
+        query.add_filter('spec.email', '=', str(principal)) # type: ignore
 
-    def add_principal(
+    @filter_principal.register
+    def filter_subjectidentifier(
         self,
-        issuer: str,
-        value: PrincipalType,
-        asserted: datetime,
-        trust: bool = False
+        principal: SubjectIdentifier,
+        query: Query
     ) -> None:
-        assert self.uid is not None
-        new = Principal.new(self.uid, issuer, value, asserted=asserted, trust=trust)
-        old = None
-        if new in self.principals:
-            # TODO: ugly
-            principals = list(self.principals)
-            old = principals[principals.index(new)]
-        must_add = any([
-            old is None,
-            old is not None and not old.trust
-        ])
-        if must_add:
-            if old is not None:
-                self._removed_principals.append(old)
-                self.principals.remove(old)
-            self.principals.add(new)
-
-    def add_to_session(self, session: ISessionManager[Any]) -> None:
-        raise NotImplementedError
-    
-    def can_destroy(self) -> bool:
-        return self.status == SubjectLifecycleType.pending
-
-    def can_select_email(self) -> bool:
-        return len([x for x in self.principals if x.spec.kind == 'EmailAddress']) > 1
-
-    def get_email(self) -> EmailAddress:
-        """Return the oldest email adress of the :class:`Subject`. If the
-        :class:`Subject` does not have any email addresses, raise 
-        :exc:`ValueError`.
-        """
-        email: EmailAddress | None = None
-        for principal in sorted(self.principals, key=lambda x: x.asserted.timestamp()):
-            if principal.spec.kind != 'EmailAddress':
-                continue
-            email = principal.spec.email
-            break
-        if email is None:
-            raise ValueError("Subject does not have any email address.")
-        return email
-
-    def get_principals(self) -> list[Principal]:
-        return list([x for x in sorted(self.principals, key=lambda x: x.key)])
-
-    def has_principal(self, principal: PrincipalType) -> bool:
-        p = Principal.new(
-            0,
-            '',
-            principal,
-            asserted=datetime.now(),
-            trust=False
-        )
-        return p in self.principals
-
-    def is_active(self) -> bool:
-        return self.status == SubjectLifecycleType.active
-
-    def is_encypted(self) -> bool:
-        return isinstance(self.claims, VersionedCipherText)
-
-    def merge(self, other: 'Subject') -> None:
-        assert self.uid is not None
-        assert isinstance(self.claims, SubjectClaimSet)
-        assert isinstance(other.claims, SubjectClaimSet)
-        for principal in other.principals:
-            principal.subject = self.uid
-            self.principals.add(principal)
-
-    def needs_fallback_email(self, allow: set[DomainName]) -> bool:
-        return not any([
-            p.spec.email.domain in allow
-            for p in self.principals
-            if p.spec.kind == 'EmailAddress'
-        ])
-    
-    def update_oidc(self, oidc: OIDCToken) -> None:
-        assert not self.is_encypted()
-        assert isinstance(self.claims, SubjectClaimSet)
-        self.claims = SubjectClaimSet.parse_obj({
-            **oidc.dict(exclude_none=True),
-            **self.claims.dict(exclude_none=True)
-        })
-    
-    async def decrypt(self, keychain: ApplicationKeychain)  -> None:
-        assert isinstance(self.claims, VersionedCipherText), self.claims
-        self.claims = await keychain.decrypt(
-            self.claims,
-            parser=lambda _, pt: SubjectClaimSet.parse_raw(pt)
-        )
-    
-    async def encrypt(self, keychain: ApplicationKeychain)  -> None:
-        assert not self.is_encypted()
-        self.claims = await keychain.encrypt(self.claims)
-
-    def dict(self, *args: Any, **kwargs: Any) -> dict[str, Any]:
-        # TODO: A very ugly solution for serialization failure.
-        try:
-            self.principals = list(self.principals) # type: ignore
-            return super().dict(*args, **kwargs)
-        finally:
-            self.principals = set(self.principals)
+        query.add_filter('spec.kind', '=', 'SubjectIdentifier') # type: ignore
+        query.add_filter('spec.iss', '=', principal.iss) # type: ignore
+        query.add_filter('spec.sub', '=', principal.sub) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/models/subjectclaimset.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,157 +2,136 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import datetime
+import os
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import TypeVar
+from typing import Union
 
+import fastapi
 import pydantic
-from headless.ext.oauth2.models.jsonwebtoken import JSONWebToken 
+from headless.ext.oauth2.types import ResponseMode
+from headless.ext.oauth2.types import ResponseType
 
-
-class SubjectClaimSet(JSONWebToken):
-    name: str | None = pydantic.Field(
-        default=None,
-        title="Name",
-        description=(
-            "End-User's full name in displayable form including all name "
-            "parts, possibly including titles and suffixes, ordered "
-            "according to the End-User's locale and preferences."
-        )
-    )
-
-    given_name: str | None = pydantic.Field(
-        default=None,
-        title="Given name",
-        description=(
-            "Given name(s) or first name(s) of the End-User. Note that in some "
-            "cultures, people can have multiple given names; all can be present, "
-            "with the names being separated by space characters."
-        )
-    )
-
-    family_name: str | None = pydantic.Field(
-        default=None,
-        title="Family name",
-        description=(
-            "Surname(s) or last name(s) of the End-User. Note that in some cultures, "
-            "people can have multiple family names or no family name; all can be "
-            "present, with the names being separated by space characters."
-        )
-    )
-
-    middle_name: str | None = pydantic.Field(
-        default=None,
-        title="Middle name",
-        description=(
-            "Middle name(s) of the End-User. Note that in some cultures, people can "
-            "have multiple middle names; all can be present, with the names being "
-            "separated by space characters. Also note that in some cultures, middle "
-            "names are not used."
-        )
-    )
-
-    nickname: str | None = pydantic.Field(
-        default=None,
-        title="Nickname",
-        description=(
-            "Casual name of the End-User that may or may not be the same as "
-            "the `given_name`. For instance, a `nickname` value of `Mike` "
-            "might be returned alongside a `given_name` value of `Michael`."
-        )
-    )
-
-    #preferred_username: str | None = pydantic.Field(
-    #    default=None,
-    #    title="Preferred username",
-    #    description=(
-    #        "Shorthand name by which the End-User wishes to be referred to "
-    #        "at the RP, such as `janedoe` or `j.doe`. This value MAY be "
-    #        "any valid JSON string including special characters such as "
-    #        "`@`, `/`, or whitespace. The RP MUST NOT rely upon this "
-    #        "value being unique, as discussed in Section 5.7 of the OpenID "
-    #        "Connect Core 1.0 specification."
-    #    )
-    #)
-
-    #profile: str | None = pydantic.Field(
-    #    default=None,
-    #    title="Profile URL",
-    #    description=(
-    #        "URL of the End-User's profile page. The contents "
-    #        "of this Web page SHOULD be about the End-User."
-    #    )
-    #)
-
-    picture: str | None = pydantic.Field(
-        default=None,
-        title="Picture",
-        description=(
-            "URL of the End-User's profile picture. This URL MUST refer "
-            "to an image file (for example, a PNG, JPEG, or GIF image "
-            "file), rather than to a Web page containing an image. Note "
-            "that this URL SHOULD specifically reference a profile photo "
-            "of the End-User suitable for displaying when describing the "
-            "End-User, rather than an arbitrary photo taken by the End-User."
-        )
-    )
-
-    website: str | None = pydantic.Field(
-        default=None,
-        title="Website",
-        description=(
-            "URL of the End-User's Web page or blog. This Web page SHOULD "
-            "contain information published by the End-User or an organization "
-            "that the End-User is affiliated with."
-        )
-    )
-
-    gender: str | None = pydantic.Field(
-        default=None,
-        title="Gender",
-        description=(
-            "End-User's gender. Values defined by this specification are "
-            "`female` and `male`. Other values MAY be used when neither "
-            "of the defined values are applicable."
-        )
-    )
-
-    birthdate: datetime.date | str | None = pydantic.Field(
-        default=None,
-        title="Birthdate",
-        description=(
-            "End-User's birthday, represented as an ISO 8601:2004 `YYYY-MM-DD` "
-            "format. The year MAY be `0000`, indicating that it is omitted. "
-            "To represent only the year, `YYYY` format is allowed. Note that "
-            "depending on the underlying platform's date related function, "
-            "providing just year can result in varying month and day, so the "
-            "implementers need to take this factor into account to correctly "
-            "process the dates."
-        )
-    )
-
-    zoneinfo: str | None = pydantic.Field(
-        default=None,
-        title="Timezone",
-        description=(
-            "String from zoneinfo time zone database representing the "
-            "End-User's time zone. For example, `Europe/Paris` or "
-            "`America/Los_Angeles`."
-        )
-    )
-
-    locale: str | None = pydantic.Field(
-        default=None,
-        title="Locale",
-        description=(
-            "End-User's locale, represented as a BCP47 language tag. This is "
-            "typically an ISO 639-1 Alpha-2 language code in lowercase and "
-            "an ISO 3166-1 Alpha-2 country code in uppercase, separated by "
-            "a dash. For example, `en-US` or `fr-CA`. As a compatibility "
-            "note, some implementations have used an underscore as the "
-            "separator rather than a dash, for example, `en_US`; "
-            "Relying Parties MAY choose to accept this locale syntax as well."
-        )
-    )
+from cbra.types import IDependant
+from cbra.core.ioc import override
+from .authorizationrequestobject import AuthorizationRequestObject
+from .authorizationrequestreference import AuthorizationRequestReference
+from .redirecturi import RedirectURI
+
+
+T = TypeVar('T', bound='BaseAuthorizationRequest')
+
+
+class BaseAuthorizationRequest(IDependant, pydantic.BaseModel):
+
+    @classmethod
+    def fromrequest(
+        cls: type[T],
+        client_id: str | None = fastapi.Query(
+            default=None,
+            title="Client ID",
+            description="Identifies the client that is requesting authorization."
+        ),
+        response_type: ResponseType | None = fastapi.Query(
+            default=None,
+            title="Response type",
+            description=(
+                "Informs the authorization server of the desired response type."
+            ),
+            example="code",
+        ),
+        redirect_uri: RedirectURI | None = fastapi.Query(
+            default=None,
+            title="Redirect URI",
+            description=(
+                "The URL to redirect the client to after completing the "
+                "flow. Must be an absolute URI that is served over https.\n\n"
+                "If `redirect_uri` is omitted, the default redirect URI for "
+                "the client specified by `client_id` is used. For clients that "
+                "do not have a redirect URI specified, this produces an error "
+                "state."
+            )
+        ),
+        scope: str | None = fastapi.Query(
+            default=None,
+            title="Scope",
+            description=(
+                "A space-delimited list specifying the requested access scope."
+            ),
+            max_length=512,
+            example="hello.world"
+        ),
+        state: str | None = fastapi.Query(
+            default=None,
+            title="State",
+            description=(
+                "An opaque value used by the client to maintain state between "
+                "the request and callback. The authorization server includes "
+                "this value when redirecting the user-agent back to the client."
+            ),
+            max_length=64,
+            example=bytes.hex(os.urandom(64))
+        ),
+        response_mode: ResponseMode | None = fastapi.Query(
+            default=None,
+            title="Response mode",
+            description=(
+                "Informs the authorization server of the mechanism to be used "
+                "for returning authorization response parameters."
+            ),
+            example="query"
+        ),
+        request: str | None = fastapi.Query(
+            default=None,
+            title="Request",
+            description=(
+                "A JSON Web Token (JWT) whose JWT Claims Set holds the "
+                "JSON-encoded OAuth 2.0 authorization request parameters. "
+                "Must not be used in combination with the `request_uri` "
+                "parameter, and all other parameters except `client_id` "
+                "must be absent.\n\n"
+                "Confidential and credentialed clients must first sign "
+                "the claims using their private key, and then encrypt the "
+                "result with the public keys that are provided by the "
+                "authorization server through the `jwks_uri` specified "
+                "in its metadata."
+            )
+        ),
+        request_uri: str | None = fastapi.Query(
+            default=None,
+            title="Request URI",
+            description=(
+                "References a Pushed Authorization Request (PAR) or a remote "
+                "object containing the authorization request.\n\n"
+                "If the authorization request was pushed to this authorization "
+                "server, then the format of the `request_uri` parameter is "
+                "`urn:ietf:params:oauth:request_uri:<reference-value>`. "
+                "Otherwise, it is an URI using the `https` scheme. If the "
+                "`request_uri` parameter is a remote object, then the external "
+                "domain must have been priorly whitelisted by the client."
+            )
+        )
+    ) -> T:
+        raise NotImplementedError
+
+    @classmethod
+    def __inject__(cls: type[T]) -> Callable[..., Awaitable[T] | T]:
+        return cls.fromrequest
+
+
+class AuthorizationRequest(BaseAuthorizationRequest):
+    __root__: Union[
+        AuthorizationRequestReference,
+        AuthorizationRequestObject
+    ]
+
+    @classmethod
+    @override(BaseAuthorizationRequest.fromrequest) # type: ignore
+    def fromrequest(cls: type[T], **kwargs: Any) -> T: # type: ignore
+        return cls.parse_obj(kwargs)
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/nullauthorizationcontext.py` & `cbra-3.0.0a7/cbra/types/unauthenticatedauthorizationcontext.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import ipaddress
 
-from cbra.types import IAuthorizationContext
-from cbra.types import ISubject
-from cbra.types import NullSubject
+from .iauthorizationcontext import IAuthorizationContext
+from .nullsubject import NullSubject
 
 
-class NullAuthorizationContext(IAuthorizationContext):
-    __module__: str = 'cbra.core.iam'
+class UnauthenticatedAuthorizationContext(IAuthorizationContext):
+    __module__: str = 'cbra.types'
 
     def __init__(
         self,
-        *,
-        remote_host: ipaddress.IPv4Address | str | None,
+        remote_host: ipaddress.IPv4Address | str | None = None
     ):
         if isinstance(remote_host, str):
             remote_host = ipaddress.IPv4Address(remote_host)
-        self._host = remote_host
+        self._remote_host = remote_host
 
     def get_remote_host(self) -> ipaddress.IPv4Address | None:
-        return self._host
+        return self._remote_host
 
-    def get_subject(self) -> ISubject:
+    def get_subject(self) -> NullSubject:
         return NullSubject()
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/nullsubjectesolver.py` & `cbra-3.0.0a7/cbra/types/nullsubjectesolver.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from cbra.types import IRequestPrincipal
-from cbra.types import ISubject
-from cbra.types import ISubjectResolver
-from cbra.types import NullSubject
+from .irequestprincipal import IRequestPrincipal
+from .isubjectresolver import ISubjectResolver
+from .nullsubject import NullSubject
 
 
 class NullSubjectResolver(ISubjectResolver):
-    __module__: str = 'cbra.core.iam'
+    __module__: str = 'cbra.types'
 
-    async def resolve(self, principal: IRequestPrincipal) -> ISubject:
+    async def resolve(self, principal: IRequestPrincipal) -> NullSubject:
         return NullSubject()
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/principalhasher.py` & `cbra-3.0.0a7/cbra/core/iam/principalhasher.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     #: The algorithm that is used to hash principals.
     #:
     #: .. warning::
     #:
     #:   Changing this for an existing dataset will cause duplicate
     #:   principals.
-    algorithm: str = 'sha256'
+    algorithm: str = 'sha1'
 
     def create_hasher(self) -> Any:
         # We use SHA-1 here because its unique enough, as it will
         # be applied on data that is already being constrained
         # such as email addresses or phone numbers. If there is
         # a collision then the user just has bad luck.
         return hashlib.new(self.algorithm)
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/services/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/services/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/services/useronboarding.py` & `cbra-3.0.0a7/cbra/core/iam/services/useronboarding.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,53 +4,45 @@
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from datetime import datetime
 from datetime import timezone
-import functools
 from typing import Any
 
 from canonical import EmailAddress
 from headless.ext.oauth2.models import OIDCToken
-from headless.ext.oauth2.models import SubjectIdentifier
 
 from cbra.core.ioc import instance
 from cbra.core.params import CurrentIssuer
-from ..memorysubjectrepository import MemorySubjectRepository
 from ..models import Subject
 from .. import types
 
 
 class UserOnboardingService:
     """Provides an interface to onboard new and existing subjects."""
     __module__: str = 'cbra.core.iam.services'
     issuer: str
-    exclude_claims: set[str] = {'email', 'email_verified', 'sub'}
     subjects: types.ISubjectRepository
 
     def __init__(
         self,
         issuer: str = CurrentIssuer,
-        subjects: types.ISubjectRepository = instance(
-            name='SubjectRepository',
-            missing=MemorySubjectRepository
-        )
+        subjects: types.ISubjectRepository = instance('SubjectRepository')
     ):
         self.issuer = issuer
         self.subjects = subjects
         self.timestamp = datetime.now(timezone.utc)
 
-    def initialize(self, claims: OIDCToken | None = None) -> Subject:
+    def initialize(self) -> Subject:
         return Subject(
             kind='User',
             created=self.timestamp,
-            seen=self.timestamp,
-            claims=claims.dict(exclude=self.exclude_claims) if claims else {}
+            seen=self.timestamp
         )
     
     async def sync(
         self,
         issuer: str,
         principal: types.PrincipalType
     ) -> tuple[types.Subject, bool]:
@@ -58,14 +50,22 @@
         onboarded = False
         subject = await self.subjects.get(principal)
         if not subject:
             onboarded = True
             subject = self.initialize()
             await self.subjects.persist(subject)
             assert subject.uid is not None
+            subject.add_principal(
+                issuer=self.issuer,
+                value=types.PublicIdentifier(
+                    iss=self.issuer,
+                    sub=str(subject.uid)
+                ),
+                asserted=self.timestamp
+            )
             await self.update(subject, issuer, [principal])
         else:
             onboarded = False
         return subject, onboarded
 
     async def email(
         self,
@@ -86,17 +86,25 @@
         onboarded = False
         if len(found) > 1:
             # The ID token identified multiple subjects and is thus unusable
             # to establish the identity
             raise NotImplementedError(found)
         if not found:
             onboarded = True
-            subject = self.initialize(token)
+            subject = self.initialize()
             await self.subjects.persist(subject)
             assert subject.uid is not None
+            subject.add_principal(
+                issuer=self.issuer,
+                value=types.PublicIdentifier(
+                    iss=self.issuer,
+                    sub=str(subject.uid)
+                ),
+                asserted=self.timestamp
+            )
         else:
             assert len(found) == 1
             subject = await self.subjects.get(found.pop())
 
         # If the subject is None here, then the subject
         # was deleted, but not its principals. This is
         # for now an unrecoverable error.
@@ -106,84 +114,32 @@
         principals = token.principals
         if token.email_verified and token.email:
             # Arbitrarily overwrite the email address here if it is trusted,
             # since we might have received it from other sources.
             subject.add_principal(token.iss, token.email, self.timestamp, trust=True)
             subject.seen = self.timestamp
             principals.remove(token.email)
-        await self.update_oidc(subject, token)
+        await self.update(subject, token.iss, principals)
         return subject, onboarded
 
-    @functools.singledispatchmethod
     async def can_use(
         self,
-        obj: OIDCToken | Subject,
-        *args: Any,
-        **kwargs: Any
-    ) -> bool:
-        raise NotImplementedError(type(obj).__name__)
-
-    @can_use.register
-    async def can_use_oidc_token(
-        self,
-        token: OIDCToken
-    ) -> bool:
-        return len(await self.subjects.find_by_principals(token.principals)) <= 1
-
-    @can_use.register
-    async def can_use_for_subject(
-        self,
         subject: Subject,
         principals: list[types.PrincipalType]
     ) -> bool:
         """Return a boolean indicating if the principals can be used
         by the subject.
         """
         found = await self.subjects.find_by_principals(principals)
         can_use = not found
         if found:
             can_use = (len(found) == 1) and (found.pop() == subject.uid)
         return can_use
 
-    async def destroy(self, uid: int) -> None:
-        await self.subjects.destroy(uid)
-
-    async def get(self, oidc: OIDCToken) -> Subject | None:
-        found = await self.subjects.find_by_principals(oidc.principals)
-        if len(found) > 1:
-            raise RuntimeError("Principals resolve to multiple Subjects.")
-        if not found:
-            return None
-        return await self.subjects.get(found.pop()) # type: ignore
-
-    async def update_oidc(
-        self,
-        subject: types.Subject,
-        oidc: OIDCToken
-    ) -> None:
-        assert subject.uid is not None
-        subject.seen = self.timestamp
-        if oidc.email and not subject.has_principal(oidc.email):
-            subject.add_principal(oidc.iss, oidc.email, self.timestamp, oidc.email_verified)
-        identifier = SubjectIdentifier(iss=oidc.iss, sub=oidc.sub)
-        if not subject.has_principal(identifier):
-            subject.add_principal(oidc.iss, identifier, self.timestamp, True)
-        subject.update_oidc(oidc)
-        await self.subjects.persist(subject)
-
-    async def update(
-        self,
-        subject: types.Subject,
-        iss: str,
-        principals: Any,
-        trust: bool = False
-    ) -> None:
+    async def update(self, subject: types.Subject, iss: str, principals: Any, trust: bool = False) -> None:
         assert subject.uid is not None
         subject.seen = self.timestamp
         for principal in principals:
             if subject.has_principal(principal):
                 continue
             subject.add_principal(iss, principal, self.timestamp, trust=trust)
-        await self.subjects.persist(subject)
-
-    async def persist(self, subject: Subject) -> None:
         await self.subjects.persist(subject)
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/subject.py` & `cbra-3.0.0a7/cbra/core/iam/subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/subjectresolver.py` & `cbra-3.0.0a7/cbra/core/iam/subjectresolver.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/types/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from .iuseronboardingservice import IUserOnboardingService
 from .isubjectrepository import ISubjectRepository
 from .principaltype import PrincipalType
 from .publicidentifier import PublicIdentifier
 from .subject import Subject
-from .subjectlifecycletype import SubjectLifecycleType
 
 
 __all__: list[str] = [
     'IUserOnboardingService',
     'ISubjectRepository',
     'PrincipalType',
     'PublicIdentifier',
     'Subject',
-    'SubjectLifecycleType',
 ]
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/types/isubjectrepository.py` & `cbra-3.0.0a7/cbra/core/iam/types/isubjectrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/types/iuseronboardingservice.py` & `cbra-3.0.0a7/cbra/core/iam/types/iuseronboardingservice.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,57 +2,23 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import overload
-from typing import Any
 from typing import Protocol
 
 from canonical import EmailAddress
 from headless.ext.oauth2.models import OIDCToken
-from headless.ext.oauth2.models import SubjectIdentifier
 
 from .subject import Subject
 from .principaltype import PrincipalType
 
 
 class IUserOnboardingService(Protocol):
-
-    @overload
-    async def can_use(
-        self,
-        subject: Subject,
-        principals: list[EmailAddress | SubjectIdentifier]
-    ) -> bool: ...
-
-    @overload
-    async def can_use(self, token: OIDCToken) -> bool: ...
-
-    @overload
-    async def get(self, oidc: OIDCToken) -> Subject | None: ...
-
-    @overload
-    async def get(self, uid: int) -> Subject | None: ...
-
-    async def update(
-        self,
-        subject: Subject,
-        iss: str,
-        principals: list[Any],
-        trust: bool
-    ) -> None: ...
-
-    async def update_oidc(
-        self,
-        subject: Subject,
-        oidc: OIDCToken
-    ) -> None: ...
-
     def initialize(self) -> Subject: ...
-    async def destroy(self, uid: int) -> None: ...
+    async def can_use(self, subject: Subject, principals: list[PrincipalType]) -> bool: ...
     async def email(self, issuer: str, email: EmailAddress) -> tuple[Subject, bool]: ...
     async def oidc(self, token: OIDCToken) -> tuple[Subject, bool]: ...
-    async def persist(self, subject: Subject) -> None: ...
-    async def sync(self, issuer: str, principal: PrincipalType) -> tuple[Subject, bool]: ...
+    async def sync(self, issuer: str, principal: PrincipalType) -> tuple[Subject, bool]: ...
+    async def update(self, subject: Subject) -> None: ...
```

### Comparing `cbra-2.0.0a91/cbra/core/iam/types/publicidentifier.py` & `cbra-3.0.0a7/cbra/core/iam/types/publicidentifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/iam/types/subject.py` & `cbra-3.0.0a7/cbra/core/iam/types/subject.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,36 +5,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from datetime import datetime
 from typing import Any
 from typing import Protocol
-from typing import TypeVar
-
-from canonical import DomainName
-from canonical import EmailAddress
-from headless.ext.oauth2.models import OIDCToken
 
 from cbra.types import ISessionManager
 from .principaltype import PrincipalType
 
 
-T = TypeVar('T', bound='Subject')
-
-
 class Subject(Protocol):
     uid: int | None
     seen: datetime
 
-    def activate(self) -> None: ...
     def add_principal(self, issuer: str, value: PrincipalType, asserted: datetime, trust: bool = False) -> None: ...
     def add_to_session(self, session: ISessionManager[Any]) -> None: ...
-    def can_destroy(self) -> bool: ...
-    def can_select_email(self) -> bool: ...
-    def get_email(self) -> EmailAddress: ...
-    def get_principals(self) -> list[Any]: ...
-    def has_principal(self, principal: PrincipalType) -> bool: ...
-    def is_active(self) -> bool: ...
-    def merge(self: T, other: T) -> None: ...
-    def needs_fallback_email(self, allow: set[DomainName]) -> bool: ...
-    def update_oidc(self, oidc: OIDCToken) -> None: ...
+    def has_principal(self, principal: PrincipalType) -> bool: ...
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/__init__.py` & `cbra-3.0.0a7/cbra/core/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/ioc/config.py` & `cbra-3.0.0a7/cbra/core/ioc/config.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/ioc/container.py` & `cbra-3.0.0a7/cbra/core/ioc/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,9 +53,9 @@
 
     def provide(self, name: str, spec: dict[str, Any]) -> None:
         self.injected[name] = Dependency.parse_obj({**spec, 'name': name})
         self.injected[name].resolve()
 
     def require(self, name: str) -> Dependency:
         if name not in self.injected:
-            raise DependencyNotSatisfied(name)
+            raise DependencyNotSatisfied
         return self.injected[name]
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/dependency.py` & `cbra-3.0.0a7/cbra/core/ioc/dependency.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,18 @@
     qualname: str
     symbol: Any = None
     instance: Any = None
     args: list[Any] = []
     kwargs: dict[str, Any] = {}
     singleton: bool = False
 
-    def get(self):
-        return self.symbol
-
     def init(self, *args: Any, **kwargs: Any) -> Any:
         assert self.symbol is not None
         return self.instance or self.symbol(*args, **kwargs)
 
     def resolve(self) -> None:
-        if self.symbol is None:
-            try:
-                self.symbol = import_symbol(self.qualname)
-            except ImportError:
-                raise
+        try:
+            self.symbol = import_symbol(self.qualname)
+        except ImportError:
+            raise
         if self.singleton:
             self.instance = self.symbol(*self.args, **self.kwargs)
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/inheriteddependencydecorator.py` & `cbra-3.0.0a7/cbra/core/ioc/inheriteddependencydecorator.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/ioc/injected.py` & `cbra-3.0.0a7/cbra/core/ioc/injected.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,11 @@
             self,
             dependency=self,
             use_cache=False
         )
 
     async def resolve(self, *args: Any, **kwargs: Any) -> Any:
         assert self.ref is not None
-        return self.ref.get()
+        return self.ref.symbol
 
     async def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return await self.resolve(*args, **kwargs)
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/instance.py` & `cbra-3.0.0a7/cbra/core/ioc/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .injected import Injected
 
 
 class Instance(Injected):
 
     @property
     def __signature__(self) -> inspect.Signature:
+        assert self.ref is not None
         return inspect.signature(self.factory)
 
     def callable(self) -> bool:
         return True
 
     async def resolve(self, *args: Any, **kwargs: Any) -> Any:
         assert self.ref is not None
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/loader.py` & `cbra-3.0.0a7/cbra/core/ioc/loader.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/ioc/requirement.py` & `cbra-3.0.0a7/cbra/core/ioc/requirement.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,37 +13,36 @@
 from .dependency import Dependency
 from .dependencynotsatisfied import DependencyNotSatisfied
 
 
 class Requirement:
     __module__: str = 'cbra.core.ioc'
     ref: Dependency | None = None
-    missing: Any
+    missing: str
     name: str
 
     @property
     def factory(self) -> Callable[..., Any]:
-        dep = self.ref or self.missing
-        assert dep is not None, self.name
-        return dep.symbol
+        assert self.ref is not None
+        return self.ref.symbol
 
-    def __init__(self, name: str, missing: Any = NotImplemented) -> None:
+    def __init__(self, name: str, missing: Any = None) -> None:
         self.missing = missing
         self.name = name
 
     def callable(self) -> bool:
         return False
 
     def add_to_container(self, container: Container) -> None:
         if self.ref is not None:
             return
         try:
             self.ref = container.require(self.name)
         except DependencyNotSatisfied:
-            if self.missing in {NotImplemented, None}:
+            if self.missing == NotImplemented:
                 raise
             self.ref = Dependency(
                 name=self.name,
                 qualname='NotImplemented',
                 symbol=self.missing
             )
```

### Comparing `cbra-2.0.0a91/cbra/core/ioc/setting_.py` & `cbra-3.0.0a7/cbra/core/ioc/setting_.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/ioc/test/__init__.py` & `cbra-3.0.0a7/cbra/core/ioc/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/messagepublisher.py` & `cbra-3.0.0a7/cbra/ext/google/aortaendpoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2020-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import logging
+from typing import cast
 from typing import Any
 
 import aorta
-import fastapi
 
-from cbra.types import IDependant
-from .ioc import instance
+from .eventarcendpoint import EventarcEndpoint
+from .messagediscarded import MessageDiscarded
 from .messagerunner import MessageRunner
+from .pubsubmessage import PubsubMessage
 
 
-class MessagePublisher(aorta.MessagePublisher, IDependant):
-    __module__: str = 'cbra.core'
-    logger: logging.Logger = logging.getLogger('aorta')
-    request: fastapi.Request
-    runner: MessageRunner
-
-    def __init__(
-        self,
-        request: fastapi.Request,
-        transport: aorta.types.ITransport = instance('MessageTransport')
-    ):
-        super().__init__(transport=transport)
-        self.request = request
-
-    async def send(
-        self,
-        messages: list[aorta.types.Envelope[Any]],
-        is_retry: bool = False
-    ) -> None:
-        for message in messages:
-            self.logger.debug(
-                "Publishing message %s/%s (id: %s)",
-                message.api_version, message.kind, message.metadata.uid
+class AortaEndpoint(EventarcEndpoint):
+    __module__: str = 'cbra.ext.google'
+    runner: MessageRunner = MessageRunner.depends()
+
+    async def on_message(self, message: PubsubMessage) -> None:
+        try:
+            data = message.get_data()
+        except ValueError:
+            self.logger.critical("Data could not be interpreted as JSON.")
+            raise MessageDiscarded
+        if data is None:
+            raise MessageDiscarded
+        envelope = aorta.parse(data)
+        if envelope is None:
+            self.logger.critical("Message is not an Aorta message type.")
+            raise MessageDiscarded
+        if not envelope.is_known():
+            self.logger.critical(
+                "Received an Aorta message of unknown type "
+                "(kind: %s, version: %s, id: %s)",
+                envelope.kind, envelope.api_version, envelope.metadata.uid
             )
-        return await super().send(messages, is_retry)
+            raise MessageDiscarded
+        assert isinstance(envelope, aorta.types.Envelope)
+        await self.runner.run(cast(aorta.types.Envelope[Any], envelope))
```

### Comparing `cbra-2.0.0a91/cbra/core/messagerunner.py` & `cbra-3.0.0a7/cbra/ext/google/messagerunner.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 import fastapi
 import fastapi.params
 from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_dependant
 from fastapi.dependencies.utils import get_parameterless_sub_dependant
 from fastapi.dependencies.utils import solve_dependencies
 
+import cbra.core as cbra
 from cbra.types import IDependant
-from .ioc import instance
 
 
 class MessageRunner(aorta.LocalRunner, IDependant):
     __module__: str = 'cbra.ext.google'
     request: fastapi.Request
 
     def __init__(
         self,
         request: fastapi.Request,
-        publisher: aorta.types.IPublisher = instance('MessagePublisher')
+        publisher: aorta.types.IPublisher = cbra.instance('MessagePublisher')
     ):
         super().__init__(publisher=publisher)
         self.request = request
 
     async def handle(
         self,
         transaction: aorta.types.ITransaction,
@@ -59,18 +59,16 @@
                     )
                     raise error.exc
                 assert dependant.call is not None
                 assert callable(dependant.call)
                 return await dependant.call(**values)
 
     def get_injectors(self, obj: Any) -> Generator[Dependant, None, None]:
-        for attname, member in inspect.getmembers(obj):
+        for attname, member in inspect.getmembers(self):
             if not isinstance(member, fastapi.params.Depends):
                 continue
-            def setter(attname: str, dep: Any = member):
-                async def f(dep: Any = dep) -> None:
-                    setattr(obj, attname, dep)
-                return f
+            async def f(dep: Any = member):
+                setattr(obj, attname, dep)
             yield get_parameterless_sub_dependant(
-                 depends=fastapi.Depends(setter(attname, member)),
+                 depends=fastapi.Depends(f),
                  path='/'
             )
```

### Comparing `cbra-2.0.0a91/cbra/core/optionsrequesthandler.py` & `cbra-3.0.0a7/cbra/core/optionsrequesthandler.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/params/applicationemailsender.py` & `cbra-3.0.0a7/cbra/core/resource/test/bookpublication.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-# Copyright (C) 2022 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import fastapi
+import datetime
 
-from cbra.types import IEmailSender
-from ..ioc import instance
+import pydantic
 
 
-__all__: list[str] = [
-    'ApplicationEmailSender'
-]
-
-
-async def get(
-    sender: IEmailSender = instance('EmailSender')
-) -> IEmailSender:
-    return sender
-
-
-ApplicationEmailSender: IEmailSender = fastapi.Depends(get)
+class BookPublication(pydantic.BaseModel):
+    published: datetime.date
+    country_code: str
```

### Comparing `cbra-2.0.0a91/cbra/core/requesthandler.py` & `cbra-3.0.0a7/cbra/core/requesthandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import asyncio
 import collections
 import inspect
-import logging
 import uuid
-from datetime import datetime
-from datetime import timezone
 from typing import get_args
 from typing import get_origin
 from typing import Awaitable
 from typing import Any
 from typing import Callable
 from typing import Generic
 from typing import TypeVar
@@ -24,23 +21,20 @@
 from inspect import Parameter
 
 import fastapi
 import fastapi.params
 import pydantic
 
 from cbra.types import Abortable
-from cbra.types import ETagSet
 from cbra.types import IEndpoint
 from cbra.types import IntegerPathParameter
 from cbra.types import MutableSignature
 from cbra.types import PathParameter
 from cbra.types import StringPathParameter
 from cbra.types import UUIDPathParameter
-from .params import IfMatchDestructive
-from .params import IfMatchRequestHeader
 
 
 E = TypeVar('E', bound='IEndpoint')
 T = TypeVar('T', bound='RequestHandler[Any]')
 
 
 class RequestHandler(Generic[E]):
@@ -65,15 +59,14 @@
     _path_types: dict[type, type[PathParameter]] = {
         int: IntegerPathParameter,
         str: StringPathParameter,
         uuid.UUID: UUIDPathParameter
     }
     _signature: inspect.Signature | None
     include_in_schema: bool = True
-    logger: logging.Logger = logging.getLogger('cbra.endpoint')
     response_model_by_alias: bool = False
     status_code: int = 200
 
     @property
     def attname(self) -> str:
         return str.lower(self._method)
 
@@ -247,22 +240,14 @@
             annotation=fastapi.Request
         )
         dependencies['response'] = Parameter(
             kind=Parameter.POSITIONAL_OR_KEYWORD,
             name='response',
             annotation=fastapi.Response
         )
-        if getattr(cls, 'versioned', False):
-            dependencies['etag'] = Parameter(
-                kind=Parameter.POSITIONAL_OR_KEYWORD,
-                name='etag',
-                annotation=ETagSet,
-                default=IfMatchDestructive if self.can_mutate() else IfMatchRequestHeader
-            )
-            self._class_params.add('etag')
         self._class_params.add('request')
         self._class_params.add('response')
 
         parameters = list(dependencies.values())
         for i, p in enumerate(parameters):
             parameters[i] = self.preprocess_parameter(p) or p
         parameters, return_annotation = self.preprocess_signature(
@@ -345,23 +330,17 @@
                 and issubclass(p.annotation, pydantic.BaseModel),
             isinstance(p, Parameter) and (where=='handler')\
                 and get_origin(p.annotation) == dict,
             not isinstance(p, Parameter)\
                 and isinstance(p, self._injectables),
             not isinstance(p, Parameter) and self.is_injectable(p)
         ])
-    
-    def can_write(self) -> bool:
-        return self.method in {'POST', 'PUT', 'PATCH', 'DELETE'}
-    
-    def can_mutate(self) -> bool:
-        return self.method in {'PUT', 'PATCH'}
 
     def is_pydantic_union(self, obj: Any):
-        origin = get_origin(obj) # type: ignore
+        origin = get_origin(obj)
         if origin != Union:
             return False
         return all([
             isinstance(x, pydantic.main.ModelMetaclass)
             for x in get_args(obj)
         ])
 
@@ -376,16 +355,14 @@
         self,
         parameters: dict[str, Parameter],
         return_annotation: Any
     ) -> tuple[list[Parameter], Any]:
         return list(parameters.values()), return_annotation
 
     async def preprocess_value(self, name: str, value: Any) -> Any:
-        if name == 'etag' and value:
-            value = ETagSet.toset(value)
         return value
 
     async def process_response(
         self,
         endpoint: IEndpoint,
         response: fastapi.Response | pydantic.BaseModel | None
     ) -> fastapi.Response:
@@ -393,16 +370,14 @@
             response = fastapi.Response(status_code=204)
         elif isinstance(response, pydantic.BaseModel):
             response = fastapi.responses.Response(
                 headers={'Content-Type': "application/json"},
                 status_code=self.status_code,
                 content=response.json(
                     by_alias=endpoint.response_model_by_alias,
-                    exclude=endpoint.response_model_exclude,
-                    exclude_none=endpoint.response_model_exclude_none,
                     indent=2,
                 )
             )
         elif isinstance(response, dict):
             response = fastapi.responses.JSONResponse(
                 status_code=self.status_code,
                 content=response
@@ -420,15 +395,14 @@
     async def _run_handler(self, **params: Any) -> Any:
         # Construct the init arguments, instance attributes and handler
         # arguments from the known parameters.
         assert self._class is not None
         attrs: dict[str, Any] = {}
         init: dict[str, Any] = {}
         kwargs: dict[str, Any] = {}
-
         for param in self._dependencies.values():
             value = await self.preprocess_value(param.name, params.pop(param.name))
 
             # PathParameter instances expose a clean() method
             # that immetialy cause the endpoint to return 404
             # on validation failure.
             if inspect.isclass(param.annotation)\
@@ -444,47 +418,25 @@
 
         if params:
             raise TypeError("Received unknown arguments.")
 
         # Initialize the endpoint and set its attributes, proceed
         # to invoke the handler.
         endpoint: IEndpoint = self._class(**init)
-        endpoint.timestamp = datetime.now(timezone.utc)
         endpoint.__dict__.update(attrs)
         response = await self.process_response(
             endpoint,
             await endpoint.run_handler(self._func, **kwargs)
         )
 
-        # TODO: Make this configurable on the endpoint/resource.
-        response.headers.setdefault('Cache-Control', 'no-cache, no-store, must-revalidate')
-        response.headers.setdefault('Expires', '0')
-        response.headers.setdefault('Permissions-Policy', 'interest-cohort=()')
-        response.headers.setdefault('Pragma', 'no-cache')
-        response.headers.setdefault('Referrer-Policy', 'no-referrer')
-        response.headers.setdefault('X-Content-Type-Options', 'nosniff')
-        response.headers.setdefault('X-Frame-Options', 'DENY')
-        response.headers.setdefault('X-DNS-Prefetch-Control', 'off')
-        response.headers.setdefault('X-XSS-Protection', '0')
-
-        if endpoint.session.is_dirty():
-            self.logger.debug("Setting session cookie")
+        # Persist the session only if there is a successful response.
+        if (200 <= response.status_code < 400) \
+        and endpoint.session.is_dirty():
             await endpoint.session.add_to_response(response)
 
-        if endpoint.csrf_protect:
-            await endpoint.session
-            response.set_cookie(
-                key='csrftoken',
-                value=endpoint.session.csrf,
-                httponly=True,
-                max_age=86400,
-                samesite='strict',
-                secure=True,
-            )
-
         # Copy the headers from the endpoint response.
         response.raw_headers = [
             *response.raw_headers,
             *endpoint.response.raw_headers
         ]
 
         return response
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/__init__.py` & `cbra-3.0.0a7/cbra/core/resource/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from .replace import Replace
 from .resource import Resource
 from .resourcemodel import ResourceModel
 from .resourceprotocol import ResourceProtocol
 from .resourcetype import ResourceType
 from .retrieve import Retrieve
 from .update import Update
-from .versioned import Versioned
 
 
 __all__: list[str] = [
     'Create',
     'Collection',
     'Delete',
     'Mutable',
@@ -29,15 +28,14 @@
     'Replace',
     'Resource',
     'ResourceModel',
     'ResourceProtocol',
     'ResourceType',
     'Retrieve',
     'Update',
-    'Versioned',
 ]
 
 
 class Mutable(
     Create,
     Delete,
     Replace,
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/collectionaction.py` & `cbra-3.0.0a7/cbra/core/resource/collectionaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/create.py` & `cbra-3.0.0a7/cbra/core/resource/create.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/createaction.py` & `cbra-3.0.0a7/cbra/core/resource/createaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Any
 from typing import TypeVar
 
 import fastapi
 import pydantic
 
 from cbra.types import IEndpoint
-from .iresource import IResource
 from .resourceaction import ResourceAction
 
 
 T = TypeVar('T', bound='CreateAction')
 
 
 class CreateAction(ResourceAction):
@@ -37,40 +36,36 @@
         return True
 
     def get_return_annotation(self) -> Any:
         return self.endpoint.model.__response_model__
 
     def get_openapi_responses(
         self,
-        cls: type[IResource],
         responses: dict[int | str, Any]
     ) -> dict[int | str, Any]:
         responses.update({
             409: {
                 'description': (
                     'The unique properties of an existing '
                     f'**{self.endpoint.verbose_name}** conflict'
                 )
             }
         })
-        return super().get_openapi_responses(cls, responses)
+        return super().get_openapi_responses(responses)
 
     def get_write_model(self) -> type[pydantic.BaseModel]:
         return self.endpoint.model.__create_model__
 
     def is_detail(self) -> bool:
         return False
 
-    def needs_resource(self) -> bool:
-        return True
-
     def parse_resource(self, resource: pydantic.BaseModel) -> pydantic.BaseModel:
-        return self.endpoint.model.__create_model__.parse_obj(resource.dict())
+        return self.endpoint.model.parse_obj(resource.dict())
 
     async def process_response(
         self,
         endpoint: IEndpoint,
         response: fastapi.Response | pydantic.BaseModel | None
-    ) -> fastapi.Response:
+    ) -> fastapi.Response | pydantic.BaseModel | None:
         if isinstance(response, pydantic.BaseModel):
             response = self.response_model.parse_obj(response.dict())
         return await super().process_response(endpoint, response)
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/customaction.py` & `cbra-3.0.0a7/cbra/core/resource/customaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 T = TypeVar('T', bound='CustomAction')
 
 
 class CustomAction(DetailAction):
     action: str
     status_code: int
     path: str
-    use_resource_model: bool = False
     _summary: str
 
     @property
     def summary(self) -> str:
         return self._summary
 
     @classmethod
@@ -47,24 +46,19 @@
     ):
         self.action = action
         self.path = action
         self.status_code = status_code
         self._summary = summary
         super().__init__(*args, **kwargs)
 
-    def can_mutate(self) -> bool:
-        # Custom actions are always detail actions, so POST
-        # requests are considered mutations.
-        return super().can_mutate() or self.method == "POST"
+    def can_write(self) -> bool:
+        return False
 
     def get_url_pattern(
         self,
         prefix: str | None,
         endpoint: type[IResource] | None = None
     ) -> str:
         return f'{super().get_url_pattern(prefix, endpoint)}/{self.path}'
 
     def is_detail(self) -> bool:
-        return True
-
-    def needs_resource(self) -> bool:
-        return False
+        return True
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/delete.py` & `cbra-3.0.0a7/cbra/core/resource/delete.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/deleteaction.py` & `cbra-3.0.0a7/cbra/core/resource/deleteaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 from typing import TypeVar
 
 from cbra.types import Operation
 from .detailaction import DetailAction
-from .iresource import IResource
 
 
 T = TypeVar('T', bound='DeleteAction')
 
 
 class DeleteAction(DetailAction):
     action: str = 'destroy'
@@ -31,23 +30,22 @@
         return cls(name=name, method='DELETE', func=func)
 
     def can_write(self) -> bool:
         return False
 
     def get_openapi_responses(
         self,
-        cls: type[IResource],
         responses: dict[int | str, Any]
     ) -> dict[int | str, Any]:
         responses.update({
             202: {
                 'description': (
                     f'The **{self.endpoint.verbose_name}** is scheduled for '
                     'deletion'
                 ),
                 'model': Operation
             }
         })
-        return super().get_openapi_responses(cls, responses)
+        return super().get_openapi_responses(responses)
 
     def get_return_annotation(self) -> Any:
         return self.endpoint.model.__response_model__ | Operation
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/detail.py` & `cbra-3.0.0a7/cbra/core/resource/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
 
-class Detail:
+class Viewer:
     __module__: str = 'cbra.core'
 
     async def get_object(self) -> Any:
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/detailaction.py` & `cbra-3.0.0a7/cbra/core/resource/detailaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from cbra.types import IEndpoint
 from .iresource import IResource
 from .resourceaction import ResourceAction
 
 
 class DetailAction(ResourceAction):
-    use_resource_model: bool = True
 
     def get_url_pattern(
         self,
         prefix: str | None,
         endpoint: type[IResource] | None = None
     ) -> str:
         endpoint = endpoint or self.endpoint
@@ -59,15 +58,14 @@
 
     async def process_response(
         self,
         endpoint: IEndpoint,
         response: fastapi.Response | pydantic.BaseModel | None
     ) -> fastapi.Response:
         if isinstance(response, pydantic.BaseModel)\
-        and not isinstance(response, self.response_model)\
-        and self.use_resource_model:
-            response = self.response_model.parse_obj(response.dict(by_alias=endpoint.response_model_by_alias))
+        and not isinstance(response, self.response_model):
+            response = self.response_model.parse_obj(response.dict())
         return await super().process_response(endpoint, response)
 
     def parse_resource(self, resource: pydantic.BaseModel) -> pydantic.BaseModel:
         parser = self.get_write_model()
         return parser.parse_obj(resource.dict())
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/iresource.py` & `cbra-3.0.0a7/cbra/core/resource/iresource.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,23 @@
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
-import aorta
-
 from cbra.types import IEndpoint
 from .persister import Persister
 from .resourcemodel import ResourceModel
 
 
 class IResource(IEndpoint, Persister):
     model: type[ResourceModel]
     path_name: str
-    publisher: aorta.types.IPublisher
     response_model_by_alias: bool = False
-    response_model_exclude: set[str] | None = None
-    response_model_exclude_none: bool = False
     resource_name: str
     resource_id: Any
     verbose_name: str
     verbose_name_plural: str
 
     async def get_object(self) -> Any:
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/listaction.py` & `cbra-3.0.0a7/cbra/core/resource/listaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/persister.py` & `cbra-3.0.0a7/cbra/core/resource/persister.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/queryresult.py` & `cbra-3.0.0a7/cbra/core/resource/queryresult.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/replace.py` & `cbra-3.0.0a7/cbra/core/resource/replace.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/replaceaction.py` & `cbra-3.0.0a7/cbra/core/resource/replaceaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,11 +32,8 @@
     def can_write(self) -> bool:
         return True
 
     def get_return_annotation(self) -> Any:
         return self.endpoint.model.__response_model__
 
     def get_write_model(self) -> type[pydantic.BaseModel]:
-        return self.endpoint.model.__replace_model__
-
-    def needs_resource(self) -> bool:
-        return True
+        return self.endpoint.model.__replace_model__
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/resource.py` & `cbra-3.0.0a7/cbra/core/resource/resource.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,78 +2,43 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from datetime import datetime
 from typing import Any
 
 import fastapi
-from starlette.datastructures import URL
 
-from cbra.types import BaseModel
 from cbra.types import RequestPrincipal
-from cbra.types import IEmailSender
 from cbra.types import IRoutable
 from ..iam import AuthorizationContextFactory
-from ..ioc import instance
-from ..messagepublisher import MessagePublisher
-from ..params import ApplicationEmailSender
 from ..sessions import RequestSession
-from .const import CURSOR_PARAM_NAME
 from .iresource import IResource
 from .resourcemodel import ResourceModel
 from .resourcetype import ResourceType
 
 
 class Resource(IResource, metaclass=ResourceType):
     __abstract__: bool = True
     __actions__: list[type[IRoutable]] = []
     __module__: str = 'cbra.core'
     context_factory: AuthorizationContextFactory = AuthorizationContextFactory.depends()
-    cursor_param_name: str = CURSOR_PARAM_NAME
-    email: IEmailSender = ApplicationEmailSender
-    max_limit: int = 100
     model: type[ResourceModel]
-    path_prefix: str | None = None
     principal: RequestPrincipal = RequestPrincipal.depends()
-    publisher: MessagePublisher = instance('MessagePublisher')
-    response_model: BaseModel
-    response_model_by_alias: bool = True
     session: RequestSession = RequestSession.depends()
-    timestamp: datetime
 
-    def __init_subclass__(cls, model: type[ResourceModel] | None):
-        if model is not None:
-            cls.model = model
+    def __init_subclass__(cls, model: type[ResourceModel]):
+        cls.model = model
 
     @classmethod
     def add_to_router(cls, router: fastapi.FastAPI, **kwargs: Any) -> None:
-        path = str.rstrip(kwargs.get('path') or '', '/')
-        if cls.path_prefix:
-            if not str.startswith(cls.path_prefix, '/'):
-                raise ValueError(f'{cls.__name__}.path_prefix must start with a slash.')
-            kwargs['path'] = f'{path}{cls.path_prefix}'
         for action in cls.__actions__:
             kwargs.setdefault('response_model_by_alias', cls.response_model_by_alias)
             action.add_to_router(cls, router, **kwargs)
 
-    def adapt(self, obj: Any) -> Any:
+    def adapt(self, obj: Any) -> ResourceModel:
         """Adapt an object of any kind to a :class:`ResourceModel` instance.
         The default implementation simply returns the object.
         """
-        return obj
-    
-    def parse_obj(self, obj: Any) -> Any:
-        return self.model.parse_obj(obj)
-    
-    def reverse(self, action: str, params: dict[str, Any]) -> URL:
-        query: dict[str, str] = {}
-        cursor = params.pop(self.cursor_param_name, None)
-        url = self.request.url_for(f'{self.path_name}.{action}')
-        if cursor is not None:
-            query[self.cursor_param_name] = cursor
-        if query:
-            url = url.include_query_params(**query)
-        return url
+        return obj
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourceaction.py` & `cbra-3.0.0a7/cbra/core/resource/resourceaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         return f'{self.endpoint.resource_name.lower()}_id'
 
     @property
     def summary(self) -> str:
         # TODO
         return self.name_template.format(
             article=self.article,
-            name=self.endpoint.verbose_name,
+            name=self.name,
             pluralname=self.endpoint.verbose_name_plural
         )
 
     def add_to_class(self, cls: type[IResource]) -> None: # type: ignore
         # Construct a resource identifier from the unprefixed path.
         formatter = Formatter()
         params: list[str] = [
@@ -96,107 +96,87 @@
             cls.resource_id = Model.depends()
             cls.__annotations__['resource_id'] = Model
 
         return super().add_to_class(cast(type[IEndpoint], cls))
 
     def add_to_router( # type: ignore
         self,
-        cls: type[IResource],
+        cls: IResource,
         router: fastapi.APIRouter, **kwargs: Any
     ) -> None:
         kwargs.setdefault('status_code', self.status_code)
         kwargs.setdefault('summary', self.summary)
         tags: list[str] = kwargs.setdefault('tags', [])
         tags.append(self.name)
         kwargs.update({
             'path': self.get_url_pattern(kwargs.get('path')),
-            'name': f'{cls.path_name}.{self.action}',
             'response_description': self.response_description.format(
                 name=self.name,
                 pluralname=self.endpoint.verbose_name_plural,
                 article=self.article
             )
         })
-        kwargs['responses'] = self.get_openapi_responses(cls, kwargs.get('responses') or {})
-        return super().add_to_router(cls, router, **kwargs) # type: ignore
+        kwargs['responses'] = self.get_openapi_responses(kwargs.get('responses') or {})
+        return super().add_to_router(cls, router, **kwargs)
+
+    def can_write(self) -> bool:
+        raise NotImplementedError
 
     def get_openapi_responses(
         self,
-        cls: type[IResource],
         responses: dict[int | str, Any]
     ) -> dict[int | str, Any]:
-        if getattr(cls, 'versioned', None):
-            responses.setdefault(412, {
-                'description': f"The **{cls.model.__name__}** was changed in between requests",
-                'headers': {
-                    'ETag': {
-                        'schema': {'type': 'string'},
-                        'description': (
-                            "The most recent version of the resource. Use this (opaque) value "
-                            "as the `If-Match` header on subsequent `POST`, `PUT` or `PATCH` "
-                            "requests."
-                        )
-                    }
-                }
-            })
-        return {
-            **responses,
-            **getattr(self._func, 'responses', {})
-        }
+        return {**responses, **getattr(self._func, 'responses', {})}
 
     def get_url_pattern(self, prefix: str | None, endpoint: type[IResource] | None = None) -> str:
         endpoint = endpoint or self.endpoint
         path: str | None = prefix
         if path is None:
             path = f'/{endpoint.path_name}'
         else:
-            path = f"{str.rstrip(path, '/')}/{endpoint.path_name}"
-        assert str.startswith(path, '/')
+            path = f"{str.lstrip(path, '/')}/{endpoint.path_name}"
         return path
 
     def get_write_model(self) -> type[pydantic.BaseModel]:
         raise NotImplementedError
 
     def is_detail(self) -> bool:
         raise NotImplementedError
 
-    def needs_resource(self) -> bool:
-        return False
-
     def parse_resource(self, resource: pydantic.BaseModel) -> pydantic.BaseModel:
         raise NotImplementedError
 
     def preprocess_parameter(self, p: Parameter) -> Parameter | None:
         """Hook to modify a parameter just before it is added to the
         new signature.
         """
 
     def preprocess_signature(
         self,
         parameters: dict[str, Parameter],
         return_annotation: Any
     ) -> tuple[list[Parameter], Any]:
-        if self.can_write() and self.needs_resource():
+        if self.can_write() and 'resource' not in parameters:
             self._handler_params.add('resource')
             parameters['resource'] = Parameter(
                 kind=Parameter.POSITIONAL_ONLY,
                 name='resource',
                 annotation=self.get_write_model(),
             )
         return super().preprocess_signature(parameters, return_annotation)
 
     def validate_handler(
         self,
         func: Callable[..., Awaitable[Any] | Any],
         signature: MutableSignature
     ) -> tuple[Callable[..., Awaitable[Any] | Any], MutableSignature]:
-        if not signature.has_param('resource') and self.can_write() and self.needs_resource():
+        if not signature.has_param('resource') and self.can_write():
             raise TypeError(
                 f"{self._endpoint_name}.{self.action} must accept "
                 "the 'resource' positional argument."
             )
         return super().validate_handler(func, signature)
 
     async def preprocess_value(self, name: str, value: Any) -> Any:
-        if name == 'resource' and self.needs_resource():
+        if name == 'resource':
             value = self.parse_resource(value)
         return await super().preprocess_value(name, value)
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourceidentifier.py` & `cbra-3.0.0a7/cbra/core/resource/resourceidentifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourcelist.py` & `cbra-3.0.0a7/cbra/core/resource/resourcelist.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourcelistmetadata.py` & `cbra-3.0.0a7/cbra/core/resource/resourcelistmetadata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourcemodel.py` & `cbra-3.0.0a7/cbra/core/resource/resourcemodel.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourcemodeltype.py` & `cbra-3.0.0a7/cbra/core/resource/resourcemodeltype.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,41 +32,39 @@
         **params: Any
     ):
         annotations: dict[str, type] = namespace.get('__annotations__') or {}
         is_abstract = namespace.pop('__abstract__', False)
         if not is_abstract:
             # Collect readonly fields to create the CreateResourceRequest
             # ReplaceResourceRequest and UpdateResourceRequest models.
-            create_fields: list[tuple[str, type, pydantic.fields.FieldInfo | None]] = []
-            key_fields: list[tuple[str, type, pydantic.fields.FieldInfo]] = []
-            update_fields: list[tuple[str, type, pydantic.fields.FieldInfo | None]] = []
-            response_fields: list[tuple[str, type, pydantic.fields.FieldInfo | None]] = []
+            create_fields: list[tuple[str, type, pydantic.main.FieldInfo | None]] = []
+            key_fields: list[tuple[str, type, pydantic.main.FieldInfo]] = []
+            update_fields: list[tuple[str, type, pydantic.main.FieldInfo | None]] = []
+            response_fields: list[tuple[str, type, pydantic.main.FieldInfo | None]] = []
             for attname, class_ in annotations.items():
                 field = namespace.get(attname)
-                if isinstance(field, pydantic.fields.FieldInfo):
+                if isinstance(field, pydantic.main.FieldInfo):
                     response_fields.append((attname, class_, cls.get_field(field, 'response')))
                     if field.extra.get('primary_key'):
                         key_fields.append((attname, class_, field))
-                        continue
-                    if field.extra.get('read_only'):
-                        continue
+                    continue
                 create_fields.append((attname, class_, cls.get_field(field, 'create')))
                 update_fields.append((attname, class_, cls.get_field(field, 'update')))
                 response_fields.append((attname, class_, cls.get_field(field, 'response')))
 
             PartialModel = type('Partial{name}Request', (pydantic.BaseModel,), {
                 '__annotations__': {attname: class_ for attname, class_, _ in create_fields},
                 **{name: field for name, _, field in create_fields if field is not None},
             })
             UpdateResourceRequest = type(f'Update{name}Request', (pydantic.BaseModel,), {
                 '__annotations__': {attname: cls.allow_empty(class_) for attname, class_, _ in update_fields},
                 **{name: field for name, _, field in update_fields if field is not None},
             })
             ResponseModel = type(name, (pydantic.BaseModel,), {
-                '__annotations__': {attname: cls.ensure_required(field, class_) for attname, class_, field in response_fields},
+                '__annotations__': {attname: cls.ensure_required(class_) for attname, class_, _ in response_fields},
                 **{name: field for name, _, field in response_fields if name in namespace},
             })
             namespace.update({
                 '__create_model__': type(f'Create{name}Request', (PartialModel,), {}),
                 '__update_model__': UpdateResourceRequest,
                 '__replace_model__': type(f'Replace{name}Request', (PartialModel,), {}),
                 '__response_model__': ResponseModel,
@@ -85,44 +83,46 @@
                         required=[name]
                     )
                 })
             })
             if key_fields:
                 namespace.update({
                     '__key_model__': type(f'{name}Identifier', (ResourceIdentifier,), {
-                        '__annotations__': {attname: cls.ensure_required(field, class_) for attname, class_, field in key_fields},
+                        '__annotations__': {attname: cls.ensure_required(class_) for attname, class_, _ in key_fields},
                         **{name: field for name, _, field in key_fields if name in namespace},
                     })
                 })
 
         return super().__new__(cls, name, bases, namespace, **params) # type: ignore
 
     @staticmethod
     def allow_empty(value: Any) -> Any:
         return value | None
 
     @staticmethod
-    def ensure_required(field: pydantic.fields.FieldInfo | None, value: Any) -> Any:
-        # TODO: this function makes no sense
-        origin = get_origin(value) # type: ignore
-        if origin == types.UnionType and field and field.extra.get('read_only'):
-            args: list[Any] = [x for x in get_args(value) if x != types.NoneType]
+    def ensure_required(value: Any) -> Any:
+        origin = get_origin(value)
+        if origin == types.UnionType:
+            args = [x for x in get_args(value) if x != types.NoneType]
             if not args:
                 raise TypeError("Field can not only contain None.")
+            value = args[0]
+            if len(args) > 1:
+                value = Union[tuple(args)] # type: ignore
         return value
 
     @staticmethod
     def get_field(
-        field: pydantic.fields.FieldInfo | None,
+        field: pydantic.main.FieldInfo | None,
         action: str
-    ) -> pydantic.fields.FieldInfo | None:
+    ) -> pydantic.main.FieldInfo | None:
         field = copy.deepcopy(field)
-        if isinstance(field, pydantic.fields.FieldInfo) and field.extra.get('read_only'):
+        if isinstance(field, pydantic.main.FieldInfo) and field.extra.get('read_only'):
             if action not in {'response', 'key'}:
                 return
             field.update_from_config({
                 'default': ...,
             })
-        elif isinstance(field, pydantic.fields.FieldInfo) and action == 'update':
+        elif isinstance(field, pydantic.main.FieldInfo) and action == 'update':
             field.update_from_config({'default': None})
         return field
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourceoptionsrequesthandler.py` & `cbra-3.0.0a7/cbra/core/resource/resourceoptionsrequesthandler.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/resourcetype.py` & `cbra-3.0.0a7/cbra/core/resource/resourcetype.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import inspect
 import itertools
 import re
 from typing import Any
 
 import inflect
 
-from cbra.types import IDependant
 from .createaction import CreateAction
 from .customaction import CustomAction
 from .deleteaction import DeleteAction
 from .listaction import ListAction
 from .replaceaction import ReplaceAction
 from .resourceaction import ResourceAction
 from .retrieveaction import RetrieveAction
@@ -43,25 +41,15 @@
         cls,
         name: str,
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         **params: Any
     ):
         actions: list[ResourceAction] = []
-        annotations: dict[str, type] = namespace.get('__annotations__') or {}
         is_abstract = namespace.pop('__abstract__', False)
-
-        # Inspect annotations for injectables.
-        for attname, hint in annotations.items():
-            if not inspect.isclass(hint)\
-            or not issubclass(hint, IDependant)\
-            or attname in namespace:
-                continue
-            namespace[attname] = hint.depends()
-
         if not is_abstract:
             Model = params.get('model', None)
             if Model is None:
                 raise TypeError('The `model` class argument is required.')
 
             # Collect actions and convert them to ResourceAction instances, if
             # necessary. First inspect the bases for known actions, and then
@@ -95,15 +83,14 @@
                 if not action.is_detail(): collection_actions.add(action.method)
                 actions.append(action)
 
             # Update the namespace with the actions and resource name.
             namespace.update({
                 '__actions__': actions,
                 'resource_name': Model.__name__,
-                'response_model': Model.__response_model__
             })
             
             # Some naming stuff.
             verbose_name = namespace.get('verbose_name') or namespace['resource_name']
             verbose_name_plural = namespace.get('verbose_name_plural')\
                 or engine.plural_noun(verbose_name)
             namespace.update({
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/retrieve.py` & `cbra-3.0.0a7/cbra/core/resource/retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 from .detail import Detail
 
 
 class Retrieve(Detail):
     __module__: str = 'cbra.core'
 
     async def retrieve(self, *args: Any) -> Any:
-        resource = self.adapt(await self.get_object()) # type: ignore
+        resource = await self.get_object()
         if resource is None:
             raise NotFound
         return resource
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/retrieveaction.py` & `cbra-3.0.0a7/cbra/core/resource/retrieveaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/test/__init__.py` & `cbra-3.0.0a7/cbra/core/resource/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/test/book.py` & `cbra-3.0.0a7/cbra/core/resource/test/book.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/test/bookpublication.py` & `cbra-3.0.0a7/cbra/types/verifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Copyright (C) 2021-2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import datetime
+from typing import Protocol
 
-import pydantic
 
+class Verifier(Protocol):
 
-class BookPublication(pydantic.BaseModel):
-    published: datetime.date
-    country_code: str
+    async def verify(
+        self,
+        signature: bytes,
+        message: bytes,
+    ) -> bool:
+        ...
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/test/bookresource.py` & `cbra-3.0.0a7/cbra/core/resource/test/bookresource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/core/resource/update.py` & `cbra-3.0.0a7/cbra/core/resource/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         new = await self.perform_update(
             old=old,
             new=resource
         )
         if not await self.can_update(old, new):
             raise Forbidden
         await self.persist(new, create=False)
-        return self.adapt(new)
+        return new
 
     async def perform_update(
         self,
         old: T,
         new: T
     ) -> T:
         return old.merge(new)
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/updateaction.py` & `cbra-3.0.0a7/cbra/core/resource/updateaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,11 +32,8 @@
     def can_write(self) -> bool:
         return True
 
     def get_return_annotation(self) -> Any:
         return self.endpoint.model.__response_model__
 
     def get_write_model(self) -> type[pydantic.BaseModel]:
-        return self.endpoint.model.__update_model__
-
-    def needs_resource(self) -> bool:
-        return True
+        return self.endpoint.model.__update_model__
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/versioned.py` & `cbra-3.0.0a7/cbra/types/notfound.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+from .abortable import Abortable
 
 
-class Versioned:
-    """Enables use of the `ETag` and `If-Match` headers."""
-    __module__: str = 'cbra'
-    versioned: bool = True
+class NotFound(Abortable):
+    __module__: str = 'cbra.types'
+    status_code: int = 404
```

### Comparing `cbra-2.0.0a91/cbra/core/resource/viewer.py` & `cbra-3.0.0a7/cbra/types/notauthorized.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# Copyright (C) 2021-2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
+from .abortable import Abortable
 
 
-class Viewer:
-    __module__: str = 'cbra.core'
-
-    async def get_object(self) -> Any:
-        raise NotImplementedError
+class NotAuthorized(Abortable):
+    __module__: str = 'cbra.types'
+    status_code: int = 401
```

### Comparing `cbra-2.0.0a91/cbra/core/secretkey.py` & `cbra-3.0.0a7/cbra/core/secretkey.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 # there is no public documentation.
                 'key': {'cek': secret_key}
             })
             await cls.keychain.add(cls.signing_key_name, spec)
         return self
 
     def __init__(self):
-        self.keychain = type(self).keychain
+        self.keychain = SecretKey.keychain
 
     async def sign(self, value: bytes | str, encoding: str = 'utf-8') -> str:
         """Sign the given value."""
         if isinstance(value, str):
             value = str.encode(value, encoding=encoding)
         return b64encode_str(await self.signing_key.sign(value))
```

### Comparing `cbra-2.0.0a91/cbra/core/utils.py` & `cbra-3.0.0a7/cbra/core/utils.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/bff/params/currentresourceserver.py` & `cbra-3.0.0a7/cbra/types/forbidden.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import fastapi
+from .abortable import Abortable
 
 
-async def get(
-    server: str = fastapi.Path(
-        default=...,
-        alias="resource",
-        title="Resource server"
-    )
-):
-    pass
+class Forbidden(Abortable):
+    __module__: str = 'cbra.types'
+    status_code: int = 403
```

### Comparing `cbra-2.0.0a91/cbra/ext/bff/resourceserverclient.py` & `cbra-3.0.0a7/cbra/types/conflict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from cbra.core.conf import settings
-from cbra.types import IDependant
+from .abortable import Abortable
 
 
-class ResourceServerClient(IDependant):
-    __module__: str = 'cbra.ext.bff'
+class Conflict(Abortable):
+    __module__: str = 'cbra.types'
+    status_code: int = 409
```

### Comparing `cbra-2.0.0a91/cbra/ext/cache/__init__.py` & `cbra-3.0.0a7/cbra/types/opaquebearertokenprincipal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import fastapi
+from typing import Any
 
-from cbra.types import ICache
-from .cacheconfiguration import CacheConfiguration
-from .memorycache import MemoryCache
+from .httpheaderprincipal import HTTPHeaderPrincipal
 
 
-__all__: list[str] = [
-    'CacheConfiguration',
-    'MemoryCache'
-]
-
-
-def cache(name: str) -> ICache:
-    config = CacheConfiguration.get(name)
-    async def f(impl: ICache = fastapi.Depends(config.factory)) -> ICache:
-        await impl.connect(config)
-        return impl
-    return fastapi.Depends(f)
-
+class OpaqueBearerTokenPrincipal(HTTPHeaderPrincipal):
 
+    @classmethod
+    def parse_scheme(
+        cls,
+        values: dict[str, Any],
+        scheme: str,
+        value: str
+    ) -> dict[str, Any]:
+        if scheme != 'bearer':
+            raise ValueError('this principal requires the Bearer scheme')
+        values.update({'token': value})
+        return values
```

### Comparing `cbra-2.0.0a91/cbra/ext/email/accesscodeextension.py` & `cbra-3.0.0a7/cbra/types/stringpathparameter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,24 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .basewrapextension import BaseWrapExtension
+from typing import Any
 
+from .pathparameter import PathParameter
+from .notfound import NotFound
 
-class AccessCodeExtension(BaseWrapExtension):
-    tags: set[str] = {'accesscode'}
-    template: str = 'accesscode.html.j2'
+
+class StringPathParameter(PathParameter):
+    __module__: str = 'cbra.types'
+    type: str = 'string'
+
+    @classmethod
+    def clean(cls, v: Any) -> str:
+        try:
+            return str(v)
+        except (TypeError, ValueError):
+            raise NotFound
```

### Comparing `cbra-2.0.0a91/cbra/ext/email/paragraphextension.py` & `cbra-3.0.0a7/cbra/types/uuidpathparameter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,26 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .basewrapextension import BaseWrapExtension
+import uuid
+from typing import Any
 
+from .pathparameter import PathParameter
+from .notfound import NotFound
 
-class ParagraphExtension(BaseWrapExtension):
-    tags: set[str] = {'paragraph'}
-    template: str = 'paragraph.html.j2'
+
+class UUIDPathParameter(PathParameter):
+    __module__: str = 'cbra.types'
+    format: str = 'uuid'
+    type: str = 'string'
+
+    @classmethod
+    def clean(cls, v: Any) -> uuid.UUID:
+        try:
+            return uuid.UUID(v)
+        except (TypeError, ValueError):
+            raise NotFound
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/__init__.py` & `cbra-3.0.0a7/cbra/ext/google/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,43 +76,35 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .aortadebugendpoint import AortaDebugEndpoint
 from .aortaendpoint import AortaEndpoint
-from .basedatastorerepository import BaseDatastoreRepository
 from .datastorequeryresult import DatastoreQueryResult
 from .datastorerepository import DatastoreRepository
 from .datastoresubjectrepository import DatastoreSubjectRepository
 from .datastoresubjectresolver import DatastoreSubjectResolver
 from .eventarcendpoint import EventarcEndpoint
 from .googleendpoint import GoogleEndpoint
 from .googlepubsubtransport import GooglePubsubTransport
-from .googlesecret import GoogleSecret
 from .googleserviceaccountprincipal import GoogleServiceAccountPrincipal
 from .messagepublished import MessagePublished
-from .polymorphicdatastorerepository import PolymorphicDatastoreRepository
 from .pubsubmessage import PubsubMessage
 from .service import Service
 
 
 __all__: list[str] = [
-    'AortaDebugEndpoint',
     'AortaEndpoint',
-    'BaseDatastoreRepository',
     'DatastoreQueryResult',
     'DatastoreRepository',
     'DatastoreSubjectResolver',
     'DatastoreSubjectRepository',
     'EventarcEndpoint',
     'GoogleEndpoint',
     'GooglePubsubTransport',
-    'GoogleSecret',
     'GoogleServiceAccountPrincipal',
     'MessagePublished',
-    'PolymorphicDatastoreRepository',
     'PubsubMessage',
     'Service'
 ]
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/datastorequeryresult.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/queryauthorizeresponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,33 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Generic
-from typing import TypeVar
+from typing import Any
 
+import pydantic
+from headless.ext import oauth2
 
-T = TypeVar('T')
+from .responsevalidationfailure import ResponseValidationFailure
 
 
-class DatastoreQueryResult(Generic[T]):
-    __module__: str = 'cbra.ext.google'
-    token: str | None
-    items: list[T]
+class QueryAuthorizeResponse(pydantic.BaseModel):
+    code: str
+    state: str | None = None
 
-    def __init__(self, token: str | None, entities: list[T]) -> None:
-        self.token = token or None
-        self.items = entities
+    async def obtain(
+        self,
+        client: oauth2.Client,
+        state: str | None,
+        **kwargs: Any
+    ) -> oauth2.TokenResponse:
+        if state != self.state:
+            raise ResponseValidationFailure(
+                "The state parameters do not match."
+            )
+        return await client.token(
+            oauth2.AuthorizationEndpointResponse.parse_obj(self.dict()).__root__,
+            **kwargs
+        )
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/datastorerepository.py` & `cbra-3.0.0a7/cbra/ext/google/datastorerepository.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,52 +3,47 @@
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import functools
-import json
 from typing import get_origin
 from typing import Any
 from typing import AsyncGenerator
 from typing import TypeVar
 
 from google.cloud.datastore import Client
 from google.cloud.datastore import Entity
 from google.cloud.datastore import Key
 from google.cloud.datastore import Query
 
 from cbra.core import ioc
-from cbra.ext.security import ApplicationKeychain
 from cbra.types import PersistedModel
 from .datastorequeryresult import DatastoreQueryResult
 from .runner import Runner
 
 
 M = TypeVar('M', bound=PersistedModel)
 Q = TypeVar('Q', bound=PersistedModel)
 R = TypeVar('R')
 
 
 class DatastoreRepository(Runner):
     __module__: str = 'cbra.ext.google'
     client: Client
-    keychain: ApplicationKeychain
     model: type[Any]
 
     def __init__(
         self,
-        client: Client | Any = ioc.inject('GoogleDatastoreClient'),
-        keychain: ApplicationKeychain = ApplicationKeychain.depends()
+        client: Client | Any = ioc.inject('GoogleDatastoreClient')
     ):
         if not isinstance(client, Client):
             raise TypeError(f"Invalid client: {repr(client)}")
         self.client = client
-        self.keychain = keychain
 
     async def allocate(self, model: type[Any], n: int = 1) -> list[int]:
         base = self.key(kind=model.__name__)
         return [
             x.id for x in
             await self.run_in_executor(
                 functools.partial( # type: ignore
@@ -162,15 +157,15 @@
             # entities' key.
             exclude.add(field)
         elif len(instance.__key__) == 1:
             exclude.add(instance.__key__[0][0]) # type: ignore
         else:
             raise NotImplementedError
         key = self.model_key(instance)
-        data = json.loads(instance.json(exclude=exclude))
+        data = instance.dict(exclude=exclude)
         assert instance.__surrogate__ is not None
         entity = Entity(key=key)
         entity.update(data) # type: ignore
         await self.run_in_executor(self.client.put, entity) # type: ignore
         return entity.key # type: ignore
 
     def construct_key(self, model: Any) -> Key:
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/datastoresubjectresolver.py` & `cbra-3.0.0a7/cbra/ext/google/datastoresubjectresolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ) -> None:
         self.repo = repo
 
     async def resolve_session(
         self,
         principal: SessionRequestPrincipal
     ) -> RequestSubject | NullSubject:
-        if principal.claims.uid is None:
+        if principal.subject is None:
             return NullSubject()
-        subject = await self.repo.resolve(principal.claims.uid)
+        subject = await self.repo.resolve(principal.subject.sub)
         if subject is None:
             return NullSubject()
         assert subject.uid is not None # nosec
         return RequestSubject(
             id=str(subject.uid),
             email=principal.claims.email,
             principal=principal
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/environ.py` & `cbra-3.0.0a7/cbra/ext/google/environ.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import os
 
 
 __all__: list[str] = [
     'GOOGLE_DATASTORE_NAMESPACE',
-    'GOOGLE_HOST_PROJECT',
     'GOOGLE_SERVICE_PROJECT',
 ]
 
 
 GOOGLE_DATASTORE_NAMESPACE: str | None = os.environ.get('GOOGLE_DATASTORE_NAMESPACE')
-
-GOOGLE_HOST_PROJECT: str | None = os.environ.get('GOOGLE_HOST_PROJECT')
-
 GOOGLE_SERVICE_PROJECT: str | None = os.environ.get('GOOGLE_SERVICE_PROJECT')
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/eventarcendpoint.py` & `cbra-3.0.0a7/cbra/ext/google/eventarcendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/googleendpoint.py` & `cbra-3.0.0a7/cbra/ext/google/googleendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/googleserviceaccountprincipal.py` & `cbra-3.0.0a7/cbra/ext/google/googleserviceaccountprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/messagepublished.py` & `cbra-3.0.0a7/cbra/ext/google/messagepublished.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/params/__init__.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationflowstate.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .applicationstoragebucket import ApplicationStorageBucket
-from .applicationstorageclient import ApplicationStorageClient
+from typing import Any
+from typing import Protocol
 
 
-__all__: list[str] = [
-    'ApplicationStorageBucket',
-    'ApplicationStorageClient'
-]
+class IAuthorizationFlowState(Protocol):
+    nonce: str
+    redirect_uri: str
+    state: str
+
+    def is_valid(self, params: Any) -> bool: ...
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/pubsubmessage.py` & `cbra-3.0.0a7/cbra/ext/google/pubsubmessage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/resourcemetadata.py` & `cbra-3.0.0a7/cbra/ext/google/resourcemetadata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/runner.py` & `cbra-3.0.0a7/cbra/ext/google/runner.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/google/service.py` & `cbra-3.0.0a7/cbra/ext/google/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,23 +4,18 @@
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
-from google.cloud import logging
-
 from cbra.core import Application
-from cbra.core.conf import settings
 from cbra.core.utils import parent_signature
-from .aortadebugendpoint import AortaDebugEndpoint
 from .aortaendpoint import AortaEndpoint
 from .environ import GOOGLE_DATASTORE_NAMESPACE
-from .environ import GOOGLE_HOST_PROJECT
 from .environ import GOOGLE_SERVICE_PROJECT
 
 
 class Service(Application):
     __module__: str = 'cbra.ext.google'
 
     @parent_signature(Application.__init__)
@@ -37,30 +32,8 @@
             )
             self.container.provide('SubjectResolver', {
                 'qualname': 'cbra.ext.google.DatastoreSubjectResolver'
             })
             self.container.provide('SubjectRepository', {
                 'qualname': 'cbra.ext.google.DatastoreSubjectRepository'
             })
-        self.add(AortaEndpoint, path="/.well-known/aorta")
-        if settings.DEBUG:
-            self.add(AortaDebugEndpoint, path="/.well-known/aorta/debug")
-
-    def logging_config(self):
-        if settings.DEPLOYMENT_ENV == 'local':
-            return super().logging_config()
-        client = logging.Client(project=GOOGLE_HOST_PROJECT or GOOGLE_SERVICE_PROJECT)
-        client.setup_logging() # type: ignore
-        config = super().logging_config()
-        config['formatters']['google-cloud'] = {
-            '()': "cbra.ext.google.logging.JSONFormatter",
-        }
-        config['handlers']['default'] = {
-            'class': 'google.cloud.logging.handlers.CloudLoggingHandler',
-            'client': client,
-            'formatter': 'google-cloud',
-            'labels': {
-                'kind': 'service'
-            }
-        }
-    
-        return config
+        self.add(AortaEndpoint, path="/.well-known/aorta")
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/types/__init__.py` & `cbra-3.0.0a7/cbra/types/nullrequestprincipal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .idatastorecursor import IDatastoreCursor
-from .idatastoreentity import IDatastoreEntity
-from .idatastorekey import IDatastoreKey
-from .idatastorequery import IDatastoreQuery
+import pydantic
 
+from .irequestprincipal import IRequestPrincipal
 
-__all__: list[str] = [
-    'IDatastoreCursor',
-    'IDatastoreEntity',
-    'IDatastoreKey',
-    'IDatastoreQuery',
-]
+
+class NullRequestPrincipal(IRequestPrincipal, pydantic.BaseModel):
+
+    def is_anonymous(self) -> bool:
+        return True
+
+    def has_audience(self) -> bool:
+        return False
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/types/idatastoreentity.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationserverstorage.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
-from typing import Iterable
-from typing import Iterator
 from typing import Protocol
+from typing import TypeVar
 
-from .idatastorekey import IDatastoreKey
+from .iauthorizationflowstate import IAuthorizationFlowState
 
+M = TypeVar('M')
 
-class IDatastoreEntity(Protocol):
-    __module__: str = 'cbra.ext.google.types'
-    key: IDatastoreKey
-    def update(self, obj: Iterable[tuple[str, Any]] | dict[str, Any]) -> None: ...
-    def __iter__(self) -> Iterator[tuple[str, Any]]: ...
-    def __len__(self) -> int: ...
-    def __setitem__(self, k: str, v: Any) -> None: ...
+
+class IAuthorizationServerStorage(Protocol):
+    __module__: str = 'cbra.ext.oauth2.types'
+
+
+    async def persist(
+        self,
+        obj: Any
+    ) -> None:
+        ...
+
+    async def destroy(self, obj: Any) -> None: ...
+    async def get_state(self, key: str) -> IAuthorizationFlowState | None:
+        ...
```

### Comparing `cbra-2.0.0a91/cbra/ext/google/types/idatastorekey.py` & `cbra-3.0.0a7/examples/endpoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,28 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Protocol
+import uuid
 
+import fastapi
+import uvicorn
 
-class IDatastoreKey(Protocol):
-    __module__: str = 'cbra.ext.google.types'
-    id: int
-    name: str
+import cbra
+
+
+class BookEndpoint(cbra.Endpoint):
+
+    async def get(self, book_id: uuid.UUID):
+        print(self.response)
+
+
+app = fastapi.FastAPI(docs_url='/ui')
+BookEndpoint.add_to_router(app, path='/books/{book_id}')
+
+
+if __name__ == '__main__':
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/authorizationcodecallbackendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/authorizationcodecallbackendpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import fastapi
 from headless.ext import oauth2
 
 from cbra.core.conf import settings
-from .endpoints import AuthorizationServerEndpoint
+from .endpoint import AuthorizationServerEndpoint
 from .types import RedirectParameters
 from .types import ResponseValidationFailure
 from .types import QueryAuthorizeResponse
 
 
 class AuthorizationCodeCallbackEndpoint(AuthorizationServerEndpoint):
     """Handles a redirect from an OAuth 2.x/OpenID Connect
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/authorizationserverstorage.py` & `cbra-3.0.0a7/cbra/ext/oauth2/memorystorage.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,65 +2,41 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import cast
-from typing import Any
+import collections
 from typing import TypeVar
 
-import cbra.core as cbra
-from cbra.core.iam.types import ISubjectRepository
-from cbra.core.iam.types import Subject
-from .types import IAuthorizationServerStorage
-from .types import ObjectIdentifier
+from .basestorage import BaseStorage
+from .models import AuthorizationState
+from .models import AuthorizationServerModel
 
 
 T = TypeVar('T')
 
 
-class AuthorizationServerStorage:
+class MemoryStorage(BaseStorage):
+    """An in-memory implementation of :class:`~cbra.ext.oauth2.BaseStorage`."""
     __module__: str = 'cbra.ext.oauth2'
-    app: IAuthorizationServerStorage
-    public: IAuthorizationServerStorage
-    subjects: ISubjectRepository
-
-    def __init__(
-        self,
-        app: IAuthorizationServerStorage = cbra.instance(
-            name='_ApplicationStorage'
-        ),
-        public: IAuthorizationServerStorage = cbra.instance(
-            name='AuthorizationServerStorage'
-        ),
-        subjects: ISubjectRepository = cbra.instance(
-            name='SubjectRepository'
-        )
-    ):
-        self.app = app
-        self.public = public
-        self.subjects = subjects
-
-    async def get_subject(self, *args: Any, **kwargs: Any) -> None | Subject:
-        return await self.subjects.get(*args, **kwargs)
-
-    async def destroy(self, obj: Any) -> None:
-        return await self.public.destroy(obj)
-
-    async def fetch(self, oid: ObjectIdentifier[T]) -> T | None:
-        return await self.app.fetch(oid) or await self.public.fetch(oid)
-
-    async def get(
-        self,
-        cls: type[T],
-        *args: Any,
-        **kwargs: Any
-    ) -> T | None:
-        if cls == Subject:
-            return cast(T, await self.get_subject(*args, **kwargs))
-        return await self.app.get(cls, *args, **kwargs)\
-            or await self.public.get(cls, *args, **kwargs)
+    objects: dict[str, dict[str, AuthorizationServerModel]] = collections.defaultdict(dict)
 
-    async def persist(self, obj: Any) -> None:
-        return await self.public.persist(obj)
+    @classmethod
+    def clear(cls) -> None:
+        cls.objects = collections.defaultdict(dict)
+
+    def __init__(self):
+        self.objects = MemoryStorage.objects
+
+    async def destroy(self, obj: AuthorizationServerModel) -> None:
+        self.objects[type(obj).__name__].pop(obj.__key__[0][1], None) # type: ignore
+
+    async def get_state(self, key: str) -> AuthorizationState | None:
+        return self._get(AuthorizationState, key)
+
+    async def persist_state(self, obj: AuthorizationState) -> None:
+        self.objects[type(obj).__name__][obj.state] = obj
+
+    def _get(self, Model: type[T], key: str) -> T | None:
+        return self.objects[Model.__name__].get(key)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/clientkeysendpoint.py` & `cbra-3.0.0a7/examples/oauth2-server.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,18 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from ckms.core import Keychain
-from ckms.types import JSONWebKeySet
+from cbra.ext import google
+from cbra.ext.oauth2 import AuthorizationEndpoint
 
-from cbra.core.params import ApplicationKeychain
-from .endpoints import AuthorizationServerEndpoint
 
+app = google.Service(docs_url='/ui')
+app.add(AuthorizationEndpoint, path='/oauth2/authorize')
 
-class ClientKeysEndpoint(AuthorizationServerEndpoint):
-    keychain: Keychain = ApplicationKeychain
-    name: str = 'oauth2.client-jwks'
-    status_code: int = 303
-    summary: str = 'Application Client JWKS Endpoint'
-    path: str = '/client-jwks.json'
 
-    async def get(self) -> JSONWebKeySet:
-        return self.keychain.as_jwks(private=False)
+if __name__ == '__main__':
+    import uvicorn
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/loginendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/loginendpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 import fastapi
 from headless.ext import oauth2
 
 import cbra.core as cbra
 from cbra.core.conf import settings
 from cbra.types import Forbidden
 from cbra.types import NotFound
-from .endpoints import AuthorizationServerEndpoint
+from .endpoint import AuthorizationServerEndpoint
 from .types import LoginResponse
 from .models import AuthorizationState
 
 
 class LoginEndpoint(AuthorizationServerEndpoint):
     __module__: str = 'cbra.ext.oauth2'
     name: str = 'oauth2.login'
     nonce_cookie_name: str = 'oidc.nonce'
-    path: str = '/login'
     redirect_cookie_name: str = 'oauth2.redirect-uri'
     state_cookie_name: str = 'oauth2.state'
     status_code: int = 303
     summary: str = 'Login Endpoint'
     tags: list[str] = ['OAuth 2.x/OpenID Connect']
 
     async def get(
@@ -69,15 +68,15 @@
         if client is None:
             raise NotFound
         params = AuthorizationState.new(redirect_uri=success_url)
         redirect_uri = self.request.url_for('oauth2.callback', client_id=client_id)
         async with client:
             url = await client.authorize(
                 state=params.state,
-                redirect_uri=str(redirect_uri),
+                redirect_uri=redirect_uri,
                 scope={'openid', 'email'},
                 nonce=params.nonce,
                 prompt='select_account'
             )
 
         # Persist the state so that the callback endpoint can find the needed
         # information to forward the request.
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/authorization.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/authorization.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationcode.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/jarmauthorizeresponse.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import secrets
+from typing import Any
 
 import pydantic
+from headless.ext import oauth2
 
-from ..types import AuthorizationCode as AuthorizationCodeType
 
+class JARMAuthorizeResponse(pydantic.BaseModel):
+    jwt: str
 
-class AuthorizationCode(pydantic.BaseModel):
-    value: AuthorizationCodeType = pydantic.Field(
-        default_factory=lambda: secrets.token_urlsafe(48)
-    )
+    async def obtain(
+        self,
+        client: oauth2.Client,
+        **kwargs: Any
+    ) -> oauth2.TokenResponse:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationrequestobject.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
 import pydantic
+from headless.ext import oauth2
 
+from .invalidauthorizeresponse import InvalidAuthorizeResponse
 
-class AuthorizationRequestObject(pydantic.BaseModel):
-    request: str
-    remote_host: str
 
-    async def load(
+class UnsupportedAuthorizationResponse(pydantic.BaseModel):
+
+    async def obtain(
         self,
-        client: Any,
-        storage: Any,
-        session_id: str
-    ):
-        raise NotImplementedError
+        client: oauth2.Client,
+        **kwargs: Any
+    ) -> oauth2.TokenResponse:
+        raise InvalidAuthorizeResponse
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/authorizationstate.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/authorizationstate.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/baseclient.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/loginresponse.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import pydantic
-from ..types import RedirectURI
 
 
-class BaseClient(pydantic.BaseModel):
-
-    def get_redirect_uri(self, uri: RedirectURI | None) -> RedirectURI:
-        raise NotImplementedError
+class LoginResponse(pydantic.BaseModel):
+    redirect_uri: str = pydantic.Field(
+        default=...,
+        title='Redirect URI',
+        description=(
+            'The URI to which the user-agent must redirect in order '
+            'to initiate the authorization flow.'
+        )
+    )
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/basetokenrequest.py` & `cbra-3.0.0a7/cbra/ext/oauth2/endpoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
+"""
+.. _ref-guides-integrating-an-oauth2-authorization-server
 
-import pydantic
+=============================================
+Integrating an OAuth 2.x authorization server
+=============================================
+"""
+import cbra.core as cbra
+from cbra.core.conf import settings
+from cbra.core.iam import ISubjectRepository
+from cbra.core.iam.types import IUserOnboardingService
+from cbra.core.iam.services import UserOnboardingService
+from .memorystorage import MemoryStorage
+from .types import IAuthorizationServerStorage
 
-from ..types import RFC9068AccessToken
-from ..types import IAuthorizationServerStorage
-from ..types import IssuedAccessToken
 
+class AuthorizationServerEndpoint(cbra.Endpoint):
+    onboard: IUserOnboardingService = cbra.ioc.instance(
+        name='SubjectOnboardingService',
+        missing=UserOnboardingService
+    )
+    storage: IAuthorizationServerStorage = cbra.ioc.instance(
+        name='AuthorizationServerStorage',
+        missing=MemoryStorage
+    )
+    subjects: ISubjectRepository = cbra.ioc.instance('SubjectRepository')
 
-class BaseTokenRequest(pydantic.BaseModel):
-
-    async def register_issued_access_token(
-        self,
-        sub: int | str,
-        token: RFC9068AccessToken,
-        signed: str,
-        scope: list[str],
-        storage: IAuthorizationServerStorage,
-        claims: dict[str, Any]
-    ) -> None:
-        """Registers the access token as being issued, so that it
-        can be later revoked or introspected.
-        """
-        issued = IssuedAccessToken.parse_rfc9068(
-            token,
-            claims=claims,
-            scope=scope,
-            signed_token=signed,
-            sub=sub
-        )
-        await storage.persist(issued)
+    def get_issuer(self) -> str:
+        return settings.OAUTH2_ISSUER or\
+            f'{self.request.url.scheme}://{self.request.url.netloc}'
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/beginonboardrequest.py` & `cbra-3.0.0a7/cbra/types/icredential.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import pydantic
 
 
-class BeginOnboardRequest(pydantic.BaseModel):
-    ctx: str
-    next: str
-    request: str
-    interact: str
+class ICredential:
+    """Used in conjunction with a :class:`IRequestPrincipal` implementation
+    to establish the identity of a subject.
+    """
+    __module__: str = 'cbra.types'
+
+    def is_verified(self) -> bool:
+        """Some credentials are verified simply by existing."""
+        return False
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/downstreamproviderconfig.py` & `cbra-3.0.0a7/cbra/types/sessionclaims.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import pydantic
+from canonical import EmailAddress
 
-from ..types import OIDCProvider
 
-
-class DownstreamProviderConfig(pydantic.BaseModel):
-    required: bool = False
-    providers: list[OIDCProvider] = []
+class SessionClaims(pydantic.BaseModel):
+    iss: str | None = None
+    sub: str | None = None
+    email: EmailAddress | None = None
+    email_verified: bool = False
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/emailchallenge.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/responsemodenotsupported.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,13 +2,22 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import pydantic
-from canonical import EmailAddress
+import fastapi
 
+from cbra.types import Abortable
 
-class EmailChallenge(pydantic.BaseModel):
-    email: EmailAddress
+
+class ResponseModeNotSupported(Abortable):
+    status_code: int = 400
+
+    def __init__(self, mode: str):
+        self.mode = mode
+
+    async def as_response(self) -> fastapi.Response:
+        return fastapi.responses.PlainTextResponse(
+            content=f'Response mode {self.mode} is not supported by this server.'
+        )
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/externalauthorizationstate/recoveryauthorizationstate.py` & `cbra-3.0.0a7/cbra/types/isessionfactory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Literal
+from typing import Generic
+from typing import TypeVar
 
-from .baseauthorizationstate import BaseAuthorizationState
+from .session import Session
 
 
-class RecoveryAuthorizationState(BaseAuthorizationState):
-    kind: Literal['set-recovery'] = 'set-recovery'
+M = TypeVar('M', bound=Session)
+
+
+class ISessionFactory(Generic[M]):
+    __module__: str = 'cbra.types'
+    model: type[M]
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/grant.py` & `cbra-3.0.0a7/cbra/types/icredentialverifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Awaitable
-from typing import Callable
-from typing import TypeAlias
-from typing import Union
+# type: ignore
+from typing import Any
+from typing import Generic
+from typing import TypeVar
 
-import pydantic
-from headless.ext.oauth2.models import TokenResponse
+from .icredential import ICredential
 
-from .authorizationcodegrant import AuthorizationCodeGrant
-from .clientcredentialsgrant import ClientCredentialsGrant
-from .refreshtokengrant import RefreshTokenGrant
 
+P = TypeVar('P')
 
-GrantType: TypeAlias = Union[
-    AuthorizationCodeGrant,
-    ClientCredentialsGrant,
-    RefreshTokenGrant
-]
 
+class ICredentialVerifier(Generic[P]):
+    """Knows how to verify a credential attached to a principal."""
+    __module__: str = 'cbra.types'
 
-class Grant(pydantic.BaseModel):
-    __root__: GrantType
-
-    def handle(
+    async def verify(
         self,
-        handler: Callable[[GrantType], Awaitable[TokenResponse]]
-    ) -> Awaitable[TokenResponse]:
-        return handler(self.__root__)
+        principal: P,
+        credential: ICredential | None,
+        providers: set[str] | None = None
+    ) -> bool:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/patchauthorizationrequest.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/invalidauthorizeresponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import pydantic
+import fastapi
 
+from cbra.types import Abortable
 
-class PatchAuthorizationRequest(pydantic.BaseModel):
-    deny: bool = False
-    email: str | None = None
-    logout: bool = False
+
+class InvalidAuthorizeResponse(Abortable):
+    status_code: int = 400
+    reason: str = (
+        "The authorization server returned an unsupported or "
+        "unrecognized response."
+    )
+
+    async def as_response(self) -> fastapi.Response:
+        return fastapi.responses.PlainTextResponse(content=self.reason)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/models/resourceowner.py` & `cbra-3.0.0a7/cbra/core/resource/collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import pydantic
-from canonical import EmailAddress
+from typing import Any
 
-from ..types import PairwiseIdentifier
-from ..types import ResourceOwnerIdentifier
-from ..types import RequestedScope
+from cbra.types import IQueryResult
+from .resourcemodel import ResourceModel
 
 
-class ResourceOwner(pydantic.BaseModel):
-    client_id: str
-    consents: set[str] = set()
-    email: EmailAddress | None = None
-    ppid: PairwiseIdentifier
-    resources: set[str] = set()
+class Collection:
+    __module__: str = 'cbra.core'
+    cursor_param_name: str = '_c'
+    model: type[ResourceModel]
 
-    @property
-    def id(self) -> ResourceOwnerIdentifier:
-        return ResourceOwnerIdentifier(client_id=self.client_id, sub=self.ppid.sub)
-    
-    @property
-    def sub(self) -> int:
-        return self.ppid.sub
+    async def list(self) -> Any:
+        result = await self.filter(None)
+        return self.model.__list_model__.parse_obj({
+            'apiVersion': 'v1',
+            'kind': f'{self.model.__name__}List',
+            'metadata': {
+                'nextUrl': self.get_next_url(result.token)
+            },
+            'items': [self.adapt(x) for x in result.items] # type: ignore
+        })
+
+    async def filter(self, params: Any) -> IQueryResult[Any]:
+        raise NotImplementedError
     
-    def consent_required(self, scope: list[RequestedScope]) -> list[RequestedScope]:
-        return [
-            x for x in scope
-            if x.name not in self.consents
-            and x.requires_consent()
-        ]
+    def get_next_url(self, token: str | None) -> str | None:
+        if not token:
+            return None
+        return self.reverse('list', params={self.cursor_param_name: token}) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/oidcregistrationendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/oidcregistrationendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/params/cookieclientidentifier.py` & `cbra-3.0.0a7/cbra/types/iroutable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+from typing import Any
+
 import fastapi
 
 
-CookieClientIdentifier: str = fastapi.Cookie(
-    default=...,
-    title="Client ID",
-    description="The client that requested the downstream authentication.",
-    alias='oauth2.client_id'
-)
+class IRoutable:
+    __module__: str = 'cbra.types'
+    response_model_by_alias: bool = False
+
+    @classmethod
+    def add_to_router(cls, endpoint: Any, router: fastapi.FastAPI, **kwargs: Any) -> None:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/params/currentissuer.py` & `cbra-3.0.0a7/cbra/core/params/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import fastapi
 
 from cbra.core.conf import settings
-from cbra.types import Request
+from ..secretkey import SecretKey
 
 
 __all__: list[str] = [
-    'CurrentIssuer'
+    'ApplicationSecretKey'
 ]
 
+ApplicationSecretKey: SecretKey = SecretKey.depends()
 
-def get_issuer(request: Request) -> str:
-    return settings.OAUTH2_ISSUER or\
-        f'{request.url.scheme}://{request.url.netloc}'
 
-
-CurrentIssuer: str = fastapi.Depends(get_issuer)
+def current_issuer(request: fastapi.Request) -> str:
+    return settings.OAUTH2_ISSUER\
+        or f'{request.url.scheme}://{request.url.netloc}'
+CurrentIssuer: str = fastapi.Depends(current_issuer)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/params/downstreamtokentesponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/redirectparameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,106 @@
+# Copyright (C) 2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import TypeVar
+from typing import Union
+
 import fastapi
-from headless.ext.oauth2.models import TokenResponse
+import pydantic
+from headless.ext import oauth2
 
-from cbra.types import Request
-from ..types import OIDCProvider
-from ..types import FatalAuthorizationException
-from ..types import IExternalAuthorizationState
-from .localopenidprovider import LocalOpenIdProvider
-from .localauthorizationrequeststate import LocalAuthorizationRequestState
-
-
-__all__: list[str] = [
-    'DownstreamTokenResponse'
-]
-
-async def get(
-    request: Request,
-    provider: OIDCProvider = LocalOpenIdProvider,
-    state: IExternalAuthorizationState = LocalAuthorizationRequestState,
-    code: str | None = fastapi.Query(
-        default=None,
-        title='Authorization code',
-        description=(
-            'The authorization code generated by the authorization server. '
-            'Required if using the Authorization Code Flow and the response '
-            'mode is `query`, otherwise this parameter is ignored.'
-        )
-    ),
-    iss: str | None = fastapi.Query(
-        default=None,
-        title='Issuer',
-        description=(
-            'Identifies the authorization server that redirected to '
-            'this endpoint, as defined in RFC 9207. If the client supports '
-            'OAuth 2.0 Authorization Server Issuer Identification, then '
-            'this parameter is **required**, if the response mode is not '
-            'JWT Secured Authorization Response Mode (JARM) per RFC 9101.\n\n'
-            'The `iss` parameter value is the issuer identifier of '
-            'the authorization server that created the authorization '
-            'response, as defined in RFC 8414.  Its value **must** '
-            'be a URL that uses the `https` scheme without any '
-            'query or fragment components.'
-        )
-    ),
-    error: str | None = fastapi.Query(
-        default=None,
-        title="Error code",
-        description=(
-            "The error code returned by the authorization server if "
-            "the user cancelled the request, refused consent, or "
-            "failed to authenticate."
-        )
-    )
-) -> TokenResponse:
-    if error:
-        return None # type: ignore
-    if code is None:
-        raise FatalAuthorizationException(
-            "The 'code' parameter is missing from the downstream "
-            "response."
+from cbra.core.ioc import override
+from cbra.types import IDependant
+from .jarmauthorizeresponse import JARMAuthorizeResponse
+from .queryauthorizeresponse import QueryAuthorizeResponse
+from .responsevalidationfailure import ResponseValidationFailure
+from .unsupportedauthorizationresponse import UnsupportedAuthorizationResponse
+
+
+__all__: list[str] = ['RedirectParameters']
+T = TypeVar('T', bound='_RedirectParameters')
+
+
+class _RedirectParameters(IDependant, pydantic.BaseModel):
+
+    @classmethod
+    def fromrequest(
+        cls: type[T],
+        code: str | None = fastapi.Query(
+            default=None,
+            title='Authorization code',
+            description=(
+                'The authorization code generated by the authorization server. '
+                'Required if using the Authorization Code Flow and the response '
+                'mode is `query`, otherwise this parameter is ignored.'
+            )
+        ),
+        state: str | None = fastapi.Query(
+            default=None,
+            title='State',
+            description=(
+                'An opaque value used by the client to maintain state '
+                'between the request and callback. The authorization '
+                'server includes this value when redirecting the '
+                'user-agent back to the client. If supplied, this '
+                'parameter **must** equal the `state` parameter used when '
+                'creating the authorization request. The `state` parameter '
+                'is ignored when using JARM because it is included in the '
+                'JSON Web Token supplied using the `jwt` parameter per '
+                'chosen response mode.'
+            )
+        ),
+        iss: str | None = fastapi.Query(
+            default=None,
+            title='Issuer',
+            description=(
+                'Identifies the authorization server that redirected to '
+                'this endpoint, as defined in RFC 9207. If the client supports '
+                'OAuth 2.0 Authorization Server Issuer Identification, then '
+                'this parameter is **required**, if the response mode is not '
+                'JWT Secured Authorization Response Mode (JARM) per RFC 9101.\n\n'
+                'The `iss` parameter value is the issuer identifier of '
+                'the authorization server that created the authorization '
+                'response, as defined in RFC 8414.  Its value **must** '
+                'be a URL that uses the `https` scheme without any '
+                'query or fragment components.'
+            )
         )
-    return await state.obtain(
-        provider=provider,
-        code=code,
-        url=f'{request.url.scheme}://{request.url.netloc}{request.url.path}',
-        iss=iss
-    )
+    ) -> T:
+        raise NotImplementedError
+
+    @classmethod
+    def __inject__(cls: type[T]) -> Callable[..., Awaitable[T] | T]:
+        return cls.fromrequest
+
+
+class RedirectParameters(_RedirectParameters):
+    __root__: Union[
+        QueryAuthorizeResponse,
+        JARMAuthorizeResponse,
+        UnsupportedAuthorizationResponse
+    ]
+
+    @classmethod
+    @override(_RedirectParameters.fromrequest) # type: ignore
+    def fromrequest(cls: type[T], **kwargs: Any) -> T: # type: ignore
+        return cls.parse_obj(kwargs)
 
-DownstreamTokenResponse: TokenResponse = fastapi.Depends(get)
+    async def obtain(
+        self,
+        client: oauth2.Client,
+        **kwargs: Any
+    ) -> oauth2.TokenResponse:
+        return await self.__root__.obtain(client, **kwargs)
+    
+    def result(self) -> QueryAuthorizeResponse | JARMAuthorizeResponse:
+        if isinstance(self.__root__, UnsupportedAuthorizationResponse):
+            raise ResponseValidationFailure("Invalid response parameters.")
+        return self.__root__
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/params/localclientprovider.py` & `cbra-3.0.0a7/examples/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import fastapi
+import uvicorn
 
-from cbra.core.conf import settings
-from ..types import OIDCProvider
+import cbra.core as cbra
+from cbra.core.sessions import RequestSession
 
 
-class ClientProvider:
-    clients: dict[str, OIDCProvider] = {}
+app: cbra.Application = cbra.Application()
 
-    def __init__(self):
-        for client in settings.OAUTH2_CLIENTS:
-            provider = OIDCProvider.parse_obj({**client, 'protocol': 'oidc'})
-            self.clients[provider.name] = provider
 
-    async def get(self, client_id: str) -> OIDCProvider | None:
-        return self.clients.get(client_id)
+@app.get('/')
+async def f(
+    request: fastapi.Request,
+    response: fastapi.Response,
+    session: RequestSession = fastapi.Depends()
+):
+    await session
+    session.set('sub', 'foo')
+    await session.add_to_response(response)
+    return session.data.dict()
 
-
-LocalClientProvider: ClientProvider = fastapi.Depends(ClientProvider)
+if __name__ == '__main__':
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/resource/types/__init__.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .scope import Scope
-from .userinfosubject import UserInfoSubject
+from typing import TypeAlias
+from typing import Union
+
+from .authorizationstate import AuthorizationState
+from .sector import Sector
 
 
 __all__: list[str] = [
-    'Scope',
-    'UserInfoSubject'
+    'AuthorizationState',
+    'Sector'
+]
+
+
+AuthorizationServerModel: TypeAlias = Union[
+    AuthorizationState,
+    Sector
 ]
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/resource/types/scope.py` & `cbra-3.0.0a7/examples/picqer-webhook.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,42 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Iterable
+import fastapi
+from headless.ext.picqer import DefaultClient
 
+from cbra.ext import google
+from cbra.ext import picqer
 
-class Scope:
-    """Represents the scope required to access an endpoint or resource."""
-    __module__: str = 'cbra.ext.oauth2.resource.types'
-    requires: set[str]
-
-    def __init__(self, scope: str | Iterable[str]):
-        if isinstance(scope, str):
-            scope = [scope]
-        self.requires = set(scope)
-
-    def missing(self, granted: set[str]) -> set[str]:
-        """Return the set containing the scope that is missing."""
-        return self.requires - granted
+
+
+class PicqerWebhookEndpoint(picqer.PicqerWebhookEndpoint):
+
+    async def on_picklists_created(self, event: picqer.v1.PicklistEvent):
+        return fastapi.Response(content=event.json(indent=2))
+
+
+app = google.Service(docs_url='/ui')
+app.add(PicqerWebhookEndpoint, path='/ext/picqer.com/v1/.webhooks')
+
+
+@app.post('/ext/picqer.com/v1/.webhooks/install')
+async def f(request: fastapi.Request):
+    async with DefaultClient() as client:
+        await PicqerWebhookEndpoint.install(
+            client,
+            callback_url=request.url_for('picqer.webhooks'),
+            generate_name=lambda x: (
+                f"{str.join('.', reversed(str.split(x, '.')))}"
+                f".picqer.{request.url.netloc}"
+            ),
+            secret='test'
+        )
+
+
+if __name__ == '__main__':
+    import uvicorn
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/resource/types/userinfosubject.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/responsevalidationfailure.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,31 +2,21 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
+import fastapi
 
-from headless.ext.oauth2.models import ClaimSet
+from cbra.types import Abortable
 
-from cbra.types import ISubject
 
+class ResponseValidationFailure(Abortable):
+    status_code: int = 403
+    reason: str
 
-class UserInfoSubject(ISubject):
-    """Describes a :term:`Resource Owner` of which the claims were
-    received from the OpenID Connect UserInfo endpoint.
-    """
-    __module__: str = 'cbra.ext.oauth2.resource.types'
-    claims: ClaimSet
+    def __init__(self, reason: str):
+        self.reason = reason
 
-    def __init__(self, claims: dict[str, Any] | ClaimSet):
-        if isinstance(claims, dict):
-            claims = ClaimSet.parse_obj(claims)
-        self.claims = claims
-
-    def is_authenticated(self) -> bool:
-        return True
-
-    def get_display_name(self) -> str:
-        raise NotImplementedError
+    async def as_response(self) -> fastapi.Response:
+        return fastapi.responses.PlainTextResponse(content=self.reason)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/authorizationlifecycle.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationlifecycle.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/basescope.py` & `cbra-3.0.0a7/cbra/types/isubjectresolver.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
+from .idependant import IDependant
+from .irequestprincipal import IRequestPrincipal
+from .isubject import ISubject
 
-import pydantic
 
-from cbra.core.iam.models import Subject
-from .iauthorizationrequest import IAuthorizationRequest
-from .iresourceowner import IResourceOwner
+class ISubjectResolver(IDependant):
+    """Resolves an :class:`IRequestPrincipal` to a :class:`ISubject`
+    implementation.
+    """
+    __module__: str = 'cbra.types'
 
-
-class BaseScope(pydantic.BaseModel):
-    name: str
-
-    def apply(
-        self,
-        subject: Subject,
-        owner: IResourceOwner,
-        claims: dict[str, Any],
-        request: IAuthorizationRequest | None = None
-    ) -> None:
-        raise NotImplementedError
-
-    def requires_consent(self) -> bool:
-        return True
+    async def resolve(self, principal: IRequestPrincipal) -> ISubject:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/emailscope.py` & `cbra-3.0.0a7/examples/fastapi-authentication.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
-from typing import Literal
+import fastapi
+import uvicorn
 
-from cbra.core.iam.models import Subject
-from .basescope import BaseScope
-from .iauthorizationrequest import IAuthorizationRequest
-from .iresourceowner import IResourceOwner
-
-
-class EmailScope(BaseScope):
-    name: Literal['email']
-
-    def apply(
-        self,
-        subject: Subject,
-        owner: IResourceOwner,
-        claims: dict[str, Any],
-        request: IAuthorizationRequest | None = None
-    ) -> None:
-        if request is not None:
-            claims['email'] = request.email
-            claims['email_verified'] = request.email_verified
+import cbra.core as cbra
+from cbra.core.iam import AuthorizationContextFactory
+from cbra.types import Principal
+
+
+app: cbra.Application = cbra.Application()
+
+
+@app.get('/')
+async def f(
+    request: fastapi.Request,
+    factory: AuthorizationContextFactory = fastapi.Depends(),
+    principal: Principal = fastapi.Depends(Principal.fromrequest)
+):
+    ctx = await factory.authenticate(request, principal)
+    return {
+        'remote_host': ctx.remote_host,
+        'is_authenticated': ctx.is_authenticated()
+    }
+
+
+if __name__ == '__main__':
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/iauthorizationserverstorage.py` & `cbra-3.0.0a7/cbra/types/pathparameter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
-from typing import Protocol
-from typing import TypeVar
+from typing import Callable
+from typing import Generator
 
-from cbra.core.iam.types import Subject
-from .objectidentifier import ObjectIdentifier
 
-
-M = TypeVar('M')
-
-
-class IAuthorizationServerStorage(Protocol):
-    __module__: str = 'cbra.ext.oauth2.types'
-
-    async def destroy(self, obj: Any) -> None: ...
-    async def get_subject(self, *args: Any, **kwargs: Any) -> Subject | None: ...
-    async def fetch(
-        self,
-        oid: ObjectIdentifier[M]
-    ) -> M | None: ...
-
-    async def get(
-        self,
-        cls: type[M],
-        *args: Any,
-        **kwargs: Any
-    ) -> M | None:
-        raise NotImplementedError
-
-    async def persist(
-        self,
-        obj: Any
+class PathParameter:
+    __module__: str = 'cbra.types'
+    format: str | None = None
+    type: str
+
+    @classmethod
+    def __modify_schema__(
+        cls,
+        field_schema: dict[str, Any]
     ) -> None:
-        ...
+        field_schema.update( # pragma: no cover
+            type=cls.type,
+            format=cls.format
+        )
+
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable[..., str | None], None, None]:
+        yield cls.validate
+
+    @classmethod
+    def clean(cls, v: Any) -> Any:
+        return v
+
+    @classmethod
+    def validate(cls, v: Any) -> str:
+        # Called by FastAPI, must simply return the value.
+        return v
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/imanagedgrant.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhooksignature.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,38 +2,53 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
-from typing import Protocol
+import base64
+import binascii
 
-from headless.ext import oauth2
-from headless.types import IClient
+import fastapi
 
-from .iaccesstoken import IAccessToken
-from .ifrontendstorage import IFrontendStorage
+from cbra.types import IDependant
+from cbra.types import Verifier
 
 
-class IManagedGrant(Protocol):
-    __module__: str = 'cbra.ext.oauth2.types'
+class WebhookSignature(IDependant):
+    __module__: str = 'cbra.ext.picqer'
+    request: fastapi.Request
+    digest: bytes | None = None
 
-    def has_access_token(self, resource: str) -> bool: ...
-    async def get_resource_client(
+    def __init__(
         self,
-        storage: IFrontendStorage,
-        client: oauth2.Client,
-        resource: str,
-        scope: set[str] | None = None
-    ) -> IClient[Any, Any]:
-        ...
+        request: fastapi.Request,
+        digest: str | None = fastapi.Header(
+            default=None,
+            alias='X-Picqer-Signature',
+            title='Signature',
+            description=(
+                'A Base64-encoded SHA256 hash of the request body that was '
+                'created using a shared secret.'
+            )
+        )
+    ) -> None:
+        self.request = request
+        self.signature = None
+        if digest:
+            try:
+                self.signature = base64.urlsafe_b64decode(str.encode(digest))
+            except (binascii.Error, TypeError, ValueError):
+                pass
 
-    async def refresh(
+    async def verify(
         self,
-        storage: IFrontendStorage,
-        client: oauth2.Client,
-        resource: str | None = None,
-        scope: set[str] | None = None
-    ) -> IAccessToken:
-        ...
+        verifier: Verifier
+    ) -> bool:
+        body = await self.request.body()
+        if self.signature is None or not body:
+            return False
+        return await verifier.verify(self.signature, body)
+
+    def __bool__(self) -> bool:
+        return bool(self.signature)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/invalidrequest.py` & `cbra-3.0.0a7/cbra/core/messagepublisher.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .fatalclientexception import FatalClientException
+import aorta
 
+from .ioc import inject
 
-class InvalidRequest(FatalClientException):
-    __module__: str = 'cbra.ext.oauth2.types'
 
-    def __init__(self, message: str | None = None):
-        super().__init__(
-            code='invalid_request',
-            message=message or (
-                'The request is missing a required parameter '
-                'includes an invalid parameter value, includes a parameter more '
-                'than once, or is otherwise malformed.'
-            )
-        )
+class MessagePublisher(aorta.MessagePublisher):
+    __module__: str = 'cbra.core'
+
+    def __init__(
+        self,
+        transport: aorta.types.ITransport = inject('MessageTransport')
+    ):
+        super().__init__(transport=transport)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/invalidscope.py` & `cbra-3.0.0a7/cbra/types/irequestprincipalintrospecter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from .tokenendpointexception import TokenEndpointException
+from typing import Any
 
 
-class InvalidScope(TokenEndpointException):
-    error: str = 'invalid_scope'
-    message: str = "The requested scope is invalid, unknown, or malformed."
+class IRequestPrincipalIntrospecter:
+    """Knows how to obtain details about a specific :class:`IRequestPrincipal`
+    implementation.
+    """
+    __module__: str
+
+    async def introspect(self, principal: Any) -> Any:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/jarmauthorizeresponse.py` & `cbra-3.0.0a7/cbra/types/isubject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,36 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
-import pydantic
-from headless.ext import oauth2
+from canonical import EmailAddress
 
+from .icredentialverifier import ICredentialVerifier
 
-class JARMAuthorizeResponse(pydantic.BaseModel):
-    jwt: str
 
-    async def obtain(
+class ISubject:
+    """Represents an identfied subject, its principal and its
+    credential.
+    """
+    __module__: str = 'cbra.types'
+    email: EmailAddress | None
+    sub: Any
+
+    def is_authenticated(self) -> bool:
+        raise NotImplementedError
+
+    async def authenticate(
         self,
-        client: oauth2.Client,
-        **kwargs: Any
-    ) -> oauth2.TokenResponse:
+        verifier: ICredentialVerifier[Any],
+        providers: set[str] | None = None
+    ) -> None:
+        """Authenticate the subject."""
+        raise NotImplementedError
+
+    def has_claim(self, name: str, value: Any) -> bool:
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/objectidentifier.py` & `cbra-3.0.0a7/examples/google-cloud-platform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Generic
-from typing import TypeVar
+from cbra.ext import google
 
-from canonical import StringType
 
-T = TypeVar('T')
+app: google.Service = google.Service()
 
 
-class ObjectIdentifier(StringType, Generic[T]):
-    pass
+if __name__ == '__main__':
+    import uvicorn
+    uvicorn.run('__main__:app', reload=True)
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/oidcprovider.py` & `cbra-3.0.0a7/cbra/core/sessions/requestsession.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,89 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
-from typing import Literal
+import fastapi
+import logging
 
-import pydantic
-from canonical import EmailAddress
-from canonical import DomainName
-from headless.ext import oauth2
-from headless.ext.oauth2 import OIDCToken
-from headless.ext.oauth2.models import AuthorizationEndpointResponse
-from headless.ext.oauth2.models import TokenResponse
-
-from .clientsecret import ClientSecret
-
-
-class OIDCProvider(pydantic.BaseModel):
-    """A downstream OpenID Connect provider."""
-    allowed_email_domains: set[DomainName] = set()
-    contacts: list[str] = []
-    credential: ClientSecret
-    name: str
-    issuer: str
-    params: dict[str, Any] = {}
-    protocol: Literal['oidc']
-    scope: set[str] = set()
-    _client: oauth2.Client | None = pydantic.PrivateAttr(None)
-
-    @property
-    def client_id(self) -> str:
-        return self.credential.client_id
-
-    @property
-    def client(self) -> oauth2.Client:
-        assert self._client is not None
-        return self._client
+from cbra.core.conf import settings
+from cbra.types import IDeferred
+from cbra.types import IDependant
+from cbra.types import ISessionFactory
+from cbra.types import ISessionManager
+from cbra.types import Session
+from ..params import ApplicationSecretKey
+from ..secretkey import SecretKey
+
+
+class RequestSession(IDeferred, IDependant, ISessionFactory[Session], ISessionManager[Session]):
+    __module__: str = 'cbra.core.session'
+    cookie_name: str
+    data: Session
+    key: SecretKey
+    logger: logging.Logger = logging.getLogger('uvicorn')
+    request: fastapi.Request
 
-    async def get_redirect_uri(
+    def __init__(
         self,
-        redirect_uri: str,
-        state: str,
-        nonce: str
-    ) -> str:
-        assert self._client is not None
-        return await self._client.authorize(
-            state=state,
-            redirect_uri=redirect_uri,
-            scope=self.scope,
-            nonce=nonce,
-            prompt='select_account'
+        request: fastapi.Request,
+        key: SecretKey = ApplicationSecretKey
+    ) -> None:
+        self.cookie_name = settings.SESSION_COOKIE_NAME
+        self.key = key
+        self.request = request
+        self.data = IDeferred.defer(self, 'data')
+
+    async def add_to_response(self, response: fastapi.Response) -> None:
+        await self.data.sign(self.key.sign)
+        if settings.SESSION_COOKIE_SAMESITE is False:
+            samesite = None
+        else:
+            samesite = settings.SESSION_COOKIE_SAMESITE
+        assert samesite is None or isinstance(samesite, str) # nosec
+        response.set_cookie(
+            key=settings.SESSION_COOKIE_NAME,
+            value=self.data.as_cookie(),
+            domain=settings.SESSION_COOKIE_DOMAIN,
+            max_age=settings.SESSION_COOKIE_AGE,
+            httponly=settings.SESSION_COOKIE_HTTPONLY,
+            secure=settings.SESSION_COOKIE_SECURE,
+            path=settings.SESSION_COOKIE_PATH,
+            samesite=samesite # type: ignore
         )
-    
-    def is_trusted_email(self, email: EmailAddress) -> bool:
-        return email.domain in self.allowed_email_domains
-    
-    async def obtain(self, code: str, state: str, redirect_uri: str):
-        assert self._client is not None
-        response = AuthorizationEndpointResponse.parse_obj({
-            'code': code,
-            'state': state
-        })
-        return await self._client.token(
-            response.__root__,
-            redirect_uri=redirect_uri
-        )
-    
-    async def verify(
-        self,
-        response: TokenResponse,
-        nonce: str | None = None
-    ) -> tuple[TokenResponse, OIDCToken | None]:
-        assert self._client is not None
-        return await self._client.verify_response(response, nonce=nonce)
-
-    async def __aenter__(self):
-        self._client = oauth2.Client(
-            issuer=self.issuer,
-            client_id=self.credential.client_id,
-            client_secret=await self.credential.get_secret(),
-            params=self.params
-        )
-        await self._client.__aenter__()
-        return self
 
-    async def __aexit__(self, *args: Any, **kwargs: Any):
-        assert self._client is not None
-        return await self._client.__aexit__(*args, **kwargs)
+    async def clear(self) -> None:
+        self.data = await self.create()
+
+    async def create(self) -> Session:
+        self.dirty = True
+        return Session.new()
+
+    async def initialize(self) -> None:
+        if settings.SESSION_COOKIE_NAME not in self.request.cookies:
+            self.data = await self.create()
+        else:
+            data = Session.parse_cookie(
+                self.request.cookies[settings.SESSION_COOKIE_NAME]
+            )
+            if data is None:
+                self.logger.critical(
+                    'Session cookie was present but could not be deserialized.'
+                )
+                self.data = await self.create()
+                await self.data.sign(self.key.sign)
+            else:
+                self.data = data
+                self.logger.debug(
+                    'Request included a session (id: %s, hmac: %s)',
+                    self.data.id, self.data.hmac
+                )
+            if not await self.data.verify(self.key.verify):
+                self.logger.critical(
+                    'Session cookie was present but the signature did not '
+                    'validate.'
+                )
+                self.data = await self.create()
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/openidscope.py` & `cbra-3.0.0a7/cbra/types/iauthorizationcontextfactory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
-from typing import Literal
+from typing import Awaitable
 
-from cbra.core.iam.models import Subject
-from .basescope import BaseScope
-from .iauthorizationrequest import IAuthorizationRequest
-from .iresourceowner import IResourceOwner
+import fastapi
 
+from .iauthorizationcontext import IAuthorizationContext
+from .irequestprincipal import IRequestPrincipal
 
-class OIDCScope(BaseScope):
-    name: Literal['openid']
 
-    def apply(
+class IAuthorizationContextFactory:
+    """Setup an authorization context for a request."""
+    __module__: str = 'cbra.types'
+
+    async def authenticate(
         self,
-        subject: Subject,
-        owner: IResourceOwner,
-        claims: dict[str, Any],
-        request: IAuthorizationRequest | None = None
-    ) -> None:
-        pass
+        request: fastapi.Request,
+        principal: IRequestPrincipal,
+        providers: set[str] | None = None,
+        subjects: set[str] | Awaitable[set[str]] | None  = None,
+        claims: dict[str, Any] | None = None
+    ) -> IAuthorizationContext:
+        raise NotImplementedError
 
-    def requires_consent(self) -> bool:
-        return False
+    def validate_audience(self, principal: IRequestPrincipal, allow: set[str]) -> None:
+        raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/redirecturi.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/redirecturi.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "urn:ietf:wg:oauth:2.0:oob",
     "urn:ietf:wg:oauth:2.0:oob:auto"
 }
 
 
 class RedirectURI(str):
     __module__: str = 'cbra.ext.oauth2.types'
+    value: urllib.parse.ParseResult
     params: dict[str, str]
 
     @classmethod
     def __modify_schema__(
         cls,
         field_schema: dict[str, Any]
     ) -> None:
@@ -73,20 +74,17 @@
 
             if p.hostname == 'localhost':
                 # Clients should use loopback IP literals rather than the
                 # string localhost as described in Section 8.4.2.
                 # (OAuth 2.1 draft).
                 raise ValueError('local redirect URIs must use loopback IP literals.')
 
-        return cls(urllib.parse.urlunparse(p))
+        return cls(p)
 
-    def redirect(self, allow_params: bool = False, **params: Any) -> str:
+    def redirect(self, **params: str) -> str:
         """Create a redirect URI with the given params."""
-        p: list[str] = list(urllib.parse.urlparse(self)) # type: ignore
-        params = {k: v for k, v in params.items() if v is not None}
-        if allow_params:
-            params.update(urllib.parse.parse_qsl(p[4]))
+        p = list(urllib.parse.urlparse(self))
         p[4] = urllib.parse.urlencode(params, quote_via=urllib.parse.quote)
         return urllib.parse.urlunparse(p)
 
     def __repr__(self) -> str: # pragma: no cover
         return f'RedirectURI({self})'
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/requestedscope.py` & `cbra-3.0.0a7/cbra/types/sessionrequestprincipal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+import base64
 from typing import Any
-from typing import Union
+from typing import TypeVar
 
+import fastapi
 import pydantic
+from ckms.utils import b64decode
 
-from cbra.core.iam.models import Subject
-from .emailscope import EmailScope
-from .genericscope import GenericScope
-from .iauthorizationrequest import IAuthorizationRequest
-from .iresourceowner import IResourceOwner
-from .openidscope import OIDCScope
-from .profilescope import ProfileScope
-from .subscope import SubScope
-from .useragentfingerprintscope import UserAgentFingerprint
-
-
-class RequestedScope(pydantic.BaseModel):
-    __root__: Union[
-        EmailScope,
-        OIDCScope,
-        ProfileScope,
-        SubScope,
-        UserAgentFingerprint,
-        GenericScope # IMPORTANT: this needs to be last
-    ]
+from .hmacsignature import HMACSignature
+from .icredential import ICredential
+from .irequestprincipal import IRequestPrincipal
+from .sessionclaims import SessionClaims
+from .sessionmodel import SessionModel
+from .subjectidentifier import SubjectIdentifier
+
+
+P = TypeVar('P', bound='IRequestPrincipal')
+
+
+class SessionRequestPrincipal(IRequestPrincipal, ICredential, SessionModel):
+    claims: SessionClaims
 
     @property
-    def name(self) -> str:
-        return self.__root__.name
+    def subject(self) -> SubjectIdentifier | None:
+        if not self.claims.iss or not self.claims.sub:
+            return None
+        return SubjectIdentifier(
+            iss=self.claims.iss,
+            sub=self.claims.sub
+        )
 
     @pydantic.root_validator(pre=True)
-    def preprocess(cls, values: dict[str, Any]) -> dict[str, Any]:
-        root: dict[str, Any] | str | None = values.get('__root__')
-        if isinstance(root, str):
-            values['__root__'] = root = {'name': root}
+    def preprocess(
+        cls,
+        values: dict[str, fastapi.Request]
+    ) -> dict[str, Any]:
+        if 'request' in values:
+            # TODO: This is ugly but we will figure that out later.
+            from cbra.core.conf import settings
+
+            cookie = values['request'].cookies.get(settings.SESSION_COOKIE_NAME)
+            if cookie is None:
+                raise ValueError('session not provided.')
+            try:
+                data = base64.urlsafe_b64decode(str.encode(cookie, 'ascii'))
+            except (ValueError, TypeError):
+                raise
+            values = cls.parse_raw(data).dict()
         return values
 
-    def apply(
-        self,
-        subject: Subject,
-        owner: IResourceOwner,
-        claims: dict[str, Any],
-        request: IAuthorizationRequest | None = None
-    ) -> None:
-        return self.__root__.apply(
-            subject=subject,
-            owner=owner,
-            claims=claims,
-            request=request
-        )
-    
-    def requires_consent(self) -> bool:
-        return self.__root__.requires_consent()
-    
-    def __str__(self) -> str:
-        return self.name
+    def has_audience(self) -> bool:
+        return False
+
+    def get_credential(self) -> ICredential | None:
+        if self.hmac is not None:
+            return HMACSignature(b64decode(self.hmac), self.digest())
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/resourceowneridentifier.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/purchaseorderevent.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import dataclasses
+from typing import Literal
 
+from headless.ext.picqer.v1 import PurchaseOrder
 
-@dataclasses.dataclass
-class ResourceOwnerIdentifier:
-    client_id: str
-    sub: int
+from .event import Event
 
-    def __hash__(self) -> int:
-        return hash((self.client_id, self.sub))
+
+class PurchaseOrderEvent(Event):
+    event: Literal[
+        "purchase_orders.created",
+        "purchase_orders.changed",
+        "purchase_orders.closed",
+        "purchase_orders.purchased",
+    ]
+
+    data: PurchaseOrder
```

### Comparing `cbra-2.0.0a91/cbra/ext/oauth2/types/responsemodenotsupported.py` & `cbra-3.0.0a7/cbra/ext/google/impl/oauth2/storage.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import fastapi
+from cbra.ext.google import DatastoreRepository
+from cbra.ext.oauth2 import BaseStorage
+from cbra.ext.oauth2.models import AuthorizationState
+from cbra.types import PersistedModel
 
-from cbra.types import Abortable
 
+class Storage(BaseStorage, DatastoreRepository):
+    __module__: str = 'cbra.ext.google.impl.oauth2'
 
-class ResponseModeNotSupported(Abortable):
-    __module__: str = 'cbra.ext.oauth2.types'
-    status_code: int = 400
+    async def destroy(self, obj: PersistedModel) -> None:
+        return await self.delete(self.model_key(obj))
 
-    def __init__(self, mode: str):
-        self.mode = mode
+    async def get_state(self, key: str) -> AuthorizationState | None:
+        return await self.get_model_by_key(AuthorizationState, key)
 
-    async def as_response(self) -> fastapi.Response:
-        return fastapi.responses.PlainTextResponse(
-            content=f'Response mode {self.mode} is not supported by this server.'
-        )
+    async def persist_state(self, obj: AuthorizationState) -> None:
+        await self.put(obj)
```

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/__init__.py` & `cbra-3.0.0a7/cbra/ext/picqer/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/picqerwebhookendpoint.py` & `cbra-3.0.0a7/cbra/ext/picqer/picqerwebhookendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/v1/event.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/event.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/v1/orderevent.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/orderevent.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/v1/picklistevent.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/picklistevent.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/v1/productevent.py` & `cbra-3.0.0a7/cbra/types/integerpathparameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Literal
+from typing import Any
 
-from headless.ext.picqer.v1 import Product
+from .pathparameter import PathParameter
+from .notfound import NotFound
 
-from .event import Event
 
+class IntegerPathParameter(PathParameter):
+    __module__: str = 'cbra.types'
+    type: str = 'integer'
 
-class ProductEvent(Event):
-    event: Literal[
-        "products.changed",
-        "products.free_stock_changed",
-        "products.stock_changed",
-        "products.assembled_stock_changed"
-    ]
-
-    data: Product
+    @classmethod
+    def clean(cls, v: Any) -> int:
+        try:
+            return int(v)
+        except (TypeError, ValueError):
+            raise NotFound
```

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/webhookresponse.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhookresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/webhooksecret.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhooksecret.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/ext/picqer/webhooksignature.py` & `cbra-3.0.0a7/cbra/types/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,75 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import base64
-import binascii
-
-import fastapi
-
-from cbra.types import IDependant
-from cbra.types import Verifier
-
+import secrets
+from datetime import datetime
+from datetime import timezone
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import TypeVar
+
+from .isessiondata import ISessionData
+from .sessionclaims import SessionClaims
+from .sessionmodel import SessionModel
+
+
+T = TypeVar('T', bound='Session')
+
+
+class Session(SessionModel, ISessionData[SessionClaims]): # type: ignore
+
+    @classmethod
+    def new(cls: type[T]) -> T:
+        now = datetime.now(timezone.utc)
+        return cls(
+            id=secrets.token_urlsafe(48),
+            iat=int(now.timestamp())
+        )
 
-class WebhookSignature(IDependant):
-    __module__: str = 'cbra.ext.picqer'
-    request: fastapi.Request
-    digest: bytes | None = None
+    def as_cookie(self) -> str:
+        assert self.hmac is not None
+        v = base64.urlsafe_b64encode(str.encode(self.json(), encoding='utf-8'))
+        return bytes.decode(v, 'ascii')
+
+    def set(self, key: str, value: Any) -> bool:
+        if self.claims is None:
+            self.claims = SessionClaims()
+        if key not in self.claims.__fields__:
+            raise AttributeError(f'Claim not supported: {key}')
+        modified = False
+        if getattr(self.claims, key) != value:
+            modified = True
+            self.hmac = None
+            setattr(self.claims, key, value)
+        return modified
+
+    def update(self, claims: dict[str, Any] | SessionClaims) -> None:
+        if isinstance(claims, dict):
+            claims = SessionClaims.parse_obj(claims)
+        if self.claims is None:
+            self.claims = SessionClaims()
+        self.claims = SessionClaims.parse_obj({
+            **self.claims.dict(),
+            **claims.dict()
+        })
+        self.hmac = None
 
-    def __init__(
+    async def sign(
         self,
-        request: fastapi.Request,
-        digest: str | None = fastapi.Header(
-            default=None,
-            alias='X-Picqer-Signature',
-            title='Signature',
-            description=(
-                'A Base64-encoded SHA256 hash of the request body that was '
-                'created using a shared secret.'
-            )
-        )
+        sign: Callable[[bytes], Awaitable[str]]
     ) -> None:
-        self.request = request
-        self.signature = None
-        if digest:
-            try:
-                self.signature = base64.urlsafe_b64decode(str.encode(digest))
-            except (binascii.Error, TypeError, ValueError):
-                pass
+        self.hmac = await sign(self.digest())
 
     async def verify(
         self,
-        verifier: Verifier
+        verify: Callable[[bytes | str, bytes], Awaitable[bool]]
     ) -> bool:
-        body = await self.request.body()
-        if self.signature is None or not body:
-            return False
-        return await verifier.verify(self.signature, body)
-
-    def __bool__(self) -> bool:
-        return bool(self.signature)
+        assert self.hmac is not None
+        return await verify(self.hmac, self.digest())
```

### Comparing `cbra-2.0.0a91/cbra/ext/webhooks/types/iwebhookenvelope.py` & `cbra-3.0.0a7/cbra/types/hmacsignature.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from typing import Any
-from typing import Protocol
+from .icredential import ICredential
+from .verifier import Verifier
 
-import pydantic
-from cbra.types import IVerifier
-from cbra.types import Request
 
+class HMACSignature(ICredential):
+    __module__: str = 'cbra.types'
 
-class IWebhookEnvelope(Protocol):
-    __module__: str = 'cbra.ext.webhooks'
-    event_name: Any
+    def __init__(self, signature: bytes, message: bytes):
+        self.message = message
+        self.signature = signature
 
-    def get_message(self) -> pydantic.BaseModel: ...
-
-    async def verify(
-        self,
-        request: Request,
-        verifier: IVerifier
-    ) -> bool: ...
+    async def verify(self, verifier: Verifier) -> bool:
+        return await verifier.verify(self.signature, self.message)
```

### Comparing `cbra-2.0.0a91/cbra/package.json` & `cbra-3.0.0a7/cbra/package.json`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/__init__.py` & `cbra-3.0.0a7/cbra/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,143 +6,103 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from .abortable import Abortable
 from .basemodel import BaseModel
 from .basemodel import BaseModelMetaclass
 from .conflict import Conflict
-from .etagset import ETagSet
 from .forbidden import Forbidden
 from .hmacsignature import HMACSignature
 from .hints import PolymorphicIterable
 from .iauthorizationcontext import IAuthorizationContext
 from .iauthorizationcontextfactory import IAuthorizationContextFactory
-from .iblob import IBlob
-from .icache import ICache
 from .icredential import ICredential
 from .icredentialverifier import ICredentialVerifier
 from .icursor import ICursor
 from .ideferred import IDeferred
 from .idependant import IDependant
 from .iendpoint import IEndpoint
-from .iemailsender import IEmailSender
 from .ihashable import IHashable
 from .imodelrepository import IModelRepository
 from .integerpathparameter import IntegerPathParameter
-from .ipolymorphiccursor import IPolymorphicCursor
-from .ipolymorphicrepository import IPolymorphicRepository
-from .ipersister import IPersister
-from .iprincipal import IPrincipal
 from .iqueryresult import IQueryResult
 from .iroutable import IRoutable
 from .irequestprincipal import IRequestPrincipal
 from .irequestprincipalintrospecter import IRequestPrincipalIntrospecter
 from .isessionfactory import ISessionFactory
 from .isessionmanager import ISessionManager
-from .istoragebucket import IStorageBucket
 from .isubject import ISubject
 from .isubjectresolver import ISubjectResolver
-from .iverifier import IVerifier
 from .jsonwebtoken import JSONWebToken
 from .jsonwebtokenprincipal import JSONWebTokenPrincipal
-from .modelinspector import ModelInspector
-from .modelmetadata import ModelMetadata
 from .mutablesignature import MutableSignature
-from .nullemailsender import NullEmailSender
 from .nullrequestprincipal import NullRequestPrincipal
 from .nullsubject import NullSubject
 from .nullsubjectesolver import NullSubjectResolver
 from .notauthorized import NotAuthorized
 from .notfound import NotFound
 from .operation import Operation
 from .oidcrequestprincipal import OIDCRequestPrincipal
 from .pathparameter import PathParameter
 from .persistedmodel import PersistedModel
-from .policyprincipal import PolicyPrincipal
-from .request import Request
 from .requestprincipal import RequestPrincipal
 from .rfc9068requestprincipal import RFC9068RequestPrincipal
-from .servicenotavailable import ServiceNotAvailable
 from .session import Session
-from .sessionclaims import SessionClaims
 from .sessionmodel import SessionModel
 from .sessionrequestprincipal import SessionRequestPrincipal
 from .stringpathparameter import StringPathParameter
 from .subjectidentifier import SubjectIdentifier
 from .unauthenticatedauthorizationcontext import UnauthenticatedAuthorizationContext
 from .uuidpathparameter import UUIDPathParameter
 from .verifier import Verifier
-from .versionconflict import VersionConflict
-from .versionedhmac import VersionedMAC
-from .versionedciphertext import VersionedCipherText
 
 
 __all__: list[str] = [
     'Abortable',
     'BaseModel',
     'BaseModelMetaclass',
     'Conflict',
-    'ETagSet',
     'Forbidden',
     'HMACSignature',
-    'IAuthorizationContext',
-    'IAuthorizationContextFactory',
-    'IBlob',
-    'ICache',
     'ICredential',
     'ICredentialVerifier',
     'ICursor',
     'IDependant',
     'IDeferred',
-    'IEmailSender',
+    'IAuthorizationContext',
+    'IAuthorizationContextFactory',
     'IEndpoint',
-    'IHashable',
     'IModelRepository',
     'IntegerPathParameter',
-    'IPersister',
-    'IPolymorphicCursor',
-    'IPolymorphicRepository',
-    'IPrincipal',
+    'IHashable',
     'IRequestPrincipalIntrospecter',
     'IRequestPrincipal',
     'IRoutable',
     'ISessionFactory',
     'ISessionManager',
-    'IStorageBucket',
     'ISubject',
     'ISubjectResolver',
     'IQueryResult',
-    'IVerifier',
     'JSONWebToken',
     'JSONWebTokenPrincipal',
-    'ModelInspector',
-    'ModelMetadata',
     'MutableSignature',
     'NotAuthorized',
     'NotFound',
-    'NullEmailSender',
     'NullRequestPrincipal',
     'NullSubject',
     'NullSubjectResolver',
     'Operation',
     'OIDCRequestPrincipal',
     'PathParameter',
     'PersistedModel',
-    'PolicyPrincipal',
     'PolymorphicIterable',
-    'Request',
     'RequestPrincipal',
     'RFC9068RequestPrincipal',
-    'ServiceNotAvailable',
     'Session',
-    'SessionClaims',
     'SessionModel',
     'SessionRequestPrincipal',
     'SubjectIdentifier',
     'StringPathParameter',
     'UnauthenticatedAuthorizationContext',
     'UUIDPathParameter',
     'Verifier',
-    'VersionConflict',
-    'VersionedCipherText',
-    'VersionedMAC',
 ]
```

### Comparing `cbra-2.0.0a91/cbra/types/basemodel.py` & `cbra-3.0.0a7/cbra/types/basemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,20 @@
         for name, field in fields.items():
             if not field.extra.get('primary_key'):
                 continue
             field.extra['name'] = name
             key_fields.append(field)
         if key_fields:
             new_class.__key__ = ModelIdentity(key_fields)
-
         return new_class # type: ignore
 
 
 class BaseModel(pydantic.BaseModel, metaclass=BaseModelMetaclass):
     __abstract__: bool = True
-    __key__: ModelIdentity | NotImplementedType
+    __key__: ModelIdentity
     __surrogate__: ModelAutoAssignedIdentity | NotImplementedType
     __module__: str = 'cbra.types'
 
     def __eq__(self: T, other: T) -> bool:
         # TODO: Compare subclasses to parents if the key is the
         # same?
         return all([
```

### Comparing `cbra-2.0.0a91/cbra/types/hints.py` & `cbra-3.0.0a7/cbra/types/hints.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/httpheaderprincipal.py` & `cbra-3.0.0a7/cbra/types/httpheaderprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/iauthorizationcontext.py` & `cbra-3.0.0a7/cbra/types/iauthorizationcontext.py`

 * *Files 26% similar despite different names*

```diff
@@ -39,29 +39,19 @@
         """
         raise NotImplementedError
 
     def is_authenticated(self) -> bool:
         """Return a boolean indicating if the request is authenticated."""
         return self.subject.is_authenticated()
 
-    def get_display_name(self) -> str:
-        """Return the display name of the currently authenticated Subject."""
-        return self.subject.get_display_name()
-
     def get_remote_host(self) -> ipaddress.IPv4Address | None:
         raise NotImplementedError
 
     def get_subject(self) -> ISubject:
         raise NotImplementedError
 
-    def has_email(self, email: str) -> bool:
-        """Return a boolean if the given email is verified for the currently
-        authenticated subject.
-        """
-        raise NotImplementedError
-
     def has_permission(self, name: str) -> bool:
         """Return a boolean indicating if the context has the given
         permission. This method should always be invoked after
         :meth:`authorize()`.
         """
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/types/icredential.py` & `cbra-3.0.0a7/cbra/types/jsonwebtoken.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright (C) 2023 Cochise Ruhulessin
+# Copyright (C) 2022 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+from .icredential import ICredential
 
 
-class ICredential:
-    """Used in conjunction with a :class:`IRequestPrincipal` implementation
-    to establish the identity of a subject.
-    """
+class JSONWebToken(ICredential):
+    """An unparsed JSON Web Token."""
     __module__: str = 'cbra.types'
+    token: str
 
-    def is_verified(self) -> bool:
-        """Some credentials are verified simply by existing."""
-        return False
+    def __init__(self, token: str):
+        self.token = token
+
+    def __str__(self) -> str:
+        return self.token
```

### Comparing `cbra-2.0.0a91/cbra/types/icredentialverifier.py` & `cbra-3.0.0a7/cbra/types/nullsubject.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-# Copyright (C) 2022 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# type: ignore
 from typing import Any
-from typing import Generic
-from typing import TypeVar
 
-from .icredential import ICredential
+from .icredentialverifier import ICredentialVerifier
+from .isubject import ISubject
 
 
-P = TypeVar('P')
-
-
-class ICredentialVerifier(Generic[P]):
-    """Knows how to verify a credential attached to a principal."""
+class NullSubject(ISubject):
+    """An :class:`ISubject` implementation that represents an non-authenticated
+    and non-identified subject.
+    """
     __module__: str = 'cbra.types'
+    email: None = None
+    sub: None = None
 
-    async def verify(
+    def is_authenticated(self) -> bool:
+        return False
+
+    async def authenticate(
         self,
-        principal: P,
-        credential: ICredential | None,
+        verifier: ICredentialVerifier[Any],
         providers: set[str] | None = None
-    ) -> bool:
-        raise NotImplementedError
+    ) -> None:
+        return
+
+    def has_claim(self, name: str, value: Any) -> bool:
+        return False
```

### Comparing `cbra-2.0.0a91/cbra/types/ideferred.py` & `cbra-3.0.0a7/cbra/types/ideferred.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/idependant.py` & `cbra-3.0.0a7/cbra/types/idependant.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/iendpoint.py` & `cbra-3.0.0a7/cbra/types/iendpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,58 +5,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import functools
 import logging
 from datetime import datetime
-from datetime import timezone
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Literal
 from typing import TypeVar
 
-import aorta
 import fastapi
 
 from .abortable import Abortable
 from .iauthorizationcontextfactory import IAuthorizationContextFactory
 from .irequestprincipal import IRequestPrincipal
 from .iroutable import IRoutable
 from .isessionmanager import ISessionManager
 from .forbidden import Forbidden
 from .notauthorized import NotAuthorized
-from .request import Request
 
 
 T = TypeVar('T', bound='IEndpoint')
 
 
 class IEndpoint:
     __module__: str = 'cbra.types'
     allowed_http_methods: list[str]
-    autodiscover: bool = True
     context_factory: IAuthorizationContextFactory
-    csrf_protect: bool = False
     handlers: list[IRoutable]
     include_in_schema: bool = True
     name: str | None = None
-    logger: logging.Logger = logging.getLogger('cbra.endpoint')
+    logger: logging.Logger = logging.getLogger('uvicorn')
     response_model_by_alias: bool = False
-    response_model_exclude: set[str] | None = None
-    response_model_exclude_none: bool = False
     session: ISessionManager[Any]
-    timestamp: datetime
-    publisher: aorta.types.IPublisher
     with_options: bool = True
 
-    #: The ``If-Match`` value provided by the current request.
-    etag: set[str] = set()
-
     #: The set of permissions supported by this endpoint. These must be
     #: defined beforehand to limit the number of calls to remote IAM
     #: systems.
     permissions: set[str]
 
     #: The list of subjects that may access this endpoint. Override this
     #: property if an endpoint needs to hardcode the allowed subjects
@@ -65,36 +53,25 @@
     allowed_subjects: set[str] = set()
 
     #: The set of trusted authorization servers. This will override the
     #: :attr:`cbra.core.conf.settings.TRUSTED_AUTHORIZATION_SERVERS`
     #: setting.
     trusted_providers: set[str] = set()
 
-    #: Indicates if this endpoint uses versioning using the ``ETag``
-    #: and friends headers.
-    versioned: bool
-
     principal: IRequestPrincipal
-    request: Request
+    request: fastapi.Request
     response: fastapi.Response
     router: fastapi.APIRouter
 
     #: Indicates if all requests to the endpoint must be authenticated.
     require_authentication: bool = False
     status_code: int = 200
     summary: str | None = None
     tags: list[str] = []
 
-    #: The current messaging transaction.
-    transaction: aorta.Transaction
-
-    #: Indicates that this endpoint is in testing mode and should not catch
-    #: any abortable errors.
-    test: bool = False
-
     @staticmethod
     def require_permission(name: str) -> Callable[..., Any]:
         """Decorate a method on an :class:`~cbra.types.IEndpoint` implementation
         to require the given permission. If the request does not have permission
         `name`, then :class:`~cbra.types.Forbidden` is raised.
         """
         def decorator_factory(
@@ -127,20 +104,18 @@
     async def run_handler(
         self,
         func: Callable[..., Any],
         *args: Any,
         **kwargs: Any
     ):
         try:
-            async with aorta.Transaction(publisher=self.publisher) as tx:
-                self.transaction = tx
-                await self.authenticate()
-                if self.require_authentication and not self.ctx.is_authenticated():
-                    raise NotAuthorized
-                return await func(self, *args, **kwargs)
+            await self.authenticate()
+            if self.require_authentication and not self.ctx.is_authenticated():
+                raise NotAuthorized
+            return await func(self, *args, **kwargs)
         except Abortable as exc:
             return await exc.as_response()
 
     async def authenticate(self) -> None:
         self.ctx = await self.context_factory.authenticate(
             request=self.request,
             principal=self.principal,
@@ -150,23 +125,19 @@
 
     async def is_authorized(self, name: str) -> bool:
         """Return a boolean if the given authorization context has a
         certain permission.
         """
         await self.ctx.authorize()
         return self.has_permission(name)
-    
+
     def has_permission(self, name: str) -> bool:
         """Return a boolean if the request has the given permission."""
         return self.ctx.has_permission(name)
 
-    def is_authenticated(self) -> bool:
-        """Return a boolean indicating if the request is authenticated."""
-        return self.ctx.is_authenticated()
-
     def set_cookie(
         self,
         key: str,
         value: str = "",
         max_age: int | None = None,
         expires: datetime | str| int | None = None,
         path: str = "/",
@@ -184,20 +155,8 @@
             domain=domain,
             secure=secure,
             httponly=httponly,
             samesite=samesite
         )
 
     def delete_cookie(self, key: str, path: str = "/") -> None:
-        return self.set_cookie(
-            key,
-            expires=datetime(1970, 1, 1, tzinfo=timezone.utc),
-            max_age=0,
-            path=path
-        )
-    
-    def publish(
-        self,
-        Message: type[aorta.Command | aorta.Event],
-        **params: Any
-    ) -> None:
-        self.transaction.publish(Message.parse_obj(params))
+        return self.set_cookie(key, expires=0, max_age=0, path=path)
```

### Comparing `cbra-2.0.0a91/cbra/types/ihashable.py` & `cbra-3.0.0a7/cbra/types/ihashable.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/imodelrepository.py` & `cbra-3.0.0a7/cbra/types/imodelrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/irequestprincipal.py` & `cbra-3.0.0a7/cbra/types/irequestprincipal.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,38 +21,28 @@
 
 
 class IRequestPrincipal:
     __module__: str = 'cbra.types'
 
     @classmethod
     def depends(cls: type[P]) -> P:
-        return fastapi.Depends(cls.__inject__())
-
-    @classmethod
-    def __inject__(cls: type[P]) -> Callable[..., Awaitable[P] | P]:
-        """Return a callable that specifies the dependencies of this
-        class in its signature.
-        """
-        return cls.fromrequest
+        return fastapi.Depends(cls.fromrequest)
 
     @classmethod
     async def fromrequest(cls: type[P], request: fastapi.Request) -> P:
         """Create a new principal from the request object."""
-        # TODO: A very ugly hack
-        body = None
-        if 'Content-Type' in request.headers:
-            if hasattr(request, '_body'):
-                body = request._body # type: ignore
-            else:
-                body = await request.body()
         return cls.parse_obj({ # type: ignore
             'request': request,
             'headers': request.headers,
             'cookies': request.cookies,
-            'content': body
+            'content': (
+                await request.body()
+                if 'Content-Type' in request.headers
+                else None
+            )
         })
 
     def get_audience(self) -> set[str]:
         """Return the audience(s) of the principal."""
         raise NotImplementedError
 
     def get_credential(self) -> ICredential | None:
```

### Comparing `cbra-2.0.0a91/cbra/types/isessiondata.py` & `cbra-3.0.0a7/cbra/types/isessiondata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/isessionmanager.py` & `cbra-3.0.0a7/cbra/types/isessionmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,54 +5,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import copy
 from typing import Any
 from typing import Generic
-from typing import Generator
 from typing import TypeVar
 
 import fastapi
 
 from .isessiondata import ISessionData
 from .sessionclaims import SessionClaims
 
 
 M = TypeVar('M', bound=ISessionData[Any])
-T = TypeVar('T', bound='ISessionManager[Any]')
 
 
 class ISessionManager(Generic[M]):
     __module__: str = 'cbra.types'
-    csrf: str
     dirty: bool = False
     data: M
 
     @property
     def claims(self) -> SessionClaims:
         # Ensure that the user does not circumvent the setter.
         return copy.deepcopy(self.data.claims or SessionClaims())
 
     def get(self, key: str) -> Any:
         return self.data.get(key)
 
     def set(self, key: str, value: Any) -> None:
-        self.dirty = True
-        self.data.set(key, value)
+        self.dirty = self.data.set(key, value)
 
     def update(self, claims: dict[str, Any]) -> None:
         self.dirty = True
         self.data.update(claims)
 
     def is_dirty(self) -> bool:
         return self.dirty
 
     async def add_to_response(self, response: fastapi.Response) -> None:
         """Update a response to include the session."""
         raise NotImplementedError
 
     async def clear(self) -> None:
-        raise NotImplementedError
-
-    def __await__(self: T) -> Generator[None, None, T]:
         raise NotImplementedError
```

### Comparing `cbra-2.0.0a91/cbra/types/jsonwebtokenprincipal.py` & `cbra-3.0.0a7/cbra/types/jsonwebtokenprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/modelautoassignedidentity.py` & `cbra-3.0.0a7/cbra/types/modelautoassignedidentity.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 
 class ModelAutoAssignedIdentity:
     """Like :class:`~cbra.types.ModelIdentity`, but for a single field
     that is an auto assigned integer.
     """
     __module__: str = 'cbra.types'
-    field: pydantic.fields.FieldInfo
+    field: pydantic.main.FieldInfo
     attname: str
 
-    def __init__(self, attname: str, field: pydantic.fields.FieldInfo):
+    def __init__(self, attname: str, field: pydantic.main.FieldInfo):
         self.attname = attname
         self.field = field
 
     @overload
     def __get__(
         self: T,
         obj: None,
```

### Comparing `cbra-2.0.0a91/cbra/types/modelidentity.py` & `cbra-3.0.0a7/cbra/types/modelidentity.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import pydantic
 import pydantic.main
 
 
 class ModelIdentity:
     """A set of fields that identify a model instance."""
     __module__: str = 'cbra.types'
-    fields: dict[str, pydantic.fields.FieldInfo]
+    fields: dict[str, pydantic.main.FieldInfo]
 
-    def __init__(self, fields: list[pydantic.fields.FieldInfo]):
+    def __init__(self, fields: list[pydantic.main.FieldInfo]):
         self.fields = collections.OrderedDict()
         for field in fields:
             assert 'name' in field.extra
             self.fields[field.extra['name']] = field
 
     @overload
     def __get__(
```

### Comparing `cbra-2.0.0a91/cbra/types/mutablesignature.py` & `cbra-3.0.0a7/cbra/types/mutablesignature.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/oidcrequestprincipal.py` & `cbra-3.0.0a7/cbra/types/oidcrequestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/operation.py` & `cbra-3.0.0a7/cbra/types/operation.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/requestprincipal.py` & `cbra-3.0.0a7/cbra/types/requestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/rfc9068requestprincipal.py` & `cbra-3.0.0a7/cbra/types/rfc9068requestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/cbra/types/session.py` & `cbra-3.0.0a7/examples/resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,79 +2,68 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import base64
+import datetime
 import secrets
-from datetime import datetime
-from datetime import timezone
-from typing import Any
-from typing import Awaitable
-from typing import Callable
-from typing import TypeVar
 
-from .isessiondata import ISessionData
-from .sessionclaims import SessionClaims
-from .sessionmodel import SessionModel
+import pydantic
+import uvicorn
 
+import cbra.core as cbra
 
-T = TypeVar('T', bound='Session')
 
+class BookPublication(pydantic.BaseModel):
+    published: datetime.date
+    country_code: str
+
+
+class Book(cbra.ResourceModel):
+    id: int | None = cbra.Field(
+        default=None,
+        read_only=True,
+        path_alias='book_id',
+        primary_key=True
+    )
+    title: str
+    publications: list[BookPublication]
+
+
+class BookResource(cbra.Resource, cbra.Create, cbra.Delete, cbra.Retrieve, cbra.Update, model=Book):
+    books: dict[int, Book] = {
+        1: Book(
+            id=1,
+            title="The Hitchhiker's Guide to the Galaxy",
+            publications=[
+                BookPublication(country_code='UK', published=datetime.date(1979, 10, 12)),
+                BookPublication(country_code='US', published=datetime.date(1980, 10, 1)),
+            ]
+        )
+    }
 
-class Session(SessionModel, ISessionData[SessionClaims]): # type: ignore
+    async def can_create(self, resource: Book) -> bool:
+        return not any([x.title == resource.title for x in self.books.values()])
 
-    @classmethod
-    def new(cls: type[T]) -> T:
-        now = datetime.now(timezone.utc)
-        return cls(
-            id=secrets.token_urlsafe(48),
-            iat=int(now.timestamp())
-        )
+    async def delete(self, resource: Book):
+        assert resource.id is not None
+        self.books.pop(resource.id)
+
+    async def get_object(self) -> Book | None:
+        return self.books.get(int(self.request.path_params['book_id']))
+
+    async def persist(self, resource: Book, create: bool = False) -> Book:
+        if create:
+            assert resource.id is None
+            resource.id = secrets.choice(range(1000, 9999))
+        assert resource.id is not None
+        self.books[resource.id] = resource
+        return resource
+
+
+app = cbra.Application(docs_url='/ui')
+BookResource.add_to_router(app, path='/')
 
-    def as_cookie(self) -> str:
-        assert self.hmac is not None
-        v = base64.urlsafe_b64encode(str.encode(self.json(exclude_none=True), encoding='utf-8'))
-        return bytes.decode(v, 'ascii')
-
-    def cycle(self) -> None:
-        self.claims = SessionClaims()
-        self.id = secrets.token_urlsafe(48)
-        self.hmac = None
-
-    def set(self, key: str, value: Any) -> bool:
-        if self.claims is None:
-            self.claims = SessionClaims()
-        if key not in self.claims.__fields__:
-            raise AttributeError(f'Claim not supported: {key}')
-        modified = False
-        if getattr(self.claims, key) != value:
-            modified = True
-            self.hmac = None
-            setattr(self.claims, key, value)
-        return modified
-
-    def update(self, claims: dict[str, Any] | SessionClaims) -> None:
-        if isinstance(claims, dict):
-            claims = SessionClaims.parse_obj(claims)
-        if self.claims is None:
-            self.claims = SessionClaims()
-        self.claims = SessionClaims.parse_obj({
-            **self.claims.dict(),
-            **claims.dict()
-        })
-        self.hmac = None
-
-    async def sign(
-        self,
-        sign: Callable[[bytes], Awaitable[str]]
-    ) -> None:
-        self.hmac = await sign(self.digest())
-
-    async def verify(
-        self,
-        verify: Callable[[bytes | str, bytes], Awaitable[bool]]
-    ) -> bool:
-        assert self.hmac is not None
-        return await verify(self.hmac, self.digest())
+if __name__ == '__main__':
+    uvicorn.run('__main__:app', reload=True) # type: ignore
```

### Comparing `cbra-2.0.0a91/cbra/types/sessionmodel.py` & `cbra-3.0.0a7/cbra/types/sessionmodel.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import base64
-import secrets
-from typing import Any
 from typing import TypeVar
 
 import pydantic
 
 from .ihashable import IHashable
 from .sessionclaims import SessionClaims
 
@@ -20,30 +18,20 @@
 T = TypeVar('T', bound='SessionModel')
 
 
 class SessionModel(pydantic.BaseModel, IHashable):
     id: str
     iat: int
     claims: SessionClaims | None = None
-    csrf: str | None = pydantic.Field(
-        default_factory=lambda: secrets.token_urlsafe(48)
-    )
     hmac: str | None = None
 
     @classmethod
     def parse_cookie(cls: type[T], value: str | None) -> T | None:
         if value is None: return None
         try:
             serialized = base64.urlsafe_b64decode(str.encode(value, 'ascii'))
             return cls.parse_raw(serialized)
         except Exception:
             return None
 
     def digest(self) -> bytes:
-        return self._hash(self.dict(exclude={'hmac'}, exclude_none=True))
-
-    def get(self, key: str) -> Any:
-        if not self.claims:
-            return None
-        if key not in self.claims.__fields__:
-            raise AttributeError(f'No such claim: {key}')
-        return getattr(self.claims, key)
+        return self._hash(self.dict(exclude={'hmac'}, exclude_none=True))
```

### Comparing `cbra-2.0.0a91/cbra.egg-info/PKG-INFO` & `cbra-3.0.0a7/cbra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbra
-Version: 2.0.0a91
+Version: 3.0.0a7
 Summary: A class-based REStful API framework built on FastAPI
 Home-page: https://docs.cochise.io/python/cbra/latest
 Author: Cochise Ruhulessin
 Author-email: cochiseruhulessin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -18,23 +18,18 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: google
 Provides-Extra: gunicorn
-Provides-Extra: sendgrid
 
 
 
 
-# OAuth 2.x
-
-- https://www.rfc-editor.org/rfc/rfc8707.html
-
 # Resources
 
 - https://tyk.io/blog/your-data-model-is-not-an-api/
 - https://shekhargulati.com/2021/10/15/web-api-design-anti-pattern-exposing-your-database-model
 - https://cloud.google.com/blog/products/api-management/why-your-web-apis-should-be-entity-oriented
 - https://cloud.google.com/blog/products/application-development/api-design-why-you-should-use-links-not-keys-to-represent-relationships-in-apis
 - https://tools.ietf.org/html/rfc7807
```

### Comparing `cbra-2.0.0a91/docs/source/_ext/djangodocs.py` & `cbra-3.0.0a7/docs/source/_ext/djangodocs.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/docs/source/conf.py` & `cbra-3.0.0a7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/examples/authentication.py` & `cbra-3.0.0a7/examples/authentication.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/examples/dependency-injection.py` & `cbra-3.0.0a7/examples/dependency-injection.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/examples/google-cloud-platform.py` & `cbra-3.0.0a7/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (C) 2022 Cochise Ruhulessin
+# Copyright (C) 2021-2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-from cbra.ext import google
+import asyncio
 
+import pytest
 
-app: google.Service = google.Service()
 
-
-if __name__ == '__main__':
-    import uvicorn
-    uvicorn.run('__main__:app', reload=True)
+@pytest.fixture(scope="session")
+def event_loop():
+    loop = asyncio.new_event_loop()
+    yield loop
+    loop.close()
```

### Comparing `cbra-2.0.0a91/examples/oauth2-callback-google.py` & `cbra-3.0.0a7/examples/oauth2-callback-google.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/setup.py` & `cbra-3.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/core/iam/models/test_unit_subject.py` & `cbra-3.0.0a7/tests/core/iam/models/test_unit_subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/core/test_unit_response_model_with_aliases.py` & `cbra-3.0.0a7/tests/ext/google/test_integration_aorta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,74 @@
-# Copyright (C) 2021-2023 Cochise Ruhulessin
+# Copyright (C) 2023 Cochise Ruhulessin
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-"""Tests that a model field that is declared as optional is also allowed
-on the response model.
-"""
-import collections
+import base64
+import datetime
 
-import pydantic
+import aorta
 import pytest
 import pytest_asyncio
 from headless.core import httpx
 
 import cbra.core as cbra
+from cbra.ext.google import AortaEndpoint
+from cbra.ext.google import MessagePublished
 
 
-QueryResult = collections.namedtuple('QueryResult', ['token', 'items'])
 
+AortaEndpoint: type[AortaEndpoint] = AortaEndpoint.configure( # type: ignore
+    {'require_authentication': False}
+)
 
-class AliasModel(cbra.ResourceModel):
-    id: int = pydantic.Field(..., primary_key=True)
-    value: str | None = pydantic.Field(..., alias='aliasedValue')
 
+@pytest.fixture
+def app() -> cbra.Application:
+    return cbra.Application()
 
-class AliasedResource(cbra.Resource, cbra.Collection, model=AliasModel):
-    response_model_by_alias: bool = True
 
-    async def retrieve(self, aliasmodel_id: int) -> AliasModel:
-        return AliasModel(id=1, aliasedValue=None)
-
-    async def filter(self, *args):
-        return QueryResult('', [AliasModel(id=1, aliasedValue=None)])
-
-
-@pytest_asyncio.fixture(scope='session') # type: ignore
-async def client():
-    app = cbra.Application()
-    app.add(AliasedResource)
-    async with httpx.Client(base_url='https://cbra', app=app) as client:
+@pytest_asyncio.fixture # type: ignore
+async def client(app: cbra.Application):
+    async with httpx.Client(base_url='http://cbra.ext.google', app=app) as client:
         yield client
 
 
 @pytest.mark.asyncio
-async def test_retrieve_response_model_with_aliases(
-    client: httpx.Client
+async def test_accept_message(
+    app: cbra.Application,
+    client: httpx.Client,
 ):
-    response = await client.get(url='/aliasmodels/1')
-    assert response.status_code == 200, response.content
+    app.add(AortaEndpoint)
 
+    event = GoogleEvent(foo=1)
+    envelope = event.envelope()
+    message = MessagePublished.parse_obj({
+        'subscription': 'projects/myproject/subscriptions/mysub',
+        'message': {
+            'messageId': 1,
+            'publishTime': datetime.datetime.now().isoformat(),
+            'data': base64.b64encode(bytes(envelope))
+        }
+    })
+    response = await client.post(
+        url='/',
+        content=message.json(by_alias=True)
+    )
+    assert response.status_code == 202, response.content
+    raise Exception
+
+class GoogleEvent(aorta.Event):
+    foo: int
+
+
+class GoogleEventListener(aorta.EventListener):
+    dep = cbra.inject('Missing')
+
+    async def handle(self, event: GoogleEvent) -> int:
+        return event.foo
+    
 
-@pytest.mark.asyncio
-async def test_list_response_model_with_aliases(
-    client: httpx.Client
-):
-    response = await client.get(url='/aliasmodels')
-    assert response.status_code == 200, response.content
+aorta.register(GoogleEventListener)
```

### Comparing `cbra-2.0.0a91/tests/ext/google/system/conftest.py` & `cbra-3.0.0a7/tests/ext/google/system/conftest.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/ext/google/system/test_system_googleendpoint.py` & `cbra-3.0.0a7/tests/ext/google/system/test_system_googleendpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 @pytest.mark.asyncio
 async def test_basic_oidc_authentication(
     app: cbra.Application,
     client: httpx.Client,
     google_id_token: str
 ): 
     claims: dict[str, Any] = JSONWebTokenPrincipal.parse_jwt(google_id_token)
-    app.add(GoogleServiceEndpoint.configure({'allowed_service_accounts': {claims['email']}})) # type: ignore
+    app.add(GoogleServiceEndpoint.configure(allowed_service_accounts={claims['email']})) # type: ignore
     response = await client.get(
         url='/',
         headers={'Authorization': f'Bearer {google_id_token}'}
     )
     assert response.status_code == 200
 
 
 @pytest.mark.asyncio
 async def test_basic_oidc_authentication_accepts_only_whitelisted(
     app: cbra.Application,
     client: httpx.Client,
     google_id_token: str
 ): 
-    app.add(GoogleServiceEndpoint.configure({'allowed_service_accounts': set()})) # type: ignore
+    app.add(GoogleServiceEndpoint.configure(allowed_service_accounts=set())) # type: ignore
     response = await client.get(
         url='/',
         headers={'Authorization': f'Bearer {google_id_token}'}
     )
     assert response.status_code == 403
```

### Comparing `cbra-2.0.0a91/tests/ext/oauth2/test_integration_authorization_request_requires_response_type.py` & `cbra-3.0.0a7/tests/test_unit_endpoint_authentication.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,73 +2,52 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import urllib.parse
-
 import pytest
+import pytest_asyncio
 from headless.core import httpx
 
+import cbra.core as cbra
 
-@pytest.mark.parametrize("state", [
-    None,
-    'state'
-])
-@pytest.mark.asyncio
-async def test_missing_response_type_returns_303_error(
-    client: httpx.Client,
-    authorization_endpoint: str,
-    state: str | None,
-    issuer: str
-):
-    params: dict[str, str] = {'client_id': 'app', 'response_type': 'foo'}
-    if state is not None:
-        params['state'] = state
-    response = await client.get(
-        url=authorization_endpoint,
-        params=params
-    )
-    assert response.status_code == 303, response.content
-    assert 'Location' in response.headers
-    p = urllib.parse.urlparse(response.headers['Location'])
-    q = dict(urllib.parse.parse_qsl(p.query))
-    assert 'error' in q
-    assert q['error'] == "invalid_request"
-    assert 'iss' in q
-    assert q['iss'] == issuer
-    if state is not None:
-        assert 'state' in q
-        assert q['state'] == state
-
-
-@pytest.mark.parametrize("state", [
-    None,
-    'state'
+
+class AuthenticationRequiredEndpoint(cbra.Endpoint):
+    require_authentication: bool = True
+    async def head(self): assert False
+    async def get(self): assert False
+    async def put(self): assert False
+    async def post(self): assert False
+    async def patch(self): assert False
+    async def delete(self): assert False
+    async def trace(self): assert False
+
+
+@pytest_asyncio.fixture # type: ignore
+async def client():
+    app = cbra.Application()
+    AuthenticationRequiredEndpoint.add_to_router(app, path='/')
+    async with httpx.Client(base_url='https://cbra', app=app) as client:
+        yield client
+
+
+@pytest.mark.parametrize("method", [
+    "HEAD",
+    "GET",
+    "POST",
+    "PUT",
+    "PATCH",
+    "DELETE",
+    "TRACE"
 ])
 @pytest.mark.asyncio
-async def test_invalid_response_type_returns_303_error(
+async def test_require_authentication(
     client: httpx.Client,
-    authorization_endpoint: str,
-    state: str | None,
-    issuer: str
+    method: str
 ):
-    params: dict[str, str] = {'client_id': 'app', 'response_type': 'foo'}
-    if state is not None:
-        params['state'] = state
-    response = await client.get(
-        url=authorization_endpoint,
-        params=params
+    response = await client.request(
+        method=method,
+        url='/',
     )
-    assert response.status_code == 303, response.content
-    assert 'Location' in response.headers
-    p = urllib.parse.urlparse(response.headers['Location'])
-    q = dict(urllib.parse.parse_qsl(p.query))
-    assert 'error' in q
-    assert 'iss' in q
-    assert q['iss'] == issuer
-    assert q['error'] == "invalid_request"
-    if state is not None:
-        assert 'state' in q
-        assert q['state'] == state
+    assert response.status_code == 401
```

### Comparing `cbra-2.0.0a91/tests/ext/oauth2/test_unit_redirecturi.py` & `cbra-3.0.0a7/tests/ext/oauth2/test_unit_redirecturi.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/ext/picqer/test_unit_signature.py` & `cbra-3.0.0a7/tests/ext/picqer/test_unit_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from headless.core import httpx
 
 import cbra.core as cbra
 from cbra import types
 from cbra.ext.picqer import PicqerWebhookEndpoint
 from cbra.ext.picqer import WebhookSecret
 
-
 VALID_SIGNATURE: str = '3TMYo2hAFdgQ9bF4MJZ4/dnELdJv5ucJPRAEnoE3Qxk='
 
 VALID_BODY: str = (
     '{"idhook":14381,"name":"created.picklists.picqer.localhost:8000","event":'
     '"picklists.created","event_triggered_at":"2023-02-25 04:34:57","data":{"i'
     'dpicklist":81146972,"picklistid":"P2023-1289","idcustomer":40454718,"idor'
     'der":118330126,"idreturn":null,"idwarehouse":6790,"idtemplate":6375,"idsh'
```

### Comparing `cbra-2.0.0a91/tests/test_unit_endpoint.py` & `cbra-3.0.0a7/tests/test_unit_endpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/test_unit_principal.py` & `cbra-3.0.0a7/tests/test_unit_principal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/test_unit_resource.py` & `cbra-3.0.0a7/tests/test_unit_resource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/test_unit_session.py` & `cbra-3.0.0a7/tests/test_unit_session.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a91/tests/types/test_unit_basemodel_identity.py` & `cbra-3.0.0a7/tests/types/test_unit_basemodel_identity.py`

 * *Files identical despite different names*

