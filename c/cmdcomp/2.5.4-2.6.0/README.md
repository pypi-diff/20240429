# Comparing `tmp/cmdcomp-2.5.4.tar.gz` & `tmp/cmdcomp-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.5.4.tar", max compression
+gzip compressed data, was "cmdcomp-2.6.0.tar", max compression
```

## Comparing `cmdcomp-2.5.4.tar` & `cmdcomp-2.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1784 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/README.md
--rw-r--r--   0        0        0       79 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/__init__.py
--rw-r--r--   0        0        0      155 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/__main__.py
--rw-r--r--   0        0        0     3114 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/app.py
--rw-r--r--   0        0        0      561 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/completion.py
--rw-r--r--   0        0        0      331 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/config.py
--rw-r--r--   0        0        0      323 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/exception.py
--rw-r--r--   0        0        0     1138 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      406 2023-11-25 09:12:44.021663 cmdcomp-2.5.4/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     2902 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2164 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1888 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1469 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      406 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0      258 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      701 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      665 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      599 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1322 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/argument/select_argument.py
--rw-r--r--   0        0        0     2901 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/base_command.py
--rw-r--r--   0        0        0      980 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/delegate_command.py
--rw-r--r--   0        0        0     1169 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/empty_command.py
--rw-r--r--   0        0        0     2331 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/positional_arguments_command.py
--rw-r--r--   0        0        0     2271 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/command/subcommands_command.py
--rw-r--r--   0        0        0      952 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/config.py
--rw-r--r--   0        0        0      452 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/mixin/has_alias.py
--rw-r--r--   0        0        0     5432 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     3238 2023-11-25 09:12:44.025663 cmdcomp-2.5.4/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1925 2023-11-25 09:12:44.033663 cmdcomp-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 cmdcomp-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1791 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/README.md
+-rw-r--r--   0        0        0       79 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/__main__.py
+-rw-r--r--   0        0        0     3114 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/app.py
+-rw-r--r--   0        0        0      561 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/completion.py
+-rw-r--r--   0        0        0      331 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/config.py
+-rw-r--r--   0        0        0      323 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/exception.py
+-rw-r--r--   0        0        0     1138 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     2902 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2164 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1896 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1469 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0      258 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      701 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      665 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      599 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1322 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/argument/select_argument.py
+-rw-r--r--   0        0        0     2901 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/base_command.py
+-rw-r--r--   0        0        0     1864 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/delegate_command.py
+-rw-r--r--   0        0        0     1169 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/empty_command.py
+-rw-r--r--   0        0        0     2331 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/positional_arguments_command.py
+-rw-r--r--   0        0        0     2271 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/command/subcommands_command.py
+-rw-r--r--   0        0        0     1008 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0      452 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/mixin/has_alias.py
+-rw-r--r--   0        0        0     6319 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     3238 2024-04-29 05:56:01.448176 cmdcomp-2.6.0/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1930 2024-04-29 05:56:01.456176 cmdcomp-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 cmdcomp-2.6.0/PKG-INFO
```

### Comparing `cmdcomp-2.5.4/README.md` & `cmdcomp-2.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,28 +12,26 @@
 `cmdcomp` generate command shell completion file (`bash` or `zsh`) from config
 `JSON`/`YAML`/`TOML` file.
 
 ![image](./docs/images/image.png)
 
 ## Why was `cmdcomp` created?
 
-The completion files for many cli tools (`aws`, `gcloud`, etc.) are provided by
-the tools themselves. However, if one wants to use these cli tools with multiple
-products and multiple environments (prd, dev, etc.), it would be useful to be
-able to switch contexts easily. In this situation, I have a simple shell script
-wrapper that easily switches between settings for each environment. (like
-`mycli prd aws s3 ...`).
+The completion files for many cli tools (`aws`, `gcloud`, etc.) are provided by the tools themselves.
+If you want to use these cli tools in multiple products or multiple environments (prd, dev, etc.),
+it is useful to be able to switch contexts easily (e.g. `mycli prd aws s3 ...`).
+`cmdcomp` provides a completion file for such a simple shell script wrapper.
+You can easily switch between settings for each environment.
+
+This tool can generate shell script completion files with config described in `YAML`, `TOML` or `JSON`.
+
+Today, more and more cli tools are being used in development,
+and if you want to generate a completion file for a simple wrapper script,
+`cmdcomp` will be of great help.
 
-`cmdcomp` can generate shell script completion files with config described in
-`YAML`, `TOML` or `JSON`.
-
-In today's development, more and more cli tools are being used.
-
-If you want to generate completion files for simple wrapper scripts, `cmdcomp`
-can be of great help.
 
 ## Install
 
 ```shell
 pip install cmdcomp
 ```
```

### Comparing `cmdcomp-2.5.4/cmdcomp/app.py` & `cmdcomp-2.6.0/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/completion.py` & `cmdcomp-2.6.0/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/model.py` & `cmdcomp-2.6.0/cmdcomp/model.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.6.0/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v1/completion.py` & `cmdcomp-2.6.0/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.6.0/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 {%- endfor %}
     esac
 }
 
 file_completion() {
     local cur prev cword opts
     _get_comp_words_by_ref -n : cur prev cword
-    dir="$(echo ${cur} | grep -o ".*/")"
+    dir="$(echo ${cur} | grep -o ".*/" || true)"
     if test "${dir}" ;then
         COMPREPLY=( $(compgen -W "$(ls -F $1/${dir} | sed -E "s@(.*)@${dir}\1@g")" -- "${cur}") )
     else
         COMPREPLY=( $(compgen -W "$(ls -F $1/)" -- "${cur}") )
     fi
 }
```

### Comparing `cmdcomp-2.5.4/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.6.0/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/argument/select_argument.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/argument/select_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/base_command.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/base_command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/delegate_command.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/delegate_command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from typing import Annotated, Literal
+from functools import cached_property
+from typing import Annotated, Literal, OrderedDict
 
 from pydantic import Field
+from typing_extensions import override
+
+from cmdcomp.v2.command.argument import V2Argument
+from cmdcomp.v2.command.base_command import InputArgument, Keyword, convert_argument
 
 from .empty_command import V2EmptyCommand
 
 
 class V2DelegateCommand(V2EmptyCommand):
     """delegate completion of other command."""
 
@@ -31,13 +36,35 @@
                 "aws",
                 ["aws", "s3"],
                 ["aws", "s3", "ls"],
             ],
         ),
     ]
 
+    arguments: OrderedDict[Keyword, InputArgument | None] = Field(
+        title="arguments of the command.",
+        description='argment key allow keyword string (like "--f", "-f") only.',
+        default_factory=OrderedDict,
+    )
+
     @property
     def targets(self) -> list[str]:
         if isinstance(self.target, str):
             return [self.target]
         else:
             return self.target
+
+    @cached_property
+    @override
+    def keyword_arguments(self) -> OrderedDict[Keyword, V2Argument]:
+        return OrderedDict(
+            [
+                (k, convert_argument(v))
+                for k, v in self.arguments.items()
+                if isinstance(k, str)
+            ]
+        )
+
+    @property
+    @override
+    def has_keyword_arguments(self) -> bool:
+        return len(self.keyword_arguments) > 0
```

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/empty_command.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/empty_command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/positional_arguments_command.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/positional_arguments_command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/command/subcommands_command.py` & `cmdcomp-2.6.0/cmdcomp/v2/command/subcommands_command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/completion.py` & `cmdcomp-2.6.0/cmdcomp/v2/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 from pathlib import Path
 from typing import Any
 
 from cmdcomp import __version__
 from cmdcomp.shell import ShellType
 from cmdcomp.v2.config import V2Config
@@ -18,13 +19,14 @@
     template = env.get_template(f"{shell.value}.sh.jinja")
 
     return template.render(
         app_name=config.app.name,
         app_aliases=config.app.aliases + config.root.aliases,
         commands={config.app.name: config.root},
         append_key_tag=_append_key_tag,
+        logfile=os.getenv("CMDCOMP_LOGFILE"),
         version=__version__,
     )
 
 
 def _append_key_tag(d: dict[str, Any], tag: str) -> dict[tuple[str, str], Any]:
     return {(tag, k): v for k, v in d.items()}
```

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.6.0/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,59 @@
 {%- set func_name = "_" + app_name|ident -%}
 {%- set scope = "" -%}
 
 {#- macro def -#}
+{%- macro output_log(logfile) -%}
+{%- if logfile is not none %}
+  echo "COMP_LINE: $COMP_LINE" >> {{ logfile }}
+  echo "COMP_POINT: $COMP_POINT" >> {{ logfile }}
+  echo "COMP_CWORD: $COMP_CWORD" >> {{ logfile }}
+  echo "COMP_WORDS: ${COMP_WORDS[@]}" >> {{ logfile }}
+  echo "COMPREPLY: ${COMPREPLY[@]}" >> {{ logfile }}
+  echo >> {{ logfile }}
+{%- endif %}
+{%- endmacro -%}
 {%- macro argument_completion(argument) -%}
 {% if argument.type == "select" -%}
 if [ $cword -eq $COMP_CWORD ] ; then
   COMPREPLY=( $(compgen -W "{{ argument.options|join(" ") }}" -- "${COMP_WORDS[COMP_CWORD]}") )
-
+  {{- output_log(logfile) }}
   return 0
 else
-  cmd_cword=$(( cmd_cword + 1 ))
+  cmd_cword=$(( cmd_cword + 2 ))
 fi
 {%- elif argument.type == "file" -%}
 if [ $cword -eq $COMP_CWORD ] ; then
-  {{ file_completion(argument.base_path or ".")|indent(2) }}
+{%- if argument.base_path is none %}
+  word="${COMP_WORDS[COMP_CWORD]}"
+{%- else %}
+  word="{{ argument.base_path }}/${COMP_WORDS[COMP_CWORD]}"
+{%- endif %}
+  COMPREPLY=()
+  for dir in $(compgen -d -S / -- "$word"); do
+    COMPREPLY+=("$dir")
+  done
+  for file in $(compgen -f -- "$word"); do
+    [ ! -d $file ] && COMPREPLY+=("$file")
+  done
 
+{%- if argument.base_path is none %}
+  IFS=$'\n' COMPREPLY=($(sort <<<"${COMPREPLY[*]}"))
+{%- else %}
+  IFS=$'\n' COMPREPLY=($(sort <<<"${COMPREPLY[*]#{{ argument.base_path }}/}"))
+{%- endif %}
+  {{- output_log(logfile) }}
   return 0
 else
   cmd_cword=$(( cmd_cword + 2 ))
 fi
 {%- elif argument.type == "command" -%}
 if [ $cword -eq $COMP_CWORD ] ; then
   COMPREPLY=( $(compgen -W "$({{ argument.execute }})" -- "${COMP_WORDS[COMP_CWORD]}") )
-
+  {{- output_log(logfile) }}
   return 0
 else
   cmd_cword=$(( cmd_cword + 2 ))
 fi
 {%- elif argument.type == "flag" -%}
 cmd_cword=$(( cmd_cword + 1 ))
 {%- endif -%}
@@ -61,65 +88,64 @@
       ;;
   {% endfor -%}
   esac
 fi
 {%- endif %}
 
 {% if command.type == "delegate" -%}
-for ((i = 0; i < {{ depth }}; i++)); do
-  for ((j = 0; j <= {{ "${#COMP_LINE}" }}; j++)); do
-    [[ $COMP_LINE == "${COMP_WORDS[i]}"* ]] && break
-    COMP_LINE=${COMP_LINE:1}
-    ((COMP_POINT--))
-  done
-  COMP_LINE={{ '${COMP_LINE#"${COMP_WORDS[i]}"}' }}
-  ((COMP_POINT -= {{ '${#COMP_WORDS[i]}' }}))
+{%- if command.has_keyword_arguments -%}
+local has_keyword_splitter=false
+for word in ${COMP_WORDS[@]::$COMP_CWORD}; do
+  [ "$word" == "--" ] && has_keyword_splitter=true && break
 done
-COMP_LINE="{{ command.targets | join(' ') }} $COMP_LINE"
-COMP_POINT=$((COMP_POINT + {{ command.targets | join(" ") | length + 1 }}))
-COMP_WORDS=({{ command.targets | join(" ") }} "${COMP_WORDS[{{ depth + 1 }}, -1]}")
-COMP_CWORD={{ "${#COMP_WORDS[@]}" }}
+if [[ $has_keyword_splitter = false && ${COMP_WORDS[COMP_CWORD]} == -* ]] ; then
+  opts="{{ command.keyword_names_with_alias|join(' ') }}"
+  COMPREPLY=( $(compgen -W "${opts}" -- "${COMP_WORDS[COMP_CWORD]}") )
+  {{- output_log(logfile) }}
+  return 0
+fi
+{% endif -%}
+local word=${COMP_WORDS[@]::$cmd_cword}
+COMP_POINT=$((COMP_POINT + {{ command.targets | join(" ") | length }} - {{ "${#word}" }} ))
+COMP_LINE="{{ command.targets | join(' ') }} ${COMP_WORDS[@]:$cmd_cword}"
+COMP_WORDS=($COMP_LINE)
+COMP_CWORD=$(( {{ "${#COMP_WORDS[@]}" }} - 1 ))
+(( COMP_CWORD < 1 )) && COMP_CWORD=1
 
-[ -x "$(command -v _command_offset)" ] && _command_offset 0
+type "_command_offset" > /dev/null 2>&1 && _command_offset 0
 {%- elif command.has_subcommands -%}
 if [[ ${COMP_WORDS[COMP_CWORD]} == -* ]] ; then
   opts="{{ command.keyword_names_with_alias|join(' ') }}"
   COMPREPLY=( $(compgen -W "${opts}" -- "${COMP_WORDS[COMP_CWORD]}") )
+  {{- output_log(logfile) }}
   return 0
 elif [ $cword -eq $COMP_CWORD ] ; then
   opts="{{ command.subcommand_names_with_alias|join(' ') }}"
   COMPREPLY=( $(compgen -W "${opts}" -- "${COMP_WORDS[COMP_CWORD]}") )
+  {{- output_log(logfile) }}
   return 0
 fi
 {%- elif command.has_positional_arguments or command.has_positional_wildcard_argument -%}
 if [[ ${COMP_WORDS[COMP_CWORD]} == -* ]] ; then
   opts="{{ command.keyword_names_with_alias|join(' ') }}"
   COMPREPLY=( $(compgen -W "${opts}" -- "${COMP_WORDS[COMP_CWORD]}") )
+  {{- output_log(logfile) }}
   return 0
 fi
 {%- else -%}
 opts="{{ command.keyword_names_with_alias|join(' ') }}"
 COMPREPLY=( $(compgen -W "${opts}" -- "${COMP_WORDS[COMP_CWORD]}") )
 {%- endif %}
 
 {%- if command.has_positional_wildcard_argument %}
 cword=$COMP_CWORD
 {{ argument_completion(command.positional_wildcard_argument) }}
 {%- endif %}
 {%- endmacro -%}
 
-{#- macro def -#}
-{%- macro file_completion(base_path) -%}
-dir="$(echo ${COMP_WORDS[COMP_CWORD]} | grep -o ".*/")"
-if test "${dir}" ;then
-    COMPREPLY=( $(compgen -W "$(ls -F "{{ base_path }}/${dir}" | sed -E "s@(.*)@${dir}\1@g")" -- "${COMP_WORDS[COMP_CWORD]}") )
-else
-    COMPREPLY=( $(compgen -W "$(ls -F "{{ base_path }}/")" -- "${COMP_WORDS[COMP_CWORD]}") )
-fi
-{%- endmacro -%}
 
 #!/bin/bash
 #
 # Code generated by cmdcomp "{{ version }}". DO NOT EDIT.
 # For more information about cmdcomp, please refer to https://github.com/yassun7010/cmdcomp .
 #
 
@@ -154,26 +180,26 @@
         ;;
     esac
   done
 
   case "${cmd}" in
     {{ func_name }})
       {{ command_completion(commands[app_name], 1)|indent(6) }}
-
+      {{- output_log(logfile) }}
       return 0
       ;;
 {% for (tag, command_name), subcommand in append_key_tag(commands[app_name].subcommands, func_name).items() recursive %}
 {%- set new_tag = tag + "_" + command_name|ident %}
     {{ new_tag }})
       {{ command_completion(subcommand, loop.depth + 1)|indent(6) }}
-
+      {{- output_log(logfile) }}
       return 0
       ;;
 {{ loop(append_key_tag(subcommand.subcommands, new_tag).items()) -}}
 {% endfor %}
   esac
 }
 
-complete -F {{ func_name }} -o bashdefault -o default {{ app_name }}
+complete -F {{ func_name }} -o bashdefault {{ app_name }}
 {%- for alias in app_aliases %}
-complete -F {{ func_name }} -o bashdefault -o default {{ alias }}
+complete -F {{ func_name }} -o bashdefault {{ alias }}
 {%- endfor -%}
```

### Comparing `cmdcomp-2.5.4/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.6.0/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.5.4/pyproject.toml` & `cmdcomp-2.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.5.4"
+version = "2.6.0"
 description = "command shell completion file generator."
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 homepage = "https://yassun7010.github.io/cmdcomp/"
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun7010/cmdcomp"
 classifiers = [
@@ -41,15 +41,15 @@
 typing-extensions = "^4.7.1"
 rich-argparse = "^1.3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pyright = "^1.1.325"
 taskipy = "^1.10.4"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = ">=0.21,<0.24"
 ipython = "^8.15.0"
 mkdocs-material = "^9.1.21"
 ruff = "^0.1.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cmdcomp-2.5.4/PKG-INFO` & `cmdcomp-2.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.5.4
+Version: 2.6.0
 Summary: command shell completion file generator.
 Home-page: https://yassun7010.github.io/cmdcomp/
 License: BSD-3-Clause
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,28 +40,26 @@
 `cmdcomp` generate command shell completion file (`bash` or `zsh`) from config
 `JSON`/`YAML`/`TOML` file.
 
 ![image](./docs/images/image.png)
 
 ## Why was `cmdcomp` created?
 
-The completion files for many cli tools (`aws`, `gcloud`, etc.) are provided by
-the tools themselves. However, if one wants to use these cli tools with multiple
-products and multiple environments (prd, dev, etc.), it would be useful to be
-able to switch contexts easily. In this situation, I have a simple shell script
-wrapper that easily switches between settings for each environment. (like
-`mycli prd aws s3 ...`).
+The completion files for many cli tools (`aws`, `gcloud`, etc.) are provided by the tools themselves.
+If you want to use these cli tools in multiple products or multiple environments (prd, dev, etc.),
+it is useful to be able to switch contexts easily (e.g. `mycli prd aws s3 ...`).
+`cmdcomp` provides a completion file for such a simple shell script wrapper.
+You can easily switch between settings for each environment.
+
+This tool can generate shell script completion files with config described in `YAML`, `TOML` or `JSON`.
+
+Today, more and more cli tools are being used in development,
+and if you want to generate a completion file for a simple wrapper script,
+`cmdcomp` will be of great help.
 
-`cmdcomp` can generate shell script completion files with config described in
-`YAML`, `TOML` or `JSON`.
-
-In today's development, more and more cli tools are being used.
-
-If you want to generate completion files for simple wrapper scripts, `cmdcomp`
-can be of great help.
 
 ## Install
 
 ```shell
 pip install cmdcomp
 ```
```

