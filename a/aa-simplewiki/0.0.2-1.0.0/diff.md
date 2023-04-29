# Comparing `tmp/aa-simplewiki-0.0.2.tar.gz` & `tmp/aa-simplewiki-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-simplewiki-0.0.2.tar", last modified: Mon Apr 24 15:48:46 2023, max compression
+gzip compressed data, was "aa-simplewiki-1.0.0.tar", last modified: Sat Apr 29 20:16:46 2023, max compression
```

## Comparing `aa-simplewiki-0.0.2.tar` & `aa-simplewiki-1.0.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/LICENSE
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/MANIFEST.in
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5500 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4467 2023-04-24 15:47:03.000000 aa-simplewiki-0.0.2/README.md
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5500 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/PKG-INFO
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/SOURCES.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/dependency_links.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-24 14:24:55.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/not-zip-safe
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/requires.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-04-24 15:48:46.000000 aa-simplewiki-0.0.2/aa_simplewiki.egg-info/top_level.txt
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/pyproject.toml
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/setup.cfg
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1200 2023-04-24 14:46:01.000000 aa-simplewiki-0.0.2/setup.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       48 2023-04-24 15:48:37.000000 aa-simplewiki-0.0.2/simplewiki/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-04-23 21:25:21.000000 aa-simplewiki-0.0.2/simplewiki/admin.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11877 2023-04-24 14:48:20.000000 aa-simplewiki-0.0.2/simplewiki/admin_helper_menus.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-04-22 07:13:40.000000 aa-simplewiki-0.0.2/simplewiki/admin_helper_sections.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/app_settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/apps.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/auth_hooks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/migrations/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0001_initial.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0002_pageitem_page_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0003_menuitem_icon.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0010_rename_path_menuitem_name.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0011_rename_name_menuitem_path.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0012_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0013_alter_menuitem_group.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0018_rename_group_menuitem_groups.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0019_alter_general_options.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/0020_menuitem_parent.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/migrations/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-04-21 10:07:09.000000 aa-simplewiki-0.0.2/simplewiki/models.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/static/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/.gitkeep
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/static/simplewiki/custom.css
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tasks.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.102739 aa-simplewiki-0.0.2/simplewiki/templates/
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-04-23 09:54:06.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/base.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-23 21:22:31.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/dynamic_page.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6552 2023-04-23 09:56:49.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-04-23 18:31:44.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2311 2023-04-21 16:05:35.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2345 2023-04-21 16:06:22.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/error.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/index.html
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-04-22 13:52:24.000000 aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/search.html
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/templatetags/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2121 2023-04-23 21:22:45.000000 aa-simplewiki-0.0.2/simplewiki/templatetags/custom_filters.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/templatetags/markdown_filters.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/simplewiki/tests/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tests/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/simplewiki/tests/test_example.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-04-21 10:07:44.000000 aa-simplewiki-0.0.2/simplewiki/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12689 2023-04-22 13:58:33.000000 aa-simplewiki-0.0.2/simplewiki/views.py
-drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-24 15:48:46.106740 aa-simplewiki-0.0.2/testauth/
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/__init__.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/celery.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/settings.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/urls.py
--rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-04-21 07:42:53.000000 aa-simplewiki-0.0.2/testauth/wsgi.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    35164 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/LICENSE
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      123 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/MANIFEST.in
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4701 2023-04-29 20:02:43.000000 aa-simplewiki-1.0.0/README.md
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.033726 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     5719 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/PKG-INFO
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2607 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        1 2023-04-29 20:14:32.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/not-zip-safe
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       24 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/requires.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       20 2023-04-29 20:16:46.000000 aa-simplewiki-1.0.0/aa_simplewiki.egg-info/top_level.txt
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      104 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/pyproject.toml
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1462 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/setup.cfg
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1205 2023-04-29 20:16:39.000000 aa-simplewiki-1.0.0/setup.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.033726 aa-simplewiki-1.0.0/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       48 2023-04-29 20:15:23.000000 aa-simplewiki-1.0.0/simplewiki/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      231 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    11877 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin_helper_menus.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     8956 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/admin_helper_sections.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      169 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/app_settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      284 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/apps.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/auth_hooks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/migrations/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1489 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0001_initial.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      395 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0002_pageitem_page_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      401 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0003_menuitem_icon.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1532 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1522 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      374 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0006_rename_pageitem_sectionitem.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      392 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0007_rename_page_title_sectionitem_section_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1657 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      658 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      381 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0010_rename_path_menuitem_name.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      372 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0011_rename_name_menuitem_path.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      576 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0012_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      579 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0013_alter_menuitem_group.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     3030 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      685 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0016_rename_section_title_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      831 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      399 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0018_rename_group_menuitem_groups.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      492 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0019_alter_general_options.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      538 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/0020_menuitem_parent.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/migrations/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     4236 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/models.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.029726 aa-simplewiki-1.0.0/simplewiki/static/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)        0 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/.gitkeep
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      199 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/static/simplewiki/custom.css
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      226 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tasks.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.029726 aa-simplewiki-1.0.0/simplewiki/templates/
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6324 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/base.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1076 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/dynamic_page.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     6552 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_menus.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9500 2023-04-29 19:49:06.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_sections.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2311 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_create_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2345 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      593 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/error.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      460 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/index.html
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     1578 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/search.html
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/templatetags/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     2121 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templatetags/custom_filters.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      407 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/templatetags/markdown_filters.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/simplewiki/tests/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       27 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tests/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      448 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/tests/test_example.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      488 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/simplewiki/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)    12689 2023-04-29 20:15:58.000000 aa-simplewiki-1.0.0/simplewiki/views.py
+drwxrwxr-x   0 sonnen    (1000) sonnen    (1000)        0 2023-04-29 20:16:46.037726 aa-simplewiki-1.0.0/testauth/
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)       52 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/__init__.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      654 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/celery.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)     9481 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/settings.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      167 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/urls.py
+-rw-rw-r--   0 sonnen    (1000) sonnen    (1000)      425 2023-04-25 22:42:57.000000 aa-simplewiki-1.0.0/testauth/wsgi.py
```

### Comparing `aa-simplewiki-0.0.2/LICENSE` & `aa-simplewiki-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/PKG-INFO` & `aa-simplewiki-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 0.0.2
-Summary: Alliance Auth Plugin
+Version: 1.0.0
+Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-simplewiki-plugin/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-simplewiki-plugin/blob/master/CHANGELOG.md
 Keywords: allianceauth,simplewiki
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -70,15 +69,15 @@
   * French
   * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
-![Showcase](https://i.imgur.com/vST5An1.png)
+![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
 ![Menu Admin](https://i.imgur.com/VGssV4d.png)
 
@@ -119,14 +118,16 @@
 
 1.) Download the repo `git clone https://github.com/meowosaurus/aa-simplewiki`
 
 2.) Make sure it's under the root folder `aa-dev`, not under `myauth` 
 
 3.) Change directory into `aa-dev` aand run `pip install -e aa-simplewiki`
 
+**Important**: If you are getting an error saying that `simplewiki` is not installed after running `pip install -e aa-simplewiki`, delete the `setup.py` file in the aa-simplewiki root directory and try again.
+
 4.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 5.) Change directory into `myauth`
 
 6.) Make migrations with `python manage.py makemigrations`
 
 7.) Migrate with `python manage.py migrate`
@@ -150,9 +151,7 @@
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
 ## Support
 * On Discord: Meowlicious#7045
-
-
```

### Comparing `aa-simplewiki-0.0.2/README.md` & `aa-simplewiki-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   * French
   * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
-![Showcase](https://i.imgur.com/vST5An1.png)
+![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
 ![Menu Admin](https://i.imgur.com/VGssV4d.png)
 
@@ -93,14 +93,16 @@
 
 1.) Download the repo `git clone https://github.com/meowosaurus/aa-simplewiki`
 
 2.) Make sure it's under the root folder `aa-dev`, not under `myauth` 
 
 3.) Change directory into `aa-dev` aand run `pip install -e aa-simplewiki`
 
+**Important**: If you are getting an error saying that `simplewiki` is not installed after running `pip install -e aa-simplewiki`, delete the `setup.py` file in the aa-simplewiki root directory and try again.
+
 4.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 5.) Change directory into `myauth`
 
 6.) Make migrations with `python manage.py makemigrations`
 
 7.) Migrate with `python manage.py migrate`
```

### Comparing `aa-simplewiki-0.0.2/aa_simplewiki.egg-info/PKG-INFO` & `aa-simplewiki-1.0.0/aa_simplewiki.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: aa-simplewiki
-Version: 0.0.2
-Summary: Alliance Auth Plugin
+Version: 1.0.0
+Summary: Alliance Auth Wiki Plugin
 Home-page: https://github.com/meowosaurus/aa-simplewiki
 Author: Meowosaurus
 Author-email: info@bjsonnen.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-simplewiki-plugin/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-simplewiki-plugin/blob/master/CHANGELOG.md
 Keywords: allianceauth,simplewiki
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -70,15 +69,15 @@
   * French
   * Italian
 
 ### Active devs:
 * [Meowosaurus](https://github.com/meowosaurus)
 
 ## Screenshots
-![Showcase](https://i.imgur.com/vST5An1.png)
+![Showcase](https://i.postimg.cc/BQc3hPYb/vmplayer-Kvz8-DNZa-M0.gif)
 
 ### Search
 ![Search](https://i.imgur.com/wW69LFN.png)
 
 ### Admin Panel
 ![Menu Admin](https://i.imgur.com/VGssV4d.png)
 
@@ -119,14 +118,16 @@
 
 1.) Download the repo `git clone https://github.com/meowosaurus/aa-simplewiki`
 
 2.) Make sure it's under the root folder `aa-dev`, not under `myauth` 
 
 3.) Change directory into `aa-dev` aand run `pip install -e aa-simplewiki`
 
+**Important**: If you are getting an error saying that `simplewiki` is not installed after running `pip install -e aa-simplewiki`, delete the `setup.py` file in the aa-simplewiki root directory and try again.
+
 4.) Add `simplewiki` to your `INSTALLED_APPS` in your projects `local.py`
 
 5.) Change directory into `myauth`
 
 6.) Make migrations with `python manage.py makemigrations`
 
 7.) Migrate with `python manage.py migrate`
@@ -150,9 +151,7 @@
 Perm | Admin Site | Auth Site 
  --- | --- | --- 
 basic_access | None | Can view all wiki pages
 editor_access | None | Can create, edit and delete wiki pages and menus
 
 ## Support
 * On Discord: Meowlicious#7045
-
-
```

### Comparing `aa-simplewiki-0.0.2/aa_simplewiki.egg-info/SOURCES.txt` & `aa-simplewiki-1.0.0/aa_simplewiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/setup.cfg` & `aa-simplewiki-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/setup.py` & `aa-simplewiki-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 setup(
     name='aa-simplewiki',
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
     license='GNU General Public License v3 (GPLv3)',
-    description='Alliance Auth Plugin',
+    description='Alliance Auth Wiki Plugin',
     install_requires=install_requires,
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/meowosaurus/aa-simplewiki',
     author='Meowosaurus',
     author_email='info@bjsonnen.de',
     classifiers=[
```

### Comparing `aa-simplewiki-0.0.2/simplewiki/admin_helper_menus.py` & `aa-simplewiki-1.0.0/simplewiki/admin_helper_menus.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/admin_helper_sections.py` & `aa-simplewiki-1.0.0/simplewiki/admin_helper_sections.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/auth_hooks.py` & `aa-simplewiki-1.0.0/simplewiki/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0001_initial.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0004_pageitem_icon_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0005_alter_menuitem_icon_alter_pageitem_content_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0008_alter_general_options_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0009_remove_menuitem_name_menuitem_path.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0012_menuitem_group.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0012_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0013_alter_menuitem_group.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0013_alter_menuitem_group.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0014_alter_menuitem_group_alter_menuitem_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0015_rename_menu_name_sectionitem_menu_path_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0017_alter_sectionitem_content_alter_sectionitem_title.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/migrations/0020_menuitem_parent.py` & `aa-simplewiki-1.0.0/simplewiki/migrations/0020_menuitem_parent.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/models.py` & `aa-simplewiki-1.0.0/simplewiki/models.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/base.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/base.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/dynamic_page.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/dynamic_page.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_menus.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_menus.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/editor_sections.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/editor_sections.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_create_menu.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_create_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/editor/partials/_edit_menu.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/error.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/error.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templates/simplewiki/search.html` & `aa-simplewiki-1.0.0/simplewiki/templates/simplewiki/search.html`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/templatetags/custom_filters.py` & `aa-simplewiki-1.0.0/simplewiki/templatetags/custom_filters.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/simplewiki/views.py` & `aa-simplewiki-1.0.0/simplewiki/views.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/testauth/celery.py` & `aa-simplewiki-1.0.0/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-simplewiki-0.0.2/testauth/settings.py` & `aa-simplewiki-1.0.0/testauth/settings.py`

 * *Files identical despite different names*

