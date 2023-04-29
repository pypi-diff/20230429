# Comparing `tmp/graphene-django-3.0.0b9.tar.gz` & `tmp/graphene-django-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.0.0b9.tar", last modified: Sun Sep 25 22:28:33 2022, max compression
+gzip compressed data, was "graphene-django-3.0.1.tar", last modified: Sat Apr 29 17:28:06 2023, max compression
```

## Comparing `graphene-django-3.0.0b9.tar` & `graphene-django-3.0.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    12480 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5018 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9018 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8566 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5012 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4241 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)    37439 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    11682 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6632 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     5945 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.293887 graphene-django-3.0.0b9/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6376 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8523 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (121)    14943 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    15043 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)    11648 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (121)    49777 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    17555 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    23812 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)    11036 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5654 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.297887 graphene-django-3.0.0b9/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14586 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 22:28:33.289887 graphene-django-3.0.0b9/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-25 22:28:33.000000 graphene-django-3.0.0b9/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-09-25 22:28:33.301887 graphene-django-3.0.0b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-09-25 22:28:29.000000 graphene-django-3.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.901130 graphene-django-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-29 17:28:03.000000 graphene-django-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-29 17:28:03.000000 graphene-django-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 17:28:06.901130 graphene-django-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 17:28:03.000000 graphene-django-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-29 17:28:03.000000 graphene-django-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.877130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.889130 graphene-django-3.0.1/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.893130 graphene-django-3.0.1/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.881130 graphene-django-3.0.1/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.885130 graphene-django-3.0.1/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49752 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.897130 graphene-django-3.0.1/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-29 17:28:03.000000 graphene-django-3.0.1/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:28:06.889130 graphene-django-3.0.1/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 17:28:06.000000 graphene-django-3.0.1/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-29 17:28:06.901130 graphene-django-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-29 17:28:03.000000 graphene-django-3.0.1/setup.py
```

### Comparing `graphene-django-3.0.0b9/LICENSE` & `graphene-django-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/PKG-INFO` & `graphene-django-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.0.0b9
+Version: 3.0.1
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.0.0b9/README.md` & `graphene-django-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/README.rst` & `graphene-django-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/compat.py` & `graphene-django-3.0.1/graphene_django/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class MissingType(object):
+class MissingType:
     def __init__(self, *args, **kwargs):
         pass
 
 
 try:
     # Postgres fields are only available in Django with psycopg2 installed
     # and we cannot have psycopg2 on PyPy
```

### Comparing `graphene-django-3.0.0b9/graphene_django/converter.py` & `graphene-django-3.0.1/graphene_django/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,21 @@
     String,
     Time,
     Decimal,
 )
 from graphene.types.json import JSONString
 from graphene.types.scalars import BigInt
 from graphene.utils.str_converters import to_camel_case
-from graphql import GraphQLError, assert_valid_name
+from graphql import GraphQLError
+
+try:
+    from graphql import assert_name
+except ImportError:
+    # Support for older versions of graphql
+    from graphql import assert_valid_name as assert_name
 from graphql.pyutils import register_description
 
 from .compat import ArrayField, HStoreField, JSONField, PGJSONField, RangeField
 from .fields import DjangoListField, DjangoConnectionField
 from .settings import graphene_settings
 from .utils.str_converters import to_const
 
@@ -52,28 +58,27 @@
 
         return blank_field_wrapper(resolver)
 
 
 def convert_choice_name(name):
     name = to_const(force_str(name))
     try:
-        assert_valid_name(name)
+        assert_name(name)
     except GraphQLError:
         name = "A_%s" % name
     return name
 
 
 def get_choices(choices):
     converted_names = []
     if isinstance(choices, OrderedDict):
         choices = choices.items()
     for value, help_text in choices:
         if isinstance(help_text, (tuple, list)):
-            for choice in get_choices(help_text):
-                yield choice
+            yield from get_choices(help_text)
         else:
             name = convert_choice_name(value)
             while name in converted_names:
                 name += "_" + str(len(converted_names))
             converted_names.append(name)
             description = str(
                 help_text
@@ -82,15 +87,15 @@
 
 
 def convert_choices_to_named_enum_with_descriptions(name, choices):
     choices = list(get_choices(choices))
     named_choices = [(c[0], c[1]) for c in choices]
     named_choices_descriptions = {c[0]: c[2] for c in choices}
 
-    class EnumWithDescriptionsType(object):
+    class EnumWithDescriptionsType:
         @property
         def description(self):
             return str(named_choices_descriptions[self.name])
 
     return_type = Enum(name, list(named_choices), type=EnumWithDescriptionsType)
     return return_type
 
@@ -99,15 +104,15 @@
     if graphene_settings.DJANGO_CHOICE_FIELD_ENUM_CUSTOM_NAME:
         # Try and import custom function
         custom_func = import_string(
             graphene_settings.DJANGO_CHOICE_FIELD_ENUM_CUSTOM_NAME
         )
         name = custom_func(field)
     elif graphene_settings.DJANGO_CHOICE_FIELD_ENUM_V2_NAMING is True:
-        name = to_camel_case("{}_{}".format(django_model_meta.object_name, field.name))
+        name = to_camel_case(f"{django_model_meta.object_name}_{field.name}")
     else:
         name = "{app_label}{object_name}{field_name}Choices".format(
             app_label=to_camel_case(django_model_meta.app_label.title()),
             object_name=django_model_meta.object_name,
             field_name=to_camel_case(field.name.title()),
         )
     return name
@@ -145,15 +150,17 @@
 def get_django_field_description(field):
     return str(field.help_text) if field.help_text else None
 
 
 @singledispatch
 def convert_django_field(field, registry=None):
     raise Exception(
-        "Don't know how to convert the Django field %s (%s)" % (field, field.__class__)
+        "Don't know how to convert the Django field {} ({})".format(
+            field, field.__class__
+        )
     )
 
 
 @convert_django_field.register(models.CharField)
 @convert_django_field.register(models.TextField)
 @convert_django_field.register(models.EmailField)
 @convert_django_field.register(models.SlugField)
@@ -307,25 +314,27 @@
         _type = registry.get_type_for_model(model)
         if not _type:
             return
 
         class CustomField(Field):
             def wrap_resolve(self, parent_resolver):
                 """
-                Implements a custom resolver which go through the `get_node` method to insure that
+                Implements a custom resolver which go through the `get_node` method to ensure that
                 it goes through the `get_queryset` method of the DjangoObjectType.
                 """
                 resolver = super().wrap_resolve(parent_resolver)
 
                 def custom_resolver(root, info, **args):
                     fk_obj = resolver(root, info, **args)
-                    if fk_obj is None:
-                        return None
-                    else:
-                        return _type.get_node(info, fk_obj.pk)
+                    if not isinstance(fk_obj, model):
+                        # In case the resolver is a custom one that overwrites
+                        # the default Django resolver
+                        # This happens, for example, when using custom awaitable resolvers.
+                        return fk_obj
+                    return _type.get_node(info, fk_obj.pk)
 
                 return custom_resolver
 
         return CustomField(
             _type,
             description=get_django_field_description(field),
             required=not field.null,
```

### Comparing `graphene-django-3.0.0b9/graphene_django/debug/middleware.py` & `graphene-django-3.0.1/graphene_django/debug/middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,54 +3,54 @@
 from promise import Promise
 
 from .sql.tracking import unwrap_cursor, wrap_cursor
 from .exception.formating import wrap_exception
 from .types import DjangoDebug
 
 
-class DjangoDebugContext(object):
+class DjangoDebugContext:
     def __init__(self):
-        self.debug_promise = None
-        self.promises = []
+        self.debug_result = None
+        self.results = []
         self.object = DjangoDebug(sql=[], exceptions=[])
         self.enable_instrumentation()
 
-    def get_debug_promise(self):
-        if not self.debug_promise:
-            self.debug_promise = Promise.all(self.promises)
-            self.promises = []
-        return self.debug_promise.then(self.on_resolve_all_promises).get()
+    def get_debug_result(self):
+        if not self.debug_result:
+            self.debug_result = self.results
+            self.results = []
+        return self.on_resolve_all_results()
 
     def on_resolve_error(self, value):
         if hasattr(self, "object"):
             self.object.exceptions.append(wrap_exception(value))
-        return Promise.reject(value)
+        return value
 
-    def on_resolve_all_promises(self, values):
-        if self.promises:
-            self.debug_promise = None
-            return self.get_debug_promise()
+    def on_resolve_all_results(self):
+        if self.results:
+            self.debug_result = None
+            return self.get_debug_result()
         self.disable_instrumentation()
         return self.object
 
-    def add_promise(self, promise):
-        if self.debug_promise:
-            self.promises.append(promise)
+    def add_result(self, result):
+        if self.debug_result:
+            self.results.append(result)
 
     def enable_instrumentation(self):
         # This is thread-safe because database connections are thread-local.
         for connection in connections.all():
             wrap_cursor(connection, self)
 
     def disable_instrumentation(self):
         for connection in connections.all():
             unwrap_cursor(connection)
 
 
-class DjangoDebugMiddleware(object):
+class DjangoDebugMiddleware:
     def resolve(self, next, root, info, **args):
         context = info.context
         django_debug = getattr(context, "django_debug", None)
         if not django_debug:
             if context is None:
                 raise Exception("DjangoDebug cannot be executed in None contexts")
             try:
@@ -58,14 +58,14 @@
             except Exception:
                 raise Exception(
                     "DjangoDebug need the context to be writable, context received: {}.".format(
                         context.__class__.__name__
                     )
                 )
         if info.schema.get_type("DjangoDebug") == info.return_type:
-            return context.django_debug.get_debug_promise()
+            return context.django_debug.get_debug_result()
         try:
-            promise = next(root, info, **args)
+            result = next(root, info, **args)
         except Exception as e:
             return context.django_debug.on_resolve_error(e)
-        context.django_debug.add_promise(promise)
-        return promise
+        context.django_debug.add_result(result)
+        return result
```

### Comparing `graphene-django-3.0.0b9/graphene_django/debug/sql/tracking.py` & `graphene-django-3.0.1/graphene_django/debug/sql/tracking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Code obtained from django-debug-toolbar sql panel tracking
-from __future__ import absolute_import, unicode_literals
 
 import json
 from threading import local
 from time import time
 
 from django.utils.encoding import force_str
 
@@ -46,28 +45,28 @@
 def unwrap_cursor(connection):
     if hasattr(connection, "_graphene_cursor"):
         previous_cursor = connection._graphene_cursor
         connection.cursor = previous_cursor
         del connection._graphene_cursor
 
 
-class ExceptionCursorWrapper(object):
+class ExceptionCursorWrapper:
     """
     Wraps a cursor and raises an exception on any operation.
     Used in Templates panel.
     """
 
     def __init__(self, cursor, db, logger):
         pass
 
     def __getattr__(self, attr):
         raise SQLQueryTriggered()
 
 
-class NormalCursorWrapper(object):
+class NormalCursorWrapper:
     """
     Wraps a cursor and logs queries.
     """
 
     def __init__(self, cursor, db, logger):
         self.cursor = cursor
         # Instance of a BaseDatabaseWrapper subclass
@@ -81,15 +80,15 @@
         else:
             return repr(element)
 
     def _quote_params(self, params):
         if not params:
             return params
         if isinstance(params, dict):
-            return dict((key, self._quote_expr(value)) for key, value in params.items())
+            return {key: self._quote_expr(value) for key, value in params.items()}
         return list(map(self._quote_expr, params))
 
     def _decode(self, param):
         try:
             return force_str(param, strings_only=True)
         except UnicodeDecodeError:
             return "(encoded string)"
```

### Comparing `graphene-django-3.0.0b9/graphene_django/debug/sql/types.py` & `graphene-django-3.0.1/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/debug/tests/test_query.py` & `graphene-django-3.0.1/graphene_django/debug/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from graphene_django import DjangoConnectionField, DjangoObjectType
 
 from ...tests.models import Reporter
 from ..middleware import DjangoDebugMiddleware
 from ..types import DjangoDebug
 
 
-class context(object):
+class context:
     pass
 
 
 def test_should_query_field():
     r1 = Reporter(last_name="ABA")
     r1.save()
     r2 = Reporter(last_name="Griffin")
```

### Comparing `graphene-django-3.0.0b9/graphene_django/fields.py` & `graphene-django-3.0.1/graphene_django/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, _type, *args, **kwargs):
         from .types import DjangoObjectType
 
         if isinstance(_type, NonNull):
             _type = _type.of_type
 
         # Django would never return a Set of None  vvvvvvv
-        super(DjangoListField, self).__init__(List(NonNull(_type)), *args, **kwargs)
+        super().__init__(List(NonNull(_type)), *args, **kwargs)
 
         assert issubclass(
             self._underlying_type, DjangoObjectType
         ), "DjangoListField only accepts DjangoObjectType types"
 
     @property
     def _underlying_type(self):
@@ -59,15 +59,15 @@
         if isinstance(queryset, QuerySet):
             # Pass queryset to the DjangoObjectType get_queryset method
             queryset = maybe_queryset(django_object_type.get_queryset(queryset, info))
 
         return queryset
 
     def wrap_resolve(self, parent_resolver):
-        resolver = super(DjangoListField, self).wrap_resolve(parent_resolver)
+        resolver = super().wrap_resolve(parent_resolver)
         _type = self.type
         if isinstance(_type, NonNull):
             _type = _type.of_type
         django_object_type = _type.of_type.of_type
         return partial(
             self.list_resolver,
             django_object_type,
@@ -83,15 +83,15 @@
             "max_limit", graphene_settings.RELAY_CONNECTION_MAX_LIMIT
         )
         self.enforce_first_or_last = kwargs.pop(
             "enforce_first_or_last",
             graphene_settings.RELAY_CONNECTION_ENFORCE_FIRST_OR_LAST,
         )
         kwargs.setdefault("offset", Int())
-        super(DjangoConnectionField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def type(self):
         from .types import DjangoObjectType
 
         _type = super(ConnectionField, self).type
         non_null = False
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/__init__.py` & `graphene-django-3.0.1/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/fields.py` & `graphene-django-3.0.1/graphene_django/filter/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ):
         self._fields = fields
         self._provided_filterset_class = filterset_class
         self._filterset_class = None
         self._filtering_args = None
         self._extra_filter_meta = extra_filter_meta
         self._base_args = None
-        super(DjangoFilterConnectionField, self).__init__(type_, *args, **kwargs)
+        super().__init__(type_, *args, **kwargs)
 
     @property
     def args(self):
         return to_arguments(self._base_args or OrderedDict(), self.filtering_args)
 
     @args.setter
     def args(self, args):
@@ -86,17 +86,15 @@
             for k, v in args.items():
                 if k in filtering_args:
                     if k == "order_by" and v is not None:
                         v = to_snake_case(v)
                     kwargs[k] = convert_enum(v)
             return kwargs
 
-        qs = super(DjangoFilterConnectionField, cls).resolve_queryset(
-            connection, iterable, info, args
-        )
+        qs = super().resolve_queryset(connection, iterable, info, args)
 
         filterset = filterset_class(
             data=filter_kwargs(), queryset=qs, request=info.context
         )
         if filterset.is_valid():
             return filterset.qs
         raise ValidationError(filterset.form.errors.as_json())
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/__init__.py` & `graphene-django-3.0.1/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.0.1/graphene_django/filter/filters/list_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from django_filters.constants import EMPTY_VALUES
-
 from .typed_filter import TypedFilter
 
 
-class ArrayFilter(TypedFilter):
+class ListFilter(TypedFilter):
     """
-    Filter made for PostgreSQL ArrayField.
+    Filter that takes a list of value as input.
+    It is for example used for `__in` filters.
     """
 
     def filter(self, qs, value):
         """
         Override the default filter class to check first whether the list is
         empty or not.
-        This needs to be done as in this case we expect to get the filter applied with
-        an empty list since it's a valid value but django_filter consider an empty list
+        This needs to be done as in this case we expect to get an empty output
+        (if not an exclude filter) but django_filter consider an empty list
         to be an empty input value (see `EMPTY_VALUES`) meaning that
         the filter does not need to be applied (hence returning the original
         queryset).
         """
-        if value in EMPTY_VALUES and value != []:
-            return qs
-        if self.distinct:
-            qs = qs.distinct()
-        lookup = "%s__%s" % (self.field_name, self.lookup_expr)
-        qs = self.get_method(qs)(**{lookup: value})
-        return qs
+        if value is not None and len(value) == 0:
+            if self.exclude:
+                return qs
+            else:
+                return qs.none()
+        else:
+            return super().filter(qs, value)
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.0.1/graphene_django/filter/filters/global_id_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     field_class = GlobalIDFormField
 
     def filter(self, qs, value):
         """Convert the filter value to a primary key before filtering"""
         _id = None
         if value is not None:
             _, _id = from_global_id(value)
-        return super(GlobalIDFilter, self).filter(qs, _id)
+        return super().filter(qs, _id)
 
 
 class GlobalIDMultipleChoiceFilter(MultipleChoiceFilter):
     field_class = GlobalIDMultipleChoiceField
 
     def filter(self, qs, value):
         gids = [from_global_id(v)[1] for v in value]
-        return super(GlobalIDMultipleChoiceFilter, self).filter(qs, gids)
+        return super().filter(qs, gids)
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.0.1/graphene_django/filter/filters/array_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from django_filters.constants import EMPTY_VALUES
+
 from .typed_filter import TypedFilter
 
 
-class ListFilter(TypedFilter):
+class ArrayFilter(TypedFilter):
     """
-    Filter that takes a list of value as input.
-    It is for example used for `__in` filters.
+    Filter made for PostgreSQL ArrayField.
     """
 
     def filter(self, qs, value):
         """
         Override the default filter class to check first whether the list is
         empty or not.
-        This needs to be done as in this case we expect to get an empty output
-        (if not an exclude filter) but django_filter consider an empty list
+        This needs to be done as in this case we expect to get the filter applied with
+        an empty list since it's a valid value but django_filter consider an empty list
         to be an empty input value (see `EMPTY_VALUES`) meaning that
         the filter does not need to be applied (hence returning the original
         queryset).
         """
-        if value is not None and len(value) == 0:
-            if self.exclude:
-                return qs
-            else:
-                return qs.none()
-        else:
-            return super(ListFilter, self).filter(qs, value)
+        if value in EMPTY_VALUES and value != []:
+            return qs
+        if self.distinct:
+            qs = qs.distinct()
+        lookup = f"{self.field_name}__{self.lookup_expr}"
+        qs = self.get_method(qs)(**{lookup: value})
+        return qs
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.0.1/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.0.1/graphene_django/filter/filters/typed_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Filter class for which the input GraphQL type can explicitly be provided.
     If it is not provided, when building the schema, it will try to guess
     it from the field.
     """
 
     def __init__(self, input_type=None, *args, **kwargs):
         self._input_type = input_type
-        super(TypedFilter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def input_type(self):
         input_type = get_type(self._input_type)
         if input_type is not None:
             if not callable(getattr(input_type, "get_type", None)):
                 raise ValueError(
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/filterset.py` & `graphene-django-3.0.1/graphene_django/filter/filterset.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         )
     )
 
 
 def setup_filterset(filterset_class):
     """Wrap a provided filterset in Graphene-specific functionality"""
     return type(
-        "Graphene{}".format(filterset_class.__name__),
+        f"Graphene{filterset_class.__name__}",
         (filterset_class, GrapheneFilterSetMixin),
         {},
     )
 
 
 def custom_filterset_factory(model, filterset_base_class=FilterSet, **meta):
     """Create a filterset for the given model using the provided meta data"""
     meta.update({"model": model})
-    meta_class = type(str("Meta"), (object,), meta)
+    meta_class = type("Meta", (object,), meta)
     filterset = type(
         str("%sFilterSet" % model._meta.object_name),
         (filterset_base_class, GrapheneFilterSetMixin),
         {"Meta": meta_class},
     )
     return filterset
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/conftest.py` & `graphene-django-3.0.1/graphene_django/filter/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mock import MagicMock
+from unittest.mock import MagicMock
 import pytest
 
 from django.db import models
 from django.db.models.query import QuerySet
 from django_filters import filters
 from django_filters import FilterSet
 import graphene
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/filters.py` & `graphene-django-3.0.1/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def assert_arguments(field, *arguments):
     ignore = ("offset", "after", "before", "first", "last", "order_by")
     args = get_args(field)
     actual = [name for name in args if name not in ignore and not name.startswith("_")]
     assert set(arguments) == set(
         actual
-    ), "Expected arguments ({}) did not match actual ({})".format(arguments, actual)
+    ), f"Expected arguments ({arguments}) did not match actual ({actual})"
 
 
 def assert_orderable(field):
     args = get_args(field)
     assert "order_by" in args, "Field cannot be ordered"
 
 
@@ -137,15 +137,15 @@
     class ArticleContextFilter(django_filters.FilterSet):
         class Meta:
             model = Article
             exclude = set()
 
         @property
         def qs(self):
-            qs = super(ArticleContextFilter, self).qs
+            qs = super().qs
             return qs.filter(reporter=self.request.reporter)
 
     class Query(ObjectType):
         context_articles = DjangoFilterConnectionField(
             ArticleNode, filterset_class=ArticleContextFilter
         )
 
@@ -162,15 +162,15 @@
         headline="a2",
         pub_date=datetime.now(),
         pub_date_time=datetime.now(),
         reporter=r2,
         editor=r2,
     )
 
-    class context(object):
+    class context:
         reporter = r2
 
     query = """
     query {
         contextArticles {
             edges {
                 node {
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_in_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,27 +345,27 @@
         reporter=sara_croche,
         editor=sara_croche,
     )
 
     schema = Schema(query=query)
 
     query = """
-    query {
-        articles (reporter_In: [%s, %s]) {
-            edges {
-                node {
+    query {{
+        articles (reporter_In: [{}, {}]) {{
+            edges {{
+                node {{
                     headline
-                    reporter {
+                    reporter {{
                         lastName
-                    }
-                }
-            }
-        }
-    }
-    """ % (
+                    }}
+                }}
+            }}
+        }}
+    }}
+    """.format(
         john_doe.id,
         jean_bon.id,
     )
     result = schema.execute(query)
     assert not result.errors
     assert result.data["articles"]["edges"] == [
         {"node": {"headline": "A", "reporter": {"lastName": "Doe"}}},
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.0.1/graphene_django/filter/tests/test_typed_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     all_articles_filters = (
         schema_str.split("  articles(")[1]
         .split("): ArticleTypeConnection\n")[0]
         .split(", ")
     )
 
     for filter_field, gql_type in filters.items():
-        assert "{}: {}".format(filter_field, gql_type) in all_articles_filters
+        assert f"{filter_field}: {gql_type}" in all_articles_filters
 
 
 def test_typed_filters_work(schema):
     reporter = Reporter.objects.create(first_name="John", last_name="Doe", email="")
     Article.objects.create(headline="A", reporter=reporter, editor=reporter, lang="es")
     Article.objects.create(headline="B", reporter=reporter, editor=reporter, lang="es")
     Article.objects.create(headline="C", reporter=reporter, editor=reporter, lang="en")
```

### Comparing `graphene-django-3.0.0b9/graphene_django/filter/utils.py` & `graphene-django-3.0.1/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/forms/converter.py` & `graphene-django-3.0.1/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/forms/forms.py` & `graphene-django-3.0.1/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/forms/mutation.py` & `graphene-django-3.0.1/graphene_django/forms/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         output_fields = fields_for_form(form, only_fields, exclude_fields)
 
         _meta = DjangoFormMutationOptions(cls)
         _meta.form_class = form_class
         _meta.fields = yank_fields_from_attrs(output_fields, _as=Field)
 
         input_fields = yank_fields_from_attrs(input_fields, _as=InputField)
-        super(DjangoFormMutation, cls).__init_subclass_with_meta__(
+        super().__init_subclass_with_meta__(
             _meta=_meta, input_fields=input_fields, **options
         )
 
     @classmethod
     def perform_mutate(cls, form, info):
         if hasattr(form, "save"):
             # `save` method won't exist on plain Django forms, but this mutation can
@@ -123,15 +123,15 @@
     def __init_subclass_with_meta__(
         cls,
         form_class=None,
         model=None,
         return_field_name=None,
         only_fields=(),
         exclude_fields=(),
-        **options
+        **options,
     ):
 
         if not form_class:
             raise Exception("form_class is required for DjangoModelFormMutation")
 
         if not model:
             model = form_class._meta.model
@@ -143,15 +143,15 @@
         input_fields = fields_for_form(form, only_fields, exclude_fields)
         if "id" not in exclude_fields:
             input_fields["id"] = graphene.ID()
 
         registry = get_global_registry()
         model_type = registry.get_type_for_model(model)
         if not model_type:
-            raise Exception("No type registered for model: {}".format(model.__name__))
+            raise Exception(f"No type registered for model: {model.__name__}")
 
         if not return_field_name:
             model_name = model.__name__
             return_field_name = model_name[:1].lower() + model_name[1:]
 
         output_fields = OrderedDict()
         output_fields[return_field_name] = graphene.Field(model_type)
@@ -159,15 +159,15 @@
         _meta = DjangoModelDjangoFormMutationOptions(cls)
         _meta.form_class = form_class
         _meta.model = model
         _meta.return_field_name = return_field_name
         _meta.fields = yank_fields_from_attrs(output_fields, _as=Field)
 
         input_fields = yank_fields_from_attrs(input_fields, _as=InputField)
-        super(DjangoModelFormMutation, cls).__init_subclass_with_meta__(
+        super().__init_subclass_with_meta__(
             _meta=_meta, input_fields=input_fields, **options
         )
 
     @classmethod
     def mutate_and_get_payload(cls, root, info, **input):
         form = cls.get_form(root, info, **input)
```

### Comparing `graphene-django-3.0.0b9/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.0.1/graphene_django/forms/tests/test_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django import forms
-from py.test import raises
+from pytest import raises
 
 import graphene
 from graphene import (
     String,
     Int,
     Boolean,
     Decimal,
```

### Comparing `graphene-django-3.0.0b9/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.0.1/graphene_django/forms/tests/test_mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from django import forms
 from django.core.exceptions import ValidationError
-from py.test import raises
+from pytest import raises
 
 from graphene import Field, ObjectType, Schema, String
 from graphene_django import DjangoObjectType
 from graphene_django.tests.forms import PetForm
 from graphene_django.tests.models import Pet
 from graphene_django.tests.mutations import PetMutation
```

### Comparing `graphene-django-3.0.0b9/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.0.1/graphene_django/management/commands/graphql_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,34 +59,30 @@
             outfile.write(print_schema(schema.graphql_schema))
 
     def get_schema(self, schema, out, indent):
         schema_dict = {"data": schema.introspect()}
         if out == "-" or out == "-.json":
             self.stdout.write(json.dumps(schema_dict, indent=indent, sort_keys=True))
         elif out == "-.graphql":
-            self.stdout.write(print_schema(schema))
+            self.stdout.write(print_schema(schema.graphql_schema))
         else:
             # Determine format
             _, file_extension = os.path.splitext(out)
 
             if file_extension == ".graphql":
                 self.save_graphql_file(out, schema)
             elif file_extension == ".json":
                 self.save_json_file(out, schema_dict, indent)
             else:
-                raise CommandError(
-                    'Unrecognised file format "{}"'.format(file_extension)
-                )
+                raise CommandError(f'Unrecognised file format "{file_extension}"')
 
             style = getattr(self, "style", None)
             success = getattr(style, "SUCCESS", lambda x: x)
 
-            self.stdout.write(
-                success("Successfully dumped GraphQL schema to {}".format(out))
-            )
+            self.stdout.write(success(f"Successfully dumped GraphQL schema to {out}"))
 
     def handle(self, *args, **options):
         options_schema = options.get("schema")
 
         if options_schema and type(options_schema) is str:
             module_str, schema_name = options_schema.rsplit(".", 1)
             mod = importlib.import_module(module_str)
```

### Comparing `graphene-django-3.0.0b9/graphene_django/registry.py` & `graphene-django-3.0.1/graphene_django/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class Registry(object):
+class Registry:
     def __init__(self):
         self._registry = {}
         self._field_registry = {}
 
     def register(self, cls):
         from .types import DjangoObjectType
```

### Comparing `graphene-django-3.0.0b9/graphene_django/rest_framework/mutation.py` & `graphene-django-3.0.1/graphene_django/rest_framework/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         _meta.lookup_field = lookup_field
         _meta.model_operations = model_operations
         _meta.serializer_class = serializer_class
         _meta.model_class = model_class
         _meta.fields = yank_fields_from_attrs(output_fields, _as=Field)
 
         input_fields = yank_fields_from_attrs(input_fields, _as=InputField)
-        super(SerializerMutation, cls).__init_subclass_with_meta__(
+        super().__init_subclass_with_meta__(
             _meta=_meta, input_fields=input_fields, **options
         )
 
     @classmethod
     def get_serializer_kwargs(cls, root, info, **input):
         lookup_field = cls._meta.lookup_field
         model_class = cls._meta.model_class
```

### Comparing `graphene-django-3.0.0b9/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.0.1/graphene_django/rest_framework/serializer_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     serializer = serializer_class()
 
     items = {
         name: convert_serializer_field(field)
         for name, field in serializer.fields.items()
     }
     ret_type = type(
-        "{}Input".format(serializer.__class__.__name__),
+        f"{serializer.__class__.__name__}Input",
         (graphene.InputObjectType,),
         items,
     )
     convert_serializer_to_input_type.cache[serializer_class.__name__] = ret_type
     return ret_type
```

### Comparing `graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
 import graphene
 from django.db import models
 from graphene import InputObjectType
-from py.test import raises
+from pytest import raises
 from rest_framework import serializers
 
 from ..serializer_converter import convert_serializer_field
 from ..types import DictType
 
 
 def _get_type(
```

### Comparing `graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.0.1/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-from py.test import raises
+from pytest import raises
 from rest_framework import serializers
 
 from graphene import Field, ResolveInfo
 from graphene.types.inputobjecttype import InputObjectType
 
 from ...types import DjangoObjectType
 from ..models import MyFakeModel, MyFakeModelWithDate, MyFakeModelWithPassword
```

### Comparing `graphene-django-3.0.0b9/graphene_django/settings.py` & `graphene-django-3.0.1/graphene_django/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
         'graphene_django.debug.DjangoDebugMiddleware',
     )
 }
 This module provides the `graphene_settings` object, that is used to access
 Graphene settings, checking for user settings first, then falling
 back to the defaults.
 """
-from __future__ import unicode_literals
 
 from django.conf import settings
 from django.test.signals import setting_changed
 
 import importlib  # Available in Python 3.1+
 
 
@@ -39,14 +38,15 @@
     "SUBSCRIPTION_PATH": None,
     # By default GraphiQL headers editor tab is enabled, set to False to hide it
     # This sets headerEditorEnabled GraphiQL option, for details go to
     # https://github.com/graphql/graphiql/tree/main/packages/graphiql#options
     "GRAPHIQL_HEADER_EDITOR_ENABLED": True,
     "GRAPHIQL_SHOULD_PERSIST_HEADERS": False,
     "ATOMIC_MUTATIONS": False,
+    "TESTING_ENDPOINT": "/graphql",
 }
 
 if settings.DEBUG:
     DEFAULTS["MIDDLEWARE"] += ("graphene_django.debug.DjangoDebugMiddleware",)
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = ("MIDDLEWARE", "SCHEMA")
@@ -73,24 +73,24 @@
     try:
         # Nod to tastypie's use of importlib.
         parts = val.split(".")
         module_path, class_name = ".".join(parts[:-1]), parts[-1]
         module = importlib.import_module(module_path)
         return getattr(module, class_name)
     except (ImportError, AttributeError) as e:
-        msg = "Could not import '%s' for Graphene setting '%s'. %s: %s." % (
+        msg = "Could not import '{}' for Graphene setting '{}'. {}: {}.".format(
             val,
             setting_name,
             e.__class__.__name__,
             e,
         )
         raise ImportError(msg)
 
 
-class GrapheneSettings(object):
+class GrapheneSettings:
     """
     A settings object, that allows API settings to be accessed as properties.
     For example:
         from graphene_django.settings import settings
         print(settings.SCHEMA)
     Any setting with string import paths will be automatically resolved
     and return the class, rather than the string literal.
```

### Comparing `graphene-django-3.0.0b9/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.0.1/graphene_django/templates/graphene/graphiql.html`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/react-dom@{{react_version}}/umd/react-dom.production.min.js"
           integrity="{{react_dom_sri}}"
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/graphiql@{{graphiql_version}}/graphiql.min.js"
           integrity="{{graphiql_sri}}"
           crossorigin="anonymous"></script>
-  <script src="https://cdn.jsdelivr.net/npm/subscriptions-transport-ws@{{subscriptions_transport_ws_version}}/browser/client.js"
+  <script src="https://cdn.jsdelivr.net/npm/graphql-ws@{{subscriptions_transport_ws_version}}/umd/graphql-ws.min.js"
           integrity="{{subscriptions_transport_ws_sri}}"
           crossorigin="anonymous"></script>
 </head>
 <body>
   <div id="editor"></div>
   {% csrf_token %}
   <script type="application/javascript">
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/issues/test_520.py` & `graphene-django-3.0.1/graphene_django/tests/issues/test_520.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from django import forms
 
 import graphene
 
 from graphene import Field, ResolveInfo
 from graphene.types.inputobjecttype import InputObjectType
-from py.test import raises
-from py.test import mark
+from pytest import raises
+from pytest import mark
 from rest_framework import serializers
 
 from ...types import DjangoObjectType
 from ...rest_framework.models import MyFakeModel
 from ...rest_framework.mutation import SerializerMutation
 from ...forms.mutation import DjangoFormMutation
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/models.py` & `graphene-django-3.0.1/graphene_django/tests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 CHOICES = ((1, "this"), (2, _("that")))
 
 
 class Person(models.Model):
@@ -33,15 +31,15 @@
         default="ot",
     )
     reporters = models.ManyToManyField("Reporter", related_name="films")
 
 
 class DoeReporterManager(models.Manager):
     def get_queryset(self):
-        return super(DoeReporterManager, self).get_queryset().filter(last_name="Doe")
+        return super().get_queryset().filter(last_name="Doe")
 
 
 class Reporter(models.Model):
     first_name = models.CharField(max_length=30)
     last_name = models.CharField(max_length=30)
     email = models.EmailField()
     pets = models.ManyToManyField("self")
@@ -53,35 +51,35 @@
         "Reporter Type",
         null=True,
         blank=True,
         choices=[(1, "Regular"), (2, "CNN Reporter")],
     )
 
     def __str__(self):  # __unicode__ on Python 2
-        return "%s %s" % (self.first_name, self.last_name)
+        return f"{self.first_name} {self.last_name}"
 
     def __init__(self, *args, **kwargs):
         """
         Override the init method so that during runtime, Django
         can know that this object can be a CNNReporter by casting
         it to the proxy model. Otherwise, as far as Django knows,
         when a CNNReporter is pulled from the database, it is still
         of type Reporter. This was added to test proxy model support.
         """
-        super(Reporter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         if self.reporter_type == 2:  # quick and dirty way without enums
             self.__class__ = CNNReporter
 
     def some_method(self):
         return 123
 
 
 class CNNReporterManager(models.Manager):
     def get_queryset(self):
-        return super(CNNReporterManager, self).get_queryset().filter(reporter_type=2)
+        return super().get_queryset().filter(reporter_type=2)
 
 
 class CNNReporter(Reporter):
     """
     This class is a proxy model for Reporter, used for testing
     proxy model support
     """
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/schema.py` & `graphene-django-3.0.1/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/schema_view.py` & `graphene-django-3.0.1/graphene_django/tests/schema_view.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_command.py` & `graphene-django-3.0.1/graphene_django/tests/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from textwrap import dedent
 
 from django.core import management
 from io import StringIO
-from mock import mock_open, patch
+from unittest.mock import mock_open, patch
 
 from graphene import ObjectType, Schema, String
 
 
 @patch("graphene_django.management.commands.graphql_schema.Command.save_json_file")
 def test_generate_json_file_on_call_graphql_schema(savefile_mock):
     out = StringIO()
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_converter.py` & `graphene-django-3.0.1/graphene_django/tests/test_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 
 import pytest
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from py.test import raises
+from pytest import raises
 
 import graphene
 from graphene import NonNull
 from graphene.relay import ConnectionField, Node
 from graphene.types.datetime import Date, DateTime, Time
 from graphene.types.json import JSONString
 from graphene.types.scalars import BigInt
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_fields.py` & `graphene-django-3.0.1/graphene_django/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_forms.py` & `graphene-django-3.0.1/graphene_django/tests/test_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.core.exceptions import ValidationError
-from py.test import raises
+from pytest import raises
 
 from ..forms import GlobalIDFormField, GlobalIDMultipleChoiceField
 
 
 # 'TXlUeXBlOmFiYw==' -> 'MyType', 'abc'
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_get_queryset.py` & `graphene-django-3.0.1/graphene_django/tests/test_get_queryset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_query.py` & `graphene-django-3.0.1/graphene_django/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import base64
 
 import pytest
 from django.db import models
 from django.db.models import Q
 from django.utils.functional import SimpleLazyObject
 from graphql_relay import to_global_id
-from py.test import raises
+from pytest import raises
 
 import graphene
 from graphene.relay import Node
 
 from ..compat import IntegerRangeField, MissingType
 from ..fields import DjangoConnectionField
 from ..types import DjangoObjectType
@@ -1147,17 +1147,17 @@
     expected = {"allReporters": {"edges": []}}
     assert not result.errors
     assert result.data == expected
 
 
 REPORTERS = [
     dict(
-        first_name="First {}".format(i),
-        last_name="Last {}".format(i),
-        email="johndoe+{}@example.com".format(i),
+        first_name=f"First {i}",
+        last_name=f"Last {i}",
+        email=f"johndoe+{i}@example.com",
         a_choice=1,
     )
     for i in range(6)
 ]
 
 
 def test_should_return_max_limit(graphene_settings):
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_schema.py` & `graphene-django-3.0.1/graphene_django/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from py.test import raises
+from pytest import raises
 
 from ..registry import Registry
 from ..types import DjangoObjectType
 from .models import Reporter
 
 
 def test_should_raise_if_no_model():
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_types.py` & `graphene-django-3.0.1/graphene_django/tests/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict, defaultdict
 from textwrap import dedent
 
 import pytest
 from django.db import models
-from mock import patch
+from unittest.mock import patch
 
 from graphene import Connection, Field, Interface, ObjectType, Schema, String
 from graphene.relay import Node
 
 from .. import registry
 from ..filter import DjangoFilterConnectionField
 from ..types import DjangoObjectType, DjangoObjectTypeOptions
@@ -100,15 +100,15 @@
     class ArticleType(DjangoObjectType):
         class Meta:
             abstract = True
 
         @classmethod
         def __init_subclass_with_meta__(cls, **options):
             options.setdefault("_meta", ArticleTypeOptions(cls))
-            super(ArticleType, cls).__init_subclass_with_meta__(**options)
+            super().__init_subclass_with_meta__(**options)
 
     class Article(ArticleType):
         class Meta:
             model = ArticleModel
             fields = "__all__"
 
     assert isinstance(Article._meta, ArticleTypeOptions)
@@ -480,15 +480,15 @@
                 model = ReporterModel
                 exclude = ["email"]
 
     assert len(record) == 0
 
 
 def custom_enum_name(field):
-    return "CustomEnum{}".format(field.name.title())
+    return f"CustomEnum{field.name.title()}"
 
 
 class TestDjangoObjectType:
     @pytest.fixture
     def PetModel(self):
         class PetModel(models.Model):
             kind = models.CharField(choices=(("cat", "Cat"), ("dog", "Dog")))
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_utils.py` & `graphene-django-3.0.1/graphene_django/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 
 import pytest
 from django.utils.translation import gettext_lazy
-from mock import patch
+from unittest.mock import patch
 
 from ..utils import camelize, get_model_fields, GraphQLTestCase
 from .models import Film, Reporter
 from ..utils.testing import graphql_query
 
 
 def test_get_model_fields_no_duplication():
     reporter_fields = get_model_fields(Reporter)
-    reporter_name_set = set([field[0] for field in reporter_fields])
+    reporter_name_set = {field[0] for field in reporter_fields}
     assert len(reporter_fields) == len(reporter_name_set)
 
     film_fields = get_model_fields(Film)
-    film_name_set = set([field[0] for field in film_fields])
+    film_name_set = {field[0] for field in film_fields}
     assert len(film_fields) == len(film_name_set)
 
 
 def test_camelize():
     assert camelize({}) == {}
     assert camelize("value_a") == "value_a"
     assert camelize({"value_a": "value_b"}) == {"valueA": "value_b"}
@@ -50,27 +50,27 @@
         def runTest(self):
             pass
 
     tc = TestClass()
     tc._pre_setup()
     tc.setUpClass()
     tc.query("query { }", operation_name="QueryName")
-    body = json.loads(post_mock.call_args.args[1])
+    body = json.loads(post_mock.call_args[0][1])
     # `operationName` field from https://graphql.org/learn/serving-over-http/#post-request
     assert (
         "operationName",
         "QueryName",
     ) in body.items(), "Field 'operationName' is not present in the final request."
 
 
 @pytest.mark.django_db
 @patch("graphene_django.utils.testing.Client.post")
 def test_graphql_query_case_operation_name(post_mock):
     graphql_query("query { }", operation_name="QueryName")
-    body = json.loads(post_mock.call_args.args[1])
+    body = json.loads(post_mock.call_args[0][1])
     # `operationName` field from https://graphql.org/learn/serving-over-http/#post-request
     assert (
         "operationName",
         "QueryName",
     ) in body.items(), "Field 'operationName' is not present in the final request."
```

### Comparing `graphene-django-3.0.0b9/graphene_django/tests/test_views.py` & `graphene-django-3.0.1/graphene_django/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
 
-from mock import patch
+from unittest.mock import patch
 
 from django.db import connection
 
 from graphene_django.settings import graphene_settings
 
 from .models import Pet
 
@@ -503,15 +503,15 @@
     assert response_json(response) == {
         "errors": [{"message": "POST body sent invalid JSON."}]
     }
 
 
 def test_handles_django_request_error(client, monkeypatch):
     def mocked_read(*args):
-        raise IOError("foo-bar")
+        raise OSError("foo-bar")
 
     monkeypatch.setattr("django.http.request.HttpRequest.read", mocked_read)
 
     valid_json = json.dumps(dict(foo="bar"))
     response = client.post(url_string(), valid_json, "application/json")
 
     assert response.status_code == 400
```

### Comparing `graphene-django-3.0.0b9/graphene_django/types.py` & `graphene-django-3.0.1/graphene_django/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,18 +164,16 @@
         ).format(cls.__name__, registry)
 
         if filter_fields and filterset_class:
             raise Exception("Can't set both filter_fields and filterset_class")
 
         if not DJANGO_FILTER_INSTALLED and (filter_fields or filterset_class):
             raise Exception(
-                (
-                    "Can only set filter_fields or filterset_class if "
-                    "Django-Filter is installed"
-                )
+                "Can only set filter_fields or filterset_class if "
+                "Django-Filter is installed"
             )
 
         assert not (fields and exclude), (
             "Cannot set both 'fields' and 'exclude' options on "
             "DjangoObjectType {class_name}.".format(class_name=cls.__name__)
         )
 
@@ -224,15 +222,15 @@
         django_fields = yank_fields_from_attrs(
             construct_fields(model, registry, fields, exclude, convert_choices_to_enum),
             _as=graphene.Field,
         )
 
         if use_connection is None and interfaces:
             use_connection = any(
-                (issubclass(interface, Node) for interface in interfaces)
+                issubclass(interface, Node) for interface in interfaces
             )
 
         if use_connection and not connection:
             # We create the connection automatically
             if not connection_class:
                 connection_class = Connection
 
@@ -251,15 +249,15 @@
         _meta.model = model
         _meta.registry = registry
         _meta.filter_fields = filter_fields
         _meta.filterset_class = filterset_class
         _meta.fields = django_fields
         _meta.connection = connection
 
-        super(DjangoObjectType, cls).__init_subclass_with_meta__(
+        super().__init_subclass_with_meta__(
             _meta=_meta, interfaces=interfaces, **options
         )
 
         # Validate fields
         validate_fields(cls, model, _meta.fields, fields, exclude)
 
         if not skip_registry:
```

### Comparing `graphene-django-3.0.0b9/graphene_django/utils/testing.py` & `graphene-django-3.0.1/graphene_django/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import warnings
 
 from django.test import Client, TestCase, TransactionTestCase
 
+from graphene_django.settings import graphene_settings
+
 DEFAULT_GRAPHQL_URL = "/graphql"
 
 
 def graphql_query(
     query,
     operation_name=None,
     input_data=None,
@@ -36,15 +38,15 @@
 
     Returns:
         Response object from client
     """
     if client is None:
         client = Client()
     if not graphql_url:
-        graphql_url = DEFAULT_GRAPHQL_URL
+        graphql_url = graphene_settings.TESTING_ENDPOINT
 
     body = {"query": query}
     if operation_name:
         body["operationName"] = operation_name
     if variables:
         body["variables"] = variables
     if input_data:
@@ -59,21 +61,21 @@
     else:
         resp = client.post(
             graphql_url, json.dumps(body), content_type="application/json"
         )
     return resp
 
 
-class GraphQLTestMixin(object):
+class GraphQLTestMixin:
     """
     Based on: https://www.sam.today/blog/testing-graphql-with-graphene-django/
     """
 
     # URL to graphql endpoint
-    GRAPHQL_URL = DEFAULT_GRAPHQL_URL
+    GRAPHQL_URL = graphene_settings.TESTING_ENDPOINT
 
     def query(
         self, query, operation_name=None, input_data=None, variables=None, headers=None
     ):
         """
         Args:
             query (string)    - GraphQL query to run
```

### Comparing `graphene-django-3.0.0b9/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.0.1/graphene_django/utils/tests/test_testing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from .. import GraphQLTestCase
 from ...tests.test_types import with_local_registry
+from ...settings import graphene_settings
 from django.test import Client
 
 
 @with_local_registry
 def test_graphql_test_case_deprecated_client_getter():
     """
     `GraphQLTestCase._client`' getter should raise pending deprecation warning.
@@ -39,7 +40,15 @@
 
     tc = TestClass()
     tc._pre_setup()
     tc.setUpClass()
 
     with pytest.warns(PendingDeprecationWarning):
         tc._client = Client()
+
+
+def test_graphql_test_case_imports_endpoint():
+    """
+    GraphQLTestCase class should import the default endpoint from settings file
+    """
+
+    assert GraphQLTestCase.GRAPHQL_URL == graphene_settings.TESTING_ENDPOINT
```

### Comparing `graphene-django-3.0.0b9/graphene_django/utils/utils.py` & `graphene-django-3.0.1/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/graphene_django/views.py` & `graphene-django-3.0.1/graphene_django/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .settings import graphene_settings
 
 
 class HttpError(Exception):
     def __init__(self, response, message=None, *args, **kwargs):
         self.response = response
         self.message = message = message or response.content.decode()
-        super(HttpError, self).__init__(message, *args, **kwargs)
+        super().__init__(message, *args, **kwargs)
 
 
 def get_accepted_content_types(request):
     def qualify(x):
         parts = x.split(";", 1)
         if len(parts) == 2:
             match = re.match(r"(^|;)q=(0(\.\d{,3})?|1(\.0{,3})?)(;|$)", parts[1])
@@ -62,22 +62,22 @@
 
     # React and ReactDOM.
     react_version = "17.0.2"
     react_sri = "sha256-Ipu/TQ50iCCVZBUsZyNJfxrDk0E2yhaEIz0vqI+kFG8="
     react_dom_sri = "sha256-nbMykgB6tsOFJ7OdVmPpdqMFVk4ZsqWocT6issAPUF0="
 
     # The GraphiQL React app.
-    graphiql_version = "1.4.1"  # "1.0.3"
-    graphiql_sri = "sha256-JUMkXBQWZMfJ7fGEsTXalxVA10lzKOS9loXdLjwZKi4="  # "sha256-VR4buIDY9ZXSyCNFHFNik6uSe0MhigCzgN4u7moCOTk="
-    graphiql_css_sri = "sha256-Md3vdR7PDzWyo/aGfsFVF4tvS5/eAUWuIsg9QHUusCY="  # "sha256-LwqxjyZgqXDYbpxQJ5zLQeNcf7WVNSJ+r8yp2rnWE/E="
+    graphiql_version = "2.4.1"  # "1.0.3"
+    graphiql_sri = "sha256-s+f7CFAPSUIygFnRC2nfoiEKd3liCUy+snSdYFAoLUc="  # "sha256-VR4buIDY9ZXSyCNFHFNik6uSe0MhigCzgN4u7moCOTk="
+    graphiql_css_sri = "sha256-88yn8FJMyGboGs4Bj+Pbb3kWOWXo7jmb+XCRHE+282k="  # "sha256-LwqxjyZgqXDYbpxQJ5zLQeNcf7WVNSJ+r8yp2rnWE/E="
 
     # The websocket transport library for subscriptions.
-    subscriptions_transport_ws_version = "0.9.18"
+    subscriptions_transport_ws_version = "5.12.1"
     subscriptions_transport_ws_sri = (
-        "sha256-i0hAXd4PdJ/cHX3/8tIy/Q/qKiWr5WSTxMFuL9tACkw="
+        "sha256-EZhvg6ANJrBsgLvLAa0uuHNLepLJVCFYS+xlb5U/bqw="
     )
 
     schema = None
     graphiql = False
     middleware = None
     root_value = None
     pretty = False
```

### Comparing `graphene-django-3.0.0b9/graphene_django.egg-info/PKG-INFO` & `graphene-django-3.0.1/graphene_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.0.0b9
+Version: 3.0.1
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
```

### Comparing `graphene-django-3.0.0b9/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.0.1/graphene_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.0b9/setup.cfg` & `graphene-django-3.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [aliases]
 test = pytest
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
-exclude = docs,graphene_django/debug/sql/*,migrations
+exclude = docs,graphene_django/debug/sql/*
 max-line-length = 120
 select = 
 	F601,
 	F632,
 	F811,
 	F821,
 	F822,
```

### Comparing `graphene-django-3.0.0b9/setup.py` & `graphene-django-3.0.1/setup.py`

 * *Files identical despite different names*

