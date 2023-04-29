# Comparing `tmp/dcef-0.2.3.tar.gz` & `tmp/dcef-0.2.5.tar.gz`

## Comparing `dcef-0.2.3.tar` & `dcef-0.2.5.tar`

### file list

```diff
@@ -1,86 +1,90 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.3/.#README.md -> paddy@Paddys-Air.routerlogin.net.2877
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.3/.#full_build.sh -> paddy@Paddys-Air.routerlogin.net.2877
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.3/.#video_script.txt -> paddy@Paddys-Air.routerlogin.net.2877
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dcef-0.2.3/.coveragerc
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 dcef-0.2.3/ENV.txt
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 dcef-0.2.3/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dcef-0.2.3/babel.config.js
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef.json
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 dcef-0.2.3/full_build.sh
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 dcef-0.2.3/introduction.ipynb
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 dcef-0.2.3/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dcef-0.2.3/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 dcef-0.2.3/tryit.ipynb
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dcef-0.2.3/tsconfig.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcef-0.2.3/video_script.txt
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 dcef-0.2.3/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dcef-0.2.3/webpack.lab.config.js
--rw-r--r--   0        0        0   401763 2020-02-02 00:00:00.000000 dcef-0.2.3/yarn.lock
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dcef-0.2.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 dcef-0.2.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dcef-0.2.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dcef-0.2.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcef-0.2.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/_version.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/all_transforms.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/channeldata.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/configure_utils.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/dcef_widget.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/lispy.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/views.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/package.json
--rw-r--r--   0        0        0  1235630 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/116.2c99b074fd692e5d339c.js
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/116.2c99b074fd692e5d339c.js.LICENSE.txt
--rw-r--r--   0        0        0   372507 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js.LICENSE.txt
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/480.c629752d1a4021a728bb.js
--rw-r--r--   0        0        0    70495 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/486.0708227d0a518f636636.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/486.0708227d0a518f636636.js.LICENSE.txt
--rw-r--r--   0        0        0     9522 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/568.8b4e60cfe6905d620fad.js
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/remoteEntry.e5d1fdcb371ac4cc9f68.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/style.js
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/nbextension/extension.js
--rw-r--r--   0        0        0  1689053 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5593556 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/nbextension/index.js.map
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.3/dcef/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/Makefile
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/commands_vs_operations.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/make.bat
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/FAQ.rst
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/conf.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/index.rst
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/install.rst
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.3/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 dcef-0.2.3/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dcef-0.2.3/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 dcef-0.2.3/js/index.ts
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 dcef-0.2.3/js/paddywidget.ts
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 dcef-0.2.3/js/plugin.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 dcef-0.2.3/js/version.ts
--rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 dcef-0.2.3/static/images/dcf-jupyter.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dcef-0.2.3/style/widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.3/style/icons/filter.svg
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 dcef-0.2.3/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dcef-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 dcef-0.2.3/README.md
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dcef-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 dcef-0.2.3/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/.#README.md -> paddy@Paddys-MacBook-Air.local.752
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/.#full_build.sh -> paddy@Paddys-Air.routerlogin.net.2877
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/.#video_script.txt -> paddy@Paddys-Air.routerlogin.net.2877
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dcef-0.2.5/.coveragerc
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 dcef-0.2.5/ENV.txt
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 dcef-0.2.5/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dcef-0.2.5/babel.config.js
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef.json
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 dcef-0.2.5/full_build.sh
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 dcef-0.2.5/introduction.ipynb
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 dcef-0.2.5/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dcef-0.2.5/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 dcef-0.2.5/tryit.ipynb
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dcef-0.2.5/tsconfig.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcef-0.2.5/video_script.txt
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 dcef-0.2.5/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dcef-0.2.5/webpack.lab.config.js
+-rw-r--r--   0        0        0   401763 2020-02-02 00:00:00.000000 dcef-0.2.5/yarn.lock
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dcef-0.2.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 dcef-0.2.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dcef-0.2.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dcef-0.2.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcef-0.2.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/_version.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/all_transforms.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/channeldata.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/configure_utils.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/dcef_widget.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/lispy.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/views.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/package.json
+-rw-r--r--   0        0        0  1239281 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/116.f2c748ce51e22b52b0cb.js
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/116.f2c748ce51e22b52b0cb.js.LICENSE.txt
+-rw-r--r--   0        0        0   372507 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js.LICENSE.txt
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/480.ccd73b95e569f66845e5.js
+-rw-r--r--   0        0        0    70495 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/486.0708227d0a518f636636.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/486.0708227d0a518f636636.js.LICENSE.txt
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/568.b3c25a51cdf2e2d0b274.js
+-rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/remoteEntry.e97dd4f5ff7087528b29.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/style.js
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/nbextension/extension.js
+-rw-r--r--   0        0        0  1693479 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dcef-0.2.5/dcef/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/commands_vs_operations.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/.#using.rst -> paddy@Paddys-Air.routerlogin.net.2877
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/conf.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/index.rst
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/install.rst
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/using.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 dcef-0.2.5/docs/source/_static/embed-bundle.js.LICENSE.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/js/.#foo.ts -> paddy@Paddys-MacBook-Air.local.752
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcef-0.2.5/js/.#plugin.ts -> paddy@Paddys-MacBook-Air.local.752
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 dcef-0.2.5/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dcef-0.2.5/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 dcef-0.2.5/js/index.ts
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 dcef-0.2.5/js/paddywidget.ts
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 dcef-0.2.5/js/plugin.ts
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 dcef-0.2.5/js/version.ts
+-rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 dcef-0.2.5/static/images/dcf-jupyter.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dcef-0.2.5/style/widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 dcef-0.2.5/style/icons/filter.svg
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 dcef-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dcef-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 dcef-0.2.5/README.md
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 dcef-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    11669 2020-02-02 00:00:00.000000 dcef-0.2.5/PKG-INFO
```

### Comparing `dcef-0.2.3/ENV.txt` & `dcef-0.2.5/ENV.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/RELEASE.md` & `dcef-0.2.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/introduction.ipynb` & `dcef-0.2.5/introduction.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.940897212543554%*

 * *Differences: {"'cells'": "{0: {'execution_count': None}, 1: {'execution_count': None, 'outputs': []}, 2: "*

 * *            "{'source': {insert: [(0, 'from dcef.all_transforms import Command\\n'), (4, 'class "*

 * *            "GroupBy2(Command):\\n')], delete: [4, 0]}}, insert: [(3, OrderedDict([('cell_type', "*

 * *            "'code'), ('execution_count', None), ('metadata', OrderedDict()), ('outputs', []), "*

 * *            "('source', ['!echo $CONDA_DEFAULT_ENV\\n', '!pwd'])])), (5, "*

 * *            "OrderedDict([('cell_type', 'code'),  […]*

```diff
@@ -1,57 +1,41 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "from dcef.dcef_widget import DCEFWidget"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "43ed73239024467aa379974b4e73a2de",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "DCEFWidget(command_config={'argspecs': {'fillna': [[3, 'fillVal', 'type', 'integer']], 'dropcol': [None], 'one\u2026"
-                        ]
-                    },
-                    "execution_count": 2,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "df = pd.read_csv('./examples/data/2014-01-citibike-tripdata.csv')\n",
                 "w = DCEFWidget(df)\n",
                 "w"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from dcef.all_transforms import Transform\n",
+                "from dcef.all_transforms import Command\n",
                 "from dcef.lispy import s\n",
                 "#Here we start adding commands to the DCF Widget.  Every call to add_command replaces a command with the same name\n",
                 "@w.add_command\n",
-                "class GroupBy2(Transform):\n",
+                "class GroupBy2(Command):\n",
                 "    command_default = [s(\"groupby2\"), s('df'), 'col', {}]\n",
                 "    command_pattern = [[3, 'colMap', 'colEnum', ['null', 'sum', 'mean', 'median', 'count']]]\n",
                 "    @staticmethod \n",
                 "    def transform(df, col, col_spec):\n",
                 "        grps = df.groupby(col)\n",
                 "        df_contents = {}\n",
                 "        for k, v in col_spec.items():\n",
@@ -86,16 +70,42 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "!echo $CONDA_DEFAULT_ENV\n",
+                "!pwd"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# notice that there is now a Groupby2 Command in the widget"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df.info()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `dcef-0.2.3/package.json` & `dcef-0.2.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'dependencies'": "{'paddy-react-edit-list': '>=1.1.33'}"}*

```diff
@@ -6,15 +6,15 @@
     "bugs": {
         "url": "https://github.com/paddymul/dcef/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^6.0.0",
         "@jupyterlab/apputils": "^3.0.2",
         "lodash": "^4.17.21",
-        "paddy-react-edit-list": ">=1.1.25",
+        "paddy-react-edit-list": ">=1.1.33",
         "react": "^18.0.0",
         "react-dom": "^18.0.0"
     },
     "description": "Fast Datagrid widget for the Jupyter Notebook and JupyterLab",
     "devDependencies": {
         "@babel/cli": "^7.6.3",
         "@babel/core": "^7.6.3",
```

### Comparing `dcef-0.2.3/tryit.ipynb` & `dcef-0.2.5/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/tsconfig.json` & `dcef-0.2.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/video_script.txt` & `dcef-0.2.5/video_script.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/webpack.config.js` & `dcef-0.2.5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/yarn.lock` & `dcef-0.2.5/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -6383,18 +6383,18 @@
   integrity sha512-k3bdm2n25tkyxcjSKzB5x8kfVxlMdgsbPr0GkZcwHsLpba6cBjqCt1KlcChKEvxHIcTB1FVMuwoijZ26xex5MQ==
   dependencies:
     got "^9.6.0"
     registry-auth-token "^4.0.0"
     registry-url "^5.0.0"
     semver "^6.2.0"
 
-paddy-react-edit-list@>=1.1.25:
-  version "1.1.25"
-  resolved "https://registry.yarnpkg.com/paddy-react-edit-list/-/paddy-react-edit-list-1.1.25.tgz#a1d925100dfa3df792b778369437b1343a242886"
-  integrity sha512-QqwWCPc09ue2ljy6ZuSfsWBm1NbFOxS6pDZNSygVZmoZUVMbiAKltwF8sPtDqIouJ+s6qbri3SpIWU0io2367Q==
+paddy-react-edit-list@>=1.1.33:
+  version "1.1.33"
+  resolved "https://registry.yarnpkg.com/paddy-react-edit-list/-/paddy-react-edit-list-1.1.33.tgz#a790b8d211aeb37d66c8ca55250f7d79b7b8e4f2"
+  integrity sha512-8wxcfZr7q5T9XQGjSDQTGX+4dz4D0kjJA/bjAoPPF/7kVib4u4W5rftLeOK3WmaI/Z8IceDNJ+oHCbX3vOfVFQ==
   dependencies:
     "@ag-grid-community/client-side-row-model" "^29.2.0"
     "@types/lodash" "^4.14.191"
     ag-grid-community "^29.2.0"
     ag-grid-react "^29.2.0"
     lodash "^4.17.21"
     react "^18.0.0"
```

### Comparing `dcef-0.2.3/dcef/all_transforms.py` & `dcef-0.2.5/dcef/all_transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,12 +118,42 @@
                 commands.append("    df_contents['%s'] = grps['%s'].apply(lambda x: x.count())" % (k, k))
         #print("commands", commands)
         commands.append("    df = pd.DataFrame(df_contents)")
         return "\n".join(commands)
     
 
 
-    
+class to_datetime(Command):
+    #argument_names = ["df", "col"]
+    command_default = [s('to_datetime'), s('df'), "col"]
+    command_pattern = [None]
+
+    @staticmethod 
+    def transform(df, col):
+        df[col] = pd.to_datetime(df[col])
+        return df
+
+    @staticmethod 
+    def transform_to_py(df, col):
+        return "    df['%s'] = pd.to_datetime(df['%s'])" % (col, col)    
+
+class reindex(Command):
+    command_default = [s('reindex'), s('df'), "col"]
+    command_pattern = [None]
+
+    @staticmethod 
+    def transform(df, col):
+        old_col = df[col]
+        df.drop(col, axis=1, inplace=True)
+        df.index = old_col.values
+        return df
+
+    @staticmethod 
+    def transform_to_py(df, col):
+        return "\n".join(
+            ["    old_col = df['%s']" % col,
+             "    df.drop('%s', axis=1, inplace=True)" % col,
+             "    df.index = old_col.values"])
 
-DefaultCommandKlsList = [FillNA, DropCol, OneHot, GroupBy]
+DefaultCommandKlsList = [DropCol, to_datetime, SafeInt, FillNA, reindex, OneHot, GroupBy]
 command_defaults, command_patterns, dcef_transform, dcef_to_py_core = configure_dcef(DefaultCommandKlsList)
```

### Comparing `dcef-0.2.3/dcef/configure_utils.py` & `dcef-0.2.5/dcef/configure_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,9 +27,9 @@
         #interpreter to return a string code block, and for the real DCF
         #interpreter as 'begin'... that way the exact same instructions
         #could be sent to either interpreter.  For now, this will do
         individual_instructions =  [x for x in map(lambda x:convert_to_python(x, {'df':5}), instructions)]
         #print("individual_instructions", individual_instructions)
         code_block =  '\n'.join(individual_instructions)
 
-        return "def clean(df):\n" + code_block
+        return "def clean(df):\n" + code_block + "\n    return df"
     return command_defaults, command_patterns, dcef_transform, dcef_to_py
```

### Comparing `dcef-0.2.3/dcef/dcf_transform.py` & `dcef-0.2.5/dcef/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/df_methods.py` & `dcef-0.2.5/dcef/df_methods.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/index.html` & `dcef-0.2.5/dcef/index.html`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/lispy.py` & `dcef-0.2.5/dcef/lispy.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/views.py` & `dcef-0.2.5/dcef/views.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/labextension/package.json` & `dcef-0.2.5/dcef/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966145833333334%*

 * *Differences: {"'dependencies'": "{'paddy-react-edit-list': '>=1.1.33'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e97dd4f5ff7087528b29.js'}}"}*

```diff
@@ -6,15 +6,15 @@
     "bugs": {
         "url": "https://github.com/paddymul/dcef/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^6.0.0",
         "@jupyterlab/apputils": "^3.0.2",
         "lodash": "^4.17.21",
-        "paddy-react-edit-list": ">=1.1.25",
+        "paddy-react-edit-list": ">=1.1.33",
         "react": "^18.0.0",
         "react-dom": "^18.0.0"
     },
     "description": "Fast Datagrid widget for the Jupyter Notebook and JupyterLab",
     "devDependencies": {
         "@babel/cli": "^7.6.3",
         "@babel/core": "^7.6.3",
@@ -61,15 +61,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/paddymul/dcef",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e5d1fdcb371ac4cc9f68.js"
+            "load": "static/remoteEntry.e97dd4f5ff7087528b29.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./dcef/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `dcef-0.2.3/dcef/labextension/static/116.2c99b074fd692e5d339c.js` & `dcef-0.2.5/dcef/labextension/static/116.f2c748ce51e22b52b0cb.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 116.2c99b074fd692e5d339c.js.LICENSE.txt */
+/*! For license information please see 116.f2c748ce51e22b52b0cb.js.LICENSE.txt */
 (self.webpackChunkdcef = self.webpackChunkdcef || []).push([
     [116], {
         1731: (e, t, o) => {
             "use strict";
 
             function n(e) {
                 return null == e || "" === e ? null : e
@@ -33233,15 +33233,15 @@
                     return s
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ColumnsEditor = void 0;
             var a = i(o(7294)),
                 l = o(3800),
-                u = o(6978),
+                u = o(8002),
                 c = o(5727),
                 p = o(7137);
             t.ColumnsEditor = function(e) {
                 var t = void 0 === e ? {
                         df: l.EmptyDf,
                         activeColumn: "stoptime",
                         getOrRequester: p.serverGetTransformRequester,
@@ -33270,192 +33270,14 @@
                     commandConfig: i
                 }), a.default.createElement(p.DependentTabs, {
                     filledOperations: h,
                     getOrRequester: r
                 }))
             }
         },
-        6467: function(e, t, o) {
-            "use strict";
-            var n = this && this.__read || function(e, t) {
-                    var o = "function" == typeof Symbol && e[Symbol.iterator];
-                    if (!o) return e;
-                    var n, r, i = o.call(e),
-                        s = [];
-                    try {
-                        for (;
-                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
-                    } catch (e) {
-                        r = {
-                            error: e
-                        }
-                    } finally {
-                        try {
-                            n && !n.done && (o = i.return) && o.call(i)
-                        } finally {
-                            if (r) throw r.error
-                        }
-                    }
-                    return s
-                },
-                r = this && this.__spreadArray || function(e, t, o) {
-                    if (o || 2 === arguments.length)
-                        for (var n, r = 0, i = t.length; r < i; r++) !n && r in t || (n || (n = Array.prototype.slice.call(t, 0, r)), n[r] = t[r]);
-                    return e.concat(n || Array.prototype.slice.call(t))
-                },
-                i = this && this.__importDefault || function(e) {
-                    return e && e.__esModule ? e : {
-                        default: e
-                    }
-                };
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), t.OperationAdder = t.ArgGetters = t.OperationDetail = void 0;
-            var s = i(o(7294)),
-                a = i(o(4439));
-            t.OperationDetail = function(e) {
-                var o = e.command,
-                    n = e.setCommand,
-                    r = e.deleteCB,
-                    i = e.columns,
-                    l = e.commandPatterns;
-                if (void 0 === o) return s.default.createElement("h2", null, " error undefined command ");
-                var u = o[0].symbol,
-                    c = l[u];
-                if (a.default.isArray(c)) {
-                    if (a.default.isEqual(c, [null])) return s.default.createElement("div", {
-                        className: "operation-detail"
-                    }, s.default.createElement("button", {
-                        onClick: r
-                    }, "X"));
-                    var p = c;
-                    return s.default.createElement("div", {
-                        className: "operation-detail"
-                    }, s.default.createElement(t.ArgGetters, {
-                        command: o,
-                        fullPattern: p,
-                        setCommand: n,
-                        columns: i,
-                        deleteCB: r
-                    }))
-                }
-                return s.default.createElement("h2", null, "unknown command ", u)
-            }, t.ArgGetters = function(e) {
-                var t = e.command,
-                    o = e.fullPattern,
-                    n = e.setCommand,
-                    r = e.columns,
-                    i = e.deleteCB;
-                return s.default.createElement("div", {
-                    className: "arg-getters"
-                }, s.default.createElement("button", {
-                    onClick: i
-                }, "X"), o.map((function(e) {
-                    var o = e[0],
-                        i = t[o];
-                    return s.default.createElement("div", {
-                        key: o
-                    }, s.default.createElement(l, {
-                        argProps: e,
-                        val: i,
-                        setter: function(e) {
-                            var r = function(e, t, o) {
-                                return e.map((function(e, n) {
-                                    return n === t ? o : e
-                                }))
-                            }(t, o, e);
-                            n(r)
-                        },
-                        columns: r
-                    }))
-                })))
-            };
-            var l = function(e) {
-                var t = e.argProps,
-                    o = e.val,
-                    i = e.setter,
-                    l = e.columns,
-                    u = n(t, 4),
-                    c = (u[0], u[1]),
-                    p = u[2],
-                    d = u[3];
-                if ("enum" === p) return s.default.createElement("fieldset", null, s.default.createElement("label", null, " ", c, " "), s.default.createElement("select", {
-                    defaultValue: o,
-                    onChange: function(e) {
-                        return i(e.target.value)
-                    }
-                }, d.map((function(e) {
-                    return s.default.createElement("option", {
-                        key: e,
-                        value: e
-                    }, e)
-                }))));
-                if ("type" === p) return "integer" === d ? s.default.createElement("fieldset", null, s.default.createElement("label", null, " ", c, " "), s.default.createElement("input", {
-                    type: "number",
-                    defaultValue: o,
-                    step: "1",
-                    onChange: function(e) {
-                        return i(parseInt(e.target.value))
-                    }
-                })) : s.default.createElement("fieldset", null, s.default.createElement("label", null, " ", c, " "), s.default.createElement("input", {
-                    value: "dont know"
-                }));
-                if ("colEnum" === p) {
-                    var h = l.map((function(e) {
-                        var t = a.default.get(o, e, "null");
-                        return s.default.createElement("td", null, s.default.createElement("select", {
-                            defaultValue: t,
-                            onChange: function(t) {
-                                var s, l, u, c, p = t.target.value;
-                                if (a.default.isString(p)) {
-                                    var d = (s = o, l = e, u = p, (c = a.default.clone(s))[l] = u, c);
-                                    i(function(e, t) {
-                                        return void 0 === t && (t = []), a.default.pickBy(e, (function(e) {
-                                            return !r([null, void 0], n(t), !1).includes(e)
-                                        }))
-                                    }(d, ["null"]))
-                                }
-                            }
-                        }, d.map((function(e) {
-                            return s.default.createElement("option", {
-                                key: e,
-                                value: e
-                            }, e)
-                        }))))
-                    }));
-                    return s.default.createElement("div", {
-                        className: "col-enum"
-                    }, s.default.createElement("table", null, s.default.createElement("thead", null, s.default.createElement("tr", null, l.map((function(e) {
-                        return s.default.createElement("th", null, e)
-                    })))), s.default.createElement("tbody", null, s.default.createElement("tr", null, h))))
-                }
-                return s.default.createElement("h3", null, " unknown argtype ")
-            };
-            t.OperationAdder = function(e) {
-                var t = e.column,
-                    o = e.addOperationCb,
-                    n = e.defaultArgs;
-                return s.default.createElement("div", {
-                    className: "operation-adder"
-                }, s.default.createElement("span", {
-                    className: "column-name"
-                }, " Column: ", t), s.default.createElement("fieldset", null, a.default.keys(n).map((function(e) {
-                    return s.default.createElement("button", {
-                        key: e,
-                        onClick: (r = e, function() {
-                            var e, i = n[r];
-                            o(("col", e = t, i.map((function(t) {
-                                return "col" === t ? e : t
-                            }))))
-                        })
-                    }, " ", e, " ");
-                    var r
-                }))))
-            }
-        },
         699: (e, t) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.bakedArgSpecs = t.symDf = void 0, t.symDf = {
                 symbol: "df"
             }, t.bakedArgSpecs = {
@@ -33465,341 +33287,14 @@
                 ],
                 resample: [
                     [3, "frequency", "enum", ["daily", "weekly", "monthly"]],
                     [4, "colMap", "colEnum", ["null", "sum", "mean", "count"]]
                 ]
             }
         },
-        6978: function(e, t, o) {
-            "use strict";
-            var n = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
-                    void 0 === n && (n = o);
-                    var r = Object.getOwnPropertyDescriptor(t, o);
-                    r && !("get" in r ? !t.__esModule : r.writable || r.configurable) || (r = {
-                        enumerable: !0,
-                        get: function() {
-                            return t[o]
-                        }
-                    }), Object.defineProperty(e, n, r)
-                } : function(e, t, o, n) {
-                    void 0 === n && (n = o), e[n] = t[o]
-                }),
-                r = this && this.__setModuleDefault || (Object.create ? function(e, t) {
-                    Object.defineProperty(e, "default", {
-                        enumerable: !0,
-                        value: t
-                    })
-                } : function(e, t) {
-                    e.default = t
-                }),
-                i = this && this.__importStar || function(e) {
-                    if (e && e.__esModule) return e;
-                    var t = {};
-                    if (null != e)
-                        for (var o in e) "default" !== o && Object.prototype.hasOwnProperty.call(e, o) && n(t, e, o);
-                    return r(t, e), t
-                },
-                s = this && this.__awaiter || function(e, t, o, n) {
-                    return new(o || (o = Promise))((function(r, i) {
-                        function s(e) {
-                            try {
-                                l(n.next(e))
-                            } catch (e) {
-                                i(e)
-                            }
-                        }
-
-                        function a(e) {
-                            try {
-                                l(n.throw(e))
-                            } catch (e) {
-                                i(e)
-                            }
-                        }
-
-                        function l(e) {
-                            var t;
-                            e.done ? r(e.value) : (t = e.value, t instanceof o ? t : new o((function(e) {
-                                e(t)
-                            }))).then(s, a)
-                        }
-                        l((n = n.apply(e, t || [])).next())
-                    }))
-                },
-                a = this && this.__generator || function(e, t) {
-                    var o, n, r, i, s = {
-                        label: 0,
-                        sent: function() {
-                            if (1 & r[0]) throw r[1];
-                            return r[1]
-                        },
-                        trys: [],
-                        ops: []
-                    };
-                    return i = {
-                        next: a(0),
-                        throw: a(1),
-                        return: a(2)
-                    }, "function" == typeof Symbol && (i[Symbol.iterator] = function() {
-                        return this
-                    }), i;
-
-                    function a(i) {
-                        return function(a) {
-                            return function(i) {
-                                if (o) throw new TypeError("Generator is already executing.");
-                                for (; s;) try {
-                                    if (o = 1, n && (r = 2 & i[0] ? n.return : i[0] ? n.throw || ((r = n.return) && r.call(n), 0) : n.next) && !(r = r.call(n, i[1])).done) return r;
-                                    switch (n = 0, r && (i = [2 & i[0], r.value]), i[0]) {
-                                        case 0:
-                                        case 1:
-                                            r = i;
-                                            break;
-                                        case 4:
-                                            return s.label++, {
-                                                value: i[1],
-                                                done: !1
-                                            };
-                                        case 5:
-                                            s.label++, n = i[1], i = [0];
-                                            continue;
-                                        case 7:
-                                            i = s.ops.pop(), s.trys.pop();
-                                            continue;
-                                        default:
-                                            if (!((r = (r = s.trys).length > 0 && r[r.length - 1]) || 6 !== i[0] && 2 !== i[0])) {
-                                                s = 0;
-                                                continue
-                                            }
-                                            if (3 === i[0] && (!r || i[1] > r[0] && i[1] < r[3])) {
-                                                s.label = i[1];
-                                                break
-                                            }
-                                            if (6 === i[0] && s.label < r[1]) {
-                                                s.label = r[1], r = i;
-                                                break
-                                            }
-                                            if (r && s.label < r[2]) {
-                                                s.label = r[2], s.ops.push(i);
-                                                break
-                                            }
-                                            r[2] && s.ops.pop(), s.trys.pop();
-                                            continue
-                                    }
-                                    i = t.call(e, s)
-                                } catch (e) {
-                                    i = [6, e], n = 0
-                                } finally {
-                                    o = r = 0
-                                }
-                                if (5 & i[0]) throw i[1];
-                                return {
-                                    value: i[0] ? i[1] : void 0,
-                                    done: !0
-                                }
-                            }([i, a])
-                        }
-                    }
-                },
-                l = this && this.__read || function(e, t) {
-                    var o = "function" == typeof Symbol && e[Symbol.iterator];
-                    if (!o) return e;
-                    var n, r, i = o.call(e),
-                        s = [];
-                    try {
-                        for (;
-                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
-                    } catch (e) {
-                        r = {
-                            error: e
-                        }
-                    } finally {
-                        try {
-                            n && !n.done && (o = i.return) && o.call(i)
-                        } finally {
-                            if (r) throw r.error
-                        }
-                    }
-                    return s
-                },
-                u = this && this.__spreadArray || function(e, t, o) {
-                    if (o || 2 === arguments.length)
-                        for (var n, r = 0, i = t.length; r < i; r++) !n && r in t || (n || (n = Array.prototype.slice.call(t, 0, r)), n[r] = t[r]);
-                    return e.concat(n || Array.prototype.slice.call(t))
-                },
-                c = this && this.__importDefault || function(e) {
-                    return e && e.__esModule ? e : {
-                        default: e
-                    }
-                };
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), t.Commands = t.OperationViewer = t.OperationsList = void 0;
-            var p = i(o(7294)),
-                d = c(o(4439)),
-                h = o(5727),
-                f = o(6467),
-                g = o(4e3),
-                v = o(4646);
-            o(9423), o(3054);
-            var y = o(3800),
-                m = function(e) {
-                    return d.default.map(Array.from(e.entries()), (function(e) {
-                        var t = l(e, 2),
-                            o = t[0],
-                            n = t[1][0].symbol;
-                        return {
-                            field: n + o.toString(),
-                            headerName: n
-                        }
-                    }))
-                };
-            t.OperationsList = function(e) {
-                var t = e.operations,
-                    o = e.activeKey,
-                    n = e.setActiveKey,
-                    r = d.default.map(Array.from(t.entries()), (function(e) {
-                        var t = l(e, 2),
-                            o = t[0],
-                            n = t[1],
-                            r = {};
-                        return r[n[0].symbol + o.toString()] = n[2], r
-                    })),
-                    i = [d.default.merge.apply(d.default, u([{}], l(r), !1))],
-                    s = m(t),
-                    a = (0, v.updateAtMatch)(d.default.clone(s), o || "___never", {
-                        cellStyle: {
-                            background: "var(--ag-range-selection-background-color-3)"
-                        }
-                    }, {
-                        cellStyle: {}
-                    }),
-                    c = {
-                        rowSelection: "single",
-                        headerHeight: 30,
-                        onCellClicked: function(e) {
-                            var t = e.column.getColId();
-                            n(t)
-                        }
-                    };
-                return p.default.createElement("div", {
-                    style: {
-                        height: 78,
-                        width: 1e3
-                    },
-                    className: "ag-theme-alpine"
-                }, p.default.createElement(g.AgGridReact, {
-                    gridOptions: c,
-                    rowData: i,
-                    columnDefs: a
-                }))
-            }, t.OperationViewer = function(e) {
-                var o, n = e.operations,
-                    r = e.setOperations,
-                    i = e.activeColumn,
-                    s = e.allColumns,
-                    a = e.commandConfig,
-                    c = d.default.map(Array.from(n.entries()), (function(e) {
-                        var t = l(e, 2),
-                            o = t[0],
-                            n = t[1],
-                            r = {};
-                        return r[n[0].symbol + o.toString()] = n, r
-                    })),
-                    h = d.default.merge.apply(d.default, u([{}], l(c), !1)),
-                    g = d.default.map(Array.from(n.entries()), (function(e) {
-                        var t = l(e, 2),
-                            o = t[0],
-                            n = {};
-                        return n[t[1][0].symbol + o.toString()] = o, n
-                    })),
-                    v = d.default.merge.apply(d.default, u([{}], l(g), !1)),
-                    y = l((0, p.useState)(""), 2),
-                    C = y[0],
-                    w = y[1],
-                    S = a.argspecs,
-                    E = a.defaultArgs;
-                return p.default.createElement("div", {
-                    className: "command-viewer"
-                }, p.default.createElement(f.OperationAdder, {
-                    column: i,
-                    addOperationCb: function(e) {
-                        var t = u(u([], l(n), !1), [e], !1);
-                        r(t);
-                        var o = m(t)[t.length - 1].field;
-                        void 0 !== o && w(o)
-                    },
-                    defaultArgs: E
-                }), p.default.createElement("div", {
-                    className: "operations-box"
-                }, p.default.createElement("h4", null, " Operations "), p.default.createElement(t.OperationsList, {
-                    operations: n,
-                    activeKey: C,
-                    setActiveKey: w
-                })), C && p.default.createElement(f.OperationDetail, {
-                    command: h[C],
-                    setCommand: (o = C, function(e) {
-                        var t = v[o],
-                            i = n.map((function(o, n) {
-                                return n === t ? e : o
-                            }));
-                        r(i)
-                    }),
-                    deleteCB: function(e) {
-                        return function() {
-                            var t = v[e],
-                                o = n.map((function(e, o) {
-                                    return o === t ? void 0 : e
-                                }));
-                            w(""), r(d.default.filter(o))
-                        }
-                    }(C),
-                    columns: s,
-                    commandPatterns: S
-                }))
-            }, t.Commands = function() {
-                var e = l((0, p.useState)(y.bakedOperations), 2),
-                    o = e[0],
-                    n = e[1],
-                    r = l((0, p.useState)(h.bakedCommandConfig), 2),
-                    i = r[0],
-                    u = r[1];
-                return (0, p.useEffect)((function() {
-                    fetch("http://localhost:5000/dcf/command-config").then((function(e) {
-                        return s(void 0, void 0, void 0, (function() {
-                            var t;
-                            return a(this, (function(o) {
-                                switch (o.label) {
-                                    case 0:
-                                        return t = u, [4, e.json()];
-                                    case 1:
-                                        return t.apply(void 0, [o.sent()]), [2]
-                                }
-                            }))
-                        }))
-                    }))
-                }), []), p.default.createElement("div", {
-                    style: {
-                        width: "100%",
-                        height: "100%"
-                    }
-                }, p.default.createElement(t.OperationViewer, {
-                    operations: o,
-                    setOperations: n,
-                    activeColumn: "new-column2",
-                    allColumns: ["foo-col", "bar-col", "baz-col"],
-                    commandConfig: i
-                }), p.default.createElement("code", {
-                    style: {
-                        fontSize: "1em",
-                        textAlign: "left"
-                    }
-                }, " ", JSON.stringify(o, null, "\t\n\r"), " "))
-            }
-        },
         3925: function(e, t, o) {
             "use strict";
             var n = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
                     void 0 === n && (n = o);
                     var r = Object.getOwnPropertyDescriptor(t, o);
                     r && !("get" in r ? !t.__esModule : r.writable || r.configurable) || (r = {
                         enumerable: !0,
@@ -33952,70 +33447,76 @@
                 value: !0
             }), t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
             var u = i(o(7294)),
                 c = o(7137),
                 p = o(379),
                 d = o(3800),
                 h = o(9249),
-                f = o(5727),
-                g = o(6230);
+                f = o(668),
+                g = o(5727),
+                v = o(6230);
 
-            function v(e) {
+            function y(e) {
                 var t = e.origDf,
                     o = e.getOrRequester,
                     n = e.commandConfig,
                     r = e.exposeCommandConfigSetter,
-                    i = l((0, u.useState)(n), 2),
-                    s = i[0];
-                r(i[1]);
-                var a = l((0, u.useState)("stoptime"), 2),
-                    c = a[0],
-                    d = a[1];
+                    i = e.dfConfig,
+                    s = e.on_dfConfig,
+                    a = l((0, u.useState)(n), 2),
+                    c = a[0];
+                r(a[1]);
+                var d = l((0, u.useState)("stoptime"), 2),
+                    g = d[0],
+                    v = d[1];
                 return u.default.createElement("div", {
                     className: "dcf-root flex flex-col",
                     style: {
                         width: "100%",
                         height: "100%"
                     }
                 }, u.default.createElement("div", {
                     className: "orig-df flex flex-row",
                     style: {
-                        height: "250px",
+                        height: "300px",
                         overflow: "hidden"
                     }
-                }, u.default.createElement(h.DFViewer, {
+                }, u.default.createElement(f.StatusBar, {
+                    config: i,
+                    setConfig: s
+                }), u.default.createElement(h.DFViewer, {
                     df: t,
-                    activeCol: c,
-                    setActiveCol: d
+                    activeCol: g,
+                    setActiveCol: v
                 })), u.default.createElement(p.ColumnsEditor, {
                     df: t,
-                    activeColumn: c,
+                    activeColumn: g,
                     getOrRequester: o,
-                    commandConfig: s
+                    commandConfig: c
                 }))
             }
             t.DCFCell = function() {
                 var e = this,
                     t = l((0, u.useState)(d.tableDf), 2),
                     o = t[0],
                     n = t[1];
                 (0, u.useEffect)((function() {
-                    (0, g.requestDf)("http://localhost:5000/dcf/df/1?slice_end=50", n)
+                    (0, v.requestDf)("http://localhost:5000/dcf/df/1?slice_end=50", n)
                 }), []);
-                var r = l((0, u.useState)(f.bakedCommandConfig), 2),
+                var r = l((0, u.useState)(g.bakedCommandConfig), 2),
                     i = r[0],
-                    v = r[1];
+                    f = r[1];
                 (0, u.useEffect)((function() {
                     fetch("http://localhost:5000/dcf/command-config").then((function(t) {
                         return s(e, void 0, void 0, (function() {
                             var e;
                             return a(this, (function(o) {
                                 switch (o.label) {
                                     case 0:
-                                        return e = v, [4, t.json()];
+                                        return e = f, [4, t.json()];
                                     case 1:
                                         return e.apply(void 0, [o.sent()]), [2]
                                 }
                             }))
                         }))
                     }))
                 }), []);
@@ -34040,22 +33541,34 @@
                     setActiveCol: C
                 })), u.default.createElement(p.ColumnsEditor, {
                     df: o,
                     activeColumn: m,
                     getOrRequester: c.serverGetTransformRequester,
                     commandConfig: i
                 }))
-            }, t.WidgetDCFCell = v, t.WidgetDCFCellExample = function() {
-                return u.default.createElement(v, {
+            }, t.WidgetDCFCell = y, t.WidgetDCFCellExample = function() {
+                var e = l((0, u.useState)({
+                        totalRows: 1309,
+                        columns: 30,
+                        rowsShown: 500,
+                        sampleSize: 1e4,
+                        summaryStats: !1,
+                        reorderdColumns: !1
+                    }), 2),
+                    t = e[0],
+                    o = e[1];
+                return u.default.createElement(y, {
                     origDf: d.tableDf,
                     getOrRequester: c.serverGetTransformRequester,
                     exposeCommandConfigSetter: function(e) {
                         return console.log("exposeCommandConfigSetter called with", e)
                     },
-                    commandConfig: f.bakedCommandConfig
+                    commandConfig: g.bakedCommandConfig,
+                    dfConfig: t,
+                    on_dfConfig: o
                 })
             }
         },
         9249: function(e, t, o) {
             "use strict";
             var n = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
                     void 0 === n && (n = o);
@@ -34148,35 +33661,43 @@
                         },
                         onCellClicked: function(e) {
                             var t = e.column.getColId();
                             void 0 !== r && void 0 !== t && r(t)
                         }
                     },
                     v = (0, l.useRef)(null);
-                return (0, l.useEffect)((function() {
-                    var e = setTimeout((function() {
-                        v.current.columnApi.autoSizeAllColumns()
-                    }), 150);
-                    return function() {
-                        return clearTimeout(e)
+                return function(e, t) {
+                    var o = 50,
+                        n = !1,
+                        r = -10;
+                    if (void 0 === v || null === v.current) r = 200;
+                    else try {
+                        var i = v.current.columnApi.getAllDisplayedColumns();
+                        r = 0 !== i.length ? i[0].getActualWidth() : 200
+                    } catch (e) {
+                        console.log("88, gridref not defined yet", e)
                     }
-                }), [v]), u.default.isEqual(o, c.EmptyDf) ? l.default.createElement("div", {
-                    className: "df-viewer"
-                }, l.default.createElement("div", {
-                    style: {
-                        height: 500,
-                        width: 2500
-                    },
-                    className: "theme-hanger ag-theme-alpine-dark"
-                })) : l.default.createElement("div", {
+                    var s = function() {
+                        if (void 0 !== v && void 0 !== v.current && null !== v.current && void 0 !== v.current.columnApi) {
+                            v.current.columnApi.autoSizeAllColumns();
+                            var e = v.current.columnApi.getAllDisplayedColumns();
+                            if (0 !== e.length) {
+                                var t = e[0].getActualWidth();
+                                !1 === n ? (r = t, n = !0) : r = t
+                            }
+                            v.current.forceUpdate()
+                        }
+                        return o > 0 && !1 === n || o > 0 && 200 === r ? (o -= 1, void setTimeout(s, 10)) : void 0
+                    };
+                    setTimeout(s, 10)
+                }(), l.default.createElement("div", {
                     className: "df-viewer"
                 }, l.default.createElement("div", {
                     style: {
-                        height: 500,
-                        width: 2500
+                        height: 500
                     },
                     className: "theme-hanger ag-theme-alpine-dark"
                 }, l.default.createElement(d.AgGridReact, {
                     ref: v,
                     gridOptions: g,
                     rowData: h,
                     columnDefs: f
@@ -34383,14 +33904,159 @@
                     DataFrame: c.default.createElement(C, {
                         style: h,
                         transformedDf: i.transformed_df
                     })
                 } [p]))
             }
         },
+        8626: function(e, t, o) {
+            "use strict";
+            var n = this && this.__read || function(e, t) {
+                    var o = "function" == typeof Symbol && e[Symbol.iterator];
+                    if (!o) return e;
+                    var n, r, i = o.call(e),
+                        s = [];
+                    try {
+                        for (;
+                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
+                    } catch (e) {
+                        r = {
+                            error: e
+                        }
+                    } finally {
+                        try {
+                            n && !n.done && (o = i.return) && o.call(i)
+                        } finally {
+                            if (r) throw r.error
+                        }
+                    }
+                    return s
+                },
+                r = this && this.__importDefault || function(e) {
+                    return e && e.__esModule ? e : {
+                        default: e
+                    }
+                };
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.ArgGetters = t.OperationDetail = void 0;
+            var i = r(o(7294)),
+                s = r(o(4439)),
+                a = o(6230);
+            t.OperationDetail = function(e) {
+                var o = e.command,
+                    n = e.setCommand,
+                    r = e.deleteCB,
+                    a = e.columns,
+                    l = e.commandPatterns;
+                if (void 0 === o) return i.default.createElement("h2", null, " error undefined command ");
+                var u = o[0].symbol,
+                    c = l[u];
+                if (s.default.isArray(c)) {
+                    if (s.default.isEqual(c, [null])) return i.default.createElement("div", {
+                        className: "operation-detail"
+                    }, i.default.createElement("button", {
+                        onClick: r
+                    }, "X"));
+                    var p = c;
+                    return i.default.createElement("div", {
+                        className: "operation-detail"
+                    }, i.default.createElement(t.ArgGetters, {
+                        command: o,
+                        fullPattern: p,
+                        setCommand: n,
+                        columns: a,
+                        deleteCB: r
+                    }))
+                }
+                return i.default.createElement("h2", null, "unknown command ", u)
+            }, t.ArgGetters = function(e) {
+                var t = e.command,
+                    o = e.fullPattern,
+                    n = e.setCommand,
+                    r = e.columns,
+                    s = e.deleteCB;
+                return i.default.createElement("div", {
+                    className: "arg-getters"
+                }, i.default.createElement("button", {
+                    onClick: s
+                }, "X"), o.map((function(e) {
+                    var o = e[0],
+                        s = t[o];
+                    return i.default.createElement("div", {
+                        key: o
+                    }, i.default.createElement(l, {
+                        argProps: e,
+                        val: s,
+                        setter: function(e) {
+                            var r = (0, a.replaceAtIdx)(t, o, e);
+                            n(r)
+                        },
+                        columns: r
+                    }))
+                })))
+            };
+            var l = function(e) {
+                var t = e.argProps,
+                    o = e.val,
+                    r = e.setter,
+                    l = e.columns,
+                    u = n(t, 4),
+                    c = (u[0], u[1]),
+                    p = u[2],
+                    d = u[3];
+                if ("enum" === p) return i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("select", {
+                    defaultValue: o,
+                    onChange: function(e) {
+                        return r(e.target.value)
+                    }
+                }, d.map((function(e) {
+                    return i.default.createElement("option", {
+                        key: e,
+                        value: e
+                    }, e)
+                }))));
+                if ("type" === p) return "integer" === d ? i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("input", {
+                    type: "number",
+                    defaultValue: o,
+                    step: "1",
+                    onChange: function(e) {
+                        return r(parseInt(e.target.value))
+                    }
+                })) : i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("input", {
+                    value: "dont know"
+                }));
+                if ("colEnum" === p) {
+                    var h = l.map((function(e) {
+                        var t = s.default.get(o, e, "null");
+                        return i.default.createElement("td", null, i.default.createElement("select", {
+                            defaultValue: t,
+                            onChange: function(t) {
+                                var n = t.target.value;
+                                if (s.default.isString(n)) {
+                                    var i = (0, a.replaceAtKey)(o, e, n);
+                                    r((0, a.objWithoutNull)(i, ["null"]))
+                                }
+                            }
+                        }, d.map((function(e) {
+                            return i.default.createElement("option", {
+                                key: e,
+                                value: e
+                            }, e)
+                        }))))
+                    }));
+                    return i.default.createElement("div", {
+                        className: "col-enum"
+                    }, i.default.createElement("table", null, i.default.createElement("thead", null, i.default.createElement("tr", null, l.map((function(e) {
+                        return i.default.createElement("th", null, e)
+                    })))), i.default.createElement("tbody", null, i.default.createElement("tr", null, h))))
+                }
+                return i.default.createElement("h3", null, " unknown argtype ")
+            }
+        },
         3643: (e, t, o) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.bakedOperations = t.sym = void 0;
             var n = o(699);
             t.sym = function(e) {
@@ -34399,14 +34065,501 @@
                 }
             }, (0, t.sym)("nonexistent"), (0, t.sym)("df"), t.bakedOperations = [
                 [(0, t.sym)("dropcol"), n.symDf, "col1"],
                 [(0, t.sym)("fillna"), n.symDf, "col2", 5],
                 [(0, t.sym)("resample"), n.symDf, "month", "monthly", {}]
             ]
         },
+        8002: function(e, t, o) {
+            "use strict";
+            var n = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
+                    void 0 === n && (n = o);
+                    var r = Object.getOwnPropertyDescriptor(t, o);
+                    r && !("get" in r ? !t.__esModule : r.writable || r.configurable) || (r = {
+                        enumerable: !0,
+                        get: function() {
+                            return t[o]
+                        }
+                    }), Object.defineProperty(e, n, r)
+                } : function(e, t, o, n) {
+                    void 0 === n && (n = o), e[n] = t[o]
+                }),
+                r = this && this.__setModuleDefault || (Object.create ? function(e, t) {
+                    Object.defineProperty(e, "default", {
+                        enumerable: !0,
+                        value: t
+                    })
+                } : function(e, t) {
+                    e.default = t
+                }),
+                i = this && this.__importStar || function(e) {
+                    if (e && e.__esModule) return e;
+                    var t = {};
+                    if (null != e)
+                        for (var o in e) "default" !== o && Object.prototype.hasOwnProperty.call(e, o) && n(t, e, o);
+                    return r(t, e), t
+                },
+                s = this && this.__awaiter || function(e, t, o, n) {
+                    return new(o || (o = Promise))((function(r, i) {
+                        function s(e) {
+                            try {
+                                l(n.next(e))
+                            } catch (e) {
+                                i(e)
+                            }
+                        }
+
+                        function a(e) {
+                            try {
+                                l(n.throw(e))
+                            } catch (e) {
+                                i(e)
+                            }
+                        }
+
+                        function l(e) {
+                            var t;
+                            e.done ? r(e.value) : (t = e.value, t instanceof o ? t : new o((function(e) {
+                                e(t)
+                            }))).then(s, a)
+                        }
+                        l((n = n.apply(e, t || [])).next())
+                    }))
+                },
+                a = this && this.__generator || function(e, t) {
+                    var o, n, r, i, s = {
+                        label: 0,
+                        sent: function() {
+                            if (1 & r[0]) throw r[1];
+                            return r[1]
+                        },
+                        trys: [],
+                        ops: []
+                    };
+                    return i = {
+                        next: a(0),
+                        throw: a(1),
+                        return: a(2)
+                    }, "function" == typeof Symbol && (i[Symbol.iterator] = function() {
+                        return this
+                    }), i;
+
+                    function a(i) {
+                        return function(a) {
+                            return function(i) {
+                                if (o) throw new TypeError("Generator is already executing.");
+                                for (; s;) try {
+                                    if (o = 1, n && (r = 2 & i[0] ? n.return : i[0] ? n.throw || ((r = n.return) && r.call(n), 0) : n.next) && !(r = r.call(n, i[1])).done) return r;
+                                    switch (n = 0, r && (i = [2 & i[0], r.value]), i[0]) {
+                                        case 0:
+                                        case 1:
+                                            r = i;
+                                            break;
+                                        case 4:
+                                            return s.label++, {
+                                                value: i[1],
+                                                done: !1
+                                            };
+                                        case 5:
+                                            s.label++, n = i[1], i = [0];
+                                            continue;
+                                        case 7:
+                                            i = s.ops.pop(), s.trys.pop();
+                                            continue;
+                                        default:
+                                            if (!((r = (r = s.trys).length > 0 && r[r.length - 1]) || 6 !== i[0] && 2 !== i[0])) {
+                                                s = 0;
+                                                continue
+                                            }
+                                            if (3 === i[0] && (!r || i[1] > r[0] && i[1] < r[3])) {
+                                                s.label = i[1];
+                                                break
+                                            }
+                                            if (6 === i[0] && s.label < r[1]) {
+                                                s.label = r[1], r = i;
+                                                break
+                                            }
+                                            if (r && s.label < r[2]) {
+                                                s.label = r[2], s.ops.push(i);
+                                                break
+                                            }
+                                            r[2] && s.ops.pop(), s.trys.pop();
+                                            continue
+                                    }
+                                    i = t.call(e, s)
+                                } catch (e) {
+                                    i = [6, e], n = 0
+                                } finally {
+                                    o = r = 0
+                                }
+                                if (5 & i[0]) throw i[1];
+                                return {
+                                    value: i[0] ? i[1] : void 0,
+                                    done: !0
+                                }
+                            }([i, a])
+                        }
+                    }
+                },
+                l = this && this.__read || function(e, t) {
+                    var o = "function" == typeof Symbol && e[Symbol.iterator];
+                    if (!o) return e;
+                    var n, r, i = o.call(e),
+                        s = [];
+                    try {
+                        for (;
+                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
+                    } catch (e) {
+                        r = {
+                            error: e
+                        }
+                    } finally {
+                        try {
+                            n && !n.done && (o = i.return) && o.call(i)
+                        } finally {
+                            if (r) throw r.error
+                        }
+                    }
+                    return s
+                },
+                u = this && this.__spreadArray || function(e, t, o) {
+                    if (o || 2 === arguments.length)
+                        for (var n, r = 0, i = t.length; r < i; r++) !n && r in t || (n || (n = Array.prototype.slice.call(t, 0, r)), n[r] = t[r]);
+                    return e.concat(n || Array.prototype.slice.call(t))
+                },
+                c = this && this.__importDefault || function(e) {
+                    return e && e.__esModule ? e : {
+                        default: e
+                    }
+                };
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.Commands = t.OperationViewer = t.OperationAdder = t.OperationsList = void 0;
+            var p = i(o(7294)),
+                d = c(o(4439)),
+                h = o(6230),
+                f = o(5727),
+                g = o(8626),
+                v = o(4e3),
+                y = o(4646);
+            o(9423), o(3054);
+            var m = o(3800),
+                C = function(e) {
+                    return d.default.map(Array.from(e.entries()), (function(e) {
+                        var t = l(e, 2),
+                            o = t[0],
+                            n = t[1][0].symbol;
+                        return {
+                            field: n + o.toString(),
+                            headerName: n
+                        }
+                    }))
+                };
+            t.OperationsList = function(e) {
+                var t = e.operations,
+                    o = e.activeKey,
+                    n = e.setActiveKey,
+                    r = d.default.map(Array.from(t.entries()), (function(e) {
+                        var t = l(e, 2),
+                            o = t[0],
+                            n = t[1],
+                            r = {};
+                        return r[n[0].symbol + o.toString()] = n[2], r
+                    })),
+                    i = [d.default.merge.apply(d.default, u([{}], l(r), !1))],
+                    s = C(t),
+                    a = (0, y.updateAtMatch)(d.default.clone(s), o || "___never", {
+                        cellStyle: {
+                            background: "var(--ag-range-selection-background-color-3)"
+                        }
+                    }, {
+                        cellStyle: {}
+                    }),
+                    c = {
+                        rowSelection: "single",
+                        headerHeight: 30,
+                        onCellClicked: function(e) {
+                            var t = e.column.getColId();
+                            n(t)
+                        }
+                    };
+                return p.default.createElement("div", {
+                    style: {
+                        height: 78,
+                        width: 1e3
+                    },
+                    className: "ag-theme-alpine"
+                }, p.default.createElement(v.AgGridReact, {
+                    gridOptions: c,
+                    rowData: i,
+                    columnDefs: a
+                }))
+            }, t.OperationAdder = function(e) {
+                var t = e.column,
+                    o = e.addOperationCb,
+                    n = e.defaultArgs;
+                return p.default.createElement("div", {
+                    className: "operation-adder"
+                }, p.default.createElement("span", {
+                    className: "column-name"
+                }, " Column: ", t), p.default.createElement("fieldset", null, d.default.keys(n).map((function(e) {
+                    return p.default.createElement("button", {
+                        key: e,
+                        onClick: (r = e, function() {
+                            var e = n[r];
+                            o((0, h.replaceInArr)(e, "col", t))
+                        })
+                    }, " ", e, " ");
+                    var r
+                }))))
+            }, t.OperationViewer = function(e) {
+                var o, n = e.operations,
+                    r = e.setOperations,
+                    i = e.activeColumn,
+                    s = e.allColumns,
+                    a = e.commandConfig,
+                    c = d.default.map(Array.from(n.entries()), (function(e) {
+                        var t = l(e, 2),
+                            o = t[0],
+                            n = t[1],
+                            r = {};
+                        return r[n[0].symbol + o.toString()] = n, r
+                    })),
+                    h = d.default.merge.apply(d.default, u([{}], l(c), !1)),
+                    f = d.default.map(Array.from(n.entries()), (function(e) {
+                        var t = l(e, 2),
+                            o = t[0],
+                            n = {};
+                        return n[t[1][0].symbol + o.toString()] = o, n
+                    })),
+                    v = d.default.merge.apply(d.default, u([{}], l(f), !1)),
+                    y = l((0, p.useState)(""), 2),
+                    m = y[0],
+                    w = y[1],
+                    S = a.argspecs,
+                    E = a.defaultArgs;
+                return p.default.createElement("div", {
+                    className: "command-viewer"
+                }, p.default.createElement(t.OperationAdder, {
+                    column: i,
+                    addOperationCb: function(e) {
+                        var t = u(u([], l(n), !1), [e], !1);
+                        r(t);
+                        var o = C(t)[t.length - 1].field;
+                        void 0 !== o && w(o)
+                    },
+                    defaultArgs: E
+                }), p.default.createElement("div", {
+                    className: "operations-box"
+                }, p.default.createElement("h4", null, " Operations "), p.default.createElement(t.OperationsList, {
+                    operations: n,
+                    activeKey: m,
+                    setActiveKey: w
+                })), m && p.default.createElement(g.OperationDetail, {
+                    command: h[m],
+                    setCommand: (o = m, function(e) {
+                        var t = v[o],
+                            i = n.map((function(o, n) {
+                                return n === t ? e : o
+                            }));
+                        r(i)
+                    }),
+                    deleteCB: function(e) {
+                        return function() {
+                            var t = v[e],
+                                o = n.map((function(e, o) {
+                                    return o === t ? void 0 : e
+                                }));
+                            w(""), r(d.default.filter(o))
+                        }
+                    }(m),
+                    columns: s,
+                    commandPatterns: S
+                }))
+            }, t.Commands = function() {
+                var e = l((0, p.useState)(m.bakedOperations), 2),
+                    o = e[0],
+                    n = e[1],
+                    r = l((0, p.useState)(f.bakedCommandConfig), 2),
+                    i = r[0],
+                    u = r[1];
+                return (0, p.useEffect)((function() {
+                    fetch("http://localhost:5000/dcf/command-config").then((function(e) {
+                        return s(void 0, void 0, void 0, (function() {
+                            var t;
+                            return a(this, (function(o) {
+                                switch (o.label) {
+                                    case 0:
+                                        return t = u, [4, e.json()];
+                                    case 1:
+                                        return t.apply(void 0, [o.sent()]), [2]
+                                }
+                            }))
+                        }))
+                    }))
+                }), []), p.default.createElement("div", {
+                    style: {
+                        width: "100%",
+                        height: "100%"
+                    }
+                }, p.default.createElement(t.OperationViewer, {
+                    operations: o,
+                    setOperations: n,
+                    activeColumn: "new-column2",
+                    allColumns: ["foo-col", "bar-col", "baz-col"],
+                    commandConfig: i
+                }), p.default.createElement("code", {
+                    style: {
+                        fontSize: "1em",
+                        textAlign: "left"
+                    }
+                }, " ", JSON.stringify(o, null, "\t\n\r"), " "))
+            }
+        },
+        668: function(e, t, o) {
+            "use strict";
+            var n = this && this.__assign || function() {
+                    return n = Object.assign || function(e) {
+                        for (var t, o = 1, n = arguments.length; o < n; o++)
+                            for (var r in t = arguments[o]) Object.prototype.hasOwnProperty.call(t, r) && (e[r] = t[r]);
+                        return e
+                    }, n.apply(this, arguments)
+                },
+                r = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
+                    void 0 === n && (n = o);
+                    var r = Object.getOwnPropertyDescriptor(t, o);
+                    r && !("get" in r ? !t.__esModule : r.writable || r.configurable) || (r = {
+                        enumerable: !0,
+                        get: function() {
+                            return t[o]
+                        }
+                    }), Object.defineProperty(e, n, r)
+                } : function(e, t, o, n) {
+                    void 0 === n && (n = o), e[n] = t[o]
+                }),
+                i = this && this.__setModuleDefault || (Object.create ? function(e, t) {
+                    Object.defineProperty(e, "default", {
+                        enumerable: !0,
+                        value: t
+                    })
+                } : function(e, t) {
+                    e.default = t
+                }),
+                s = this && this.__importStar || function(e) {
+                    if (e && e.__esModule) return e;
+                    var t = {};
+                    if (null != e)
+                        for (var o in e) "default" !== o && Object.prototype.hasOwnProperty.call(e, o) && r(t, e, o);
+                    return i(t, e), t
+                },
+                a = this && this.__read || function(e, t) {
+                    var o = "function" == typeof Symbol && e[Symbol.iterator];
+                    if (!o) return e;
+                    var n, r, i = o.call(e),
+                        s = [];
+                    try {
+                        for (;
+                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
+                    } catch (e) {
+                        r = {
+                            error: e
+                        }
+                    } finally {
+                        try {
+                            n && !n.done && (o = i.return) && o.call(i)
+                        } finally {
+                            if (r) throw r.error
+                        }
+                    }
+                    return s
+                };
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.StatusBarEx = t.StatusBar = void 0;
+            var l = s(o(7294)),
+                u = o(4e3),
+                c = [{
+                    field: "totalRows"
+                }, {
+                    field: "columns"
+                }, {
+                    field: "rowsShown"
+                }, {
+                    field: "sampleSize"
+                }, {
+                    field: "summaryStats"
+                }, {
+                    field: "reorderdColumns"
+                }];
+
+            function p(e) {
+                var t = e.config,
+                    o = e.setConfig,
+                    r = t.totalRows,
+                    i = t.columns,
+                    s = t.rowsShown,
+                    a = t.sampleSize,
+                    p = t.summaryStats,
+                    d = t.reorderdColumns,
+                    h = [{
+                        totalRows: r,
+                        columns: i,
+                        rowsShown: s,
+                        sampleSize: a,
+                        summaryStats: p.toString(),
+                        reorderdColumns: d.toString()
+                    }],
+                    f = (0, l.useRef)(null);
+                return l.default.createElement("div", {
+                    className: "statusBar"
+                }, l.default.createElement("div", {
+                    style: {
+                        height: 50
+                    },
+                    className: "theme-hanger ag-theme-alpine-dark"
+                }, l.default.createElement(u.AgGridReact, {
+                    ref: f,
+                    onCellClicked: function(e) {
+                        var r = e.column.getColId();
+                        "summaryStats" === r ? o(n(n({}, t), {
+                            summaryStats: !t.summaryStats
+                        })) : "reorderdColumns" === r && o(n(n({}, t), {
+                            reorderdColumns: !t.reorderdColumns
+                        }))
+                    },
+                    gridOptions: {
+                        rowSelection: "single"
+                    },
+                    defaultColDef: {
+                        type: "left-aligned",
+                        cellStyle: {
+                            textAlign: "left"
+                        }
+                    },
+                    rowData: h,
+                    columnDefs: c
+                })))
+            }
+            t.StatusBar = p, t.StatusBarEx = function() {
+                var e = a((0, l.useState)({
+                        totalRows: 1309,
+                        columns: 30,
+                        rowsShown: 500,
+                        sampleSize: 1e4,
+                        summaryStats: !1,
+                        reorderdColumns: !1
+                    }), 2),
+                    t = e[0],
+                    o = e[1];
+                return l.default.createElement(p, {
+                    config: t,
+                    setConfig: o
+                })
+            }
+        },
         5727: (e, t, o) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.bakedCommandConfig = t.bakedOperationDefaults = void 0;
             var n = o(6230),
                 r = o(699);
@@ -34555,17 +34708,17 @@
                     "start station latitude": 40.73652889,
                     bikeid: 20062,
                     "birth year": "1972",
                     gender: 2
                 }]
             }
         },
-        6230: function(e, t) {
+        6230: function(e, t, o) {
             "use strict";
-            var o = this && this.__awaiter || function(e, t, o, n) {
+            var n = this && this.__awaiter || function(e, t, o, n) {
                     return new(o || (o = Promise))((function(r, i) {
                         function s(e) {
                             try {
                                 l(n.next(e))
                             } catch (e) {
                                 i(e)
                             }
@@ -34584,15 +34737,15 @@
                             e.done ? r(e.value) : (t = e.value, t instanceof o ? t : new o((function(e) {
                                 e(t)
                             }))).then(s, a)
                         }
                         l((n = n.apply(e, t || [])).next())
                     }))
                 },
-                n = this && this.__generator || function(e, t) {
+                r = this && this.__generator || function(e, t) {
                     var o, n, r, i, s = {
                         label: 0,
                         sent: function() {
                             if (1 & r[0]) throw r[1];
                             return r[1]
                         },
                         trys: [],
@@ -34658,35 +34811,83 @@
                                 return {
                                     value: i[0] ? i[1] : void 0,
                                     done: !0
                                 }
                             }([i, a])
                         }
                     }
+                },
+                i = this && this.__read || function(e, t) {
+                    var o = "function" == typeof Symbol && e[Symbol.iterator];
+                    if (!o) return e;
+                    var n, r, i = o.call(e),
+                        s = [];
+                    try {
+                        for (;
+                            (void 0 === t || t-- > 0) && !(n = i.next()).done;) s.push(n.value)
+                    } catch (e) {
+                        r = {
+                            error: e
+                        }
+                    } finally {
+                        try {
+                            n && !n.done && (o = i.return) && o.call(i)
+                        } finally {
+                            if (r) throw r.error
+                        }
+                    }
+                    return s
+                },
+                s = this && this.__spreadArray || function(e, t, o) {
+                    if (o || 2 === arguments.length)
+                        for (var n, r = 0, i = t.length; r < i; r++) !n && r in t || (n || (n = Array.prototype.slice.call(t, 0, r)), n[r] = t[r]);
+                    return e.concat(n || Array.prototype.slice.call(t))
+                },
+                a = this && this.__importDefault || function(e) {
+                    return e && e.__esModule ? e : {
+                        default: e
+                    }
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t.sym = t.requestDf = void 0, t.requestDf = function(e, t) {
+            }), t.objWithoutNull = t.replaceAtKey = t.replaceAtIdx = t.replaceInArr = t.sym = t.requestDf = void 0;
+            var l = a(o(4439));
+            t.requestDf = function(e, t) {
                 return fetch(e).then((function(e) {
-                    return o(void 0, void 0, void 0, (function() {
+                    return n(void 0, void 0, void 0, (function() {
                         var o;
-                        return n(this, (function(n) {
+                        return r(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return [4, e.json()];
                                 case 1:
                                     return o = n.sent(), t(o), [2]
                             }
                         }))
                     }))
                 }))
             }, t.sym = function(e) {
                 return {
                     symbol: e
                 }
+            }, t.replaceInArr = function(e, t, o) {
+                return e.map((function(e) {
+                    return e === t ? o : e
+                }))
+            }, t.replaceAtIdx = function(e, t, o) {
+                return e.map((function(e, n) {
+                    return n === t ? o : e
+                }))
+            }, t.replaceAtKey = function(e, t, o) {
+                var n = l.default.clone(e);
+                return n[t] = o, n
+            }, t.objWithoutNull = function(e, t) {
+                return void 0 === t && (t = []), l.default.pickBy(e, (function(e) {
+                    return !s([null, void 0], i(t), !1).includes(e)
+                }))
             }
         },
         7116: function(e, t, o) {
             "use strict";
             var n = this && this.__createBinding || (Object.create ? function(e, t, o, n) {
                     void 0 === n && (n = o);
                     var r = Object.getOwnPropertyDescriptor(t, o);
@@ -34712,15 +34913,15 @@
                     var t = {};
                     if (null != e)
                         for (var o in e) "default" !== o && Object.prototype.hasOwnProperty.call(e, o) && n(t, e, o);
                     return r(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t.DFViewer = t.CommandUtils = t.DependentTabs = t.CommandsComponent = t.ColumnsEditor = t.OperationUtils = t.staticData = t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
+            }), t.StatusBar = t.DFViewer = t.CommandUtils = t.DependentTabs = t.CommandsComponent = t.ColumnsEditor = t.OperationUtils = t.staticData = t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
             var s = o(3925);
             Object.defineProperty(t, "DCFCell", {
                 enumerable: !0,
                 get: function() {
                     return s.DCFCell
                 }
             }), Object.defineProperty(t, "WidgetDCFCell", {
@@ -34729,22 +34930,22 @@
                     return s.WidgetDCFCell
                 }
             }), Object.defineProperty(t, "WidgetDCFCellExample", {
                 enumerable: !0,
                 get: function() {
                     return s.WidgetDCFCellExample
                 }
-            }), t.staticData = i(o(3800)), t.OperationUtils = i(o(3643)), t.ColumnsEditor = i(o(379)), t.CommandsComponent = i(o(6978)), t.DependentTabs = i(o(7137)), t.CommandUtils = i(o(699));
+            }), t.staticData = i(o(3800)), t.OperationUtils = i(o(3643)), t.ColumnsEditor = i(o(379)), t.CommandsComponent = i(o(8002)), t.DependentTabs = i(o(7137)), t.CommandUtils = i(o(699));
             var a = o(9249);
             Object.defineProperty(t, "DFViewer", {
                 enumerable: !0,
                 get: function() {
                     return a.DFViewer
                 }
-            })
+            }), t.StatusBar = i(o(668))
         },
         2703: (e, t, o) => {
             "use strict";
             var n = o(414);
 
             function r() {}
```

### Comparing `dcef-0.2.3/dcef/labextension/static/116.2c99b074fd692e5d339c.js.LICENSE.txt` & `dcef-0.2.5/dcef/labextension/static/116.f2c748ce51e22b52b0cb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js` & `dcef-0.2.5/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js.LICENSE.txt` & `dcef-0.2.5/dcef/labextension/static/250.ca3c9f855fbc1747d0ae.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/labextension/static/480.c629752d1a4021a728bb.js` & `dcef-0.2.5/dcef/labextension/static/568.b3c25a51cdf2e2d0b274.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,127 +1,125 @@
 (self.webpackChunkdcef = self.webpackChunkdcef || []).push([
-    [480], {
+    [568], {
         8399: function(e, n, t) {
             "use strict";
-            var o = this && this.__importDefault || function(e) {
-                return e && e.__esModule ? e : {
-                    default: e
-                }
-            };
+            var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
+                    void 0 === o && (o = t), Object.defineProperty(e, o, {
+                        enumerable: !0,
+                        get: function() {
+                            return n[t]
+                        }
+                    })
+                } : function(e, n, t, o) {
+                    void 0 === o && (o = t), e[o] = n[t]
+                }),
+                i = this && this.__setModuleDefault || (Object.create ? function(e, n) {
+                    Object.defineProperty(e, "default", {
+                        enumerable: !0,
+                        value: n
+                    })
+                } : function(e, n) {
+                    e.default = n
+                }),
+                l = this && this.__importStar || function(e) {
+                    if (e && e.__esModule) return e;
+                    var n = {};
+                    if (null != e)
+                        for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
+                    return i(n, e), n
+                };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.DCEFWidgetView = n.DCEFWidgetModel = void 0;
-            const i = t(2492),
-                l = t(9694),
-                a = t(745),
-                r = o(t(7294)),
-                s = t(8657);
+            const a = t(2492),
+                s = t(2156),
+                r = l(t(7294)),
+                d = l(t(745)),
+                u = t(8657);
             t(9423), t(3054), t(4260), t(801);
-            class d extends i.DOMWidgetModel {
+            class c extends a.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: d.model_name,
-                        _model_module: d.model_module,
-                        _model_module_version: d.model_module_version,
-                        _view_name: d.view_name,
-                        _view_module: d.view_module,
-                        _view_module_version: d.view_module_version,
-                        command_config: {},
-                        commands: [],
-                        operation_results: {}
+                        _model_name: c.model_name,
+                        _model_module: c.model_module,
+                        _model_module_version: c.model_module_version,
+                        _view_name: c.view_name,
+                        _view_module: c.view_module,
+                        _view_module_version: c.view_module_version,
+                        commandConfig: {},
+                        operations: [],
+                        operation_results: {},
+                        dfConfig: {}
                     })
                 }
             }
-            n.DCEFWidgetModel = d, d.serializers = Object.assign({}, i.DOMWidgetModel.serializers), d.model_name = "DCEFWidgetModel", d.model_module = s.MODULE_NAME, d.model_module_version = s.MODULE_VERSION, d.view_name = "ExampleView", d.view_module = s.MODULE_NAME, d.view_module_version = s.MODULE_VERSION;
-            class u extends i.DOMWidgetView {
+            n.DCEFWidgetModel = c, c.serializers = Object.assign({}, a.DOMWidgetModel.serializers), c.model_name = "DCEFWidgetModel", c.model_module = u.MODULE_NAME, c.model_module_version = u.MODULE_VERSION, c.view_name = "ExampleView", c.view_module = u.MODULE_NAME, c.view_module_version = u.MODULE_VERSION;
+            class p extends a.DOMWidgetView {
                 constructor() {
-                    super(...arguments), this.setCommandConfig = e => {
-                        console.log("default setCommandConfig")
-                    }, this.setPyCode = e => {
-                        console.log("default setPyCode")
-                    }, this.setTransformedDf = e => {
-                        console.log("default setTransformedDf")
-                    }
+                    super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
                 }
                 render() {
-                    console.log("DCFWidget View... renamed "), this.el.classList.add("custom-widget");
-                    const e = a.createRoot(this.el),
-                        n = this.model,
-                        t = this;
-                    n.on("change:command_config", (() => {
-                        t.setCommandConfig(n.get("command_config"))
+                    this.el.classList.add("custom-widget");
+                    const e = this.model,
+                        n = this;
+                    e.on("change:commandConfig", (() => {
+                        n.setCommandConfig(e.get("commandConfig"))
                     }), this);
-                    const o = n.get("command_config");
-                    console.log("widget, commandConfig", o, n);
-                    const i = r.default.createElement(l.WidgetDCFCell, {
-                        origDf: n.get("js_df"),
-                        getOrRequester: e => (n.on("change:operation_results", (() => {
-                            const t = n.get("operation_results");
-                            console.log("about to call setOpResult with", t), e(t)
-                        }), this), e => {
-                            console.log("orRequester passed operations", e), n.set("commands", e), n.save_changes()
-                        }),
-                        commandConfig: o,
-                        exposeCommandConfigSetter: e => {
-                            t.setCommandConfig = e
-                        }
-                    }, null);
-                    e.render(i)
+                    const t = {
+                            getOrRequester: n => (e.on("change:operation_results", (() => {
+                                const t = e.get("operation_results");
+                                console.log("about to call setOpResult with", t), n(t)
+                            }), this), n => {
+                                console.log("orRequester passed operations", n), e.set("operations", n), e.save_changes()
+                            }),
+                            exposeCommandConfigSetter: e => {
+                                n.setCommandConfig = e
+                            }
+                        },
+                        o = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                        i = this.el.getBoundingClientRect().y,
+                        l = o.getBoundingClientRect().y - i + 50;
+                    o.scroll(0, l);
+                    const a = d.createRoot(this.el),
+                        u = r.default.createElement((() => {
+                            const [e, n] = r.useState(0), o = () => {
+                                n((e => e + 1))
+                            };
+                            r.useEffect((() => {
+                                this.listenTo(this.model, "change", o)
+                            }), []);
+                            const i = Object.assign({}, t);
+                            for (const e of Object.keys(this.model.attributes)) i[e] = this.model.get(e), i["on_" + e] = n => {
+                                this.model.set(e, n), this.touch()
+                            };
+                            return r.default.createElement(s.WidgetDCFCell, i)
+                        }), {});
+                    a.render(u)
                 }
             }
-            n.DCEFWidgetView = u
+            n.DCEFWidgetView = p
         },
-        4480: function(e, n, t) {
+        1568: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
                             return n[t]
                         }
                     })
                 } : function(e, n, t, o) {
                     void 0 === o && (o = t), e[o] = n[t]
                 }),
-                i = this && this.__setModuleDefault || (Object.create ? function(e, n) {
-                    Object.defineProperty(e, "default", {
-                        enumerable: !0,
-                        value: n
-                    })
-                } : function(e, n) {
-                    e.default = n
-                }),
-                l = this && this.__importStar || function(e) {
-                    if (e && e.__esModule) return e;
-                    var n = {};
-                    if (null != e)
-                        for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
-                    return i(n, e), n
+                i = this && this.__exportStar || function(e, n) {
+                    for (var t in e) "default" === t || Object.prototype.hasOwnProperty.call(n, t) || o(n, e, t)
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
-            });
-            const a = t(2492),
-                r = t(3033),
-                s = t(8657),
-                d = l(t(8399)),
-                u = {
-                    id: "dcef:plugin",
-                    requires: [a.IJupyterWidgetRegistry],
-                    optional: [r.IThemeManager],
-                    activate: function(e, n, t) {
-                        console.log("dcef_widget plugin.ts after change EXTENSION_ID"), n.registerWidget({
-                            name: s.MODULE_NAME,
-                            version: s.MODULE_VERSION,
-                            exports: Object.assign({}, d)
-                        })
-                    },
-                    autoStart: !0
-                };
-            n.default = u
+            }), i(t(8657), n), i(t(8399), n)
         },
         8657: (e, n, t) => {
             "use strict";
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.MODULE_NAME = n.MODULE_VERSION = void 0;
             const o = t(4147);
@@ -158,11 +156,11 @@
                 hmr: !0,
                 transform: void 0,
                 insertInto: void 0
             }), o.locals && (e.exports = o.locals)
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.25","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.33","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `dcef-0.2.3/dcef/labextension/static/486.0708227d0a518f636636.js` & `dcef-0.2.5/dcef/labextension/static/486.0708227d0a518f636636.js`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/labextension/static/568.8b4e60cfe6905d620fad.js` & `dcef-0.2.5/dcef/labextension/static/480.ccd73b95e569f66845e5.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,155 @@
 (self.webpackChunkdcef = self.webpackChunkdcef || []).push([
-    [568], {
+    [480], {
         8399: function(e, n, t) {
             "use strict";
-            var o = this && this.__importDefault || function(e) {
-                return e && e.__esModule ? e : {
-                    default: e
-                }
-            };
+            var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
+                    void 0 === o && (o = t), Object.defineProperty(e, o, {
+                        enumerable: !0,
+                        get: function() {
+                            return n[t]
+                        }
+                    })
+                } : function(e, n, t, o) {
+                    void 0 === o && (o = t), e[o] = n[t]
+                }),
+                i = this && this.__setModuleDefault || (Object.create ? function(e, n) {
+                    Object.defineProperty(e, "default", {
+                        enumerable: !0,
+                        value: n
+                    })
+                } : function(e, n) {
+                    e.default = n
+                }),
+                l = this && this.__importStar || function(e) {
+                    if (e && e.__esModule) return e;
+                    var n = {};
+                    if (null != e)
+                        for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
+                    return i(n, e), n
+                };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.DCEFWidgetView = n.DCEFWidgetModel = void 0;
-            const l = t(2492),
-                i = t(9694),
-                a = t(745),
-                s = o(t(7294)),
-                r = t(8657);
+            const a = t(2492),
+                r = t(2156),
+                s = l(t(7294)),
+                d = l(t(745)),
+                u = t(8657);
             t(9423), t(3054), t(4260), t(801);
-            class d extends l.DOMWidgetModel {
+            class c extends a.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: d.model_name,
-                        _model_module: d.model_module,
-                        _model_module_version: d.model_module_version,
-                        _view_name: d.view_name,
-                        _view_module: d.view_module,
-                        _view_module_version: d.view_module_version,
-                        command_config: {},
-                        commands: [],
-                        operation_results: {}
+                        _model_name: c.model_name,
+                        _model_module: c.model_module,
+                        _model_module_version: c.model_module_version,
+                        _view_name: c.view_name,
+                        _view_module: c.view_module,
+                        _view_module_version: c.view_module_version,
+                        commandConfig: {},
+                        operations: [],
+                        operation_results: {},
+                        dfConfig: {}
                     })
                 }
             }
-            n.DCEFWidgetModel = d, d.serializers = Object.assign({}, l.DOMWidgetModel.serializers), d.model_name = "DCEFWidgetModel", d.model_module = r.MODULE_NAME, d.model_module_version = r.MODULE_VERSION, d.view_name = "ExampleView", d.view_module = r.MODULE_NAME, d.view_module_version = r.MODULE_VERSION;
-            class u extends l.DOMWidgetView {
+            n.DCEFWidgetModel = c, c.serializers = Object.assign({}, a.DOMWidgetModel.serializers), c.model_name = "DCEFWidgetModel", c.model_module = u.MODULE_NAME, c.model_module_version = u.MODULE_VERSION, c.view_name = "ExampleView", c.view_module = u.MODULE_NAME, c.view_module_version = u.MODULE_VERSION;
+            class p extends a.DOMWidgetView {
                 constructor() {
-                    super(...arguments), this.setCommandConfig = e => {
-                        console.log("default setCommandConfig")
-                    }, this.setPyCode = e => {
-                        console.log("default setPyCode")
-                    }, this.setTransformedDf = e => {
-                        console.log("default setTransformedDf")
-                    }
+                    super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
                 }
                 render() {
-                    console.log("DCFWidget View... renamed "), this.el.classList.add("custom-widget");
-                    const e = a.createRoot(this.el),
-                        n = this.model,
-                        t = this;
-                    n.on("change:command_config", (() => {
-                        t.setCommandConfig(n.get("command_config"))
+                    this.el.classList.add("custom-widget");
+                    const e = this.model,
+                        n = this;
+                    e.on("change:commandConfig", (() => {
+                        n.setCommandConfig(e.get("commandConfig"))
                     }), this);
-                    const o = n.get("command_config");
-                    console.log("widget, commandConfig", o, n);
-                    const l = s.default.createElement(i.WidgetDCFCell, {
-                        origDf: n.get("js_df"),
-                        getOrRequester: e => (n.on("change:operation_results", (() => {
-                            const t = n.get("operation_results");
-                            console.log("about to call setOpResult with", t), e(t)
-                        }), this), e => {
-                            console.log("orRequester passed operations", e), n.set("commands", e), n.save_changes()
-                        }),
-                        commandConfig: o,
-                        exposeCommandConfigSetter: e => {
-                            t.setCommandConfig = e
-                        }
-                    }, null);
-                    e.render(l)
+                    const t = {
+                            getOrRequester: n => (e.on("change:operation_results", (() => {
+                                const t = e.get("operation_results");
+                                console.log("about to call setOpResult with", t), n(t)
+                            }), this), n => {
+                                console.log("orRequester passed operations", n), e.set("operations", n), e.save_changes()
+                            }),
+                            exposeCommandConfigSetter: e => {
+                                n.setCommandConfig = e
+                            }
+                        },
+                        o = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                        i = this.el.getBoundingClientRect().y,
+                        l = o.getBoundingClientRect().y - i + 50;
+                    o.scroll(0, l);
+                    const a = d.createRoot(this.el),
+                        u = s.default.createElement((() => {
+                            const [e, n] = s.useState(0), o = () => {
+                                n((e => e + 1))
+                            };
+                            s.useEffect((() => {
+                                this.listenTo(this.model, "change", o)
+                            }), []);
+                            const i = Object.assign({}, t);
+                            for (const e of Object.keys(this.model.attributes)) i[e] = this.model.get(e), i["on_" + e] = n => {
+                                this.model.set(e, n), this.touch()
+                            };
+                            return s.default.createElement(r.WidgetDCFCell, i)
+                        }), {});
+                    a.render(u)
                 }
             }
-            n.DCEFWidgetView = u
+            n.DCEFWidgetView = p
         },
-        1568: function(e, n, t) {
+        4480: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
                             return n[t]
                         }
                     })
                 } : function(e, n, t, o) {
                     void 0 === o && (o = t), e[o] = n[t]
                 }),
-                l = this && this.__exportStar || function(e, n) {
-                    for (var t in e) "default" === t || Object.prototype.hasOwnProperty.call(n, t) || o(n, e, t)
+                i = this && this.__setModuleDefault || (Object.create ? function(e, n) {
+                    Object.defineProperty(e, "default", {
+                        enumerable: !0,
+                        value: n
+                    })
+                } : function(e, n) {
+                    e.default = n
+                }),
+                l = this && this.__importStar || function(e) {
+                    if (e && e.__esModule) return e;
+                    var n = {};
+                    if (null != e)
+                        for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
+                    return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
-            }), l(t(8657), n), l(t(8399), n)
+            });
+            const a = t(2492),
+                r = t(3033),
+                s = t(8657),
+                d = l(t(8399)),
+                u = {
+                    id: "dcef:plugin",
+                    requires: [a.IJupyterWidgetRegistry],
+                    optional: [r.IThemeManager],
+                    activate: function(e, n, t) {
+                        console.log("dcef_widget plugin.ts after change EXTENSION_ID"), n.registerWidget({
+                            name: s.MODULE_NAME,
+                            version: s.MODULE_VERSION,
+                            exports: Object.assign({}, d)
+                        })
+                    },
+                    autoStart: !0
+                };
+            n.default = u
         },
         8657: (e, n, t) => {
             "use strict";
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.MODULE_NAME = n.MODULE_VERSION = void 0;
             const o = t(4147);
@@ -128,11 +186,11 @@
                 hmr: !0,
                 transform: void 0,
                 insertInto: void 0
             }), o.locals && (e.exports = o.locals)
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.25","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.33","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `dcef-0.2.3/dcef/labextension/static/remoteEntry.e5d1fdcb371ac4cc9f68.js` & `dcef-0.2.5/dcef/labextension/static/remoteEntry.e97dd4f5ff7087528b29.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, f, l, d, u, s, c, p, h, v, b, m, g = {
+    var e, r, t, n, a, o, i, d, l, f, u, s, c, p, h, v, b, m, g = {
             8699: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(250), t.e(41), t.e(568)]).then((() => () => t(1568))),
-                        "./extension": () => Promise.all([t.e(250), t.e(41), t.e(480)]).then((() => () => t(4480)))
+                        "./index": () => Promise.all([t.e(250), t.e(933), t.e(568)]).then((() => () => t(1568))),
+                        "./extension": () => Promise.all([t.e(250), t.e(933), t.e(480)]).then((() => () => t(4480)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         y = {};
 
     function w(e) {
         var r = y[e];
@@ -38,89 +38,89 @@
     }
     w.m = g, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        41: "92df930318f60b3c0b13",
-        116: "2c99b074fd692e5d339c",
+        116: "f2c748ce51e22b52b0cb",
         250: "ca3c9f855fbc1747d0ae",
         439: "7d7d3f19781fd5feb401",
-        480: "c629752d1a4021a728bb",
+        480: "ccd73b95e569f66845e5",
         486: "0708227d0a518f636636",
-        568: "8b4e60cfe6905d620fad"
+        568: "b3c25a51cdf2e2d0b274",
+        933: "cc4c0e56aefc9b598d57"
     } [e] + ".js?v=" + {
-        41: "92df930318f60b3c0b13",
-        116: "2c99b074fd692e5d339c",
+        116: "f2c748ce51e22b52b0cb",
         250: "ca3c9f855fbc1747d0ae",
         439: "7d7d3f19781fd5feb401",
-        480: "c629752d1a4021a728bb",
+        480: "ccd73b95e569f66845e5",
         486: "0708227d0a518f636636",
-        568: "8b4e60cfe6905d620fad"
+        568: "b3c25a51cdf2e2d0b274",
+        933: "cc4c0e56aefc9b598d57"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dcef:", w.l = (t, n, o, a) => {
+    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dcef:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, f;
-            if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var u = l[d];
-                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + o) {
+            var i, d;
+            if (void 0 !== a)
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var u = l[f];
+                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + a) {
                         i = u;
                         break
                     }
                 }
-            i || (f = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), f && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, w.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         w.S = {};
         var e = {},
             r = {};
         w.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
-                var a = w.S[t],
+                var o = w.S[t],
                     i = "dcef",
-                    f = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            f = o[r];
-                        (!f || !f.loaded && (!n != !f.eager ? n : i > f.from)) && (o[r] = {
+                    d = (e, r, t, n) => {
+                        var a = o[e] = o[e] || {},
+                            d = a[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (f("dcef", "0.2.1", (() => Promise.all([w.e(250), w.e(41), w.e(568)]).then((() => () => w(1568))))), f("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), f("paddy-react-edit-list", "1.1.25", (() => Promise.all([w.e(250), w.e(116), w.e(439)]).then((() => () => w(7116)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("dcef", "0.2.1", (() => Promise.all([w.e(250), w.e(933), w.e(568)]).then((() => () => w(1568))))), d("lodash", "4.17.21", (() => w.e(486).then((() => () => w(6486))))), d("paddy-react-edit-list", "1.1.33", (() => Promise.all([w.e(250), w.e(116), w.e(439)]).then((() => () => w(7116)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -134,160 +134,160 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
-                f = (typeof i)[0];
-            if (a != f) return "o" == a && "n" == f || "s" == f || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+                d = (typeof i)[0];
+            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(f = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, f);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var f = e[a];
-            i.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? i.pop() + " " + i.pop() : o(f))
+        for (o = 1; o < e.length; o++) {
+            var d = e[o];
+            i.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? i.pop() + " " + i.pop() : a(d))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
-            for (var i = 0, f = 1, l = !0;; f++, i++) {
-                var d, u, s = f < e.length ? (typeof e[f])[0] : "";
-                if (i >= r.length || "o" == (u = (typeof(d = r[i]))[0])) return !l || ("u" == s ? f > n && !o : "" == s != o);
+                a = n < 0;
+            a && (n = -n - 1);
+            for (var i = 0, d = 1, l = !0;; d++, i++) {
+                var f, u, s = d < e.length ? (typeof e[d])[0] : "";
+                if (i >= r.length || "o" == (u = (typeof(f = r[i]))[0])) return !l || ("u" == s ? d > n && !a : "" == s != a);
                 if ("u" == u) {
                     if (!l || "u" != s) return !1
                 } else if (l)
                     if (s == u)
-                        if (f <= n) {
-                            if (d != e[f]) return !1
+                        if (d <= n) {
+                            if (f != e[d]) return !1
                         } else {
-                            if (o ? d > e[f] : d < e[f]) return !1;
-                            d != e[f] && (l = !1)
+                            if (a ? f > e[d] : f < e[d]) return !1;
+                            f != e[d] && (l = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (o || f <= n) return !1;
-                    l = !1, f--
+                    if (a || d <= n) return !1;
+                    l = !1, d--
                 } else {
-                    if (f <= n || u < s != o) return !1;
+                    if (d <= n || u < s != a) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, f--)
+                } else "s" != s && "n" != s && (l = !1, d--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, f = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
-        var o = f(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+        var a = d(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), s(e[t][a])
     }, u = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, o) {
-        var a = w.I(r);
-        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = c(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && u(r, t, n);
-        return a ? s(a) : o()
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
+        var o = w.I(r);
+        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && u(r, t, n);
+        return o ? s(o) : a()
     })), v = {}, b = {
+        2156: () => h("default", "paddy-react-edit-list", [0, 1, 1, 33], (() => Promise.all([w.e(116), w.e(439)]).then((() => () => w(7116))))),
         2492: () => p("default", "@jupyter-widgets/base", [, [1, 6, 0, 0],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1
         ]),
-        9694: () => h("default", "paddy-react-edit-list", [0, 1, 1, 25], (() => Promise.all([w.e(116), w.e(439)]).then((() => () => w(7116))))),
         3033: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         4439: () => h("default", "lodash", [1, 4, 17, 21], (() => w.e(486).then((() => () => w(6486)))))
     }, m = {
-        41: [2492, 9694],
         439: [4439],
-        480: [3033]
+        480: [3033],
+        933: [2156, 2492]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var o = b[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var a = b[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             49: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^4(1|39)$/.test(r)) e[r] = 0;
+                else if (/^(439|933)$/.test(r)) e[r] = 0;
             else {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = w.p + w.u(r),
+                var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                t.push(n[2] = a);
+                var o = w.p + w.u(r),
                     i = new Error;
-                w.l(a, (t => {
+                w.l(o, (t => {
                     if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, o, [a, i, f] = t,
+                var n, a, [o, i, d] = t,
                     l = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
-                    f && f(w)
+                    d && d(w)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkdcef = self.webpackChunkdcef || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
     var S = w(8699);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).dcef = S
 })();
```

### Comparing `dcef-0.2.3/dcef/labextension/static/third-party-licenses.json` & `dcef-0.2.5/dcef/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'packages'": "{4: {'versionInfo': '1.1.33'}}"}*

```diff
@@ -24,15 +24,15 @@
             "name": "lodash",
             "versionInfo": "4.17.21"
         },
         {
             "extractedText": "ISC License\n\nCopyright (c) 2022, Momtchil Momtchev <momtchil@momtchev.com>\n\nPermission to use, copy, modify, and/or distribute this software for any\npurpose with or without fee is hereby granted, provided that the above\ncopyright notice and this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES\nWITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF\nMERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR\nANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES\nWHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN\nACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF\nOR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.",
             "licenseId": "ISC",
             "name": "paddy-react-edit-list",
-            "versionInfo": "1.1.25"
+            "versionInfo": "1.1.33"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2013-present, Facebook, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "prop-types",
             "versionInfo": "15.8.1"
         },
```

### Comparing `dcef-0.2.3/dcef/nbextension/index.js` & `dcef-0.2.5/dcef/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -36969,15 +36969,15 @@
                         return a
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.ColumnsEditor = void 0;
                 var s = i(n(6255)),
                     l = n(1475),
-                    u = n(1840),
+                    u = n(4710),
                     c = n(3308),
                     p = n(5732);
                 t.ColumnsEditor = function(e) {
                     var t = void 0 === e ? {
                             df: l.EmptyDf,
                             activeColumn: "stoptime",
                             getOrRequester: p.serverGetTransformRequester,
@@ -37006,192 +37006,14 @@
                         commandConfig: i
                     }), s.default.createElement(p.DependentTabs, {
                         filledOperations: g,
                         getOrRequester: o
                     }))
                 }
             },
-            591: function(e, t, n) {
-                "use strict";
-                var r = this && this.__read || function(e, t) {
-                        var n = "function" == typeof Symbol && e[Symbol.iterator];
-                        if (!n) return e;
-                        var r, o, i = n.call(e),
-                            a = [];
-                        try {
-                            for (;
-                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
-                        } catch (e) {
-                            o = {
-                                error: e
-                            }
-                        } finally {
-                            try {
-                                r && !r.done && (n = i.return) && n.call(i)
-                            } finally {
-                                if (o) throw o.error
-                            }
-                        }
-                        return a
-                    },
-                    o = this && this.__spreadArray || function(e, t, n) {
-                        if (n || 2 === arguments.length)
-                            for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
-                        return e.concat(r || Array.prototype.slice.call(t))
-                    },
-                    i = this && this.__importDefault || function(e) {
-                        return e && e.__esModule ? e : {
-                            default: e
-                        }
-                    };
-                Object.defineProperty(t, "__esModule", {
-                    value: !0
-                }), t.OperationAdder = t.ArgGetters = t.OperationDetail = void 0;
-                var a = i(n(6255)),
-                    s = i(n(2275));
-                t.OperationDetail = function(e) {
-                    var n = e.command,
-                        r = e.setCommand,
-                        o = e.deleteCB,
-                        i = e.columns,
-                        l = e.commandPatterns;
-                    if (void 0 === n) return a.default.createElement("h2", null, " error undefined command ");
-                    var u = n[0].symbol,
-                        c = l[u];
-                    if (s.default.isArray(c)) {
-                        if (s.default.isEqual(c, [null])) return a.default.createElement("div", {
-                            className: "operation-detail"
-                        }, a.default.createElement("button", {
-                            onClick: o
-                        }, "X"));
-                        var p = c;
-                        return a.default.createElement("div", {
-                            className: "operation-detail"
-                        }, a.default.createElement(t.ArgGetters, {
-                            command: n,
-                            fullPattern: p,
-                            setCommand: r,
-                            columns: i,
-                            deleteCB: o
-                        }))
-                    }
-                    return a.default.createElement("h2", null, "unknown command ", u)
-                }, t.ArgGetters = function(e) {
-                    var t = e.command,
-                        n = e.fullPattern,
-                        r = e.setCommand,
-                        o = e.columns,
-                        i = e.deleteCB;
-                    return a.default.createElement("div", {
-                        className: "arg-getters"
-                    }, a.default.createElement("button", {
-                        onClick: i
-                    }, "X"), n.map((function(e) {
-                        var n = e[0],
-                            i = t[n];
-                        return a.default.createElement("div", {
-                            key: n
-                        }, a.default.createElement(l, {
-                            argProps: e,
-                            val: i,
-                            setter: function(e) {
-                                var o = function(e, t, n) {
-                                    return e.map((function(e, r) {
-                                        return r === t ? n : e
-                                    }))
-                                }(t, n, e);
-                                r(o)
-                            },
-                            columns: o
-                        }))
-                    })))
-                };
-                var l = function(e) {
-                    var t = e.argProps,
-                        n = e.val,
-                        i = e.setter,
-                        l = e.columns,
-                        u = r(t, 4),
-                        c = (u[0], u[1]),
-                        p = u[2],
-                        d = u[3];
-                    if ("enum" === p) return a.default.createElement("fieldset", null, a.default.createElement("label", null, " ", c, " "), a.default.createElement("select", {
-                        defaultValue: n,
-                        onChange: function(e) {
-                            return i(e.target.value)
-                        }
-                    }, d.map((function(e) {
-                        return a.default.createElement("option", {
-                            key: e,
-                            value: e
-                        }, e)
-                    }))));
-                    if ("type" === p) return "integer" === d ? a.default.createElement("fieldset", null, a.default.createElement("label", null, " ", c, " "), a.default.createElement("input", {
-                        type: "number",
-                        defaultValue: n,
-                        step: "1",
-                        onChange: function(e) {
-                            return i(parseInt(e.target.value))
-                        }
-                    })) : a.default.createElement("fieldset", null, a.default.createElement("label", null, " ", c, " "), a.default.createElement("input", {
-                        value: "dont know"
-                    }));
-                    if ("colEnum" === p) {
-                        var g = l.map((function(e) {
-                            var t = s.default.get(n, e, "null");
-                            return a.default.createElement("td", null, a.default.createElement("select", {
-                                defaultValue: t,
-                                onChange: function(t) {
-                                    var a, l, u, c, p = t.target.value;
-                                    if (s.default.isString(p)) {
-                                        var d = (a = n, l = e, u = p, (c = s.default.clone(a))[l] = u, c);
-                                        i(function(e, t) {
-                                            return void 0 === t && (t = []), s.default.pickBy(e, (function(e) {
-                                                return !o([null, void 0], r(t), !1).includes(e)
-                                            }))
-                                        }(d, ["null"]))
-                                    }
-                                }
-                            }, d.map((function(e) {
-                                return a.default.createElement("option", {
-                                    key: e,
-                                    value: e
-                                }, e)
-                            }))))
-                        }));
-                        return a.default.createElement("div", {
-                            className: "col-enum"
-                        }, a.default.createElement("table", null, a.default.createElement("thead", null, a.default.createElement("tr", null, l.map((function(e) {
-                            return a.default.createElement("th", null, e)
-                        })))), a.default.createElement("tbody", null, a.default.createElement("tr", null, g))))
-                    }
-                    return a.default.createElement("h3", null, " unknown argtype ")
-                };
-                t.OperationAdder = function(e) {
-                    var t = e.column,
-                        n = e.addOperationCb,
-                        r = e.defaultArgs;
-                    return a.default.createElement("div", {
-                        className: "operation-adder"
-                    }, a.default.createElement("span", {
-                        className: "column-name"
-                    }, " Column: ", t), a.default.createElement("fieldset", null, s.default.keys(r).map((function(e) {
-                        return a.default.createElement("button", {
-                            key: e,
-                            onClick: (o = e, function() {
-                                var e, i = r[o];
-                                n(("col", e = t, i.map((function(t) {
-                                    return "col" === t ? e : t
-                                }))))
-                            })
-                        }, " ", e, " ");
-                        var o
-                    }))))
-                }
-            },
             4176: (e, t) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.bakedArgSpecs = t.symDf = void 0, t.symDf = {
                     symbol: "df"
                 }, t.bakedArgSpecs = {
@@ -37201,341 +37023,14 @@
                     ],
                     resample: [
                         [3, "frequency", "enum", ["daily", "weekly", "monthly"]],
                         [4, "colMap", "colEnum", ["null", "sum", "mean", "count"]]
                     ]
                 }
             },
-            1840: function(e, t, n) {
-                "use strict";
-                var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
-                        void 0 === r && (r = n);
-                        var o = Object.getOwnPropertyDescriptor(t, n);
-                        o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
-                            enumerable: !0,
-                            get: function() {
-                                return t[n]
-                            }
-                        }), Object.defineProperty(e, r, o)
-                    } : function(e, t, n, r) {
-                        void 0 === r && (r = n), e[r] = t[n]
-                    }),
-                    o = this && this.__setModuleDefault || (Object.create ? function(e, t) {
-                        Object.defineProperty(e, "default", {
-                            enumerable: !0,
-                            value: t
-                        })
-                    } : function(e, t) {
-                        e.default = t
-                    }),
-                    i = this && this.__importStar || function(e) {
-                        if (e && e.__esModule) return e;
-                        var t = {};
-                        if (null != e)
-                            for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && r(t, e, n);
-                        return o(t, e), t
-                    },
-                    a = this && this.__awaiter || function(e, t, n, r) {
-                        return new(n || (n = Promise))((function(o, i) {
-                            function a(e) {
-                                try {
-                                    l(r.next(e))
-                                } catch (e) {
-                                    i(e)
-                                }
-                            }
-
-                            function s(e) {
-                                try {
-                                    l(r.throw(e))
-                                } catch (e) {
-                                    i(e)
-                                }
-                            }
-
-                            function l(e) {
-                                var t;
-                                e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
-                                    e(t)
-                                }))).then(a, s)
-                            }
-                            l((r = r.apply(e, t || [])).next())
-                        }))
-                    },
-                    s = this && this.__generator || function(e, t) {
-                        var n, r, o, i, a = {
-                            label: 0,
-                            sent: function() {
-                                if (1 & o[0]) throw o[1];
-                                return o[1]
-                            },
-                            trys: [],
-                            ops: []
-                        };
-                        return i = {
-                            next: s(0),
-                            throw: s(1),
-                            return: s(2)
-                        }, "function" == typeof Symbol && (i[Symbol.iterator] = function() {
-                            return this
-                        }), i;
-
-                        function s(i) {
-                            return function(s) {
-                                return function(i) {
-                                    if (n) throw new TypeError("Generator is already executing.");
-                                    for (; a;) try {
-                                        if (n = 1, r && (o = 2 & i[0] ? r.return : i[0] ? r.throw || ((o = r.return) && o.call(r), 0) : r.next) && !(o = o.call(r, i[1])).done) return o;
-                                        switch (r = 0, o && (i = [2 & i[0], o.value]), i[0]) {
-                                            case 0:
-                                            case 1:
-                                                o = i;
-                                                break;
-                                            case 4:
-                                                return a.label++, {
-                                                    value: i[1],
-                                                    done: !1
-                                                };
-                                            case 5:
-                                                a.label++, r = i[1], i = [0];
-                                                continue;
-                                            case 7:
-                                                i = a.ops.pop(), a.trys.pop();
-                                                continue;
-                                            default:
-                                                if (!((o = (o = a.trys).length > 0 && o[o.length - 1]) || 6 !== i[0] && 2 !== i[0])) {
-                                                    a = 0;
-                                                    continue
-                                                }
-                                                if (3 === i[0] && (!o || i[1] > o[0] && i[1] < o[3])) {
-                                                    a.label = i[1];
-                                                    break
-                                                }
-                                                if (6 === i[0] && a.label < o[1]) {
-                                                    a.label = o[1], o = i;
-                                                    break
-                                                }
-                                                if (o && a.label < o[2]) {
-                                                    a.label = o[2], a.ops.push(i);
-                                                    break
-                                                }
-                                                o[2] && a.ops.pop(), a.trys.pop();
-                                                continue
-                                        }
-                                        i = t.call(e, a)
-                                    } catch (e) {
-                                        i = [6, e], r = 0
-                                    } finally {
-                                        n = o = 0
-                                    }
-                                    if (5 & i[0]) throw i[1];
-                                    return {
-                                        value: i[0] ? i[1] : void 0,
-                                        done: !0
-                                    }
-                                }([i, s])
-                            }
-                        }
-                    },
-                    l = this && this.__read || function(e, t) {
-                        var n = "function" == typeof Symbol && e[Symbol.iterator];
-                        if (!n) return e;
-                        var r, o, i = n.call(e),
-                            a = [];
-                        try {
-                            for (;
-                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
-                        } catch (e) {
-                            o = {
-                                error: e
-                            }
-                        } finally {
-                            try {
-                                r && !r.done && (n = i.return) && n.call(i)
-                            } finally {
-                                if (o) throw o.error
-                            }
-                        }
-                        return a
-                    },
-                    u = this && this.__spreadArray || function(e, t, n) {
-                        if (n || 2 === arguments.length)
-                            for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
-                        return e.concat(r || Array.prototype.slice.call(t))
-                    },
-                    c = this && this.__importDefault || function(e) {
-                        return e && e.__esModule ? e : {
-                            default: e
-                        }
-                    };
-                Object.defineProperty(t, "__esModule", {
-                    value: !0
-                }), t.Commands = t.OperationViewer = t.OperationsList = void 0;
-                var p = i(n(6255)),
-                    d = c(n(2275)),
-                    g = n(3308),
-                    h = n(591),
-                    f = n(8891),
-                    v = n(725);
-                n(9423), n(3054);
-                var y = n(1475),
-                    m = function(e) {
-                        return d.default.map(Array.from(e.entries()), (function(e) {
-                            var t = l(e, 2),
-                                n = t[0],
-                                r = t[1][0].symbol;
-                            return {
-                                field: r + n.toString(),
-                                headerName: r
-                            }
-                        }))
-                    };
-                t.OperationsList = function(e) {
-                    var t = e.operations,
-                        n = e.activeKey,
-                        r = e.setActiveKey,
-                        o = d.default.map(Array.from(t.entries()), (function(e) {
-                            var t = l(e, 2),
-                                n = t[0],
-                                r = t[1],
-                                o = {};
-                            return o[r[0].symbol + n.toString()] = r[2], o
-                        })),
-                        i = [d.default.merge.apply(d.default, u([{}], l(o), !1))],
-                        a = m(t),
-                        s = (0, v.updateAtMatch)(d.default.clone(a), n || "___never", {
-                            cellStyle: {
-                                background: "var(--ag-range-selection-background-color-3)"
-                            }
-                        }, {
-                            cellStyle: {}
-                        }),
-                        c = {
-                            rowSelection: "single",
-                            headerHeight: 30,
-                            onCellClicked: function(e) {
-                                var t = e.column.getColId();
-                                r(t)
-                            }
-                        };
-                    return p.default.createElement("div", {
-                        style: {
-                            height: 78,
-                            width: 1e3
-                        },
-                        className: "ag-theme-alpine"
-                    }, p.default.createElement(f.AgGridReact, {
-                        gridOptions: c,
-                        rowData: i,
-                        columnDefs: s
-                    }))
-                }, t.OperationViewer = function(e) {
-                    var n, r = e.operations,
-                        o = e.setOperations,
-                        i = e.activeColumn,
-                        a = e.allColumns,
-                        s = e.commandConfig,
-                        c = d.default.map(Array.from(r.entries()), (function(e) {
-                            var t = l(e, 2),
-                                n = t[0],
-                                r = t[1],
-                                o = {};
-                            return o[r[0].symbol + n.toString()] = r, o
-                        })),
-                        g = d.default.merge.apply(d.default, u([{}], l(c), !1)),
-                        f = d.default.map(Array.from(r.entries()), (function(e) {
-                            var t = l(e, 2),
-                                n = t[0],
-                                r = {};
-                            return r[t[1][0].symbol + n.toString()] = n, r
-                        })),
-                        v = d.default.merge.apply(d.default, u([{}], l(f), !1)),
-                        y = l((0, p.useState)(""), 2),
-                        w = y[0],
-                        C = y[1],
-                        b = s.argspecs,
-                        S = s.defaultArgs;
-                    return p.default.createElement("div", {
-                        className: "command-viewer"
-                    }, p.default.createElement(h.OperationAdder, {
-                        column: i,
-                        addOperationCb: function(e) {
-                            var t = u(u([], l(r), !1), [e], !1);
-                            o(t);
-                            var n = m(t)[t.length - 1].field;
-                            void 0 !== n && C(n)
-                        },
-                        defaultArgs: S
-                    }), p.default.createElement("div", {
-                        className: "operations-box"
-                    }, p.default.createElement("h4", null, " Operations "), p.default.createElement(t.OperationsList, {
-                        operations: r,
-                        activeKey: w,
-                        setActiveKey: C
-                    })), w && p.default.createElement(h.OperationDetail, {
-                        command: g[w],
-                        setCommand: (n = w, function(e) {
-                            var t = v[n],
-                                i = r.map((function(n, r) {
-                                    return r === t ? e : n
-                                }));
-                            o(i)
-                        }),
-                        deleteCB: function(e) {
-                            return function() {
-                                var t = v[e],
-                                    n = r.map((function(e, n) {
-                                        return n === t ? void 0 : e
-                                    }));
-                                C(""), o(d.default.filter(n))
-                            }
-                        }(w),
-                        columns: a,
-                        commandPatterns: b
-                    }))
-                }, t.Commands = function() {
-                    var e = l((0, p.useState)(y.bakedOperations), 2),
-                        n = e[0],
-                        r = e[1],
-                        o = l((0, p.useState)(g.bakedCommandConfig), 2),
-                        i = o[0],
-                        u = o[1];
-                    return (0, p.useEffect)((function() {
-                        fetch("http://localhost:5000/dcf/command-config").then((function(e) {
-                            return a(void 0, void 0, void 0, (function() {
-                                var t;
-                                return s(this, (function(n) {
-                                    switch (n.label) {
-                                        case 0:
-                                            return t = u, [4, e.json()];
-                                        case 1:
-                                            return t.apply(void 0, [n.sent()]), [2]
-                                    }
-                                }))
-                            }))
-                        }))
-                    }), []), p.default.createElement("div", {
-                        style: {
-                            width: "100%",
-                            height: "100%"
-                        }
-                    }, p.default.createElement(t.OperationViewer, {
-                        operations: n,
-                        setOperations: r,
-                        activeColumn: "new-column2",
-                        allColumns: ["foo-col", "bar-col", "baz-col"],
-                        commandConfig: i
-                    }), p.default.createElement("code", {
-                        style: {
-                            fontSize: "1em",
-                            textAlign: "left"
-                        }
-                    }, " ", JSON.stringify(n, null, "\t\n\r"), " "))
-                }
-            },
             1314: function(e, t, n) {
                 "use strict";
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
                         void 0 === r && (r = n);
                         var o = Object.getOwnPropertyDescriptor(t, n);
                         o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
                             enumerable: !0,
@@ -37688,70 +37183,76 @@
                     value: !0
                 }), t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
                 var u = i(n(6255)),
                     c = n(5732),
                     p = n(3677),
                     d = n(1475),
                     g = n(1251),
-                    h = n(3308),
-                    f = n(9867);
+                    h = n(4336),
+                    f = n(3308),
+                    v = n(9867);
 
-                function v(e) {
+                function y(e) {
                     var t = e.origDf,
                         n = e.getOrRequester,
                         r = e.commandConfig,
                         o = e.exposeCommandConfigSetter,
-                        i = l((0, u.useState)(r), 2),
-                        a = i[0];
-                    o(i[1]);
-                    var s = l((0, u.useState)("stoptime"), 2),
-                        c = s[0],
-                        d = s[1];
+                        i = e.dfConfig,
+                        a = e.on_dfConfig,
+                        s = l((0, u.useState)(r), 2),
+                        c = s[0];
+                    o(s[1]);
+                    var d = l((0, u.useState)("stoptime"), 2),
+                        f = d[0],
+                        v = d[1];
                     return u.default.createElement("div", {
                         className: "dcf-root flex flex-col",
                         style: {
                             width: "100%",
                             height: "100%"
                         }
                     }, u.default.createElement("div", {
                         className: "orig-df flex flex-row",
                         style: {
-                            height: "250px",
+                            height: "300px",
                             overflow: "hidden"
                         }
-                    }, u.default.createElement(g.DFViewer, {
+                    }, u.default.createElement(h.StatusBar, {
+                        config: i,
+                        setConfig: a
+                    }), u.default.createElement(g.DFViewer, {
                         df: t,
-                        activeCol: c,
-                        setActiveCol: d
+                        activeCol: f,
+                        setActiveCol: v
                     })), u.default.createElement(p.ColumnsEditor, {
                         df: t,
-                        activeColumn: c,
+                        activeColumn: f,
                         getOrRequester: n,
-                        commandConfig: a
+                        commandConfig: c
                     }))
                 }
                 t.DCFCell = function() {
                     var e = this,
                         t = l((0, u.useState)(d.tableDf), 2),
                         n = t[0],
                         r = t[1];
                     (0, u.useEffect)((function() {
-                        (0, f.requestDf)("http://localhost:5000/dcf/df/1?slice_end=50", r)
+                        (0, v.requestDf)("http://localhost:5000/dcf/df/1?slice_end=50", r)
                     }), []);
-                    var o = l((0, u.useState)(h.bakedCommandConfig), 2),
+                    var o = l((0, u.useState)(f.bakedCommandConfig), 2),
                         i = o[0],
-                        v = o[1];
+                        h = o[1];
                     (0, u.useEffect)((function() {
                         fetch("http://localhost:5000/dcf/command-config").then((function(t) {
                             return a(e, void 0, void 0, (function() {
                                 var e;
                                 return s(this, (function(n) {
                                     switch (n.label) {
                                         case 0:
-                                            return e = v, [4, t.json()];
+                                            return e = h, [4, t.json()];
                                         case 1:
                                             return e.apply(void 0, [n.sent()]), [2]
                                     }
                                 }))
                             }))
                         }))
                     }), []);
@@ -37776,22 +37277,34 @@
                         setActiveCol: w
                     })), u.default.createElement(p.ColumnsEditor, {
                         df: n,
                         activeColumn: m,
                         getOrRequester: c.serverGetTransformRequester,
                         commandConfig: i
                     }))
-                }, t.WidgetDCFCell = v, t.WidgetDCFCellExample = function() {
-                    return u.default.createElement(v, {
+                }, t.WidgetDCFCell = y, t.WidgetDCFCellExample = function() {
+                    var e = l((0, u.useState)({
+                            totalRows: 1309,
+                            columns: 30,
+                            rowsShown: 500,
+                            sampleSize: 1e4,
+                            summaryStats: !1,
+                            reorderdColumns: !1
+                        }), 2),
+                        t = e[0],
+                        n = e[1];
+                    return u.default.createElement(y, {
                         origDf: d.tableDf,
                         getOrRequester: c.serverGetTransformRequester,
                         exposeCommandConfigSetter: function(e) {
                             return console.log("exposeCommandConfigSetter called with", e)
                         },
-                        commandConfig: h.bakedCommandConfig
+                        commandConfig: f.bakedCommandConfig,
+                        dfConfig: t,
+                        on_dfConfig: n
                     })
                 }
             },
             1251: function(e, t, n) {
                 "use strict";
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
                         void 0 === r && (r = n);
@@ -37884,35 +37397,43 @@
                             },
                             onCellClicked: function(e) {
                                 var t = e.column.getColId();
                                 void 0 !== o && void 0 !== t && o(t)
                             }
                         },
                         v = (0, l.useRef)(null);
-                    return (0, l.useEffect)((function() {
-                        var e = setTimeout((function() {
-                            v.current.columnApi.autoSizeAllColumns()
-                        }), 150);
-                        return function() {
-                            return clearTimeout(e)
+                    return function(e, t) {
+                        var n = 50,
+                            r = !1,
+                            o = -10;
+                        if (void 0 === v || null === v.current) o = 200;
+                        else try {
+                            var i = v.current.columnApi.getAllDisplayedColumns();
+                            o = 0 !== i.length ? i[0].getActualWidth() : 200
+                        } catch (e) {
+                            console.log("88, gridref not defined yet", e)
                         }
-                    }), [v]), u.default.isEqual(n, c.EmptyDf) ? l.default.createElement("div", {
-                        className: "df-viewer"
-                    }, l.default.createElement("div", {
-                        style: {
-                            height: 500,
-                            width: 2500
-                        },
-                        className: "theme-hanger ag-theme-alpine-dark"
-                    })) : l.default.createElement("div", {
+                        var a = function() {
+                            if (void 0 !== v && void 0 !== v.current && null !== v.current && void 0 !== v.current.columnApi) {
+                                v.current.columnApi.autoSizeAllColumns();
+                                var e = v.current.columnApi.getAllDisplayedColumns();
+                                if (0 !== e.length) {
+                                    var t = e[0].getActualWidth();
+                                    !1 === r ? (o = t, r = !0) : o = t
+                                }
+                                v.current.forceUpdate()
+                            }
+                            return n > 0 && !1 === r || n > 0 && 200 === o ? (n -= 1, void setTimeout(a, 10)) : void 0
+                        };
+                        setTimeout(a, 10)
+                    }(), l.default.createElement("div", {
                         className: "df-viewer"
                     }, l.default.createElement("div", {
                         style: {
-                            height: 500,
-                            width: 2500
+                            height: 500
                         },
                         className: "theme-hanger ag-theme-alpine-dark"
                     }, l.default.createElement(d.AgGridReact, {
                         ref: v,
                         gridOptions: f,
                         rowData: g,
                         columnDefs: h
@@ -38119,14 +37640,159 @@
                         DataFrame: c.default.createElement(w, {
                             style: g,
                             transformedDf: i.transformed_df
                         })
                     } [p]))
                 }
             },
+            5338: function(e, t, n) {
+                "use strict";
+                var r = this && this.__read || function(e, t) {
+                        var n = "function" == typeof Symbol && e[Symbol.iterator];
+                        if (!n) return e;
+                        var r, o, i = n.call(e),
+                            a = [];
+                        try {
+                            for (;
+                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
+                        } catch (e) {
+                            o = {
+                                error: e
+                            }
+                        } finally {
+                            try {
+                                r && !r.done && (n = i.return) && n.call(i)
+                            } finally {
+                                if (o) throw o.error
+                            }
+                        }
+                        return a
+                    },
+                    o = this && this.__importDefault || function(e) {
+                        return e && e.__esModule ? e : {
+                            default: e
+                        }
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.ArgGetters = t.OperationDetail = void 0;
+                var i = o(n(6255)),
+                    a = o(n(2275)),
+                    s = n(9867);
+                t.OperationDetail = function(e) {
+                    var n = e.command,
+                        r = e.setCommand,
+                        o = e.deleteCB,
+                        s = e.columns,
+                        l = e.commandPatterns;
+                    if (void 0 === n) return i.default.createElement("h2", null, " error undefined command ");
+                    var u = n[0].symbol,
+                        c = l[u];
+                    if (a.default.isArray(c)) {
+                        if (a.default.isEqual(c, [null])) return i.default.createElement("div", {
+                            className: "operation-detail"
+                        }, i.default.createElement("button", {
+                            onClick: o
+                        }, "X"));
+                        var p = c;
+                        return i.default.createElement("div", {
+                            className: "operation-detail"
+                        }, i.default.createElement(t.ArgGetters, {
+                            command: n,
+                            fullPattern: p,
+                            setCommand: r,
+                            columns: s,
+                            deleteCB: o
+                        }))
+                    }
+                    return i.default.createElement("h2", null, "unknown command ", u)
+                }, t.ArgGetters = function(e) {
+                    var t = e.command,
+                        n = e.fullPattern,
+                        r = e.setCommand,
+                        o = e.columns,
+                        a = e.deleteCB;
+                    return i.default.createElement("div", {
+                        className: "arg-getters"
+                    }, i.default.createElement("button", {
+                        onClick: a
+                    }, "X"), n.map((function(e) {
+                        var n = e[0],
+                            a = t[n];
+                        return i.default.createElement("div", {
+                            key: n
+                        }, i.default.createElement(l, {
+                            argProps: e,
+                            val: a,
+                            setter: function(e) {
+                                var o = (0, s.replaceAtIdx)(t, n, e);
+                                r(o)
+                            },
+                            columns: o
+                        }))
+                    })))
+                };
+                var l = function(e) {
+                    var t = e.argProps,
+                        n = e.val,
+                        o = e.setter,
+                        l = e.columns,
+                        u = r(t, 4),
+                        c = (u[0], u[1]),
+                        p = u[2],
+                        d = u[3];
+                    if ("enum" === p) return i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("select", {
+                        defaultValue: n,
+                        onChange: function(e) {
+                            return o(e.target.value)
+                        }
+                    }, d.map((function(e) {
+                        return i.default.createElement("option", {
+                            key: e,
+                            value: e
+                        }, e)
+                    }))));
+                    if ("type" === p) return "integer" === d ? i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("input", {
+                        type: "number",
+                        defaultValue: n,
+                        step: "1",
+                        onChange: function(e) {
+                            return o(parseInt(e.target.value))
+                        }
+                    })) : i.default.createElement("fieldset", null, i.default.createElement("label", null, " ", c, " "), i.default.createElement("input", {
+                        value: "dont know"
+                    }));
+                    if ("colEnum" === p) {
+                        var g = l.map((function(e) {
+                            var t = a.default.get(n, e, "null");
+                            return i.default.createElement("td", null, i.default.createElement("select", {
+                                defaultValue: t,
+                                onChange: function(t) {
+                                    var r = t.target.value;
+                                    if (a.default.isString(r)) {
+                                        var i = (0, s.replaceAtKey)(n, e, r);
+                                        o((0, s.objWithoutNull)(i, ["null"]))
+                                    }
+                                }
+                            }, d.map((function(e) {
+                                return i.default.createElement("option", {
+                                    key: e,
+                                    value: e
+                                }, e)
+                            }))))
+                        }));
+                        return i.default.createElement("div", {
+                            className: "col-enum"
+                        }, i.default.createElement("table", null, i.default.createElement("thead", null, i.default.createElement("tr", null, l.map((function(e) {
+                            return i.default.createElement("th", null, e)
+                        })))), i.default.createElement("tbody", null, i.default.createElement("tr", null, g))))
+                    }
+                    return i.default.createElement("h3", null, " unknown argtype ")
+                }
+            },
             6815: (e, t, n) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.bakedOperations = t.sym = void 0;
                 var r = n(4176);
                 t.sym = function(e) {
@@ -38135,14 +37801,501 @@
                     }
                 }, (0, t.sym)("nonexistent"), (0, t.sym)("df"), t.bakedOperations = [
                     [(0, t.sym)("dropcol"), r.symDf, "col1"],
                     [(0, t.sym)("fillna"), r.symDf, "col2", 5],
                     [(0, t.sym)("resample"), r.symDf, "month", "monthly", {}]
                 ]
             },
+            4710: function(e, t, n) {
+                "use strict";
+                var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
+                        void 0 === r && (r = n);
+                        var o = Object.getOwnPropertyDescriptor(t, n);
+                        o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        }), Object.defineProperty(e, r, o)
+                    } : function(e, t, n, r) {
+                        void 0 === r && (r = n), e[r] = t[n]
+                    }),
+                    o = this && this.__setModuleDefault || (Object.create ? function(e, t) {
+                        Object.defineProperty(e, "default", {
+                            enumerable: !0,
+                            value: t
+                        })
+                    } : function(e, t) {
+                        e.default = t
+                    }),
+                    i = this && this.__importStar || function(e) {
+                        if (e && e.__esModule) return e;
+                        var t = {};
+                        if (null != e)
+                            for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && r(t, e, n);
+                        return o(t, e), t
+                    },
+                    a = this && this.__awaiter || function(e, t, n, r) {
+                        return new(n || (n = Promise))((function(o, i) {
+                            function a(e) {
+                                try {
+                                    l(r.next(e))
+                                } catch (e) {
+                                    i(e)
+                                }
+                            }
+
+                            function s(e) {
+                                try {
+                                    l(r.throw(e))
+                                } catch (e) {
+                                    i(e)
+                                }
+                            }
+
+                            function l(e) {
+                                var t;
+                                e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                                    e(t)
+                                }))).then(a, s)
+                            }
+                            l((r = r.apply(e, t || [])).next())
+                        }))
+                    },
+                    s = this && this.__generator || function(e, t) {
+                        var n, r, o, i, a = {
+                            label: 0,
+                            sent: function() {
+                                if (1 & o[0]) throw o[1];
+                                return o[1]
+                            },
+                            trys: [],
+                            ops: []
+                        };
+                        return i = {
+                            next: s(0),
+                            throw: s(1),
+                            return: s(2)
+                        }, "function" == typeof Symbol && (i[Symbol.iterator] = function() {
+                            return this
+                        }), i;
+
+                        function s(i) {
+                            return function(s) {
+                                return function(i) {
+                                    if (n) throw new TypeError("Generator is already executing.");
+                                    for (; a;) try {
+                                        if (n = 1, r && (o = 2 & i[0] ? r.return : i[0] ? r.throw || ((o = r.return) && o.call(r), 0) : r.next) && !(o = o.call(r, i[1])).done) return o;
+                                        switch (r = 0, o && (i = [2 & i[0], o.value]), i[0]) {
+                                            case 0:
+                                            case 1:
+                                                o = i;
+                                                break;
+                                            case 4:
+                                                return a.label++, {
+                                                    value: i[1],
+                                                    done: !1
+                                                };
+                                            case 5:
+                                                a.label++, r = i[1], i = [0];
+                                                continue;
+                                            case 7:
+                                                i = a.ops.pop(), a.trys.pop();
+                                                continue;
+                                            default:
+                                                if (!((o = (o = a.trys).length > 0 && o[o.length - 1]) || 6 !== i[0] && 2 !== i[0])) {
+                                                    a = 0;
+                                                    continue
+                                                }
+                                                if (3 === i[0] && (!o || i[1] > o[0] && i[1] < o[3])) {
+                                                    a.label = i[1];
+                                                    break
+                                                }
+                                                if (6 === i[0] && a.label < o[1]) {
+                                                    a.label = o[1], o = i;
+                                                    break
+                                                }
+                                                if (o && a.label < o[2]) {
+                                                    a.label = o[2], a.ops.push(i);
+                                                    break
+                                                }
+                                                o[2] && a.ops.pop(), a.trys.pop();
+                                                continue
+                                        }
+                                        i = t.call(e, a)
+                                    } catch (e) {
+                                        i = [6, e], r = 0
+                                    } finally {
+                                        n = o = 0
+                                    }
+                                    if (5 & i[0]) throw i[1];
+                                    return {
+                                        value: i[0] ? i[1] : void 0,
+                                        done: !0
+                                    }
+                                }([i, s])
+                            }
+                        }
+                    },
+                    l = this && this.__read || function(e, t) {
+                        var n = "function" == typeof Symbol && e[Symbol.iterator];
+                        if (!n) return e;
+                        var r, o, i = n.call(e),
+                            a = [];
+                        try {
+                            for (;
+                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
+                        } catch (e) {
+                            o = {
+                                error: e
+                            }
+                        } finally {
+                            try {
+                                r && !r.done && (n = i.return) && n.call(i)
+                            } finally {
+                                if (o) throw o.error
+                            }
+                        }
+                        return a
+                    },
+                    u = this && this.__spreadArray || function(e, t, n) {
+                        if (n || 2 === arguments.length)
+                            for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
+                        return e.concat(r || Array.prototype.slice.call(t))
+                    },
+                    c = this && this.__importDefault || function(e) {
+                        return e && e.__esModule ? e : {
+                            default: e
+                        }
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.Commands = t.OperationViewer = t.OperationAdder = t.OperationsList = void 0;
+                var p = i(n(6255)),
+                    d = c(n(2275)),
+                    g = n(9867),
+                    h = n(3308),
+                    f = n(5338),
+                    v = n(8891),
+                    y = n(725);
+                n(9423), n(3054);
+                var m = n(1475),
+                    w = function(e) {
+                        return d.default.map(Array.from(e.entries()), (function(e) {
+                            var t = l(e, 2),
+                                n = t[0],
+                                r = t[1][0].symbol;
+                            return {
+                                field: r + n.toString(),
+                                headerName: r
+                            }
+                        }))
+                    };
+                t.OperationsList = function(e) {
+                    var t = e.operations,
+                        n = e.activeKey,
+                        r = e.setActiveKey,
+                        o = d.default.map(Array.from(t.entries()), (function(e) {
+                            var t = l(e, 2),
+                                n = t[0],
+                                r = t[1],
+                                o = {};
+                            return o[r[0].symbol + n.toString()] = r[2], o
+                        })),
+                        i = [d.default.merge.apply(d.default, u([{}], l(o), !1))],
+                        a = w(t),
+                        s = (0, y.updateAtMatch)(d.default.clone(a), n || "___never", {
+                            cellStyle: {
+                                background: "var(--ag-range-selection-background-color-3)"
+                            }
+                        }, {
+                            cellStyle: {}
+                        }),
+                        c = {
+                            rowSelection: "single",
+                            headerHeight: 30,
+                            onCellClicked: function(e) {
+                                var t = e.column.getColId();
+                                r(t)
+                            }
+                        };
+                    return p.default.createElement("div", {
+                        style: {
+                            height: 78,
+                            width: 1e3
+                        },
+                        className: "ag-theme-alpine"
+                    }, p.default.createElement(v.AgGridReact, {
+                        gridOptions: c,
+                        rowData: i,
+                        columnDefs: s
+                    }))
+                }, t.OperationAdder = function(e) {
+                    var t = e.column,
+                        n = e.addOperationCb,
+                        r = e.defaultArgs;
+                    return p.default.createElement("div", {
+                        className: "operation-adder"
+                    }, p.default.createElement("span", {
+                        className: "column-name"
+                    }, " Column: ", t), p.default.createElement("fieldset", null, d.default.keys(r).map((function(e) {
+                        return p.default.createElement("button", {
+                            key: e,
+                            onClick: (o = e, function() {
+                                var e = r[o];
+                                n((0, g.replaceInArr)(e, "col", t))
+                            })
+                        }, " ", e, " ");
+                        var o
+                    }))))
+                }, t.OperationViewer = function(e) {
+                    var n, r = e.operations,
+                        o = e.setOperations,
+                        i = e.activeColumn,
+                        a = e.allColumns,
+                        s = e.commandConfig,
+                        c = d.default.map(Array.from(r.entries()), (function(e) {
+                            var t = l(e, 2),
+                                n = t[0],
+                                r = t[1],
+                                o = {};
+                            return o[r[0].symbol + n.toString()] = r, o
+                        })),
+                        g = d.default.merge.apply(d.default, u([{}], l(c), !1)),
+                        h = d.default.map(Array.from(r.entries()), (function(e) {
+                            var t = l(e, 2),
+                                n = t[0],
+                                r = {};
+                            return r[t[1][0].symbol + n.toString()] = n, r
+                        })),
+                        v = d.default.merge.apply(d.default, u([{}], l(h), !1)),
+                        y = l((0, p.useState)(""), 2),
+                        m = y[0],
+                        C = y[1],
+                        b = s.argspecs,
+                        S = s.defaultArgs;
+                    return p.default.createElement("div", {
+                        className: "command-viewer"
+                    }, p.default.createElement(t.OperationAdder, {
+                        column: i,
+                        addOperationCb: function(e) {
+                            var t = u(u([], l(r), !1), [e], !1);
+                            o(t);
+                            var n = w(t)[t.length - 1].field;
+                            void 0 !== n && C(n)
+                        },
+                        defaultArgs: S
+                    }), p.default.createElement("div", {
+                        className: "operations-box"
+                    }, p.default.createElement("h4", null, " Operations "), p.default.createElement(t.OperationsList, {
+                        operations: r,
+                        activeKey: m,
+                        setActiveKey: C
+                    })), m && p.default.createElement(f.OperationDetail, {
+                        command: g[m],
+                        setCommand: (n = m, function(e) {
+                            var t = v[n],
+                                i = r.map((function(n, r) {
+                                    return r === t ? e : n
+                                }));
+                            o(i)
+                        }),
+                        deleteCB: function(e) {
+                            return function() {
+                                var t = v[e],
+                                    n = r.map((function(e, n) {
+                                        return n === t ? void 0 : e
+                                    }));
+                                C(""), o(d.default.filter(n))
+                            }
+                        }(m),
+                        columns: a,
+                        commandPatterns: b
+                    }))
+                }, t.Commands = function() {
+                    var e = l((0, p.useState)(m.bakedOperations), 2),
+                        n = e[0],
+                        r = e[1],
+                        o = l((0, p.useState)(h.bakedCommandConfig), 2),
+                        i = o[0],
+                        u = o[1];
+                    return (0, p.useEffect)((function() {
+                        fetch("http://localhost:5000/dcf/command-config").then((function(e) {
+                            return a(void 0, void 0, void 0, (function() {
+                                var t;
+                                return s(this, (function(n) {
+                                    switch (n.label) {
+                                        case 0:
+                                            return t = u, [4, e.json()];
+                                        case 1:
+                                            return t.apply(void 0, [n.sent()]), [2]
+                                    }
+                                }))
+                            }))
+                        }))
+                    }), []), p.default.createElement("div", {
+                        style: {
+                            width: "100%",
+                            height: "100%"
+                        }
+                    }, p.default.createElement(t.OperationViewer, {
+                        operations: n,
+                        setOperations: r,
+                        activeColumn: "new-column2",
+                        allColumns: ["foo-col", "bar-col", "baz-col"],
+                        commandConfig: i
+                    }), p.default.createElement("code", {
+                        style: {
+                            fontSize: "1em",
+                            textAlign: "left"
+                        }
+                    }, " ", JSON.stringify(n, null, "\t\n\r"), " "))
+                }
+            },
+            4336: function(e, t, n) {
+                "use strict";
+                var r = this && this.__assign || function() {
+                        return r = Object.assign || function(e) {
+                            for (var t, n = 1, r = arguments.length; n < r; n++)
+                                for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
+                            return e
+                        }, r.apply(this, arguments)
+                    },
+                    o = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
+                        void 0 === r && (r = n);
+                        var o = Object.getOwnPropertyDescriptor(t, n);
+                        o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        }), Object.defineProperty(e, r, o)
+                    } : function(e, t, n, r) {
+                        void 0 === r && (r = n), e[r] = t[n]
+                    }),
+                    i = this && this.__setModuleDefault || (Object.create ? function(e, t) {
+                        Object.defineProperty(e, "default", {
+                            enumerable: !0,
+                            value: t
+                        })
+                    } : function(e, t) {
+                        e.default = t
+                    }),
+                    a = this && this.__importStar || function(e) {
+                        if (e && e.__esModule) return e;
+                        var t = {};
+                        if (null != e)
+                            for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && o(t, e, n);
+                        return i(t, e), t
+                    },
+                    s = this && this.__read || function(e, t) {
+                        var n = "function" == typeof Symbol && e[Symbol.iterator];
+                        if (!n) return e;
+                        var r, o, i = n.call(e),
+                            a = [];
+                        try {
+                            for (;
+                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
+                        } catch (e) {
+                            o = {
+                                error: e
+                            }
+                        } finally {
+                            try {
+                                r && !r.done && (n = i.return) && n.call(i)
+                            } finally {
+                                if (o) throw o.error
+                            }
+                        }
+                        return a
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.StatusBarEx = t.StatusBar = void 0;
+                var l = a(n(6255)),
+                    u = n(8891),
+                    c = [{
+                        field: "totalRows"
+                    }, {
+                        field: "columns"
+                    }, {
+                        field: "rowsShown"
+                    }, {
+                        field: "sampleSize"
+                    }, {
+                        field: "summaryStats"
+                    }, {
+                        field: "reorderdColumns"
+                    }];
+
+                function p(e) {
+                    var t = e.config,
+                        n = e.setConfig,
+                        o = t.totalRows,
+                        i = t.columns,
+                        a = t.rowsShown,
+                        s = t.sampleSize,
+                        p = t.summaryStats,
+                        d = t.reorderdColumns,
+                        g = [{
+                            totalRows: o,
+                            columns: i,
+                            rowsShown: a,
+                            sampleSize: s,
+                            summaryStats: p.toString(),
+                            reorderdColumns: d.toString()
+                        }],
+                        h = (0, l.useRef)(null);
+                    return l.default.createElement("div", {
+                        className: "statusBar"
+                    }, l.default.createElement("div", {
+                        style: {
+                            height: 50
+                        },
+                        className: "theme-hanger ag-theme-alpine-dark"
+                    }, l.default.createElement(u.AgGridReact, {
+                        ref: h,
+                        onCellClicked: function(e) {
+                            var o = e.column.getColId();
+                            "summaryStats" === o ? n(r(r({}, t), {
+                                summaryStats: !t.summaryStats
+                            })) : "reorderdColumns" === o && n(r(r({}, t), {
+                                reorderdColumns: !t.reorderdColumns
+                            }))
+                        },
+                        gridOptions: {
+                            rowSelection: "single"
+                        },
+                        defaultColDef: {
+                            type: "left-aligned",
+                            cellStyle: {
+                                textAlign: "left"
+                            }
+                        },
+                        rowData: g,
+                        columnDefs: c
+                    })))
+                }
+                t.StatusBar = p, t.StatusBarEx = function() {
+                    var e = s((0, l.useState)({
+                            totalRows: 1309,
+                            columns: 30,
+                            rowsShown: 500,
+                            sampleSize: 1e4,
+                            summaryStats: !1,
+                            reorderdColumns: !1
+                        }), 2),
+                        t = e[0],
+                        n = e[1];
+                    return l.default.createElement(p, {
+                        config: t,
+                        setConfig: n
+                    })
+                }
+            },
             3308: (e, t, n) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.bakedCommandConfig = t.bakedOperationDefaults = void 0;
                 var r = n(9867),
                     o = n(4176);
@@ -38291,17 +38444,17 @@
                         "start station latitude": 40.73652889,
                         bikeid: 20062,
                         "birth year": "1972",
                         gender: 2
                     }]
                 }
             },
-            9867: function(e, t) {
+            9867: function(e, t, n) {
                 "use strict";
-                var n = this && this.__awaiter || function(e, t, n, r) {
+                var r = this && this.__awaiter || function(e, t, n, r) {
                         return new(n || (n = Promise))((function(o, i) {
                             function a(e) {
                                 try {
                                     l(r.next(e))
                                 } catch (e) {
                                     i(e)
                                 }
@@ -38320,15 +38473,15 @@
                                 e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                     e(t)
                                 }))).then(a, s)
                             }
                             l((r = r.apply(e, t || [])).next())
                         }))
                     },
-                    r = this && this.__generator || function(e, t) {
+                    o = this && this.__generator || function(e, t) {
                         var n, r, o, i, a = {
                             label: 0,
                             sent: function() {
                                 if (1 & o[0]) throw o[1];
                                 return o[1]
                             },
                             trys: [],
@@ -38394,35 +38547,83 @@
                                     return {
                                         value: i[0] ? i[1] : void 0,
                                         done: !0
                                     }
                                 }([i, s])
                             }
                         }
+                    },
+                    i = this && this.__read || function(e, t) {
+                        var n = "function" == typeof Symbol && e[Symbol.iterator];
+                        if (!n) return e;
+                        var r, o, i = n.call(e),
+                            a = [];
+                        try {
+                            for (;
+                                (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
+                        } catch (e) {
+                            o = {
+                                error: e
+                            }
+                        } finally {
+                            try {
+                                r && !r.done && (n = i.return) && n.call(i)
+                            } finally {
+                                if (o) throw o.error
+                            }
+                        }
+                        return a
+                    },
+                    a = this && this.__spreadArray || function(e, t, n) {
+                        if (n || 2 === arguments.length)
+                            for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
+                        return e.concat(r || Array.prototype.slice.call(t))
+                    },
+                    s = this && this.__importDefault || function(e) {
+                        return e && e.__esModule ? e : {
+                            default: e
+                        }
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.sym = t.requestDf = void 0, t.requestDf = function(e, t) {
+                }), t.objWithoutNull = t.replaceAtKey = t.replaceAtIdx = t.replaceInArr = t.sym = t.requestDf = void 0;
+                var l = s(n(2275));
+                t.requestDf = function(e, t) {
                     return fetch(e).then((function(e) {
-                        return n(void 0, void 0, void 0, (function() {
+                        return r(void 0, void 0, void 0, (function() {
                             var n;
-                            return r(this, (function(r) {
+                            return o(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
                                         return [4, e.json()];
                                     case 1:
                                         return n = r.sent(), t(n), [2]
                                 }
                             }))
                         }))
                     }))
                 }, t.sym = function(e) {
                     return {
                         symbol: e
                     }
+                }, t.replaceInArr = function(e, t, n) {
+                    return e.map((function(e) {
+                        return e === t ? n : e
+                    }))
+                }, t.replaceAtIdx = function(e, t, n) {
+                    return e.map((function(e, r) {
+                        return r === t ? n : e
+                    }))
+                }, t.replaceAtKey = function(e, t, n) {
+                    var r = l.default.clone(e);
+                    return r[t] = n, r
+                }, t.objWithoutNull = function(e, t) {
+                    return void 0 === t && (t = []), l.default.pickBy(e, (function(e) {
+                        return !a([null, void 0], i(t), !1).includes(e)
+                    }))
                 }
             },
             8481: function(e, t, n) {
                 "use strict";
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
                         void 0 === r && (r = n);
                         var o = Object.getOwnPropertyDescriptor(t, n);
@@ -38448,15 +38649,15 @@
                         var t = {};
                         if (null != e)
                             for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && r(t, e, n);
                         return o(t, e), t
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.DFViewer = t.CommandUtils = t.DependentTabs = t.CommandsComponent = t.ColumnsEditor = t.OperationUtils = t.staticData = t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
+                }), t.StatusBar = t.DFViewer = t.CommandUtils = t.DependentTabs = t.CommandsComponent = t.ColumnsEditor = t.OperationUtils = t.staticData = t.WidgetDCFCellExample = t.WidgetDCFCell = t.DCFCell = void 0;
                 var a = n(1314);
                 Object.defineProperty(t, "DCFCell", {
                     enumerable: !0,
                     get: function() {
                         return a.DCFCell
                     }
                 }), Object.defineProperty(t, "WidgetDCFCell", {
@@ -38465,22 +38666,22 @@
                         return a.WidgetDCFCell
                     }
                 }), Object.defineProperty(t, "WidgetDCFCellExample", {
                     enumerable: !0,
                     get: function() {
                         return a.WidgetDCFCellExample
                     }
-                }), t.staticData = i(n(1475)), t.OperationUtils = i(n(6815)), t.ColumnsEditor = i(n(3677)), t.CommandsComponent = i(n(1840)), t.DependentTabs = i(n(5732)), t.CommandUtils = i(n(4176));
+                }), t.staticData = i(n(1475)), t.OperationUtils = i(n(6815)), t.ColumnsEditor = i(n(3677)), t.CommandsComponent = i(n(4710)), t.DependentTabs = i(n(5732)), t.CommandUtils = i(n(4176));
                 var s = n(1251);
                 Object.defineProperty(t, "DFViewer", {
                     enumerable: !0,
                     get: function() {
                         return s.DFViewer
                     }
-                })
+                }), t.StatusBar = i(n(4336))
             },
             3783: (e, t, n) => {
                 "use strict";
                 var r = n(7306);
 
                 function o() {}
 
@@ -48397,81 +48598,109 @@
                         }),
                         s = e.href;
                     e.href = URL.createObjectURL(a), s && URL.revokeObjectURL(s)
                 }
             },
             8669: function(e, t, n) {
                 "use strict";
-                var r = this && this.__importDefault || function(e) {
-                    return e && e.__esModule ? e : {
-                        default: e
-                    }
-                };
+                var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
+                        void 0 === r && (r = n), Object.defineProperty(e, r, {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        })
+                    } : function(e, t, n, r) {
+                        void 0 === r && (r = n), e[r] = t[n]
+                    }),
+                    o = this && this.__setModuleDefault || (Object.create ? function(e, t) {
+                        Object.defineProperty(e, "default", {
+                            enumerable: !0,
+                            value: t
+                        })
+                    } : function(e, t) {
+                        e.default = t
+                    }),
+                    i = this && this.__importStar || function(e) {
+                        if (e && e.__esModule) return e;
+                        var t = {};
+                        if (null != e)
+                            for (var n in e) "default" !== n && Object.prototype.hasOwnProperty.call(e, n) && r(t, e, n);
+                        return o(t, e), t
+                    };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.DCEFWidgetView = t.DCEFWidgetModel = void 0;
-                const o = n(9146),
-                    i = n(8481),
-                    a = n(8791),
-                    s = r(n(6255)),
-                    l = n(840);
+                const a = n(9146),
+                    s = n(8481),
+                    l = i(n(6255)),
+                    u = i(n(8791)),
+                    c = n(840);
                 n(9423), n(3054), n(4260), n(801);
-                class u extends o.DOMWidgetModel {
+                class p extends a.DOMWidgetModel {
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
-                            _model_name: u.model_name,
-                            _model_module: u.model_module,
-                            _model_module_version: u.model_module_version,
-                            _view_name: u.view_name,
-                            _view_module: u.view_module,
-                            _view_module_version: u.view_module_version,
-                            command_config: {},
-                            commands: [],
-                            operation_results: {}
+                            _model_name: p.model_name,
+                            _model_module: p.model_module,
+                            _model_module_version: p.model_module_version,
+                            _view_name: p.view_name,
+                            _view_module: p.view_module,
+                            _view_module_version: p.view_module_version,
+                            commandConfig: {},
+                            operations: [],
+                            operation_results: {},
+                            dfConfig: {}
                         })
                     }
                 }
-                t.DCEFWidgetModel = u, u.serializers = Object.assign({}, o.DOMWidgetModel.serializers), u.model_name = "DCEFWidgetModel", u.model_module = l.MODULE_NAME, u.model_module_version = l.MODULE_VERSION, u.view_name = "ExampleView", u.view_module = l.MODULE_NAME, u.view_module_version = l.MODULE_VERSION;
-                class c extends o.DOMWidgetView {
+                t.DCEFWidgetModel = p, p.serializers = Object.assign({}, a.DOMWidgetModel.serializers), p.model_name = "DCEFWidgetModel", p.model_module = c.MODULE_NAME, p.model_module_version = c.MODULE_VERSION, p.view_name = "ExampleView", p.view_module = c.MODULE_NAME, p.view_module_version = c.MODULE_VERSION;
+                class d extends a.DOMWidgetView {
                     constructor() {
-                        super(...arguments), this.setCommandConfig = e => {
-                            console.log("default setCommandConfig")
-                        }, this.setPyCode = e => {
-                            console.log("default setPyCode")
-                        }, this.setTransformedDf = e => {
-                            console.log("default setTransformedDf")
-                        }
+                        super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
                     }
                     render() {
-                        console.log("DCFWidget View... renamed "), this.el.classList.add("custom-widget");
-                        const e = a.createRoot(this.el),
-                            t = this.model,
-                            n = this;
-                        t.on("change:command_config", (() => {
-                            n.setCommandConfig(t.get("command_config"))
+                        this.el.classList.add("custom-widget");
+                        const e = this.model,
+                            t = this;
+                        e.on("change:commandConfig", (() => {
+                            t.setCommandConfig(e.get("commandConfig"))
                         }), this);
-                        const r = t.get("command_config");
-                        console.log("widget, commandConfig", r, t);
-                        const o = s.default.createElement(i.WidgetDCFCell, {
-                            origDf: t.get("js_df"),
-                            getOrRequester: e => (t.on("change:operation_results", (() => {
-                                const n = t.get("operation_results");
-                                console.log("about to call setOpResult with", n), e(n)
-                            }), this), e => {
-                                console.log("orRequester passed operations", e), t.set("commands", e), t.save_changes()
-                            }),
-                            commandConfig: r,
-                            exposeCommandConfigSetter: e => {
-                                n.setCommandConfig = e
-                            }
-                        }, null);
-                        e.render(o)
+                        const n = {
+                                getOrRequester: t => (e.on("change:operation_results", (() => {
+                                    const n = e.get("operation_results");
+                                    console.log("about to call setOpResult with", n), t(n)
+                                }), this), t => {
+                                    console.log("orRequester passed operations", t), e.set("operations", t), e.save_changes()
+                                }),
+                                exposeCommandConfigSetter: e => {
+                                    t.setCommandConfig = e
+                                }
+                            },
+                            r = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                            o = this.el.getBoundingClientRect().y,
+                            i = r.getBoundingClientRect().y - o + 50;
+                        r.scroll(0, i);
+                        const a = u.createRoot(this.el),
+                            c = l.default.createElement((() => {
+                                const [e, t] = l.useState(0), r = () => {
+                                    t((e => e + 1))
+                                };
+                                l.useEffect((() => {
+                                    this.listenTo(this.model, "change", r)
+                                }), []);
+                                const o = Object.assign({}, n);
+                                for (const e of Object.keys(this.model.attributes)) o[e] = this.model.get(e), o["on_" + e] = t => {
+                                    this.model.set(e, t), this.touch()
+                                };
+                                return l.default.createElement(s.WidgetDCFCell, o)
+                            }), {});
+                        a.render(c)
                     }
                 }
-                t.DCEFWidgetView = c
+                t.DCEFWidgetView = d
             },
             5268: function(e, t, n) {
                 "use strict";
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
                         void 0 === r && (r = n), Object.defineProperty(e, r, {
                             enumerable: !0,
                             get: function() {
@@ -48517,15 +48746,15 @@
             },
             9146: t => {
                 "use strict";
                 t.exports = e
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.25","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+                e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.33","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
             }
         },
         n = {};
 
     function r(e) {
         var o = n[e];
         if (void 0 !== o) return o.exports;
```

### Comparing `dcef-0.2.3/dcef/nbextension/index.js.LICENSE.txt` & `dcef-0.2.5/dcef/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/dcef/noarch/index.html` & `dcef-0.2.5/dcef/noarch/index.html`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/Makefile` & `dcef-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/commands_vs_operations.md` & `dcef-0.2.5/docs/commands_vs_operations.md`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/make.bat` & `dcef-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/source/FAQ.rst` & `dcef-0.2.5/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/source/conf.py` & `dcef-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/source/index.rst` & `dcef-0.2.5/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    using
    install
+   contributing
    FAQ
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `dcef-0.2.3/docs/source/using.rst` & `dcef-0.2.5/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/docs/source/_static/embed-bundle.js.LICENSE.txt` & `dcef-0.2.5/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/js/extension.ts` & `dcef-0.2.5/js/extension.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/js/paddywidget.ts` & `dcef-0.2.5/js/paddywidget.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/js/plugin.ts` & `dcef-0.2.5/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/static/images/dcf-jupyter.png` & `dcef-0.2.5/static/images/dcf-jupyter.png`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/.gitignore` & `dcef-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/LICENSE.txt` & `dcef-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcef-0.2.3/README.md` & `dcef-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 Using `pip`:
 
 ```bash
 pip install dcef
 ```
 
+## Documentation
+
+To get started with using DCEF, check out the full documentation:
+
+https://dcef.readthedocs.io/
+
+
 # Using DCEF
 
 in a jupyter lab notebook just add the following to a cell
 
 ```python
 from dcef.dcef_widget import DCEFWidget
 DCEFWidget(df=df)  #df being the dataframe you want to explore
@@ -40,15 +47,15 @@
 ## Writing your own commands
 
 Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
-class DropCol(Transform):
+class DropCol(Command):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
 
     @staticmethod 
     def transform(df, col):
         df.drop(col, axis=1, inplace=True)
         return df
```

### Comparing `dcef-0.2.3/pyproject.toml` & `dcef-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.2.3"
+version = "0.2.5"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `dcef-0.2.3/PKG-INFO` & `dcef-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcef
-Version: 0.2.3
+Version: 0.2.5
 Summary: Data Cleaning Framework - UI for quickly cleaning pandas dataframes 
 Project-URL: Homepage, https://github.com/bloomberg/dcef
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -67,14 +67,21 @@
 
 Using `pip`:
 
 ```bash
 pip install dcef
 ```
 
+## Documentation
+
+To get started with using DCEF, check out the full documentation:
+
+https://dcef.readthedocs.io/
+
+
 # Using DCEF
 
 in a jupyter lab notebook just add the following to a cell
 
 ```python
 from dcef.dcef_widget import DCEFWidget
 DCEFWidget(df=df)  #df being the dataframe you want to explore
@@ -95,15 +102,15 @@
 ## Writing your own commands
 
 Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
-class DropCol(Transform):
+class DropCol(Command):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
 
     @staticmethod 
     def transform(df, col):
         df.drop(col, axis=1, inplace=True)
         return df
```

