# Comparing `tmp/cognitrix-0.2.1.tar.gz` & `tmp/cognitrix-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitrix-0.2.1.tar", max compression
+gzip compressed data, was "cognitrix-0.2.2.tar", max compression
```

## Comparing `cognitrix-0.2.1.tar` & `cognitrix-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0    11324 2024-03-13 15:27:01.846250 cognitrix-0.2.1/LICENSE
--rw-r--r--   0        0        0     2846 2024-03-13 15:27:01.846250 cognitrix-0.2.1/README.md
--rw-r--r--   0        0        0      134 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/__init__.py
--rw-r--r--   0        0        0       74 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/agents/__init__.py
--rw-r--r--   0        0        0      270 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/agents/assistant.py
--rw-r--r--   0        0        0    13719 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/agents/base.py
--rw-r--r--   0        0        0     2419 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/agents/core.py
--rw-r--r--   0        0        0    10417 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/agents/templates.py
--rw-r--r--   0        0        0      629 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/app.py
--rw-r--r--   0        0        0     6130 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/cli.py
--rw-r--r--   0        0        0      533 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/config.py
--rw-r--r--   0        0        0      357 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/__init__.py
--rw-r--r--   0        0        0     3875 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/anthropic_llm.py
--rw-r--r--   0        0        0     4846 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/base.py
--rw-r--r--   0        0        0     1610 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/clarifai_llm.py
--rw-r--r--   0        0        0     2434 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/cohere_llm.py
--rw-r--r--   0        0        0     3333 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/google_llm.py
--rw-r--r--   0        0        0     2116 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/groq_llm.py
--rw-r--r--   0        0        0     4010 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/openai_llm.py
--rw-r--r--   0        0        0     2969 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/llms/together_llm.py
--rw-r--r--   0        0        0       37 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/tasks/__init__.py
--rw-r--r--   0        0        0      922 2024-03-13 15:27:01.846250 cognitrix-0.2.1/cognitrix/tasks/base.py
--rw-r--r--   0        0        0      343 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/__init__.py
--rw-r--r--   0        0        0      587 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/base.py
--rw-r--r--   0        0        0    17366 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/misc.py
--rw-r--r--   0        0        0     2553 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/python.py
--rw-r--r--   0        0        0     5059 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/serpapi.py
--rw-r--r--   0        0        0      917 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/tools/tool.py
--rw-r--r--   0        0        0      337 2024-03-13 15:27:01.850250 cognitrix-0.2.1/cognitrix/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-03-13 15:27:01.850250 cognitrix-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4813 1970-01-01 00:00:00.000000 cognitrix-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 11:07:51.888374 cognitrix-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2847 2024-04-29 11:07:51.888374 cognitrix-0.2.2/README.md
+-rw-r--r--   0        0        0      134 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/agents/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/agents/assistant.py
+-rw-r--r--   0        0        0    17194 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/agents/base.py
+-rw-r--r--   0        0        0     2419 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/agents/core.py
+-rw-r--r--   0        0        0    17917 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/agents/templates.py
+-rw-r--r--   0        0        0      518 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/app.py
+-rw-r--r--   0        0        0     6906 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/cli.py
+-rw-r--r--   0        0        0      896 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/config.py
+-rw-r--r--   0        0        0      450 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/__init__.py
+-rw-r--r--   0        0        0     3895 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/anthropic_llm.py
+-rw-r--r--   0        0        0     2877 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/base.py
+-rw-r--r--   0        0        0     1610 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/clarifai_llm.py
+-rw-r--r--   0        0        0     2283 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/cohere_llm.py
+-rw-r--r--   0        0        0     3523 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/google_llm.py
+-rw-r--r--   0        0        0     2978 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/groq_llm.py
+-rw-r--r--   0        0        0     4002 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/local_llm.py
+-rw-r--r--   0        0        0     1233 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/mindsdb_llm.py
+-rw-r--r--   0        0        0     4266 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/openai_llm.py
+-rw-r--r--   0        0        0     2264 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/session.py
+-rw-r--r--   0        0        0     2499 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/llms/together_llm.py
+-rw-r--r--   0        0        0       37 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tasks/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tasks/base.py
+-rw-r--r--   0        0        0      392 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tools/__init__.py
+-rw-r--r--   0        0        0     2053 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tools/base.py
+-rw-r--r--   0        0        0    25001 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tools/misc.py
+-rw-r--r--   0        0        0     2561 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tools/python.py
+-rw-r--r--   0        0        0      925 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/tools/tool.py
+-rw-r--r--   0        0        0     2955 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/transcriber.py
+-rw-r--r--   0        0        0     5363 2024-04-29 11:07:51.888374 cognitrix-0.2.2/cognitrix/utils/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-29 11:07:51.892374 cognitrix-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5022 1970-01-01 00:00:00.000000 cognitrix-0.2.2/PKG-INFO
```

### Comparing `cognitrix-0.2.1/LICENSE` & `cognitrix-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitrix-0.2.1/README.md` & `cognitrix-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
 ### Usage
 Run with default settings
 ```bash
 cognitrix
 ```
 
-List supported platforms
+List supported providers
 ```bash
-cognitrix --platforms
+cognitrix --providers
 ```
 
-Run with specific platform
+Run with specific provider
 ```bash
-cognitrix --platform <platform_name>
+cognitrix --provider <provider_name>
 ```
 
 Create a new agent
 ```bash
 cognitrix agents --new
 ```
 
@@ -70,8 +70,8 @@
 ### Contributing
 Cognitrix is open source and contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
 
 ### License
 This project is licensed under the MIT license. See [LICENSE.md](LICENSE.md) for more details.
 
 ### Acknowledgments
-Cognitrix was created by [Amos Amissah](https://github.com/theonlyamos) and is heavily inspired by projects like AutoGPT and EngineerGPT. Special thanks to the open-source community for their contributions and the AI companies providing LLM APIs.
+Cognitrix was created by [Amos Amissah](https://github.com/theonlyamos) and is heavily inspired by projects like AutoGPT and GPT Engineer. Special thanks to the open-source community for their contributions and the AI companies providing LLM APIs.
```

### Comparing `cognitrix-0.2.1/cognitrix/agents/core.py` & `cognitrix-0.2.2/cognitrix/agents/core.py`

 * *Files identical despite different names*

### Comparing `cognitrix-0.2.1/cognitrix/app.py` & `cognitrix-0.2.2/cognitrix/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from llms import Together
 from llms import Cohere
 from agents import AIAssistant
 from tools import (
-    Calculator, YoutubePlayer,
-    WorldNews, PythonREPL,
-    FSBrowser, SearchTool,
-    InternetBrowser, tool
+    Calculator, YoutubePlayer,PythonREPL,
+    InternetBrowser, FSBrowser
 )
 
 if __name__ == "__main__":
     llm = Cohere()
     # llm = TogetherLLM()
     assistant = AIAssistant(llm=llm, name='Adam')
     assistant.add_tool(Calculator())
     assistant.add_tool(YoutubePlayer())
-    assistant.add_tool(WorldNews())
     assistant.add_tool(FSBrowser())
     assistant.add_tool(PythonREPL())
     assistant.add_tool(InternetBrowser())
-    assistant.add_tool(SearchTool())
     assistant.start()
```

### Comparing `cognitrix-0.2.1/cognitrix/cli.py` & `cognitrix-0.2.2/cognitrix/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,139 @@
 import os
 import sys
+import asyncio
 import logging
 import argparse
 from pathlib import Path
 from argparse import Namespace
 
 from cognitrix.llms import (
     Cohere, OpenAI,LLM
 )
 
-from .agents import AIAssistant, Agent
-from .tools import (
-    Calculator, YoutubePlayer,
-    WorldNews, PythonREPL,
-    FSBrowser, SearchTool,
-    InternetBrowser, take_screenshot,
-    text_input, key_press, mouse_click,
-    mouse_double_click, mouse_right_click
-)
+from cognitrix.agents import AIAssistant, Agent
+from cognitrix.llms.session import Session
+from cognitrix.tools import Tool
 
-from .config import VERSION
+from cognitrix.config import VERSION
 
 def add_agent():
-    new_agent = Agent.create_agent() # type: ignore
+    new_agent = asyncio.run(Agent.create_agent()) # type: ignore
     if new_agent:
-        print(f"\nAgent {new_agent.name} added successfully!")
+        description = input("\n[Enter agent system prompt]: ")
+        if description:
+            new_agent.prompt_template = description
+            asyncio.run(new_agent.save())
+        print(f"\nAgent **{new_agent.name}** added successfully!")
     else:
         print("\nError creating agent")
     sys.exit()
 
 def list_agents():
     agents_str = "\nAvailable Agents:"
-    for index, agent in enumerate(Agent.list_agents()):
+    for index, agent in enumerate(asyncio.run(Agent.list_agents())):
         agents_str += (f"\n[{index}] {agent.name}")                 #type: ignore
     print(agents_str)
     
-def list_platforms():
-    print("\nAvailable Platforms:")
+def list_providers():
+    print("\nAvailable providers:")
     for index, l in enumerate(LLM.list_llms()):
         print(f"[{index}] {l}")
+        
+def list_tools():
+    print("\nAvailable Tools:")
+    for index, l in enumerate(Tool.list_all_tools()):
+        print(f"[{index}] {l.name}")
+        
+def list_sessions():
+    print("\nSaved Sessions:")
+    sessions = Session.list_sessions()
+    for index, s in enumerate(sessions):
+        print(f"[{index}] [{s.datetime}] {s.id}")
 
 def manage_agents(args: Namespace):
     try:
         if args.new:
             add_agent()
         elif args.list:
             list_agents()
     except KeyboardInterrupt:
         print()
         sys.exit()
     except Exception as e:
-        logging.warning(str(e))
+        logging.exception(e)
         sys.exit(1)
 
 def str_or_file(string):
     if len(string) > 100:
         return string
     if Path(string).is_file() or Path(os.curdir, string).is_file():
         with open(Path(string), 'rt') as file:
             return file.read()
     return string
 
 def start(args: Namespace):
     try:
-        if args.platforms:
-            list_platforms()
+        if args.providers:
+            list_providers()
             sys.exit()
         elif args.agents:
             list_agents()              #type: ignore
             sys.exit()
-        platform = None
-        if args.platform:
-            platform = LLM.load_llm(model_name=args.platform)
-        platform = platform() if platform else Cohere()
+        elif args.tools:
+            list_tools()
+            sys.exit()
+        elif args.sessions:
+            list_sessions()
+            sys.exit()
+        
+        provider = None
+        if args.provider:
+            provider = LLM.load_llm(model_name=args.provider)
+        provider = provider() if provider else Cohere()
+        
         
         if args.api_key:
-            platform.api_key = args.api_key
+            provider.api_key = args.api_key
         if args.model:
-            platform.model = args.model
+            provider.model = args.model
         
-        platform.temperature = args.temperature
+        provider.temperature = args.temperature
         if args.system_prompt:
-            platform.system_prompt = args.system_prompt
+            provider.system_prompt = args.system_prompt
         # llm = TogetherLLM()
         loaded_agent = None
         if args.agent:
             loaded_agent = Agent.load_agent(args.agent)
             
             if loaded_agent:
                 assistant = loaded_agent
             else:
-                assistant_description = "You are an ai assistant. Your main goal is to help the user complete tasks"
-                assistant = AIAssistant.create_agent(name=args.agent, task_description=assistant_description, llm=platform) #type: ignore
+                # assistant_description = "You are an ai assistant. Your main goal is to help the user complete tasks"
+                assistant = asyncio.run(AIAssistant.create_agent(name=args.agent, llm=provider)) #type: ignore
 
         else:
-            assistant = AIAssistant(llm=platform, name=args.name, verbose=args.verbose)
+            assistant = AIAssistant(llm=provider, name=args.name, verbose=args.verbose)
         
         if assistant:
-            assistant.llm = platform
+            if args.provider:
+                assistant.llm = provider
             assistant.name = args.name
-            assistant.add_tool(take_screenshot)
-            assistant.add_tool(text_input)
-            assistant.add_tool(key_press)
-            assistant.add_tool(mouse_click)
-            assistant.add_tool(mouse_double_click)
-            assistant.add_tool(mouse_right_click)
-            # assistant.add_tool(Calculator())
-            # assistant.add_tool(YoutubePlayer())
-            # assistant.add_tool(WorldNews())
-            # assistant.add_tool(FSBrowser())
-            # assistant.add_tool(PythonREPL())
-            # assistant.add_tool(InternetBrowser())
-            # assistant.add_tool(SearchTool())
-            assistant.start()
+            if args.load_all_tools:
+                assistant.tools = Tool.list_all_tools()
+            
+            assistant.format_system_prompt()
+            asyncio.run(assistant.save())
+            
+            if args.audio:
+                assistant.start_audio()
+            else:
+                assistant.start(args.session)
     except Exception as e:
-        logging.error(str(e))
+        logging.exception(e)
         parser.print_help()
         sys.exit(1)
 
 def get_arguments():
     global parser
     
     subparsers = parser.add_subparsers()
@@ -127,37 +142,42 @@
     agents_parser.add_argument('--new', action='store_true', help='Create a new agent')
     agents_parser.add_argument('--list', action='store_false', help='List all saved agents')
     agents_parser.add_argument('--update', action='store_true', help='Update an agent')
     agents_parser.add_argument('--remove', action='store_true', help='Delete an agent')
     
     agents_parser.set_defaults(func=manage_agents)
 
-    parser.add_argument('--name', type=str, default='Adam', help='Set name of agent')
-    parser.add_argument('--platform', default='', help='Set llm platform to use')
-    parser.add_argument('--platforms', action='store_true', help='Get a list of all supported platforms')
+    parser.add_argument('--name', type=str, default='Assistant', help='Set name of agent')
+    parser.add_argument('--provider', default='', help='Set llm provider to use')
+    parser.add_argument('--providers', action='store_true', help='Get a list of all supported providers')
     parser.add_argument('--agents', action='store_true', help='List all saved agents')
     parser.add_argument('--agent', type=str, default='Assistant', help='Set which saved agent to use')
+    parser.add_argument('--tools', action='store_true', help='List all available tools')
+    parser.add_argument('--load-all-tools', action='store_true', help='Add all available tools to agent')
     parser.add_argument('--model', type=str, default='', help='Specify model or model_url to use')
     parser.add_argument('--api-key', type=str, default='', help='Set api key of selected llm')
     parser.add_argument('--api-base', type=str, default='', help='Set api base of selected llm. Set if using local llm.')
     parser.add_argument('--temperature', type=float, default=0.1, help='Set temperature of model')
     parser.add_argument('--system-prompt', type=str_or_file, default='', help='Set system prompt of model. Can be a string or a text file path')
     parser.add_argument('--prompt-template', type=str_or_file, default='', help='Set prompt template of model. Can be a string or a text file path')
+    parser.add_argument('--audio', action='store_true', help='Get input from microphone')
+    parser.add_argument('--session', type=str, default="", help='Load saved session')
+    parser.add_argument('--sessions', action='store_true', help='Get a list of all saved sessions')
     parser.add_argument('--verbose', action='store_true', help='Set verbose mode')
     parser.add_argument('-v','--version', action='version', version=f'%(prog)s {VERSION}')
     parser.set_defaults(func=start)
     return parser.parse_args()
 
 def main():
     global parser
     try:
         parser = argparse.ArgumentParser(description="Build and run AI agents on your computer")
         args = get_arguments()
         args.func(args)
 
     except Exception as e:
-        logging.error(str(e))
+        logging.exception(e)
         parser.print_help()
         sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cognitrix-0.2.1/cognitrix/llms/anthropic_llm.py` & `cognitrix-0.2.2/cognitrix/llms/anthropic_llm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from cognitrix.llms.base import LLM
 from cognitrix.utils import image_to_base64
 from typing import Any
 from dotenv import load_dotenv
-from anthropic import Anthropic
+from anthropic import Anthropic as AnthropicLLM
 import logging
 import sys
 import os
 
 logging.basicConfig(
     format='%(asctime)s - %(levelname)s - [%(filename)s:%(lineno)d] - %(message)s',
     datefmt='%d-%b-%y %H:%M:%S',
     level=logging.WARNING
 )
 logger = logging.getLogger('cognitrix.log')
 load_dotenv()
 
 
-class Claude(LLM):
+class Anthropic(LLM):
     """A class for interacting with the Claude API.
 
     Args:
         model (str): The name of the OpenAI model to use
         temperature (float): The temperature to use when generating text
         api_key (str): Your OpenAI API key
         chat_history (list): Chat history
         max_tokens (int): The maximum number of tokens to generate in the completion
         supports_system_prompt (bool): Flag to indicate if system prompt should be supported
         system_prompt (str): System prompt to prepend to queries
     """
-    model: str = 'claude-3-sonnet-20240229'
+    model: str = 'claude-3-opus-20240229'
     """model endpoint to use""" 
     
     temperature: float = 0.1
     """What sampling temperature to use.""" 
     
     chat_history: list[str] = []
     """Chat history"""
@@ -103,15 +103,15 @@
             query (dict): The query to generate a response to.
             kwds (dict): Additional keyword arguments to pass to the Claude API.
 
         Returns:
             str|None: A string containing the generated response.
         """
 
-        client = Anthropic(api_key=self.api_key)
+        client = AnthropicLLM(api_key=self.api_key)
         result = client.messages.create(
             model=self.model,
             max_tokens=self.max_tokens,
             temperature=self.temperature,
             system=self.system_prompt,
             messages=self.format_query(query)
         )
```

### Comparing `cognitrix-0.2.1/cognitrix/llms/clarifai_llm.py` & `cognitrix-0.2.2/cognitrix/llms/clarifai_llm.py`

 * *Files identical despite different names*

### Comparing `cognitrix-0.2.1/cognitrix/llms/cohere_llm.py` & `cognitrix-0.2.2/cognitrix/llms/cohere_llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,38 +31,33 @@
     """model endpoint to use""" 
     
     temperature: float = 0.1
     """What sampling temperature to use.""" 
     
     api_key: str = os.getenv('CO_API_KEY', '')
     """Cohere API key""" 
-    
-    def format_query(self, message: str) -> str:
-        """Formats a message for the Cohere API"""
-
-        formatted_message = self.system_prompt + '\nUser: ' + message
-
-        return formatted_message
 
     def __call__(self, query, **kwds: Any)->str:
         """Generates a response to a query using the Cohere API.
 
         Args:
         query: The query to generate a response to.
         kwds: Additional keyword arguments to pass to the Cohere API.
 
         Returns:
         A string containing the generated response.
         """
+        
         client = cohere.Client(api_key=self.api_key)
         response = client.chat( 
             model=self.model,
             message=query['message'],
             temperature=self.temperature,
             chat_history=self.chat_history,
+            preamble_override=self.system_prompt,
             prompt_truncation='auto',
             stream=False,
             citation_quality='accurate',
             connectors=[{"id": "web-search"}]
         )
         
         return response.text
```

### Comparing `cognitrix-0.2.1/cognitrix/llms/google_llm.py` & `cognitrix-0.2.2/cognitrix/llms/google_llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 from cognitrix.llms.base import LLM
 from typing import Any
 import google.generativeai as genai
 from dotenv import load_dotenv
+from PIL import Image
 import logging
 import sys
 import os
+import io
+
+from cognitrix.utils import image_to_base64
 
 logging.basicConfig(
     format='%(asctime)s - %(levelname)s - [%(filename)s:%(lineno)d] - %(message)s',
     datefmt='%d-%b-%y %H:%M:%S',
     level=logging.WARNING
 )
 logger = logging.getLogger('cognitrix.log')
 load_dotenv()
 
 
-class Gemini(LLM):
+class Google(LLM):
     """A class for interacting with the Gemini API.
 
     Args:
         model (str): The name of the OpenAI model to use
         temperature (float): The temperature to use when generating text
         api_key (str): Your OpenAI API key
         chat_history (list): Chat history
         max_tokens (int): The maximum number of tokens to generate in the completion
         supports_system_prompt (bool): Flag to indicate if system prompt should be supported
         system_prompt (str): System prompt to prepend to queries
     """
-    model: str = 'gemini-pro'
+    model: str = 'gemini-1.5-pro-latest'
     """model endpoint to use""" 
     
-    vision_model: str = 'gemini-pro-vision'
-    """vision model endpoint to use""" 
-    
     temperature: float = 0.0
     """What sampling temperature to use.""" 
     
     chat_history: list[str] = []
     """Chat history"""
     
     api_key: str = os.getenv('GOOGLE_API_KEY', '')
     """GOOGLE API key""" 
     
+    max_tokens: int = 2048
+    """Maximum output tokens"""
+    
     supports_system_prompt: bool = False
     """Flag to indicate if system prompt should be supported"""
     
     is_multimodal: bool = True
     """Whether the model is multimodal."""
     
     def format_query(self, message: dict[str, str]) -> list:
-        """Formats a message for the Gemini API"""
+        """Formats messages for the Gemini API"""
         formatted_message = [*self.chat_history, message]
         
         messages = []
         if self.system_prompt:
             messages.append(self.system_prompt)
         
         for fm in formatted_message:
             if fm['type'] == 'text': 
                 messages.append(fm['message'])
             elif fm['type'] == 'image':
-                self.model = self.vision_model
-                messages.append(fm['image'])
+                screenshot_bytes = io.BytesIO()
+                fm['image'].save(screenshot_bytes, format='JPEG')
+                upload_image = Image.open(screenshot_bytes)
+                messages.append(upload_image)
                 messages.append('Above is the screenshot')
 
         return messages
 
     def __call__(self, query, **kwds: Any)->str|None:
         """Generates a response to a query using the Gemini API.
 
@@ -97,15 +103,15 @@
 
         response.resolve()
         
         return response.text
     
 if __name__ == "__main__":
     try:
-        assistant = Gemini()
+        assistant = Google()
         # assistant.add_tool(calculator)
         while True:
             message = input("\nEnter Query$ ")
             result = assistant(message)
             print(result)
     except KeyboardInterrupt:
         sys.exit(1)
```

### Comparing `cognitrix-0.2.1/cognitrix/llms/groq_llm.py` & `cognitrix-0.2.2/cognitrix/llms/mindsdb_llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,40 @@
-from groq import Groq as GroqLLM
-from cognitrix.llms.base import LLM
-from typing import Any, Optional
-from dotenv import load_dotenv
-import logging
-import sys
+from cognitrix.llms import OpenAI
+from openai import OpenAI as OpenAILLM
+from typing import Optional
 import os
 
-logging.basicConfig(
-    format='%(asctime)s - %(levelname)s - [%(filename)s:%(lineno)d] - %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-    level=logging.WARNING
-)
-logger = logging.getLogger('cognitrix.log')
-load_dotenv()
-
-
-class Groq(LLM):
-    """A class for interacting with the Groq API.
-
-    Args:
-        model: The name of the Groq model to use.
-        temperature: The temperature to use when generating text.
-        api_key: Your Groq API key.
-    """
-    model: str = 'mixtral-8x7b-32768'
-    """model endpoint to use""" 
-    
-    temperature: float = 0.1
-    """What sampling temperature to use.""" 
+class MindsDB(OpenAI):
+    """A class for interacting with the MindsDB API."""
     
-    chat_history: list[str] = []
-    """Chat history"""
+    model: str ='gemini-1.5-pro'
     
-    api_key: str = os.getenv('GROQ_API_KEY', '')
-    """Groq API key""" 
+    api_key: str = os.getenv('MINDSDB_API_KEY', '')
     
-    supports_system_prompt: bool = True
-    """Flag to indicate if system prompt should be supported"""
+    base_url: str = 'https://llm.mdb.ai'
     
-    system_prompt: str = ""
-    """System prompt to prepend to queries"""
-
-    def __call__(self, query, **kwds: Any)->str|None:
-        """Generates a response to a query using the Groq API.
+    def __call__(self, query: dict, **kwds: dict)->Optional[str]:
+        """Generates a response to a query using the OpenAI API.
 
         Args:
-        query: The query to generate a response to.
-        kwds: Additional keyword arguments to pass to the Groq API.
+            query (dict): The query to generate a response to.
+            kwds (dict): Additional keyword arguments to pass to the OpenAI API.
 
         Returns:
-        A string containing the generated response.
+            A string containing the generated response.
         """
 
-        client = GroqLLM(api_key=self.api_key)
+        client = OpenAILLM(api_key=self.api_key, base_url=self.base_url)
+            
+        formatted_messages = self.format_query(query)
+        
         response = client.chat.completions.create(
             model=self.model,
             messages=[
-                {"role": "user", "content": query}
+                {"role": "user", "content": self.system_prompt},
+                *formatted_messages
             ],
             temperature=self.temperature,
-            top_p=1,
-            stop=None,
+            max_tokens=self.max_tokens
         )
-            
-        return response.choices[0].message.content
-    
-if __name__ == "__main__":
-    try:
-        assistant = Groq()
-        # assistant.add_tool(calculator)
-        while True:
-            message = input("\nEnter Query$ ")
-            result = assistant(message)
-            print(result)
-    except KeyboardInterrupt:
-        sys.exit(1)
+        
+        return response.choices[0].message.content
```

### Comparing `cognitrix-0.2.1/cognitrix/llms/openai_llm.py` & `cognitrix-0.2.2/cognitrix/llms/openai_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from openai import OpenAI as OpenAILLM
 from cognitrix.llms.base import LLM
+from cognitrix.tools.base import Tool
 from cognitrix.utils import image_to_base64
-from typing import Any, Optional
+from typing import Any, List, Optional
 from dotenv import load_dotenv
 import logging
 import sys
 import os
 
 logging.basicConfig(
     format='%(asctime)s - %(levelname)s - [%(filename)s:%(lineno)d] - %(message)s',
@@ -37,26 +38,29 @@
     
     temperature: float = 0.1
     """What sampling temperature to use.""" 
     
     api_key: str = os.getenv('OPENAI_API_KEY', '')
     """OpenAI API key""" 
     
-    max_tokens: int = 4000
+    max_tokens: int = 4096
     """The maximum number of tokens to generate in the completion.""" 
     
     chat_history: list[str] = []
     """Chat history"""
     
     supports_system_prompt: bool = True
     """Flag to indicate if system prompt should be supported"""
     
     system_prompt: str = ""
     """System prompt to prepend to queries"""
     
+    tools: List[Tool] = []
+    """Functions to call"""
+    
     def format_query(self, message: dict[str, str]) -> list:
         """Formats a message for the Claude API.
 
         Args:
             message (dict[str, str]): The message to be formatted for the Claude API.
 
         Returns:
@@ -74,50 +78,56 @@
                     "content": [
                         {
                             "type": "text",
                             "text": fm['message']
                         }
                     ]
                 })
-            else:
+            elif fm['type'] == 'image':
                 base64_image = image_to_base64(fm['image'])
-                self.model = self.vision_model
+                # self.model = self.vision_model
                 messages.append({
                     "role": fm['role'].lower(),
                     "content": [
                         {
                             "type": "text",
                             "text": "This is the result of the latest screenshot"
                         },
                         {
                             "type": "image_url",
                             "image_url": f"data:image/jpeg;base64,{base64_image}"
                         }
                     ]
                 })
-            
+            else:
+                print(fm)
+        
         return messages
 
     def __call__(self, query: dict, **kwds: dict)->Optional[str]:
         """Generates a response to a query using the OpenAI API.
 
         Args:
             query (dict): The query to generate a response to.
             kwds (dict): Additional keyword arguments to pass to the OpenAI API.
 
         Returns:
             A string containing the generated response.
         """
 
         client = OpenAILLM(api_key=self.api_key)
+        if self.base_url:
+            client.base_url = self.base_url
+            
         formatted_messages = self.format_query(query)
+        
         response = client.chat.completions.create(
             model=self.model,
             messages=[
                 {"role": "system", "content": self.system_prompt},
                 *formatted_messages
             ],
             temperature=self.temperature,
             max_tokens=self.max_tokens
         )
-            
+        
         return response.choices[0].message.content
```

### Comparing `cognitrix-0.2.1/cognitrix/tasks/base.py` & `cognitrix-0.2.2/cognitrix/tasks/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 import asyncio
 
 class Task(BaseModel):
     """
     Initializes the Task object by assigning values to its attributes.
 
     Args:
-        func (function): The function to be executed by the task.
+        description (str): The task to perform or query to answer.
         args (tuple): The positional arguments to be passed to the function.
         kwargs (dict): The keyword arguments to be passed to the function.
 
     Returns:
         None
     """
     
     description: str
+    """The task|query to perform|answer"""
+    
     func: Optional[Callable] = None
+    """Assigned tool to complete the task"""
+    
     done: bool = False
+    """Checks/Sets whether the task has been completed"""
     
     async def start(self):
         if self.func:
             self.task = asyncio.create_task(self.func())
 
     async def join(self):
         if self.task:
```

### Comparing `cognitrix-0.2.1/cognitrix/tools/python.py` & `cognitrix-0.2.2/cognitrix/tools/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import Field
 from typing import Dict, Optional
-from ..tools.base import Tool
+from cognitrix.tools.base import Tool
 from io import StringIO
 import multiprocessing
 import functools
 import logging
 import sys
 
 NotImplementedErrorMessage = 'this tool does not suport async'
```

### Comparing `cognitrix-0.2.1/cognitrix/tools/tool.py` & `cognitrix-0.2.2/cognitrix/tools/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
 from typing import Callable
-from ..tools import Tool
+from cognitrix.tools import Tool
 import inspect
 
 def tool(func: Callable, *args, **kwargs):
     @wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
```

### Comparing `cognitrix-0.2.1/pyproject.toml` & `cognitrix-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognitrix"
-version = "0.2.1"
+version = "0.2.2"
 description = "Package for creating AI Agents using llms"
 authors = ["theonlyamos <theonlyamos@gmail.com>"]
 license = "Apache2"
 readme = "README.md"
 homepage = "https://github.com/theonlyamos/cognitrix"
 repository = "https://github.com/theonlyamos/cognitrix"
 keywords = ["cognitrix", "ai", "agents", "ai agents", "ai-agents", "llms", "autonomous agents"]
@@ -42,14 +42,19 @@
 openai = "^1.12.0"
 groq = "^0.4.1"
 google-generativeai = "^0.4.0"
 uuid = "^1.30"
 pillow = "^10.2.0"
 pyautogui = "^0.9.54"
 anthropic = "^0.17.0"
+aiofiles = "^23.2.1"
+xmltodict = "^0.13.0"
+deepgram-sdk = "==3.*"
+beautifulsoup4 = "^4.12.3"
+pyttsx3 = "^2.90"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `cognitrix-0.2.1/PKG-INFO` & `cognitrix-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitrix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package for creating AI Agents using llms
 Home-page: https://github.com/theonlyamos/cognitrix
 License: Apache2
 Keywords: cognitrix,ai,agents,ai agents,ai-agents,llms,autonomous agents
 Author: theonlyamos
 Author-email: theonlyamos@gmail.com
 Requires-Python: >=3.12,<4.0
@@ -19,30 +19,35 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: anthropic (>=0.17.0,<0.18.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: clarifai (>=10.1.0,<11.0.0)
 Requires-Dist: cohere (>=4.50,<5.0)
+Requires-Dist: deepgram-sdk (==3.*)
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0)
 Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
 Requires-Dist: groq (>=0.4.1,<0.5.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pyautogui (>=0.9.54,<0.10.0)
 Requires-Dist: pydantic (>=2.6.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: pyttsx3 (>=2.90,<3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: serpapi (>=0.1.5,<0.2.0)
 Requires-Dist: together (>=0.2.11,<0.3.0)
 Requires-Dist: uuid (>=1.30,<2.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/theonlyamos/cognitrix/issues
 Project-URL: Repository, https://github.com/theonlyamos/cognitrix
 Description-Content-Type: text/markdown
 
 ### Cognitrix
 Cognitrix is an open-source autonous AI agents orchestrator built in Python. It allows you to create and manage AI agents easily.
 
@@ -78,22 +83,22 @@
 
 ### Usage
 Run with default settings
 ```bash
 cognitrix
 ```
 
-List supported platforms
+List supported providers
 ```bash
-cognitrix --platforms
+cognitrix --providers
 ```
 
-Run with specific platform
+Run with specific provider
 ```bash
-cognitrix --platform <platform_name>
+cognitrix --provider <provider_name>
 ```
 
 Create a new agent
 ```bash
 cognitrix agents --new
 ```
 
@@ -115,8 +120,8 @@
 ### Contributing
 Cognitrix is open source and contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
 
 ### License
 This project is licensed under the MIT license. See [LICENSE.md](LICENSE.md) for more details.
 
 ### Acknowledgments
-Cognitrix was created by [Amos Amissah](https://github.com/theonlyamos) and is heavily inspired by projects like AutoGPT and EngineerGPT. Special thanks to the open-source community for their contributions and the AI companies providing LLM APIs.
+Cognitrix was created by [Amos Amissah](https://github.com/theonlyamos) and is heavily inspired by projects like AutoGPT and GPT Engineer. Special thanks to the open-source community for their contributions and the AI companies providing LLM APIs.
```

