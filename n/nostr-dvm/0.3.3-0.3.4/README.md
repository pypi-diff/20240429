# Comparing `tmp/nostr_dvm-0.3.3.tar.gz` & `tmp/nostr_dvm-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.3.3.tar", last modified: Tue Apr 16 12:36:19 2024, max compression
+gzip compressed data, was "nostr_dvm-0.3.4.tar", last modified: Mon Apr 29 13:36:26 2024, max compression
```

## Comparing `nostr_dvm-0.3.3.tar` & `nostr_dvm-0.3.4.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.718750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39831 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.722750 nostr_dvm-0.3.3/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.726750 nostr_dvm-0.3.3/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 12:36:19.000000 nostr_dvm-0.3.3/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:36:19.730750 nostr_dvm-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 12:36:15.000000 nostr_dvm-0.3.3/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39816 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.075397 nostr_dvm-0.3.4/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/tests/test_events.py
```

### Comparing `nostr_dvm-0.3.3/LICENSE` & `nostr_dvm-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/PKG-INFO` & `nostr_dvm-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.3
+Version: 0.3.4
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.3/README.md` & `nostr_dvm-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/bot.py` & `nostr_dvm-0.3.4/nostr_dvm/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,28 +139,28 @@
                     # if user selects an index from the overview list...
                     if decrypted_text != "" and decrypted_text[0].isdigit():
 
                         split = decrypted_text.split(' ')
                         index = int(split[0]) - 1
                         # if user sends index info, e.g. 1 info, we fetch the nip89 information and reply with it.
                         if len(split) > 1 and split[1].lower() == "info":
-                            answer_nip89(nostr_event, index)
+                            answer_nip89(nostr_event, index, giftwrap, sender)
                         # otherwise we probably have to do some work, so build an event from input and send it to the DVM
                         else:
                             task = self.dvm_config.SUPPORTED_DVMS[index].TASK
                             print("[" + self.NAME + "] Request from " + str(user.name) + " (" + str(user.nip05) +
                                   ", Balance: " + str(user.balance) + " Sats) Task: " + str(task))
 
                             if user.isblacklisted:
                                 # If users are blacklisted for some reason, tell them.
                                 answer_blacklisted(nostr_event, giftwrap, sender)
 
                             else:
                                 # Parse inputs to params
-                                tags = build_params(decrypted_text, nostr_event, index)
+                                tags = build_params(decrypted_text, sender, index)
                                 p_tag = Tag.parse(['p', self.dvm_config.SUPPORTED_DVMS[index].PUBLIC_KEY])
 
                                 if self.dvm_config.SUPPORTED_DVMS[index].SUPPORTS_ENCRYPTION:
                                     tags_str = []
                                     for tag in tags:
                                         tags_str.append(tag.as_vec())
                                     params_as_str = json.dumps(tags_str)
@@ -530,23 +530,23 @@
             if giftwrap:
                 self.client.send_sealed_msg(PublicKey.parse(sender), info, None)
             else:
                     evt = EventBuilder.encrypted_direct_msg(self.keys, nostr_event.author(),
                                                             info, None).to_event(self.keys)
                     send_event(evt, client=self.client, dvm_config=dvm_config)
 
-        def build_params(decrypted_text, nostr_event, index):
+        def build_params(decrypted_text, author, index):
             tags = []
             splitzero = decrypted_text.split(' -')
             split = splitzero[0].split(' ')
             # If only a command without parameters is sent, we assume no input is required, and that means the dvm might take in the user as input (e.g. for content discovery)
             if len(split) == 1:
                 remaining_text = decrypted_text.replace(split[0], "")
                 params = remaining_text.split(" -")
-                tag = Tag.parse(["param", "user", nostr_event.author().to_hex()])
+                tag = Tag.parse(["param", "user", author])
                 tags.append(tag)
                 for i in params:
                     print(i)
                     if i != " ":
                         try:
                             split = i.split(" ")
                             if len(split) > 1:
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/dvm.py` & `nostr_dvm-0.3.4/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.3.4/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/subscription.py` & `nostr_dvm-0.3.4/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,18 @@
             url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + '&pubkey=' + options["users"][0][1] + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
         else:
             url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
 
         headers = {'Content-type': 'application/x-www-form-urlencoded'}
         response = requests.get(url, headers=headers)
         #print(response.text)
-
+        result_list = []
         try:
             ob = json.loads(response.text)
             data = ob['data']
-            result_list = []
             for el in data:
                 try:
                     e_tag = Tag.parse(["e", el['id']])
                     result_list.append(e_tag.as_vec())
                 except Exception as e:
                     print("ERROR: " + str(e))
         except Exception as e:
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     admin_config.UPDATE_PROFILE = False
-    admin_config.REBROADCAST_NIP89 = True
+    admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config)
 
 
 def build_example_subscription(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
@@ -246,15 +246,15 @@
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
     admin_config.UPDATE_PROFILE = False
-    admin_config.REBROADCAST_NIP89 = True
+    admin_config.REBROADCAST_NIP89 = False
     admin_config.REBROADCAST_NIP88 = False
 
    # admin_config.FETCH_NIP88 = True
    # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
    # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
+    RelayOptions, RelayLimits
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
@@ -83,30 +84,33 @@
 
     def process(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = DVMTaskInterface.set_options(request_form)
-
-        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        relaylimits = RelayLimits.disable()
+        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(relaylimits))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
         database = NostrDatabase.sqlite("db/nostr_recent_notes2.db")
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
         cli.add_relay("wss://relay.damus.io")
         cli.add_relay("wss://nos.lol")
         cli.add_relay("wss://pablof7z.nostr1.com")
 
+        ropts = RelayOptions().ping(False)
+        cli.add_relay_with_opts("wss://nostr.band", ropts)
+
         cli.connect()
 
         user = PublicKey.parse(options["user"])
-        followers_filter = Filter().author(user).kinds([Kind(3)]).limit(1)
+        followers_filter = Filter().author(user).kinds([Kind(3)])
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
         print(followers)
 
         # Negentropy reconciliation
         # Query events from database
         timestamp_hour_ago = Timestamp.now().as_secs() - 7200
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
@@ -232,15 +236,15 @@
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     admin_config.UPDATE_PROFILE = False
-    admin_config.REBROADCAST_NIP89 = True
+    admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                                    admin_config=admin_config)
 
 
 def build_example_subscription(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,124 @@
 import json
 import os
-from datetime import timedelta
-from threading import Thread
-
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind
+from nostr_sdk import Tag, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
-from nostr_dvm.utils.output_utils import post_process_list_to_users
+from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
-This File contains a Module to find inactive follows for a user on nostr
-
-Accepted Inputs: None needed
-Outputs: A list of users that have been inactive 
+This File contains a Module to search for notes
+Accepted Inputs: a search query
+Outputs: A list of events 
 Params:  None
 """
 
 
-class DiscoverNonFollowers(DVMTaskInterface):
-    KIND: Kind = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
-    TASK: str = "people to block"
+class TrendingNotesNostrBand(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
+    TASK: str = "trending-content"
     FIX_COST: float = 0
-    client: Client
     dvm_config: DVMConfig
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
+        for tag in tags:
+            if tag.as_vec()[0] == 'i':
+                input_value = tag.as_vec()[1]
+                input_type = tag.as_vec()[2]
+                if input_type != "text":
+                    return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
+        print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
-        # default values
-        users = []
-        # users.append(event.author().to_hex())
-
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
-                users.append(tag.as_vec()[1])
+                input_type = tag.as_vec()[2]
 
         options = {
-            "users": users,
+
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
-        from nostr_sdk import Filter
-        from types import SimpleNamespace
-        ns = SimpleNamespace()
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        cli = Client.with_opts(signer, opts)
-        # cli.add_relay("wss://relay.nostr.band")
-        for relay in self.dvm_config.RELAY_LIST:
-            cli.add_relay(relay)
-        cli.connect()
-
         options = DVMTaskInterface.set_options(request_form)
-        step = 20
 
-        pubkeys = []
-        for user in options["users"]:
-            pubkeys.append(PublicKey.parse(user))
-
-        kind1984_filter = Filter().authors(pubkeys).kind(Kind(1984))
-        reports = cli.get_events_of([kind1984_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
-
-        bad_actors = []
-        ns.dic = {}
-        reasons = ["spam", "illegal", "impersonation"]
-        # init
-        for report in reports:
-            for tag in report.tags():
-                if tag.as_vec()[0] == "p":
-                    ns.dic[tag.as_vec()[1]] = 0
-
-        for report in reports:
-            print(report.as_json())
-            for tag in report.tags():
-                if tag.as_vec()[0] == "p":
-                    if len(tag.as_vec()) > 2 and tag.as_vec()[2] in reasons or len(tag.as_vec()) <= 2:
-                        ns.dic[tag.as_vec()[1]] += 1
-
-
-        #result = {k for (k, v) in ns.dic.items() if v > 0}
-        #result = sorted(ns.dic.items(), key=lambda x: x[1], reverse=True)
-        finallist_sorted = sorted(ns.dic.items(), key=lambda x: x[1], reverse=True)
-        converted_dict = dict(finallist_sorted)
-        print(json.dumps(converted_dict))
-        for k in converted_dict:
-            p_tag = Tag.parse(["p", k])
-            bad_actors.append(p_tag.as_vec())
+        import requests
 
-        print(json.dumps(bad_actors))
-        return json.dumps(bad_actors)
+        url = "https://api.nostr.band/v0/trending/notes"
+        try:
+            response = requests.get(url)
+            response_json = response.json()
+            result_list = []
+            i = 0
+            if len(response_json["notes"]) > 0:
+                for note in response_json["notes"]:
+                    i += 1
+                    if i < 20:
+                        e_tag = Tag.parse(["e", note["id"]])
+                        print(e_tag.as_vec())
+                        result_list.append(e_tag.as_vec())
+                    else:
+                        break
+
+            return json.dumps(result_list)
+
+        except Exception as e:
+            print(e)
+            return json.dumps([])
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
         for tag in event.tags():
             if tag.as_vec()[0] == 'output':
                 format = tag.as_vec()[1]
                 if format == "text/plain":  # check for output type
-                    result = post_process_list_to_users(result)
+                    result = post_process_list_to_events(result)
 
         # if not text/plain, don't post-process
         return result
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     # Add NIP89
+
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
-        "about": "I discover users you follow, but that don't follow you back.",
+        "image": "https://nostr.band/android-chrome-192x192.png",
+        "about": "I show trending notes from nostr.band",
+        "amount": "Free",
         "encryptionSupported": True,
         "cashuAccepted": True,
-        "nip90Params": {
-            "user": {
-                "required": False,
-                "values": [],
-                "description": "Do the task for another user"
-            },
-            "since_days": {
-                "required": False,
-                "values": [],
-                "description": "The number of days a user has not been active to be considered inactive"
-            }
-        }
+        "nip90Params": {}
     }
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return DiscoverNonFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                admin_config=admin_config)
+    return TrendingNotesNostrBand(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                  admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(DiscoverNonFollowers)
+    process_venv(TrendingNotesNostrBand)
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from datetime import timedelta
 from threading import Thread
 
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind
+from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind, RelayOptions, \
+    RelayLimits
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
@@ -20,16 +21,16 @@
 Outputs: A list of users that have been inactive 
 Params:  None
 """
 
 
 class DiscoverInactiveFollows(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
-    TASK: str = "inactive-follows"
-    FIX_COST: float = 50
+    TASK: str = "inactive-followings"
+    FIX_COST: float = 100
     client: Client
     dvm_config: DVMConfig
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
@@ -64,47 +65,66 @@
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
+
+        #relaylimits = RelayLimits().event_max_num_tags(max_num_tags=10000)
+        #relaylimits.event_max_size(None)
+        relaylimits = RelayLimits.disable()
+
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))).relay_limits(relaylimits)
+
+
         cli = Client.with_opts(signer, opts)
         for relay in self.dvm_config.RELAY_LIST:
             cli.add_relay(relay)
+        ropts = RelayOptions().ping(False)
+        cli.add_relay_with_opts("wss://nostr.band", ropts)
+
         cli.connect()
 
         options = DVMTaskInterface.set_options(request_form)
         step = 20
 
-        followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(Kind(3)).limit(1)
-        followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
+        followers_filter = Filter().author(PublicKey.parse(options["user"])).kind(Kind(3))
+        followers = cli.get_events_of([followers_filter], timedelta(seconds=5))
+
 
         if len(followers) > 0:
             result_list = []
             newest = 0
             best_entry = followers[0]
             for entry in followers:
+                print(len(best_entry.tags()))
+                print(best_entry.created_at().as_secs())
                 if entry.created_at().as_secs() > newest:
                     newest = entry.created_at().as_secs()
                     best_entry = entry
 
+
             print(best_entry.as_json())
+            print(len(best_entry.tags()))
+            print(best_entry.created_at().as_secs())
+            print(Timestamp.now().as_secs())
             followings = []
             ns.dic = {}
+            tagcount = 0
             for tag in best_entry.tags():
+                tagcount += 1
                 if tag.as_vec()[0] == "p":
                     following = tag.as_vec()[1]
                     followings.append(following)
                     ns.dic[following] = "False"
-            print("Followings: " + str(len(followings)))
+            print("Followings: " + str(len(followings)) + " Tags: " + str(tagcount))
 
             not_active_since_seconds = int(options["since_days"]) * 24 * 60 * 60
             dif = Timestamp.now().as_secs() - not_active_since_seconds
             not_active_since = Timestamp.from_secs(dif)
 
             def scanList(users, instance, i, st, notactivesince):
                 from nostr_sdk import Filter
@@ -180,14 +200,15 @@
     dvm_config.USE_OWN_VENV = False
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
         "about": "I discover users you follow, but that have been inactive on Nostr",
+        "action": "unfollow", #follow, mute, unmute
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {
             "user": {
                 "required": False,
                 "values": [],
                 "description": "Do the task for another user"
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from datetime import timedelta
 from threading import Thread
 
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind
+from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind, RelayOptions, \
+    RelayLimits
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
@@ -58,23 +59,27 @@
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        relaylimits = RelayLimits.disable()
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(relaylimits))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         cli = Client.with_opts(signer, opts)
         # cli.add_relay("wss://relay.nostr.band")
         for relay in self.dvm_config.RELAY_LIST:
             cli.add_relay(relay)
+        #add nostr band, too.
+        ropts = RelayOptions().ping(False)
+        cli.add_relay_with_opts("wss://nostr.band", ropts)
+
         cli.connect()
 
         options = DVMTaskInterface.set_options(request_form)
         step = 20
 
         followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(Kind(3))
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,124 +1,128 @@
 import json
 import os
-from nostr_sdk import Tag, Kind
+from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
+from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
-from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
-from nostr_dvm.utils.output_utils import post_process_list_to_events
+from nostr_dvm.utils.definitions import EventDefinitions
 
 """
-This File contains a Module to search for notes
-Accepted Inputs: a search query
-Outputs: A list of events 
-Params:  None
+This File contains a module to transform an Image to a short Video Clip on n-server and receive results back. 
+
+Accepted Inputs: An url to an Image
+Outputs: An url to a video
+, 
 """
 
 
-class TrendingNotesNostrBand(DVMTaskInterface):
-    KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
-    TASK: str = "trending-content"
-    FIX_COST: float = 0
-    dvm_config: DVMConfig
+class VideoGenerationSVD(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_VIDEO
+    TASK: str = "image-to-video"
+    FIX_COST: float = 120
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
-                if input_type != "text":
+                if input_type != "url":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
-        self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
+        request_form = {"jobID": event.id().to_hex() + "_" + self.NAME.replace(" ", "")}
+        request_form["trainerFilePath"] = r'modules\stablevideodiffusion\stablevideodiffusion.trainer'
+
+        url = ""
+        frames = 7  # 25
+        model = "stabilityai/stable-video-diffusion-img2vid-xt" #,stabilityai/stable-video-diffusion-img2vid
 
-        request_form = {"jobID": event.id().to_hex()}
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
+                if input_type == "url":
+                    url = str(tag.as_vec()[1]).split('#')[0]
+        # TODO add params as defined above
+
+        io_input = {
+            "id": "input_image",
+            "type": "input",
+            "src": "url:Image",
+            "uri": url
+        }
+
+        io_output = {
+            "id": "output_video",
+            "type": "output",
+            "src": "request:stream:Video"
+        }
+
+        request_form['data'] = json.dumps([io_input, io_output])
 
         options = {
+            "model": model,
+            "fps": frames
 
         }
         request_form['options'] = json.dumps(options)
+
         return request_form
 
     def process(self, request_form):
-        options = DVMTaskInterface.set_options(request_form)
-
-        import requests
-
-        url = "https://api.nostr.band/v0/trending/notes"
         try:
-            response = requests.get(url)
-            response_json = response.json()
-            result_list = []
-            i = 0
-            if len(response_json["notes"]) > 0:
-                for note in response_json["notes"]:
-                    i += 1
-                    if i < 20:
-                        e_tag = Tag.parse(["e", note["id"]])
-                        print(e_tag.as_vec())
-                        result_list.append(e_tag.as_vec())
-                    else:
-                        break
-
-            return json.dumps(result_list)
+            # Call the process route of n-server with our request form.
+            response = send_request_to_server(request_form, self.options['server'])
+            if bool(json.loads(response)['success']):
+                print("Job " + request_form['jobID'] + " sent to server")
+
+            pool = ThreadPool(processes=1)
+            thread = pool.apply_async(check_server_status, (request_form['jobID'], self.options['server']))
+            print("Wait for results of server...")
+            result = thread.get()
+            return result
 
         except Exception as e:
-            print(e)
-            return json.dumps([])
-
-    def post_process(self, result, event):
-        """Overwrite the interface function to return a social client readable format, if requested"""
-        for tag in event.tags():
-            if tag.as_vec()[0] == 'output':
-                format = tag.as_vec()[1]
-                if format == "text/plain":  # check for output type
-                    result = post_process_list_to_events(result)
-
-        # if not text/plain, don't post-process
-        return result
+            raise Exception(e)
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config):
+def build_example(name, identifier, admin_config, server_address):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     admin_config.LUD16 = dvm_config.LN_ADDRESS
-    # Add NIP89
+    # A module might have options it can be initialized with, here we set a default model, and the server
+    # address it should use. These parameters can be freely defined in the task component
+    options = {'server': server_address}
 
     nip89info = {
         "name": name,
-        "image": "https://nostr.band/android-chrome-192x192.png",
-        "about": "I show trending notes from nostr.band",
-        "amount": "Free",
+        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
+        "about": "I create a short video based on an image",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return TrendingNotesNostrBand(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                  admin_config=admin_config)
+    return VideoGenerationSVD(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                               admin_config=admin_config, options=options)
 
 
 if __name__ == '__main__':
-    process_venv(TrendingNotesNostrBand)
+    process_venv(VideoGenerationSVD)
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/dvmconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     PUBLIC_KEY: str = ""
     FIX_COST: float = None
     PER_UNIT_COST: float = None
 
     RELAY_LIST = ["wss://relay.damus.io", "wss://nos.lol", "wss://nostr.wine",
                   "wss://nostr.mom", "wss://nostr.oxtr.dev", "wss://relay.nostr.bg",
                   "wss://relay.f7z.io", "wss://pablof7z.nostr1.com", "wss://relay.nostr.net", "wss://140.f7z.io",
-                  "wss://relay.snort.social", "wss://offchain.pub/"]
+                  ]
 
     RELAY_TIMEOUT = 5
     EXTERNAL_POST_PROCESS_TYPE = PostProcessFunctionType.NONE  # Leave this on None, except the DVM is external
     LNBITS_INVOICE_KEY = ''  # Will all automatically generated by default, or read from .env
     LNBITS_ADMIN_KEY = ''  # In order to pay invoices, e.g. from the bot to DVMs, or reimburse users.
     LNBITS_URL = 'https://lnbits.com'
     LN_ADDRESS = ''
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/nip89_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,19 @@
     filter = Filter().kind(EventDefinitions.KIND_ANNOUNCEMENT).custom_tag(SingleLetterTag.lowercase(Alphabet.K), ktags)
     events = client.get_events_of([filter], timedelta(seconds=5))
     for event in events:
         print(event.as_json())
 
 
 def nip89_fetch_events_pubkey(client, pubkey, kind):
-    ktags = [str(kind)]
-    # for i in range(5000, 5999):
-    #     ktags.append(str(i))
-    nip89filter = (Filter().kind(EventDefinitions.KIND_ANNOUNCEMENT).author(PublicKey.from_hex(pubkey)).
+
+    ktags = [str(kind.as_u64())]
+    nip89filter = (Filter().kind(EventDefinitions.KIND_ANNOUNCEMENT).author(PublicKey.parse(pubkey)).
                    custom_tag(SingleLetterTag.lowercase(Alphabet.K), ktags))
-    events = client.get_events_of([nip89filter], timedelta(seconds=2))
+    events = client.get_events_of([nip89filter], timedelta(seconds=4))
 
     dvms = {}
     for event in events:
         if dvms.get(event.author().to_hex()):
             if dvms.get(event.author().to_hex()).created_at().as_secs() < event.created_at().as_secs():
                 dvms[event.author().to_hex()] = event
         else:
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.3.4/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.3/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.3.4/nostr_dvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.3
+Version: 0.3.4
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.3/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.3.4/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 nostr_dvm/interfaces/dvmtaskinterface.py
 nostr_dvm/tasks/__init__.py
 nostr_dvm/tasks/advanced_search.py
 nostr_dvm/tasks/advanced_search_wine.py
 nostr_dvm/tasks/content_discovery_currently_popular.py
 nostr_dvm/tasks/content_discovery_currently_popular_followers.py
 nostr_dvm/tasks/convert_media.py
+nostr_dvm/tasks/discovery_bot_farms.py
 nostr_dvm/tasks/discovery_censor_wot.py
 nostr_dvm/tasks/discovery_inactive_follows.py
 nostr_dvm/tasks/discovery_nonfollowers.py
 nostr_dvm/tasks/discovery_trending_notes_nostrband.py
 nostr_dvm/tasks/imagegeneration_openai_dalle.py
 nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
 nostr_dvm/tasks/imagegeneration_sd21_mlx.py
```

### Comparing `nostr_dvm-0.3.3/setup.py` & `nostr_dvm-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.3'
+VERSION = '0.3.4'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
                     'This is an early stage release. Interfaces might change/brick')
 
 # Setting up
 setup(
     name="nostr-dvm",
```

### Comparing `nostr_dvm-0.3.3/tests/test_dvm_client.py` & `nostr_dvm-0.3.4/tests/test_dvm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import time
 from pathlib import Path
 from threading import Thread
 
 import dotenv
 from nostr_sdk import Keys, Client, Tag, EventBuilder, Filter, HandleNotification, Timestamp, nip04_decrypt, \
-    nip04_encrypt, NostrSigner, PublicKey, Event
+    nip04_encrypt, NostrSigner, PublicKey, Event, Kind, RelayOptions
 
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.nostr_utils import send_event, check_and_set_private_key
 from nostr_dvm.utils.definitions import EventDefinitions
 
 
 # TODO HINT: Best use this path with a previously whitelisted privkey, as zapping events is not implemented in the lib/code
@@ -118,14 +118,42 @@
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
     send_event(event, client=client, dvm_config=config)
     return event.as_json()
 
 
+def nostr_client_test_inactive_filter(user):
+    keys = Keys.parse(check_and_set_private_key("test_client"))
+
+    relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz",
+                  ]
+
+    relaysTag = Tag.parse(relay_list)
+    alttag = Tag.parse(["alt", "This is a NIP90 DVM AI task to find people that are inactive"])
+    paramTag = Tag.parse(["param", "user", user])
+    paramTag2 = Tag.parse(["param", "since_days", "120"])
+
+    tags = [relaysTag, alttag, paramTag, paramTag2]
+
+
+    event = EventBuilder(EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY, str("Give me inactive users"),
+                         tags).to_event(keys)
+
+    signer = NostrSigner.keys(keys)
+    client = Client(signer)
+    for relay in relay_list:
+        client.add_relay(relay)
+    ropts = RelayOptions().ping(False)
+    client.add_relay_with_opts("wss://nostr.band", ropts)
+    client.connect()
+    config = DVMConfig
+    send_event(event, client=client, dvm_config=config)
+    return event.as_json()
+
 def nostr_client_test_tts(prompt):
     keys = Keys.parse(check_and_set_private_key("test_client"))
 
     iTag = Tag.parse(["i", prompt, "text"])
     paramTag1 = Tag.parse(["param", "language", "en"])
 
     bidTag = Tag.parse(['bid', str(1000 * 1000), str(1000 * 1000)])
@@ -197,25 +225,31 @@
     for relay in dvmconfig.RELAY_LIST:
         client.add_relay(relay)
     client.connect()
 
     dm_zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_DM,
                                                EventDefinitions.KIND_ZAP]).since(
         Timestamp.now())  # events to us specific
-    dvm_filter = (Filter().kinds([EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
-                                  EventDefinitions.KIND_FEEDBACK]).since(Timestamp.now()))  # public events
+    kinds = [EventDefinitions.KIND_NIP90_GENERIC]
+    SUPPORTED_KINDS = [Kind(6301)]
+
+    for kind in SUPPORTED_KINDS:
+        if kind not in kinds:
+            kinds.append(kind)
+    dvm_filter = (Filter().kinds(kinds).since(Timestamp.now()))
     client.subscribe([dm_zap_filter, dvm_filter], None)
 
     # nostr_client_test_translation("This is the result of the DVM in spanish", "text", "es", 20, 20)
     # nostr_client_test_translation("note1p8cx2dz5ss5gnk7c59zjydcncx6a754c0hsyakjvnw8xwlm5hymsnc23rs", "event", "es", 20,20)
     # nostr_client_test_translation("44a0a8b395ade39d46b9d20038b3f0c8a11168e67c442e3ece95e4a1703e2beb", "event", "zh", 20, 20)
     # nostr_client_test_image("a beautiful purple ostrich watching the sunset")
     # nostr_client_test_search_profile("dontbelieve")
     wot = ["99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64"]
-    nostr_client_test_censor_filter(wot)
+    #nostr_client_test_censor_filter(wot)
+    nostr_client_test_inactive_filter("99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64")
 
     # nostr_client_test_tts("Hello, this is a test. Mic check one, two.")
 
     # cashutoken = "cashuAeyJ0b2tlbiI6W3sicHJvb2ZzIjpbeyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MSwiQyI6IjAyNWU3ODZhOGFkMmExYTg0N2YxMzNiNGRhM2VhMGIyYWRhZGFkOTRiYzA4M2E2NWJjYjFlOTgwYTE1NGIyMDA2NCIsInNlY3JldCI6InQ1WnphMTZKMGY4UElQZ2FKTEg4V3pPck5rUjhESWhGa291LzVzZFd4S0U9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6NCwiQyI6IjAyOTQxNmZmMTY2MzU5ZWY5ZDc3MDc2MGNjZmY0YzliNTMzMzVmZTA2ZGI5YjBiZDg2Njg5Y2ZiZTIzMjVhYWUwYiIsInNlY3JldCI6IlRPNHB5WE43WlZqaFRQbnBkQ1BldWhncm44UHdUdE5WRUNYWk9MTzZtQXM9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MTYsIkMiOiIwMmRiZTA3ZjgwYmMzNzE0N2YyMDJkNTZiMGI3ZTIzZTdiNWNkYTBhNmI3Yjg3NDExZWYyOGRiZDg2NjAzNzBlMWIiLCJzZWNyZXQiOiJHYUNIdHhzeG9HM3J2WWNCc0N3V0YxbU1NVXczK0dDN1RKRnVwOHg1cURzPSJ9XSwibWludCI6Imh0dHBzOi8vbG5iaXRzLmJpdGNvaW5maXhlc3RoaXMub3JnL2Nhc2h1L2FwaS92MS9ScDlXZGdKZjlxck51a3M1eVQ2SG5rIn1dfQ=="
     # nostr_client_test_image_private("a beautiful ostrich watching the sunset")
     class NotificationHandler(HandleNotification):
         def handle(self, relay_url, subscription_id, event: Event):
```

### Comparing `nostr_dvm-0.3.3/tests/test_events.py` & `nostr_dvm-0.3.4/tests/test_events.py`

 * *Files identical despite different names*

