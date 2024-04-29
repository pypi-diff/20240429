# Comparing `tmp/typon-0.0.1.tar.gz` & `tmp/typon-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typon-0.0.1.tar", last modified: Mon Apr 22 15:10:58 2024, max compression
+gzip compressed data, was "typon-0.3.tar", last modified: Mon Apr 29 12:07:51 2024, max compression
```

## Comparing `typon-0.0.1.tar` & `typon-0.3.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.480599 typon-0.0.1/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       70 2024-04-22 15:05:49.000000 typon-0.0.1/MANIFEST.in
--rw-r--r--   0 xavier    (1000) xavier    (1000)      378 2024-04-22 15:10:58.480599 typon-0.0.1/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1337 2024-04-22 15:05:49.000000 typon-0.0.1/README.md
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.456599 typon-0.0.1/docs/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.460599 typon-0.0.1/docs/source/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1926 2024-04-22 15:05:49.000000 typon-0.0.1/docs/source/conf.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      519 2024-04-22 15:05:49.000000 typon-0.0.1/pyproject.toml
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-22 15:10:58.480599 typon-0.0.1/setup.cfg
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.460599 typon-0.0.1/typon/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:05:49.000000 typon-0.0.1/typon/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.460599 typon-0.0.1/typon/include/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       61 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/.clang-format
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       57 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/.clang-tidy
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.464599 typon-0.0.1/typon/include/python/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1437 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/basedef.hpp
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.464599 typon-0.0.1/typon/include/python/builtins/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      976 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/bool.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1579 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/bytes.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      573 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/complex.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6337 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/dict.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      384 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/exception.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4745 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/int.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5487 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/list.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1899 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/mutex.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2679 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/print.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1028 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/range.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1851 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/set.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2550 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/slice.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8968 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins/str.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    13063 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/builtins.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      308 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/dataclasses.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2700 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/hashlib.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      251 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/io.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      468 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/json.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4105 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/os.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    31468 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/referencemodel.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7513 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/socket.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      539 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/stat.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      693 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/sys.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      602 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/time.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      399 2024-04-22 15:05:49.000000 typon-0.0.1/typon/include/python/typon.hpp
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.464599 typon-0.0.1/typon/runtime/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       64 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/.clang-format
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       57 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/.clang-tidy
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       35 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/.git
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        5 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/.gitignore
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8451 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/README.md
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.460599 typon-0.0.1/typon/runtime/rt/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.468599 typon-0.0.1/typon/runtime/rt/examples/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       30 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/.gitignore
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      851 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/Makefile
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      134 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/Makefile.clang++-14
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      786 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/Makefile.g++-11
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      609 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/await_ready.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1229 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/await_result.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      951 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/cat.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      732 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/fork.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2208 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/fork_exceptions.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      797 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/fork_variations.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      679 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/future_awaited.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      577 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/future_detached.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      348 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/loop.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      714 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/mutex.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      644 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_accelerated_fork.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      230 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_baseline.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      403 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_fork.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      589 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_fork_into.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      624 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_fork_void.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      406 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_future.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      423 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_indirection.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      292 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_sequential.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      838 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/promise.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      383 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/shuffle_baseline.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      839 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/shuffle_fork.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      434 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/sleep.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      535 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/sum_baseline.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1063 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/sum_fork.cpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3624 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/examples/webserver.cpp
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.460599 typon-0.0.1/typon/runtime/rt/include/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.472599 typon-0.0.1/typon/runtime/rt/include/typon/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      309 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/defer.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1287 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/event_count.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4070 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/fork.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      553 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/fork_refcount.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4966 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/forked.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4833 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/future.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3147 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/garbage_collector.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3724 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/generator.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4065 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/io.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3647 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/join.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      260 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/logger.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1553 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/meta.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2202 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/mutex.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1018 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/pool.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4489 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/promise.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      303 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/random.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2984 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/result.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      523 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/ring.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1947 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/ring_buffer.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1437 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/root.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8866 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/scheduler.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2827 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/span.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4991 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/stack.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      324 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/syscall_completion.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3181 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/task.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      254 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/theft_point.hpp
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1846 2024-04-22 15:05:50.000000 typon-0.0.1/typon/runtime/rt/include/typon/typon.hpp
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.472599 typon-0.0.1/typon/trans/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       90 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/__main__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2642 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/main.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.472599 typon-0.0.1/typon/trans/stdlib/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5178 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/builtins_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       55 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/dataclasses_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       45 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/enum_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      214 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/hashlib_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       41 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/io_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       64 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/json_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/os_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      931 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/socket_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      449 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/stat_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       78 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/sys_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       41 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/time_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      160 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/typing_.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.472599 typon-0.0.1/typon/trans/stdlib/typon/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       81 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/stdlib/typon/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5424 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/test_runner.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/tests/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      204 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/a_a_call_py_1.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      598 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/actor_inc.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1284 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/actors.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1180 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/builtins_test.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      291 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/forward_decl.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      414 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/gen_func.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1020 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/inheritance.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      705 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/mutex_inc.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      141 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/out_of_order.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      168 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/pyext.post.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      683 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/pyext.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      504 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/usertype.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1440 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/webserver.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1291 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/tests/webserver_eval.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       17 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1772 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/consts.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6501 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/error_display.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      150 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/exceptions.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      332 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/format.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/desugar_compare/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1306 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/desugar_compare/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/desugar_op/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1625 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/desugar_op/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/desugar_subscript/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1339 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/desugar_subscript/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/desugar_with/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1401 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/desugar_with/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3879 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/class_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    17502 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/expr.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    15063 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/function.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6453 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/module.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4957 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/visitors.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4654 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     8113 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/block.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4960 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/class_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1693 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/consts.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    13252 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/expr.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2227 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/file.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4693 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/function.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     9126 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/module.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      656 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/search.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.476599 typon-0.0.1/typon/trans/transpiler/phases/if_main/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      654 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/if_main/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.480599 typon-0.0.1/typon/trans/transpiler/phases/typing/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1040 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2714 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/annotations.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    13619 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/block.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1694 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/class_.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5600 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/common.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11163 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/exceptions.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    15935 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/expr.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     5365 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/modules.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2993 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/scope.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    16611 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/stdlib.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    22542 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/typing/types.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1574 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/phases/utils.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3762 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/transpiler.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4092 2024-04-22 15:05:49.000000 typon-0.0.1/typon/trans/transpiler/utils.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-22 15:10:58.480599 typon-0.0.1/typon.egg-info/
--rw-r--r--   0 xavier    (1000) xavier    (1000)      378 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6633 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/SOURCES.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        1 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/dependency_links.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       48 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/entry_points.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      164 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/requires.txt
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       16 2024-04-22 15:10:58.000000 typon-0.0.1/typon.egg-info/top_level.txt
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.410182 typon-0.3/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       70 2024-04-23 16:10:17.000000 typon-0.3/MANIFEST.in
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2163 2024-04-29 12:07:51.410182 typon-0.3/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1451 2024-04-26 15:41:14.000000 typon-0.3/README.md
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/docs/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/docs/source/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1926 2024-04-23 16:10:17.000000 typon-0.3/docs/source/conf.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      880 2024-04-29 12:07:41.000000 typon-0.3/pyproject.toml
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-04-29 12:07:51.410182 typon-0.3/setup.cfg
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 16:10:17.000000 typon-0.3/typon/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/include/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       61 2024-04-23 16:10:17.000000 typon-0.3/typon/include/.clang-format
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       57 2024-04-23 16:10:17.000000 typon-0.3/typon/include/.clang-tidy
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/include/python/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1437 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/basedef.hpp
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/include/python/builtins/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      976 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/bool.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1579 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/bytes.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      573 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/complex.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6337 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/dict.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      384 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/exception.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4745 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/int.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5487 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/list.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1899 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/mutex.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2679 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/print.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1028 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/range.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1851 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/set.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2550 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/slice.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8968 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins/str.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    13063 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/builtins.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      308 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/dataclasses.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2700 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/hashlib.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      251 2024-04-23 16:10:17.000000 typon-0.3/typon/include/python/io.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      468 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/json.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4105 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/os.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    31468 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/referencemodel.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7513 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/socket.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      539 2024-04-23 16:10:17.000000 typon-0.3/typon/include/python/stat.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      693 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/sys.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      602 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/time.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      399 2024-04-26 14:36:38.000000 typon-0.3/typon/include/python/typon.hpp
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.402182 typon-0.3/typon/runtime/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       64 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/.clang-format
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       57 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/.clang-tidy
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       35 2024-04-23 16:10:17.000000 typon-0.3/typon/runtime/.git
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        5 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/.gitignore
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8451 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/README.md
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/runtime/rt/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.402182 typon-0.3/typon/runtime/rt/examples/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       30 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/.gitignore
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      851 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/Makefile
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      134 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/Makefile.clang++-14
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      786 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/Makefile.g++-11
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      609 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/examples/await_ready.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1229 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/examples/await_result.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      951 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/cat.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      732 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/examples/fork.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2208 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/fork_exceptions.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      797 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/fork_variations.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      679 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/future_awaited.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      577 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/future_detached.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      348 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/loop.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      714 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/examples/mutex.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      644 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_accelerated_fork.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      230 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_baseline.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      403 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_fork.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      589 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_fork_into.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      624 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_fork_void.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      406 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_future.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      423 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_indirection.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      292 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/naive_fibonacci_sequential.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      838 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/promise.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      383 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/shuffle_baseline.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      839 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/shuffle_fork.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      434 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/sleep.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      535 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/sum_baseline.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1063 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/sum_fork.cpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3624 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/examples/webserver.cpp
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.398182 typon-0.3/typon/runtime/rt/include/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.402182 typon-0.3/typon/runtime/rt/include/typon/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      309 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/defer.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1287 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/event_count.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4070 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/fork.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      553 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/fork_refcount.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4966 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/forked.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4833 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/future.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3147 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/garbage_collector.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3724 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/generator.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4065 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/io.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3647 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/join.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      260 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/logger.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1553 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/meta.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2202 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/mutex.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1018 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/pool.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4489 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/promise.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      303 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/random.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2984 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/result.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      523 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/ring.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1947 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/ring_buffer.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1437 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/root.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8866 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/scheduler.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2827 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/span.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4991 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/stack.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      324 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/syscall_completion.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3181 2024-04-26 14:37:04.000000 typon-0.3/typon/runtime/rt/include/typon/task.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      254 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/theft_point.hpp
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1846 2024-04-23 16:10:18.000000 typon-0.3/typon/runtime/rt/include/typon/typon.hpp
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       90 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/__main__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2642 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/main.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/stdlib/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5178 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/builtins_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       55 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/dataclasses_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       45 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/enum_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      214 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/hashlib_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       41 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/io_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       64 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/json_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/os_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      931 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/socket_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      449 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/stat_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       78 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/stdlib/sys_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       41 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/time_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      160 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/typing_.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/stdlib/typon/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       81 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/stdlib/typon/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5424 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/test_runner.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/tests/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      204 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/tests/a_a_call_py_1.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      598 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/actor_inc.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1284 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/actors.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1180 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/builtins_test.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      291 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/tests/forward_decl.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      414 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/gen_func.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1020 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/inheritance.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      705 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/mutex_inc.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      141 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/out_of_order.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      168 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/pyext.post.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      683 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/pyext.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      504 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/usertype.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1440 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/webserver.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1291 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/tests/webserver_eval.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       17 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1772 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/consts.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6501 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/error_display.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      150 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/exceptions.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      332 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/format.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/phases/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/desugar_compare/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1306 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/desugar_compare/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/desugar_op/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1625 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/desugar_op/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/desugar_subscript/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1339 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/desugar_subscript/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/desugar_with/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1401 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/phases/desugar_with/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/emit_cpp/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3879 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/class_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    17502 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/expr.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    15063 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/function.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6453 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/module.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4957 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp/visitors.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4654 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     8113 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/block.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4960 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/class_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1693 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/consts.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    13252 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/expr.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2227 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/file.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4693 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/function.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     9126 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/module.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      656 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/emit_cpp2/search.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.406182 typon-0.3/typon/trans/transpiler/phases/if_main/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      654 2024-04-23 16:10:17.000000 typon-0.3/typon/trans/transpiler/phases/if_main/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.410182 typon-0.3/typon/trans/transpiler/phases/typing/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1040 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2714 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/annotations.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    13619 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/block.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1694 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/class_.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5600 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/common.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11163 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/exceptions.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    15935 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/expr.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     5365 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/modules.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2993 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/scope.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    16611 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/stdlib.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    22542 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/typing/types.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1574 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/phases/utils.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3762 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/transpiler.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4092 2024-04-26 14:36:38.000000 typon-0.3/typon/trans/transpiler/utils.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-04-29 12:07:51.410182 typon-0.3/typon.egg-info/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2163 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6633 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/SOURCES.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        1 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/dependency_links.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       48 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/entry_points.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      164 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/requires.txt
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       16 2024-04-29 12:07:51.000000 typon-0.3/typon.egg-info/top_level.txt
```

### Comparing `typon-0.0.1/README.md` & `typon-0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 # Typon compiler
 
 Typon is a two-part project to bring practical GIL-free concurrency to Python:
 1. [`typon-concurrency`](https://lab.nexedi.com/typon/typon-concurrency), a C++ concurrency runtime
 2. typon-compiler (this repository), a compiler from Python syntax into C++
 
-## Directory structure
-
-### `docs`, documentation
-
-Currently using Sphinx.
-
-### `include`, standard library and compiler primitives/intrisics
-
-TODO.
-
-### `runtime`, concurrency runtime (Git submodule)
-
-See the [runtime repository](https://lab.nexedi.com/typon/typon-concurrency).
+## Getting started
 
-### `trans`, transpiler 
+### Install
 
-This repository, TODO.
-
-## Getting started
+#### From code
 
 ```bash
 git clone https://lab.nexedi.com/typon/typon-compiler.git --recursive
 python3 -m venv typenv
 source typenv/bin/activate
 pip install ./typon-compiler
-apt install libfmt-dev liburing-dev python3.12-dev libssl-dev
+```
+
+#### From PyPI
+
+```
+pip install typon
+```
+
+### Install dependencies
+
+```
+apt install g++-13 libfmt-dev liburing-dev python3.12-dev libssl-dev
 ```
 
 ## Basic usage
 
 Typon can be used from the command-line to compile a Python file:
 
 ```
 typon [-o/--output output] [-d/--debug] [-v/--verbose] input
 ```
 
 Once generated, the C++ code file can be compiled using your compiler of choice:
 
 ```
-$(CXX) -O3 input.cpp $(typon --cpp-flags) 
+$(CXX) -O3 $(typon --cpp-flags) input.cpp
 ```
 
 Currently, you'll get the best support with G++ 13.
 
+## Directory structure
+
+### `docs`, documentation
+
+Currently using Sphinx.
+
+### `include`, standard library and compiler primitives/intrinsics
+
+TODO.
+
+### `runtime`, concurrency runtime (Git submodule)
+
+See the [runtime repository](https://lab.nexedi.com/typon/typon-concurrency).
+
+### `trans`, transpiler
+
+This repository, TODO.
+
 ## Test harness
 
 `cd` into the `trans` directory, set up your `.env` file (you can copy the `.env.example` file), and run `python3 test_runner.py`.
+
```

### Comparing `typon-0.0.1/docs/source/conf.py` & `typon-0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/basedef.hpp` & `typon-0.3/typon/include/python/basedef.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/bool.hpp` & `typon-0.3/typon/include/python/builtins/bool.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/bytes.hpp` & `typon-0.3/typon/include/python/builtins/bytes.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/complex.hpp` & `typon-0.3/typon/include/python/builtins/complex.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/dict.hpp` & `typon-0.3/typon/include/python/builtins/dict.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/int.hpp` & `typon-0.3/typon/include/python/builtins/int.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/list.hpp` & `typon-0.3/typon/include/python/builtins/list.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/mutex.hpp` & `typon-0.3/typon/include/python/builtins/mutex.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/print.hpp` & `typon-0.3/typon/include/python/builtins/print.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/range.hpp` & `typon-0.3/typon/include/python/builtins/range.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/set.hpp` & `typon-0.3/typon/include/python/builtins/set.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/slice.hpp` & `typon-0.3/typon/include/python/builtins/slice.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins/str.hpp` & `typon-0.3/typon/include/python/builtins/str.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/builtins.hpp` & `typon-0.3/typon/include/python/builtins.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/hashlib.hpp` & `typon-0.3/typon/include/python/hashlib.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/os.hpp` & `typon-0.3/typon/include/python/os.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/referencemodel.hpp` & `typon-0.3/typon/include/python/referencemodel.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/socket.hpp` & `typon-0.3/typon/include/python/socket.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/stat.hpp` & `typon-0.3/typon/include/python/stat.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/sys.hpp` & `typon-0.3/typon/include/python/sys.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/include/python/time.hpp` & `typon-0.3/typon/include/python/time.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/README.md` & `typon-0.3/typon/runtime/README.md`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/Makefile` & `typon-0.3/typon/runtime/rt/examples/Makefile`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/Makefile.g++-11` & `typon-0.3/typon/runtime/rt/examples/Makefile.g++-11`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/await_ready.cpp` & `typon-0.3/typon/runtime/rt/examples/await_ready.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/await_result.cpp` & `typon-0.3/typon/runtime/rt/examples/await_result.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/cat.cpp` & `typon-0.3/typon/runtime/rt/examples/cat.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/fork.cpp` & `typon-0.3/typon/runtime/rt/examples/fork.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/fork_exceptions.cpp` & `typon-0.3/typon/runtime/rt/examples/fork_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/fork_variations.cpp` & `typon-0.3/typon/runtime/rt/examples/fork_variations.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/future_awaited.cpp` & `typon-0.3/typon/runtime/rt/examples/future_awaited.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/future_detached.cpp` & `typon-0.3/typon/runtime/rt/examples/future_detached.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/mutex.cpp` & `typon-0.3/typon/runtime/rt/examples/mutex.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_accelerated_fork.cpp` & `typon-0.3/typon/runtime/rt/examples/naive_fibonacci_accelerated_fork.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_fork_into.cpp` & `typon-0.3/typon/runtime/rt/examples/naive_fibonacci_fork_into.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/naive_fibonacci_fork_void.cpp` & `typon-0.3/typon/runtime/rt/examples/naive_fibonacci_fork_void.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/promise.cpp` & `typon-0.3/typon/runtime/rt/examples/promise.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/shuffle_fork.cpp` & `typon-0.3/typon/runtime/rt/examples/shuffle_fork.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/sum_baseline.cpp` & `typon-0.3/typon/runtime/rt/examples/sum_baseline.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/sum_fork.cpp` & `typon-0.3/typon/runtime/rt/examples/sum_fork.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/examples/webserver.cpp` & `typon-0.3/typon/runtime/rt/examples/webserver.cpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/event_count.hpp` & `typon-0.3/typon/runtime/rt/include/typon/event_count.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/fork.hpp` & `typon-0.3/typon/runtime/rt/include/typon/fork.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/fork_refcount.hpp` & `typon-0.3/typon/runtime/rt/include/typon/fork_refcount.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/forked.hpp` & `typon-0.3/typon/runtime/rt/include/typon/forked.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/future.hpp` & `typon-0.3/typon/runtime/rt/include/typon/future.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/garbage_collector.hpp` & `typon-0.3/typon/runtime/rt/include/typon/garbage_collector.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/generator.hpp` & `typon-0.3/typon/runtime/rt/include/typon/generator.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/io.hpp` & `typon-0.3/typon/runtime/rt/include/typon/io.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/join.hpp` & `typon-0.3/typon/runtime/rt/include/typon/join.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/meta.hpp` & `typon-0.3/typon/runtime/rt/include/typon/meta.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/mutex.hpp` & `typon-0.3/typon/runtime/rt/include/typon/mutex.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/pool.hpp` & `typon-0.3/typon/runtime/rt/include/typon/pool.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/promise.hpp` & `typon-0.3/typon/runtime/rt/include/typon/promise.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/result.hpp` & `typon-0.3/typon/runtime/rt/include/typon/result.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/ring.hpp` & `typon-0.3/typon/runtime/rt/include/typon/ring.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/ring_buffer.hpp` & `typon-0.3/typon/runtime/rt/include/typon/ring_buffer.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/root.hpp` & `typon-0.3/typon/runtime/rt/include/typon/root.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/scheduler.hpp` & `typon-0.3/typon/runtime/rt/include/typon/scheduler.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/span.hpp` & `typon-0.3/typon/runtime/rt/include/typon/span.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/stack.hpp` & `typon-0.3/typon/runtime/rt/include/typon/stack.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/task.hpp` & `typon-0.3/typon/runtime/rt/include/typon/task.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/runtime/rt/include/typon/typon.hpp` & `typon-0.3/typon/runtime/rt/include/typon/typon.hpp`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/main.py` & `typon-0.3/typon/trans/main.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/stdlib/builtins_.py` & `typon-0.3/typon/trans/stdlib/builtins_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/stdlib/os_.py` & `typon-0.3/typon/trans/stdlib/os_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/stdlib/socket_.py` & `typon-0.3/typon/trans/stdlib/socket_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/test_runner.py` & `typon-0.3/typon/trans/test_runner.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/actor_inc.py` & `typon-0.3/typon/trans/tests/actor_inc.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/actors.py` & `typon-0.3/typon/trans/tests/actors.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/builtins_test.py` & `typon-0.3/typon/trans/tests/builtins_test.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/inheritance.py` & `typon-0.3/typon/trans/tests/inheritance.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/mutex_inc.py` & `typon-0.3/typon/trans/tests/mutex_inc.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/pyext.py` & `typon-0.3/typon/trans/tests/pyext.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/webserver.py` & `typon-0.3/typon/trans/tests/webserver.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/tests/webserver_eval.py` & `typon-0.3/typon/trans/tests/webserver_eval.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/consts.py` & `typon-0.3/typon/trans/transpiler/consts.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/error_display.py` & `typon-0.3/typon/trans/transpiler/error_display.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/desugar_compare/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/desugar_compare/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/desugar_op/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/desugar_op/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/desugar_subscript/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/desugar_subscript/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/desugar_with/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/desugar_with/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/class_.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp/class_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/expr.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp/expr.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/function.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp/function.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/module.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp/module.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp/visitors.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp/visitors.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/block.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/block.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/class_.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/class_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/consts.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/consts.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/expr.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/expr.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/file.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/file.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/function.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/function.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/module.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/module.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/emit_cpp2/search.py` & `typon-0.3/typon/trans/transpiler/phases/emit_cpp2/search.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/if_main/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/if_main/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/__init__.py` & `typon-0.3/typon/trans/transpiler/phases/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/annotations.py` & `typon-0.3/typon/trans/transpiler/phases/typing/annotations.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/block.py` & `typon-0.3/typon/trans/transpiler/phases/typing/block.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/class_.py` & `typon-0.3/typon/trans/transpiler/phases/typing/class_.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/common.py` & `typon-0.3/typon/trans/transpiler/phases/typing/common.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/exceptions.py` & `typon-0.3/typon/trans/transpiler/phases/typing/exceptions.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/expr.py` & `typon-0.3/typon/trans/transpiler/phases/typing/expr.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/modules.py` & `typon-0.3/typon/trans/transpiler/phases/typing/modules.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/scope.py` & `typon-0.3/typon/trans/transpiler/phases/typing/scope.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/stdlib.py` & `typon-0.3/typon/trans/transpiler/phases/typing/stdlib.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/typing/types.py` & `typon-0.3/typon/trans/transpiler/phases/typing/types.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/phases/utils.py` & `typon-0.3/typon/trans/transpiler/phases/utils.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/transpiler.py` & `typon-0.3/typon/trans/transpiler/transpiler.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon/trans/transpiler/utils.py` & `typon-0.3/typon/trans/transpiler/utils.py`

 * *Files identical despite different names*

### Comparing `typon-0.0.1/typon.egg-info/SOURCES.txt` & `typon-0.3/typon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

