# Comparing `tmp/idds-monitor-1.2.8.tar.gz` & `tmp/idds-monitor-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-monitor-1.2.8.tar", last modified: Sat Apr 29 14:38:44 2023, max compression
+gzip compressed data, was "idds-monitor-1.2.9.tar", last modified: Sat Apr 29 19:25:01 2023, max compression
```

## Comparing `idds-monitor-1.2.8.tar` & `idds-monitor-1.2.9.tar`

### file list

```diff
@@ -1,528 +1,528 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.372177 idds-monitor-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-29 14:38:44.372177 idds-monitor-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.316175 idds-monitor-1.2.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.316175 idds-monitor-1.2.8/data/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/404.html
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/basic-table.html
--rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/blank.html
--rw-r--r--   0 runner    (1001) docker     (123)    38831 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/dashboard.html.backup
--rw-r--r--   0 runner    (1001) docker     (123)    38831 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/dashboard1.html
--rw-r--r--   0 runner    (1001) docker     (123)   232847 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/fontawesome.html
--rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/index.html.back
--rw-r--r--   0 runner    (1001) docker     (123)    59131 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/map-google.html
--rw-r--r--   0 runner    (1001) docker     (123)    22143 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/backup/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.308174 idds-monitor-1.2.8/data/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.316175 idds-monitor-1.2.8/data/bootstrap/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.324175 idds-monitor-1.2.8/data/bootstrap/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)    75728 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   184946 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    51515 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   115661 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    75801 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)   184950 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    51590 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   115738 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    94576 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    34718 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)    94589 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    41119 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    71446 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (123)   111059 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    49492 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28877 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    71303 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)   111003 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    49419 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28850 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   203731 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   500230 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   153117 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   422371 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   202974 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (123)   500122 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   153222 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   622580 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.328175 idds-monitor-1.2.8/data/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)   216787 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   410135 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    80827 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   318338 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   147542 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (123)   277557 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    76585 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   217908 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   156888 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   278810 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    62417 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   211771 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-29 14:38:44.000000 idds-monitor-1.2.8/data/conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/conf.js.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.328175 idds-monitor-1.2.8/data/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.328175 idds-monitor-1.2.8/data/css/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.308174 idds-monitor-1.2.8/data/css/icons/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.328175 idds-monitor-1.2.8/data/css/icons/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-brands.css
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-brands.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-regular.css
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-regular.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-solid.css
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-solid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome-all.css
--rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome-all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    47300 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    35628 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.332175 idds-monitor-1.2.8/data/css/icons/font-awesome/less/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_animated.less
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_bordered-pulled.less
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_core.less
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_fixed-width.less
--rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_icons.less
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_larger.less
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_list.less
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_mixins.less
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_rotated-flipped.less
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_screen-reader.less
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_stacked.less
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/_variables.less
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-brands.less
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-regular.less
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-solid.less
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/less/fontawesome.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.332175 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_animated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_core.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 runner    (1001) docker     (123)    71096 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_larger.scss
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_list.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_stacked.scss
--rw-r--r--   0 runner    (1001) docker     (123)    24203 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-brands.scss
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-regular.scss
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-solid.scss
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fontawesome.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.336176 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)    98940 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   510455 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98704 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63904 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    54684 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30788 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   104302 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   115152 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   421894 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   114932 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44004 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.308174 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.336176 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/
--rw-r--r--   0 runner    (1001) docker     (123)    90505 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css
--rw-r--r--   0 runner    (1001) docker     (123)    70850 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77567 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.340176 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot
--rw-r--r--   0 runner    (1001) docker     (123)   239073 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99212 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    50312 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff
--rw-r--r--   0 runner    (1001) docker     (123)    38384 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   261608 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)  1985766 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   261388 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    99736 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.340176 idds-monitor-1.2.8/data/css/icons/themify-icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.340176 idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    78748 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.eot
--rw-r--r--   0 runner    (1001) docker     (123)   234630 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78584 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56108 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.340176 idds-monitor-1.2.8/data/css/icons/themify-icons/ie7/
--rw-r--r--   0 runner    (1001) docker     (123)    36547 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/ie7/ie7.css
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/ie7/ie7.js
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/themify-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/themify-icons/themify-icons.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/css/icons/weather-icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.340176 idds-monitor-1.2.8/data/css/icons/weather-icons/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-core.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-variables.css
--rw-r--r--   0 runner    (1001) docker     (123)   150543 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-wind.css
--rw-r--r--   0 runner    (1001) docker     (123)   150543 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-wind.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    34012 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.344176 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   185225 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.344176 idds-monitor-1.2.8/data/css/icons/weather-icons/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.344176 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-beaufort.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-day.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-direction.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-misc.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-moon.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-neutral.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-night.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-time.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/css/variables-wind-names.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.344176 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-day.less
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-direction.less
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-misc.less
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-moon.less
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-night.less
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-time.less
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less
--rw-r--r--   0 runner    (1001) docker     (123)    30994 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-wind.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-beaufort.less
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-day.less
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-direction.less
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-misc.less
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-moon.less
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-night.less
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-time.less
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-wind-names.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less
--rw-r--r--   0 runner    (1001) docker     (123)    19436 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-owm.less
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-yahoo.less
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-classes.less
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-core.less
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-variables.less
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-wind.less
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-wind.min.less
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons.less
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons.min.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-direction.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-time.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-beaufort.scss
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-direction.scss
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-misc.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-time.scss
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-wind-names.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss
--rw-r--r--   0 runner    (1001) docker     (123)    19614 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-owm.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-classes.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-core.scss
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-wind.min.scss
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-wind.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons.min.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)   286030 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/style.extra.css
--rw-r--r--   0 runner    (1001) docker     (123)   245218 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/css/style.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/detail_processing.html
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/detail_request.html
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/detail_transform.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.348176 idds-monitor-1.2.8/data/js/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/app-style-switcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/js/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/js/pages/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/dashboard1.js
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/dashboard1.js.back
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/dashboard2.js.back
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/detail_processing.js
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/detail_request.js
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/detail_transform.js
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/processing.js
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/pages/dashboards/transform.js
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/sidebarmenu.js
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/js/waves.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/plugins/bower_components/chartist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/chartist/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/chartist/dist/chartist.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    40223 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/chartist/dist/chartist.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/counterup/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/counterup/jquery.counterup.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/
--rw-r--r--   0 runner    (1001) docker     (123)    61030 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.js
--rw-r--r--   0 runner    (1001) docker     (123)    30547 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    42062 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/jquery.gmaps.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.controls.js
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.core.js
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.events.js
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.geofences.js
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.layers.js
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.markers.js
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.routes.js
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.static.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/plugins/bower_components/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/core.js
--rw-r--r--   0 runner    (1001) docker     (123)    86929 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    69919 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/jquery.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/jquery-datatables/
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    86549 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.352177 idds-monitor-1.2.8/data/plugins/bower_components/jquery-sparkline/
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    35899 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js
--rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js
--rw-r--r--   0 runner    (1001) docker     (123)    48633 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/esm/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/esm/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/umd/
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/umd/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/custom-select.png
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/idds.png
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/idds_log.png
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/idds_log_text.png
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/idds_log_text1.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.356177 idds-monitor-1.2.8/data/plugins/images/large/
--rw-r--r--   0 runner    (1001) docker     (123)    87878 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/large/img1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/logo-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/logo-light-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/logo-light-text.png
--rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/logo-text.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.360177 idds-monitor-1.2.8/data/plugins/images/users/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/1-old.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/1.png
--rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    23280 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/2.png
--rw-r--r--   0 runner    (1001) docker     (123)    43005 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/3.png
--rw-r--r--   0 runner    (1001) docker     (123)    72937 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    78151 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62316 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/6.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    80126 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55544 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/8.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/agent.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/agent2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    25255 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/arijit.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/d1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/d2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/d3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/d4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/d5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/genu.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/govinda.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/hritik.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/pawandeep.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/profile.png
--rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/ritesh.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    30783 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/sonu.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/plugins/images/users/varun.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/processing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.360177 idds-monitor-1.2.8/data/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.364177 idds-monitor-1.2.8/data/scss/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (123)    59422 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.364177 idds-monitor-1.2.8/data/scss/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.364177 idds-monitor-1.2.8/data/scss/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/helpers/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/bootstrap/vendor/_rfs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/components.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/animation/
--rw-r--r--   0 runner    (1001) docker     (123)    56455 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/animation/animation.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/breadcrumb/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/breadcrumb/breadcrumb.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/buttons/buttons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/core.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/extra/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/extra/extra.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/layout/layout.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/loader/spinner.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/scafholdings/
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/scafholdings/scafholding.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/sidebar/sidebar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/topbar/
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/topbar/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/topbar/notify.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/core/wave-effects/
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/core/wave-effects/wave-effects.scss
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/custom.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/mixins/padding-margin.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/responsive.scss
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/style.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/theme-colors/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/theme-colors/theme-colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/variable.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/data/scss/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/widgets/comments.scss
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/widgets/feeds.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/widgets/profile.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/widgets/steamline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/scss/widgets/widgets.scss
--rw-r--r--   0 runner    (1001) docker     (123)    26819 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/data/transform.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.312174 idds-monitor-1.2.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.368177 idds-monitor-1.2.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.372177 idds-monitor-1.2.8/lib/idds/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/lib/idds/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:38:37.000000 idds-monitor-1.2.8/lib/idds/monitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:44.372177 idds-monitor-1.2.8/lib/idds_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-29 14:38:44.000000 idds-monitor-1.2.8/lib/idds_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-04-29 14:38:44.000000 idds-monitor-1.2.8/lib/idds_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:38:44.000000 idds-monitor-1.2.8/lib/idds_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 14:38:44.000000 idds-monitor-1.2.8/lib/idds_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-29 14:38:44.372177 idds-monitor-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-29 14:38:28.000000 idds-monitor-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.331788 idds-monitor-1.2.9/data/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/basic-table.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/blank.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38831 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/dashboard.html.backup
+-rw-r--r--   0 runner    (1001) docker     (123)    38831 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/dashboard1.html
+-rw-r--r--   0 runner    (1001) docker     (123)   232847 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/fontawesome.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/index.html.back
+-rw-r--r--   0 runner    (1001) docker     (123)    59131 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/map-google.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22143 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/backup/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.331788 idds-monitor-1.2.9/data/bootstrap/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.339789 idds-monitor-1.2.9/data/bootstrap/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    75728 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   184946 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    51515 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115661 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    75801 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)   184950 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    51590 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115738 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    94576 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    34718 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)    94589 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    41119 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    71446 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (123)   111059 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    49492 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28877 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    71303 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)   111003 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    49419 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28850 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   203731 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   500230 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   153117 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   422371 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   202974 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (123)   500122 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   153222 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   622580 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.343789 idds-monitor-1.2.9/data/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   216787 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   410135 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    80827 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   318338 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   147542 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   277557 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    76585 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   217908 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   156888 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   278810 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    62417 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   211771 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 19:25:01.000000 idds-monitor-1.2.9/data/conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/conf.js.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.343789 idds-monitor-1.2.9/data/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.343789 idds-monitor-1.2.9/data/css/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/css/icons/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.347789 idds-monitor-1.2.9/data/css/icons/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-brands.css
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-regular.css
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-regular.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-solid.css
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-solid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome-all.css
+-rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    47300 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    35628 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.347789 idds-monitor-1.2.9/data/css/icons/font-awesome/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_animated.less
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_bordered-pulled.less
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_core.less
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_fixed-width.less
+-rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_icons.less
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_larger.less
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_list.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_mixins.less
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_rotated-flipped.less
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_screen-reader.less
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_stacked.less
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/_variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-brands.less
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-regular.less
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-solid.less
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/less/fontawesome.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.351789 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_animated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_core.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    71096 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_larger.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_list.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_stacked.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    24203 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-brands.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-regular.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-solid.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fontawesome.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.355790 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    98940 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   510455 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98704 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63904 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    54684 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30788 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   104302 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   115152 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   421894 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   114932 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44004 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.359790 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    90505 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css
+-rw-r--r--   0 runner    (1001) docker     (123)    70850 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77567 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.363790 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   239073 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99212 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    50312 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    38384 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   261608 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  1985766 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   261388 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    99736 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.363790 idds-monitor-1.2.9/data/css/icons/themify-icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.363790 idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    78748 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   234630 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78584 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56108 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.363790 idds-monitor-1.2.9/data/css/icons/themify-icons/ie7/
+-rw-r--r--   0 runner    (1001) docker     (123)    36547 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/ie7/ie7.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/ie7/ie7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/themify-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/themify-icons/themify-icons.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/css/icons/weather-icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.367790 idds-monitor-1.2.9/data/css/icons/weather-icons/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-variables.css
+-rw-r--r--   0 runner    (1001) docker     (123)   150543 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-wind.css
+-rw-r--r--   0 runner    (1001) docker     (123)   150543 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-wind.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    34012 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.367790 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   185225 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.371791 idds-monitor-1.2.9/data/css/icons/weather-icons/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.371791 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-beaufort.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-day.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-direction.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-moon.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-neutral.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-night.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-time.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/css/variables-wind-names.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.375791 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-day.less
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-direction.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-misc.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-moon.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-night.less
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-time.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less
+-rw-r--r--   0 runner    (1001) docker     (123)    30994 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-wind.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.375791 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-beaufort.less
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-day.less
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-direction.less
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-misc.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-moon.less
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-night.less
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-time.less
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-wind-names.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.375791 idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less
+-rw-r--r--   0 runner    (1001) docker     (123)    19436 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-owm.less
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-yahoo.less
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-classes.less
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-core.less
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-wind.less
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-wind.min.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons.min.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.379791 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.379791 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-time.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.383791 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-beaufort.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-direction.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-misc.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-time.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-wind-names.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.383791 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    19614 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-owm.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-classes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-core.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-wind.min.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-wind.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons.min.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)   286030 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/style.extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)   245218 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/detail_processing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/detail_request.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/detail_transform.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.383791 idds-monitor-1.2.9/data/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/app-style-switcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/js/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/js/pages/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/dashboard1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/dashboard1.js.back
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/dashboard2.js.back
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/detail_processing.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/detail_request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/detail_transform.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/processing.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/pages/dashboards/transform.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/sidebarmenu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/js/waves.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/bower_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/data/plugins/bower_components/chartist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/bower_components/chartist/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/chartist/dist/chartist.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    40223 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/chartist/dist/chartist.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.323788 idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/bower_components/counterup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/counterup/jquery.counterup.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.387791 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    61030 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30547 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42062 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/jquery.gmaps.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.391792 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.controls.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.events.js
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.geofences.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.layers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.markers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.routes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.static.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/data/plugins/bower_components/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.391792 idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86929 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69919 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/jquery.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.391792 idds-monitor-1.2.9/data/plugins/bower_components/jquery-datatables/
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86549 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.391792 idds-monitor-1.2.9/data/plugins/bower_components/jquery-sparkline/
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35899 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    48633 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/esm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/esm/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.395792 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/umd/
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/umd/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.399792 idds-monitor-1.2.9/data/plugins/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/custom-select.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/idds.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/idds_log.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/idds_log_text.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/idds_log_text1.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.399792 idds-monitor-1.2.9/data/plugins/images/large/
+-rw-r--r--   0 runner    (1001) docker     (123)    87878 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/large/img1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/logo-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/logo-light-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/logo-light-text.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/logo-text.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.403792 idds-monitor-1.2.9/data/plugins/images/users/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/1-old.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23280 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43005 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72937 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    78151 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62316 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    80126 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55544 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/8.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/agent.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/agent2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    25255 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/arijit.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/d1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/d2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/d3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/d4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/d5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/genu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/govinda.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/hritik.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/pawandeep.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/ritesh.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    30783 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/sonu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/plugins/images/users/varun.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/processing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.407792 idds-monitor-1.2.9/data/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.415793 idds-monitor-1.2.9/data/scss/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    59422 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.415793 idds-monitor-1.2.9/data/scss/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.415793 idds-monitor-1.2.9/data/scss/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/helpers/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/bootstrap/vendor/_rfs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/components.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/animation/
+-rw-r--r--   0 runner    (1001) docker     (123)    56455 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/animation/animation.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/breadcrumb/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/breadcrumb/breadcrumb.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/buttons/buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/core.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/extra/extra.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/layout/layout.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/loader/spinner.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/scafholdings/
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/scafholdings/scafholding.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/sidebar/sidebar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.423793 idds-monitor-1.2.9/data/scss/core/topbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/topbar/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/topbar/notify.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/data/scss/core/wave-effects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/core/wave-effects/wave-effects.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/custom.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/data/scss/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/mixins/padding-margin.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/data/scss/theme-colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/theme-colors/theme-colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/variable.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/data/scss/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/widgets/comments.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/widgets/feeds.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/widgets/profile.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/widgets/steamline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/scss/widgets/widgets.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    26819 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/data/transform.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.327788 idds-monitor-1.2.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/lib/idds/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/lib/idds/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-monitor-1.2.9/lib/idds/monitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/lib/idds_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-29 19:25:01.000000 idds-monitor-1.2.9/lib/idds_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-04-29 19:25:01.000000 idds-monitor-1.2.9/lib/idds_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:25:01.000000 idds-monitor-1.2.9/lib/idds_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:25:01.000000 idds-monitor-1.2.9/lib/idds_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-29 19:25:01.427794 idds-monitor-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-29 19:24:44.000000 idds-monitor-1.2.9/setup.py
```

### Comparing `idds-monitor-1.2.8/PKG-INFO` & `idds-monitor-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-monitor
-Version: 1.2.8
+Version: 1.2.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-monitor-1.2.8/data/backup/404.html` & `idds-monitor-1.2.9/data/backup/404.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/basic-table.html` & `idds-monitor-1.2.9/data/backup/basic-table.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/blank.html` & `idds-monitor-1.2.9/data/backup/blank.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/dashboard.html.backup` & `idds-monitor-1.2.9/data/backup/dashboard.html.backup`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/dashboard1.html` & `idds-monitor-1.2.9/data/backup/dashboard1.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/fontawesome.html` & `idds-monitor-1.2.9/data/backup/fontawesome.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/index.html.back` & `idds-monitor-1.2.9/data/backup/index.html.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/map-google.html` & `idds-monitor-1.2.9/data/backup/map-google.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/backup/profile.html` & `idds-monitor-1.2.9/data/backup/profile.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/.DS_Store` & `idds-monitor-1.2.9/data/bootstrap/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.min.css` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `idds-monitor-1.2.9/data/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.min.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.min.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.esm.min.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.min.js` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/bootstrap/dist/js/bootstrap.min.js.map` & `idds-monitor-1.2.9/data/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/conf.js.template` & `idds-monitor-1.2.9/data/conf.js.template`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/.DS_Store` & `idds-monitor-1.2.9/data/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/.DS_Store` & `idds-monitor-1.2.9/data/css/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-brands.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-brands.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-brands.min.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-brands.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-regular.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-regular.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-regular.min.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-regular.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-solid.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-solid.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fa-solid.min.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fa-solid.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome-all.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome-all.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome-all.min.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/css/fontawesome.min.css` & `idds-monitor-1.2.9/data/css/icons/font-awesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/_icons.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/_icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/_mixins.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/_mixins.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/_rotated-flipped.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/_rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/_variables.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/_variables.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-brands.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-brands.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-regular.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-regular.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/fa-solid.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/fa-solid.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/less/fontawesome.less` & `idds-monitor-1.2.9/data/css/icons/font-awesome/less/fontawesome.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_icons.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_mixins.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_rotated-flipped.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_stacked.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_stacked.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/_variables.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-brands.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-brands.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-regular.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-regular.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/scss/fa-solid.scss` & `idds-monitor-1.2.9/data/css/icons/font-awesome/scss/fa-solid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.eot` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.svg` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.eot` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.svg` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.eot` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.svg` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2` & `idds-monitor-1.2.9/data/css/icons/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/material-design-iconic-font.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/css/materialdesignicons.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/Material-Design-Iconic-Font.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2` & `idds-monitor-1.2.9/data/css/icons/material-design-iconic-font/fonts/materialdesignicons-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.eot` & `idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.svg` & `idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.ttf` & `idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/fonts/themify.woff` & `idds-monitor-1.2.9/data/css/icons/themify-icons/fonts/themify.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/ie7/ie7.css` & `idds-monitor-1.2.9/data/css/icons/themify-icons/ie7/ie7.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/ie7/ie7.js` & `idds-monitor-1.2.9/data/css/icons/themify-icons/ie7/ie7.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/themify-icons.css` & `idds-monitor-1.2.9/data/css/icons/themify-icons/themify-icons.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/themify-icons/themify-icons.less` & `idds-monitor-1.2.9/data/css/icons/themify-icons/themify-icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-core.css` & `idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-core.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-wind.css` & `idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-wind.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons-wind.min.css` & `idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons-wind.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons.css` & `idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/css/weather-icons.min.css` & `idds-monitor-1.2.9/data/css/icons/weather-icons/css/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot` & `idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg` & `idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf` & `idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff` & `idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2` & `idds-monitor-1.2.9/data/css/icons/weather-icons/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-beaufort.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-day.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-day.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-misc.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-misc.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-moon-aliases.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-moon.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-moon.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-neutral.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-night.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-night.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-aliases.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-classes/classes-wind-degrees.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-day.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-day.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-moon.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-moon.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-neutral.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/icon-variables/variables-night.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/icon-variables/variables-night.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-forecast-io.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-owm.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-owm.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-wmo4680.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/mappings/wi-yahoo.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/mappings/wi-yahoo.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons-core.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons-core.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/less/weather-icons.min.less` & `idds-monitor-1.2.9/data/css/icons/weather-icons/less/weather-icons.min.less`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-beaufort.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-day.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-misc.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon-aliases.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-moon.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-neutral.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-night.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-aliases.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-classes/classes-wind-degrees.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-day.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-moon.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-neutral.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/icon-variables/variables-night.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-forecast-io.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-owm.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-owm.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-wmo4680.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/mappings/wi-yahoo.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons-core.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons-core.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons.min.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons.min.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/icons/weather-icons/sass/weather-icons.scss` & `idds-monitor-1.2.9/data/css/icons/weather-icons/sass/weather-icons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/style.css` & `idds-monitor-1.2.9/data/css/style.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/style.extra.css` & `idds-monitor-1.2.9/data/css/style.extra.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/css/style.min.css` & `idds-monitor-1.2.9/data/css/style.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/dashboard.html` & `idds-monitor-1.2.9/data/dashboard.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/detail_processing.html` & `idds-monitor-1.2.9/data/detail_processing.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/detail_request.html` & `idds-monitor-1.2.9/data/detail_request.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/detail_transform.html` & `idds-monitor-1.2.9/data/detail_transform.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/custom.js` & `idds-monitor-1.2.9/data/js/custom.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/dashboard1.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/dashboard1.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/dashboard1.js.back` & `idds-monitor-1.2.9/data/js/pages/dashboards/dashboard1.js.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/dashboard2.js.back` & `idds-monitor-1.2.9/data/js/pages/dashboards/dashboard2.js.back`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/detail_processing.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/detail_processing.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/detail_request.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/detail_request.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/detail_transform.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/detail_transform.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/processing.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/processing.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/pages/dashboards/transform.js` & `idds-monitor-1.2.9/data/js/pages/dashboards/transform.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/sidebarmenu.js` & `idds-monitor-1.2.9/data/js/sidebarmenu.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/js/waves.js` & `idds-monitor-1.2.9/data/js/waves.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/.DS_Store` & `idds-monitor-1.2.9/data/plugins/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/.DS_Store` & `idds-monitor-1.2.9/data/plugins/bower_components/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/chartist/dist/chartist.min.css` & `idds-monitor-1.2.9/data/plugins/bower_components/chartist/dist/chartist.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/chartist/dist/chartist.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/chartist/dist/chartist.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css` & `idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/chartist-plugin-tooltips/dist/chartist-plugin-tooltip.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/counterup/jquery.counterup.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/counterup/jquery.counterup.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/gmaps.min.js.map` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/gmaps.min.js.map`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.controls.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.controls.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.core.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.core.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.events.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.events.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.geometry.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.layers.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.layers.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.map_types.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.markers.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.markers.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.native_extensions.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.overlays.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.routes.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.routes.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.static.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.static.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.streetview.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/gmaps/lib/gmaps.utils.js` & `idds-monitor-1.2.9/data/plugins/bower_components/gmaps/lib/gmaps.utils.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/core.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/core.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/jquery.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery/dist/jquery.slim.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery-datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery-sparkline/jquery.charts-sparkline.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/jquery-sparkline/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/css/perfect-scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.common.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.esm.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/perfect-scrollbar/dist/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/esm/popper.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/popper-utils.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/popper.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/bower_components/popper.js/dist/umd/popper.min.js` & `idds-monitor-1.2.9/data/plugins/bower_components/popper.js/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/.DS_Store` & `idds-monitor-1.2.9/data/plugins/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/custom-select.png` & `idds-monitor-1.2.9/data/plugins/images/custom-select.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/favicon.png` & `idds-monitor-1.2.9/data/plugins/images/favicon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/idds.png` & `idds-monitor-1.2.9/data/plugins/images/idds.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/idds_log.png` & `idds-monitor-1.2.9/data/plugins/images/idds_log.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/idds_log_text.png` & `idds-monitor-1.2.9/data/plugins/images/idds_log_text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/idds_log_text1.png` & `idds-monitor-1.2.9/data/plugins/images/idds_log_text1.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/large/img1.jpg` & `idds-monitor-1.2.9/data/plugins/images/large/img1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/logo-icon.png` & `idds-monitor-1.2.9/data/plugins/images/logo-icon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/logo-light-icon.png` & `idds-monitor-1.2.9/data/plugins/images/logo-light-icon.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/logo-light-text.png` & `idds-monitor-1.2.9/data/plugins/images/logo-light-text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/logo-text.png` & `idds-monitor-1.2.9/data/plugins/images/logo-text.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/1-old.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/1-old.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/1.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/1.png` & `idds-monitor-1.2.9/data/plugins/images/users/1.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/2.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/2.png` & `idds-monitor-1.2.9/data/plugins/images/users/2.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/3.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/3.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/3.png` & `idds-monitor-1.2.9/data/plugins/images/users/3.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/4.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/4.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/5.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/5.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/6.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/6.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/7.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/7.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/8.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/8.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/agent.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/agent.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/agent2.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/agent2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/arijit.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/arijit.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/d1.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/d1.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/d2.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/d2.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/d3.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/d3.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/d4.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/d4.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/d5.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/d5.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/genu.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/genu.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/govinda.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/govinda.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/hritik.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/hritik.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/pawandeep.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/pawandeep.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/profile.png` & `idds-monitor-1.2.9/data/plugins/images/users/profile.png`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/ritesh.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/ritesh.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/sonu.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/sonu.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/plugins/images/users/varun.jpg` & `idds-monitor-1.2.9/data/plugins/images/users/varun.jpg`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/processing.html` & `idds-monitor-1.2.9/data/processing.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/.DS_Store` & `idds-monitor-1.2.9/data/scss/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/.DS_Store` & `idds-monitor-1.2.9/data/scss/bootstrap/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_accordion.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_alert.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_badge.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_breadcrumb.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_button-group.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_buttons.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_card.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_carousel.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_close.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_containers.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_dropdown.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_functions.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_images.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_list-group.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_mixins.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_modal.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_nav.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_navbar.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_pagination.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_popover.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_progress.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_reboot.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_root.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_spinners.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_tables.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_toasts.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_tooltip.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_type.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_utilities.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/_variables.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/bootstrap-grid.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/bootstrap-reboot.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/bootstrap-reboot.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/bootstrap.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_floating-labels.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-check.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-control.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-range.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_form-select.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_input-group.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_labels.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/forms/_validation.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/forms/_validation.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/helpers/_position.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_border-radius.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_breakpoints.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_buttons.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_caret.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_deprecate.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_forms.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_gradients.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_grid.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_pagination.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_pagination.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_reset-text.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_table-variants.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_transition.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_utilities.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/mixins/_visually-hidden.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/utilities/_api.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/bootstrap/vendor/_rfs.scss` & `idds-monitor-1.2.9/data/scss/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/.DS_Store` & `idds-monitor-1.2.9/data/scss/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/animation/animation.scss` & `idds-monitor-1.2.9/data/scss/core/animation/animation.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/breadcrumb/breadcrumb.scss` & `idds-monitor-1.2.9/data/scss/core/breadcrumb/breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/buttons/buttons.scss` & `idds-monitor-1.2.9/data/scss/core/buttons/buttons.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/extra/extra.scss` & `idds-monitor-1.2.9/data/scss/core/extra/extra.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/layout/layout.scss` & `idds-monitor-1.2.9/data/scss/core/layout/layout.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/loader/spinner.scss` & `idds-monitor-1.2.9/data/scss/core/loader/spinner.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/scafholdings/scafholding.scss` & `idds-monitor-1.2.9/data/scss/core/scafholdings/scafholding.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/sidebar/sidebar.scss` & `idds-monitor-1.2.9/data/scss/core/sidebar/sidebar.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/topbar/header.scss` & `idds-monitor-1.2.9/data/scss/core/topbar/header.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/topbar/notify.scss` & `idds-monitor-1.2.9/data/scss/core/topbar/notify.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/core/wave-effects/wave-effects.scss` & `idds-monitor-1.2.9/data/scss/core/wave-effects/wave-effects.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/mixins/padding-margin.scss` & `idds-monitor-1.2.9/data/scss/mixins/padding-margin.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/responsive.scss` & `idds-monitor-1.2.9/data/scss/responsive.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/style.scss` & `idds-monitor-1.2.9/data/scss/style.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/theme-colors/theme-colors.scss` & `idds-monitor-1.2.9/data/scss/theme-colors/theme-colors.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/variable.scss` & `idds-monitor-1.2.9/data/scss/variable.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/widgets/comments.scss` & `idds-monitor-1.2.9/data/scss/widgets/comments.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/widgets/feeds.scss` & `idds-monitor-1.2.9/data/scss/widgets/feeds.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/widgets/profile.scss` & `idds-monitor-1.2.9/data/scss/widgets/profile.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/scss/widgets/steamline.scss` & `idds-monitor-1.2.9/data/scss/widgets/steamline.scss`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/data/transform.html` & `idds-monitor-1.2.9/data/transform.html`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/lib/idds_monitor.egg-info/PKG-INFO` & `idds-monitor-1.2.9/lib/idds_monitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-monitor
-Version: 1.2.8
+Version: 1.2.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-monitor-1.2.8/lib/idds_monitor.egg-info/SOURCES.txt` & `idds-monitor-1.2.9/lib/idds_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-monitor-1.2.8/setup.py` & `idds-monitor-1.2.9/setup.py`

 * *Files identical despite different names*

