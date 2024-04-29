# Comparing `tmp/freemocap-1.1.1.tar.gz` & `tmp/freemocap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freemocap-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freemocap-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freemocap-1.1.1.tar` & `freemocap-1.2.0.tar`

### file list

```diff
@@ -1,281 +1,275 @@
--rw-r--r--   0        0        0     1649 2024-03-18 13:05:20.785697 freemocap-1.1.1/.flake8
--rwxr-xr-x   0        0        0      492 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      423 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      730 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/coverage-testing.yml
--rw-r--r--   0        0        0     1138 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/flit_publish_to_pypi.yml
--rwxr-xr-x   0        0        0      385 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/linting-flake8.yml
--rw-r--r--   0        0        0     2049 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/linux_installer.yml
--rw-r--r--   0        0        0     2613 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/mac_installer.yml
--rw-r--r--   0        0        0     1246 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/publish_to_pypi.yml
--rwxr-xr-x   0        0        0     1018 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/python-testing.yml
--rwxr-xr-x   0        0        0      733 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/version-testing.yml
--rw-r--r--   0        0        0     2312 2024-03-18 13:05:20.785697 freemocap-1.1.1/.github/workflows/windows_installer.yml
--rw-r--r--   0        0        0     2011 2024-03-18 13:05:20.785697 freemocap-1.1.1/.gitignore
--rw-r--r--   0        0        0      229 2024-03-18 13:05:20.785697 freemocap-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      657 2024-03-18 13:05:20.785697 freemocap-1.1.1/CITATION.cff
--rw-r--r--   0        0        0      327 2024-03-18 13:05:20.785697 freemocap-1.1.1/CODEOWNERS
--rw-r--r--   0        0        0     1513 2024-03-18 13:05:20.785697 freemocap-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3552 2024-03-18 13:05:20.785697 freemocap-1.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2024-03-18 13:05:20.785697 freemocap-1.1.1/LICENSE
--rw-r--r--   0        0        0      234 2024-03-18 13:05:20.785697 freemocap-1.1.1/MANIFEST.in
--rw-r--r--   0        0        0     4112 2024-03-18 13:05:20.785697 freemocap-1.1.1/README.md
--rwxr-xr-x   0        0        0      607 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/builds/install_packages
--rwxr-xr-x   0        0        0       66 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/installer.sh
--rwxr-xr-x   0        0        0      278 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/build.sh
--rwxr-xr-x   0        0        0      161 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/run_uvicorn_server.sh
--rwxr-xr-x   0        0        0      381 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/run_web_server.sh
--rwxr-xr-x   0        0        0      118 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/shell.sh
--rwxr-xr-x   0        0        0      104 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/test.sh
--rwxr-xr-x   0        0        0       71 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/linux/up.sh
--rw-r--r--   0        0        0      410 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/windows/installChocolatey.cmd
--rw-r--r--   0        0        0      112 2024-03-18 13:05:20.785697 freemocap-1.1.1/bin/windows/run_web_server.cmd
--rw-r--r--   0        0        0     4783 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/batch_process/batch_process.py
--rw-r--r--   0        0        0     1415 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/batch_process/headless_calibration.py
--rw-r--r--   0        0        0     3495 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/directory_view.py
--rw-r--r--   0        0        0      331 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/freemocap-ui/.gitignore
--rw-r--r--   0        0        0     2358 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/freemocap-ui/README.md
--rw-r--r--   0        0        0      804 2024-03-18 13:05:20.785697 freemocap-1.1.1/experimental/freemocap-ui/config-overrides.js
--rw-r--r--   0        0        0   725486 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2548 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/package.json
--rw-r--r--   0        0        0     3585 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/favicon.ico
--rw-r--r--   0        0        0     1919 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/index.html
--rw-r--r--   0        0        0     4153 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/logo192.png
--rw-r--r--   0        0        0    12066 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/logo512.png
--rw-r--r--   0        0        0      492 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/manifest.json
--rw-r--r--   0        0        0       67 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/public/robots.txt
--rw-r--r--   0        0        0       33 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/scripts/cert.sh
--rw-r--r--   0        0        0      634 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/App.css
--rw-r--r--   0        0        0      383 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/App.test.tsx
--rw-r--r--   0        0        0      210 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/App.tsx
--rw-r--r--   0        0        0      346 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/app/hooks.ts
--rw-r--r--   0        0        0      461 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/app/store.ts
--rw-r--r--   0        0        0     1057 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/components/start-stop-process.tsx
--rw-r--r--   0        0        0      512 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
--rw-r--r--   0        0        0     1159 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
--rw-r--r--   0        0        0      105 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/components/webcam/webcam.tsx
--rw-r--r--   0        0        0      642 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
--rw-r--r--   0        0        0     1383 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/Counter.module.css
--rw-r--r--   0        0        0     2156 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/Counter.tsx
--rw-r--r--   0        0        0      220 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/counterAPI.ts
--rw-r--r--   0        0        0      912 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
--rw-r--r--   0        0        0     3161 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/counterSlice.ts
--rw-r--r--   0        0        0      325 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/hooks/use-device-stream.ts
--rw-r--r--   0        0        0      857 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
--rw-r--r--   0        0        0      376 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/index.css
--rw-r--r--   0        0        0      642 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/index.tsx
--rw-r--r--   0        0        0      461 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/Copyright.tsx
--rw-r--r--   0        0        0     2033 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/Header.tsx
--rw-r--r--   0        0        0     2823 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/Navigator.tsx
--rw-r--r--   0        0        0     5588 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/Paperbase.tsx
--rw-r--r--   0        0        0      440 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
--rw-r--r--   0        0        0      290 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
--rw-r--r--   0        0        0     2398 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/content/Content.tsx
--rw-r--r--   0        0        0      769 2024-03-18 13:05:20.789697 freemocap-1.1.1/experimental/freemocap-ui/src/layout/routing/router.tsx
--rw-r--r--   0        0        0     1160 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/logo.svg
--rw-r--r--   0        0        0       40 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/react-app-env.d.ts
--rw-r--r--   0        0        0     6114 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/serviceWorker.ts
--rw-r--r--   0        0        0      697 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/Capture.tsx
--rw-r--r--   0        0        0      442 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/Record.ts
--rw-r--r--   0        0        0      208 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/cam.ts
--rw-r--r--   0        0        0      341 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/download.ts
--rw-r--r--   0        0        0     1879 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/frame-capture.tsx
--rw-r--r--   0        0        0      519 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/image_send_worker.ts
--rw-r--r--   0        0        0     2252 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/recorder.ts
--rw-r--r--   0        0        0     1563 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/services/supported_recorder.ts
--rw-r--r--   0        0        0      254 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/setupTests.ts
--rw-r--r--   0        0        0     1682 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/Capture.tsx
--rw-r--r--   0        0        0      835 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/Config.tsx
--rw-r--r--   0        0        0     1298 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
--rw-r--r--   0        0        0      121 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/ShowCameras.tsx
--rw-r--r--   0        0        0      129 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/UserConfig.tsx
--rw-r--r--   0        0        0     1090 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
--rw-r--r--   0        0        0      851 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
--rw-r--r--   0        0        0     1090 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
--rw-r--r--   0        0        0     2118 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
--rw-r--r--   0        0        0      599 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/freemocap-ui/tsconfig.json
--rw-r--r--   0        0        0      790 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/python_scratch/qt_drag_and_drop.py
--rw-r--r--   0        0        0        2 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/__init__.py
--rw-r--r--   0        0        0      423 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/app_factory.py
--rw-r--r--   0        0        0       89 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/globals.py
--rw-r--r--   0        0        0      241 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/middleware/cors.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/models/__init__.py
--rw-r--r--   0        0        0      534 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/camera/__init__.py
--rw-r--r--   0        0        0     1034 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/camera/cam_data_ws.py
--rw-r--r--   0        0        0     3135 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/camera/camera_route.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/health/__init__.py
--rw-r--r--   0        0        0      305 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/health/health_check_route.py
--rw-r--r--   0        0        0      209 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/home/home.py
--rw-r--r--   0        0        0     7413 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/session/session_router.py
--rw-r--r--   0        0        0      221 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/routes/startup/startup.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/services/__init__.py
--rw-r--r--   0        0        0      138 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/services/board_detect_service.py
--rw-r--r--   0        0        0       50 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/services/mediapipe_detect_service.py
--rw-r--r--   0        0        0     2021 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/react_fastapi/api/services/user_config.py
--rw-r--r--   0        0        0      315 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/rerun_playground.py
--rw-r--r--   0        0        0     1637 2024-03-18 13:05:20.793697 freemocap-1.1.1/experimental/tool_bar.py
--rw-r--r--   0        0        0   661822 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2776 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/.idea/workspace.xml
--rw-r--r--   0        0        0      693 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/__init__.py
--rw-r--r--   0        0        0      945 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/__main__.py
--rw-r--r--   0        0        0    44734 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/charuco/charuco_board_image.png
--rw-r--r--   0        0        0   332173 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/charuco/charuco_board_image_highRes.png
--rw-r--r--   0        0        0    26593 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/logo/freemocap-logo-black-border.svg
--rw-r--r--   0        0        0   126495 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png
--rw-r--r--   0        0        0   124841 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
--rw-r--r--   0        0        0    99678 2024-03-18 13:05:20.797697 freemocap-1.1.1/freemocap/assets/logo/freemocap_skelly_logo.ico
--rw-r--r--   0        0        0   259115 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/assets/mac_app_files/freemocap.icns
--rw-r--r--   0        0        0     1148 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/assets/mac_app_files/info.plist
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
--rw-r--r--   0        0        0     7091 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
--rw-r--r--   0        0        0    71193 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
--rw-r--r--   0        0        0     2712 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
--rw-r--r--   0        0        0    13416 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
--rw-r--r--   0        0        0      820 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
--rw-r--r--   0        0        0     1163 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
--rw-r--r--   0        0        0     2842 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py
--rw-r--r--   0        0        0     5621 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
--rw-r--r--   0        0        0    14583 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/__init__.py
--rw-r--r--   0        0        0     2251 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py
--rw-r--r--   0        0        0     3368 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py
--rw-r--r--   0        0        0    23381 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/__init__.py
--rw-r--r--   0        0        0     2413 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/__init__.py
--rw-r--r--   0        0        0      151 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/get_numpy_path.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/__init__.py
--rw-r--r--   0        0        0     3024 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py
--rw-r--r--   0        0        0     1716 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py
--rw-r--r--   0        0        0     4670 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py
--rw-r--r--   0        0        0      798 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/__init__.py
--rw-r--r--   0        0        0    57981 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/alpha_freemocap_blender_megascript.py
--rw-r--r--   0        0        0     1091 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/cgtinker_blendarmocap_load.py
--rw-r--r--   0        0        0    42906 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/freemocap_blender_megascript_take2.py
--rw-r--r--   0        0        0     1804 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/run_alpha_megascript.py
--rw-r--r--   0        0        0     1790 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/run_cgtinker_method.py
--rw-r--r--   0        0        0     2511 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/run_megascript_take2.py
--rw-r--r--   0        0        0     3245 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/generate_jupyter_notebook/__init__.py
--rw-r--r--   0        0        0    10465 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb
--rw-r--r--   0        0        0     1089 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.801697 freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/__init__.py
--rw-r--r--   0        0        0    13879 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py
--rw-r--r--   0        0        0     6235 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py
--rw-r--r--   0        0        0     4240 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py
--rw-r--r--   0        0        0     1654 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/__init__.py
--rw-r--r--   0        0        0     6040 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
--rw-r--r--   0        0        0     4207 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py
--rw-r--r--   0        0        0     2583 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py
--rw-r--r--   0        0        0     2891 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py
--rw-r--r--   0        0        0     3482 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py
--rw-r--r--   0        0        0     2041 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py
--rw-r--r--   0        0        0     5670 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/data_saver/__init__.py
--rw-r--r--   0        0        0     9165 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/data_saver/data_loader.py
--rw-r--r--   0        0        0     4852 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/data_saver/data_models.py
--rw-r--r--   0        0        0     4193 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/data_saver/data_saver.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/generate_jupyter_notebook/__init__.py
--rw-r--r--   0        0        0    10465 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb
--rw-r--r--   0        0        0     1089 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/recording_models/__init__.py
--rw-r--r--   0        0        0     1473 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/recording_models/post_processing_parameter_models.py
--rw-r--r--   0        0        0    10773 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/data_layer/recording_models/recording_info_model.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/actions_and_menus/__init__.py
--rw-r--r--   0        0        0     5493 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/actions_and_menus/actions.py
--rw-r--r--   0        0        0     2717 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/actions_and_menus/menu_bar.py
--rw-r--r--   0        0        0     2129 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/freemocap_main.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/main_window/__init__.py
--rw-r--r--   0        0        0    25383 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/main_window/freemocap_main_window.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/__init__.py
--rw-r--r--   0        0        0      362 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
--rw-r--r--   0        0        0     1325 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/css_file_watcher.py
--rw-r--r--   0        0        0     3905 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/qt_style_sheet.css
--rw-r--r--   0        0        0     5105 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
--rw-r--r--   0        0        0     1500 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/scss_file_watcher.py
--rw-r--r--   0        0        0      305 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/__init__.py
--rw-r--r--   0        0        0     1850 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/colors.py
--rw-r--r--   0        0        0     1127 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/copy_timestamps_folder.py
--rw-r--r--   0        0        0      194 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/get_qt_app.py
--rw-r--r--   0        0        0      693 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/save_and_load_gui_state.py
--rw-r--r--   0        0        0      864 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0     6876 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/active_recording_widget.py
--rw-r--r--   0        0        0    11878 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/camera_controller_group_box.py
--rw-r--r--   0        0        0     3728 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/central_tab_widget.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/__init__.py
--rw-r--r--   0        0        0    14844 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
--rw-r--r--   0        0        0     1924 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
--rw-r--r--   0        0        0     5237 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
--rw-r--r--   0        0        0    10941 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
--rw-r--r--   0        0        0    12727 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
--rw-r--r--   0        0        0     2316 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel_dock_widget.py
--rw-r--r--   0        0        0     6618 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/directory_view_widget.py
--rw-r--r--   0        0        0     7903 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/home_widget.py
--rw-r--r--   0        0        0    10889 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/import_videos_wizard.py
--rw-r--r--   0        0        0     3089 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/jupyter_console_widget.py
--rw-r--r--   0        0        0     7817 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/log_view_widget.py
--rw-r--r--   0        0        0      415 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/logo_svg_widget.py
--rw-r--r--   0        0        0     3864 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/opencv_conflict_dialog.py
--rw-r--r--   0        0        0     3931 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/widgets/welcome_screen_dialog.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/__init__.py
--rw-r--r--   0        0        0     2380 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
--rw-r--r--   0        0        0     1269 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/download_sample_data_thread_worker.py
--rw-r--r--   0        0        0     1726 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/export_to_blender_thread_worker.py
--rw-r--r--   0        0        0     2793 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
--rw-r--r--   0        0        0     2791 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/logging/__init__.py
--rw-r--r--   0        0        0     7505 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/logging/configure_logging.py
--rw-r--r--   0        0        0      256 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/logging/queue_logger.py
--rw-r--r--   0        0        0      259 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/open_file.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/paths_and_filenames/__init__.py
--rw-r--r--   0        0        0     3286 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/paths_and_filenames/file_and_folder_names.py
--rw-r--r--   0        0        0    11618 2024-03-18 13:05:20.805697 freemocap-1.1.1/freemocap/system/paths_and_filenames/path_getters.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/system/user_data/__init__.py
--rw-r--r--   0        0        0      957 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/system/user_data/pipedream_pings.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/__init__.py
--rw-r--r--   0        0        0     1982 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/conftest.py
--rw-r--r--   0        0        0     3685 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_by_camera_reprojection_filtering.py
--rw-r--r--   0        0        0     3151 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_geometry_utilities.py
--rw-r--r--   0        0        0     2126 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_image_tracking_data_shape.py
--rw-r--r--   0        0        0     2396 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_mediapipe_skeleton_data_shape.py
--rw-r--r--   0        0        0      925 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_synchronized_video_frame_counts.py
--rw-r--r--   0        0        0     1359 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/tests/test_total_body_center_of_mass_data_shape.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/__init__.py
--rw-r--r--   0        0        0     1268 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/create_nested_dict_from_pydantic.py
--rw-r--r--   0        0        0     2015 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/download_sample_data.py
--rw-r--r--   0        0        0     1022 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/fix_opencv_conflict.py
--rw-r--r--   0        0        0        0 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/geometry/__init__.py
--rw-r--r--   0        0        0      446 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/geometry/project_3d_data_to_z_plane.py
--rw-r--r--   0        0        0      631 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py
--rw-r--r--   0        0        0      742 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0      691 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/get_video_paths.py
--rw-r--r--   0        0        0      111 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/kill_event_exception.py
--rw-r--r--   0        0        0      708 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/remove_empty_directories.py
--rw-r--r--   0        0        0      486 2024-03-18 13:05:20.809697 freemocap-1.1.1/freemocap/utilities/save_dictionary_to_json.py
--rw-r--r--   0        0        0    25394 2024-03-18 13:05:20.809697 freemocap-1.1.1/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb
--rw-r--r--   0        0        0     5252 2024-03-18 13:05:20.809697 freemocap-1.1.1/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
--rw-r--r--   0        0        0    21821 2024-03-18 13:05:20.809697 freemocap-1.1.1/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
--rw-r--r--   0        0        0    13464 2024-03-18 13:05:20.809697 freemocap-1.1.1/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
--rw-r--r--   0        0        0      690 2024-03-18 13:05:20.809697 freemocap-1.1.1/noxfile.py
--rw-r--r--   0        0        0     1748 2024-03-18 13:05:20.809697 freemocap-1.1.1/poetry_pyproject.toml
--rw-r--r--   0        0        0     3929 2024-03-18 13:05:20.809697 freemocap-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       50 2024-03-18 13:05:20.809697 freemocap-1.1.1/setup.py
--rw-r--r--   0        0        0     7306 1970-01-01 00:00:00.000000 freemocap-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1649 2024-04-29 19:29:24.857720 freemocap-1.2.0/.flake8
+-rwxr-xr-x   0        0        0      492 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      423 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      730 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/coverage-testing.yml
+-rw-r--r--   0        0        0     1138 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/flit_publish_to_pypi.yml
+-rwxr-xr-x   0        0        0      385 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/linting-flake8.yml
+-rw-r--r--   0        0        0     2049 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/linux_installer.yml
+-rw-r--r--   0        0        0     2613 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/mac_installer.yml
+-rw-r--r--   0        0        0     1246 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/publish_to_pypi.yml
+-rwxr-xr-x   0        0        0     1018 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/python-testing.yml
+-rwxr-xr-x   0        0        0      733 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/version-testing.yml
+-rw-r--r--   0        0        0     2312 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/windows_installer.yml
+-rw-r--r--   0        0        0     2043 2024-04-29 19:29:24.857720 freemocap-1.2.0/.gitignore
+-rw-r--r--   0        0        0      229 2024-04-29 19:29:24.857720 freemocap-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      657 2024-04-29 19:29:24.857720 freemocap-1.2.0/CITATION.cff
+-rw-r--r--   0        0        0      327 2024-04-29 19:29:24.857720 freemocap-1.2.0/CODEOWNERS
+-rw-r--r--   0        0        0     1513 2024-04-29 19:29:24.857720 freemocap-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3552 2024-04-29 19:29:24.857720 freemocap-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2024-04-29 19:29:24.857720 freemocap-1.2.0/LICENSE
+-rw-r--r--   0        0        0      234 2024-04-29 19:29:24.857720 freemocap-1.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     4112 2024-04-29 19:29:24.857720 freemocap-1.2.0/README.md
+-rwxr-xr-x   0        0        0      607 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/builds/install_packages
+-rwxr-xr-x   0        0        0       66 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/installer.sh
+-rwxr-xr-x   0        0        0      278 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/build.sh
+-rwxr-xr-x   0        0        0      161 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/run_uvicorn_server.sh
+-rwxr-xr-x   0        0        0      381 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/run_web_server.sh
+-rwxr-xr-x   0        0        0      118 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/shell.sh
+-rwxr-xr-x   0        0        0      104 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/test.sh
+-rwxr-xr-x   0        0        0       71 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/up.sh
+-rw-r--r--   0        0        0      410 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/windows/installChocolatey.cmd
+-rw-r--r--   0        0        0      112 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/windows/run_web_server.cmd
+-rw-r--r--   0        0        0     4783 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/batch_process/batch_process.py
+-rw-r--r--   0        0        0     1415 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/batch_process/headless_calibration.py
+-rw-r--r--   0        0        0     3495 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/directory_view.py
+-rw-r--r--   0        0        0      331 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/.gitignore
+-rw-r--r--   0        0        0     2358 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/README.md
+-rw-r--r--   0        0        0      804 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/config-overrides.js
+-rw-r--r--   0        0        0   725486 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2548 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/package.json
+-rw-r--r--   0        0        0     3585 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/favicon.ico
+-rw-r--r--   0        0        0     1919 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/index.html
+-rw-r--r--   0        0        0     4153 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/logo192.png
+-rw-r--r--   0        0        0    12066 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/logo512.png
+-rw-r--r--   0        0        0      492 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/robots.txt
+-rw-r--r--   0        0        0       33 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/scripts/cert.sh
+-rw-r--r--   0        0        0      634 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.css
+-rw-r--r--   0        0        0      383 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.test.tsx
+-rw-r--r--   0        0        0      210 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.tsx
+-rw-r--r--   0        0        0      346 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/app/hooks.ts
+-rw-r--r--   0        0        0      461 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/app/store.ts
+-rw-r--r--   0        0        0     1057 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/start-stop-process.tsx
+-rw-r--r--   0        0        0      512 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
+-rw-r--r--   0        0        0     1159 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
+-rw-r--r--   0        0        0      105 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
+-rw-r--r--   0        0        0      642 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
+-rw-r--r--   0        0        0     1383 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.module.css
+-rw-r--r--   0        0        0     2156 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.tsx
+-rw-r--r--   0        0        0      220 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
+-rw-r--r--   0        0        0      912 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
+-rw-r--r--   0        0        0     3161 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
+-rw-r--r--   0        0        0      325 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
+-rw-r--r--   0        0        0      857 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
+-rw-r--r--   0        0        0      376 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/index.css
+-rw-r--r--   0        0        0      642 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/index.tsx
+-rw-r--r--   0        0        0      461 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Copyright.tsx
+-rw-r--r--   0        0        0     2033 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Header.tsx
+-rw-r--r--   0        0        0     2823 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Navigator.tsx
+-rw-r--r--   0        0        0     5588 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Paperbase.tsx
+-rw-r--r--   0        0        0      440 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
+-rw-r--r--   0        0        0      290 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
+-rw-r--r--   0        0        0     2398 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/Content.tsx
+-rw-r--r--   0        0        0      769 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/routing/router.tsx
+-rw-r--r--   0        0        0     1160 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/react-app-env.d.ts
+-rw-r--r--   0        0        0     6114 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/serviceWorker.ts
+-rw-r--r--   0        0        0      697 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/Capture.tsx
+-rw-r--r--   0        0        0      442 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/Record.ts
+-rw-r--r--   0        0        0      208 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/cam.ts
+-rw-r--r--   0        0        0      341 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/download.ts
+-rw-r--r--   0        0        0     1879 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/frame-capture.tsx
+-rw-r--r--   0        0        0      519 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/image_send_worker.ts
+-rw-r--r--   0        0        0     2252 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/recorder.ts
+-rw-r--r--   0        0        0     1563 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/supported_recorder.ts
+-rw-r--r--   0        0        0      254 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/setupTests.ts
+-rw-r--r--   0        0        0     1682 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/Capture.tsx
+-rw-r--r--   0        0        0      835 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/Config.tsx
+-rw-r--r--   0        0        0     1298 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
+-rw-r--r--   0        0        0      121 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/ShowCameras.tsx
+-rw-r--r--   0        0        0      129 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/UserConfig.tsx
+-rw-r--r--   0        0        0     1090 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
+-rw-r--r--   0        0        0      851 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
+-rw-r--r--   0        0        0     1090 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
+-rw-r--r--   0        0        0     2118 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
+-rw-r--r--   0        0        0      599 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/tsconfig.json
+-rw-r--r--   0        0        0      790 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/python_scratch/qt_drag_and_drop.py
+-rw-r--r--   0        0        0        2 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/app_factory.py
+-rw-r--r--   0        0        0       89 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/globals.py
+-rw-r--r--   0        0        0      241 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/middleware/cors.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/models/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/cam_data_ws.py
+-rw-r--r--   0        0        0     3135 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/camera_route.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/health/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/health/health_check_route.py
+-rw-r--r--   0        0        0      209 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/home/home.py
+-rw-r--r--   0        0        0     7413 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/session/session_router.py
+-rw-r--r--   0        0        0      221 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/startup/startup.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/board_detect_service.py
+-rw-r--r--   0        0        0       50 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/mediapipe_detect_service.py
+-rw-r--r--   0        0        0     2021 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/user_config.py
+-rw-r--r--   0        0        0      315 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/rerun_playground.py
+-rw-r--r--   0        0        0     1637 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/tool_bar.py
+-rw-r--r--   0        0        0   661822 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2776 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/.idea/workspace.xml
+-rw-r--r--   0        0        0      693 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/__init__.py
+-rw-r--r--   0        0        0      945 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/__main__.py
+-rw-r--r--   0        0        0    44734 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.png
+-rw-r--r--   0        0        0     2948 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.svg
+-rw-r--r--   0        0        0   332173 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image_highRes.png
+-rw-r--r--   0        0        0    26593 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-logo-black-border.svg
+-rw-r--r--   0        0        0   126495 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png
+-rw-r--r--   0        0        0   124841 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
+-rw-r--r--   0        0        0    99678 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap_skelly_logo.ico
+-rw-r--r--   0        0        0   259115 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/assets/mac_app_files/freemocap.icns
+-rw-r--r--   0        0        0     1148 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/assets/mac_app_files/info.plist
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
+-rw-r--r--   0        0        0     7091 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
+-rw-r--r--   0        0        0    71193 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
+-rw-r--r--   0        0        0     2712 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
+-rw-r--r--   0        0        0    13416 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
+-rw-r--r--   0        0        0      820 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
+-rw-r--r--   0        0        0     1163 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
+-rw-r--r--   0        0        0     2842 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py
+-rw-r--r--   0        0        0     5621 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
+-rw-r--r--   0        0        0    14583 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/__init__.py
+-rw-r--r--   0        0        0     2251 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py
+-rw-r--r--   0        0        0     3368 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py
+-rw-r--r--   0        0        0    23381 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/get_numpy_path.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/__init__.py
+-rw-r--r--   0        0        0     3024 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py
+-rw-r--r--   0        0        0     1709 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py
+-rw-r--r--   0        0        0     6781 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py
+-rw-r--r--   0        0        0      791 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py
+-rw-r--r--   0        0        0     3076 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/__init__.py
+-rw-r--r--   0        0        0    10465 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb
+-rw-r--r--   0        0        0     1089 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/__init__.py
+-rw-r--r--   0        0        0    13879 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py
+-rw-r--r--   0        0        0     4240 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py
+-rw-r--r--   0        0        0     1654 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/__init__.py
+-rw-r--r--   0        0        0     5952 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
+-rw-r--r--   0        0        0     4207 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py
+-rw-r--r--   0        0        0     1674 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py
+-rw-r--r--   0        0        0     2617 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py
+-rw-r--r--   0        0        0     3482 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py
+-rw-r--r--   0        0        0     2041 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py
+-rw-r--r--   0        0        0     5670 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/__init__.py
+-rw-r--r--   0        0        0     9173 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_loader.py
+-rw-r--r--   0        0        0     4854 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_models.py
+-rw-r--r--   0        0        0     4195 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_saver.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/__init__.py
+-rw-r--r--   0        0        0    10465 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb
+-rw-r--r--   0        0        0     1089 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/post_processing_parameter_models.py
+-rw-r--r--   0        0        0    10940 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/recording_info_model.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/__init__.py
+-rw-r--r--   0        0        0     5822 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/actions.py
+-rw-r--r--   0        0        0     2777 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/menu_bar.py
+-rw-r--r--   0        0        0     2129 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/freemocap_main.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/main_window/__init__.py
+-rw-r--r--   0        0        0    25937 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/main_window/freemocap_main_window.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
+-rw-r--r--   0        0        0     1325 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/css_file_watcher.py
+-rw-r--r--   0        0        0     3905 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.css
+-rw-r--r--   0        0        0     5105 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
+-rw-r--r--   0        0        0     1500 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
+-rw-r--r--   0        0        0      305 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/colors.py
+-rw-r--r--   0        0        0     1127 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/copy_timestamps_folder.py
+-rw-r--r--   0        0        0      194 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/get_qt_app.py
+-rw-r--r--   0        0        0     1105 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/save_and_load_gui_state.py
+-rw-r--r--   0        0        0      864 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     7141 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/active_recording_widget.py
+-rw-r--r--   0        0        0    11878 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/camera_controller_group_box.py
+-rw-r--r--   0        0        0     3728 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/central_tab_widget.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/__init__.py
+-rw-r--r--   0        0        0    14844 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
+-rw-r--r--   0        0        0     1924 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     3636 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
+-rw-r--r--   0        0        0    13078 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
+-rw-r--r--   0        0        0    12727 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
+-rw-r--r--   0        0        0     2316 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     6771 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/directory_view_widget.py
+-rw-r--r--   0        0        0     7903 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/home_widget.py
+-rw-r--r--   0        0        0    10889 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/import_videos_wizard.py
+-rw-r--r--   0        0        0     3089 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/jupyter_console_widget.py
+-rw-r--r--   0        0        0     7817 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/log_view_widget.py
+-rw-r--r--   0        0        0      415 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/logo_svg_widget.py
+-rw-r--r--   0        0        0     3864 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/opencv_conflict_dialog.py
+-rw-r--r--   0        0        0     2701 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/set_data_folder_dialog.py
+-rw-r--r--   0        0        0     3989 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/welcome_screen_dialog.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/__init__.py
+-rw-r--r--   0        0        0     2380 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
+-rw-r--r--   0        0        0     1269 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/download_sample_data_thread_worker.py
+-rw-r--r--   0        0        0     1654 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/export_to_blender_thread_worker.py
+-rw-r--r--   0        0        0     2793 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
+-rw-r--r--   0        0        0     2791 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/__init__.py
+-rw-r--r--   0        0        0     7505 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/configure_logging.py
+-rw-r--r--   0        0        0      256 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/queue_logger.py
+-rw-r--r--   0        0        0      259 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/open_file.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/__init__.py
+-rw-r--r--   0        0        0     3347 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/file_and_folder_names.py
+-rw-r--r--   0        0        0    12662 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/path_getters.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/user_data/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/user_data/pipedream_pings.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/conftest.py
+-rw-r--r--   0        0        0     3685 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_by_camera_reprojection_filtering.py
+-rw-r--r--   0        0        0     3151 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_geometry_utilities.py
+-rw-r--r--   0        0        0     2145 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_image_tracking_data_shape.py
+-rw-r--r--   0        0        0     2415 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_mediapipe_skeleton_data_shape.py
+-rw-r--r--   0        0        0      943 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_synchronized_video_frame_counts.py
+-rw-r--r--   0        0        0     1378 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/__init__.py
+-rw-r--r--   0        0        0     1268 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/create_nested_dict_from_pydantic.py
+-rw-r--r--   0        0        0     2450 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/download_sample_data.py
+-rw-r--r--   0        0        0     1022 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/fix_opencv_conflict.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/__init__.py
+-rw-r--r--   0        0        0      446 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/project_3d_data_to_z_plane.py
+-rw-r--r--   0        0        0      631 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py
+-rw-r--r--   0        0        0      813 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0      691 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/get_video_paths.py
+-rw-r--r--   0        0        0      111 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/kill_event_exception.py
+-rw-r--r--   0        0        0      708 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/remove_empty_directories.py
+-rw-r--r--   0        0        0      486 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/save_dictionary_to_json.py
+-rw-r--r--   0        0        0    25394 2024-04-29 19:29:24.877720 freemocap-1.2.0/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb
+-rw-r--r--   0        0        0     5252 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
+-rw-r--r--   0        0        0    21821 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
+-rw-r--r--   0        0        0    13464 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
+-rw-r--r--   0        0        0      690 2024-04-29 19:29:24.881720 freemocap-1.2.0/noxfile.py
+-rw-r--r--   0        0        0     1748 2024-04-29 19:29:24.881720 freemocap-1.2.0/poetry_pyproject.toml
+-rw-r--r--   0        0        0     3930 2024-04-29 19:29:24.881720 freemocap-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-29 19:29:24.881720 freemocap-1.2.0/setup.py
+-rw-r--r--   0        0        0     7307 1970-01-01 00:00:00.000000 freemocap-1.2.0/PKG-INFO
```

### Comparing `freemocap-1.1.1/.flake8` & `freemocap-1.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/coverage-testing.yml` & `freemocap-1.2.0/.github/workflows/coverage-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/flit_publish_to_pypi.yml` & `freemocap-1.2.0/.github/workflows/flit_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/linux_installer.yml` & `freemocap-1.2.0/.github/workflows/linux_installer.yml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       - name: Unzip PyApp
         run: |
           unzip pyapp.zip
       - name: Create Linux Installer
         run: |
           cd ${{ github.workspace }}/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.1.1
+          export PYAPP_PROJECT_VERSION=v1.2.0
           export PYAPP_PROJECT_DEPENDENCY_FILE=${{ github.workspace }}/requirements.txt
           export PYAPP_EXEC_SCRIPT=${{ github.workspace }}/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root ${{ github.workspace }}
           cd ${{ github.workspace }}
           mv ${{ github.workspace }}/bin/pyapp freemocap_app && chmod +x freemocap_app
```

### Comparing `freemocap-1.1.1/.github/workflows/mac_installer.yml` & `freemocap-1.2.0/.github/workflows/mac_installer.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
       - name: Unzip PyApp
         run: |
           unzip pyapp.zip
       - name: Create Mac Installer
         run: |
           cd ${{ github.workspace }}/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.1.1
+          export PYAPP_PROJECT_VERSION=v1.2.0
           export PYAPP_PROJECT_DEPENDENCY_FILE=${{ github.workspace }}/requirements.txt
           export PYAPP_EXEC_SCRIPT=${{ github.workspace }}/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root ${{ github.workspace }}
           cd ${{ github.workspace }}
           mv ${{ github.workspace }}/bin/pyapp freemocap_app
```

### Comparing `freemocap-1.1.1/.github/workflows/publish_to_pypi.yml` & `freemocap-1.2.0/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/python-testing.yml` & `freemocap-1.2.0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/version-testing.yml` & `freemocap-1.2.0/.github/workflows/version-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/.github/workflows/windows_installer.yml` & `freemocap-1.2.0/.github/workflows/windows_installer.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           ls -la
         shell: bash
       - name: Create Windows Installer
         run: |
           WORKSPACE=$(cygpath -u "${{ github.workspace}}")
           cd $WORKSPACE/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.1.1
+          export PYAPP_PROJECT_VERSION=v1.2.0
           export PYAPP_PROJECT_DEPENDENCY_FILE=$WORKSPACE/requirements.txt
           export PYAPP_EXEC_SCRIPT=$WORKSPACE/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root $WORKSPACE
           cd $WORKSPACE
           mv $WORKSPACE/bin/pyapp freemocap_app.exe
```

### Comparing `freemocap-1.1.1/.gitignore` & `freemocap-1.2.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -150,7 +150,8 @@
 
 
 .DS_Store
 
 desktop.ini
 
 node_modules/
+freemocap/system/gui_state.json
```

### Comparing `freemocap-1.1.1/CITATION.cff` & `freemocap-1.2.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/CODE_OF_CONDUCT.md` & `freemocap-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/CONTRIBUTING.md` & `freemocap-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/LICENSE` & `freemocap-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/README.md` & `freemocap-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/bin/builds/install_packages` & `freemocap-1.2.0/bin/builds/install_packages`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/batch_process/batch_process.py` & `freemocap-1.2.0/experimental/batch_process/batch_process.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/batch_process/headless_calibration.py` & `freemocap-1.2.0/experimental/batch_process/headless_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/directory_view.py` & `freemocap-1.2.0/experimental/directory_view.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/README.md` & `freemocap-1.2.0/experimental/freemocap-ui/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/config-overrides.js` & `freemocap-1.2.0/experimental/freemocap-ui/config-overrides.js`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/package-lock.json` & `freemocap-1.2.0/experimental/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/package.json` & `freemocap-1.2.0/experimental/freemocap-ui/package.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/public/favicon.ico` & `freemocap-1.2.0/experimental/freemocap-ui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/public/index.html` & `freemocap-1.2.0/experimental/freemocap-ui/public/index.html`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/public/logo192.png` & `freemocap-1.2.0/experimental/freemocap-ui/public/logo192.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/public/logo512.png` & `freemocap-1.2.0/experimental/freemocap-ui/public/logo512.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/App.css` & `freemocap-1.2.0/experimental/freemocap-ui/src/App.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/components/start-stop-process.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/components/start-stop-process.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/Counter.module.css` & `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.module.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/Counter.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/features/counter/counterSlice.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/index.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/layout/Header.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Header.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/layout/Navigator.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Navigator.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/layout/Paperbase.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Paperbase.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/layout/content/Content.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/Content.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/layout/routing/router.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/layout/routing/router.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/logo.svg` & `freemocap-1.2.0/experimental/freemocap-ui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/serviceWorker.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/serviceWorker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/services/Capture.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/services/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/services/frame-capture.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/services/frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/services/image_send_worker.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/services/image_send_worker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/services/recorder.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/services/recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/services/supported_recorder.ts` & `freemocap-1.2.0/experimental/freemocap-ui/src/services/supported_recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/Capture.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/Config.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/Config.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/SessionWorkflow.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx` & `freemocap-1.2.0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/freemocap-ui/tsconfig.json` & `freemocap-1.2.0/experimental/freemocap-ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/python_scratch/qt_drag_and_drop.py` & `freemocap-1.2.0/experimental/python_scratch/qt_drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/react_fastapi/api/routes/__init__.py` & `freemocap-1.2.0/experimental/react_fastapi/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/react_fastapi/api/routes/camera/cam_data_ws.py` & `freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/cam_data_ws.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/react_fastapi/api/routes/camera/camera_route.py` & `freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/camera_route.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/react_fastapi/api/routes/session/session_router.py` & `freemocap-1.2.0/experimental/react_fastapi/api/routes/session/session_router.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/react_fastapi/api/services/user_config.py` & `freemocap-1.2.0/experimental/react_fastapi/api/services/user_config.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/experimental/tool_bar.py` & `freemocap-1.2.0/experimental/tool_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap-ui/package-lock.json` & `freemocap-1.2.0/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/.idea/workspace.xml` & `freemocap-1.2.0/freemocap/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/__init__.py` & `freemocap-1.2.0/freemocap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A free and open source markerless motion capture system for everyone 💀✨"""
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v1.1.1"
+__version__ = "v1.2.0"
 __description__ = "A free and open source markerless motion capture system for everyone 💀✨"
 
 __package_name__ = "freemocap"
 __repo_url__ = f"https://github.com/freemocap/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
 
 from freemocap.system.logging.configure_logging import configure_logging, LogLevel
```

### Comparing `freemocap-1.1.1/freemocap/__main__.py` & `freemocap-1.2.0/freemocap/__main__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/charuco/charuco_board_image.png` & `freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/charuco/charuco_board_image_highRes.png` & `freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image_highRes.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/logo/freemocap-logo-black-border.svg` & `freemocap-1.2.0/freemocap/assets/logo/freemocap-logo-black-border.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png` & `freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png` & `freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/logo/freemocap_skelly_logo.ico` & `freemocap-1.2.0/freemocap/assets/logo/freemocap_skelly_logo.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/mac_app_files/freemocap.icns` & `freemocap-1.2.0/freemocap/assets/mac_app_files/freemocap.icns`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/assets/mac_app_files/info.plist` & `freemocap-1.2.0/freemocap/assets/mac_app_files/info.plist`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py` & `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py` & `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py` & `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py` & `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py` & `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py` & `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py` & `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import subprocess
 from importlib.metadata import distribution
 from pathlib import Path
 
-from ajc27_freemocap_blender_addon.run_as_main import ajc27_run_as_main_function
+from ajc27_freemocap_blender_addon.main import ajc27_run_as_main_function
 
 from freemocap.core_processes.export_data.blender_stuff.export_to_blender.methods.ajc_addon.install.bpy_install_addon import (
     INSTALL_ADDON_SCRIPT_PATH,
 )
 
 FREEMOCAP_BLENDER_ADDON_PACKAGE_NAME = "ajc27_freemocap_blender_addon"
```

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py` & `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 
 def run_simple(recording_path_input: str, blender_file_save_path_input: str):
-    from ajc27_freemocap_blender_addon.run_as_main import ajc27_run_as_main_function
+    from ajc27_freemocap_blender_addon.main import ajc27_run_as_main_function
 
     ajc27_run_as_main_function(recording_path=str(recording_path_input),
                                blend_file_path=str(blender_file_save_path_input))
 
 
 if __name__ == "__main__":
     print(f"\n\n\n\nRunning {__file__} as a subprocess to install the addon...\n\n\n")
```

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/legacy/run_cgtinker_method.py` & `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,90 @@
 import logging
-import subprocess
+import platform
 from pathlib import Path
-from typing import Union
+from typing import Union, Optional
 
 logger = logging.getLogger(__name__)
 
 
-def run_cgtinker_method(
-    recording_folder_path: Union[str, Path],
-    blender_file_path: Union[str, Path],
-    blender_exe_path: Union[str, Path],
-):
-    path_to_this_py_file = Path(__file__).parent.resolve()
-
-    blender_script_path = path_to_this_py_file / "cgtinker_blendarmocap_load.py"
-
-    # freemocap_blender_megascript_path = (
-    #     path_to_this_py_file / "freemocap_blender_megascript_take2.py"
-    # )
-
+def guess_blender_exe_path_from_path(base_path: Union[str, Path]) -> Optional[Path]:
+    base_path = Path(base_path)
     try:
-        blender_exe_path = Path(blender_exe_path)
-        if not blender_exe_path.exists():
-            raise FileNotFoundError(f"Could not find the blender executable at {blender_exe_path}")
-    except Exception as e:
-        logger.error(e)
+        blender_folder_paths = [path for path in base_path.rglob("blender.exe")]
+    except OSError:
+        logger.info(f"Unable to access: {str(base_path)}")
         return
 
-    command_list = [
-        str(blender_exe_path),
-        "--background",
-        "--python",
-        str(blender_script_path),
-        "--",
-        str(recording_folder_path),
-        str(blender_file_path),
-        "1",  # bind to rig
-        "1",  # load synchronized_videos
-        "9999",  # timeout
-        "0",  # load raw data
-        "1,",  # load quick
-    ]
-
-    logger.info(f"Starting `blender` sub-process with this command: \n {command_list}")
-
-    blender_process = subprocess.Popen(command_list, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    while True:
-        output = blender_process.stdout.readline()
-        if blender_process.poll() is not None:
-            break
-        if output:
-            print(output.strip().decode())
-
-    if blender_process.returncode == 0:
-        logger.error("Blender returned an error:")
-        logger.error(blender_process.stderr.read().decode())
-    logger.debug("Done with cgtinker Blender Export")
+    if blender_folder_paths:
+
+        if len(blender_folder_paths) == 0:
+            return None
+
+        best_guess = blender_folder_paths[-1]
+
+        return best_guess
+
+
+def get_best_guess_of_blender_path():
+    if platform.system() == "Windows":
+        # check all lettered drives and the user's home directory
+        paths_to_check = [
+            Path(f"{letter}:/Program Files/Blender Foundation") for letter in "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+        ]
+
+        paths_to_check.append(Path.home() / "Blender Foundation")
+
+        for base_path in paths_to_check:
+            blender_exe_path = guess_blender_exe_path_from_path(base_path)
+            if blender_exe_path is not None and blender_exe_path.is_file():
+                logger.info(f"Found `blender.exe` at: {str(blender_exe_path)}")
+
+                return str(blender_exe_path)
+        else:
+            logger.warning(
+                "Could not find `blender.exe` in the expected locations. Please locate it manually (or install Blender, if it isn't installed)."
+            )
+            return None
+
+    if platform.system() == "Darwin":
+        blender_app_path = Path("/Applications/Blender.app")
+
+        if blender_app_path.exists():
+            logger.info(f"Mac machine detected - guessing that `blender` is installed at: {str(blender_app_path)}")
+
+            blender_exe_path = blender_app_path / "Contents/MacOS/Blender"
+            return str(blender_exe_path)
+        else:
+            logger.warning(
+                "Could not find Blender executable in the applications folder. Please locate it manually (or install Blender, if it isn't installed)."
+            )
+            return None
+
+    if platform.system() == "Linux":
+        blender_path_list = [
+            Path("/usr/bin"),
+            Path("/usr/sbin"),
+            Path("/usr/local/bin"),
+            Path("/usr/local/sbin"),
+            Path("/bin"),
+            Path("/sbin"),
+            Path("/snap/bin"),
+        ]
+        for path in blender_path_list:
+            blender_path = path / "blender"
+            if blender_path.exists():
+                logger.info(f"Linux machine detected - guessing that `blender` is installed at: {str(blender_path)}")
+
+                return str(blender_path)
+
+        logger.info(
+            "Could not find Blender executable in bin. Please locate it manually (or install Blender, if it isn't installed)."
+        )
+        return None
+
+    else:
+        logger.info("Machine system not detected, please locate Blender path manually.")
+        return None
+
+
+if __name__ == "__main__":
+    print(f" blender path: {get_best_guess_of_blender_path()}")
```

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb` & `freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py` & `freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py` & `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py` & `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py` & `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,13 @@
         raise exception
 
     # TODO: deprecate save_data function in favor of DataSaver
     save_data(
         skel3d_frame_marker_xyz=skel3d_frame_marker_xyz,
         segment_COM_frame_imgPoint_XYZ=anatomical_data_dict["segment_COM"],
         totalBodyCOM_frame_XYZ=anatomical_data_dict["total_body_COM"],
-        skeleton_segment_lengths_dict=anatomical_data_dict["skeleton_segment_lengths"],
         processing_parameters=recording_processing_parameter_model,
         queue=logging_queue,
     )
     DataSaver(recording_folder_path=recording_processing_parameter_model.recording_info_model.path).save_all()
 
     logger.info(f"Done processing {recording_processing_parameter_model.recording_info_model.path}")
```

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import logging
 import multiprocessing
 from pathlib import Path
-from typing import Dict
 import numpy as np
-import pandas as pd
-from freemocap.core_processes.detecting_things_in_2d_images.mediapipe_stuff.convert_mediapipe_npy_to_csv import (
-    convert_mediapipe_npy_to_csv,
-)
 
-from freemocap.core_processes.post_process_skeleton_data.estimate_skeleton_segment_lengths import (
-    estimate_skeleton_segment_lengths,
-    mediapipe_skeleton_segment_definitions,
+
+from freemocap.core_processes.post_process_skeleton_data.post_process_skeleton import save_numpy_array_to_disk
+from freemocap.core_processes.detecting_things_in_2d_images.mediapipe_stuff.data_models.mediapipe_skeleton_names_and_connections import (
+    mediapipe_names_and_connections_dict,
 )
-from freemocap.core_processes.post_process_skeleton_data.calculate_center_of_mass import run_center_of_mass_calculations
 from freemocap.data_layer.recording_models.post_processing_parameter_models import ProcessingParameterModel
 from freemocap.system.logging.queue_logger import DirectQueueHandler
-from freemocap.system.paths_and_filenames.file_and_folder_names import MEDIAPIPE_BODY_3D_DATAFRAME_CSV_FILE_NAME
 from freemocap.system.logging.configure_logging import log_view_logging_format_string
+from freemocap.system.paths_and_filenames.file_and_folder_names import (
+    CENTER_OF_MASS_FOLDER_NAME,
+    SEGMENT_CENTER_OF_MASS_NPY_FILE_NAME,
+    TOTAL_BODY_CENTER_OF_MASS_NPY_FILE_NAME,
+)
+from freemocap.utilities.save_dictionary_to_json import save_dictionary_to_json
+
 
 logger = logging.getLogger(__name__)
 
 
-def calculate_anatomical_data(
-    processing_parameters: ProcessingParameterModel,
+def save_data(
     skel3d_frame_marker_xyz: np.ndarray,
+    segment_COM_frame_imgPoint_XYZ: np.ndarray,
+    totalBodyCOM_frame_XYZ: np.ndarray,
+    processing_parameters: ProcessingParameterModel,
     queue: multiprocessing.Queue,
-) -> Dict[str, np.ndarray]:
+):
     if queue:
         handler = DirectQueueHandler(queue)
         handler.setFormatter(logging.Formatter(fmt=log_view_logging_format_string, datefmt="%Y-%m-%dT%H:%M:%S"))
         logger.addHandler(handler)
 
-    logger.info("Calculating center of mass...")
-    segment_COM_frame_imgPoint_XYZ, totalBodyCOM_frame_XYZ = run_center_of_mass_calculations(
-        processed_skel3d_frame_marker_xyz=skel3d_frame_marker_xyz
+    path_to_folder_where_we_will_save_this_data = processing_parameters.recording_info_model.output_data_folder_path
+
+    logger.info("Saving post-processed data")
+    save_numpy_array_to_disk(
+        array_to_save=skel3d_frame_marker_xyz,
+        file_name="mediaPipeSkel_3d_body_hands_face.npy",
+        save_directory=path_to_folder_where_we_will_save_this_data,
     )
 
-    convert_mediapipe_npy_to_csv(
-        mediapipe_3d_frame_trackedPoint_xyz=skel3d_frame_marker_xyz,
-        output_data_folder_path=processing_parameters.recording_info_model.output_data_folder_path,
-    )  # TODO: separate functionality of splitting into CSVs and savings to disk
-
-    path_to_skeleton_body_csv = (
-        Path(processing_parameters.recording_info_model.output_data_folder_path)
-        / MEDIAPIPE_BODY_3D_DATAFRAME_CSV_FILE_NAME
+    logger.info("Saving segment center of mass data")
+    save_numpy_array_to_disk(
+        array_to_save=segment_COM_frame_imgPoint_XYZ,
+        file_name=SEGMENT_CENTER_OF_MASS_NPY_FILE_NAME,
+        save_directory=Path(path_to_folder_where_we_will_save_this_data) / CENTER_OF_MASS_FOLDER_NAME,
     )
-    skeleton_dataframe = pd.read_csv(path_to_skeleton_body_csv)
 
-    logger.info("Estimating skeleton segment lengths...")
-    skeleton_segment_lengths_dict = estimate_skeleton_segment_lengths(
-        skeleton_dataframe=skeleton_dataframe,
-        skeleton_segment_definitions=mediapipe_skeleton_segment_definitions,
+    logger.info("Saving total body center of mass data")
+    save_numpy_array_to_disk(
+        array_to_save=totalBodyCOM_frame_XYZ,
+        file_name=TOTAL_BODY_CENTER_OF_MASS_NPY_FILE_NAME,
+        save_directory=Path(path_to_folder_where_we_will_save_this_data) / CENTER_OF_MASS_FOLDER_NAME,
     )
 
-    return {
-        "segment_COM": segment_COM_frame_imgPoint_XYZ,
-        "total_body_COM": totalBodyCOM_frame_XYZ,
-        "skeleton_segment_lengths": skeleton_segment_lengths_dict,
-    }
+    save_dictionary_to_json(
+        save_path=processing_parameters.recording_info_model.output_data_folder_path,
+        file_name="mediapipe_names_and_connections_dict.json",
+        dictionary=mediapipe_names_and_connections_dict,
+    )
```

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py` & `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/data_layer/data_saver/data_loader.py` & `freemocap-1.2.0/freemocap/data_layer/data_saver/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self._load_data()
 
     def _load_data(self):
         self._load_timestamps()
         self._load_data_frames()
         self._load_full_npy_data()
         self._load_center_of_mass_data()
-        self._load_segment_lengths()
+        # self._load_segment_lengths()
         self._load_names_and_connections()
         self._load_skeleton_schema()
         self._validate_data()
 
     def _load_data_frames(self):
         self.body_dataframe = self._load_dataframe(MEDIAPIPE_BODY_3D_DATAFRAME_CSV_FILE_NAME)
         self.number_of_frames = len(self.body_dataframe)
@@ -114,17 +114,17 @@
     def _load_full_npy_data(self):
         self.data_frame_name_xyz = np.load(get_full_npy_file_path(output_data_folder=self._output_folder_path))
 
     def _load_names_and_connections(self):
         with open(self._output_folder_path / "mediapipe_names_and_connections_dict.json", "r") as file:
             self.names_and_connections = json.loads(file.read())
 
-    def _load_segment_lengths(self):
-        with open(self._output_folder_path / "mediapipe_skeleton_segment_lengths.json", "r") as file:
-            self.segment_lengths = json.loads(file.read())
+    # def _load_segment_lengths(self):
+    #     with open(self._output_folder_path / "mediapipe_skeleton_segment_lengths.json", "r") as file:
+    #         self.segment_lengths = json.loads(file.read())
 
     def load_frame_data(self, frame_number: int) -> FrameData:
         return FrameData(
             timestamps=self.get_timestamps(frame_number), tracked_points=self.get_tracked_points(frame_number)
         )
 
     def get_timestamps(self, frame_number):
```

### Comparing `freemocap-1.1.1/freemocap/data_layer/data_saver/data_models.py` & `freemocap-1.2.0/freemocap/data_layer/data_saver/data_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 class InfoDict(BaseModel):
     """
     A dictionary of information about this recording, such as the measured segement lengths and the schemas that we can use to interpret the tracked points (i.e./e.g. how to connect the dots of skeleton)
     """
 
-    segment_lengths: Dict[str, Any] = Field(default_factory=dict, description="The lengths of the segments of the body")
+    # segment_lengths: Dict[str, Any] = Field(default_factory=dict, description="The lengths of the segments of the body")
     schemas: List[BaseModel] = Field(default_factory=list, description="The schemas for the tracked points")
 
 
 if __name__ == "__main__":
     # nested_dict = create_nested_dict(FramePacket)
     # print(json.dumps(nested_dict, indent=4))
```

### Comparing `freemocap-1.1.1/freemocap/data_layer/data_saver/data_saver.py` & `freemocap-1.2.0/freemocap/data_layer/data_saver/data_saver.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             frame_data_row[f"{key}_y"] = tracked_point["y"]
             frame_data_row[f"{key}_z"] = tracked_point["z"]
 
         return frame_data_row
 
     def _get_info_dict(self):
         return InfoDict(
-            segment_lengths=self._data_loader.segment_lengths,
+            # segment_lengths=self._data_loader.segment_lengths,
             schemas=[self._data_loader.skeleton_schema.dict()],
         )
 
 
 if __name__ == "__main__":
     # recording_data_saver = DataSaver(recording_folder_path=get_sample_data_path())
     recording_data_saver = DataSaver(
```

### Comparing `freemocap-1.1.1/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb` & `freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py` & `freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/data_layer/recording_models/post_processing_parameter_models.py` & `freemocap-1.2.0/freemocap/data_layer/recording_models/post_processing_parameter_models.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/data_layer/recording_models/recording_info_model.py` & `freemocap-1.2.0/freemocap/data_layer/recording_models/recording_info_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     MEDIAPIPE_3D_NPY_FILE_NAME,
 )
 from freemocap.system.paths_and_filenames.path_getters import create_camera_calibration_file_name, get_blender_file_path
 from freemocap.tests.test_image_tracking_data_shape import test_image_tracking_data_shape
 from freemocap.tests.test_mediapipe_skeleton_data_shape import test_mediapipe_skeleton_data_shape
 from freemocap.tests.test_synchronized_video_frame_counts import test_synchronized_video_frame_counts
 from freemocap.tests.test_total_body_center_of_mass_data_shape import test_total_body_center_of_mass_data_shape
+from freemocap.utilities.get_number_of_frames_of_videos_in_a_folder import get_number_of_frames_of_videos_in_a_folder
 from freemocap.utilities.get_video_paths import get_video_paths
 
 logger = logging.getLogger(__name__)
 
 
 class RecordingInfoModel:
     def __init__(
@@ -149,15 +150,15 @@
 
 
 class RecordingFolderStatusChecker:
     def __init__(self, recording_info_model: RecordingInfoModel):
         self.recording_info_model = recording_info_model
 
     @property
-    def status_check(self) -> Dict[str, Union[bool, str, float]]:
+    def status_check(self) -> Dict[str, Union[bool, str, float, dict]]:
         return {
             "synchronized_videos_status_check": self.check_synchronized_videos_status(),
             "data2d_status_check": self.check_data2d_status(),
             "data3d_status_check": self.check_data3d_status(),
             "center_of_mass_data_status_check": self.check_center_of_mass_data_status(),
             "blender_file_status_check": self.check_blender_file_status(),
             "single_video_check": self.check_single_video(),
@@ -223,43 +224,45 @@
         if not toml_status:
             logger.debug(
                 "No calibration file found with session name, checking for other calibration files in recording session"
             )
             toml_status = self.check_for_calibration_toml_with_different_name()
         return toml_status
 
-    def get_number_of_mp4s_in_synched_videos_directory(self) -> float:
+    def get_number_of_mp4s_in_synched_videos_directory(self) -> int:
         synchronized_directory_path = Path(self.recording_info_model.synchronized_videos_folder_path)
-        video_count = 0.0
 
         if not synchronized_directory_path.exists():
-            return video_count
+            return 0
 
-        for file in synchronized_directory_path.iterdir():
-            if file.is_file() and file.suffix.lower() == ".mp4":
-                video_count += 1
+        video_count = len(get_video_paths(synchronized_directory_path))
 
-        logger.info(f"Number of `.mp4`'s in {self.recording_info_model.synchronized_videos_folder_path}: {video_count}")
+        logger.info(f"Number of `.mp4`'s in {synchronized_directory_path}: {video_count}")
         return video_count
 
-    def get_number_of_frames_in_videos(self):
+    def get_number_of_frames_in_videos(self) -> Dict[str, int]:
         timestamps_directory_path = Path(self.recording_info_model.synchronized_videos_folder_path) / "timestamps"
 
-        if not timestamps_directory_path.exists():
-            return "No 'timestamps' directory found"  # TODO: Check frame status without using timestamps with openCV or FFProbe
-
         if timestamps_directory_path.exists():
             frame_counts = {}
 
             for npy_file in timestamps_directory_path.iterdir():
                 if npy_file.is_file() and npy_file.suffix.lower() == ".npy":
                     video_npy = np.load(str(npy_file))
-                    frame_counts[npy_file.name] = str(len(video_npy) - 1)
+                    frame_counts[npy_file.name] = len(video_npy) - 1
+        else:
+            logger.debug("No 'timestamps' directory, finding frame counts from synchronized videos")
+            try:
+                frame_counts = get_number_of_frames_of_videos_in_a_folder(
+                    self.recording_info_model.synchronized_videos_folder_path
+                )
+            except ValueError:
+                frame_counts = {}
 
-            return frame_counts
+        return frame_counts
 
     def check_for_calibration_toml_with_different_name(self) -> bool:
         try:
             for file in Path(self.recording_info_model.path).iterdir():
                 if file.is_file() and file.name.endswith("camera_calibration.toml"):
                     self.recording_info_model.calibration_toml_path = str(file)
                     logger.info(f"Found calibration file at: {self.recording_info_model.calibration_toml_path}")
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/actions_and_menus/actions.py` & `freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 CREATE_NEW_RECORDING_ACTION_NAME = "New Recording"
 LOAD_MOST_RECENT_RECORDING_ACTION_NAME = "Load Most Recent Recording"
 LOAD_RECORDING_ACTION_NAME = "Load Recording"
 IMPORT_VIDEOS_ACTION_NAME = "Import Videos"
 DOWNLOAD_SAMPLE_DATA_ACTION_NAME = "Download Sample Data (3 cameras, ~1000 frames)"
 DOWNLOAD_TEST_DATA_ACTION_NAME = "Download Test Data (3 cameras, ~200 frames)"
+SET_DATA_FOLDER_ACTION_NAME = "Set Freemocap Data Folder Location"
 RESET_TO_DEFAULTS_ACTION_NAME = "Reset to Default GUI Settings"
 KILL_THREADS_AND_PROCESSES_ACTION_NAME = "Kill Threads and Processes"
 REBOOT_GUI_ACTION_NAME = "Reboot GUI"
 EXIT_ACTION_NAME = "Exit"
 
 OPEN_DOCS_ACTION_NAME = "Open Documentation"
 FREEMOCAP_FOUNDATION_ACTION_NAME = "Freemocap Foundation"
@@ -52,14 +53,18 @@
         )
 
         self.download_test_data_action = QAction(DOWNLOAD_TEST_DATA_ACTION_NAME, parent=freemocap_main_window)
         self.download_test_data_action.triggered.connect(
             lambda: freemocap_main_window.download_data(download_url=FIGSHARE_TEST_ZIP_FILE_URL)
         )
 
+        self.set_data_folder_action = QAction(SET_DATA_FOLDER_ACTION_NAME, parent=freemocap_main_window)
+        self.set_data_folder_action.setShortcut("Ctrl+S")
+        self.set_data_folder_action.triggered.connect(freemocap_main_window.open_settings_dialog)
+
         self.reset_to_defaults_action = QAction(RESET_TO_DEFAULTS_ACTION_NAME, parent=freemocap_main_window)
         self.reset_to_defaults_action.triggered.connect(freemocap_main_window.reset_to_default_gui_settings)
 
         self.reboot_gui_action = QAction(REBOOT_GUI_ACTION_NAME, parent=freemocap_main_window)
         self.reboot_gui_action.setShortcut("Ctrl+R")
         self.reboot_gui_action.triggered.connect(freemocap_main_window.reboot_gui)
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/actions_and_menus/menu_bar.py` & `freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         # file menu
         file_menu = self.addMenu("&File")
 
         file_menu.addAction(actions.create_new_recording_action)
         file_menu.addAction(actions.load_most_recent_recording_action)
         file_menu.addAction(actions.load_existing_recording_action)
         file_menu.addAction(actions.import_videos_action)
+        file_menu.addAction(actions.set_data_folder_action)
         file_menu.addAction(actions.reset_to_defaults_action)
         file_menu.addAction(actions.exit_action)
 
         # Actions Menu
         actions_menu = self.addMenu("&Controller")
         actions_menu.addAction(actions.kill_running_threads_and_processes_action)
         actions_menu.addAction(actions.reboot_gui_action)
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/freemocap_main.py` & `freemocap-1.2.0/freemocap/gui/qt/freemocap_main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/main_window/freemocap_main_window.py` & `freemocap-1.2.0/freemocap/gui/qt/main_window/freemocap_main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 from skelly_viewer import SkellyViewer
 from skellycam import (
     SkellyCamParameterTreeWidget,
     SkellyCamWidget,
 )
 from tqdm import tqdm
 
-from freemocap.core_processes.export_data.blender_stuff.get_best_guess_of_blender_path import (
-    get_best_guess_of_blender_path,
-)
+
 from freemocap.data_layer.generate_jupyter_notebook.generate_jupyter_notebook import (
     generate_jupyter_notebook,
 )
 from freemocap.data_layer.recording_models.post_processing_parameter_models import (
     ProcessingParameterModel,
 )
 from freemocap.data_layer.recording_models.recording_info_model import (
@@ -39,14 +37,15 @@
 from freemocap.gui.qt.style_sheet.scss_file_watcher import SCSSFileWatcher
 from freemocap.gui.qt.style_sheet.set_css_style_sheet import apply_css_style_sheet
 from freemocap.gui.qt.utilities.copy_timestamps_folder import copy_directory_if_contains_timestamps
 from freemocap.gui.qt.utilities.get_qt_app import get_qt_app
 from freemocap.gui.qt.utilities.save_and_load_gui_state import (
     GuiState,
     load_gui_state,
+    save_gui_state,
 )
 from freemocap.gui.qt.utilities.update_most_recent_recording_toml import (
     update_most_recent_recording_toml,
 )
 from freemocap.gui.qt.widgets.active_recording_widget import ActiveRecordingInfoWidget
 from freemocap.gui.qt.widgets.camera_controller_group_box import CameraControllerGroupBox
 from freemocap.gui.qt.widgets.central_tab_widget import CentralTabWidget
@@ -60,14 +59,15 @@
 from freemocap.gui.qt.widgets.directory_view_widget import DirectoryViewWidget
 from freemocap.gui.qt.widgets.home_widget import (
     HomeWidget,
 )
 from freemocap.gui.qt.widgets.import_videos_wizard import ImportVideosWizard
 from freemocap.gui.qt.widgets.log_view_widget import LogViewWidget
 from freemocap.gui.qt.widgets.opencv_conflict_dialog import OpencvConflictDialog
+from freemocap.gui.qt.widgets.set_data_folder_dialog import SetDataFolderDialog
 from freemocap.gui.qt.widgets.welcome_screen_dialog import WelcomeScreenDialog
 from freemocap.gui.qt.workers.download_sample_data_thread_worker import DownloadDataThreadWorker
 from freemocap.gui.qt.workers.export_to_blender_thread_worker import ExportToBlenderThreadWorker
 
 # reboot GUI method based on this - https://stackoverflow.com/a/56563926/14662833
 from freemocap.system.open_file import open_file
 from freemocap.system.paths_and_filenames.file_and_folder_names import (
@@ -253,15 +253,15 @@
         center_tab_widget.set_camera_view_tab_enabled(True)
         center_tab_widget.set_visualize_data_tab_enabled(True)
 
         return center_tab_widget
 
     def _create_directory_view_widget(self):
         return DirectoryViewWidget(
-            top_level_folder_path=self._freemocap_data_folder_path,
+            gui_state=self._gui_state,
             get_active_recording_info_callable=self._active_recording_info_widget.get_active_recording_info,
         )
 
     def _create_control_panel_widget(self, log_update: Callable):
         self._camera_configuration_parameter_tree_widget = SkellyCamParameterTreeWidget(self._skellycam_widget)
 
         self._process_motion_capture_data_panel = ProcessMotionCaptureDataPanel(
@@ -271,17 +271,15 @@
             kill_thread_event=self._kill_thread_event,
             log_update=log_update,
         )
         self._process_motion_capture_data_panel.processing_finished_signal.connect(
             self._handle_processing_finished_signal
         )
 
-        self._visualization_control_panel = VisualizationControlPanel(
-            parent=self, blender_executable_path=get_best_guess_of_blender_path()
-        )
+        self._visualization_control_panel = VisualizationControlPanel(parent=self, gui_state=self._gui_state)
         self._visualization_control_panel.export_to_blender_button.clicked.connect(
             self._export_active_recording_to_blender
         )
 
         self._visualization_control_panel.generate_jupyter_notebook_button.clicked.connect(
             self._generate_jupyter_notebook
         )
@@ -297,29 +295,28 @@
         logger.debug("Exporting active recording to Blender...")
         recording_path = self._active_recording_info_widget.get_active_recording_info(return_path=True)
 
         if self._visualization_control_panel.blender_executable_path is None:
             logger.error("Blender executable path is None!")
             return
 
-        self._visualization_control_panel.get_user_selected_method_string()
         self._export_to_blender_thread_worker = ExportToBlenderThreadWorker(
             recording_path=recording_path,
-            blender_file_path=get_blender_file_path(recording_path),
-            blender_executable_path=self._visualization_control_panel.blender_executable_path,
-            blender_method=self._visualization_control_panel.get_user_selected_method_string(),
+            blender_file_path=Path(get_blender_file_path(recording_path)),
+            blender_executable_path=Path(self._visualization_control_panel.blender_executable_path),
             kill_thread_event=self._kill_thread_event,
         )
         self._export_to_blender_thread_worker.start()
-        self._export_to_blender_thread_worker.finished.connect(self._handle_export_to_blender_finished)
+        self._export_to_blender_thread_worker.success.connect(self._handle_export_to_blender_finished)
 
-    def _handle_export_to_blender_finished(self) -> None:
-        if (
-            self._controller_group_box.auto_open_in_blender_checked
-        ):
+    @Slot()
+    def _handle_export_to_blender_finished(self, success_value: bool) -> None:
+        if success_value is False:
+            logger.error("Blender export failed!")
+        elif self._controller_group_box.auto_open_in_blender_checked:
             if Path(self._active_recording_info_widget.active_recording_info.blender_file_path).exists():
                 open_file(self._active_recording_info_widget.active_recording_info.blender_file_path)
             else:
                 logger.error(
                     "Blender file does not exist! Did something go wrong in the `export_to_blender` call above?"
                 )
 
@@ -352,15 +349,17 @@
         self._active_recording_info_widget.update_parameter_tree()
         # self._recording_name_label.setText(f"Recording Name: {recording_info_model.name}")
         self._update_skelly_viewer_widget()
         self._directory_view_widget.handle_new_active_recording_selected()
 
         try:
             self._process_motion_capture_data_panel.update_calibration_path()
-        except AttributeError:  # Active Recording and Data Panel widgets rely on each other, so we're guaranteed to hit this every time the app opens
+        except (
+            AttributeError
+        ):  # Active Recording and Data Panel widgets rely on each other, so we're guaranteed to hit this every time the app opens
             logger.debug("Process motion capture data panel not created yet, skipping claibraiton setting")
         except Exception as e:
             logger.error(e)
 
         update_most_recent_recording_toml(recording_info_model=recording_info_model)
 
     def _update_skelly_viewer_widget(self):
@@ -428,14 +427,20 @@
             self._gui_state.generate_jupyter_notebook
         )
         self._controller_group_box._auto_open_in_blender_checkbox.setChecked(self._gui_state.auto_open_in_blender)
         self._controller_group_box._charuco_square_size_line_edit.setText(str(self._gui_state.charuco_square_size))
         self._process_motion_capture_data_panel._calibration_control_panel._charuco_square_size_line_edit.setText(
             str(self._gui_state.charuco_square_size)
         )
+        self._visualization_control_panel._blender_executable_label.setText(str(self._gui_state.blender_path))
+        self._visualization_control_panel._blender_executable_path = str(self._gui_state.blender_path)
+
+        save_gui_state(self._gui_state, get_gui_state_json_path())
+
+        self._active_recording_info_widget.set_active_recording(recording_folder_path=get_most_recent_recording_path())
 
     def open_import_videos_dialog(self):
         # from this tutorial - https://www.youtube.com/watch?v=gg5TepTc2Jg&t=649s
         logger.info("Opening `Import Videos` dialog... ")
 
         import_videos_path = QFileDialog.getExistingDirectory(
             self,
@@ -467,14 +472,24 @@
     def open_opencv_conflict_dialog(self):
         self._opencv_conflict_dialog = OpencvConflictDialog(
             gui_state=self._gui_state, kill_thread_event=self._kill_thread_event, parent=self
         )
 
         self._opencv_conflict_dialog.exec()
 
+    def open_settings_dialog(self):
+        self._settings_dialog = SetDataFolderDialog(
+            gui_state=self._gui_state, kill_thread_event=self._kill_thread_event, parent=self
+        )
+
+        self._settings_dialog.exec()
+
+        if self._settings_dialog.result():
+            self.reboot_gui()
+
     def download_data(self, download_url: str):
         logger.info("Downloading sample data")
         self.download_data_thread_worker = DownloadDataThreadWorker(dowload_url=download_url)
         self.download_data_thread_worker.start()
         self.download_data_thread_worker.finished.connect(self._handle_download_data_finished)
 
     @Slot(str)
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/style_sheet/css_file_watcher.py` & `freemocap-1.2.0/freemocap/gui/qt/style_sheet/css_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/style_sheet/qt_style_sheet.css` & `freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/style_sheet/qt_style_sheet.scss` & `freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/style_sheet/scss_file_watcher.py` & `freemocap-1.2.0/freemocap/gui/qt/style_sheet/scss_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/utilities/colors.py` & `freemocap-1.2.0/freemocap/gui/qt/utilities/colors.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/utilities/copy_timestamps_folder.py` & `freemocap-1.2.0/freemocap/gui/qt/utilities/copy_timestamps_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py` & `freemocap-1.2.0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/active_recording_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/active_recording_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 from PySide6.QtCore import Signal, QFileSystemWatcher
 from PySide6.QtWidgets import QApplication, QVBoxLayout, QWidget
 from pyqtgraph.parametertree import Parameter, ParameterTree
 
 from freemocap.data_layer.recording_models.recording_info_model import (
     RecordingInfoModel,
@@ -15,15 +15,15 @@
 
 
 class ActiveRecordingInfoWidget(QWidget):
     new_active_recording_selected_signal = Signal(RecordingInfoModel)
 
     def __init__(
         self,
-        parent: QWidget = None,
+        parent: Optional[QWidget] = None,
     ):
         super().__init__(parent=parent)
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
 
         self._active_recording_info = None
         self._directory_watcher = self._create_directory_watcher()
@@ -36,15 +36,15 @@
     def active_recording_info(self):
         return self._active_recording_info
 
     @property
     def active_recording_view_widget(self):
         return self._active_recording_view_widget
 
-    def get_active_recording_info(self, return_path: bool = False) -> Union[RecordingInfoModel, Path]:
+    def get_active_recording_info(self, return_path: bool = False) -> Union[RecordingInfoModel, Path, None]:
         # this is redundant to the `active_recording_info` property,
         # but it will be more intuitive to send this down as a callable
         # rather than relying on 'pass-by-reference' magic lol
 
         if self._active_recording_info is None:
             most_recent_path = get_most_recent_recording_path()
             if most_recent_path is not None:
@@ -53,16 +53,21 @@
         if return_path:
             return self._active_recording_info.path
 
         return self._active_recording_info
 
     def set_active_recording(
         self,
-        recording_folder_path: Union[str, Path],
+        recording_folder_path: Union[str, Path, None],
     ):
+        if recording_folder_path is None or recording_folder_path == "None":
+            logger.info("No recording folder path provided - clearing active recording")
+            self._active_recording_info = None
+            return
+
         logger.debug(f"Setting active recording to {recording_folder_path}")
 
         self._active_recording_info = RecordingInfoModel(recording_folder_path=str(recording_folder_path))
 
         self._update_file_watch_path(folder_to_watch=self._active_recording_info.path)
 
         logger.debug(
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/camera_controller_group_box.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/camera_controller_group_box.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/central_tab_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/central_tab_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,24 @@
 
 REPROJECTION_ERROR_FILTER_THRESHOLD = "Reprojection Error Filter Threshold (%)"
 
 MINIMUM_CAMERAS_TO_REPROJECT = "Minimum Cameras to Reproject"
 
 ANIPOSE_TREE_NAME = "Anipose Triangulation"
 
+YOLO_CROP_TREE_NAME = "YOLO Crop"
+
 USE_YOLO_CROP_METHOD = "Use YOLO Crop Method"
 
+YOLO_MODEL_SIZE = "YOLO Model Size"
+
+BOUNDING_BOX_BUFFER_METHOD = "Buffer Bounding Box:"
+
+BOUNDING_BOX_BUFFER_PERCENTAGE = "Bounding Box Buffer Percentage"
+
 STATIC_IMAGE_MODE = "Static Image Mode"
 
 MINIUMUM_TRACKING_CONFIDENCE = "Minimum Tracking Confidence"
 
 MINIMUM_DETECTION_CONFIDENCE = "Minimum Detection Confidence"
 
 MEDIAPIPE_MODEL_COMPLEXITY = "Model Complexity"
@@ -62,18 +70,46 @@
         "2 (Slowest/Most accurate)",
     ]
     return Parameter.create(
         name=MEDIAPIPE_TREE_NAME,
         type="group",
         children=[
             dict(
-                name=USE_YOLO_CROP_METHOD,
-                type="bool",
-                value=parameter_model.use_yolo_crop_method,
-                tip="If true, `skellytracker` will use YOLO to pre-crop the person from the image before running the `mediapipe` tracker",
+                name=YOLO_CROP_TREE_NAME,
+                type="group",
+                children=[
+                    dict(
+                        name=USE_YOLO_CROP_METHOD,
+                        type="bool",
+                        value=parameter_model.use_yolo_crop_method,
+                        tip="If true, `skellytracker` will use YOLO to pre-crop the person from the image before running the `mediapipe` tracker",
+                    ),
+                    dict(
+                        name=YOLO_MODEL_SIZE,
+                        type="list",
+                        limits=["nano", "small", "medium", "large", "extra_large", "high_res"],
+                        value=parameter_model.yolo_model_size,
+                        tip="Smaller models are faster but may be less accurate",
+                    ),
+                    dict(
+                        name=BOUNDING_BOX_BUFFER_METHOD,
+                        type="list",
+                        limits=["By box size", "By image size"],
+                        value=parameter_model.buffer_size_method,
+                        tip="Buffer bounding box by percentage of either box size or image size",
+                    ),
+                    dict(
+                        name=BOUNDING_BOX_BUFFER_PERCENTAGE,
+                        type="int",
+                        value=parameter_model.bounding_box_buffer_percentage,
+                        limits=(0, 100),
+                        step=1,
+                        tip="Percentage to increase size of bounding box",
+                    ),
+                ],
             ),
             dict(
                 name=MEDIAPIPE_MODEL_COMPLEXITY,
                 type="list",
                 limits=mediapipe_model_complexity_list,
                 value=mediapipe_model_complexity_list[parameter_model.mediapipe_model_complexity],
                 tip="Which Mediapipe model to use - higher complexity is slower but more accurate. "
@@ -209,14 +245,19 @@
             ),
             min_detection_confidence=parameter_values_dictionary[MINIMUM_DETECTION_CONFIDENCE],
             min_tracking_confidence=parameter_values_dictionary[MINIUMUM_TRACKING_CONFIDENCE],
             static_image_mode=parameter_values_dictionary[STATIC_IMAGE_MODE],
             run_image_tracking=parameter_values_dictionary[RUN_IMAGE_TRACKING_NAME],
             num_processes=parameter_values_dictionary[NUMBER_OF_PROCESSES_PARAMETER_NAME],
             use_yolo_crop_method=parameter_values_dictionary[USE_YOLO_CROP_METHOD],
+            yolo_model_size=parameter_values_dictionary[YOLO_MODEL_SIZE],
+            buffer_size_method=get_bounding_box_buffer_method_from_string(
+                parameter_values_dictionary[BOUNDING_BOX_BUFFER_METHOD]
+            ),
+            bounding_box_buffer_percentage=parameter_values_dictionary[BOUNDING_BOX_BUFFER_PERCENTAGE],
         ),
         anipose_triangulate_3d_parameters_model=AniposeTriangulate3DParametersModel(
             run_reprojection_error_filtering=parameter_values_dictionary[RUN_REPROJECTION_ERROR_FILTERING],
             reprojection_error_confidence_cutoff=parameter_values_dictionary[REPROJECTION_ERROR_FILTER_THRESHOLD],
             minimum_cameras_to_reproject=parameter_values_dictionary[MINIMUM_CAMERAS_TO_REPROJECT],
             confidence_threshold_cutoff=parameter_values_dictionary[ANIPOSE_CONFIDENCE_CUTOFF],
             use_triangulate_ransac_method=parameter_values_dictionary[USE_RANSAC_METHOD],
@@ -239,14 +280,22 @@
         "0 (Fastest/Least accurate)": 0,
         "1 (Middle ground)": 1,
         "2 (Slowest/Most accurate)": 2,
     }
     return mediapipe_model_complexity_dictionary[mediapipe_model_complexity_value]
 
 
+def get_bounding_box_buffer_method_from_string(buffer_method_string: str) -> str:
+    bounding_box_buffer_method_dict = {
+        "By box size": "buffer_by_box_size",
+        "By image size": "buffer_by_image_size",
+    }
+    return bounding_box_buffer_method_dict[buffer_method_string]
+
+
 def extract_processing_parameter_model_from_tree(parameter_object, value_dictionary: dict = None):
     if value_dictionary is None:
         value_dictionary = {}
 
     for child in parameter_object.children():
         if child.hasChildren():
             extract_processing_parameter_model_from_tree(child, value_dictionary)
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/control_panel_dock_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/directory_view_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/directory_view_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from pathlib import Path
 from typing import Union, Callable
 
 from PySide6.QtCore import Signal, Qt
 from PySide6.QtWidgets import QLabel, QMenu, QTreeView, QVBoxLayout, QWidget, QPushButton, QFileSystemModel
 from qtpy import QtGui
 
+from freemocap.gui.qt.utilities.save_and_load_gui_state import GuiState
 from freemocap.system.open_file import open_file
 from freemocap.system.paths_and_filenames.path_getters import get_recording_session_folder_path
 
 logger = logging.getLogger(__name__)
 
 
 class DirectoryViewWidget(QWidget):
     new_active_recording_selected_signal = Signal(str)
 
-    def __init__(self, top_level_folder_path: Union[str, Path], get_active_recording_info_callable: Callable):
+    def __init__(self, gui_state: GuiState, get_active_recording_info_callable: Callable):
         self._root_folder = None
         logger.debug("Creating QtDirectoryViewWidget")
         super().__init__()
         self._minimum_width = 300
         self.setMinimumWidth(self._minimum_width)
 
-        self._top_level_folder_path = top_level_folder_path
+        self._gui_state = gui_state
         self._get_active_recording_info_callable = get_active_recording_info_callable
 
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
 
         self._file_system_model = QFileSystemModel()
 
@@ -41,25 +42,25 @@
         self._tree_view_widget.doubleClicked.connect(self._open_file)
 
         self._tree_view_widget.setModel(self._file_system_model)
 
         self._tree_view_widget.setAlternatingRowColors(True)
         self._tree_view_widget.setColumnWidth(0, 250)
 
-        if self._top_level_folder_path is not None:
-            self.set_folder_as_root(self._top_level_folder_path)
+        self._path_label = QLabel(str(self._gui_state.freemocap_data_folder_path))
+
+        if self._gui_state.freemocap_data_folder_path is not None:
+            self.set_folder_as_root(self._gui_state.freemocap_data_folder_path)
 
         self._show_freemocap_data_folder_button = QPushButton("Show FreeMoCap Data Folder")
         self._show_freemocap_data_folder_button.clicked.connect(
-            lambda: self.set_folder_as_root(self._top_level_folder_path)
+            lambda: self.set_folder_as_root(self._gui_state.freemocap_data_folder_path)
         )
 
         self._layout.addWidget(self._show_freemocap_data_folder_button)
-
-        self._path_label = QLabel(str(self._top_level_folder_path))
         self._layout.addWidget(self._path_label)
 
     def expand_directory_to_path(self, path: Union[str, Path], collapse_other_directories: bool = True):
         if collapse_other_directories:
             logger.debug("Collapsing other directories")
             self._tree_view_widget.collapseAll()
         logger.debug(f"Expanding directory at  path: {str(path)}")
@@ -79,14 +80,16 @@
         logger.debug(f"Setting root folder to {str(folder_path)}")
         self._root_folder = folder_path
         self._tree_view_widget.setWindowTitle(str(folder_path))
         self._file_system_model.setRootPath(str(folder_path))
         self._tree_view_widget.setRootIndex(self._file_system_model.index(str(folder_path)))
         self._tree_view_widget.setColumnWidth(0, int(self._minimum_width * 0.9))
 
+        self._path_label.setText(str(folder_path))
+
     def _context_menu(self):
         menu = QMenu()
         open = menu.addAction("Open file")
         open.triggered.connect(self._open_file)
 
         set_as_active_recording = menu.addAction("Set as Active Recording folder")
         set_as_active_recording.triggered.connect(self._set_recording_as_active)
@@ -139,15 +142,16 @@
 
 if __name__ == "__main__":
     import sys
 
     from PySide6.QtWidgets import QApplication
 
     app = QApplication(sys.argv)
-    directory_view_widget = DirectoryViewWidget(top_level_folder_path=Path.home())
+    gui_state = GuiState()
+    directory_view_widget = DirectoryViewWidget(gui_state=gui_state)
 
     directory_view_widget.show()
 
     # index = directory_view_widget.expand_directory_to_path(Path.home() / ".atom")
     directory_view_widget.expand_directory_to_path(Path.home() / "Downloads")
 
     sys.exit(app.exec())
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/home_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/home_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/import_videos_wizard.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/import_videos_wizard.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/jupyter_console_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/log_view_widget.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/opencv_conflict_dialog.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/opencv_conflict_dialog.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/widgets/welcome_screen_dialog.py` & `freemocap-1.2.0/freemocap/gui/qt/widgets/welcome_screen_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self._layout.addWidget(single_camera_doc_link)
 
         multi_camera_doc_text = "To get 3d data from FreeMoCap, you need to record with multiple cameras and calibrate them with a charuco board.\nClick the link below for a tutorial on calibrating multiple cameras."
         multi_camera_docs_label = QLabel(multi_camera_doc_text)
         multi_camera_docs_label.setWordWrap(True)
         self._layout.addWidget(multi_camera_docs_label, 1)
 
-        multi_camera_recording_doc_link_string = '&#10132; <a href="https://freemocap.github.io/documentation/multi-camera-calibration.html</a>'
+        multi_camera_recording_doc_link_string = '&#10132; <a href="https://freemocap.github.io/documentation/multi-camera-calibration.html" style="color: #333333;"> Multi camera recording tutorial</a>'
         multi_camera_doc_link = QLabel(multi_camera_recording_doc_link_string)
         multi_camera_doc_link.setOpenExternalLinks(True)
         self._layout.addWidget(multi_camera_doc_link)
 
         sample_data_text = "You can also download sample data from the File Menu to try processing a session and see what the output looks like."
         sample_data_label = QLabel(sample_data_text)
         sample_data_label.setWordWrap(True)
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py` & `freemocap-1.2.0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/workers/download_sample_data_thread_worker.py` & `freemocap-1.2.0/freemocap/gui/qt/workers/download_sample_data_thread_worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,9 +27,9 @@
                 self.finished.emit(downloaded_data_path)
             else:
                 logger.error(f"Could not find downloaded data at {downloaded_data_path}")
                 raise FileNotFoundError(f"Could not find downloaded data at {downloaded_data_path}")
 
         except Exception as e:  # noqa
             logger.exception(e)
-            logger.error(f"Error downloading sample data from {self._dowload_url}")
+            logger.error(f"Error downloading sample data from {self.download_url}")
             raise e
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/workers/export_to_blender_thread_worker.py` & `freemocap-1.2.0/freemocap/gui/qt/workers/export_to_blender_thread_worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 
 from freemocap.core_processes.export_data.blender_stuff.export_to_blender.export_to_blender import export_to_blender
 
 logger = logging.getLogger(__name__)
 
 
 class ExportToBlenderThreadWorker(QThread):
-    finished = Signal()
+    success = Signal(bool)
     in_progress = Signal(str)
 
     def __init__(
         self,
         recording_path: Path,
         blender_file_path: Path,
         blender_executable_path: Path,
-        blender_method: str,
         kill_thread_event: threading.Event,
     ):
         super().__init__()
         logger.debug("Initializing Export to Blender Thread Worker")
         self._kill_thread_event = kill_thread_event
         self.recording_path = recording_path
         self.blender_file_path = blender_file_path
         self.blender_executable_path = blender_executable_path
-        self.blender_method = blender_method
 
         self._work_done = False
 
     @property
     def work_done(self):
         return self._work_done
 
@@ -42,17 +40,16 @@
         logger.info("Beginning to synchronize videos")
 
         try:
             export_to_blender(
                 recording_folder_path=self.recording_path,
                 blender_file_path=self.blender_file_path,
                 blender_exe_path=self.blender_executable_path,
-                method=self.blender_method,
             )
+            self.success.emit(True)
+            logger.debug("Blender Export Complete")
         except Exception as e:
             logger.exception("something went wrong in the Blender export")
-            logger.exception(e)
+            logger.error(e)
+            self.success.emit(False)
 
-        self.finished.emit()
         self._work_done = True
-
-        logger.debug("Blender Export Complete")
```

### Comparing `freemocap-1.1.1/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py` & `freemocap-1.2.0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py` & `freemocap-1.2.0/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/system/logging/configure_logging.py` & `freemocap-1.2.0/freemocap/system/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/system/paths_and_filenames/file_and_folder_names.py` & `freemocap-1.2.0/freemocap/system/paths_and_filenames/file_and_folder_names.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,18 @@
 
 TOTAL_BODY_CENTER_OF_MASS_NPY_FILE_NAME = "total_body_center_of_mass_xyz.npy"
 SEGMENT_CENTER_OF_MASS_NPY_FILE_NAME = "segmentCOM_frame_joint_xyz.npy"
 
 RECORDING_PARAMETERS_JSON_FILE_NAME = "recording_parameters.json"
 
 # Figshare info
-FIGSHARE_SAMPLE_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/41368323"
-FIGSHARE_TEST_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/40293973"
-FREEMOCAP_TEST_DATA_RECORDING_NAME = "freemocap_sample_data"
+FIGSHARE_SAMPLE_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/45797067"
+FIGSHARE_TEST_ZIP_FILE_URL = "https://figshare.com/ndownloader/files/45797073"
+FREEMOCAP_TEST_DATA_RECORDING_NAME = "freemocap_test_data"
+FREEMOCAP_SAMPLE_DATA_RECORDING_NAME = "freemocap_sample_data"
 
 # logo
 PATH_TO_FREEMOCAP_LOGO_SVG = str(Path(freemocap.__file__).parent / "assets/logo/freemocap-logo-black-border.svg")
 
 # progress bars
 LOG_VIEW_PROGRESS_BAR_STRING = "Log Progress"
```

### Comparing `freemocap-1.1.1/freemocap/system/paths_and_filenames/path_getters.py` & `freemocap-1.2.0/freemocap/system/paths_and_filenames/path_getters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import toml
 
+from freemocap.gui.qt.utilities.save_and_load_gui_state import load_gui_state
 from freemocap.system.paths_and_filenames.file_and_folder_names import (
     LOGS_INFO_AND_SETTINGS_FOLDER_NAME,
     LOG_FILE_FOLDER_NAME,
     BASE_FREEMOCAP_DATA_FOLDER_NAME,
     CALIBRATIONS_FOLDER_NAME,
     logger,
     RECORDING_SESSIONS_FOLDER_NAME,
@@ -46,22 +47,35 @@
 def create_camera_calibration_file_name(recording_name: str):
     return f"{recording_name}_camera_calibration.toml"
 
 
 freemocap_data_folder_path = None
 
 
-def get_freemocap_data_folder_path(create_folder: bool = True):
+def get_freemocap_data_folder_path(create_folder: bool = True) -> str:
     global freemocap_data_folder_path
 
-    if freemocap_data_folder_path is None:
-        freemocap_data_folder_path = Path(os_independent_home_dir(), BASE_FREEMOCAP_DATA_FOLDER_NAME)
+    try:
+        if freemocap_data_folder_path is None:
+            freemocap_data_folder_path = Path(os_independent_home_dir(), BASE_FREEMOCAP_DATA_FOLDER_NAME)
+        if Path(get_gui_state_json_path()).exists():
+            gui_state = load_gui_state(get_gui_state_json_path())
+        else:  # if GUI state isn't in new location, look in old location
+            gui_state = load_gui_state(
+                str(Path(freemocap_data_folder_path) / LOGS_INFO_AND_SETTINGS_FOLDER_NAME / GUI_STATE_JSON_FILENAME)
+            )
+        freemocap_data_folder_path = Path(gui_state.freemocap_data_folder_path)
+    except Exception as e:
+        print(e)  # Cannot log this due to circular import from logging config
+    finally:
+        if freemocap_data_folder_path is None:
+            freemocap_data_folder_path = Path(os_independent_home_dir(), BASE_FREEMOCAP_DATA_FOLDER_NAME)
 
-        if create_folder:
-            freemocap_data_folder_path.mkdir(exist_ok=create_folder, parents=True)
+    if create_folder:
+        freemocap_data_folder_path.mkdir(exist_ok=create_folder, parents=True)
 
     return str(freemocap_data_folder_path)
 
 
 def get_calibrations_folder_path(create_folder: bool = True):
     calibration_folder_path = Path(get_freemocap_data_folder_path()) / CALIBRATIONS_FOLDER_NAME
 
@@ -112,21 +126,23 @@
 
     session_name = time.strftime(f"session_{session_time_tag_format()}" + string_tag)
     logger.debug(f"Creating default session name: {session_name}")
 
     return session_name
 
 
-session_folder_path = None
+session_folder_path: Optional[Path] = None
 
 
 def create_new_session_folder():
     global session_folder_path
     if session_folder_path is None:
         session_folder_path = Path(get_recording_session_folder_path()) / default_session_name()
+    elif not session_folder_path.is_relative_to(get_freemocap_data_folder_path()):
+        session_folder_path = Path(get_recording_session_folder_path()) / default_session_name()
 
     return str(session_folder_path)
 
 
 def get_recording_session_folder_path(create_folder: bool = True):
     recording_session_folder_path = Path(get_freemocap_data_folder_path()) / RECORDING_SESSIONS_FOLDER_NAME
 
@@ -156,26 +172,26 @@
 
 
 def get_most_recent_recording_toml_path():
     return str(Path(get_logs_info_and_settings_folder_path()) / MOST_RECENT_RECORDING_TOML_FILENAME)
 
 
 def get_gui_state_json_path():
-    return str(Path(get_logs_info_and_settings_folder_path()) / GUI_STATE_JSON_FILENAME)
+    return str(Path(__file__).parent.parent / GUI_STATE_JSON_FILENAME)
 
 
-def get_most_recent_recording_path(subfolder_str: str = None):
+def get_most_recent_recording_path(subfolder_str: Optional[str] = None) -> Optional[str]:
     if not Path(get_most_recent_recording_toml_path()).exists():
         logger.error(f"{MOST_RECENT_RECORDING_TOML_FILENAME} not found at {get_most_recent_recording_toml_path()}!!")
         return None
 
     try:
         most_recent_recording_dict = toml.load(str(get_most_recent_recording_toml_path()))
         most_recent_recording_path = most_recent_recording_dict["most_recent_recording_path"]
-    except (ValueError, toml.TomlDecodeError, KeyError) as e:
+    except (ValueError, toml.TomlDecodeError, KeyError, FileNotFoundError) as e:
         logger.exception(e)
         return None
 
     if not Path(most_recent_recording_path).exists():
         logger.error(f"Most recent recording path {most_recent_recording_path} not found!!")
         return None
```

### Comparing `freemocap-1.1.1/freemocap/system/user_data/pipedream_pings.py` & `freemocap-1.2.0/freemocap/system/user_data/pipedream_pings.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/tests/conftest.py` & `freemocap-1.2.0/freemocap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/tests/test_by_camera_reprojection_filtering.py` & `freemocap-1.2.0/freemocap/tests/test_by_camera_reprojection_filtering.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/tests/test_geometry_utilities.py` & `freemocap-1.2.0/freemocap/tests/test_geometry_utilities.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/tests/test_image_tracking_data_shape.py` & `freemocap-1.2.0/freemocap/tests/test_image_tracking_data_shape.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 
     list_of_video_paths = get_video_paths(Path(synchronized_video_folder_path))
     number_of_videos = len(list_of_video_paths)
     assert (
         image_tracking_data.shape[0] == number_of_videos
     ), f"Number of videos in {image_tracking_data_file_path} does not match number of videos in synchronized videos folder"
 
-    frame_count = get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path)
+    frame_counts = list(get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path).values())
 
     assert (
-        len(set(frame_count)) == 1
-    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_count}"
+        len(set(frame_counts)) == 1
+    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_counts}"
     assert (
-        image_tracking_data.shape[1] == frame_count[0]
+        image_tracking_data.shape[1] == frame_counts[0]
     ), f"Number of frames in {image_tracking_data_file_path} does not match number of frames of videos in {synchronized_video_folder_path}"
 
     # TODO - check number of tracked points vs 'expected' number of tracked points
 
     assert (
         image_tracking_data.shape[3] == 3
     ), f"Data has {image_tracking_data.shape[3]} dimensions, expected 3 dimensions"
```

### Comparing `freemocap-1.1.1/freemocap/tests/test_mediapipe_skeleton_data_shape.py` & `freemocap-1.2.0/freemocap/tests/test_mediapipe_skeleton_data_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,20 @@
 
     skeleton_reprojection_error_fr_mar = np.load(reprojection_error_file_path)
 
     assert (
         len(skeleton_reprojection_error_fr_mar.shape) == 2
     ), f"3d skeleton reprojection error data file should have 2 dimensions {reprojection_error_file_path}"
 
-    frame_count = get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path)
+    frame_counts = list(get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path).values())
     assert (
-        len(set(frame_count)) == 1
-    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_count}"
+        len(set(frame_counts)) == 1
+    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_counts}"
 
-    number_of_frames = frame_count[0]
+    number_of_frames = frame_counts[0]
 
     assert skel3d_frame_marker_xyz.shape[0] == number_of_frames
     assert skeleton_reprojection_error_fr_mar.shape[0] == number_of_frames
 
     # TODO - check number of tracked points vs 'expected' number of tracked points
 
     assert (
```

### Comparing `freemocap-1.1.1/freemocap/tests/test_synchronized_video_frame_counts.py` & `freemocap-1.2.0/freemocap/tests/test_synchronized_video_frame_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     """
     Test if all the videos in this folder have precisely the same number of frames
     """
     list_of_video_paths = get_video_paths(Path(synchronized_video_folder_path))
 
     assert len(list_of_video_paths) > 0, f"No videos found in {synchronized_video_folder_path}"
 
-    frame_count = get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path)
+    frame_counts = list(get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path).values())
 
     assert (
-        len(set(frame_count)) == 1
-    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_count}"
+        len(set(frame_counts)) == 1
+    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_counts}"
```

### Comparing `freemocap-1.1.1/freemocap/tests/test_total_body_center_of_mass_data_shape.py` & `freemocap-1.2.0/freemocap/tests/test_total_body_center_of_mass_data_shape.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 ):
     assert Path(
         total_body_center_of_mass_file_path
     ).is_file(), f"No file found at {total_body_center_of_mass_file_path}"
 
     total_body_center_of_mass_fr_xyz = np.load(total_body_center_of_mass_file_path)
 
-    frame_count = get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path)
+    frame_counts = list(get_number_of_frames_of_videos_in_a_folder(synchronized_video_folder_path).values())
     assert (
-        len(set(frame_count)) == 1
-    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_count}"
+        len(set(frame_counts)) == 1
+    ), f"Videos in {synchronized_video_folder_path} have different frame counts: {frame_counts}"
 
-    number_of_frames = frame_count[0]
+    number_of_frames = frame_counts[0]
 
     assert (
         total_body_center_of_mass_fr_xyz.shape[0] == number_of_frames
     ), f"Number of frames in {total_body_center_of_mass_file_path} does not match number of frames of videos in {synchronized_video_folder_path}"
 
     assert (
         total_body_center_of_mass_fr_xyz.shape[1] == 3
```

### Comparing `freemocap-1.1.1/freemocap/utilities/create_nested_dict_from_pydantic.py` & `freemocap-1.2.0/freemocap/utilities/create_nested_dict_from_pydantic.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/utilities/download_sample_data.py` & `freemocap-1.2.0/freemocap/utilities/download_sample_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import logging
 import zipfile
 from pathlib import Path
 
 import requests
 
 from freemocap.system.paths_and_filenames.file_and_folder_names import (
+    FIGSHARE_SAMPLE_ZIP_FILE_URL,
+    FREEMOCAP_SAMPLE_DATA_RECORDING_NAME,
     FREEMOCAP_TEST_DATA_RECORDING_NAME,
     FIGSHARE_TEST_ZIP_FILE_URL,
 )
 from freemocap.system.paths_and_filenames.path_getters import get_recording_session_folder_path
 
 logger = logging.getLogger(__name__)
 
@@ -34,15 +36,20 @@
 
         r = requests.get(sample_data_zip_file_url, stream=True, timeout=(5, 60))
         r.raise_for_status()  # Check if request was successful
 
         z = zipfile.ZipFile(io.BytesIO(r.content))
         z.extractall(recording_session_folder_path)
 
-        figshare_sample_data_path = recording_session_folder_path / FREEMOCAP_TEST_DATA_RECORDING_NAME
+        if sample_data_zip_file_url == FIGSHARE_TEST_ZIP_FILE_URL:
+            figshare_sample_data_path = recording_session_folder_path / FREEMOCAP_TEST_DATA_RECORDING_NAME
+        elif sample_data_zip_file_url == FIGSHARE_SAMPLE_ZIP_FILE_URL:
+            figshare_sample_data_path = recording_session_folder_path / FREEMOCAP_SAMPLE_DATA_RECORDING_NAME
+        else:
+            figshare_sample_data_path = recording_session_folder_path / "unknown_sample_data"
         logger.info(f"Sample data extracted to {str(figshare_sample_data_path)}")
         return str(figshare_sample_data_path)
 
     except requests.exceptions.RequestException as e:
         logger.error(f"Request failed: {e}")
         raise e
     except zipfile.BadZipFile as e:
```

### Comparing `freemocap-1.1.1/freemocap/utilities/fix_opencv_conflict.py` & `freemocap-1.2.0/freemocap/utilities/fix_opencv_conflict.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py` & `freemocap-1.2.0/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `freemocap-1.2.0/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import cv2
 
 from freemocap.utilities.get_video_paths import get_video_paths
 
 logger = logging.getLogger(__name__)
 
 
-def get_number_of_frames_of_videos_in_a_folder(folder_path: Union[str, Path]):
+def get_number_of_frames_of_videos_in_a_folder(folder_path: Union[str, Path]) -> dict[str, int]:
     """
     Get the number of frames in the first video in a folder
     """
 
     list_of_video_paths = get_video_paths(Path(folder_path))
 
     if len(list_of_video_paths) == 0:
         logger.error(f"No videos found in {folder_path}")
-        return None
+        raise ValueError(f"No videos found in {folder_path}")
 
-    frame_count = []
+    frame_count = {}
     for video_path in list_of_video_paths:
         cap = cv2.VideoCapture(str(video_path))
-        frame_count.append(int(cap.get(cv2.CAP_PROP_FRAME_COUNT)))
+        frame_count[video_path.name] = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         cap.release()
 
     return frame_count
```

### Comparing `freemocap-1.1.1/freemocap/utilities/get_video_paths.py` & `freemocap-1.2.0/freemocap/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/freemocap/utilities/remove_empty_directories.py` & `freemocap-1.2.0/freemocap/utilities/remove_empty_directories.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb` & `freemocap-1.2.0/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/ipython_jupyter_notebooks/batch_process_session_folders.ipynb` & `freemocap-1.2.0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb` & `freemocap-1.2.0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb` & `freemocap-1.2.0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/noxfile.py` & `freemocap-1.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/poetry_pyproject.toml` & `freemocap-1.2.0/poetry_pyproject.toml`

 * *Files identical despite different names*

### Comparing `freemocap-1.1.1/pyproject.toml` & `freemocap-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,27 @@
     "Blender3d",
     "synchronization",
     "computer vision"
 ]
 
 dependencies = [
     "skellycam==2023.12.1090",
-    "skelly_viewer==2024.03.1021",
+    "skelly_viewer==2024.04.1022",
     "skellyforge==2023.12.1005",
     "skelly_synchronize==2023.12.1029",
-    "ajc27_freemocap_blender_addon==2023.10.1016",
+    "skellytracker==2024.04.1014",
+    "ajc27_freemocap_blender_addon==2023.10.1017",
     "mediapipe==0.10.9",
     "opencv-contrib-python==4.8.*",
     "toml==0.10.2",
     "aniposelib==0.4.3",
     "libsass==0.21.0",
     "ipykernel==6.23.1",
     "plotly==5.14.1",
     "pydantic==1.*",
-    "skellytracker==2024.3.1009",
     "PySide6==6.6.*",
     "packaging===23.2",
 ]
 
 requires-python = ">=3.9,<3.12"
 
 dynamic = ["version", "description"]
@@ -97,15 +97,15 @@
 
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.github.io/documentation/"
 Github = "https://github.com/freemocap/freemocap"
 
 [tool.bumpver]
-current_version = "v1.1.1"
+current_version = "v1.2.0"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `freemocap-1.1.1/PKG-INFO` & `freemocap-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freemocap
-Version: 1.1.1
+Version: 1.2.0
 Summary: A free and open source markerless motion capture system for everyone 💀✨
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d animation,Blender,Blender3d,synchronization,computer vision
 Author: Endurance Idehen, Aaron Cherian, Jonathan Samir Matthis
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -31,27 +31,27 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Video (UVC)
 Requires-Dist: skellycam==2023.12.1090
-Requires-Dist: skelly_viewer==2024.03.1021
+Requires-Dist: skelly_viewer==2024.04.1022
 Requires-Dist: skellyforge==2023.12.1005
 Requires-Dist: skelly_synchronize==2023.12.1029
-Requires-Dist: ajc27_freemocap_blender_addon==2023.10.1016
+Requires-Dist: skellytracker==2024.04.1014
+Requires-Dist: ajc27_freemocap_blender_addon==2023.10.1017
 Requires-Dist: mediapipe==0.10.9
 Requires-Dist: opencv-contrib-python==4.8.*
 Requires-Dist: toml==0.10.2
 Requires-Dist: aniposelib==0.4.3
 Requires-Dist: libsass==0.21.0
 Requires-Dist: ipykernel==6.23.1
 Requires-Dist: plotly==5.14.1
 Requires-Dist: pydantic==1.*
-Requires-Dist: skellytracker==2024.3.1009
 Requires-Dist: PySide6==6.6.*
 Requires-Dist: packaging===23.2
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__igd_x07_/tmpvf4sex41_TarContainer/0/280", line 75, column 87: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freemocap Version: 1.1.1 Summary: A free and open
+Metadata-Version: 2.1 Name: freemocap Version: 1.2.0 Summary: A free and open
 source markerless motion capture system for everyone ðâ¨ Keywords:
 camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless
 motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d
 animation,Blender,Blender3d,synchronization,computer vision Author: Endurance
 Idehen, Aaron Cherian, Jonathan Samir Matthis Author-email: Skelly FreeMoCap
 freemocap.org> Requires-Python: >=3.9,<3.12 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI
@@ -21,30 +21,30 @@
 Multimedia :: Video :: Display Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
 Topic :: Scientific/Engineering :: Visualization Classifier: Topic ::
 Scientific/Engineering :: Human Machine Interfaces Classifier: Topic :: System
 :: Hardware Classifier: Topic :: System :: Hardware :: Universal Serial Bus
 (USB) Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) ::
 Video (UVC) Requires-Dist: skellycam==2023.12.1090 Requires-Dist:
-skelly_viewer==2024.03.1021 Requires-Dist: skellyforge==2023.12.1005 Requires-
+skelly_viewer==2024.04.1022 Requires-Dist: skellyforge==2023.12.1005 Requires-
 Dist: skelly_synchronize==2023.12.1029 Requires-Dist:
-ajc27_freemocap_blender_addon==2023.10.1016 Requires-Dist: mediapipe==0.10.9
+skellytracker==2024.04.1014 Requires-Dist:
+ajc27_freemocap_blender_addon==2023.10.1017 Requires-Dist: mediapipe==0.10.9
 Requires-Dist: opencv-contrib-python==4.8.* Requires-Dist: toml==0.10.2
 Requires-Dist: aniposelib==0.4.3 Requires-Dist: libsass==0.21.0 Requires-Dist:
 ipykernel==6.23.1 Requires-Dist: plotly==5.14.1 Requires-Dist: pydantic==1.*
-Requires-Dist: skellytracker==2024.3.1009 Requires-Dist: PySide6==6.6.*
-Requires-Dist: packaging===23.2 Requires-Dist: black ; extra == "dev" Requires-
-Dist: bumpver ; extra == "dev" Requires-Dist: isort ; extra == "dev" Requires-
-Dist: pip-tools ; extra == "dev" Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: pytest-cov ; extra == "dev" Requires-Dist: flit ; extra == "dev"
-Requires-Dist: flake8 ; extra == "dev" Requires-Dist: flake8-bugbear ; extra ==
-"dev" Requires-Dist: flake8-bandit ; extra == "dev" Project-URL: Documentation,
-https://freemocap.github.io/documentation/ Project-URL: Github, https://
-github.com/freemocap/freemocap Project-URL: Homepage, https://freemocap.org
-Provides-Extra: dev
+Requires-Dist: PySide6==6.6.* Requires-Dist: packaging===23.2 Requires-Dist:
+black ; extra == "dev" Requires-Dist: bumpver ; extra == "dev" Requires-Dist:
+isort ; extra == "dev" Requires-Dist: pip-tools ; extra == "dev" Requires-Dist:
+pytest ; extra == "dev" Requires-Dist: pytest-cov ; extra == "dev" Requires-
+Dist: flit ; extra == "dev" Requires-Dist: flake8 ; extra == "dev" Requires-
+Dist: flake8-bugbear ; extra == "dev" Requires-Dist: flake8-bandit ; extra ==
+"dev" Project-URL: Documentation, https://freemocap.github.io/documentation/
+Project-URL: Github, https://github.com/freemocap/freemocap Project-URL:
+Homepage, https://freemocap.org Provides-Extra: dev
                                 [Project Logo]
                         ******** TThhee FFrreeeeMMooCCaapp PPrroojjeecctt ********
    ****** AA ffrreeee--aanndd--ooppeenn--ssoouurrccee,, hhaarrddwwaarree--aanndd--ssooffttwwaarree--aaggnnoossttiicc,, mmiinniimmaall--ccoosstt,,
 rreesseeaarrcchh--ggrraaddee,, mmoottiioonn ccaappttuurree ssyysstteemm aanndd ppllaattffoorrmm ffoorr ddeecceennttrraalliizzeedd sscciieennttiiffiicc
                      rreesseeaarrcchh,, eedduuccaattiioonn,, aanndd ttrraaiinniinngg ******
      _[_D_O_I_-_v_i_a_-_Z_e_n_o_d_o_._o_r_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-
       _0_0_0_0_0_0_._s_v_g_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_A_G_P_L_v_3_]_[_C_o_n_t_r_i_b_u_t_i_o_n_s_ _W_e_l_c_o_m_e_]_[_h_t_t_p_s_:_/_/
```

