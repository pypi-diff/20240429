# Comparing `tmp/jupyverse-0.5.0.tar.gz` & `tmp/jupyverse-0.5.1.tar.gz`

## Comparing `jupyverse-0.5.0.tar` & `jupyverse-0.5.1.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    76121 2020-02-02 00:00:00.000000 jupyverse-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.5.0/config.yaml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.5.0/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/environment.yml
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/index.md
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/kernels.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/notebook.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/yjs.md
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/tutorials/jupyterhub_jupyverse_deployment.md
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/tutorials/standalone_jupyverse_deployment.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/notebook/__init__.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.5.0/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.5.0/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/COPYING.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/pyproject.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/main.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/py.typed
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/utils.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yblob.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yfile.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yunicode.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py
--rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/__init__.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/widgets.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_app.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_contents.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_execute.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_kernels.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_server.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/data/notebook1.ipynb
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/COPYING.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyverse-0.5.0/README.md
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 jupyverse-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 jupyverse-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    77661 2020-02-02 00:00:00.000000 jupyverse-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.5.1/config.yaml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.5.1/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.5.1/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.5.1/binder/environment.yml
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyverse-0.5.1/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.5.1/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.5.1/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/index.md
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/notebook.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/tutorials/jupyterhub_jupyverse_deployment.md
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/tutorials/standalone_jupyverse_deployment.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupyverse-0.5.1/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/notebook/__init__.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.5.1/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.5.1/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.5.1/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/COPYING.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/fps_notebook/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/fps_notebook/main.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/notebook/fps_notebook/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/utils.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/yblob.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/yfile.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/ynotebook.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/yunicode.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/awareness.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
+-rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/yroom.py
+-rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/ystore.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/yutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywidgets/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyverse-0.5.1/plugins/yjs/fps_yjs/ywidgets/widgets.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_app.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_contents.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_execute.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_kernels.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_server.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.1/tests/data/notebook1.ipynb
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.5.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.1/COPYING.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyverse-0.5.1/README.md
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 jupyverse-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyverse-0.5.1/PKG-INFO
```

### Comparing `jupyverse-0.5.0/.pre-commit-config.yaml` & `jupyverse-0.5.1/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -12,11 +12,11 @@
       - id: check-yaml
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.5.0/CHANGELOG.md` & `jupyverse-0.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.5.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.5.0...4ddd9ab118c9ed47340d44b6eb57b68894b1bcc5))
+
+### Merged PRs
+
+- Check terminal websocket before removing it [#405](https://github.com/jupyter-server/jupyverse/pull/405) ([@davidbrochart](https://github.com/davidbrochart))
+- Update documentation URL [#404](https://github.com/jupyter-server/jupyverse/pull/404) ([@davidbrochart](https://github.com/davidbrochart))
+- Set watchfiles log level to WARNING [#403](https://github.com/jupyter-server/jupyverse/pull/403) ([@davidbrochart](https://github.com/davidbrochart))
+- Update ypywidgets v0.7.0 for tests [#400](https://github.com/jupyter-server/jupyverse/pull/400) ([@davidbrochart](https://github.com/davidbrochart))
+- Remove output trailing newline [#399](https://github.com/jupyter-server/jupyverse/pull/399) ([@davidbrochart](https://github.com/davidbrochart))
+- Save anonymous user info in database [#397](https://github.com/jupyter-server/jupyverse/pull/397) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2024-04-12&to=2024-04-29&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2024-04-12..2024-04-29&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2024-04-12..2024-04-29&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.5.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.4.2...66aac71cf07cbc14c5196cc1c144b9965fec7d2c))
 
 ### Merged PRs
 
 - Replace RetroLab with Notebook [#396](https://github.com/jupyter-server/jupyverse/pull/396) ([@davidbrochart](https://github.com/davidbrochart))
@@ -13,16 +34,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2024-01-02&to=2024-04-12&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2024-01-02..2024-04-12&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2024-01-02..2024-04-12&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.4.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.4.1...2f084c7c744bb2d2865bdad223c680eca5c8a2cb))
 
 ### Merged PRs
 
 - Update pycrdt >=0.8.2 [#379](https://github.com/jupyter-server/jupyverse/pull/379) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.5.0/CONTRIBUTING.md` & `jupyverse-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/config.yaml` & `jupyverse-0.5.1/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/mkdocs.yml` & `jupyverse-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/.devcontainer/devcontainer.json` & `jupyverse-0.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/.github/workflows/check-release.yml` & `jupyverse-0.5.1/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/.github/workflows/test.yml` & `jupyverse-0.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/binder/jupyter_notebook_config.py` & `jupyverse-0.5.1/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/index.md` & `jupyverse-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/install.md` & `jupyverse-0.5.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/jupyter.svg` & `jupyverse-0.5.1/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/plugins/auth.md` & `jupyverse-0.5.1/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/tutorials/jupyterhub_jupyverse_deployment.md` & `jupyverse-0.5.1/docs/tutorials/jupyterhub_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/tutorials/standalone_jupyverse_deployment.md` & `jupyverse-0.5.1/docs/tutorials/standalone_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/usage/microservices.md` & `jupyverse-0.5.1/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/usage/multi_user.md` & `jupyverse-0.5.1/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/docs/usage/single_user.md` & `jupyverse-0.5.1/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/COPYING.md` & `jupyverse-0.5.1/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/pyproject.toml` & `jupyverse-0.5.1/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/notebook/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.5.1/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/notebooks/admin_users.ipynb` & `jupyverse-0.5.1/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/notebooks/admin_users.py` & `jupyverse-0.5.1/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/COPYING.md` & `jupyverse-0.5.1/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/pyproject.toml` & `jupyverse-0.5.1/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/fps_auth/backends.py` & `jupyverse-0.5.1/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/fps_auth/config.py` & `jupyverse-0.5.1/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/fps_auth/db.py` & `jupyverse-0.5.1/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/fps_auth/main.py` & `jupyverse-0.5.1/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth/fps_auth/routes.py` & `jupyverse-0.5.1/plugins/auth/fps_auth/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                     users = (await session.execute(statement)).unique().all()
                 return [usr.User for usr in users if usr.User.is_active]
 
             @router.get("/api/me")
             async def get_api_me(
                 permissions: Optional[str] = None,
                 user: UserRead = Depends(backend.current_user()),
+                update_user = Depends(backend.update_user),
             ):
                 checked_permissions: Dict[str, List[str]] = {}
                 if permissions is None:
                     permissions = "{}"
                 else:
                     permissions = permissions.replace("'", '"')
                 permissions_dict = json.loads(permissions)
@@ -92,14 +93,22 @@
 
                 keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
                 identity = {k: getattr(user, k) for k in keys}
                 if not identity["name"] and not identity["display_name"]:
                     moon = get_anonymous_username()
                     identity["name"] = f"Anonymous {moon}"
                     identity["display_name"] = f"Anonymous {moon}"
+                    identity["initials"] = f"A{moon[0]}"
+                    await update_user(
+                        dict(
+                            name=identity["name"],
+                            display_name=identity["display_name"],
+                            permissions=checked_permissions,
+                        )
+                    )
                 return {
                     "identity": identity,
                     "permissions": checked_permissions,
                 }
 
             # redefine GET /me because we want our current_user dependency
             # it is first defined in users_router and so it wins over the one in
```

### Comparing `jupyverse-0.5.0/plugins/auth_fief/COPYING.md` & `jupyverse-0.5.1/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_fief/pyproject.toml` & `jupyverse-0.5.1/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/config.py` & `jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.5.1/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_jupyterhub/COPYING.md` & `jupyverse-0.5.1/plugins/auth_jupyterhub/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_jupyterhub/pyproject.toml` & `jupyverse-0.5.1/plugins/auth_jupyterhub/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py` & `jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py` & `jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py` & `jupyverse-0.5.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/contents/COPYING.md` & `jupyverse-0.5.1/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/contents/pyproject.toml` & `jupyverse-0.5.1/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.5.1/plugins/contents/fps_contents/fileid.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 import aiosqlite
 from anyio import Path
 from watchfiles import Change, awatch
 
 from jupyverse_api import Singleton
 
-logger = logging.getLogger("contents")
+contents_logger = logging.getLogger("contents")
+watchfiles_logger = logging.getLogger("watchfiles")
+watchfiles_logger.setLevel(logging.WARNING)
 
 
 class Watcher:
     def __init__(self, path: str) -> None:
         self.path = path
         self._event = asyncio.Event()
 
@@ -106,54 +108,54 @@
                     added_paths = set()
                     for change, changed_path in changes:
                         # get relative path
                         changed_path = Path(changed_path).relative_to(await Path().absolute())
                         changed_path_str = str(changed_path)
 
                         if change == Change.deleted:
-                            logger.debug("File %s was deleted", changed_path_str)
+                            contents_logger.debug("File %s was deleted", changed_path_str)
                             async with db.execute(
                                 "SELECT COUNT(*) FROM fileids WHERE path = ?", (changed_path_str,)
                             ) as cursor:
                                 if not (await cursor.fetchone())[0]:
                                     # path is not indexed, ignore
-                                    logger.debug(
+                                    contents_logger.debug(
                                         "File %s is not indexed, ignoring", changed_path_str
                                     )
                                     continue
                             # path is indexed
                             await maybe_rename(
                                 db, changed_path_str, deleted_paths, added_paths, False
                             )
                         elif change == Change.added:
-                            logger.debug("File %s was added", changed_path_str)
+                            contents_logger.debug("File %s was added", changed_path_str)
                             await maybe_rename(
                                 db, changed_path_str, added_paths, deleted_paths, True
                             )
                         elif change == Change.modified:
-                            logger.debug("File %s was modified", changed_path_str)
+                            contents_logger.debug("File %s was modified", changed_path_str)
                             if changed_path_str == self.db_path:
                                 continue
                             async with db.execute(
                                 "SELECT COUNT(*) FROM fileids WHERE path = ?", (changed_path_str,)
                             ) as cursor:
                                 if not (await cursor.fetchone())[0]:
                                     # path is not indexed, ignore
-                                    logger.debug(
+                                    contents_logger.debug(
                                         "File %s is not indexed, ignoring", changed_path_str
                                     )
                                     continue
                             mtime = (await changed_path.stat()).st_mtime
                             await db.execute(
                                 "UPDATE fileids SET mtime = ? WHERE path = ?",
                                 (mtime, changed_path_str),
                             )
 
                     for path in deleted_paths - added_paths:
-                        logger.debug("Unindexing file %s ", path)
+                        contents_logger.debug("Unindexing file %s ", path)
                         await db.execute("DELETE FROM fileids WHERE path = ?", (path,))
                     await db.commit()
 
             for change in changes:
                 changed_path = change[1]
                 # get relative path
                 relative_changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
@@ -199,12 +201,12 @@
     for other_path in other_paths:
         mtime2 = await get_mtime(other_path, db_or_fs2)
         if mtime1 == mtime2:
             # same files, according to modification times
             path1, path2 = changed_path, other_path
             if is_added_path:
                 path1, path2 = path2, path1
-            logger.debug("File %s was renamed to %s", path1, path2)
+            contents_logger.debug("File %s was renamed to %s", path1, path2)
             await db.execute("UPDATE fileids SET path = ? WHERE path = ?", (path2, path1))
             other_paths.remove(other_path)
             return
     changed_paths.add(changed_path)
```

### Comparing `jupyverse-0.5.0/plugins/contents/fps_contents/routes.py` & `jupyverse-0.5.1/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/frontend/COPYING.md` & `jupyverse-0.5.1/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/frontend/pyproject.toml` & `jupyverse-0.5.1/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/jupyterlab/COPYING.md` & `jupyverse-0.5.1/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.5.1/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.5.1/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/COPYING.md` & `jupyverse-0.5.1/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/pyproject.toml` & `jupyverse-0.5.1/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,33 +219,36 @@
 
     async def _handle_outputs(self, outputs: Array, msg: Dict[str, Any]):
         msg_type = msg["header"]["msg_type"]
         content = msg["content"]
         if msg_type == "stream":
             with outputs.doc.transaction():
                 # TODO: uncomment when changes are made in jupyter-ydoc
+                text = content["text"]
+                if text.endswith((os.linesep, "\n")):
+                    text = text[:-1]
                 if (not outputs) or (outputs[-1]["name"] != content["name"]):  # type: ignore
                     outputs.append(
                         #Map(
                         #    {
                         #        "name": content["name"],
                         #        "output_type": msg_type,
                         #        "text": Array([content["text"]]),
                         #    }
                         #)
                         {
                             "name": content["name"],
                             "output_type": msg_type,
-                            "text": [content["text"]],
+                            "text": [text],
                         }
                     )
                 else:
                     #outputs[-1]["text"].append(content["text"])  # type: ignore
                     last_output = outputs[-1]
-                    last_output["text"].append(content["text"])  # type: ignore
+                    last_output["text"].append(text)  # type: ignore
                     outputs[-1] = last_output
         elif msg_type in ("display_data", "execute_result"):
             if "application/vnd.jupyter.ywidget-view+json" in content["data"]:
                 # this is a collaborative widget
                 model_id = content["data"]["application/vnd.jupyter.ywidget-view+json"]["model_id"]
                 if self.yjs is not None and self.yjs.widgets is not None:  # type: ignore
                     if model_id in self.yjs.widgets.widgets:  # type: ignore
```

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.5.1/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/lab/COPYING.md` & `jupyverse-0.5.1/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/lab/pyproject.toml` & `jupyverse-0.5.1/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/lab/fps_lab/main.py` & `jupyverse-0.5.1/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/lab/fps_lab/routes.py` & `jupyverse-0.5.1/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.5.1/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/COPYING.md` & `jupyverse-0.5.1/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/pyproject.toml` & `jupyverse-0.5.1/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/routes.py` & `jupyverse-0.5.1/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/index.html` & `jupyverse-0.5.1/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.5.1/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.5.1/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.5.1/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.5.1/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/nbconvert/COPYING.md` & `jupyverse-0.5.1/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/nbconvert/pyproject.toml` & `jupyverse-0.5.1/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.5.1/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/noauth/COPYING.md` & `jupyverse-0.5.1/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/noauth/pyproject.toml` & `jupyverse-0.5.1/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.5.1/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/notebook/COPYING.md` & `jupyverse-0.5.1/plugins/notebook/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/notebook/pyproject.toml` & `jupyverse-0.5.1/plugins/notebook/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/notebook/fps_notebook/main.py` & `jupyverse-0.5.1/plugins/notebook/fps_notebook/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/notebook/fps_notebook/routes.py` & `jupyverse-0.5.1/plugins/notebook/fps_notebook/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/resource_usage/COPYING.md` & `jupyverse-0.5.1/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/resource_usage/pyproject.toml` & `jupyverse-0.5.1/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.5.1/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.5.1/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/terminals/COPYING.md` & `jupyverse-0.5.1/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/terminals/pyproject.toml` & `jupyverse-0.5.1/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.5.1/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.5.1/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.5.1/plugins/terminals/fps_terminals/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,11 @@
             if self.data_or_disconnect is None:
                 await self.websocket.send_json(["disconnect", 1])
             else:
                 for websocket in self.websockets:
                     await websocket.send_json(["stdout", self.data_or_disconnect])
 
     def quit(self, websocket):
-        self.websockets.remove(websocket)
+        if websocket in self.weksockets:
+            self.websockets.remove(websocket)
         if not self.websockets:
             os.close(self.fd)
```

### Comparing `jupyverse-0.5.0/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.5.1/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/webdav/COPYING.md` & `jupyverse-0.5.1/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/webdav/pyproject.toml` & `jupyverse-0.5.1/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/webdav/fps_webdav/routes.py` & `jupyverse-0.5.1/plugins/webdav/fps_webdav/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.5.1/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/COPYING.md` & `jupyverse-0.5.1/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/pyproject.toml` & `jupyverse-0.5.1/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/utils.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/ybasedoc.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yblob.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/yblob.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/ynotebook.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yunicode.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ydocs/yunicode.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/awareness.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/yroom.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/ystore.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywebsocket/yutils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/widgets.py` & `jupyverse-0.5.1/plugins/yjs/fps_yjs/ywidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/conftest.py` & `jupyverse-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_app.py` & `jupyverse-0.5.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_auth.py` & `jupyverse-0.5.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_contents.py` & `jupyverse-0.5.1/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_execute.py` & `jupyverse-0.5.1/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_kernels.py` & `jupyverse-0.5.1/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/test_server.py` & `jupyverse-0.5.1/tests/test_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 "data": {"text/plain": ["3"]},
                 "execution_count": 1.0,
                 "metadata": {},
                 "output_type": "execute_result",
             }
         ]
         assert cells[1]["outputs"] == [
-            {"name": "stdout", "output_type": "stream", "text": ["Hello World!\n"]}
+            {"name": "stdout", "output_type": "stream", "text": ["Hello World!"]}
         ]
         assert cells[2]["outputs"] == [
             {
                 "data": {"text/plain": ["7"]},
                 "execution_count": 3.0,
                 "metadata": {},
                 "output_type": "execute_result",
```

### Comparing `jupyverse-0.5.0/tests/test_settings.py` & `jupyverse-0.5.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/utils.py` & `jupyverse-0.5.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/data/notebook0.ipynb` & `jupyverse-0.5.1/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/tests/data/notebook1.ipynb` & `jupyverse-0.5.1/tests/data/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/.gitignore` & `jupyverse-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/COPYING.md` & `jupyverse-0.5.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.5.0/README.md` & `jupyverse-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 
 A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
 - JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jupyterlab)
 - Jupyter Notebook frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-notebook)
 
-Documentation is available [here](https://davidbrochart.github.io/jupyverse).
+Documentation is available [here](https://jupyter-server.github.io/jupyverse).
 
 ## Motivation
 
 For the motivations behind this project, please refer to this issue in the
 [Jupyter server team compass](https://github.com/jupyter-server/team-compass/issues/11).
```

### Comparing `jupyverse-0.5.0/pyproject.toml` & `jupyverse-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     "pytest-timeout",
     "pytest-env",
     "httpx",
     "httpx-ws >=0.4.1",
     "requests",
     "websockets",
     "ipykernel",
-    "ypywidgets >=0.6.4,<0.7.0",
-    "ypywidgets-textual >=0.2.2,<0.3.0",
+    "ypywidgets >=0.7.0,<0.8.0",
+    "ypywidgets-textual >=0.4.0,<0.5.0",
 ]
 docs = [ "mkdocs", "mkdocs-material" ]
 
 [tool.hatch.envs.dev]
 # TODO: if/when hatch gets support for defining editable dependencies, the
 # pre-install commands here and post-install commands in the matrix can be moved
 # to the dependencies section
@@ -180,16 +180,7 @@
 ]
 
 [tool.hatch.version]
 path = "jupyverse/__init__.py"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
-
-[tool.pixi.project]
-name = ""
-channels = ["conda-forge"]
-platforms = ["linux-64"]
-
-[tool.pixi.dependencies]
-pip = ">=24.0,<25"
-python = "<3.12"
```

### Comparing `jupyverse-0.5.0/PKG-INFO` & `jupyverse-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyverse
-Version: 0.5.0
+Version: 0.5.1
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
@@ -42,27 +42,27 @@
 Requires-Dist: pytest-env; extra == 'test'
 Requires-Dist: pytest-rerunfailures; extra == 'test'
 Requires-Dist: pytest-timeout; extra == 'test'
 Requires-Dist: requests; extra == 'test'
 Requires-Dist: ruff>=0.1.2; extra == 'test'
 Requires-Dist: types-setuptools; extra == 'test'
 Requires-Dist: websockets; extra == 'test'
-Requires-Dist: ypywidgets-textual<0.3.0,>=0.2.2; extra == 'test'
-Requires-Dist: ypywidgets<0.7.0,>=0.6.4; extra == 'test'
+Requires-Dist: ypywidgets-textual<0.5.0,>=0.4.0; extra == 'test'
+Requires-Dist: ypywidgets<0.8.0,>=0.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/test/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 
 # jupyverse
 
 A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
 - JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jupyterlab)
 - Jupyter Notebook frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-notebook)
 
-Documentation is available [here](https://davidbrochart.github.io/jupyverse).
+Documentation is available [here](https://jupyter-server.github.io/jupyverse).
 
 ## Motivation
 
 For the motivations behind this project, please refer to this issue in the
 [Jupyter server team compass](https://github.com/jupyter-server/team-compass/issues/11).
```

