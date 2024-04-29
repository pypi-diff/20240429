# Comparing `tmp/tonkord.py-2.0.tar.gz` & `tmp/tonkord.py-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonkord.py-2.0.tar", last modified: Mon Apr 29 11:55:12 2024, max compression
+gzip compressed data, was "tonkord.py-2.2.2.tar", last modified: Mon Apr 29 12:02:39 2024, max compression
```

## Comparing `tonkord.py-2.0.tar` & `tonkord.py-2.2.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.159483 tonkord.py-2.0/
--rw-rw-rw-   0        0        0     1102 2024-04-23 05:06:43.000000 tonkord.py-2.0/LICENSE
--rw-rw-rw-   0        0        0      116 2024-04-23 05:06:43.000000 tonkord.py-2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2573 2024-04-29 11:55:12.158487 tonkord.py-2.0/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-04-29 11:16:51.000000 tonkord.py-2.0/README.rst
--rw-rw-rw-   0        0        0      919 2024-04-23 05:06:43.000000 tonkord.py-2.0/pyproject.toml
--rw-rw-rw-   0        0        0       67 2024-04-23 05:06:43.000000 tonkord.py-2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:55:12.159483 tonkord.py-2.0/setup.cfg
--rw-rw-rw-   0        0        0     3512 2024-04-29 11:48:28.000000 tonkord.py-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.090710 tonkord.py-2.0/tests/
--rw-rw-rw-   0        0        0     2188 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_annotated_annotation.py
--rw-rw-rw-   0        0        0     5361 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_autocomplete.py
--rw-rw-rw-   0        0        0    10738 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_description.py
--rw-rw-rw-   0        0        0    20190 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_group.py
--rw-rw-rw-   0        0        0     6780 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_invoke.py
--rw-rw-rw-   0        0        0     2213 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_colour.py
--rw-rw-rw-   0        0        0    16294 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_commands_cog.py
--rw-rw-rw-   0        0        0     4894 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_commands_description.py
--rw-rw-rw-   0        0        0     5332 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_tasks.py
--rw-rw-rw-   0        0        0     4153 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_files.py
--rw-rw-rw-   0        0        0    10566 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.117621 tonkord.py-2.0/tonkord/
--rw-rw-rw-   0        0        0     1993 2024-04-29 11:55:07.000000 tonkord.py-2.0/tonkord/__init__.py
--rw-rw-rw-   0        0        0    11394 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/__main__.py
--rw-rw-rw-   0        0        0     1444 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/_types.py
--rw-rw-rw-   0        0        0    68645 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/abc.py
--rw-rw-rw-   0        0        0    28940 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/activity.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.134565 tonkord.py-2.0/tonkord/app_commands/
--rw-rw-rw-   0        0        0      444 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18620 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/checks.py
--rw-rw-rw-   0        0        0    97078 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19748 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/errors.py
--rw-rw-rw-   0        0        0    39593 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/models.py
--rw-rw-rw-   0        0        0    13386 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    33225 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    11044 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/translator.py
--rw-rw-rw-   0        0        0    49299 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/tree.py
--rw-rw-rw-   0        0        0    19929 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/appinfo.py
--rw-rw-rw-   0        0        0    16692 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/asset.py
--rw-rw-rw-   0        0        0    39755 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/audit_logs.py
--rw-rw-rw-   0        0        0    27638 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/automod.py
--rw-rw-rw-   0        0        0     3859 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/backoff.py
--rw-rw-rw-   0        0        0   121700 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/channel.py
--rw-rw-rw-   0        0        0    98085 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/client.py
--rw-rw-rw-   0        0        0    15014 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/colour.py
--rw-rw-rw-   0        0        0    20993 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/components.py
--rw-rw-rw-   0        0        0     3124 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/context_managers.py
--rw-rw-rw-   0        0        0    23479 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/embeds.py
--rw-rw-rw-   0        0        0     8831 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/emoji.py
--rw-rw-rw-   0        0        0    25928 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/enums.py
--rw-rw-rw-   0        0        0     9232 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.083732 tonkord.py-2.0/tonkord/ext/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.139549 tonkord.py-2.0/tonkord/ext/commands/
--rw-rw-rw-   0        0        0      458 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2711 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    53628 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    32370 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    41097 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/context.py
--rw-rw-rw-   0        0        0    47543 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/converter.py
--rw-rw-rw-   0        0        0    10006 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    92194 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36964 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    23572 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    59452 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/help.py
--rw-rw-rw-   0        0        0    38076 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     9593 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6443 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.140545 tonkord.py-2.0/tonkord/ext/tasks/
--rw-rw-rw-   0        0        0    30480 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5601 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/file.py
--rw-rw-rw-   0        0        0    61982 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/flags.py
--rw-rw-rw-   0        0        0    37212 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/gateway.py
--rw-rw-rw-   0        0        0   160673 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/guild.py
--rw-rw-rw-   0        0        0    97147 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/http.py
--rw-rw-rw-   0        0        0    13751 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/integrations.py
--rw-rw-rw-   0        0        0    48955 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/interactions.py
--rw-rw-rw-   0        0        0    21211 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/invite.py
--rw-rw-rw-   0        0        0    43155 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/member.py
--rw-rw-rw-   0        0        0     5745 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/mentions.py
--rw-rw-rw-   0        0        0    91350 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/message.py
--rw-rw-rw-   0        0        0     1531 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/mixins.py
--rw-rw-rw-   0        0        0     3837 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/object.py
--rw-rw-rw-   0        0        0     3771 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/oggparse.py
--rw-rw-rw-   0        0        0    16882 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/opus.py
--rw-rw-rw-   0        0        0     8223 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/partial_emoji.py
--rw-rw-rw-   0        0        0    32389 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/permissions.py
--rw-rw-rw-   0        0        0    30450 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/player.py
--rw-rw-rw-   0        0        0        0 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/py.typed
--rw-rw-rw-   0        0        0    18600 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/raw_models.py
--rw-rw-rw-   0        0        0     9430 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/reaction.py
--rw-rw-rw-   0        0        0    18745 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/role.py
--rw-rw-rw-   0        0        0    24311 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/scheduled_event.py
--rw-rw-rw-   0        0        0    21301 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/shard.py
--rw-rw-rw-   0        0        0     6871 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/sku.py
--rw-rw-rw-   0        0        0     6690 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/stage_instance.py
--rw-rw-rw-   0        0        0    77030 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/state.py
--rw-rw-rw-   0        0        0    16713 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/sticker.py
--rw-rw-rw-   0        0        0     5164 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/team.py
--rw-rw-rw-   0        0        0     9736 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/template.py
--rw-rw-rw-   0        0        0    33420 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/threads.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.150512 tonkord.py-2.0/tonkord/types/
--rw-rw-rw-   0        0        0      159 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/__init__.py
--rw-rw-rw-   0        0        0     2841 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/activity.py
--rw-rw-rw-   0        0        0     2550 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/appinfo.py
--rw-rw-rw-   0        0        0     8870 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/audit_log.py
--rw-rw-rw-   0        0        0     4184 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/automod.py
--rw-rw-rw-   0        0        0     5131 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/channel.py
--rw-rw-rw-   0        0        0     6484 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/command.py
--rw-rw-rw-   0        0        0     3606 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/components.py
--rw-rw-rw-   0        0        0     2419 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/embed.py
--rw-rw-rw-   0        0        0     1574 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/emoji.py
--rw-rw-rw-   0        0        0     9128 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/gateway.py
--rw-rw-rw-   0        0        0     5781 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/guild.py
--rw-rw-rw-   0        0        0     2370 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/integration.py
--rw-rw-rw-   0        0        0     7421 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/interactions.py
--rw-rw-rw-   0        0        0     2797 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/invite.py
--rw-rw-rw-   0        0        0     2155 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/member.py
--rw-rw-rw-   0        0        0     4840 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/message.py
--rw-rw-rw-   0        0        0     1815 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/role.py
--rw-rw-rw-   0        0        0     3405 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1657 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/sku.py
--rw-rw-rw-   0        0        0     1210 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/snowflake.py
--rw-rw-rw-   0        0        0     2343 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/sticker.py
--rw-rw-rw-   0        0        0     1607 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/team.py
--rw-rw-rw-   0        0        0     1658 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/template.py
--rw-rw-rw-   0        0        0     2534 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/threads.py
--rw-rw-rw-   0        0        0     1813 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/user.py
--rw-rw-rw-   0        0        0     2352 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/voice.py
--rw-rw-rw-   0        0        0     2045 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/webhook.py
--rw-rw-rw-   0        0        0     1500 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1948 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.154499 tonkord.py-2.0/tonkord/ui/
--rw-rw-rw-   0        0        0      326 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/__init__.py
--rw-rw-rw-   0        0        0    11085 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/button.py
--rw-rw-rw-   0        0        0     8386 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/dynamic.py
--rw-rw-rw-   0        0        0     5555 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/item.py
--rw-rw-rw-   0        0        0     7252 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/modal.py
--rw-rw-rw-   0        0        0    45302 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/select.py
--rw-rw-rw-   0        0        0     8583 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/text_input.py
--rw-rw-rw-   0        0        0    26827 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/view.py
--rw-rw-rw-   0        0        0    18771 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/user.py
--rw-rw-rw-   0        0        0    43235 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/utils.py
--rw-rw-rw-   0        0        0    20211 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/voice_client.py
--rw-rw-rw-   0        0        0    28278 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/voice_state.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.156495 tonkord.py-2.0/tonkord/webhook/
--rw-rw-rw-   0        0        0      195 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/__init__.py
--rw-rw-rw-   0        0        0    72495 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/async_.py
--rw-rw-rw-   0        0        0    44265 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/sync.py
--rw-rw-rw-   0        0        0     7757 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/welcome_screen.py
--rw-rw-rw-   0        0        0    10751 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.157490 tonkord.py-2.0/tonkord.py.egg-info/
--rw-rw-rw-   0        0        0     2573 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3427 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      641 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.444497 tonkord.py-2.2.2/
+-rw-rw-rw-   0        0        0     1102 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0      116 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2575 2024-04-29 12:02:39.444497 tonkord.py-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-04-29 11:16:51.000000 tonkord.py-2.2.2/README.rst
+-rw-rw-rw-   0        0        0      919 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       67 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:02:39.444497 tonkord.py-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     3512 2024-04-29 12:01:06.000000 tonkord.py-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.375723 tonkord.py-2.2.2/tests/
+-rw-rw-rw-   0        0        0     2188 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_annotated_annotation.py
+-rw-rw-rw-   0        0        0     5361 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_app_commands_autocomplete.py
+-rw-rw-rw-   0        0        0    10738 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_app_commands_description.py
+-rw-rw-rw-   0        0        0    20190 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_app_commands_group.py
+-rw-rw-rw-   0        0        0     6780 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_app_commands_invoke.py
+-rw-rw-rw-   0        0        0     2213 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_colour.py
+-rw-rw-rw-   0        0        0    16294 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_ext_commands_cog.py
+-rw-rw-rw-   0        0        0     4894 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_ext_commands_description.py
+-rw-rw-rw-   0        0        0     5332 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_ext_tasks.py
+-rw-rw-rw-   0        0        0     4153 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_files.py
+-rw-rw-rw-   0        0        0    10566 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.401638 tonkord.py-2.2.2/tonkord/
+-rw-rw-rw-   0        0        0     1995 2024-04-29 12:02:36.000000 tonkord.py-2.2.2/tonkord/__init__.py
+-rw-rw-rw-   0        0        0    11394 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/__main__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/_types.py
+-rw-rw-rw-   0        0        0    68645 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/abc.py
+-rw-rw-rw-   0        0        0    28940 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/activity.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.414595 tonkord.py-2.2.2/tonkord/app_commands/
+-rw-rw-rw-   0        0        0      444 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18620 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    97078 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19748 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    39593 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13386 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    33225 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    11044 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    49299 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    19929 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/appinfo.py
+-rw-rw-rw-   0        0        0    16692 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/asset.py
+-rw-rw-rw-   0        0        0    39755 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/audit_logs.py
+-rw-rw-rw-   0        0        0    27638 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/automod.py
+-rw-rw-rw-   0        0        0     3859 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/backoff.py
+-rw-rw-rw-   0        0        0   121700 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/channel.py
+-rw-rw-rw-   0        0        0    98085 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/client.py
+-rw-rw-rw-   0        0        0    15014 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/colour.py
+-rw-rw-rw-   0        0        0    20993 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/components.py
+-rw-rw-rw-   0        0        0     3124 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/context_managers.py
+-rw-rw-rw-   0        0        0    23479 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/embeds.py
+-rw-rw-rw-   0        0        0     8831 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/emoji.py
+-rw-rw-rw-   0        0        0    25928 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/enums.py
+-rw-rw-rw-   0        0        0     9232 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.368747 tonkord.py-2.2.2/tonkord/ext/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.422569 tonkord.py-2.2.2/tonkord/ext/commands/
+-rw-rw-rw-   0        0        0      458 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2711 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    53628 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    32370 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    41097 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    47527 2024-04-29 11:58:16.000000 tonkord.py-2.2.2/tonkord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    10006 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    92194 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36964 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    23572 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    59452 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    38076 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     9593 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6443 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.422569 tonkord.py-2.2.2/tonkord/ext/tasks/
+-rw-rw-rw-   0        0        0    30480 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5601 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/file.py
+-rw-rw-rw-   0        0        0    61982 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/flags.py
+-rw-rw-rw-   0        0        0    37212 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/gateway.py
+-rw-rw-rw-   0        0        0   160673 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/guild.py
+-rw-rw-rw-   0        0        0    97147 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/http.py
+-rw-rw-rw-   0        0        0    13751 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/integrations.py
+-rw-rw-rw-   0        0        0    48955 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/interactions.py
+-rw-rw-rw-   0        0        0    21211 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/invite.py
+-rw-rw-rw-   0        0        0    43155 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/member.py
+-rw-rw-rw-   0        0        0     5745 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/mentions.py
+-rw-rw-rw-   0        0        0    91350 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/message.py
+-rw-rw-rw-   0        0        0     1531 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/mixins.py
+-rw-rw-rw-   0        0        0     3837 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/object.py
+-rw-rw-rw-   0        0        0     3771 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/oggparse.py
+-rw-rw-rw-   0        0        0    16882 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/opus.py
+-rw-rw-rw-   0        0        0     8223 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/partial_emoji.py
+-rw-rw-rw-   0        0        0    32389 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/permissions.py
+-rw-rw-rw-   0        0        0    30450 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/player.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/py.typed
+-rw-rw-rw-   0        0        0    18600 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/raw_models.py
+-rw-rw-rw-   0        0        0     9430 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/reaction.py
+-rw-rw-rw-   0        0        0    18745 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/role.py
+-rw-rw-rw-   0        0        0    24311 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/scheduled_event.py
+-rw-rw-rw-   0        0        0    21301 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/shard.py
+-rw-rw-rw-   0        0        0     6871 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/sku.py
+-rw-rw-rw-   0        0        0     6690 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/stage_instance.py
+-rw-rw-rw-   0        0        0    77030 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/state.py
+-rw-rw-rw-   0        0        0    16713 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/sticker.py
+-rw-rw-rw-   0        0        0     5164 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/team.py
+-rw-rw-rw-   0        0        0     9736 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/template.py
+-rw-rw-rw-   0        0        0    33420 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/threads.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.434530 tonkord.py-2.2.2/tonkord/types/
+-rw-rw-rw-   0        0        0      159 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/__init__.py
+-rw-rw-rw-   0        0        0     2841 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/activity.py
+-rw-rw-rw-   0        0        0     2550 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8870 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4184 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/automod.py
+-rw-rw-rw-   0        0        0     5131 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/channel.py
+-rw-rw-rw-   0        0        0     6484 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/command.py
+-rw-rw-rw-   0        0        0     3606 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/components.py
+-rw-rw-rw-   0        0        0     2419 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/embed.py
+-rw-rw-rw-   0        0        0     1574 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/emoji.py
+-rw-rw-rw-   0        0        0     9128 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/gateway.py
+-rw-rw-rw-   0        0        0     5781 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/guild.py
+-rw-rw-rw-   0        0        0     2370 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/integration.py
+-rw-rw-rw-   0        0        0     7421 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/interactions.py
+-rw-rw-rw-   0        0        0     2797 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/invite.py
+-rw-rw-rw-   0        0        0     2155 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/member.py
+-rw-rw-rw-   0        0        0     4840 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/message.py
+-rw-rw-rw-   0        0        0     1815 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/role.py
+-rw-rw-rw-   0        0        0     3405 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1657 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/sku.py
+-rw-rw-rw-   0        0        0     1210 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2343 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/sticker.py
+-rw-rw-rw-   0        0        0     1607 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/team.py
+-rw-rw-rw-   0        0        0     1658 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/template.py
+-rw-rw-rw-   0        0        0     2534 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/threads.py
+-rw-rw-rw-   0        0        0     1813 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/user.py
+-rw-rw-rw-   0        0        0     2352 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/voice.py
+-rw-rw-rw-   0        0        0     2045 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/webhook.py
+-rw-rw-rw-   0        0        0     1500 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1948 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/types/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.440510 tonkord.py-2.2.2/tonkord/ui/
+-rw-rw-rw-   0        0        0      326 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/__init__.py
+-rw-rw-rw-   0        0        0    11085 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/button.py
+-rw-rw-rw-   0        0        0     8386 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/dynamic.py
+-rw-rw-rw-   0        0        0     5555 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/item.py
+-rw-rw-rw-   0        0        0     7252 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/modal.py
+-rw-rw-rw-   0        0        0    45302 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/select.py
+-rw-rw-rw-   0        0        0     8583 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/text_input.py
+-rw-rw-rw-   0        0        0    26827 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/ui/view.py
+-rw-rw-rw-   0        0        0    18771 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/user.py
+-rw-rw-rw-   0        0        0    43219 2024-04-29 11:59:46.000000 tonkord.py-2.2.2/tonkord/utils.py
+-rw-rw-rw-   0        0        0    20211 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/voice_client.py
+-rw-rw-rw-   0        0        0    28278 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/voice_state.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.441507 tonkord.py-2.2.2/tonkord/webhook/
+-rw-rw-rw-   0        0        0      195 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    72495 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/webhook/async_.py
+-rw-rw-rw-   0        0        0    44265 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7757 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10751 2024-04-23 05:06:43.000000 tonkord.py-2.2.2/tonkord/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:02:39.442504 tonkord.py-2.2.2/tonkord.py.egg-info/
+-rw-rw-rw-   0        0        0     2575 2024-04-29 12:02:39.000000 tonkord.py-2.2.2/tonkord.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3427 2024-04-29 12:02:39.000000 tonkord.py-2.2.2/tonkord.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:02:39.000000 tonkord.py-2.2.2/tonkord.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      641 2024-04-29 12:02:39.000000 tonkord.py-2.2.2/tonkord.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 12:02:39.000000 tonkord.py-2.2.2/tonkord.py.egg-info/top_level.txt
```

### Comparing `tonkord.py-2.0/LICENSE` & `tonkord.py-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/PKG-INFO` & `tonkord.py-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkord.py
-Version: 2.0
+Version: 2.2.2
 Summary: A Python wrapper for the Discord API
 Home-page: https://9tonkla.cloud
 Author: tonkoranit
 License: MIT
 Project-URL: Documentation, https://9tonkla.cloud
 Project-URL: Issue tracker, https://9tonkla.cloud
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tonkord.py-2.0/pyproject.toml` & `tonkord.py-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/setup.py` & `tonkord.py-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_annotated_annotation.py` & `tonkord.py-2.2.2/tests/test_annotated_annotation.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_app_commands_autocomplete.py` & `tonkord.py-2.2.2/tests/test_app_commands_autocomplete.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_app_commands_description.py` & `tonkord.py-2.2.2/tests/test_app_commands_description.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_app_commands_group.py` & `tonkord.py-2.2.2/tests/test_app_commands_group.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_app_commands_invoke.py` & `tonkord.py-2.2.2/tests/test_app_commands_invoke.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_colour.py` & `tonkord.py-2.2.2/tests/test_colour.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_ext_commands_cog.py` & `tonkord.py-2.2.2/tests/test_ext_commands_cog.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_ext_commands_description.py` & `tonkord.py-2.2.2/tests/test_ext_commands_description.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_ext_tasks.py` & `tonkord.py-2.2.2/tests/test_ext_tasks.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_files.py` & `tonkord.py-2.2.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tests/test_utils.py` & `tonkord.py-2.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/__init__.py` & `tonkord.py-2.2.2/tonkord/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 """
 
 __title__ = 'tonkord'
 __author__ = 'tonkoranit'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2015-present Rapptz'
-__version__ = '2.0'
+__version__ = '2.2.2'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
```

### Comparing `tonkord.py-2.0/tonkord/__main__.py` & `tonkord.py-2.2.2/tonkord/__main__.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/_types.py` & `tonkord.py-2.2.2/tonkord/_types.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/abc.py` & `tonkord.py-2.2.2/tonkord/abc.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/activity.py` & `tonkord.py-2.2.2/tonkord/activity.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/checks.py` & `tonkord.py-2.2.2/tonkord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/commands.py` & `tonkord.py-2.2.2/tonkord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/errors.py` & `tonkord.py-2.2.2/tonkord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/models.py` & `tonkord.py-2.2.2/tonkord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/namespace.py` & `tonkord.py-2.2.2/tonkord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/transformers.py` & `tonkord.py-2.2.2/tonkord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/translator.py` & `tonkord.py-2.2.2/tonkord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/app_commands/tree.py` & `tonkord.py-2.2.2/tonkord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/appinfo.py` & `tonkord.py-2.2.2/tonkord/appinfo.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/asset.py` & `tonkord.py-2.2.2/tonkord/asset.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/audit_logs.py` & `tonkord.py-2.2.2/tonkord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/automod.py` & `tonkord.py-2.2.2/tonkord/automod.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/backoff.py` & `tonkord.py-2.2.2/tonkord/backoff.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/channel.py` & `tonkord.py-2.2.2/tonkord/channel.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/client.py` & `tonkord.py-2.2.2/tonkord/client.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/colour.py` & `tonkord.py-2.2.2/tonkord/colour.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/components.py` & `tonkord.py-2.2.2/tonkord/components.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/context_managers.py` & `tonkord.py-2.2.2/tonkord/context_managers.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/embeds.py` & `tonkord.py-2.2.2/tonkord/embeds.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/emoji.py` & `tonkord.py-2.2.2/tonkord/emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/enums.py` & `tonkord.py-2.2.2/tonkord/enums.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/errors.py` & `tonkord.py-2.2.2/tonkord/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/_types.py` & `tonkord.py-2.2.2/tonkord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/bot.py` & `tonkord.py-2.2.2/tonkord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/cog.py` & `tonkord.py-2.2.2/tonkord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/context.py` & `tonkord.py-2.2.2/tonkord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/converter.py` & `tonkord.py-2.2.2/tonkord/ext/commands/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,21 +41,21 @@
     Type,
     TypeVar,
     Union,
     runtime_checkable,
 )
 import types
 
-import discord
+import tonkord
 
 from .errors import *
 
 if TYPE_CHECKING:
-    from discord.state import Channel
-    from discord.threads import Thread
+    from tonkord.state import Channel
+    from tonkord.threads import Thread
 
     from .parameters import Parameter
     from ._types import BotT, _Bot
     from .context import Context
 
 __all__ = (
     'Converter',
@@ -94,19 +94,19 @@
     for guild in bot.guilds:
         result = getattr(guild, getter)(argument)
         if result:
             return result
     return result
 
 
-_utils_get = discord.utils.get
+_utils_get = tonkord.utils.get
 T = TypeVar('T')
 T_co = TypeVar('T_co', covariant=True)
-CT = TypeVar('CT', bound=discord.abc.GuildChannel)
-TT = TypeVar('TT', bound=discord.Thread)
+CT = TypeVar('CT', bound=tonkord.abc.GuildChannel)
+TT = TypeVar('TT', bound=tonkord.Thread)
 
 
 @runtime_checkable
 class Converter(Protocol[T_co]):
     """The base class of custom converters that require the :class:`.Context`
     to be passed to be useful.
 
@@ -148,39 +148,39 @@
 
 class IDConverter(Converter[T_co]):
     @staticmethod
     def _get_id_match(argument):
         return _ID_REGEX.match(argument)
 
 
-class ObjectConverter(IDConverter[discord.Object]):
+class ObjectConverter(IDConverter[tonkord.Object]):
     """Converts to a :class:`~discord.Object`.
 
     The argument must follow the valid ID or mention formats (e.g. ``<@80088516616269824>``).
 
     .. versionadded:: 2.0
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by member, role, or channel mention.
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Object:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Object:
         match = self._get_id_match(argument) or re.match(r'<(?:@(?:!|&)?|#)([0-9]{15,20})>$', argument)
 
         if match is None:
             raise ObjectNotFound(argument)
 
         result = int(match.group(1))
 
-        return discord.Object(id=result)
+        return tonkord.Object(id=result)
 
 
-class MemberConverter(IDConverter[discord.Member]):
+class MemberConverter(IDConverter[tonkord.Member]):
     """Converts to a :class:`~discord.Member`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
@@ -200,15 +200,15 @@
         optionally caching the result if :attr:`.MemberCacheFlags.joined` is enabled.
 
     .. deprecated:: 2.3
         Looking up users by discriminator will be removed in a future version due to
         the removal of discriminators in an API change.
     """
 
-    async def query_member_named(self, guild: discord.Guild, argument: str) -> Optional[discord.Member]:
+    async def query_member_named(self, guild: tonkord.Guild, argument: str) -> Optional[tonkord.Member]:
         cache = guild._state.member_cache_flags.joined
         username, _, discriminator = argument.rpartition('#')
 
         # If # isn't found then "discriminator" actually has the username
         if not username:
             discriminator, username = username, discriminator
 
@@ -216,38 +216,38 @@
             lookup = username
             predicate = lambda m: m.name == username and m.discriminator == discriminator
         else:
             lookup = argument
             predicate = lambda m: m.name == argument or m.global_name == argument or m.nick == argument
 
         members = await guild.query_members(lookup, limit=100, cache=cache)
-        return discord.utils.find(predicate, members)
+        return tonkord.utils.find(predicate, members)
 
-    async def query_member_by_id(self, bot: _Bot, guild: discord.Guild, user_id: int) -> Optional[discord.Member]:
+    async def query_member_by_id(self, bot: _Bot, guild: tonkord.Guild, user_id: int) -> Optional[tonkord.Member]:
         ws = bot._get_websocket(shard_id=guild.shard_id)
         cache = guild._state.member_cache_flags.joined
         if ws.is_ratelimited():
             # If we're being rate limited on the WS, then fall back to using the HTTP API
             # So we don't have to wait ~60 seconds for the query to finish
             try:
                 member = await guild.fetch_member(user_id)
-            except discord.HTTPException:
+            except tonkord.HTTPException:
                 return None
 
             if cache:
                 guild._add_member(member)
             return member
 
         # If we're not being rate limited then we can use the websocket to actually query
         members = await guild.query_members(limit=1, user_ids=[user_id], cache=cache)
         if not members:
             return None
         return members[0]
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Member:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Member:
         bot = ctx.bot
         match = self._get_id_match(argument) or re.match(r'<@!?([0-9]{15,20})>$', argument)
         guild = ctx.guild
         result = None
         user_id = None
 
         if match is None:
@@ -259,30 +259,30 @@
         else:
             user_id = int(match.group(1))
             if guild:
                 result = guild.get_member(user_id) or _utils_get(ctx.message.mentions, id=user_id)
             else:
                 result = _get_from_guilds(bot, 'get_member', user_id)
 
-        if not isinstance(result, discord.Member):
+        if not isinstance(result, tonkord.Member):
             if guild is None:
                 raise MemberNotFound(argument)
 
             if user_id is not None:
                 result = await self.query_member_by_id(bot, guild, user_id)
             else:
                 result = await self.query_member_named(guild, argument)
 
             if not result:
                 raise MemberNotFound(argument)
 
         return result
 
 
-class UserConverter(IDConverter[discord.User]):
+class UserConverter(IDConverter[tonkord.User]):
     """Converts to a :class:`~discord.User`.
 
     All lookups are via the global user cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
@@ -300,26 +300,26 @@
         and it's not available in cache.
 
     .. deprecated:: 2.3
         Looking up users by discriminator will be removed in a future version due to
         the removal of discriminators in an API change.
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.User:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.User:
         match = self._get_id_match(argument) or re.match(r'<@!?([0-9]{15,20})>$', argument)
         result = None
         state = ctx._state
 
         if match is not None:
             user_id = int(match.group(1))
             result = ctx.bot.get_user(user_id) or _utils_get(ctx.message.mentions, id=user_id)
             if result is None:
                 try:
                     result = await ctx.bot.fetch_user(user_id)
-                except discord.HTTPException:
+                except tonkord.HTTPException:
                     raise UserNotFound(argument) from None
 
             return result  # type: ignore
 
         username, _, discriminator = argument.rpartition('#')
 
         # If # isn't found then "discriminator" actually has the username
@@ -327,22 +327,22 @@
             discriminator, username = username, discriminator
 
         if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
             predicate = lambda u: u.name == username and u.discriminator == discriminator
         else:
             predicate = lambda u: u.name == argument or u.global_name == argument
 
-        result = discord.utils.find(predicate, state._users.values())
+        result = tonkord.utils.find(predicate, state._users.values())
         if result is None:
             raise UserNotFound(argument)
 
         return result
 
 
-class PartialMessageConverter(Converter[discord.PartialMessage]):
+class PartialMessageConverter(Converter[tonkord.PartialMessage]):
     """Converts to a :class:`discord.PartialMessage`.
 
     .. versionadded:: 1.7
 
     The creation strategy is as follows (in order):
 
     1. By "{channel ID}-{message ID}" (retrieved by shift-clicking on "Copy ID")
@@ -358,15 +358,15 @@
             r'(?P<guild_id>[0-9]{15,20}|@me)'
             r'/(?P<channel_id>[0-9]{15,20})/(?P<message_id>[0-9]{15,20})/?$'
         )
         match = id_regex.match(argument) or link_regex.match(argument)
         if not match:
             raise MessageNotFound(argument)
         data = match.groupdict()
-        channel_id = discord.utils._get_as_snowflake(data, 'channel_id') or ctx.channel.id
+        channel_id = tonkord.utils._get_as_snowflake(data, 'channel_id') or ctx.channel.id
         message_id = int(data['message_id'])
         guild_id = data.get('guild_id')
         if guild_id is None:
             guild_id = ctx.guild and ctx.guild.id
         elif guild_id == '@me':
             guild_id = None
         else:
@@ -385,90 +385,90 @@
             guild = ctx.bot.get_guild(guild_id)
             if guild is None:
                 return None
             return guild._resolve_channel(channel_id)
 
         return ctx.bot.get_channel(channel_id)
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.PartialMessage:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.PartialMessage:
         guild_id, message_id, channel_id = self._get_id_matches(ctx, argument)
         channel = self._resolve_channel(ctx, guild_id, channel_id)
-        if not channel or not isinstance(channel, discord.abc.Messageable):
+        if not channel or not isinstance(channel, tonkord.abc.Messageable):
             raise ChannelNotFound(channel_id)
-        return discord.PartialMessage(channel=channel, id=message_id)
+        return tonkord.PartialMessage(channel=channel, id=message_id)
 
 
-class MessageConverter(IDConverter[discord.Message]):
+class MessageConverter(IDConverter[tonkord.Message]):
     """Converts to a :class:`discord.Message`.
 
     .. versionadded:: 1.1
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by "{channel ID}-{message ID}" (retrieved by shift-clicking on "Copy ID")
     2. Lookup by message ID (the message **must** be in the context channel)
     3. Lookup by message URL
 
     .. versionchanged:: 1.5
          Raise :exc:`.ChannelNotFound`, :exc:`.MessageNotFound` or :exc:`.ChannelNotReadable` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Message:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Message:
         guild_id, message_id, channel_id = PartialMessageConverter._get_id_matches(ctx, argument)
         message = ctx.bot._connection._get_message(message_id)
         if message:
             return message
         channel = PartialMessageConverter._resolve_channel(ctx, guild_id, channel_id)
-        if not channel or not isinstance(channel, discord.abc.Messageable):
+        if not channel or not isinstance(channel, tonkord.abc.Messageable):
             raise ChannelNotFound(channel_id)
         try:
             return await channel.fetch_message(message_id)
-        except discord.NotFound:
+        except tonkord.NotFound:
             raise MessageNotFound(argument)
-        except discord.Forbidden:
+        except tonkord.Forbidden:
             raise ChannelNotReadable(channel)  # type: ignore # type-checker thinks channel could be a DMChannel at this point
 
 
-class GuildChannelConverter(IDConverter[discord.abc.GuildChannel]):
+class GuildChannelConverter(IDConverter[tonkord.abc.GuildChannel]):
     """Converts to a :class:`~discord.abc.GuildChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by name.
 
     .. versionadded:: 2.0
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.abc.GuildChannel:
-        return self._resolve_channel(ctx, argument, 'channels', discord.abc.GuildChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.abc.GuildChannel:
+        return self._resolve_channel(ctx, argument, 'channels', tonkord.abc.GuildChannel)
 
     @staticmethod
     def _resolve_channel(ctx: Context[BotT], argument: str, attribute: str, type: Type[CT]) -> CT:
         bot = ctx.bot
 
         match = IDConverter._get_id_match(argument) or re.match(r'<#([0-9]{15,20})>$', argument)
         result = None
         guild = ctx.guild
 
         if match is None:
             # not a mention
             if guild:
                 iterable: Iterable[CT] = getattr(guild, attribute)
-                result: Optional[CT] = discord.utils.get(iterable, name=argument)
+                result: Optional[CT] = tonkord.utils.get(iterable, name=argument)
             else:
 
                 def check(c):
                     return isinstance(c, type) and c.name == argument
 
-                result = discord.utils.find(check, bot.get_all_channels())  # type: ignore
+                result = tonkord.utils.find(check, bot.get_all_channels())  # type: ignore
         else:
             channel_id = int(match.group(1))
             if guild:
                 # guild.get_channel returns an explicit union instead of the base class
                 result = guild.get_channel(channel_id)  # type: ignore
             else:
                 result = _get_from_guilds(bot, 'get_channel', channel_id)
@@ -484,27 +484,27 @@
         result = None
         guild = ctx.guild
 
         if match is None:
             # not a mention
             if guild:
                 iterable: Iterable[TT] = getattr(guild, attribute)
-                result: Optional[TT] = discord.utils.get(iterable, name=argument)
+                result: Optional[TT] = tonkord.utils.get(iterable, name=argument)
         else:
             thread_id = int(match.group(1))
             if guild:
                 result = guild.get_thread(thread_id)  # type: ignore
 
         if not result or not isinstance(result, type):
             raise ThreadNotFound(argument)
 
         return result
 
 
-class TextChannelConverter(IDConverter[discord.TextChannel]):
+class TextChannelConverter(IDConverter[tonkord.TextChannel]):
     """Converts to a :class:`~discord.TextChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
@@ -512,19 +512,19 @@
     2. Lookup by mention.
     3. Lookup by name
 
     .. versionchanged:: 1.5
          Raise :exc:`.ChannelNotFound` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.TextChannel:
-        return GuildChannelConverter._resolve_channel(ctx, argument, 'text_channels', discord.TextChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.TextChannel:
+        return GuildChannelConverter._resolve_channel(ctx, argument, 'text_channels', tonkord.TextChannel)
 
 
-class VoiceChannelConverter(IDConverter[discord.VoiceChannel]):
+class VoiceChannelConverter(IDConverter[tonkord.VoiceChannel]):
     """Converts to a :class:`~discord.VoiceChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
@@ -532,38 +532,38 @@
     2. Lookup by mention.
     3. Lookup by name
 
     .. versionchanged:: 1.5
          Raise :exc:`.ChannelNotFound` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.VoiceChannel:
-        return GuildChannelConverter._resolve_channel(ctx, argument, 'voice_channels', discord.VoiceChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.VoiceChannel:
+        return GuildChannelConverter._resolve_channel(ctx, argument, 'voice_channels', tonkord.VoiceChannel)
 
 
-class StageChannelConverter(IDConverter[discord.StageChannel]):
+class StageChannelConverter(IDConverter[tonkord.StageChannel]):
     """Converts to a :class:`~discord.StageChannel`.
 
     .. versionadded:: 1.7
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.StageChannel:
-        return GuildChannelConverter._resolve_channel(ctx, argument, 'stage_channels', discord.StageChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.StageChannel:
+        return GuildChannelConverter._resolve_channel(ctx, argument, 'stage_channels', tonkord.StageChannel)
 
 
-class CategoryChannelConverter(IDConverter[discord.CategoryChannel]):
+class CategoryChannelConverter(IDConverter[tonkord.CategoryChannel]):
     """Converts to a :class:`~discord.CategoryChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
@@ -571,56 +571,56 @@
     2. Lookup by mention.
     3. Lookup by name
 
     .. versionchanged:: 1.5
          Raise :exc:`.ChannelNotFound` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.CategoryChannel:
-        return GuildChannelConverter._resolve_channel(ctx, argument, 'categories', discord.CategoryChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.CategoryChannel:
+        return GuildChannelConverter._resolve_channel(ctx, argument, 'categories', tonkord.CategoryChannel)
 
 
-class ThreadConverter(IDConverter[discord.Thread]):
+class ThreadConverter(IDConverter[tonkord.Thread]):
     """Converts to a :class:`~discord.Thread`.
 
     All lookups are via the local guild.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by name.
 
     .. versionadded: 2.0
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Thread:
-        return GuildChannelConverter._resolve_thread(ctx, argument, 'threads', discord.Thread)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Thread:
+        return GuildChannelConverter._resolve_thread(ctx, argument, 'threads', tonkord.Thread)
 
 
-class ForumChannelConverter(IDConverter[discord.ForumChannel]):
+class ForumChannelConverter(IDConverter[tonkord.ForumChannel]):
     """Converts to a :class:`~discord.ForumChannel`.
 
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by name
 
     .. versionadded:: 2.0
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.ForumChannel:
-        return GuildChannelConverter._resolve_channel(ctx, argument, 'forums', discord.ForumChannel)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.ForumChannel:
+        return GuildChannelConverter._resolve_channel(ctx, argument, 'forums', tonkord.ForumChannel)
 
 
-class ColourConverter(Converter[discord.Colour]):
+class ColourConverter(Converter[tonkord.Colour]):
     """Converts to a :class:`~discord.Colour`.
 
     .. versionchanged:: 1.5
         Add an alias named ColorConverter
 
     The following formats are accepted:
 
@@ -638,29 +638,29 @@
     .. versionchanged:: 1.5
          Raise :exc:`.BadColourArgument` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.7
         Added support for ``rgb`` function and 3-digit hex shortcuts
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Colour:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Colour:
         try:
-            return discord.Colour.from_str(argument)
+            return tonkord.Colour.from_str(argument)
         except ValueError:
             arg = argument.lower().replace(' ', '_')
-            method = getattr(discord.Colour, arg, None)
+            method = getattr(tonkord.Colour, arg, None)
             if arg.startswith('from_') or method is None or not inspect.ismethod(method):
                 raise BadColourArgument(arg)
             return method()
 
 
 ColorConverter = ColourConverter
 
 
-class RoleConverter(IDConverter[discord.Role]):
+class RoleConverter(IDConverter[tonkord.Role]):
     """Converts to a :class:`~discord.Role`.
 
     All lookups are via the local guild. If in a DM context, the converter raises
     :exc:`.NoPrivateMessage` exception.
 
     The lookup strategy is as follows (in order):
 
@@ -668,82 +668,82 @@
     2. Lookup by mention.
     3. Lookup by name
 
     .. versionchanged:: 1.5
          Raise :exc:`.RoleNotFound` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Role:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Role:
         guild = ctx.guild
         if not guild:
             raise NoPrivateMessage()
 
         match = self._get_id_match(argument) or re.match(r'<@&([0-9]{15,20})>$', argument)
         if match:
             result = guild.get_role(int(match.group(1)))
         else:
-            result = discord.utils.get(guild._roles.values(), name=argument)
+            result = tonkord.utils.get(guild._roles.values(), name=argument)
 
         if result is None:
             raise RoleNotFound(argument)
         return result
 
 
-class GameConverter(Converter[discord.Game]):
+class GameConverter(Converter[tonkord.Game]):
     """Converts to a :class:`~discord.Game`."""
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Game:
-        return discord.Game(name=argument)
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Game:
+        return tonkord.Game(name=argument)
 
 
-class InviteConverter(Converter[discord.Invite]):
+class InviteConverter(Converter[tonkord.Invite]):
     """Converts to a :class:`~discord.Invite`.
 
     This is done via an HTTP request using :meth:`.Bot.fetch_invite`.
 
     .. versionchanged:: 1.5
          Raise :exc:`.BadInviteArgument` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Invite:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Invite:
         try:
             invite = await ctx.bot.fetch_invite(argument)
             return invite
         except Exception as exc:
             raise BadInviteArgument(argument) from exc
 
 
-class GuildConverter(IDConverter[discord.Guild]):
+class GuildConverter(IDConverter[tonkord.Guild]):
     """Converts to a :class:`~discord.Guild`.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by name. (There is no disambiguation for Guilds with multiple matching names).
 
     .. versionadded:: 1.7
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Guild:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Guild:
         match = self._get_id_match(argument)
         result = None
 
         if match is not None:
             guild_id = int(match.group(1))
             result = ctx.bot.get_guild(guild_id)
 
         if result is None:
-            result = discord.utils.get(ctx.bot.guilds, name=argument)
+            result = tonkord.utils.get(ctx.bot.guilds, name=argument)
 
             if result is None:
                 raise GuildNotFound(argument)
         return result
 
 
-class EmojiConverter(IDConverter[discord.Emoji]):
+class EmojiConverter(IDConverter[tonkord.Emoji]):
     """Converts to a :class:`~discord.Emoji`.
 
     All lookups are done for the local guild first, if available. If that lookup
     fails, then it checks the client's global cache.
 
     The lookup strategy is as follows (in order):
 
@@ -751,118 +751,118 @@
     2. Lookup by extracting ID from the emoji.
     3. Lookup by name
 
     .. versionchanged:: 1.5
          Raise :exc:`.EmojiNotFound` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.Emoji:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.Emoji:
         match = self._get_id_match(argument) or re.match(r'<a?:[a-zA-Z0-9\_]{1,32}:([0-9]{15,20})>$', argument)
         result = None
         bot = ctx.bot
         guild = ctx.guild
 
         if match is None:
             # Try to get the emoji by name. Try local guild first.
             if guild:
-                result = discord.utils.get(guild.emojis, name=argument)
+                result = tonkord.utils.get(guild.emojis, name=argument)
 
             if result is None:
-                result = discord.utils.get(bot.emojis, name=argument)
+                result = tonkord.utils.get(bot.emojis, name=argument)
         else:
             emoji_id = int(match.group(1))
 
             # Try to look up emoji by id.
             result = bot.get_emoji(emoji_id)
 
         if result is None:
             raise EmojiNotFound(argument)
 
         return result
 
 
-class PartialEmojiConverter(Converter[discord.PartialEmoji]):
+class PartialEmojiConverter(Converter[tonkord.PartialEmoji]):
     """Converts to a :class:`~discord.PartialEmoji`.
 
     This is done by extracting the animated flag, name and ID from the emoji.
 
     .. versionchanged:: 1.5
          Raise :exc:`.PartialEmojiConversionFailure` instead of generic :exc:`.BadArgument`
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.PartialEmoji:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.PartialEmoji:
         match = re.match(r'<(a?):([a-zA-Z0-9\_]{1,32}):([0-9]{15,20})>$', argument)
 
         if match:
             emoji_animated = bool(match.group(1))
             emoji_name = match.group(2)
             emoji_id = int(match.group(3))
 
-            return discord.PartialEmoji.with_state(
+            return tonkord.PartialEmoji.with_state(
                 ctx.bot._connection, animated=emoji_animated, name=emoji_name, id=emoji_id
             )
 
         raise PartialEmojiConversionFailure(argument)
 
 
-class GuildStickerConverter(IDConverter[discord.GuildSticker]):
+class GuildStickerConverter(IDConverter[tonkord.GuildSticker]):
     """Converts to a :class:`~discord.GuildSticker`.
 
     All lookups are done for the local guild first, if available. If that lookup
     fails, then it checks the client's global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by name.
 
     .. versionadded:: 2.0
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.GuildSticker:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.GuildSticker:
         match = self._get_id_match(argument)
         result = None
         bot = ctx.bot
         guild = ctx.guild
 
         if match is None:
             # Try to get the sticker by name. Try local guild first.
             if guild:
-                result = discord.utils.get(guild.stickers, name=argument)
+                result = tonkord.utils.get(guild.stickers, name=argument)
 
             if result is None:
-                result = discord.utils.get(bot.stickers, name=argument)
+                result = tonkord.utils.get(bot.stickers, name=argument)
         else:
             sticker_id = int(match.group(1))
 
             # Try to look up sticker by id.
             result = bot.get_sticker(sticker_id)
 
         if result is None:
             raise GuildStickerNotFound(argument)
 
         return result
 
 
-class ScheduledEventConverter(IDConverter[discord.ScheduledEvent]):
+class ScheduledEventConverter(IDConverter[tonkord.ScheduledEvent]):
     """Converts to a :class:`~discord.ScheduledEvent`.
 
     Lookups are done for the local guild if available. Otherwise, for a DM context,
     lookup is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by url.
     3. Lookup by name.
 
     .. versionadded:: 2.0
     """
 
-    async def convert(self, ctx: Context[BotT], argument: str) -> discord.ScheduledEvent:
+    async def convert(self, ctx: Context[BotT], argument: str) -> tonkord.ScheduledEvent:
         guild = ctx.guild
         match = self._get_id_match(argument)
         result = None
 
         if match:
             # ID match
             event_id = int(match.group(1))
@@ -886,18 +886,18 @@
 
                 if guild:
                     event_id = int(match.group('event_id'))
                     result = guild.get_scheduled_event(event_id)
             else:
                 # lookup by name
                 if guild:
-                    result = discord.utils.get(guild.scheduled_events, name=argument)
+                    result = tonkord.utils.get(guild.scheduled_events, name=argument)
                 else:
                     for guild in ctx.bot.guilds:
-                        result = discord.utils.get(guild.scheduled_events, name=argument)
+                        result = tonkord.utils.get(guild.scheduled_events, name=argument)
                         if result:
                             break
         if result is None:
             raise ScheduledEventNotFound(argument)
 
         return result
 
@@ -979,20 +979,20 @@
             type = match[1]
             id = int(match[2])
             transformed = transforms[type](id)
             return transformed
 
         result = re.sub(r'<(@[!&]?|#)([0-9]{15,20})>', repl, argument)
         if self.escape_markdown:
-            result = discord.utils.escape_markdown(result)
+            result = tonkord.utils.escape_markdown(result)
         elif self.remove_markdown:
-            result = discord.utils.remove_markdown(result)
+            result = tonkord.utils.remove_markdown(result)
 
         # Completely ensure no mentions escape:
-        return discord.utils.escape_mentions(result)
+        return tonkord.utils.escape_mentions(result)
 
 
 class Greedy(List[T]):
     r"""A special converter that greedily consumes arguments until it can't.
     As a consequence of this behaviour, most input errors are silently discarded,
     since it is used as an indicator of when to stop parsing.
 
@@ -1032,15 +1032,15 @@
         if not isinstance(params, tuple):
             params = (params,)
         if len(params) != 1:
             raise TypeError('Greedy[...] only takes a single argument')
         converter = params[0]
 
         args = getattr(converter, '__args__', ())
-        if discord.utils.PY_310 and converter.__class__ is types.UnionType:  # type: ignore
+        if tonkord.utils.PY_310 and converter.__class__ is types.UnionType:  # type: ignore
             converter = Union[args]  # type: ignore
 
         origin = getattr(converter, '__origin__', None)
 
         if not (callable(converter) or isinstance(converter, Converter) or origin is not None):
             raise TypeError('Greedy[...] expects a type or a Converter instance.')
 
@@ -1189,35 +1189,35 @@
 
 
 def is_generic_type(tp: Any, *, _GenericAlias: type = _GenericAlias) -> bool:
     return isinstance(tp, type) and issubclass(tp, Generic) or isinstance(tp, _GenericAlias)
 
 
 CONVERTER_MAPPING: Dict[type, Any] = {
-    discord.Object: ObjectConverter,
-    discord.Member: MemberConverter,
-    discord.User: UserConverter,
-    discord.Message: MessageConverter,
-    discord.PartialMessage: PartialMessageConverter,
-    discord.TextChannel: TextChannelConverter,
-    discord.Invite: InviteConverter,
-    discord.Guild: GuildConverter,
-    discord.Role: RoleConverter,
-    discord.Game: GameConverter,
-    discord.Colour: ColourConverter,
-    discord.VoiceChannel: VoiceChannelConverter,
-    discord.StageChannel: StageChannelConverter,
-    discord.Emoji: EmojiConverter,
-    discord.PartialEmoji: PartialEmojiConverter,
-    discord.CategoryChannel: CategoryChannelConverter,
-    discord.Thread: ThreadConverter,
-    discord.abc.GuildChannel: GuildChannelConverter,
-    discord.GuildSticker: GuildStickerConverter,
-    discord.ScheduledEvent: ScheduledEventConverter,
-    discord.ForumChannel: ForumChannelConverter,
+    tonkord.Object: ObjectConverter,
+    tonkord.Member: MemberConverter,
+    tonkord.User: UserConverter,
+    tonkord.Message: MessageConverter,
+    tonkord.PartialMessage: PartialMessageConverter,
+    tonkord.TextChannel: TextChannelConverter,
+    tonkord.Invite: InviteConverter,
+    tonkord.Guild: GuildConverter,
+    tonkord.Role: RoleConverter,
+    tonkord.Game: GameConverter,
+    tonkord.Colour: ColourConverter,
+    tonkord.VoiceChannel: VoiceChannelConverter,
+    tonkord.StageChannel: StageChannelConverter,
+    tonkord.Emoji: EmojiConverter,
+    tonkord.PartialEmoji: PartialEmojiConverter,
+    tonkord.CategoryChannel: CategoryChannelConverter,
+    tonkord.Thread: ThreadConverter,
+    tonkord.abc.GuildChannel: GuildChannelConverter,
+    tonkord.GuildSticker: GuildStickerConverter,
+    tonkord.ScheduledEvent: ScheduledEventConverter,
+    tonkord.ForumChannel: ForumChannelConverter,
 }
 
 
 async def _actual_conversion(ctx: Context[BotT], converter: Any, argument: str, param: inspect.Parameter):
     if converter is bool:
         return _convert_to_bool(argument)
 
@@ -1232,15 +1232,15 @@
     try:
         if inspect.isclass(converter) and issubclass(converter, Converter):
             if inspect.ismethod(converter.convert):
                 return await converter.convert(ctx, argument)
             else:
                 return await converter().convert(ctx, argument)
         elif isinstance(converter, Converter):
-            return await converter.convert(ctx, argument)  # type: ignore
+            return await converter.convert(ctx, argument)
     except CommandError:
         raise
     except Exception as exc:
         raise ConversionError(converter, exc) from exc  # type: ignore
 
     try:
         return converter(argument)
```

### Comparing `tonkord.py-2.0/tonkord/ext/commands/cooldowns.py` & `tonkord.py-2.2.2/tonkord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/core.py` & `tonkord.py-2.2.2/tonkord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/errors.py` & `tonkord.py-2.2.2/tonkord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/flags.py` & `tonkord.py-2.2.2/tonkord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/help.py` & `tonkord.py-2.2.2/tonkord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/hybrid.py` & `tonkord.py-2.2.2/tonkord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/parameters.py` & `tonkord.py-2.2.2/tonkord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/commands/view.py` & `tonkord.py-2.2.2/tonkord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ext/tasks/__init__.py` & `tonkord.py-2.2.2/tonkord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/file.py` & `tonkord.py-2.2.2/tonkord/file.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/flags.py` & `tonkord.py-2.2.2/tonkord/flags.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/gateway.py` & `tonkord.py-2.2.2/tonkord/gateway.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/guild.py` & `tonkord.py-2.2.2/tonkord/guild.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/http.py` & `tonkord.py-2.2.2/tonkord/http.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/integrations.py` & `tonkord.py-2.2.2/tonkord/integrations.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/interactions.py` & `tonkord.py-2.2.2/tonkord/interactions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/invite.py` & `tonkord.py-2.2.2/tonkord/invite.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/member.py` & `tonkord.py-2.2.2/tonkord/member.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/mentions.py` & `tonkord.py-2.2.2/tonkord/mentions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/message.py` & `tonkord.py-2.2.2/tonkord/message.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/mixins.py` & `tonkord.py-2.2.2/tonkord/mixins.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/object.py` & `tonkord.py-2.2.2/tonkord/object.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/oggparse.py` & `tonkord.py-2.2.2/tonkord/oggparse.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/opus.py` & `tonkord.py-2.2.2/tonkord/opus.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/partial_emoji.py` & `tonkord.py-2.2.2/tonkord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/permissions.py` & `tonkord.py-2.2.2/tonkord/permissions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/player.py` & `tonkord.py-2.2.2/tonkord/player.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/raw_models.py` & `tonkord.py-2.2.2/tonkord/raw_models.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/reaction.py` & `tonkord.py-2.2.2/tonkord/reaction.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/role.py` & `tonkord.py-2.2.2/tonkord/role.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/scheduled_event.py` & `tonkord.py-2.2.2/tonkord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/shard.py` & `tonkord.py-2.2.2/tonkord/shard.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/sku.py` & `tonkord.py-2.2.2/tonkord/sku.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/stage_instance.py` & `tonkord.py-2.2.2/tonkord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/state.py` & `tonkord.py-2.2.2/tonkord/state.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/sticker.py` & `tonkord.py-2.2.2/tonkord/sticker.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/team.py` & `tonkord.py-2.2.2/tonkord/team.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/template.py` & `tonkord.py-2.2.2/tonkord/template.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/threads.py` & `tonkord.py-2.2.2/tonkord/threads.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/activity.py` & `tonkord.py-2.2.2/tonkord/types/activity.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/appinfo.py` & `tonkord.py-2.2.2/tonkord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/audit_log.py` & `tonkord.py-2.2.2/tonkord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/automod.py` & `tonkord.py-2.2.2/tonkord/types/automod.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/channel.py` & `tonkord.py-2.2.2/tonkord/types/channel.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/command.py` & `tonkord.py-2.2.2/tonkord/types/command.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/components.py` & `tonkord.py-2.2.2/tonkord/types/components.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/embed.py` & `tonkord.py-2.2.2/tonkord/types/embed.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/emoji.py` & `tonkord.py-2.2.2/tonkord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/gateway.py` & `tonkord.py-2.2.2/tonkord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/guild.py` & `tonkord.py-2.2.2/tonkord/types/guild.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/integration.py` & `tonkord.py-2.2.2/tonkord/types/integration.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/interactions.py` & `tonkord.py-2.2.2/tonkord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/invite.py` & `tonkord.py-2.2.2/tonkord/types/invite.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/member.py` & `tonkord.py-2.2.2/tonkord/types/member.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/message.py` & `tonkord.py-2.2.2/tonkord/types/message.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/role.py` & `tonkord.py-2.2.2/tonkord/types/role.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/scheduled_event.py` & `tonkord.py-2.2.2/tonkord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/sku.py` & `tonkord.py-2.2.2/tonkord/types/sku.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/snowflake.py` & `tonkord.py-2.2.2/tonkord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/sticker.py` & `tonkord.py-2.2.2/tonkord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/team.py` & `tonkord.py-2.2.2/tonkord/types/team.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/template.py` & `tonkord.py-2.2.2/tonkord/types/template.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/threads.py` & `tonkord.py-2.2.2/tonkord/types/threads.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/user.py` & `tonkord.py-2.2.2/tonkord/types/user.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/voice.py` & `tonkord.py-2.2.2/tonkord/types/voice.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/webhook.py` & `tonkord.py-2.2.2/tonkord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/welcome_screen.py` & `tonkord.py-2.2.2/tonkord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/types/widget.py` & `tonkord.py-2.2.2/tonkord/types/widget.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/button.py` & `tonkord.py-2.2.2/tonkord/ui/button.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/dynamic.py` & `tonkord.py-2.2.2/tonkord/ui/dynamic.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/item.py` & `tonkord.py-2.2.2/tonkord/ui/item.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/modal.py` & `tonkord.py-2.2.2/tonkord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/select.py` & `tonkord.py-2.2.2/tonkord/ui/select.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/text_input.py` & `tonkord.py-2.2.2/tonkord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/ui/view.py` & `tonkord.py-2.2.2/tonkord/ui/view.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/user.py` & `tonkord.py-2.2.2/tonkord/user.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/utils.py` & `tonkord.py-2.2.2/tonkord/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
 
 
 if HAS_ORJSON:
 
     def _to_json(obj: Any) -> str:
         return orjson.dumps(obj).decode('utf-8')
 
-    _from_json = orjson.loads  # type: ignore
+    _from_json = orjson.loads
 
 else:
 
     def _to_json(obj: Any) -> str:
         return json.dumps(obj, separators=(',', ':'), ensure_ascii=True)
 
     _from_json = json.loads
```

### Comparing `tonkord.py-2.0/tonkord/voice_client.py` & `tonkord.py-2.2.2/tonkord/voice_client.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/voice_state.py` & `tonkord.py-2.2.2/tonkord/voice_state.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/webhook/async_.py` & `tonkord.py-2.2.2/tonkord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/webhook/sync.py` & `tonkord.py-2.2.2/tonkord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/welcome_screen.py` & `tonkord.py-2.2.2/tonkord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord/widget.py` & `tonkord.py-2.2.2/tonkord/widget.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord.py.egg-info/PKG-INFO` & `tonkord.py-2.2.2/tonkord.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkord.py
-Version: 2.0
+Version: 2.2.2
 Summary: A Python wrapper for the Discord API
 Home-page: https://9tonkla.cloud
 Author: tonkoranit
 License: MIT
 Project-URL: Documentation, https://9tonkla.cloud
 Project-URL: Issue tracker, https://9tonkla.cloud
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tonkord.py-2.0/tonkord.py.egg-info/SOURCES.txt` & `tonkord.py-2.2.2/tonkord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tonkord.py-2.0/tonkord.py.egg-info/requires.txt` & `tonkord.py-2.2.2/tonkord.py.egg-info/requires.txt`

 * *Files identical despite different names*

