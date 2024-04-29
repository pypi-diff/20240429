# Comparing `tmp/hysteria2-2.3.0.tar.gz` & `tmp/hysteria2-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hysteria2-2.3.0.tar", last modified: Sun Mar 10 13:58:38 2024, max compression
+gzip compressed data, was "hysteria2-2.4.3.tar", last modified: Mon Apr 29 09:33:20 2024, max compression
```

## Comparing `hysteria2-2.3.0.tar` & `hysteria2-2.4.3.tar`

### file list

```diff
@@ -1,338 +1,356 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.041152 hysteria2-2.3.0/
--rw-r--r--   0 runner     (501) staff       (20)     1170 2024-03-10 13:58:30.000000 hysteria2-2.3.0/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1069 2024-03-10 13:58:30.000000 hysteria2-2.3.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      195 2024-03-10 13:58:30.000000 hysteria2-2.3.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5476 2024-03-10 13:58:38.040804 hysteria2-2.3.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3772 2024-03-10 13:58:30.000000 hysteria2-2.3.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.930235 hysteria2-2.3.0/gobuild/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-03-10 13:58:30.000000 hysteria2-2.3.0/gobuild/.gitkeep
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.930544 hysteria2-2.3.0/hysteria2/
--rw-r--r--   0 runner     (501) staff       (20)       60 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.934039 hysteria2-2.3.0/hysteria2-go/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.934757 hysteria2-2.3.0/hysteria2-go/.github/
--rw-r--r--   0 runner     (501) staff       (20)       57 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/FUNDING.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.936119 hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner     (501) staff       (20)      536 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner     (501) staff       (20)      511 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.zh.md
--rw-r--r--   0 runner     (501) staff       (20)      605 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner     (501) staff       (20)      597 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md
--rw-r--r--   0 runner     (501) staff       (20)      204 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.937504 hysteria2-2.3.0/hysteria2-go/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1171 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/workflows/docker.yml
--rw-r--r--   0 runner     (501) staff       (20)     1188 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/workflows/master.yml
--rw-r--r--   0 runner     (501) staff       (20)     1947 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      668 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.github/workflows/scripts.yml
--rw-r--r--   0 runner     (501) staff       (20)     9265 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)       57 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/CHANGELOG.md
--rw-r--r--   0 runner     (501) staff       (20)     1257 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/Dockerfile
--rw-r--r--   0 runner     (501) staff       (20)     1052 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)     8029 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/PROTOCOL.md
--rw-r--r--   0 runner     (501) staff       (20)     2219 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.939134 hysteria2-2.3.0/hysteria2-go/app/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.943103 hysteria2-2.3.0/hysteria2-go/app/cmd/
--rw-r--r--   0 runner     (501) staff       (20)    27471 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/client.go
--rw-r--r--   0 runner     (501) staff       (20)     3775 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/client_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1022 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/client_test.yaml
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/errors.go
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/ping.go
--rw-r--r--   0 runner     (501) staff       (20)     4779 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/root.go
--rw-r--r--   0 runner     (501) staff       (20)    29322 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/server.go
--rw-r--r--   0 runner     (501) staff       (20)     3860 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2091 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/server_test.yaml
--rw-r--r--   0 runner     (501) staff       (20)     4506 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/speedtest.go
--rw-r--r--   0 runner     (501) staff       (20)     2292 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/update.go
--rw-r--r--   0 runner     (501) staff       (20)      359 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/cmd/version.go
--rw-r--r--   0 runner     (501) staff       (20)     2752 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/go.mod
--rw-r--r--   0 runner     (501) staff       (20)    58835 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.923033 hysteria2-2.3.0/hysteria2-go/app/internal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.944615 hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/
--rw-r--r--   0 runner     (501) staff       (20)     1047 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/tcp.go
--rw-r--r--   0 runner     (501) staff       (20)      743 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/tcp_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3633 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/udp.go
--rw-r--r--   0 runner     (501) staff       (20)      749 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.946077 hysteria2-2.3.0/hysteria2-go/app/internal/http/
--rw-r--r--   0 runner     (501) staff       (20)     7744 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/http/server.go
--rw-r--r--   0 runner     (501) staff       (20)     1316 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/http/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)      582 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/http/server_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1363 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/http/test.crt
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/http/test.key
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.947879 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/
--rw-r--r--   0 runner     (501) staff       (20)      328 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/getsockopt_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      551 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/syscall_socketcall_linux_386.s
--rw-r--r--   0 runner     (501) staff       (20)     2734 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/tcp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      424 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/redirect/tcp_others.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.948957 hysteria2-2.3.0/hysteria2-go/app/internal/socks5/
--rw-r--r--   0 runner     (501) staff       (20)     7613 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server.go
--rw-r--r--   0 runner     (501) staff       (20)      578 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1423 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server_test.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.950344 hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/
--rw-r--r--   0 runner     (501) staff       (20)     1408 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/tcp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      418 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/tcp_others.go
--rw-r--r--   0 runner     (501) staff       (20)     3082 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/udp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      453 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/udp_others.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.951285 hysteria2-2.3.0/hysteria2-go/app/internal/url/
--rw-r--r--   0 runner     (501) staff       (20)    35764 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/url/url.go
--rw-r--r--   0 runner     (501) staff       (20)     1760 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/url/url_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.952941 hysteria2-2.3.0/hysteria2-go/app/internal/utils/
--rw-r--r--   0 runner     (501) staff       (20)     1549 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils/bpsconv.go
--rw-r--r--   0 runner     (501) staff       (20)     1088 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils/bpsconv_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3887 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils/geoloader.go
--rw-r--r--   0 runner     (501) staff       (20)      267 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils/qr.go
--rw-r--r--   0 runner     (501) staff       (20)     2519 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils/update.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.953282 hysteria2-2.3.0/hysteria2-go/app/internal/utils_test/
--rw-r--r--   0 runner     (501) staff       (20)     1823 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/internal/utils_test/mock.go
--rw-r--r--   0 runner     (501) staff       (20)      225 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/main.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.953653 hysteria2-2.3.0/hysteria2-go/app/misc/
--rw-r--r--   0 runner     (501) staff       (20)     1405 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/misc/socks5_test.py
--rw-r--r--   0 runner     (501) staff       (20)      310 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/app/pprof.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.954331 hysteria2-2.3.0/hysteria2-go/core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.956720 hysteria2-2.3.0/hysteria2-go/core/client/
--rw-r--r--   0 runner     (501) staff       (20)      171 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     8123 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/client.go
--rw-r--r--   0 runner     (501) staff       (20)     4190 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/config.go
--rw-r--r--   0 runner     (501) staff       (20)     3613 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/mock_udpIO.go
--rw-r--r--   0 runner     (501) staff       (20)     3135 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/reconnect.go
--rw-r--r--   0 runner     (501) staff       (20)     3402 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/udp.go
--rw-r--r--   0 runner     (501) staff       (20)     2934 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/client/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.957075 hysteria2-2.3.0/hysteria2-go/core/errors/
--rw-r--r--   0 runner     (501) staff       (20)     1590 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/errors/errors.go
--rw-r--r--   0 runner     (501) staff       (20)     1202 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/go.mod
--rw-r--r--   0 runner     (501) staff       (20)     6814 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.924979 hysteria2-2.3.0/hysteria2-go/core/internal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.957419 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.959946 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/
--rw-r--r--   0 runner     (501) staff       (20)      602 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bandwidth.go
--rw-r--r--   0 runner     (501) staff       (20)    31585 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go
--rw-r--r--   0 runner     (501) staff       (20)    32614 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go
--rw-r--r--   0 runner     (501) staff       (20)      327 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/clock.go
--rw-r--r--   0 runner     (501) staff       (20)     5684 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go
--rw-r--r--   0 runner     (501) staff       (20)     3225 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go
--rw-r--r--   0 runner     (501) staff       (20)     5609 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.960217 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/brutal/
--rw-r--r--   0 runner     (501) staff       (20)     5356 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/brutal/brutal.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.960573 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/common/
--rw-r--r--   0 runner     (501) staff       (20)     2296 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/common/pacer.go
--rw-r--r--   0 runner     (501) staff       (20)      449 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/congestion/utils.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.961308 hysteria2-2.3.0/hysteria2-go/core/internal/frag/
--rw-r--r--   0 runner     (501) staff       (20)     1952 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/frag/frag.go
--rw-r--r--   0 runner     (501) staff       (20)     5867 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/frag/frag_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.964475 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/
--rw-r--r--   0 runner     (501) staff       (20)      543 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     8008 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/close_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2583 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/masq_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.966237 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/
--rw-r--r--   0 runner     (501) staff       (20)     2675 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go
--rw-r--r--   0 runner     (501) staff       (20)     9787 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go
--rw-r--r--   0 runner     (501) staff       (20)     8645 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     3662 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     2168 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     4692 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)     7704 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/smoke_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6021 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/stress_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1363 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/test.crt
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/test.key
--rw-r--r--   0 runner     (501) staff       (20)     5163 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1611 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/utils_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.966801 hysteria2-2.3.0/hysteria2-go/core/internal/pmtud/
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/pmtud/avail.go
--rw-r--r--   0 runner     (501) staff       (20)      480 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/pmtud/unavail.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.967933 hysteria2-2.3.0/hysteria2-go/core/internal/protocol/
--rw-r--r--   0 runner     (501) staff       (20)     1826 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/protocol/http.go
--rw-r--r--   0 runner     (501) staff       (20)      637 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/protocol/padding.go
--rw-r--r--   0 runner     (501) staff       (20)     6130 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/protocol/proxy.go
--rw-r--r--   0 runner     (501) staff       (20)    11136 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/protocol/proxy_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.968477 hysteria2-2.3.0/hysteria2-go/core/internal/utils/
--rw-r--r--   0 runner     (501) staff       (20)      316 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/utils/atomic.go
--rw-r--r--   0 runner     (501) staff       (20)     1517 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/internal/utils/qstream.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.971245 hysteria2-2.3.0/hysteria2-go/core/server/
--rw-r--r--   0 runner     (501) staff       (20)      311 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/.mockery.yaml
--rw-r--r--   0 runner     (501) staff       (20)     7566 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/config.go
--rw-r--r--   0 runner     (501) staff       (20)     1512 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/copy.go
--rw-r--r--   0 runner     (501) staff       (20)     4693 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)     3130 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/mock_udpEventLogger.go
--rw-r--r--   0 runner     (501) staff       (20)     4943 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/mock_udpIO.go
--rw-r--r--   0 runner     (501) staff       (20)     9078 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/server.go
--rw-r--r--   0 runner     (501) staff       (20)     5871 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/udp.go
--rw-r--r--   0 runner     (501) staff       (20)     5208 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/core/server/udp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.971975 hysteria2-2.3.0/hysteria2-go/extras/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.974621 hysteria2-2.3.0/hysteria2-go/extras/auth/
--rw-r--r--   0 runner     (501) staff       (20)      621 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/command.go
--rw-r--r--   0 runner     (501) staff       (20)     1756 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/http.go
--rw-r--r--   0 runner     (501) staff       (20)      760 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)      547 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/http_test.py
--rw-r--r--   0 runner     (501) staff       (20)      477 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/password.go
--rw-r--r--   0 runner     (501) staff       (20)     1106 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/password_test.go
--rw-r--r--   0 runner     (501) staff       (20)      847 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/userpass.go
--rw-r--r--   0 runner     (501) staff       (20)     1729 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/auth/userpass_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.975028 hysteria2-2.3.0/hysteria2-go/extras/correctnet/
--rw-r--r--   0 runner     (501) staff       (20)     2064 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/correctnet/correctnet.go
--rw-r--r--   0 runner     (501) staff       (20)     1436 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/go.mod
--rw-r--r--   0 runner     (501) staff       (20)    10839 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.975412 hysteria2-2.3.0/hysteria2-go/extras/masq/
--rw-r--r--   0 runner     (501) staff       (20)     2865 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/masq/server.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.976462 hysteria2-2.3.0/hysteria2-go/extras/obfs/
--rw-r--r--   0 runner     (501) staff       (20)     2915 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/obfs/conn.go
--rw-r--r--   0 runner     (501) staff       (20)     1527 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/obfs/salamander.go
--rw-r--r--   0 runner     (501) staff       (20)     1048 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/obfs/salamander_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.983004 hysteria2-2.3.0/hysteria2-go/extras/outbounds/
--rw-r--r--   0 runner     (501) staff       (20)      263 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/.mockery.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.985441 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/
--rw-r--r--   0 runner     (501) staff       (20)     7162 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/compile.go
--rw-r--r--   0 runner     (501) staff       (20)     5953 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/compile_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1468 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers.go
--rw-r--r--   0 runner     (501) staff       (20)     6123 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4808 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go
--rw-r--r--   0 runner     (501) staff       (20)     2489 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1716 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/parse.go
--rw-r--r--   0 runner     (501) staff       (20)     1611 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/parse_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.003662 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/
--rw-r--r--   0 runner     (501) staff       (20)  9640091 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat
--rw-r--r--   0 runner     (501) staff       (20)  4143750 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat
--rw-r--r--   0 runner     (501) staff       (20)     1080 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/load.go
--rw-r--r--   0 runner     (501) staff       (20)     1348 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go
--rw-r--r--   0 runner     (501) staff       (20)    21809 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1561 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto
--rw-r--r--   0 runner     (501) staff       (20)     3266 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl.go
--rw-r--r--   0 runner     (501) staff       (20)     1675 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1956 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_https.go
--rw-r--r--   0 runner     (501) staff       (20)     5508 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_standard.go
--rw-r--r--   0 runner     (501) staff       (20)     1053 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_system.go
--rw-r--r--   0 runner     (501) staff       (20)     3913 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/interface.go
--rw-r--r--   0 runner     (501) staff       (20)     1225 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/interface_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3906 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go
--rw-r--r--   0 runner     (501) staff       (20)     4741 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/mock_UDPConn.go
--rw-r--r--   0 runner     (501) staff       (20)    11736 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct.go
--rw-r--r--   0 runner     (501) staff       (20)     1287 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      628 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct_others.go
--rw-r--r--   0 runner     (501) staff       (20)     4596 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_http.go
--rw-r--r--   0 runner     (501) staff       (20)     6928 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_socks5.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.005599 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/
--rw-r--r--   0 runner     (501) staff       (20)     3031 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/client.go
--rw-r--r--   0 runner     (501) staff       (20)     3381 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/protocol.go
--rw-r--r--   0 runner     (501) staff       (20)     9544 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/protocol_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2163 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/server.go
--rw-r--r--   0 runner     (501) staff       (20)      796 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest.go
--rw-r--r--   0 runner     (501) staff       (20)      963 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/utils.go
--rw-r--r--   0 runner     (501) staff       (20)     1603 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/outbounds/utils_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.005996 hysteria2-2.3.0/hysteria2-go/extras/trafficlogger/
--rw-r--r--   0 runner     (501) staff       (20)     3228 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/trafficlogger/http.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.926766 hysteria2-2.3.0/hysteria2-go/extras/transport/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.007104 hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/
--rw-r--r--   0 runner     (501) staff       (20)     1960 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/addr.go
--rw-r--r--   0 runner     (501) staff       (20)     2488 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/addr_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6861 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/conn.go
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/go.work
--rw-r--r--   0 runner     (501) staff       (20)    32526 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/go.work.sum
--rw-r--r--   0 runner     (501) staff       (20)    14484 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/hyperbole.py
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/logo.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.927322 hysteria2-2.3.0/hysteria2-go/media-kit/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.013521 hysteria2-2.3.0/hysteria2-go/media-kit/png/
--rw-r--r--   0 runner     (501) staff       (20)    18296 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/black 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38595 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/black 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    19475 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/black 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    40667 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/black 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    17502 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    37286 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18565 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38855 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18334 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38791 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    19526 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    40734 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12744 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12395 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12672 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    12013 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 4@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    17426 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/white 1@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    37014 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/white 2@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    18330 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/white 3@2x.png
--rw-r--r--   0 runner     (501) staff       (20)    38461 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/png/white 4@2x.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.019804 hysteria2-2.3.0/hysteria2-go/media-kit/svg/
--rw-r--r--   0 runner     (501) staff       (20)     2126 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    14333 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2427 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    14626 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2347 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    15086 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2662 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    15393 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2189 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    14396 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    14689 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 4.svg
--rw-r--r--   0 runner     (501) staff       (20)      714 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 1.svg
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 2.svg
--rw-r--r--   0 runner     (501) staff       (20)      651 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 3.svg
--rw-r--r--   0 runner     (501) staff       (20)      767 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 4.svg
--rw-r--r--   0 runner     (501) staff       (20)     2326 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 1.svg
--rw-r--r--   0 runner     (501) staff       (20)    15065 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 2.svg
--rw-r--r--   0 runner     (501) staff       (20)     2641 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 3.svg
--rw-r--r--   0 runner     (501) staff       (20)    15372 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 4.svg
--rw-r--r--   0 runner     (501) staff       (20)      488 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/platforms.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.020561 hysteria2-2.3.0/hysteria2-go/scripts/
--rw-r--r--   0 runner     (501) staff       (20)       25 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/scripts/_redirects
--rw-r--r--   0 runner     (501) staff       (20)    24873 2024-03-10 13:58:30.000000 hysteria2-2.3.0/hysteria2-go/scripts/install_server.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.022062 hysteria2-2.3.0/hysteria2.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5476 2024-03-10 13:58:37.000000 hysteria2-2.3.0/hysteria2.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    11355 2024-03-10 13:58:37.000000 hysteria2-2.3.0/hysteria2.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-10 13:58:37.000000 hysteria2-2.3.0/hysteria2.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-10 13:58:37.000000 hysteria2-2.3.0/hysteria2.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-03-10 13:58:37.000000 hysteria2-2.3.0/hysteria2.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.023023 hysteria2-2.3.0/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    11911 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)        7 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/VERSION
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:37.927984 hysteria2-2.3.0/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.030529 hysteria2-2.3.0/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23979 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65638 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.033283 hysteria2-2.3.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28251 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    50369 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17981 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    25057 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    42266 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1625 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    32147 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    11792 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4695 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     8262 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8862 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    79524 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9103 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125761 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    93848 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.033641 hysteria2-2.3.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    15337 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.039892 hysteria2-2.3.0/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2350 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3105 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)    11103 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)      817 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner     (501) staff       (20)     1423 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner     (501) staff       (20)      952 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1040 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner     (501) staff       (20)     1031 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/libsize.py
--rw-r--r--   0 runner     (501) staff       (20)     1282 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner     (501) staff       (20)    13487 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     6930 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     8955 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     8359 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner     (501) staff       (20)       94 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1965 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner     (501) staff       (20)     1139 2024-03-10 13:58:30.000000 hysteria2-2.3.0/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-03-10 13:58:38.041235 hysteria2-2.3.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2742 2024-03-10 13:58:30.000000 hysteria2-2.3.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-10 13:58:38.040331 hysteria2-2.3.0/src/
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-03-10 13:58:30.000000 hysteria2-2.3.0/src/hysteria2.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.919344 hysteria2-2.4.3/
+-rw-r--r--   0 runner     (501) staff       (20)     1170 2024-04-29 09:32:26.000000 hysteria2-2.4.3/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2024-04-29 09:32:26.000000 hysteria2-2.4.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      195 2024-04-29 09:32:26.000000 hysteria2-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5476 2024-04-29 09:33:20.918952 hysteria2-2.4.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3772 2024-04-29 09:32:26.000000 hysteria2-2.4.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.715710 hysteria2-2.4.3/gobuild/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-29 09:32:26.000000 hysteria2-2.4.3/gobuild/.gitkeep
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.716029 hysteria2-2.4.3/hysteria2/
+-rw-r--r--   0 runner     (501) staff       (20)       60 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.722065 hysteria2-2.4.3/hysteria2-go/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.723227 hysteria2-2.4.3/hysteria2-go/.github/
+-rw-r--r--   0 runner     (501) staff       (20)       57 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/FUNDING.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.725498 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner     (501) staff       (20)      536 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner     (501) staff       (20)      511 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.zh.md
+-rw-r--r--   0 runner     (501) staff       (20)      605 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner     (501) staff       (20)      597 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.727756 hysteria2-2.4.3/hysteria2-go/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1171 2024-04-29 09:32:26.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/docker.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1188 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/master.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1947 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      668 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.github/workflows/scripts.yml
+-rw-r--r--   0 runner     (501) staff       (20)     9265 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)       57 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/CHANGELOG.md
+-rw-r--r--   0 runner     (501) staff       (20)     1257 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/Dockerfile
+-rw-r--r--   0 runner     (501) staff       (20)     1052 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)     8028 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/PROTOCOL.md
+-rw-r--r--   0 runner     (501) staff       (20)     2288 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.730018 hysteria2-2.4.3/hysteria2-go/app/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.737213 hysteria2-2.4.3/hysteria2-go/app/cmd/
+-rw-r--r--   0 runner     (501) staff       (20)    32611 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     4790 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1386 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/client_test.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/errors.go
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/ping.go
+-rw-r--r--   0 runner     (501) staff       (20)     4779 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/root.go
+-rw-r--r--   0 runner     (501) staff       (20)    29942 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     3860 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2091 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     4506 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/speedtest.go
+-rw-r--r--   0 runner     (501) staff       (20)     2292 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/update.go
+-rw-r--r--   0 runner     (501) staff       (20)      359 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/cmd/version.go
+-rw-r--r--   0 runner     (501) staff       (20)     3167 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)    60261 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.702829 hysteria2-2.4.3/hysteria2-go/app/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.739497 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/
+-rw-r--r--   0 runner     (501) staff       (20)     1047 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp.go
+-rw-r--r--   0 runner     (501) staff       (20)      743 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)      749 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.742143 hysteria2-2.4.3/hysteria2-go/app/internal/http/
+-rw-r--r--   0 runner     (501) staff       (20)     7744 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     1316 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      582 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/test.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/http/test.key
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.745287 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/.mockery.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.700842 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.746295 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/
+-rw-r--r--   0 runner     (501) staff       (20)    10390 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     4297 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go
+-rw-r--r--   0 runner     (501) staff       (20)     1343 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager.go
+-rw-r--r--   0 runner     (501) staff       (20)     1789 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/manager_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5951 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux.go
+-rw-r--r--   0 runner     (501) staff       (20)     3044 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/proxymux/mux_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.749131 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/
+-rw-r--r--   0 runner     (501) staff       (20)      328 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      551 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/syscall_socketcall_linux_386.s
+-rw-r--r--   0 runner     (501) staff       (20)     2734 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      424 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_others.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.751450 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/
+-rw-r--r--   0 runner     (501) staff       (20)     1981 2024-04-29 09:32:27.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1900 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts.go
+-rw-r--r--   0 runner     (501) staff       (20)     2300 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/sockopts/sockopts_linux_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.753401 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/
+-rw-r--r--   0 runner     (501) staff       (20)     7613 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      578 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1423 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.755880 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      418 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_others.go
+-rw-r--r--   0 runner     (501) staff       (20)     3082 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      453 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_others.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.756954 hysteria2-2.4.3/hysteria2-go/app/internal/tun/
+-rw-r--r--   0 runner     (501) staff       (20)     1450 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tun/log.go
+-rw-r--r--   0 runner     (501) staff       (20)     5114 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/tun/server.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.758160 hysteria2-2.4.3/hysteria2-go/app/internal/url/
+-rw-r--r--   0 runner     (501) staff       (20)    35764 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/url/url.go
+-rw-r--r--   0 runner     (501) staff       (20)     1760 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/url/url_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.760832 hysteria2-2.4.3/hysteria2-go/app/internal/utils/
+-rw-r--r--   0 runner     (501) staff       (20)     1549 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv.go
+-rw-r--r--   0 runner     (501) staff       (20)     1088 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3887 2024-04-29 09:32:28.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/geoloader.go
+-rw-r--r--   0 runner     (501) staff       (20)      267 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/qr.go
+-rw-r--r--   0 runner     (501) staff       (20)     2519 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils/update.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.761353 hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/
+-rw-r--r--   0 runner     (501) staff       (20)     1823 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/mock.go
+-rw-r--r--   0 runner     (501) staff       (20)      225 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/main.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.761974 hysteria2-2.4.3/hysteria2-go/app/misc/
+-rw-r--r--   0 runner     (501) staff       (20)     1405 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/misc/socks5_test.py
+-rw-r--r--   0 runner     (501) staff       (20)      310 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/app/pprof.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.762907 hysteria2-2.4.3/hysteria2-go/core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.766663 hysteria2-2.4.3/hysteria2-go/core/client/
+-rw-r--r--   0 runner     (501) staff       (20)      171 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     8098 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     4190 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     3613 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/mock_udpIO.go
+-rw-r--r--   0 runner     (501) staff       (20)     3135 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/reconnect.go
+-rw-r--r--   0 runner     (501) staff       (20)     3402 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)     2934 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/client/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.767080 hysteria2-2.4.3/hysteria2-go/core/errors/
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/errors/errors.go
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)     6432 2024-04-29 09:32:29.000000 hysteria2-2.4.3/hysteria2-go/core/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.706366 hysteria2-2.4.3/hysteria2-go/core/internal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.767994 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.772033 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/
+-rw-r--r--   0 runner     (501) staff       (20)      602 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth.go
+-rw-r--r--   0 runner     (501) staff       (20)    31585 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go
+-rw-r--r--   0 runner     (501) staff       (20)    32614 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go
+-rw-r--r--   0 runner     (501) staff       (20)      327 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/clock.go
+-rw-r--r--   0 runner     (501) staff       (20)     5684 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go
+-rw-r--r--   0 runner     (501) staff       (20)     3225 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go
+-rw-r--r--   0 runner     (501) staff       (20)     5609 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.772724 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/
+-rw-r--r--   0 runner     (501) staff       (20)     5432 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/brutal.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.773353 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/
+-rw-r--r--   0 runner     (501) staff       (20)     2267 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/pacer.go
+-rw-r--r--   0 runner     (501) staff       (20)      449 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/congestion/utils.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.774464 hysteria2-2.4.3/hysteria2-go/core/internal/frag/
+-rw-r--r--   0 runner     (501) staff       (20)     1952 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag.go
+-rw-r--r--   0 runner     (501) staff       (20)     5867 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.779698 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/
+-rw-r--r--   0 runner     (501) staff       (20)      543 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     8156 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/close_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2558 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/masq_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.783108 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/
+-rw-r--r--   0 runner     (501) staff       (20)     2675 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go
+-rw-r--r--   0 runner     (501) staff       (20)     9787 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     8645 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     3662 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     2168 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     4692 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)     7704 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/smoke_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6021 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/stress_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.key
+-rw-r--r--   0 runner     (501) staff       (20)     5297 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1611 2024-04-29 09:32:30.000000 hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/utils_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.784264 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/avail.go
+-rw-r--r--   0 runner     (501) staff       (20)      480 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/pmtud/unavail.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.786646 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/
+-rw-r--r--   0 runner     (501) staff       (20)     1826 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/http.go
+-rw-r--r--   0 runner     (501) staff       (20)      637 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/padding.go
+-rw-r--r--   0 runner     (501) staff       (20)     6130 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy.go
+-rw-r--r--   0 runner     (501) staff       (20)    11136 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.787686 hysteria2-2.4.3/hysteria2-go/core/internal/utils/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/utils/atomic.go
+-rw-r--r--   0 runner     (501) staff       (20)     1517 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/internal/utils/qstream.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.792560 hysteria2-2.4.3/hysteria2-go/core/server/
+-rw-r--r--   0 runner     (501) staff       (20)      311 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/.mockery.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     7566 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     1512 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/copy.go
+-rw-r--r--   0 runner     (501) staff       (20)     4693 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)     3130 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_udpEventLogger.go
+-rw-r--r--   0 runner     (501) staff       (20)     4943 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/mock_udpIO.go
+-rw-r--r--   0 runner     (501) staff       (20)     9058 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     5871 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)     5208 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/core/server/udp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.793861 hysteria2-2.4.3/hysteria2-go/extras/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.798274 hysteria2-2.4.3/hysteria2-go/extras/auth/
+-rw-r--r--   0 runner     (501) staff       (20)      621 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/command.go
+-rw-r--r--   0 runner     (501) staff       (20)     1756 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http.go
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      547 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.py
+-rw-r--r--   0 runner     (501) staff       (20)      477 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/password.go
+-rw-r--r--   0 runner     (501) staff       (20)     1106 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/password_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      847 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/userpass.go
+-rw-r--r--   0 runner     (501) staff       (20)     1729 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/auth/userpass_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.798852 hysteria2-2.4.3/hysteria2-go/extras/correctnet/
+-rw-r--r--   0 runner     (501) staff       (20)     2064 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/correctnet/correctnet.go
+-rw-r--r--   0 runner     (501) staff       (20)     1436 2024-04-29 09:32:31.000000 hysteria2-2.4.3/hysteria2-go/extras/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)    10610 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.799347 hysteria2-2.4.3/hysteria2-go/extras/masq/
+-rw-r--r--   0 runner     (501) staff       (20)     2865 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/masq/server.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.801087 hysteria2-2.4.3/hysteria2-go/extras/obfs/
+-rw-r--r--   0 runner     (501) staff       (20)     2915 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander.go
+-rw-r--r--   0 runner     (501) staff       (20)     1048 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.811187 hysteria2-2.4.3/hysteria2-go/extras/outbounds/
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/.mockery.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.815500 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/
+-rw-r--r--   0 runner     (501) staff       (20)     7738 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile.go
+-rw-r--r--   0 runner     (501) staff       (20)     6601 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1468 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers.go
+-rw-r--r--   0 runner     (501) staff       (20)     6123 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4808 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go
+-rw-r--r--   0 runner     (501) staff       (20)     2489 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1716 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse.go
+-rw-r--r--   0 runner     (501) staff       (20)     1611 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.858627 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/
+-rw-r--r--   0 runner     (501) staff       (20)  9640091 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat
+-rw-r--r--   0 runner     (501) staff       (20)  4143750 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load.go
+-rw-r--r--   0 runner     (501) staff       (20)     1348 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    21809 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1561 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto
+-rw-r--r--   0 runner     (501) staff       (20)     3266 2024-04-29 09:32:32.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl.go
+-rw-r--r--   0 runner     (501) staff       (20)     1675 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1956 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_https.go
+-rw-r--r--   0 runner     (501) staff       (20)     5508 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_standard.go
+-rw-r--r--   0 runner     (501) staff       (20)     1053 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_system.go
+-rw-r--r--   0 runner     (501) staff       (20)     3913 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface.go
+-rw-r--r--   0 runner     (501) staff       (20)     1225 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3906 2024-04-29 09:32:33.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     4741 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_UDPConn.go
+-rw-r--r--   0 runner     (501) staff       (20)    11736 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct.go
+-rw-r--r--   0 runner     (501) staff       (20)     1287 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      628 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_others.go
+-rw-r--r--   0 runner     (501) staff       (20)     4596 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_http.go
+-rw-r--r--   0 runner     (501) staff       (20)     6928 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_socks5.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.861763 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/
+-rw-r--r--   0 runner     (501) staff       (20)     3031 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     3381 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol.go
+-rw-r--r--   0 runner     (501) staff       (20)     9544 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2163 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      796 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest.go
+-rw-r--r--   0 runner     (501) staff       (20)      963 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils.go
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.862379 hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/
+-rw-r--r--   0 runner     (501) staff       (20)     3228 2024-04-29 09:32:34.000000 hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/http.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.709363 hysteria2-2.4.3/hysteria2-go/extras/transport/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.863968 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/
+-rw-r--r--   0 runner     (501) staff       (20)     1960 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr.go
+-rw-r--r--   0 runner     (501) staff       (20)     2488 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6863 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/conn.go
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/go.work
+-rw-r--r--   0 runner     (501) staff       (20)    33613 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/go.work.sum
+-rw-r--r--   0 runner     (501) staff       (20)    14484 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/hyperbole.py
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/logo.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.710123 hysteria2-2.4.3/hysteria2-go/media-kit/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.876350 hysteria2-2.4.3/hysteria2-go/media-kit/png/
+-rw-r--r--   0 runner     (501) staff       (20)    18296 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38595 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    19475 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    40667 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/black 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    17502 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    37286 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18565 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38855 2024-04-29 09:32:35.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18334 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38791 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    19526 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    40734 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12744 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12395 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12672 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    12013 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 4@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    17426 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 1@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    37014 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 2@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    18330 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 3@2x.png
+-rw-r--r--   0 runner     (501) staff       (20)    38461 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/png/white 4@2x.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.887123 hysteria2-2.4.3/hysteria2-go/media-kit/svg/
+-rw-r--r--   0 runner     (501) staff       (20)     2126 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14333 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2427 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14626 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2347 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15086 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2662 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15393 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2189 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14396 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    14689 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)      714 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)      651 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)      767 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2326 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 1.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15065 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 2.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2641 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 3.svg
+-rw-r--r--   0 runner     (501) staff       (20)    15372 2024-04-29 09:32:36.000000 hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 4.svg
+-rw-r--r--   0 runner     (501) staff       (20)      488 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/platforms.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.888224 hysteria2-2.4.3/hysteria2-go/scripts/
+-rw-r--r--   0 runner     (501) staff       (20)       25 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/scripts/_redirects
+-rw-r--r--   0 runner     (501) staff       (20)    26403 2024-04-29 09:32:37.000000 hysteria2-2.4.3/hysteria2-go/scripts/install_server.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.891002 hysteria2-2.4.3/hysteria2.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5476 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12021 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-29 09:33:20.000000 hysteria2-2.4.3/hysteria2.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.892831 hysteria2-2.4.3/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    11911 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1684 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)        7 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/VERSION
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.711232 hysteria2-2.4.3/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.904300 hysteria2-2.4.3/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    23979 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     7069 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    65638 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8458 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.908603 hysteria2-2.4.3/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    28251 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    50369 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5491 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    17981 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    25057 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)    42266 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     1625 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    32147 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)    11792 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     4731 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     4695 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     8262 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner     (501) staff       (20)     8862 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    79524 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9103 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   125761 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    93848 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.909111 hysteria2-2.4.3/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner     (501) staff       (20)     4185 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)    15337 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    27013 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.917758 hysteria2-2.4.3/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)     2350 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     3105 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    11103 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      817 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     1423 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner     (501) staff       (20)      952 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     1040 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner     (501) staff       (20)     1031 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/libsize.py
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner     (501) staff       (20)    13487 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     8955 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     8359 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)       94 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1965 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2024-04-29 09:32:37.000000 hysteria2-2.4.3/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-29 09:33:20.919466 hysteria2-2.4.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2742 2024-04-29 09:32:37.000000 hysteria2-2.4.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-29 09:33:20.918328 hysteria2-2.4.3/src/
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-04-29 09:32:37.000000 hysteria2-2.4.3/src/hysteria2.cpp
```

### Comparing `hysteria2-2.3.0/CMakeLists.txt` & `hysteria2-2.4.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/LICENSE` & `hysteria2-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/PKG-INFO` & `hysteria2-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteria2
-Version: 2.3.0
+Version: 2.4.3
 Summary: Python bindings for hysteria2.
 Home-page: https://github.com/LorenEteval/hysteria2-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MIT
 Description: # hysteria2-python
```

### Comparing `hysteria2-2.3.0/README.md` & `hysteria2-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md` & `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md` & `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md` & `hysteria2-2.4.3/hysteria2-go/.github/ISSUE_TEMPLATE/feature_request.zh.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/workflows/docker.yml` & `hysteria2-2.4.3/hysteria2-go/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/workflows/master.yml` & `hysteria2-2.4.3/hysteria2-go/.github/workflows/master.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     steps:
       - name: Check out
         uses: actions/checkout@v4
 
       - name: Setup Go
         uses: actions/setup-go@v5
         with:
-          go-version: "1.21"
+          go-version: "1.22"
 
       - name: Setup Python # This is for the build script
         uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: nttld/setup-ndk@v1
```

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/workflows/release.yml` & `hysteria2-2.4.3/hysteria2-go/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - name: Get version
         id: get_version
         run: echo "version=$(git describe --tags --always --match 'app/v*' | sed -n 's|app/\([^/-]*\)\(-.*\)\{0,1\}|\1|p')" >> $GITHUB_OUTPUT
 
       - name: Setup Go
         uses: actions/setup-go@v5
         with:
-          go-version: "1.21"
+          go-version: "1.22"
 
       - name: Setup Python # This is for the build script
         uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: nttld/setup-ndk@v1
@@ -46,15 +46,15 @@
       - name: Generate hashes
         run: |
           for file in build/*; do
             sha256sum $file >> build/hashes.txt
           done
 
       - name: Upload GitHub
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           files: build/*
 
       - name: Upload CF bucket
         uses: shallwefootball/upload-s3-action@v1.3.3
         with:
           aws_key_id: ${{ secrets.CF_KEY_ID }}
```

### Comparing `hysteria2-2.3.0/hysteria2-go/.github/workflows/scripts.yml` & `hysteria2-2.4.3/hysteria2-go/.github/workflows/scripts.yml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/.gitignore` & `hysteria2-2.4.3/hysteria2-go/.gitignore`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/Dockerfile` & `hysteria2-2.4.3/hysteria2-go/Dockerfile`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/LICENSE.md` & `hysteria2-2.4.3/hysteria2-go/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/PROTOCOL.md` & `hysteria2-2.4.3/hysteria2-go/PROTOCOL.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 After (and only after) a client passes authentication, the server MUST consider this QUIC connection to be a Hysteria proxy connection. It MUST then start processing proxy requests from the client as described in the next section.
 
 ## Proxy Requests
 
 ### TCP
 
-For each TCP connection, the client MUST create a new QUIC unidirectional stream and send the following TCPRequest message:
+For each TCP connection, the client MUST create a new QUIC bidirectional stream and send the following TCPRequest message:
 
 ```
 [varint] 0x401 (TCPRequest ID)
 [varint] Address length
 [bytes] Address string (host:port)
 [varint] Padding length
 [bytes] Random padding
```

### Comparing `hysteria2-2.3.0/hysteria2-go/README.md` & `hysteria2-2.4.3/hysteria2-go/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,41 +19,41 @@
 
 ### [Hysteria 1.x (legacy)](https://v1.hysteria.network/)
 
 ---
 
 <div class="feature-grid">
   <div>
-    <h3>🛠️ Packed to the gills</h3>
-    <p>Expansive range of modes including SOCKS5, HTTP proxy, TCP/UDP forwarding, Linux TProxy - not to mention additional features continually being added.</p>
+    <h3>🛠️ Jack of all trades</h3>
+    <p>Wide range of modes including SOCKS5, HTTP Proxy, TCP/UDP Forwarding, Linux TProxy, TUN - with more features being added constantly.</p>
   </div>
 
   <div>
-    <h3>⚡ Lightning fast</h3>
-    <p>Powered by a custom QUIC protocol, Hysteria delivers unparalleled performance over even the most unreliable and lossy networks.</p>
+    <h3>⚡ Blazing fast</h3>
+    <p>Powered by a customized QUIC protocol, Hysteria is designed to deliver unparalleled performance over unreliable and lossy networks.</p>
   </div>
 
   <div>
     <h3>✊ Censorship resistant</h3>
-    <p>Our protocol is designed to masquerade as standard HTTP/3 traffic, making it very difficult to detect and block without widespread collateral damage.</p>
+    <p>The protocol masquerades as standard HTTP/3 traffic, making it very difficult for censors to detect and block without widespread collateral damage.</p>
   </div>
   
   <div>
     <h3>💻 Cross-platform</h3>
-    <p>We have builds for all major platforms and architectures. Deploy anywhere & use everywhere.</p>
+    <p>We have builds for every major platform and architecture. Deploy anywhere & use everywhere. Not to mention the long list of 3rd party apps.</p>
   </div>
 
   <div>
     <h3>🔗 Easy integration</h3>
     <p>With built-in support for custom authentication, traffic statistics & access control, Hysteria is easy to integrate into your infrastructure.</p>
   </div>
   
   <div>
-    <h3>🤗 Open standards</h3>
-    <p>We have well-documented specifications and code for developers to contribute and build their own apps.</p>
+    <h3>🤗 Chill and supportive</h3>
+    <p>We have well-documented specifications and code for developers to contribute and/or build their own apps. And a helpful community, too.</p>
   </div>
 </div>
 
 ---
 
 **If you find Hysteria useful, consider giving it a ⭐️!**
```

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/client.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/client.go`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 
 import (
 	"bytes"
 	"crypto/sha256"
 	"crypto/x509"
 	"encoding/hex"
 	"errors"
+	"fmt"
 	"net"
+	"net/netip"
 	"os"
+	"runtime"
+	"slices"
 	"strconv"
 	"strings"
 	"time"
 
 	"github.com/spf13/cobra"
 	"github.com/spf13/viper"
 	"go.uber.org/zap"
 
 	"github.com/apernet/hysteria/app/internal/forwarding"
 	"github.com/apernet/hysteria/app/internal/http"
+	"github.com/apernet/hysteria/app/internal/proxymux"
 	"github.com/apernet/hysteria/app/internal/redirect"
+	"github.com/apernet/hysteria/app/internal/sockopts"
 	"github.com/apernet/hysteria/app/internal/socks5"
 	"github.com/apernet/hysteria/app/internal/tproxy"
+	"github.com/apernet/hysteria/app/internal/tun"
 	"github.com/apernet/hysteria/app/internal/url"
 	"github.com/apernet/hysteria/app/internal/utils"
 	"github.com/apernet/hysteria/core/client"
 	"github.com/apernet/hysteria/extras/correctnet"
 	"github.com/apernet/hysteria/extras/obfs"
 	"github.com/apernet/hysteria/extras/transport/udphop"
 )
@@ -62,14 +69,15 @@
 	SOCKS5        *socks5Config         `mapstructure:"socks5"`
 	HTTP          *httpConfig           `mapstructure:"http"`
 	TCPForwarding []tcpForwardingEntry  `mapstructure:"tcpForwarding"`
 	UDPForwarding []udpForwardingEntry  `mapstructure:"udpForwarding"`
 	TCPTProxy     *tcpTProxyConfig      `mapstructure:"tcpTProxy"`
 	UDPTProxy     *udpTProxyConfig      `mapstructure:"udpTProxy"`
 	TCPRedirect   *tcpRedirectConfig    `mapstructure:"tcpRedirect"`
+	TUN           *tunConfig            `mapstructure:"tun"`
 }
 
 type clientConfigTransportUDP struct {
 	HopInterval time.Duration `mapstructure:"hopInterval"`
 }
 
 type clientConfigTransport struct {
@@ -90,21 +98,28 @@
 	SNI       string `mapstructure:"sni"`
 	Insecure  bool   `mapstructure:"insecure"`
 	PinSHA256 string `mapstructure:"pinSHA256"`
 	CA        string `mapstructure:"ca"`
 }
 
 type clientConfigQUIC struct {
-	InitStreamReceiveWindow     uint64        `mapstructure:"initStreamReceiveWindow"`
-	MaxStreamReceiveWindow      uint64        `mapstructure:"maxStreamReceiveWindow"`
-	InitConnectionReceiveWindow uint64        `mapstructure:"initConnReceiveWindow"`
-	MaxConnectionReceiveWindow  uint64        `mapstructure:"maxConnReceiveWindow"`
-	MaxIdleTimeout              time.Duration `mapstructure:"maxIdleTimeout"`
-	KeepAlivePeriod             time.Duration `mapstructure:"keepAlivePeriod"`
-	DisablePathMTUDiscovery     bool          `mapstructure:"disablePathMTUDiscovery"`
+	InitStreamReceiveWindow     uint64                   `mapstructure:"initStreamReceiveWindow"`
+	MaxStreamReceiveWindow      uint64                   `mapstructure:"maxStreamReceiveWindow"`
+	InitConnectionReceiveWindow uint64                   `mapstructure:"initConnReceiveWindow"`
+	MaxConnectionReceiveWindow  uint64                   `mapstructure:"maxConnReceiveWindow"`
+	MaxIdleTimeout              time.Duration            `mapstructure:"maxIdleTimeout"`
+	KeepAlivePeriod             time.Duration            `mapstructure:"keepAlivePeriod"`
+	DisablePathMTUDiscovery     bool                     `mapstructure:"disablePathMTUDiscovery"`
+	Sockopts                    clientConfigQUICSockopts `mapstructure:"sockopts"`
+}
+
+type clientConfigQUICSockopts struct {
+	BindInterface       *string `mapstructure:"bindInterface"`
+	FirewallMark        *uint32 `mapstructure:"fwmark"`
+	FdControlUnixSocket *string `mapstructure:"fdControlUnixSocket"`
 }
 
 type clientConfigBandwidth struct {
 	Up   string `mapstructure:"up"`
 	Down string `mapstructure:"down"`
 }
 
@@ -142,14 +157,31 @@
 	Timeout time.Duration `mapstructure:"timeout"`
 }
 
 type tcpRedirectConfig struct {
 	Listen string `mapstructure:"listen"`
 }
 
+type tunConfig struct {
+	Name    string        `mapstructure:"name"`
+	MTU     uint32        `mapstructure:"mtu"`
+	Timeout time.Duration `mapstructure:"timeout"`
+	Address struct {
+		IPv4 string `mapstructure:"ipv4"`
+		IPv6 string `mapstructure:"ipv6"`
+	} `mapstructure:"address"`
+	Route *struct {
+		Strict      bool     `mapstructure:"strict"`
+		IPv4        []string `mapstructure:"ipv4"`
+		IPv6        []string `mapstructure:"ipv6"`
+		IPv4Exclude []string `mapstructure:"ipv4Exclude"`
+		IPv6Exclude []string `mapstructure:"ipv6Exclude"`
+	} `mapstructure:"route"`
+}
+
 func (c *clientConfig) fillServerAddr(hyConfig *client.Config) error {
 	if c.Server == "" {
 		return configError{Field: "server", Err: errors.New("server address is empty")}
 	}
 	var addr net.Addr
 	var err error
 	host, port, hostPort := parseServerAddrString(c.Server)
@@ -169,26 +201,41 @@
 	}
 	return nil
 }
 
 // fillConnFactory must be called after fillServerAddr, as we have different logic
 // for ConnFactory depending on whether we have a port hopping address.
 func (c *clientConfig) fillConnFactory(hyConfig *client.Config) error {
+	so := &sockopts.SocketOptions{
+		BindInterface:       c.QUIC.Sockopts.BindInterface,
+		FirewallMark:        c.QUIC.Sockopts.FirewallMark,
+		FdControlUnixSocket: c.QUIC.Sockopts.FdControlUnixSocket,
+	}
+	if err := so.CheckSupported(); err != nil {
+		var unsupportedErr *sockopts.UnsupportedError
+		if errors.As(err, &unsupportedErr) {
+			return configError{
+				Field: "quic.sockopts." + unsupportedErr.Field,
+				Err:   errors.New("unsupported on this platform"),
+			}
+		}
+		return configError{Field: "quic.sockopts", Err: err}
+	}
 	// Inner PacketConn
 	var newFunc func(addr net.Addr) (net.PacketConn, error)
 	switch strings.ToLower(c.Transport.Type) {
 	case "", "udp":
 		if hyConfig.ServerAddr.Network() == "udphop" {
 			hopAddr := hyConfig.ServerAddr.(*udphop.UDPHopAddr)
 			newFunc = func(addr net.Addr) (net.PacketConn, error) {
-				return udphop.NewUDPHopPacketConn(hopAddr, c.Transport.UDP.HopInterval, nil)
+				return udphop.NewUDPHopPacketConn(hopAddr, c.Transport.UDP.HopInterval, so.ListenUDP)
 			}
 		} else {
 			newFunc = func(addr net.Addr) (net.PacketConn, error) {
-				return net.ListenUDP("udp", nil)
+				return so.ListenUDP()
 			}
 		}
 	default:
 		return configError{Field: "transport.type", Err: errors.New("unsupported transport type")}
 	}
 	// Obfuscation
 	var ob obfs.Obfuscator
@@ -540,14 +587,19 @@
 		})
 	}
 	if config.TCPRedirect != nil {
 		runner.Add("TCP redirect", func() error {
 			return clientTCPRedirect(*config.TCPRedirect, c)
 		})
 	}
+	if config.TUN != nil {
+		runner.Add("TUN", func() error {
+			return clientTUN(*config.TUN, c)
+		})
+	}
 
 	runner.Run()
 }
 
 type clientModeRunner struct {
 	ModeMap map[string]func() error
 }
@@ -584,15 +636,15 @@
 	}
 }
 
 func clientSOCKS5(config socks5Config, c client.Client) error {
 	if config.Listen == "" {
 		return configError{Field: "listen", Err: errors.New("listen address is empty")}
 	}
-	l, err := correctnet.Listen("tcp", config.Listen)
+	l, err := proxymux.ListenSOCKS(config.Listen)
 	if err != nil {
 		return configError{Field: "listen", Err: err}
 	}
 	var authFunc func(username, password string) bool
 	username, password := config.Username, config.Password
 	if username != "" && password != "" {
 		authFunc = func(u, p string) bool {
@@ -609,15 +661,15 @@
 	return s.Serve(l)
 }
 
 func clientHTTP(config httpConfig, c client.Client) error {
 	if config.Listen == "" {
 		return configError{Field: "listen", Err: errors.New("listen address is empty")}
 	}
-	l, err := correctnet.Listen("tcp", config.Listen)
+	l, err := proxymux.ListenHTTP(config.Listen)
 	if err != nil {
 		return configError{Field: "listen", Err: err}
 	}
 	var authFunc func(username, password string) bool
 	username, password := config.Username, config.Password
 	if username != "" && password != "" {
 		authFunc = func(u, p string) bool {
@@ -737,14 +789,100 @@
 		HyClient:    c,
 		EventLogger: &tcpRedirectLogger{},
 	}
 	logger.Info("TCP redirect listening", zap.String("addr", config.Listen))
 	return p.ListenAndServe(laddr)
 }
 
+func clientTUN(config tunConfig, c client.Client) error {
+	supportedPlatforms := []string{"linux", "darwin", "windows", "android"}
+	if !slices.Contains(supportedPlatforms, runtime.GOOS) {
+		logger.Error("TUN is not supported on this platform", zap.String("platform", runtime.GOOS))
+	}
+	if config.Name == "" {
+		return configError{Field: "name", Err: errors.New("name is empty")}
+	}
+	if config.MTU == 0 {
+		config.MTU = 1500
+	}
+	timeout := int64(config.Timeout.Seconds())
+	if timeout == 0 {
+		timeout = 300
+	}
+	if config.Address.IPv4 == "" {
+		config.Address.IPv4 = "100.100.100.101/30"
+	}
+	prefix4, err := netip.ParsePrefix(config.Address.IPv4)
+	if err != nil {
+		return configError{Field: "address.ipv4", Err: err}
+	}
+	if config.Address.IPv6 == "" {
+		config.Address.IPv6 = "2001::ffff:ffff:ffff:fff1/126"
+	}
+	prefix6, err := netip.ParsePrefix(config.Address.IPv6)
+	if err != nil {
+		return configError{Field: "address.ipv6", Err: err}
+	}
+	server := &tun.Server{
+		HyClient:     c,
+		EventLogger:  &tunLogger{},
+		Logger:       logger,
+		IfName:       config.Name,
+		MTU:          config.MTU,
+		Timeout:      timeout,
+		Inet4Address: []netip.Prefix{prefix4},
+		Inet6Address: []netip.Prefix{prefix6},
+	}
+	if config.Route != nil {
+		server.AutoRoute = true
+		server.StructRoute = config.Route.Strict
+
+		parsePrefixes := func(field string, ss []string) ([]netip.Prefix, error) {
+			var prefixes []netip.Prefix
+			for i, s := range ss {
+				var p netip.Prefix
+				if strings.Contains(s, "/") {
+					var err error
+					p, err = netip.ParsePrefix(s)
+					if err != nil {
+						return nil, configError{Field: fmt.Sprintf("%s[%d]", field, i), Err: err}
+					}
+				} else {
+					pa, err := netip.ParseAddr(s)
+					if err != nil {
+						return nil, configError{Field: fmt.Sprintf("%s[%d]", field, i), Err: err}
+					}
+					p = netip.PrefixFrom(pa, pa.BitLen())
+				}
+				prefixes = append(prefixes, p)
+			}
+			return prefixes, nil
+		}
+
+		server.Inet4RouteAddress, err = parsePrefixes("route.ipv4", config.Route.IPv4)
+		if err != nil {
+			return err
+		}
+		server.Inet6RouteAddress, err = parsePrefixes("route.ipv6", config.Route.IPv6)
+		if err != nil {
+			return err
+		}
+		server.Inet4RouteExcludeAddress, err = parsePrefixes("route.ipv4Exclude", config.Route.IPv4Exclude)
+		if err != nil {
+			return err
+		}
+		server.Inet6RouteExcludeAddress, err = parsePrefixes("route.ipv6Exclude", config.Route.IPv6Exclude)
+		if err != nil {
+			return err
+		}
+	}
+	logger.Info("TUN listening", zap.String("interface", config.Name))
+	return server.Serve()
+}
+
 // parseServerAddrString parses server address string.
 // Server address can be in either "host:port" or "host" format (in which case we assume port 443).
 func parseServerAddrString(addrStr string) (host, port, hostPort string) {
 	h, p, err := net.SplitHostPort(addrStr)
 	if err != nil {
 		return addrStr, "443", net.JoinHostPort(addrStr, "443")
 	}
@@ -796,118 +934,144 @@
 	logger.Debug("SOCKS5 TCP request", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr))
 }
 
 func (l *socks5Logger) TCPError(addr net.Addr, reqAddr string, err error) {
 	if err == nil {
 		logger.Debug("SOCKS5 TCP closed", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr))
 	} else {
-		logger.Error("SOCKS5 TCP error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr), zap.Error(err))
+		logger.Warn("SOCKS5 TCP error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr), zap.Error(err))
 	}
 }
 
 func (l *socks5Logger) UDPRequest(addr net.Addr) {
 	logger.Debug("SOCKS5 UDP request", zap.String("addr", addr.String()))
 }
 
 func (l *socks5Logger) UDPError(addr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("SOCKS5 UDP closed", zap.String("addr", addr.String()))
 	} else {
-		logger.Error("SOCKS5 UDP error", zap.String("addr", addr.String()), zap.Error(err))
+		logger.Warn("SOCKS5 UDP error", zap.String("addr", addr.String()), zap.Error(err))
 	}
 }
 
 type httpLogger struct{}
 
 func (l *httpLogger) ConnectRequest(addr net.Addr, reqAddr string) {
 	logger.Debug("HTTP CONNECT request", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr))
 }
 
 func (l *httpLogger) ConnectError(addr net.Addr, reqAddr string, err error) {
 	if err == nil {
 		logger.Debug("HTTP CONNECT closed", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr))
 	} else {
-		logger.Error("HTTP CONNECT error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr), zap.Error(err))
+		logger.Warn("HTTP CONNECT error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr), zap.Error(err))
 	}
 }
 
 func (l *httpLogger) HTTPRequest(addr net.Addr, reqURL string) {
 	logger.Debug("HTTP request", zap.String("addr", addr.String()), zap.String("reqURL", reqURL))
 }
 
 func (l *httpLogger) HTTPError(addr net.Addr, reqURL string, err error) {
 	if err == nil {
 		logger.Debug("HTTP closed", zap.String("addr", addr.String()), zap.String("reqURL", reqURL))
 	} else {
-		logger.Error("HTTP error", zap.String("addr", addr.String()), zap.String("reqURL", reqURL), zap.Error(err))
+		logger.Warn("HTTP error", zap.String("addr", addr.String()), zap.String("reqURL", reqURL), zap.Error(err))
 	}
 }
 
 type tcpLogger struct{}
 
 func (l *tcpLogger) Connect(addr net.Addr) {
 	logger.Debug("TCP forwarding connect", zap.String("addr", addr.String()))
 }
 
 func (l *tcpLogger) Error(addr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("TCP forwarding closed", zap.String("addr", addr.String()))
 	} else {
-		logger.Error("TCP forwarding error", zap.String("addr", addr.String()), zap.Error(err))
+		logger.Warn("TCP forwarding error", zap.String("addr", addr.String()), zap.Error(err))
 	}
 }
 
 type udpLogger struct{}
 
 func (l *udpLogger) Connect(addr net.Addr) {
 	logger.Debug("UDP forwarding connect", zap.String("addr", addr.String()))
 }
 
 func (l *udpLogger) Error(addr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("UDP forwarding closed", zap.String("addr", addr.String()))
 	} else {
-		logger.Error("UDP forwarding error", zap.String("addr", addr.String()), zap.Error(err))
+		logger.Warn("UDP forwarding error", zap.String("addr", addr.String()), zap.Error(err))
 	}
 }
 
 type tcpTProxyLogger struct{}
 
 func (l *tcpTProxyLogger) Connect(addr, reqAddr net.Addr) {
 	logger.Debug("TCP transparent proxy connect", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 }
 
 func (l *tcpTProxyLogger) Error(addr, reqAddr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("TCP transparent proxy closed", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 	} else {
-		logger.Error("TCP transparent proxy error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
+		logger.Warn("TCP transparent proxy error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
 	}
 }
 
 type udpTProxyLogger struct{}
 
 func (l *udpTProxyLogger) Connect(addr, reqAddr net.Addr) {
 	logger.Debug("UDP transparent proxy connect", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 }
 
 func (l *udpTProxyLogger) Error(addr, reqAddr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("UDP transparent proxy closed", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 	} else {
-		logger.Error("UDP transparent proxy error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
+		logger.Warn("UDP transparent proxy error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
 	}
 }
 
 type tcpRedirectLogger struct{}
 
 func (l *tcpRedirectLogger) Connect(addr, reqAddr net.Addr) {
 	logger.Debug("TCP redirect connect", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 }
 
 func (l *tcpRedirectLogger) Error(addr, reqAddr net.Addr, err error) {
 	if err == nil {
 		logger.Debug("TCP redirect closed", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()))
 	} else {
-		logger.Error("TCP redirect error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
+		logger.Warn("TCP redirect error", zap.String("addr", addr.String()), zap.String("reqAddr", reqAddr.String()), zap.Error(err))
+	}
+}
+
+type tunLogger struct{}
+
+func (l *tunLogger) TCPRequest(addr, reqAddr string) {
+	logger.Debug("TUN TCP request", zap.String("addr", addr), zap.String("reqAddr", reqAddr))
+}
+
+func (l *tunLogger) TCPError(addr, reqAddr string, err error) {
+	if err == nil {
+		logger.Debug("TUN TCP closed", zap.String("addr", addr), zap.String("reqAddr", reqAddr))
+	} else {
+		logger.Warn("TUN TCP error", zap.String("addr", addr), zap.String("reqAddr", reqAddr), zap.Error(err))
+	}
+}
+
+func (l *tunLogger) UDPRequest(addr string) {
+	logger.Debug("TUN UDP request", zap.String("addr", addr))
+}
+
+func (l *tunLogger) UDPError(addr string, err error) {
+	if err == nil {
+		logger.Debug("TUN UDP closed", zap.String("addr", addr))
+	} else {
+		logger.Warn("TUN UDP error", zap.String("addr", addr), zap.Error(err))
 	}
 }
```

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/ping.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/ping.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/root.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/root.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/server.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/server.go`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 	"encoding/json"
 	"errors"
 	"fmt"
 	"net"
 	"net/http"
 	"net/http/httputil"
 	"net/url"
+	"os"
 	"strconv"
 	"strings"
 	"time"
 
 	"github.com/caddyserver/certmagic"
 	"github.com/mholt/acmez/acme"
 	"github.com/spf13/cobra"
@@ -79,14 +80,15 @@
 
 type serverConfigACME struct {
 	Domains        []string `mapstructure:"domains"`
 	Email          string   `mapstructure:"email"`
 	CA             string   `mapstructure:"ca"`
 	DisableHTTP    bool     `mapstructure:"disableHTTP"`
 	DisableTLSALPN bool     `mapstructure:"disableTLSALPN"`
+	ListenHost     string   `mapstructure:"listenHost"`
 	AltHTTPPort    int      `mapstructure:"altHTTPPort"`
 	AltTLSALPNPort int      `mapstructure:"altTLSALPNPort"`
 	Dir            string   `mapstructure:"dir"`
 }
 
 type serverConfigQUIC struct {
 	InitStreamReceiveWindow     uint64        `mapstructure:"initStreamReceiveWindow"`
@@ -249,14 +251,28 @@
 		return configError{Field: "tls", Err: errors.New("cannot set both tls and acme")}
 	}
 	if c.TLS != nil {
 		// Local TLS cert
 		if c.TLS.Cert == "" || c.TLS.Key == "" {
 			return configError{Field: "tls", Err: errors.New("empty cert or key path")}
 		}
+		// Try loading the cert-key pair here to catch errors early
+		// (e.g. invalid files or insufficient permissions)
+		certPEMBlock, err := os.ReadFile(c.TLS.Cert)
+		if err != nil {
+			return configError{Field: "tls.cert", Err: err}
+		}
+		keyPEMBlock, err := os.ReadFile(c.TLS.Key)
+		if err != nil {
+			return configError{Field: "tls.key", Err: err}
+		}
+		_, err = tls.X509KeyPair(certPEMBlock, keyPEMBlock)
+		if err != nil {
+			return configError{Field: "tls", Err: fmt.Errorf("invalid cert-key pair: %w", err)}
+		}
 		// Use GetCertificate instead of Certificates so that
 		// users can update the cert without restarting the server.
 		hyConfig.TLSConfig.GetCertificate = func(info *tls.ClientHelloInfo) (*tls.Certificate, error) {
 			cert, err := tls.LoadX509KeyPair(c.TLS.Cert, c.TLS.Key)
 			return &cert, err
 		}
 	} else {
@@ -276,14 +292,15 @@
 			Logger:             logger,
 		}
 		cmIssuer := certmagic.NewACMEIssuer(cmCfg, certmagic.ACMEIssuer{
 			Email:                   c.ACME.Email,
 			Agreed:                  true,
 			DisableHTTPChallenge:    c.ACME.DisableHTTP,
 			DisableTLSALPNChallenge: c.ACME.DisableTLSALPN,
+			ListenHost:              c.ACME.ListenHost,
 			AltHTTPPort:             c.ACME.AltHTTPPort,
 			AltTLSALPNPort:          c.ACME.AltTLSALPNPort,
 			Logger:                  logger,
 		})
 		switch strings.ToLower(c.ACME.CA) {
 		case "letsencrypt", "le", "":
 			// Default to Let's Encrypt
@@ -809,27 +826,27 @@
 	logger.Debug("TCP request", zap.String("addr", addr.String()), zap.String("id", id), zap.String("reqAddr", reqAddr))
 }
 
 func (l *serverLogger) TCPError(addr net.Addr, id, reqAddr string, err error) {
 	if err == nil {
 		logger.Debug("TCP closed", zap.String("addr", addr.String()), zap.String("id", id), zap.String("reqAddr", reqAddr))
 	} else {
-		logger.Error("TCP error", zap.String("addr", addr.String()), zap.String("id", id), zap.String("reqAddr", reqAddr), zap.Error(err))
+		logger.Warn("TCP error", zap.String("addr", addr.String()), zap.String("id", id), zap.String("reqAddr", reqAddr), zap.Error(err))
 	}
 }
 
 func (l *serverLogger) UDPRequest(addr net.Addr, id string, sessionID uint32, reqAddr string) {
 	logger.Debug("UDP request", zap.String("addr", addr.String()), zap.String("id", id), zap.Uint32("sessionID", sessionID), zap.String("reqAddr", reqAddr))
 }
 
 func (l *serverLogger) UDPError(addr net.Addr, id string, sessionID uint32, err error) {
 	if err == nil {
 		logger.Debug("UDP closed", zap.String("addr", addr.String()), zap.String("id", id), zap.Uint32("sessionID", sessionID))
 	} else {
-		logger.Error("UDP error", zap.String("addr", addr.String()), zap.String("id", id), zap.Uint32("sessionID", sessionID), zap.Error(err))
+		logger.Warn("UDP error", zap.String("addr", addr.String()), zap.String("id", id), zap.Uint32("sessionID", sessionID), zap.Error(err))
 	}
 }
 
 type masqHandlerLogWrapper struct {
 	H    http.Handler
 	QUIC bool
 }
```

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/server_test.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/server_test.yaml` & `hysteria2-2.4.3/hysteria2-go/app/cmd/server_test.yaml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/speedtest.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/speedtest.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/cmd/update.go` & `hysteria2-2.4.3/hysteria2-go/app/cmd/update.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/go.mod` & `hysteria2-2.4.3/hysteria2-go/app/go.mod`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 
 go 1.21
 
 require (
 	github.com/apernet/go-tproxy v0.0.0-20230809025308-8f4723fd742f
 	github.com/apernet/hysteria/core v0.0.0-00010101000000-000000000000
 	github.com/apernet/hysteria/extras v0.0.0-00010101000000-000000000000
+	github.com/apernet/sing-tun v0.2.6-0.20240323130332-b9f6511036ad
 	github.com/caddyserver/certmagic v0.17.2
 	github.com/mdp/qrterminal/v3 v3.1.1
 	github.com/mholt/acmez v1.0.4
+	github.com/sagernet/sing v0.3.2
 	github.com/spf13/cobra v1.7.0
 	github.com/spf13/viper v1.15.0
 	github.com/stretchr/testify v1.8.4
 	github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301
 	go.uber.org/zap v1.24.0
+	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db
+	golang.org/x/sys v0.19.0
 )
 
 require (
-	github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d // indirect
+	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 // indirect
 	github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 // indirect
 	github.com/davecgh/go-spew v1.1.1 // indirect
-	github.com/fsnotify/fsnotify v1.6.0 // indirect
+	github.com/fsnotify/fsnotify v1.7.0 // indirect
+	github.com/go-ole/go-ole v1.3.0 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
 	github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 // indirect
 	github.com/hashicorp/golang-lru/v2 v2.0.5 // indirect
 	github.com/hashicorp/hcl v1.0.0 // indirect
 	github.com/inconshreveable/mousetrap v1.1.0 // indirect
 	github.com/klauspost/cpuid/v2 v2.1.1 // indirect
 	github.com/libdns/libdns v0.2.1 // indirect
@@ -32,32 +37,34 @@
 	github.com/miekg/dns v1.1.55 // indirect
 	github.com/mitchellh/mapstructure v1.5.0 // indirect
 	github.com/onsi/ginkgo/v2 v2.9.5 // indirect
 	github.com/patrickmn/go-cache v2.1.0+incompatible // indirect
 	github.com/pelletier/go-toml/v2 v2.0.6 // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
 	github.com/quic-go/qpack v0.4.0 // indirect
+	github.com/sagernet/netlink v0.0.0-20220905062125-8043b4a9aa97 // indirect
+	github.com/scjalliance/comshim v0.0.0-20230315213746-5e51f40bd3b9 // indirect
 	github.com/spf13/afero v1.9.3 // indirect
 	github.com/spf13/cast v1.5.0 // indirect
 	github.com/spf13/jwalterweatherman v1.1.0 // indirect
 	github.com/spf13/pflag v1.0.5 // indirect
 	github.com/stretchr/objx v0.5.0 // indirect
 	github.com/subosito/gotenv v1.4.2 // indirect
 	github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf // indirect
+	github.com/vishvananda/netns v0.0.0-20211101163701-50045581ed74 // indirect
 	go.uber.org/atomic v1.11.0 // indirect
-	go.uber.org/mock v0.3.0 // indirect
+	go.uber.org/mock v0.4.0 // indirect
 	go.uber.org/multierr v1.11.0 // indirect
-	golang.org/x/crypto v0.17.0 // indirect
-	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db // indirect
+	go4.org/netipx v0.0.0-20231129151722-fdeea329fbba // indirect
+	golang.org/x/crypto v0.22.0 // indirect
 	golang.org/x/mod v0.12.0 // indirect
-	golang.org/x/net v0.17.0 // indirect
-	golang.org/x/sys v0.15.0 // indirect
+	golang.org/x/net v0.24.0 // indirect
 	golang.org/x/text v0.14.0 // indirect
 	golang.org/x/tools v0.11.1 // indirect
-	google.golang.org/protobuf v1.28.1 // indirect
+	google.golang.org/protobuf v1.33.0 // indirect
 	gopkg.in/ini.v1 v1.67.0 // indirect
 	gopkg.in/yaml.v3 v3.0.1 // indirect
 	rsc.io/qr v0.2.0 // indirect
 )
 
 replace github.com/apernet/hysteria/core => ../core
```

### Comparing `hysteria2-2.3.0/hysteria2-go/app/go.sum` & `hysteria2-2.4.3/hysteria2-go/app/go.sum`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 cloud.google.com/go/storage v1.10.0/go.mod h1:FLPqc6j+Ki4BU591ie1oL6qBQGu2Bl/tZ9ullr3+Kg0=
 cloud.google.com/go/storage v1.14.0/go.mod h1:GrKmX003DSIwi9o29oFT7YDnHYwZoctc3fOKtUw0Xmo=
 dmitri.shuralyov.com/gpu/mtl v0.0.0-20190408044501-666a987793e9/go.mod h1:H6x//7gZCb22OMCxBHrMx7a5I7Hp++hsVxbQ4BYO7hU=
 github.com/BurntSushi/toml v0.3.1/go.mod h1:xHWCNGjB5oqiDr8zfno3MHue2Ht5sIBksp03qcyfWMU=
 github.com/BurntSushi/xgb v0.0.0-20160522181843-27f122750802/go.mod h1:IVnqGOEym/WlBOVXweHU+Q+/VP0lqqI8lqeDx9IjBqo=
 github.com/apernet/go-tproxy v0.0.0-20230809025308-8f4723fd742f h1:uVh0qpEslrWjgzx9vOcyCqsOY3c9kofDZ1n+qaw35ZY=
 github.com/apernet/go-tproxy v0.0.0-20230809025308-8f4723fd742f/go.mod h1:xkkq9D4ygcldQQhKS/w9CadiCKwCngU7K9E3DaKahpM=
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d h1:K1DMSNtPcaZ/lihYmOHnjThNfUX7cD6SNuVRFnVLVmI=
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d/go.mod h1:4GInxO6ypy63J2NaO5rQx1wRp6K8YHI6zqLG+VswU6I=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
+github.com/apernet/sing-tun v0.2.6-0.20240323130332-b9f6511036ad h1:QzQ2sKpc9o42HNRR8ukM5uMC/RzR2HgZd/Nvaqol2C0=
+github.com/apernet/sing-tun v0.2.6-0.20240323130332-b9f6511036ad/go.mod h1:S5IydyLSN/QAfvY+r2GoomPJ6hidtXWm/Ad18sJVssk=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 h1:4NNbNM2Iq/k57qEu7WfL67UrbPq1uFWxW4qODCohi+0=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6/go.mod h1:J29hk+f9lJrblVIfiJOtTFk+OblBawmib4uz/VdKzlg=
 github.com/benbjohnson/clock v1.1.0 h1:Q92kusRqC1XV2MjkWETPvjJVqKetz1OzxZB7mHJLju8=
 github.com/benbjohnson/clock v1.1.0/go.mod h1:J11/hYXuz8f4ySSvYwY0FKfm+ezbsZBKZxNJlLklBHA=
 github.com/caddyserver/certmagic v0.17.2 h1:o30seC1T/dBqBCNNGNHWwj2i5/I/FMjBbTAhjADP3nE=
 github.com/caddyserver/certmagic v0.17.2/go.mod h1:ouWUuC490GOLJzkyN35eXfV8bSbwMwSf4bdhkIxtdQE=
 github.com/census-instrumentation/opencensus-proto v0.2.1/go.mod h1:f6KPmirojxKA12rnyqOA5BBL4O983OfeGPqjHWSTneU=
@@ -64,21 +66,23 @@
 github.com/envoyproxy/go-control-plane v0.9.1-0.20191026205805-5f8ba28d4473/go.mod h1:YTl/9mNaCwkRvm6d1a2C3ymFceY/DCBVvsKhRF0iEA4=
 github.com/envoyproxy/go-control-plane v0.9.4/go.mod h1:6rpuAdCZL397s3pYoYcLgu1mIlRU8Am5FuJP05cCM98=
 github.com/envoyproxy/go-control-plane v0.9.7/go.mod h1:cwu0lG7PUMfa9snN8LXBig5ynNVH9qI8YYLbd1fK2po=
 github.com/envoyproxy/go-control-plane v0.9.9-0.20201210154907-fd9021fe5dad/go.mod h1:cXg6YxExXjJnVBQHBLXeUAgxn2UodCpnH306RInaBQk=
 github.com/envoyproxy/protoc-gen-validate v0.1.0/go.mod h1:iSmxcyjqTsJpI2R4NaDN7+kN2VEUnK/pcBlmesArF7c=
 github.com/frankban/quicktest v1.14.3 h1:FJKSZTDHjyhriyC81FLQ0LY93eSai0ZyR/ZIkd3ZUKE=
 github.com/frankban/quicktest v1.14.3/go.mod h1:mgiwOwqx65TmIk1wJ6Q7wvnVMocbUorkibMOrVTHZps=
-github.com/fsnotify/fsnotify v1.6.0 h1:n+5WquG0fcWoWp6xPWfHdbskMCQaFnG6PfBrh1Ky4HY=
-github.com/fsnotify/fsnotify v1.6.0/go.mod h1:sl3t1tCWJFWoRz9R8WJCbQihKKwmorjAbSClcnxKAGw=
+github.com/fsnotify/fsnotify v1.7.0 h1:8JEhPFa5W2WU7YfeZzPNqzMP6Lwt7L2715Ggo0nosvA=
+github.com/fsnotify/fsnotify v1.7.0/go.mod h1:40Bi/Hjc2AVfZrqy+aj+yEI+/bRxZnMJyTJwOpGvigM=
 github.com/go-gl/glfw v0.0.0-20190409004039-e6da0acd62b1/go.mod h1:vR7hzQXu2zJy9AVAgeJqvqgH9Q5CA+iKCZ2gyEVpxRU=
 github.com/go-gl/glfw/v3.3/glfw v0.0.0-20191125211704-12ad95a8df72/go.mod h1:tQ2UAYgL5IevRw8kRxooKSPJfGvJ9fJQFa0TUsXzTg8=
 github.com/go-gl/glfw/v3.3/glfw v0.0.0-20200222043503-6f7a984d4dc4/go.mod h1:tQ2UAYgL5IevRw8kRxooKSPJfGvJ9fJQFa0TUsXzTg8=
 github.com/go-logr/logr v1.2.4 h1:g01GSCwiDw2xSZfjJ2/T9M+S6pFdcNtFYsp+Y43HYDQ=
 github.com/go-logr/logr v1.2.4/go.mod h1:jdQByPbusPIv2/zmleS9BjJVeZ6kBagPoEUsqbVz/1A=
+github.com/go-ole/go-ole v1.3.0 h1:Dt6ye7+vXGIKZ7Xtk4s6/xVdGDQynvom7xCFEdWr6uE=
+github.com/go-ole/go-ole v1.3.0/go.mod h1:5LS6F96DhAwUc7C+1HLexzMXY1xGRSryjyPPKW6zv78=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 h1:tfuBGBXKqDEevZMzYi5KSi8KkcZtzBcTgAUUtapy0OI=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572/go.mod h1:9Pwr4B2jHnOSGXyyzV8ROjYa2ojvAY6HCGYYfMoC3Ls=
 github.com/golang/glog v0.0.0-20160126235308-23def4e6c14b/go.mod h1:SBH7ygxi8pfUlaOkMMuAQtPIUF8ecWP5IEl/CR7VP2Q=
 github.com/golang/groupcache v0.0.0-20190702054246-869f871628b6/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/groupcache v0.0.0-20191227052852-215e87163ea7/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/groupcache v0.0.0-20200121045136-8c9f03a8e57e/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/mock v1.1.1/go.mod h1:oTYuIxOrZwtPieC+H1uAHpcLFnEyAGVDL/k47Jfbm0A=
@@ -98,29 +102,27 @@
 github.com/golang/protobuf v1.4.0-rc.1.0.20200221234624-67d41d38c208/go.mod h1:xKAWHe0F5eneWXFV3EuXVDTCmh+JuBKY0li0aMyXATA=
 github.com/golang/protobuf v1.4.0-rc.2/go.mod h1:LlEzMj4AhA7rCAGe4KMBDvJI+AwstrUpVNzEA03Pprs=
 github.com/golang/protobuf v1.4.0-rc.4.0.20200313231945-b860323f09d0/go.mod h1:WU3c8KckQ9AFe+yFwt9sWVRKCVIyN9cPHBJSNnbL67w=
 github.com/golang/protobuf v1.4.0/go.mod h1:jodUvKwWbYaEsadDk5Fwe5c77LiNKVO9IDvqG2KuDX0=
 github.com/golang/protobuf v1.4.1/go.mod h1:U8fpvMrcmy5pZrNK1lt4xCsGvpyWQ/VVv6QDs8UjoX8=
 github.com/golang/protobuf v1.4.2/go.mod h1:oDoupMAO8OvCJWAcko0GGGIgR6R6ocIYbsSw735rRwI=
 github.com/golang/protobuf v1.4.3/go.mod h1:oDoupMAO8OvCJWAcko0GGGIgR6R6ocIYbsSw735rRwI=
-github.com/golang/protobuf v1.5.0/go.mod h1:FsONVRAS9T7sI+LIUmWTfcYkHO4aIWwzhcaSAoJOfIk=
 github.com/golang/protobuf v1.5.3 h1:KhyjKVUg7Usr/dYsdSqoFveMYd5ko72D+zANwlG1mmg=
 github.com/golang/protobuf v1.5.3/go.mod h1:XVQd3VNwM+JqD3oG2Ue2ip4fOMUkwXdXDdiuN0vRsmY=
 github.com/google/btree v0.0.0-20180813153112-4030bb1f1f0c/go.mod h1:lNA+9X1NB3Zf8V7Ke586lFgjr2dZNuvo3lPJSGZ5JPQ=
 github.com/google/btree v1.0.0/go.mod h1:lNA+9X1NB3Zf8V7Ke586lFgjr2dZNuvo3lPJSGZ5JPQ=
 github.com/google/go-cmp v0.2.0/go.mod h1:oXzfMopK8JAjlY9xF4vHSVASa0yLyX7SntLO5aqRK0M=
 github.com/google/go-cmp v0.3.0/go.mod h1:8QqcDgzrUqlUb/G2PQTWiueGozuR1884gddMywk6iLU=
 github.com/google/go-cmp v0.3.1/go.mod h1:8QqcDgzrUqlUb/G2PQTWiueGozuR1884gddMywk6iLU=
 github.com/google/go-cmp v0.4.0/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.4.1/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.0/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.1/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.2/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.4/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
-github.com/google/go-cmp v0.5.5/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.9 h1:O2Tfq5qg4qc4AmwVlvv0oLiVAGB7enBSJ2x2DqQFi38=
 github.com/google/go-cmp v0.5.9/go.mod h1:17dUlkBOakJ0+DkrSSNjCkIjxS6bF9zb3elmeNGIjoY=
 github.com/google/martian v2.1.0+incompatible/go.mod h1:9I4somxYTbIHy5NJKHRl3wXiIaQGbYVAs8BPL6v8lEs=
 github.com/google/martian/v3 v3.0.0/go.mod h1:y5Zk1BBys9G+gd6Jrk0W3cC1+ELVxBWuIGO+w/tUAp0=
 github.com/google/martian/v3 v3.1.0/go.mod h1:y5Zk1BBys9G+gd6Jrk0W3cC1+ELVxBWuIGO+w/tUAp0=
 github.com/google/pprof v0.0.0-20181206194817-3ea8567a2e57/go.mod h1:zfwlbNMJ+OItoe0UupaVj+oy1omPYYDuagoSzA8v9mc=
 github.com/google/pprof v0.0.0-20190515194954-54271f7e092f/go.mod h1:zfwlbNMJ+OItoe0UupaVj+oy1omPYYDuagoSzA8v9mc=
@@ -194,14 +196,20 @@
 github.com/prometheus/client_model v0.0.0-20190812154241-14fe0d1b01d4/go.mod h1:xMI15A0UPsDsEKsMN9yxemIoYk6Tm2C1GtYGdfGttqA=
 github.com/quic-go/qpack v0.4.0 h1:Cr9BXA1sQS2SmDUWjSofMPNKmvF6IiIfDRmgU0w1ZCo=
 github.com/quic-go/qpack v0.4.0/go.mod h1:UZVnYIfi5GRk+zI9UMaCPsmZ2xKJP7XBUvVyT1Knj9A=
 github.com/rogpeppe/go-internal v1.3.0/go.mod h1:M8bDsm7K2OlrFYOpmOWEs/qY81heoFRclV5y23lUDJ4=
 github.com/rogpeppe/go-internal v1.6.1 h1:/FiVV8dS/e+YqF2JvO3yXRFbBLTIuSDkuC7aBOAvL+k=
 github.com/rogpeppe/go-internal v1.6.1/go.mod h1:xXDCJY+GAPziupqXw64V24skbSoqbTEfhy4qGm1nDQc=
 github.com/russross/blackfriday/v2 v2.1.0/go.mod h1:+Rmxgy9KzJVeS9/2gXHxylqXiyQDYRxCVz55jmeOWTM=
+github.com/sagernet/netlink v0.0.0-20220905062125-8043b4a9aa97 h1:iL5gZI3uFp0X6EslacyapiRz7LLSJyr4RajF/BhMVyE=
+github.com/sagernet/netlink v0.0.0-20220905062125-8043b4a9aa97/go.mod h1:xLnfdiJbSp8rNqYEdIW/6eDO4mVoogml14Bh2hSiFpM=
+github.com/sagernet/sing v0.3.2 h1:CwWcxUBPkMvwgfe2/zUgY5oHG9qOL8Aob/evIFYK9jo=
+github.com/sagernet/sing v0.3.2/go.mod h1:qHySJ7u8po9DABtMYEkNBcOumx7ZZJf/fbv2sfTkNHE=
+github.com/scjalliance/comshim v0.0.0-20230315213746-5e51f40bd3b9 h1:rc/CcqLH3lh8n+csdOuDfP+NuykE0U6AeYSJJHKDgSg=
+github.com/scjalliance/comshim v0.0.0-20230315213746-5e51f40bd3b9/go.mod h1:a/83NAfUXvEuLpmxDssAXxgUgrEy12MId3Wd7OTs76s=
 github.com/spf13/afero v1.9.3 h1:41FoI0fD7OR7mGcKE/aOiLkGreyf8ifIOQmJANWogMk=
 github.com/spf13/afero v1.9.3/go.mod h1:iUV7ddyEEZPO5gA3zD4fJt6iStLlL+Lg4m2cihcDf8Y=
 github.com/spf13/cast v1.5.0 h1:rj3WzYc11XZaIZMPKmwP96zkFEnnAmV8s6XbB2aY32w=
 github.com/spf13/cast v1.5.0/go.mod h1:SpXXQ5YoyJw6s3/6cMTQuxvgRl3PCJiyaX9p6b155UU=
 github.com/spf13/cobra v1.7.0 h1:hyqWnYt1ZQShIddO5kBpj3vu05/++x6tJ6dg8EC572I=
 github.com/spf13/cobra v1.7.0/go.mod h1:uLxZILRyS/50WlhOIKD7W6V5bgeIt+4sICxh6uRMrb0=
 github.com/spf13/jwalterweatherman v1.1.0 h1:ue6voC5bR5F8YxI5S67j9i582FU4Qvo2bmqnqMYADFk=
@@ -227,14 +235,16 @@
 github.com/stretchr/testify v1.8.4/go.mod h1:sz/lmYIOXD/1dqDmKjjqLyZ2RngseejIcXlSw2iwfAo=
 github.com/subosito/gotenv v1.4.2 h1:X1TuBLAMDFbaTAChgCBLu3DU3UPyELpnF2jjJ2cz/S8=
 github.com/subosito/gotenv v1.4.2/go.mod h1:ayKnFf/c6rvx/2iiLrJUk1e6plDbT3edrFNGqEflhK0=
 github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf h1:7PflaKRtU4np/epFxRXlFhlzLXZzKFrH5/I4so5Ove0=
 github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf/go.mod h1:CLUSJbazqETbaR+i0YAhXBICV9TrKH93pziccMhmhpM=
 github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301 h1:d/Wr/Vl/wiJHc3AHYbYs5I3PucJvRuw3SvbmlIRf+oM=
 github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301/go.mod h1:ntmMHL/xPq1WLeKiw8p/eRATaae6PiVRNipHFJxI8PM=
+github.com/vishvananda/netns v0.0.0-20211101163701-50045581ed74 h1:gga7acRE695APm9hlsSMoOoE65U4/TcqNj90mc69Rlg=
+github.com/vishvananda/netns v0.0.0-20211101163701-50045581ed74/go.mod h1:DD4vA1DwXk04H54A1oHXtwZmA0grkVMdPxx/VGLCah0=
 github.com/yuin/goldmark v1.1.25/go.mod h1:3hX8gzYuyVAZsxl0MRgGTJEmQBFcNTphYh9decYSb74=
 github.com/yuin/goldmark v1.1.27/go.mod h1:3hX8gzYuyVAZsxl0MRgGTJEmQBFcNTphYh9decYSb74=
 github.com/yuin/goldmark v1.1.32/go.mod h1:3hX8gzYuyVAZsxl0MRgGTJEmQBFcNTphYh9decYSb74=
 github.com/yuin/goldmark v1.2.1/go.mod h1:3hX8gzYuyVAZsxl0MRgGTJEmQBFcNTphYh9decYSb74=
 github.com/yuin/goldmark v1.3.5/go.mod h1:mwnBkeHKe2W/ZEtQ+71ViKU8L12m81fl3OWwC1Zlc8k=
 github.com/yuin/goldmark v1.4.13/go.mod h1:6yULJ656Px+3vBD8DxQVa3kxgyrAnzto9xy5taEt/CY=
 go.opencensus.io v0.21.0/go.mod h1:mSImk1erAIZhrmZN+AvHh14ztQfjbGwt4TtuofqLduU=
@@ -245,32 +255,34 @@
 go.opencensus.io v0.22.5/go.mod h1:5pWMHQbX5EPX2/62yrJeAkowc+lfs/XD7Uxpq3pI6kk=
 go.uber.org/atomic v1.7.0/go.mod h1:fEN4uk6kAWBTFdckzkM89CLk9XfWZrxpCo0nPH17wJc=
 go.uber.org/atomic v1.11.0 h1:ZvwS0R+56ePWxUNi+Atn9dWONBPp/AUETXlHW0DxSjE=
 go.uber.org/atomic v1.11.0/go.mod h1:LUxbIzbOniOlMKjJjyPfpl4v+PKK2cNJn91OQbhoJI0=
 go.uber.org/goleak v1.1.11/go.mod h1:cwTWslyiVhfpKIDGSZEM2HlOvcqm+tG4zioyIeLoqMQ=
 go.uber.org/goleak v1.2.1 h1:NBol2c7O1ZokfZ0LEU9K6Whx/KnwvepVetCUhtKja4A=
 go.uber.org/goleak v1.2.1/go.mod h1:qlT2yGI9QafXHhZZLxlSuNsMw3FFLxBr+tBRlmO1xH4=
-go.uber.org/mock v0.3.0 h1:3mUxI1No2/60yUYax92Pt8eNOEecx2D3lcXZh2NEZJo=
-go.uber.org/mock v0.3.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
+go.uber.org/mock v0.4.0 h1:VcM4ZOtdbR4f6VXfiOpwpVJDL6lCReaZ6mw31wqh7KU=
+go.uber.org/mock v0.4.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
 go.uber.org/multierr v1.6.0/go.mod h1:cdWPpRnG4AhwMwsgIHip0KRBQjJy5kYEpYjJxpXp9iU=
 go.uber.org/multierr v1.11.0 h1:blXXJkSxSSfBVBlC76pxqeO+LN3aDfLQo+309xJstO0=
 go.uber.org/multierr v1.11.0/go.mod h1:20+QtiLqy0Nd6FdQB9TLXag12DsQkrbs3htMFfDN80Y=
 go.uber.org/zap v1.21.0/go.mod h1:wjWOCqI0f2ZZrJF/UufIOkiC8ii6tm1iqIsLo76RfJw=
 go.uber.org/zap v1.24.0 h1:FiJd5l1UOLj0wCgbSE0rwwXHzEdAZS6hiiSnxJN/D60=
 go.uber.org/zap v1.24.0/go.mod h1:2kMP+WWQ8aoFoedH3T2sq6iJ2yDWpHbP0f6MQbS9Gkg=
+go4.org/netipx v0.0.0-20231129151722-fdeea329fbba h1:0b9z3AuHCjxk0x/opv64kcgZLBseWJUpBw5I82+2U4M=
+go4.org/netipx v0.0.0-20231129151722-fdeea329fbba/go.mod h1:PLyyIXexvUFg3Owu6p/WfdlivPbZJsZdgWZlrGope/Y=
 golang.org/x/crypto v0.0.0-20190308221718-c2843e01d9a2/go.mod h1:djNgcEr1/C05ACkg1iLfiJU5Ep61QUkGW8qpdssI0+w=
 golang.org/x/crypto v0.0.0-20190510104115-cbcb75029529/go.mod h1:yigFU9vqHzYiE8UmvKecakEJjdnWj3jj499lnFckfCI=
 golang.org/x/crypto v0.0.0-20190605123033-f99c8df09eb5/go.mod h1:yigFU9vqHzYiE8UmvKecakEJjdnWj3jj499lnFckfCI=
 golang.org/x/crypto v0.0.0-20191011191535-87dc89f01550/go.mod h1:yigFU9vqHzYiE8UmvKecakEJjdnWj3jj499lnFckfCI=
 golang.org/x/crypto v0.0.0-20200622213623-75b288015ac9/go.mod h1:LzIPMQfyMNhhGPhUkYOs5KpL4U8rLKemX1yGLhDgUto=
 golang.org/x/crypto v0.0.0-20210421170649-83a5a9bb288b/go.mod h1:T9bdIzuCu7OtxOm1hfPfRQxPLYneinmdGuTeoZ9dtd4=
 golang.org/x/crypto v0.0.0-20210921155107-089bfa567519/go.mod h1:GvvjBRRGRdwPK5ydBHafDWAxML/pGHZbMvKqRZ5+Abc=
 golang.org/x/crypto v0.0.0-20211108221036-ceb1ce70b4fa/go.mod h1:GvvjBRRGRdwPK5ydBHafDWAxML/pGHZbMvKqRZ5+Abc=
-golang.org/x/crypto v0.17.0 h1:r8bRNjWL3GshPW3gkd+RpvzWrZAwPS49OmTGZ/uhM4k=
-golang.org/x/crypto v0.17.0/go.mod h1:gCAAfMLgwOJRpTjQ2zCCt2OcSfYMTeZVSRtQlPC7Nq4=
+golang.org/x/crypto v0.22.0 h1:g1v0xeRhjcugydODzvb3mEM9SQ0HGp9s/nh3COQ/C30=
+golang.org/x/crypto v0.22.0/go.mod h1:vr6Su+7cTlO45qkww3VDJlzDn0ctJvRgYbC2NvXHt+M=
 golang.org/x/exp v0.0.0-20190121172915-509febef88a4/go.mod h1:CJ0aWSM057203Lf6IL+f9T1iT9GByDxfZKAQTCR3kQA=
 golang.org/x/exp v0.0.0-20190306152737-a1d7652674e8/go.mod h1:CJ0aWSM057203Lf6IL+f9T1iT9GByDxfZKAQTCR3kQA=
 golang.org/x/exp v0.0.0-20190510132918-efd6b22b2522/go.mod h1:ZjyILWgesfNpC6sMxTJOJm9Kp84zZh5NQWvqDGG3Qr8=
 golang.org/x/exp v0.0.0-20190829153037-c13cbed26979/go.mod h1:86+5VVa7VpoJ4kLfm080zCjGlMRFzhUhsZKEZO7MGek=
 golang.org/x/exp v0.0.0-20191030013958-a1ab85dbe136/go.mod h1:JXzH8nQsPlswgeRAPE3MuO9GYsAcnJvJ4vnMwN/5qkY=
 golang.org/x/exp v0.0.0-20191129062945-2f5052295587/go.mod h1:2RIsYlXP63K8oxa1u096TMicItID8zy7Y6sNkU49FU4=
 golang.org/x/exp v0.0.0-20191227195350-da58074b4299/go.mod h1:2RIsYlXP63K8oxa1u096TMicItID8zy7Y6sNkU49FU4=
@@ -338,16 +350,16 @@
 golang.org/x/net v0.0.0-20201209123823-ac852fbbde11/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20201224014010-6772e930b67b/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20210226172049-e18ecbb05110/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20210405180319-a5a99cb37ef4/go.mod h1:p54w0d4576C0XHj96bSt6lcn1PtDYWL6XObtHCRCNQM=
 golang.org/x/net v0.0.0-20220630215102-69896b714898/go.mod h1:XRhObCWvk6IyKnWLug+ECip1KBveYUHfp+8e9klMJ9c=
 golang.org/x/net v0.0.0-20220722155237-a158d28d115b/go.mod h1:XRhObCWvk6IyKnWLug+ECip1KBveYUHfp+8e9klMJ9c=
 golang.org/x/net v0.2.0/go.mod h1:KqCZLdyyvdV855qA2rE3GC2aiw5xGR5TEjj8smXukLY=
-golang.org/x/net v0.17.0 h1:pVaXccu2ozPjCXewfr1S7xza/zcXTity9cCdXQYSjIM=
-golang.org/x/net v0.17.0/go.mod h1:NxSsAGuq816PNPmqtQdLE42eU2Fs7NoRIZrHJAlaCOE=
+golang.org/x/net v0.24.0 h1:1PcaxkF854Fu3+lvBIx5SYn9wRlBzzcnHZSiaFFAb0w=
+golang.org/x/net v0.24.0/go.mod h1:2Q7sJY5mzlzWjKtYUEXSlBWCdyaioyXzRB2RtU8KVE8=
 golang.org/x/oauth2 v0.0.0-20180821212333-d2e6202438be/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20190226205417-e64efc72b421/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20190604053449-0f29369cfe45/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20191202225959-858c2ad4c8b6/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20200107190931-bf48bf16ab8d/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20200902213428-5d25da1a8d43/go.mod h1:KelEdhl1UZF7XfJ4dDtk6s++YSgaE7mD/BuKKDLBl4A=
 golang.org/x/oauth2 v0.0.0-20201109201403-9fd604954f58/go.mod h1:KelEdhl1UZF7XfJ4dDtk6s++YSgaE7mD/BuKKDLBl4A=
@@ -380,14 +392,15 @@
 golang.org/x/sys v0.0.0-20191001151750-bb3f8db39f24/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20191204072324-ce4227a45e2e/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20191228213918-04cbcbbfeed8/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200113162924-86b910548bc1/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200122134326-e047566fdf82/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200202164722-d101bd2416d5/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200212091648-12a6c2dcc1e4/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
+golang.org/x/sys v0.0.0-20200217220822-9197077df867/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200223170610-d5e6a3e2c0ae/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200302150141-5c8b2ff67527/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200323222414-85ca7c5b95cd/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200331124033-c3d80250170d/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200501052902-10377860bb8e/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200511232937-7e40ca221e25/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200515095857-1151b9dac4a9/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
@@ -403,18 +416,18 @@
 golang.org/x/sys v0.0.0-20210330210617-4fbd30eecc44/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20210423185535-09eb48e85fd7/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20210510120138-977fb7262007/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20210615035016-665e8c7367d1/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220520151302-bc2c85ada10a/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220704084225-05e143d24a9e/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220722155257-8c9f86f7a55f/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.0.0-20220908164124-27713097b956/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
+golang.org/x/sys v0.1.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.2.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.15.0 h1:h48lPFYpsTvQJZF4EKyI4aLHaev3CxivZmv7yZig9pc=
-golang.org/x/sys v0.15.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/sys v0.19.0 h1:q5f1RH2jigJ1MoAWp2KTp3gm5zAGFUTarQZ5U386+4o=
+golang.org/x/sys v0.19.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/term v0.0.0-20201126162022-7de9c90e9dd1/go.mod h1:bj7SfCRtBDWHUb9snDiAeCFNEtKQo2Wmx5Cou7ajbmo=
 golang.org/x/term v0.0.0-20210927222741-03fcf44c2211/go.mod h1:jbD1KX2456YbFQfuXm/mYQcufACuNUgVhRMnK/tPxf8=
 golang.org/x/term v0.2.0/go.mod h1:TVmDHMZPmdnySmBfhjOoOdhjzdE1h4u1VwSiw2l1Nuc=
 golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.0/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.1-0.20180807135948-17ff2d5776d2/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.2/go.mod h1:bEr9sfX3Q8Zfm5fL9x+3itogRgK3+ptLWKqgva+5dAk=
@@ -423,14 +436,16 @@
 golang.org/x/text v0.3.7/go.mod h1:u+2+/6zg+i71rQMx5EYifcz6MCKuco9NR6JIITiCfzQ=
 golang.org/x/text v0.4.0/go.mod h1:mrYo+phRRbMaCq/xk9113O4dZlRixOauAjOtrjsXDZ8=
 golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
 golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
 golang.org/x/time v0.0.0-20181108054448-85acf8d2951c/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/time v0.0.0-20190308202827-9d24e82272b4/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/time v0.0.0-20191024005414-555d28b269f0/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
+golang.org/x/time v0.5.0 h1:o7cqy6amK/52YcAKIPlM3a+Fpj35zvRj2TP+e1xFSfk=
+golang.org/x/time v0.5.0/go.mod h1:3BpzKBy/shNhVucY/MWOyx10tF3SFh9QdLuxbVysPQM=
 golang.org/x/tools v0.0.0-20180917221912-90fa682c2a6e/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190114222345-bf090417da8b/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190226205152-f727befe758c/go.mod h1:9Yl7xja0Znq3iFh3HoIrodX9oNMXvdceNzlUR8zjMvY=
 golang.org/x/tools v0.0.0-20190311212946-11955173bddd/go.mod h1:LCzVGOaR6xXOjkQ3onu1FJEFr0SW1gC7cKk1uF8kGRs=
 golang.org/x/tools v0.0.0-20190312151545-0bb0c0a6e846/go.mod h1:LCzVGOaR6xXOjkQ3onu1FJEFr0SW1gC7cKk1uF8kGRs=
 golang.org/x/tools v0.0.0-20190312170243-e65039ee4138/go.mod h1:LCzVGOaR6xXOjkQ3onu1FJEFr0SW1gC7cKk1uF8kGRs=
 golang.org/x/tools v0.0.0-20190425150028-36563e24a262/go.mod h1:RgjU9mgBXZiqYHBnxXauZ1Gv1EHHAz9KjViQ78xBX0Q=
@@ -567,17 +582,16 @@
 google.golang.org/protobuf v1.20.1-0.20200309200217-e05f789c0967/go.mod h1:A+miEFZTKqfCUM6K7xSMQL9OKL/b6hQv+e19PK+JZNE=
 google.golang.org/protobuf v1.21.0/go.mod h1:47Nbq4nVaFHyn7ilMalzfO3qCViNmqZ2kzikPIcrTAo=
 google.golang.org/protobuf v1.22.0/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.23.0/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.23.1-0.20200526195155-81db48ad09cc/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.24.0/go.mod h1:r/3tXBNzIEhYS9I1OUVjXDlt8tc493IdKGjtUeSXeh4=
 google.golang.org/protobuf v1.25.0/go.mod h1:9JNX74DMeImyA3h4bdi1ymwjUzf21/xIlbajtzgsN7c=
-google.golang.org/protobuf v1.26.0-rc.1/go.mod h1:jlhhOSvTdKEhbULTjvd4ARK9grFBp09yW+WbY/TyQbw=
-google.golang.org/protobuf v1.28.1 h1:d0NfwRgPtno5B1Wa6L2DAG+KivqkdutMf1UhdNx175w=
-google.golang.org/protobuf v1.28.1/go.mod h1:HV8QOd/L58Z+nl8r43ehVNZIU/HEI6OcFqwMG9pJV4I=
+google.golang.org/protobuf v1.33.0 h1:uNO2rsAINq/JlFpSdYEKIZ0uKD/R9cpdv0T+yoGwGmI=
+google.golang.org/protobuf v1.33.0/go.mod h1:c6P6GXX6sHbq/GpV6MGZEdwhWPcYBgnhAHhKbcUYpos=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f h1:BLraFXnmrev5lT+xlilqcH8XK9/i0At2xKjWk4p6zsU=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/errgo.v2 v2.1.0/go.mod h1:hNsd1EY+bozCKY1Ytp96fpM3vjJbqLJn88ws8XvfDNI=
 gopkg.in/ini.v1 v1.67.0 h1:Dgnx+6+nfE+IfzjUEISNeydPJh9AXNNsWbGP9KzCsOA=
 gopkg.in/ini.v1 v1.67.0/go.mod h1:pNLf8WUiyNEtQjuu5G5vTm06TEv9tsIgeAvK8hOrP4k=
```

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/tcp.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/tcp_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/tcp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/udp.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/forwarding/udp_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/forwarding/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/http/server.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/http/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/http/server_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/http/server_test.py` & `hysteria2-2.4.3/hysteria2-go/app/internal/http/server_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/http/test.crt` & `hysteria2-2.4.3/hysteria2-go/app/internal/http/test.crt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/http/test.key` & `hysteria2-2.4.3/hysteria2-go/app/internal/http/test.key`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/redirect/getsockopt_linux_386.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/redirect/tcp_linux.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/redirect/tcp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/socks5/server_test.py` & `hysteria2-2.4.3/hysteria2-go/app/internal/socks5/server_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/tcp_linux.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/tcp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/tproxy/udp_linux.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/tproxy/udp_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/url/url.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/url/url.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/url/url_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/url/url_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/utils/bpsconv.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/utils/bpsconv_test.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/utils/bpsconv_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/utils/geoloader.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/utils/geoloader.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/utils/update.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/utils/update.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/internal/utils_test/mock.go` & `hysteria2-2.4.3/hysteria2-go/app/internal/utils_test/mock.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/app/misc/socks5_test.py` & `hysteria2-2.4.3/hysteria2-go/app/misc/socks5_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/client.go` & `hysteria2-2.4.3/hysteria2-go/core/client/client.go`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,16 @@
 		KeepAlivePeriod:                c.config.QUICConfig.KeepAlivePeriod,
 		DisablePathMTUDiscovery:        c.config.QUICConfig.DisablePathMTUDiscovery,
 		EnableDatagrams:                true,
 	}
 	// Prepare RoundTripper
 	var conn quic.EarlyConnection
 	rt := &http3.RoundTripper{
-		EnableDatagrams: true,
 		TLSClientConfig: tlsConfig,
-		QuicConfig:      quicConfig,
+		QUICConfig:      quicConfig,
 		Dial: func(ctx context.Context, _ string, tlsCfg *tls.Config, cfg *quic.Config) (quic.EarlyConnection, error) {
 			qc, err := quic.DialEarly(ctx, pktConn, c.config.ServerAddr, tlsCfg, cfg)
 			if err != nil {
 				return nil, err
 			}
 			conn = qc
 			return qc, nil
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/config.go` & `hysteria2-2.4.3/hysteria2-go/core/client/config.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/mock_udpIO.go` & `hysteria2-2.4.3/hysteria2-go/core/client/mock_udpIO.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/reconnect.go` & `hysteria2-2.4.3/hysteria2-go/core/client/reconnect.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/udp.go` & `hysteria2-2.4.3/hysteria2-go/core/client/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/client/udp_test.go` & `hysteria2-2.4.3/hysteria2-go/core/client/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/errors/errors.go` & `hysteria2-2.4.3/hysteria2-go/core/errors/errors.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/go.mod` & `hysteria2-2.4.3/hysteria2-go/core/go.mod`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 module github.com/apernet/hysteria/core
 
 go 1.21
 
 require (
-	github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d
+	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6
 	github.com/stretchr/testify v1.8.4
 	go.uber.org/goleak v1.2.1
 	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db
-	golang.org/x/time v0.4.0
+	golang.org/x/time v0.5.0
 )
 
 require (
 	github.com/davecgh/go-spew v1.1.1 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
 	github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 // indirect
 	github.com/kr/text v0.2.0 // indirect
 	github.com/niemeyer/pretty v0.0.0-20200227124842-a10e7caefd8e // indirect
 	github.com/onsi/ginkgo/v2 v2.9.5 // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
 	github.com/quic-go/qpack v0.4.0 // indirect
 	github.com/stretchr/objx v0.5.0 // indirect
-	go.uber.org/mock v0.3.0 // indirect
-	golang.org/x/crypto v0.17.0 // indirect
+	go.uber.org/mock v0.4.0 // indirect
+	golang.org/x/crypto v0.22.0 // indirect
 	golang.org/x/mod v0.12.0 // indirect
-	golang.org/x/net v0.17.0 // indirect
-	golang.org/x/sys v0.15.0 // indirect
+	golang.org/x/net v0.24.0 // indirect
+	golang.org/x/sys v0.19.0 // indirect
 	golang.org/x/text v0.14.0 // indirect
 	golang.org/x/tools v0.11.1 // indirect
-	google.golang.org/protobuf v1.28.1 // indirect
+	google.golang.org/protobuf v1.33.0 // indirect
 	gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f // indirect
 	gopkg.in/yaml.v3 v3.0.1 // indirect
 )
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/go.sum` & `hysteria2-2.4.3/hysteria2-go/core/go.sum`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d h1:K1DMSNtPcaZ/lihYmOHnjThNfUX7cD6SNuVRFnVLVmI=
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d/go.mod h1:4GInxO6ypy63J2NaO5rQx1wRp6K8YHI6zqLG+VswU6I=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
 github.com/chzyer/logex v1.1.10/go.mod h1:+Ywpsq7O8HXn0nuIou7OrIPyXbp3wmkHB+jjWRnGsAI=
 github.com/chzyer/readline v0.0.0-20180603132655-2972be24d48e/go.mod h1:nSuG5e5PlCu98SY8svDHJxuZscDgtXS6KTTbou5AhLI=
 github.com/chzyer/test v0.0.0-20180213035817-a1ea475d72b1/go.mod h1:Q3SI9o4m/ZMnBNeIyt5eFwwo7qiLfzFZmjNmxjkiQlU=
 github.com/creack/pty v1.1.9/go.mod h1:oKZEueFk5CKHvIhNR5MUki03XCEU+Q6VDXinZuGJ33E=
 github.com/davecgh/go-spew v1.1.0/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
 github.com/davecgh/go-spew v1.1.1/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/go-logr/logr v1.2.4 h1:g01GSCwiDw2xSZfjJ2/T9M+S6pFdcNtFYsp+Y43HYDQ=
 github.com/go-logr/logr v1.2.4/go.mod h1:jdQByPbusPIv2/zmleS9BjJVeZ6kBagPoEUsqbVz/1A=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 h1:tfuBGBXKqDEevZMzYi5KSi8KkcZtzBcTgAUUtapy0OI=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572/go.mod h1:9Pwr4B2jHnOSGXyyzV8ROjYa2ojvAY6HCGYYfMoC3Ls=
-github.com/golang/protobuf v1.5.0/go.mod h1:FsONVRAS9T7sI+LIUmWTfcYkHO4aIWwzhcaSAoJOfIk=
 github.com/golang/protobuf v1.5.3 h1:KhyjKVUg7Usr/dYsdSqoFveMYd5ko72D+zANwlG1mmg=
 github.com/golang/protobuf v1.5.3/go.mod h1:XVQd3VNwM+JqD3oG2Ue2ip4fOMUkwXdXDdiuN0vRsmY=
-github.com/google/go-cmp v0.5.5/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.9 h1:O2Tfq5qg4qc4AmwVlvv0oLiVAGB7enBSJ2x2DqQFi38=
 github.com/google/go-cmp v0.5.9/go.mod h1:17dUlkBOakJ0+DkrSSNjCkIjxS6bF9zb3elmeNGIjoY=
 github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 h1:yAJXTCF9TqKcTiHJAE8dj7HMvPfh66eeA2JYW7eFpSE=
 github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38/go.mod h1:kpwsk12EmLew5upagYY7GY0pfYCcupk39gWOCRROcvE=
 github.com/ianlancetaylor/demangle v0.0.0-20200824232613-28f6c0f3b639/go.mod h1:aSSvb/t6k1mPoxDqO4vJh6VOCGPwU4O0C2/Eqndh1Sc=
 github.com/kr/pty v1.1.1/go.mod h1:pFQYn66WHrOpPYNljwOMqo10TkYh1fy3cYio2l3bCsQ=
 github.com/kr/text v0.1.0/go.mod h1:4Jbv+DJW3UT/LiOwJeYQe1efqtUx/iVham/4vfdArNI=
@@ -41,36 +39,34 @@
 github.com/stretchr/testify v1.6.1/go.mod h1:6Fq8oRcR53rry900zMqJjRRixrwX3KX962/h/Wwjteg=
 github.com/stretchr/testify v1.7.1/go.mod h1:6Fq8oRcR53rry900zMqJjRRixrwX3KX962/h/Wwjteg=
 github.com/stretchr/testify v1.8.0/go.mod h1:yNjHg4UonilssWZ8iaSj1OCr/vHnekPRkoO+kdMU+MU=
 github.com/stretchr/testify v1.8.4 h1:CcVxjf3Q8PM0mHUKJCdn+eZZtm5yQwehR5yeSVQQcUk=
 github.com/stretchr/testify v1.8.4/go.mod h1:sz/lmYIOXD/1dqDmKjjqLyZ2RngseejIcXlSw2iwfAo=
 go.uber.org/goleak v1.2.1 h1:NBol2c7O1ZokfZ0LEU9K6Whx/KnwvepVetCUhtKja4A=
 go.uber.org/goleak v1.2.1/go.mod h1:qlT2yGI9QafXHhZZLxlSuNsMw3FFLxBr+tBRlmO1xH4=
-go.uber.org/mock v0.3.0 h1:3mUxI1No2/60yUYax92Pt8eNOEecx2D3lcXZh2NEZJo=
-go.uber.org/mock v0.3.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
-golang.org/x/crypto v0.17.0 h1:r8bRNjWL3GshPW3gkd+RpvzWrZAwPS49OmTGZ/uhM4k=
-golang.org/x/crypto v0.17.0/go.mod h1:gCAAfMLgwOJRpTjQ2zCCt2OcSfYMTeZVSRtQlPC7Nq4=
+go.uber.org/mock v0.4.0 h1:VcM4ZOtdbR4f6VXfiOpwpVJDL6lCReaZ6mw31wqh7KU=
+go.uber.org/mock v0.4.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
+golang.org/x/crypto v0.22.0 h1:g1v0xeRhjcugydODzvb3mEM9SQ0HGp9s/nh3COQ/C30=
+golang.org/x/crypto v0.22.0/go.mod h1:vr6Su+7cTlO45qkww3VDJlzDn0ctJvRgYbC2NvXHt+M=
 golang.org/x/exp v0.0.0-20221205204356-47842c84f3db h1:D/cFflL63o2KSLJIwjlcIt8PR064j/xsmdEJL/YvY/o=
 golang.org/x/exp v0.0.0-20221205204356-47842c84f3db/go.mod h1:CxIveKay+FTh1D0yPZemJVgC/95VzuuOLq5Qi4xnoYc=
 golang.org/x/mod v0.12.0 h1:rmsUpXtvNzj340zd98LZ4KntptpfRHwpFOHG188oHXc=
 golang.org/x/mod v0.12.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
-golang.org/x/net v0.17.0 h1:pVaXccu2ozPjCXewfr1S7xza/zcXTity9cCdXQYSjIM=
-golang.org/x/net v0.17.0/go.mod h1:NxSsAGuq816PNPmqtQdLE42eU2Fs7NoRIZrHJAlaCOE=
+golang.org/x/net v0.24.0 h1:1PcaxkF854Fu3+lvBIx5SYn9wRlBzzcnHZSiaFFAb0w=
+golang.org/x/net v0.24.0/go.mod h1:2Q7sJY5mzlzWjKtYUEXSlBWCdyaioyXzRB2RtU8KVE8=
 golang.org/x/sys v0.0.0-20191204072324-ce4227a45e2e/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
-golang.org/x/sys v0.15.0 h1:h48lPFYpsTvQJZF4EKyI4aLHaev3CxivZmv7yZig9pc=
-golang.org/x/sys v0.15.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/sys v0.19.0 h1:q5f1RH2jigJ1MoAWp2KTp3gm5zAGFUTarQZ5U386+4o=
+golang.org/x/sys v0.19.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
 golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
-golang.org/x/time v0.4.0 h1:Z81tqI5ddIoXDPvVQ7/7CC9TnLM7ubaFG2qXYd5BbYY=
-golang.org/x/time v0.4.0/go.mod h1:3BpzKBy/shNhVucY/MWOyx10tF3SFh9QdLuxbVysPQM=
+golang.org/x/time v0.5.0 h1:o7cqy6amK/52YcAKIPlM3a+Fpj35zvRj2TP+e1xFSfk=
+golang.org/x/time v0.5.0/go.mod h1:3BpzKBy/shNhVucY/MWOyx10tF3SFh9QdLuxbVysPQM=
 golang.org/x/tools v0.11.1 h1:ojD5zOW8+7dOGzdnNgersm8aPfcDjhMp12UfG93NIMc=
 golang.org/x/tools v0.11.1/go.mod h1:anzJrxPjNtfgiYQYirP2CPGzGLxrH2u2QBhn6Bf3qY8=
-golang.org/x/xerrors v0.0.0-20191204190536-9bdfabe68543/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
-google.golang.org/protobuf v1.26.0-rc.1/go.mod h1:jlhhOSvTdKEhbULTjvd4ARK9grFBp09yW+WbY/TyQbw=
-google.golang.org/protobuf v1.28.1 h1:d0NfwRgPtno5B1Wa6L2DAG+KivqkdutMf1UhdNx175w=
-google.golang.org/protobuf v1.28.1/go.mod h1:HV8QOd/L58Z+nl8r43ehVNZIU/HEI6OcFqwMG9pJV4I=
+google.golang.org/protobuf v1.33.0 h1:uNO2rsAINq/JlFpSdYEKIZ0uKD/R9cpdv0T+yoGwGmI=
+google.golang.org/protobuf v1.33.0/go.mod h1:c6P6GXX6sHbq/GpV6MGZEdwhWPcYBgnhAHhKbcUYpos=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f h1:BLraFXnmrev5lT+xlilqcH8XK9/i0At2xKjWk4p6zsU=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/yaml.v3 v3.0.0-20200313102051-9f266ea9e77c/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 gopkg.in/yaml.v3 v3.0.1 h1:fxVm/GzAzEWqLHuvctI91KS9hhNmmWOoWu0XTYJS7CA=
 gopkg.in/yaml.v3 v3.0.1/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bandwidth.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bandwidth_sampler.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/bbr_sender.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/packet_number_indexed_queue.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/ringbuffer.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/bbr/windowed_filter.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/brutal/brutal.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/brutal/brutal.go`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,27 @@
 }
 
 func (b *BrutalSender) HasPacingBudget(now time.Time) bool {
 	return b.pacer.Budget(now) >= b.maxDatagramSize
 }
 
 func (b *BrutalSender) CanSend(bytesInFlight congestion.ByteCount) bool {
-	return bytesInFlight < b.GetCongestionWindow()
+	return bytesInFlight <= b.GetCongestionWindow()
 }
 
 func (b *BrutalSender) GetCongestionWindow() congestion.ByteCount {
 	rtt := b.rttStats.SmoothedRTT()
 	if rtt <= 0 {
 		return 10240
 	}
-	return congestion.ByteCount(float64(b.bps) * rtt.Seconds() * congestionWindowMultiplier / b.ackRate)
+	cwnd := congestion.ByteCount(float64(b.bps) * rtt.Seconds() * congestionWindowMultiplier / b.ackRate)
+	if cwnd < b.maxDatagramSize {
+		cwnd = b.maxDatagramSize
+	}
+	return cwnd
 }
 
 func (b *BrutalSender) OnPacketSent(sentTime time.Time, bytesInFlight congestion.ByteCount,
 	packetNumber congestion.PacketNumber, bytes congestion.ByteCount, isRetransmittable bool,
 ) {
 	b.pacer.SentPacket(sentTime, bytes)
 }
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/congestion/common/pacer.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/congestion/common/pacer.go`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 package common
 
 import (
-	"math"
 	"time"
 
 	"github.com/apernet/quic-go/congestion"
 )
 
 const (
-	maxBurstPackets = 10
+	maxBurstPackets               = 10
+	maxBurstPacingDelayMultiplier = 4
 )
 
 // Pacer implements a token bucket pacing algorithm.
 type Pacer struct {
 	budgetAtLastSent congestion.ByteCount
 	maxDatagramSize  congestion.ByteCount
 	lastSentTime     time.Time
@@ -42,54 +42,38 @@
 	if p.lastSentTime.IsZero() {
 		return p.maxBurstSize()
 	}
 	budget := p.budgetAtLastSent + (p.getBandwidth()*congestion.ByteCount(now.Sub(p.lastSentTime).Nanoseconds()))/1e9
 	if budget < 0 { // protect against overflows
 		budget = congestion.ByteCount(1<<62 - 1)
 	}
-	return minByteCount(p.maxBurstSize(), budget)
+	return min(p.maxBurstSize(), budget)
 }
 
 func (p *Pacer) maxBurstSize() congestion.ByteCount {
-	return maxByteCount(
-		congestion.ByteCount((congestion.MinPacingDelay+time.Millisecond).Nanoseconds())*p.getBandwidth()/1e9,
+	return max(
+		congestion.ByteCount((maxBurstPacingDelayMultiplier*congestion.MinPacingDelay).Nanoseconds())*p.getBandwidth()/1e9,
 		maxBurstPackets*p.maxDatagramSize,
 	)
 }
 
 // TimeUntilSend returns when the next packet should be sent.
 // It returns the zero value of time.Time if a packet can be sent immediately.
 func (p *Pacer) TimeUntilSend() time.Time {
 	if p.budgetAtLastSent >= p.maxDatagramSize {
 		return time.Time{}
 	}
-	return p.lastSentTime.Add(maxDuration(
-		congestion.MinPacingDelay,
-		time.Duration(math.Ceil(float64(p.maxDatagramSize-p.budgetAtLastSent)*1e9/
-			float64(p.getBandwidth())))*time.Nanosecond,
-	))
+	diff := 1e9 * uint64(p.maxDatagramSize-p.budgetAtLastSent)
+	bw := uint64(p.getBandwidth())
+	// We might need to round up this value.
+	// Otherwise, we might have a budget (slightly) smaller than the datagram size when the timer expires.
+	d := diff / bw
+	// this is effectively a math.Ceil, but using only integer math
+	if diff%bw > 0 {
+		d++
+	}
+	return p.lastSentTime.Add(max(congestion.MinPacingDelay, time.Duration(d)*time.Nanosecond))
 }
 
 func (p *Pacer) SetMaxDatagramSize(s congestion.ByteCount) {
 	p.maxDatagramSize = s
 }
-
-func maxByteCount(a, b congestion.ByteCount) congestion.ByteCount {
-	if a < b {
-		return b
-	}
-	return a
-}
-
-func minByteCount(a, b congestion.ByteCount) congestion.ByteCount {
-	if a < b {
-		return a
-	}
-	return b
-}
-
-func maxDuration(a, b time.Duration) time.Duration {
-	if a > b {
-		return a
-	}
-	return b
-}
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/frag/frag.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/frag/frag_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/frag/frag_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/.mockery.yaml` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/.mockery.yaml`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/close_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/close_test.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 package integration_tests
 
 import (
 	"io"
+	"sync"
 	"testing"
 	"time"
 
 	"github.com/stretchr/testify/assert"
 	"github.com/stretchr/testify/mock"
 
 	"github.com/apernet/hysteria/core/client"
@@ -44,21 +45,22 @@
 	addr := "hi-and-goodbye:2333"
 
 	// Test close from client side:
 	// Client creates a connection, writes something, then closes it.
 	// Server outbound connection should write the same thing, then close.
 	sobConn := mocks.NewMockConn(t)
 	sobConnCh := make(chan struct{}) // For close signal only
+	sobConnChCloseFunc := sync.OnceFunc(func() { close(sobConnCh) })
 	sobConn.EXPECT().Read(mock.Anything).RunAndReturn(func(bs []byte) (int, error) {
 		<-sobConnCh
 		return 0, io.EOF
 	})
 	sobConn.EXPECT().Write([]byte("happy")).Return(5, nil)
 	sobConn.EXPECT().Close().RunAndReturn(func() error {
-		close(sobConnCh)
+		sobConnChCloseFunc()
 		return nil
 	})
 	serverOb.EXPECT().TCP(addr).Return(sobConn, nil).Once()
 	conn, err := c.TCP(addr)
 	assert.NoError(t, err)
 	_, err = conn.Write([]byte("happy"))
 	assert.NoError(t, err)
@@ -129,14 +131,15 @@
 	// 4 packets in total. The server should have one UDP session and receive all
 	// 4 packets. Then the UDP connection on the server side will receive a packet
 	// every 1 second, 4 packets in total. The client session should receive all
 	// 4 packets. Then the session will be idle for 3 seconds - should be enough
 	// to trigger the server's UDP idle timeout.
 	sobConn := mocks.NewMockUDPConn(t)
 	sobConnCh := make(chan []byte, 1)
+	sobConnChCloseFunc := sync.OnceFunc(func() { close(sobConnCh) })
 	sobConn.EXPECT().ReadFrom(mock.Anything).RunAndReturn(func(bs []byte) (int, string, error) {
 		d := <-sobConnCh
 		if d == nil {
 			return 0, "", io.EOF
 		} else {
 			return copy(bs, d), addr, nil
 		}
@@ -163,15 +166,15 @@
 		bs, rAddr, err := cu.Receive()
 		assert.NoError(t, err)
 		assert.Equal(t, "sad", string(bs))
 		assert.Equal(t, addr, rAddr)
 	}
 	// Now we wait for 3 seconds, the server should close the UDP session.
 	sobConn.EXPECT().Close().RunAndReturn(func() error {
-		close(sobConnCh)
+		sobConnChCloseFunc()
 		return nil
 	})
 	eventLogger.EXPECT().UDPError(mock.Anything, mock.Anything, uint32(1), nil).Once()
 	time.Sleep(3 * time.Second)
 }
 
 // TestClientServerClientShutdown tests whether the server can handle the client's shutdown correctly.
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/masq_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/masq_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 	assert.NoError(t, err)
 	defer s.Close()
 	go s.Serve()
 
 	// QUIC connection & RoundTripper
 	var conn quic.EarlyConnection
 	rt := &http3.RoundTripper{
-		EnableDatagrams: true,
 		TLSClientConfig: &tls.Config{
 			InsecureSkipVerify: true,
 		},
 		Dial: func(ctx context.Context, _ string, tlsCfg *tls.Config, cfg *quic.Config) (quic.EarlyConnection, error) {
 			qc, err := quic.DialAddrEarly(ctx, udpAddr.String(), tlsCfg, cfg)
 			if err != nil {
 				return nil, err
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Authenticator.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Conn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_EventLogger.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_Outbound.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_TrafficLogger.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/mocks/mock_UDPConn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/smoke_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/smoke_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/stress_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/stress_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/test.crt` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.crt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/test.key` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/test.key`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/trafficlogger_test.go`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 package integration_tests
 
 import (
 	"io"
+	"sync"
 	"testing"
 	"time"
 
 	"github.com/stretchr/testify/assert"
 	"github.com/stretchr/testify/mock"
 
 	"github.com/apernet/hysteria/core/client"
@@ -42,26 +43,27 @@
 	assert.NoError(t, err)
 	defer c.Close()
 
 	addr := "dontcare.cc:4455"
 
 	sobConn := mocks.NewMockConn(t)
 	sobConnCh := make(chan []byte, 1)
+	sobConnChCloseFunc := sync.OnceFunc(func() { close(sobConnCh) })
 	sobConn.EXPECT().Read(mock.Anything).RunAndReturn(func(bs []byte) (int, error) {
 		b := <-sobConnCh
 		if b == nil {
 			return 0, io.EOF
 		} else {
 			return copy(bs, b), nil
 		}
 	})
 	sobConn.EXPECT().Close().RunAndReturn(func() error {
-		close(sobConnCh)
+		sobConnChCloseFunc()
 		return nil
-	}).Once()
+	})
 	serverOb.EXPECT().TCP(addr).Return(sobConn, nil).Once()
 
 	conn, err := c.TCP(addr)
 	assert.NoError(t, err)
 
 	// Client reads from server
 	trafficLogger.EXPECT().Log("nobody", uint64(0), uint64(11)).Return(true).Once()
@@ -121,26 +123,27 @@
 	assert.NoError(t, err)
 	defer c.Close()
 
 	addr := "shady.org:43211"
 
 	sobConn := mocks.NewMockUDPConn(t)
 	sobConnCh := make(chan []byte, 1)
+	sobConnChCloseFunc := sync.OnceFunc(func() { close(sobConnCh) })
 	sobConn.EXPECT().ReadFrom(mock.Anything).RunAndReturn(func(bs []byte) (int, string, error) {
 		b := <-sobConnCh
 		if b == nil {
 			return 0, "", io.EOF
 		} else {
 			return copy(bs, b), addr, nil
 		}
 	})
 	sobConn.EXPECT().Close().RunAndReturn(func() error {
-		close(sobConnCh)
+		sobConnChCloseFunc()
 		return nil
-	}).Once()
+	})
 	serverOb.EXPECT().UDP(addr).Return(sobConn, nil).Once()
 
 	conn, err := c.UDP()
 	assert.NoError(t, err)
 
 	// Client writes to server
 	trafficLogger.EXPECT().Log("nobody", uint64(9), uint64(0)).Return(true).Once()
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/integration_tests/utils_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/integration_tests/utils_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/protocol/http.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/protocol/padding.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/padding.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/protocol/proxy.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/protocol/proxy_test.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/protocol/proxy_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/internal/utils/qstream.go` & `hysteria2-2.4.3/hysteria2-go/core/internal/utils/qstream.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/config.go` & `hysteria2-2.4.3/hysteria2-go/core/server/config.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/copy.go` & `hysteria2-2.4.3/hysteria2-go/core/server/copy.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/mock_UDPConn.go` & `hysteria2-2.4.3/hysteria2-go/core/server/mock_UDPConn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/mock_udpEventLogger.go` & `hysteria2-2.4.3/hysteria2-go/core/server/mock_udpEventLogger.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/mock_udpIO.go` & `hysteria2-2.4.3/hysteria2-go/core/server/mock_udpIO.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/server.go` & `hysteria2-2.4.3/hysteria2-go/core/server/server.go`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,16 @@
 	_ = s.config.Conn.Close()
 	return err
 }
 
 func (s *serverImpl) handleClient(conn quic.Connection) {
 	handler := newH3sHandler(s.config, conn)
 	h3s := http3.Server{
-		EnableDatagrams: true,
-		Handler:         handler,
-		StreamHijacker:  handler.ProxyStreamHijacker,
+		Handler:        handler,
+		StreamHijacker: handler.ProxyStreamHijacker,
 	}
 	err := h3s.ServeQUICConn(conn)
 	// If the client is authenticated, we need to log the disconnect event
 	if handler.authenticated && s.config.EventLogger != nil {
 		s.config.EventLogger.Disconnect(conn.RemoteAddr(), handler.authID, err)
 	}
 	_ = conn.CloseWithError(closeErrCodeOK, "")
@@ -176,15 +175,15 @@
 		}
 	} else {
 		// Not an auth request, pretend to be a normal HTTP server
 		h.masqHandler(w, r)
 	}
 }
 
-func (h *h3sHandler) ProxyStreamHijacker(ft http3.FrameType, conn quic.Connection, stream quic.Stream, err error) (bool, error) {
+func (h *h3sHandler) ProxyStreamHijacker(ft http3.FrameType, id quic.ConnectionTracingID, stream quic.Stream, err error) (bool, error) {
 	if err != nil || !h.authenticated {
 		return false, nil
 	}
 
 	// Wraps the stream with QStream, which handles Close() properly
 	stream = &utils.QStream{Stream: stream}
```

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/udp.go` & `hysteria2-2.4.3/hysteria2-go/core/server/udp.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/core/server/udp_test.go` & `hysteria2-2.4.3/hysteria2-go/core/server/udp_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/command.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/command.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/http.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/http_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/http_test.py` & `hysteria2-2.4.3/hysteria2-go/extras/auth/http_test.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/password_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/password_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/userpass.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/userpass.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/auth/userpass_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/auth/userpass_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/correctnet/correctnet.go` & `hysteria2-2.4.3/hysteria2-go/extras/correctnet/correctnet.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/go.mod` & `hysteria2-2.4.3/hysteria2-go/extras/go.mod`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 require (
 	github.com/apernet/hysteria/core v0.0.0-00010101000000-000000000000
 	github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6
 	github.com/hashicorp/golang-lru/v2 v2.0.5
 	github.com/miekg/dns v1.1.55
 	github.com/stretchr/testify v1.8.4
 	github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301
-	golang.org/x/crypto v0.17.0
-	golang.org/x/net v0.17.0
-	google.golang.org/protobuf v1.28.1
+	golang.org/x/crypto v0.22.0
+	golang.org/x/net v0.24.0
+	google.golang.org/protobuf v1.33.0
 )
 
 require (
-	github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d // indirect
+	github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 // indirect
 	github.com/davecgh/go-spew v1.1.1 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
 	github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 // indirect
 	github.com/onsi/ginkgo/v2 v2.9.5 // indirect
 	github.com/patrickmn/go-cache v2.1.0+incompatible // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
 	github.com/quic-go/qpack v0.4.0 // indirect
 	github.com/stretchr/objx v0.5.0 // indirect
 	github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf // indirect
-	go.uber.org/mock v0.3.0 // indirect
+	go.uber.org/mock v0.4.0 // indirect
 	golang.org/x/exp v0.0.0-20221205204356-47842c84f3db // indirect
 	golang.org/x/mod v0.12.0 // indirect
-	golang.org/x/sys v0.15.0 // indirect
+	golang.org/x/sys v0.19.0 // indirect
 	golang.org/x/text v0.14.0 // indirect
 	golang.org/x/tools v0.11.1 // indirect
 	gopkg.in/yaml.v3 v3.0.1 // indirect
 )
 
 replace github.com/apernet/hysteria/core => ../core
```

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/go.sum` & `hysteria2-2.4.3/hysteria2-go/extras/go.sum`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d h1:K1DMSNtPcaZ/lihYmOHnjThNfUX7cD6SNuVRFnVLVmI=
-github.com/apernet/quic-go v0.41.1-0.20240301003057-e18162de481d/go.mod h1:4GInxO6ypy63J2NaO5rQx1wRp6K8YHI6zqLG+VswU6I=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6 h1:ZfaQo52EyyhNCxfMNk64W1YHcIh+0rCkp3e0gR7BO5E=
+github.com/apernet/quic-go v0.43.1-0.20240429030958-51a0843014d6/go.mod h1:j3QaAM7sVJqptDQyIQRWA6mASCfuxoHJszn67JQh1GE=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6 h1:4NNbNM2Iq/k57qEu7WfL67UrbPq1uFWxW4qODCohi+0=
 github.com/babolivier/go-doh-client v0.0.0-20201028162107-a76cff4cb8b6/go.mod h1:J29hk+f9lJrblVIfiJOtTFk+OblBawmib4uz/VdKzlg=
 github.com/chzyer/logex v1.1.10/go.mod h1:+Ywpsq7O8HXn0nuIou7OrIPyXbp3wmkHB+jjWRnGsAI=
 github.com/chzyer/readline v0.0.0-20180603132655-2972be24d48e/go.mod h1:nSuG5e5PlCu98SY8svDHJxuZscDgtXS6KTTbou5AhLI=
 github.com/chzyer/test v0.0.0-20180213035817-a1ea475d72b1/go.mod h1:Q3SI9o4m/ZMnBNeIyt5eFwwo7qiLfzFZmjNmxjkiQlU=
 github.com/davecgh/go-spew v1.1.0/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
 github.com/davecgh/go-spew v1.1.1/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/go-logr/logr v1.2.4 h1:g01GSCwiDw2xSZfjJ2/T9M+S6pFdcNtFYsp+Y43HYDQ=
 github.com/go-logr/logr v1.2.4/go.mod h1:jdQByPbusPIv2/zmleS9BjJVeZ6kBagPoEUsqbVz/1A=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 h1:tfuBGBXKqDEevZMzYi5KSi8KkcZtzBcTgAUUtapy0OI=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572/go.mod h1:9Pwr4B2jHnOSGXyyzV8ROjYa2ojvAY6HCGYYfMoC3Ls=
-github.com/golang/protobuf v1.5.0/go.mod h1:FsONVRAS9T7sI+LIUmWTfcYkHO4aIWwzhcaSAoJOfIk=
 github.com/golang/protobuf v1.5.3 h1:KhyjKVUg7Usr/dYsdSqoFveMYd5ko72D+zANwlG1mmg=
 github.com/golang/protobuf v1.5.3/go.mod h1:XVQd3VNwM+JqD3oG2Ue2ip4fOMUkwXdXDdiuN0vRsmY=
-github.com/google/go-cmp v0.5.5/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.5.9 h1:O2Tfq5qg4qc4AmwVlvv0oLiVAGB7enBSJ2x2DqQFi38=
 github.com/google/go-cmp v0.5.9/go.mod h1:17dUlkBOakJ0+DkrSSNjCkIjxS6bF9zb3elmeNGIjoY=
 github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38 h1:yAJXTCF9TqKcTiHJAE8dj7HMvPfh66eeA2JYW7eFpSE=
 github.com/google/pprof v0.0.0-20210407192527-94a9f03dee38/go.mod h1:kpwsk12EmLew5upagYY7GY0pfYCcupk39gWOCRROcvE=
 github.com/hashicorp/golang-lru/v2 v2.0.5 h1:wW7h1TG88eUIJ2i69gaE3uNVtEPIagzhGvHgwfx2Vm4=
 github.com/hashicorp/golang-lru/v2 v2.0.5/go.mod h1:QeFd9opnmA6QUJc5vARoKUSoFhyfM2/ZepoAG6RGpeM=
 github.com/ianlancetaylor/demangle v0.0.0-20200824232613-28f6c0f3b639/go.mod h1:aSSvb/t6k1mPoxDqO4vJh6VOCGPwU4O0C2/Eqndh1Sc=
@@ -52,65 +50,65 @@
 github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf h1:7PflaKRtU4np/epFxRXlFhlzLXZzKFrH5/I4so5Ove0=
 github.com/txthinking/runnergroup v0.0.0-20210608031112-152c7c4432bf/go.mod h1:CLUSJbazqETbaR+i0YAhXBICV9TrKH93pziccMhmhpM=
 github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301 h1:d/Wr/Vl/wiJHc3AHYbYs5I3PucJvRuw3SvbmlIRf+oM=
 github.com/txthinking/socks5 v0.0.0-20230325130024-4230056ae301/go.mod h1:ntmMHL/xPq1WLeKiw8p/eRATaae6PiVRNipHFJxI8PM=
 github.com/yuin/goldmark v1.4.13/go.mod h1:6yULJ656Px+3vBD8DxQVa3kxgyrAnzto9xy5taEt/CY=
 go.uber.org/goleak v1.2.1 h1:NBol2c7O1ZokfZ0LEU9K6Whx/KnwvepVetCUhtKja4A=
 go.uber.org/goleak v1.2.1/go.mod h1:qlT2yGI9QafXHhZZLxlSuNsMw3FFLxBr+tBRlmO1xH4=
-go.uber.org/mock v0.3.0 h1:3mUxI1No2/60yUYax92Pt8eNOEecx2D3lcXZh2NEZJo=
-go.uber.org/mock v0.3.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
+go.uber.org/mock v0.4.0 h1:VcM4ZOtdbR4f6VXfiOpwpVJDL6lCReaZ6mw31wqh7KU=
+go.uber.org/mock v0.4.0/go.mod h1:a6FSlNadKUHUa9IP5Vyt1zh4fC7uAwxMutEAscFbkZc=
 golang.org/x/crypto v0.0.0-20190308221718-c2843e01d9a2/go.mod h1:djNgcEr1/C05ACkg1iLfiJU5Ep61QUkGW8qpdssI0+w=
 golang.org/x/crypto v0.0.0-20210921155107-089bfa567519/go.mod h1:GvvjBRRGRdwPK5ydBHafDWAxML/pGHZbMvKqRZ5+Abc=
-golang.org/x/crypto v0.17.0 h1:r8bRNjWL3GshPW3gkd+RpvzWrZAwPS49OmTGZ/uhM4k=
-golang.org/x/crypto v0.17.0/go.mod h1:gCAAfMLgwOJRpTjQ2zCCt2OcSfYMTeZVSRtQlPC7Nq4=
+golang.org/x/crypto v0.22.0 h1:g1v0xeRhjcugydODzvb3mEM9SQ0HGp9s/nh3COQ/C30=
+golang.org/x/crypto v0.22.0/go.mod h1:vr6Su+7cTlO45qkww3VDJlzDn0ctJvRgYbC2NvXHt+M=
 golang.org/x/exp v0.0.0-20221205204356-47842c84f3db h1:D/cFflL63o2KSLJIwjlcIt8PR064j/xsmdEJL/YvY/o=
 golang.org/x/exp v0.0.0-20221205204356-47842c84f3db/go.mod h1:CxIveKay+FTh1D0yPZemJVgC/95VzuuOLq5Qi4xnoYc=
 golang.org/x/mod v0.6.0-dev.0.20220419223038-86c51ed26bb4/go.mod h1:jJ57K6gSWd91VN4djpZkiMVwK6gcyfeH4XE8wZrZaV4=
 golang.org/x/mod v0.7.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
 golang.org/x/mod v0.12.0 h1:rmsUpXtvNzj340zd98LZ4KntptpfRHwpFOHG188oHXc=
 golang.org/x/mod v0.12.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
 golang.org/x/net v0.0.0-20190620200207-3b0461eec859/go.mod h1:z5CRVTTTmAJ677TzLLGU+0bjPO0LkuOLi4/5GtJWs/s=
 golang.org/x/net v0.0.0-20210226172049-e18ecbb05110/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20220722155237-a158d28d115b/go.mod h1:XRhObCWvk6IyKnWLug+ECip1KBveYUHfp+8e9klMJ9c=
 golang.org/x/net v0.2.0/go.mod h1:KqCZLdyyvdV855qA2rE3GC2aiw5xGR5TEjj8smXukLY=
-golang.org/x/net v0.17.0 h1:pVaXccu2ozPjCXewfr1S7xza/zcXTity9cCdXQYSjIM=
-golang.org/x/net v0.17.0/go.mod h1:NxSsAGuq816PNPmqtQdLE42eU2Fs7NoRIZrHJAlaCOE=
+golang.org/x/net v0.24.0 h1:1PcaxkF854Fu3+lvBIx5SYn9wRlBzzcnHZSiaFFAb0w=
+golang.org/x/net v0.24.0/go.mod h1:2Q7sJY5mzlzWjKtYUEXSlBWCdyaioyXzRB2RtU8KVE8=
 golang.org/x/sync v0.0.0-20190423024810-112230192c58/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
 golang.org/x/sync v0.0.0-20220722155255-886fb9371eb4/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
 golang.org/x/sync v0.1.0/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
 golang.org/x/sync v0.3.0 h1:ftCYgMx6zT/asHUrPw8BLLscYtGznsLAnjq5RH9P66E=
 golang.org/x/sync v0.3.0/go.mod h1:FU7BRWz2tNW+3quACPkgCx/L+uEAv1htQ0V83Z9Rj+Y=
 golang.org/x/sys v0.0.0-20190215142949-d0b11bdaac8a/go.mod h1:STP8DvDyc/dI5b8T5hshtkjS+E42TnysNCUPdjciGhY=
 golang.org/x/sys v0.0.0-20191204072324-ce4227a45e2e/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20201119102817-f84b799fce68/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20210615035016-665e8c7367d1/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220520151302-bc2c85ada10a/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220722155257-8c9f86f7a55f/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.2.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.15.0 h1:h48lPFYpsTvQJZF4EKyI4aLHaev3CxivZmv7yZig9pc=
-golang.org/x/sys v0.15.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/sys v0.19.0 h1:q5f1RH2jigJ1MoAWp2KTp3gm5zAGFUTarQZ5U386+4o=
+golang.org/x/sys v0.19.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/term v0.0.0-20201126162022-7de9c90e9dd1/go.mod h1:bj7SfCRtBDWHUb9snDiAeCFNEtKQo2Wmx5Cou7ajbmo=
 golang.org/x/term v0.0.0-20210927222741-03fcf44c2211/go.mod h1:jbD1KX2456YbFQfuXm/mYQcufACuNUgVhRMnK/tPxf8=
 golang.org/x/term v0.2.0/go.mod h1:TVmDHMZPmdnySmBfhjOoOdhjzdE1h4u1VwSiw2l1Nuc=
 golang.org/x/text v0.3.0/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.3/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
 golang.org/x/text v0.3.7/go.mod h1:u+2+/6zg+i71rQMx5EYifcz6MCKuco9NR6JIITiCfzQ=
 golang.org/x/text v0.4.0/go.mod h1:mrYo+phRRbMaCq/xk9113O4dZlRixOauAjOtrjsXDZ8=
 golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
 golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
+golang.org/x/time v0.5.0 h1:o7cqy6amK/52YcAKIPlM3a+Fpj35zvRj2TP+e1xFSfk=
+golang.org/x/time v0.5.0/go.mod h1:3BpzKBy/shNhVucY/MWOyx10tF3SFh9QdLuxbVysPQM=
 golang.org/x/tools v0.0.0-20180917221912-90fa682c2a6e/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20191119224855-298f0cb1881e/go.mod h1:b+2E5dAYhXwXZwtnZ6UAqBI28+e2cm9otk0dWdXHAEo=
 golang.org/x/tools v0.1.12/go.mod h1:hNGJHUnrk76NpqgfD5Aqm5Crs+Hm0VOH/i9J2+nxYbc=
 golang.org/x/tools v0.3.0/go.mod h1:/rWhSS2+zyEVwoJf8YAX6L2f0ntZ7Kn/mGgAWcipA5k=
 golang.org/x/tools v0.11.1 h1:ojD5zOW8+7dOGzdnNgersm8aPfcDjhMp12UfG93NIMc=
 golang.org/x/tools v0.11.1/go.mod h1:anzJrxPjNtfgiYQYirP2CPGzGLxrH2u2QBhn6Bf3qY8=
 golang.org/x/xerrors v0.0.0-20190717185122-a985d3407aa7/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
-golang.org/x/xerrors v0.0.0-20191204190536-9bdfabe68543/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
-google.golang.org/protobuf v1.26.0-rc.1/go.mod h1:jlhhOSvTdKEhbULTjvd4ARK9grFBp09yW+WbY/TyQbw=
-google.golang.org/protobuf v1.28.1 h1:d0NfwRgPtno5B1Wa6L2DAG+KivqkdutMf1UhdNx175w=
-google.golang.org/protobuf v1.28.1/go.mod h1:HV8QOd/L58Z+nl8r43ehVNZIU/HEI6OcFqwMG9pJV4I=
+google.golang.org/protobuf v1.33.0 h1:uNO2rsAINq/JlFpSdYEKIZ0uKD/R9cpdv0T+yoGwGmI=
+google.golang.org/protobuf v1.33.0/go.mod h1:c6P6GXX6sHbq/GpV6MGZEdwhWPcYBgnhAHhKbcUYpos=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f h1:BLraFXnmrev5lT+xlilqcH8XK9/i0At2xKjWk4p6zsU=
 gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/yaml.v3 v3.0.0-20200313102051-9f266ea9e77c/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 gopkg.in/yaml.v3 v3.0.1 h1:fxVm/GzAzEWqLHuvctI91KS9hhNmmWOoWu0XTYJS7CA=
 gopkg.in/yaml.v3 v3.0.1/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
```

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/masq/server.go` & `hysteria2-2.4.3/hysteria2-go/extras/masq/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/obfs/conn.go` & `hysteria2-2.4.3/hysteria2-go/extras/obfs/conn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/obfs/salamander.go` & `hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/obfs/salamander_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/obfs/salamander_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/compile.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile.go`

 * *Files 15% similar despite different names*

```diff
@@ -37,23 +37,24 @@
 	Match(host HostInfo, proto Protocol, port uint16) (O, net.IP)
 }
 
 type compiledRule[O Outbound] struct {
 	Outbound      O
 	HostMatcher   hostMatcher
 	Protocol      Protocol
-	Port          uint16
+	StartPort     uint16
+	EndPort       uint16
 	HijackAddress net.IP
 }
 
 func (r *compiledRule[O]) Match(host HostInfo, proto Protocol, port uint16) bool {
 	if r.Protocol != ProtocolBoth && r.Protocol != proto {
 		return false
 	}
-	if r.Port != 0 && r.Port != port {
+	if r.StartPort != 0 && (port < r.StartPort || port > r.EndPort) {
 		return false
 	}
 	return r.HostMatcher.Match(host)
 }
 
 type matchResult[O Outbound] struct {
 	Outbound      O
@@ -96,43 +97,42 @@
 type GeoLoader interface {
 	LoadGeoIP() (map[string]*v2geo.GeoIP, error)
 	LoadGeoSite() (map[string]*v2geo.GeoSite, error)
 }
 
 // Compile compiles TextRules into a CompiledRuleSet.
 // Names in the outbounds map MUST be in all lower case.
-// geoipFunc is a function that returns the GeoIP database needed by the GeoIP matcher.
-// It will be called every time a GeoIP matcher is used during compilation, but won't
-// be called if there is no GeoIP rule. We use a function here so that database loading
-// is on-demand (only required if used by rules).
+// We want on-demand loading of GeoIP/GeoSite databases, so instead of passing the
+// databases directly, we use a GeoLoader interface to load them only when needed
+// by at least one rule.
 func Compile[O Outbound](rules []TextRule, outbounds map[string]O,
 	cacheSize int, geoLoader GeoLoader,
 ) (CompiledRuleSet[O], error) {
 	compiledRules := make([]compiledRule[O], len(rules))
 	for i, rule := range rules {
 		outbound, ok := outbounds[strings.ToLower(rule.Outbound)]
 		if !ok {
 			return nil, &CompilationError{rule.LineNum, fmt.Sprintf("outbound %s not found", rule.Outbound)}
 		}
 		hm, errStr := compileHostMatcher(rule.Address, geoLoader)
 		if errStr != "" {
 			return nil, &CompilationError{rule.LineNum, errStr}
 		}
-		proto, port, ok := parseProtoPort(rule.ProtoPort)
+		proto, startPort, endPort, ok := parseProtoPort(rule.ProtoPort)
 		if !ok {
 			return nil, &CompilationError{rule.LineNum, fmt.Sprintf("invalid protocol/port: %s", rule.ProtoPort)}
 		}
 		var hijackAddress net.IP
 		if rule.HijackAddress != "" {
 			hijackAddress = net.ParseIP(rule.HijackAddress)
 			if hijackAddress == nil {
 				return nil, &CompilationError{rule.LineNum, fmt.Sprintf("invalid hijack address (must be an IP address): %s", rule.HijackAddress)}
 			}
 		}
-		compiledRules[i] = compiledRule[O]{outbound, hm, proto, port, hijackAddress}
+		compiledRules[i] = compiledRule[O]{outbound, hm, proto, startPort, endPort, hijackAddress}
 	}
 	cache, err := lru.New[string, matchResult[O]](cacheSize)
 	if err != nil {
 		return nil, err
 	}
 	return &compiledRuleSetImpl[O]{compiledRules, cache}, nil
 }
@@ -145,52 +145,71 @@
 //	proto
 //	*/port
 //	*/*
 //	*
 //	[empty] (same as *)
 //
 // proto must be either "tcp" or "udp", case-insensitive.
-func parseProtoPort(protoPort string) (Protocol, uint16, bool) {
+func parseProtoPort(protoPort string) (Protocol, uint16, uint16, bool) {
 	protoPort = strings.ToLower(protoPort)
 	if protoPort == "" || protoPort == "*" || protoPort == "*/*" {
-		return ProtocolBoth, 0, true
+		return ProtocolBoth, 0, 0, true
 	}
 	parts := strings.SplitN(protoPort, "/", 2)
 	if len(parts) == 1 {
 		// No port, only protocol
 		switch parts[0] {
 		case "tcp":
-			return ProtocolTCP, 0, true
+			return ProtocolTCP, 0, 0, true
 		case "udp":
-			return ProtocolUDP, 0, true
+			return ProtocolUDP, 0, 0, true
 		default:
-			return ProtocolBoth, 0, false
+			return ProtocolBoth, 0, 0, false
 		}
 	} else {
 		// Both protocol and port
 		var proto Protocol
-		var port uint16
+		var startPort, endPort uint16
 		switch parts[0] {
 		case "tcp":
 			proto = ProtocolTCP
 		case "udp":
 			proto = ProtocolUDP
 		case "*":
 			proto = ProtocolBoth
 		default:
-			return ProtocolBoth, 0, false
+			return ProtocolBoth, 0, 0, false
 		}
 		if parts[1] != "*" {
-			p64, err := strconv.ParseUint(parts[1], 10, 16)
-			if err != nil {
-				return ProtocolBoth, 0, false
+			// We allow either a single port or a range (e.g. "1000-2000")
+			ports := strings.SplitN(strings.TrimSpace(parts[1]), "-", 2)
+			if len(ports) == 1 {
+				p64, err := strconv.ParseUint(parts[1], 10, 16)
+				if err != nil {
+					return ProtocolBoth, 0, 0, false
+				}
+				startPort = uint16(p64)
+				endPort = startPort
+			} else {
+				p64, err := strconv.ParseUint(ports[0], 10, 16)
+				if err != nil {
+					return ProtocolBoth, 0, 0, false
+				}
+				startPort = uint16(p64)
+				p64, err = strconv.ParseUint(ports[1], 10, 16)
+				if err != nil {
+					return ProtocolBoth, 0, 0, false
+				}
+				endPort = uint16(p64)
+				if startPort > endPort {
+					return ProtocolBoth, 0, 0, false
+				}
 			}
-			port = uint16(p64)
 		}
-		return proto, port, true
+		return proto, startPort, endPort, true
 	}
 }
 
 func compileHostMatcher(addr string, geoLoader GeoLoader) (hostMatcher, string) {
 	addr = strings.ToLower(addr) // Normalize to lower case
 	if addr == "*" || addr == "all" {
 		// Match all hosts
```

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/compile_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/compile_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 }
 
 func (l *testGeoLoader) LoadGeoSite() (map[string]*v2geo.GeoSite, error) {
 	return v2geo.LoadGeoSite("v2geo/geosite.dat")
 }
 
 func TestCompile(t *testing.T) {
-	ob1, ob2, ob3, ob4, ob5 := 1, 2, 3, 4, 5
+	ob1, ob2, ob3, ob4, ob5, ob6 := 1, 2, 3, 4, 5, 6
 	rules := []TextRule{
 		{
 			Outbound:      "ob1",
 			Address:       "1.2.3.4",
 			ProtoPort:     "",
 			HijackAddress: "",
 		},
@@ -86,21 +86,28 @@
 		},
 		{
 			Outbound:      "ob5",
 			Address:       "suffix:microsoft.com",
 			ProtoPort:     "*/*",
 			HijackAddress: "",
 		},
+		{
+			Outbound:      "ob6",
+			Address:       "all",
+			ProtoPort:     "tcp/6881-6889",
+			HijackAddress: "",
+		},
 	}
 	comp, err := Compile[int](rules, map[string]int{
 		"ob1": ob1,
 		"ob2": ob2,
 		"ob3": ob3,
 		"ob4": ob4,
 		"ob5": ob5,
+		"ob6": ob6,
 	}, 100, &testGeoLoader{})
 	assert.NoError(t, err)
 
 	tests := []struct {
 		host         HostInfo
 		proto        Protocol
 		port         uint16
@@ -238,21 +245,46 @@
 				Name: "fakemicrosoft.com",
 			},
 			proto:        ProtocolTCP,
 			port:         5000,
 			wantOutbound: 0, // no match default
 			wantIP:       nil,
 		},
+		{
+			host: HostInfo{
+				IPv4: net.ParseIP("223.1.1.1"),
+			},
+			proto:        ProtocolTCP,
+			port:         6883,
+			wantOutbound: ob6, // match range port rule 6881-6889
+			wantIP:       nil,
+		},
 	}
 
 	for _, test := range tests {
 		gotOutbound, gotIP := comp.Match(test.host, test.proto, test.port)
 		assert.Equal(t, test.wantOutbound, gotOutbound)
 		assert.Equal(t, test.wantIP, gotIP)
 	}
+
+	// Test Invalid Port Range Rule
+	eb1 := 1
+	invalidRules := []TextRule{
+		{
+			Outbound:      "eb1",
+			Address:       "1.1.2.0/24",
+			ProtoPort:     "*/3-1",
+			HijackAddress: "",
+		},
+	}
+
+	_, err = Compile[int](invalidRules, map[string]int{
+		"eb1": eb1,
+	}, 100, &testGeoLoader{})
+	assert.Error(t, err)
 }
 
 func Test_parseGeoSiteName(t *testing.T) {
 	tests := []struct {
 		name  string
 		s     string
 		want  string
```

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/matchers_v2geo_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/parse.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/parse_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/parse_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geoip.dat`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/geosite.dat`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/load.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/load_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.pb.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl/v2geo/v2geo.proto`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/acl_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/acl_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_https.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_https.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_standard.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_standard.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/dns_system.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/dns_system.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/interface.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/interface_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/interface_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_PluggableOutbound.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/mock_UDPConn.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/mock_UDPConn.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct_linux.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_linux.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_direct_others.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_direct_others.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_http.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/ob_socks5.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/ob_socks5.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/client.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/client.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/protocol.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/protocol_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/protocol_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest/server.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest/server.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/speedtest.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/speedtest.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/utils.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/outbounds/utils_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/outbounds/utils_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/trafficlogger/http.go` & `hysteria2-2.4.3/hysteria2-go/extras/trafficlogger/http.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/addr.go` & `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/addr_test.go` & `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/addr_test.go`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/extras/transport/udphop/conn.go` & `hysteria2-2.4.3/hysteria2-go/extras/transport/udphop/conn.go`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 type udpPacket struct {
 	Buf  []byte
 	N    int
 	Addr net.Addr
 	Err  error
 }
 
-type ListenUDPFunc func() (net.PacketConn, error)
+type ListenUDPFunc = func() (net.PacketConn, error)
 
 func NewUDPHopPacketConn(addr *UDPHopAddr, hopInterval time.Duration, listenUDPFunc ListenUDPFunc) (net.PacketConn, error) {
 	if hopInterval == 0 {
 		hopInterval = defaultHopInterval
 	} else if hopInterval < 5*time.Second {
 		return nil, errors.New("hop interval must be at least 5 seconds")
 	}
```

### Comparing `hysteria2-2.3.0/hysteria2-go/go.work.sum` & `hysteria2-2.4.3/hysteria2-go/go.work.sum`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 dmitri.shuralyov.com/service/change v0.0.0-20181023043359-a85b471d5412 h1:GvWw74lx5noHocd+f6HBMXK6DuggBB1dhVkuGZbv7qM=
 dmitri.shuralyov.com/service/change v0.0.0-20181023043359-a85b471d5412/go.mod h1:a1inKt/atXimZ4Mv927x+r7UpyzRUf4emIoiiSC2TN4=
 dmitri.shuralyov.com/state v0.0.0-20180228185332-28bcc343414c h1:ivON6cwHK1OH26MZyWDCnbTRZZf0IhNsENoNAKFS1g4=
 dmitri.shuralyov.com/state v0.0.0-20180228185332-28bcc343414c/go.mod h1:0PRwlb0D6DFvNNtx+9ybjezNCa8XF0xaYcETyp6rHWU=
 git.apache.org/thrift.git v0.0.0-20180902110319-2566ecd5d999 h1:OR8VhtwhcAI3U48/rzBsVOuHi0zDPzYI1xASVcdSgR8=
 git.apache.org/thrift.git v0.0.0-20180902110319-2566ecd5d999/go.mod h1:fPE2ZNJGynbRyZ4dJvy6G277gSllfV2HJqblrnkyeyg=
 github.com/BurntSushi/toml v0.3.1 h1:WXkYYl6Yr3qBf1K79EBnL4mak0OimBfB0XUf9Vl28OQ=
+github.com/BurntSushi/toml v1.2.1 h1:9F2/+DoOYIOksmaJFPw1tGFy1eDnIJXg+UHjuD8lTak=
+github.com/BurntSushi/toml v1.2.1/go.mod h1:CxXYINrC8qIiEnFrOxCa7Jy5BFHlXnUU2pbicEuybxQ=
 github.com/BurntSushi/xgb v0.0.0-20160522181843-27f122750802 h1:1BDTz0u9nC3//pOCMdNH+CiXJVYJh5UQNCOBG7jbELc=
 github.com/anmitsu/go-shlex v0.0.0-20161002113705-648efa622239 h1:kFOfPq6dUM1hTo4JG6LR5AXSUEsOjtdm0kw0FtQtMJA=
 github.com/anmitsu/go-shlex v0.0.0-20161002113705-648efa622239/go.mod h1:2FmKhYUyUczH0OGQWaF5ceTx0UBShxjsH6f8oGKYe2c=
 github.com/armon/go-metrics v0.4.0 h1:yCQqn7dwca4ITXb+CbubHmedzaQYHhNhrEXLYUeEe8Q=
 github.com/armon/go-metrics v0.4.0/go.mod h1:E6amYzXo6aW1tqzoZGT755KkbgrJsSdpwZ+3JqfkOG4=
 github.com/beorn7/perks v0.0.0-20180321164747-3a771d992973 h1:xJ4a3vCFaGF/jqvzLMYoU8P317H5OQ+Via4RmuPwCS0=
 github.com/beorn7/perks v0.0.0-20180321164747-3a771d992973/go.mod h1:Dwedo/Wpr24TaqPxmxbtue+5NUziq4I4S80YR8gNf3Q=
@@ -49,14 +51,16 @@
 github.com/coreos/go-systemd v0.0.0-20181012123002-c6f51f82210d/go.mod h1:F5haX7vjVVG0kc13fIWeqUViNPyEJxv/OmvnBo0Yme4=
 github.com/coreos/go-systemd/v22 v22.3.2 h1:D9/bQk5vlXQFZ6Kwuu6zaiXJ9oTPe68++AzAJc1DzSI=
 github.com/coreos/go-systemd/v22 v22.3.2/go.mod h1:Y58oyj3AT4RCenI/lSvhwexgC+NSVTIJ3seZv2GcEnc=
 github.com/cpuguy83/go-md2man/v2 v2.0.2 h1:p1EgwI/C7NhT0JmVkwCD2ZBK8j4aeHQX2pMHHBfMQ6w=
 github.com/creack/pty v1.1.9 h1:uDmaGzcdjhF4i/plgjmEsriH11Y0o7RKapEf/LDaM3w=
 github.com/dustin/go-humanize v1.0.0 h1:VSnTsYCnlFHaM2/igO1h6X3HA71jcobQuxemgkq4zYo=
 github.com/dustin/go-humanize v1.0.0/go.mod h1:HtrtbFcZ19U5GC7JDqmcUSB87Iq5E25KnS6fMYU6eOk=
+github.com/dvyukov/go-fuzz v0.0.0-20210103155950-6a8e9d1f2415 h1:q1oJaUPdmpDm/VyXosjgPgr6wS7c5iV2p0PwJD73bUI=
+github.com/dvyukov/go-fuzz v0.0.0-20210103155950-6a8e9d1f2415/go.mod h1:11Gm+ccJnvAhCNLlf5+cS9KjtbaD5I5zaZpFMsTHWTw=
 github.com/envoyproxy/go-control-plane v0.9.9-0.20201210154907-fd9021fe5dad h1:EmNYJhPYy0pOFjCx2PrgtaBXmee0iUX9hLlxE1xHOJE=
 github.com/envoyproxy/protoc-gen-validate v0.1.0 h1:EQciDnbrYxy13PgWoY8AqoxGiPrpgBZ1R8UNe3ddc+A=
 github.com/fatih/color v1.13.0 h1:8LOYc1KYPPmyKMuN8QV2DNRWNbLo6LZ0iLs8+mlH53w=
 github.com/fatih/color v1.13.0/go.mod h1:kLAiJbzzSOZDVNGyDpeOxJ47H46qBXwg5ILebYFFOfk=
 github.com/flynn/go-shlex v0.0.0-20150515145356-3f9db97f8568 h1:BHsljHzVlRcyQhjrss6TZTdY2VfCqZPbv5k3iBFa2ZQ=
 github.com/flynn/go-shlex v0.0.0-20150515145356-3f9db97f8568/go.mod h1:xEzjJPgXI435gkrCt3MPfRiAkVrwSbHsst4LCFVfpJc=
 github.com/francoispqt/gojay v1.2.13 h1:d2m3sFjloqoIUQU3TsHBgj6qg/BVGlTBeHDUmyJnXKk=
@@ -150,15 +154,19 @@
 github.com/neelance/astrewrite v0.0.0-20160511093645-99348263ae86 h1:D6paGObi5Wud7xg83MaEFyjxQB1W5bz5d0IFppr+ymk=
 github.com/neelance/astrewrite v0.0.0-20160511093645-99348263ae86/go.mod h1:kHJEU3ofeGjhHklVoIGuVj85JJwZ6kWPaJwCIxgnFmo=
 github.com/neelance/sourcemap v0.0.0-20151028013722-8c68805598ab h1:eFXv9Nu1lGbrNbj619aWwZfVF5HBrm9Plte8aNptuTI=
 github.com/neelance/sourcemap v0.0.0-20151028013722-8c68805598ab/go.mod h1:Qr6/a/Q4r9LP1IltGz7tA7iOK1WonHEYhu1HRBA7ZiM=
 github.com/openzipkin/zipkin-go v0.1.1 h1:A/ADD6HaPnAKj3yS7HjGHRK77qi41Hi0DirOOIQAeIw=
 github.com/openzipkin/zipkin-go v0.1.1/go.mod h1:NtoC/o8u3JlF1lSlyPNswIbeQH9bJTmOf0Erfk+hxe8=
 github.com/pkg/sftp v1.13.1 h1:I2qBYMChEhIjOgazfJmV3/mZM256btk6wkCDRmW7JYs=
+github.com/prometheus/client_golang v0.8.0/go.mod h1:7SWBe2y4D6OKWSNQJUaRYU/AaXPKyh/dDVn+NZz0KFw=
+github.com/prometheus/client_model v0.0.0-20180712105110-5c3871d89910/go.mod h1:MbSGuTsp3dbXC40dX6PRTWyKYBIrTGTE9sqQNg2J8bo=
 github.com/prometheus/client_model v0.0.0-20190812154241-14fe0d1b01d4 h1:gQz4mCbXsO+nc9n1hCxHcGA3Zx3Eo+UHZoInFGUIXNM=
+github.com/prometheus/common v0.0.0-20180801064454-c7de2306084e/go.mod h1:daVV7qP5qjZbuso7PdcryaAu0sAZbrN9i7WWcTMWvro=
+github.com/prometheus/procfs v0.0.0-20180725123919-05ee40e3a273/go.mod h1:c3At6R/oaqEKCNdg8wHV1ftS6bRYblBhIjjI8uT2IGk=
 github.com/russross/blackfriday v1.5.2 h1:HyvC0ARfnZBqnXwABFeSZHpKvJHJJfPz81GNueLj0oo=
 github.com/russross/blackfriday v1.5.2/go.mod h1:JO/DiYxRf+HjHt06OyowR9PTA263kcR/rfWxYHBV53g=
 github.com/russross/blackfriday/v2 v2.1.0 h1:JIOH55/0cWyOuilr9/qlrm0BSXldqnqwMsf35Ld67mk=
 github.com/sagikazarmark/crypt v0.9.0 h1:fipzMFW34hFUEc4D7fsLQFtE7yElkpgyS2zruedRdZk=
 github.com/sagikazarmark/crypt v0.9.0/go.mod h1:RnH7sEhxfdnPm1z+XMgSLjWTEIjyK4z2dw6+4vHTMuo=
 github.com/sergi/go-diff v1.0.0 h1:Kpca3qRNrduNnOQeazBd0ysaKrUJiIuISHxogkT9RPQ=
 github.com/sergi/go-diff v1.0.0/go.mod h1:0CfEIISq7TuYL3j771MWULgwwjU+GofnZX9QAmXWZgo=
@@ -233,16 +241,16 @@
 golang.org/x/build v0.0.0-20190111050920-041ab4dc3f9d h1:E2M5QgjZ/Jg+ObCQAudsXxuTsLj7Nl5RV/lZcQZmKSo=
 golang.org/x/build v0.0.0-20190111050920-041ab4dc3f9d/go.mod h1:OWs+y06UdEOHN4y+MfF/py+xQ/tYqIWW03b70/CG9Rw=
 golang.org/x/crypto v0.0.0-20181030102418-4d3f4d9ffa16/go.mod h1:6SG95UA2DQfeDnfUPMdvaQW0Q7yPrPDi9nlGo2tz2b4=
 golang.org/x/crypto v0.0.0-20190313024323-a1f597ede03a/go.mod h1:djNgcEr1/C05ACkg1iLfiJU5Ep61QUkGW8qpdssI0+w=
 golang.org/x/crypto v0.0.0-20200221231518-2aa609cf4a9d/go.mod h1:LzIPMQfyMNhhGPhUkYOs5KpL4U8rLKemX1yGLhDgUto=
 golang.org/x/crypto v0.1.0/go.mod h1:RecgLatLF4+eUMCP1PoPZQb+cVrJcOPbHkTkbkB9sbw=
 golang.org/x/crypto v0.4.0/go.mod h1:3quD/ATkf6oY+rnes5c3ExXTbLc8mueNue5/DoinL80=
-golang.org/x/crypto v0.17.0 h1:r8bRNjWL3GshPW3gkd+RpvzWrZAwPS49OmTGZ/uhM4k=
-golang.org/x/crypto v0.17.0/go.mod h1:gCAAfMLgwOJRpTjQ2zCCt2OcSfYMTeZVSRtQlPC7Nq4=
+golang.org/x/exp/typeparams v0.0.0-20221208152030-732eee02a75a h1:Jw5wfR+h9mnIYH+OtGT2im5wV1YGGDora5vTv/aa5bE=
+golang.org/x/exp/typeparams v0.0.0-20221208152030-732eee02a75a/go.mod h1:AbB0pIl9nAr9wVwH+Z2ZpaocVmF5I4GyWCDIsVjR0bk=
 golang.org/x/image v0.0.0-20190802002840-cff245a6509b h1:+qEpEAPhDZ1o0x3tHzZTQDArnOixOzGD9HUJfcg0mb4=
 golang.org/x/lint v0.0.0-20180702182130-06c8688daad7/go.mod h1:UVdnD1Gm6xHRNCYTkRU2/jEulfH38KcIWyp/GAMgvoE=
 golang.org/x/lint v0.0.0-20201208152925-83fdc39ff7b5 h1:2M3HP5CCK1Si9FQhwnzYhXdG6DXeebvUHFpre8QvbyI=
 golang.org/x/mobile v0.0.0-20190719004257-d2bd2a29d028 h1:4+4C/Iv2U4fMZBiMCc98MG1In4gJY5YRhtpDNeDeHWs=
 golang.org/x/mod v0.8.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
 golang.org/x/mod v0.10.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
 golang.org/x/mod v0.11.0/go.mod h1:iBbtSCu2XBx23ZKBPSOrRkjjQPZFPuis4dIYUhu/chs=
@@ -250,44 +258,44 @@
 golang.org/x/net v0.0.0-20181029044818-c44066c5c816/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20181106065722-10aee1819953/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20190313220215-9f648a60d977/go.mod h1:t9HGtf8HONx5eT2rtn7q6eTqICYqUVnKs3thJo3Qplg=
 golang.org/x/net v0.1.0/go.mod h1:Cx3nUiGt4eDBEyega/BKRp+/AlGL8hYe7U9odMt2Cco=
 golang.org/x/net v0.3.0/go.mod h1:MBQ8lrhLObU/6UmLb4fmbmk5OcyYmqtbGd/9yIeKjEE=
 golang.org/x/net v0.10.0/go.mod h1:0qNGK6F8kojg2nk9dLZ2mShWaEBan6FAoqfSigmmuDg=
 golang.org/x/net v0.12.0/go.mod h1:zEVYFnQC7m/vmpQFELhcD1EWkZlX69l4oqgmer6hfKA=
+golang.org/x/net v0.21.0/go.mod h1:bIjVDfnllIU7BJ2DNgfnXvpSvtn8VRwhlsaeUTyUS44=
 golang.org/x/oauth2 v0.0.0-20181017192945-9dcd33a902f4/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20181203162652-d668ce993890/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20221014153046-6fdb5e3db783 h1:nt+Q6cXKz4MosCSpnbMtqiQ8Oz0pxTef2B4Vca2lvfk=
 golang.org/x/oauth2 v0.0.0-20221014153046-6fdb5e3db783/go.mod h1:h4gKUeWbJ4rQPri7E0u6Gs4e9Ri2zaLxzw5DI5XGrYg=
 golang.org/x/perf v0.0.0-20180704124530-6e6d33e29852 h1:xYq6+9AtI+xP3M4r0N1hCkHrInHDBohhquRgx9Kk6gI=
 golang.org/x/perf v0.0.0-20180704124530-6e6d33e29852/go.mod h1:JLpeXjPJfIyPr5TlbXLkXWLhP8nz10XfvxElABhCtcw=
 golang.org/x/sync v0.2.0/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
 golang.org/x/sys v0.0.0-20180909124046-d0be0721c37e/go.mod h1:STP8DvDyc/dI5b8T5hshtkjS+E42TnysNCUPdjciGhY=
 golang.org/x/sys v0.0.0-20181029174526-d69651ed3497/go.mod h1:STP8DvDyc/dI5b8T5hshtkjS+E42TnysNCUPdjciGhY=
 golang.org/x/sys v0.0.0-20190316082340-a2f829d7f35f/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
-golang.org/x/sys v0.1.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.3.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.5.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.6.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.8.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.10.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.15.0 h1:h48lPFYpsTvQJZF4EKyI4aLHaev3CxivZmv7yZig9pc=
-golang.org/x/sys v0.15.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/term v0.3.0/go.mod h1:q750SLmJuPmVoN1blW3UFBPREJfb1KmY3vwxfr+nFDA=
 golang.org/x/term v0.5.0/go.mod h1:jMB1sMXY+tzblOD4FWmEbocvup2/aLOaQEp7JmGp78k=
 golang.org/x/term v0.8.0 h1:n5xxQn2i3PC0yLAbjTpNT85q/Kgzcr2gIoX9OrJUols=
 golang.org/x/term v0.10.0 h1:3R7pNqamzBraeqj/Tj8qt1aQ2HpmlC+Cx/qL/7hn4/c=
 golang.org/x/term v0.10.0/go.mod h1:lpqdcUyK/oCiQxvxVrppt5ggO2KCZ5QblwqPnfZ6d5o=
 golang.org/x/term v0.13.0 h1:bb+I9cTfFazGW51MZqBVmZy7+JEJMouUHTUSKVQLBek=
 golang.org/x/term v0.13.0/go.mod h1:LTmsnFJwVN6bCy1rVCoS+qHT1HhALEFxKncY3WNNh4U=
 golang.org/x/term v0.15.0 h1:y/Oo/a/q3IXu26lQgl04j/gjuBDOBlx7X6Om1j2CPW4=
 golang.org/x/term v0.15.0/go.mod h1:BDl952bC7+uMoWR75FIrCDx79TPU9oHkTZ9yRbYOrX0=
+golang.org/x/term v0.17.0 h1:mkTF7LCd6WGJNL3K1Ad7kwxNfYAW6a8a8QqtMblp/4U=
+golang.org/x/term v0.17.0/go.mod h1:lLRBjIVuehSbZlaOtGMbcMncT+aqLLLmKrsjNrUguwk=
+golang.org/x/term v0.19.0 h1:+ThwsDv+tYfnJFhF4L8jITxu1tdTWRTZpdsWgEgjL6Q=
+golang.org/x/term v0.19.0/go.mod h1:2CuTdWZ7KHSQwUzKva0cbMg6q2DMI3Mmxp+gKJbskEk=
 golang.org/x/text v0.9.0/go.mod h1:e1OnstbJyHTd6l/uOt8jFFHp6TRDWZR/bV3emEE/zU8=
-golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
-golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
 golang.org/x/time v0.0.0-20180412165947-fbb02b2291d2/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/time v0.1.0 h1:xYY+Bajn2a7VBmTM5GikTmnK8ZuX8YgnQCqZpbBNtmA=
 golang.org/x/time v0.1.0/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/tools v0.0.0-20180828015842-6cd1fcedba52/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20181030000716-a0a13e073c7b/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.2.0/go.mod h1:y4OqIKeOV/fWJetJ8bXPU1sEVniLMIyDAZWeHdV+NTA=
 golang.org/x/tools v0.6.0/go.mod h1:Xwgl3UAJ/d3gWutnCtw505GrjyAbvKui8lOU390QaIU=
@@ -320,14 +328,16 @@
 gopkg.in/inf.v0 v0.9.1/go.mod h1:cWUDdTG/fYaXco+Dcufb5Vnc6Gp2YChqWtbxRZE0mXw=
 gopkg.in/yaml.v2 v2.2.1/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.2.8 h1:obN1ZagJSUGI0Ek/LBmuj4SNLPfIny3KsKFopxRdj10=
 grpc.go4.org v0.0.0-20170609214715-11d0a25b4919 h1:tmXTu+dfa+d9Evp8NpJdgOy6+rt8/x4yG7qPBrtNfLY=
 grpc.go4.org v0.0.0-20170609214715-11d0a25b4919/go.mod h1:77eQGdRu53HpSqPFJFmuJdjuHRquDANNeA4x7B8WQ9o=
 honnef.co/go/tools v0.0.0-20180728063816-88497007e858/go.mod h1:rf3lG4BRIbNafJWhAfAdb/ePZxsR/4RtNHQocxwk9r4=
 honnef.co/go/tools v0.0.1-2020.1.4 h1:UoveltGrhghAA7ePc+e+QYDHXrBps2PqFZiHkGR/xK8=
+honnef.co/go/tools v0.4.5 h1:YGD4H+SuIOOqsyoLOpZDWcieM28W47/zRO7f+9V3nvo=
+honnef.co/go/tools v0.4.5/go.mod h1:GUV+uIBCLpdf0/v6UhHHG/yzI/z6qPskBeQCjcNB96k=
 rsc.io/binaryregexp v0.2.0 h1:HfqmD5MEmC0zvwBuF187nq9mdnXjXsSivRiXN7SmRkE=
 rsc.io/quote/v3 v3.1.0 h1:9JKUTTIUgS6kzR9mK1YuGKv6Nl+DijDNIc0ghT58FaY=
 rsc.io/sampler v1.3.0 h1:7uVkIFmeBqHfdjD+gZwtXXI+RODJ2Wc4O7MPEh/QiW4=
 sourcegraph.com/sourcegraph/go-diff v0.5.0 h1:eTiIR0CoWjGzJcnQ3OkhIl/b9GJovq4lSAVRt0ZFEG8=
 sourcegraph.com/sourcegraph/go-diff v0.5.0/go.mod h1:kuch7UrkMzY0X+p9CRK03kfuPQ2zzQcaEFbx8wA8rck=
 sourcegraph.com/sqs/pbtypes v0.0.0-20180604144634-d3ebe8f20ae4 h1:JPJh2pk3+X4lXAkZIk2RuE/7/FoK9maXw+TNPJhVS/c=
 sourcegraph.com/sqs/pbtypes v0.0.0-20180604144634-d3ebe8f20ae4/go.mod h1:ketZ/q3QxT9HOBeFhu6RdvsftgpsbFHBF5Cas6cDKZ0=
```

### Comparing `hysteria2-2.3.0/hysteria2-go/hyperbole.py` & `hysteria2-2.4.3/hysteria2-go/hyperbole.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/logo.svg` & `hysteria2-2.4.3/hysteria2-go/logo.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/black 1@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/black 2@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/black 3@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/black 4@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/black 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 1@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 2@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 3@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/dark bg 4@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/dark bg 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 1@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 2@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 3@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/light bg 4@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/light bg 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 1@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 2@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 3@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/symbol 4@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/symbol 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/white 1@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 1@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/white 2@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 2@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/white 3@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 3@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/png/white 4@2x.png` & `hysteria2-2.4.3/hysteria2-go/media-kit/png/white 4@2x.png`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 1.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 2.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 3.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/black 4.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/black 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 1.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 2.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 3.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/dark bg 4.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/dark bg 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 1.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 2.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 3.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/light bg 4.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/light bg 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 1.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 2.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 3.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/symbol 4.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/symbol 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 1.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 1.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 2.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 2.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 3.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 3.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/media-kit/svg/white 4.svg` & `hysteria2-2.4.3/hysteria2-go/media-kit/svg/white 4.svg`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/hysteria2-go/scripts/install_server.sh` & `hysteria2-2.4.3/hysteria2-go/scripts/install_server.sh`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 
 # User for running hysteria
 HYSTERIA_USER="${HYSTERIA_USER:-}"
 
 # Directory for ACME certificates storage
 HYSTERIA_HOME_DIR="${HYSTERIA_HOME_DIR:-}"
 
+# SELinux context of systemd unit files
+SECONTEXT_SYSTEMD_UNIT="${SECONTEXT_SYSTEMD_UNIT:-}"
+
 
 ###
 # ARGUMENTS
 ###
 
 # Supported operation: install, remove, check_update
 OPERATION=
@@ -172,14 +175,45 @@
     warning "Ignored systemd command: systemctl $@"
     return
   fi
 
   command systemctl "$@"
 }
 
+chcon() {
+  if ! has_command chcon || [[ "x$FORCE_NO_SELINUX" == "x1" ]]; then
+    return
+  fi
+
+  command chcon "$@"
+}
+
+get_selinux_context() {
+  local _file="$1"
+
+  local _lsres="$(ls -dZ "$_file" | head -1)"
+  local _sectx=''
+  case "$(echo "$_lsres" | wc -w)" in
+    2)
+      _sectx="$(echo "$_lsres" | cut -d ' ' -f 1)"
+      ;;
+    5)
+      _sectx="$(echo "$_lsres" | cut -d ' ' -f 4)"
+      ;;
+    *)
+      ;;
+  esac
+
+  if [[ "x$_sectx" == "x?" ]]; then
+    _sectx=""
+  fi
+
+  echo "$_sectx"
+}
+
 show_argument_error_and_exit() {
   local _error_msg="$1"
 
   error "$_error_msg"
   echo "Try \"$0 --help\" for usage." >&2
   exit 22
 }
@@ -217,14 +251,15 @@
   local _saved_ifs="$IFS"
   IFS=$'\n'
   local _preserved_env=(
     $(env | grep "^PACKAGE_MANAGEMENT_INSTALL=" || true)
     $(env | grep "^OPERATING_SYSTEM=" || true)
     $(env | grep "^ARCHITECTURE=" || true)
     $(env | grep "^HYSTERIA_\w*=" || true)
+    $(env | grep "^SECONTEXT_SYSTEMD_UNIT=" || true)
     $(env | grep "^FORCE_\w*=" || true)
   )
   IFS="$_saved_ifs"
 
   exec sudo env \
     "${_preserved_env[@]}" \
     "$@"
@@ -232,14 +267,15 @@
 
 detect_package_manager() {
   if [[ -n "$PACKAGE_MANAGEMENT_INSTALL" ]]; then
     return 0
   fi
 
   if has_command apt; then
+    apt update
     PACKAGE_MANAGEMENT_INSTALL='apt -y --no-install-recommends install'
     return 0
   fi
 
   if has_command dnf; then
     PACKAGE_MANAGEMENT_INSTALL='dnf -y install'
     return 0
@@ -402,14 +438,38 @@
       error "This script only supports Linux distributions with systemd."
       note "Specify FORCE_NO_SYSTEMD=1 to disable this check and force this script to run as if systemd exists."
       note "Specify FORCE_NO_SYSTEMD=2 to disable this check and skip all systemd related commands."
       ;;
   esac
 }
 
+check_environment_selinux() {
+  if ! has_command chcon; then
+    return
+  fi
+
+  note "SELinux is detected"
+
+  if [[ "x$FORCE_NO_SELINUX" == "x1" ]]; then
+    warning "FORCE_NO_SELINUX=1, we will skip all SELinux related commands."
+    return
+  fi
+
+  if [[ -z "$SECONTEXT_SYSTEMD_UNIT" ]]; then
+    if [[ -z "$FORCE_NO_SYSTEMD" ]] && [[ -e "$SYSTEMD_SERVICES_DIR" ]]; then
+      local _sectx="$(get_selinux_context "$SYSTEMD_SERVICES_DIR")"
+      if [[ -z "$_sectx" ]]; then
+        warning "Failed to obtain SEContext of $SYSTEMD_SERVICES_DIR"
+      else
+        SECONTEXT_SYSTEMD_UNIT="$_sectx"
+      fi
+    fi
+  fi
+}
+
 check_environment_curl() {
   if has_command curl; then
     return
   fi
 
   install_software curl
 }
@@ -422,14 +482,15 @@
   install_software grep
 }
 
 check_environment() {
   check_environment_operating_system
   check_environment_architecture
   check_environment_systemd
+  check_environment_selinux
   check_environment_curl
   check_environment_grep
 }
 
 vercmp_segment() {
   local _lhs="$1"
   local _rhs="$2"
@@ -913,14 +974,18 @@
 perform_install_hysteria_systemd() {
   if [[ "x$FORCE_NO_SYSTEMD" == "x2" ]]; then
     return
   fi
 
   install_content -Dm644 "$(tpl_hysteria_server_service)" "$SYSTEMD_SERVICES_DIR/hysteria-server.service" "1"
   install_content -Dm644 "$(tpl_hysteria_server_x_service)" "$SYSTEMD_SERVICES_DIR/hysteria-server@.service" "1"
+  if [[ -n "$SECONTEXT_SYSTEMD_UNIT" ]]; then
+    chcon "$SECONTEXT_SYSTEMD_UNIT" "$SYSTEMD_SERVICES_DIR/hysteria-server.service"
+    chcon "$SECONTEXT_SYSTEMD_UNIT" "$SYSTEMD_SERVICES_DIR/hysteria-server@.service"
+  fi
 
   systemctl daemon-reload
 }
 
 perform_remove_hysteria_systemd() {
   remove_file "$SYSTEMD_SERVICES_DIR/hysteria-server.service"
   remove_file "$SYSTEMD_SERVICES_DIR/hysteria-server@.service"
```

### Comparing `hysteria2-2.3.0/hysteria2.egg-info/PKG-INFO` & `hysteria2-2.4.3/hysteria2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysteria2
-Version: 2.3.0
+Version: 2.4.3
 Summary: Python bindings for hysteria2.
 Home-page: https://github.com/LorenEteval/hysteria2-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MIT
 Description: # hysteria2-python
```

### Comparing `hysteria2-2.3.0/hysteria2.egg-info/SOURCES.txt` & `hysteria2-2.4.3/hysteria2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,39 @@
 hysteria2-go/app/internal/forwarding/udp.go
 hysteria2-go/app/internal/forwarding/udp_test.go
 hysteria2-go/app/internal/http/server.go
 hysteria2-go/app/internal/http/server_test.go
 hysteria2-go/app/internal/http/server_test.py
 hysteria2-go/app/internal/http/test.crt
 hysteria2-go/app/internal/http/test.key
+hysteria2-go/app/internal/proxymux/.mockery.yaml
+hysteria2-go/app/internal/proxymux/manager.go
+hysteria2-go/app/internal/proxymux/manager_test.go
+hysteria2-go/app/internal/proxymux/mux.go
+hysteria2-go/app/internal/proxymux/mux_test.go
+hysteria2-go/app/internal/proxymux/internal/mocks/mock_Conn.go
+hysteria2-go/app/internal/proxymux/internal/mocks/mock_Listener.go
 hysteria2-go/app/internal/redirect/getsockopt_linux.go
 hysteria2-go/app/internal/redirect/getsockopt_linux_386.go
 hysteria2-go/app/internal/redirect/syscall_socketcall_linux_386.s
 hysteria2-go/app/internal/redirect/tcp_linux.go
 hysteria2-go/app/internal/redirect/tcp_others.go
+hysteria2-go/app/internal/sockopts/fd_control_unix_socket_test.py
+hysteria2-go/app/internal/sockopts/sockopts.go
+hysteria2-go/app/internal/sockopts/sockopts_linux.go
+hysteria2-go/app/internal/sockopts/sockopts_linux_test.go
 hysteria2-go/app/internal/socks5/server.go
 hysteria2-go/app/internal/socks5/server_test.go
 hysteria2-go/app/internal/socks5/server_test.py
 hysteria2-go/app/internal/tproxy/tcp_linux.go
 hysteria2-go/app/internal/tproxy/tcp_others.go
 hysteria2-go/app/internal/tproxy/udp_linux.go
 hysteria2-go/app/internal/tproxy/udp_others.go
+hysteria2-go/app/internal/tun/log.go
+hysteria2-go/app/internal/tun/server.go
 hysteria2-go/app/internal/url/url.go
 hysteria2-go/app/internal/url/url_test.go
 hysteria2-go/app/internal/utils/bpsconv.go
 hysteria2-go/app/internal/utils/bpsconv_test.go
 hysteria2-go/app/internal/utils/geoloader.go
 hysteria2-go/app/internal/utils/qr.go
 hysteria2-go/app/internal/utils/update.go
```

### Comparing `hysteria2-2.3.0/pybind11/CMakeLists.txt` & `hysteria2-2.4.3/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/LICENSE` & `hysteria2-2.4.3/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/attr.h` & `hysteria2-2.4.3/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/buffer_info.h` & `hysteria2-2.4.3/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/cast.h` & `hysteria2-2.4.3/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/chrono.h` & `hysteria2-2.4.3/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/complex.h` & `hysteria2-2.4.3/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/class.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/common.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/descr.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/init.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/internals.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/type_caster_base.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/detail/typeid.h` & `hysteria2-2.4.3/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/eigen.h` & `hysteria2-2.4.3/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/embed.h` & `hysteria2-2.4.3/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/eval.h` & `hysteria2-2.4.3/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/functional.h` & `hysteria2-2.4.3/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/gil.h` & `hysteria2-2.4.3/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/iostream.h` & `hysteria2-2.4.3/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/numpy.h` & `hysteria2-2.4.3/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/operators.h` & `hysteria2-2.4.3/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/options.h` & `hysteria2-2.4.3/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/pybind11.h` & `hysteria2-2.4.3/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/pytypes.h` & `hysteria2-2.4.3/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/stl/filesystem.h` & `hysteria2-2.4.3/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/stl.h` & `hysteria2-2.4.3/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/include/pybind11/stl_bind.h` & `hysteria2-2.4.3/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/FindCatch.cmake` & `hysteria2-2.4.3/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/FindEigen3.cmake` & `hysteria2-2.4.3/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/FindPythonLibsNew.cmake` & `hysteria2-2.4.3/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/JoinPaths.cmake` & `hysteria2-2.4.3/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/check-style.sh` & `hysteria2-2.4.3/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/cmake_uninstall.cmake.in` & `hysteria2-2.4.3/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/codespell_ignore_lines_from_errors.py` & `hysteria2-2.4.3/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/libsize.py` & `hysteria2-2.4.3/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/make_changelog.py` & `hysteria2-2.4.3/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/pybind11Common.cmake` & `hysteria2-2.4.3/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/pybind11Config.cmake.in` & `hysteria2-2.4.3/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/pybind11NewTools.cmake` & `hysteria2-2.4.3/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/pybind11Tools.cmake` & `hysteria2-2.4.3/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/setup_global.py.in` & `hysteria2-2.4.3/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/pybind11/tools/setup_main.py.in` & `hysteria2-2.4.3/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `hysteria2-2.3.0/setup.py` & `hysteria2-2.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ROOT_DIR = pathlib.Path().resolve()
 PACKAGE_NAME = 'hysteria2'
 BINDING_NAME = 'hysteria2'
 CMAKE_BUILD_CACHE = 'CMakeBuildCache'
 
 
 def getHysteriaVersion():
-    return '2.3.0'
+    return '2.4.3'
 
 
 def runCommand(command):
     subprocess.run(command, check=True)
 
 
 def buildHysteria():
```

### Comparing `hysteria2-2.3.0/src/hysteria2.cpp` & `hysteria2-2.4.3/src/hysteria2.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 
     PYBIND11_MODULE(hysteria2, m) {
         m.def("startFromJSON",
             &startFromJSON,
             "Start Hysteria2 client with JSON",
             py::arg("json"));
 
-        m.attr("__version__") = "2.3.0";
+        m.attr("__version__") = "2.4.3";
     }
 }
```

