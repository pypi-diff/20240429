# Comparing `tmp/nagatoai_core-0.1.0.tar.gz` & `tmp/nagatoai_core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagatoai_core-0.1.0.tar", max compression
+gzip compressed data, was "nagatoai_core-0.7.0.tar", max compression
```

## Comparing `nagatoai_core-0.1.0.tar` & `nagatoai_core-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,25 @@
--rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.1.0/LICENSE
--rw-r--r--   0        0        0     5831 2024-04-04 04:33:06.328422 nagatoai_core-0.1.0/README.md
--rw-r--r--   0        0        0     2307 2024-04-04 04:33:06.531442 nagatoai_core-0.1.0/nagatoai_core/agent/agent.py
--rw-r--r--   0        0        0     3362 2024-04-04 04:33:06.485160 nagatoai_core-0.1.0/nagatoai_core/agent/anthropic.py
--rw-r--r--   0        0        0      480 2024-03-31 11:58:16.105932 nagatoai_core-0.1.0/nagatoai_core/agent/message.py
--rw-r--r--   0        0        0     3783 2024-04-04 04:33:06.536748 nagatoai_core-0.1.0/nagatoai_core/agent/openai.py
--rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.1.0/nagatoai_core/mission/mission.py
--rw-r--r--   0        0        0     2158 2024-03-31 11:58:27.969342 nagatoai_core-0.1.0/nagatoai_core/mission/task.py
--rw-r--r--   0        0        0    24740 2024-03-31 11:58:36.424922 nagatoai_core-0.1.0/nagatoai_core/prompt/templates.py
--rw-r--r--   0        0        0      550 2024-04-04 04:33:06.327853 nagatoai_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 nagatoai_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8094 2024-04-29 06:24:03.515213 nagatoai_core-0.7.0/README.md
+-rw-r--r--   0        0        0     3007 2024-04-11 04:55:58.042433 nagatoai_core-0.7.0/nagatoai_core/agent/agent.py
+-rw-r--r--   0        0        0    10086 2024-04-16 03:58:07.727447 nagatoai_core-0.7.0/nagatoai_core/agent/anthropic.py
+-rw-r--r--   0        0        0     8372 2024-04-29 06:24:03.515970 nagatoai_core-0.7.0/nagatoai_core/agent/groq.py
+-rw-r--r--   0        0        0     1128 2024-04-11 04:55:58.043642 nagatoai_core-0.7.0/nagatoai_core/agent/message.py
+-rw-r--r--   0        0        0     8515 2024-04-18 05:28:06.141468 nagatoai_core-0.7.0/nagatoai_core/agent/openai.py
+-rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.7.0/nagatoai_core/mission/mission.py
+-rw-r--r--   0        0        0     2280 2024-04-11 04:55:58.044144 nagatoai_core-0.7.0/nagatoai_core/mission/task.py
+-rw-r--r--   0        0        0    29235 2024-04-16 03:58:07.728448 nagatoai_core-0.7.0/nagatoai_core/prompt/templates.py
+-rw-r--r--   0        0        0     1007 2024-04-11 04:55:58.044929 nagatoai_core-0.7.0/nagatoai_core/tool/abstract_tool.py
+-rw-r--r--   0        0        0     1330 2024-04-18 05:28:06.141811 nagatoai_core-0.7.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py
+-rw-r--r--   0        0        0     1280 2024-04-16 03:58:07.728840 nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/confirm.py
+-rw-r--r--   0        0        0     1138 2024-04-16 03:58:07.729054 nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/input.py
+-rw-r--r--   0        0        0      443 2024-04-16 03:58:07.729329 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/base_config.py
+-rw-r--r--   0        0        0     3264 2024-04-16 03:58:07.729584 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_finder.py
+-rw-r--r--   0        0        0     2550 2024-04-16 03:58:07.729869 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py
+-rw-r--r--   0        0        0     2150 2024-04-18 05:28:06.142322 nagatoai_core-0.7.0/nagatoai_core/tool/lib/web/page_scraper.py
+-rw-r--r--   0        0        0     1441 2024-04-11 04:55:58.046686 nagatoai_core-0.7.0/nagatoai_core/tool/provider/abstract_tool_provider.py
+-rw-r--r--   0        0        0     1755 2024-04-11 04:55:58.046901 nagatoai_core-0.7.0/nagatoai_core/tool/provider/anthropic.py
+-rw-r--r--   0        0        0     1869 2024-04-16 03:58:07.730257 nagatoai_core-0.7.0/nagatoai_core/tool/provider/openai.py
+-rw-r--r--   0        0        0     1247 2024-04-11 04:55:58.047121 nagatoai_core-0.7.0/nagatoai_core/tool/registry.py
+-rw-r--r--   0        0        0     2574 2024-04-11 04:55:58.047983 nagatoai_core-0.7.0/nagatoai_core/tool/schema.py
+-rw-r--r--   0        0        0      663 2024-04-29 06:24:03.516380 nagatoai_core-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8921 1970-01-01 00:00:00.000000 nagatoai_core-0.7.0/PKG-INFO
```

### Comparing `nagatoai_core-0.1.0/LICENSE` & `nagatoai_core-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.1.0/README.md` & `nagatoai_core-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![X (formerly Twitter)](https://img.shields.io/twitter/follow/Ed_Forson?style=social)](https://twitter.com/Ed_Forson)
 [![GitHub](https://img.shields.io/github/followers/kenshiro-o?label=Follow&style=social)](https://github.com/kenshiro-o)
 
 # Nagato-AI
 
-![Official Nagato AI Poster](docs/assets/Official_nagatoai_core_Poster.webp)
+![Official Nagato AI Poster](docs/assets/Official_Nagato_AI_Poster.webp)
 
 
 Nagato-AI is an intuitive AI Agent library that works across multiple LLMs.
 
 Currently it supports OpenAI's GPT and Anthpropic's Claude LLMs. You can create agents from any of the aforementioned family of models and combine them together to build the most effective AI Agent system you desire.
 
 The name _Nagato_ is inspired from the popular anime Naruto. In Naruto, Nagato is a very powerful ninja who possesses special eyes (Rinnegan) that gives him immense powers.
@@ -32,14 +32,22 @@
 
 Assuming your program's entrypoint is defined in a file called `main.py`, you can run it by typing the following command:
 
 ```
 poetry run python main.py
 ```
 
+
+## LLMs supported
+
+Nagato currently supports the following LLMs
+* Claude 3 (Anthropic)
+* GPT-3 to GPT-4 (OpenAI)
+* Groq (which gives you access to Llama 3) 🔥
+
 ## Examples of AI Agent configuration
 
 Nagato is built with flexibility at its core, so you could program it using your paradigm of choice. However these are some of the ways I've seen people use Nagato so far.
 
 ### Coordinator, worker, and critic agents
 
 In this configuration we have the following:
@@ -55,38 +63,39 @@
     organization="<org-id>",
     api_key="<api-key>",
 )
 
 anthropic_api_key = "<api-key>"
 anthropic_client = Anthropic(api_key=anthropic_api_key)
 
+groq_client = Groq(api_key="<api-key>")
+
 coordinator_agent: Agent = AnthropicAgent(
     anthropic_client,
     "claude-3-opus-20240229",
     "Coordinator",
     COORDINATOR_SYSTEM_PROMPT,
     "Coordinator Agent",
 )
 
-researcher_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-sonnet-20240229",
+researcher_agent: Agent = OpenAIAgent(
+    openai_client,
+    "gpt-4-turbo-2024-04-09",
     "Researcher",
     RESEARCHER_SYSTEM_PROMPT,
     "Researcher Agent",
 )
 
-critic_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-opus-20240229",
+critic_agent: Agent = GroqAgent(
+    groq_client,
+    "llama3-70b-8192",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
-
 ...
 ```
 
 The full blow example is available [here](docs/examples/coordinator_researcher_critic.py)
 
 ### Worker and critic agents
 
@@ -100,19 +109,14 @@
         goal="Fetch last 100 user tweets",
         description="Fetch the tweets from the user using the Twitter API. Limit the number of tweets fetched to 100 only."),
     Task(
         goal="Perform sentiment analysis on the tweets",
         description="Feed the tweets to the AI Agent to analyze sentiment per overall sentiment acoss tweets. Range of values for sentiment can be: Positive, Negative, or Neutral"
     )]
 
-openai_client = OpenAI(
-    organization="<org-id>",
-    api_key="<api-key>",
-)
-
 anthropic_api_key = "<api-key>"
 anthropic_client = Anthropic(api_key=anthropic_api_key)
 
 researcher_agent: Agent = AnthropicAgent(
     anthropic_client,
     "claude-3-sonnet-20240229",
     "Researcher",
@@ -139,25 +143,88 @@
 
     critic_exchange = critic_agent(critic_prompt, task, 0.7, 2000)
 
     # Evaluate whether the task was completed based on the answer from the critic agent
     ...
 ```
 
+## Tool calling
+
+Check the full example [here](docs/examples/coordinator_researcher_critic.py) to see how tool calling works.
+We now support tool calling for  GPT, Claude 3, and Llama 3 (via Groq) models.
+
+
+### Tool creation
+
+Creating a tool is straightforward. You must create have these two elements in place for a tool to be usable:
+
+1. A config class that contains the parameters that your tool will be called with
+2. A tool class that inherits from `AbstractTool`, and contains the main logic for your tool.
+
+For instance the below shows how we've created a tool to get the user to confirm yes/no in the terminal
+
+```python
+from typing import Any, Type
+
+from pydantic import BaseModel, Field
+from rich.prompt import Confirm
+
+from nagatoai_core.tool.abstract_tool import AbstractTool
+
+
+class HumanConfirmInputConfig(BaseModel):
+    """
+    HumanConfirmInputConfig represents the configuration for the HumanConfirmInputTool.
+    """
+
+    message: str = Field(
+        ...,
+        description="The message to display to the user to confirm whether to proceed or not",
+    )
+
+
+class HumanConfirmInputTool(AbstractTool):
+    """
+    HumanConfirmInputTool represents a tool that prompts the user to confirm whether to proceed or not.
+    """
+
+    name: str = "human_confirm_input"
+    description: str = (
+        """Prompts the user to confirm whether to proceed or not. Returns a boolean value indicating the user's choice."""
+    )
+    args_schema: Type[BaseModel] = HumanConfirmInputConfig
+
+    def _run(self, config: HumanConfirmInputConfig) -> Any:
+        """
+        Prompts the user to confirm whether to proceed or not.
+        :param message: The message to display to the user to confirm whether to proceed or not.
+        :return: A boolean value indicating the user's choice.
+        """
+        confirm = Confirm.ask("[bold yellow]" + config.message + "[/bold yellow]")
+
+        return confirm
+```
+
+
+
 # What's next
 
 Nagato is still in its very early development phase. This means that I am likely to introduce breaking changes over the next iterations of the library.
 
 Moreover, there is a lot of functionality currently missing from Nagato. I will remedy this over time. There is no official roadmap per se but I plan to add the following capabilities to Nagato:
 
-* introduction of tools (e.g. surfing the web)
-* support for function calling (complement to adding tools)
-* support for other LLMs beyond OpenAI's and Anthropic's
-* short/long-term memory for agents
-* LLMOps instrumentation
+* ✅ implement function calling (complement to adding tools)
+* ✅ introduce basic tools (e.g. surfing the web)
+* ✅ Support for Llama 3 (via Groq)
+* 🎯 cache results from function calling
+* 🎯 implement short/long-term memory for agents (with RAG and memory synthesis)
+* 🎯 implement self-reflection and re-planning for agents
+* 🎯 implement additional modalities (e.g. image, sound, etc.)
+* 🎯 Support for local LLMs (e.g. via Ollama)
+* 🎯 LLMOps instrumentation
 
 # How can you support
 
 I'd be grateful if you could do some of the following to support this project:
 
 * star this repository on Github
 * follow me on [X/Twitter](https://twitter.com/Ed_Forson)
```

### Comparing `nagatoai_core-0.1.0/nagatoai_core/agent/agent.py` & `nagatoai_core-0.7.0/nagatoai_core/agent/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import List, Union
 import uuid
 
-from .message import Exchange
+from .message import Exchange, ToolResult
 from nagatoai_core.mission.task import Task
+from nagatoai_core.tool.provider.abstract_tool_provider import AbstractToolProvider
 
 
 class Agent(ABC):
     """
     Agent represents the base class for all AI Agents.
     Any concrete AI Agent must inherit from this class and implement the generate_response method.
     """
@@ -37,20 +38,37 @@
         """
         Returns the agent's id as a string.
         """
         return str(self.agent_id)
 
     @abstractmethod
     def chat(
-        self, prompt: str, task: Union[Task, None], temperature: float, max_tokens: int
+        self,
+        prompt: str,
+        tools: List[AbstractToolProvider],
+        temperature: float,
+        max_tokens: int,
     ) -> Exchange:
         """
         Generates a response for the current prompt and prompt history.
         :param prompt: The current prompt.
-        :param task: the task to reason about
+        :param tools: the tools available to the agent.
+        :param temperature: The temperature of the agent.
+        :param max_tokens: The maximum number of tokens to generate.
+        :return: Exchange object containing the user message and the agent response.
+        """
+        pass
+
+    @abstractmethod
+    def send_tool_run_results(
+        self, tool_results: List[ToolResult], temperature: float, max_tokens: int
+    ) -> Exchange:
+        """
+        Returns the results of the running of one or multiple tools
+        :param tool_results: The results of the running of one or multiple tools
         :param temperature: The temperature of the agent.
         :param max_tokens: The maximum number of tokens to generate.
         :return: Exchange object containing the user message and the agent response.
         """
         pass
 
     @property
```

### Comparing `nagatoai_core-0.1.0/nagatoai_core/mission/mission.py` & `nagatoai_core-0.7.0/nagatoai_core/mission/mission.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.1.0/nagatoai_core/mission/task.py` & `nagatoai_core-0.7.0/nagatoai_core/mission/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
-from typing import Union
+from typing import Union, Optional
+from datetime import datetime
 
 from pydantic import BaseModel
 
 
 # Create a status enum with values PENDING, IN_PROGRESS, COMPLETED, and FAILED
 class TaskStatus(Enum):
     PENDING = 0
@@ -48,14 +49,16 @@
     Task represents a task that an agent must complete
     """
 
     goal: str
     description: str
     result: Union[TaskResult, None] = None
     status: TaskStatus = TaskStatus.PENDING
+    start_time: Optional[datetime] = None
+    end_time: Optional[datetime] = None
 
     def update(self, result: TaskResult):
         """
         Updates the task with the result from its execution
         :param result: The result for executing the task
         """
         if result.outcome == TaskOutcome.MEETS_REQUIREMENT:
```

### Comparing `nagatoai_core-0.1.0/nagatoai_core/prompt/templates.py` & `nagatoai_core-0.7.0/nagatoai_core/prompt/templates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,36 @@
-OBJECTIVE_PROMPT = """Based on the following problem statement included in the <problem> tags, please do the following:
+TOOLS_AVAILABLE_TEMPLATE = """<tools_available>
+    {tools_available}
+</tools_available>"""
+
+OBJECTIVE_PROMPT = """Think step by step. Based on the following problem statement included in the <problem> tags, and the list of tools available under the <tools_available> tag, please do the following:
 1. Formulate an objective for the problem statement. Include this objective in the <objective> tags.
 2. Break down the objective into smaller tasks. Include these tasks in the <tasks><task> tags.
+3. If necessary, inside each task recommend, but do not mandate, the use of a given tool under <tools_recommended> if you believe it would aid in the completion of the task. If you do not recommend any tool then do not include a <tools_recommended> tag.
 
 ---
 Use the following example as reference:
 EXAMPLE 1:
 For the following problem statement
 <problem>
 It is my mother's 60th birthday in 2 weeks. I still haven't found a gift for her. Please help me find the right gift for her birthday.
 </problem>
 
+And the following tools available:
+<tools_available>
+    <tool>
+        <name>google_form</name>
+        <description>Tool to create a questionnaire for gathering information.</description>
+    </tool>
+    <tool>
+        <name>serp_search</name>
+        <description>SEO Search</description>
+    </tool>
+</tools_available>
+
 The objective could be:
 <objective>
 Find the right gift for the user mother's 60th birthday.
 </objective>
 
 Then the tasks could be:
 <tasks>
@@ -25,14 +42,19 @@
         Compile a detailed questionnaire designed to understand the preferences, hobbies, needs, and desires of the user's mother without directly hinting that it's for a gift selection for her 60th birthday.
         1. **Personal Interests:** Questions about her hobbies, favorite leisure activities, and any new interests she might want to explore.
         2. **Items She Needs:** Inquire discreetly if there's something specific she has mentioned wanting or needing recently.
         3. **Cherished Memories:** Ask about any special memories or life milestones she cherishes, which could inspire a meaningful gift.
         4. **Lifestyle:** Understand her lifestyle, including whether she prefers experiences over physical gifts, or if there are any changes she's considering making to her lifestyle.
         5. **Preferences:** Get insights into her preference regarding jewelry, clothing sizes, favorite colors, authors, artists, or other personal tastes that could influence the gift choice.
       </description>
+      <tools_recommended>
+        <tool>
+            <name>google_form</name>
+        </tool>
+      </tools_recommended>
     </task>
     <task>
         <goal>Generate a comprehensive document outlining gift ideas based on the answers from the questionnaire.</goal>
         <description>
             Analyze the responses to the Mother's 60th Birthday Gift Questionnaire to identify suitable gift ideas.
             1. **Read and Summarize:** Carefully read through the responses provided to the questionnaire. Summarize each response to capture the essence of the mother's interests, needs, and preferences.                                                                                                                                                                                                                                                                                                  │
             2. **Gift Categories Identification:** Based on the summary, categorize the responses into relevant gift categories. These categories could include hobbies, daily needs, cherished memories, lifestyle preferences, and aspirational gifts.
@@ -52,29 +74,32 @@
 ---
 
 For the problem statement below:
 <problem>
 {problem_statement}
 </problem>
 
-Please provide the objective and tasks as per the example above.
+And the tools available:
+{tools_available}
+
+Please provide the objective and tasks as per the example above. Recommend (but do not mandate) the use of tools where necessary.
 """
 
 
 COORDINATOR_SYSTEM_PROMPT = """You are an AI Agent with advanced reasoning capabilities. Your role is to assist users in solving complex problems. Your approach to problem solving is methodical.
 When given a problem statement, you use your advanced reasoning abilities to turn the problem statement into a single objective that can be broken down into smaller tasks.
 Once the objective is formulated, you break it down into smaller tasks that can be completed sequentially to achieve the objective.
 """
 
 
 RESEARCHER_SYSTEM_PROMPT = """You are an AI Agent with advanced research capabilities. Your role is to assist users in conducting in-depth research on various topics.
 When given a research question or topic, you use your advanced research abilities to gather relevant information, analyze data, and provide detailed insights.
 """
 
-RESEARCHER_TASK_PROMPT = """Execute the following task using the appropriate tools at your disposal. Provide a detailed result based on your research findings.
+RESEARCHER_TASK_PROMPT_WITH_EXAMPLE = """Execute the following task using the appropriate tools at your disposal. Provide a detailed result based on your research findings.
 ---
 For an example task in this format:
 <task>
     <goal>
     Gather information about the user mother's tastes, preferences, and needs to identify potential gift ideas.
     </goal>
     <description>
@@ -105,24 +130,96 @@
 
 For the task below:
 <task>
     <goal>{goal}</goal>
     <description>{description}</description>
 </task>
 
+Please provide a detailed result inside <task_result> tags. Ensure to output correctly formed XML tags (e.g. opening <task_result> and closing </task_result> tags).
+"""
+
+
+RESEARCHER_TASK_PROMPT_NO_EXAMPLE = """Execute the following task using the appropriate tools at your disposal. Provide a detailed result based on your execution.
+
+For the task below:
+<task>
+    <goal>{goal}</goal>
+    <description>{description}</description>
+</task>
+
 Please provide a detailed result inside <task_result> tags.
 """
 
 
+RESEARCHER_TASK_PROMPT_WITH_PREVIOUS_UNSATISFACTORY_TASK_RESULT = """The task below has already been executed, however the result was deemed unsatisfactory by the reviewer agent. The reviewer agent provided details of its review inside the <task_evaluation> tags below:
+
+<task_evaluation>
+    <goal>{goal}</goal>
+    <outcome>{outcome}</outcome>
+    <evaluation>{evaluation}</evaluation>
+</task_evaluation>
+
+The possible values inside the <outcome> tag are:
+- MEETS_REQUIREMENT: the reslt meets the requirements of the task.
+- PARTIALLY_MEETS_REQUIREMENT: the result partially meets the requirements of the task. Some aspects are missing or incomplete.
+- DOES_NOT_MEET_REQUIREMENT: the result does not meet the requirements of the task. The result is inaccurate or incomplete.
+- OTHER: for any other evaluation that does not fit the above categories. Provide a detailed explanation in the <evaluation> tag.
+
+The outcome of your task is {outcome}. Additionally, the reviewer provided detailed feedback on why it did not meet the requirements inside the <evaluation> tags.
+
+Therefore, your task is to address the issues raised by the reviewer agent and provide a revised result.
+
+Execute the task below while taking into account the feedback provided by the reviewer agent.
+<task>
+    <goal>{goal}</goal>
+    <description>{description}</description>
+</task>
+
+Please provide a detailed result inside <task_result> tags.
+"""
+
+# If any tools are required to complete the task, list them under the <tools_to_use> tag.
+# If you have been provided a list of tools as part of the input, then list any of these tools that are required to complete the task. Please list them under the <tools_to_use> tag in your text text response too.
+# <tools_to_use>
+#     <tool>
+#         <name>google_form</name>
+#         <inputs>
+#             <input>
+#                 <name>question_1</name>
+#                 <value>What are your hobbies and favorite leisure activities?</value>
+#             </input>
+#             <input>
+#                 <name>question_2</name>
+#                 <value>Is there something specific you have mentioned wanting or needing recently?</value>
+#             </input>
+#             <input>
+#                 <name>question_3</name>
+#                 <value>What special memories or life milestones do you cherish?</value>
+#             </input>
+#             <input>
+#                 <name>question_4</name>
+#                 <value>Do you prefer experiences over physical gifts?</value>
+#             </input>
+#             <input>
+#                 <name>question_5</name>
+#                 <value>What are your preferences regarding jewelry, clothing sizes, favorite colors, authors, artists, or other personal tastes?</value>
+#             </input>
+#         </inputs>
+#     </tool>
+# </tools_to_use>
+
+# If a tool must be used to complete the task, then I would also expect the stop_reason to be "tool_use" in the response.
+
+
 CRITIC_SYSTEM_PROMPT = """You are an AI Agent with advanced analytical capabilities. Your role is to evaluate the work of other agents and provide constructive feedback.
 When given a result from another agent, you analyze the result based on the original task's goal and description to determine wether the result from the agent satisfies the task requirements.
 """
 
 CRITIC_PROMPT = """Analyze the result provided by the agent and evaluate whether it meets the requirements of the task.
-Determine whether the task's goal has been met and ptovide detailed feedback based on your assessment on whether the result meets the requirements of the task.
+Determine whether the task's goal has been met and provide detailed feedback based on your assessment on whether the result meets the requirements of the task.
 If the requirement is not met, provide feedback on what aspects are missing or incomplete.
 If for instance a tool is required to complete the task and the agent did not use the tool, then list the tool required under the <tools_required> tag.
 ---
 For example for the given task below:
 <task>
     <goal>
     Gather information about the user mother's tastes, preferences, and needs to identify potential gift ideas.
@@ -261,15 +358,15 @@
 </task>
 
 <task_result>
     <goal>{goal}</goal>
     <result>{result}</result>
 </task_result>
 
-Please provide an evaluation of the result in the format described above.
+Please provide an evaluation of the result in the format described above. Ensure to output correctly formed XML tags (e.g. opening <task_evaluation> and closing </task_evaluation> tags).
 """
 
 MARKDOWN_AGENT_SYSTEM_PROMPT = """You are an AI Agent with advanced markdown capabilities.
 Your role is to assist users in summarising and formatting text which comes from the outputs of the run of multiple AI Agents trying to solve a given problem.
 The input text will contain xml that represent the structure of the outputs from the agents. You are adept at transforming this xml into properly formatted markdown content.
 """
```

### Comparing `nagatoai_core-0.1.0/pyproject.toml` & `nagatoai_core-0.7.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 [tool.poetry]
 name = "nagatoai_core"
-version = "0.1.0"
+version = "0.7.0"
 description = "Nagato-AI is an intuitive AI Agent library that works across multiple LLMs"
 authors = ["Eddie Forson <eddie@edforson.me>"]
 readme = "README.md"
 package-mode = true
+exclude = [
+    ".env",
+    ".env.*",
+    "inputs",
+    "outputs"
+]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-anthropic = "^0.21.3"
+anthropic = "^0.23.1"
 rich = "^13.7.1"
 requests = "^2.31.0"
 pytest = "^8.1.1"
 openai = "^1.14.3"
 beautifulsoup4 = "^4.12.3"
 lxml = "^5.1.0"
 pydantic = "^2.6.4"
 python-dotenv = "^1.0.1"
+pydantic-settings = "^2.2.1"
+groq = "^0.5.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nagatoai_core-0.1.0/PKG-INFO` & `nagatoai_core-0.7.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: nagatoai_core
-Version: 0.1.0
+Version: 0.7.0
 Summary: Nagato-AI is an intuitive AI Agent library that works across multiple LLMs
 Author: Eddie Forson
 Author-email: eddie@edforson.me
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anthropic (>=0.21.3,<0.22.0)
+Requires-Dist: anthropic (>=0.23.1,<0.24.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: groq (>=0.5.0,<0.6.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 [![X (formerly Twitter)](https://img.shields.io/twitter/follow/Ed_Forson?style=social)](https://twitter.com/Ed_Forson)
 [![GitHub](https://img.shields.io/github/followers/kenshiro-o?label=Follow&style=social)](https://github.com/kenshiro-o)
 
 # Nagato-AI
 
-![Official Nagato AI Poster](docs/assets/Official_nagatoai_core_Poster.webp)
+![Official Nagato AI Poster](docs/assets/Official_Nagato_AI_Poster.webp)
 
 
 Nagato-AI is an intuitive AI Agent library that works across multiple LLMs.
 
 Currently it supports OpenAI's GPT and Anthpropic's Claude LLMs. You can create agents from any of the aforementioned family of models and combine them together to build the most effective AI Agent system you desire.
 
 The name _Nagato_ is inspired from the popular anime Naruto. In Naruto, Nagato is a very powerful ninja who possesses special eyes (Rinnegan) that gives him immense powers.
@@ -52,14 +54,22 @@
 
 Assuming your program's entrypoint is defined in a file called `main.py`, you can run it by typing the following command:
 
 ```
 poetry run python main.py
 ```
 
+
+## LLMs supported
+
+Nagato currently supports the following LLMs
+* Claude 3 (Anthropic)
+* GPT-3 to GPT-4 (OpenAI)
+* Groq (which gives you access to Llama 3) 🔥
+
 ## Examples of AI Agent configuration
 
 Nagato is built with flexibility at its core, so you could program it using your paradigm of choice. However these are some of the ways I've seen people use Nagato so far.
 
 ### Coordinator, worker, and critic agents
 
 In this configuration we have the following:
@@ -75,38 +85,39 @@
     organization="<org-id>",
     api_key="<api-key>",
 )
 
 anthropic_api_key = "<api-key>"
 anthropic_client = Anthropic(api_key=anthropic_api_key)
 
+groq_client = Groq(api_key="<api-key>")
+
 coordinator_agent: Agent = AnthropicAgent(
     anthropic_client,
     "claude-3-opus-20240229",
     "Coordinator",
     COORDINATOR_SYSTEM_PROMPT,
     "Coordinator Agent",
 )
 
-researcher_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-sonnet-20240229",
+researcher_agent: Agent = OpenAIAgent(
+    openai_client,
+    "gpt-4-turbo-2024-04-09",
     "Researcher",
     RESEARCHER_SYSTEM_PROMPT,
     "Researcher Agent",
 )
 
-critic_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-opus-20240229",
+critic_agent: Agent = GroqAgent(
+    groq_client,
+    "llama3-70b-8192",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
-
 ...
 ```
 
 The full blow example is available [here](docs/examples/coordinator_researcher_critic.py)
 
 ### Worker and critic agents
 
@@ -120,19 +131,14 @@
         goal="Fetch last 100 user tweets",
         description="Fetch the tweets from the user using the Twitter API. Limit the number of tweets fetched to 100 only."),
     Task(
         goal="Perform sentiment analysis on the tweets",
         description="Feed the tweets to the AI Agent to analyze sentiment per overall sentiment acoss tweets. Range of values for sentiment can be: Positive, Negative, or Neutral"
     )]
 
-openai_client = OpenAI(
-    organization="<org-id>",
-    api_key="<api-key>",
-)
-
 anthropic_api_key = "<api-key>"
 anthropic_client = Anthropic(api_key=anthropic_api_key)
 
 researcher_agent: Agent = AnthropicAgent(
     anthropic_client,
     "claude-3-sonnet-20240229",
     "Researcher",
@@ -159,25 +165,88 @@
 
     critic_exchange = critic_agent(critic_prompt, task, 0.7, 2000)
 
     # Evaluate whether the task was completed based on the answer from the critic agent
     ...
 ```
 
+## Tool calling
+
+Check the full example [here](docs/examples/coordinator_researcher_critic.py) to see how tool calling works.
+We now support tool calling for  GPT, Claude 3, and Llama 3 (via Groq) models.
+
+
+### Tool creation
+
+Creating a tool is straightforward. You must create have these two elements in place for a tool to be usable:
+
+1. A config class that contains the parameters that your tool will be called with
+2. A tool class that inherits from `AbstractTool`, and contains the main logic for your tool.
+
+For instance the below shows how we've created a tool to get the user to confirm yes/no in the terminal
+
+```python
+from typing import Any, Type
+
+from pydantic import BaseModel, Field
+from rich.prompt import Confirm
+
+from nagatoai_core.tool.abstract_tool import AbstractTool
+
+
+class HumanConfirmInputConfig(BaseModel):
+    """
+    HumanConfirmInputConfig represents the configuration for the HumanConfirmInputTool.
+    """
+
+    message: str = Field(
+        ...,
+        description="The message to display to the user to confirm whether to proceed or not",
+    )
+
+
+class HumanConfirmInputTool(AbstractTool):
+    """
+    HumanConfirmInputTool represents a tool that prompts the user to confirm whether to proceed or not.
+    """
+
+    name: str = "human_confirm_input"
+    description: str = (
+        """Prompts the user to confirm whether to proceed or not. Returns a boolean value indicating the user's choice."""
+    )
+    args_schema: Type[BaseModel] = HumanConfirmInputConfig
+
+    def _run(self, config: HumanConfirmInputConfig) -> Any:
+        """
+        Prompts the user to confirm whether to proceed or not.
+        :param message: The message to display to the user to confirm whether to proceed or not.
+        :return: A boolean value indicating the user's choice.
+        """
+        confirm = Confirm.ask("[bold yellow]" + config.message + "[/bold yellow]")
+
+        return confirm
+```
+
+
+
 # What's next
 
 Nagato is still in its very early development phase. This means that I am likely to introduce breaking changes over the next iterations of the library.
 
 Moreover, there is a lot of functionality currently missing from Nagato. I will remedy this over time. There is no official roadmap per se but I plan to add the following capabilities to Nagato:
 
-* introduction of tools (e.g. surfing the web)
-* support for function calling (complement to adding tools)
-* support for other LLMs beyond OpenAI's and Anthropic's
-* short/long-term memory for agents
-* LLMOps instrumentation
+* ✅ implement function calling (complement to adding tools)
+* ✅ introduce basic tools (e.g. surfing the web)
+* ✅ Support for Llama 3 (via Groq)
+* 🎯 cache results from function calling
+* 🎯 implement short/long-term memory for agents (with RAG and memory synthesis)
+* 🎯 implement self-reflection and re-planning for agents
+* 🎯 implement additional modalities (e.g. image, sound, etc.)
+* 🎯 Support for local LLMs (e.g. via Ollama)
+* 🎯 LLMOps instrumentation
 
 # How can you support
 
 I'd be grateful if you could do some of the following to support this project:
 
 * star this repository on Github
 * follow me on [X/Twitter](https://twitter.com/Ed_Forson)
```

