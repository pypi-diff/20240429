# Comparing `tmp/aitelegrambot-0.5.2.tar.gz` & `tmp/aitelegrambot-0.6.0.tar.gz`

## Comparing `aitelegrambot-0.5.2.tar` & `aitelegrambot-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,17 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/.env.example
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/Makefile.venv
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/.env.example
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/.gitignore
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/CHANGELOG.md
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/LICENSE.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/Makefile.venv
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/pyproject.toml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/docs/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/docs/commands.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/docs/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/docs/commands.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/LICENSE.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/.env.example
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/Makefile.venv
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/README.md
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/commands.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.6.0/PKG-INFO
```

### Comparing `aitelegrambot-0.5.2/CHANGELOG.md` & `aitelegrambot-0.6.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -63,7 +63,13 @@
 ## 0.5.1
 
 - Fix bug
 
 ## 0.5.2
 
 - Fix bug
+
+## 0.6.0
+
+- add help command.
+- Reply to the user even when streaming messages is disabled.
+- Fix bugs with pull and delete commands.
```

### Comparing `aitelegrambot-0.5.2/Makefile.venv` & `aitelegrambot-0.6.0/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.2/aitelegrambot/LICENSE.md` & `aitelegrambot-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.2/aitelegrambot/pyproject.toml` & `aitelegrambot-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/aitelegrambot"]
 [project]
 name = "aitelegrambot"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
   "ollama",
   "python-telegram-bot",
   "python-dotenv",
 ]
 authors = [
   {name = "tusharhero", email = "tusharhero@sdf.org"},
```

### Comparing `aitelegrambot-0.5.2/aitelegrambot/docs/commands.md` & `aitelegrambot-0.6.0/docs/commands.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 # Commands
 Commands refer to the commands users can run in the telegram bot.
 ## Normal Commands
 Commands only available for normal users.
 ### Start command
 #### invocation
 ```
-\start
+/start
 ```
 #### description
 
 It is the welcome message command, it just gives information the
 version of aitelegram being used.
 
 ### Inference command
 #### invocation
 ```
-\infer <query>
+/infer <query>
 ```
 #### description
 
 It is used to run an inference on the LLM, it can act in two ways
 according to the `ENABLE_STREAMING_RESPONSE` option, if it is disabled
 (default), the bot will send at the entire response at once, when the
 inference is done. If the option is enabled, the bot will stream the
 tokens into the response as it is being generated.
 
+### Help command
+#### invocation
+```
+/help
+```
+#### description
+
+Returns a list of all the commands.
+
 ## Administration Commands
 Commands only available for the administrator.
 ### List model command
 #### invocation
 ```
-\list_models
+/list_models
 ```
 #### description
 
 It lists each available model along with the command to switch to it.
 
 ### Change model command
 #### invocation
 ```
-\change_model <model_name>
+/change_model <model_name>
 ```
 #### description
 
 Changes the model to <model_name>.
 
 ### Pull model
 #### invocation
 ```
-\pull_model <model_name>
+/pull_model <model_name>
 ```
 #### description
 
 Pull <model_name> from Ollama's servers.
 
 ### Remove model
 #### invocation
 ```
-\delete_model <model_name>
+/delete_model <model_name>
 ```
 #### description
 
 Delete <model_name>.
```

### Comparing `aitelegrambot-0.5.2/aitelegrambot/docs/setup.md` & `aitelegrambot-0.6.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/__main__.py` & `aitelegrambot-0.6.0/src/aitelegrambot/__main__.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/bot.py` & `aitelegrambot-0.6.0/src/aitelegrambot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         ollama_state: OllamaState = OllamaState(
             Client(host=ollama_host), default_model, message_chunk_size
         )
         self.normal_command_handlers: CommandHandlers = NormalCommandHandlers(
             ollama_state
         )
         self.normal_command_handlers.inference = (
-            self.normal_command_handlers.steaming_inference
+            self.normal_command_handlers.stream_inference
             if enable_streaming_response
             else self.normal_command_handlers.basic_inference
         )
 
         self.administrative_command_handlers: CommandHandlers = (
             AdministrationCommandHandlers(ollama_state, administrator_user_id)
         )
@@ -82,14 +82,17 @@
         """
         Run the bot.
         """
         self.application.add_handler(
             CommandHandler("start", self.normal_command_handlers.start),
         )
         self.application.add_handler(
+            CommandHandler("help", self.normal_command_handlers.help),
+        )
+        self.application.add_handler(
             CommandHandler("infer", self.normal_command_handlers.inference),
         )
         self.application.add_handler(
             CommandHandler(
                 "list_models", self.administrative_command_handlers.list_models
             )
         )
```

### Comparing `aitelegrambot-0.5.2/aitelegrambot/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.6.0/src/aitelegrambot/commandhandlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,36 @@
 
         Arguments:
         ==========
         update: The update to be processed.
         context: The context for the message.
         """
         await context.bot.send_message(
-            chat_id=update.effective_chat.id, text=constants.WELCOME_MESSAGE
+            chat_id=update.effective_chat.id,
+            text=constants.WELCOME_MESSAGE,
+            parse_mode="Markdown",
+        )
+
+    async def help(
+        self,
+        update: Update,
+        context: ContextTypes.DEFAULT_TYPE,
+    ):
+        """
+        Informs the user about its commands.
+
+        Arguments:
+        ==========
+        update: The update to be processed.
+        context: The context for the message.
+        """
+        await context.bot.send_message(
+            chat_id=update.effective_chat.id,
+            text=constants.HELP_MESSAGE,
+            parse_mode="Markdown",
         )
 
     async def basic_inference(
         self,
         update: Update,
         context: ContextTypes.DEFAULT_TYPE,
     ):
@@ -99,15 +120,18 @@
         Arguments:
         ==========
         update: The update to be processed.
         context: The context for the inference.
         """
         query: str = self.get_content(update.message.text)
 
-        await update.message.reply_text(
+        message: Message = await update.message.reply_text(
+            text="wait...", parse_mode="Markdown"
+        )
+        await message.edit_text(
             text=self.ollama_state.client.chat(
                 model=self.ollama_state.model,
                 messages=[
                     {
                         "role": "user",
                         "content": query,
                     },
@@ -252,15 +276,15 @@
         model: str = self.get_content(update.message.text)
         if len(model) == 0:
             await update.message.reply_text(
                 "We don't have any models!\nTry pulling them."
             )
             return None
         await update.message.reply_text(f"Pulling {model}!")
-        self.ollama_state.pull(model)
+        self.ollama_state.client.pull(model)
         await update.message.reply_text(f"Done pulling {model}!")
 
     async def remove_model(
         self,
         update: Update,
         context: ContextTypes.DEFAULT_TYPE,
     ):
@@ -273,9 +297,9 @@
         context: The context for the inference.
         """
         if not self.is_admin(update):
             await update.message.reply_text("You are not an Admin!")
             return None
         model: str = self.get_content(update.message.text)
         await update.message.reply_text(f"Deleting {model}!")
-        self.ollama_state.delete(model)
+        self.ollama_state.client.delete(model)
         await update.message.reply_text(f"Done deleting {model}!")
```

### Comparing `aitelegrambot-0.5.2/PKG-INFO` & `aitelegrambot-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.5.2
+Version: 0.6.0
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
```

