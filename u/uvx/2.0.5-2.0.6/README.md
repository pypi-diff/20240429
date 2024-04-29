# Comparing `tmp/uvx-2.0.5.tar.gz` & `tmp/uvx-2.0.6.tar.gz`

## Comparing `uvx-2.0.5.tar` & `uvx-2.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 uvx-2.0.5/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.5/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.5/.gitignore
--rw-rw-r--   0     1000     1000      717 2024-04-26 21:14:32.000000 uvx-2.0.5/CHANGELOG.md
--rw-rw-r--   0     1000     1000    92159 2024-04-26 21:14:04.000000 uvx-2.0.5/Cargo.lock
--rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.5/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.5/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.5/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.5/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.5/src/cli.rs
--rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.5/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.5/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.5/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.5/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5187 2024-04-26 21:07:25.000000 uvx-2.0.5/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.5/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.5/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.5/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.5/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.5/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.5/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.5/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.5/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.5/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.5/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.5/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.5/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.5/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.5/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.5/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.5/src/main.rs
--rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.5/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.5/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.5/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.5/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.5/src/venv.rs
--rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 uvx-2.0.6/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.6/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.6/.gitignore
+-rw-rw-r--   0     1000     1000      814 2024-04-29 13:43:30.000000 uvx-2.0.6/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    92159 2024-04-29 13:42:51.000000 uvx-2.0.6/Cargo.lock
+-rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.6/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.6/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.6/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.6/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.6/src/cli.rs
+-rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.6/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.6/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2262 2024-04-29 13:40:19.000000 uvx-2.0.6/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.6/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5100 2024-04-29 13:41:31.000000 uvx-2.0.6/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.6/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.6/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.6/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.6/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.6/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.6/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.6/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.6/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.6/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.6/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.6/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.6/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.6/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.6/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.6/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.6/src/main.rs
+-rw-rw-r--   0     1000     1000     8649 2024-04-29 13:41:09.000000 uvx-2.0.6/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.6/src/pip.rs
+-rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.0.6/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.6/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.6/src/venv.rs
+-rw-rw-r--   0     1000     1000      835 2024-04-29 13:42:40.000000 uvx-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.6/PKG-INFO
```

### Comparing `uvx-2.0.5/Cargo.toml` & `uvx-2.0.6/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.5"
+version = "2.0.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.5/.gitignore` & `uvx-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/CHANGELOG.md` & `uvx-2.0.6/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.6 (2024-04-26)
+
+### Fix
+
+* ensure `~/.local/bin` exists before trying to write symlinks
+
 ## v2.0.5 (2024-04-26)
 
 ### Updates
 
 * **cargo**: bump dependencies
 
 ## v2.0.4 (2024-04-26)
```

### Comparing `uvx-2.0.5/Cargo.lock` & `uvx-2.0.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3321,15 +3321,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.5"
+version = "2.0.6"
 dependencies = [
  "anstyle",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
```

### Comparing `uvx-2.0.5/README.md` & `uvx-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/animate.rs` & `uvx-2.0.6/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/cli.rs` & `uvx-2.0.6/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/cmd.rs` & `uvx-2.0.6/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/completions.rs` & `uvx-2.0.6/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/ensurepath.rs` & `uvx-2.0.6/src/commands/ensurepath.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use chrono::Local;
 use owo_colors::OwoColorize;
 use tokio::{fs::OpenOptions, io::AsyncWriteExt};
 
 use crate::{
     cli::{EnsurepathOptions, Process},
     helpers::ResultToString,
-    metadata::{get_bin_dir, get_home_dir},
+    metadata::{ensure_bin_dir, get_home_dir},
 };
 
 pub fn now() -> String {
     let dt = Local::now();
 
     match dt.to_string().split_once('.') {
         None => String::new(),
@@ -56,15 +56,15 @@
     final_text.push_str(text);
     final_text.push('\n');
 
     append(&path, final_text).await
 }
 
 pub async fn ensure_path(force: bool) -> Result<(), String> {
-    let bin_path = get_bin_dir();
+    let bin_path = ensure_bin_dir().await;
     let bin_dir = bin_path.to_str().unwrap_or_default();
 
     let path = std::env::var("PATH").unwrap_or_default();
 
     let parts: Vec<&str> = path.split(':').collect();
 
     if parts.contains(&bin_dir) && !force {
```

### Comparing `uvx-2.0.5/src/commands/inject.rs` & `uvx-2.0.6/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/install.rs` & `uvx-2.0.6/src/commands/install.rs`

 * *Files 5% similar despite different names*

```diff
@@ -114,21 +114,18 @@
 
     let symlinks = find_symlinks(requirement, &meta.installed_version, venv).await;
 
     let mut results = HashMap::new();
     for symlink in symlinks {
         let result = create_symlink(&symlink, venv_root, force, binaries).await;
 
-        let success = match result {
-            Ok(_success) => _success,
-            Err(msg) => {
-                eprintln!("⚠️ {}", format!("{}", msg,).yellow());
-                false
-            },
-        };
+        let success = result.unwrap_or_else(|msg| {
+            eprintln!("⚠️ {}", msg.yellow());
+            false
+        });
 
         results.insert(symlink.clone(), success);
     }
 
     meta.scripts = results;
     meta.save(venv_root).await?;
```

### Comparing `uvx-2.0.5/src/commands/list.rs` & `uvx-2.0.6/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/reinstall.rs` & `uvx-2.0.6/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/reinstall_all.rs` & `uvx-2.0.6/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/run.rs` & `uvx-2.0.6/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/runpip.rs` & `uvx-2.0.6/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/runpython.rs` & `uvx-2.0.6/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/runuv.rs` & `uvx-2.0.6/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/self_update.rs` & `uvx-2.0.6/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/uninject.rs` & `uvx-2.0.6/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/uninstall.rs` & `uvx-2.0.6/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/uninstall_all.rs` & `uvx-2.0.6/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/upgrade.rs` & `uvx-2.0.6/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/commands/upgrade_all.rs` & `uvx-2.0.6/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/helpers.rs` & `uvx-2.0.6/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/main.rs` & `uvx-2.0.6/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/metadata.rs` & `uvx-2.0.6/src/metadata.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use crate::uv::{uv_get_installed_version, uv_venv, Helpers};
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use pep508_rs::Requirement;
 use serde::{Deserialize, Serialize};
 use std::collections::{HashMap, HashSet};
 use std::path::{Path, PathBuf};
-use tokio::fs::File;
+use tokio::fs::{create_dir_all, File};
 use tokio::io::AsyncReadExt;
 use tokio::io::AsyncWriteExt;
 use uv_interpreter::PythonEnvironment;
 
 const BIN_DIR: &str = ".local/bin";
 const WORK_DIR: &str = ".local/uvx";
 const INDENT: &str = "    ";
@@ -25,14 +25,24 @@
 }
 
 pub fn get_bin_dir() -> PathBuf {
     let home_dir = get_home_dir();
     home_dir.join(BIN_DIR)
 }
 
+pub async fn ensure_bin_dir() -> PathBuf {
+    let bin_dir = get_bin_dir();
+
+    if !bin_dir.exists() {
+        let _ = create_dir_all(&bin_dir).await;
+    }
+
+    bin_dir
+}
+
 pub fn get_work_dir() -> PathBuf {
     let home_dir = get_home_dir();
     home_dir.join(WORK_DIR)
 }
 
 pub fn get_venv_dir() -> PathBuf {
     let work_dir = get_work_dir();
```

### Comparing `uvx-2.0.5/src/pip.rs` & `uvx-2.0.6/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/symlinks.rs` & `uvx-2.0.6/src/symlinks.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::path::Path;
 
 use pep508_rs::Requirement;
 use uv_interpreter::PythonEnvironment;
 
-use crate::metadata::get_bin_dir;
+use crate::metadata::ensure_bin_dir;
 use configparser::ini::Ini;
 
 pub async fn console_scripts(entry_points_path: &str) -> Result<Vec<String>, String> {
     let Ok(ini) = tokio::fs::read_to_string(entry_points_path).await else {
         return Ok(Vec::new()); // file missing = empty list
     };
 
@@ -52,15 +52,15 @@
 
 pub async fn create_symlink(
     symlink: &str,
     venv: &Path,
     force: bool,
     binaries: &[&str],
 ) -> Result<bool, String> {
-    let bin_dir = get_bin_dir();
+    let bin_dir = ensure_bin_dir().await;
 
     if !binaries.is_empty() && !binaries.contains(&symlink) {
         return Ok(false);
     }
 
     let target_path = bin_dir.join(symlink);
 
@@ -108,21 +108,21 @@
         .map_or(false, |link| link.starts_with(target_path))
 }
 
 pub async fn check_symlink(
     symlink: &str,
     target_path: &Path,
 ) -> bool {
-    let symlink_path = get_bin_dir().join(symlink);
+    let symlink_path = ensure_bin_dir().await.join(symlink);
 
     is_symlink(&symlink_path) && points_to(&symlink_path, target_path)
 }
 
 pub async fn remove_symlink(symlink: &str) -> Result<(), String> {
-    let bin_dir = get_bin_dir();
+    let bin_dir = ensure_bin_dir().await;
     let target_path = bin_dir.join(symlink);
 
     if is_symlink(&target_path) {
         tokio::fs::remove_file(&target_path)
             .await
             .map_err(|_| format!("Failed to remove symlink {:?}", &target_path))?;
     };
```

### Comparing `uvx-2.0.5/src/uv.rs` & `uvx-2.0.6/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/src/venv.rs` & `uvx-2.0.6/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.5/pyproject.toml` & `uvx-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,7 +28,8 @@
     "pip", # self-update
     "patchelf", # idk, but required
 ]
 
 
 [tool.maturin]
 bindings = "bin"
+stripped = true
```

### Comparing `uvx-2.0.5/PKG-INFO` & `uvx-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.5
+Version: 2.0.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

