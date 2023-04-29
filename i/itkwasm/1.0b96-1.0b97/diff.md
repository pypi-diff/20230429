# Comparing `tmp/itkwasm-1.0b96.tar.gz` & `tmp/itkwasm-1.0b97.tar.gz`

## Comparing `itkwasm-1.0b96.tar` & `itkwasm-1.0b97.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/.gitignore
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/Makefile
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/conf.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/make.bat
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/requirements.txt
--rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/genindex.html
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/index.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/objects.inv
--rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/search.html
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/webpack-macros.html
--rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/_to_numpy_array.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/binary_file.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/binary_stream.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/environment_dispatch.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/float_types.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/image.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/int_types.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/interface_types.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/mesh.py
--rw-r--r--   0        0        0    20129 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pipeline.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pipeline_input.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pipeline_output.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pixel_types.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pointset.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/polydata.py
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/pyodide.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/text_file.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/text_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b96/itkwasm/transform.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_function_factory.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_image.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_js_package_config.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_mesh.py
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_pipeline.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_pointset.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_polydata.py
--rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_pyodide.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test_transform.py
--rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/baseline/test_pipeline_write_read_image.png
--rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/cow.vtk
--rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/cthead1.png
--rwxr-xr-x   0        0        0   620974 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/input-output-files-test.wasi.wasm
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/input.bin
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/input.txt
--rwxr-xr-x   0        0        0  1135160 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/median-filter-test.wasi.wasm
--rwxr-xr-x   0        0        0  1278174 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/mesh-read-write-test.wasi.wasm
--rwxr-xr-x   0        0        0  2174461 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/mesh-to-poly-data.wasi.wasm
--rwxr-xr-x   0        0        0  1287522 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/poly-data-to-mesh.wasi.wasm
--rwxr-xr-x   0        0        0   269115 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/input/stdout-stderr-test.wasi.wasm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test-accelerator/pyproject.toml
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test-accelerator/test_accelerator/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test-accelerator/test_accelerator/faster_mod.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test-accelerator/test_accelerator/fastest_mod.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b96/test/test-accelerator/test_accelerator/slower_mod.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm-1.0b96/.gitignore
--rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 itkwasm-1.0b96/LICENSE
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 itkwasm-1.0b96/README.md
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 itkwasm-1.0b96/pyproject.toml
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 itkwasm-1.0b96/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/Makefile
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/conf.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/requirements.txt
+-rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/index.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/search.html
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0    12757 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/webpack-macros.html
+-rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   335757 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0   176654 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0    63341 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0   101691 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0        0        0   181264 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   105112 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    60236 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   389948 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154840 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/_to_numpy_array.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/binary_file.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/binary_stream.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/environment_dispatch.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/float_types.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/image.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/int_types.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/interface_types.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/mesh.py
+-rw-r--r--   0        0        0    20129 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pipeline.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pipeline_input.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pipeline_output.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pixel_types.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pointset.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/polydata.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/pyodide.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/text_file.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/text_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b97/itkwasm/transform.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_function_factory.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_image.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_js_package_config.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_mesh.py
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_pipeline.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_pointset.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_polydata.py
+-rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_pyodide.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test_transform.py
+-rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/baseline/test_pipeline_write_read_image.png
+-rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/cow.vtk
+-rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/cthead1.png
+-rwxr-xr-x   0        0        0   620974 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/input-output-files-test.wasi.wasm
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/input.bin
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/input.txt
+-rwxr-xr-x   0        0        0  1135160 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/median-filter-test.wasi.wasm
+-rwxr-xr-x   0        0        0  1278174 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/mesh-read-write-test.wasi.wasm
+-rwxr-xr-x   0        0        0  2174461 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/mesh-to-poly-data.wasi.wasm
+-rwxr-xr-x   0        0        0  1287522 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/poly-data-to-mesh.wasi.wasm
+-rwxr-xr-x   0        0        0   269115 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/input/stdout-stderr-test.wasi.wasm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test-accelerator/pyproject.toml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test-accelerator/test_accelerator/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test-accelerator/test_accelerator/faster_mod.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test-accelerator/test_accelerator/fastest_mod.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm-1.0b97/test/test-accelerator/test_accelerator/slower_mod.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 itkwasm-1.0b97/.gitignore
+-rw-r--r--   0        0        0    11360 2020-02-02 00:00:00.000000 itkwasm-1.0b97/LICENSE
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 itkwasm-1.0b97/README.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 itkwasm-1.0b97/pyproject.toml
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 itkwasm-1.0b97/PKG-INFO
```

### Comparing `itkwasm-1.0b96/docs/Makefile` & `itkwasm-1.0b97/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/conf.py` & `itkwasm-1.0b97/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/make.bat` & `itkwasm-1.0b97/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/doctrees/environment.pickle` & `itkwasm-1.0b97/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/doctrees/index.doctree` & `itkwasm-1.0b97/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/genindex.html` & `itkwasm-1.0b97/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/index.html` & `itkwasm-1.0b97/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/search.html` & `itkwasm-1.0b97/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/searchindex.js` & `itkwasm-1.0b97/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/alabaster.css` & `itkwasm-1.0b97/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/basic.css` & `itkwasm-1.0b97/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/doctools.js` & `itkwasm-1.0b97/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/language_data.js` & `itkwasm-1.0b97/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/pygments.css` & `itkwasm-1.0b97/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/searchtools.js` & `itkwasm-1.0b97/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/sphinx_highlight.js` & `itkwasm-1.0b97/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/webpack-macros.html` & `itkwasm-1.0b97/docs/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/scripts/bootstrap.js` & `itkwasm-1.0b97/docs/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/scripts/bootstrap.js.map` & `itkwasm-1.0b97/docs/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/scripts/pydata-sphinx-theme.js` & `itkwasm-1.0b97/docs/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `itkwasm-1.0b97/docs/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/styles/bootstrap.css` & `itkwasm-1.0b97/docs/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/styles/pydata-sphinx-theme.css` & `itkwasm-1.0b97/docs/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `itkwasm-1.0b97/docs/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/__init__.py` & `itkwasm-1.0b97/itkwasm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """itkwasm: Python interface to itk-wasm WebAssembly modules."""
 
-__version__ = "1.0b96"
+__version__ = "1.0b97"
 
 from .interface_types import InterfaceTypes
 from .image import Image, ImageType
 from .pointset import PointSet, PointSetType
 from .mesh import Mesh, MeshType
 from .polydata import PolyData, PolyDataType
 from .binary_file import BinaryFile
```

### Comparing `itkwasm-1.0b96/itkwasm/_to_numpy_array.py` & `itkwasm-1.0b97/itkwasm/_to_numpy_array.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/environment_dispatch.py` & `itkwasm-1.0b97/itkwasm/environment_dispatch.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/image.py` & `itkwasm-1.0b97/itkwasm/image.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/mesh.py` & `itkwasm-1.0b97/itkwasm/mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pipeline.py` & `itkwasm-1.0b97/itkwasm/pipeline.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pipeline_input.py` & `itkwasm-1.0b97/itkwasm/pipeline_input.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pipeline_output.py` & `itkwasm-1.0b97/itkwasm/pipeline_output.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pixel_types.py` & `itkwasm-1.0b97/itkwasm/pixel_types.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pointset.py` & `itkwasm-1.0b97/itkwasm/pointset.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/polydata.py` & `itkwasm-1.0b97/itkwasm/polydata.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/itkwasm/pyodide.py` & `itkwasm-1.0b97/itkwasm/pyodide.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     def web_worker(self, value):
         self._web_worker = value
 
 js_resources = JsResources()
 
 def to_py(js_proxy):
     import pyodide
-    if isinstance(js_proxy, pyodide.ffi.JsArray):
+    if hasattr(js_proxy, 'constructor') and js_proxy.constructor.name == "Uint8Array":
+        return js_proxy.to_bytes()
+    elif isinstance(js_proxy, pyodide.ffi.JsArray):
         return [to_py(value) for value in js_proxy]
     elif hasattr(js_proxy, "imageType"):
         image_dict = js_proxy.to_py()
         image_type = ImageType(**image_dict['imageType'])
         image_dict['imageType'] = image_type
         dimension = image_type.dimension
         component_type = image_type.componentType
@@ -135,15 +137,16 @@
     elif hasattr(js_proxy, "data") and isinstance(js_proxy.data, str):
         text_stream_dict = js_proxy.to_py()
         return TextStream(**text_stream_dict)
     elif hasattr(js_proxy, "data"):
         binary_stream_dict = js_proxy.to_py()
         binary_stream_dict['data'] = bytes(binary_stream_dict['data'])
         return BinaryStream(**binary_stream_dict)
-    return js_proxy.to_py()
+    # Is not a JsProxy, int, etc
+    return js_proxy
 
 def to_js(py):
     import pyodide
     import js
     if isinstance(py, list):
         js_array = pyodide.ffi.to_js([])
         for value in py:
```

### Comparing `itkwasm-1.0b96/test/test_function_factory.py` & `itkwasm-1.0b97/test/test_function_factory.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_image.py` & `itkwasm-1.0b97/test/test_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_js_package_config.py` & `itkwasm-1.0b97/test/test_js_package_config.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_mesh.py` & `itkwasm-1.0b97/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_pipeline.py` & `itkwasm-1.0b97/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_pointset.py` & `itkwasm-1.0b97/test/test_pointset.py`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test_pyodide.py` & `itkwasm-1.0b97/test/test_pyodide.py`

 * *Files 3% similar despite different names*

```diff
@@ -285,7 +285,32 @@
         with open(text_file.path, 'r') as fp:
             data_py = fp.read()
 
         assert data_py == data
 
     for text_file in text_files_py:
         verify_text_file(text_file)
+
+@run_in_pyodide(packages=['micropip', 'numpy'])
+async def test_uint8array_conversion(selenium, package_wheel):
+    import micropip
+    await micropip.install(package_wheel)
+
+    from itkwasm.pyodide import to_js, to_py
+
+    data = bytes([222,173,190,239])
+
+    data_js = to_js(data)
+    data_py = to_py(data_js)
+
+    assert isinstance(data_py, bytes)
+
+    assert data_py[0], 222
+    assert data_py[1], 173
+    assert data_py[2], 190
+    assert data_py[3], 239
+
+    ivalue = 8
+    ivalue_js = to_js(ivalue)
+    ivalue_py = to_py(ivalue_js)
+
+    assert ivalue == ivalue_py
```

### Comparing `itkwasm-1.0b96/test/baseline/test_pipeline_write_read_image.png` & `itkwasm-1.0b97/test/baseline/test_pipeline_write_read_image.png`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/cow.vtk` & `itkwasm-1.0b97/test/input/cow.vtk`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/cthead1.png` & `itkwasm-1.0b97/test/input/cthead1.png`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/input-output-files-test.wasi.wasm` & `itkwasm-1.0b97/test/input/input-output-files-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/median-filter-test.wasi.wasm` & `itkwasm-1.0b97/test/input/median-filter-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/mesh-read-write-test.wasi.wasm` & `itkwasm-1.0b97/test/input/mesh-read-write-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/mesh-to-poly-data.wasi.wasm` & `itkwasm-1.0b97/test/input/mesh-to-poly-data.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/poly-data-to-mesh.wasi.wasm` & `itkwasm-1.0b97/test/input/poly-data-to-mesh.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/input/stdout-stderr-test.wasi.wasm` & `itkwasm-1.0b97/test/input/stdout-stderr-test.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/test/test-accelerator/pyproject.toml` & `itkwasm-1.0b97/test/test-accelerator/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/.gitignore` & `itkwasm-1.0b97/.gitignore`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/LICENSE` & `itkwasm-1.0b97/LICENSE`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/README.md` & `itkwasm-1.0b97/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm-1.0b96/pyproject.toml` & `itkwasm-1.0b97/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 test = [
     "hatch build -t wheel",
     "pytest --dist-dir=./dist --rt=chrome",
 ]
 download-pyodide = [
   "curl -L https://github.com/pyodide/pyodide/releases/download/0.23.1/pyodide-0.23.1.tar.bz2 -o pyodide.tar.bz2",
   "tar xjf pyodide.tar.bz2",
-  "rm -rf dist",
+  "rm -rf dist pyodide.tar.bz2",
   "mv pyodide dist",
 ]
 
 [tool.hatch.envs.docs]
 dependencies = [
     "sphinx",
     "pydata-sphinx-theme",
```

### Comparing `itkwasm-1.0b96/PKG-INFO` & `itkwasm-1.0b97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm
-Version: 1.0b96
+Version: 1.0b97
 Summary: Python interface to itk-wasm WebAssembly (Wasm) modules.
 Project-URL: Home, https://wasm.itk.org/
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 Author-email: Matt McCormick <matt.mccormick@kitware.com>
 License: 
                                          Apache License
```

