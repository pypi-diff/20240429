# Comparing `tmp/mountaineer-0.4.2.dev2.tar.gz` & `tmp/mountaineer-0.4.2.dev3.tar.gz`

## Comparing `mountaineer-0.4.2.dev2.tar` & `mountaineer-0.4.2.dev3.tar`

### file list

```diff
@@ -1,259 +1,260 @@
--rw-r--r--   0     1001      127      269 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev2/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    14036 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    19767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/README.md
--rw-r--r--   0     1001      127      105 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4677 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    14334 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     4816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10097 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     1924 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8419 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cache.py
--rw-r--r--   0     1001      127    18059 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cli.py
--rw-r--r--   0     1001      127    11390 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     4002 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    10172 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    29025 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11199 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     5070 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15443 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2039 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/logging.py
--rw-r--r--   0     1001      127    12826 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/webservice.py
--rw-r--r--   0     1001      127   125089 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-04-23 16:35:54.000000 mountaineer-0.4.2.dev2/Cargo.lock
--rw-r--r--   0     1001      127     1599 2024-04-23 16:35:52.000000 mountaineer-0.4.2.dev2/pyproject.toml
--rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev2/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/build.rs
+-rw-r--r--   0     1001      127     4195 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/go.sum
+-rw-r--r--   0     1001      127     6499 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev3/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    20289 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/README.md
+-rw-r--r--   0     1001      127      105 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   109872 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4677 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      479 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     4816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10097 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8419 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18916 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cache.py
+-rw-r--r--   0     1001      127    19226 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10172 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    29298 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11199 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5070 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/config.py
+-rw-r--r--   0     1001      127      197 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/console.py
+-rw-r--r--   0     1001      127       40 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    16439 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2313 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12826 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8414 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127     1213 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   127639 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/lexers.rs
+-rw-r--r--   0     1001      127     9118 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-29 06:28:07.000000 mountaineer-0.4.2.dev3/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-29 06:28:33.000000 mountaineer-0.4.2.dev3/Cargo.lock
+-rw-r--r--   0     1001      127     1624 2024-04-29 06:28:24.000000 mountaineer-0.4.2.dev3/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev3/PKG-INFO
```

### Comparing `mountaineer-0.4.2.dev2/src_go/build.rs` & `mountaineer-0.4.2.dev3/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src_go/go/js_build.go` & `mountaineer-0.4.2.dev3/src_go/go/js_build.go`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 package main
 
 import (
-	"C"
 	"fmt"
-	"sync"
-)
-import (
 	"os"
-	"unsafe"
+	"sync"
 
 	"github.com/evanw/esbuild/pkg/api"
 )
 
+// #include <stdint.h>
+//
+// extern void rust_callback(int32_t);
+import "C"
+
 var (
 	mutex    sync.Mutex
 	contexts = make(map[int]*ESBuildContext)
 	nextID   = 1
 )
 
 type ESBuildContext struct {
@@ -84,15 +85,14 @@
 
 	id := nextID
 	nextID++
 	contexts[id] = &ESBuildContext{
 		Filename: filename,
 		Context:  ctx,
 	}
-	fmt.Printf("Created context with ID %d for %s\n", id, filename)
 	return C.int(id), nil
 }
 
 //export RebuildContext
 func RebuildContext(id C.int) (returnError *C.char) {
 	mutex.Lock()
 
@@ -110,77 +110,28 @@
 		for _, err := range result.Errors {
 			errorString += ParseErrorLocation(err.Location)
 			errorString += fmt.Sprintf("%s\n\n", err.Text)
 		}
 		return C.CString(errorString)
 	}
 
-	// fmt.Printf("#### START ####\n")
-	// fmt.Printf("Filename: %s (output: %d)\n", context.Filename, len(result.OutputFiles))
-
 	for i := range result.OutputFiles {
 		outputFile := result.OutputFiles[i]
-		// fmt.Printf("------------\n")
-		// fmt.Printf("Output file: %s\n", outputFile)
-		// fmt.Printf("Path: %s\n", outputFile.Path)
-		// fmt.Printf("Contents: %s\n", outputFile.Contents)
-
 		// Write the output to a file
 		err := os.WriteFile(outputFile.Path, outputFile.Contents, 0644)
 		if err != nil {
 			// Log the error
 			fmt.Println(err)
 			return C.CString(err.Error())
 		}
 	}
 
-	// fmt.Printf("#### DONE ####\n")
 	return nil
 }
 
-//export RebuildContexts
-func RebuildContexts(ids *C.int, count C.int) (returnErrors **C.char, returnErrorCount C.int) {
-	// Convert C array to Go slice
-	goIDs := make([]int, count)
-	for i := 0; i < int(count); i++ {
-		goIDs[i] = int(*(*C.int)(unsafe.Pointer(uintptr(unsafe.Pointer(ids)) + uintptr(i)*unsafe.Sizeof(*ids))))
-	}
-
-	// Semaphore channel to limit concurrency
-	var sem = make(chan struct{}, 25)
-
-	errors := make([]*C.char, 0)
-	var wg sync.WaitGroup
-	for _, id := range goIDs {
-		wg.Add(1)
-		sem <- struct{}{} // Acquire semaphore
-
-		// Launch a goroutine for each id
-		go func(id int) {
-			defer wg.Done()
-			defer func() { <-sem }() // Release semaphore
-
-			err := RebuildContext(C.int(id))
-			if err != nil {
-				errors = append(errors, err)
-			}
-		}(id)
-	}
-
-	wg.Wait()
-
-	// Convert slice to C array
-	errorsArray := (**C.char)(C.malloc(C.size_t(len(errors)) * C.size_t(unsafe.Sizeof(uintptr(0)))))
-	for i, err := range errors {
-		*(**C.char)(unsafe.Pointer(uintptr(unsafe.Pointer(errorsArray)) + uintptr(i)*unsafe.Sizeof(uintptr(0)))) = err
-	}
-
-	return errorsArray, C.int(len(errors))
-}
-
 //export RemoveContext
 func RemoveContext(id C.int) {
 	mutex.Lock()
 	defer mutex.Unlock()
 
 	// Dispose of the ESBuild context to free up resources
 	context, exists := contexts[int(id)]
```

### Comparing `mountaineer-0.4.2.dev2/src_go/src/lib.rs` & `mountaineer-0.4.2.dev3/src_go/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,357 +4,404 @@
 00000030: 616d 656c 5f63 6173 655f 7479 7065 7329  amel_case_types)
 00000040: 5d0a 2321 5b61 6c6c 6f77 286e 6f6e 5f73  ].#![allow(non_s
 00000050: 6e61 6b65 5f63 6173 6529 5d0a 0a69 6e63  nake_case)]..inc
 00000060: 6c75 6465 2128 636f 6e63 6174 2128 656e  lude!(concat!(en
 00000070: 7621 2822 4f55 545f 4449 5222 292c 2022  v!("OUT_DIR"), "
 00000080: 2f62 696e 6469 6e67 732e 7273 2229 293b  /bindings.rs"));
 00000090: 0a0a 6578 7465 726e 2063 7261 7465 206c  ..extern crate l
-000000a0: 6962 633b 0a0a 7573 6520 6c69 6263 3a3a  ibc;..use libc::
-000000b0: 6672 6565 3b0a 7573 6520 7374 643a 3a66  free;.use std::f
-000000c0: 6669 3a3a 7b63 5f69 6e74 2c20 4353 7472  fi::{c_int, CStr
-000000d0: 696e 677d 3b0a 0a70 7562 2066 6e20 6765  ing};..pub fn ge
-000000e0: 745f 6275 696c 645f 636f 6e74 6578 7428  t_build_context(
-000000f0: 0a20 2020 2066 696c 656e 616d 653a 2026  .    filename: &
-00000100: 7374 722c 0a20 2020 206e 6f64 655f 6d6f  str,.    node_mo
-00000110: 6475 6c65 735f 7061 7468 3a20 2673 7472  dules_path: &str
-00000120: 2c0a 2020 2020 656e 7669 726f 6e6d 656e  ,.    environmen
-00000130: 743a 2026 7374 722c 0a20 2020 206c 6976  t: &str,.    liv
-00000140: 655f 7265 6c6f 6164 5f70 6f72 743a 2069  e_reload_port: i
-00000150: 3332 2c0a 2020 2020 6973 5f73 6572 7665  32,.    is_serve
-00000160: 723a 2062 6f6f 6c2c 0a29 202d 3e20 5265  r: bool,.) -> Re
-00000170: 7375 6c74 3c63 5f69 6e74 2c20 5374 7269  sult<c_int, Stri
-00000180: 6e67 3e20 7b0a 2020 2020 6c65 7420 635f  ng> {.    let c_
-00000190: 6669 6c65 6e61 6d65 203d 2043 5374 7269  filename = CStri
-000001a0: 6e67 3a3a 6e65 7728 6669 6c65 6e61 6d65  ng::new(filename
-000001b0: 292e 756e 7772 6170 2829 3b0a 2020 2020  ).unwrap();.    
-000001c0: 6c65 7420 635f 6e6f 6465 5f6d 6f64 756c  let c_node_modul
-000001d0: 6573 5f70 6174 6820 3d20 4353 7472 696e  es_path = CStrin
-000001e0: 673a 3a6e 6577 286e 6f64 655f 6d6f 6475  g::new(node_modu
-000001f0: 6c65 735f 7061 7468 292e 756e 7772 6170  les_path).unwrap
-00000200: 2829 3b0a 2020 2020 6c65 7420 635f 656e  ();.    let c_en
-00000210: 7669 726f 6e6d 656e 7420 3d20 4353 7472  vironment = CStr
-00000220: 696e 673a 3a6e 6577 2865 6e76 6972 6f6e  ing::new(environ
-00000230: 6d65 6e74 292e 756e 7772 6170 2829 3b0a  ment).unwrap();.
-00000240: 2020 2020 6c65 7420 6973 5f73 6572 7665      let is_serve
-00000250: 7220 3d20 6966 2069 735f 7365 7276 6572  r = if is_server
-00000260: 207b 2031 207d 2065 6c73 6520 7b20 3020   { 1 } else { 0 
-00000270: 7d3b 0a0a 2020 2020 756e 7361 6665 207b  };..    unsafe {
-00000280: 0a20 2020 2020 2020 206c 6574 2072 6573  .        let res
-00000290: 756c 7420 3d20 4765 7442 7569 6c64 436f  ult = GetBuildCo
-000002a0: 6e74 6578 7428 0a20 2020 2020 2020 2020  ntext(.         
-000002b0: 2020 2063 5f66 696c 656e 616d 652e 696e     c_filename.in
-000002c0: 746f 5f72 6177 2829 2c0a 2020 2020 2020  to_raw(),.      
-000002d0: 2020 2020 2020 635f 6e6f 6465 5f6d 6f64        c_node_mod
-000002e0: 756c 6573 5f70 6174 682e 696e 746f 5f72  ules_path.into_r
-000002f0: 6177 2829 2c0a 2020 2020 2020 2020 2020  aw(),.          
-00000300: 2020 635f 656e 7669 726f 6e6d 656e 742e    c_environment.
-00000310: 696e 746f 5f72 6177 2829 2c0a 2020 2020  into_raw(),.    
-00000320: 2020 2020 2020 2020 6c69 7665 5f72 656c          live_rel
-00000330: 6f61 645f 706f 7274 2c0a 2020 2020 2020  oad_port,.      
-00000340: 2020 2020 2020 6973 5f73 6572 7665 722c        is_server,
-00000350: 0a20 2020 2020 2020 2029 3b0a 2020 2020  .        );.    
-00000360: 2020 2020 6c65 7420 6964 203d 2072 6573      let id = res
-00000370: 756c 742e 7230 3b0a 2020 2020 2020 2020  ult.r0;.        
-00000380: 6c65 7420 6572 726f 7220 3d20 7265 7375  let error = resu
-00000390: 6c74 2e72 313b 0a0a 2020 2020 2020 2020  lt.r1;..        
-000003a0: 6966 2065 7272 6f72 2e69 735f 6e75 6c6c  if error.is_null
-000003b0: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
-000003c0: 204f 6b28 6964 290a 2020 2020 2020 2020   Ok(id).        
-000003d0: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-000003e0: 2020 2020 206c 6574 2065 7272 6f72 5f73       let error_s
-000003f0: 7472 203d 2043 5374 7269 6e67 3a3a 6672  tr = CString::fr
-00000400: 6f6d 5f72 6177 2865 7272 6f72 293b 0a20  om_raw(error);. 
-00000410: 2020 2020 2020 2020 2020 206c 6574 2065             let e
-00000420: 7272 6f72 5f73 7472 696e 6720 3d20 6572  rror_string = er
-00000430: 726f 725f 7374 720a 2020 2020 2020 2020  ror_str.        
-00000440: 2020 2020 2020 2020 2e69 6e74 6f5f 7374          .into_st
-00000450: 7269 6e67 2829 0a20 2020 2020 2020 2020  ring().         
-00000460: 2020 2020 2020 202e 756e 7772 6170 5f6f         .unwrap_o
-00000470: 725f 656c 7365 287c 5f7c 2053 7472 696e  r_else(|_| Strin
-00000480: 673a 3a66 726f 6d28 2255 6e6b 6e6f 776e  g::from("Unknown
-00000490: 2065 7272 6f72 2229 293b 0a20 2020 2020   error"));.     
-000004a0: 2020 2020 2020 2045 7272 2865 7272 6f72         Err(error
-000004b0: 5f73 7472 696e 6729 0a20 2020 2020 2020  _string).       
-000004c0: 207d 0a20 2020 207d 0a7d 0a0a 7075 6220   }.    }.}..pub 
-000004d0: 666e 2072 6562 7569 6c64 5f63 6f6e 7465  fn rebuild_conte
-000004e0: 7874 2863 6f6e 7465 7874 5f70 7472 3a20  xt(context_ptr: 
-000004f0: 635f 696e 7429 202d 3e20 5265 7375 6c74  c_int) -> Result
-00000500: 3c28 292c 2053 7472 696e 673e 207b 0a20  <(), String> {. 
-00000510: 2020 2075 6e73 6166 6520 7b0a 2020 2020     unsafe {.    
-00000520: 2020 2020 6c65 7420 6572 726f 7220 3d20      let error = 
-00000530: 5265 6275 696c 6443 6f6e 7465 7874 2863  RebuildContext(c
-00000540: 6f6e 7465 7874 5f70 7472 293b 0a20 2020  ontext_ptr);.   
-00000550: 2020 2020 2069 6620 6572 726f 722e 6973       if error.is
-00000560: 5f6e 756c 6c28 2920 7b0a 2020 2020 2020  _null() {.      
-00000570: 2020 2020 2020 4f6b 2828 2929 0a20 2020        Ok(()).   
-00000580: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
-00000590: 2020 2020 2020 2020 2020 6c65 7420 6572            let er
-000005a0: 726f 725f 7374 7220 3d20 4353 7472 696e  ror_str = CStrin
-000005b0: 673a 3a66 726f 6d5f 7261 7728 6572 726f  g::from_raw(erro
-000005c0: 7229 3b0a 2020 2020 2020 2020 2020 2020  r);.            
-000005d0: 6c65 7420 6572 726f 725f 7374 7269 6e67  let error_string
-000005e0: 203d 2065 7272 6f72 5f73 7472 0a20 2020   = error_str.   
-000005f0: 2020 2020 2020 2020 2020 2020 202e 696e               .in
-00000600: 746f 5f73 7472 696e 6728 290a 2020 2020  to_string().    
-00000610: 2020 2020 2020 2020 2020 2020 2e75 6e77              .unw
-00000620: 7261 705f 6f72 5f65 6c73 6528 7c5f 7c20  rap_or_else(|_| 
-00000630: 5374 7269 6e67 3a3a 6672 6f6d 2822 556e  String::from("Un
-00000640: 6b6e 6f77 6e20 6572 726f 7222 2929 3b0a  known error"));.
-00000650: 2020 2020 2020 2020 2020 2020 4572 7228              Err(
-00000660: 6572 726f 725f 7374 7269 6e67 290a 2020  error_string).  
-00000670: 2020 2020 2020 7d0a 2020 2020 7d0a 7d0a        }.    }.}.
-00000680: 0a70 7562 2066 6e20 7265 6275 696c 645f  .pub fn rebuild_
-00000690: 636f 6e74 6578 7473 2869 6473 3a20 5665  contexts(ids: Ve
-000006a0: 633c 635f 696e 743e 2920 2d3e 2052 6573  c<c_int>) -> Res
-000006b0: 756c 743c 2829 2c20 5665 633c 5374 7269  ult<(), Vec<Stri
-000006c0: 6e67 3e3e 207b 0a20 2020 2075 6e73 6166  ng>> {.    unsaf
-000006d0: 6520 7b0a 2020 2020 2020 2020 6c65 7420  e {.        let 
-000006e0: 7265 7375 6c74 203d 2052 6562 7569 6c64  result = Rebuild
-000006f0: 436f 6e74 6578 7473 2869 6473 2e61 735f  Contexts(ids.as_
-00000700: 7074 7228 2920 6173 202a 6d75 7420 6933  ptr() as *mut i3
-00000710: 322c 2069 6473 2e6c 656e 2829 2061 7320  2, ids.len() as 
-00000720: 635f 696e 7429 3b0a 2020 2020 2020 2020  c_int);.        
-00000730: 6c65 7420 6572 726f 7273 5f70 7472 203d  let errors_ptr =
-00000740: 2072 6573 756c 742e 7230 3b0a 2020 2020   result.r0;.    
-00000750: 2020 2020 6c65 7420 6572 726f 7273 5f63      let errors_c
-00000760: 6f75 6e74 203d 2072 6573 756c 742e 7231  ount = result.r1
-00000770: 3b0a 0a20 2020 2020 2020 2069 6620 6572  ;..        if er
-00000780: 726f 7273 5f63 6f75 6e74 203d 3d20 3020  rors_count == 0 
-00000790: 7b0a 2020 2020 2020 2020 2020 2020 4f6b  {.            Ok
-000007a0: 2828 2929 0a20 2020 2020 2020 207d 2065  (()).        } e
-000007b0: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
-000007c0: 2020 6c65 7420 6d75 7420 6572 726f 7273    let mut errors
-000007d0: 203d 2056 6563 3a3a 7769 7468 5f63 6170   = Vec::with_cap
-000007e0: 6163 6974 7928 6572 726f 7273 5f63 6f75  acity(errors_cou
-000007f0: 6e74 2061 7320 7573 697a 6529 3b0a 2020  nt as usize);.  
-00000800: 2020 2020 2020 2020 2020 6c65 7420 6572            let er
-00000810: 726f 7273 5f73 6c69 6365 203d 2073 7464  rors_slice = std
-00000820: 3a3a 736c 6963 653a 3a66 726f 6d5f 7261  ::slice::from_ra
-00000830: 775f 7061 7274 7328 6572 726f 7273 5f70  w_parts(errors_p
-00000840: 7472 2c20 6572 726f 7273 5f63 6f75 6e74  tr, errors_count
-00000850: 2061 7320 7573 697a 6529 3b0a 2020 2020   as usize);.    
-00000860: 2020 2020 2020 2020 666f 7220 2665 7272          for &err
-00000870: 6f72 2069 6e20 6572 726f 7273 5f73 6c69  or in errors_sli
-00000880: 6365 207b 0a20 2020 2020 2020 2020 2020  ce {.           
-00000890: 2020 2020 206c 6574 2065 7272 6f72 5f73       let error_s
-000008a0: 7472 203d 2043 5374 7269 6e67 3a3a 6672  tr = CString::fr
-000008b0: 6f6d 5f72 6177 2865 7272 6f72 293b 0a20  om_raw(error);. 
-000008c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000008d0: 6574 2065 7272 6f72 5f73 7472 696e 6720  et error_string 
-000008e0: 3d20 6572 726f 725f 7374 720a 2020 2020  = error_str.    
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2e69 6e74 6f5f 7374 7269 6e67 2829 0a20  .into_string(). 
-00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000920: 2020 202e 756e 7772 6170 5f6f 725f 656c     .unwrap_or_el
-00000930: 7365 287c 5f7c 2053 7472 696e 673a 3a66  se(|_| String::f
-00000940: 726f 6d28 2255 6e6b 6e6f 776e 2065 7272  rom("Unknown err
-00000950: 6f72 2229 293b 0a20 2020 2020 2020 2020  or"));.         
-00000960: 2020 2020 2020 2065 7272 6f72 732e 7075         errors.pu
-00000970: 7368 2865 7272 6f72 5f73 7472 696e 6729  sh(error_string)
-00000980: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
-00000990: 2020 2020 2020 2020 2020 2020 6672 6565              free
-000009a0: 2865 7272 6f72 735f 7074 7220 6173 202a  (errors_ptr as *
-000009b0: 6d75 7420 5f29 3b0a 2020 2020 2020 2020  mut _);.        
-000009c0: 2020 2020 4572 7228 6572 726f 7273 290a      Err(errors).
-000009d0: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-000009e0: 7d0a 0a70 7562 2066 6e20 7265 6d6f 7665  }..pub fn remove
-000009f0: 5f63 6f6e 7465 7874 2863 6f6e 7465 7874  _context(context
-00000a00: 5f70 7472 3a20 635f 696e 7429 207b 0a20  _ptr: c_int) {. 
-00000a10: 2020 2075 6e73 6166 6520 7b0a 2020 2020     unsafe {.    
-00000a20: 2020 2020 5265 6d6f 7665 436f 6e74 6578      RemoveContex
-00000a30: 7428 636f 6e74 6578 745f 7074 7229 3b0a  t(context_ptr);.
-00000a40: 2020 2020 7d0a 7d0a 0a23 5b63 6667 2874      }.}..#[cfg(t
-00000a50: 6573 7429 5d0a 6d6f 6420 7465 7374 7320  est)].mod tests 
-00000a60: 7b0a 2020 2020 7573 6520 7375 7065 723a  {.    use super:
-00000a70: 3a2a 3b0a 2020 2020 7573 6520 7374 643a  :*;.    use std:
-00000a80: 3a66 733b 0a20 2020 2075 7365 2074 656d  :fs;.    use tem
-00000a90: 7066 696c 653a 3a74 656d 7064 6972 3b0a  pfile::tempdir;.
-00000aa0: 0a20 2020 2023 5b74 6573 745d 0a20 2020  .    #[test].   
-00000ab0: 2066 6e20 7465 7374 5f62 7569 6c64 5f6a   fn test_build_j
-00000ac0: 7328 2920 7b0a 2020 2020 2020 2020 6c65  s() {.        le
-00000ad0: 7420 7465 6d70 5f64 6972 203d 2074 656d  t temp_dir = tem
-00000ae0: 7064 6972 2829 2e75 6e77 7261 7028 293b  pdir().unwrap();
-00000af0: 0a20 2020 2020 2020 206c 6574 206a 735f  .        let js_
-00000b00: 6669 6c65 5f70 6174 6820 3d20 7465 6d70  file_path = temp
-00000b10: 5f64 6972 2e70 6174 6828 292e 6a6f 696e  _dir.path().join
-00000b20: 2822 7373 722e 6a73 2229 3b0a 2020 2020  ("ssr.js");.    
-00000b30: 2020 2020 6c65 7420 6f75 7470 7574 5f66      let output_f
-00000b40: 696c 655f 7061 7468 203d 2074 656d 705f  ile_path = temp_
-00000b50: 6469 722e 7061 7468 2829 2e6a 6f69 6e28  dir.path().join(
-00000b60: 2273 7372 2e6a 732e 6f75 7422 293b 0a0a  "ssr.js.out");..
-00000b70: 2020 2020 2020 2020 2f2f 2057 7269 7465          // Write
-00000b80: 2061 2073 696d 706c 6520 6a61 7661 7363   a simple javasc
-00000b90: 7269 7074 2066 756e 6374 696f 6e20 746f  ript function to
-00000ba0: 2061 2066 696c 6520 696e 2061 2074 6d70   a file in a tmp
-00000bb0: 2064 6972 6563 746f 7279 0a20 2020 2020   directory.     
-00000bc0: 2020 206c 6574 2069 6e69 7469 616c 5f6a     let initial_j
-00000bd0: 7320 3d20 7223 2322 6578 706f 7274 2063  s = r##"export c
-00000be0: 6f6e 7374 2049 6e64 6578 203d 2028 2920  onst Index = () 
-00000bf0: 3d3e 2022 3c49 4e49 5449 414c 3e22 3b22  => "<INITIAL>";"
-00000c00: 2323 3b0a 2020 2020 2020 2020 6673 3a3a  ##;.        fs::
-00000c10: 7772 6974 6528 266a 735f 6669 6c65 5f70  write(&js_file_p
-00000c20: 6174 682c 2069 6e69 7469 616c 5f6a 7329  ath, initial_js)
-00000c30: 2e75 6e77 7261 7028 293b 0a0a 2020 2020  .unwrap();..    
-00000c40: 2020 2020 6c65 7420 636f 6e74 6578 745f      let context_
-00000c50: 6964 203d 0a20 2020 2020 2020 2020 2020  id =.           
-00000c60: 2067 6574 5f62 7569 6c64 5f63 6f6e 7465   get_build_conte
-00000c70: 7874 2826 6a73 5f66 696c 655f 7061 7468  xt(&js_file_path
-00000c80: 2e74 6f5f 7374 7228 292e 756e 7772 6170  .to_str().unwrap
-00000c90: 2829 2c20 2222 2c20 2264 6576 656c 6f70  (), "", "develop
-00000ca0: 6d65 6e74 222c 2030 2c20 7472 7565 292e  ment", 0, true).
-00000cb0: 756e 7772 6170 2829 3b0a 2020 2020 2020  unwrap();.      
-00000cc0: 2020 6173 7365 7274 5f6e 6521 2863 6f6e    assert_ne!(con
-00000cd0: 7465 7874 5f69 642c 2030 293b 0a0a 2020  text_id, 0);..  
-00000ce0: 2020 2020 2020 7265 6275 696c 645f 636f        rebuild_co
-00000cf0: 6e74 6578 7428 636f 6e74 6578 745f 6964  ntext(context_id
-00000d00: 292e 756e 7772 6170 2829 3b0a 2020 2020  ).unwrap();.    
-00000d10: 2020 2020 6173 7365 7274 2128 6f75 7470      assert!(outp
-00000d20: 7574 5f66 696c 655f 7061 7468 2e65 7869  ut_file_path.exi
-00000d30: 7374 7328 2929 3b0a 0a20 2020 2020 2020  sts());..       
-00000d40: 202f 2f20 4765 7420 7468 6520 6f75 7470   // Get the outp
-00000d50: 7574 2066 696c 6520 636f 6e74 656e 7473  ut file contents
-00000d60: 2061 6e64 2063 6865 636b 2074 6861 7420   and check that 
-00000d70: 3c68 746d 6c3e 2069 7320 696e 2074 6865  <html> is in the
-00000d80: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00000d90: 6c65 7420 6f75 7470 7574 203d 2066 733a  let output = fs:
-00000da0: 3a72 6561 645f 746f 5f73 7472 696e 6728  :read_to_string(
-00000db0: 266f 7574 7075 745f 6669 6c65 5f70 6174  &output_file_pat
-00000dc0: 6829 2e75 6e77 7261 7028 293b 0a20 2020  h).unwrap();.   
-00000dd0: 2020 2020 2070 7269 6e74 6c6e 2128 224f       println!("O
-00000de0: 7574 7075 7420 313a 207b 7d22 2c20 6f75  utput 1: {}", ou
-00000df0: 7470 7574 293b 0a20 2020 2020 2020 2061  tput);.        a
-00000e00: 7373 6572 7421 280a 2020 2020 2020 2020  ssert!(.        
-00000e10: 2020 2020 6f75 7470 7574 2e63 6f6e 7461      output.conta
-00000e20: 696e 7328 223c 494e 4954 4941 4c3e 2229  ins("<INITIAL>")
-00000e30: 2c0a 2020 2020 2020 2020 2020 2020 224f  ,.            "O
-00000e40: 7574 7075 7420 646f 6573 206e 6f74 2063  utput does not c
-00000e50: 6f6e 7461 696e 2065 7870 6563 7465 6420  ontain expected 
-00000e60: 3c49 4e49 5449 414c 3e20 7461 6722 0a20  <INITIAL> tag". 
-00000e70: 2020 2020 2020 2029 3b0a 0a20 2020 2020         );..     
-00000e80: 2020 202f 2f20 5570 6461 7465 2074 6865     // Update the
-00000e90: 2066 696c 650a 2020 2020 2020 2020 6c65   file.        le
-00000ea0: 7420 7570 6461 7465 645f 6a73 203d 2072  t updated_js = r
-00000eb0: 2323 2265 7870 6f72 7420 636f 6e73 7420  ##"export const 
-00000ec0: 496e 6465 7820 3d20 2829 203d 3e20 223c  Index = () => "<
-00000ed0: 5550 4441 5445 443e 223b 2223 233b 0a20  UPDATED>";"##;. 
-00000ee0: 2020 2020 2020 2066 733a 3a77 7269 7465         fs::write
-00000ef0: 2826 6a73 5f66 696c 655f 7061 7468 2c20  (&js_file_path, 
-00000f00: 7570 6461 7465 645f 6a73 292e 756e 7772  updated_js).unwr
-00000f10: 6170 2829 3b0a 0a20 2020 2020 2020 2072  ap();..        r
-00000f20: 6562 7569 6c64 5f63 6f6e 7465 7874 2863  ebuild_context(c
-00000f30: 6f6e 7465 7874 5f69 6429 2e75 6e77 7261  ontext_id).unwra
-00000f40: 7028 293b 0a0a 2020 2020 2020 2020 2f2f  p();..        //
-00000f50: 2043 6865 636b 2074 6861 7420 3c64 6976   Check that <div
-00000f60: 3e20 6973 2069 6e20 7468 6520 7570 6461  > is in the upda
-00000f70: 7465 6420 6f75 7470 7574 0a20 2020 2020  ted output.     
-00000f80: 2020 206c 6574 2075 7064 6174 6564 5f6f     let updated_o
-00000f90: 7574 7075 7420 3d20 6673 3a3a 7265 6164  utput = fs::read
-00000fa0: 5f74 6f5f 7374 7269 6e67 2826 6f75 7470  _to_string(&outp
-00000fb0: 7574 5f66 696c 655f 7061 7468 292e 756e  ut_file_path).un
-00000fc0: 7772 6170 2829 3b0a 2020 2020 2020 2020  wrap();.        
-00000fd0: 7072 696e 746c 6e21 2822 4f75 7470 7574  println!("Output
-00000fe0: 2032 3a20 7b7d 222c 206f 7574 7075 7429   2: {}", output)
-00000ff0: 3b0a 2020 2020 2020 2020 6173 7365 7274  ;.        assert
-00001000: 2128 0a20 2020 2020 2020 2020 2020 2075  !(.            u
-00001010: 7064 6174 6564 5f6f 7574 7075 742e 636f  pdated_output.co
-00001020: 6e74 6169 6e73 2822 3c55 5044 4154 4544  ntains("<UPDATED
-00001030: 3e22 292c 0a20 2020 2020 2020 2020 2020  >"),.           
-00001040: 2022 5570 6461 7465 6420 6f75 7470 7574   "Updated output
-00001050: 2064 6f65 7320 6e6f 7420 636f 6e74 6169   does not contai
-00001060: 6e20 6578 7065 6374 6564 203c 5550 4441  n expected <UPDA
-00001070: 5445 443e 2074 6167 220a 2020 2020 2020  TED> tag".      
-00001080: 2020 293b 0a20 2020 207d 0a0a 2020 2020    );.    }..    
-00001090: 235b 7465 7374 5d0a 2020 2020 666e 2074  #[test].    fn t
-000010a0: 6573 745f 7265 6275 696c 645f 636f 6e74  est_rebuild_cont
-000010b0: 6578 7473 2829 207b 0a20 2020 2020 2020  exts() {.       
-000010c0: 206c 6574 2074 656d 705f 6469 7220 3d20   let temp_dir = 
-000010d0: 7465 6d70 6469 7228 292e 756e 7772 6170  tempdir().unwrap
-000010e0: 2829 3b0a 2020 2020 2020 2020 6c65 7420  ();.        let 
-000010f0: 6a73 5f66 696c 655f 7061 7468 203d 2074  js_file_path = t
-00001100: 656d 705f 6469 722e 7061 7468 2829 2e6a  emp_dir.path().j
-00001110: 6f69 6e28 2273 7372 2e6a 7322 293b 0a20  oin("ssr.js");. 
-00001120: 2020 2020 2020 206c 6574 206f 7574 7075         let outpu
-00001130: 745f 6669 6c65 5f70 6174 6820 3d20 7465  t_file_path = te
-00001140: 6d70 5f64 6972 2e70 6174 6828 292e 6a6f  mp_dir.path().jo
-00001150: 696e 2822 7373 722e 6a73 2e6f 7574 2229  in("ssr.js.out")
-00001160: 3b0a 0a20 2020 2020 2020 202f 2f20 5772  ;..        // Wr
-00001170: 6974 6520 6120 7369 6d70 6c65 206a 6176  ite a simple jav
-00001180: 6173 6372 6970 7420 6675 6e63 7469 6f6e  ascript function
-00001190: 2074 6f20 6120 6669 6c65 2069 6e20 6120   to a file in a 
-000011a0: 746d 7020 6469 7265 6374 6f72 790a 2020  tmp directory.  
-000011b0: 2020 2020 2020 6c65 7420 696e 6974 6961        let initia
-000011c0: 6c5f 6a73 203d 2072 2323 2265 7870 6f72  l_js = r##"expor
-000011d0: 7420 636f 6e73 7420 496e 6465 7820 3d20  t const Index = 
-000011e0: 2829 203d 3e20 223c 494e 4954 4941 4c3e  () => "<INITIAL>
-000011f0: 223b 2223 233b 0a20 2020 2020 2020 2066  ";"##;.        f
-00001200: 733a 3a77 7269 7465 2826 6a73 5f66 696c  s::write(&js_fil
-00001210: 655f 7061 7468 2c20 696e 6974 6961 6c5f  e_path, initial_
-00001220: 6a73 292e 756e 7772 6170 2829 3b0a 0a20  js).unwrap();.. 
-00001230: 2020 2020 2020 206c 6574 2063 6f6e 7465         let conte
-00001240: 7874 5f69 6420 3d0a 2020 2020 2020 2020  xt_id =.        
-00001250: 2020 2020 6765 745f 6275 696c 645f 636f      get_build_co
-00001260: 6e74 6578 7428 266a 735f 6669 6c65 5f70  ntext(&js_file_p
-00001270: 6174 682e 746f 5f73 7472 2829 2e75 6e77  ath.to_str().unw
-00001280: 7261 7028 292c 2022 222c 2022 6465 7665  rap(), "", "deve
-00001290: 6c6f 706d 656e 7422 2c20 302c 2074 7275  lopment", 0, tru
-000012a0: 6529 2e75 6e77 7261 7028 293b 0a20 2020  e).unwrap();.   
-000012b0: 2020 2020 2061 7373 6572 745f 6e65 2128       assert_ne!(
-000012c0: 636f 6e74 6578 745f 6964 2c20 3029 3b0a  context_id, 0);.
-000012d0: 0a20 2020 2020 2020 2072 6562 7569 6c64  .        rebuild
-000012e0: 5f63 6f6e 7465 7874 7328 7665 6321 5b63  _contexts(vec![c
-000012f0: 6f6e 7465 7874 5f69 645d 292e 756e 7772  ontext_id]).unwr
-00001300: 6170 2829 3b0a 2020 2020 2020 2020 6173  ap();.        as
-00001310: 7365 7274 2128 6f75 7470 7574 5f66 696c  sert!(output_fil
-00001320: 655f 7061 7468 2e65 7869 7374 7328 2929  e_path.exists())
-00001330: 3b0a 2020 2020 7d0a 0a20 2020 2023 5b74  ;.    }..    #[t
-00001340: 6573 745d 0a20 2020 2066 6e20 7465 7374  est].    fn test
-00001350: 5f65 7863 6570 7469 6f6e 5f74 6872 6f77  _exception_throw
-00001360: 6e28 2920 7b0a 2020 2020 2020 2020 6c65  n() {.        le
-00001370: 7420 7465 6d70 5f64 6972 203d 2074 656d  t temp_dir = tem
-00001380: 7064 6972 2829 2e75 6e77 7261 7028 293b  pdir().unwrap();
-00001390: 0a20 2020 2020 2020 206c 6574 206a 735f  .        let js_
-000013a0: 6669 6c65 5f70 6174 6820 3d20 7465 6d70  file_path = temp
-000013b0: 5f64 6972 2e70 6174 6828 292e 6a6f 696e  _dir.path().join
-000013c0: 2822 7373 722e 6a73 2229 3b0a 2020 2020  ("ssr.js");.    
-000013d0: 2020 2020 6c65 7420 6f75 7470 7574 5f66      let output_f
-000013e0: 696c 655f 7061 7468 203d 2074 656d 705f  ile_path = temp_
-000013f0: 6469 722e 7061 7468 2829 2e6a 6f69 6e28  dir.path().join(
-00001400: 2273 7372 2e6a 732e 6f75 7422 293b 0a0a  "ssr.js.out");..
-00001410: 2020 2020 2020 2020 2f2f 2057 7269 7465          // Write
-00001420: 2061 2073 696d 706c 6520 6a61 7661 7363   a simple javasc
-00001430: 7269 7074 2066 756e 6374 696f 6e20 746f  ript function to
-00001440: 2061 2066 696c 6520 696e 2061 2074 6d70   a file in a tmp
-00001450: 2064 6972 6563 746f 7279 0a20 2020 2020   directory.     
-00001460: 2020 206c 6574 2069 6e69 7469 616c 5f6a     let initial_j
-00001470: 7320 3d20 7223 2322 6578 706f 7274 2063  s = r##"export c
-00001480: 6f6e 7374 2049 6e64 6578 2049 4e56 414c  onst Index INVAL
-00001490: 4944 2053 594e 5441 5820 2829 203d 3e20  ID SYNTAX () => 
-000014a0: 223c 494e 4954 4941 4c3e 223b 2223 233b  "<INITIAL>";"##;
-000014b0: 0a20 2020 2020 2020 2066 733a 3a77 7269  .        fs::wri
-000014c0: 7465 2826 6a73 5f66 696c 655f 7061 7468  te(&js_file_path
-000014d0: 2c20 696e 6974 6961 6c5f 6a73 292e 756e  , initial_js).un
-000014e0: 7772 6170 2829 3b0a 0a20 2020 2020 2020  wrap();..       
-000014f0: 206c 6574 2063 6f6e 7465 7874 5f69 6420   let context_id 
-00001500: 3d0a 2020 2020 2020 2020 2020 2020 6765  =.            ge
-00001510: 745f 6275 696c 645f 636f 6e74 6578 7428  t_build_context(
-00001520: 266a 735f 6669 6c65 5f70 6174 682e 746f  &js_file_path.to
-00001530: 5f73 7472 2829 2e75 6e77 7261 7028 292c  _str().unwrap(),
-00001540: 2022 222c 2022 6465 7665 6c6f 706d 656e   "", "developmen
-00001550: 7422 2c20 302c 2074 7275 6529 2e75 6e77  t", 0, true).unw
-00001560: 7261 7028 293b 0a20 2020 2020 2020 2061  rap();.        a
-00001570: 7373 6572 745f 6e65 2128 636f 6e74 6578  ssert_ne!(contex
-00001580: 745f 6964 2c20 3029 3b0a 0a20 2020 2020  t_id, 0);..     
-00001590: 2020 206c 6574 2072 6573 756c 7420 3d20     let result = 
-000015a0: 7265 6275 696c 645f 636f 6e74 6578 7428  rebuild_context(
-000015b0: 636f 6e74 6578 745f 6964 293b 0a20 2020  context_id);.   
-000015c0: 2020 2020 2061 7373 6572 7421 280a 2020       assert!(.  
-000015d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000015e0: 2e69 735f 6572 7228 292c 0a20 2020 2020  .is_err(),.     
-000015f0: 2020 2020 2020 2022 4578 7065 6374 6564         "Expected
-00001600: 2061 6e20 6572 726f 7220 6475 7269 6e67   an error during
-00001610: 2072 6562 7569 6c64 5f63 6f6e 7465 7874   rebuild_context
-00001620: 2c20 6275 7420 6e6f 6e65 206f 6363 7572  , but none occur
-00001630: 7265 642e 220a 2020 2020 2020 2020 293b  red.".        );
-00001640: 0a20 2020 2020 2020 2061 7373 6572 7421  .        assert!
-00001650: 2821 6f75 7470 7574 5f66 696c 655f 7061  (!output_file_pa
-00001660: 7468 2e65 7869 7374 7328 2929 3b0a 2020  th.exists());.  
-00001670: 2020 7d0a 7d0a                             }.}.
+000000a0: 6962 633b 0a0a 7573 6520 7374 643a 3a66  ibc;..use std::f
+000000b0: 6669 3a3a 7b63 5f69 6e74 2c20 4353 7472  fi::{c_int, CStr
+000000c0: 696e 677d 3b0a 7573 6520 7374 643a 3a73  ing};.use std::s
+000000d0: 796e 633a 3a7b 6d70 7363 2c20 4172 637d  ync::{mpsc, Arc}
+000000e0: 3b0a 7573 6520 7374 643a 3a74 6872 6561  ;.use std::threa
+000000f0: 643b 0a0a 7075 6220 666e 2067 6574 5f62  d;..pub fn get_b
+00000100: 7569 6c64 5f63 6f6e 7465 7874 280a 2020  uild_context(.  
+00000110: 2020 6669 6c65 6e61 6d65 3a20 2673 7472    filename: &str
+00000120: 2c0a 2020 2020 6e6f 6465 5f6d 6f64 756c  ,.    node_modul
+00000130: 6573 5f70 6174 683a 2026 7374 722c 0a20  es_path: &str,. 
+00000140: 2020 2065 6e76 6972 6f6e 6d65 6e74 3a20     environment: 
+00000150: 2673 7472 2c0a 2020 2020 6c69 7665 5f72  &str,.    live_r
+00000160: 656c 6f61 645f 706f 7274 3a20 6933 322c  eload_port: i32,
+00000170: 0a20 2020 2069 735f 7365 7276 6572 3a20  .    is_server: 
+00000180: 626f 6f6c 2c0a 2920 2d3e 2052 6573 756c  bool,.) -> Resul
+00000190: 743c 635f 696e 742c 2053 7472 696e 673e  t<c_int, String>
+000001a0: 207b 0a20 2020 206c 6574 2063 5f66 696c   {.    let c_fil
+000001b0: 656e 616d 6520 3d20 4353 7472 696e 673a  ename = CString:
+000001c0: 3a6e 6577 2866 696c 656e 616d 6529 2e75  :new(filename).u
+000001d0: 6e77 7261 7028 293b 0a20 2020 206c 6574  nwrap();.    let
+000001e0: 2063 5f6e 6f64 655f 6d6f 6475 6c65 735f   c_node_modules_
+000001f0: 7061 7468 203d 2043 5374 7269 6e67 3a3a  path = CString::
+00000200: 6e65 7728 6e6f 6465 5f6d 6f64 756c 6573  new(node_modules
+00000210: 5f70 6174 6829 2e75 6e77 7261 7028 293b  _path).unwrap();
+00000220: 0a20 2020 206c 6574 2063 5f65 6e76 6972  .    let c_envir
+00000230: 6f6e 6d65 6e74 203d 2043 5374 7269 6e67  onment = CString
+00000240: 3a3a 6e65 7728 656e 7669 726f 6e6d 656e  ::new(environmen
+00000250: 7429 2e75 6e77 7261 7028 293b 0a20 2020  t).unwrap();.   
+00000260: 206c 6574 2069 735f 7365 7276 6572 203d   let is_server =
+00000270: 2069 6620 6973 5f73 6572 7665 7220 7b20   if is_server { 
+00000280: 3120 7d20 656c 7365 207b 2030 207d 3b0a  1 } else { 0 };.
+00000290: 0a20 2020 2075 6e73 6166 6520 7b0a 2020  .    unsafe {.  
+000002a0: 2020 2020 2020 6c65 7420 7265 7375 6c74        let result
+000002b0: 203d 2047 6574 4275 696c 6443 6f6e 7465   = GetBuildConte
+000002c0: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
+000002d0: 635f 6669 6c65 6e61 6d65 2e69 6e74 6f5f  c_filename.into_
+000002e0: 7261 7728 292c 0a20 2020 2020 2020 2020  raw(),.         
+000002f0: 2020 2063 5f6e 6f64 655f 6d6f 6475 6c65     c_node_module
+00000300: 735f 7061 7468 2e69 6e74 6f5f 7261 7728  s_path.into_raw(
+00000310: 292c 0a20 2020 2020 2020 2020 2020 2063  ),.            c
+00000320: 5f65 6e76 6972 6f6e 6d65 6e74 2e69 6e74  _environment.int
+00000330: 6f5f 7261 7728 292c 0a20 2020 2020 2020  o_raw(),.       
+00000340: 2020 2020 206c 6976 655f 7265 6c6f 6164       live_reload
+00000350: 5f70 6f72 742c 0a20 2020 2020 2020 2020  _port,.         
+00000360: 2020 2069 735f 7365 7276 6572 2c0a 2020     is_server,.  
+00000370: 2020 2020 2020 293b 0a20 2020 2020 2020        );.       
+00000380: 206c 6574 2069 6420 3d20 7265 7375 6c74   let id = result
+00000390: 2e72 303b 0a20 2020 2020 2020 206c 6574  .r0;.        let
+000003a0: 2065 7272 6f72 203d 2072 6573 756c 742e   error = result.
+000003b0: 7231 3b0a 0a20 2020 2020 2020 2069 6620  r1;..        if 
+000003c0: 6572 726f 722e 6973 5f6e 756c 6c28 2920  error.is_null() 
+000003d0: 7b0a 2020 2020 2020 2020 2020 2020 4f6b  {.            Ok
+000003e0: 2869 6429 0a20 2020 2020 2020 207d 2065  (id).        } e
+000003f0: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
+00000400: 2020 6c65 7420 6572 726f 725f 7374 7220    let error_str 
+00000410: 3d20 4353 7472 696e 673a 3a66 726f 6d5f  = CString::from_
+00000420: 7261 7728 6572 726f 7229 3b0a 2020 2020  raw(error);.    
+00000430: 2020 2020 2020 2020 6c65 7420 6572 726f          let erro
+00000440: 725f 7374 7269 6e67 203d 2065 7272 6f72  r_string = error
+00000450: 5f73 7472 0a20 2020 2020 2020 2020 2020  _str.           
+00000460: 2020 2020 202e 696e 746f 5f73 7472 696e       .into_strin
+00000470: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00000480: 2020 2020 2e75 6e77 7261 705f 6f72 5f65      .unwrap_or_e
+00000490: 6c73 6528 7c5f 7c20 5374 7269 6e67 3a3a  lse(|_| String::
+000004a0: 6672 6f6d 2822 556e 6b6e 6f77 6e20 6572  from("Unknown er
+000004b0: 726f 7222 2929 3b0a 2020 2020 2020 2020  ror"));.        
+000004c0: 2020 2020 4572 7228 6572 726f 725f 7374      Err(error_st
+000004d0: 7269 6e67 290a 2020 2020 2020 2020 7d0a  ring).        }.
+000004e0: 2020 2020 7d0a 7d0a 0a70 7562 2066 6e20      }.}..pub fn 
+000004f0: 7265 6275 696c 645f 636f 6e74 6578 7428  rebuild_context(
+00000500: 636f 6e74 6578 745f 7074 723a 2063 5f69  context_ptr: c_i
+00000510: 6e74 2920 2d3e 2052 6573 756c 743c 2829  nt) -> Result<()
+00000520: 2c20 5374 7269 6e67 3e20 7b0a 2020 2020  , String> {.    
+00000530: 756e 7361 6665 207b 0a20 2020 2020 2020  unsafe {.       
+00000540: 206c 6574 2065 7272 6f72 203d 2052 6562   let error = Reb
+00000550: 7569 6c64 436f 6e74 6578 7428 636f 6e74  uildContext(cont
+00000560: 6578 745f 7074 7229 3b0a 2020 2020 2020  ext_ptr);.      
+00000570: 2020 6966 2065 7272 6f72 2e69 735f 6e75    if error.is_nu
+00000580: 6c6c 2829 207b 0a20 2020 2020 2020 2020  ll() {.         
+00000590: 2020 204f 6b28 2829 290a 2020 2020 2020     Ok(()).      
+000005a0: 2020 7d20 656c 7365 207b 0a20 2020 2020    } else {.     
+000005b0: 2020 2020 2020 206c 6574 2065 7272 6f72         let error
+000005c0: 5f73 7472 203d 2043 5374 7269 6e67 3a3a  _str = CString::
+000005d0: 6672 6f6d 5f72 6177 2865 7272 6f72 293b  from_raw(error);
+000005e0: 0a20 2020 2020 2020 2020 2020 206c 6574  .            let
+000005f0: 2065 7272 6f72 5f73 7472 696e 6720 3d20   error_string = 
+00000600: 6572 726f 725f 7374 720a 2020 2020 2020  error_str.      
+00000610: 2020 2020 2020 2020 2020 2e69 6e74 6f5f            .into_
+00000620: 7374 7269 6e67 2829 0a20 2020 2020 2020  string().       
+00000630: 2020 2020 2020 2020 202e 756e 7772 6170           .unwrap
+00000640: 5f6f 725f 656c 7365 287c 5f7c 2053 7472  _or_else(|_| Str
+00000650: 696e 673a 3a66 726f 6d28 2255 6e6b 6e6f  ing::from("Unkno
+00000660: 776e 2065 7272 6f72 2229 293b 0a20 2020  wn error"));.   
+00000670: 2020 2020 2020 2020 2045 7272 2865 7272           Err(err
+00000680: 6f72 5f73 7472 696e 6729 0a20 2020 2020  or_string).     
+00000690: 2020 207d 0a20 2020 207d 0a7d 0a0a 7479     }.    }.}..ty
+000006a0: 7065 2043 616c 6c62 6163 6b20 3d20 6479  pe Callback = dy
+000006b0: 6e20 466e 2863 5f69 6e74 2920 2b20 5365  n Fn(c_int) + Se
+000006c0: 6e64 202b 2053 796e 633b 0a0a 7075 6220  nd + Sync;..pub 
+000006d0: 666e 2072 6562 7569 6c64 5f63 6f6e 7465  fn rebuild_conte
+000006e0: 7874 7328 6964 733a 2056 6563 3c63 5f69  xts(ids: Vec<c_i
+000006f0: 6e74 3e2c 2063 616c 6c62 6163 6b3a 2041  nt>, callback: A
+00000700: 7263 3c42 6f78 3c43 616c 6c62 6163 6b3e  rc<Box<Callback>
+00000710: 3e29 202d 3e20 5265 7375 6c74 3c28 292c  >) -> Result<(),
+00000720: 2056 6563 3c53 7472 696e 673e 3e20 7b0a   Vec<String>> {.
+00000730: 2020 2020 6c65 7420 2874 782c 2072 7829      let (tx, rx)
+00000740: 203d 206d 7073 633a 3a63 6861 6e6e 656c   = mpsc::channel
+00000750: 2829 3b0a 2020 2020 6c65 7420 6d75 7420  ();.    let mut 
+00000760: 6861 6e64 6c65 7320 3d20 5665 633a 3a6e  handles = Vec::n
+00000770: 6577 2829 3b0a 0a20 2020 2066 6f72 2069  ew();..    for i
+00000780: 6420 696e 2069 6473 2e63 6c6f 6e65 2829  d in ids.clone()
+00000790: 2e69 6e74 6f5f 6974 6572 2829 207b 0a20  .into_iter() {. 
+000007a0: 2020 2020 2020 206c 6574 2074 7820 3d20         let tx = 
+000007b0: 7478 2e63 6c6f 6e65 2829 3b0a 0a20 2020  tx.clone();..   
+000007c0: 2020 2020 206c 6574 2068 616e 646c 6520       let handle 
+000007d0: 3d20 7468 7265 6164 3a3a 7370 6177 6e28  = thread::spawn(
+000007e0: 6d6f 7665 207c 7c20 7b0a 2020 2020 2020  move || {.      
+000007f0: 2020 2020 2020 756e 7361 6665 207b 0a20        unsafe {. 
+00000800: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000810: 6574 2065 7272 6f72 5f70 7472 203d 2052  et error_ptr = R
+00000820: 6562 7569 6c64 436f 6e74 6578 7428 6964  ebuildContext(id
+00000830: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00000840: 2020 206c 6574 2072 6573 756c 7420 3d20     let result = 
+00000850: 6966 2021 6572 726f 725f 7074 722e 6973  if !error_ptr.is
+00000860: 5f6e 756c 6c28 2920 7b0a 2020 2020 2020  _null() {.      
+00000870: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00000880: 7420 6572 726f 725f 6373 7472 203d 2043  t error_cstr = C
+00000890: 5374 7269 6e67 3a3a 6672 6f6d 5f72 6177  String::from_raw
+000008a0: 2865 7272 6f72 5f70 7472 293b 0a20 2020  (error_ptr);.   
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 206c 6574 2065 7272 6f72 5f73 7472 696e   let error_strin
+000008d0: 6720 3d20 6572 726f 725f 6373 7472 0a20  g = error_cstr. 
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 2020 202e 696e 746f 5f73 7472         .into_str
+00000900: 696e 6728 290a 2020 2020 2020 2020 2020  ing().          
+00000910: 2020 2020 2020 2020 2020 2020 2020 2e75                .u
+00000920: 6e77 7261 705f 6f72 5f65 6c73 6528 7c5f  nwrap_or_else(|_
+00000930: 7c20 5374 7269 6e67 3a3a 6672 6f6d 2822  | String::from("
+00000940: 556e 6b6e 6f77 6e20 6572 726f 7222 2929  Unknown error"))
+00000950: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00000960: 2020 2020 2020 536f 6d65 2865 7272 6f72        Some(error
+00000970: 5f73 7472 696e 6729 0a20 2020 2020 2020  _string).       
+00000980: 2020 2020 2020 2020 207d 2065 6c73 6520           } else 
+00000990: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000009a0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
+000009b0: 2020 2020 2020 2020 2020 207d 3b0a 0a20             };.. 
+000009c0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+000009d0: 2f20 5365 6e64 2062 6f74 6820 7468 6520  / Send both the 
+000009e0: 4944 2061 6e64 2072 6573 756c 7420 746f  ID and result to
+000009f0: 2074 6865 206d 6169 6e20 7468 7265 6164   the main thread
+00000a00: 2076 6961 2063 6861 6e6e 656c 0a20 2020   via channel.   
+00000a10: 2020 2020 2020 2020 2020 2020 2074 782e               tx.
+00000a20: 7365 6e64 2828 6964 2c20 7265 7375 6c74  send((id, result
+00000a30: 2e63 6c6f 6e65 2829 2929 2e75 6e77 7261  .clone())).unwra
+00000a40: 7028 293b 0a20 2020 2020 2020 2020 2020  p();.           
+00000a50: 207d 0a20 2020 2020 2020 207d 293b 0a20   }.        });. 
+00000a60: 2020 2020 2020 2068 616e 646c 6573 2e70         handles.p
+00000a70: 7573 6828 6861 6e64 6c65 293b 0a20 2020  ush(handle);.   
+00000a80: 207d 0a0a 2020 2020 2f2f 2043 6c65 616e   }..    // Clean
+00000a90: 7570 2068 616e 646c 6573 2061 6e64 2063  up handles and c
+00000aa0: 6f6c 6c65 6374 2065 7272 6f72 730a 2020  ollect errors.  
+00000ab0: 2020 6c65 7420 6d75 7420 6572 726f 7273    let mut errors
+00000ac0: 203d 2056 6563 3a3a 6e65 7728 293b 0a0a   = Vec::new();..
+00000ad0: 2020 2020 2f2f 2043 6f6c 6c65 6374 2072      // Collect r
+00000ae0: 6573 756c 7473 2069 6e20 7468 6520 6f72  esults in the or
+00000af0: 6465 7220 7468 6579 2061 7265 2063 6f6d  der they are com
+00000b00: 706c 6574 6564 0a20 2020 2066 6f72 205f  pleted.    for _
+00000b10: 2069 6e20 302e 2e69 6473 2e6c 656e 2829   in 0..ids.len()
+00000b20: 207b 0a20 2020 2020 2020 2069 6620 6c65   {.        if le
+00000b30: 7420 4f6b 2828 6964 2c20 6572 7229 2920  t Ok((id, err)) 
+00000b40: 3d20 7278 2e72 6563 7628 2920 7b0a 2020  = rx.recv() {.  
+00000b50: 2020 2020 2020 2020 2020 6966 206c 6574            if let
+00000b60: 2053 6f6d 6528 6572 726f 7229 203d 2065   Some(error) = e
+00000b70: 7272 207b 0a20 2020 2020 2020 2020 2020  rr {.           
+00000b80: 2020 2020 2065 7272 6f72 732e 7075 7368       errors.push
+00000b90: 2865 7272 6f72 293b 0a20 2020 2020 2020  (error);.       
+00000ba0: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2f2f                //
+00000bc0: 2043 616c 6c20 7468 6520 6361 6c6c 6261   Call the callba
+00000bd0: 636b 2077 6974 6820 7468 6520 4944 0a20  ck with the ID. 
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000bf0: 616c 6c62 6163 6b28 6964 293b 0a20 2020  allback(id);.   
+00000c00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000c10: 2020 207d 0a20 2020 207d 0a0a 2020 2020     }.    }..    
+00000c20: 2f2f 2043 6c6f 7365 206f 7574 2074 6865  // Close out the
+00000c30: 2077 6f72 6b65 7273 0a20 2020 2066 6f72   workers.    for
+00000c40: 2068 616e 646c 6520 696e 2068 616e 646c   handle in handl
+00000c50: 6573 207b 0a20 2020 2020 2020 2068 616e  es {.        han
+00000c60: 646c 652e 6a6f 696e 2829 2e75 6e77 7261  dle.join().unwra
+00000c70: 7028 293b 0a20 2020 207d 0a0a 2020 2020  p();.    }..    
+00000c80: 6966 2065 7272 6f72 732e 6973 5f65 6d70  if errors.is_emp
+00000c90: 7479 2829 207b 0a20 2020 2020 2020 204f  ty() {.        O
+00000ca0: 6b28 2829 290a 2020 2020 7d20 656c 7365  k(()).    } else
+00000cb0: 207b 0a20 2020 2020 2020 2045 7272 2865   {.        Err(e
+00000cc0: 7272 6f72 7329 0a20 2020 207d 0a7d 0a0a  rrors).    }.}..
+00000cd0: 7075 6220 666e 2072 656d 6f76 655f 636f  pub fn remove_co
+00000ce0: 6e74 6578 7428 636f 6e74 6578 745f 7074  ntext(context_pt
+00000cf0: 723a 2063 5f69 6e74 2920 7b0a 2020 2020  r: c_int) {.    
+00000d00: 756e 7361 6665 207b 0a20 2020 2020 2020  unsafe {.       
+00000d10: 2052 656d 6f76 6543 6f6e 7465 7874 2863   RemoveContext(c
+00000d20: 6f6e 7465 7874 5f70 7472 293b 0a20 2020  ontext_ptr);.   
+00000d30: 207d 0a7d 0a0a 235b 6366 6728 7465 7374   }.}..#[cfg(test
+00000d40: 295d 0a6d 6f64 2074 6573 7473 207b 0a20  )].mod tests {. 
+00000d50: 2020 2075 7365 2073 7570 6572 3a3a 2a3b     use super::*;
+00000d60: 0a20 2020 2075 7365 2073 7464 3a3a 6673  .    use std::fs
+00000d70: 3b0a 2020 2020 7573 6520 7465 6d70 6669  ;.    use tempfi
+00000d80: 6c65 3a3a 7465 6d70 6469 723b 0a0a 2020  le::tempdir;..  
+00000d90: 2020 235b 7465 7374 5d0a 2020 2020 666e    #[test].    fn
+00000da0: 2074 6573 745f 6275 696c 645f 6a73 2829   test_build_js()
+00000db0: 207b 0a20 2020 2020 2020 206c 6574 2074   {.        let t
+00000dc0: 656d 705f 6469 7220 3d20 7465 6d70 6469  emp_dir = tempdi
+00000dd0: 7228 292e 756e 7772 6170 2829 3b0a 2020  r().unwrap();.  
+00000de0: 2020 2020 2020 6c65 7420 6a73 5f66 696c        let js_fil
+00000df0: 655f 7061 7468 203d 2074 656d 705f 6469  e_path = temp_di
+00000e00: 722e 7061 7468 2829 2e6a 6f69 6e28 2273  r.path().join("s
+00000e10: 7372 2e6a 7322 293b 0a20 2020 2020 2020  sr.js");.       
+00000e20: 206c 6574 206f 7574 7075 745f 6669 6c65   let output_file
+00000e30: 5f70 6174 6820 3d20 7465 6d70 5f64 6972  _path = temp_dir
+00000e40: 2e70 6174 6828 292e 6a6f 696e 2822 7373  .path().join("ss
+00000e50: 722e 6a73 2e6f 7574 2229 3b0a 0a20 2020  r.js.out");..   
+00000e60: 2020 2020 202f 2f20 5772 6974 6520 6120       // Write a 
+00000e70: 7369 6d70 6c65 206a 6176 6173 6372 6970  simple javascrip
+00000e80: 7420 6675 6e63 7469 6f6e 2074 6f20 6120  t function to a 
+00000e90: 6669 6c65 2069 6e20 6120 746d 7020 6469  file in a tmp di
+00000ea0: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+00000eb0: 6c65 7420 696e 6974 6961 6c5f 6a73 203d  let initial_js =
+00000ec0: 2072 2323 2265 7870 6f72 7420 636f 6e73   r##"export cons
+00000ed0: 7420 496e 6465 7820 3d20 2829 203d 3e20  t Index = () => 
+00000ee0: 223c 494e 4954 4941 4c3e 223b 2223 233b  "<INITIAL>";"##;
+00000ef0: 0a20 2020 2020 2020 2066 733a 3a77 7269  .        fs::wri
+00000f00: 7465 2826 6a73 5f66 696c 655f 7061 7468  te(&js_file_path
+00000f10: 2c20 696e 6974 6961 6c5f 6a73 292e 756e  , initial_js).un
+00000f20: 7772 6170 2829 3b0a 0a20 2020 2020 2020  wrap();..       
+00000f30: 206c 6574 2063 6f6e 7465 7874 5f69 6420   let context_id 
+00000f40: 3d0a 2020 2020 2020 2020 2020 2020 6765  =.            ge
+00000f50: 745f 6275 696c 645f 636f 6e74 6578 7428  t_build_context(
+00000f60: 266a 735f 6669 6c65 5f70 6174 682e 746f  &js_file_path.to
+00000f70: 5f73 7472 2829 2e75 6e77 7261 7028 292c  _str().unwrap(),
+00000f80: 2022 222c 2022 6465 7665 6c6f 706d 656e   "", "developmen
+00000f90: 7422 2c20 302c 2074 7275 6529 2e75 6e77  t", 0, true).unw
+00000fa0: 7261 7028 293b 0a20 2020 2020 2020 2061  rap();.        a
+00000fb0: 7373 6572 745f 6e65 2128 636f 6e74 6578  ssert_ne!(contex
+00000fc0: 745f 6964 2c20 3029 3b0a 0a20 2020 2020  t_id, 0);..     
+00000fd0: 2020 2072 6562 7569 6c64 5f63 6f6e 7465     rebuild_conte
+00000fe0: 7874 2863 6f6e 7465 7874 5f69 6429 2e75  xt(context_id).u
+00000ff0: 6e77 7261 7028 293b 0a20 2020 2020 2020  nwrap();.       
+00001000: 2061 7373 6572 7421 286f 7574 7075 745f   assert!(output_
+00001010: 6669 6c65 5f70 6174 682e 6578 6973 7473  file_path.exists
+00001020: 2829 293b 0a0a 2020 2020 2020 2020 2f2f  ());..        //
+00001030: 2047 6574 2074 6865 206f 7574 7075 7420   Get the output 
+00001040: 6669 6c65 2063 6f6e 7465 6e74 7320 616e  file contents an
+00001050: 6420 6368 6563 6b20 7468 6174 203c 6874  d check that <ht
+00001060: 6d6c 3e20 6973 2069 6e20 7468 6520 6f75  ml> is in the ou
+00001070: 7470 7574 0a20 2020 2020 2020 206c 6574  tput.        let
+00001080: 206f 7574 7075 7420 3d20 6673 3a3a 7265   output = fs::re
+00001090: 6164 5f74 6f5f 7374 7269 6e67 2826 6f75  ad_to_string(&ou
+000010a0: 7470 7574 5f66 696c 655f 7061 7468 292e  tput_file_path).
+000010b0: 756e 7772 6170 2829 3b0a 2020 2020 2020  unwrap();.      
+000010c0: 2020 7072 696e 746c 6e21 2822 4f75 7470    println!("Outp
+000010d0: 7574 2031 3a20 7b7d 222c 206f 7574 7075  ut 1: {}", outpu
+000010e0: 7429 3b0a 2020 2020 2020 2020 6173 7365  t);.        asse
+000010f0: 7274 2128 0a20 2020 2020 2020 2020 2020  rt!(.           
+00001100: 206f 7574 7075 742e 636f 6e74 6169 6e73   output.contains
+00001110: 2822 3c49 4e49 5449 414c 3e22 292c 0a20  ("<INITIAL>"),. 
+00001120: 2020 2020 2020 2020 2020 2022 4f75 7470             "Outp
+00001130: 7574 2064 6f65 7320 6e6f 7420 636f 6e74  ut does not cont
+00001140: 6169 6e20 6578 7065 6374 6564 203c 494e  ain expected <IN
+00001150: 4954 4941 4c3e 2074 6167 220a 2020 2020  ITIAL> tag".    
+00001160: 2020 2020 293b 0a0a 2020 2020 2020 2020      );..        
+00001170: 2f2f 2055 7064 6174 6520 7468 6520 6669  // Update the fi
+00001180: 6c65 0a20 2020 2020 2020 206c 6574 2075  le.        let u
+00001190: 7064 6174 6564 5f6a 7320 3d20 7223 2322  pdated_js = r##"
+000011a0: 6578 706f 7274 2063 6f6e 7374 2049 6e64  export const Ind
+000011b0: 6578 203d 2028 2920 3d3e 2022 3c55 5044  ex = () => "<UPD
+000011c0: 4154 4544 3e22 3b22 2323 3b0a 2020 2020  ATED>";"##;.    
+000011d0: 2020 2020 6673 3a3a 7772 6974 6528 266a      fs::write(&j
+000011e0: 735f 6669 6c65 5f70 6174 682c 2075 7064  s_file_path, upd
+000011f0: 6174 6564 5f6a 7329 2e75 6e77 7261 7028  ated_js).unwrap(
+00001200: 293b 0a0a 2020 2020 2020 2020 7265 6275  );..        rebu
+00001210: 696c 645f 636f 6e74 6578 7428 636f 6e74  ild_context(cont
+00001220: 6578 745f 6964 292e 756e 7772 6170 2829  ext_id).unwrap()
+00001230: 3b0a 0a20 2020 2020 2020 202f 2f20 4368  ;..        // Ch
+00001240: 6563 6b20 7468 6174 203c 6469 763e 2069  eck that <div> i
+00001250: 7320 696e 2074 6865 2075 7064 6174 6564  s in the updated
+00001260: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
+00001270: 6c65 7420 7570 6461 7465 645f 6f75 7470  let updated_outp
+00001280: 7574 203d 2066 733a 3a72 6561 645f 746f  ut = fs::read_to
+00001290: 5f73 7472 696e 6728 266f 7574 7075 745f  _string(&output_
+000012a0: 6669 6c65 5f70 6174 6829 2e75 6e77 7261  file_path).unwra
+000012b0: 7028 293b 0a20 2020 2020 2020 2070 7269  p();.        pri
+000012c0: 6e74 6c6e 2128 224f 7574 7075 7420 323a  ntln!("Output 2:
+000012d0: 207b 7d22 2c20 6f75 7470 7574 293b 0a20   {}", output);. 
+000012e0: 2020 2020 2020 2061 7373 6572 7421 280a         assert!(.
+000012f0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00001300: 7465 645f 6f75 7470 7574 2e63 6f6e 7461  ted_output.conta
+00001310: 696e 7328 223c 5550 4441 5445 443e 2229  ins("<UPDATED>")
+00001320: 2c0a 2020 2020 2020 2020 2020 2020 2255  ,.            "U
+00001330: 7064 6174 6564 206f 7574 7075 7420 646f  pdated output do
+00001340: 6573 206e 6f74 2063 6f6e 7461 696e 2065  es not contain e
+00001350: 7870 6563 7465 6420 3c55 5044 4154 4544  xpected <UPDATED
+00001360: 3e20 7461 6722 0a20 2020 2020 2020 2029  > tag".        )
+00001370: 3b0a 2020 2020 7d0a 0a20 2020 2023 5b74  ;.    }..    #[t
+00001380: 6573 745d 0a20 2020 2066 6e20 7465 7374  est].    fn test
+00001390: 5f72 6562 7569 6c64 5f63 6f6e 7465 7874  _rebuild_context
+000013a0: 7328 2920 7b0a 2020 2020 2020 2020 6c65  s() {.        le
+000013b0: 7420 7465 6d70 5f64 6972 203d 2074 656d  t temp_dir = tem
+000013c0: 7064 6972 2829 2e75 6e77 7261 7028 293b  pdir().unwrap();
+000013d0: 0a20 2020 2020 2020 206c 6574 206a 735f  .        let js_
+000013e0: 6669 6c65 5f70 6174 6820 3d20 7465 6d70  file_path = temp
+000013f0: 5f64 6972 2e70 6174 6828 292e 6a6f 696e  _dir.path().join
+00001400: 2822 7373 722e 6a73 2229 3b0a 2020 2020  ("ssr.js");.    
+00001410: 2020 2020 6c65 7420 6f75 7470 7574 5f66      let output_f
+00001420: 696c 655f 7061 7468 203d 2074 656d 705f  ile_path = temp_
+00001430: 6469 722e 7061 7468 2829 2e6a 6f69 6e28  dir.path().join(
+00001440: 2273 7372 2e6a 732e 6f75 7422 293b 0a0a  "ssr.js.out");..
+00001450: 2020 2020 2020 2020 2f2f 2057 7269 7465          // Write
+00001460: 2061 2073 696d 706c 6520 6a61 7661 7363   a simple javasc
+00001470: 7269 7074 2066 756e 6374 696f 6e20 746f  ript function to
+00001480: 2061 2066 696c 6520 696e 2061 2074 6d70   a file in a tmp
+00001490: 2064 6972 6563 746f 7279 0a20 2020 2020   directory.     
+000014a0: 2020 206c 6574 2069 6e69 7469 616c 5f6a     let initial_j
+000014b0: 7320 3d20 7223 2322 6578 706f 7274 2063  s = r##"export c
+000014c0: 6f6e 7374 2049 6e64 6578 203d 2028 2920  onst Index = () 
+000014d0: 3d3e 2022 3c49 4e49 5449 414c 3e22 3b22  => "<INITIAL>";"
+000014e0: 2323 3b0a 2020 2020 2020 2020 6673 3a3a  ##;.        fs::
+000014f0: 7772 6974 6528 266a 735f 6669 6c65 5f70  write(&js_file_p
+00001500: 6174 682c 2069 6e69 7469 616c 5f6a 7329  ath, initial_js)
+00001510: 2e75 6e77 7261 7028 293b 0a0a 2020 2020  .unwrap();..    
+00001520: 2020 2020 6c65 7420 636f 6e74 6578 745f      let context_
+00001530: 6964 203d 0a20 2020 2020 2020 2020 2020  id =.           
+00001540: 2067 6574 5f62 7569 6c64 5f63 6f6e 7465   get_build_conte
+00001550: 7874 2826 6a73 5f66 696c 655f 7061 7468  xt(&js_file_path
+00001560: 2e74 6f5f 7374 7228 292e 756e 7772 6170  .to_str().unwrap
+00001570: 2829 2c20 2222 2c20 2264 6576 656c 6f70  (), "", "develop
+00001580: 6d65 6e74 222c 2030 2c20 7472 7565 292e  ment", 0, true).
+00001590: 756e 7772 6170 2829 3b0a 2020 2020 2020  unwrap();.      
+000015a0: 2020 6173 7365 7274 5f6e 6521 2863 6f6e    assert_ne!(con
+000015b0: 7465 7874 5f69 642c 2030 293b 0a0a 2020  text_id, 0);..  
+000015c0: 2020 2020 2020 7265 6275 696c 645f 636f        rebuild_co
+000015d0: 6e74 6578 7473 2876 6563 215b 636f 6e74  ntexts(vec![cont
+000015e0: 6578 745f 6964 5d29 2e75 6e77 7261 7028  ext_id]).unwrap(
+000015f0: 293b 0a20 2020 2020 2020 2061 7373 6572  );.        asser
+00001600: 7421 286f 7574 7075 745f 6669 6c65 5f70  t!(output_file_p
+00001610: 6174 682e 6578 6973 7473 2829 293b 0a20  ath.exists());. 
+00001620: 2020 207d 0a0a 2020 2020 235b 7465 7374     }..    #[test
+00001630: 5d0a 2020 2020 666e 2074 6573 745f 6578  ].    fn test_ex
+00001640: 6365 7074 696f 6e5f 7468 726f 776e 2829  ception_thrown()
+00001650: 207b 0a20 2020 2020 2020 206c 6574 2074   {.        let t
+00001660: 656d 705f 6469 7220 3d20 7465 6d70 6469  emp_dir = tempdi
+00001670: 7228 292e 756e 7772 6170 2829 3b0a 2020  r().unwrap();.  
+00001680: 2020 2020 2020 6c65 7420 6a73 5f66 696c        let js_fil
+00001690: 655f 7061 7468 203d 2074 656d 705f 6469  e_path = temp_di
+000016a0: 722e 7061 7468 2829 2e6a 6f69 6e28 2273  r.path().join("s
+000016b0: 7372 2e6a 7322 293b 0a20 2020 2020 2020  sr.js");.       
+000016c0: 206c 6574 206f 7574 7075 745f 6669 6c65   let output_file
+000016d0: 5f70 6174 6820 3d20 7465 6d70 5f64 6972  _path = temp_dir
+000016e0: 2e70 6174 6828 292e 6a6f 696e 2822 7373  .path().join("ss
+000016f0: 722e 6a73 2e6f 7574 2229 3b0a 0a20 2020  r.js.out");..   
+00001700: 2020 2020 202f 2f20 5772 6974 6520 6120       // Write a 
+00001710: 7369 6d70 6c65 206a 6176 6173 6372 6970  simple javascrip
+00001720: 7420 6675 6e63 7469 6f6e 2074 6f20 6120  t function to a 
+00001730: 6669 6c65 2069 6e20 6120 746d 7020 6469  file in a tmp di
+00001740: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+00001750: 6c65 7420 696e 6974 6961 6c5f 6a73 203d  let initial_js =
+00001760: 2072 2323 2265 7870 6f72 7420 636f 6e73   r##"export cons
+00001770: 7420 496e 6465 7820 494e 5641 4c49 4420  t Index INVALID 
+00001780: 5359 4e54 4158 2028 2920 3d3e 2022 3c49  SYNTAX () => "<I
+00001790: 4e49 5449 414c 3e22 3b22 2323 3b0a 2020  NITIAL>";"##;.  
+000017a0: 2020 2020 2020 6673 3a3a 7772 6974 6528        fs::write(
+000017b0: 266a 735f 6669 6c65 5f70 6174 682c 2069  &js_file_path, i
+000017c0: 6e69 7469 616c 5f6a 7329 2e75 6e77 7261  nitial_js).unwra
+000017d0: 7028 293b 0a0a 2020 2020 2020 2020 6c65  p();..        le
+000017e0: 7420 636f 6e74 6578 745f 6964 203d 0a20  t context_id =. 
+000017f0: 2020 2020 2020 2020 2020 2067 6574 5f62             get_b
+00001800: 7569 6c64 5f63 6f6e 7465 7874 2826 6a73  uild_context(&js
+00001810: 5f66 696c 655f 7061 7468 2e74 6f5f 7374  _file_path.to_st
+00001820: 7228 292e 756e 7772 6170 2829 2c20 2222  r().unwrap(), ""
+00001830: 2c20 2264 6576 656c 6f70 6d65 6e74 222c  , "development",
+00001840: 2030 2c20 7472 7565 292e 756e 7772 6170   0, true).unwrap
+00001850: 2829 3b0a 2020 2020 2020 2020 6173 7365  ();.        asse
+00001860: 7274 5f6e 6521 2863 6f6e 7465 7874 5f69  rt_ne!(context_i
+00001870: 642c 2030 293b 0a0a 2020 2020 2020 2020  d, 0);..        
+00001880: 6c65 7420 7265 7375 6c74 203d 2072 6562  let result = reb
+00001890: 7569 6c64 5f63 6f6e 7465 7874 2863 6f6e  uild_context(con
+000018a0: 7465 7874 5f69 6429 3b0a 2020 2020 2020  text_id);.      
+000018b0: 2020 6173 7365 7274 2128 0a20 2020 2020    assert!(.     
+000018c0: 2020 2020 2020 2072 6573 756c 742e 6973         result.is
+000018d0: 5f65 7272 2829 2c0a 2020 2020 2020 2020  _err(),.        
+000018e0: 2020 2020 2245 7870 6563 7465 6420 616e      "Expected an
+000018f0: 2065 7272 6f72 2064 7572 696e 6720 7265   error during re
+00001900: 6275 696c 645f 636f 6e74 6578 742c 2062  build_context, b
+00001910: 7574 206e 6f6e 6520 6f63 6375 7272 6564  ut none occurred
+00001920: 2e22 0a20 2020 2020 2020 2029 3b0a 2020  .".        );.  
+00001930: 2020 2020 2020 6173 7365 7274 2128 216f        assert!(!o
+00001940: 7574 7075 745f 6669 6c65 5f70 6174 682e  utput_file_path.
+00001950: 6578 6973 7473 2829 293b 0a20 2020 207d  exists());.    }
+00001960: 0a7d 0a                                  .}.
```

### Comparing `mountaineer-0.4.2.dev2/Cargo.toml` & `mountaineer-0.4.2.dev3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.4.2-dev2"
+version = "0.4.2-dev3"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.4.2.dev2/.github/poetry.lock` & `mountaineer-0.4.2.dev3/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/pyproject.toml` & `mountaineer-0.4.2.dev3/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.4.2.dev3/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/scripts/check_dependencies.py` & `mountaineer-0.4.2.dev3/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/scripts/update_version.py` & `mountaineer-0.4.2.dev3/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/workflows/publish_docs.yml` & `mountaineer-0.4.2.dev3/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/.github/workflows/test.yml` & `mountaineer-0.4.2.dev3/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -335,14 +335,22 @@
                 export PATH=/opt/rh/llvm-toolset-7/root/usr/bin:/opt/rh/llvm-toolset-7/root/usr/sbin:/opt/rh/devtoolset-10/root/usr/bin:$PATH
                 export LIBCLANG_PATH=/opt/rh/llvm-toolset-7/root/usr/lib64/
             elif [ "$DISTRO" = "ubuntu" ]; then
                 # Ubuntu specific package installation
                 # Clang is already installed as part of the base image
                 apt-get update
                 apt-get -y install wget
+
+                # The maturin environment includes the gcc cross-compilers for aarch64, but it
+                # doesn't include the necessary headers
+                # This causes issues when rust / bindgen tries to run clang, which will fail with
+                # missing headers like 'bits/libc-header-start.h' file not found
+                # We install the headers here to fix this issue
+                apt install -y gcc-aarch64-linux-gnu g++-aarch64-linux-gnu
+                find /usr -name libc-header-start.h
             else
                 echo "Unsupported distribution: $DISTRO"
                 exit 1
             fi
 
             clang --version
```

### Comparing `mountaineer-0.4.2.dev2/.gitignore` & `mountaineer-0.4.2.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/Dockerfile` & `mountaineer-0.4.2.dev3/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/LICENSE` & `mountaineer-0.4.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/Makefile` & `mountaineer-0.4.2.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/README.md` & `mountaineer-0.4.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/benchmarking/poetry.lock` & `mountaineer-0.4.2.dev3/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/README.md` & `mountaineer-0.4.2.dev3/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/app.py` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.4.2.dev3/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/poetry.lock` & `mountaineer-0.4.2.dev3/ci_webapp/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry 1.7.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "annotated-types"
 version = "0.6.0"
 description = "Reusable constraint types to use with typing.Annotated"
 optional = false
 python-versions = ">=3.8"
@@ -292,14 +292,49 @@
 python-versions = ">=3.5"
 files = [
     {file = "inflection-0.5.1-py2.py3-none-any.whl", hash = "sha256:f38b2b640938a4f35ade69ac3d053042959b62a0f1076a5bbaa1b9526605a8a2"},
     {file = "inflection-0.5.1.tar.gz", hash = "sha256:1a29730d366e996aaacffb2f1f1cb9593dc38e2ddd30c91250c6dde09ea9b417"},
 ]
 
 [[package]]
+name = "markdown-it-py"
+version = "3.0.0"
+description = "Python port of markdown-it. Markdown parsing, done right!"
+optional = false
+python-versions = ">=3.8"
+files = [
+    {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
+    {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
+]
+
+[package.dependencies]
+mdurl = ">=0.1,<1.0"
+
+[package.extras]
+benchmarking = ["psutil", "pytest", "pytest-benchmark"]
+code-style = ["pre-commit (>=3.0,<4.0)"]
+compare = ["commonmark (>=0.9,<1.0)", "markdown (>=3.4,<4.0)", "mistletoe (>=1.0,<2.0)", "mistune (>=2.0,<3.0)", "panflute (>=2.3,<3.0)"]
+linkify = ["linkify-it-py (>=1,<3)"]
+plugins = ["mdit-py-plugins"]
+profiling = ["gprof2dot"]
+rtd = ["jupyter_sphinx", "mdit-py-plugins", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
+testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
+
+[[package]]
+name = "mdurl"
+version = "0.1.2"
+description = "Markdown URL utilities"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
+    {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
+]
+
+[[package]]
 name = "mountaineer"
 version = "0.1.0"
 description = ""
 optional = false
 python-versions = "^3.11"
 files = []
 develop = true
@@ -308,17 +343,17 @@
 asyncpg = "^0.29.0"
 click = "^8.1.7"
 fastapi = "^0.109.0"
 inflection = "^0.5.1"
 packaging = "^23.2"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
+rich = "^13.7.1"
 sqlalchemy = {version = "^2.0.26", extras = ["asyncio"]}
 sqlmodel = "^0.0.14"
-tqdm = "^4.66.1"
 uvicorn = {version = "^0.27.0.post1", extras = ["standard"]}
 watchdog = "^3.0.0"
 
 [package.source]
 type = "directory"
 url = ".."
 
@@ -530,14 +565,29 @@
 python-dotenv = ">=0.21.0"
 
 [package.extras]
 toml = ["tomli (>=2.0.1)"]
 yaml = ["pyyaml (>=6.0.1)"]
 
 [[package]]
+name = "pygments"
+version = "2.17.2"
+description = "Pygments is a syntax highlighting package written in Python."
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "pygments-2.17.2-py3-none-any.whl", hash = "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c"},
+    {file = "pygments-2.17.2.tar.gz", hash = "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"},
+]
+
+[package.extras]
+plugins = ["importlib-metadata"]
+windows-terminal = ["colorama (>=0.4.6)"]
+
+[[package]]
 name = "pyright"
 version = "1.1.352"
 description = "Command line wrapper for pyright"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pyright-1.1.352-py3-none-any.whl", hash = "sha256:0040cf173c6a60704e553bfd129dfe54de59cc76d0b2b80f77cfab4f50701d64"},
@@ -586,14 +636,15 @@
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc"},
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673"},
     {file = "PyYAML-6.0.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b"},
     {file = "PyYAML-6.0.1-cp311-cp311-win32.whl", hash = "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741"},
     {file = "PyYAML-6.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9"},
+    {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef"},
     {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0"},
     {file = "PyYAML-6.0.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4"},
     {file = "PyYAML-6.0.1-cp312-cp312-win32.whl", hash = "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54"},
     {file = "PyYAML-6.0.1-cp312-cp312-win_amd64.whl", hash = "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df"},
     {file = "PyYAML-6.0.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47"},
     {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98"},
     {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c"},
@@ -621,14 +672,32 @@
     {file = "PyYAML-6.0.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5"},
     {file = "PyYAML-6.0.1-cp39-cp39-win32.whl", hash = "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c"},
     {file = "PyYAML-6.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486"},
     {file = "PyYAML-6.0.1.tar.gz", hash = "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43"},
 ]
 
 [[package]]
+name = "rich"
+version = "13.7.1"
+description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
+optional = false
+python-versions = ">=3.7.0"
+files = [
+    {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
+    {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
+]
+
+[package.dependencies]
+markdown-it-py = ">=2.2.0"
+pygments = ">=2.13.0,<3.0.0"
+
+[package.extras]
+jupyter = ["ipywidgets (>=7.5.1,<9)"]
+
+[[package]]
 name = "ruff"
 version = "0.1.15"
 description = "An extremely fast Python linter and code formatter, written in Rust."
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "ruff-0.1.15-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:5fe8d54df166ecc24106db7dd6a68d44852d14eb0729ea4672bb4d96c320b7df"},
@@ -793,34 +862,14 @@
 [package.dependencies]
 anyio = ">=3.4.0,<5"
 
 [package.extras]
 full = ["httpx (>=0.22.0)", "itsdangerous", "jinja2", "python-multipart (>=0.0.7)", "pyyaml"]
 
 [[package]]
-name = "tqdm"
-version = "4.66.2"
-description = "Fast, Extensible Progress Meter"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "tqdm-4.66.2-py3-none-any.whl", hash = "sha256:1ee4f8a893eb9bef51c6e35730cebf234d5d0b6bd112b0271e10ed7c24a02bd9"},
-    {file = "tqdm-4.66.2.tar.gz", hash = "sha256:6cd52cdf0fef0e0f543299cfc96fec90d7b8a7e88745f411ec33eb44d5ed3531"},
-]
-
-[package.dependencies]
-colorama = {version = "*", markers = "platform_system == \"Windows\""}
-
-[package.extras]
-dev = ["pytest (>=6)", "pytest-cov", "pytest-timeout", "pytest-xdist"]
-notebook = ["ipywidgets (>=6)"]
-slack = ["slack-sdk"]
-telegram = ["requests"]
-
-[[package]]
 name = "types-setuptools"
 version = "69.1.0.20240301"
 description = "Typing stubs for setuptools"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "types-setuptools-69.1.0.20240301.tar.gz", hash = "sha256:f99cf5a7f5c281c55f16ba860da68cb2cd8f3b3a472f78ec8e744240fc3aa09e"},
```

### Comparing `mountaineer-0.4.2.dev2/ci_webapp/pyproject.toml` & `mountaineer-0.4.2.dev3/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/README.md` & `mountaineer-0.4.2.dev3/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.4.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/poetry.lock` & `mountaineer-0.4.2.dev3/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/create_mountaineer_app/pyproject.toml` & `mountaineer-0.4.2.dev3/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/client_actions.md` & `mountaineer-0.4.2.dev3/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/cma.md` & `mountaineer-0.4.2.dev3/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/database.md` & `mountaineer-0.4.2.dev3/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/deploy.md` & `mountaineer-0.4.2.dev3/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/error_handling.md` & `mountaineer-0.4.2.dev3/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/index.md` & `mountaineer-0.4.2.dev3/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/internal/core_library.md` & `mountaineer-0.4.2.dev3/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/links.md` & `mountaineer-0.4.2.dev3/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.4.2.dev3/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.4.2.dev3/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/media/network_debug.png` & `mountaineer-0.4.2.dev3/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.4.2.dev3/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/metadata.md` & `mountaineer-0.4.2.dev3/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/postcss.md` & `mountaineer-0.4.2.dev3/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/quickstart.md` & `mountaineer-0.4.2.dev3/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/static_analysis.md` & `mountaineer-0.4.2.dev3/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/structure.md` & `mountaineer-0.4.2.dev3/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.4.2.dev3/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/docs/views.md` & `mountaineer-0.4.2.dev3/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/mkdocs.yml` & `mountaineer-0.4.2.dev3/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/docs_website/poetry.lock` & `mountaineer-0.4.2.dev3/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/media/header.png` & `mountaineer-0.4.2.dev3/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__init__.py` & `mountaineer-0.4.2.dev3/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_app.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cache.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cli.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_controller.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_logging.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_paths.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_watch.py` & `mountaineer-0.4.2.dev3/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/actions/fields.py` & `mountaineer-0.4.2.dev3/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/actions/passthrough.py` & `mountaineer-0.4.2.dev3/mountaineer/actions/passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/actions/sideeffect.py` & `mountaineer-0.4.2.dev3/mountaineer/actions/sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/annotation_helpers.py` & `mountaineer-0.4.2.dev3/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/app.py` & `mountaineer-0.4.2.dev3/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/cache.py` & `mountaineer-0.4.2.dev3/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/cli.py` & `mountaineer-0.4.2.dev3/mountaineer/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import asyncio
 import socket
-from contextlib import contextmanager
+from contextlib import contextmanager, redirect_stdout
 from dataclasses import dataclass
 from functools import partial
 from importlib import import_module
 from importlib.metadata import distributions
+from io import StringIO
 from multiprocessing import Event, Process, Queue, get_start_method, set_start_method
 from multiprocessing.queues import Queue as QueueType
 from pathlib import Path
 from signal import SIGINT, signal
 from tempfile import mkdtemp
 from threading import Thread
-from time import sleep, time
+from time import monotonic_ns, sleep, time
 from traceback import format_exception
 from typing import Any, Callable, MutableMapping
 
 from click import secho
 from fastapi import Request
+from rich.traceback import install as rich_traceback_install
 
 from mountaineer.app import AppController
 from mountaineer.client_builder.builder import ClientBuilder
+from mountaineer.console import CONSOLE, ERROR_CONSOLE
 from mountaineer.controllers.exception_controller import ExceptionController
 from mountaineer.js_compiler.exceptions import BuildProcessException
 from mountaineer.logging import LOGGER
 from mountaineer.watch import (
     CallbackDefinition,
     CallbackMetadata,
     CallbackType,
@@ -85,15 +88,31 @@
         )
 
     def run(self):
         LOGGER.debug(
             f"Starting isolated environment process with\nbuild_config: {self.build_config}\nrunserver_config: {self.runserver_config}"
         )
 
-        app_controller = import_from_string(self.build_config.webcontroller)
+        CONSOLE.rule("[bold red]Mountaineer Build Started")
+
+        with (
+            # We don't want to print stdout on the initial import, since this will just duplicate
+            # the init code / logging of the app. We use our error console to avoid
+            # capturing the stdout of our logging
+            ERROR_CONSOLE.status("[bold blue]Loading app...", spinner="dots"),
+            StringIO() as buf,
+            redirect_stdout(buf),
+        ):
+            start = monotonic_ns()
+            app_controller = import_from_string(self.build_config.webcontroller)
+            LOGGER.debug(f"Load app logs: {buf.getvalue()}")
+        CONSOLE.print(
+            f"[bold green]🎒 Loaded app in {(monotonic_ns() - start) / 1e9:.2f}s"
+        )
+
         if not isinstance(app_controller, AppController):
             raise ValueError(
                 f"Expected {self.build_config.webcontroller} to be an instance of AppController"
             )
 
         # Mount our exceptions controller, since we'll need these artifacts built
         # as part of the JS build phase
@@ -196,35 +215,36 @@
                 self.run_build(app_controller)
 
         LOGGER.debug("Will launch rebuild thread")
         rebuild_thread = Thread(target=wait_for_rebuild)
         rebuild_thread.start()
 
     def run_build(self, app_controller: AppController):
-        secho("Starting build...", fg="yellow")
         start = time()
         js_compiler = ClientBuilder(
             app_controller,
             live_reload_port=(
                 self.runserver_config.live_reload_port
                 if self.runserver_config
                 else None
             ),
             build_cache=self.build_config.build_cache,
         )
         try:
             js_compiler.build()
-            secho(f"Build finished in {time() - start:.2f} seconds", fg="green")
+            CONSOLE.print(
+                f"[bold green]🚀 App launched in {time() - start:.2f} seconds"
+            )
 
             # Completed successfully
             app_controller.build_exception = None
 
             self.alert_notification_channel()
         except BuildProcessException as e:
-            secho(f"Build failed: {e}", fg="red")
+            CONSOLE.print(f"[bold red]⚠️ Build failed: {e}")
             app_controller.build_exception = e
 
     def stop(self, hard_timeout: float = 5.0):
         """
         Client-side stop method to shut down the running process.
         """
         # If we've already stopped, don't try to stop again
@@ -340,14 +360,16 @@
     :param webcontroller: Ex. "ci_webapp.app:controller"
     :param port: Desired port for the webapp while running locally
     :param subscribe_to_mountaineer: See `handle_watch` for more details.
 
     """
     update_multiprocessing_settings()
 
+    rich_traceback_install()
+
     current_process: IsolatedEnvProcess | None = None
 
     # The global cache will let us keep cache files warm across
     # different builds
     global_build_cache = Path(mkdtemp())
 
     # Start the webservice - it should persist for the lifetime of the
@@ -416,15 +438,15 @@
     app_controller = import_from_string(webcontroller)
     js_compiler = ClientBuilder(
         app_controller,
         live_reload_port=None,
     )
     start = time()
     js_compiler.build()
-    secho(f"Build finished in {time() - start:.2f} seconds", fg="green")
+    CONSOLE.print(f"[bold green]App built in {time() - start:.2f}s")
 
 
 def update_multiprocessing_settings():
     """
     fork() is still the default on Linux, and can result in stalls with our asyncio
     event loops. For consistency and expected behavior, try to switch to spawn()
     if it's not already enabled.
@@ -512,20 +534,28 @@
     )
 
 
 @contextmanager
 def init_global_state(webcontroller: str):
     """
     Initialize global state: signal to each builder that they can
-    initialize global state before the fork.
+    set up their own global state before the fork.
 
     """
     global_state: dict[Any, Any] = {}
 
-    app_controller = import_from_string(webcontroller)
+    with (
+        ERROR_CONSOLE.status(
+            "[bold blue]Setting up global state before fork...", spinner="dots"
+        ),
+        StringIO() as buf,
+        redirect_stdout(buf),
+    ):
+        app_controller = import_from_string(webcontroller)
+        LOGGER.debug(f"init_global_state Load app logs: {buf.getvalue()}")
 
     if not isinstance(app_controller, AppController):
         raise ValueError(f"Unknown app controller: {app_controller}")
 
     async def entrypoint():
         await asyncio.gather(
             *[builder.init_state(global_state) for builder in app_controller.builders]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_actions.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_links.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/builder.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from mountaineer.client_builder.build_links import OpenAPIToTypescriptLinkConverter
 from mountaineer.client_builder.build_schemas import OpenAPIToTypescriptSchemaConverter
 from mountaineer.client_builder.openapi import OpenAPIDefinition, OpenAPISchema
 from mountaineer.client_builder.typescript import (
     TSLiteral,
     python_payload_to_typescript,
 )
+from mountaineer.console import CONSOLE
 from mountaineer.controller import ControllerBase
 from mountaineer.io import gather_with_concurrency
 from mountaineer.js_compiler.base import ClientBundleMetadata
 from mountaineer.js_compiler.exceptions import BuildProcessException
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, generate_relative_import
 from mountaineer.static import get_static_path
@@ -66,34 +67,38 @@
 
     def build(self):
         asyncio.run(self.async_build())
 
     async def async_build(self):
         # Avoid rebuilding if we don't need to
         if self.cache_is_outdated():
-            secho("Building useServer, cache outdated...", fg="green")
+            start = monotonic_ns()
 
-            # Make sure our application definitions are in a valid state before we start
-            # to build the client code
-            self.validate_unique_paths()
-
-            # Static files that don't depend on client code
-            self.generate_static_files()
-
-            # The order of these generators don't particularly matter since most TSX linters
-            # won't refresh until they're all complete. However, this ordering better aligns
-            # with semantic dependencies so we keep the linearity where possible.
-            self.generate_model_definitions()
-            self.generate_action_definitions()
-            self.generate_link_shortcuts()
-            self.generate_link_aggregator()
-            self.generate_view_servers()
-            self.generate_index_file()
+            with CONSOLE.status("Building useServer", spinner="dots"):
+                # Make sure our application definitions are in a valid state before we start
+                # to build the client code
+                self.validate_unique_paths()
+
+                # Static files that don't depend on client code
+                self.generate_static_files()
+
+                # The order of these generators don't particularly matter since most TSX linters
+                # won't refresh until they're all complete. However, this ordering better aligns
+                # with semantic dependencies so we keep the linearity where possible.
+                self.generate_model_definitions()
+                self.generate_action_definitions()
+                self.generate_link_shortcuts()
+                self.generate_link_aggregator()
+                self.generate_view_servers()
+                self.generate_index_file()
+            CONSOLE.print(
+                f"[bold green]🔨 Built useServer in {(monotonic_ns() - start) / 1e9:.2f}s"
+            )
         else:
-            secho("useServer up to date", fg="green")
+            CONSOLE.print("[bold green]useServer up to date")
 
         await self.build_javascript_chunks()
 
         # Update the cached paths attached to the app
         for controller_definition in self.app.controllers:
             controller = controller_definition.controller
             controller.resolve_paths(self.view_root, force=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/openapi.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/client_builder/typescript.py` & `mountaineer-0.4.2.dev3/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/config.py` & `mountaineer-0.4.2.dev3/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/controller.py` & `mountaineer-0.4.2.dev3/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/controllers/exception_controller.py` & `mountaineer-0.4.2.dev3/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/cropper.py` & `mountaineer-0.4.2.dev3/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/database/cli.py` & `mountaineer-0.4.2.dev3/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/database/config.py` & `mountaineer-0.4.2.dev3/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/database/dependencies/core.py` & `mountaineer-0.4.2.dev3/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/database/sqlmodel.py` & `mountaineer-0.4.2.dev3/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/database/validator.py` & `mountaineer-0.4.2.dev3/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/dependencies/base.py` & `mountaineer-0.4.2.dev3/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/dependencies/core/core.py` & `mountaineer-0.4.2.dev3/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/exceptions.py` & `mountaineer-0.4.2.dev3/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/io.py` & `mountaineer-0.4.2.dev3/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/js_compiler/base.py` & `mountaineer-0.4.2.dev3/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/js_compiler/javascript.py` & `mountaineer-0.4.2.dev3/mountaineer/js_compiler/javascript.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from dataclasses import dataclass
 from pathlib import Path
 from threading import Thread
 from time import monotonic_ns
 from typing import Any
 
 from inflection import underscore
+from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
 from mountaineer import mountaineer as mountaineer_rs  # type: ignore
+from mountaineer.console import CONSOLE
 from mountaineer.controller import ControllerBase
 from mountaineer.js_compiler.base import ClientBuilderBase, ClientBundleMetadata
 from mountaineer.js_compiler.exceptions import BuildProcessException
 from mountaineer.logging import LOGGER
 from mountaineer.paths import ManagedViewPath, generate_relative_import
 
 
@@ -101,31 +103,55 @@
                 break
 
             build_params = [
                 mountaineer_rs.BuildContextParams(*params) for params in payload
             ]
 
             start = monotonic_ns()
-            try:
-                # TODO: Right now this raises pyo3_runtime.PanicException, which isn't caught
-                # appropriately. Our try/except block should be catching this.
-                mountaineer_rs.build_javascript(build_params)
-            except Exception as e:
-                LOGGER.error(f"Error building JS: {e}")
-                output_queue.put(
-                    CompiledOutput(
-                        success=False,
-                        exception_type=e.__class__.__name__,
-                        exception_message=str(e),
-                    )
+
+            with Progress(
+                SpinnerColumn(),
+                *Progress.get_default_columns(),
+                TimeElapsedColumn(),
+                console=CONSOLE,
+                transient=True,
+            ) as progress:
+                build_task = progress.add_task(
+                    "[cyan]Compiling...", total=len(build_params)
                 )
-                continue
 
-            LOGGER.debug(
-                f"Processed payload in {(monotonic_ns() - start) / 1e9} seconds"
+                try:
+
+                    def build_complete_callback(callback_args: tuple[int]):
+                        """
+                        Callback called when each individual file build is complete. For a successful
+                        build this callback |N| should match the input build_params.
+
+                        """
+                        progress.advance(build_task, 1)
+
+                    # Right now this raises pyo3_runtime.PanicException, which isn't caught
+                    # appropriately. Our try/except block should be catching this.
+                    mountaineer_rs.build_javascript(
+                        build_params, build_complete_callback
+                    )
+
+                except Exception as e:
+                    LOGGER.error(f"Error building JS: {e}")
+                    output_queue.put(
+                        CompiledOutput(
+                            success=False,
+                            exception_type=e.__class__.__name__,
+                            exception_message=str(e),
+                        )
+                    )
+                    continue
+
+            CONSOLE.print(
+                f"[bold green]📬 Compiled frontend in {(monotonic_ns() - start) / 1e9:.2f}s"
             )
 
             output_queue.put(CompiledOutput(success=True))
 
     async def start_build(self):
         self.pending_files = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mountaineer-0.4.2.dev2/mountaineer/js_compiler/postcss.py` & `mountaineer-0.4.2.dev3/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.4.2.dev3/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/logging.py` & `mountaineer-0.4.2.dev3/mountaineer/logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import logging
 from contextlib import contextmanager
 from json import dumps as json_dumps
 from logging import Formatter, StreamHandler, getLogger
+from os import environ
 from time import monotonic_ns
 
 from click import secho
 
+VERBOSITY_MAPPING = {
+    "INFO": logging.INFO,
+    "DEBUG": logging.DEBUG,
+    "WARNING": logging.WARNING,
+    "ERROR": logging.ERROR,
+}
+
 
 class JsonFormatter(Formatter):
     def format(self, record):
         log_record = {
             "level": record.levelname,
             "name": record.name,
             "timestamp": self.formatTime(record, self.datefmt),
@@ -37,16 +45,14 @@
 def setup_logger(name, log_level=logging.DEBUG):
     """
     Constructor for the main logger used by Mountaineer. Provided
     convenient defaults for log level and formatting, alongside coloring
     of stdout/stderr messages and JSON fields for structured parsing.
 
     """
-    # TODO - env driven logging configuration
-
     logger = getLogger(name)
     logger.setLevel(log_level)
 
     # Create a handler that writes log records to the standard error
     handler = ColorHandler()
     handler.setLevel(log_level)
 
@@ -71,8 +77,12 @@
 
     """
     start = monotonic_ns()
     yield
     LOGGER.debug(f"{message} : Took {(monotonic_ns() - start)/1e9:.2f}s")
 
 
-LOGGER = setup_logger(__name__)
+# Our global logger should only surface warnings and above by default
+LOGGER = setup_logger(
+    __name__,
+    log_level=VERBOSITY_MAPPING[environ.get("MOUNTAINEER_LOG_LEVEL", "WARNING")],
+)
```

### Comparing `mountaineer-0.4.2.dev2/mountaineer/paths.py` & `mountaineer-0.4.2.dev3/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/render.py` & `mountaineer-0.4.2.dev3/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/ssr.py` & `mountaineer-0.4.2.dev3/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/static/api.ts` & `mountaineer-0.4.2.dev3/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/static/live_reload.ts` & `mountaineer-0.4.2.dev3/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/test_utilities.py` & `mountaineer-0.4.2.dev3/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/views/package-lock.json` & `mountaineer-0.4.2.dev3/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/mountaineer/watch.py` & `mountaineer-0.4.2.dev3/mountaineer/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from enum import Flag, auto
 from pathlib import Path
 from threading import Timer
 from typing import Any, Callable
 
-from click import secho
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
+from mountaineer.console import CONSOLE
 from mountaineer.paths import resolve_package_path
 
 
 class CallbackType(Flag):
     CREATED = auto()
     MODIFIED = auto()
     DELETED = auto()
@@ -62,31 +62,31 @@
         self.pending_events: list[CallbackEvent] = []
 
     def on_modified(self, event):
         super().on_modified(event)
         if self.should_ignore_path(event.src_path):
             return
         if not event.is_directory:
-            secho(f"File modified: {event.src_path}", fg="yellow")
+            CONSOLE.print(f"[yellow]File modified: {event.src_path}")
             self._debounce(CallbackType.MODIFIED, Path(event.src_path))
 
     def on_created(self, event):
         super().on_created(event)
         if self.should_ignore_path(event.src_path):
             return
         if not event.is_directory:
-            secho(f"File created: {event.src_path}", fg="yellow")
+            CONSOLE.print(f"[yellow]File created: {event.src_path}")
             self._debounce(CallbackType.CREATED, Path(event.src_path))
 
     def on_deleted(self, event):
         super().on_deleted(event)
         if self.should_ignore_path(event.src_path):
             return
         if not event.is_directory:
-            secho(f"File deleted: {event.src_path}", fg="yellow")
+            CONSOLE.print(f"[yellow]File deleted: {event.src_path}")
             self._debounce(CallbackType.DELETED, Path(event.src_path))
 
     def _debounce(self, action: CallbackType, path: Path):
         if self.debounce_timer is not None:
             self.debounce_timer.cancel()
 
         self.pending_events.append(CallbackEvent(action=action, path=path))
@@ -174,26 +174,26 @@
                 for callback_definition in self.callbacks:
                     callback_definition.callback(CallbackMetadata(events=[]))
 
             self.event_handler = ChangeEventHandler(callbacks=self.callbacks)
             self.observer = Observer()
 
             for path in self.paths:
-                secho(f"Watching {path}", fg="green")
+                CONSOLE.print(f"[green]Watching {path}")
                 if os.path.isdir(path):
                     self.observer.schedule(self.event_handler, path, recursive=True)
                 else:
                     self.observer.schedule(
                         self.event_handler, os.path.dirname(path), recursive=False
                     )
 
             self.observer.start()
 
             try:
-                secho("Starting observer...")
+                CONSOLE.print("Starting observer...")
                 self.observer.join()
             except KeyboardInterrupt:
                 self.observer.stop()
                 self.observer.join()
 
     def check_packages_installed(self):
         for package in self.packages:
```

### Comparing `mountaineer-0.4.2.dev2/mountaineer/watch_server.py` & `mountaineer-0.4.2.dev3/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/poetry.lock` & `mountaineer-0.4.2.dev3/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -359,14 +359,38 @@
 python-versions = ">=3.7"
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
+name = "markdown-it-py"
+version = "3.0.0"
+description = "Python port of markdown-it. Markdown parsing, done right!"
+optional = false
+python-versions = ">=3.8"
+files = [
+    {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
+    {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
+]
+
+[package.dependencies]
+mdurl = ">=0.1,<1.0"
+
+[package.extras]
+benchmarking = ["psutil", "pytest", "pytest-benchmark"]
+code-style = ["pre-commit (>=3.0,<4.0)"]
+compare = ["commonmark (>=0.9,<1.0)", "markdown (>=3.4,<4.0)", "mistletoe (>=1.0,<2.0)", "mistune (>=2.0,<3.0)", "panflute (>=2.3,<3.0)"]
+linkify = ["linkify-it-py (>=1,<3)"]
+plugins = ["mdit-py-plugins"]
+profiling = ["gprof2dot"]
+rtd = ["jupyter_sphinx", "mdit-py-plugins", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
+testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
+
+[[package]]
 name = "maturin"
 version = "1.5.1"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "maturin-1.5.1-py3-none-linux_armv6l.whl", hash = "sha256:589e9b7024007e130b136ba6f1c2c8393a87e42cf968d12852913ab1e3c69ed3"},
@@ -385,14 +409,25 @@
 ]
 
 [package.extras]
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
+name = "mdurl"
+version = "0.1.2"
+description = "Markdown URL utilities"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
+    {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
+]
+
+[[package]]
 name = "mypy"
 version = "1.9.0"
 description = "Optional static typing for Python"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "mypy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f"},
@@ -611,14 +646,29 @@
 python-dotenv = ">=0.21.0"
 
 [package.extras]
 toml = ["tomli (>=2.0.1)"]
 yaml = ["pyyaml (>=6.0.1)"]
 
 [[package]]
+name = "pygments"
+version = "2.17.2"
+description = "Pygments is a syntax highlighting package written in Python."
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "pygments-2.17.2-py3-none-any.whl", hash = "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c"},
+    {file = "pygments-2.17.2.tar.gz", hash = "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"},
+]
+
+[package.extras]
+plugins = ["importlib-metadata"]
+windows-terminal = ["colorama (>=0.4.6)"]
+
+[[package]]
 name = "pyinstrument"
 version = "4.6.2"
 description = "Call stack profiler for Python. Shows you why your code is slow!"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pyinstrument-4.6.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:7a1b1cd768ea7ea9ab6f5490f7e74431321bcc463e9441dbc2f769617252d9e2"},
@@ -817,14 +867,32 @@
     {file = "PyYAML-6.0.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5"},
     {file = "PyYAML-6.0.1-cp39-cp39-win32.whl", hash = "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c"},
     {file = "PyYAML-6.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486"},
     {file = "PyYAML-6.0.1.tar.gz", hash = "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43"},
 ]
 
 [[package]]
+name = "rich"
+version = "13.7.1"
+description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
+optional = false
+python-versions = ">=3.7.0"
+files = [
+    {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
+    {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
+]
+
+[package.dependencies]
+markdown-it-py = ">=2.2.0"
+pygments = ">=2.13.0,<3.0.0"
+
+[package.extras]
+jupyter = ["ipywidgets (>=7.5.1,<9)"]
+
+[[package]]
 name = "ruff"
 version = "0.1.15"
 description = "An extremely fast Python linter and code formatter, written in Rust."
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "ruff-0.1.15-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:5fe8d54df166ecc24106db7dd6a68d44852d14eb0729ea4672bb4d96c320b7df"},
@@ -1331,8 +1399,8 @@
     {file = "websockets-12.0-py3-none-any.whl", hash = "sha256:dc284bbc8d7c78a6c69e0c7325ab46ee5e40bb4d50e494d8131a07ef47500e9e"},
     {file = "websockets-12.0.tar.gz", hash = "sha256:81df9cbcbb6c260de1e007e58c011bfebe2dafc8435107b0537f393dd38c8b1b"},
 ]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.11"
-content-hash = "379f8c83f526bc77bffd329114b3e311c69b7f7ef5a658bdb7db79d80c983b8f"
+content-hash = "0dbc14c375afc9aa51c9fc2d81907696d98c49eeab22604744478b470733821a"
```

### Comparing `mountaineer-0.4.2.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.4.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/benches/lexers_benchmark.rs` & `mountaineer-0.4.2.dev3/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/benches/source_map_benchmark.rs` & `mountaineer-0.4.2.dev3/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/benches/ssr_benchmark.rs` & `mountaineer-0.4.2.dev3/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/lexers.rs` & `mountaineer-0.4.2.dev3/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/lib.rs` & `mountaineer-0.4.2.dev3/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use errors::AppError;
 use pyo3::exceptions::{PyConnectionAbortedError, PyValueError};
 use pyo3::prelude::*;
+use pyo3::types::PyTuple;
 use std::ffi::c_int;
 use std::fs;
 use std::path::Path;
+use std::sync::{Arc, Mutex};
 use std::time::Duration;
 
 mod errors;
 mod lexers;
 mod logging;
 mod source_map;
 mod ssr;
@@ -137,15 +139,19 @@
             Err(_err) => Err(PyValueError::new_err("Unable to parse source map mappings")),
         }
     }
 
     #[pyfn(m)]
     #[pyo3(name = "build_javascript")]
     // PyRef to support borrow checking: https://github.com/PyO3/pyo3/issues/1177
-    fn build_javascript(_py: Python, params: Vec<PyRef<BuildContextParams>>) -> PyResult<bool> {
+    fn build_javascript(
+        _py: Python,
+        params: Vec<PyRef<BuildContextParams>>,
+        callback: PyObject,
+    ) -> PyResult<bool> {
         #[allow(clippy::print_stdout)]
         if cfg!(debug_assertions) {
             println!("Running in debug mode");
         }
 
         let mut context_ids = Vec::<c_int>::new();
 
@@ -164,15 +170,31 @@
                 Err(err) => {
                     println!("Error getting build context: {:?}", err);
                     return Err(PyErr::new::<PyValueError, _>(err));
                 }
             }
         }
 
-        let rebuild_result = src_go::rebuild_contexts(context_ids);
+        let callback_arc = Arc::new(Mutex::new(callback));
+        let rebuild_result = _py.allow_threads(move || {
+            let callback_cloned = Arc::clone(&callback_arc);
+            fn callback(id: c_int, cb: Arc<Mutex<PyObject>>) {
+                let _ = Python::with_gil(|py| -> PyResult<()> {
+                    let args = PyTuple::new(py, &[id.to_object(py)]);
+                    let cb_lock = cb.lock().unwrap();
+                    cb_lock.call1(py, args)?;
+                    Ok(())
+                });
+            }
+            src_go::rebuild_contexts(
+                context_ids,
+                Arc::new(Box::new(move |id| callback(id, callback_cloned.clone()))),
+            )
+        });
+
         if let Err(err) = rebuild_result {
             println!("Error rebuilding contexts: {:?}", err);
             return Err(PyErr::new::<PyValueError, _>(err.join("\n")));
         }
 
         // We expect that each input path will have an `.js.out.map` file
         // Make the paths referenced in this file absolute to make it clearer for
```

### Comparing `mountaineer-0.4.2.dev2/src/logging.rs` & `mountaineer-0.4.2.dev3/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/source_map.rs` & `mountaineer-0.4.2.dev3/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/ssr.rs` & `mountaineer-0.4.2.dev3/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/src/timeout.rs` & `mountaineer-0.4.2.dev3/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev2/Cargo.lock` & `mountaineer-0.4.2.dev3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.4.2-dev2"
+version = "0.4.2-dev3"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.4.2.dev2/pyproject.toml` & `mountaineer-0.4.2.dev3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "maturin>=1.3.0",]
 build-backend = "maturin"
 
 [project]
 name = "mountaineer"
-dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]",]
+dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]", "rich",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.4.2.dev2"
+version = "0.4.2.dev3"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
@@ -32,14 +32,15 @@
 inflection = "^0.5.1"
 click = "^8.1.7"
 packaging = "^23.2"
 pydantic-settings = "^2.1.0"
 sqlmodel = "^0.0.14"
 asyncpg = "^0.29.0"
 watchdog = "^3.0.0"
+rich = "^13.7.1"
 
 [tool.ruff.lint]
 select = [ "E4", "E7", "E9", "F", "I001", "T201",]
 
 [tool.poetry.dependencies.uvicorn]
 extras = [ "standard",]
 version = "^0.27.0.post1"
```

### Comparing `mountaineer-0.4.2.dev2/PKG-INFO` & `mountaineer-0.4.2.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.4.2.dev2
+Version: 0.4.2.dev3
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
 Requires-Dist: pydantic-settings
 Requires-Dist: sqlmodel
 Requires-Dist: asyncpg
 Requires-Dist: sqlalchemy[asyncio]
+Requires-Dist: rich
 License-File: LICENSE
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ![Mountaineer Header](https://raw.githubusercontent.com/piercefreeman/mountaineer/main/media/header.png)
 
 <p align="center"><i>Move fast. Climb mountains. Don't break things.</i></p>
```

