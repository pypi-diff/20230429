# Comparing `tmp/django-medicio_ds-1.1.0.tar.gz` & `tmp/django-medicio_ds-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-medicio_ds-1.1.0.tar", last modified: Tue Feb  7 06:15:16 2023, max compression
+gzip compressed data, was "django-medicio_ds-1.2.0.tar", last modified: Sat Apr 29 03:41:33 2023, max compression
```

## Comparing `django-medicio_ds-1.1.0.tar` & `django-medicio_ds-1.2.0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.450340 django-medicio_ds-1.1.0/
--rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:36.000000 django-medicio_ds-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      270 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2795 2023-02-07 06:15:16.450340 django-medicio_ds-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2293 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.178826 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/
--rw-rw-rw-   0        0        0     2795 2023-02-07 06:15:16.000000 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9756 2023-02-07 06:15:16.000000 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 06:15:16.000000 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-02-07 06:15:16.000000 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-07 06:15:16.000000 django-medicio_ds-1.1.0/django_medicio_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.189333 django-medicio_ds-1.1.0/medicio/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/__init__.py
--rw-rw-rw-   0        0        0       66 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/admin.py
--rw-rw-rw-   0        0        0      152 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/apps.py
--rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/forms.py
--rw-rw-rw-   0        0        0       60 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/models.py
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.135741 django-medicio_ds-1.1.0/medicio/static/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.138742 django-medicio_ds-1.1.0/medicio/static/medicio/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.204336 django-medicio_ds-1.1.0/medicio/static/medicio/img/
--rw-rw-rw-   0        0        0    87275 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/about.jpg
--rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0    64859 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-1.jpg
--rw-rw-rw-   0        0        0    48057 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-2.jpg
--rw-rw-rw-   0        0        0    58282 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-3.jpg
--rw-rw-rw-   0        0        0    56173 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-4.jpg
--rw-rw-rw-   0        0        0    26888 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-5.jpg
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.211322 django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/
--rw-rw-rw-   0        0        0    28289 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-1.jpg
--rw-rw-rw-   0        0        0    24589 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-2.jpg
--rw-rw-rw-   0        0        0    26594 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-3.jpg
--rw-rw-rw-   0        0        0    30658 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-4.jpg
--rw-rw-rw-   0        0        0      491 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/favicon.png
--rw-rw-rw-   0        0        0    58416 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/features.jpg
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.223375 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/
--rw-rw-rw-   0        0        0    87051 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-1.jpg
--rw-rw-rw-   0        0        0    52988 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-2.jpg
--rw-rw-rw-   0        0        0    67200 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-3.jpg
--rw-rw-rw-   0        0        0   115379 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-4.jpg
--rw-rw-rw-   0        0        0    58795 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-5.jpg
--rw-rw-rw-   0        0        0    59213 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-6.jpg
--rw-rw-rw-   0        0        0    97603 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-7.jpg
--rw-rw-rw-   0        0        0   113565 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-8.jpg
--rw-rw-rw-   0        0        0     6762 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/logo.png
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.228409 django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/
--rw-rw-rw-   0        0        0   253128 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-1.jpg
--rw-rw-rw-   0        0        0   137686 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-2.jpg
--rw-rw-rw-   0        0        0   195419 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-3.jpg
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.236430 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/
--rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-1.jpg
--rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-2.jpg
--rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-3.jpg
--rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-4.jpg
--rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-5.jpg
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.238058 django-medicio_ds-1.1.0/medicio/static/medicio/js/
--rw-rw-rw-   0        0        0     6560 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/js/main.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.249586 django-medicio_ds-1.1.0/medicio/static/medicio/scss/
--rw-rw-rw-   0        0        0     3011 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_footer.scss
--rw-rw-rw-   0        0        0     2001 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_general.scss
--rw-rw-rw-   0        0        0     1504 2023-02-07 05:35:11.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_header.scss
--rw-rw-rw-   0        0        0     3301 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_hero.scss
--rw-rw-rw-   0        0        0     3669 2022-12-08 08:45:17.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_nav.scss
--rw-rw-rw-   0        0        0    20148 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_sections.scss
--rw-rw-rw-   0        0        0      497 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/_variables.scss
--rw-rw-rw-   0        0        0      136 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/scss/style.scss
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.149748 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.254348 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/
--rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.compat.css
--rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.css
--rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.min.css
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.257351 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.140742 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.323026 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:37.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.345165 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.263353 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.267310 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/index.html
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.141742 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.350567 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/
--rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/animations.css
--rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/boxicons.css
--rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/boxicons.min.css
--rw-rw-rw-   0        0        0      683 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/transformations.css
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.361216 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/
--rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.eot
--rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.svg
--rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.ttf
--rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff
--rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff2
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.142742 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.387883 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/
--rw-rw-rw-   0        0        0   137917 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/all.css
--rw-rw-rw-   0        0        0   100782 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/all.min.css
--rw-rw-rw-   0        0        0    22257 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.css
--rw-rw-rw-   0        0        0    17821 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.min.css
--rw-rw-rw-   0        0        0   112809 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.css
--rw-rw-rw-   0        0        0    80388 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.min.css
--rw-rw-rw-   0        0        0      619 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.css
--rw-rw-rw-   0        0        0      566 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.min.css
--rw-rw-rw-   0        0        0      611 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.css
--rw-rw-rw-   0        0        0      558 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.min.css
--rw-rw-rw-   0        0        0    21336 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.css
--rw-rw-rw-   0        0        0    16699 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.min.css
--rw-rw-rw-   0        0        0     1845 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.css
--rw-rw-rw-   0        0        0     1750 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.min.css
--rw-rw-rw-   0        0        0    40712 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.css
--rw-rw-rw-   0        0        0    26235 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.min.css
--rw-rw-rw-   0        0        0      871 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.css
--rw-rw-rw-   0        0        0      794 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.min.css
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.401328 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/
--rw-rw-rw-   0        0        0   181852 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0   105536 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    60520 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    23940 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   388460 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   154228 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-rw-rw-   0        0        0    10556 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
--rw-rw-rw-   0        0        0     4960 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.149243 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.408217 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/
--rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/glightbox.css
--rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/glightbox.min.css
--rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/plyr.css
--rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/plyr.min.css
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.410818 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/js/
--rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/js/glightbox.js
--rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/js/glightbox.min.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.414193 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.416381 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/purecounter/
--rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/purecounter/purecounter.js
--rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/purecounter/purecounter_vanilla.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.419756 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/swiper/
--rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.js
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.150753 django-medicio_ds-1.1.0/medicio/templates/
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.446485 django-medicio_ds-1.1.0/medicio/templates/medicio/
--rw-rw-rw-   0        0        0     2869 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/__pricing.html
--rw-rw-rw-   0        0        0     1059 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_about.html
--rw-rw-rw-   0        0        0     1643 2023-02-07 06:05:57.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_appointment.html
--rw-rw-rw-   0        0        0     4213 2023-02-07 06:07:16.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_contact.html
--rw-rw-rw-   0        0        0      695 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_counts.html
--rw-rw-rw-   0        0        0      670 2023-02-07 06:02:36.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_cta.html
--rw-rw-rw-   0        0        0     1753 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_departments.html
--rw-rw-rw-   0        0        0     3232 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_doctors.html
--rw-rw-rw-   0        0        0      818 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_faq.html
--rw-rw-rw-   0        0        0      847 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_features.html
--rw-rw-rw-   0        0        0      778 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_gallery.html
--rw-rw-rw-   0        0        0     1475 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_hero.html
--rw-rw-rw-   0        0        0     2869 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_pricing.html
--rw-rw-rw-   0        0        0     1424 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_services.html
--rw-rw-rw-   0        0        0     4156 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_testimonials.html
--rw-rw-rw-   0        0        0     1160 2022-12-08 08:45:17.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/_why_us.html
--rw-rw-rw-   0        0        0     1688 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/footer.html
--rw-rw-rw-   0        0        0     1955 2023-02-07 06:14:49.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/header.html
--rw-rw-rw-   0        0        0     4780 2022-12-21 07:32:32.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/index.html
--rw-rw-rw-   0        0        0     1488 2023-02-07 05:17:27.000000 django-medicio_ds-1.1.0/medicio/templates/medicio/seo.html
-drwxrwxrwx   0        0        0        0 2023-02-07 06:15:16.449219 django-medicio_ds-1.1.0/medicio/templatetags/
--rw-rw-rw-   0        0        0        0 2022-12-21 07:32:05.000000 django-medicio_ds-1.1.0/medicio/templatetags/__init__.py
--rw-rw-rw-   0        0        0     4756 2023-02-07 05:15:00.000000 django-medicio_ds-1.1.0/medicio/templatetags/medicio_tags.py
--rw-rw-rw-   0        0        0       63 2022-11-26 09:41:39.000000 django-medicio_ds-1.1.0/medicio/tests.py
--rw-rw-rw-   0        0        0      221 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/medicio/urls.py
--rw-rw-rw-   0        0        0     3810 2022-12-21 06:25:16.000000 django-medicio_ds-1.1.0/medicio/views.py
--rw-rw-rw-   0        0        0      112 2022-11-26 09:41:39.000000 django-medicio_ds-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      750 2023-02-07 06:15:16.452426 django-medicio_ds-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-11-26 09:41:38.000000 django-medicio_ds-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.570486 django-medicio_ds-1.2.0/
+-rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:36.000000 django-medicio_ds-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      270 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2795 2023-04-29 03:41:33.570486 django-medicio_ds-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2293 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.347292 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/
+-rw-rw-rw-   0        0        0     2795 2023-04-29 03:41:32.000000 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9756 2023-04-29 03:41:32.000000 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 03:41:32.000000 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-04-29 03:41:32.000000 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-29 03:41:32.000000 django-medicio_ds-1.2.0/django_medicio_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.407663 django-medicio_ds-1.2.0/medicio/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/admin.py
+-rw-rw-rw-   0        0        0      152 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/apps.py
+-rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/forms.py
+-rw-rw-rw-   0        0        0       60 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/models.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.314357 django-medicio_ds-1.2.0/medicio/static/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.318732 django-medicio_ds-1.2.0/medicio/static/medicio/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.466422 django-medicio_ds-1.2.0/medicio/static/medicio/img/
+-rw-rw-rw-   0        0        0    87275 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/about.jpg
+-rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0    64859 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-1.jpg
+-rw-rw-rw-   0        0        0    48057 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-2.jpg
+-rw-rw-rw-   0        0        0    58282 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-3.jpg
+-rw-rw-rw-   0        0        0    56173 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-4.jpg
+-rw-rw-rw-   0        0        0    26888 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-5.jpg
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.490180 django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/
+-rw-rw-rw-   0        0        0    28289 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-1.jpg
+-rw-rw-rw-   0        0        0    24589 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-2.jpg
+-rw-rw-rw-   0        0        0    26594 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-3.jpg
+-rw-rw-rw-   0        0        0    30658 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-4.jpg
+-rw-rw-rw-   0        0        0      491 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/favicon.png
+-rw-rw-rw-   0        0        0    58416 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/features.jpg
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.544334 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/
+-rw-rw-rw-   0        0        0    87051 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-1.jpg
+-rw-rw-rw-   0        0        0    52988 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-2.jpg
+-rw-rw-rw-   0        0        0    67200 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-3.jpg
+-rw-rw-rw-   0        0        0   115379 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-4.jpg
+-rw-rw-rw-   0        0        0    58795 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-5.jpg
+-rw-rw-rw-   0        0        0    59213 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-6.jpg
+-rw-rw-rw-   0        0        0    97603 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-7.jpg
+-rw-rw-rw-   0        0        0   113565 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-8.jpg
+-rw-rw-rw-   0        0        0     6762 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.566801 django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/
+-rw-rw-rw-   0        0        0   253128 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-1.jpg
+-rw-rw-rw-   0        0        0   137686 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-2.jpg
+-rw-rw-rw-   0        0        0   195419 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-3.jpg
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.596843 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/
+-rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-1.jpg
+-rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-2.jpg
+-rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-3.jpg
+-rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-4.jpg
+-rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-5.jpg
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.597844 django-medicio_ds-1.2.0/medicio/static/medicio/js/
+-rw-rw-rw-   0        0        0     6560 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/js/main.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.612550 django-medicio_ds-1.2.0/medicio/static/medicio/scss/
+-rw-rw-rw-   0        0        0     3011 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_footer.scss
+-rw-rw-rw-   0        0        0     2001 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_general.scss
+-rw-rw-rw-   0        0        0     1504 2023-02-07 05:35:11.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_header.scss
+-rw-rw-rw-   0        0        0     3301 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_hero.scss
+-rw-rw-rw-   0        0        0     3669 2022-12-08 08:45:17.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_nav.scss
+-rw-rw-rw-   0        0        0    20148 2023-04-29 03:37:07.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_sections.scss
+-rw-rw-rw-   0        0        0      497 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/_variables.scss
+-rw-rw-rw-   0        0        0      136 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.327339 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.633557 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/
+-rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.compat.css
+-rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.css
+-rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.min.css
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.638146 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.322301 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.999894 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:37.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.173935 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.671032 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.680395 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/index.html
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.323308 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.197909 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/
+-rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/animations.css
+-rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/boxicons.css
+-rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/boxicons.min.css
+-rw-rw-rw-   0        0        0      683 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/transformations.css
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.243993 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/
+-rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.eot
+-rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.svg
+-rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.ttf
+-rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff
+-rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff2
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.324315 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.370422 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/
+-rw-rw-rw-   0        0        0   137917 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/all.css
+-rw-rw-rw-   0        0        0   100782 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/all.min.css
+-rw-rw-rw-   0        0        0    22257 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.css
+-rw-rw-rw-   0        0        0    17821 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.min.css
+-rw-rw-rw-   0        0        0   112809 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.css
+-rw-rw-rw-   0        0        0    80388 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.min.css
+-rw-rw-rw-   0        0        0      619 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.css
+-rw-rw-rw-   0        0        0      566 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.min.css
+-rw-rw-rw-   0        0        0      611 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.css
+-rw-rw-rw-   0        0        0      558 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.min.css
+-rw-rw-rw-   0        0        0    21336 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.css
+-rw-rw-rw-   0        0        0    16699 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.min.css
+-rw-rw-rw-   0        0        0     1845 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.css
+-rw-rw-rw-   0        0        0     1750 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.min.css
+-rw-rw-rw-   0        0        0    40712 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.css
+-rw-rw-rw-   0        0        0    26235 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.min.css
+-rw-rw-rw-   0        0        0      871 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.css
+-rw-rw-rw-   0        0        0      794 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.min.css
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.421475 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/
+-rw-rw-rw-   0        0        0   181852 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0   105536 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    60520 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    23940 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   388460 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   154228 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-rw-rw-   0        0        0    10556 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
+-rw-rw-rw-   0        0        0     4960 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.325321 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.441044 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/
+-rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/glightbox.css
+-rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/glightbox.min.css
+-rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/plyr.css
+-rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/plyr.min.css
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.462525 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/js/
+-rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/js/glightbox.js
+-rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/js/glightbox.min.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.503413 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.518487 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/purecounter/
+-rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/purecounter/purecounter.js
+-rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/purecounter/purecounter_vanilla.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.522490 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/swiper/
+-rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:32.327339 django-medicio_ds-1.2.0/medicio/templates/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.555647 django-medicio_ds-1.2.0/medicio/templates/medicio/
+-rw-rw-rw-   0        0        0     2869 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/__pricing.html
+-rw-rw-rw-   0        0        0     1059 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_about.html
+-rw-rw-rw-   0        0        0     1643 2023-02-07 06:05:57.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_appointment.html
+-rw-rw-rw-   0        0        0     4213 2023-02-07 06:07:16.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_contact.html
+-rw-rw-rw-   0        0        0      695 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_counts.html
+-rw-rw-rw-   0        0        0      670 2023-02-07 06:02:36.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_cta.html
+-rw-rw-rw-   0        0        0     1753 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_departments.html
+-rw-rw-rw-   0        0        0     3232 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_doctors.html
+-rw-rw-rw-   0        0        0      818 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_faq.html
+-rw-rw-rw-   0        0        0      847 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_features.html
+-rw-rw-rw-   0        0        0      778 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_gallery.html
+-rw-rw-rw-   0        0        0     1475 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_hero.html
+-rw-rw-rw-   0        0        0     2869 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_pricing.html
+-rw-rw-rw-   0        0        0     1223 2023-04-29 03:40:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_services.html
+-rw-rw-rw-   0        0        0     4156 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_testimonials.html
+-rw-rw-rw-   0        0        0     1160 2022-12-08 08:45:17.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/_why_us.html
+-rw-rw-rw-   0        0        0     1688 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/footer.html
+-rw-rw-rw-   0        0        0     1955 2023-02-07 06:14:49.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/header.html
+-rw-rw-rw-   0        0        0     4780 2022-12-21 07:32:32.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/index.html
+-rw-rw-rw-   0        0        0     1488 2023-02-07 05:17:27.000000 django-medicio_ds-1.2.0/medicio/templates/medicio/seo.html
+drwxrwxrwx   0        0        0        0 2023-04-29 03:41:33.568486 django-medicio_ds-1.2.0/medicio/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-12-21 07:32:05.000000 django-medicio_ds-1.2.0/medicio/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     4756 2023-02-07 05:15:00.000000 django-medicio_ds-1.2.0/medicio/templatetags/medicio_tags.py
+-rw-rw-rw-   0        0        0       63 2022-11-26 09:41:39.000000 django-medicio_ds-1.2.0/medicio/tests.py
+-rw-rw-rw-   0        0        0      221 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/medicio/urls.py
+-rw-rw-rw-   0        0        0     3810 2022-12-21 06:25:16.000000 django-medicio_ds-1.2.0/medicio/views.py
+-rw-rw-rw-   0        0        0      112 2022-11-26 09:41:39.000000 django-medicio_ds-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      750 2023-04-29 03:41:33.572487 django-medicio_ds-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-11-26 09:41:38.000000 django-medicio_ds-1.2.0/setup.py
```

### Comparing `django-medicio_ds-1.1.0/LICENSE` & `django-medicio_ds-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/PKG-INFO` & `django-medicio_ds-1.2.0/django_medicio_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-medicio_ds
-Version: 1.1.0
+Name: django-medicio-ds
+Version: 1.2.0
 Summary: medicio_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-medicio_ds-1.1.0/README.md` & `django-medicio_ds-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/django_medicio_ds.egg-info/PKG-INFO` & `django-medicio_ds-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-medicio-ds
-Version: 1.1.0
+Name: django-medicio_ds
+Version: 1.2.0
 Summary: medicio_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-medicio_ds-1.1.0/django_medicio_ds.egg-info/SOURCES.txt` & `django-medicio_ds-1.2.0/django_medicio_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/forms.py` & `django-medicio_ds-1.2.0/medicio/forms.py`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/about.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/about.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/apple-touch-icon.png` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-1.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-2.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-3.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-4.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/departments-5.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/departments-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-1.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-2.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-3.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/doctors/doctors-4.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/doctors/doctors-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/features.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/features.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-1.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-2.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-3.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-4.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-5.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-6.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-6.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-7.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-7.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/gallery/gallery-8.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/gallery/gallery-8.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/logo.png` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-1.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-2.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/slide/slide-3.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/slide/slide-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-1.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-2.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-3.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-4.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/img/testimonials/testimonials-5.jpg` & `django-medicio_ds-1.2.0/medicio/static/medicio/img/testimonials/testimonials-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/js/main.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/js/main.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_footer.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_general.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_header.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_hero.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_nav.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/scss/_sections.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.compat.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/animate.css/animate.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/aos/aos.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/aos/aos.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js.map` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.json` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/bootstrap-icons/index.html` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/animations.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/boxicons.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/boxicons.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/css/transformations.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.eot` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.svg` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.ttf` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/all.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/all.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/glightbox.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/glightbox.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/plyr.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/css/plyr.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/js/glightbox.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/glightbox/js/glightbox.min.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/php-email-form/php-email-form.php` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/php-email-form/validate.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/purecounter/purecounter.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/purecounter/purecounter.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/purecounter/purecounter_vanilla.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.css` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.js` & `django-medicio_ds-1.2.0/medicio/static/medicio/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/__pricing.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/__pricing.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_about.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_about.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_appointment.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_appointment.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_contact.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_contact.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_counts.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_counts.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_cta.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_cta.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_departments.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_departments.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_doctors.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_doctors.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_faq.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_faq.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_features.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_features.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_gallery.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_gallery.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_hero.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_hero.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_pricing.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_pricing.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_services.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_services.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 {% load static %}
 
 {% block services %}
 <style>
 .services {
   .image {
-    display: inline-flex;
-    justify-content: center;
-    align-items: center;
-    width: 80px;
-    height: 80px;
-    margin-bottom: 20px;
-    background: $white;
-    border-radius: 50%;
-    transition: 0.5s;
-    color: $primary;
-    overflow: hidden;
-    box-shadow: 0px 0 25px rgba(0, 0, 0, 0.15);
+    text-align: center;
+    border: 1px solid lighten($secondary, 60);
+    transition: all ease-in-out 0.3s;
   }
 }
 </style>
 <section id="services" class="services services">
   <div class="container" data-aos="fade-up">
 
     <div class="section-title">
```

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_testimonials.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/_why_us.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/_why_us.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/footer.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/footer.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/header.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/header.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/index.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/index.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templates/medicio/seo.html` & `django-medicio_ds-1.2.0/medicio/templates/medicio/seo.html`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/templatetags/medicio_tags.py` & `django-medicio_ds-1.2.0/medicio/templatetags/medicio_tags.py`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/medicio/views.py` & `django-medicio_ds-1.2.0/medicio/views.py`

 * *Files identical despite different names*

### Comparing `django-medicio_ds-1.1.0/setup.cfg` & `django-medicio_ds-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6d65 6469 6369   = django-medici
 00000020: 6f5f 6473 0d0a 7665 7273 696f 6e20 3d20  o_ds..version = 
-00000030: 312e 312e 300d 0a61 7574 686f 7220 3d20  1.1.0..author = 
+00000030: 312e 322e 300d 0a61 7574 686f 7220 3d20  1.2.0..author = 
 00000040: 6879 756e 676a 696e 206b 696d 0d0a 6175  hyungjin kim..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2068 6a33  thor_email = hj3
 00000060: 3431 3540 676d 6169 6c2e 636f 6d0d 0a64  415@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 206d 6564  escription = med
 00000080: 6963 696f 5f70 726f 2070 6f72 7469 6e67  icio_pro porting
 00000090: 2066 6f72 2064 6a61 6e67 6f0d 0a6c 6f6e   for django..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

