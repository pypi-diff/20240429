# Comparing `tmp/corgea_cli-1.2.4.tar.gz` & `tmp/corgea_cli-1.3.0.tar.gz`

## Comparing `corgea_cli-1.2.4.tar` & `corgea_cli-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.2.4/Cargo.toml
--rw-r--r--   0     1001      127     3285 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/.github/workflows/release.yml
--rw-r--r--   0     1001      127       39 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/.gitignore
--rwxr-xr-x   0     1001      127     3282 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/.legacy/cli.sh
--rw-r--r--   0     1001      127    37633 2024-04-23 01:16:45.000000 corgea_cli-1.2.4/Cargo.lock
--rw-r--r--   0     1001      127      490 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/README.md
--rw-r--r--   0     1001      127      575 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/_redirects
--rwxr-xr-x   0     1001      127      844 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/build_release.sh
--rw-r--r--   0     1001      127      698 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/src/cicd.rs
--rw-r--r--   0     1001      127     2102 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/src/config.rs
--rw-r--r--   0     1001      127      627 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/src/login.rs
--rw-r--r--   0     1001      127     3213 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/src/main.rs
--rw-r--r--   0     1001      127    10894 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/src/scan.rs
--rw-r--r--   0     1001      127     1109 2024-04-23 01:16:41.000000 corgea_cli-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 corgea_cli-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.3.0/Cargo.toml
+-rw-r--r--   0     1001      127     3285 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127       39 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/.gitignore
+-rw-r--r--   0     1001      127    37633 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/Cargo.lock
+-rw-r--r--   0     1001      127    26530 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/LICENSE
+-rw-r--r--   0     1001      127      490 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/README.md
+-rwxr-xr-x   0     1001      127      844 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/build_release.sh
+-rw-r--r--   0     1001      127      698 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/cicd.rs
+-rw-r--r--   0     1001      127     2102 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/config.rs
+-rw-r--r--   0     1001      127      627 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/login.rs
+-rw-r--r--   0     1001      127     3213 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/main.rs
+-rw-r--r--   0     1001      127    12146 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/scan.rs
+-rw-r--r--   0     1001      127     1109 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 corgea_cli-1.3.0/PKG-INFO
```

### Comparing `corgea_cli-1.2.4/Cargo.toml` & `corgea_cli-1.3.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "corgea"
-version = "1.2.4"
+version = "1.3.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 clap = {  version = "4.4.13", features = ["derive"] }
 dirs = "5.0.1"
```

### Comparing `corgea_cli-1.2.4/.github/workflows/release.yml` & `corgea_cli-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/Cargo.lock` & `corgea_cli-1.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "corgea"
-version = "1.2.4"
+version = "1.3.0"
 dependencies = [
  "clap",
  "dirs",
  "reqwest",
  "serde",
  "serde_derive",
  "serde_json",
```

### Comparing `corgea_cli-1.2.4/build_release.sh` & `corgea_cli-1.3.0/build_release.sh`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/src/cicd.rs` & `corgea_cli-1.3.0/src/cicd.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/src/config.rs` & `corgea_cli-1.3.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/src/login.rs` & `corgea_cli-1.3.0/src/login.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/src/main.rs` & `corgea_cli-1.3.0/src/main.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/src/scan.rs` & `corgea_cli-1.3.0/src/scan.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::collections::HashSet;
 use serde_json::Value;
 use std::io::{self, Read};
 use crate::Config;
 use reqwest::header;
 use uuid::Uuid;
 use std::path::Path;
 use std::process::Command;
@@ -131,14 +132,32 @@
                                         }
                                     }
                                 }
                             }
                         }
                     }
                 }
+                // checkmarx
+            } else if input.contains("Cx") && data.get("results").is_some() && data.get("scanID").is_some() {
+                scanner = "checkmarx".to_string();
+                if let Some(results) = data.get("results").and_then(|v| v.as_array()) {
+                    for result in results {
+                        if let Some(data) = result.get("data") {
+                            if let Some(nodes) = data.get("nodes").and_then(|v| v.as_array()) {
+                                for node in nodes {
+                                    if let Some(path) = node.get("fileName") {
+                                        if let Some(truncated_path) = path.as_str() {
+                                            paths.push(truncated_path.get(1..).unwrap_or("").to_string());
+                                        }
+                                    }
+                                }
+                            }
+                        }
+                    }
+                }
             }
         }
         Err(e) => {
             eprintln!("Failed to parse JSON report: {}", e);
             eprintln!("Only reports in JSON format are supported.");
             std::process::exit(1);
         }
@@ -177,20 +196,26 @@
     let git_config_upload_url = format!(
         "{}/api/cli/git-config-upload?token={}&run_id={}", base_url, token, run_id
     );
     let client = reqwest::blocking::Client::new();
 
     println!("Uploading required files for the scan...");
 
+    let mut uploaded_paths = HashSet::new();
+
     for path in &paths {
         if !Path::new(&path).exists() {
             eprintln!("Required file {} not found which is required for the scan, exiting.", path);
             std::process::exit(1);
         }
 
+        if uploaded_paths.contains(path) {
+            continue;
+        }
+
         let src_upload_url = format!(
             "{}/api/cli/code-upload?token={}&run_id={}&path={}", base_url, token, run_id, path
         );
         let fp = Path::new(&path);
 
         let form = reqwest::blocking::multipart::Form::new()
             .file("file", fp)
@@ -202,14 +227,16 @@
             .send();
 
         match res {
             Ok(response) => {
                 if !response.status().is_success() {
                     eprintln!("Failed to upload file: {}", response.status());
                     std::process::exit(1);
+                } else {
+                    uploaded_paths.insert(path.clone());
                 }
             }
             Err(e) => {
                 eprintln!("Failed to send request: {}", e);
                 std::process::exit(1);
             }
         }
```

### Comparing `corgea_cli-1.2.4/pyproject.toml` & `corgea_cli-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.2.4/PKG-INFO` & `corgea_cli-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: corgea-cli
-Version: 1.2.4
+Version: 1.3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
+License-File: LICENSE
 Summary: The Corgea CLI. Scan for vulnerabilties, create fixes.
 Author-email: Adam Bronte <adam@corgea.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://corgea.com
 Project-URL: Documentation, https://docs.corgea.app
 Project-URL: Repository, https://github.com/Corgea/cli
```

