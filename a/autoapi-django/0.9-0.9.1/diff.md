# Comparing `tmp/autoapi-django-0.9.tar.gz` & `tmp/autoapi-django-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoapi-django-0.9.tar", last modified: Sat Apr 29 09:33:55 2023, max compression
+gzip compressed data, was "autoapi-django-0.9.1.tar", last modified: Sat Apr 29 10:09:01 2023, max compression
```

## Comparing `autoapi-django-0.9.tar` & `autoapi-django-0.9.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/
--rw-r--r--   0 th        (1000) th        (1000)     1107 2023-04-07 21:50:01.000000 autoapi-django-0.9/LICENSE.txt
--rw-r--r--   0 th        (1000) th        (1000)       34 2023-04-07 21:50:01.000000 autoapi-django-0.9/MANIFEST.in
--rw-r--r--   0 th        (1000) th        (1000)     3041 2023-04-29 09:33:55.756359 autoapi-django-0.9/PKG-INFO
--rw-r--r--   0 th        (1000) th        (1000)     1280 2023-04-08 23:10:32.000000 autoapi-django-0.9/README.md
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/__init__.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/api/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      726 2023-04-08 23:19:52.000000 autoapi-django-0.9/autoapi/api/encoders.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/api/http_explorer/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/http_explorer/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      789 2023-04-08 23:34:33.000000 autoapi-django-0.9/autoapi/api/http_explorer/interface.py
--rw-r--r--   0 th        (1000) th        (1000)      573 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/http_explorer/openapi_views.py
--rw-r--r--   0 th        (1000) th        (1000)     1017 2023-04-08 23:34:32.000000 autoapi-django-0.9/autoapi/api/http_explorer/swagger.py
--rw-r--r--   0 th        (1000) th        (1000)      288 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/response.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/api/routes/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/routes/__init__.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/api/routes/django/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/routes/django/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)     4945 2023-04-23 19:46:47.000000 autoapi-django-0.9/autoapi/api/routes/django/base.py
--rw-r--r--   0 th        (1000) th        (1000)     1541 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/api/routes/django/http.py
--rw-r--r--   0 th        (1000) th        (1000)      745 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/api/routes/interface.py
--rw-r--r--   0 th        (1000) th        (1000)      466 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/api/routes/urls.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/api/schema_serializers/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/api/schema_serializers/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      459 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/api/schema_serializers/interface.py
--rw-r--r--   0 th        (1000) th        (1000)     7090 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/api/schema_serializers/openapi.py
--rw-r--r--   0 th        (1000) th        (1000)     2250 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/app.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/auth/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/auth/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      428 2023-04-09 16:42:28.000000 autoapi-django-0.9/autoapi/auth/interface.py
--rw-r--r--   0 th        (1000) th        (1000)      400 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/auth/provider.py
--rw-r--r--   0 th        (1000) th        (1000)      101 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/auth/vars.py
--rw-r--r--   0 th        (1000) th        (1000)     6821 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/dependencies.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/deserializers/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/deserializers/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      476 2023-04-23 19:39:05.000000 autoapi-django-0.9/autoapi/deserializers/content_deserializer.py
--rw-r--r--   0 th        (1000) th        (1000)      956 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/interface.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.746359 autoapi-django-0.9/autoapi/deserializers/parsers/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)      333 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/bool.py
--rw-r--r--   0 th        (1000) th        (1000)      372 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/deserializers/parsers/date.py
--rw-r--r--   0 th        (1000) th        (1000)      392 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/deserializers/parsers/datetime.py
--rw-r--r--   0 th        (1000) th        (1000)      660 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/exception.py
--rw-r--r--   0 th        (1000) th        (1000)      336 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/float.py
--rw-r--r--   0 th        (1000) th        (1000)      330 2023-04-23 19:36:47.000000 autoapi-django-0.9/autoapi/deserializers/parsers/int.py
--rw-r--r--   0 th        (1000) th        (1000)      706 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/list.py
--rw-r--r--   0 th        (1000) th        (1000)      929 2023-04-23 19:40:49.000000 autoapi-django-0.9/autoapi/deserializers/parsers/model.py
--rw-r--r--   0 th        (1000) th        (1000)      330 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/deserializers/parsers/str.py
--rw-r--r--   0 th        (1000) th        (1000)      372 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/deserializers/parsers/time.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/autoapi/schema/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/schema/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)     1305 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/annotation.py
--rw-r--r--   0 th        (1000) th        (1000)     1932 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/data.py
--rw-r--r--   0 th        (1000) th        (1000)      124 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/schema/empty.py
--rw-r--r--   0 th        (1000) th        (1000)      216 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/enums.py
--rw-r--r--   0 th        (1000) th        (1000)     2211 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/schema/interfaces.py
--rw-r--r--   0 th        (1000) th        (1000)     2840 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/method.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/autoapi/schema/parsers/
--rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/parsers/__init__.py
--rw-r--r--   0 th        (1000) th        (1000)     1063 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/parsers/dataclass.py
--rw-r--r--   0 th        (1000) th        (1000)      483 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/schema/parsers/date.py
--rw-r--r--   0 th        (1000) th        (1000)      491 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/schema/parsers/datetime.py
--rw-r--r--   0 th        (1000) th        (1000)     1416 2023-04-23 19:30:38.000000 autoapi-django-0.9/autoapi/schema/parsers/django.py
--rw-r--r--   0 th        (1000) th        (1000)     1008 2023-04-22 11:43:50.000000 autoapi-django-0.9/autoapi/schema/parsers/exception.py
--rw-r--r--   0 th        (1000) th        (1000)      456 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/parsers/file.py
--rw-r--r--   0 th        (1000) th        (1000)      486 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/parsers/primitive.py
--rw-r--r--   0 th        (1000) th        (1000)      483 2023-04-23 19:30:33.000000 autoapi-django-0.9/autoapi/schema/parsers/time.py
--rw-r--r--   0 th        (1000) th        (1000)     1153 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/service.py
--rw-r--r--   0 th        (1000) th        (1000)      375 2023-04-08 23:06:09.000000 autoapi-django-0.9/autoapi/schema/types.py
--rw-r--r--   0 th        (1000) th        (1000)     3867 2023-04-08 22:16:13.000000 autoapi-django-0.9/autoapi/schema/utils.py
--rw-r--r--   0 th        (1000) th        (1000)      327 2023-04-08 22:23:53.000000 autoapi-django-0.9/autoapi/settings.py
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.736359 autoapi-django-0.9/autoapi/templates/
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/autoapi/templates/autoapi/
--rw-r--r--   0 th        (1000) th        (1000)      666 2023-04-07 21:50:01.000000 autoapi-django-0.9/autoapi/templates/autoapi/swagger.html
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/autoapi_django.egg-info/
--rw-r--r--   0 th        (1000) th        (1000)     3041 2023-04-29 09:33:55.000000 autoapi-django-0.9/autoapi_django.egg-info/PKG-INFO
--rw-r--r--   0 th        (1000) th        (1000)     2155 2023-04-29 09:33:55.000000 autoapi-django-0.9/autoapi_django.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1000) th        (1000)        1 2023-04-29 09:33:55.000000 autoapi-django-0.9/autoapi_django.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1000) th        (1000)       87 2023-04-29 09:33:55.000000 autoapi-django-0.9/autoapi_django.egg-info/requires.txt
--rw-r--r--   0 th        (1000) th        (1000)        8 2023-04-29 09:33:55.000000 autoapi-django-0.9/autoapi_django.egg-info/top_level.txt
--rw-r--r--   0 th        (1000) th        (1000)      981 2023-04-29 09:33:46.000000 autoapi-django-0.9/pyproject.toml
--rw-r--r--   0 th        (1000) th        (1000)       38 2023-04-29 09:33:55.756359 autoapi-django-0.9/setup.cfg
-drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 09:33:55.756359 autoapi-django-0.9/tests/
--rw-r--r--   0 th        (1000) th        (1000)     2475 2023-04-22 11:43:50.000000 autoapi-django-0.9/tests/test_auth.py
--rw-r--r--   0 th        (1000) th        (1000)     1140 2023-04-22 11:43:50.000000 autoapi-django-0.9/tests/test_quickstart.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/
+-rw-r--r--   0 th        (1000) th        (1000)     1107 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/LICENSE.txt
+-rw-r--r--   0 th        (1000) th        (1000)       34 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/MANIFEST.in
+-rw-r--r--   0 th        (1000) th        (1000)     3043 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/PKG-INFO
+-rw-r--r--   0 th        (1000) th        (1000)     1280 2023-04-08 23:10:32.000000 autoapi-django-0.9.1/README.md
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.456361 autoapi-django-0.9.1/autoapi/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/__init__.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.456361 autoapi-django-0.9.1/autoapi/api/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      726 2023-04-08 23:19:52.000000 autoapi-django-0.9.1/autoapi/api/encoders.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.456361 autoapi-django-0.9.1/autoapi/api/http_explorer/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/http_explorer/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      789 2023-04-08 23:34:33.000000 autoapi-django-0.9.1/autoapi/api/http_explorer/interface.py
+-rw-r--r--   0 th        (1000) th        (1000)      573 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/http_explorer/openapi_views.py
+-rw-r--r--   0 th        (1000) th        (1000)     1017 2023-04-08 23:34:32.000000 autoapi-django-0.9.1/autoapi/api/http_explorer/swagger.py
+-rw-r--r--   0 th        (1000) th        (1000)      288 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/response.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.466361 autoapi-django-0.9.1/autoapi/api/routes/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/routes/__init__.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.466361 autoapi-django-0.9.1/autoapi/api/routes/django/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/routes/django/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)     5354 2023-04-29 10:07:20.000000 autoapi-django-0.9.1/autoapi/api/routes/django/base.py
+-rw-r--r--   0 th        (1000) th        (1000)     1541 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/api/routes/django/http.py
+-rw-r--r--   0 th        (1000) th        (1000)      745 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/api/routes/interface.py
+-rw-r--r--   0 th        (1000) th        (1000)      466 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/api/routes/urls.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.466361 autoapi-django-0.9.1/autoapi/api/schema_serializers/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/api/schema_serializers/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      459 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/api/schema_serializers/interface.py
+-rw-r--r--   0 th        (1000) th        (1000)     7090 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/api/schema_serializers/openapi.py
+-rw-r--r--   0 th        (1000) th        (1000)     2250 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/app.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.466361 autoapi-django-0.9.1/autoapi/auth/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/auth/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      428 2023-04-09 16:42:28.000000 autoapi-django-0.9.1/autoapi/auth/interface.py
+-rw-r--r--   0 th        (1000) th        (1000)      400 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/auth/provider.py
+-rw-r--r--   0 th        (1000) th        (1000)      101 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/auth/vars.py
+-rw-r--r--   0 th        (1000) th        (1000)     6821 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/dependencies.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.466361 autoapi-django-0.9.1/autoapi/deserializers/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/deserializers/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      476 2023-04-23 19:39:05.000000 autoapi-django-0.9.1/autoapi/deserializers/content_deserializer.py
+-rw-r--r--   0 th        (1000) th        (1000)      956 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/interface.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.476361 autoapi-django-0.9.1/autoapi/deserializers/parsers/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)      333 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/bool.py
+-rw-r--r--   0 th        (1000) th        (1000)      372 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/date.py
+-rw-r--r--   0 th        (1000) th        (1000)      392 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/datetime.py
+-rw-r--r--   0 th        (1000) th        (1000)      660 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/exception.py
+-rw-r--r--   0 th        (1000) th        (1000)      336 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/float.py
+-rw-r--r--   0 th        (1000) th        (1000)      330 2023-04-23 19:36:47.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/int.py
+-rw-r--r--   0 th        (1000) th        (1000)      706 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/list.py
+-rw-r--r--   0 th        (1000) th        (1000)      929 2023-04-23 19:40:49.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/model.py
+-rw-r--r--   0 th        (1000) th        (1000)      330 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/str.py
+-rw-r--r--   0 th        (1000) th        (1000)      372 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/deserializers/parsers/time.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.486361 autoapi-django-0.9.1/autoapi/schema/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/schema/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)     1305 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/annotation.py
+-rw-r--r--   0 th        (1000) th        (1000)     1932 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/data.py
+-rw-r--r--   0 th        (1000) th        (1000)      124 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/schema/empty.py
+-rw-r--r--   0 th        (1000) th        (1000)      216 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/enums.py
+-rw-r--r--   0 th        (1000) th        (1000)     2211 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/schema/interfaces.py
+-rw-r--r--   0 th        (1000) th        (1000)     2840 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/method.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/autoapi/schema/parsers/
+-rw-r--r--   0 th        (1000) th        (1000)        0 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/parsers/__init__.py
+-rw-r--r--   0 th        (1000) th        (1000)     1063 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/parsers/dataclass.py
+-rw-r--r--   0 th        (1000) th        (1000)      483 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/schema/parsers/date.py
+-rw-r--r--   0 th        (1000) th        (1000)      491 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/schema/parsers/datetime.py
+-rw-r--r--   0 th        (1000) th        (1000)     1416 2023-04-23 19:30:38.000000 autoapi-django-0.9.1/autoapi/schema/parsers/django.py
+-rw-r--r--   0 th        (1000) th        (1000)     1008 2023-04-22 11:43:50.000000 autoapi-django-0.9.1/autoapi/schema/parsers/exception.py
+-rw-r--r--   0 th        (1000) th        (1000)      456 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/parsers/file.py
+-rw-r--r--   0 th        (1000) th        (1000)      486 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/parsers/primitive.py
+-rw-r--r--   0 th        (1000) th        (1000)      483 2023-04-23 19:30:33.000000 autoapi-django-0.9.1/autoapi/schema/parsers/time.py
+-rw-r--r--   0 th        (1000) th        (1000)     1153 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/service.py
+-rw-r--r--   0 th        (1000) th        (1000)      375 2023-04-08 23:06:09.000000 autoapi-django-0.9.1/autoapi/schema/types.py
+-rw-r--r--   0 th        (1000) th        (1000)     3867 2023-04-08 22:16:13.000000 autoapi-django-0.9.1/autoapi/schema/utils.py
+-rw-r--r--   0 th        (1000) th        (1000)      327 2023-04-08 22:23:53.000000 autoapi-django-0.9.1/autoapi/settings.py
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.446361 autoapi-django-0.9.1/autoapi/templates/
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/autoapi/templates/autoapi/
+-rw-r--r--   0 th        (1000) th        (1000)      666 2023-04-07 21:50:01.000000 autoapi-django-0.9.1/autoapi/templates/autoapi/swagger.html
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/autoapi_django.egg-info/
+-rw-r--r--   0 th        (1000) th        (1000)     3043 2023-04-29 10:09:01.000000 autoapi-django-0.9.1/autoapi_django.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1000) th        (1000)     2155 2023-04-29 10:09:01.000000 autoapi-django-0.9.1/autoapi_django.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1000) th        (1000)        1 2023-04-29 10:09:01.000000 autoapi-django-0.9.1/autoapi_django.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1000) th        (1000)       87 2023-04-29 10:09:01.000000 autoapi-django-0.9.1/autoapi_django.egg-info/requires.txt
+-rw-r--r--   0 th        (1000) th        (1000)        8 2023-04-29 10:09:01.000000 autoapi-django-0.9.1/autoapi_django.egg-info/top_level.txt
+-rw-r--r--   0 th        (1000) th        (1000)      983 2023-04-29 10:08:35.000000 autoapi-django-0.9.1/pyproject.toml
+-rw-r--r--   0 th        (1000) th        (1000)       38 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/setup.cfg
+drwxr-xr-x   0 th        (1000) th        (1000)        0 2023-04-29 10:09:01.496361 autoapi-django-0.9.1/tests/
+-rw-r--r--   0 th        (1000) th        (1000)     2475 2023-04-22 11:43:50.000000 autoapi-django-0.9.1/tests/test_auth.py
+-rw-r--r--   0 th        (1000) th        (1000)     1140 2023-04-22 11:43:50.000000 autoapi-django-0.9.1/tests/test_quickstart.py
```

### Comparing `autoapi-django-0.9/LICENSE.txt` & `autoapi-django-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/PKG-INFO` & `autoapi-django-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoapi-django
-Version: 0.9
+Version: 0.9.1
 Summary: Library for generating transport logic for web application
 Author-email: Artem Romanukov <vens148@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2018 Sebastián Ramírez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoapi-django-0.9/README.md` & `autoapi-django-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/encoders.py` & `autoapi-django-0.9.1/autoapi/api/encoders.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/http_explorer/interface.py` & `autoapi-django-0.9.1/autoapi/api/http_explorer/interface.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/http_explorer/openapi_views.py` & `autoapi-django-0.9.1/autoapi/api/http_explorer/openapi_views.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/http_explorer/swagger.py` & `autoapi-django-0.9.1/autoapi/api/http_explorer/swagger.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/routes/django/base.py` & `autoapi-django-0.9.1/autoapi/api/routes/django/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import traceback
 
 from typing import Any
 from uuid import uuid4
 from pathlib import Path
 
 import magic
+from django.contrib.auth import login, logout
 
 from django.core.files import File
 from django.http import HttpRequest, HttpResponse, StreamingHttpResponse, FileResponse, JsonResponse
 from django.utils.decorators import method_decorator
 from django.views import View
 from django.views.decorators.csrf import csrf_exempt
 
@@ -35,15 +36,22 @@
             self.auth.authorize(request)
             if request.method == 'GET':
                 kwargs = self._GET(request)
             elif request.method == 'POST':
                 kwargs = self._POST(request)
             else:
                 raise ValueError(f'HTTP method {request.method} does not allowed')
+            user_before_execution = self.auth.user_context_var.get()
             result = self.execute_method(**kwargs)
+            user_after_execution = self.auth.user_context_var.get()
+            if user_before_execution != user_after_execution:
+                if user_after_execution:
+                    login(request, user_after_execution)
+                else:
+                    logout(request)
             return self._make_http_response(result)
         except BaseException as exc:
             result = self._wrap_panic(exc)
             logging.warning(traceback.format_exc(), f'Exception ID: {result.panic["id"]}')
             return self._make_http_response(result)
 
     def execute_method(self, **kwargs) -> Response:
```

### Comparing `autoapi-django-0.9/autoapi/api/routes/django/http.py` & `autoapi-django-0.9.1/autoapi/api/routes/django/http.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/routes/interface.py` & `autoapi-django-0.9.1/autoapi/api/routes/interface.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/api/schema_serializers/openapi.py` & `autoapi-django-0.9.1/autoapi/api/schema_serializers/openapi.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/app.py` & `autoapi-django-0.9.1/autoapi/app.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/dependencies.py` & `autoapi-django-0.9.1/autoapi/dependencies.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/deserializers/interface.py` & `autoapi-django-0.9.1/autoapi/deserializers/interface.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/deserializers/parsers/exception.py` & `autoapi-django-0.9.1/autoapi/deserializers/parsers/exception.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/deserializers/parsers/list.py` & `autoapi-django-0.9.1/autoapi/deserializers/parsers/list.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/deserializers/parsers/model.py` & `autoapi-django-0.9.1/autoapi/deserializers/parsers/model.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/annotation.py` & `autoapi-django-0.9.1/autoapi/schema/annotation.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/data.py` & `autoapi-django-0.9.1/autoapi/schema/data.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/interfaces.py` & `autoapi-django-0.9.1/autoapi/schema/interfaces.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/method.py` & `autoapi-django-0.9.1/autoapi/schema/method.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/parsers/dataclass.py` & `autoapi-django-0.9.1/autoapi/schema/parsers/dataclass.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/parsers/django.py` & `autoapi-django-0.9.1/autoapi/schema/parsers/django.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/parsers/exception.py` & `autoapi-django-0.9.1/autoapi/schema/parsers/exception.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/service.py` & `autoapi-django-0.9.1/autoapi/schema/service.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/schema/utils.py` & `autoapi-django-0.9.1/autoapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi/templates/autoapi/swagger.html` & `autoapi-django-0.9.1/autoapi/templates/autoapi/swagger.html`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/autoapi_django.egg-info/PKG-INFO` & `autoapi-django-0.9.1/autoapi_django.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoapi-django
-Version: 0.9
+Version: 0.9.1
 Summary: Library for generating transport logic for web application
 Author-email: Artem Romanukov <vens148@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2018 Sebastián Ramírez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autoapi-django-0.9/autoapi_django.egg-info/SOURCES.txt` & `autoapi-django-0.9.1/autoapi_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/pyproject.toml` & `autoapi-django-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "autoapi-django"
-version = "0.9"
+version = "0.9.1"
 description = "Library for generating transport logic for web application"
 authors = [
     {name = "Artem Romanukov", email="vens148@gmail.com"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `autoapi-django-0.9/tests/test_auth.py` & `autoapi-django-0.9.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `autoapi-django-0.9/tests/test_quickstart.py` & `autoapi-django-0.9.1/tests/test_quickstart.py`

 * *Files identical despite different names*

