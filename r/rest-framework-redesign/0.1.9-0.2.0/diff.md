# Comparing `tmp/rest_framework_redesign-0.1.9.tar.gz` & `tmp/rest_framework_redesign-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.9.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.2.0.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.9.tar` & `rest_framework_redesign-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.9/LICENSE
--rw-r--r--   0        0        0      618 2023-04-24 10:13:18.845427 rest_framework_redesign-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.9/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.9/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.9/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.9/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.9/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    23116 2023-04-24 06:12:40.271460 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     3741 2023-04-24 06:13:07.927873 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.9/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.9/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.2.0/LICENSE
+-rw-r--r--   0        0        0      618 2023-04-29 18:14:43.682039 rest_framework_redesign-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.2.0/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.2.0/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.2.0/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.2.0/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.2.0/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    23068 2023-04-29 07:11:26.577366 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     3741 2023-04-24 06:13:07.927873 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1638 2023-04-29 07:10:39.778473 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      737 2023-04-29 07:10:32.794493 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.2.0/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.2.0/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rest_framework_redesign-0.2.0/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.9/LICENSE` & `rest_framework_redesign-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/pyproject.toml` & `rest_framework_redesign-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.9"
+version = "0.2.0"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.9/README.md` & `rest_framework_redesign-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -151,24 +151,22 @@
         <h1 class="display-4">{{ name }}</h1>
       </div>
       <div class="lead">
         {% block description %}
           {{ description }}
         {% endblock %}
       </div>
-
-      {% if paginator %}
-        <nav style="float: right">
-          {% get_pagination_html paginator %}
-        </nav>
-      {% endif %}
     </section>
 
     {% block request_forms %}
       <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
+        {% if paginator %}
+          {% get_pagination_html paginator %}
+        {% endif %}
+
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
                 <div class="btn-group w-100" role="group">
                   <a class="btn btn-lg btn-primary w-100" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource">
```

#### html2text {}

```diff
@@ -25,16 +25,16 @@
    4. {{_breadcrumb_name_}}
    5. {% endif %} {% empty %} {% block breadcrumbs_empty %} {% endblock
       breadcrumbs_empty %} {% endfor %}
 {% endblock %} {% block content %}
  %}">
 ****** {{ name }} ******
 {% block description %} {{ description }} {% endblock %}
-{% if paginator %}  {% get_pagination_html paginator %}  {% endif %}  {% block
-request_forms %}  {% if 'GET' in allowed_methods %}
+ {% block request_forms %}  {% if paginator %} {% get_pagination_html paginator
+%} {% endif %} {% if 'GET' in allowed_methods %}
  {% if api_settings.URL_FORMAT_OVERRIDE %}
  {%_translate_"GET"_%}
 
     * * {% translate 'Select a format' %} *
     * {% for format in available_formats %}
     * {{_format_}}
     * {% endfor %}
```

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-<div class="mb-4">
-  <nav aria-label="Pagination">
-    <ol class="pagination">
-      {% if previous_url %}
-        <li class="page-item">
-          <a class="page-link" href="{{ previous_url }}" aria-label="Previous">
-            <span aria-hidden="true">&laquo;</span>
-          </a>
-        </li>
-      {% else %}
+<nav aria-label="Pagination" class="d-flex align-items-center">
+  <ol class="pagination flex-wrap gap-3 mb-0">
+    {% if previous_url %}
+      <li class="page-item">
+        <a class="page-link" href="{{ previous_url }}" aria-label="Previous">
+          <span aria-hidden="true">&laquo;</span>
+        </a>
+      </li>
+    {% else %}
+      <li class="page-item disabled">
+        <a class="page-link" href="#" aria-label="Previous">
+          <span aria-hidden="true">&laquo;</span>
+        </a>
+      </li>
+    {% endif %}
+
+    {% for page_link in page_links %}
+      {% if page_link.is_break %}
         <li class="page-item disabled">
-          <a class="page-link" href="#" aria-label="Previous">
-            <span aria-hidden="true">&laquo;</span>
+          <a class="page-link" href="#">
+            <span aria-hidden="true">&hellip;</span>
           </a>
         </li>
-      {% endif %}
-
-      {% for page_link in page_links %}
-        {% if page_link.is_break %}
-          <li class="page-item disabled">
-            <a class="page-link" href="#">
-              <span aria-hidden="true">&hellip;</span>
+      {% else %}
+        {% if page_link.is_active %}
+          <li class="page-item active" aria-current="page">
+            <a class="page-link" href="{{ page_link.url }}">
+              {{ page_link.number }}
             </a>
           </li>
         {% else %}
-          {% if page_link.is_active %}
-            <li class="page-item active" aria-current="page">
-              <a class="page-link" href="{{ page_link.url }}">
-                {{ page_link.number }}
-              </a>
-            </li>
-          {% else %}
-            <li class="page-item">
-              <a class="page-link" href="{{ page_link.url }}">
-                {{ page_link.number }}
-              </a>
-            </li>
-          {% endif %}
+          <li class="page-item">
+            <a class="page-link" href="{{ page_link.url }}">
+              {{ page_link.number }}
+            </a>
+          </li>
         {% endif %}
-      {% endfor %}
-
-      {% if next_url %}
-        <li class="page-item">
-          <a class="page-link" href="{{ next_url }}" aria-label="Next">
-            <span aria-hidden="true">&raquo;</span>
-          </a>
-        </li>
-      {% else %}
-        <li class="page-item disabled">
-          <a href="#" aria-label="Next">
-            <span aria-hidden="true">&raquo;</span>
-          </a>
-        </li>
       {% endif %}
-    </ol>
-  </nav>
-</div>
+    {% endfor %}
+
+    {% if next_url %}
+      <li class="page-item">
+        <a class="page-link" href="{{ next_url }}" aria-label="Next">
+          <span aria-hidden="true">&raquo;</span>
+        </a>
+      </li>
+    {% else %}
+      <li class="page-item disabled">
+        <a href="#" aria-label="Next">
+          <span aria-hidden="true">&raquo;</span>
+        </a>
+      </li>
+    {% endif %}
+  </ol>
+</nav>
```

#### html2text {}

```diff
@@ -9,7 +9,8 @@
    9. {% else %}
   10. {{_page_link.number_}}
   11. {% endif %} {% endif %} {% endfor %} {% if next_url %}
   12. »
   13. {% else %}
   14. »
   15. {% endif %}
+
```

### Comparing `rest_framework_redesign-0.1.9/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.2.0/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<nav aria-label="Pagination">
-  <ol class="pagination flex-wrap">
+<nav aria-label="Pagination" class="d-flex align-items-center">
+  <ol class="pagination flex-wrap gap-3 mb-0">
     {% if previous_url %}
       <li class="page-item">
         <a href="{{ previous_url }}" class="page-link">
           &laquo; Previous
         </a>
       </li>
     {% else %}
```

### Comparing `rest_framework_redesign-0.1.9/PKG-INFO` & `rest_framework_redesign-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.9
+Version: 0.2.0
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

