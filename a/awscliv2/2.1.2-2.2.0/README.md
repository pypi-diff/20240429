# Comparing `tmp/awscliv2-2.1.2.tar.gz` & `tmp/awscliv2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awscliv2-2.1.2.tar", max compression
+gzip compressed data, was "awscliv2-2.2.0.tar", max compression
```

## Comparing `awscliv2-2.1.2.tar` & `awscliv2-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2022-05-25 20:59:55.021712 awscliv2-2.1.2/LICENSE
--rw-r--r--   0        0        0     3794 2022-05-25 20:59:55.021712 awscliv2-2.1.2/README.md
--rw-r--r--   0        0        0        0 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/__init__.py
--rw-r--r--   0        0        0      117 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/__main__.py
--rw-r--r--   0        0        0     5579 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/awscli_runner.py
--rw-r--r--   0        0        0     2178 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/cli_parser.py
--rw-r--r--   0        0        0      403 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/constants.py
--rw-r--r--   0        0        0      626 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/exceptions.py
--rw-r--r--   0        0        0     4079 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/installers.py
--rw-r--r--   0        0        0     3082 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/interactive_process.py
--rw-r--r--   0        0        0      715 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/logger.py
--rw-r--r--   0        0        0     1786 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/main.py
--rw-r--r--   0        0        0        0 2022-05-25 20:59:55.021712 awscliv2-2.1.2/awscliv2/py.typed
--rw-r--r--   0        0        0     2731 2022-05-25 21:00:32.589926 awscliv2-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4738 2022-05-25 21:00:36.193225 awscliv2-2.1.2/setup.py
--rw-r--r--   0        0        0     5245 2022-05-25 21:00:36.193583 awscliv2-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-05-25 22:38:33.719561 awscliv2-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4702 2022-05-25 22:38:33.719561 awscliv2-2.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/__init__.py
+-rw-r--r--   0        0        0      117 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/__main__.py
+-rw-r--r--   0        0        0     6245 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/api.py
+-rw-r--r--   0        0        0     2268 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/cli_parser.py
+-rw-r--r--   0        0        0      403 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/constants.py
+-rw-r--r--   0        0        0      626 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/exceptions.py
+-rw-r--r--   0        0        0     4079 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/installers.py
+-rw-r--r--   0        0        0     3086 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/interactive_process.py
+-rw-r--r--   0        0        0      715 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/logger.py
+-rw-r--r--   0        0        0     1855 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/main.py
+-rw-r--r--   0        0        0        0 2022-05-25 22:38:33.719561 awscliv2-2.2.0/awscliv2/py.typed
+-rw-r--r--   0        0        0     2731 2022-05-25 22:39:14.563021 awscliv2-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5696 2022-05-25 22:39:18.306274 awscliv2-2.2.0/setup.py
+-rw-r--r--   0        0        0     6153 2022-05-25 22:39:18.306759 awscliv2-2.2.0/PKG-INFO
```

### Comparing `awscliv2-2.1.2/LICENSE` & `awscliv2-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awscliv2-2.1.2/README.md` & `awscliv2-2.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-# AWS CLI v2 for Python 
+# AWS CLI v2 for Python
 
 [![PyPI - awscliv2](https://img.shields.io/pypi/v/awscliv2.svg?color=blue&label=awscliv2)](https://pypi.org/project/awscliv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/awscliv2.svg?color=blue)](https://pypi.org/project/awscliv2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/awscliv2?color=blue)](https://pypistats.org/packages/awscliv2)
 
 Wrapper for [AWS CLI v2](https://awscli.amazonaws.com/v2/documentation/api/latest/index.html).
-Comes with zero dependencies, updates `awscli`, gives access to all services!
+
+- No dependency hell, like with original [awscli](https://pypi.org/project/awscli/)
+- Can install and update `awscliv2` binaries
+- Provides access to all services
+- Has Python interface
 
 - [AWS CLI v2 for Python](#aws-cli-v2-for-python)
   - [Before you start](#before-you-start)
   - [Installation](#installation)
   - [Usage](#usage)
+    - [From command line](#from-command-line)
     - [Docker fallback](#docker-fallback)
     - [Extra commands](#extra-commands)
+    - [As a Python module](#as-a-python-module)
   - [Development](#development)
   - [How to help](#how-to-help)
   - [Versioning](#versioning)
   - [Latest changes](#latest-changes)
 
 ## Before you start
 
@@ -35,14 +42,16 @@
 
 ```bash
 alias aws='awsv2'
 ```
 
 ## Usage
 
+### From command line
+
 Install `AWS CLI v2`:
 
 ```bash
 # do not worry if this fails, you can still use awsv2 if you have docker installed
 awsv2 --install
 ```
 
@@ -82,31 +91,66 @@
 - `$(cwd)` -> `/aws` - Docker image workdir
 
 ### Extra commands
 
 `awscliv2` contains a few commands to make your life easier, especially in CI or any non-TTY environment.
 
 - `awsv2 -U/--update/--install` - Install `AWS CLI v2`
-- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>]` - set profile in `~/.aws/credentials`
+- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>] [<region>]` - set profile in `~/.aws/credentials`
 - `awsv2 --assume-role <profile_name> <source_profile> <role_arn>` - create a new profile with assume role credentials
 - `awsv2 -V/--version` - Output `awscliv2` and `AWS CLI v2` versions
 
+### As a Python module
+
+Basic usage
+
+```python
+from awscliv2.api import AWSAPI
+from awscliv2.exceptions import AWSCLIError
+
+aws_api = AWSAPI()
+
+try:
+    output = aws_api.execute(["s3", "ls"])
+except AWSCLIError as e:
+    print(f"Something went wrong: {e}")
+else:
+    print(output)
+```
+
+Install binaries for your OS from Python
+
+```python
+from awscliv2.installers import install_multiplatform
+
+install_multiplatform()
+```
+
+You can also set credentials or assume roles
+
+```python
+from awscliv2.api import AWSAPI
+
+aws_api = AWSAPI()
+
+aws_api.set_credentials("profile_name", "access_key", "secret_key", "", "region")
+aws_api.assume_role("name", "source_profile", "role_arn")
+```
+
 ## Development
 
 - Install [poetry](https://python-poetry.org/)
 - Run `poetry install`
 - Use `black` formatter in your IDE
 
 ## How to help
 
 - Ping AWS team to release an official PyPI package
-- Help me to test MacOS installer and add Windows installer
 - Share your experience in issues
 
 ## Versioning
 
 `awscliv2` version follows [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ## Latest changes
 
-Full changelog can be found in [Changelog](./CHANGELOG.md).
-Release notes can be found in [Releases](https://github.com/youtype/awscliv2/releases).
+Full changelog can be found in [Releases](https://github.com/youtype/awscliv2/releases).
```

### Comparing `awscliv2-2.1.2/awscliv2/awscli_runner.py` & `awscliv2-2.2.0/awscliv2/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,34 @@
 from configparser import ConfigParser
 from io import StringIO
 from pathlib import Path
 from typing import List, Optional, Sequence, TextIO
 
 import executor  # type: ignore
 
-from awscliv2.constants import DOCKER_PATH, IMAGE_NAME
+from awscliv2.constants import DOCKER_PATH, ENCODING, IMAGE_NAME
 from awscliv2.exceptions import AWSCLIError, ExecutableNotFoundError, SubprocessError
 from awscliv2.interactive_process import InteractiveProcess
 from awscliv2.logger import get_logger
 
 
-class AWSCLIRunner:
+class AWSAPI:
     """
-    Runner for all AWS CLI v2 commands.
+    API for all AWS CLI v2 commands.
 
     Supports installed and dockerized AWS CLI v2.
+
+    Arguments:
+        encoding -- Input/output encoding, default utf-8.
+        output -- Output stream, default sys.stdout.
     """
 
-    def __init__(self, encoding: str) -> None:
+    def __init__(self, encoding: str = ENCODING, output: Optional[TextIO] = None) -> None:
         self.encoding = encoding
+        self.output = output
         self.logger = get_logger()
 
     @staticmethod
     def get_awscli_v2_cmd() -> List[str]:
         """
         Get command to run AWS CLI v2.
         """
@@ -48,48 +53,69 @@
             "-v",
             f"{Path.home().as_posix()}/.aws:/root/.aws",
             "-v",
             f"{Path.cwd().as_posix()}:/aws",
             IMAGE_NAME,
         ]
 
-    def _run_subprocess(self, cmd: Sequence[str], stdout: TextIO = sys.stdout) -> int:
+    def _run_subprocess(self, cmd: Sequence[str]) -> int:
         process = InteractiveProcess(cmd, encoding=self.encoding)
         try:
-            return_code = process.run(stdout=stdout)
+            return_code = process.run(stdout=self.output or sys.stdout)
         except SubprocessError as e:
             raise AWSCLIError(str(e)) from e
 
         return return_code
 
     def _run_detached_subprocess(self, cmd: Sequence[str]) -> int:
         try:
             executor.execute(*cmd, encoding=self.encoding)
         except executor.ExternalCommandFailed as e:
             self.logger.error(f"Command failed with code {e.returncode}")
             return e.returncode
 
         return 0
 
-    def run_awscli_v2(self, args: Sequence[str], stdout: TextIO = sys.stdout) -> int:
+    def execute(self, args: Sequence[str]) -> str:
+        """
+        Execute AWS CLI v2 command.
+
+        Returns:
+            Command output.
+        """
+        old_output = self.output
+        self.output = StringIO()
+        self.run_awscli_v2(args)
+        self.output.seek(0)
+        result = self.output.read()
+        self.output = old_output
+        return result
+
+    def run_awscli_v2(self, args: Sequence[str]) -> int:
         """
         Run AWS CLI.
+
+        Returns:
+            Process exit code.
         """
         cmd = [
             *self.get_awscli_v2_cmd(),
             *args,
         ]
         try:
-            return self._run_subprocess(cmd, stdout=stdout)
+            return self._run_subprocess(cmd)
         except ExecutableNotFoundError as e:
             raise AWSCLIError(f"Executable not found: {cmd[0]}") from e
 
     def run_awscli_v2_detached(self, args: Sequence[str]) -> int:
         """
         Run AWS CLI as a detached subprocess.
+
+        Returns:
+            Process exit code.
         """
         cmd = [
             *self.get_awscli_v2_cmd(),
             *args,
         ]
         try:
             return self._run_detached_subprocess(cmd)
@@ -101,15 +127,15 @@
         Print AWS CLI v2 version.
 
         Returns:
             Process exit code.
         """
         return self.run_awscli_v2(["--version"])
 
-    def run_assume_role(self, profile_name: str, source_profile: str, role_arn: str) -> None:
+    def assume_role(self, profile_name: str, source_profile: str, role_arn: str) -> None:
         """
         Add assume role to credentials.
         """
         aws_path = Path.home() / ".aws"
         if not aws_path.exists():
             aws_path.mkdir(parents=True, exist_ok=True)
         credentials_path = aws_path / "credentials"
@@ -124,15 +150,14 @@
                 "sts",
                 "assume-role",
                 "--role-arn",
                 role_arn,
                 "--role-session-name",
                 f"{profile_name}-{source_profile}",
             ],
-            stdout=stdout,
         )
         if return_code:
             raise AWSCLIError(stdout.getvalue().strip())
 
         credentials_json = stdout.getvalue()
         credentials_data = json.loads(credentials_json)
         self.set_credentials(
@@ -143,15 +168,16 @@
         )
 
     def set_credentials(
         self,
         profile_name: str,
         aws_access_key_id: str,
         aws_secret_access_key: str,
-        aws_session_token: Optional[str] = None,
+        aws_session_token: str = "",
+        region: str = "",
     ) -> None:
         """
         Add or update credentials in `~/.aws/credentials`
         """
         aws_path = Path.home() / ".aws"
         if not aws_path.exists():
             aws_path.mkdir(parents=True, exist_ok=True)
@@ -163,14 +189,16 @@
         config.read(credentials_path)
         credentials = {
             "aws_access_key_id": aws_access_key_id,
             "aws_secret_access_key": aws_secret_access_key,
         }
         if aws_session_token:
             credentials["aws_session_token"] = aws_session_token
+        if region:
+            credentials["region"] = region
 
         config[profile_name] = credentials
 
         output = StringIO()
         config.write(output)
         credentials_path.write_text(output.getvalue(), encoding=self.encoding)
         self.logger.info(
```

### Comparing `awscliv2-2.1.2/awscliv2/cli_parser.py` & `awscliv2-2.2.0/awscliv2/cli_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,19 +48,23 @@
 
 def parse_args(args: Sequence[str]) -> CLINamespace:
     """
     Parse CLI arguments.
     """
     parser = argparse.ArgumentParser(PROG_NAME, description="Can be used as a regular AWS CLI v2")
     parser.add_argument(
-        "--configure", nargs="+", help="Configure profile: <name> <access_key> <secret_key>"
+        "--configure",
+        nargs="+",
+        metavar="STR",
+        help="Configure profile: <name> <access_key> <secret_key> [<session_token>] [<region>]",
     )
     parser.add_argument(
         "--assume-role",
-        nargs="+",
+        nargs=3,
+        metavar="STR",
         help="Configure assume role profile: <name> <source_profile> <role_arn>",
     )
     parser.add_argument("-V", "--version", action="store_true", help="Show version")
     parser.add_argument(
         "-U", "--update", action="store_true", help="Install AWS CLI v2 (deprecated)"
     )
     parser.add_argument("-i", "--install", action="store_true", help="Install AWS CLI v2")
```

### Comparing `awscliv2-2.1.2/awscliv2/exceptions.py` & `awscliv2-2.2.0/awscliv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `awscliv2-2.1.2/awscliv2/installers.py` & `awscliv2-2.2.0/awscliv2/installers.py`

 * *Files identical despite different names*

### Comparing `awscliv2-2.1.2/awscliv2/interactive_process.py` & `awscliv2-2.2.0/awscliv2/interactive_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
             if self.finished:
                 break
 
             output_data = process.stdout.read(1)
             if not output_data:
                 break
             output_data_dec = output_data.decode(self.encoding)
-            if output.endswith("\n") and not output_data_dec.strip():
-                continue
+            # if output.endswith("\n") and not output_data_dec.strip():
+            #     continue
             output = f"{output[-10:]}{output_data_dec}"
             stdout.write(output_data_dec)
             stdout.flush()
 
     def readall(self, process: Popen, stdin: TextIO) -> None:  # type: ignore
         """
         Write input from `stdin` stream to `process`.
```

### Comparing `awscliv2-2.1.2/awscliv2/logger.py` & `awscliv2-2.2.0/awscliv2/logger.py`

 * *Files identical despite different names*

### Comparing `awscliv2-2.1.2/awscliv2/main.py` & `awscliv2-2.2.0/awscliv2/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 """
 Main entrypoint for CLI.
 """
 import sys
 from typing import Sequence
 
-from awscliv2.awscli_runner import AWSCLIRunner
+from awscliv2.api import AWSAPI
 from awscliv2.cli_parser import get_version, parse_args
 from awscliv2.exceptions import AWSCLIError
 from awscliv2.installers import install_multiplatform
 from awscliv2.logger import get_logger
 
 
-def main(args: Sequence[str]) -> None:
+def main(args: Sequence[str]) -> int:
     """
     Main program entrypoint.
     """
     namespace = parse_args(args)
-    runner = AWSCLIRunner(encoding=namespace.encoding)
+    runner = AWSAPI(encoding=namespace.encoding, output=sys.stdout)
 
     if namespace.install or namespace.update:
         install_multiplatform()
         runner.print_version()
-        sys.exit(0)
+        return 0
 
     if namespace.version:
         version = get_version()
         print(version)
         cmd = " ".join(runner.get_awscli_v2_cmd())
         print(f"AWS CLI v2 command: {cmd}")
         runner.print_version()
-        sys.exit(0)
+        return 0
 
     if namespace.assume_role:
         try:
-            return runner.run_assume_role(*namespace.assume_role[:3])
+            runner.assume_role(*namespace.assume_role[:3])
         except TypeError:
             raise AWSCLIError("Use --assume-role <name> <source_profile> <role_arn>") from None
+        return 0
 
     if namespace.configure:
         try:
-            return runner.set_credentials(*namespace.configure[:4])
+            runner.set_credentials(*namespace.configure[:5])
         except TypeError:
             raise AWSCLIError(
-                "Use --configure <profile_name> <access_key> <secret_key> [<session_token>]"
+                "Use --configure <profile_name> <access_key>"
+                " <secret_key> [<session_token>] [<region>]"
             ) from None
+        return 0
 
     if not namespace.other:
         raise AWSCLIError("No command provided")
 
-    sys.exit(runner.run_awscli_v2_detached(namespace.other))
+    exit_code = runner.run_awscli_v2_detached(namespace.other)
+    return exit_code
 
 
 def main_cli() -> None:
     """
     Main entrypoint for CLI.
     """
     try:
-        main(sys.argv[1:])
+        sys.exit(main(sys.argv[1:]))
     except AWSCLIError as e:
         message = str(e)
         if message:
             logger = get_logger()
             logger.error(message)
         sys.exit(e.returncode)
```

### Comparing `awscliv2-2.1.2/pyproject.toml` & `awscliv2-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "awscliv2",
     "tests",
 ]
 src_paths = []
 
 [tool.poetry]
 name = "awscliv2"
-version = "2.1.2"
+version = "2.2.0"
 description = "Wrapper for AWS CLI v2"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/awscliv2/"
 repository = "https://github.com/youtype/awscliv2"
 documentation = "https://youtype.github.io/awscliv2/"
```

### Comparing `awscliv2-2.1.2/setup.py` & `awscliv2-2.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['awscliv2 = awscliv2.main:main_cli',
                      'awsv2 = awscliv2.main:main_cli']}
 
 setup_kwargs = {
     'name': 'awscliv2',
-    'version': '2.1.2',
+    'version': '2.2.0',
     'description': 'Wrapper for AWS CLI v2',
-    'long_description': "# AWS CLI v2 for Python \n\n[![PyPI - awscliv2](https://img.shields.io/pypi/v/awscliv2.svg?color=blue&label=awscliv2)](https://pypi.org/project/awscliv2)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/awscliv2.svg?color=blue)](https://pypi.org/project/awscliv2)\n\nWrapper for [AWS CLI v2](https://awscli.amazonaws.com/v2/documentation/api/latest/index.html).\nComes with zero dependencies, updates `awscli`, gives access to all services!\n\n- [AWS CLI v2 for Python](#aws-cli-v2-for-python)\n  - [Before you start](#before-you-start)\n  - [Installation](#installation)\n  - [Usage](#usage)\n    - [Docker fallback](#docker-fallback)\n    - [Extra commands](#extra-commands)\n  - [Development](#development)\n  - [How to help](#how-to-help)\n  - [Versioning](#versioning)\n  - [Latest changes](#latest-changes)\n\n## Before you start\n\n- This is not an official AWS CLI v2 application, [rant there](https://github.com/aws/aws-cli/issues/4947)\n- Check the source code of this app, as you are working with sensitive data\n- By default this app uses [amazon/aws-cli](https://hub.docker.com/r/amazon/aws-cli) Docker image\n- To use [binaries for your OS](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html), run `awsv2 --install`\n- Cross-check the source code again, probably I want to steal your credentials\n\n## Installation\n\n```bash\npython -m pip install awscliv2\n```\n\nYou can add an alias to your `~/.bashrc` or `~/.zshrc` to use it as a regular `AWS CLI v2`\n\n```bash\nalias aws='awsv2'\n```\n\n## Usage\n\nInstall `AWS CLI v2`:\n\n```bash\n# do not worry if this fails, you can still use awsv2 if you have docker installed\nawsv2 --install\n```\n\nConfigure default profile if needed:\n\n```bash\nAWS_ACCESS_KEY_ID='my-access-key'\nAWS_SECRET_ACCESS_KEY='my-secret-key'\n\n# --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>]\nawsv2 --configure default ${AWS_ACCESS_KEY_ID} ${AWS_SECRET_ACCESS_KEY}\nawsv2 configure set region us-west-1\n```\n\nUse `AWS CLI` as usual:\n\n```bash\n# alias for\n# docker run --rm -i -v ~/.aws:/root/.aws -v $(pwd):/aws amazon/aws-cli $@\nawsv2 s3 ls\n\n# or as a python module\npython -m awscliv2 s3 ls\n```\n\nAlso, you can check [scripts/example.sh](https://github.com/youtype/awscliv2/blob/main/scripts/example.sh)\n\n### Docker fallback\n\nUnless you run `awsv2 --install` once, application will use [amazon/aws-cli](https://hub.docker.com/r/amazon/aws-cli) Docker image. The image is not ideal, and it uses `root` user, so fix downloaded file permissions manually. Or just run `awsv2 --install`\n\nUpdate it with `docker pull amazon/aws-cli`.\n\nContainer uses two volumes:\n\n- `$HOME/.aws` -> `/root/.aws` - credentials and config store\n- `$(cwd)` -> `/aws` - Docker image workdir\n\n### Extra commands\n\n`awscliv2` contains a few commands to make your life easier, especially in CI or any non-TTY environment.\n\n- `awsv2 -U/--update/--install` - Install `AWS CLI v2`\n- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>]` - set profile in `~/.aws/credentials`\n- `awsv2 --assume-role <profile_name> <source_profile> <role_arn>` - create a new profile with assume role credentials\n- `awsv2 -V/--version` - Output `awscliv2` and `AWS CLI v2` versions\n\n## Development\n\n- Install [poetry](https://python-poetry.org/)\n- Run `poetry install`\n- Use `black` formatter in your IDE\n\n## How to help\n\n- Ping AWS team to release an official PyPI package\n- Help me to test MacOS installer and add Windows installer\n- Share your experience in issues\n\n## Versioning\n\n`awscliv2` version follows [PEP 440](https://www.python.org/dev/peps/pep-0440/).\n\n## Latest changes\n\nFull changelog can be found in [Changelog](./CHANGELOG.md).\nRelease notes can be found in [Releases](https://github.com/youtype/awscliv2/releases).\n",
+    'long_description': '# AWS CLI v2 for Python\n\n[![PyPI - awscliv2](https://img.shields.io/pypi/v/awscliv2.svg?color=blue&label=awscliv2)](https://pypi.org/project/awscliv2)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/awscliv2.svg?color=blue)](https://pypi.org/project/awscliv2)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/awscliv2?color=blue)](https://pypistats.org/packages/awscliv2)\n\nWrapper for [AWS CLI v2](https://awscli.amazonaws.com/v2/documentation/api/latest/index.html).\n\n- No dependency hell, like with original [awscli](https://pypi.org/project/awscli/)\n- Can install and update `awscliv2` binaries\n- Provides access to all services\n- Has Python interface\n\n- [AWS CLI v2 for Python](#aws-cli-v2-for-python)\n  - [Before you start](#before-you-start)\n  - [Installation](#installation)\n  - [Usage](#usage)\n    - [From command line](#from-command-line)\n    - [Docker fallback](#docker-fallback)\n    - [Extra commands](#extra-commands)\n    - [As a Python module](#as-a-python-module)\n  - [Development](#development)\n  - [How to help](#how-to-help)\n  - [Versioning](#versioning)\n  - [Latest changes](#latest-changes)\n\n## Before you start\n\n- This is not an official AWS CLI v2 application, [rant there](https://github.com/aws/aws-cli/issues/4947)\n- Check the source code of this app, as you are working with sensitive data\n- By default this app uses [amazon/aws-cli](https://hub.docker.com/r/amazon/aws-cli) Docker image\n- To use [binaries for your OS](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html), run `awsv2 --install`\n- Cross-check the source code again, probably I want to steal your credentials\n\n## Installation\n\n```bash\npython -m pip install awscliv2\n```\n\nYou can add an alias to your `~/.bashrc` or `~/.zshrc` to use it as a regular `AWS CLI v2`\n\n```bash\nalias aws=\'awsv2\'\n```\n\n## Usage\n\n### From command line\n\nInstall `AWS CLI v2`:\n\n```bash\n# do not worry if this fails, you can still use awsv2 if you have docker installed\nawsv2 --install\n```\n\nConfigure default profile if needed:\n\n```bash\nAWS_ACCESS_KEY_ID=\'my-access-key\'\nAWS_SECRET_ACCESS_KEY=\'my-secret-key\'\n\n# --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>]\nawsv2 --configure default ${AWS_ACCESS_KEY_ID} ${AWS_SECRET_ACCESS_KEY}\nawsv2 configure set region us-west-1\n```\n\nUse `AWS CLI` as usual:\n\n```bash\n# alias for\n# docker run --rm -i -v ~/.aws:/root/.aws -v $(pwd):/aws amazon/aws-cli $@\nawsv2 s3 ls\n\n# or as a python module\npython -m awscliv2 s3 ls\n```\n\nAlso, you can check [scripts/example.sh](https://github.com/youtype/awscliv2/blob/main/scripts/example.sh)\n\n### Docker fallback\n\nUnless you run `awsv2 --install` once, application will use [amazon/aws-cli](https://hub.docker.com/r/amazon/aws-cli) Docker image. The image is not ideal, and it uses `root` user, so fix downloaded file permissions manually. Or just run `awsv2 --install`\n\nUpdate it with `docker pull amazon/aws-cli`.\n\nContainer uses two volumes:\n\n- `$HOME/.aws` -> `/root/.aws` - credentials and config store\n- `$(cwd)` -> `/aws` - Docker image workdir\n\n### Extra commands\n\n`awscliv2` contains a few commands to make your life easier, especially in CI or any non-TTY environment.\n\n- `awsv2 -U/--update/--install` - Install `AWS CLI v2`\n- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>] [<region>]` - set profile in `~/.aws/credentials`\n- `awsv2 --assume-role <profile_name> <source_profile> <role_arn>` - create a new profile with assume role credentials\n- `awsv2 -V/--version` - Output `awscliv2` and `AWS CLI v2` versions\n\n### As a Python module\n\nBasic usage\n\n```python\nfrom awscliv2.api import AWSAPI\nfrom awscliv2.exceptions import AWSCLIError\n\naws_api = AWSAPI()\n\ntry:\n    output = aws_api.execute(["s3", "ls"])\nexcept AWSCLIError as e:\n    print(f"Something went wrong: {e}")\nelse:\n    print(output)\n```\n\nInstall binaries for your OS from Python\n\n```python\nfrom awscliv2.installers import install_multiplatform\n\ninstall_multiplatform()\n```\n\nYou can also set credentials or assume roles\n\n```python\nfrom awscliv2.api import AWSAPI\n\naws_api = AWSAPI()\n\naws_api.set_credentials("profile_name", "access_key", "secret_key", "", "region")\naws_api.assume_role("name", "source_profile", "role_arn")\n```\n\n## Development\n\n- Install [poetry](https://python-poetry.org/)\n- Run `poetry install`\n- Use `black` formatter in your IDE\n\n## How to help\n\n- Ping AWS team to release an official PyPI package\n- Share your experience in issues\n\n## Versioning\n\n`awscliv2` version follows [PEP 440](https://www.python.org/dev/peps/pep-0440/).\n\n## Latest changes\n\nFull changelog can be found in [Releases](https://github.com/youtype/awscliv2/releases).\n',
     'author': 'Vlad Emelianov',
     'author_email': 'vlad.emelianov.nz@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://youtype.github.io/awscliv2/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `awscliv2-2.1.2/PKG-INFO` & `awscliv2-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awscliv2
-Version: 2.1.2
+Version: 2.2.0
 Summary: Wrapper for AWS CLI v2
 Home-page: https://youtype.github.io/awscliv2/
 License: MIT
 Keywords: awscli,awscliv2,wrapper
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -29,28 +29,35 @@
 Requires-Dist: pip
 Project-URL: Bug Tracker, https://github.com/youtype/awscliv2/issues
 Project-URL: Documentation, https://awscliv2.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/youtype/awscliv2
 Project-URL: Source, https://github.com/youtype/awscliv2
 Description-Content-Type: text/markdown
 
-# AWS CLI v2 for Python 
+# AWS CLI v2 for Python
 
 [![PyPI - awscliv2](https://img.shields.io/pypi/v/awscliv2.svg?color=blue&label=awscliv2)](https://pypi.org/project/awscliv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/awscliv2.svg?color=blue)](https://pypi.org/project/awscliv2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/awscliv2?color=blue)](https://pypistats.org/packages/awscliv2)
 
 Wrapper for [AWS CLI v2](https://awscli.amazonaws.com/v2/documentation/api/latest/index.html).
-Comes with zero dependencies, updates `awscli`, gives access to all services!
+
+- No dependency hell, like with original [awscli](https://pypi.org/project/awscli/)
+- Can install and update `awscliv2` binaries
+- Provides access to all services
+- Has Python interface
 
 - [AWS CLI v2 for Python](#aws-cli-v2-for-python)
   - [Before you start](#before-you-start)
   - [Installation](#installation)
   - [Usage](#usage)
+    - [From command line](#from-command-line)
     - [Docker fallback](#docker-fallback)
     - [Extra commands](#extra-commands)
+    - [As a Python module](#as-a-python-module)
   - [Development](#development)
   - [How to help](#how-to-help)
   - [Versioning](#versioning)
   - [Latest changes](#latest-changes)
 
 ## Before you start
 
@@ -70,14 +77,16 @@
 
 ```bash
 alias aws='awsv2'
 ```
 
 ## Usage
 
+### From command line
+
 Install `AWS CLI v2`:
 
 ```bash
 # do not worry if this fails, you can still use awsv2 if you have docker installed
 awsv2 --install
 ```
 
@@ -117,32 +126,67 @@
 - `$(cwd)` -> `/aws` - Docker image workdir
 
 ### Extra commands
 
 `awscliv2` contains a few commands to make your life easier, especially in CI or any non-TTY environment.
 
 - `awsv2 -U/--update/--install` - Install `AWS CLI v2`
-- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>]` - set profile in `~/.aws/credentials`
+- `awsv2 --configure <profile_name> <aws_access_key_id> <aws_secret_access_key> [<aws_session_token>] [<region>]` - set profile in `~/.aws/credentials`
 - `awsv2 --assume-role <profile_name> <source_profile> <role_arn>` - create a new profile with assume role credentials
 - `awsv2 -V/--version` - Output `awscliv2` and `AWS CLI v2` versions
 
+### As a Python module
+
+Basic usage
+
+```python
+from awscliv2.api import AWSAPI
+from awscliv2.exceptions import AWSCLIError
+
+aws_api = AWSAPI()
+
+try:
+    output = aws_api.execute(["s3", "ls"])
+except AWSCLIError as e:
+    print(f"Something went wrong: {e}")
+else:
+    print(output)
+```
+
+Install binaries for your OS from Python
+
+```python
+from awscliv2.installers import install_multiplatform
+
+install_multiplatform()
+```
+
+You can also set credentials or assume roles
+
+```python
+from awscliv2.api import AWSAPI
+
+aws_api = AWSAPI()
+
+aws_api.set_credentials("profile_name", "access_key", "secret_key", "", "region")
+aws_api.assume_role("name", "source_profile", "role_arn")
+```
+
 ## Development
 
 - Install [poetry](https://python-poetry.org/)
 - Run `poetry install`
 - Use `black` formatter in your IDE
 
 ## How to help
 
 - Ping AWS team to release an official PyPI package
-- Help me to test MacOS installer and add Windows installer
 - Share your experience in issues
 
 ## Versioning
 
 `awscliv2` version follows [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ## Latest changes
 
-Full changelog can be found in [Changelog](./CHANGELOG.md).
-Release notes can be found in [Releases](https://github.com/youtype/awscliv2/releases).
+Full changelog can be found in [Releases](https://github.com/youtype/awscliv2/releases).
```

