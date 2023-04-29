# Comparing `tmp/bulrush-0.5.2.tar.gz` & `tmp/bulrush-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulrush-0.5.2.tar", last modified: Sun May 15 21:05:49 2022, max compression
+gzip compressed data, was "bulrush-0.6.2.tar", last modified: Sat Apr 29 14:27:15 2023, max compression
```

## Comparing `bulrush-0.5.2.tar` & `bulrush-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.360171 bulrush-0.5.2/
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      734 2022-05-15 20:22:56.000000 bulrush-0.5.2/LICENSE
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     8640 2022-05-15 21:05:49.359955 bulrush-0.5.2/PKG-INFO
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     8156 2022-05-15 20:22:56.000000 bulrush-0.5.2/README.md
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.355308 bulrush-0.5.2/bulrush/
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      675 2022-05-15 20:57:41.000000 bulrush-0.5.2/bulrush/__init__.py
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      702 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/image_extractor.py
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1460 2022-05-15 20:24:25.000000 bulrush-0.5.2/bulrush/license_generator.py
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1253 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/schema_generator.py
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.354015 bulrush-0.5.2/bulrush/static/
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.356218 bulrush-0.5.2/bulrush/static/css/
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     5597 2022-05-15 20:25:45.000000 bulrush-0.5.2/bulrush/static/css/main.css
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.359684 bulrush-0.5.2/bulrush/templates/
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1760 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/analytics.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      512 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/archives.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1451 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/article.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      913 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/article_infos.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      839 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/article_list.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     4944 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/base.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)       90 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/category.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      103 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/comments.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      445 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/disqus_script.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      279 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/github.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1065 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/index.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     3157 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/mailchimp.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1491 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/meta_tags.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      634 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/page.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      688 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/pagination.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      530 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/period_archives.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     1856 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/social.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)       85 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/tag.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      209 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/taglist.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      470 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/tags.html
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      257 2022-05-15 20:22:56.000000 bulrush-0.5.2/bulrush/templates/translations.html
-drwxr-xr-x   0 jonrsharpe   (501) staff       (20)        0 2022-05-15 21:05:49.356085 bulrush-0.5.2/bulrush.egg-info/
--rw-r--r--   0 jonrsharpe   (501) staff       (20)     8640 2022-05-15 21:05:49.000000 bulrush-0.5.2/bulrush.egg-info/PKG-INFO
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      988 2022-05-15 21:05:49.000000 bulrush-0.5.2/bulrush.egg-info/SOURCES.txt
--rw-r--r--   0 jonrsharpe   (501) staff       (20)        1 2022-05-15 21:05:49.000000 bulrush-0.5.2/bulrush.egg-info/dependency_links.txt
--rw-r--r--   0 jonrsharpe   (501) staff       (20)       21 2022-05-15 21:05:49.000000 bulrush-0.5.2/bulrush.egg-info/requires.txt
--rw-r--r--   0 jonrsharpe   (501) staff       (20)        8 2022-05-15 21:05:49.000000 bulrush-0.5.2/bulrush.egg-info/top_level.txt
--rw-r--r--   0 jonrsharpe   (501) staff       (20)       38 2022-05-15 21:05:49.360226 bulrush-0.5.2/setup.cfg
--rw-r--r--   0 jonrsharpe   (501) staff       (20)      973 2022-05-15 21:05:03.000000 bulrush-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.974168 bulrush-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-29 14:26:50.000000 bulrush-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 14:27:15.974168 bulrush-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-29 14:26:50.000000 bulrush-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/image_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/license_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/schema_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.966168 bulrush-0.6.2/bulrush/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush/static/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/analytics.html
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/archives.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article_infos.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/category.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/comments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/disqus_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/github.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/mailchimp.html
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/mermaid.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/meta_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/period_archives.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/social.html
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/taglist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:27:15.974168 bulrush-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-29 14:26:50.000000 bulrush-0.6.2/setup.py
```

### Comparing `bulrush-0.5.2/LICENSE` & `bulrush-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/PKG-INFO` & `bulrush-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bulrush
-Version: 0.5.2
+Version: 0.6.2
 Summary: Bulrush theme for Pelican
 Home-page: https://github.com/textbook/bulrush
 Author: Jonathan Sharpe
 Author-email: mail@jonrshar.pe
 License: ISC
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pelican :: Themes
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -43,14 +42,16 @@
 the default styling.
 
  - [x] **Service integrations** - including Disqus, GitHub, Google Analytics
 and MailChimp.
 
  - [x] **PyPI package available** - so it can be `pip install`-ed.
 
+ - [x] **[Mermaid][25] integration** - so you can include generated diagrams.
+
 Installation
 ------------
 
 Bulrush is available via the [Python Package Index][22], so you can install it
 with:
 
 ```bash
@@ -117,27 +118,28 @@
 
 Settings
 --------
 
 As well as the [basic settings][14], Bulrush supports the following options in
 your `pelicanconf.py`:
 
-| Setting name | What does it do? |
-| --- | --- |
+| Setting name           | What does it do?                                                                                                     |
+|------------------------|----------------------------------------------------------------------------------------------------------------------|
 | `BULRUSH_SHOW_SUMMARY` | A boolean, whether to show a summary rather than full article on index, category and tag pages. Defaults to `False`. |
-| `DISQUS_SITENAME` | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied. |
-| `GITHUB_URL` | Enables the "Fork me on GitHub" ribbon. |
-| `GOOGLE_ANALYTICS` | Set to `'UA-XXXX-YYYY'` to activate Google Analytics. |
-| `LICENSE` | A string or dictionary describing the license for the site; see details below. |
-| `LINKS` | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar. |
-| `MAILCHIMP` | Configure to activate a [MailChimp][20] sign-up form; see details below. |
-| `MENUITEMS` | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation. |
-| `SITESUBTITLE` | A subtitle to appear in the header. |
-| `SOCIAL` | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar. |
-| `TWITTER_USERNAME` | Enables Twitter meta-tags in the article and page headers. |
+| `DISQUS_SITENAME`      | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied.  |
+| `GITHUB_URL`           | Enables the "Fork me on GitHub" ribbon.                                                                              |
+| `GOOGLE_ANALYTICS`     | Set to `'UA-XXXX-YYYY'` to activate Google Analytics.                                                                |
+| `LICENSE`              | A string or dictionary describing the license for the site; see details below.                                       |
+| `LINKS`                | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar.                    |
+| `MAILCHIMP`            | Configure to activate a [MailChimp][20] sign-up form; see details below.                                             |
+| `MERMAID`              | Activate [Mermaid][25] diagram support; see details below.                                                           |
+| `MENUITEMS`            | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation.                                    |
+| `SITESUBTITLE`         | A subtitle to appear in the header.                                                                                  |
+| `SOCIAL`               | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar.                                |
+| `TWITTER_USERNAME`     | Enables Twitter meta-tags in the article and page headers.                                                           |
 
 If `DISPLAY_CATEGORIES_ON_MENU` is omitted or set explicitly to `True`, the
 categories are shown in the tabbed navigation with any `MENUITEMS`. If
 `DISPLAY_PAGES_ON_MENU` is omitted or set explicitly to `True`, they are listed
 in the sidebar with any `SOCIAL` or other `LINKS`.
 
 ### Social Links
@@ -195,14 +197,54 @@
  - License definition (`dict`): A dictionary specifying the `name`, `url` and
    optional `icon` (must be a Font Awesome icon name, default is
    [`file-text-o`][23]).
 
 The license details will be displayed at the bottom of the sidebar on every
 page.
 
+### Mermaid Configuration
+
+Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
+written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
+with the `mermaid` class:
+
+```markdown
+<pre class="mermaid">
+graph TD;
+    A-->B;
+    A-->C;
+    B-->D;
+    C-->D;
+</pre>
+```
+
+If you set `MERMAID = True`, this will simply enable Mermaid with some default
+settings:
+
+```javascript
+  const defaults = {
+    securityLevel: "loose",
+    theme: "default",
+    themeVariables: {
+      fontFamily: 'BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif',
+    },
+  };
+```
+
+To override these settings, or any of Mermaid's own [default configuration][26]
+you can pass a _dictionary_ instead. This will be shallowly merged into the
+defaults:
+
+```python
+MERMAID = dict(
+    securityLevel="strict",
+    theme="forest",  # disables fontFamily override
+)
+```
+
 Custom Styling
 --------------
 
 If any of the entries in `EXTRA_PATH_METADATA` have `'path'`s ending with
 `'.css'` they will be included in the base template, allowing the site style
 to be overridden as required. For example, in your `pelicanconf.py`:
 
@@ -241,17 +283,17 @@
   [9]: https://github.com/miracle2k/webassets/
   [10]: ./screenshot-980px.png
   [11]: ./screenshot-480px.png
   [12]: ./screenshot-840px.png
   [13]: ./screenshot-1440px.png
   [14]: http://docs.getpelican.com/en/3.6.3/settings.html#basic-settings
   [15]: https://github.com/getpelican/pelican-plugins/tree/master/assets
-  [17]: https://github.com/textbook/bulrush/blob/master/templates/social.html
+  [17]: https://github.com/textbook/bulrush/blob/main/templates/social.html
   [18]: https://help.github.com/articles/about-pull-requests/
   [19]: http://kb.mailchimp.com/accounts/billing/add-or-remove-monkeyrewards
   [20]: http://eepurl.com/cNv6Rb
   [21]: http://kb.mailchimp.com/lists/signup-forms/add-a-signup-form-to-your-website
   [22]: https://pypi.python.org/pypi/bulrush
   [23]: http://fontawesome.io/icon/file-text-o/
   [24]: ./screenshot-social.png
-
-
+  [25]: https://mermaid.js.org/
+  [26]: https://mermaid.js.org/config/setup/modules/mermaidAPI.html#mermaidapi-configuration-defaults
```

### Comparing `bulrush-0.5.2/README.md` & `bulrush-0.6.2/bulrush.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: bulrush
+Version: 0.6.2
+Summary: Bulrush theme for Pelican
+Home-page: https://github.com/textbook/bulrush
+Author: Jonathan Sharpe
+Author-email: mail@jonrshar.pe
+License: ISC
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pelican :: Themes
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Bulrush
 =======
 
 A [Bulma][1]-based [Pelican][2] blog theme; clean, flexible and responsive.
 
  ![Screenshot - Bulrush at 1440px][13]
 
@@ -27,14 +42,16 @@
 the default styling.
 
  - [x] **Service integrations** - including Disqus, GitHub, Google Analytics
 and MailChimp.
 
  - [x] **PyPI package available** - so it can be `pip install`-ed.
 
+ - [x] **[Mermaid][25] integration** - so you can include generated diagrams.
+
 Installation
 ------------
 
 Bulrush is available via the [Python Package Index][22], so you can install it
 with:
 
 ```bash
@@ -101,27 +118,28 @@
 
 Settings
 --------
 
 As well as the [basic settings][14], Bulrush supports the following options in
 your `pelicanconf.py`:
 
-| Setting name | What does it do? |
-| --- | --- |
+| Setting name           | What does it do?                                                                                                     |
+|------------------------|----------------------------------------------------------------------------------------------------------------------|
 | `BULRUSH_SHOW_SUMMARY` | A boolean, whether to show a summary rather than full article on index, category and tag pages. Defaults to `False`. |
-| `DISQUS_SITENAME` | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied. |
-| `GITHUB_URL` | Enables the "Fork me on GitHub" ribbon. |
-| `GOOGLE_ANALYTICS` | Set to `'UA-XXXX-YYYY'` to activate Google Analytics. |
-| `LICENSE` | A string or dictionary describing the license for the site; see details below. |
-| `LINKS` | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar. |
-| `MAILCHIMP` | Configure to activate a [MailChimp][20] sign-up form; see details below. |
-| `MENUITEMS` | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation. |
-| `SITESUBTITLE` | A subtitle to appear in the header. |
-| `SOCIAL` | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar. |
-| `TWITTER_USERNAME` | Enables Twitter meta-tags in the article and page headers. |
+| `DISQUS_SITENAME`      | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied.  |
+| `GITHUB_URL`           | Enables the "Fork me on GitHub" ribbon.                                                                              |
+| `GOOGLE_ANALYTICS`     | Set to `'UA-XXXX-YYYY'` to activate Google Analytics.                                                                |
+| `LICENSE`              | A string or dictionary describing the license for the site; see details below.                                       |
+| `LINKS`                | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar.                    |
+| `MAILCHIMP`            | Configure to activate a [MailChimp][20] sign-up form; see details below.                                             |
+| `MERMAID`              | Activate [Mermaid][25] diagram support; see details below.                                                           |
+| `MENUITEMS`            | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation.                                    |
+| `SITESUBTITLE`         | A subtitle to appear in the header.                                                                                  |
+| `SOCIAL`               | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar.                                |
+| `TWITTER_USERNAME`     | Enables Twitter meta-tags in the article and page headers.                                                           |
 
 If `DISPLAY_CATEGORIES_ON_MENU` is omitted or set explicitly to `True`, the
 categories are shown in the tabbed navigation with any `MENUITEMS`. If
 `DISPLAY_PAGES_ON_MENU` is omitted or set explicitly to `True`, they are listed
 in the sidebar with any `SOCIAL` or other `LINKS`.
 
 ### Social Links
@@ -179,14 +197,54 @@
  - License definition (`dict`): A dictionary specifying the `name`, `url` and
    optional `icon` (must be a Font Awesome icon name, default is
    [`file-text-o`][23]).
 
 The license details will be displayed at the bottom of the sidebar on every
 page.
 
+### Mermaid Configuration
+
+Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
+written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
+with the `mermaid` class:
+
+```markdown
+<pre class="mermaid">
+graph TD;
+    A-->B;
+    A-->C;
+    B-->D;
+    C-->D;
+</pre>
+```
+
+If you set `MERMAID = True`, this will simply enable Mermaid with some default
+settings:
+
+```javascript
+  const defaults = {
+    securityLevel: "loose",
+    theme: "default",
+    themeVariables: {
+      fontFamily: 'BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif',
+    },
+  };
+```
+
+To override these settings, or any of Mermaid's own [default configuration][26]
+you can pass a _dictionary_ instead. This will be shallowly merged into the
+defaults:
+
+```python
+MERMAID = dict(
+    securityLevel="strict",
+    theme="forest",  # disables fontFamily override
+)
+```
+
 Custom Styling
 --------------
 
 If any of the entries in `EXTRA_PATH_METADATA` have `'path'`s ending with
 `'.css'` they will be included in the base template, allowing the site style
 to be overridden as required. For example, in your `pelicanconf.py`:
 
@@ -225,15 +283,17 @@
   [9]: https://github.com/miracle2k/webassets/
   [10]: ./screenshot-980px.png
   [11]: ./screenshot-480px.png
   [12]: ./screenshot-840px.png
   [13]: ./screenshot-1440px.png
   [14]: http://docs.getpelican.com/en/3.6.3/settings.html#basic-settings
   [15]: https://github.com/getpelican/pelican-plugins/tree/master/assets
-  [17]: https://github.com/textbook/bulrush/blob/master/templates/social.html
+  [17]: https://github.com/textbook/bulrush/blob/main/templates/social.html
   [18]: https://help.github.com/articles/about-pull-requests/
   [19]: http://kb.mailchimp.com/accounts/billing/add-or-remove-monkeyrewards
   [20]: http://eepurl.com/cNv6Rb
   [21]: http://kb.mailchimp.com/lists/signup-forms/add-a-signup-form-to-your-website
   [22]: https://pypi.python.org/pypi/bulrush
   [23]: http://fontawesome.io/icon/file-text-o/
   [24]: ./screenshot-social.png
+  [25]: https://mermaid.js.org/
+  [26]: https://mermaid.js.org/config/setup/modules/mermaidAPI.html#mermaidapi-configuration-defaults
```

### Comparing `bulrush-0.5.2/bulrush/__init__.py` & `bulrush-0.6.2/bulrush/__init__.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/image_extractor.py` & `bulrush-0.6.2/bulrush/image_extractor.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/license_generator.py` & `bulrush-0.6.2/bulrush/license_generator.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/schema_generator.py` & `bulrush-0.6.2/bulrush/schema_generator.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/static/css/main.css` & `bulrush-0.6.2/bulrush/static/css/main.css`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/analytics.html` & `bulrush-0.6.2/bulrush/templates/analytics.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/archives.html` & `bulrush-0.6.2/bulrush/templates/archives.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/article.html` & `bulrush-0.6.2/bulrush/templates/article.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/article_infos.html` & `bulrush-0.6.2/bulrush/templates/article_infos.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/article_list.html` & `bulrush-0.6.2/bulrush/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/base.html` & `bulrush-0.6.2/bulrush/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 <!DOCTYPE html>
 <html lang="{{ DEFAULT_LANG }}">
 <head prefix="og: http://ogp.me/ns# article: http://ogp.me/ns/article#">
   <meta charset="utf-8"/>
   <meta name="viewport" content="width=device-width">
   <title>{% block title %}{{ SITENAME }}{% endblock %}</title>
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
-  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.5/css/bulma.min.css">
+  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.9.4/css/bulma.min.css">
   {% assets output="css/main.%(version)s.css", "css/main.css" %}
     <link rel="stylesheet" href="{{ SITEURL }}/{{ ASSET_URL }}">
   {% endassets %}
   <style media="print">.is-hidden-print{display:none !important}</style>
   {% for extra_path in EXTRA_PATH_METADATA.values() %}
     {% if extra_path.get('path', '').endswith('.css') %}
       <link rel="stylesheet" href="{{ SITEURL }}/{{ extra_path['path'] }}">
     {% endif %}
   {% endfor %}
+  {% if MERMAID %}
+    {% include 'mermaid.html' %}
+  {% endif %}
   {% block tags %}
   {% endblock %}
 </head>
 
 <body id="index" class="home">
 <header class="hero is-primary">
   <div class="hero-head">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 
 
  {% assets output="css/main.%(version)s.css", "css/main.css" %}
  {% endassets %}
  {% for extra_path in EXTRA_PATH_METADATA.values() %} {% if extra_path.get
 ('path', '').endswith('.css') %}
- {% endif %} {% endfor %} {% block tags %} {% endblock %}
+ {% endif %} {% endfor %} {% if MERMAID %} {% include 'mermaid.html' %} {%
+endif %} {% block tags %} {% endblock %}
 html" %} is-active{% endif %}" href="{{ SITEURL }}/">{{ SITENAME }}
 
 
 {% for title, link in MENUITEMS|reverse %} {{_title_}} {% endfor %} {% if
 DISPLAY_CATEGORIES_ON_MENU %} {% for cat, null in categories|reverse %} {{_cat
 }} {% endfor %} {% endif %}
 {% block content %} {% endblock %}
```

### Comparing `bulrush-0.5.2/bulrush/templates/index.html` & `bulrush-0.6.2/bulrush/templates/index.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/mailchimp.html` & `bulrush-0.6.2/bulrush/templates/mailchimp.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/meta_tags.html` & `bulrush-0.6.2/bulrush/templates/meta_tags.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/page.html` & `bulrush-0.6.2/bulrush/templates/page.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/pagination.html` & `bulrush-0.6.2/bulrush/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/period_archives.html` & `bulrush-0.6.2/bulrush/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush/templates/social.html` & `bulrush-0.6.2/bulrush/templates/social.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.5.2/bulrush.egg-info/PKG-INFO` & `bulrush-0.6.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: bulrush
-Version: 0.5.2
-Summary: Bulrush theme for Pelican
-Home-page: https://github.com/textbook/bulrush
-Author: Jonathan Sharpe
-Author-email: mail@jonrshar.pe
-License: ISC
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pelican :: Themes
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Bulrush
 =======
 
 A [Bulma][1]-based [Pelican][2] blog theme; clean, flexible and responsive.
 
  ![Screenshot - Bulrush at 1440px][13]
 
@@ -43,14 +27,16 @@
 the default styling.
 
  - [x] **Service integrations** - including Disqus, GitHub, Google Analytics
 and MailChimp.
 
  - [x] **PyPI package available** - so it can be `pip install`-ed.
 
+ - [x] **[Mermaid][25] integration** - so you can include generated diagrams.
+
 Installation
 ------------
 
 Bulrush is available via the [Python Package Index][22], so you can install it
 with:
 
 ```bash
@@ -117,27 +103,28 @@
 
 Settings
 --------
 
 As well as the [basic settings][14], Bulrush supports the following options in
 your `pelicanconf.py`:
 
-| Setting name | What does it do? |
-| --- | --- |
+| Setting name           | What does it do?                                                                                                     |
+|------------------------|----------------------------------------------------------------------------------------------------------------------|
 | `BULRUSH_SHOW_SUMMARY` | A boolean, whether to show a summary rather than full article on index, category and tag pages. Defaults to `False`. |
-| `DISQUS_SITENAME` | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied. |
-| `GITHUB_URL` | Enables the "Fork me on GitHub" ribbon. |
-| `GOOGLE_ANALYTICS` | Set to `'UA-XXXX-YYYY'` to activate Google Analytics. |
-| `LICENSE` | A string or dictionary describing the license for the site; see details below. |
-| `LINKS` | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar. |
-| `MAILCHIMP` | Configure to activate a [MailChimp][20] sign-up form; see details below. |
-| `MENUITEMS` | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation. |
-| `SITESUBTITLE` | A subtitle to appear in the header. |
-| `SOCIAL` | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar. |
-| `TWITTER_USERNAME` | Enables Twitter meta-tags in the article and page headers. |
+| `DISQUS_SITENAME`      | Enables Disqus comments. Note that you should set up the full Comment Count Link, as no additional text is applied.  |
+| `GITHUB_URL`           | Enables the "Fork me on GitHub" ribbon.                                                                              |
+| `GOOGLE_ANALYTICS`     | Set to `'UA-XXXX-YYYY'` to activate Google Analytics.                                                                |
+| `LICENSE`              | A string or dictionary describing the license for the site; see details below.                                       |
+| `LINKS`                | A list of tuples `('Title', 'URL')` for links to appear in the "blogroll" section of the sidebar.                    |
+| `MAILCHIMP`            | Configure to activate a [MailChimp][20] sign-up form; see details below.                                             |
+| `MERMAID`              | Activate [Mermaid][25] diagram support; see details below.                                                           |
+| `MENUITEMS`            | A list of tuples `('Title', 'URL')` for items to appear in the tabbed navigation.                                    |
+| `SITESUBTITLE`         | A subtitle to appear in the header.                                                                                  |
+| `SOCIAL`               | A list of tuples `('Title', 'URL')` to appear in the "social" section of the sidebar.                                |
+| `TWITTER_USERNAME`     | Enables Twitter meta-tags in the article and page headers.                                                           |
 
 If `DISPLAY_CATEGORIES_ON_MENU` is omitted or set explicitly to `True`, the
 categories are shown in the tabbed navigation with any `MENUITEMS`. If
 `DISPLAY_PAGES_ON_MENU` is omitted or set explicitly to `True`, they are listed
 in the sidebar with any `SOCIAL` or other `LINKS`.
 
 ### Social Links
@@ -195,14 +182,54 @@
  - License definition (`dict`): A dictionary specifying the `name`, `url` and
    optional `icon` (must be a Font Awesome icon name, default is
    [`file-text-o`][23]).
 
 The license details will be displayed at the bottom of the sidebar on every
 page.
 
+### Mermaid Configuration
+
+Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
+written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
+with the `mermaid` class:
+
+```markdown
+<pre class="mermaid">
+graph TD;
+    A-->B;
+    A-->C;
+    B-->D;
+    C-->D;
+</pre>
+```
+
+If you set `MERMAID = True`, this will simply enable Mermaid with some default
+settings:
+
+```javascript
+  const defaults = {
+    securityLevel: "loose",
+    theme: "default",
+    themeVariables: {
+      fontFamily: 'BlinkMacSystemFont, -apple-system, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif',
+    },
+  };
+```
+
+To override these settings, or any of Mermaid's own [default configuration][26]
+you can pass a _dictionary_ instead. This will be shallowly merged into the
+defaults:
+
+```python
+MERMAID = dict(
+    securityLevel="strict",
+    theme="forest",  # disables fontFamily override
+)
+```
+
 Custom Styling
 --------------
 
 If any of the entries in `EXTRA_PATH_METADATA` have `'path'`s ending with
 `'.css'` they will be included in the base template, allowing the site style
 to be overridden as required. For example, in your `pelicanconf.py`:
 
@@ -241,17 +268,17 @@
   [9]: https://github.com/miracle2k/webassets/
   [10]: ./screenshot-980px.png
   [11]: ./screenshot-480px.png
   [12]: ./screenshot-840px.png
   [13]: ./screenshot-1440px.png
   [14]: http://docs.getpelican.com/en/3.6.3/settings.html#basic-settings
   [15]: https://github.com/getpelican/pelican-plugins/tree/master/assets
-  [17]: https://github.com/textbook/bulrush/blob/master/templates/social.html
+  [17]: https://github.com/textbook/bulrush/blob/main/templates/social.html
   [18]: https://help.github.com/articles/about-pull-requests/
   [19]: http://kb.mailchimp.com/accounts/billing/add-or-remove-monkeyrewards
   [20]: http://eepurl.com/cNv6Rb
   [21]: http://kb.mailchimp.com/lists/signup-forms/add-a-signup-form-to-your-website
   [22]: https://pypi.python.org/pypi/bulrush
   [23]: http://fontawesome.io/icon/file-text-o/
   [24]: ./screenshot-social.png
-
-
+  [25]: https://mermaid.js.org/
+  [26]: https://mermaid.js.org/config/setup/modules/mermaidAPI.html#mermaidapi-configuration-defaults
```

### Comparing `bulrush-0.5.2/bulrush.egg-info/SOURCES.txt` & `bulrush-0.6.2/bulrush.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 bulrush/templates/base.html
 bulrush/templates/category.html
 bulrush/templates/comments.html
 bulrush/templates/disqus_script.html
 bulrush/templates/github.html
 bulrush/templates/index.html
 bulrush/templates/mailchimp.html
+bulrush/templates/mermaid.html
 bulrush/templates/meta_tags.html
 bulrush/templates/page.html
 bulrush/templates/pagination.html
 bulrush/templates/period_archives.html
 bulrush/templates/social.html
 bulrush/templates/tag.html
 bulrush/templates/taglist.html
```

### Comparing `bulrush-0.5.2/setup.py` & `bulrush-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
             'static/css/*.css',
         ]
     },
     packages=['bulrush'],
     test_suite='tests',
     tests_require=['pelican'],
     url='https://github.com/textbook/bulrush',
-    version='0.5.2',
+    version='0.6.2',
 )
```

