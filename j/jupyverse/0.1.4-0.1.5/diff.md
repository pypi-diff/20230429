# Comparing `tmp/jupyverse-0.1.4.tar.gz` & `tmp/jupyverse-0.1.5.tar.gz`

## Comparing `jupyverse-0.1.4.tar` & `jupyverse-0.1.5.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    60173 2020-02-02 00:00:00.000000 jupyverse-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.4/config.yaml
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 jupyverse-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.4/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.4/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/microservices.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.4/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.4/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.4/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.4/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.4/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.4/README.md
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 jupyverse-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyverse-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    61129 2020-02-02 00:00:00.000000 jupyverse-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.5/config.yaml
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.5/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.5/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.5/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.5/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.5/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_kernels.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.5/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.5/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.5/README.md
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 jupyverse-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 jupyverse-0.1.5/PKG-INFO
```

### Comparing `jupyverse-0.1.4/.pre-commit-config.yaml` & `jupyverse-0.1.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.262
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.1.4/CHANGELOG.md` & `jupyverse-0.1.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.5
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.4...bea8fa74efe86fa59ea6054f6e332ffd3d58b23f))
+
+### Merged PRs
+
+- Update with FastAPI-Users v11 [#296](https://github.com/jupyter-server/jupyverse/pull/296) ([@davidbrochart](https://github.com/davidbrochart))
+- Update documentation on microservices with authentication [#295](https://github.com/jupyter-server/jupyverse/pull/295) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-18&to=2023-04-29&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-18..2023-04-29&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-18..2023-04-29&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.4
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.3...a42f7c4d0e951d620108afb4ca25e57da5bae2a1))
 
 ### Merged PRs
 
 - Move routes to jupyverse_api [#293](https://github.com/jupyter-server/jupyverse/pull/293) ([@davidbrochart](https://github.com/davidbrochart))
@@ -15,16 +32,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-06&to=2023-04-18&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-06..2023-04-18&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-06..2023-04-18&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.3
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.2...b5faf93e3296d855c7ebeda0c25e9861400ad469))
 
 ### Merged PRs
 
 - Add fps-lab and fps-frontend dependencies to jupyverse [#287](https://github.com/jupyter-server/jupyverse/pull/287) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.1.4/CONTRIBUTING.md` & `jupyverse-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/config.yaml` & `jupyverse-0.1.5/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/mkdocs.yml` & `jupyverse-0.1.5/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 site_name: Jupyverse
 site_description: A composable Jupyter server based on FastAPI
+repo_url: https://github.com/jupyter-server/jupyverse
 
 theme:
   name: 'material'
   palette:
     - scheme: default
       primary: 'black'
       accent: 'black'
@@ -21,14 +22,15 @@
   features:
     - navigation.instant
     - navigation.top
     - navigation.sections
     - search.suggest
     - search.highlight
     - content.code.annotate
+    - content.code.copy
 
 nav:
 - Overview: index.md
 - install.md
 - Usage:
   - usage/single_user.md
   - usage/multi_user.md
```

### Comparing `jupyverse-0.1.4/.devcontainer/devcontainer.json` & `jupyverse-0.1.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/.github/workflows/check-release.yml` & `jupyverse-0.1.5/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/.github/workflows/main.yml` & `jupyverse-0.1.5/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,16 @@
       run: |
         pip install hatch
         hatch env create dev.jupyterlab-auth
 
     - name: Check types
       run: |
         hatch run dev.jupyterlab-noauth:typecheck
-        hatch run dev.jupyterlab-noauth:typecheck
         hatch run dev.jupyterlab-auth:typecheck
-        hatch run dev.retrolab-auth_fief:typecheck
+        hatch run dev.jupyterlab-auth_fief:typecheck
+        hatch run dev.retrolab-noauth:typecheck
         hatch run dev.retrolab-auth:typecheck
         hatch run dev.retrolab-auth_fief:typecheck
 
     - name: Run tests
       run: |
         hatch run dev.jupyterlab-auth:test
```

### Comparing `jupyverse-0.1.4/binder/jupyter_notebook_config.py` & `jupyverse-0.1.5/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/index.md` & `jupyverse-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/install.md` & `jupyverse-0.1.5/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/jupyter.svg` & `jupyverse-0.1.5/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/plugins/auth.md` & `jupyverse-0.1.5/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/usage/microservices.md` & `jupyverse-0.1.5/docs/usage/microservices.md`

 * *Files 8% similar despite different names*

```diff
@@ -68,33 +68,33 @@
 pip install fps-auth
 pip install fps-contents
 pip install fps-frontend
 pip install fps-lab
 pip install fps-jupyterlab
 pip install fps-login
 ```
-Now just launch Jupyverse at port `8001`:
+Now we launch Jupyverse at port `8001` and pass our own authentication token. In production, you would either create your own token, or let Jupyverse create it, and copy/paste it for server 2.
 ```bash
-jupyverse --port=8001
+jupyverse --port=8001 --set auth.token=5e9b01f993bc4fb48b2bf6958fd22981
 ```
 If you open your browser at `http://127.0.0.1:8000` (the URL of the Nginx reverse proxy), you should see the JupyterLab UI you're used to. But if you look closer, you can see that there is no icon for kernels in the launcher tab. And in the terminal where you launched Jupyverse, you will see a bunch of `404` for requests at e.g. `GET /api/kernels`. This is expected, because we didn't install the kernels plugin. You can still use JupyterLab if you don't want to execute a notebook, for instance. But let's close it for now, and install the kernels plugin in another Jupyverse instance.
 
 ### Server 2: the kernels API
 
 Let's create a new environment in a new terminal:
 ```bash
 micromamba create -n jupyverse2
 micromamba activate jupyverse2
 micromamba install -c conda-forge python
 ```
-This time, we only want to install the kernels plugin. It also requires an authentication system (for the sake of simplicity we will install `fps-noauth` which gives unrestricted access) and the frontend plugin. Let's not forget to install a kernel, such as `ipykernel`:
+This time, we only want to install the kernels plugin. Let's not forget to install a kernel, such as `ipykernel`:
 ```bash
 pip install fps-kernels
-pip install fps-noauth
+pip install fps-auth
 pip install fps-frontend
 pip install ipykernel
 ```
-Launch Juyverse at port `8002`:
+Launch Juyverse at port `8002` with the same authentication token as for server 1:
 ```bash
-jupyverse --port=8002
+jupyverse --port=8002 --set auth.token=5e9b01f993bc4fb48b2bf6958fd22981
 ```
 Now if you re-open a browser at `http://127.0.0.1:8000`, you should be able to create or open a notebook, and execute it.
```

### Comparing `jupyverse-0.1.4/docs/usage/multi_user.md` & `jupyverse-0.1.5/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/docs/usage/single_user.md` & `jupyverse-0.1.5/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/COPYING.md` & `jupyverse-0.1.5/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/pyproject.toml` & `jupyverse-0.1.5/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.1.5/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth/COPYING.md` & `jupyverse-0.1.5/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth/pyproject.toml` & `jupyverse-0.1.5/plugins/kernels/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_auth"
-description = "An FPS plugin for the authentication API"
+name = "fps_kernels"
+description = "An FPS plugin for the kernels API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
-dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
-    "aiosqlite",
-    "fastapi-users[sqlalchemy,oauth] >=10.1.4,<11",
-    "sqlalchemy >=1,<2",
+    "pyzmq",
+    "websockets",
+    "python-dateutil",
+    "types-python-dateutil",
+    "watchfiles >=0.16.1,<1",
     "jupyverse-api >=0.1.2,<1",
 ]
-
+dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -32,12 +33,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {auth = "fps_auth.main:AuthComponent"}
-"jupyverse.components" = {auth = "fps_auth.main:AuthComponent"}
+"asphalt.components"   = {kernels = "fps_kernels.main:KernelsComponent"}
+"jupyverse.components" = {kernels = "fps_kernels.main:KernelsComponent"}
 
 [tool.hatch.version]
-path = "fps_auth/__init__.py"
+path = "fps_kernels/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/auth/fps_auth/backends.py` & `jupyverse-0.1.5/plugins/auth/fps_auth/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import uuid
 from dataclasses import dataclass
-from typing import Any, Dict, Generic, List, Optional, Tuple
+from typing import Any, Dict, Generic, List, Optional, Tuple, cast
 
 import httpx
 from fastapi import Depends, HTTPException, Response, WebSocket, status
 from fastapi_users import (
     BaseUserManager,
     FastAPIUsers,
     UUIDIDMixin,
@@ -48,19 +48,19 @@
     class NoAuthScheme:
         def __call__(self):
             return "noauth"
 
     class NoAuthTransport(Transport):
         scheme = NoAuthScheme()  # type: ignore
 
-        async def get_login_response(self, token: str, response: Response):
-            pass
+        async def get_login_response(self, token: str) -> Response:
+            return Response()
 
-        async def get_logout_response(self, response: Response):
-            pass
+        async def get_logout_response(self) -> Response:
+            return Response()
 
         @staticmethod
         def get_openapi_login_responses_success():
             pass
 
         @staticmethod
         def get_openapi_logout_responses_success():
@@ -76,18 +76,19 @@
         async def write_token(self, user: models.UP):
             pass
 
         async def destroy_token(self, token: str, user: models.UP):
             pass
 
     class GitHubTransport(CookieTransport):
-        async def get_login_response(self, token: str, response: Response):
-            await super().get_login_response(token, response)
+        async def get_login_response(self, token: str) -> Response:
+            response = await super().get_login_response(token)
             response.status_code = status.HTTP_302_FOUND
             response.headers["Location"] = "/lab"
+            return response
 
     def get_noauth_strategy() -> NoAuthStrategy:
         return NoAuthStrategy()
 
     def get_jwt_strategy() -> JWTStrategy:
         return JWTStrategy(secret=db.secret, lifetime_seconds=None)
 
@@ -186,27 +187,37 @@
                             user = None
                             break
             else:
                 # "noauth" or "token" authentication
                 if frontend_config.collaborative:
                     if not user and auth_config.mode == "noauth":
                         user = await create_guest(user_manager)
-                        await cookie_authentication.login(get_jwt_strategy(), user, response)
+                        token = await get_jwt_strategy().write_token(user)
+                        cookie_transport = cast(CookieTransport, cookie_authentication.transport)
+                        cookie_transport._set_login_cookie(response, token)
 
                     elif not user and auth_config.mode == "token":
                         global_user = await user_manager.get_by_email(auth_config.global_email)
                         if global_user and global_user.username == token:
                             user = await create_guest(user_manager)
-                            await cookie_authentication.login(get_jwt_strategy(), user, response)
+                            token = await get_jwt_strategy().write_token(user)
+                            cookie_transport = cast(
+                                CookieTransport, cookie_authentication.transport
+                            )
+                            cookie_transport._set_login_cookie(response, token)
                 else:
                     if auth_config.mode == "token":
                         global_user = await user_manager.get_by_email(auth_config.global_email)
                         if global_user and global_user.username == token:
                             user = global_user
-                            await cookie_authentication.login(get_jwt_strategy(), user, response)
+                            token = await get_jwt_strategy().write_token(user)
+                            cookie_transport = cast(
+                                CookieTransport, cookie_authentication.transport
+                            )
+                            cookie_transport._set_login_cookie(response, token)
 
             if user:
                 return user
 
             elif auth_config.login_url:
                 raise RedirectException(auth_config.login_url)
```

### Comparing `jupyverse-0.1.4/plugins/auth/fps_auth/config.py` & `jupyverse-0.1.5/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth/fps_auth/db.py` & `jupyverse-0.1.5/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth/fps_auth/main.py` & `jupyverse-0.1.5/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth/fps_auth/routes.py` & `jupyverse-0.1.5/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth_fief/COPYING.md` & `jupyverse-0.1.5/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth_fief/pyproject.toml` & `jupyverse-0.1.5/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.1.5/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/contents/COPYING.md` & `jupyverse-0.1.5/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/contents/pyproject.toml` & `jupyverse-0.1.5/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.1.5/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/contents/fps_contents/routes.py` & `jupyverse-0.1.5/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/frontend/COPYING.md` & `jupyverse-0.1.5/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/frontend/pyproject.toml` & `jupyverse-0.1.5/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/jupyterlab/COPYING.md` & `jupyverse-0.1.5/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.1.5/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.1.5/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/COPYING.md` & `jupyverse-0.1.5/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/pyproject.toml` & `jupyverse-0.1.5/plugins/login/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_kernels"
-description = "An FPS plugin for the kernels API"
+name = "fps_login"
+description = "An FPS plugin for the login API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
-    "pyzmq",
-    "websockets",
-    "python-dateutil",
-    "types-python-dateutil",
-    "watchfiles >=0.16.1,<1",
-    "jupyverse-api >=0.1.2,<1",
+  "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
@@ -33,12 +28,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {kernels = "fps_kernels.main:KernelsComponent"}
-"jupyverse.components" = {kernels = "fps_kernels.main:KernelsComponent"}
+"asphalt.components"   = {login = "fps_login.main:LoginComponent"}
+"jupyverse.components" = {login = "fps_login.main:LoginComponent"}
 
 [tool.hatch.version]
-path = "fps_kernels/__init__.py"
+path = "fps_login/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.1.5/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/lab/COPYING.md` & `jupyverse-0.1.5/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/lab/pyproject.toml` & `jupyverse-0.1.5/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/lab/fps_lab/main.py` & `jupyverse-0.1.5/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/lab/fps_lab/routes.py` & `jupyverse-0.1.5/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.1.5/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/COPYING.md` & `jupyverse-0.1.5/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/pyproject.toml` & `jupyverse-0.1.5/plugins/retrolab/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_login"
-description = "An FPS plugin for the login API"
+name = "fps_retrolab"
+description = "An FPS plugin for the RetroLab API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
-  "jupyverse-api >=0.1.2,<1",
+    "retrolab",
+    "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
@@ -28,12 +29,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {login = "fps_login.main:LoginComponent"}
-"jupyverse.components" = {login = "fps_login.main:LoginComponent"}
+"asphalt.components"   = {retrolab = "fps_retrolab.main:RetroLabComponent"}
+"jupyverse.components" = {retrolab = "fps_retrolab.main:RetroLabComponent"}
 
 [tool.hatch.version]
-path = "fps_login/__init__.py"
+path = "fps_retrolab/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/routes.py` & `jupyverse-0.1.5/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/index.html` & `jupyverse-0.1.5/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.1.5/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.1.5/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.1.5/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.1.5/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/nbconvert/COPYING.md` & `jupyverse-0.1.5/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/nbconvert/pyproject.toml` & `jupyverse-0.1.5/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.1.5/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/noauth/COPYING.md` & `jupyverse-0.1.5/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/noauth/pyproject.toml` & `jupyverse-0.1.5/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.1.5/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/resource_usage/COPYING.md` & `jupyverse-0.1.5/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/resource_usage/pyproject.toml` & `jupyverse-0.1.5/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.1.5/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/retrolab/COPYING.md` & `jupyverse-0.1.5/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/retrolab/pyproject.toml` & `jupyverse-0.1.5/plugins/terminals/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_retrolab"
-description = "An FPS plugin for the RetroLab API"
+name = "fps_terminals"
+description = "An FPS plugin for the terminals API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
-    "retrolab",
+    "websockets",
+    "pywinpty;platform_system=='Windows'",
     "jupyverse-api >=0.1.2,<1",
 ]
-dynamic = [ "version",]
+dynamic = ["version"]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -29,12 +30,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {retrolab = "fps_retrolab.main:RetroLabComponent"}
-"jupyverse.components" = {retrolab = "fps_retrolab.main:RetroLabComponent"}
+"asphalt.components"   = {terminals = "fps_terminals.main:TerminalsComponent"}
+"jupyverse.components" = {terminals = "fps_terminals.main:TerminalsComponent"}
 
 [tool.hatch.version]
-path = "fps_retrolab/__init__.py"
+path = "fps_terminals/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.1.5/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.1.5/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/terminals/COPYING.md` & `jupyverse-0.1.5/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/terminals/pyproject.toml` & `jupyverse-0.1.5/plugins/yjs/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_terminals"
-description = "An FPS plugin for the terminals API"
-keywords = ["jupyter", "server", "fastapi", "plugins"]
+name = "fps_yjs"
+description = "An FPS plugin for the Yjs API"
+keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-    "websockets",
-    "pywinpty;platform_system=='Windows'",
+    "jupyter_ydoc >=0.3.4,<0.4.0",
+    "ypy-websocket >=0.8.2,<1",
+    "y-py >=0.6.0,<0.7.0",
     "jupyverse-api >=0.1.2,<1",
 ]
-dynamic = ["version"]
+dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -30,12 +31,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {terminals = "fps_terminals.main:TerminalsComponent"}
-"jupyverse.components" = {terminals = "fps_terminals.main:TerminalsComponent"}
+"asphalt.components"   = {yjs = "fps_yjs.main:YjsComponent"}
+"jupyverse.components" = {yjs = "fps_yjs.main:YjsComponent"}
 
 [tool.hatch.version]
-path = "fps_terminals/__init__.py"
+path = "fps_yjs/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.1.5/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.1.5/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.1.5/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.1.5/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/yjs/COPYING.md` & `jupyverse-0.1.5/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/yjs/pyproject.toml` & `jupyverse-0.1.5/plugins/auth/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_yjs"
-description = "An FPS plugin for the Yjs API"
-keywords = [ "jupyter", "server", "fastapi", "plugins" ]
+name = "fps_auth"
+description = "An FPS plugin for the authentication API"
+keywords = ["jupyter", "server", "fastapi", "plugins"]
+dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
-    "jupyter_ydoc >=0.3.4,<0.4.0",
-    "ypy-websocket >=0.8.2,<1",
-    "y-py >=0.6.0,<0.7.0",
+    "aiosqlite",
+    "fastapi-users[sqlalchemy,oauth] >=11,<12",
+    "sqlalchemy >=1,<2",
     "jupyverse-api >=0.1.2,<1",
 ]
-dynamic = [ "version",]
+
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -31,12 +32,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {yjs = "fps_yjs.main:YjsComponent"}
-"jupyverse.components" = {yjs = "fps_yjs.main:YjsComponent"}
+"asphalt.components"   = {auth = "fps_auth.main:AuthComponent"}
+"jupyverse.components" = {auth = "fps_auth.main:AuthComponent"}
 
 [tool.hatch.version]
-path = "fps_yjs/__init__.py"
+path = "fps_auth/__init__.py"
```

### Comparing `jupyverse-0.1.4/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.1.5/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.1.5/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/conftest.py` & `jupyverse-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/test_auth.py` & `jupyverse-0.1.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/test_contents.py` & `jupyverse-0.1.5/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/test_kernels.py` & `jupyverse-0.1.5/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/test_server.py` & `jupyverse-0.1.5/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/test_settings.py` & `jupyverse-0.1.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/tests/utils.py` & `jupyverse-0.1.5/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,30 +26,30 @@
     }
     response = await http.post(f"http://127.0.0.1:{port}/auth/register", json=register_body)
     # check that we cannot register if not logged in
     assert response.status_code == 403
     # log in as admin
     login_body = {"username": "admin@jupyter.com", "password": "jupyverse"}
     response = await http.post(f"http://127.0.0.1:{port}/auth/login", data=login_body)
-    assert response.status_code == 200
+    assert response.status_code == 204
     # register user
     response = await http.post(f"http://127.0.0.1:{port}/auth/register", json=register_body)
     assert response.status_code == 201
 
     # log out
     response = await http.post(f"http://127.0.0.1:{port}/auth/logout")
-    assert response.status_code == 200
+    assert response.status_code == 204
     # check that we can't get our identity, since we're not logged in
     response = await http.get(f"http://127.0.0.1:{port}/api/me")
     assert response.status_code == 403
 
     # log in with registered user
     login_body = {"username": f"{username}@example.com", "password": username}
     response = await http.post(f"http://127.0.0.1:{port}/auth/login", data=login_body)
-    assert response.status_code == 200
+    assert response.status_code == 204
     # we should now have a cookie
     assert "fastapiusersauth" in http.cookies
     # check our identity, since we're logged in
     response = await http.get(
         f"http://127.0.0.1:{port}/api/me", params={"permissions": permissions}
     )
     assert response.status_code == 200
```

### Comparing `jupyverse-0.1.4/tests/data/notebook0.ipynb` & `jupyverse-0.1.5/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/.gitignore` & `jupyverse-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/COPYING.md` & `jupyverse-0.1.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/README.md` & `jupyverse-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/pyproject.toml` & `jupyverse-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.4/PKG-INFO` & `jupyverse-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

