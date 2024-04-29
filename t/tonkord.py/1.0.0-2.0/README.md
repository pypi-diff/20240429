# Comparing `tmp/tonkord.py-1.0.0.tar.gz` & `tmp/tonkord.py-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonkord.py-1.0.0.tar", last modified: Mon Apr 29 11:52:08 2024, max compression
+gzip compressed data, was "tonkord.py-2.0.tar", last modified: Mon Apr 29 11:55:12 2024, max compression
```

## Comparing `tonkord.py-1.0.0.tar` & `tonkord.py-2.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.144821 tonkord.py-1.0.0/
--rw-rw-rw-   0        0        0     1102 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      116 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2575 2024-04-29 11:52:08.143824 tonkord.py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-04-29 11:16:51.000000 tonkord.py-1.0.0/README.rst
--rw-rw-rw-   0        0        0      919 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       67 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:52:08.144821 tonkord.py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3512 2024-04-29 11:48:28.000000 tonkord.py-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.057111 tonkord.py-1.0.0/tests/
--rw-rw-rw-   0        0        0     2188 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_annotated_annotation.py
--rw-rw-rw-   0        0        0     5361 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_app_commands_autocomplete.py
--rw-rw-rw-   0        0        0    10738 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_app_commands_description.py
--rw-rw-rw-   0        0        0    20190 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_app_commands_group.py
--rw-rw-rw-   0        0        0     6780 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_app_commands_invoke.py
--rw-rw-rw-   0        0        0     2213 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_colour.py
--rw-rw-rw-   0        0        0    16294 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_ext_commands_cog.py
--rw-rw-rw-   0        0        0     4894 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_ext_commands_description.py
--rw-rw-rw-   0        0        0     5332 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_ext_tasks.py
--rw-rw-rw-   0        0        0     4153 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_files.py
--rw-rw-rw-   0        0        0    10566 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.099970 tonkord.py-1.0.0/tonkord/
--rw-rw-rw-   0        0        0     1995 2024-04-29 11:52:04.000000 tonkord.py-1.0.0/tonkord/__init__.py
--rw-rw-rw-   0        0        0    11394 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/__main__.py
--rw-rw-rw-   0        0        0     1444 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/_types.py
--rw-rw-rw-   0        0        0    68645 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/abc.py
--rw-rw-rw-   0        0        0    28940 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/activity.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.117909 tonkord.py-1.0.0/tonkord/app_commands/
--rw-rw-rw-   0        0        0      444 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18620 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/checks.py
--rw-rw-rw-   0        0        0    97078 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19748 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/errors.py
--rw-rw-rw-   0        0        0    39593 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/models.py
--rw-rw-rw-   0        0        0    13386 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    33225 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    11044 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/translator.py
--rw-rw-rw-   0        0        0    49299 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/app_commands/tree.py
--rw-rw-rw-   0        0        0    19929 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/appinfo.py
--rw-rw-rw-   0        0        0    16692 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/asset.py
--rw-rw-rw-   0        0        0    39755 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/audit_logs.py
--rw-rw-rw-   0        0        0    27638 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/automod.py
--rw-rw-rw-   0        0        0     3859 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/backoff.py
--rw-rw-rw-   0        0        0   121700 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/channel.py
--rw-rw-rw-   0        0        0    98085 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/client.py
--rw-rw-rw-   0        0        0    15014 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/colour.py
--rw-rw-rw-   0        0        0    20993 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/components.py
--rw-rw-rw-   0        0        0     3124 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/context_managers.py
--rw-rw-rw-   0        0        0    23479 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/embeds.py
--rw-rw-rw-   0        0        0     8831 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/emoji.py
--rw-rw-rw-   0        0        0    25928 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/enums.py
--rw-rw-rw-   0        0        0     9232 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.048139 tonkord.py-1.0.0/tonkord/ext/
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.124886 tonkord.py-1.0.0/tonkord/ext/commands/
--rw-rw-rw-   0        0        0      458 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2711 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    53628 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    32370 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    41097 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/context.py
--rw-rw-rw-   0        0        0    47543 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/converter.py
--rw-rw-rw-   0        0        0    10006 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    92194 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36964 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    23572 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    59452 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/help.py
--rw-rw-rw-   0        0        0    38076 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     9593 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6443 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.124886 tonkord.py-1.0.0/tonkord/ext/tasks/
--rw-rw-rw-   0        0        0    30480 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5601 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/file.py
--rw-rw-rw-   0        0        0    61982 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/flags.py
--rw-rw-rw-   0        0        0    37212 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/gateway.py
--rw-rw-rw-   0        0        0   160673 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/guild.py
--rw-rw-rw-   0        0        0    97147 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/http.py
--rw-rw-rw-   0        0        0    13751 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/integrations.py
--rw-rw-rw-   0        0        0    48955 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/interactions.py
--rw-rw-rw-   0        0        0    21211 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/invite.py
--rw-rw-rw-   0        0        0    43155 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/member.py
--rw-rw-rw-   0        0        0     5745 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/mentions.py
--rw-rw-rw-   0        0        0    91350 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/message.py
--rw-rw-rw-   0        0        0     1531 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/mixins.py
--rw-rw-rw-   0        0        0     3837 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/object.py
--rw-rw-rw-   0        0        0     3771 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/oggparse.py
--rw-rw-rw-   0        0        0    16882 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/opus.py
--rw-rw-rw-   0        0        0     8223 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/partial_emoji.py
--rw-rw-rw-   0        0        0    32389 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/permissions.py
--rw-rw-rw-   0        0        0    30450 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/player.py
--rw-rw-rw-   0        0        0        0 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/py.typed
--rw-rw-rw-   0        0        0    18600 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/raw_models.py
--rw-rw-rw-   0        0        0     9430 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/reaction.py
--rw-rw-rw-   0        0        0    18745 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/role.py
--rw-rw-rw-   0        0        0    24311 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/scheduled_event.py
--rw-rw-rw-   0        0        0    21301 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/shard.py
--rw-rw-rw-   0        0        0     6871 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/sku.py
--rw-rw-rw-   0        0        0     6690 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/stage_instance.py
--rw-rw-rw-   0        0        0    77030 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/state.py
--rw-rw-rw-   0        0        0    16713 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/sticker.py
--rw-rw-rw-   0        0        0     5164 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/team.py
--rw-rw-rw-   0        0        0     9736 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/template.py
--rw-rw-rw-   0        0        0    33420 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/threads.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.136847 tonkord.py-1.0.0/tonkord/types/
--rw-rw-rw-   0        0        0      159 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/__init__.py
--rw-rw-rw-   0        0        0     2841 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/activity.py
--rw-rw-rw-   0        0        0     2550 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/appinfo.py
--rw-rw-rw-   0        0        0     8870 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/audit_log.py
--rw-rw-rw-   0        0        0     4184 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/automod.py
--rw-rw-rw-   0        0        0     5131 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/channel.py
--rw-rw-rw-   0        0        0     6484 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/command.py
--rw-rw-rw-   0        0        0     3606 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/components.py
--rw-rw-rw-   0        0        0     2419 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/embed.py
--rw-rw-rw-   0        0        0     1574 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/emoji.py
--rw-rw-rw-   0        0        0     9128 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/gateway.py
--rw-rw-rw-   0        0        0     5781 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/guild.py
--rw-rw-rw-   0        0        0     2370 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/integration.py
--rw-rw-rw-   0        0        0     7421 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/interactions.py
--rw-rw-rw-   0        0        0     2797 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/invite.py
--rw-rw-rw-   0        0        0     2155 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/member.py
--rw-rw-rw-   0        0        0     4840 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/message.py
--rw-rw-rw-   0        0        0     1815 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/role.py
--rw-rw-rw-   0        0        0     3405 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1657 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/sku.py
--rw-rw-rw-   0        0        0     1210 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/snowflake.py
--rw-rw-rw-   0        0        0     2343 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/sticker.py
--rw-rw-rw-   0        0        0     1607 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/team.py
--rw-rw-rw-   0        0        0     1658 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/template.py
--rw-rw-rw-   0        0        0     2534 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/threads.py
--rw-rw-rw-   0        0        0     1813 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/user.py
--rw-rw-rw-   0        0        0     2352 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/voice.py
--rw-rw-rw-   0        0        0     2045 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/webhook.py
--rw-rw-rw-   0        0        0     1500 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1948 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/types/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.140834 tonkord.py-1.0.0/tonkord/ui/
--rw-rw-rw-   0        0        0      326 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/__init__.py
--rw-rw-rw-   0        0        0    11085 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/button.py
--rw-rw-rw-   0        0        0     8386 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/dynamic.py
--rw-rw-rw-   0        0        0     5555 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/item.py
--rw-rw-rw-   0        0        0     7252 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/modal.py
--rw-rw-rw-   0        0        0    45302 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/select.py
--rw-rw-rw-   0        0        0     8583 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/text_input.py
--rw-rw-rw-   0        0        0    26827 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/ui/view.py
--rw-rw-rw-   0        0        0    18771 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/user.py
--rw-rw-rw-   0        0        0    43235 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/utils.py
--rw-rw-rw-   0        0        0    20211 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/voice_client.py
--rw-rw-rw-   0        0        0    28278 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/voice_state.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.141830 tonkord.py-1.0.0/tonkord/webhook/
--rw-rw-rw-   0        0        0      195 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/webhook/__init__.py
--rw-rw-rw-   0        0        0    72495 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/webhook/async_.py
--rw-rw-rw-   0        0        0    44265 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/webhook/sync.py
--rw-rw-rw-   0        0        0     7757 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/welcome_screen.py
--rw-rw-rw-   0        0        0    10751 2024-04-23 05:06:43.000000 tonkord.py-1.0.0/tonkord/widget.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:52:08.141830 tonkord.py-1.0.0/tonkord.py.egg-info/
--rw-rw-rw-   0        0        0     2575 2024-04-29 11:52:07.000000 tonkord.py-1.0.0/tonkord.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3427 2024-04-29 11:52:08.000000 tonkord.py-1.0.0/tonkord.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:52:07.000000 tonkord.py-1.0.0/tonkord.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      641 2024-04-29 11:52:07.000000 tonkord.py-1.0.0/tonkord.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 11:52:07.000000 tonkord.py-1.0.0/tonkord.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.159483 tonkord.py-2.0/
+-rw-rw-rw-   0        0        0     1102 2024-04-23 05:06:43.000000 tonkord.py-2.0/LICENSE
+-rw-rw-rw-   0        0        0      116 2024-04-23 05:06:43.000000 tonkord.py-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2573 2024-04-29 11:55:12.158487 tonkord.py-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-04-29 11:16:51.000000 tonkord.py-2.0/README.rst
+-rw-rw-rw-   0        0        0      919 2024-04-23 05:06:43.000000 tonkord.py-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       67 2024-04-23 05:06:43.000000 tonkord.py-2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:55:12.159483 tonkord.py-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3512 2024-04-29 11:48:28.000000 tonkord.py-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.090710 tonkord.py-2.0/tests/
+-rw-rw-rw-   0        0        0     2188 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_annotated_annotation.py
+-rw-rw-rw-   0        0        0     5361 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_autocomplete.py
+-rw-rw-rw-   0        0        0    10738 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_description.py
+-rw-rw-rw-   0        0        0    20190 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_group.py
+-rw-rw-rw-   0        0        0     6780 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_app_commands_invoke.py
+-rw-rw-rw-   0        0        0     2213 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_colour.py
+-rw-rw-rw-   0        0        0    16294 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_commands_cog.py
+-rw-rw-rw-   0        0        0     4894 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_commands_description.py
+-rw-rw-rw-   0        0        0     5332 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_ext_tasks.py
+-rw-rw-rw-   0        0        0     4153 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_files.py
+-rw-rw-rw-   0        0        0    10566 2024-04-23 05:06:43.000000 tonkord.py-2.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.117621 tonkord.py-2.0/tonkord/
+-rw-rw-rw-   0        0        0     1993 2024-04-29 11:55:07.000000 tonkord.py-2.0/tonkord/__init__.py
+-rw-rw-rw-   0        0        0    11394 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/__main__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/_types.py
+-rw-rw-rw-   0        0        0    68645 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/abc.py
+-rw-rw-rw-   0        0        0    28940 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/activity.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.134565 tonkord.py-2.0/tonkord/app_commands/
+-rw-rw-rw-   0        0        0      444 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18620 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    97078 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19748 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    39593 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13386 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    33225 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    11044 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    49299 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    19929 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/appinfo.py
+-rw-rw-rw-   0        0        0    16692 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/asset.py
+-rw-rw-rw-   0        0        0    39755 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/audit_logs.py
+-rw-rw-rw-   0        0        0    27638 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/automod.py
+-rw-rw-rw-   0        0        0     3859 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/backoff.py
+-rw-rw-rw-   0        0        0   121700 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/channel.py
+-rw-rw-rw-   0        0        0    98085 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/client.py
+-rw-rw-rw-   0        0        0    15014 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/colour.py
+-rw-rw-rw-   0        0        0    20993 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/components.py
+-rw-rw-rw-   0        0        0     3124 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/context_managers.py
+-rw-rw-rw-   0        0        0    23479 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/embeds.py
+-rw-rw-rw-   0        0        0     8831 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/emoji.py
+-rw-rw-rw-   0        0        0    25928 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/enums.py
+-rw-rw-rw-   0        0        0     9232 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.083732 tonkord.py-2.0/tonkord/ext/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.139549 tonkord.py-2.0/tonkord/ext/commands/
+-rw-rw-rw-   0        0        0      458 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2711 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    53628 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    32370 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    41097 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    47543 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    10006 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    92194 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36964 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    23572 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    59452 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    38076 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     9593 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6443 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.140545 tonkord.py-2.0/tonkord/ext/tasks/
+-rw-rw-rw-   0        0        0    30480 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5601 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/file.py
+-rw-rw-rw-   0        0        0    61982 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/flags.py
+-rw-rw-rw-   0        0        0    37212 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/gateway.py
+-rw-rw-rw-   0        0        0   160673 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/guild.py
+-rw-rw-rw-   0        0        0    97147 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/http.py
+-rw-rw-rw-   0        0        0    13751 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/integrations.py
+-rw-rw-rw-   0        0        0    48955 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/interactions.py
+-rw-rw-rw-   0        0        0    21211 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/invite.py
+-rw-rw-rw-   0        0        0    43155 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/member.py
+-rw-rw-rw-   0        0        0     5745 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/mentions.py
+-rw-rw-rw-   0        0        0    91350 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/message.py
+-rw-rw-rw-   0        0        0     1531 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/mixins.py
+-rw-rw-rw-   0        0        0     3837 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/object.py
+-rw-rw-rw-   0        0        0     3771 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/oggparse.py
+-rw-rw-rw-   0        0        0    16882 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/opus.py
+-rw-rw-rw-   0        0        0     8223 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/partial_emoji.py
+-rw-rw-rw-   0        0        0    32389 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/permissions.py
+-rw-rw-rw-   0        0        0    30450 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/player.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/py.typed
+-rw-rw-rw-   0        0        0    18600 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/raw_models.py
+-rw-rw-rw-   0        0        0     9430 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/reaction.py
+-rw-rw-rw-   0        0        0    18745 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/role.py
+-rw-rw-rw-   0        0        0    24311 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/scheduled_event.py
+-rw-rw-rw-   0        0        0    21301 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/shard.py
+-rw-rw-rw-   0        0        0     6871 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/sku.py
+-rw-rw-rw-   0        0        0     6690 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/stage_instance.py
+-rw-rw-rw-   0        0        0    77030 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/state.py
+-rw-rw-rw-   0        0        0    16713 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/sticker.py
+-rw-rw-rw-   0        0        0     5164 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/team.py
+-rw-rw-rw-   0        0        0     9736 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/template.py
+-rw-rw-rw-   0        0        0    33420 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/threads.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.150512 tonkord.py-2.0/tonkord/types/
+-rw-rw-rw-   0        0        0      159 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/__init__.py
+-rw-rw-rw-   0        0        0     2841 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/activity.py
+-rw-rw-rw-   0        0        0     2550 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8870 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4184 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/automod.py
+-rw-rw-rw-   0        0        0     5131 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/channel.py
+-rw-rw-rw-   0        0        0     6484 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/command.py
+-rw-rw-rw-   0        0        0     3606 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/components.py
+-rw-rw-rw-   0        0        0     2419 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/embed.py
+-rw-rw-rw-   0        0        0     1574 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/emoji.py
+-rw-rw-rw-   0        0        0     9128 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/gateway.py
+-rw-rw-rw-   0        0        0     5781 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/guild.py
+-rw-rw-rw-   0        0        0     2370 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/integration.py
+-rw-rw-rw-   0        0        0     7421 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/interactions.py
+-rw-rw-rw-   0        0        0     2797 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/invite.py
+-rw-rw-rw-   0        0        0     2155 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/member.py
+-rw-rw-rw-   0        0        0     4840 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/message.py
+-rw-rw-rw-   0        0        0     1815 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/role.py
+-rw-rw-rw-   0        0        0     3405 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1657 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/sku.py
+-rw-rw-rw-   0        0        0     1210 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2343 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/sticker.py
+-rw-rw-rw-   0        0        0     1607 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/team.py
+-rw-rw-rw-   0        0        0     1658 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/template.py
+-rw-rw-rw-   0        0        0     2534 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/threads.py
+-rw-rw-rw-   0        0        0     1813 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/user.py
+-rw-rw-rw-   0        0        0     2352 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/voice.py
+-rw-rw-rw-   0        0        0     2045 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/webhook.py
+-rw-rw-rw-   0        0        0     1500 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1948 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/types/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.154499 tonkord.py-2.0/tonkord/ui/
+-rw-rw-rw-   0        0        0      326 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/__init__.py
+-rw-rw-rw-   0        0        0    11085 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/button.py
+-rw-rw-rw-   0        0        0     8386 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/dynamic.py
+-rw-rw-rw-   0        0        0     5555 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/item.py
+-rw-rw-rw-   0        0        0     7252 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/modal.py
+-rw-rw-rw-   0        0        0    45302 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/select.py
+-rw-rw-rw-   0        0        0     8583 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/text_input.py
+-rw-rw-rw-   0        0        0    26827 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/ui/view.py
+-rw-rw-rw-   0        0        0    18771 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/user.py
+-rw-rw-rw-   0        0        0    43235 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/utils.py
+-rw-rw-rw-   0        0        0    20211 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/voice_client.py
+-rw-rw-rw-   0        0        0    28278 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/voice_state.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.156495 tonkord.py-2.0/tonkord/webhook/
+-rw-rw-rw-   0        0        0      195 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    72495 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/async_.py
+-rw-rw-rw-   0        0        0    44265 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7757 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10751 2024-04-23 05:06:43.000000 tonkord.py-2.0/tonkord/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:55:12.157490 tonkord.py-2.0/tonkord.py.egg-info/
+-rw-rw-rw-   0        0        0     2573 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3427 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      641 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 11:55:12.000000 tonkord.py-2.0/tonkord.py.egg-info/top_level.txt
```

### Comparing `tonkord.py-1.0.0/LICENSE` & `tonkord.py-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/PKG-INFO` & `tonkord.py-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkord.py
-Version: 1.0.0
+Version: 2.0
 Summary: A Python wrapper for the Discord API
 Home-page: https://9tonkla.cloud
 Author: tonkoranit
 License: MIT
 Project-URL: Documentation, https://9tonkla.cloud
 Project-URL: Issue tracker, https://9tonkla.cloud
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tonkord.py-1.0.0/pyproject.toml` & `tonkord.py-2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/setup.py` & `tonkord.py-2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_annotated_annotation.py` & `tonkord.py-2.0/tests/test_annotated_annotation.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_app_commands_autocomplete.py` & `tonkord.py-2.0/tests/test_app_commands_autocomplete.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_app_commands_description.py` & `tonkord.py-2.0/tests/test_app_commands_description.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_app_commands_group.py` & `tonkord.py-2.0/tests/test_app_commands_group.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_app_commands_invoke.py` & `tonkord.py-2.0/tests/test_app_commands_invoke.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_colour.py` & `tonkord.py-2.0/tests/test_colour.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_ext_commands_cog.py` & `tonkord.py-2.0/tests/test_ext_commands_cog.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_ext_commands_description.py` & `tonkord.py-2.0/tests/test_ext_commands_description.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_ext_tasks.py` & `tonkord.py-2.0/tests/test_ext_tasks.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_files.py` & `tonkord.py-2.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tests/test_utils.py` & `tonkord.py-2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/__init__.py` & `tonkord.py-2.0/tonkord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 """
 
 __title__ = 'tonkord'
 __author__ = 'tonkoranit'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2015-present Rapptz'
-__version__ = '1.0.0'
+__version__ = '2.0'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
```

### Comparing `tonkord.py-1.0.0/tonkord/__main__.py` & `tonkord.py-2.0/tonkord/__main__.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/_types.py` & `tonkord.py-2.0/tonkord/_types.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/abc.py` & `tonkord.py-2.0/tonkord/abc.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/activity.py` & `tonkord.py-2.0/tonkord/activity.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/checks.py` & `tonkord.py-2.0/tonkord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/commands.py` & `tonkord.py-2.0/tonkord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/errors.py` & `tonkord.py-2.0/tonkord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/models.py` & `tonkord.py-2.0/tonkord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/namespace.py` & `tonkord.py-2.0/tonkord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/transformers.py` & `tonkord.py-2.0/tonkord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/translator.py` & `tonkord.py-2.0/tonkord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/app_commands/tree.py` & `tonkord.py-2.0/tonkord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/appinfo.py` & `tonkord.py-2.0/tonkord/appinfo.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/asset.py` & `tonkord.py-2.0/tonkord/asset.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/audit_logs.py` & `tonkord.py-2.0/tonkord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/automod.py` & `tonkord.py-2.0/tonkord/automod.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/backoff.py` & `tonkord.py-2.0/tonkord/backoff.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/channel.py` & `tonkord.py-2.0/tonkord/channel.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/client.py` & `tonkord.py-2.0/tonkord/client.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/colour.py` & `tonkord.py-2.0/tonkord/colour.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/components.py` & `tonkord.py-2.0/tonkord/components.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/context_managers.py` & `tonkord.py-2.0/tonkord/context_managers.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/embeds.py` & `tonkord.py-2.0/tonkord/embeds.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/emoji.py` & `tonkord.py-2.0/tonkord/emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/enums.py` & `tonkord.py-2.0/tonkord/enums.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/errors.py` & `tonkord.py-2.0/tonkord/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/_types.py` & `tonkord.py-2.0/tonkord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/bot.py` & `tonkord.py-2.0/tonkord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/cog.py` & `tonkord.py-2.0/tonkord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/context.py` & `tonkord.py-2.0/tonkord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/converter.py` & `tonkord.py-2.0/tonkord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/cooldowns.py` & `tonkord.py-2.0/tonkord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/core.py` & `tonkord.py-2.0/tonkord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/errors.py` & `tonkord.py-2.0/tonkord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/flags.py` & `tonkord.py-2.0/tonkord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/help.py` & `tonkord.py-2.0/tonkord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/hybrid.py` & `tonkord.py-2.0/tonkord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/parameters.py` & `tonkord.py-2.0/tonkord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/commands/view.py` & `tonkord.py-2.0/tonkord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ext/tasks/__init__.py` & `tonkord.py-2.0/tonkord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/file.py` & `tonkord.py-2.0/tonkord/file.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/flags.py` & `tonkord.py-2.0/tonkord/flags.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/gateway.py` & `tonkord.py-2.0/tonkord/gateway.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/guild.py` & `tonkord.py-2.0/tonkord/guild.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/http.py` & `tonkord.py-2.0/tonkord/http.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/integrations.py` & `tonkord.py-2.0/tonkord/integrations.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/interactions.py` & `tonkord.py-2.0/tonkord/interactions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/invite.py` & `tonkord.py-2.0/tonkord/invite.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/member.py` & `tonkord.py-2.0/tonkord/member.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/mentions.py` & `tonkord.py-2.0/tonkord/mentions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/message.py` & `tonkord.py-2.0/tonkord/message.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/mixins.py` & `tonkord.py-2.0/tonkord/mixins.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/object.py` & `tonkord.py-2.0/tonkord/object.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/oggparse.py` & `tonkord.py-2.0/tonkord/oggparse.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/opus.py` & `tonkord.py-2.0/tonkord/opus.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/partial_emoji.py` & `tonkord.py-2.0/tonkord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/permissions.py` & `tonkord.py-2.0/tonkord/permissions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/player.py` & `tonkord.py-2.0/tonkord/player.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/raw_models.py` & `tonkord.py-2.0/tonkord/raw_models.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/reaction.py` & `tonkord.py-2.0/tonkord/reaction.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/role.py` & `tonkord.py-2.0/tonkord/role.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/scheduled_event.py` & `tonkord.py-2.0/tonkord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/shard.py` & `tonkord.py-2.0/tonkord/shard.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/sku.py` & `tonkord.py-2.0/tonkord/sku.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/stage_instance.py` & `tonkord.py-2.0/tonkord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/state.py` & `tonkord.py-2.0/tonkord/state.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/sticker.py` & `tonkord.py-2.0/tonkord/sticker.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/team.py` & `tonkord.py-2.0/tonkord/team.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/template.py` & `tonkord.py-2.0/tonkord/template.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/threads.py` & `tonkord.py-2.0/tonkord/threads.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/activity.py` & `tonkord.py-2.0/tonkord/types/activity.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/appinfo.py` & `tonkord.py-2.0/tonkord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/audit_log.py` & `tonkord.py-2.0/tonkord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/automod.py` & `tonkord.py-2.0/tonkord/types/automod.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/channel.py` & `tonkord.py-2.0/tonkord/types/channel.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/command.py` & `tonkord.py-2.0/tonkord/types/command.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/components.py` & `tonkord.py-2.0/tonkord/types/components.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/embed.py` & `tonkord.py-2.0/tonkord/types/embed.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/emoji.py` & `tonkord.py-2.0/tonkord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/gateway.py` & `tonkord.py-2.0/tonkord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/guild.py` & `tonkord.py-2.0/tonkord/types/guild.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/integration.py` & `tonkord.py-2.0/tonkord/types/integration.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/interactions.py` & `tonkord.py-2.0/tonkord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/invite.py` & `tonkord.py-2.0/tonkord/types/invite.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/member.py` & `tonkord.py-2.0/tonkord/types/member.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/message.py` & `tonkord.py-2.0/tonkord/types/message.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/role.py` & `tonkord.py-2.0/tonkord/types/role.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/scheduled_event.py` & `tonkord.py-2.0/tonkord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/sku.py` & `tonkord.py-2.0/tonkord/types/sku.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/snowflake.py` & `tonkord.py-2.0/tonkord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/sticker.py` & `tonkord.py-2.0/tonkord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/team.py` & `tonkord.py-2.0/tonkord/types/team.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/template.py` & `tonkord.py-2.0/tonkord/types/template.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/threads.py` & `tonkord.py-2.0/tonkord/types/threads.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/user.py` & `tonkord.py-2.0/tonkord/types/user.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/voice.py` & `tonkord.py-2.0/tonkord/types/voice.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/webhook.py` & `tonkord.py-2.0/tonkord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/welcome_screen.py` & `tonkord.py-2.0/tonkord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/types/widget.py` & `tonkord.py-2.0/tonkord/types/widget.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/button.py` & `tonkord.py-2.0/tonkord/ui/button.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/dynamic.py` & `tonkord.py-2.0/tonkord/ui/dynamic.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/item.py` & `tonkord.py-2.0/tonkord/ui/item.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/modal.py` & `tonkord.py-2.0/tonkord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/select.py` & `tonkord.py-2.0/tonkord/ui/select.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/text_input.py` & `tonkord.py-2.0/tonkord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/ui/view.py` & `tonkord.py-2.0/tonkord/ui/view.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/user.py` & `tonkord.py-2.0/tonkord/user.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/utils.py` & `tonkord.py-2.0/tonkord/utils.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/voice_client.py` & `tonkord.py-2.0/tonkord/voice_client.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/voice_state.py` & `tonkord.py-2.0/tonkord/voice_state.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/webhook/async_.py` & `tonkord.py-2.0/tonkord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/webhook/sync.py` & `tonkord.py-2.0/tonkord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/welcome_screen.py` & `tonkord.py-2.0/tonkord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord/widget.py` & `tonkord.py-2.0/tonkord/widget.py`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord.py.egg-info/PKG-INFO` & `tonkord.py-2.0/tonkord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkord.py
-Version: 1.0.0
+Version: 2.0
 Summary: A Python wrapper for the Discord API
 Home-page: https://9tonkla.cloud
 Author: tonkoranit
 License: MIT
 Project-URL: Documentation, https://9tonkla.cloud
 Project-URL: Issue tracker, https://9tonkla.cloud
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tonkord.py-1.0.0/tonkord.py.egg-info/SOURCES.txt` & `tonkord.py-2.0/tonkord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tonkord.py-1.0.0/tonkord.py.egg-info/requires.txt` & `tonkord.py-2.0/tonkord.py.egg-info/requires.txt`

 * *Files identical despite different names*

