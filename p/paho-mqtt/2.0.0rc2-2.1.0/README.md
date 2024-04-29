# Comparing `tmp/paho_mqtt-2.0.0rc2.tar.gz` & `tmp/paho_mqtt-2.1.0.tar.gz`

## Comparing `paho_mqtt-2.0.0rc2.tar` & `paho_mqtt-2.1.0.tar`

### file list

```diff
@@ -1,149 +1,151 @@
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/about.html
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/edl-v10
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/epl-v20
--rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/notice.html
--rwxr-xr-x   0        0        0     4247 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/aws_iot.py
--rwxr-xr-x   0        0        0     1087 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_logger.py
--rwxr-xr-x   0        0        0     3098 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_mqtt_clear_retain.py
--rwxr-xr-x   0        0        0     1753 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_pub-wait.py
--rwxr-xr-x   0        0        0     4135 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_pub_opts.py
--rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_rpc_math.py
--rwxr-xr-x   0        0        0     1692 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_session_present.py
--rwxr-xr-x   0        0        0     1642 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub-class.py
--rwxr-xr-x   0        0        0     1827 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub-multiple-callback.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub-srv.py
--rwxr-xr-x   0        0        0     1610 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub-ws.py
--rwxr-xr-x   0        0        0     1602 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub.py
--rwxr-xr-x   0        0        0     3647 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/client_sub_opts.py
--rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/context.py
--rwxr-xr-x   0        0        0     3454 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/loop_asyncio.py
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/loop_select.py
--rwxr-xr-x   0        0        0     3005 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/loop_trio.py
--rwxr-xr-x   0        0        0      781 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/publish_multiple.py
--rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/publish_single.py
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/publish_utf8-27.py
--rwxr-xr-x   0        0        0      793 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/publish_utf8-3.py
--rwxr-xr-x   0        0        0     2865 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/server_rpc_math.py
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/subscribe_callback.py
--rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/examples/subscribe_simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/__init__.py
--rw-r--r--   0        0        0   198197 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/client.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/enums.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/matcher.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/packettypes.py
--rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/properties.py
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/publish.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/reasoncodes.py
--rw-r--r--   0        0        0    11462 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/subscribe.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/src/paho/mqtt/subscribeoptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/consts.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/debug_helpers.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/mqtt5_props.py
--rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/paho_test.py
--rw-r--r--   0        0        0    34679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_client.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_matcher.py
--rw-r--r--   0        0        0    56646 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_mqttv5.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_reasoncodes.py
--rw-r--r--   0        0        0     8761 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_websocket_integration.py
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/test_websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/__init__.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/conftest.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_asyncio.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_decorators.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_keepalive_pingreq.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_no_clean_session.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_reconnect_on_failure.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_empty_password_set.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_empty_set.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_set.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_unicode_set.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_will_set.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_will_unpwd_set.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_01_zero_length_clientid.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos0.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos1.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos2.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_02_unsubscribe.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_b2c_qos1.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_c2b_qos1_disconnect.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_c2b_qos2_disconnect.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_fill_inflight.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos0.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos0_v5.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos1_disconnect.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_qos0.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_qos0_no_payload.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_04_retain_qos0.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_bad_cacert.py
--rwxr-xr-x   0        0        0     1442 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_alpn.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_cert_auth.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_cert_auth_pw.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_no_auth.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_fake_cacert.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-asyncio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-decorators.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-keepalive-pingreq.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-no-clean-session.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-reconnect-on-failure.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-unpwd-empty-password-set.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-unpwd-empty-set.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-unpwd-set.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-unpwd-unicode-set.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-will-set.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-will-unpwd-set.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/01-zero-length-clientid.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos0.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos1.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos2.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/02-unsubscribe.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-b2c-qos1.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-b2c-qos2.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-c2b-qos1-disconnect.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-c2b-qos2-disconnect.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-fill-inflight.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-helper-qos0-v5.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-helper-qos0.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-helper-qos1-disconnect.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-qos0-no-payload.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-qos0.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/04-retain-qos0.py
--rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-alpn.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-cert-auth-pw.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-cert-auth.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-no-auth.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-fake-cacert.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/all-ca.crt
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client-expired.crt
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client-pw.crt
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client-pw.key
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client-revoked.crt
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client-revoked.key
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client.crt
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/client.key
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/crl.pem
--rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/gen.sh
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/openssl.cnf
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/server-expired.crt
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/server.crt
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/server.key
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-alt-ca.crt
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-alt-ca.key
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-bad-root-ca.crt
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-bad-root-ca.key
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-ca.srl
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-fake-root-ca.crt
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-fake-root-ca.key
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-root-ca.crt
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-root-ca.key
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-signing-ca.crt
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/ssl/test-signing-ca.key
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/testsupport/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/tests/testsupport/broker.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/.gitignore
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/LICENSE.txt
--rw-r--r--   0        0        0    47648 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/README.rst
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    48700 2020-02-02 00:00:00.000000 paho_mqtt-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/about.html
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/edl-v10
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/epl-v20
+-rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/notice.html
+-rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/aws_iot.py
+-rwxr-xr-x   0        0        0     1119 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_logger.py
+-rwxr-xr-x   0        0        0     3191 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_mqtt_clear_retain.py
+-rwxr-xr-x   0        0        0     1694 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_pub-wait.py
+-rwxr-xr-x   0        0        0     4088 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_pub_opts.py
+-rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_rpc_math.py
+-rwxr-xr-x   0        0        0     1815 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_session_present.py
+-rwxr-xr-x   0        0        0     1752 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub-class.py
+-rwxr-xr-x   0        0        0     1859 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub-multiple-callback.py
+-rwxr-xr-x   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub-srv.py
+-rwxr-xr-x   0        0        0     1616 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub-ws.py
+-rwxr-xr-x   0        0        0     1600 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub.py
+-rwxr-xr-x   0        0        0     3742 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/client_sub_opts.py
+-rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/context.py
+-rwxr-xr-x   0        0        0     3546 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/loop_asyncio.py
+-rwxr-xr-x   0        0        0     2576 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/loop_select.py
+-rwxr-xr-x   0        0        0     3097 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/loop_trio.py
+-rwxr-xr-x   0        0        0      781 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/publish_multiple.py
+-rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/publish_single.py
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/publish_utf8-27.py
+-rwxr-xr-x   0        0        0      798 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/publish_utf8-3.py
+-rwxr-xr-x   0        0        0     2861 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/server_rpc_math.py
+-rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/subscribe_callback.py
+-rwxr-xr-x   0        0        0      774 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/examples/subscribe_simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/__init__.py
+-rw-r--r--   0        0        0   202624 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/client.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/enums.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/matcher.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/packettypes.py
+-rw-r--r--   0        0        0    17369 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/properties.py
+-rw-r--r--   0        0        0    11576 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/publish.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/py.typed
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/reasoncodes.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/subscribe.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/src/paho/mqtt/subscribeoptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/consts.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/debug_helpers.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/mqtt5_props.py
+-rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/paho_test.py
+-rw-r--r--   0        0        0    37082 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_client.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_matcher.py
+-rw-r--r--   0        0        0    57106 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_mqttv5.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_reasoncodes.py
+-rw-r--r--   0        0        0     8761 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_websocket_integration.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/test_websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/__init__.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/conftest.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_asyncio.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_decorators.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_keepalive_pingreq.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_no_clean_session.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_reconnect_on_failure.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_unpwd_empty_password_set.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_unpwd_empty_set.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_unpwd_set.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_unpwd_unicode_set.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_will_set.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_will_unpwd_set.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_01_zero_length_clientid.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos0.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos1.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos2.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_02_unsubscribe.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_b2c_qos1.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_b2c_qos2.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_c2b_qos1_disconnect.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_c2b_qos2_disconnect.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_fill_inflight.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos0.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos0_v5.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos1_disconnect.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_qos0.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_03_publish_qos0_no_payload.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_04_retain_qos0.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_bad_cacert.py
+-rwxr-xr-x   0        0        0     1442 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_alpn.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_cert_auth.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_cert_auth_pw.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_no_auth.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/test_08_ssl_fake_cacert.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-asyncio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-decorators.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-keepalive-pingreq.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-no-clean-session.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-reconnect-on-failure.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-unpwd-empty-password-set.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-unpwd-empty-set.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-unpwd-set.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-unpwd-unicode-set.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-will-set.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-will-unpwd-set.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/01-zero-length-clientid.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos0.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos1.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos2.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/02-unsubscribe.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-b2c-qos1.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-b2c-qos2.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-c2b-qos1-disconnect.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-c2b-qos2-disconnect.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-fill-inflight.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-helper-qos0-v5.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-helper-qos0.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-helper-qos1-disconnect.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-qos0-no-payload.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/03-publish-qos0.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/04-retain-qos0.py
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-alpn.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-cert-auth-pw.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-cert-auth.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-no-auth.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/lib/clients/08-ssl-fake-cacert.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/all-ca.crt
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client-expired.crt
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client-pw.crt
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client-pw.key
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client-revoked.crt
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client-revoked.key
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client.crt
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/client.key
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/crl.pem
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/gen.sh
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/openssl.cnf
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/server-expired.crt
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/server.crt
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/server.key
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-alt-ca.crt
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-alt-ca.key
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-bad-root-ca.crt
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-bad-root-ca.key
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-ca.srl
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-fake-root-ca.crt
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-fake-root-ca.key
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-root-ca.crt
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-root-ca.key
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-signing-ca.crt
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/ssl/test-signing-ca.key
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/testsupport/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/tests/testsupport/broker.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/.gitignore
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/README.rst
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    23463 2020-02-02 00:00:00.000000 paho_mqtt-2.1.0/PKG-INFO
```

### Comparing `paho_mqtt-2.0.0rc2/CONTRIBUTING.md` & `paho_mqtt-2.1.0/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -88,23 +88,27 @@
 
 Making a release
 ----------------
 
 The process to make a release is the following:
 * Update the Changelog with the release version and date. Ensure it's up-to-date with latest fixes & PRs merged.
 * Make sure test pass, check that Github actions are green.
+* Check that documentation build (`cd docs; make html`)
+* Bump the version number in ``paho/mqtt/__init__.py``, commit the change.
 * Make a dry-run of build:
    * Build using hatch: ``python -m hatch build``
    * Check with twine for common errors: ``python -m twine check dist/*``
    * Try uploading it to testpypi: ``python3 -m twine upload --repository testpypi dist/*``
-* Bump the version number in ``paho/mqtt/__init__.py``, commit the change.
 * Do a GPG signed tag (assuming your GPG is correctly configured, it's ``git tag -s -m "Version 1.2.3" v1.2.3``)
 * Push the commit and it's tag to Github
 * Make sure your git is clean, especially the ``dist/`` folder.
 * Build a release: ``python -m hatch build``
 * You can also get the latest build from Github action. It should be identical to your local build:
   https://github.com/eclipse/paho.mqtt.python/actions/workflows/build.yml?query=branch%3Amaster
 * Then upload the dist file, you can follow instruction on https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives
   It should mostly be ``python -m twine upload dist/*``
 * Create a release on Github, copy-pasting the release note from Changelog.
+* Build and publish the documentation
+   * To build the documentation, run `make clean html` in `docs` folder
+   * Copy `_build/html/` to https://github.com/eclipse/paho-website/tree/master/files/paho.mqtt.python/html
 * Announce the release on the Mailing list.
 * To allow installing from a git clone, update the version in ``paho/mqtt/__init__.py`` to next number WITH .dev0 (example ``1.2.3.dev0``)
```

### Comparing `paho_mqtt-2.0.0rc2/about.html` & `paho_mqtt-2.1.0/about.html`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/edl-v10` & `paho_mqtt-2.1.0/edl-v10`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/epl-v20` & `paho_mqtt-2.1.0/epl-v20`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/notice.html` & `paho_mqtt-2.1.0/notice.html`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/aws_iot.py` & `paho_mqtt-2.1.0/examples/aws_iot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime
 import functools
 import hashlib
 import hmac
 import os
 import uuid
 
-from paho.mqtt.client import Client
+from paho.mqtt.client import Client, CallbackAPIVersion
 
 
 def get_amazon_auth_headers(access_key, secret_key, region, host, port, headers=None):
     """ Get the amazon auth headers for working with the amazon websockets
     protocol
 
     Requires a lot of extra stuff:
@@ -118,12 +118,12 @@
         access_key,
         secret_key,
         region,
         host,
         port,
     )
 
-    client = Client(transport="websockets")
+    client = Client(CallbackAPIVersion.VERSION2, transport="websockets")
 
     client.ws_set_options(headers=extra_headers)
 
     # Use client as normal from here
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_logger.py` & `paho_mqtt-2.1.0/examples/client_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 logging.basicConfig(level=logging.DEBUG)
 
 # If you want to use a specific client id, use
 # mqttc = mqtt.Client("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = mqtt.Client()
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 
 logger = logging.getLogger(__name__)
 mqttc.enable_logger(logger)
 
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 mqttc.subscribe("$SYS/#", 0)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_mqtt_clear_retain.py` & `paho_mqtt-2.1.0/examples/client_mqtt_clear_retain.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 final_mid = 0
 
 
-def on_connect(mqttc, userdata, flags, rc):
+def on_connect(mqttc, userdata, flags, reason_code, properties):
     if userdata:
-        print("rc: " + str(rc))
+        print(f"reason_code: {reason_code}")
 
 
 def on_message(mqttc, userdata, msg):
     global final_mid
     if msg.retain == 0:
         pass
         # sys.exit()
     else:
         if userdata:
             print("Clearing topic " + msg.topic)
         (rc, final_mid) = mqttc.publish(msg.topic, None, 1, True)
 
 
-def on_publish(mqttc, userdata, mid):
+def on_publish(mqttc, userdata, mid, reason_code, properties):
     global final_mid
     if mid == final_mid:
         sys.exit()
 
 
 def on_log(mqttc, userdata, level, string):
     print(string)
@@ -97,15 +97,15 @@
             verbose = True
 
     if not topic:
         print("You must provide a topic to clear.\n")
         print_usage()
         sys.exit(2)
 
-    mqttc = mqtt.Client(client_id)
+    mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id)
     mqttc._userdata = verbose
     mqttc.on_message = on_message
     mqttc.on_publish = on_publish
     mqttc.on_connect = on_connect
     if debug:
         mqttc.on_log = on_log
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_pub-wait.py` & `paho_mqtt-2.1.0/examples/client_pub-wait.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,44 +18,38 @@
 # This shows a simple example of waiting for a message to be published.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("rc: " + str(rc))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("reason_code: " + str(reason_code))
 
 
 def on_message(mqttc, obj, msg):
     print(msg.topic + " " + str(msg.qos) + " " + str(msg.payload))
 
 
-def on_publish(mqttc, obj, mid):
+def on_publish(mqttc, obj, mid, reason_code, properties):
     print("mid: " + str(mid))
-    pass
-
-
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: " + str(mid) + " " + str(granted_qos))
 
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 
 # If you want to use a specific client id, use
 # mqttc = mqtt.Client("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = mqtt.Client()
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
 mqttc.on_publish = on_publish
-mqttc.on_subscribe = on_subscribe
 # Uncomment to enable debug messages
 # mqttc.on_log = on_log
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 
 mqttc.loop_start()
 
 print("tuple")
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_pub_opts.py` & `paho_mqtt-2.1.0/examples/client_pub_opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,30 +40,26 @@
 parser.add_argument('-F', '--cacerts', required=False, default=None)
 parser.add_argument('--tls-version', required=False, default=None, help='TLS protocol version, can be one of tlsv1.2 tlsv1.1 or tlsv1\n')
 parser.add_argument('-D', '--debug', action='store_true')
 
 args, unknown = parser.parse_known_args()
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("connect rc: " + str(rc))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("connect reason_code: " + str(reason_code))
 
 
 def on_message(mqttc, obj, msg):
     print(msg.topic + " " + str(msg.qos) + " " + str(msg.payload))
 
 
-def on_publish(mqttc, obj, mid):
+def on_publish(mqttc, obj, mid, reason_code, properties):
     print("mid: " + str(mid))
 
 
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: " + str(mid) + " " + str(granted_qos))
-
-
 def on_log(mqttc, obj, level, string):
     print(string)
 
 usetls = args.use_tls
 
 if args.cacerts:
     usetls = True
@@ -71,15 +67,15 @@
 port = args.port
 if port is None:
     if usetls:
         port = 8883
     else:
         port = 1883
 
-mqttc = mqtt.Client(args.clientid,clean_session = not args.disable_clean_session)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, args.clientid, clean_session = not args.disable_clean_session)
 
 if usetls:
     if args.tls_version == "tlsv1.2":
        tlsVersion = ssl.PROTOCOL_TLSv1_2
     elif args.tls_version == "tlsv1.1":
        tlsVersion = ssl.PROTOCOL_TLSv1_1
     elif args.tls_version == "tlsv1":
@@ -102,15 +98,14 @@
 
 if args.username or args.password:
     mqttc.username_pw_set(args.username, args.password)
 
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
 mqttc.on_publish = on_publish
-mqttc.on_subscribe = on_subscribe
 
 if args.debug:
     mqttc.on_log = on_log
 
 print("Connecting to "+args.host+" port: "+str(port))
 mqttc.connect(args.host, port, args.keepalive)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_rpc_math.py` & `paho_mqtt-2.1.0/examples/client_rpc_math.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #   http://www.eclipse.org/org/documents/edl-v10.php.
 #
 # Contributors:
 #   Frank Pagliughi - initial implementation
 #
 
 # This shows an example of an MQTTv5 Remote Procedure Call (RPC) client.
+# You should run the server_rpc_math.py before.
+
 
 import json
 import sys
 import time
 
 import context  # Ensures paho is in PYTHONPATH
 
@@ -33,18 +35,18 @@
 # This correlates the outbound request with the returned reply
 corr_id = b"1"
 
 # This is sent in the message callback when we get the response
 reply = None
 
 # The MQTTv5 callback takes the additional 'props' parameter.
-def on_connect(mqttc, userdata, flags, rc, props):
+def on_connect(mqttc, userdata, flags, reason_code, props):
     global client_id, reply_to
 
-    print("Connected: '"+str(flags)+"', '"+str(rc)+"', '"+str(props))
+    print(f"Connected: '{flags}', '{reason_code}',  '{props}'")
     if hasattr(props, 'AssignedClientIdentifier'):
         client_id = props.AssignedClientIdentifier
     reply_to = "replies/math/" + client_id
     mqttc.subscribe(reply_to)
 
 
 # An incoming message should be the reply to our request
@@ -61,19 +63,19 @@
         reply = msg.payload
 
 
 if len(sys.argv) < 3:
     print("USAGE: client_rpc_math.py [add|mult] n1 n2 ...")
     sys.exit(1)
 
-mqttc = mqtt.Client(client_id="", protocol=mqtt.MQTTv5)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="", protocol=mqtt.MQTTv5)
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
 
-mqttc.connect(host='localhost', clean_start=True)
+mqttc.connect(host="mqtt.eclipseprojects.io", clean_start=True)
 mqttc.loop_start()
 
 # Wait for connection to set `client_id`, etc.
 while not mqttc.is_connected():
     time.sleep(0.1)
 
 # Properties for the request specify the ResponseTopic and CorrelationData
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_session_present.py` & `paho_mqtt-2.1.0/examples/client_session_present.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,45 +18,45 @@
 # This demonstrates the session present flag when connecting.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
-def on_connect(mqttc, obj, flags, rc):
+def on_connect(mqttc, obj, flags, reason_code, properties):
     if obj == 0:
         print("First connection:")
     elif obj == 1:
         print("Second connection:")
     elif obj == 2:
         print("Third connection (with clean session=True):")
-    print("    Session present: " + str(flags['session present']))
-    print("    Connection result: " + str(rc))
+    print("    Session present: " + str(flags.session_present))
+    print("    Connection result: " + str(reason_code))
     mqttc.disconnect()
 
 
-def on_disconnect(mqttc, obj, rc):
+def on_disconnect(mqttc, obj, flags, reason_code, properties):
     mqttc.user_data_set(obj + 1)
     if obj == 0:
         mqttc.reconnect()
 
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 
-mqttc = mqtt.Client(client_id="asdfj", clean_session=False)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="asdfj", clean_session=False)
 mqttc.on_connect = on_connect
 mqttc.on_disconnect = on_disconnect
 # Uncomment to enable debug messages
 # mqttc.on_log = on_log
 mqttc.user_data_set(0)
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 
 mqttc.loop_forever()
 
 # Clear session
-mqttc = mqtt.Client(client_id="asdfj", clean_session=True)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="asdfj", clean_session=True)
 mqttc.on_connect = on_connect
 mqttc.user_data_set(2)
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 mqttc.loop_forever()
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub-class.py` & `paho_mqtt-2.1.0/examples/client_sub-class.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
 class MyMQTTClass(mqtt.Client):
 
-    def on_connect(self, mqttc, obj, flags, rc):
-        print("rc: "+str(rc))
+    def on_connect(self, mqttc, obj, flags, reason_code, properties):
+        print("rc: "+str(reason_code))
 
     def on_connect_fail(self, mqttc, obj):
         print("Connect failed")
 
     def on_message(self, mqttc, obj, msg):
         print(msg.topic+" "+str(msg.qos)+" "+str(msg.payload))
 
-    def on_publish(self, mqttc, obj, mid):
+    def on_publish(self, mqttc, obj, mid, reason_codes, properties):
         print("mid: "+str(mid))
 
-    def on_subscribe(self, mqttc, obj, mid, granted_qos):
-        print("Subscribed: "+str(mid)+" "+str(granted_qos))
+    def on_subscribe(self, mqttc, obj, mid, reason_code_list, properties):
+        print("Subscribed: "+str(mid)+" "+str(reason_code_list))
 
     def on_log(self, mqttc, obj, level, string):
         print(string)
 
     def run(self):
         self.connect("mqtt.eclipseprojects.io", 1883, 60)
         self.subscribe("$SYS/#", 0)
@@ -50,11 +50,11 @@
         return rc
 
 
 # If you want to use a specific client id, use
 # mqttc = MyMQTTClass("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = MyMQTTClass()
+mqttc = MyMQTTClass(mqtt.CallbackAPIVersion.VERSION2)
 rc = mqttc.run()
 
 print("rc: "+str(rc))
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub-multiple-callback.py` & `paho_mqtt-2.1.0/examples/client_sub-multiple-callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # This callback will be called for messages that we receive that do not
     # match any patterns defined in topic specific callbacks, i.e. in this case
     # those messages that do not have topics $SYS/broker/messages/# nor
     # $SYS/broker/bytes/#
     print(msg.topic + " " + str(msg.qos) + " " + str(msg.payload))
 
 
-mqttc = mqtt.Client()
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 
 # Add message callbacks that will only trigger on a specific subscription match.
 mqttc.message_callback_add("$SYS/broker/messages/#", on_message_msgs)
 mqttc.message_callback_add("$SYS/broker/bytes/#", on_message_bytes)
 mqttc.on_message = on_message
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 mqttc.subscribe("$SYS/#", 0)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub-srv.py` & `paho_mqtt-2.1.0/examples/client_sub-srv.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,41 +18,37 @@
 # This shows a simple example of an MQTT subscriber using connect_srv method.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("Connected to %s:%s" % (mqttc._host, mqttc._port))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("Connected to %s:%s" % (mqttc.host, mqttc.port))
 
 def on_message(mqttc, obj, msg):
     print(msg.topic+" "+str(msg.qos)+" "+str(msg.payload))
 
-def on_publish(mqttc, obj, mid):
-    print("mid: "+str(mid))
-
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: "+str(mid)+" "+str(granted_qos))
+def on_subscribe(mqttc, obj, mid, reason_code_list, properties):
+    print("Subscribed: "+str(mid)+" "+str(reason_code_list))
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 # If you want to use a specific client id, use
 # mqttc = mqtt.Client("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = mqtt.Client()
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
-mqttc.on_publish = on_publish
 mqttc.on_subscribe = on_subscribe
 # Uncomment to enable debug messages
 #mqttc.on_log = on_log
-mqttc.connect_srv("mosquitto.org", 60)
+mqttc.connect_srv("eclipseprojects.io", 60)
 mqttc.subscribe("$SYS/broker/version", 0)
 
 
 rc = 0
 while rc == 0:
     rc = mqttc.loop()
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub-ws.py` & `paho_mqtt-2.1.0/examples/client_sub-ws.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,37 +18,33 @@
 # This shows a simple example of an MQTT subscriber.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("rc: "+str(rc))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("reason_code: "+str(reason_code))
 
 def on_message(mqttc, obj, msg):
     print(msg.topic+" "+str(msg.qos)+" "+str(msg.payload))
 
-def on_publish(mqttc, obj, mid):
-    print("mid: "+str(mid))
-
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: "+str(mid)+" "+str(granted_qos))
+def on_subscribe(mqttc, obj, mid, reason_code_list, properties):
+    print("Subscribed: "+str(mid)+" "+str(reason_code_list))
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 # If you want to use a specific client id, use
 # mqttc = mqtt.Client("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = mqtt.Client(transport="websockets")
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, transport="websockets")
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
-mqttc.on_publish = on_publish
 mqttc.on_subscribe = on_subscribe
 # Uncomment to enable debug messages
 mqttc.on_log = on_log
-mqttc.connect("test.mosquitto.org", 8080, 60)
+mqttc.connect("mqtt.eclipseprojects.io", 80, 60)
 mqttc.subscribe("$SYS/broker/version", 0)
 
 mqttc.loop_forever()
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub.py` & `paho_mqtt-2.1.0/examples/client_sub.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,42 +18,37 @@
 # This shows a simple example of an MQTT subscriber.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.client as mqtt
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("rc: " + str(rc))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("reason_code: " + str(reason_code))
 
 
 def on_message(mqttc, obj, msg):
     print(msg.topic + " " + str(msg.qos) + " " + str(msg.payload))
 
 
-def on_publish(mqttc, obj, mid):
-    print("mid: " + str(mid))
-
-
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: " + str(mid) + " " + str(granted_qos))
+def on_subscribe(mqttc, obj, mid, reason_code_list, properties):
+    print("Subscribed: " + str(mid) + " " + str(reason_code_list))
 
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 
 # If you want to use a specific client id, use
 # mqttc = mqtt.Client("client-id")
 # but note that the client id must be unique on the broker. Leaving the client
 # id parameter empty will generate a random id for you.
-mqttc = mqtt.Client()
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
-mqttc.on_publish = on_publish
 mqttc.on_subscribe = on_subscribe
 # Uncomment to enable debug messages
 # mqttc.on_log = on_log
 mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
 mqttc.subscribe("$SYS/#")
 
 mqttc.loop_forever()
```

### Comparing `paho_mqtt-2.0.0rc2/examples/client_sub_opts.py` & `paho_mqtt-2.1.0/examples/client_sub_opts.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,28 +37,28 @@
 parser.add_argument('-F', '--cacerts', required=False, default=None)
 parser.add_argument('--tls-version', required=False, default=None, help='TLS protocol version, can be one of tlsv1.2 tlsv1.1 or tlsv1\n')
 parser.add_argument('-D', '--debug', action='store_true')
 
 args, unknown = parser.parse_known_args()
 
 
-def on_connect(mqttc, obj, flags, rc):
-    print("rc: " + str(rc))
+def on_connect(mqttc, obj, flags, reason_code, properties):
+    print("reason_code: " + str(reason_code))
 
 
 def on_message(mqttc, obj, msg):
     print(msg.topic + " " + str(msg.qos) + " " + str(msg.payload))
 
 
 def on_publish(mqttc, obj, mid):
     print("mid: " + str(mid))
 
 
-def on_subscribe(mqttc, obj, mid, granted_qos):
-    print("Subscribed: " + str(mid) + " " + str(granted_qos))
+def on_subscribe(mqttc, obj, mid, reason_code_list, properties):
+    print("Subscribed: " + str(mid) + " " + str(reason_code_list))
 
 
 def on_log(mqttc, obj, level, string):
     print(string)
 
 usetls = args.use_tls
 
@@ -68,15 +68,15 @@
 port = args.port
 if port is None:
     if usetls:
         port = 8883
     else:
         port = 1883
 
-mqttc = mqtt.Client(args.clientid,clean_session = not args.disable_clean_session)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, args.clientid,clean_session = not args.disable_clean_session)
 
 if usetls:
     if args.tls_version == "tlsv1.2":
        tlsVersion = ssl.PROTOCOL_TLSv1_2
     elif args.tls_version == "tlsv1.1":
        tlsVersion = ssl.PROTOCOL_TLSv1_1
     elif args.tls_version == "tlsv1":
```

### Comparing `paho_mqtt-2.0.0rc2/examples/context.py` & `paho_mqtt-2.1.0/examples/context.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/loop_asyncio.py` & `paho_mqtt-2.1.0/examples/loop_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,32 +60,32 @@
         print("misc_loop finished")
 
 
 class AsyncMqttExample:
     def __init__(self, loop):
         self.loop = loop
 
-    def on_connect(self, client, userdata, flags, rc):
+    def on_connect(self, client, userdata, flags, reason_code, properties):
         print("Subscribing")
         client.subscribe(topic)
 
     def on_message(self, client, userdata, msg):
         if not self.got_message:
             print("Got unexpected message: {}".format(msg.decode()))
         else:
             self.got_message.set_result(msg.payload)
 
-    def on_disconnect(self, client, userdata, rc):
-        self.disconnected.set_result(rc)
+    def on_disconnect(self, client, userdata, flags, reason_code, properties):
+        self.disconnected.set_result(reason_code)
 
     async def main(self):
         self.disconnected = self.loop.create_future()
         self.got_message = None
 
-        self.client = mqtt.Client(client_id=client_id)
+        self.client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id=client_id)
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
         self.client.on_disconnect = self.on_disconnect
 
         aioh = AsyncioHelper(self.loop, self.client)
 
         self.client.connect('mqtt.eclipseprojects.io', 1883, 60)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/loop_select.py` & `paho_mqtt-2.1.0/examples/loop_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 print("Using client_id / topic: " + client_id)
 
 
 class SelectMqttExample:
     def __init__(self):
         pass
 
-    def on_connect(self, client, userdata, flags, rc):
+    def on_connect(self, client, userdata, flags, reason_code, properties):
         print("Subscribing")
         client.subscribe(topic)
 
     def on_message(self, client, userdata, msg):
         if self.state not in {1, 3, 5}:
             print("Got unexpected message: {}".format(msg.decode()))
             return
 
         print("Got message with len {}".format(len(msg.payload)))
         self.state += 1
         self.t = time()
 
-    def on_disconnect(self, client, userdata, rc):
-        self.disconnected = True, rc
+    def on_disconnect(self, client, userdata, flags, reason_code, properties):
+        self.disconnected = True, reason_code
 
     def do_select(self):
         sock = self.client.socket()
         if not sock:
             raise Exception("Socket is gone")
 
         print("Selecting for reading" + (" and writing" if self.client.want_write() else ""))
@@ -56,15 +56,15 @@
         self.client.loop_misc()
 
     def main(self):
         self.disconnected = (False, None)
         self.t = time()
         self.state = 0
 
-        self.client = mqtt.Client(client_id=client_id)
+        self.client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id=client_id)
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
         self.client.on_disconnect = self.on_disconnect
 
         self.client.connect('mqtt.eclipseprojects.io', 1883, 60)
         print("Socket opened")
         self.client.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/loop_trio.py` & `paho_mqtt-2.1.0/examples/loop_trio.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,33 +50,33 @@
 
     def on_socket_unregister_write(self, client, userdata, sock):
         print("finished large write")
         self._event_large_write = trio.Event()
 
 
 class TrioAsyncMqttExample:
-    def on_connect(self, client, userdata, flags, rc):
+    def on_connect(self, client, userdata, flags, reason_code, properties):
         print("Subscribing")
         client.subscribe(topic)
 
     def on_message(self, client, userdata, msg):
         print("Got response with {} bytes".format(len(msg.payload)))
 
-    def on_disconnect(self, client, userdata, rc):
-        print('Disconnect result {}'.format(rc))
+    def on_disconnect(self, client, userdata, flags, reason_code, properties):
+        print('Disconnect result {}'.format(reason_code))
 
     async def test_write(self, cancel_scope: trio.CancelScope):
         for c in range(3):
             await trio.sleep(5)
             print("Publishing")
             self.client.publish(topic, b'Hello' * 40000, qos=1)
         cancel_scope.cancel()
 
     async def main(self):
-        self.client = mqtt.Client(client_id=client_id)
+        self.client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id=client_id)
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
         self.client.on_disconnect = self.on_disconnect
 
         trio_helper = TrioAsyncHelper(self.client)
 
         self.client.connect('mqtt.eclipseprojects.io', 1883, 60)
```

### Comparing `paho_mqtt-2.0.0rc2/examples/publish_multiple.py` & `paho_mqtt-2.1.0/examples/publish_multiple.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/publish_single.py` & `paho_mqtt-2.1.0/examples/publish_single.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/publish_utf8-27.py` & `paho_mqtt-2.1.0/examples/publish_utf8-27.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/publish_utf8-3.py` & `paho_mqtt-2.1.0/examples/publish_utf8-3.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.publish as publish
 
 topic = u"paho/test/single/ô"
 payload = u'German umlauts like "ä" ü"ö" are not supported'
-publish.single(topic, payload, hostname="test.mosquitto.org")
+publish.single(topic, payload, hostname="mqtt.eclipseprojects.io")
```

### Comparing `paho_mqtt-2.0.0rc2/examples/server_rpc_math.py` & `paho_mqtt-2.1.0/examples/server_rpc_math.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 def mult(nums):
     prod = 1
     for x in nums:
         prod *= x
     return prod
 
 # Remember that the MQTTv5 callback takes the additional 'props' parameter.
-def on_connect(mqttc, userdata, flags, rc, props):
-    print("Connected: '"+str(flags)+"', '"+str(rc)+"', '"+str(props))
-    if not flags["session present"]:
+def on_connect(mqttc, userdata, flags, reason_code, props):
+    print(f"Connected: '{flags}', '{reason_code}',  '{props}'")
+    if not flags.session_present:
         print("Subscribing to math requests")
         mqttc.subscribe("requests/math/#")
 
 # Each incoming message should be an RPC request on the
 # 'requests/math/#' topic.
 def on_message(mqttc, userdata, msg):
     print(msg.topic + "  " + str(msg.payload))
@@ -81,17 +81,16 @@
 def on_log(mqttc, obj, level, string):
     print(string)
 
 
 # Typically with an RPC service, you want to make sure that you're the only
 # client answering requests for specific topics. Using a known client ID
 # might help.
-mqttc = mqtt.Client(client_id="paho_rpc_math_srvr", protocol=mqtt.MQTTv5)
+mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="paho_rpc_math_srvr", protocol=mqtt.MQTTv5)
 mqttc.on_message = on_message
 mqttc.on_connect = on_connect
 
 # Uncomment to enable debug messages
 #mqttc.on_log = on_log
 
-#mqttc.connect("mqtt.eclipseprojects.io", 1883, 60)
-mqttc.connect(host="localhost", clean_start=False)
+mqttc.connect(host="mqtt.eclipseprojects.io", clean_start=False)
 mqttc.loop_forever()
```

### Comparing `paho_mqtt-2.0.0rc2/examples/subscribe_callback.py` & `paho_mqtt-2.1.0/examples/subscribe_callback.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/examples/subscribe_simple.py` & `paho_mqtt-2.1.0/examples/subscribe_simple.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/client.py` & `paho_mqtt-2.1.0/src/paho/mqtt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,31 +35,36 @@
 import urllib.request
 import uuid
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, NamedTuple, Sequence, Tuple, Union, cast
 
 from paho.mqtt.packettypes import PacketTypes
 
-from .enums import CallbackAPIVersion, ConnackCode, ConnectionState, LogLevel, MessageState, MessageType, MQTTErrorCode, MQTTProtocolVersion, PahoClientMode
+from .enums import CallbackAPIVersion, ConnackCode, LogLevel, MessageState, MessageType, MQTTErrorCode, MQTTProtocolVersion, PahoClientMode, _ConnectionState
 from .matcher import MQTTMatcher
 from .properties import Properties
-from .reasoncodes import ReasonCodes
+from .reasoncodes import ReasonCode, ReasonCodes
 from .subscribeoptions import SubscribeOptions
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 if TYPE_CHECKING:
     try:
         from typing import TypedDict  # type: ignore
     except ImportError:
         from typing_extensions import TypedDict
 
+    try:
+        from typing import Protocol  # type: ignore
+    except ImportError:
+        from typing_extensions import Protocol  # type: ignore
+
     class _InPacket(TypedDict):
         command: int
         have_remaining: int
         remaining_count: list[int]
         remaining_mult: int
         remaining_length: int
         packet: bytearray
@@ -72,14 +77,26 @@
         mid: int
         qos: int
         pos: int
         to_process: int
         packet: bytes
         info: MQTTMessageInfo | None
 
+    class SocketLike(Protocol):
+        def recv(self, buffer_size: int) -> bytes:
+            ...
+        def send(self, buffer: bytes) -> int:
+            ...
+        def close(self) -> None:
+            ...
+        def fileno(self) -> int:
+            ...
+        def setblocking(self, flag: bool) -> None:
+            ...
+
 
 try:
     import ssl
 except ImportError:
     ssl = None  # type: ignore[assignment]
 
 
@@ -104,14 +121,16 @@
 
 
 if platform.system() == 'Windows':
     EAGAIN = errno.WSAEWOULDBLOCK  # type: ignore[attr-defined]
 else:
     EAGAIN = errno.EAGAIN
 
+# Avoid linter complain. We kept importing it as ReasonCodes (plural) for compatibility
+_ = ReasonCodes
 
 # Keep copy of enums values for compatibility.
 CONNECT = MessageType.CONNECT
 CONNACK = MessageType.CONNACK
 PUBLISH = MessageType.PUBLISH
 PUBACK = MessageType.PUBACK
 PUBREC = MessageType.PUBREC
@@ -196,82 +215,84 @@
 # * int/float are converted to string and utf8 encoded (e.g. 1 is converted to b"1")
 # * None is converted to a zero-length payload (i.e. b"")
 PayloadType = Union[str, bytes, bytearray, int, float, None]
 
 HTTPHeader = Dict[str, str]
 WebSocketHeaders = Union[Callable[[HTTPHeader], HTTPHeader], HTTPHeader]
 
-SocketLike = Union[socket.socket, "ssl.SSLSocket", "WebsocketWrapper"]
-
 CleanStartOption = Union[bool, Literal[3]]
 
 
 class ConnectFlags(NamedTuple):
-    """Contains additional information for on_connect
-
-    session_present: this flag is useful for clients that are
-        using clean session set to False only (MQTTv3) or clean_start = False (MQTTv5).
-        In that case, if client  that reconnects to a broker that it has previously
-        connected to, this flag indicates whether the broker still has the
-        session information for the client. If true, the session still exists.
-    """
+    """Contains additional information passed to `on_connect` callback"""
 
     session_present: bool
+    """
+    this flag is useful for clients that are
+    using clean session set to False only (MQTTv3) or clean_start = False (MQTTv5).
+    In that case, if client  that reconnects to a broker that it has previously
+    connected to, this flag indicates whether the broker still has the
+    session information for the client. If true, the session still exists.
+    """
 
 
 class DisconnectFlags(NamedTuple):
-    """Contains additional information of on_disconnect
-
-    is_disconnect_packet_from_server: tell whether this on_disconnect call is the result
-        of receiving an DISCONNECT packet from the broker or if the on_disconnect is only
-        generated by the client library.
-        When true, the reason code is generated by the broker.
-    """
+    """Contains additional information passed to `on_disconnect` callback"""
 
     is_disconnect_packet_from_server: bool
+    """
+    tells whether this on_disconnect call is the result
+    of receiving an DISCONNECT packet from the broker or if the on_disconnect is only
+    generated by the client library.
+    When true, the reason code is generated by the broker.
+    """
 
 
 CallbackOnConnect_v1_mqtt3 = Callable[["Client", Any, Dict[str, Any], MQTTErrorCode], None]
-CallbackOnConnect_v1_mqtt5 = Callable[["Client", Any, Dict[str, Any], ReasonCodes, Union[Properties, None]], None]
+CallbackOnConnect_v1_mqtt5 = Callable[["Client", Any, Dict[str, Any], ReasonCode, Union[Properties, None]], None]
 CallbackOnConnect_v1 = Union[CallbackOnConnect_v1_mqtt5, CallbackOnConnect_v1_mqtt3]
-CallbackOnConnect_v2 = Callable[["Client", Any, ConnectFlags, ReasonCodes, Union[Properties, None]], None]
+CallbackOnConnect_v2 = Callable[["Client", Any, ConnectFlags, ReasonCode, Union[Properties, None]], None]
 CallbackOnConnect = Union[CallbackOnConnect_v1, CallbackOnConnect_v2]
 CallbackOnConnectFail = Callable[["Client", Any], None]
 CallbackOnDisconnect_v1_mqtt3 = Callable[["Client", Any, MQTTErrorCode], None]
-CallbackOnDisconnect_v1_mqtt5 = Callable[["Client", Any, Union[ReasonCodes, int, None], Union[Properties, None]], None]
+CallbackOnDisconnect_v1_mqtt5 = Callable[["Client", Any, Union[ReasonCode, int, None], Union[Properties, None]], None]
 CallbackOnDisconnect_v1 = Union[CallbackOnDisconnect_v1_mqtt3, CallbackOnDisconnect_v1_mqtt5]
-CallbackOnDisconnect_v2 = Callable[["Client", Any, DisconnectFlags, ReasonCodes, Union[Properties, None]], None]
+CallbackOnDisconnect_v2 = Callable[["Client", Any, DisconnectFlags, ReasonCode, Union[Properties, None]], None]
 CallbackOnDisconnect = Union[CallbackOnDisconnect_v1, CallbackOnDisconnect_v2]
 CallbackOnLog = Callable[["Client", Any, int, str], None]
 CallbackOnMessage = Callable[["Client", Any, "MQTTMessage"], None]
 CallbackOnPreConnect = Callable[["Client", Any], None]
 CallbackOnPublish_v1 = Callable[["Client", Any, int], None]
-CallbackOnPublish_v2 = Callable[["Client", Any, int, ReasonCodes, Properties], None]
+CallbackOnPublish_v2 = Callable[["Client", Any, int, ReasonCode, Properties], None]
 CallbackOnPublish = Union[CallbackOnPublish_v1, CallbackOnPublish_v2]
-CallbackOnSocket = Callable[["Client", Any, SocketLike], None]
+CallbackOnSocket = Callable[["Client", Any, "SocketLike"], None]
 CallbackOnSubscribe_v1_mqtt3 = Callable[["Client", Any, int, Tuple[int, ...]], None]
-CallbackOnSubscribe_v1_mqtt5 = Callable[["Client", Any, int, List[ReasonCodes], Properties], None]
+CallbackOnSubscribe_v1_mqtt5 = Callable[["Client", Any, int, List[ReasonCode], Properties], None]
 CallbackOnSubscribe_v1 = Union[CallbackOnSubscribe_v1_mqtt3, CallbackOnSubscribe_v1_mqtt5]
-CallbackOnSubscribe_v2 = Callable[["Client", Any, int, List[ReasonCodes], Union[Properties, None]], None]
+CallbackOnSubscribe_v2 = Callable[["Client", Any, int, List[ReasonCode], Union[Properties, None]], None]
 CallbackOnSubscribe = Union[CallbackOnSubscribe_v1, CallbackOnSubscribe_v2]
 CallbackOnUnsubscribe_v1_mqtt3 = Callable[["Client", Any, int], None]
-CallbackOnUnsubscribe_v1_mqtt5 = Callable[["Client", Any, int, Properties, Union[ReasonCodes, List[ReasonCodes]]], None]
+CallbackOnUnsubscribe_v1_mqtt5 = Callable[["Client", Any, int, Properties, Union[ReasonCode, List[ReasonCode]]], None]
 CallbackOnUnsubscribe_v1 = Union[CallbackOnUnsubscribe_v1_mqtt3, CallbackOnUnsubscribe_v1_mqtt5]
-CallbackOnUnsubscribe_v2 = Callable[["Client", Any, int, List[ReasonCodes], Union[Properties, None]], None]
+CallbackOnUnsubscribe_v2 = Callable[["Client", Any, int, List[ReasonCode], Union[Properties, None]], None]
 CallbackOnUnsubscribe = Union[CallbackOnUnsubscribe_v1, CallbackOnUnsubscribe_v2]
 
 # This is needed for typing because class Client redefined the name "socket"
 _socket = socket
 
 
 class WebsocketConnectionError(ConnectionError):
+    """ WebsocketConnectionError is a subclass of ConnectionError.
+
+        It's raised when unable to perform the Websocket handshake.
+    """
     pass
 
 
-def error_string(mqtt_errno: MQTTErrorCode) -> str:
+def error_string(mqtt_errno: MQTTErrorCode | int) -> str:
     """Return the error string associated with an mqtt error number."""
     if mqtt_errno == MQTT_ERR_SUCCESS:
         return "No error."
     elif mqtt_errno == MQTT_ERR_NOMEM:
         return "Out of memory."
     elif mqtt_errno == MQTT_ERR_PROTOCOL:
         return "A network protocol error occurred when communicating with the broker."
@@ -303,17 +324,17 @@
         return "Message queue full."
     elif mqtt_errno == MQTT_ERR_KEEPALIVE:
         return "Client or broker did not communicate in the keepalive interval."
     else:
         return "Unknown error."
 
 
-def connack_string(connack_code: int|ReasonCodes) -> str:
+def connack_string(connack_code: int|ReasonCode) -> str:
     """Return the string associated with a CONNACK result or CONNACK reason code."""
-    if isinstance(connack_code, ReasonCodes):
+    if isinstance(connack_code, ReasonCode):
         return str(connack_code)
 
     if connack_code == CONNACK_ACCEPTED:
         return "Connection Accepted."
     elif connack_code == CONNACK_REFUSED_PROTOCOL_VERSION:
         return "Connection Refused: unacceptable protocol version."
     elif connack_code == CONNACK_REFUSED_IDENTIFIER_REJECTED:
@@ -324,64 +345,70 @@
         return "Connection Refused: bad user name or password."
     elif connack_code == CONNACK_REFUSED_NOT_AUTHORIZED:
         return "Connection Refused: not authorised."
     else:
         return "Connection Refused: unknown reason."
 
 
-def convert_connack_rc_to_reason_code(connack_code: ConnackCode) -> ReasonCodes:
-    """Convert a MQTTv3 / MQTTv3.1.1 connack result to Reason code.
+def convert_connack_rc_to_reason_code(connack_code: ConnackCode) -> ReasonCode:
+    """Convert a MQTTv3 / MQTTv3.1.1 connack result to `ReasonCode`.
+
+    This is used in `on_connect` callback to have a consistent API.
 
     Be careful that the numeric value isn't the same, for example:
+
     >>> ConnackCode.CONNACK_REFUSED_SERVER_UNAVAILABLE == 3
     >>> convert_connack_rc_to_reason_code(ConnackCode.CONNACK_REFUSED_SERVER_UNAVAILABLE) == 136
 
     It's recommended to compare by names
-    >>> code_to_test = ReasonCodes(PacketTypes.CONNACK, "Server unavailable")
+
+    >>> code_to_test = ReasonCode(PacketTypes.CONNACK, "Server unavailable")
     >>> convert_connack_rc_to_reason_code(ConnackCode.CONNACK_REFUSED_SERVER_UNAVAILABLE) == code_to_test
     """
     if connack_code == ConnackCode.CONNACK_ACCEPTED:
-        return ReasonCodes(PacketTypes.CONNACK, "Success")
+        return ReasonCode(PacketTypes.CONNACK, "Success")
     if connack_code == ConnackCode.CONNACK_REFUSED_PROTOCOL_VERSION:
-        return ReasonCodes(PacketTypes.CONNACK, "Unsupported protocol version")
+        return ReasonCode(PacketTypes.CONNACK, "Unsupported protocol version")
     if connack_code == ConnackCode.CONNACK_REFUSED_IDENTIFIER_REJECTED:
-        return ReasonCodes(PacketTypes.CONNACK, "Client identifier not valid")
+        return ReasonCode(PacketTypes.CONNACK, "Client identifier not valid")
     if connack_code == ConnackCode.CONNACK_REFUSED_SERVER_UNAVAILABLE:
-        return ReasonCodes(PacketTypes.CONNACK, "Server unavailable")
+        return ReasonCode(PacketTypes.CONNACK, "Server unavailable")
     if connack_code == ConnackCode.CONNACK_REFUSED_BAD_USERNAME_PASSWORD:
-        return ReasonCodes(PacketTypes.CONNACK, "Bad user name or password")
+        return ReasonCode(PacketTypes.CONNACK, "Bad user name or password")
     if connack_code == ConnackCode.CONNACK_REFUSED_NOT_AUTHORIZED:
-        return ReasonCodes(PacketTypes.CONNACK, "Not authorized")
+        return ReasonCode(PacketTypes.CONNACK, "Not authorized")
 
-    return ReasonCodes(PacketTypes.CONNACK, "Unspecified error")
+    return ReasonCode(PacketTypes.CONNACK, "Unspecified error")
 
 
-def convert_disconnect_error_code_to_reason_code(rc: MQTTErrorCode) -> ReasonCodes:
+def convert_disconnect_error_code_to_reason_code(rc: MQTTErrorCode) -> ReasonCode:
     """Convert an MQTTErrorCode to Reason code.
 
-    This is used in on_disconnect callback to have a consistent API.
+    This is used in `on_disconnect` callback to have a consistent API.
 
     Be careful that the numeric value isn't the same, for example:
+
     >>> MQTTErrorCode.MQTT_ERR_PROTOCOL == 2
     >>> convert_disconnect_error_code_to_reason_code(MQTTErrorCode.MQTT_ERR_PROTOCOL) == 130
 
     It's recommended to compare by names
-    >>> code_to_test = ReasonCodes(PacketTypes.DISCONNECT, "Protocol error")
+
+    >>> code_to_test = ReasonCode(PacketTypes.DISCONNECT, "Protocol error")
     >>> convert_disconnect_error_code_to_reason_code(MQTTErrorCode.MQTT_ERR_PROTOCOL) == code_to_test
     """
     if rc == MQTTErrorCode.MQTT_ERR_SUCCESS:
-        return ReasonCodes(PacketTypes.DISCONNECT, "Success")
+        return ReasonCode(PacketTypes.DISCONNECT, "Success")
     if rc == MQTTErrorCode.MQTT_ERR_KEEPALIVE:
-        return ReasonCodes(PacketTypes.DISCONNECT, "Keep alive timeout")
+        return ReasonCode(PacketTypes.DISCONNECT, "Keep alive timeout")
     if rc == MQTTErrorCode.MQTT_ERR_CONN_LOST:
-        return ReasonCodes(PacketTypes.DISCONNECT, "Unspecified error")
-    return ReasonCodes(PacketTypes.DISCONNECT, "Unspecified error")
+        return ReasonCode(PacketTypes.DISCONNECT, "Unspecified error")
+    return ReasonCode(PacketTypes.DISCONNECT, "Unspecified error")
 
 
-def base62(
+def _base62(
     num: int,
     base: str = string.digits + string.ascii_letters,
     padding: int = 1,
 ) -> str:
     """Convert a number to base-62 representation."""
     if num < 0:
         raise ValueError("Number must be positive or zero")
@@ -394,16 +421,16 @@
 
 
 def topic_matches_sub(sub: str, topic: str) -> bool:
     """Check whether a topic matches a subscription.
 
     For example:
 
-    foo/bar would match the subscription foo/# or +/bar
-    non/matching would not match the subscription non/+/+
+    * Topic "foo/bar" would match the subscription "foo/#" or "+/bar"
+    * Topic "non/matching" would not match the subscription "non/+/+"
     """
     matcher = MQTTMatcher()
     matcher[sub] = True
     try:
         next(matcher.iter_match(topic))
         return True
     except StopIteration:
@@ -434,15 +461,15 @@
 
 def _force_bytes(s: str | bytes) -> bytes:
     if isinstance(s, str):
         return s.encode("utf-8")
     return s
 
 
-def _encode_payload(payload: str | bytes | bytearray | int | float | None) -> bytes:
+def _encode_payload(payload: str | bytes | bytearray | int | float | None) -> bytes|bytearray:
     if isinstance(payload, str):
         return payload.encode("utf-8")
 
     if isinstance(payload, (int, float)):
         return str(payload).encode("ascii")
 
     if payload is None:
@@ -453,26 +480,29 @@
             "payload must be a string, bytearray, int, float or None."
         )
 
     return payload
 
 
 class MQTTMessageInfo:
-    """This is a class returned from Client.publish() and can be used to find
+    """This is a class returned from `Client.publish()` and can be used to find
     out the mid of the message that was published, and to determine whether the
     message has been published, and/or wait until it is published.
     """
 
     __slots__ = 'mid', '_published', '_condition', 'rc', '_iterpos'
 
     def __init__(self, mid: int):
         self.mid = mid
+        """ The message Id (int)"""
         self._published = False
         self._condition = threading.Condition()
         self.rc: MQTTErrorCode = MQTTErrorCode.MQTT_ERR_SUCCESS
+        """ The `MQTTErrorCode` that give status for this message.
+        This value could change until the message `is_published`"""
         self._iterpos = 0
 
     def __str__(self) -> str:
         return str((self.rc, self.mid))
 
     def __iter__(self) -> Iterator[MQTTErrorCode | int]:
         self._iterpos = 0
@@ -506,19 +536,19 @@
 
     def wait_for_publish(self, timeout: float | None = None) -> None:
         """Block until the message associated with this object is published, or
         until the timeout occurs. If timeout is None, this will never time out.
         Set timeout to a positive number of seconds, e.g. 1.2, to enable the
         timeout.
 
-        Raises ValueError if the message was not queued due to the outgoing
-        queue being full.
+        :raises ValueError: if the message was not queued due to the outgoing
+            queue being full.
 
-        Raises RuntimeError if the message was not published for another
-        reason.
+        :raises RuntimeError: if the message was not published for another
+            reason.
         """
         if self.rc == MQTT_ERR_QUEUE_SIZE:
             raise ValueError('Message is not queued due to ERR_QUEUE_SIZE')
         elif self.rc == MQTT_ERR_AGAIN:
             pass
         elif self.rc > 0:
             raise RuntimeError(f'Message publish failed: {error_string(self.rc)}')
@@ -533,194 +563,194 @@
                 self._condition.wait(timeout_tenth)
 
         if self.rc > 0:
             raise RuntimeError(f'Message publish failed: {error_string(self.rc)}')
 
     def is_published(self) -> bool:
         """Returns True if the message associated with this object has been
-        published, else returns False."""
+        published, else returns False.
+
+        To wait for this to become true, look at `wait_for_publish`.
+        """
         if self.rc == MQTTErrorCode.MQTT_ERR_QUEUE_SIZE:
             raise ValueError('Message is not queued due to ERR_QUEUE_SIZE')
         elif self.rc == MQTTErrorCode.MQTT_ERR_AGAIN:
             pass
         elif self.rc > 0:
             raise RuntimeError(f'Message publish failed: {error_string(self.rc)}')
 
         with self._condition:
             return self._published
 
 
 class MQTTMessage:
-    """ This is a class that describes an incoming or outgoing message. It is
-    passed to the on_message callback as the message parameter.
-
-    Members:
-
-    topic : String. topic that the message was published on.
-    payload : Bytes/Byte array. the message payload.
-    qos : Integer. The message Quality of Service 0, 1 or 2.
-    retain : Boolean. If true, the message is a retained message and not fresh.
-    mid : Integer. The message id.
-    properties: Properties class. In MQTT v5.0, the properties associated with the message.
+    """ This is a class that describes an incoming message. It is
+    passed to the `on_message` callback as the message parameter.
     """
-
     __slots__ = 'timestamp', 'state', 'dup', 'mid', '_topic', 'payload', 'qos', 'retain', 'info', 'properties'
 
     def __init__(self, mid: int = 0, topic: bytes = b""):
         self.timestamp = 0.0
         self.state = mqtt_ms_invalid
         self.dup = False
         self.mid = mid
+        """ The message id (int)."""
         self._topic = topic
         self.payload = b""
+        """the message payload (bytes)"""
         self.qos = 0
+        """ The message Quality of Service (0, 1 or 2)."""
         self.retain = False
+        """ If true, the message is a retained message and not fresh."""
         self.info = MQTTMessageInfo(mid)
         self.properties: Properties | None = None
+        """ In MQTT v5.0, the properties associated with the message. (`Properties`)"""
 
     def __eq__(self, other: object) -> bool:
         """Override the default Equals behavior"""
         if isinstance(other, self.__class__):
             return self.mid == other.mid
         return False
 
     def __ne__(self, other: object) -> bool:
         """Define a non-equality test"""
         return not self.__eq__(other)
 
     @property
     def topic(self) -> str:
+        """topic that the message was published on.
+
+        This property is read-only.
+        """
         return self._topic.decode('utf-8')
 
     @topic.setter
     def topic(self, value: bytes) -> None:
         self._topic = value
 
 
 class Client:
     """MQTT version 3.1/3.1.1/5.0 client class.
 
     This is the main class for use communicating with an MQTT broker.
 
     General usage flow:
 
-    * Use connect()/connect_async() to connect to a broker
-    * Call loop() frequently to maintain network traffic flow with the broker
-    * Or use loop_start() to set a thread running to call loop() for you.
-    * Or use loop_forever() to handle calling loop() for you in a blocking
-    * function.
-    * Use subscribe() to subscribe to a topic and receive messages
-    * Use publish() to send messages
-    * Use disconnect() to disconnect from the broker
+    * Use `connect()`, `connect_async()` or `connect_srv()` to connect to a broker
+    * Use `loop_start()` to set a thread running to call `loop()` for you.
+    * Or use `loop_forever()` to handle calling `loop()` for you in a blocking function.
+    * Or call `loop()` frequently to maintain network traffic flow with the broker
+    * Use `subscribe()` to subscribe to a topic and receive messages
+    * Use `publish()` to send messages
+    * Use `disconnect()` to disconnect from the broker
 
     Data returned from the broker is made available with the use of callback
     functions as described below.
 
-    Callbacks
-    =========
-
-    A number of callback functions are available to receive data back from the
-    broker. To use a callback, define a function and then assign it to the
-    client:
-
-    def on_connect(client, userdata, flags, rc):
-        print("Connection returned " + str(rc))
-
-    client.on_connect = on_connect
-
-    Callbacks can also be attached using decorators:
-
-    client = paho.mqtt.Client()
-
-    @client.connect_callback()
-    def on_connect(client, userdata, flags, rc):
-        print("Connection returned " + str(rc))
-
-
-    **IMPORTANT** the required function signature for a callback can differ
-    depending on whether you are using MQTT v5 or MQTT v3.1.1/v3.1. See the
-    documentation for each callback.
-
-    All of the callbacks as described below have a "client" and an "userdata"
-    argument. "client" is the Client instance that is calling the callback.
-    "userdata" is user data of any type and can be set when creating a new client
-    instance or with user_data_set(userdata).
-
-    If you wish to suppress exceptions within a callback, you should set
-    `client.suppress_exceptions = True`
-
-    The callbacks are listed below, documentation for each of them can be found
-    at the same function name:
-
-    on_connect, on_connect_fail, on_disconnect, on_message, on_publish,
-    on_subscribe, on_unsubscribe, on_log, on_socket_open, on_socket_close,
-    on_socket_register_write, on_socket_unregister_write
-    """
-
-    def __init__(
-        self,
-        callback_api_version: CallbackAPIVersion,
-        client_id: str = "",
-        clean_session: bool | None = None,
-        userdata: Any = None,
-        protocol: int = MQTTv311,
-        transport: Literal["tcp", "websockets"] = "tcp",
-        reconnect_on_failure: bool = True,
-        manual_ack: bool = False,
-    ) -> None:
-        """
-        callback_api_version define the API version for user-callback (on_connect, on_publish,...).
+    :param CallbackAPIVersion callback_api_version: define the API version for user-callback (on_connect, on_publish,...).
         This field is required and it's recommended to use the latest version (CallbackAPIVersion.API_VERSION2).
-        See each callback for description of API for each version. The file migrations.md contains details on
+        See each callback for description of API for each version. The file docs/migrations.rst contains details on
         how to migrate between version.
 
-        client_id is the unique client id string used when connecting to the
+    :param str client_id: the unique client id string used when connecting to the
         broker. If client_id is zero length or None, then the behaviour is
         defined by which protocol version is in use. If using MQTT v3.1.1, then
         a zero length client id will be sent to the broker and the broker will
         generate a random for the client. If using MQTT v3.1 then an id will be
         randomly generated. In both cases, clean_session must be True. If this
         is not the case a ValueError will be raised.
 
-        clean_session is a boolean that determines the client type. If True,
+    :param bool clean_session: a boolean that determines the client type. If True,
         the broker will remove all information about this client when it
         disconnects. If False, the client is a persistent client and
         subscription information and queued messages will be retained when the
         client disconnects.
         Note that a client will never discard its own outgoing messages on
         disconnect. Calling connect() or reconnect() will cause the messages to
         be resent.  Use reinitialise() to reset a client to its original state.
         The clean_session argument only applies to MQTT versions v3.1.1 and v3.1.
         It is not accepted if the MQTT version is v5.0 - use the clean_start
         argument on connect() instead.
 
-        userdata is user defined data of any type that is passed as the "userdata"
+    :param userdata: user defined data of any type that is passed as the "userdata"
         parameter to callbacks. It may be updated at a later point with the
         user_data_set() function.
 
-        The protocol argument allows explicit setting of the MQTT version to
+    :param int protocol: allows explicit setting of the MQTT version to
         use for this client. Can be paho.mqtt.client.MQTTv311 (v3.1.1),
         paho.mqtt.client.MQTTv31 (v3.1) or paho.mqtt.client.MQTTv5 (v5.0),
         with the default being v3.1.1.
 
-        Set transport to "websockets" to use WebSockets as the transport
+    :param transport: use "websockets" to use WebSockets as the transport
         mechanism. Set to "tcp" to use raw TCP, which is the default.
+        Use "unix" to use Unix sockets as the transport mechanism; note that
+        this option is only available on platforms that support Unix sockets,
+        and the "host" argument is interpreted as the path to the Unix socket
+        file in this case.
 
-        Normally, when a message is received, the library automatically
+    :param bool manual_ack: normally, when a message is received, the library automatically
         acknowledges after on_message callback returns.  manual_ack=True allows the application to
         acknowledge receipt after it has completed processing of a message
         using a the ack() method. This addresses vulnerability to message loss
         if applications fails while processing a message, or while it pending
         locally.
 
-        """
+    Callbacks
+    =========
+
+    A number of callback functions are available to receive data back from the
+    broker. To use a callback, define a function and then assign it to the
+    client::
+
+        def on_connect(client, userdata, flags, reason_code, properties):
+            print(f"Connected with result code {reason_code}")
+
+        client.on_connect = on_connect
+
+    Callbacks can also be attached using decorators::
+
+        mqttc = paho.mqtt.Client()
+
+        @mqttc.connect_callback()
+        def on_connect(client, userdata, flags, reason_code, properties):
+            print(f"Connected with result code {reason_code}")
+
+    All of the callbacks as described below have a "client" and an "userdata"
+    argument. "client" is the `Client` instance that is calling the callback.
+    userdata" is user data of any type and can be set when creating a new client
+    instance or with `user_data_set()`.
+
+    If you wish to suppress exceptions within a callback, you should set
+    ``mqttc.suppress_exceptions = True``
+
+    The callbacks are listed below, documentation for each of them can be found
+    at the same function name:
+
+    `on_connect`, `on_connect_fail`, `on_disconnect`, `on_message`, `on_publish`,
+    `on_subscribe`, `on_unsubscribe`, `on_log`, `on_socket_open`, `on_socket_close`,
+    `on_socket_register_write`, `on_socket_unregister_write`
+    """
+
+    def __init__(
+        self,
+        callback_api_version: CallbackAPIVersion = CallbackAPIVersion.VERSION1,
+        client_id: str | None = "",
+        clean_session: bool | None = None,
+        userdata: Any = None,
+        protocol: MQTTProtocolVersion = MQTTv311,
+        transport: Literal["tcp", "websockets", "unix"] = "tcp",
+        reconnect_on_failure: bool = True,
+        manual_ack: bool = False,
+    ) -> None:
         transport = transport.lower()  # type: ignore
-        if transport not in ("websockets", "tcp"):
+        if transport == "unix" and not hasattr(socket, "AF_UNIX"):
+            raise ValueError('"unix" transport not supported')
+        elif transport not in ("websockets", "tcp", "unix"):
             raise ValueError(
-                f'transport must be "websockets" or "tcp", not {transport}')
+                f'transport must be "websockets", "tcp" or "unix", not {transport}')
 
         self._manual_ack = manual_ack
         self._transport = transport
         self._protocol = protocol
         self._userdata = userdata
         self._sock: SocketLike | None = None
         self._sockpairR: socket.socket | None = None
@@ -736,15 +766,15 @@
                 category=DeprecationWarning,
                 stacklevel=2,
             )
         if isinstance(self._callback_api_version, str):
             # Help user to migrate, it probably provided a client id
             # as first arguments
             raise ValueError(
-                "Unsupported callback API version: version 2.0 added a callback_api_version, see migrations.md for details"
+                "Unsupported callback API version: version 2.0 added a callback_api_version, see docs/migrations.rst for details"
             )
         if self._callback_api_version not in CallbackAPIVersion:
             raise ValueError("Unsupported callback API version")
 
         self._clean_start: int = MQTT_CLEAN_START_FIRST_ONLY
 
         if protocol == MQTTv5:
@@ -757,15 +787,15 @@
                 raise ValueError(
                     'A client id must be provided if clean session is False.')
             self._clean_session = clean_session
 
         # [MQTT-3.1.3-4] Client Id must be UTF-8 encoded string.
         if client_id == "" or client_id is None:
             if protocol == MQTTv31:
-                self._client_id = base62(uuid.uuid4().int, padding=22).encode("utf8")
+                self._client_id = _base62(uuid.uuid4().int, padding=22).encode("utf8")
             else:
                 self._client_id = b""
         else:
             self._client_id = _force_bytes(client_id)
 
         self._username: bytes | None = None
         self._password: bytes | None = None
@@ -784,15 +814,15 @@
         self._last_msg_out = time_func()
         self._reconnect_min_delay = 1
         self._reconnect_max_delay = 120
         self._reconnect_delay: int | None = None
         self._reconnect_on_failure = reconnect_on_failure
         self._ping_t = 0.0
         self._last_mid = 0
-        self._state = ConnectionState.MQTT_CS_NEW
+        self._state = _ConnectionState.MQTT_CS_NEW
         self._out_messages: collections.OrderedDict[
             int, MQTTMessage
         ] = collections.OrderedDict()
         self._in_messages: collections.OrderedDict[
             int, MQTTMessage
         ] = collections.OrderedDict()
         self._max_inflight_messages = 20
@@ -847,187 +877,213 @@
         self.suppress_exceptions = False # For callbacks
 
     def __del__(self) -> None:
         self._reset_sockets()
 
     @property
     def host(self) -> str:
-        """Host to connect to. If `connect()` hasn't been called yet, returns an empty string."""
+        """
+        Host to connect to. If `connect()` hasn't been called yet, returns an empty string.
+
+        This property may not be changed if the connection is already open.
+        """
         return self._host
 
     @host.setter
     def host(self, value: str) -> None:
-        """
-        Update host. This may not be called if the connection is already open.
-        """
         if not self._connection_closed():
             raise RuntimeError("updating host on established connection is not supported")
 
         if not value:
             raise ValueError("Invalid host.")
         self._host = value
 
     @property
     def port(self) -> int:
-        """Broker TCP port to connect to."""
+        """
+        Broker TCP port to connect to.
+
+        This property may not be changed if the connection is already open.
+        """
         return self._port
 
     @port.setter
     def port(self, value: int) -> None:
-        """
-        Update port. This may not be called if the connection is already open.
-        """
         if not self._connection_closed():
             raise RuntimeError("updating port on established connection is not supported")
 
         if value <= 0:
             raise ValueError("Invalid port number.")
         self._port = value
 
     @property
     def keepalive(self) -> int:
-        """Client keepalive interval (in seconds)."""
+        """
+        Client keepalive interval (in seconds).
+
+        This property may not be changed if the connection is already open.
+        """
         return self._keepalive
 
     @keepalive.setter
     def keepalive(self, value: int) -> None:
-        """Update the client keepalive interval. This may not be called if the connection is already open."""
         if not self._connection_closed():
             # The issue here is that the previous value of keepalive matter to possibly
             # sent ping packet.
             raise RuntimeError("updating keepalive on established connection is not supported")
 
         if value < 0:
             raise ValueError("Keepalive must be >=0.")
 
         self._keepalive = value
 
     @property
-    def transport(self) -> Literal["tcp", "websockets"]:
-        """Transport method used for the connection."""
+    def transport(self) -> Literal["tcp", "websockets", "unix"]:
+        """
+        Transport method used for the connection ("tcp" or "websockets").
+
+        This property may not be changed if the connection is already open.
+        """
         return self._transport
 
     @transport.setter
     def transport(self, value: Literal["tcp", "websockets"]) -> None:
-        """
-        Update transport which should be "tcp" or "websockets".
-        This may not be called if the connection is already open.
-        """
         if not self._connection_closed():
             raise RuntimeError("updating transport on established connection is not supported")
 
         self._transport = value
 
     @property
     def protocol(self) -> MQTTProtocolVersion:
-        """Protocol version used (MQTT v3, MQTT v3.11, MQTTv5)"""
-        return self.protocol
+        """
+        Protocol version used (MQTT v3, MQTT v3.11, MQTTv5)
+
+        This property is read-only.
+        """
+        return self._protocol
 
     @property
     def connect_timeout(self) -> float:
-        """Connection establishment timeout in seconds"""
+        """
+        Connection establishment timeout in seconds.
+
+        This property may not be changed if the connection is already open.
+        """
         return self._connect_timeout
 
     @connect_timeout.setter
     def connect_timeout(self, value: float) -> None:
-        "Change connect_timeout. This may not be called if the connection is already open."
         if not self._connection_closed():
             raise RuntimeError("updating connect_timeout on established connection is not supported")
 
         if value <= 0.0:
             raise ValueError("timeout must be a positive number")
 
         self._connect_timeout = value
 
     @property
     def username(self) -> str | None:
-        """The username used to connect to the MQTT broker, or None if no username is used."""
+        """The username used to connect to the MQTT broker, or None if no username is used.
+
+        This property may not be changed if the connection is already open.
+        """
         if self._username is None:
             return None
         return self._username.decode("utf-8")
 
     @username.setter
     def username(self, value: str | None) -> None:
-        """
-        Update username. This may not be called if the connection is already open.
-        """
         if not self._connection_closed():
             raise RuntimeError("updating username on established connection is not supported")
 
         if value is None:
             self._username = None
         else:
             self._username = value.encode("utf-8")
 
     @property
     def password(self) -> str | None:
-        """The password used to connect to the MQTT broker, or None if no password is used."""
+        """The password used to connect to the MQTT broker, or None if no password is used.
+
+        This property may not be changed if the connection is already open.
+        """
         if self._password is None:
             return None
         return self._password.decode("utf-8")
 
     @password.setter
     def password(self, value: str | None) -> None:
-        """
-        Update password. This may not be called if the connection is already open.
-        """
         if not self._connection_closed():
             raise RuntimeError("updating password on established connection is not supported")
 
         if value is None:
             self._password = None
         else:
             self._password = value.encode("utf-8")
 
     @property
     def max_inflight_messages(self) -> int:
-        """Maximum number of messages with QoS > 0 that can be partway through the network flow at once"""
+        """
+        Maximum number of messages with QoS > 0 that can be partway through the network flow at once
+
+        This property may not be changed if the connection is already open.
+        """
         return self._max_inflight_messages
 
     @max_inflight_messages.setter
     def max_inflight_messages(self, value: int) -> None:
-        "Update max_inflight_messages. This may not be called if the connection is already open."
         if not self._connection_closed():
             # Not tested. Some doubt that everything is okay when max_inflight change between 0
             # and > 0 value because _update_inflight is skipped when _max_inflight_messages == 0
             raise RuntimeError("updating max_inflight_messages on established connection is not supported")
 
         if value < 0:
             raise ValueError("Invalid inflight.")
 
         self._max_inflight_messages = value
 
     @property
     def max_queued_messages(self) -> int:
-        """Maximum number of message in the outgoing message queue, 0 means unlimited"""
+        """
+        Maximum number of message in the outgoing message queue, 0 means unlimited
+
+        This property may not be changed if the connection is already open.
+        """
         return self._max_queued_messages
 
     @max_queued_messages.setter
     def max_queued_messages(self, value: int) -> None:
-        "Update max_queued_messages. This may not be called if the connection is already open."
         if not self._connection_closed():
             # Not tested.
             raise RuntimeError("updating max_queued_messages on established connection is not supported")
 
         if value < 0:
             raise ValueError("Invalid queue size.")
 
         self._max_queued_messages = value
 
     @property
     def will_topic(self) -> str | None:
-        """The topic name a will message is sent to when disconnecting unexpectedly. None if a will shall not be sent."""
+        """
+        The topic name a will message is sent to when disconnecting unexpectedly. None if a will shall not be sent.
+
+        This property is read-only. Use `will_set()` to change its value.
+        """
         if self._will_topic is None:
             return None
 
         return self._will_topic.decode("utf-8")
 
     @property
     def will_payload(self) -> bytes | None:
-        """The payload for the will message that is sent when disconnecting unexpectedly. None if a will shall not be sent."""
+        """
+        The payload for the will message that is sent when disconnecting unexpectedly. None if a will shall not be sent.
+
+        This property is read-only. Use `will_set()` to change its value.
+        """
         return self._will_payload
 
     @property
     def logger(self) -> logging.Logger | None:
         return self._logger
 
     @logger.setter
@@ -1102,21 +1158,21 @@
     def ws_set_options(
         self,
         path: str = "/mqtt",
         headers: WebSocketHeaders | None = None,
     ) -> None:
         """ Set the path and headers for a websocket connection
 
-        path is a string starting with / which should be the endpoint of the
-        mqtt connection on the remote server
+        :param str path: a string starting with / which should be the endpoint of the
+            mqtt connection on the remote server
 
-        headers can be either a dict or a callable object. If it is a dict then
-        the extra items in the dict are added to the websocket headers. If it is
-        a callable, then the default websocket headers are passed into this
-        function and the result is used as the new headers.
+        :param headers:  can be either a dict or a callable object. If it is a dict then
+            the extra items in the dict are added to the websocket headers. If it is
+            a callable, then the default websocket headers are passed into this
+            function and the result is used as the new headers.
         """
         self._websocket_path = path
 
         if headers is not None:
             if isinstance(headers, dict) or callable(headers):
                 self._websocket_extra_headers = headers
             else:
@@ -1125,18 +1181,18 @@
 
     def tls_set_context(
         self,
         context: ssl.SSLContext | None = None,
     ) -> None:
         """Configure network encryption and authentication context. Enables SSL/TLS support.
 
-        context : an ssl.SSLContext object. By default this is given by
-        `ssl.create_default_context()`, if available.
+        :param context: an ssl.SSLContext object. By default this is given by
+            ``ssl.create_default_context()``, if available.
 
-        Must be called before connect() or connect_async()."""
+        Must be called before `connect()`, `connect_async()` or `connect_srv()`."""
         if self._ssl_context is not None:
             raise ValueError('SSL/TLS has already been configured.')
 
         if context is None:
             context = ssl.create_default_context()
 
         self._ssl = True
@@ -1155,51 +1211,54 @@
         tls_version: int | None = None,
         ciphers: str | None = None,
         keyfile_password: str | None = None,
         alpn_protocols: list[str] | None = None,
     ) -> None:
         """Configure network encryption and authentication options. Enables SSL/TLS support.
 
-        ca_certs : a string path to the Certificate Authority certificate files
-        that are to be treated as trusted by this client. If this is the only
-        option given then the client will operate in a similar manner to a web
-        browser. That is to say it will require the broker to have a
-        certificate signed by the Certificate Authorities in ca_certs and will
-        communicate using TLS v1,2, but will not attempt any form of
-        authentication. This provides basic network encryption but may not be
-        sufficient depending on how the broker is configured.
-        By default, on Python 2.7.9+ or 3.4+, the default certification
-        authority of the system is used. On older Python version this parameter
-        is mandatory.
-
-        certfile and keyfile are strings pointing to the PEM encoded client
-        certificate and private keys respectively. If these arguments are not
-        None then they will be used as client information for TLS based
-        authentication.  Support for this feature is broker dependent. Note
-        that if either of these files in encrypted and needs a password to
-        decrypt it, then this can be passed using the keyfile_password
-        argument - you should take precautions to ensure that your password is
-        not hard coded into your program by loading the password from a file
-        for example. If you do not provide keyfile_password, the password will
-        be requested to be typed in at a terminal window.
-
-        cert_reqs allows the certificate requirements that the client imposes
-        on the broker to be changed. By default this is ssl.CERT_REQUIRED,
-        which means that the broker must provide a certificate. See the ssl
-        pydoc for more information on this parameter.
-
-        tls_version allows the version of the SSL/TLS protocol used to be
-        specified. By default TLS v1.2 is used. Previous versions are allowed
-        but not recommended due to possible security problems.
-
-        ciphers is a string specifying which encryption ciphers are allowable
-        for this connection, or None to use the defaults. See the ssl pydoc for
-        more information.
+        :param str ca_certs: a string path to the Certificate Authority certificate files
+            that are to be treated as trusted by this client. If this is the only
+            option given then the client will operate in a similar manner to a web
+            browser. That is to say it will require the broker to have a
+            certificate signed by the Certificate Authorities in ca_certs and will
+            communicate using TLS v1,2, but will not attempt any form of
+            authentication. This provides basic network encryption but may not be
+            sufficient depending on how the broker is configured.
+
+            By default, on Python 2.7.9+ or 3.4+, the default certification
+            authority of the system is used. On older Python version this parameter
+            is mandatory.
+        :param str certfile: PEM encoded client certificate filename. Used with
+            keyfile for client TLS based authentication. Support for this feature is
+            broker dependent. Note that if the files in encrypted and needs a password to
+            decrypt it, then this can be passed using the keyfile_password argument - you
+            should take precautions to ensure that your password is
+            not hard coded into your program by loading the password from a file
+            for example. If you do not provide keyfile_password, the password will
+            be requested to be typed in at a terminal window.
+        :param str keyfile: PEM encoded client private keys filename. Used with
+            certfile for client TLS based authentication. Support for this feature is
+            broker dependent. Note that if the files in encrypted and needs a password to
+            decrypt it, then this can be passed using the keyfile_password argument - you
+            should take precautions to ensure that your password is
+            not hard coded into your program by loading the password from a file
+            for example. If you do not provide keyfile_password, the password will
+            be requested to be typed in at a terminal window.
+        :param cert_reqs: the certificate requirements that the client imposes
+            on the broker to be changed. By default this is ssl.CERT_REQUIRED,
+            which means that the broker must provide a certificate. See the ssl
+            pydoc for more information on this parameter.
+        :param tls_version: the version of the SSL/TLS protocol used to be
+            specified. By default TLS v1.2 is used. Previous versions are allowed
+            but not recommended due to possible security problems.
+        :param str ciphers: encryption ciphers that are allowed
+            for this connection, or None to use the defaults. See the ssl pydoc for
+            more information.
 
-        Must be called before connect() or connect_async()."""
+        Must be called before `connect()`, `connect_async()` or `connect_srv()`."""
         if ssl is None:
             raise ValueError('This platform has no SSL/TLS.')
 
         if not hasattr(ssl, 'SSLContext'):
             # Require Python version that has SSL context support in standard library
             raise ValueError(
                 'Python 2.7.9 and 3.2 are the minimum supported versions for TLS.')
@@ -1258,16 +1317,16 @@
         useful in initial server testing, but makes it possible for a malicious
         third party to impersonate your server through DNS spoofing, for
         example.
 
         Do not use this function in a real system. Setting value to true means
         there is no point using encryption.
 
-        Must be called before connect() and after either tls_set() or
-        tls_set_context()."""
+        Must be called before `connect()` and after either `tls_set()` or
+        `tls_set_context()`."""
 
         if self._ssl_context is None:
             raise ValueError(
                 'Must configure SSL context before using tls_insecure_set.')
 
         self._tls_insecure = value
 
@@ -1281,71 +1340,90 @@
         """Configure proxying of MQTT connection. Enables support for SOCKS or
         HTTP proxies.
 
         Proxying is done through the PySocks library. Brief descriptions of the
         proxy_args parameters are below; see the PySocks docs for more info.
 
         (Required)
-        proxy_type: One of {socks.HTTP, socks.SOCKS4, or socks.SOCKS5}
-        proxy_addr: IP address or DNS name of proxy server
+
+        :param proxy_type: One of {socks.HTTP, socks.SOCKS4, or socks.SOCKS5}
+        :param proxy_addr: IP address or DNS name of proxy server
 
         (Optional)
-        proxy_port: (int) port number of the proxy server. If not provided,
+
+        :param proxy_port: (int) port number of the proxy server. If not provided,
             the PySocks package default value will be utilized, which differs by proxy_type.
-        proxy_rdns: boolean indicating whether proxy lookup should be performed
+        :param proxy_rdns: boolean indicating whether proxy lookup should be performed
             remotely (True, default) or locally (False)
-        proxy_username: username for SOCKS5 proxy, or userid for SOCKS4 proxy
-        proxy_password: password for SOCKS5 proxy
+        :param proxy_username: username for SOCKS5 proxy, or userid for SOCKS4 proxy
+        :param proxy_password: password for SOCKS5 proxy
+
+        Example::
 
-        Must be called before connect() or connect_async()."""
+            mqttc.proxy_set(proxy_type=socks.HTTP, proxy_addr='1.2.3.4', proxy_port=4231)
+        """
         if socks is None:
             raise ValueError("PySocks must be installed for proxy support.")
         elif not self._proxy_is_valid(proxy_args):
             raise ValueError("proxy_type and/or proxy_addr are invalid.")
         else:
             self._proxy = proxy_args
 
     def enable_logger(self, logger: logging.Logger | None = None) -> None:
-        """ Enables a logger to send log messages to """
+        """
+        Enables a logger to send log messages to
+
+        :param logging.Logger logger: if specified, that ``logging.Logger`` object will be used, otherwise
+            one will be created automatically.
+
+        See `disable_logger` to undo this action.
+        """
         if logger is None:
             if self._logger is not None:
                 # Do not replace existing logger
                 return
             logger = logging.getLogger(__name__)
         self.logger = logger
 
     def disable_logger(self) -> None:
+        """
+        Disable logging using standard python logging package. This has no effect on the `on_log` callback.
+        """
         self._logger = None
 
     def connect(
         self,
         host: str,
         port: int = 1883,
         keepalive: int = 60,
         bind_address: str = "",
         bind_port: int = 0,
         clean_start: CleanStartOption = MQTT_CLEAN_START_FIRST_ONLY,
         properties: Properties | None = None,
     ) -> MQTTErrorCode:
         """Connect to a remote broker. This is a blocking call that establishes
         the underlying connection and transmits a CONNECT packet.
+        Note that the connection status will not be updated until a CONNACK is received and
+        processed (this requires a running network loop, see `loop_start`, `loop_forever`, `loop`...).
 
-        host is the hostname or IP address of the remote broker.
-        port is the network port of the server host to connect to. Defaults to
-        1883. Note that the default port for MQTT over SSL/TLS is 8883 so if you
-        are using tls_set() the port may need providing.
-        keepalive: Maximum period in seconds between communications with the
-        broker. If no other messages are being exchanged, this controls the
-        rate at which the client will send ping messages to the broker.
-        clean_start: (MQTT v5.0 only) True, False or MQTT_CLEAN_START_FIRST_ONLY.
-        Sets the MQTT v5.0 clean_start flag always, never or on the first successful connect only,
-        respectively.  MQTT session data (such as outstanding messages and subscriptions)
-        is cleared on successful connect when the clean_start flag is set.
-        properties: (MQTT v5.0 only) the MQTT v5.0 properties to be sent in the
-        MQTT connect packet.
+        :param str host: the hostname or IP address of the remote broker.
+        :param int port: the network port of the server host to connect to. Defaults to
+            1883. Note that the default port for MQTT over SSL/TLS is 8883 so if you
+            are using `tls_set()` the port may need providing.
+        :param int keepalive: Maximum period in seconds between communications with the
+            broker. If no other messages are being exchanged, this controls the
+            rate at which the client will send ping messages to the broker.
+        :param bool clean_start: (MQTT v5.0 only) True, False or MQTT_CLEAN_START_FIRST_ONLY.
+            Sets the MQTT v5.0 clean_start flag always, never or on the first successful connect only,
+            respectively.  MQTT session data (such as outstanding messages and subscriptions)
+            is cleared on successful connect when the clean_start flag is set.
+            For MQTT v3.1.1, the ``clean_session`` argument of `Client` should be used for similar
+            result.
+        :param Properties properties: (MQTT v5.0 only) the MQTT v5.0 properties to be sent in the
+            MQTT connect packet.
         """
 
         if self._protocol == MQTTv5:
             self._mqttv5_first_connect = True
         else:
             if clean_start != MQTT_CLEAN_START_FIRST_ONLY:
                 raise ValueError("Clean start only applies to MQTT V5")
@@ -1363,22 +1441,22 @@
         bind_address: str = "",
         bind_port: int = 0,
         clean_start: CleanStartOption = MQTT_CLEAN_START_FIRST_ONLY,
         properties: Properties | None = None,
     ) -> MQTTErrorCode:
         """Connect to a remote broker.
 
-        domain is the DNS domain to search for SRV records; if None,
-        try to determine local domain name.
-        keepalive, bind_address, clean_start and properties are as for connect()
+        :param str domain: the DNS domain to search for SRV records; if None,
+            try to determine local domain name.
+        :param keepalive, bind_address, clean_start and properties: see `connect()`
         """
 
         if HAVE_DNS is False:
             raise ValueError(
-                'No DNS resolver library found, try "pip install dnspython" or "pip3 install dnspython3".')
+                'No DNS resolver library found, try "pip install dnspython".')
 
         if domain is None:
             domain = socket.getfqdn()
             domain = domain[domain.find('.') + 1:]
 
         try:
             rr = f'_mqtt._tcp.{domain}'
@@ -1411,48 +1489,50 @@
         keepalive: int = 60,
         bind_address: str = "",
         bind_port: int = 0,
         clean_start: CleanStartOption = MQTT_CLEAN_START_FIRST_ONLY,
         properties: Properties | None = None,
     ) -> None:
         """Connect to a remote broker asynchronously. This is a non-blocking
-        connect call that can be used with loop_start() to provide very quick
+        connect call that can be used with `loop_start()` to provide very quick
         start.
 
         Any already established connection will be terminated immediately.
 
-        host is the hostname or IP address of the remote broker.
-        port is the network port of the server host to connect to. Defaults to
-        1883. Note that the default port for MQTT over SSL/TLS is 8883 so if you
-        are using tls_set() the port may need providing.
-        keepalive: Maximum period in seconds between communications with the
-        broker. If no other messages are being exchanged, this controls the
-        rate at which the client will send ping messages to the broker.
-        clean_start: (MQTT v5.0 only) True, False or MQTT_CLEAN_START_FIRST_ONLY.
-        Sets the MQTT v5.0 clean_start flag always, never or on the first successful connect only,
-        respectively.  MQTT session data (such as outstanding messages and subscriptions)
-        is cleared on successful connect when the clean_start flag is set.
-        properties: (MQTT v5.0 only) the MQTT v5.0 properties to be sent in the
-        MQTT connect packet.  Use the Properties class.
+        :param str host: the hostname or IP address of the remote broker.
+        :param int port: the network port of the server host to connect to. Defaults to
+            1883. Note that the default port for MQTT over SSL/TLS is 8883 so if you
+            are using `tls_set()` the port may need providing.
+        :param int keepalive: Maximum period in seconds between communications with the
+            broker. If no other messages are being exchanged, this controls the
+            rate at which the client will send ping messages to the broker.
+        :param bool clean_start: (MQTT v5.0 only) True, False or MQTT_CLEAN_START_FIRST_ONLY.
+            Sets the MQTT v5.0 clean_start flag always, never or on the first successful connect only,
+            respectively.  MQTT session data (such as outstanding messages and subscriptions)
+            is cleared on successful connect when the clean_start flag is set.
+            For MQTT v3.1.1, the ``clean_session`` argument of `Client` should be used for similar
+            result.
+        :param Properties properties: (MQTT v5.0 only) the MQTT v5.0 properties to be sent in the
+            MQTT connect packet.
         """
         if bind_port < 0:
             raise ValueError('Invalid bind port number.')
 
         # Switch to state NEW to allow update of host, port & co.
         self._sock_close()
-        self._state = ConnectionState.MQTT_CS_NEW
+        self._state = _ConnectionState.MQTT_CS_NEW
 
         self.host = host
         self.port = port
         self.keepalive = keepalive
         self._bind_address = bind_address
         self._bind_port = bind_port
         self._clean_start = clean_start
         self._connect_properties = properties
-        self._state = ConnectionState.MQTT_CS_CONNECT_ASYNC
+        self._state = _ConnectionState.MQTT_CS_CONNECT_ASYNC
 
     def reconnect_delay_set(self, min_delay: int = 1, max_delay: int = 120) -> None:
         """ Configure the exponential reconnect delay
 
             When connection is lost, wait initially min_delay seconds and
             double this time every attempt. The wait is capped at max_delay.
             Once the client is fully connected (e.g. not only TCP socket, but
@@ -1479,15 +1559,15 @@
             "remaining_length": 0,
             "packet": bytearray(b""),
             "to_process": 0,
             "pos": 0,
         }
 
         self._ping_t = 0.0
-        self._state = ConnectionState.MQTT_CS_CONNECTING
+        self._state = _ConnectionState.MQTT_CS_CONNECTING
 
         self._sock_close()
 
         # Mark all currently outgoing QoS = 0 packets as lost,
         # or `wait_for_publish()` could hang forever
         for pkt in self._out_packet:
             if pkt["command"] & 0xF0 == PUBLISH and pkt["qos"] == 0 and pkt["info"] is not None:
@@ -1522,29 +1602,29 @@
         self._call_socket_open(self._sock)
 
         return self._send_connect(self._keepalive)
 
     def loop(self, timeout: float = 1.0) -> MQTTErrorCode:
         """Process network events.
 
-        It is strongly recommended that you use loop_start(), or
-        loop_forever(), or if you are using an external event loop using
-        loop_read(), loop_write(), and loop_misc(). Using loop() on it's own is
+        It is strongly recommended that you use `loop_start()`, or
+        `loop_forever()`, or if you are using an external event loop using
+        `loop_read()`, `loop_write()`, and `loop_misc()`. Using loop() on it's own is
         no longer recommended.
 
         This function must be called regularly to ensure communication with the
         broker is carried out. It calls select() on the network socket to wait
         for network events. If incoming data is present it will then be
-        processed. Outgoing commands, from e.g. publish(), are normally sent
+        processed. Outgoing commands, from e.g. `publish()`, are normally sent
         immediately that their function is called, but this is not always
         possible. loop() will also attempt to send any remaining outgoing
         messages, which also includes commands that are part of the flow for
         messages with QoS>0.
 
-        timeout: The time in seconds to wait for incoming/outgoing network
+        :param int timeout: The time in seconds to wait for incoming/outgoing network
             traffic before timing out and returning.
 
         Returns MQTT_ERR_SUCCESS on success.
         Returns >0 on error.
 
         A ValueError will be raised if timeout < 0"""
 
@@ -1584,22 +1664,22 @@
         except TypeError:
             # Socket isn't correct type, in likelihood connection is lost
             # ... or we called disconnect(). In that case the socket will
             # be closed but some loop (like loop_forever) will continue to
             # call _loop(). We still want to break that loop by returning an
             # rc != MQTT_ERR_SUCCESS and we don't want state to change from
             # mqtt_cs_disconnecting.
-            if self._state not in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED):
-                self._state = ConnectionState.MQTT_CS_CONNECTION_LOST
+            if self._state not in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED):
+                self._state = _ConnectionState.MQTT_CS_CONNECTION_LOST
             return MQTTErrorCode.MQTT_ERR_CONN_LOST
         except ValueError:
             # Can occur if we just reconnected but rlist/wlist contain a -1 for
             # some reason.
-            if self._state not in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED):
-                self._state = ConnectionState.MQTT_CS_CONNECTION_LOST
+            if self._state not in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED):
+                self._state = _ConnectionState.MQTT_CS_CONNECTION_LOST
             return MQTTErrorCode.MQTT_ERR_CONN_LOST
         except Exception:
             # Note that KeyboardInterrupt, etc. can still terminate since they
             # are not derived from Exception
             return MQTTErrorCode.MQTT_ERR_UNKNOWN
 
         if self._sock in socklist[0] or pending_bytes > 0:
@@ -1635,47 +1715,46 @@
         properties: Properties | None = None,
     ) -> MQTTMessageInfo:
         """Publish a message on a topic.
 
         This causes a message to be sent to the broker and subsequently from
         the broker to any clients subscribing to matching topics.
 
-        topic: The topic that the message should be published on.
-        payload: The actual message to send. If not given, or set to None a
-        zero length message will be used. Passing an int or float will result
-        in the payload being converted to a string representing that number. If
-        you wish to send a true int/float, use struct.pack() to create the
-        payload you require.
-        qos: The quality of service level to use.
-        retain: If set to true, the message will be set as the "last known
-        good"/retained message for the topic.
-        properties: (MQTT v5.0 only) the MQTT v5.0 properties to be included.
-        Use the Properties class.
-
-        Returns a MQTTMessageInfo class, which can be used to determine whether
-        the message has been delivered (using info.is_published()) or to block
-        waiting for the message to be delivered (info.wait_for_publish()). The
+        :param str topic: The topic that the message should be published on.
+        :param payload: The actual message to send. If not given, or set to None a
+            zero length message will be used. Passing an int or float will result
+            in the payload being converted to a string representing that number. If
+            you wish to send a true int/float, use struct.pack() to create the
+            payload you require.
+        :param int qos: The quality of service level to use.
+        :param bool retain: If set to true, the message will be set as the "last known
+            good"/retained message for the topic.
+        :param Properties properties: (MQTT v5.0 only) the MQTT v5.0 properties to be included.
+
+        Returns a `MQTTMessageInfo` class, which can be used to determine whether
+        the message has been delivered (using `is_published()`) or to block
+        waiting for the message to be delivered (`wait_for_publish()`). The
         message ID and return code of the publish() call can be found at
-        info.mid and info.rc.
+        :py:attr:`info.mid <MQTTMessage.mid>` and :py:attr:`info.rc <MQTTMessage.rc>`.
 
-        For backwards compatibility, the MQTTMessageInfo class is iterable so
-        the old construct of (rc, mid) = client.publish(...) is still valid.
+        For backwards compatibility, the `MQTTMessageInfo` class is iterable so
+        the old construct of ``(rc, mid) = client.publish(...)`` is still valid.
 
         rc is MQTT_ERR_SUCCESS to indicate success or MQTT_ERR_NO_CONN if the
         client is not currently connected.  mid is the message ID for the
         publish request. The mid value can be used to track the publish request
         by checking against the mid argument in the on_publish() callback if it
         is defined.
 
-        A ValueError will be raised if topic is None, has zero length or is
-        invalid (contains a wildcard), except if the MQTT version used is v5.0.
-        For v5.0, a zero length topic can be used when a Topic Alias has been set.
-
-        A ValueError will be raised if qos is not one of 0, 1 or 2, or if
-        the length of the payload is greater than 268435455 bytes."""
+        :raises ValueError: if topic is None, has zero length or is
+            invalid (contains a wildcard), except if the MQTT version used is v5.0.
+            For v5.0, a zero length topic can be used when a Topic Alias has been set.
+        :raises ValueError: if qos is not one of 0, 1 or 2
+        :raises ValueError: if the length of the payload is greater than 268435455 bytes.
+        """
         if self._protocol != MQTTv5:
             if topic is None or len(topic) == 0:
                 raise ValueError('Invalid topic.')
 
         topic_bytes = topic.encode('utf-8')
 
         self._raise_for_invalid_topic(topic_bytes)
@@ -1739,34 +1818,34 @@
 
     def username_pw_set(
         self, username: str | None, password: str | None = None
     ) -> None:
         """Set a username and optionally a password for broker authentication.
 
         Must be called before connect() to have any effect.
-        Requires a broker that supports MQTT v3.1.
+        Requires a broker that supports MQTT v3.1 or more.
 
-        username: The username to authenticate with. Need have no relationship to the client id. Must be str
+        :param str username: The username to authenticate with. Need have no relationship to the client id. Must be str
             [MQTT-3.1.3-11].
             Set to None to reset client back to not using username/password for broker authentication.
-        password: The password to authenticate with. Optional, set to None if not required. If it is str, then it
+        :param str password: The password to authenticate with. Optional, set to None if not required. If it is str, then it
             will be encoded as UTF-8.
         """
 
         # [MQTT-3.1.3-11] User name must be UTF-8 encoded string
         self._username = None if username is None else username.encode('utf-8')
         if isinstance(password, str):
             self._password = password.encode('utf-8')
         else:
             self._password = password
 
     def enable_bridge_mode(self) -> None:
         """Sets the client in a bridge mode instead of client mode.
 
-        Must be called before connect() to have any effect.
+        Must be called before `connect()` to have any effect.
         Requires brokers that support bridge mode.
 
         Under bridge mode, the broker will identify the client as a bridge and
         not send it's own messages back to it. Hence a subsciption of # is
         possible without message loops. This feature also correctly propagates
         the retain flag on the messages.
 
@@ -1776,42 +1855,43 @@
         self._client_mode = MQTT_BRIDGE
 
     def _connection_closed(self) -> bool:
         """
         Return true if the connection is closed (and not trying to be opened).
         """
         return (
-            self._state == ConnectionState.MQTT_CS_NEW
-            or (self._state in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED) and self._sock is None))
+            self._state == _ConnectionState.MQTT_CS_NEW
+            or (self._state in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED) and self._sock is None))
 
     def is_connected(self) -> bool:
         """Returns the current status of the connection
 
         True if connection exists
         False if connection is closed
         """
-        return self._state == ConnectionState.MQTT_CS_CONNECTED
+        return self._state == _ConnectionState.MQTT_CS_CONNECTED
 
     def disconnect(
         self,
-        reasoncode: ReasonCodes | None = None,
+        reasoncode: ReasonCode | None = None,
         properties: Properties | None = None,
     ) -> MQTTErrorCode:
         """Disconnect a connected client from the broker.
-        reasoncode: (MQTT v5.0 only) a ReasonCodes instance setting the MQTT v5.0
-        reasoncode to be sent with the disconnect.  It is optional, the receiver
-        then assuming that 0 (success) is the value.
-        properties: (MQTT v5.0 only) a Properties instance setting the MQTT v5.0 properties
-        to be included. Optional - if not set, no properties are sent.
+
+        :param ReasonCode reasoncode: (MQTT v5.0 only) a ReasonCode instance setting the MQTT v5.0
+            reasoncode to be sent with the disconnect packet. It is optional, the receiver
+            then assuming that 0 (success) is the value.
+        :param Properties properties: (MQTT v5.0 only) a Properties instance setting the MQTT v5.0 properties
+            to be included. Optional - if not set, no properties are sent.
         """
         if self._sock is None:
-            self._state = ConnectionState.MQTT_CS_DISCONNECTED
+            self._state = _ConnectionState.MQTT_CS_DISCONNECTED
             return MQTT_ERR_NO_CONN
         else:
-            self._state = ConnectionState.MQTT_CS_DISCONNECTING
+            self._state = _ConnectionState.MQTT_CS_DISCONNECTING
 
         return self._send_disconnect(reasoncode, properties)
 
     def subscribe(
         self,
         topic: str | tuple[str, int] | tuple[str, SubscribeOptions] | list[tuple[str, int]] | list[tuple[str, SubscribeOptions]],
         qos: int = 0,
@@ -1822,74 +1902,74 @@
 
         This function may be called in three different ways (and a further three for MQTT v5.0):
 
         Simple string and integer
         -------------------------
         e.g. subscribe("my/topic", 2)
 
-        topic: A string specifying the subscription topic to subscribe to.
-        qos: The desired quality of service level for the subscription.
-             Defaults to 0.
-        options and properties: Not used.
+        :topic: A string specifying the subscription topic to subscribe to.
+        :qos: The desired quality of service level for the subscription.
+            Defaults to 0.
+        :options and properties: Not used.
 
         Simple string and subscribe options (MQTT v5.0 only)
         ----------------------------------------------------
         e.g. subscribe("my/topic", options=SubscribeOptions(qos=2))
 
-        topic: A string specifying the subscription topic to subscribe to.
-        qos: Not used.
-        options: The MQTT v5.0 subscribe options.
-        properties: a Properties instance setting the MQTT v5.0 properties
-        to be included. Optional - if not set, no properties are sent.
+        :topic: A string specifying the subscription topic to subscribe to.
+        :qos: Not used.
+        :options: The MQTT v5.0 subscribe options.
+        :properties: a Properties instance setting the MQTT v5.0 properties
+            to be included. Optional - if not set, no properties are sent.
 
         String and integer tuple
         ------------------------
         e.g. subscribe(("my/topic", 1))
 
-        topic: A tuple of (topic, qos). Both topic and qos must be present in
+        :topic: A tuple of (topic, qos). Both topic and qos must be present in
                the tuple.
-        qos and options: Not used.
-        properties: Only used for MQTT v5.0.  A Properties instance setting the
-        MQTT v5.0 properties. Optional - if not set, no properties are sent.
+        :qos and options: Not used.
+        :properties: Only used for MQTT v5.0.  A Properties instance setting the
+            MQTT v5.0 properties. Optional - if not set, no properties are sent.
 
         String and subscribe options tuple (MQTT v5.0 only)
         ---------------------------------------------------
         e.g. subscribe(("my/topic", SubscribeOptions(qos=1)))
 
-        topic: A tuple of (topic, SubscribeOptions). Both topic and subscribe
+        :topic: A tuple of (topic, SubscribeOptions). Both topic and subscribe
                 options must be present in the tuple.
-        qos and options: Not used.
-        properties: a Properties instance setting the MQTT v5.0 properties
-        to be included. Optional - if not set, no properties are sent.
+        :qos and options: Not used.
+        :properties: a Properties instance setting the MQTT v5.0 properties
+            to be included. Optional - if not set, no properties are sent.
 
         List of string and integer tuples
         ---------------------------------
         e.g. subscribe([("my/topic", 0), ("another/topic", 2)])
 
         This allows multiple topic subscriptions in a single SUBSCRIPTION
         command, which is more efficient than using multiple calls to
         subscribe().
 
-        topic: A list of tuple of format (topic, qos). Both topic and qos must
+        :topic: A list of tuple of format (topic, qos). Both topic and qos must
                be present in all of the tuples.
-        qos, options and properties: Not used.
+        :qos, options and properties: Not used.
 
         List of string and subscribe option tuples (MQTT v5.0 only)
         -----------------------------------------------------------
         e.g. subscribe([("my/topic", SubscribeOptions(qos=0), ("another/topic", SubscribeOptions(qos=2)])
 
         This allows multiple topic subscriptions in a single SUBSCRIPTION
         command, which is more efficient than using multiple calls to
         subscribe().
 
-        topic: A list of tuple of format (topic, SubscribeOptions). Both topic and subscribe
+        :topic: A list of tuple of format (topic, SubscribeOptions). Both topic and subscribe
                 options must be present in all of the tuples.
-        qos and options: Not used.
-        properties: a Properties instance setting the MQTT v5.0 properties
-        to be included. Optional - if not set, no properties are sent.
+        :qos and options: Not used.
+        :properties: a Properties instance setting the MQTT v5.0 properties
+            to be included. Optional - if not set, no properties are sent.
 
         The function returns a tuple (result, mid), where result is
         MQTT_ERR_SUCCESS to indicate success or (MQTT_ERR_NO_CONN, None) if the
         client is not currently connected.  mid is the message ID for the
         subscribe request. The mid value can be used to track the subscribe
         request by checking against the mid argument in the on_subscribe()
         callback if it is defined.
@@ -1954,32 +2034,32 @@
 
         if self._sock is None:
             return (MQTT_ERR_NO_CONN, None)
 
         return self._send_subscribe(False, topic_qos_list, properties)
 
     def unsubscribe(
-        self, topic: str, properties: Properties | None = None
+        self, topic: str | list[str], properties: Properties | None = None
     ) -> tuple[MQTTErrorCode, int | None]:
         """Unsubscribe the client from one or more topics.
 
-        topic: A single string, or list of strings that are the subscription
-               topics to unsubscribe from.
-        properties: (MQTT v5.0 only) a Properties instance setting the MQTT v5.0 properties
-        to be included. Optional - if not set, no properties are sent.
+        :param topic: A single string, or list of strings that are the subscription
+            topics to unsubscribe from.
+        :param properties: (MQTT v5.0 only) a Properties instance setting the MQTT v5.0 properties
+            to be included. Optional - if not set, no properties are sent.
 
         Returns a tuple (result, mid), where result is MQTT_ERR_SUCCESS
         to indicate success or (MQTT_ERR_NO_CONN, None) if the client is not
         currently connected.
         mid is the message ID for the unsubscribe request. The mid value can be
         used to track the unsubscribe request by checking against the mid
         argument in the on_unsubscribe() callback if it is defined.
 
-        Raises a ValueError if topic is None or has zero string length, or is
-        not a string or list.
+        :raises ValueError: if topic is None or has zero string length, or is
+            not a string or list.
         """
         topic_list = None
         if topic is None:
             raise ValueError('Invalid topic.')
         if isinstance(topic, (bytes, str)):
             if len(topic) == 0:
                 raise ValueError('Invalid topic.')
@@ -1996,21 +2076,21 @@
 
         if self._sock is None:
             return (MQTTErrorCode.MQTT_ERR_NO_CONN, None)
 
         return self._send_unsubscribe(False, topic_list, properties)
 
     def loop_read(self, max_packets: int = 1) -> MQTTErrorCode:
-        """Process read network events. Use in place of calling loop() if you
+        """Process read network events. Use in place of calling `loop()` if you
         wish to handle your client reads as part of your own application.
 
-        Use socket() to obtain the client socket to call select() or equivalent
+        Use `socket()` to obtain the client socket to call select() or equivalent
         on.
 
-        Do not use if you are using the threaded interface loop_start()."""
+        Do not use if you are using `loop_start()` or `loop_forever()`."""
         if self._sock is None:
             return MQTTErrorCode.MQTT_ERR_NO_CONN
 
         max_packets = len(self._out_messages) + len(self._in_messages)
         if max_packets < 1:
             max_packets = 1
 
@@ -2021,23 +2101,23 @@
             if rc > 0:
                 return self._loop_rc_handle(rc)
             elif rc == MQTTErrorCode.MQTT_ERR_AGAIN:
                 return MQTTErrorCode.MQTT_ERR_SUCCESS
         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
     def loop_write(self) -> MQTTErrorCode:
-        """Process write network events. Use in place of calling loop() if you
+        """Process write network events. Use in place of calling `loop()` if you
         wish to handle your client writes as part of your own application.
 
-        Use socket() to obtain the client socket to call select() or equivalent
+        Use `socket()` to obtain the client socket to call select() or equivalent
         on.
 
-        Use want_write() to determine if there is data waiting to be written.
+        Use `want_write()` to determine if there is data waiting to be written.
 
-        Do not use if you are using the threaded interface loop_start()."""
+        Do not use if you are using `loop_start()` or `loop_forever()`."""
         if self._sock is None:
             return MQTTErrorCode.MQTT_ERR_NO_CONN
 
         try:
             rc = self._packet_write()
             if rc == MQTTErrorCode.MQTT_ERR_AGAIN:
                 return MQTTErrorCode.MQTT_ERR_SUCCESS
@@ -2049,39 +2129,39 @@
             if self.want_write():
                 self._call_socket_register_write()
             else:
                 self._call_socket_unregister_write()
 
     def want_write(self) -> bool:
         """Call to determine if there is network data waiting to be written.
-        Useful if you are calling select() yourself rather than using loop().
+        Useful if you are calling select() yourself rather than using `loop()`, `loop_start()` or `loop_forever()`.
         """
         return len(self._out_packet) > 0
 
     def loop_misc(self) -> MQTTErrorCode:
-        """Process miscellaneous network events. Use in place of calling loop() if you
+        """Process miscellaneous network events. Use in place of calling `loop()` if you
         wish to call select() or equivalent on.
 
-        Do not use if you are using the threaded interface loop_start()."""
+        Do not use if you are using `loop_start()` or `loop_forever()`."""
         if self._sock is None:
             return MQTTErrorCode.MQTT_ERR_NO_CONN
 
         now = time_func()
         self._check_keepalive()
 
         if self._ping_t > 0 and now - self._ping_t >= self._keepalive:
             # client->ping_t != 0 means we are waiting for a pingresp.
             # This hasn't happened in the keepalive time so we should disconnect.
             self._sock_close()
 
-            if self._state in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED):
-                self._state = ConnectionState.MQTT_CS_DISCONNECTED
+            if self._state in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED):
+                self._state = _ConnectionState.MQTT_CS_DISCONNECTED
                 rc = MQTTErrorCode.MQTT_ERR_SUCCESS
             else:
-                self._state = ConnectionState.MQTT_CS_CONNECTION_LOST
+                self._state = _ConnectionState.MQTT_CS_CONNECTION_LOST
                 rc = MQTTErrorCode.MQTT_ERR_KEEPALIVE
 
             self._do_on_disconnect(
                 packet_from_broker=False,
                 v1_rc=rc,
             )
 
@@ -2118,28 +2198,31 @@
         retain: bool = False,
         properties: Properties | None = None,
     ) -> None:
         """Set a Will to be sent by the broker in case the client disconnects unexpectedly.
 
         This must be called before connect() to have any effect.
 
-        topic: The topic that the will message should be published on.
-        payload: The message to send as a will. If not given, or set to None a
-        zero length message will be used as the will. Passing an int or float
-        will result in the payload being converted to a string representing
-        that number. If you wish to send a true int/float, use struct.pack() to
-        create the payload you require.
-        qos: The quality of service level to use for the will.
-        retain: If set to true, the will message will be set as the "last known
-        good"/retained message for the topic.
-        properties: (MQTT v5.0 only) a Properties instance setting the MQTT v5.0 properties
-        to be included with the will message. Optional - if not set, no properties are sent.
+        :param str topic: The topic that the will message should be published on.
+        :param payload: The message to send as a will. If not given, or set to None a
+            zero length message will be used as the will. Passing an int or float
+            will result in the payload being converted to a string representing
+            that number. If you wish to send a true int/float, use struct.pack() to
+            create the payload you require.
+        :param int qos: The quality of service level to use for the will.
+        :param bool retain: If set to true, the will message will be set as the "last known
+            good"/retained message for the topic.
+        :param Properties properties: (MQTT v5.0 only) the MQTT v5.0 properties
+            to be included with the will message. Optional - if not set, no properties are sent.
 
-        Raises a ValueError if qos is not 0, 1 or 2, or if topic is None or has
-        zero string length.
+        :raises ValueError: if qos is not 0, 1 or 2, or if topic is None or has
+            zero string length.
+
+        See `will_clear` to clear will. Note that will are NOT send if the client disconnect cleanly
+        for example by calling `disconnect()`.
         """
         if topic is None or len(topic) == 0:
             raise ValueError('Invalid topic.')
 
         if qos < 0 or qos > 2:
             raise ValueError('Invalid QoS level.')
 
@@ -2151,15 +2234,15 @@
         self._will = True
         self._will_topic = topic.encode('utf-8')
         self._will_qos = qos
         self._will_retain = retain
         self._will_properties = properties
 
     def will_clear(self) -> None:
-        """ Removes a will that was previously configured with will_set().
+        """ Removes a will that was previously configured with `will_set()`.
 
         Must be called before connect() to have any effect."""
         self._will = False
         self._will_topic = b""
         self._will_payload = b""
         self._will_qos = 0
         self._will_retain = False
@@ -2174,33 +2257,32 @@
         retry_first_connection: bool = False,
     ) -> MQTTErrorCode:
         """This function calls the network loop functions for you in an
         infinite blocking loop. It is useful for the case where you only want
         to run the MQTT client loop in your program.
 
         loop_forever() will handle reconnecting for you if reconnect_on_failure is
-        true (this is the default behavior). If you call disconnect() in a callback
+        true (this is the default behavior). If you call `disconnect()` in a callback
         it will return.
 
-
-        timeout: The time in seconds to wait for incoming/outgoing network
+        :param int timeout: The time in seconds to wait for incoming/outgoing network
           traffic before timing out and returning.
-        retry_first_connection: Should the first connection attempt be retried on failure.
+        :param bool retry_first_connection: Should the first connection attempt be retried on failure.
           This is independent of the reconnect_on_failure setting.
 
-        Raises OSError/WebsocketConnectionError on first connection failures unless retry_first_connection=True
+        :raises OSError: if the first connection fail unless retry_first_connection=True
         """
 
         run = True
 
         while run:
             if self._thread_terminate is True:
                 break
 
-            if self._state == ConnectionState.MQTT_CS_CONNECT_ASYNC:
+            if self._state == _ConnectionState.MQTT_CS_CONNECT_ASYNC:
                 try:
                     self.reconnect()
                 except OSError:
                     self._handle_on_connect_fail()
                     if not retry_first_connection:
                         raise
                     self._easy_log(
@@ -2221,15 +2303,15 @@
                     and len(self._out_packet) == 0
                         and len(self._out_messages) == 0):
                     rc = MQTTErrorCode.MQTT_ERR_NOMEM
                     run = False
 
             def should_exit() -> bool:
                 return (
-                    self._state in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED) or
+                    self._state in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED) or
                     run is False or  # noqa: B023 (uses the run variable from the outer scope on purpose)
                     self._thread_terminate is True
                 )
 
             if should_exit() or not self._reconnect_on_failure:
                 run = False
             else:
@@ -2246,474 +2328,480 @@
                             MQTT_LOG_DEBUG, "Connection failed, retrying")
 
         return rc
 
     def loop_start(self) -> MQTTErrorCode:
         """This is part of the threaded client interface. Call this once to
         start a new thread to process network traffic. This provides an
-        alternative to repeatedly calling loop() yourself.
+        alternative to repeatedly calling `loop()` yourself.
+
+        Under the hood, this will call `loop_forever` in a thread, which means that
+        the thread will terminate if you call `disconnect()`
         """
         if self._thread is not None:
             return MQTTErrorCode.MQTT_ERR_INVAL
 
         self._sockpairR, self._sockpairW = _socketpair_compat()
         self._thread_terminate = False
         self._thread = threading.Thread(target=self._thread_main, name=f"paho-mqtt-client-{self._client_id.decode()}")
         self._thread.daemon = True
         self._thread.start()
 
         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
     def loop_stop(self) -> MQTTErrorCode:
         """This is part of the threaded client interface. Call this once to
-        stop the network thread previously created with loop_start(). This call
+        stop the network thread previously created with `loop_start()`. This call
         will block until the network thread finishes.
+
+        This don't guarantee that publish packet are sent, use `wait_for_publish` or
+        `on_publish` to ensure `publish` are sent.
         """
         if self._thread is None:
             return MQTTErrorCode.MQTT_ERR_INVAL
 
         self._thread_terminate = True
         if threading.current_thread() != self._thread:
             self._thread.join()
-            self._thread = None
 
         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
     @property
     def callback_api_version(self) -> CallbackAPIVersion:
         """
         Return the callback API version used for user-callback. See docstring for
-        each user-callback (on_connect, on_publish, ...) for details.
+        each user-callback (`on_connect`, `on_publish`, ...) for details.
+
+        This property is read-only.
         """
         return self._callback_api_version
 
     @property
     def on_log(self) -> CallbackOnLog | None:
-        """If implemented, called when the client has log information.
-        Defined to allow debugging."""
-        return self._on_log
+        """The callback called when the client has log information.
+        Defined to allow debugging.
 
-    @on_log.setter
-    def on_log(self, func: CallbackOnLog | None) -> None:
-        """ Define the logging callback implementation.
+        Expected signature is::
 
-        Expected signature is:
             log_callback(client, userdata, level, buf)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        level:      gives the severity of the message and will be one of
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param int level: gives the severity of the message and will be one of
                     MQTT_LOG_INFO, MQTT_LOG_NOTICE, MQTT_LOG_WARNING,
                     MQTT_LOG_ERR, and MQTT_LOG_DEBUG.
-        buf:        the message itself
+        :param str buf: the message itself
 
-        Decorator: @client.log_callback() (```client``` is the name of the
+        Decorator: @client.log_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_log
+
+    @on_log.setter
+    def on_log(self, func: CallbackOnLog | None) -> None:
         self._on_log = func
 
     def log_callback(self) -> Callable[[CallbackOnLog], CallbackOnLog]:
         def decorator(func: CallbackOnLog) -> CallbackOnLog:
             self.on_log = func
             return func
         return decorator
 
     @property
     def on_pre_connect(self) -> CallbackOnPreConnect | None:
-        """If implemented, called immediately prior to the connection is made
-        request."""
-        return self._on_pre_connect
+        """The callback called immediately prior to the connection is made
+        request.
 
-    @on_pre_connect.setter
-    def on_pre_connect(self, func: CallbackOnPreConnect | None) -> None:
-        """ Define the pre_connect callback implementation.
+        Expected signature (for all callback API version)::
 
-        Expected signature (for all callback API version):
             connect_callback(client, userdata)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
+        :parama Client client: the client instance for this callback
+        :parama userdata: the private user data as set in Client() or user_data_set()
 
-        Decorator: @client.pre_connect_callback() (```client``` is the name of the
+        Decorator: @client.pre_connect_callback() (``client`` is the name of the
             instance which this callback is being attached to)
 
         """
+        return self._on_pre_connect
+
+    @on_pre_connect.setter
+    def on_pre_connect(self, func: CallbackOnPreConnect | None) -> None:
         with self._callback_mutex:
             self._on_pre_connect = func
 
     def pre_connect_callback(
         self,
     ) -> Callable[[CallbackOnPreConnect], CallbackOnPreConnect]:
         def decorator(func: CallbackOnPreConnect) -> CallbackOnPreConnect:
             self.on_pre_connect = func
             return func
         return decorator
 
     @property
     def on_connect(self) -> CallbackOnConnect | None:
-        """If implemented, called when the broker responds to our connection
-        request."""
-        return self._on_connect
+        """The callback called when the broker reponds to our connection request.
 
-    @on_connect.setter
-    def on_connect(self, func: CallbackOnConnect | None) -> None:
-        """ Define the connect callback implementation.
+        Expected signature for callback API version 2::
 
-        Expected signature for callback API version 2:
             connect_callback(client, userdata, connect_flags, reason_code, properties)
 
         Expected signature for callback API version 1 change with MQTT protocol version:
-            * For MQTT v3.1 and v3.1.1 it's:
+            * For MQTT v3.1 and v3.1.1 it's::
+
                 connect_callback(client, userdata, flags, rc)
 
-            * For MQTT it's v5.0:
+            * For MQTT v5.0 it's::
+
                 connect_callback(client, userdata, flags, reason_code, properties)
 
 
-        client:        the client instance for this callback
-        userdata:      the private user data as set in Client() or user_data_set()
-        connect_flags: the flags for this connection, it has type ConnectFlags
-        reason_code:   the connection reason code received from the broken.
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param ConnectFlags connect_flags: the flags for this connection
+        :param ReasonCode reason_code: the connection reason code received from the broken.
                        In MQTT v5.0 it's the reason code defined by the standard.
                        In MQTT v3, we convert return code to a reason code, see
-                       convert_connack_rc_to_reason_code().
-                       ReasonCode may be compared to integer.
-        properties:    the MQTT v5.0 properties received from the broker.  An instance
-                       of the Properties class.
+                       `convert_connack_rc_to_reason_code()`.
+                       `ReasonCode` may be compared to integer.
+        :param Properties properties: the MQTT v5.0 properties received from the broker.
                        For MQTT v3.1 and v3.1.1 properties is not provided and an empty Properties
                        object is always used.
-        flags:         response flags sent by the broker
-        rc:            the connection result
+        :param dict flags: response flags sent by the broker
+        :param int rc: the connection result, should have a value of `ConnackCode`
 
         flags is a dict that contains response flags from the broker:
             flags['session present'] - this flag is useful for clients that are
                 using clean session set to 0 only. If a client with clean
                 session=0, that reconnects to a broker that it has previously
                 connected to, this flag indicates whether the broker still has the
                 session information for the client. If 1, the session still exists.
 
         The value of rc indicates success or not:
-            0: Connection successful
-            1: Connection refused - incorrect protocol version
-            2: Connection refused - invalid client identifier
-            3: Connection refused - server unavailable
-            4: Connection refused - bad username or password
-            5: Connection refused - not authorised
-            6-255: Currently unused.
+            - 0: Connection successful
+            - 1: Connection refused - incorrect protocol version
+            - 2: Connection refused - invalid client identifier
+            - 3: Connection refused - server unavailable
+            - 4: Connection refused - bad username or password
+            - 5: Connection refused - not authorised
+            - 6-255: Currently unused.
 
-        Decorator: @client.connect_callback() (```client``` is the name of the
+        Decorator: @client.connect_callback() (``client`` is the name of the
             instance which this callback is being attached to)
-
         """
+        return self._on_connect
+
+    @on_connect.setter
+    def on_connect(self, func: CallbackOnConnect | None) -> None:
         with self._callback_mutex:
             self._on_connect = func
 
     def connect_callback(
         self,
     ) -> Callable[[CallbackOnConnect], CallbackOnConnect]:
         def decorator(func: CallbackOnConnect) -> CallbackOnConnect:
             self.on_connect = func
             return func
         return decorator
 
     @property
     def on_connect_fail(self) -> CallbackOnConnectFail | None:
-        """If implemented, called when the client failed to connect
-        to the broker."""
-        return self._on_connect_fail
+        """The callback called when the client failed to connect
+        to the broker.
 
-    @on_connect_fail.setter
-    def on_connect_fail(self, func: CallbackOnConnectFail | None) -> None:
-        """ Define the connection failure callback implementation
+        Expected signature is (for all callback_api_version)::
 
-        Expected signature is (for all callback_api_version):
             connect_fail_callback(client, userdata)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
+        :param Client client: the client instance for this callback
+        :parama userdata: the private user data as set in Client() or user_data_set()
 
-        Decorator: @client.connect_fail_callback() (```client``` is the name of the
+        Decorator: @client.connect_fail_callback() (``client`` is the name of the
             instance which this callback is being attached to)
-
         """
+        return self._on_connect_fail
+
+    @on_connect_fail.setter
+    def on_connect_fail(self, func: CallbackOnConnectFail | None) -> None:
         with self._callback_mutex:
             self._on_connect_fail = func
 
     def connect_fail_callback(
         self,
     ) -> Callable[[CallbackOnConnectFail], CallbackOnConnectFail]:
         def decorator(func: CallbackOnConnectFail) -> CallbackOnConnectFail:
             self.on_connect_fail = func
             return func
         return decorator
 
     @property
     def on_subscribe(self) -> CallbackOnSubscribe | None:
-        """If implemented, called when the broker responds to a subscribe
-        request."""
-        return self._on_subscribe
+        """The callback called when the broker responds to a subscribe
+        request.
 
-    @on_subscribe.setter
-    def on_subscribe(self, func: CallbackOnSubscribe | None) -> None:
-        """ Define the subscribe callback implementation.
+        Expected signature for callback API version 2::
 
-        Expected signature for callback API version 2:
             subscribe_callback(client, userdata, mid, reason_code_list, properties)
 
         Expected signature for callback API version 1 change with MQTT protocol version:
-            * For MQTT v3.1 and v3.1.1 it's:
+            * For MQTT v3.1 and v3.1.1 it's::
+
                 subscribe_callback(client, userdata, mid, granted_qos)
 
-            * For MQTT v5.0 it's:
+            * For MQTT v5.0 it's::
+
                 subscribe_callback(client, userdata, mid, reason_code_list, properties)
 
-        client:           the client instance for this callback
-        userdata:         the private user data as set in Client() or user_data_set()
-        mid:              matches the mid variable returned from the corresponding
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param int mid: matches the mid variable returned from the corresponding
                           subscribe() call.
-        reason_code_list: reason codes received from the broker for each subscription.
+        :param list[ReasonCode] reason_code_list: reason codes received from the broker for each subscription.
                           In MQTT v5.0 it's the reason code defined by the standard.
                           In MQTT v3, we convert granted QoS to a reason code.
-                          It's a list of ReasonCodes instances.
-        properties:       the MQTT v5.0 properties received from the broker.  An instance
-                          of the Properties class.
+                          It's a list of ReasonCode instances.
+        :param Properties properties: the MQTT v5.0 properties received from the broker.
                           For MQTT v3.1 and v3.1.1 properties is not provided and an empty Properties
                           object is always used.
-        granted_qos:      list of integers that give the QoS level the broker has
+        :param list[int] granted_qos: list of integers that give the QoS level the broker has
                           granted for each of the different subscription requests.
 
-        Decorator: @client.subscribe_callback() (```client``` is the name of the
+        Decorator: @client.subscribe_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_subscribe
+
+    @on_subscribe.setter
+    def on_subscribe(self, func: CallbackOnSubscribe | None) -> None:
         with self._callback_mutex:
             self._on_subscribe = func
 
     def subscribe_callback(
         self,
     ) -> Callable[[CallbackOnSubscribe], CallbackOnSubscribe]:
         def decorator(func: CallbackOnSubscribe) -> CallbackOnSubscribe:
             self.on_subscribe = func
             return func
         return decorator
 
     @property
     def on_message(self) -> CallbackOnMessage | None:
-        """If implemented, called when a message has been received on a topic
+        """The callback called when a message has been received on a topic
         that the client subscribes to.
 
-        This callback will be called for every message received. Use
-        message_callback_add() to define multiple callbacks that will be called
-        for specific topic filters."""
-        return self._on_message
-
-    @on_message.setter
-    def on_message(self, func: CallbackOnMessage | None) -> None:
-        """ Define the message received callback implementation.
+        This callback will be called for every message received unless a
+        `message_callback_add()` matched the message.
 
         Expected signature is (for all callback API version):
             message_callback(client, userdata, message)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        message:    an instance of MQTTMessage.
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param MQTTMessage message: the received message.
                     This is a class with members topic, payload, qos, retain.
 
-        Decorator: @client.message_callback() (```client``` is the name of the
+        Decorator: @client.message_callback() (``client`` is the name of the
             instance which this callback is being attached to)
-
         """
+        return self._on_message
+
+    @on_message.setter
+    def on_message(self, func: CallbackOnMessage | None) -> None:
         with self._callback_mutex:
             self._on_message = func
 
     def message_callback(
         self,
     ) -> Callable[[CallbackOnMessage], CallbackOnMessage]:
         def decorator(func: CallbackOnMessage) -> CallbackOnMessage:
             self.on_message = func
             return func
         return decorator
 
     @property
     def on_publish(self) -> CallbackOnPublish | None:
-        """If implemented, called when a message that was to be sent using the
-        publish() call has completed transmission to the broker.
+        """The callback called when a message that was to be sent using the
+        `publish()` call has completed transmission to the broker.
 
         For messages with QoS levels 1 and 2, this means that the appropriate
         handshakes have completed. For QoS 0, this simply means that the message
         has left the client.
-        This callback is important because even if the publish() call returns
-        success, it does not always mean that the message has been sent."""
-        return self._on_publish
+        This callback is important because even if the `publish()` call returns
+        success, it does not always mean that the message has been sent.
 
-    @on_publish.setter
-    def on_publish(self, func: CallbackOnPublish | None) -> None:
-        """ Define the published message callback implementation.
+        See also `wait_for_publish` which could be simpler to use.
+
+        Expected signature for callback API version 2::
 
-        Expected signature for callback API version 2:
             publish_callback(client, userdata, mid, reason_code, properties)
 
-        Expected signature for callback API version 1:
+        Expected signature for callback API version 1::
+
             publish_callback(client, userdata, mid)
 
-        client:      the client instance for this callback
-        userdata:    the private user data as set in Client() or user_data_set()
-        mid:         matches the mid variable returned from the corresponding
-                     publish() call, to allow outgoing messages to be tracked.
-        reason_code: the connection reason code received from the broken.
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param int mid: matches the mid variable returned from the corresponding
+                     `publish()` call, to allow outgoing messages to be tracked.
+        :param ReasonCode reason_code: the connection reason code received from the broken.
                      In MQTT v5.0 it's the reason code defined by the standard.
                      In MQTT v3 it's always the reason code Success
-        properties:  the MQTT v5.0 properties received from the broker.  An instance
-                     of the Properties class.
+        :parama Properties properties: the MQTT v5.0 properties received from the broker.
                      For MQTT v3.1 and v3.1.1 properties is not provided and an empty Properties
                      object is always used.
 
         Note: for QoS = 0, the reason_code and the properties don't really exist, it's the client
         library that generate them. It's always an empty properties and a success reason code.
         Because the (MQTTv5) standard don't have reason code for PUBLISH packet, the library create them
         at PUBACK packet, as if the message was sent with QoS = 1.
 
-        Decorator: @client.publish_callback() (```client``` is the name of the
+        Decorator: @client.publish_callback() (``client`` is the name of the
             instance which this callback is being attached to)
 
         """
+        return self._on_publish
+
+    @on_publish.setter
+    def on_publish(self, func: CallbackOnPublish | None) -> None:
         with self._callback_mutex:
             self._on_publish = func
 
     def publish_callback(
         self,
     ) -> Callable[[CallbackOnPublish], CallbackOnPublish]:
         def decorator(func: CallbackOnPublish) -> CallbackOnPublish:
             self.on_publish = func
             return func
         return decorator
 
     @property
     def on_unsubscribe(self) -> CallbackOnUnsubscribe | None:
-        """If implemented, called when the broker responds to an unsubscribe
-        request."""
-        return self._on_unsubscribe
+        """The callback called when the broker responds to an unsubscribe
+        request.
 
-    @on_unsubscribe.setter
-    def on_unsubscribe(self, func: CallbackOnUnsubscribe | None) -> None:
-        """ Define the unsubscribe callback implementation.
+        Expected signature for callback API version 2::
 
-        Expected signature for callback API version 2:
             unsubscribe_callback(client, userdata, mid, reason_code_list, properties)
 
         Expected signature for callback API version 1 change with MQTT protocol version:
-            * For MQTT v3.1 and v3.1.1 it's:
+            * For MQTT v3.1 and v3.1.1 it's::
+
                 unsubscribe_callback(client, userdata, mid)
 
-            * For MQTT v5.0 it's:
+            * For MQTT v5.0 it's::
+
                 unsubscribe_callback(client, userdata, mid, properties, v1_reason_codes)
 
-        client:           the client instance for this callback
-        userdata:         the private user data as set in Client() or user_data_set()
-        mid:              matches the mid variable returned from the corresponding
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param mid: matches the mid variable returned from the corresponding
                           unsubscribe() call.
-        reason_code_list: reason codes received from the broker for each unsubscription.
+        :param list[ReasonCode] reason_code_list: reason codes received from the broker for each unsubscription.
                           In MQTT v5.0 it's the reason code defined by the standard.
                           In MQTT v3, there is not equivalent from broken and empty list
                           is always used.
-        properties:       the MQTT v5.0 properties received from the broker.  An instance
-                          of the Properties class.
+        :param Properties properties: the MQTT v5.0 properties received from the broker.
                           For MQTT v3.1 and v3.1.1 properties is not provided and an empty Properties
                           object is always used.
-        v1_reason_codes:  the MQTT v5.0 reason codes received from the broker for each
-                          unsubscribe topic.  A list of ReasonCodes instances OR a single
-                          ReasonCodes when we unsubscribe from a single topic.
+        :param v1_reason_codes: the MQTT v5.0 reason codes received from the broker for each
+                          unsubscribe topic.  A list of ReasonCode instances OR a single
+                          ReasonCode when we unsubscribe from a single topic.
 
-        Decorator: @client.unsubscribe_callback() (```client``` is the name of the
+        Decorator: @client.unsubscribe_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_unsubscribe
+
+    @on_unsubscribe.setter
+    def on_unsubscribe(self, func: CallbackOnUnsubscribe | None) -> None:
         with self._callback_mutex:
             self._on_unsubscribe = func
 
     def unsubscribe_callback(
         self,
     ) -> Callable[[CallbackOnUnsubscribe], CallbackOnUnsubscribe]:
         def decorator(func: CallbackOnUnsubscribe) -> CallbackOnUnsubscribe:
             self.on_unsubscribe = func
             return func
         return decorator
 
     @property
     def on_disconnect(self) -> CallbackOnDisconnect | None:
-        """If implemented, called when the client disconnects from the broker.
-        """
-        return self._on_disconnect
+        """The callback called when the client disconnects from the broker.
 
-    @on_disconnect.setter
-    def on_disconnect(self, func: CallbackOnDisconnect | None) -> None:
-        """ Define the disconnect callback implementation.
+        Expected signature for callback API version 2::
 
-        Expected signature for callback API version 2:
             disconnect_callback(client, userdata, disconnect_flags, reason_code, properties)
 
         Expected signature for callback API version 1 change with MQTT protocol version:
-            * For MQTT v3.1 and v3.1.1 it's:
+            * For MQTT v3.1 and v3.1.1 it's::
+
                 disconnect_callback(client, userdata, rc)
 
-            * For MQTT it's v5.0:
+            * For MQTT v5.0 it's::
+
                 disconnect_callback(client, userdata, reason_code, properties)
 
-        client:           the client instance for this callback
-        userdata:         the private user data as set in Client() or user_data_set()
-        disconnect_flags: the flags for this disconnection, it has type DisconnectFlags
-        reason_code:      the disconnection reason code possibly received from the broker (see flags).
+        :param Client client: the client instance for this callback
+        :param userdata:  the private user data as set in Client() or user_data_set()
+        :param DisconnectFlag disconnect_flags: the flags for this disconnection.
+        :param ReasonCode reason_code:  the disconnection reason code possibly received from the broker (see disconnect_flags).
                           In MQTT v5.0 it's the reason code defined by the standard.
                           In MQTT v3 it's never received from the broker, we convert an MQTTErrorCode,
-                          see convert_disconnect_error_code_to_reason_code().
-                          ReasonCode may be compared to integer.
-        properties:       the MQTT v5.0 properties received from the broker.  An instance
-                          of the Properties class.
+                          see `convert_disconnect_error_code_to_reason_code()`.
+                          `ReasonCode` may be compared to integer.
+        :param Properties properties: the MQTT v5.0 properties received from the broker.
                           For MQTT v3.1 and v3.1.1 properties is not provided and an empty Properties
                           object is always used.
-        rc:               the disconnection result
+        :param int rc: the disconnection result
                           The rc parameter indicates the disconnection state. If
                           MQTT_ERR_SUCCESS (0), the callback was called in response to
                           a disconnect() call. If any other value the disconnection
                           was unexpected, such as might be caused by a network error.
 
-        Decorator: @client.disconnect_callback() (```client``` is the name of the
+        Decorator: @client.disconnect_callback() (``client`` is the name of the
             instance which this callback is being attached to)
 
         """
+        return self._on_disconnect
+
+    @on_disconnect.setter
+    def on_disconnect(self, func: CallbackOnDisconnect | None) -> None:
         with self._callback_mutex:
             self._on_disconnect = func
 
     def disconnect_callback(
         self,
     ) -> Callable[[CallbackOnDisconnect], CallbackOnDisconnect]:
         def decorator(func: CallbackOnDisconnect) -> CallbackOnDisconnect:
             self.on_disconnect = func
             return func
         return decorator
 
     @property
     def on_socket_open(self) -> CallbackOnSocket | None:
-        """If implemented, called just after the socket was opend."""
-        return self._on_socket_open
-
-    @on_socket_open.setter
-    def on_socket_open(self, func: CallbackOnSocket | None) -> None:
-        """Define the socket_open callback implementation.
+        """The callback called just after the socket was opend.
 
         This should be used to register the socket to an external event loop for reading.
 
-        Expected signature is (for all callback API version):
+        Expected signature is (for all callback API version)::
+
             socket_open_callback(client, userdata, socket)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        sock:       the socket which was just opened.
+        :param Client client:     the client instance for this callback
+        :param userdata:   the private user data as set in Client() or user_data_set()
+        :param SocketLike sock: the socket which was just opened.
 
-        Decorator: @client.socket_open_callback() (```client``` is the name of the
+        Decorator: @client.socket_open_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_socket_open
+
+    @on_socket_open.setter
+    def on_socket_open(self, func: CallbackOnSocket | None) -> None:
         with self._callback_mutex:
             self._on_socket_open = func
 
     def socket_open_callback(
         self,
     ) -> Callable[[CallbackOnSocket], CallbackOnSocket]:
         def decorator(func: CallbackOnSocket) -> CallbackOnSocket:
@@ -2734,33 +2822,33 @@
                     self._easy_log(
                         MQTT_LOG_ERR, 'Caught exception in on_socket_open: %s', err)
                     if not self.suppress_exceptions:
                         raise
 
     @property
     def on_socket_close(self) -> CallbackOnSocket | None:
-        """If implemented, called just before the socket is closed."""
-        return self._on_socket_close
-
-    @on_socket_close.setter
-    def on_socket_close(self, func: CallbackOnSocket | None) -> None:
-        """Define the socket_close callback implementation.
+        """The callback called just before the socket is closed.
 
         This should be used to unregister the socket from an external event loop for reading.
 
-        Expected signature is (for all callback API version):
+        Expected signature is (for all callback API version)::
+
             socket_close_callback(client, userdata, socket)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        sock:       the socket which is about to be closed.
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param SocketLike sock: the socket which is about to be closed.
 
-        Decorator: @client.socket_close_callback() (```client``` is the name of the
+        Decorator: @client.socket_close_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_socket_close
+
+    @on_socket_close.setter
+    def on_socket_close(self, func: CallbackOnSocket | None) -> None:
         with self._callback_mutex:
             self._on_socket_close = func
 
     def socket_close_callback(
         self,
     ) -> Callable[[CallbackOnSocket], CallbackOnSocket]:
         def decorator(func: CallbackOnSocket) -> CallbackOnSocket:
@@ -2781,33 +2869,33 @@
                     self._easy_log(
                         MQTT_LOG_ERR, 'Caught exception in on_socket_close: %s', err)
                     if not self.suppress_exceptions:
                         raise
 
     @property
     def on_socket_register_write(self) -> CallbackOnSocket | None:
-        """If implemented, called when the socket needs writing but can't."""
-        return self._on_socket_register_write
-
-    @on_socket_register_write.setter
-    def on_socket_register_write(self, func: CallbackOnSocket | None) -> None:
-        """Define the socket_register_write callback implementation.
+        """The callback called when the socket needs writing but can't.
 
         This should be used to register the socket with an external event loop for writing.
 
-        Expected signature is (for all callback API version):
+        Expected signature is (for all callback API version)::
+
             socket_register_write_callback(client, userdata, socket)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        sock:       the socket which should be registered for writing
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param SocketLike sock: the socket which should be registered for writing
 
-        Decorator: @client.socket_register_write_callback() (```client``` is the name of the
+        Decorator: @client.socket_register_write_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_socket_register_write
+
+    @on_socket_register_write.setter
+    def on_socket_register_write(self, func: CallbackOnSocket | None) -> None:
         with self._callback_mutex:
             self._on_socket_register_write = func
 
     def socket_register_write_callback(
         self,
     ) -> Callable[[CallbackOnSocket], CallbackOnSocket]:
         def decorator(func: CallbackOnSocket) -> CallbackOnSocket:
@@ -2833,35 +2921,35 @@
                 if not self.suppress_exceptions:
                     raise
 
     @property
     def on_socket_unregister_write(
         self,
     ) -> CallbackOnSocket | None:
-        """If implemented, called when the socket doesn't need writing anymore."""
-        return self._on_socket_unregister_write
-
-    @on_socket_unregister_write.setter
-    def on_socket_unregister_write(
-        self, func: CallbackOnSocket | None
-    ) -> None:
-        """Define the socket_unregister_write callback implementation.
+        """The callback called when the socket doesn't need writing anymore.
 
         This should be used to unregister the socket from an external event loop for writing.
 
-        Expected signature is (for all callback API version):
+        Expected signature is (for all callback API version)::
+
             socket_unregister_write_callback(client, userdata, socket)
 
-        client:     the client instance for this callback
-        userdata:   the private user data as set in Client() or user_data_set()
-        sock:       the socket which should be unregistered for writing
+        :param Client client: the client instance for this callback
+        :param userdata: the private user data as set in Client() or user_data_set()
+        :param SocketLike sock: the socket which should be unregistered for writing
 
-        Decorator: @client.socket_unregister_write_callback() (```client``` is the name of the
+        Decorator: @client.socket_unregister_write_callback() (``client`` is the name of the
             instance which this callback is being attached to)
         """
+        return self._on_socket_unregister_write
+
+    @on_socket_unregister_write.setter
+    def on_socket_unregister_write(
+        self, func: CallbackOnSocket | None
+    ) -> None:
         with self._callback_mutex:
             self._on_socket_unregister_write = func
 
     def socket_unregister_write_callback(
         self,
     ) -> Callable[[CallbackOnSocket], CallbackOnSocket]:
         def decorator(
@@ -2891,22 +2979,34 @@
                     MQTT_LOG_ERR, 'Caught exception in on_socket_unregister_write: %s', err)
                 if not self.suppress_exceptions:
                     raise
 
     def message_callback_add(self, sub: str, callback: CallbackOnMessage) -> None:
         """Register a message callback for a specific topic.
         Messages that match 'sub' will be passed to 'callback'. Any
-        non-matching messages will be passed to the default on_message
+        non-matching messages will be passed to the default `on_message`
         callback.
 
         Call multiple times with different 'sub' to define multiple topic
         specific callbacks.
 
         Topic specific callbacks may be removed with
-        message_callback_remove()."""
+        `message_callback_remove()`.
+
+        See `on_message` for the expected signature of the callback.
+
+        Decorator: @client.topic_callback(sub) (``client`` is the name of the
+            instance which this callback is being attached to)
+
+        Example::
+
+            @client.topic_callback("mytopic/#")
+            def handle_mytopic(client, userdata, message):
+                ...
+        """
         if callback is None or sub is None:
             raise ValueError("sub and callback must both be defined.")
 
         with self._callback_mutex:
             self._on_message_filtered[sub] = callback
 
     def topic_callback(
@@ -2915,15 +3015,15 @@
         def decorator(func: CallbackOnMessage) -> CallbackOnMessage:
             self.message_callback_add(sub, func)
             return func
         return decorator
 
     def message_callback_remove(self, sub: str) -> None:
         """Remove a message callback previously registered with
-        message_callback_add()."""
+        `message_callback_add()`."""
         if sub is None:
             raise ValueError("sub must defined.")
 
         with self._callback_mutex:
             try:
                 del self._on_message_filtered[sub]
             except KeyError:  # no such subscription
@@ -2936,22 +3036,22 @@
     def _loop_rc_handle(
         self,
         rc: MQTTErrorCode,
     ) -> MQTTErrorCode:
         if rc:
             self._sock_close()
 
-            if self._state in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED):
-                self._state = ConnectionState.MQTT_CS_DISCONNECTED
+            if self._state in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED):
+                self._state = _ConnectionState.MQTT_CS_DISCONNECTED
                 rc = MQTTErrorCode.MQTT_ERR_SUCCESS
 
             self._do_on_disconnect(packet_from_broker=False, v1_rc=rc)
 
         if rc == MQTT_ERR_CONN_LOST:
-            self._state = ConnectionState.MQTT_CS_CONNECTION_LOST
+            self._state = _ConnectionState.MQTT_CS_CONNECTION_LOST
 
         return rc
 
     def _packet_read(self) -> MQTTErrorCode:
         # This gets called if pselect() indicates that there is network data
         # available - ie. at least one byte.  What we do depends on what data we
         # already have.
@@ -3098,15 +3198,15 @@
                                     elif self._callback_api_version == CallbackAPIVersion.VERSION2:
                                         on_publish = cast(CallbackOnPublish_v2, on_publish)
 
                                         on_publish(
                                             self,
                                             self._userdata,
                                             packet["mid"],
-                                            ReasonCodes(PacketTypes.PUBACK),
+                                            ReasonCode(PacketTypes.PUBACK),
                                             Properties(PacketTypes.PUBACK),
                                         )
                                     else:
                                         raise RuntimeError("Unsupported callback API version")
                                 except Exception as err:
                                     self._easy_log(
                                         MQTT_LOG_ERR, 'Caught exception in on_publish: %s', err)
@@ -3127,16 +3227,16 @@
                             packet_from_broker=False,
                             v1_rc=MQTTErrorCode.MQTT_ERR_SUCCESS,
                         )
                         self._sock_close()
                         # Only change to disconnected if the disconnection was wanted
                         # by the client (== state was disconnecting). If the broker disconnected
                         # use unilaterally don't change the state and client may reconnect.
-                        if self._state == ConnectionState.MQTT_CS_DISCONNECTING:
-                            self._state = ConnectionState.MQTT_CS_DISCONNECTED
+                        if self._state == _ConnectionState.MQTT_CS_DISCONNECTING:
+                            self._state = _ConnectionState.MQTT_CS_DISCONNECTED
                         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
                 else:
                     # We haven't finished with this packet
                     self._out_packet.appendleft(packet)
             else:
                 break
@@ -3165,15 +3265,15 @@
         now = time_func()
 
         with self._msgtime_mutex:
             last_msg_out = self._last_msg_out
             last_msg_in = self._last_msg_in
 
         if self._sock is not None and (now - last_msg_out >= self._keepalive or now - last_msg_in >= self._keepalive):
-            if self._state == ConnectionState.MQTT_CS_CONNECTED and self._ping_t == 0:
+            if self._state == _ConnectionState.MQTT_CS_CONNECTED and self._ping_t == 0:
                 try:
                     self._send_pingreq()
                 except Exception:
                     self._sock_close()
                     self._do_on_disconnect(
                         packet_from_broker=False,
                         v1_rc=MQTTErrorCode.MQTT_ERR_CONN_LOST,
@@ -3181,16 +3281,16 @@
                 else:
                     with self._msgtime_mutex:
                         self._last_msg_out = now
                         self._last_msg_in = now
             else:
                 self._sock_close()
 
-                if self._state in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED):
-                    self._state = ConnectionState.MQTT_CS_DISCONNECTED
+                if self._state in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED):
+                    self._state = _ConnectionState.MQTT_CS_DISCONNECTED
                     rc = MQTTErrorCode.MQTT_ERR_SUCCESS
                 else:
                     rc = MQTTErrorCode.MQTT_ERR_KEEPALIVE
 
                 self._do_on_disconnect(
                     packet_from_broker=False,
                     v1_rc=rc,
@@ -3264,25 +3364,25 @@
         packet.extend(struct.pack("!H", len(data)))
         packet.extend(data)
 
     def _send_publish(
         self,
         mid: int,
         topic: bytes,
-        payload: bytes = b"",
+        payload: bytes|bytearray = b"",
         qos: int = 0,
         retain: bool = False,
         dup: bool = False,
         info: MQTTMessageInfo | None = None,
         properties: Properties | None = None,
     ) -> MQTTErrorCode:
         # we assume that topic and payload are already properly encoded
         if not isinstance(topic, bytes):
             raise TypeError('topic must be bytes, not str')
-        if payload and not isinstance(payload, bytes):
+        if payload and not isinstance(payload, (bytes, bytearray)):
             raise TypeError('payload must be bytes if set')
 
         if self._sock is None:
             return MQTTErrorCode.MQTT_ERR_NO_CONN
 
         command = PUBLISH | ((dup & 0x1) << 3) | (qos << 1) | retain
         packet = bytearray()
@@ -3363,15 +3463,15 @@
     def _send_simple_command(self, command: int) -> MQTTErrorCode:
         # For DISCONNECT, PINGREQ and PINGRESP
         remaining_length = 0
         packet = struct.pack('!BB', command, remaining_length)
         return self._packet_queue(command, packet, 0, 0)
 
     def _send_connect(self, keepalive: int) -> MQTTErrorCode:
-        proto_ver = self._protocol
+        proto_ver = int(self._protocol)
         # hard-coded UTF-8 encoded string
         protocol = b"MQTT" if proto_ver >= MQTTv311 else b"MQIsdp"
 
         remaining_length = 2 + len(protocol) + 1 + \
             1 + 2 + 2 + len(self._client_id)
 
         connect_flags = 0
@@ -3469,15 +3569,15 @@
                 keepalive,
                 self._client_id
             )
         return self._packet_queue(command, packet, 0, 0)
 
     def _send_disconnect(
         self,
-        reasoncode: ReasonCodes | None = None,
+        reasoncode: ReasonCode | None = None,
         properties: Properties | None = None,
     ) -> MQTTErrorCode:
         if self._protocol == MQTTv5:
             self._easy_log(MQTT_LOG_DEBUG, "Sending DISCONNECT reasonCode=%s properties=%s",
                            reasoncode,
                            properties
                            )
@@ -3489,15 +3589,15 @@
         command = DISCONNECT
         packet = bytearray()
         packet.append(command)
 
         if self._protocol == MQTTv5:
             if properties is not None or reasoncode is not None:
                 if reasoncode is None:
-                    reasoncode = ReasonCodes(DISCONNECT >> 4, identifier=0)
+                    reasoncode = ReasonCode(DISCONNECT >> 4, identifier=0)
                 remaining_length += 1
                 if properties is not None:
                     packed_props = properties.pack()
                     remaining_length += len(packed_props)
 
         self._pack_remaining_length(packet, remaining_length)
 
@@ -3750,18 +3850,18 @@
 
         if self._protocol == MQTTv5:
             (flags, result) = struct.unpack(
                 "!BB", self._in_packet['packet'][:2])
             if result == 1:
                 # This is probably a failure from a broker that doesn't support
                 # MQTT v5.
-                reason = ReasonCodes(CONNACK >> 4, aName="Unsupported protocol version")
+                reason = ReasonCode(CONNACK >> 4, aName="Unsupported protocol version")
                 properties = None
             else:
-                reason = ReasonCodes(CONNACK >> 4, identifier=result)
+                reason = ReasonCode(CONNACK >> 4, identifier=result)
                 properties = Properties(CONNACK >> 4)
                 properties.unpack(self._in_packet['packet'][2:])
         else:
             (flags, result) = struct.unpack("!BB", self._in_packet['packet'])
             reason = convert_connack_rc_to_reason_code(result)
             properties = None
         if self._protocol == MQTTv311:
@@ -3781,19 +3881,19 @@
                 if not self._reconnect_on_failure:
                     return MQTT_ERR_PROTOCOL
                 self._easy_log(
                     MQTT_LOG_DEBUG,
                     "Received CONNACK (%s, %s), attempting to use non-empty CID",
                     flags, result,
                 )
-                self._client_id = base62(uuid.uuid4().int, padding=22).encode("utf8")
+                self._client_id = _base62(uuid.uuid4().int, padding=22).encode("utf8")
                 return self.reconnect()
 
         if result == 0:
-            self._state = ConnectionState.MQTT_CS_CONNECTED
+            self._state = _ConnectionState.MQTT_CS_CONNECTED
             self._reconnect_delay = None
 
         if self._protocol == MQTTv5:
             self._easy_log(
                 MQTT_LOG_DEBUG, "Received CONNACK (%s, %s) properties=%s", flags, reason, properties)
         else:
             self._easy_log(
@@ -3915,15 +4015,15 @@
         else:
             return MQTTErrorCode.MQTT_ERR_PROTOCOL
 
     def _handle_disconnect(self) -> None:
         packet_type = DISCONNECT >> 4
         reasonCode = properties = None
         if self._in_packet['remaining_length'] > 2:
-            reasonCode = ReasonCodes(packet_type)
+            reasonCode = ReasonCode(packet_type)
             reasonCode.unpack(self._in_packet['packet'])
             if self._in_packet['remaining_length'] > 3:
                 properties = Properties(packet_type)
                 props, props_len = properties.unpack(
                     self._in_packet['packet'][1:])
         self._easy_log(MQTT_LOG_DEBUG, "Received DISCONNECT %s %s",
                        reasonCode,
@@ -3942,19 +4042,19 @@
         self._easy_log(MQTT_LOG_DEBUG, "Received SUBACK")
         pack_format = f"!H{len(self._in_packet['packet']) - 2}s"
         (mid, packet) = struct.unpack(pack_format, self._in_packet['packet'])
 
         if self._protocol == MQTTv5:
             properties = Properties(SUBACK >> 4)
             props, props_len = properties.unpack(packet)
-            reasoncodes = [ReasonCodes(SUBACK >> 4, identifier=c) for c in packet[props_len:]]
+            reasoncodes = [ReasonCode(SUBACK >> 4, identifier=c) for c in packet[props_len:]]
         else:
             pack_format = f"!{'B' * len(packet)}"
             granted_qos = struct.unpack(pack_format, packet)
-            reasoncodes = [ReasonCodes(SUBACK >> 4, identifier=c) for c in granted_qos]
+            reasoncodes = [ReasonCode(SUBACK >> 4, identifier=c) for c in granted_qos]
             properties = Properties(SUBACK >> 4)
 
         with self._callback_mutex:
             on_subscribe = self.on_subscribe
 
         if on_subscribe:
             with self._in_callback_mutex:  # Don't call loop_write after _send_publish()
@@ -4060,45 +4160,45 @@
 
             return rc
         else:
             return MQTTErrorCode.MQTT_ERR_PROTOCOL
 
     def ack(self, mid: int, qos: int) -> MQTTErrorCode:
         """
-           send an acknowledgement for a given message id. (stored in message.mid )
-           only useful in QoS=1 and auto_ack=False
+           send an acknowledgement for a given message id (stored in :py:attr:`message.mid <MQTTMessage.mid>`).
+           only useful in QoS>=1 and ``manual_ack=True`` (option of `Client`)
         """
         if self._manual_ack :
             if qos == 1:
                 return self._send_puback(mid)
             elif qos == 2:
                 return self._send_pubcomp(mid)
 
         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
     def manual_ack_set(self, on: bool) -> None:
         """
            The paho library normally acknowledges messages as soon as they are delivered to the caller.
            If manual_ack is turned on, then the caller MUST manually acknowledge every message once
-           application processing is complete.
+           application processing is complete using `ack()`
         """
         self._manual_ack = on
 
 
     def _handle_pubrel(self) -> MQTTErrorCode:
         if self._protocol == MQTTv5:
             if self._in_packet['remaining_length'] < 2:
                 return MQTTErrorCode.MQTT_ERR_PROTOCOL
         elif self._in_packet['remaining_length'] != 2:
             return MQTTErrorCode.MQTT_ERR_PROTOCOL
 
         mid, = struct.unpack("!H", self._in_packet['packet'][:2])
         if self._protocol == MQTTv5:
             if self._in_packet['remaining_length'] > 2:
-                reasonCode = ReasonCodes(PUBREL >> 4)
+                reasonCode = ReasonCode(PUBREL >> 4)
                 reasonCode.unpack(self._in_packet['packet'][2:])
                 if self._in_packet['remaining_length'] > 3:
                     properties = Properties(PUBREL >> 4)
                     props, props_len = properties.unpack(
                         self._in_packet['packet'][3:])
         self._easy_log(MQTT_LOG_DEBUG, "Received PUBREL (Mid: %d)", mid)
 
@@ -4157,15 +4257,15 @@
                 return MQTTErrorCode.MQTT_ERR_PROTOCOL
         elif self._in_packet['remaining_length'] != 2:
             return MQTTErrorCode.MQTT_ERR_PROTOCOL
 
         mid, = struct.unpack("!H", self._in_packet['packet'][:2])
         if self._protocol == MQTTv5:
             if self._in_packet['remaining_length'] > 2:
-                reasonCode = ReasonCodes(PUBREC >> 4)
+                reasonCode = ReasonCode(PUBREC >> 4)
                 reasonCode.unpack(self._in_packet['packet'][2:])
                 if self._in_packet['remaining_length'] > 3:
                     properties = Properties(PUBREC >> 4)
                     props, props_len = properties.unpack(
                         self._in_packet['packet'][3:])
         self._easy_log(MQTT_LOG_DEBUG, "Received PUBREC (Mid: %d)", mid)
 
@@ -4187,15 +4287,15 @@
 
         mid, = struct.unpack("!H", self._in_packet['packet'][:2])
         if self._protocol == MQTTv5:
             packet = self._in_packet['packet'][2:]
             properties = Properties(UNSUBACK >> 4)
             props, props_len = properties.unpack(packet)
             reasoncodes_list = [
-                ReasonCodes(UNSUBACK >> 4, identifier=c)
+                ReasonCode(UNSUBACK >> 4, identifier=c)
                 for c in packet[props_len:]
             ]
         else:
             reasoncodes_list = []
             properties = Properties(UNSUBACK >> 4)
 
         self._easy_log(MQTT_LOG_DEBUG, "Received UNSUBACK (Mid: %d)", mid)
@@ -4205,15 +4305,15 @@
         if on_unsubscribe:
             with self._in_callback_mutex:
                 try:
                     if self._callback_api_version == CallbackAPIVersion.VERSION1:
                         if self._protocol == MQTTv5:
                             on_unsubscribe = cast(CallbackOnUnsubscribe_v1_mqtt5, on_unsubscribe)
 
-                            reasoncodes: ReasonCodes | list[ReasonCodes] = reasoncodes_list
+                            reasoncodes: ReasonCode | list[ReasonCode] = reasoncodes_list
                             if len(reasoncodes_list) == 1:
                                 reasoncodes = reasoncodes_list[0]
 
                             on_unsubscribe(
                                 self, self._userdata, mid, properties, reasoncodes)
                         else:
                             on_unsubscribe = cast(CallbackOnUnsubscribe_v1_mqtt3, on_unsubscribe)
@@ -4242,15 +4342,15 @@
 
         return MQTTErrorCode.MQTT_ERR_SUCCESS
 
     def _do_on_disconnect(
         self,
         packet_from_broker: bool,
         v1_rc: MQTTErrorCode,
-        reason: ReasonCodes | None = None,
+        reason: ReasonCode | None = None,
         properties: Properties | None = None,
     ) -> None:
         with self._callback_mutex:
             on_disconnect = self.on_disconnect
 
         if on_disconnect:
             with self._in_callback_mutex:
@@ -4291,15 +4391,15 @@
                         raise RuntimeError("Unsupported callback API version")
                 except Exception as err:
                     self._easy_log(
                         MQTT_LOG_ERR, 'Caught exception in on_disconnect: %s', err)
                     if not self.suppress_exceptions:
                         raise
 
-    def _do_on_publish(self, mid: int, reason_code: ReasonCodes, properties: Properties) -> MQTTErrorCode:
+    def _do_on_publish(self, mid: int, reason_code: ReasonCode, properties: Properties) -> MQTTErrorCode:
         with self._callback_mutex:
             on_publish = self.on_publish
 
         if on_publish:
             with self._in_callback_mutex:
                 try:
                     if self._callback_api_version == CallbackAPIVersion.VERSION1:
@@ -4342,15 +4442,15 @@
                 return MQTTErrorCode.MQTT_ERR_PROTOCOL
         elif self._in_packet['remaining_length'] != 2:
             return MQTTErrorCode.MQTT_ERR_PROTOCOL
 
         packet_type_enum = PUBACK if cmd == "PUBACK" else PUBCOMP
         packet_type = packet_type_enum.value >> 4
         mid, = struct.unpack("!H", self._in_packet['packet'][:2])
-        reasonCode = ReasonCodes(packet_type)
+        reasonCode = ReasonCode(packet_type)
         properties = Properties(packet_type)
         if self._protocol == MQTTv5:
             if self._in_packet['remaining_length'] > 2:
                 reasonCode.unpack(self._in_packet['packet'][2:])
                 if self._in_packet['remaining_length'] > 3:
                     props, props_len = properties.unpack(
                         self._in_packet['packet'][3:])
@@ -4415,15 +4515,18 @@
                 try:
                     on_connect_fail(self, self._userdata)
                 except Exception as err:
                     self._easy_log(
                         MQTT_LOG_ERR, 'Caught exception in on_connect_fail: %s', err)
 
     def _thread_main(self) -> None:
-        self.loop_forever(retry_first_connection=True)
+        try:
+            self.loop_forever(retry_first_connection=True)
+        finally:
+            self._thread = None
 
     def _reconnect_wait(self) -> None:
         # See reconnect_delay_set for details
         now = time_func()
         with self._reconnect_delay_mutex:
             if self._reconnect_delay is None:
                 self._reconnect_delay = self._reconnect_min_delay
@@ -4432,15 +4535,15 @@
                     self._reconnect_delay * 2,
                     self._reconnect_max_delay,
                 )
 
             target_time = now + self._reconnect_delay
 
         remaining = target_time - now
-        while (self._state not in (ConnectionState.MQTT_CS_DISCONNECTING, ConnectionState.MQTT_CS_DISCONNECTED)
+        while (self._state not in (_ConnectionState.MQTT_CS_DISCONNECTING, _ConnectionState.MQTT_CS_DISCONNECTED)
                 and not self._thread_terminate
                 and remaining > 0):
 
             time.sleep(min(remaining, 1))
             remaining = target_time - time_func()
 
     @staticmethod
@@ -4496,31 +4599,40 @@
             return dict(zip(proxy_keys, socks_default))
 
         # If we didn't find a proxy through any of the above methods, return
         # None to indicate that the connection should be handled normally
         return None
 
     def _create_socket(self) -> SocketLike:
-        sock = self._create_socket_connection()
+        if self._transport == "unix":
+            sock = self._create_unix_socket_connection()
+        else:
+            sock = self._create_socket_connection()
+
         if self._ssl:
             sock = self._ssl_wrap_socket(sock)
 
         if self._transport == "websockets":
             sock.settimeout(self._keepalive)
-            return WebsocketWrapper(
+            return _WebsocketWrapper(
                 socket=sock,
                 host=self._host,
                 port=self._port,
                 is_ssl=self._ssl,
                 path=self._websocket_path,
                 extra_headers=self._websocket_extra_headers,
             )
 
         return sock
 
+    def _create_unix_socket_connection(self) -> _socket.socket:
+        unix_socket = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
+        unix_socket.connect(self._host)
+        return unix_socket
+
     def _create_socket_connection(self) -> _socket.socket:
         proxy = self._get_proxy()
         addr = (self._host, self._port)
         source = (self._bind_address, self._bind_port)
 
         if proxy:
             return socks.create_connection(addr, timeout=self._connect_timeout, source_address=source, **proxy)
@@ -4562,15 +4674,15 @@
             # TODO: this type error is a true error:
             # error: Module has no attribute "match_hostname"  [attr-defined]
             # Python 3.12 no longer have this method.
             ssl.match_hostname(ssl_sock.getpeercert(), self._host)  # type: ignore
 
         return ssl_sock
 
-class WebsocketWrapper:
+class _WebsocketWrapper:
     OPCODE_CONTINUATION = 0x0
     OPCODE_TEXT = 0x1
     OPCODE_BINARY = 0x2
     OPCODE_CONNCLOSE = 0x8
     OPCODE_PING = 0x9
     OPCODE_PONG = 0xa
 
@@ -4647,15 +4759,18 @@
         self._socket.send(header)
 
         has_secret = False
         has_upgrade = False
 
         while True:
             # read HTTP response header as lines
-            byte = self._socket.recv(1)
+            try:
+                byte = self._socket.recv(1)
+            except ConnectionResetError:
+                byte = b""
 
             self._readbuffer.extend(byte)
 
             # line end
             if byte == b"\n":
                 if len(self._readbuffer) > 2:
                     # check upgrade
@@ -4810,27 +4925,27 @@
 
             # check if full frame arrived and reset readbuffer and payloadhead if needed
             if readindex == payload_length:
                 self._readbuffer = bytearray()
                 self._payload_head = 0
 
                 # respond to non-binary opcodes, their arrival is not guaranteed because of non-blocking sockets
-                if opcode == WebsocketWrapper.OPCODE_CONNCLOSE:
+                if opcode == _WebsocketWrapper.OPCODE_CONNCLOSE:
                     frame = self._create_frame(
-                        WebsocketWrapper.OPCODE_CONNCLOSE, payload, 0)
+                        _WebsocketWrapper.OPCODE_CONNCLOSE, payload, 0)
                     self._socket.send(frame)
 
-                if opcode == WebsocketWrapper.OPCODE_PING:
+                if opcode == _WebsocketWrapper.OPCODE_PING:
                     frame = self._create_frame(
-                        WebsocketWrapper.OPCODE_PONG, payload, 0)
+                        _WebsocketWrapper.OPCODE_PONG, payload, 0)
                     self._socket.send(frame)
 
             # This isn't *proper* handling of continuation frames, but given
             # that we only support binary frames, it is *probably* good enough.
-            if (opcode == WebsocketWrapper.OPCODE_BINARY or opcode == WebsocketWrapper.OPCODE_CONTINUATION) \
+            if (opcode == _WebsocketWrapper.OPCODE_BINARY or opcode == _WebsocketWrapper.OPCODE_CONTINUATION) \
                     and payload_length > 0:
                 return result
             else:
                 raise BlockingIOError
 
         except ConnectionError:
             self.connected = False
@@ -4838,15 +4953,15 @@
 
     def _send_impl(self, data: bytes) -> int:
 
         # if previous frame was sent successfully
         if len(self._sendbuffer) == 0:
             # create websocket frame
             frame = self._create_frame(
-                WebsocketWrapper.OPCODE_BINARY, bytearray(data))
+                _WebsocketWrapper.OPCODE_BINARY, bytearray(data))
             self._sendbuffer.extend(frame)
             self._requested_size = len(data)
 
         # try to write out as much as possible
         length = self._socket.send(self._sendbuffer)
 
         self._sendbuffer = self._sendbuffer[length:]
```

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/matcher.py` & `paho_mqtt-2.1.0/src/paho/mqtt/matcher.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/packettypes.py` & `paho_mqtt-2.1.0/src/paho/mqtt/packettypes.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/properties.py` & `paho_mqtt-2.1.0/src/paho/mqtt/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""
-*******************************************************************
-  Copyright (c) 2017, 2019 IBM Corp.
-
-  All rights reserved. This program and the accompanying materials
-  are made available under the terms of the Eclipse Public License v2.0
-  and Eclipse Distribution License v1.0 which accompany this distribution.
-
-  The Eclipse Public License is available at
-     http://www.eclipse.org/legal/epl-v20.html
-  and the Eclipse Distribution License is available at
-    http://www.eclipse.org/org/documents/edl-v10.php.
-
-  Contributors:
-     Ian Craggs - initial implementation and/or documentation
-*******************************************************************
-"""
+# *******************************************************************
+#   Copyright (c) 2017, 2019 IBM Corp.
+#
+#   All rights reserved. This program and the accompanying materials
+#   are made available under the terms of the Eclipse Public License v2.0
+#   and Eclipse Distribution License v1.0 which accompany this distribution.
+#
+#   The Eclipse Public License is available at
+#      http://www.eclipse.org/legal/epl-v20.html
+#   and the Eclipse Distribution License is available at
+#     http://www.eclipse.org/org/documents/edl-v10.php.
+#
+#   Contributors:
+#      Ian Craggs - initial implementation and/or documentation
+# *******************************************************************
 
 import struct
 
 from .packettypes import PacketTypes
 
 
 class MQTTException(Exception):
@@ -137,22 +135,22 @@
 class Properties:
     """MQTT v5.0 properties class.
 
     See Properties.names for a list of accepted property names along with their numeric values.
 
     See Properties.properties for the data type of each property.
 
-    Example of use:
+    Example of use::
 
         publish_properties = Properties(PacketTypes.PUBLISH)
         publish_properties.UserProperty = ("a", "2")
         publish_properties.UserProperty = ("c", "3")
 
     First the object is created with packet type as argument, no properties will be present at
-    this point.  Then properties are added as attributes, the name of which is the string property
+    this point. Then properties are added as attributes, the name of which is the string property
     name without the spaces.
 
     """
 
     def __init__(self, packetType):
         self.packetType = packetType
         self.types = ["Byte", "Two Byte Integer", "Four Byte Integer", "Variable Byte Integer",
```

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/publish.py` & `paho_mqtt-2.1.0/src/paho/mqtt/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 """
 from __future__ import annotations
 
 import collections
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, List, Tuple, Union
 
-from paho.mqtt.enums import CallbackAPIVersion
+from paho.mqtt.enums import CallbackAPIVersion, MQTTProtocolVersion
 from paho.mqtt.properties import Properties
-from paho.mqtt.reasoncodes import ReasonCodes
+from paho.mqtt.reasoncodes import ReasonCode
 
 from .. import mqtt
 from . import client as paho
 
 if TYPE_CHECKING:
     try:
         from typing import NotRequired, Required, TypedDict  # type: ignore
@@ -88,15 +88,15 @@
         if len(userdata) > 0:
             _do_publish(client)
     else:
         raise mqtt.MQTTException(paho.connack_string(reason_code))
 
 
 def _on_publish(
-    client: paho.Client, userdata: collections.deque[MessagesList], mid: int, reason_codes: ReasonCodes, properties: Properties,
+    client: paho.Client, userdata: collections.deque[MessagesList], mid: int, reason_codes: ReasonCode, properties: Properties,
 ) -> None:
     """Internal callback"""
     #pylint: disable=unused-argument
 
     if len(userdata) == 0:
         client.disconnect()
     else:
@@ -108,25 +108,25 @@
     hostname: str = "localhost",
     port: int = 1883,
     client_id: str = "",
     keepalive: int = 60,
     will: MessageDict | None = None,
     auth: AuthParameter | None = None,
     tls: TLSParameter | None = None,
-    protocol: int = paho.MQTTv311,
+    protocol: MQTTProtocolVersion = paho.MQTTv311,
     transport: Literal["tcp", "websockets"] = "tcp",
     proxy_args: Any | None = None,
 ) -> None:
     """Publish multiple messages to a broker, then disconnect cleanly.
 
     This function creates an MQTT client, connects to a broker and publishes a
     list of messages. Once the messages have been delivered, it disconnects
     cleanly from the broker.
 
-    msgs : a list of messages to publish. Each message is either a dict or a
+    :param msgs: a list of messages to publish. Each message is either a dict or a
            tuple.
 
            If a dict, only the topic must be present. Default values will be
            used for any missing arguments. The dict must be of the form:
 
            msg = {'topic':"<topic>", 'payload':"<payload>", 'qos':<qos>,
            'retain':<retain>}
@@ -135,51 +135,52 @@
            will be published.
            If qos is not present, the default of 0 is used.
            If retain is not present, the default of False is used.
 
            If a tuple, then it must be of the form:
            ("<topic>", "<payload>", qos, retain)
 
-    hostname : a string containing the address of the broker to connect to.
+    :param str hostname: the address of the broker to connect to.
                Defaults to localhost.
 
-    port : the port to connect to the broker on. Defaults to 1883.
+    :param int port: the port to connect to the broker on. Defaults to 1883.
 
-    client_id : the MQTT client id to use. If "" or None, the Paho library will
+    :param str client_id: the MQTT client id to use. If "" or None, the Paho library will
                 generate a client id automatically.
 
-    keepalive : the keepalive timeout value for the client. Defaults to 60
+    :param int keepalive: the keepalive timeout value for the client. Defaults to 60
                 seconds.
 
-    will : a dict containing will parameters for the client: will = {'topic':
+    :param will: a dict containing will parameters for the client: will = {'topic':
            "<topic>", 'payload':"<payload">, 'qos':<qos>, 'retain':<retain>}.
            Topic is required, all other parameters are optional and will
            default to None, 0 and False respectively.
            Defaults to None, which indicates no will should be used.
 
-    auth : a dict containing authentication parameters for the client:
+    :param auth: a dict containing authentication parameters for the client:
            auth = {'username':"<username>", 'password':"<password>"}
            Username is required, password is optional and will default to None
            if not provided.
            Defaults to None, which indicates no authentication is to be used.
 
-    tls : a dict containing TLS configuration parameters for the client:
+    :param tls: a dict containing TLS configuration parameters for the client:
           dict = {'ca_certs':"<ca_certs>", 'certfile':"<certfile>",
           'keyfile':"<keyfile>", 'tls_version':"<tls_version>",
           'ciphers':"<ciphers">, 'insecure':"<bool>"}
           ca_certs is required, all other parameters are optional and will
           default to None if not provided, which results in the client using
           the default behaviour - see the paho.mqtt.client documentation.
           Alternatively, tls input can be an SSLContext object, which will be
           processed using the tls_set_context method.
           Defaults to None, which indicates that TLS should not be used.
 
-    transport : set to "tcp" to use the default setting of transport which is
+    :param str transport: set to "tcp" to use the default setting of transport which is
           raw TCP. Set to "websockets" to use WebSockets as the transport.
-    proxy_args: a dictionary that will be given to the client.
+
+    :param proxy_args: a dictionary that will be given to the client.
     """
 
     if not isinstance(msgs, Iterable):
         raise TypeError('msgs must be an iterable')
     if len(msgs) == 0:
         raise ValueError('msgs is empty')
 
@@ -187,14 +188,15 @@
         CallbackAPIVersion.VERSION2,
         client_id=client_id,
         userdata=collections.deque(msgs),
         protocol=protocol,
         transport=transport,
     )
 
+    client.enable_logger()
     client.on_publish = _on_publish
     client.on_connect = _on_connect  # type: ignore
 
     if proxy_args is not None:
         client.proxy_set(**proxy_args)
 
     if auth:
@@ -234,70 +236,71 @@
     hostname: str = "localhost",
     port: int = 1883,
     client_id: str = "",
     keepalive: int = 60,
     will: MessageDict | None = None,
     auth: AuthParameter | None = None,
     tls: TLSParameter | None = None,
-    protocol: int = paho.MQTTv311,
+    protocol: MQTTProtocolVersion = paho.MQTTv311,
     transport: Literal["tcp", "websockets"] = "tcp",
     proxy_args: Any | None = None,
 ) -> None:
     """Publish a single message to a broker, then disconnect cleanly.
 
     This function creates an MQTT client, connects to a broker and publishes a
     single message. Once the message has been delivered, it disconnects cleanly
     from the broker.
 
-    topic : the only required argument must be the topic string to which the
+    :param str topic: the only required argument must be the topic string to which the
             payload will be published.
 
-    payload : the payload to be published. If "" or None, a zero length payload
+    :param payload: the payload to be published. If "" or None, a zero length payload
               will be published.
 
-    qos : the qos to use when publishing,  default to 0.
+    :param int qos: the qos to use when publishing,  default to 0.
 
-    retain : set the message to be retained (True) or not (False).
+    :param bool retain: set the message to be retained (True) or not (False).
 
-    hostname : a string containing the address of the broker to connect to.
+    :param str hostname: the address of the broker to connect to.
                Defaults to localhost.
 
-    port : the port to connect to the broker on. Defaults to 1883.
+    :param int port: the port to connect to the broker on. Defaults to 1883.
 
-    client_id : the MQTT client id to use. If "" or None, the Paho library will
+    :param str client_id: the MQTT client id to use. If "" or None, the Paho library will
                 generate a client id automatically.
 
-    keepalive : the keepalive timeout value for the client. Defaults to 60
+    :param int keepalive: the keepalive timeout value for the client. Defaults to 60
                 seconds.
 
-    will : a dict containing will parameters for the client: will = {'topic':
+    :param will: a dict containing will parameters for the client: will = {'topic':
            "<topic>", 'payload':"<payload">, 'qos':<qos>, 'retain':<retain>}.
            Topic is required, all other parameters are optional and will
            default to None, 0 and False respectively.
            Defaults to None, which indicates no will should be used.
 
-    auth : a dict containing authentication parameters for the client:
-           auth = {'username':"<username>", 'password':"<password>"}
+    :param auth: a dict containing authentication parameters for the client:
            Username is required, password is optional and will default to None
+           auth = {'username':"<username>", 'password':"<password>"}
            if not provided.
            Defaults to None, which indicates no authentication is to be used.
 
-    tls : a dict containing TLS configuration parameters for the client:
+    :param tls: a dict containing TLS configuration parameters for the client:
           dict = {'ca_certs':"<ca_certs>", 'certfile':"<certfile>",
           'keyfile':"<keyfile>", 'tls_version':"<tls_version>",
           'ciphers':"<ciphers">, 'insecure':"<bool>"}
           ca_certs is required, all other parameters are optional and will
           default to None if not provided, which results in the client using
           the default behaviour - see the paho.mqtt.client documentation.
           Defaults to None, which indicates that TLS should not be used.
           Alternatively, tls input can be an SSLContext object, which will be
           processed using the tls_set_context method.
 
-    transport : set to "tcp" to use the default setting of transport which is
+    :param transport: set to "tcp" to use the default setting of transport which is
           raw TCP. Set to "websockets" to use WebSockets as the transport.
-    proxy_args: a dictionary that will be given to the client.
+
+    :param proxy_args: a dictionary that will be given to the client.
     """
 
     msg: MessageDict = {'topic':topic, 'payload':payload, 'qos':qos, 'retain':retain}
 
     multiple([msg], hostname, port, client_id, keepalive, will, auth, tls,
              protocol, transport, proxy_args)
```

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/reasoncodes.py` & `paho_mqtt-2.1.0/src/paho/mqtt/reasoncodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-*******************************************************************
-  Copyright (c) 2017, 2019 IBM Corp.
-
-  All rights reserved. This program and the accompanying materials
-  are made available under the terms of the Eclipse Public License v2.0
-  and Eclipse Distribution License v1.0 which accompany this distribution.
-
-  The Eclipse Public License is available at
-     http://www.eclipse.org/legal/epl-v20.html
-  and the Eclipse Distribution License is available at
-    http://www.eclipse.org/org/documents/edl-v10.php.
-
-  Contributors:
-     Ian Craggs - initial implementation and/or documentation
-*******************************************************************
-"""
+# *******************************************************************
+#   Copyright (c) 2017, 2019 IBM Corp.
+#
+#   All rights reserved. This program and the accompanying materials
+#   are made available under the terms of the Eclipse Public License v2.0
+#   and Eclipse Distribution License v1.0 which accompany this distribution.
+#
+#   The Eclipse Public License is available at
+#      http://www.eclipse.org/legal/epl-v20.html
+#   and the Eclipse Distribution License is available at
+#     http://www.eclipse.org/org/documents/edl-v10.php.
+#
+#   Contributors:
+#      Ian Craggs - initial implementation and/or documentation
+# *******************************************************************
 
 import functools
+import warnings
+from typing import Any
 
 from .packettypes import PacketTypes
 
 
 @functools.total_ordering
-class ReasonCodes:
+class ReasonCode:
     """MQTT version 5.0 reason codes class.
 
-    See ReasonCodes.names for a list of possible numeric values along with their
+    See ReasonCode.names for a list of possible numeric values along with their
     names and the packets to which they apply.
 
     """
 
-    def __init__(self, packetType, aName="Success", identifier=-1):
+    def __init__(self, packetType: int, aName: str ="Success", identifier: int =-1):
         """
         packetType: the type of the packet, such as PacketTypes.CONNECT that
             this reason code will be used with.  Some reason codes have different
             names for the same identifier when used a different packet type.
 
         aName: the String name of the reason code to be created.  Ignored
             if the identifier is set.
@@ -172,26 +172,52 @@
         return self.__getName__(self.packetType, self.value)
 
     def __eq__(self, other):
         if isinstance(other, int):
             return self.value == other
         if isinstance(other, str):
             return other == str(self)
-        if isinstance(other, ReasonCodes):
+        if isinstance(other, ReasonCode):
             return self.value == other.value
         return False
 
     def __lt__(self, other):
         if isinstance(other, int):
             return self.value < other
-        if isinstance(other, ReasonCodes):
+        if isinstance(other, ReasonCode):
             return self.value < other.value
         return NotImplemented
 
+    def __repr__(self):
+        try:
+            packet_name = PacketTypes.Names[self.packetType]
+        except IndexError:
+            packet_name = "Unknown"
+
+        return f"ReasonCode({packet_name}, {self.getName()!r})"
+
     def __str__(self):
         return self.getName()
 
     def json(self):
         return self.getName()
 
     def pack(self):
         return bytearray([self.value])
+
+    @property
+    def is_failure(self) -> bool:
+        return self.value >= 0x80
+
+
+class _CompatibilityIsInstance(type):
+    def __instancecheck__(self, other: Any) -> bool:
+        return isinstance(other, ReasonCode)
+
+
+class ReasonCodes(ReasonCode, metaclass=_CompatibilityIsInstance):
+    def __init__(self, *args, **kwargs):
+        warnings.warn("ReasonCodes is deprecated, use ReasonCode (singular) instead",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init__(*args, **kwargs)
```

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/subscribe.py` & `paho_mqtt-2.1.0/src/paho/mqtt/subscribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,69 +68,70 @@
              clean_session=True, proxy_args=None):
     """Subscribe to a list of topics and process them in a callback function.
 
     This function creates an MQTT client, connects to a broker and subscribes
     to a list of topics. Incoming messages are processed by the user provided
     callback.  This is a blocking function and will never return.
 
-    callback : function of the form "on_message(client, userdata, message)" for
+    :param callback: function with the same signature as `on_message` for
                processing the messages received.
 
-    topics : either a string containing a single topic to subscribe to, or a
+    :param topics: either a string containing a single topic to subscribe to, or a
              list of topics to subscribe to.
 
-    qos : the qos to use when subscribing. This is applied to all topics.
+    :param int qos: the qos to use when subscribing. This is applied to all topics.
 
-    userdata : passed to the callback
+    :param userdata: passed to the callback
 
-    hostname : a string containing the address of the broker to connect to.
+    :param str hostname: the address of the broker to connect to.
                Defaults to localhost.
 
-    port : the port to connect to the broker on. Defaults to 1883.
+    :param int port: the port to connect to the broker on. Defaults to 1883.
 
-    client_id : the MQTT client id to use. If "" or None, the Paho library will
+    :param str client_id: the MQTT client id to use. If "" or None, the Paho library will
                 generate a client id automatically.
 
-    keepalive : the keepalive timeout value for the client. Defaults to 60
+    :param int keepalive: the keepalive timeout value for the client. Defaults to 60
                 seconds.
 
-    will : a dict containing will parameters for the client: will = {'topic':
+    :param will: a dict containing will parameters for the client: will = {'topic':
            "<topic>", 'payload':"<payload">, 'qos':<qos>, 'retain':<retain>}.
            Topic is required, all other parameters are optional and will
            default to None, 0 and False respectively.
+
            Defaults to None, which indicates no will should be used.
 
-    auth : a dict containing authentication parameters for the client:
+    :param auth: a dict containing authentication parameters for the client:
            auth = {'username':"<username>", 'password':"<password>"}
            Username is required, password is optional and will default to None
            if not provided.
            Defaults to None, which indicates no authentication is to be used.
 
-    tls : a dict containing TLS configuration parameters for the client:
+    :param tls: a dict containing TLS configuration parameters for the client:
           dict = {'ca_certs':"<ca_certs>", 'certfile':"<certfile>",
           'keyfile':"<keyfile>", 'tls_version':"<tls_version>",
           'ciphers':"<ciphers">, 'insecure':"<bool>"}
           ca_certs is required, all other parameters are optional and will
           default to None if not provided, which results in the client using
           the default behaviour - see the paho.mqtt.client documentation.
           Alternatively, tls input can be an SSLContext object, which will be
           processed using the tls_set_context method.
           Defaults to None, which indicates that TLS should not be used.
 
-    transport : set to "tcp" to use the default setting of transport which is
+    :param str transport: set to "tcp" to use the default setting of transport which is
           raw TCP. Set to "websockets" to use WebSockets as the transport.
 
-    clean_session : a boolean that determines the client type. If True,
+    :param clean_session: a boolean that determines the client type. If True,
                     the broker will remove all information about this client
                     when it disconnects. If False, the client is a persistent
                     client and subscription information and queued messages
                     will be retained when the client disconnects.
                     Defaults to True.
 
-    proxy_args: a dictionary that will be given to the client.
+    :param proxy_args: a dictionary that will be given to the client.
     """
 
     if qos < 0 or qos > 2:
         raise ValueError('qos must be in the range 0-2')
 
     callback_userdata = {
         'callback':callback,
@@ -142,14 +143,15 @@
         paho.CallbackAPIVersion.VERSION2,
         client_id=client_id,
         userdata=callback_userdata,
         protocol=protocol,
         transport=transport,
         clean_session=clean_session,
     )
+    client.enable_logger()
 
     client.on_message = _on_message_callback
     client.on_connect = _on_connect
 
     if proxy_args is not None:
         client.proxy_set(**proxy_args)
 
@@ -187,77 +189,77 @@
            clean_session=True, proxy_args=None):
     """Subscribe to a list of topics and return msg_count messages.
 
     This function creates an MQTT client, connects to a broker and subscribes
     to a list of topics. Once "msg_count" messages have been received, it
     disconnects cleanly from the broker and returns the messages.
 
-    topics : either a string containing a single topic to subscribe to, or a
+    :param topics: either a string containing a single topic to subscribe to, or a
              list of topics to subscribe to.
 
-    qos : the qos to use when subscribing. This is applied to all topics.
+    :param int qos: the qos to use when subscribing. This is applied to all topics.
 
-    msg_count : the number of messages to retrieve from the broker.
+    :param int msg_count: the number of messages to retrieve from the broker.
                 if msg_count == 1 then a single MQTTMessage will be returned.
                 if msg_count > 1 then a list of MQTTMessages will be returned.
 
-    retained : If set to True, retained messages will be processed the same as
+    :param bool retained: If set to True, retained messages will be processed the same as
                non-retained messages. If set to False, retained messages will
                be ignored. This means that with retained=False and msg_count=1,
                the function will return the first message received that does
                not have the retained flag set.
 
-    hostname : a string containing the address of the broker to connect to.
+    :param str hostname: the address of the broker to connect to.
                Defaults to localhost.
 
-    port : the port to connect to the broker on. Defaults to 1883.
+    :param int port: the port to connect to the broker on. Defaults to 1883.
 
-    client_id : the MQTT client id to use. If "" or None, the Paho library will
+    :param str client_id: the MQTT client id to use. If "" or None, the Paho library will
                 generate a client id automatically.
 
-    keepalive : the keepalive timeout value for the client. Defaults to 60
+    :param int keepalive: the keepalive timeout value for the client. Defaults to 60
                 seconds.
 
-    will : a dict containing will parameters for the client: will = {'topic':
+    :param will: a dict containing will parameters for the client: will = {'topic':
            "<topic>", 'payload':"<payload">, 'qos':<qos>, 'retain':<retain>}.
            Topic is required, all other parameters are optional and will
            default to None, 0 and False respectively.
            Defaults to None, which indicates no will should be used.
 
-    auth : a dict containing authentication parameters for the client:
+    :param auth: a dict containing authentication parameters for the client:
            auth = {'username':"<username>", 'password':"<password>"}
            Username is required, password is optional and will default to None
            if not provided.
            Defaults to None, which indicates no authentication is to be used.
 
-    tls : a dict containing TLS configuration parameters for the client:
+    :param tls: a dict containing TLS configuration parameters for the client:
           dict = {'ca_certs':"<ca_certs>", 'certfile':"<certfile>",
           'keyfile':"<keyfile>", 'tls_version':"<tls_version>",
           'ciphers':"<ciphers">, 'insecure':"<bool>"}
           ca_certs is required, all other parameters are optional and will
           default to None if not provided, which results in the client using
           the default behaviour - see the paho.mqtt.client documentation.
           Alternatively, tls input can be an SSLContext object, which will be
           processed using the tls_set_context method.
           Defaults to None, which indicates that TLS should not be used.
 
-    protocol : the MQTT protocol version to use. Defaults to MQTTv311.
+    :param protocol: the MQTT protocol version to use. Defaults to MQTTv311.
 
-    transport : set to "tcp" to use the default setting of transport which is
+    :param transport: set to "tcp" to use the default setting of transport which is
           raw TCP. Set to "websockets" to use WebSockets as the transport.
 
-    clean_session : a boolean that determines the client type. If True,
+    :param clean_session: a boolean that determines the client type. If True,
                     the broker will remove all information about this client
                     when it disconnects. If False, the client is a persistent
                     client and subscription information and queued messages
                     will be retained when the client disconnects.
                     Defaults to True. If protocol is MQTTv50, clean_session
                     is ignored.
 
-    proxy_args: a dictionary that will be given to the client.
+    :param proxy_args: a dictionary that will be given to the client.
     """
 
     if msg_count < 1:
         raise ValueError('msg_count must be > 0')
 
     # Set ourselves up to return a single message if msg_count == 1, or a list
     # if > 1.
```

### Comparing `paho_mqtt-2.0.0rc2/src/paho/mqtt/subscribeoptions.py` & `paho_mqtt-2.1.0/src/paho/mqtt/subscribeoptions.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/debug_helpers.py` & `paho_mqtt-2.1.0/tests/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/mqtt5_props.py` & `paho_mqtt-2.1.0/tests/mqtt5_props.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/paho_test.py` & `paho_mqtt-2.1.0/tests/paho_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     assert packet_matches(name, packet_recvd, expected)
     return True
 
 
 def expect_no_packet(sock, delay=1):
     """ expect that nothing is received within given delay
     """
-    sock.settimeout(delay)
     try:
         previous_timeout = sock.gettimeout()
+        sock.settimeout(delay)
         data = sock.recv(1024)
     except socket.timeout:
         data = None
     finally:
         sock.settimeout(previous_timeout)
 
     if data is not None:
@@ -224,15 +224,16 @@
     if proto_ver == 5:
         properties = mqtt5_props.prop_finalise(properties)
         rl += len(properties)
         # This will break if len(properties) > 127
         pack_format = pack_format + "%ds"%(len(properties))
 
     if payload is not None:
-        payload = payload.encode("utf-8")
+        if isinstance(payload, str):
+            payload = payload.encode("utf-8")
         rl = rl + len(payload)
         pack_format = pack_format + str(len(payload)) + "s"
     else:
         payload = b""
         pack_format = pack_format + "0s"
 
     rlpacked = pack_remaining_length(rl)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/test_client.py` & `paho_mqtt-2.1.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import unicodedata
 
 import paho.mqtt.client as client
 import pytest
 from paho.mqtt.enums import CallbackAPIVersion, MQTTErrorCode, MQTTProtocolVersion
 from paho.mqtt.packettypes import PacketTypes
 from paho.mqtt.properties import Properties
-from paho.mqtt.reasoncodes import ReasonCodes
+from paho.mqtt.reasoncodes import ReasonCode
 
 import tests.paho_test as paho_test
 
 # Import test fixture
 from tests.testsupport.broker import FakeBroker, fake_broker  # noqa: F401
 
 
@@ -27,14 +27,15 @@
     """
 
     def test_01_con_discon_success(self, proto_ver, callback_version, fake_broker):
         mqttc = client.Client(
             callback_version,
             "01-con-discon-success",
             protocol=proto_ver,
+            transport=fake_broker.transport,
         )
 
         def on_connect(mqttc, obj, flags, rc_or_reason_code, properties_or_none=None):
             assert rc_or_reason_code == 0
             mqttc.disconnect()
 
         mqttc.on_connect = on_connect
@@ -66,23 +67,24 @@
             mqttc.loop_stop()
 
         packet_in = fake_broker.receive_packet(1)
         assert not packet_in  # Check connection is closed
 
     def test_01_con_failure_rc(self, proto_ver, callback_version, fake_broker):
         mqttc = client.Client(
-            callback_version, "01-con-failure-rc", protocol=proto_ver)
+            callback_version, "01-con-failure-rc",
+            protocol=proto_ver, transport=fake_broker.transport)
 
         def on_connect(mqttc, obj, flags, rc_or_reason_code, properties_or_none=None):
             assert rc_or_reason_code > 0
             assert rc_or_reason_code != 0
             if callback_version == CallbackAPIVersion.VERSION1:
                 assert rc_or_reason_code == 1
             else:
-                assert rc_or_reason_code == ReasonCodes(PacketTypes.CONNACK, "Unsupported protocol version")
+                assert rc_or_reason_code == ReasonCode(PacketTypes.CONNACK, "Unsupported protocol version")
 
         mqttc.on_connect = on_connect
 
         mqttc.connect_async("localhost", fake_broker.port)
         mqttc.loop_start()
 
         try:
@@ -103,15 +105,17 @@
             packet_in = fake_broker.receive_packet(1)
             assert not packet_in  # Check connection is closed
 
         finally:
             mqttc.loop_stop()
 
     def test_connection_properties(self, proto_ver, callback_version, fake_broker):
-        mqttc = client.Client(CallbackAPIVersion.VERSION2, "client-id", protocol=proto_ver)
+        mqttc = client.Client(
+            CallbackAPIVersion.VERSION2, "client-id",
+            protocol=proto_ver, transport=fake_broker.transport)
         mqttc.enable_logger()
 
         is_connected = threading.Event()
         is_disconnected = threading.Event()
 
         def on_connect(mqttc, obj, flags, rc, properties):
             assert rc == 0
@@ -127,15 +131,15 @@
 
         mqttc.host = "localhost"
         mqttc.connect_timeout = 7
         mqttc.port = fake_broker.port
         mqttc.keepalive = 7
         mqttc.max_inflight_messages = 7
         mqttc.max_queued_messages = 7
-        mqttc.transport = "tcp"
+        mqttc.transport = fake_broker.transport
         mqttc.username = "username"
         mqttc.password = "password"
 
         mqttc.reconnect()
 
         # As soon as connection try to be established, no longer accept updates
         with pytest.raises(RuntimeError):
@@ -180,15 +184,15 @@
             with pytest.raises(RuntimeError):
                 mqttc.max_inflight_messages = 7
 
             with pytest.raises(RuntimeError):
                 mqttc.max_queued_messages = 7
 
             with pytest.raises(RuntimeError):
-                mqttc.transport = "tcp"
+                mqttc.transport = fake_broker.transport
 
             with pytest.raises(RuntimeError):
                 mqttc.username = "username"
 
             with pytest.raises(RuntimeError):
                 mqttc.password = "password"
 
@@ -213,19 +217,21 @@
 
 class Test_connect_v5:
     """
     Tests on connect/disconnect behaviour of the client with MQTTv5
     """
 
     def test_01_broker_no_support(self, fake_broker):
-        mqttc = client.Client(CallbackAPIVersion.VERSION2, "01-broker-no-support", protocol=MQTTProtocolVersion.MQTTv5)
+        mqttc = client.Client(
+            CallbackAPIVersion.VERSION2, "01-broker-no-support",
+            protocol=MQTTProtocolVersion.MQTTv5, transport=fake_broker.transport)
 
         def on_connect(mqttc, obj, flags, reason, properties):
             assert reason == 132
-            assert reason == ReasonCodes(client.CONNACK >> 4, aName="Unsupported protocol version")
+            assert reason == ReasonCode(client.CONNACK >> 4, aName="Unsupported protocol version")
             mqttc.disconnect()
 
         mqttc.on_connect = on_connect
 
         mqttc.connect_async("localhost", fake_broker.port)
         mqttc.loop_start()
 
@@ -257,14 +263,15 @@
 class TestConnectionLost:
     def test_with_loop_start(self, fake_broker: FakeBroker):
         mqttc = client.Client(
             CallbackAPIVersion.VERSION1,
             "test_with_loop_start",
             protocol=MQTTProtocolVersion.MQTTv311,
             reconnect_on_failure=False,
+            transport=fake_broker.transport
         )
 
         on_connect_reached = threading.Event()
         on_disconnect_reached = threading.Event()
 
 
         def on_connect(mqttc, obj, flags, rc):
@@ -307,14 +314,15 @@
             mqttc.loop_stop()
 
     def test_with_loop(self, fake_broker: FakeBroker):
         mqttc = client.Client(
             CallbackAPIVersion.VERSION1,
             "test_with_loop",
             clean_session=True,
+            transport=fake_broker.transport,
         )
 
         on_connect_reached = threading.Event()
         on_disconnect_reached = threading.Event()
 
 
         def on_connect(mqttc, obj, flags, rc):
@@ -363,14 +371,15 @@
 
 
 class TestPublish:
     def test_publish_before_connect(self, fake_broker: FakeBroker) -> None:
         mqttc = client.Client(
             CallbackAPIVersion.VERSION1,
             "test_publish_before_connect",
+            transport=fake_broker.transport,
         )
 
         def on_connect(mqttc, obj, flags, rc):
             assert rc == 0
 
         mqttc.on_connect = on_connect
 
@@ -414,21 +423,74 @@
 
         finally:
             mqttc.loop_stop()
 
         packet_in = fake_broker.receive_packet(1)
         assert not packet_in  # Check connection is closed
 
+    @pytest.mark.parametrize("user_payload,sent_payload", [
+        ("string", b"string"),
+        (b"byte", b"byte"),
+        (bytearray(b"bytearray"), b"bytearray"),
+        (42, b"42"),
+        (4.2, b"4.2"),
+        (None, b""),
+    ])
+    def test_publish_various_payload(self, user_payload: client.PayloadType, sent_payload: bytes, fake_broker: FakeBroker) -> None:
+        mqttc = client.Client(
+            CallbackAPIVersion.VERSION2,
+            "test_publish_various_payload",
+            transport=fake_broker.transport,
+        )
+
+        mqttc.connect("localhost", fake_broker.port)
+        mqttc.loop_start()
+        mqttc.enable_logger()
+
+        try:
+            fake_broker.start()
+
+            connect_packet = paho_test.gen_connect(
+                "test_publish_various_payload", keepalive=60,
+                proto_ver=client.MQTTv311)
+            fake_broker.expect_packet("connect", connect_packet)
+
+            connack_packet = paho_test.gen_connack(rc=0)
+            count = fake_broker.send_packet(connack_packet)
+            assert count  # Check connection was not closed
+            assert count == len(connack_packet)
+
+            mqttc.publish("test", user_payload)
+
+            publish_packet = paho_test.gen_publish(
+                b"test", payload=sent_payload, qos=0
+            )
+            fake_broker.expect_packet("publish", publish_packet)
+
+            mqttc.disconnect()
+
+            disconnect_packet = paho_test.gen_disconnect()
+            packet_in = fake_broker.receive_packet(1000)
+            assert packet_in  # Check connection was not closed
+            assert packet_in == disconnect_packet
+
+        finally:
+            mqttc.loop_stop()
+
+        packet_in = fake_broker.receive_packet(1)
+        assert not packet_in  # Check connection is closed
+
+
 @pytest.mark.parametrize("callback_version", [
     (CallbackAPIVersion.VERSION1),
     (CallbackAPIVersion.VERSION2),
 ])
 class TestPublishBroker2Client:
     def test_invalid_utf8_topic(self, callback_version, fake_broker):
-        mqttc = client.Client(callback_version, "client-id")
+        mqttc = client.Client(callback_version, "client-id", transport=fake_broker.transport)
 
         def on_message(client, userdata, msg):
             with pytest.raises(UnicodeDecodeError):
                 assert msg.topic
             client.disconnect()
 
         mqttc.on_message = on_message
@@ -462,15 +524,15 @@
         finally:
             mqttc.loop_stop()
 
         packet_in = fake_broker.receive_packet(1)
         assert not packet_in  # Check connection is closed
 
     def test_valid_utf8_topic_recv(self, callback_version, fake_broker):
-        mqttc = client.Client(callback_version, "client-id")
+        mqttc = client.Client(callback_version, "client-id", transport=fake_broker.transport)
 
         # It should be non-ascii multi-bytes character
         topic = unicodedata.lookup('SNOWMAN')
 
         def on_message(client, userdata, msg):
             assert msg.topic == topic
             client.disconnect()
@@ -508,15 +570,15 @@
         finally:
             mqttc.loop_stop()
 
         packet_in = fake_broker.receive_packet(1)
         assert not packet_in  # Check connection is closed
 
     def test_valid_utf8_topic_publish(self, callback_version, fake_broker):
-        mqttc = client.Client(callback_version, "client-id")
+        mqttc = client.Client(callback_version, "client-id", transport=fake_broker.transport)
 
         # It should be non-ascii multi-bytes character
         topic = unicodedata.lookup('SNOWMAN')
 
         mqttc.connect_async("localhost", fake_broker.port)
         mqttc.loop_start()
 
@@ -554,15 +616,15 @@
         finally:
             mqttc.loop_stop()
 
         packet_in = fake_broker.receive_packet(1)
         assert not packet_in  # Check connection is closed
 
     def test_message_callback(self, callback_version, fake_broker):
-        mqttc = client.Client(callback_version, "client-id")
+        mqttc = client.Client(callback_version, "client-id", transport=fake_broker.transport)
         userdata = {
             'on_message': 0,
             'callback1': 0,
             'callback2': 0,
         }
         mqttc.user_data_set(userdata)
 
@@ -684,24 +746,25 @@
         assert rc_again < 0
 
         # This might probably not be done: User might use rc as number in
         # operation
         assert rc_ok + 1 == 1
 
     def test_migration_callback_version(self):
-        with pytest.raises(ValueError, match="see migrations.md"):
+        with pytest.raises(ValueError, match="see docs/migrations.rst"):
             _ = client.Client("client-id")
 
     def test_callback_v1_mqtt3(self, fake_broker):
         callback_called = []
         with pytest.deprecated_call():
             mqttc = client.Client(
                 CallbackAPIVersion.VERSION1,
                 "client-id",
                 userdata=callback_called,
+                transport=fake_broker.transport,
             )
 
         def on_connect(cl, userdata, flags, rc):
             assert isinstance(cl, client.Client)
             assert isinstance(flags, dict)
             assert isinstance(flags["session present"], int)
             assert isinstance(rc, int)
@@ -819,40 +882,41 @@
 
     def test_callback_v2_mqtt3(self, fake_broker):
         callback_called = []
         mqttc = client.Client(
             CallbackAPIVersion.VERSION2,
             "client-id",
             userdata=callback_called,
+            transport=fake_broker.transport,
         )
 
         def on_connect(cl, userdata, flags, reason, properties):
             assert isinstance(cl, client.Client)
             assert isinstance(flags, client.ConnectFlags)
-            assert isinstance(reason, ReasonCodes)
+            assert isinstance(reason, ReasonCode)
             assert isinstance(properties, Properties)
             assert reason == 0
             assert properties.isEmpty()
             userdata.append("on_connect")
             cl.subscribe([("topic", 0)])
 
         def on_subscribe(cl, userdata, mid, reason_code_list, properties):
             assert isinstance(cl, client.Client)
             assert isinstance(mid, int)
             assert isinstance(reason_code_list, list)
-            assert isinstance(reason_code_list[0], ReasonCodes)
+            assert isinstance(reason_code_list[0], ReasonCode)
             assert isinstance(properties, Properties)
             assert properties.isEmpty()
             userdata.append("on_subscribe")
             cl.publish("topic", "payload", 2)
 
         def on_publish(cl, userdata, mid, reason_code, properties):
             assert isinstance(cl, client.Client)
             assert isinstance(mid, int)
-            assert isinstance(reason_code, ReasonCodes)
+            assert isinstance(reason_code, ReasonCode)
             assert isinstance(properties, Properties)
             assert properties.isEmpty()
             userdata.append("on_publish")
 
         def on_message(cl, userdata, message):
             assert isinstance(cl, client.Client)
             assert isinstance(message, client.MQTTMessage)
@@ -868,15 +932,15 @@
             assert properties.isEmpty()
             userdata.append("on_unsubscribe")
             cl.disconnect()
 
         def on_disconnect(cl, userdata, flags, reason_code, properties):
             assert isinstance(cl, client.Client)
             assert isinstance(flags, client.DisconnectFlags)
-            assert isinstance(reason_code, ReasonCodes)
+            assert isinstance(reason_code, ReasonCode)
             assert isinstance(properties, Properties)
             assert properties.isEmpty()
             userdata.append("on_disconnect")
 
         mqttc.on_connect = on_connect
         mqttc.on_subscribe = on_subscribe
         mqttc.on_publish = on_publish
```

### Comparing `paho_mqtt-2.0.0rc2/tests/test_matcher.py` & `paho_mqtt-2.1.0/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/test_mqttv5.py` & `paho_mqtt-2.1.0/tests/test_mqttv5.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,151 +13,178 @@
 
   Contributors:
      Ian Craggs - initial implementation and/or documentation
 *******************************************************************
 """
 
 import logging
+import queue
 import sys
 import threading
 import time
 import unittest
 import unittest.mock
 
 import paho.mqtt
 import paho.mqtt.client
 from paho.mqtt.enums import CallbackAPIVersion
 from paho.mqtt.packettypes import PacketTypes
 from paho.mqtt.properties import Properties
 from paho.mqtt.subscribeoptions import SubscribeOptions
 
+DEFAULT_TIMEOUT = 5
+# timeout for something that should not happen but we wait to
+# give it time to happen if it does due to a bug.
+WAIT_NON_EVENT_TIMEOUT = 1
 
 class Callbacks:
 
     def __init__(self):
-        self.messages = []
-        self.publisheds = []
-        self.subscribeds = []
-        self.unsubscribeds = []
-        self.disconnecteds = []
-        self.connecteds = []
-        self.conn_failures = []
+        self.messages = queue.Queue()
+        self.publisheds = queue.Queue()
+        self.subscribeds = queue.Queue()
+        self.unsubscribeds  = queue.Queue()
+        self.disconnecteds  = queue.Queue()
+        self.connecteds  = queue.Queue()
+        self.conn_failures  = queue.Queue()
 
     def __str__(self):
-        return str(self.messages) + str(self.messagedicts) + str(self.publisheds) + \
-            str(self.subscribeds) + \
-            str(self.unsubscribeds) + str(self.disconnects)
+        return str(self.messages.queue) + str(self.messagedicts.queue) + str(self.publisheds.queue) + \
+            str(self.subscribeds.queue) + \
+            str(self.unsubscribeds.queue) + str(self.disconnects.queue)
 
     def clear(self):
         self.__init__()
 
     def on_connect(self, client, userdata, flags, reasonCode, properties):
-        self.connecteds.append({"userdata": userdata, "flags": flags,
-                                "reasonCode": reasonCode, "properties": properties})
+        self.connecteds.put({"userdata": userdata, "flags": flags,
+                             "reasonCode": reasonCode, "properties": properties})
 
     def on_connect_fail(self, client, userdata):
-        self.conn_failures.append({"userdata": userdata})
-
-    def wait(self, alist, timeout=2):
-        interval = 0.2
-        total = 0
-        while len(alist) == 0 and total < timeout:
-            time.sleep(interval)
-            total += interval
-        return alist.pop(0)  # if len(alist) > 0 else None
+        self.conn_failures.put({"userdata": userdata})
 
     def wait_connect_fail(self):
-        return self.wait(self.conn_failures, timeout=10)
+        return self.conn_failures.get(timeout=10)
 
     def wait_connected(self):
-        return self.wait(self.connecteds)
+        return self.connecteds.get(timeout=2)
 
     def on_disconnect(self, client, userdata, reasonCode, properties=None):
-        self.disconnecteds.append(
+        self.disconnecteds.put(
             {"reasonCode": reasonCode, "properties": properties})
 
     def wait_disconnected(self):
-        return self.wait(self.disconnecteds)
+        return self.disconnecteds.get(timeout=2)
 
     def on_message(self, client, userdata, message):
-        self.messages.append({"userdata": userdata, "message": message})
+        self.messages.put({"userdata": userdata, "message": message})
 
     def published(self, client, userdata, msgid):
-        self.publisheds.append(msgid)
+        self.publisheds.put(msgid)
 
     def wait_published(self):
-        return self.wait(self.publisheds)
+        return self.publisheds.get(timeout=2)
 
     def on_subscribe(self, client, userdata, mid, reasonCodes, properties):
-        self.subscribeds.append({"mid": mid, "userdata": userdata,
-                                 "properties": properties, "reasonCodes": reasonCodes})
+        self.subscribeds.put({"mid": mid, "userdata": userdata,
+                              "properties": properties, "reasonCodes": reasonCodes})
 
     def wait_subscribed(self):
-        return self.wait(self.subscribeds)
+        return self.subscribeds.get(timeout=2)
 
     def unsubscribed(self, client, userdata, mid, properties, reasonCodes):
-        self.unsubscribeds.append({"mid": mid, "userdata": userdata,
-                                   "properties": properties, "reasonCodes": reasonCodes})
+        self.unsubscribeds.put({"mid": mid, "userdata": userdata,
+                                "properties": properties, "reasonCodes": reasonCodes})
 
     def wait_unsubscribed(self):
-        return self.wait(self.unsubscribeds)
+        return self.unsubscribeds.get(timeout=2)
 
     def on_log(self, client, userdata, level, buf):
         print(buf)
 
     def register(self, client):
         client.on_connect = self.on_connect
         client.on_subscribe = self.on_subscribe
         client.on_publish = self.published
         client.on_unsubscribe = self.unsubscribed
         client.on_message = self.on_message
         client.on_disconnect = self.on_disconnect
         client.on_connect_fail = self.on_connect_fail
         client.on_log = self.on_log
 
+    def get_messages(self, count: int, timeout: float = DEFAULT_TIMEOUT):
+        result = []
+        deadline = time.time() + timeout
+        while len(result) < count:
+            get_timeout = deadline - time.time()
+            if get_timeout <= 0:
+                result.append(self.messages.get_nowait())
+            else:
+                result.append(self.messages.get(timeout=get_timeout))
+
+        return result
+
+    def get_at_most_messages(self, count: int, timeout: float = DEFAULT_TIMEOUT):
+        result = []
+        deadline = time.time() + timeout
+        try:
+            while len(result) < count:
+                get_timeout = deadline - time.time()
+                if get_timeout <= 0:
+                    result.append(self.messages.get_nowait())
+                else:
+                    result.append(self.messages.get(timeout=get_timeout))
+        except queue.Empty:
+            pass
+
+        return result
+
 
 def cleanRetained(port):
     callback = Callbacks()
     curclient = paho.mqtt.client.Client(
         CallbackAPIVersion.VERSION1,
         b"clean retained",
         protocol=paho.mqtt.client.MQTTv5,
     )
-    curclient.loop_start()
     callback.register(curclient)
     curclient.connect(host="localhost", port=port)
+    curclient.loop_start()
     callback.wait_connected()
     curclient.subscribe("#", options=SubscribeOptions(qos=0))
     callback.wait_subscribed()  # wait for retained messages to arrive
-    time.sleep(1)
-    for message in callback.messages:
-        logging.info("deleting retained message for topic", message["message"])
-        curclient.publish(message["message"].topic, b"", 0, retain=True)
+    try:
+        while True:
+            message = callback.messages.get(timeout=WAIT_NON_EVENT_TIMEOUT)
+            if message["message"].payload != b"":
+                logging.info("deleting retained message for topic", message["message"])
+                curclient.publish(message["message"].topic, b"", 0, retain=True)
+    except queue.Empty:
+        pass
     curclient.disconnect()
     curclient.loop_stop()
-    time.sleep(.1)
 
 
 def cleanup(port):
     # clean all client state
     print("clean up starting")
     clientids = ("aclient", "bclient")
 
+    def _on_connect(client, *args):
+        client.disconnect()
+
     for clientid in clientids:
         curclient = paho.mqtt.client.Client(
             CallbackAPIVersion.VERSION1,
             clientid.encode("utf-8"),
             protocol=paho.mqtt.client.MQTTv5,
         )
-        curclient.loop_start()
+        curclient.on_connect = _on_connect
         curclient.connect(host="localhost", port=port, clean_start=True)
-        time.sleep(.1)
-        curclient.disconnect()
-        time.sleep(.1)
-        curclient.loop_stop()
+        curclient.loop_forever()
 
     # clean retained messages
     cleanRetained(port)
     print("clean up finished")
 
 
 class Test(unittest.TestCase):
@@ -181,17 +208,23 @@
                 kwargs={
                     "config": ["listener 0"],
                 },
             )
             cls._test_broker.daemon = True
             cls._test_broker.start()
             # Wait a bit for TCP server to bind to an address
-            time.sleep(0.5)
-            # Hack to find the port used by the test broker...
-            cls._test_broker_port = mqtt.brokers.listeners.TCPListeners.server.socket.getsockname()[1]
+            for _ in range(20):
+                time.sleep(0.1)
+                if mqtt.brokers.listeners.TCPListeners.server is not None:
+                    port = mqtt.brokers.listeners.TCPListeners.server.socket.getsockname()[1]
+                    if port != 0:
+                        cls._test_broker_port = port
+                        break
+            else:
+                raise ValueError("can't find the test broker port")
         setData()
         cleanup(cls._test_broker_port)
 
         callback = Callbacks()
         callback2 = Callbacks()
 
         #aclient = mqtt_client.Client(b"\xEF\xBB\xBF" + "myclientid".encode("utf-8"))
@@ -205,39 +238,41 @@
     @classmethod
     def tearDownClass(cls):
         # Another hack to stop the test broker... we rely on fact that it use a sockserver.TCPServer
         import mqtt.brokers
         mqtt.brokers.listeners.TCPListeners.server.shutdown()
         cls._test_broker.join(5)
 
-    def waitfor(self, queue, depth, limit):
-        total = 0
-        while len(queue) < depth and total < limit:
-            interval = .5
-            total += interval
-            time.sleep(interval)
-
     def test_basic(self):
+        import datetime
+        print(datetime.datetime.now(), "start")
         aclient.connect(host="localhost", port=self._test_broker_port)
         aclient.loop_start()
+        print(datetime.datetime.now(), "loop_start")
         response = callback.wait_connected()
+        print(datetime.datetime.now(), "connected")
         self.assertEqual(response["reasonCode"].getName(), "Success")
 
         aclient.subscribe(topics[0], options=SubscribeOptions(qos=2))
         response = callback.wait_subscribed()
+        print(datetime.datetime.now(), "wait_subscribed")
         self.assertEqual(response["reasonCodes"][0].getName(), "Granted QoS 2")
 
         aclient.publish(topics[0], b"qos 0")
         aclient.publish(topics[0], b"qos 1", 1)
         aclient.publish(topics[0], b"qos 2", 2)
-        i = 0
-        while len(callback.messages) < 3 and i < 10:
-            time.sleep(.2)
-            i += 1
-        self.assertEqual(len(callback.messages), 3)
+
+        msgs = callback.get_messages(3)
+        print(datetime.datetime.now(), "publish get")
+        got_payload = {
+            x["message"].payload
+            for x in msgs
+        }
+
+        self.assertEqual(got_payload, {b"qos 0", b"qos 1", b"qos 2"})
         aclient.disconnect()
 
         callback.clear()
         aclient.loop_stop()
 
     def test_connect_fail(self):
         clientid = "connection failure"
@@ -264,43 +299,44 @@
         aclient.publish(topics[1], b"qos 0", 0,
                         retain=True, properties=publish_properties)
         aclient.publish(topics[2], b"qos 1", 1,
                         retain=True, properties=publish_properties)
         aclient.publish(topics[3], b"qos 2", 2,
                         retain=True, properties=publish_properties)
         # wait until those messages are published
-        time.sleep(1)
+        time.sleep(WAIT_NON_EVENT_TIMEOUT)
         aclient.subscribe(wildtopics[5], options=SubscribeOptions(qos=2))
         response = callback.wait_subscribed()
         self.assertEqual(response["reasonCodes"][0].getName(), "Granted QoS 2")
+        msgs = callback.get_messages(3)
 
-        time.sleep(1)
         aclient.disconnect()
         aclient.loop_stop()
 
-        self.assertEqual(len(callback.messages), 3)
-        userprops = callback.messages[0]["message"].properties.UserProperty
+        self.assertTrue(callback.messages.empty())
+
+        userprops = msgs[0]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        userprops = callback.messages[1]["message"].properties.UserProperty
+        userprops = msgs[1]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        userprops = callback.messages[2]["message"].properties.UserProperty
+        userprops = msgs[2]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        qoss = [callback.messages[i]["message"].qos for i in range(3)]
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
 
         cleanRetained(self._test_broker_port)
 
     def test_will_message(self):
         # will messages and keep alive
         callback.clear()
         callback2.clear()
-        self.assertEqual(len(callback2.messages), 0, callback2.messages)
+        self.assertTrue(callback2.messages.empty(), callback2.messages.queue)
 
         will_properties = Properties(PacketTypes.WILLMESSAGE)
         will_properties.WillDelayInterval = 0  # this is the default anyway
         will_properties.UserProperty = ("a", "2")
         will_properties.UserProperty = ("c", "3")
 
         aclient.will_set(topics[2], payload=b"will message",
@@ -314,20 +350,19 @@
         response = callback2.wait_connected()
         bclient.subscribe(topics[2], qos=2)
         response = callback2.wait_subscribed()
         self.assertEqual(response["reasonCodes"][0].getName(), "Granted QoS 2")
 
         # keep alive timeout ought to be triggered so the will message is received
         aclient.loop_stop()  # so that pings aren't sent
-        self.waitfor(callback2.messages, 1, 10)
+        msg = callback2.messages.get(timeout=10)
         bclient.disconnect()
         bclient.loop_stop()
-        # should have the will message
-        self.assertEqual(len(callback2.messages), 1, callback2.messages)
-        props = callback2.messages[0]["message"].properties
+
+        props = msg["message"].properties
         self.assertEqual(props.UserProperty, [("a", "2"), ("c", "3")])
 
     def test_zero_length_clientid(self):
         logging.info("Zero length clientid test starting")
 
         callback0 = Callbacks()
 
@@ -387,36 +422,42 @@
         ocallback.wait_subscribed()
         oclient.disconnect()
         oclient.loop_stop()
 
         bclient.loop_start()
         bclient.connect(host="localhost", port=self._test_broker_port)
         callback2.wait_connected()
-        bclient.publish(topics[1], b"qos 0", 0)
-        bclient.publish(topics[2], b"qos 1", 1)
-        bclient.publish(topics[3], b"qos 2", 2)
-        time.sleep(2)
+        msg1 = bclient.publish(topics[1], b"qos 0", 0)
+        msg2 = bclient.publish(topics[2], b"qos 1", 1)
+        msg3 = bclient.publish(topics[3], b"qos 2", 2)
+
+        msg1.wait_for_publish()
+        msg2.wait_for_publish()
+        msg3.wait_for_publish()
+
         bclient.disconnect()
         bclient.loop_stop()
 
         oclient = paho.mqtt.client.Client(
             CallbackAPIVersion.VERSION1, clientid, protocol=paho.mqtt.client.MQTTv5,
         )
         ocallback.register(oclient)
         oclient.loop_start()
         oclient.connect(host="localhost", port=self._test_broker_port, clean_start=False)
         ocallback.wait_connected()
-        time.sleep(2)
+
+        msgs = ocallback.get_at_most_messages(3)
+
         oclient.disconnect()
         oclient.loop_stop()
 
-        self.assertTrue(len(ocallback.messages) in [
-                        2, 3], len(ocallback.messages))
+        self.assertTrue(len(msgs) in [
+                        2, 3], ocallback.messages.qsize())
         logging.info("This server %s queueing QoS 0 messages for offline clients" %
-                     ("is" if len(ocallback.messages) == 3 else "is not"))
+                     ("is" if len(msgs) == 3 else "is not"))
 
     def test_overlapping_subscriptions(self):
         # overlapping subscriptions. When there is more than one matching subscription for the same client for a topic,
         # the server may send back one message with the highest QoS of any matching subscription, or one message for
         # each subscription with a matching QoS.
         ocallback = Callbacks()
         clientid = b"overlapping subscriptions"
@@ -430,26 +471,26 @@
         oclient.connect(host="localhost", port=self._test_broker_port)
         ocallback.wait_connected()
         oclient.subscribe([(wildtopics[6], SubscribeOptions(qos=2)),
                            (wildtopics[0], SubscribeOptions(qos=1))])
         ocallback.wait_subscribed()
         oclient.publish(topics[3], b"overlapping topic filters", 2)
         ocallback.wait_published()
-        time.sleep(1)
-        self.assertTrue(len(ocallback.messages) in [1, 2], ocallback.messages)
-        if len(ocallback.messages) == 1:
+
+        msgs = ocallback.get_at_most_messages(2)
+        if len(msgs) == 1:
             logging.info(
                 "This server is publishing one message for all matching overlapping subscriptions, not one for each.")
             self.assertEqual(
-                ocallback.messages[0]["message"].qos, 2, ocallback.messages[0]["message"].qos)
+                msgs[0]["message"].qos, 2, msgs[0]["message"].qos)
         else:
             logging.info(
                 "This server is publishing one message per each matching overlapping subscription.")
-            self.assertTrue((ocallback.messages[0]["message"].qos == 2 and ocallback.messages[1]["message"].qos == 1) or
-                            (ocallback.messages[0]["message"].qos == 1 and ocallback.messages[1]["message"].qos == 2), callback.messages)
+            self.assertTrue((msgs[0]["message"].qos == 2 and msgs[1]["message"].qos == 1) or
+                            (msgs[0]["message"].qos == 1 and msgs[1]["message"].qos == 2), msgs)
         oclient.disconnect()
         oclient.loop_stop()
         ocallback.clear()
 
     def test_subscribe_failure(self):
         # Subscribe failure.  A new feature of MQTT 3.1.1 is the ability to send back negative responses to subscribe
         # requests.  One way of doing this is to subscribe to a topic which is not allowed to be subscribed to.
@@ -491,21 +532,22 @@
 
         aclient.connect(host="localhost", port=self._test_broker_port)
         aclient.loop_start()
         callback.wait_connected()
         aclient.publish(topics[0], b"topic 0 - unsubscribed", 1, retain=False)
         aclient.publish(topics[1], b"topic 1", 1, retain=False)
         aclient.publish(topics[2], b"topic 2", 1, retain=False)
-        time.sleep(2)
+
+        msgs = callback2.get_messages(2)
 
         bclient.disconnect()
         bclient.loop_stop()
         aclient.disconnect()
         aclient.loop_stop()
-        self.assertEqual(len(callback2.messages), 2, callback2.messages)
+        self.assertEqual(len(msgs), 2)
 
     def new_client(self, clientid):
         callback = Callbacks()
         client = paho.mqtt.client.Client(
             CallbackAPIVersion.VERSION1,
             clientid.encode("utf-8"),
             protocol=paho.mqtt.client.MQTTv5,
@@ -640,32 +682,31 @@
         publish_properties.UserProperty = ("c", "3")
         uclient.publish(topics[0], b"", 0, retain=False,
                         properties=publish_properties)
         uclient.publish(topics[0], b"", 1, retain=False,
                         properties=publish_properties)
         uclient.publish(topics[0], b"", 2, retain=False,
                         properties=publish_properties)
-        count = 0
-        while len(ucallback.messages) < 3 and count < 50:
-            time.sleep(.1)
-            count += 1
+
+        msgs = ucallback.get_messages(3)
+
         uclient.disconnect()
         ucallback.wait_disconnected()
         uclient.loop_stop()
-        self.assertEqual(len(ucallback.messages), 3, ucallback.messages)
-        userprops = ucallback.messages[0]["message"].properties.UserProperty
+        self.assertTrue(ucallback.messages.empty(), ucallback.messages.queue)
+        userprops = msgs[0]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        userprops = ucallback.messages[1]["message"].properties.UserProperty
+        userprops = msgs[1]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        userprops = ucallback.messages[2]["message"].properties.UserProperty
+        userprops = msgs[2]["message"].properties.UserProperty
         self.assertTrue(userprops in [[("a", "2"), ("c", "3")], [
                         ("c", "3"), ("a", "2")]], userprops)
-        qoss = [ucallback.messages[i]["message"].qos for i in range(3)]
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
 
     def test_payload_format(self):
         clientid = "payload format"
         pclient, pcallback = self.new_client(clientid)
         pclient.loop_start()
         pclient.connect_async(host="localhost", port=self._test_broker_port)
@@ -682,36 +723,34 @@
         info = pclient.publish(
             topics[0], b"qos 1", 1, retain=False, properties=publish_properties)
         info.wait_for_publish()
         info = pclient.publish(
             topics[0], b"qos 2", 2, retain=False, properties=publish_properties)
         info.wait_for_publish()
 
-        count = 0
-        while len(pcallback.messages) < 3 and count < 50:
-            time.sleep(.1)
-            count += 1
+        msgs = pcallback.get_messages(3)
+
         pclient.disconnect()
         pcallback.wait_disconnected()
         pclient.loop_stop()
 
-        self.assertEqual(len(pcallback.messages), 3, pcallback.messages)
-        props = pcallback.messages[0]["message"].properties
+        self.assertTrue(pcallback.messages.empty(), pcallback.messages.queue)
+        props = msgs[0]["message"].properties
         self.assertEqual(props.ContentType, "My name", props.ContentType)
         self.assertEqual(props.PayloadFormatIndicator,
                          1, props.PayloadFormatIndicator)
-        props = pcallback.messages[1]["message"].properties
+        props = msgs[1]["message"].properties
         self.assertEqual(props.ContentType, "My name", props.ContentType)
         self.assertEqual(props.PayloadFormatIndicator,
                          1, props.PayloadFormatIndicator)
-        props = pcallback.messages[2]["message"].properties
+        props = msgs[2]["message"].properties
         self.assertEqual(props.ContentType, "My name", props.ContentType)
         self.assertEqual(props.PayloadFormatIndicator,
                          1, props.PayloadFormatIndicator)
-        qoss = [pcallback.messages[i]["message"].qos for i in range(3)]
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
 
     def test_message_expiry(self):
         clientid = "message expiry"
 
         connect_properties = Properties(PacketTypes.CONNECT)
         connect_properties.SessionExpiryInterval = 99999
@@ -746,21 +785,22 @@
                          2, retain=False, properties=publish_properties)
 
         time.sleep(3)
         lbclient, lbcallback = self.new_client(f"{clientid} b")
         lbclient.loop_start()
         lbclient.connect(host="localhost", port=self._test_broker_port, clean_start=False)
         lbcallback.wait_connected()
-        self.waitfor(lbcallback.messages, 1, 3)
-        time.sleep(1)
-        self.assertEqual(len(lbcallback.messages), 2, lbcallback.messages)
-        self.assertTrue(lbcallback.messages[0]["message"].properties.MessageExpiryInterval < 6,
-                        lbcallback.messages[0]["message"].properties.MessageExpiryInterval)
-        self.assertTrue(lbcallback.messages[1]["message"].properties.MessageExpiryInterval < 6,
-                        lbcallback.messages[1]["message"].properties.MessageExpiryInterval)
+
+        msgs = lbcallback.get_messages(2)
+
+        self.assertTrue(lbcallback.messages.empty(), lbcallback.messages.queue)
+        self.assertTrue(msgs[0]["message"].properties.MessageExpiryInterval < 6,
+                        msgs[0]["message"].properties.MessageExpiryInterval)
+        self.assertTrue(msgs[1]["message"].properties.MessageExpiryInterval < 6,
+                        msgs[1]["message"].properties.MessageExpiryInterval)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         lbclient.disconnect()
         lbcallback.wait_disconnected()
         lbclient.loop_stop()
@@ -782,19 +822,24 @@
         lbcallback.wait_connected()
         lbclient.loop_start()
         lbclient.subscribe(
             topics[0], options=SubscribeOptions(qos=2, noLocal=True))
         lbcallback.wait_subscribed()
 
         laclient.publish(topics[0], b"noLocal test", 1, retain=False)
-        self.waitfor(lbcallback.messages, 1, 3)
-        time.sleep(1)
 
-        self.assertEqual(lacallback.messages, [], lacallback.messages)
-        self.assertEqual(len(lbcallback.messages), 1, lbcallback.messages)
+        lbcallback.messages.get(timeout=DEFAULT_TIMEOUT)
+        try:
+            lacallback.messages.get(timeout=WAIT_NON_EVENT_TIMEOUT)
+            raise ValueError("unexpected message received")
+        except queue.Empty:
+            pass
+
+        self.assertTrue(lacallback.messages.empty(), lacallback.messages.queue)
+        self.assertTrue(lbcallback.messages.empty(), lbcallback.messages.queue)
         laclient.disconnect()
         lacallback.wait_disconnected()
         lbclient.disconnect()
         lbcallback.wait_disconnected()
         laclient.loop_stop()
         lbclient.loop_stop()
 
@@ -802,29 +847,27 @@
         clientid = 'subscribe options - retain as published'
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port)
         lacallback.wait_connected()
         laclient.subscribe(topics[0], options=SubscribeOptions(
             qos=2, retainAsPublished=True))
         lacallback.wait_subscribed()
-        self.waitfor(lacallback.subscribeds, 1, 3)
         laclient.publish(
             topics[0], b"retain as published false", 1, retain=False)
         laclient.publish(
             topics[0], b"retain as published true", 1, retain=True)
 
-        self.waitfor(lacallback.messages, 2, 3)
-        time.sleep(1)
+        msgs = lacallback.get_messages(2)
 
-        self.assertEqual(len(lacallback.messages), 2, lacallback.messages)
+        self.assertTrue(lacallback.messages.empty(), lacallback.messages.queue)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
-        self.assertEqual(lacallback.messages[0]["message"].retain, False)
-        self.assertEqual(lacallback.messages[1]["message"].retain, True)
+        self.assertEqual(msgs[0]["message"].retain, False)
+        self.assertEqual(msgs[1]["message"].retain, True)
 
         # retainHandling
         clientid = 'subscribe options - retain handling'
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port)
         lacallback.wait_connected()
         laclient.publish(topics[1], b"qos 0", 0, retain=True)
@@ -832,78 +875,80 @@
         laclient.publish(topics[3], b"qos 2", 2, retain=True)
         time.sleep(1)
 
         # retain handling 1 only gives us retained messages on a new subscription
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=1))
         lacallback.wait_subscribed()
-        self.assertEqual(len(lacallback.messages), 3)
-        qoss = [lacallback.messages[i]["message"].qos for i in range(3)]
+
+        msgs = lacallback.get_messages(3)
+
+        self.assertTrue(lacallback.messages.empty())
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
         lacallback.clear()
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=1))
         lacallback.wait_subscribed()
         time.sleep(1)
-        self.assertEqual(len(lacallback.messages), 0)
+        self.assertTrue(lacallback.messages.empty())
 
         # remove that subscription
         properties = Properties(PacketTypes.UNSUBSCRIBE)
         properties.UserProperty = ("a", "2")
         properties.UserProperty = ("c", "3")
         laclient.unsubscribe(wildtopics[5], properties)
         lacallback.wait_unsubscribed()
 
         # check that we really did remove that subscription
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=1))
         lacallback.wait_subscribed()
-        self.assertEqual(len(lacallback.messages), 3)
-        qoss = [lacallback.messages[i]["message"].qos for i in range(3)]
+        msgs = lacallback.get_messages(3)
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
         lacallback.clear()
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=1))
         lacallback.wait_subscribed()
-        time.sleep(1)
-        self.assertEqual(len(lacallback.messages), 0)
+        time.sleep(WAIT_NON_EVENT_TIMEOUT)
+        self.assertTrue(lacallback.messages.empty())
 
         # remove that subscription
         properties = Properties(PacketTypes.UNSUBSCRIBE)
         properties.UserProperty = ("a", "2")
         properties.UserProperty = ("c", "3")
         laclient.unsubscribe(wildtopics[5], properties)
         lacallback.wait_unsubscribed()
 
         lacallback.clear()
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=2))
         lacallback.wait_subscribed()
-        self.assertEqual(len(lacallback.messages), 0)
+        self.assertTrue(lacallback.messages.empty())
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=2))
         lacallback.wait_subscribed()
-        self.assertEqual(len(lacallback.messages), 0)
+        self.assertTrue(lacallback.messages.empty())
 
         # remove that subscription
         laclient.unsubscribe(wildtopics[5])
         lacallback.wait_unsubscribed()
 
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=0))
         lacallback.wait_subscribed()
-        self.assertEqual(len(lacallback.messages), 3)
-        qoss = [lacallback.messages[i]["message"].qos for i in range(3)]
+        msgs = lacallback.get_messages(3)
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
         lacallback.clear()
         laclient.subscribe(
             wildtopics[5], options=SubscribeOptions(2, retainHandling=0))
-        time.sleep(1)
-        self.assertEqual(len(lacallback.messages), 3)
-        qoss = [lacallback.messages[i]["message"].qos for i in range(3)]
+        msgs = lacallback.get_messages(3)
+        qoss = [x["message"].qos for x in msgs]
         self.assertTrue(1 in qoss and 2 in qoss and 0 in qoss, qoss)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         cleanRetained(self._test_broker_port)
 
@@ -931,27 +976,27 @@
 
         sub_properties.clear()
         sub_properties.SubscriptionIdentifier = 3
         lbclient.subscribe(f"{topics[0]}/#", qos=2, properties=sub_properties)
 
         lbclient.publish(topics[0], b"sub identifier test", 1, retain=False)
 
-        self.waitfor(lacallback.messages, 1, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
-        self.assertEqual(lacallback.messages[0]["message"].properties.SubscriptionIdentifier[0],
-                         456789, lacallback.messages[0]["message"].properties.SubscriptionIdentifier)
+        msg = lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
+        self.assertTrue(lacallback.messages.empty(), lacallback.messages.queue)
+        self.assertEqual(msg["message"].properties.SubscriptionIdentifier[0],
+                         456789, msg["message"].properties.SubscriptionIdentifier)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
-        self.waitfor(lbcallback.messages, 1, 3)
-        self.assertEqual(len(lbcallback.messages), 1, lbcallback.messages)
+        msg = lbcallback.messages.get(timeout=DEFAULT_TIMEOUT)
+        self.assertTrue(lbcallback.messages.empty(), lbcallback.messages.queue)
         expected_subsids = {2, 3}
         received_subsids = set(
-            lbcallback.messages[0]["message"].properties.SubscriptionIdentifier)
+            msg["message"].properties.SubscriptionIdentifier)
         self.assertEqual(received_subsids, expected_subsids, received_subsids)
         lbclient.disconnect()
         lbcallback.wait_disconnected()
         lbclient.loop_stop()
 
     def test_request_response(self):
         clientid = 'request response'
@@ -978,27 +1023,25 @@
         publish_properties.ResponseTopic = topics[0]
         publish_properties.CorrelationData = b"334"
         # client a is the requester
         laclient.publish(topics[0], b"request", 1,
                          properties=publish_properties)
 
         # client b is the responder
-        self.waitfor(lbcallback.messages, 1, 3)
-        self.assertEqual(len(lbcallback.messages), 1, lbcallback.messages)
-        self.assertEqual(lbcallback.messages[0]["message"].properties.ResponseTopic, topics[0],
-                         lbcallback.messages[0]["message"].properties)
-        self.assertEqual(lbcallback.messages[0]["message"].properties.CorrelationData, b"334",
-                         lbcallback.messages[0]["message"].properties)
+        msg = lbcallback.messages.get(timeout=DEFAULT_TIMEOUT)
+        self.assertEqual(msg["message"].properties.ResponseTopic, topics[0],
+                         msg["message"].properties)
+        self.assertEqual(msg["message"].properties.CorrelationData, b"334",
+                         msg["message"].properties)
 
-        lbclient.publish(lbcallback.messages[0]["message"].properties.ResponseTopic, b"response", 1,
-                         properties=lbcallback.messages[0]["message"].properties)
+        lbclient.publish(msg["message"].properties.ResponseTopic, b"response", 1,
+                         properties=msg["message"].properties)
 
         # client a gets the response
-        self.waitfor(lacallback.messages, 1, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
+        lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
 
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
         lbclient.disconnect()
         lbcallback.wait_disconnected()
         lbclient.loop_stop()
@@ -1025,34 +1068,31 @@
         laclient.subscribe(topics[0], qos=2)
         lacallback.wait_subscribed()
 
         publish_properties = Properties(PacketTypes.PUBLISH)
         publish_properties.TopicAlias = 1
         laclient.publish(topics[0], b"topic alias 1",
                          1, properties=publish_properties)
-        self.waitfor(lacallback.messages, 1, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
+        lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
 
         laclient.publish("", b"topic alias 2", 1,
                          properties=publish_properties)
-        self.waitfor(lacallback.messages, 2, 3)
-        self.assertEqual(len(lacallback.messages), 2, lacallback.messages)
+        lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
 
         laclient.disconnect()  # should get rid of the topic aliases but not subscriptions
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         # check aliases have been deleted
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port, clean_start=False,
                          properties=connect_properties)
 
         laclient.publish(topics[0], b"topic alias 3", 1)
-        self.waitfor(lacallback.messages, 1, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
+        lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
 
         publish_properties = Properties(PacketTypes.PUBLISH)
         publish_properties.TopicAlias = 1
         laclient.publish("", b"topic alias 4", 1,
                          properties=publish_properties)
 
         # should get back a disconnect with Topic alias invalid
@@ -1072,35 +1112,34 @@
         laclient.loop_start()
 
         laclient.subscribe(topics[0], qos=2)
         lacallback.wait_subscribed()
 
         for qos in range(3):
             laclient.publish(topics[0], b"topic alias 1", qos)
-        self.waitfor(lacallback.messages, 3, 3)
-        self.assertEqual(len(lacallback.messages), 3, lacallback.messages)
+        msgs = lacallback.get_messages(3)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         # first message should set the topic alias
         self.assertTrue(hasattr(
-            lacallback.messages[0]["message"].properties, "TopicAlias"), lacallback.messages[0]["message"].properties)
-        topicalias = lacallback.messages[0]["message"].properties.TopicAlias
+            msgs[0]["message"].properties, "TopicAlias"), msgs[0]["message"].properties)
+        topicalias = msgs[0]["message"].properties.TopicAlias
 
         self.assertTrue(topicalias > 0)
-        self.assertEqual(lacallback.messages[0]["message"].topic, topics[0])
+        self.assertEqual(msgs[0]["message"].topic, topics[0])
 
         self.assertEqual(
-            lacallback.messages[1]["message"].properties.TopicAlias, topicalias)
-        self.assertEqual(lacallback.messages[1]["message"].topic, "")
+            msgs[1]["message"].properties.TopicAlias, topicalias)
+        self.assertEqual(msgs[1]["message"].topic, "")
 
         self.assertEqual(
-            lacallback.messages[2]["message"].properties.TopicAlias, topicalias)
-        self.assertEqual(lacallback.messages[2]["message"].topic, "")
+            msgs[2]["message"].properties.TopicAlias, topicalias)
+        self.assertEqual(msgs[2]["message"].topic, "")
 
         serverTopicAliasMaximum = 0  # no server topic alias allowed
         connect_properties = Properties(PacketTypes.CONNECT)
         # connect_properties.TopicAliasMaximum = serverTopicAliasMaximum # default is 0
 
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port, properties=connect_properties)
@@ -1108,27 +1147,26 @@
         laclient.loop_start()
 
         laclient.subscribe(topics[0], qos=2)
         lacallback.wait_subscribed()
 
         for qos in range(3):
             laclient.publish(topics[0], b"topic alias 2", qos)
-        self.waitfor(lacallback.messages, 3, 3)
-        self.assertEqual(len(lacallback.messages), 3, lacallback.messages)
+        msgs = lacallback.get_messages(3)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         # No topic aliases
         self.assertFalse(hasattr(
-            lacallback.messages[0]["message"].properties, "TopicAlias"), lacallback.messages[0]["message"].properties)
+            msgs[0]["message"].properties, "TopicAlias"), msgs[0]["message"].properties)
         self.assertFalse(hasattr(
-            lacallback.messages[1]["message"].properties, "TopicAlias"), lacallback.messages[1]["message"].properties)
+            msgs[1]["message"].properties, "TopicAlias"), msgs[1]["message"].properties)
         self.assertFalse(hasattr(
-            lacallback.messages[2]["message"].properties, "TopicAlias"), lacallback.messages[2]["message"].properties)
+            msgs[2]["message"].properties, "TopicAlias"), msgs[2]["message"].properties)
 
         serverTopicAliasMaximum = 0  # no server topic alias allowed
         connect_properties = Properties(PacketTypes.CONNECT)
         connect_properties.TopicAliasMaximum = serverTopicAliasMaximum  # default is 0
 
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port, properties=connect_properties)
@@ -1136,27 +1174,26 @@
         laclient.loop_start()
 
         laclient.subscribe(topics[0], qos=2)
         lacallback.wait_subscribed()
 
         for qos in range(3):
             laclient.publish(topics[0], b"topic alias 3", qos)
-        self.waitfor(lacallback.messages, 3, 3)
-        self.assertEqual(len(lacallback.messages), 3, lacallback.messages)
+        msgs = lacallback.get_messages(3)
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         # No topic aliases
         self.assertFalse(hasattr(
-            lacallback.messages[0]["message"].properties, "TopicAlias"), lacallback.messages[0]["message"].properties)
+            msgs[0]["message"].properties, "TopicAlias"), msgs[0]["message"].properties)
         self.assertFalse(hasattr(
-            lacallback.messages[1]["message"].properties, "TopicAlias"), lacallback.messages[1]["message"].properties)
+            msgs[1]["message"].properties, "TopicAlias"), msgs[1]["message"].properties)
         self.assertFalse(hasattr(
-            lacallback.messages[2]["message"].properties, "TopicAlias"), lacallback.messages[2]["message"].properties)
+            msgs[2]["message"].properties, "TopicAlias"), msgs[2]["message"].properties)
 
     def test_maximum_packet_size(self):
         clientid = 'maximum packet size'
 
         # 1. server max packet size
         laclient, lacallback = self.new_client(f"{clientid} a")
         laclient.connect(host="localhost", port=self._test_broker_port)
@@ -1169,16 +1206,14 @@
 
         if serverMaximumPacketSize < 65535:
             # publish bigger packet than server can accept
             payload = b"."*serverMaximumPacketSize
             laclient.publish(topics[0], payload, 0)
             # should get back a disconnect with packet size too big
             response = lacallback.wait_disconnected()
-            self.assertEqual(len(lacallback.disconnecteds),
-                             0, lacallback.disconnecteds)
             self.assertEqual(response["reasonCode"].getName(),
                              "Packet too large", response["reasonCode"].getName())
         else:
             laclient.disconnect()
             lacallback.wait_disconnected()
         laclient.loop_stop()
 
@@ -1198,22 +1233,24 @@
 
         laclient.subscribe(topics[0], qos=2)
         response = lacallback.wait_subscribed()
 
         # send a small enough packet, should get this one back
         payload = b"."*(int(maximumPacketSize/2))
         laclient.publish(topics[0], payload, 0)
-        self.waitfor(lacallback.messages, 1, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
+        lacallback.messages.get(timeout=DEFAULT_TIMEOUT)
 
         # send a packet too big to receive
         payload = b"."*maximumPacketSize
         laclient.publish(topics[0], payload, 1)
-        self.waitfor(lacallback.messages, 2, 3)
-        self.assertEqual(len(lacallback.messages), 1, lacallback.messages)
+        try:
+            lacallback.messages.get(timeout=WAIT_NON_EVENT_TIMEOUT)
+            raise ValueError("unexpected message received")
+        except queue.Empty:
+            pass
 
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
     """
     def test_server_keep_alive(self):
@@ -1262,21 +1299,20 @@
         lbclient.subscribe(topics[0], qos=2)
         lbcallback.wait_subscribed()
 
         # abort client a and wait for the will message
         laclient.loop_stop()
         laclient.socket().close()
         start = time.time()
-        while lbcallback.messages == []:
-            time.sleep(.1)
+        msg = lbcallback.messages.get(DEFAULT_TIMEOUT)
         duration = time.time() - start
         self.assertAlmostEqual(duration, 4, delta=1)
-        self.assertEqual(lbcallback.messages[0]["message"].topic, topics[0])
+        self.assertEqual(msg["message"].topic, topics[0])
         self.assertEqual(
-            lbcallback.messages[0]["message"].payload, b"test_will_delay will message")
+            msg["message"].payload, b"test_will_delay will message")
 
         lbclient.disconnect()
         lbcallback.wait_disconnected()
         lbclient.loop_stop()
 
     def test_shared_subscriptions(self):
         clientid = 'shared subscriptions'
@@ -1310,35 +1346,56 @@
 
         lacallback.clear()
         lbcallback.clear()
 
         count = 1
         for i in range(count):
             lbclient.publish(topics[0], f"message {i}", 0)
-        j = 0
-        while len(lacallback.messages) + len(lbcallback.messages) < 2*count and j < 20:
-            time.sleep(.1)
-            j += 1
-        time.sleep(1)
-        self.assertEqual(len(lacallback.messages), count)
-        self.assertEqual(len(lbcallback.messages), count)
+
+        lacallback.get_messages(count)
+        lbcallback.get_messages(count)
+
+        self.assertTrue(lacallback.messages.empty())
+        self.assertTrue(lbcallback.messages.empty())
 
         lacallback.clear()
         lbcallback.clear()
 
         for i in range(count):
             lbclient.publish(shared_pub_topic, f"message {i}", 0)
-        j = 0
-        while len(lacallback.messages) + len(lbcallback.messages) < count and j < 20:
-            time.sleep(.1)
-            j += 1
-        time.sleep(1)
         # Each message should only be received once
-        self.assertEqual(len(lacallback.messages) +
-                         len(lbcallback.messages), count)
+        result = []
+        deadline = time.time() + DEFAULT_TIMEOUT
+        while len(result) < count and time.time() < deadline:
+            get_timeout = deadline - time.time()
+            try:
+                if get_timeout <= 0:
+                    result.append(lacallback.messages.get_nowait())
+                else:
+                    result.append(lacallback.messages.get(timeout=get_timeout))
+            except queue.Empty:
+                # The message could be sent to other client, so empty queue
+                # could be normal
+                pass
+
+            try:
+                get_timeout = deadline - time.time()
+                if get_timeout <= 0:
+                    result.append(lbcallback.messages.get_nowait())
+                else:
+                    result.append(lbcallback.messages.get(timeout=get_timeout))
+            except queue.Empty:
+                # The message could be sent to other client, so empty queue
+                # could be normal
+                pass
+
+        self.assertEqual(
+            {x["message"].payload for x in result},
+            {f"message {i}".encode() for i in range(count)}
+        )
 
         laclient.disconnect()
         lacallback.wait_disconnected()
         laclient.loop_stop()
 
         lbclient.disconnect()
         lbcallback.wait_disconnected()
```

### Comparing `paho_mqtt-2.0.0rc2/tests/test_reasoncodes.py` & `paho_mqtt-2.1.0/tests/test_reasoncodes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,47 @@
+import pytest
 from paho.mqtt.packettypes import PacketTypes
-from paho.mqtt.reasoncodes import ReasonCodes
+from paho.mqtt.reasoncodes import ReasonCode, ReasonCodes
 
 
 class TestReasonCode:
     def test_equality(self):
-        rc_success = ReasonCodes(PacketTypes.CONNACK, "Success")
+        rc_success = ReasonCode(PacketTypes.CONNACK, "Success")
         assert rc_success == 0
         assert rc_success == "Success"
         assert rc_success != "Protocol error"
-        assert rc_success == ReasonCodes(PacketTypes.CONNACK, "Success")
+        assert rc_success == ReasonCode(PacketTypes.CONNACK, "Success")
 
-        rc_protocol_error = ReasonCodes(PacketTypes.CONNACK, "Protocol error")
+        rc_protocol_error = ReasonCode(PacketTypes.CONNACK, "Protocol error")
         assert rc_protocol_error == 130
         assert rc_protocol_error == "Protocol error"
         assert rc_protocol_error != "Success"
-        assert rc_protocol_error == ReasonCodes(PacketTypes.CONNACK, "Protocol error")
+        assert rc_protocol_error == ReasonCode(PacketTypes.CONNACK, "Protocol error")
 
     def test_comparison(self):
-        rc_success = ReasonCodes(PacketTypes.CONNACK, "Success")
-        rc_protocol_error = ReasonCodes(PacketTypes.CONNACK, "Protocol error")
+        rc_success = ReasonCode(PacketTypes.CONNACK, "Success")
+        rc_protocol_error = ReasonCode(PacketTypes.CONNACK, "Protocol error")
 
         assert not rc_success > 0
         assert rc_protocol_error > 0
         assert not rc_success != 0
         assert rc_protocol_error != 0
+
+    def test_compatibility(self):
+        rc_success = ReasonCode(PacketTypes.CONNACK, "Success")
+        with pytest.deprecated_call():
+            rc_success_old = ReasonCodes(PacketTypes.CONNACK, "Success")
+        assert rc_success == rc_success_old
+
+        assert isinstance(rc_success, ReasonCode)
+        assert isinstance(rc_success_old, ReasonCodes)
+        # User might use isinstance with the old name (plural)
+        # while the library give them a ReasonCode (singular) in the callbacks
+        assert isinstance(rc_success, ReasonCodes)
+        # The other way around is probably never used... but still support it
+        assert isinstance(rc_success_old, ReasonCode)
+
+        # Check that isinstance implementation don't always return True
+        assert not isinstance(rc_success, dict)
+        assert not isinstance(rc_success_old, dict)
+        assert not isinstance({}, ReasonCode)
+        assert not isinstance({}, ReasonCodes)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/test_websocket_integration.py` & `paho_mqtt-2.1.0/tests/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/test_websockets.py` & `paho_mqtt-2.1.0/tests/test_websockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import socket
 from unittest.mock import Mock
 
 import pytest
-from paho.mqtt.client import WebsocketConnectionError, WebsocketWrapper
+from paho.mqtt.client import WebsocketConnectionError, _WebsocketWrapper
 
 
 class TestHeaders:
     """ Make sure headers are used correctly """
 
     @pytest.mark.parametrize("wargs,expected_sent", [
         (
@@ -117,15 +117,15 @@
         )
 
         # Do a copy to avoid modifying input
         wargs_with_socket = dict(wargs)
         wargs_with_socket["socket"] = mocksock
 
         with pytest.raises(WebsocketConnectionError) as exc:
-            WebsocketWrapper(**wargs_with_socket)
+            _WebsocketWrapper(**wargs_with_socket)
 
         # We're not creating the response hash properly so it should raise this
         # error
         assert str(exc.value) == "WebSocket handshake error, invalid secret key"
 
         # Only sends the header once
         assert mocksock.send.call_count == 1
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/conftest.py` & `paho_mqtt-2.1.0/tests/lib/conftest.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_asyncio.py` & `paho_mqtt-2.1.0/tests/lib/test_01_asyncio.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_decorators.py` & `paho_mqtt-2.1.0/tests/lib/test_01_decorators.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_keepalive_pingreq.py` & `paho_mqtt-2.1.0/tests/lib/test_01_keepalive_pingreq.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_no_clean_session.py` & `paho_mqtt-2.1.0/tests/lib/test_01_no_clean_session.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_reconnect_on_failure.py` & `paho_mqtt-2.1.0/tests/lib/test_01_reconnect_on_failure.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_empty_password_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_unpwd_empty_password_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_empty_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_unpwd_empty_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_unpwd_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_unpwd_unicode_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_unpwd_unicode_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_will_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_will_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_will_unpwd_set.py` & `paho_mqtt-2.1.0/tests/lib/test_01_will_unpwd_set.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_01_zero_length_clientid.py` & `paho_mqtt-2.1.0/tests/lib/test_01_zero_length_clientid.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos0.py` & `paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos0.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos1.py` & `paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos1.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_02_subscribe_qos2.py` & `paho_mqtt-2.1.0/tests/lib/test_02_subscribe_qos2.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_02_unsubscribe.py` & `paho_mqtt-2.1.0/tests/lib/test_02_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_b2c_qos1.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos0.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Test whether a client responds correctly to a PUBLISH with QoS 1.
+# Test whether a client sends a correct PUBLISH to a topic with QoS 0.
+# Use paho.mqtt.publish helper for that.
 
 # The client should connect with keepalive=60, clean session set,
-# and client id publish-qos1-test
+# and client id publish-helper-qos0-test
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
-# the CONNACK the client should verify that rc==0.
-# The test will send the client a PUBLISH message with topic
-# "pub/qos1/receive", payload of "message", QoS=1 and mid=123. The client
-# should handle this as per the spec by sending a PUBACK message.
-# The client should then exit with return code==0.
-import pytest
+# the CONNACK and verifying that rc=0, the client should send a PUBLISH message
+# to topic "pub/qos0/test" with payload "message" and QoS=0. If rc!=0, the
+# client should exit with an error.
+# After sending the PUBLISH message, the client should send a
+# DISCONNECT message.
+
 
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("publish-qos1-test", keepalive=60)
+connect_packet = paho_test.gen_connect(
+    "publish-helper-qos0-test", keepalive=60,
+)
 connack_packet = paho_test.gen_connack(rc=0)
 
-disconnect_packet = paho_test.gen_disconnect()
-
-mid = 123
 publish_packet = paho_test.gen_publish(
-    "pub/qos1/receive", qos=1, mid=mid, payload="message")
-puback_packet = paho_test.gen_puback(mid)
+    "pub/qos0/test", qos=0, payload="message"
+)
+
+disconnect_packet = paho_test.gen_disconnect()
 
 
-# msg.retain changed when typing was added
-@pytest.mark.xfail
-def test_03_publish_b2c_qos1(server_socket, start_client):
-    start_client("03-publish-b2c-qos1.py")
+def test_03_publish_helper_qos0(server_socket, start_client):
+    start_client("03-publish-helper-qos0.py")
 
     (conn, address) = server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
-    conn.send(publish_packet)
 
-    paho_test.expect_packet(conn, "puback", puback_packet)
+    paho_test.expect_packet(conn, "publish", publish_packet)
+    paho_test.expect_packet(conn, "disconnect", disconnect_packet)
 
     conn.close()
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_c2b_qos1_disconnect.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_c2b_qos1_disconnect.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_c2b_qos2_disconnect.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_c2b_qos2_disconnect.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_fill_inflight.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_fill_inflight.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos0.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_qos0.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # Test whether a client sends a correct PUBLISH to a topic with QoS 0.
-# Use paho.mqtt.publish helper for that.
 
 # The client should connect with keepalive=60, clean session set,
-# and client id publish-helper-qos0-test
+# and client id publish-qos0-test
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
 # the CONNACK and verifying that rc=0, the client should send a PUBLISH message
 # to topic "pub/qos0/test" with payload "message" and QoS=0. If rc!=0, the
 # client should exit with an error.
-# After sending the PUBLISH message, the client should send a
-# DISCONNECT message.
+# After sending the PUBLISH message, the client should send a DISCONNECT message.
 
 
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect(
-    "publish-helper-qos0-test", keepalive=60,
-)
+connect_packet = paho_test.gen_connect("publish-qos0-test", keepalive=60)
 connack_packet = paho_test.gen_connack(rc=0)
 
-publish_packet = paho_test.gen_publish(
-    "pub/qos0/test", qos=0, payload="message"
-)
+publish_packet = paho_test.gen_publish("pub/qos0/test", qos=0, payload="message")
 
 disconnect_packet = paho_test.gen_disconnect()
 
 
-def test_03_publish_helper_qos0(server_socket, start_client):
-    start_client("03-publish-helper-qos0.py")
-
+def test_03_publish_qos0(server_socket, start_client):
+    start_client("03-publish-qos0.py")
     (conn, address) = server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
 
     paho_test.expect_packet(conn, "publish", publish_packet)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos0_v5.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos0_v5.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_helper_qos1_disconnect.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_helper_qos1_disconnect.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_qos0.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_qos0_no_payload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Test whether a client sends a correct PUBLISH to a topic with QoS 0.
+# Test whether a client sends a correct PUBLISH to a topic with QoS 0 and no payload.
 
 # The client should connect with keepalive=60, clean session set,
-# and client id publish-qos0-test
+# and client id publish-qos0-test-np
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
 # the CONNACK and verifying that rc=0, the client should send a PUBLISH message
-# to topic "pub/qos0/test" with payload "message" and QoS=0. If rc!=0, the
-# client should exit with an error.
+# to topic "pub/qos0/no-payload/test" with zero length payload and QoS=0. If
+# rc!=0, the client should exit with an error.
 # After sending the PUBLISH message, the client should send a DISCONNECT message.
 
 
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("publish-qos0-test", keepalive=60)
+connect_packet = paho_test.gen_connect("publish-qos0-test-np", keepalive=60)
 connack_packet = paho_test.gen_connack(rc=0)
 
-publish_packet = paho_test.gen_publish("pub/qos0/test", qos=0, payload="message")
+publish_packet = paho_test.gen_publish("pub/qos0/no-payload/test", qos=0)
 
 disconnect_packet = paho_test.gen_disconnect()
 
 
-def test_03_publish_qos0(server_socket, start_client):
-    start_client("03-publish-qos0.py")
+def test_03_publish_qos0_no_payload(server_socket, start_client):
+    start_client("03-publish-qos0-no-payload.py")
+
     (conn, address) = server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
 
     paho_test.expect_packet(conn, "publish", publish_packet)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_03_publish_qos0_no_payload.py` & `paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_alpn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-# Test whether a client sends a correct PUBLISH to a topic with QoS 0 and no payload.
-
+# Test whether a client produces a correct connect and subsequent disconnect when using SSL.
+# Client must provide a certificate.
+#
 # The client should connect with keepalive=60, clean session set,
-# and client id publish-qos0-test-np
+# and client id 08-ssl-connect-alpn
+# It should use the CA certificate ssl/all-ca.crt for verifying the server.
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
-# the CONNACK and verifying that rc=0, the client should send a PUBLISH message
-# to topic "pub/qos0/no-payload/test" with zero length payload and QoS=0. If
-# rc!=0, the client should exit with an error.
-# After sending the PUBLISH message, the client should send a DISCONNECT message.
-
+# the CONNACK and verifying that rc=0, the client should send a DISCONNECT
+# message. If rc!=0, the client should exit with an error.
+#
+# Additionally, the secure socket must have been negotiated with the "paho-test-protocol"
 
-import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("publish-qos0-test-np", keepalive=60)
-connack_packet = paho_test.gen_connack(rc=0)
+from tests import paho_test
+from tests.paho_test import ssl
 
-publish_packet = paho_test.gen_publish("pub/qos0/no-payload/test", qos=0)
 
-disconnect_packet = paho_test.gen_disconnect()
+def test_08_ssl_connect_alpn(alpn_ssl_server_socket, start_client):
+    connect_packet = paho_test.gen_connect("08-ssl-connect-alpn", keepalive=60)
+    connack_packet = paho_test.gen_connack(rc=0)
+    disconnect_packet = paho_test.gen_disconnect()
 
+    start_client("08-ssl-connect-alpn.py")
 
-def test_03_publish_qos0_no_payload(server_socket, start_client):
-    start_client("03-publish-qos0-no-payload.py")
-
-    (conn, address) = server_socket.accept()
+    (conn, address) = alpn_ssl_server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
 
-    paho_test.expect_packet(conn, "publish", publish_packet)
     paho_test.expect_packet(conn, "disconnect", disconnect_packet)
 
+    if ssl.HAS_ALPN:
+        negotiated_protocol = conn.selected_alpn_protocol()
+        if negotiated_protocol != "paho-test-protocol":
+            raise Exception(f"Unexpected protocol '{negotiated_protocol}'")
+
     conn.close()
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_04_retain_qos0.py` & `paho_mqtt-2.1.0/tests/lib/test_04_retain_qos0.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_alpn.py` & `paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_cert_auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 # Test whether a client produces a correct connect and subsequent disconnect when using SSL.
 # Client must provide a certificate.
 #
 # The client should connect with keepalive=60, clean session set,
-# and client id 08-ssl-connect-alpn
+# and client id 08-ssl-connect-crt-auth
 # It should use the CA certificate ssl/all-ca.crt for verifying the server.
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
 # the CONNACK and verifying that rc=0, the client should send a DISCONNECT
 # message. If rc!=0, the client should exit with an error.
-#
-# Additionally, the secure socket must have been negotiated with the "paho-test-protocol"
-
 
-from tests import paho_test
-from tests.paho_test import ssl
+import tests.paho_test as paho_test
 
+connect_packet = paho_test.gen_connect("08-ssl-connect-crt-auth", keepalive=60)
+connack_packet = paho_test.gen_connack(rc=0)
+disconnect_packet = paho_test.gen_disconnect()
 
-def test_08_ssl_connect_alpn(alpn_ssl_server_socket, start_client):
-    connect_packet = paho_test.gen_connect("08-ssl-connect-alpn", keepalive=60)
-    connack_packet = paho_test.gen_connack(rc=0)
-    disconnect_packet = paho_test.gen_disconnect()
 
-    start_client("08-ssl-connect-alpn.py")
+def test_08_ssl_connect_crt_auth(ssl_server_socket, start_client):
+    start_client("08-ssl-connect-cert-auth.py")
 
-    (conn, address) = alpn_ssl_server_socket.accept()
+    (conn, address) = ssl_server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
 
     paho_test.expect_packet(conn, "disconnect", disconnect_packet)
 
-    if ssl.HAS_ALPN:
-        negotiated_protocol = conn.selected_alpn_protocol()
-        if negotiated_protocol != "paho-test-protocol":
-            raise Exception(f"Unexpected protocol '{negotiated_protocol}'")
-
     conn.close()
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_cert_auth.py` & `paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_cert_auth_pw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Test whether a client produces a correct connect and subsequent disconnect when using SSL.
-# Client must provide a certificate.
+# Client must provide a certificate - the private key is encrypted with a password.
 #
 # The client should connect with keepalive=60, clean session set,
 # and client id 08-ssl-connect-crt-auth
 # It should use the CA certificate ssl/all-ca.crt for verifying the server.
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
 # the CONNACK and verifying that rc=0, the client should send a DISCONNECT
 # message. If rc!=0, the client should exit with an error.
 
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("08-ssl-connect-crt-auth", keepalive=60)
+connect_packet = paho_test.gen_connect("08-ssl-connect-crt-auth-pw", keepalive=60)
 connack_packet = paho_test.gen_connack(rc=0)
 disconnect_packet = paho_test.gen_disconnect()
 
 
-def test_08_ssl_connect_crt_auth(ssl_server_socket, start_client):
-    start_client("08-ssl-connect-cert-auth.py")
+def test_08_ssl_connect_crt_auth_pw(ssl_server_socket, start_client):
+    start_client("08-ssl-connect-cert-auth-pw.py")
 
     (conn, address) = ssl_server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_cert_auth_pw.py` & `paho_mqtt-2.1.0/tests/lib/test_08_ssl_connect_no_auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # Test whether a client produces a correct connect and subsequent disconnect when using SSL.
-# Client must provide a certificate - the private key is encrypted with a password.
 #
-# The client should connect with keepalive=60, clean session set,
-# and client id 08-ssl-connect-crt-auth
+# The client should connect with keepalive=60, clean session set,# and client id 08-ssl-connect-no-auth
 # It should use the CA certificate ssl/all-ca.crt for verifying the server.
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
 # the CONNACK and verifying that rc=0, the client should send a DISCONNECT
 # message. If rc!=0, the client should exit with an error.
-
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("08-ssl-connect-crt-auth-pw", keepalive=60)
+connect_packet = paho_test.gen_connect("08-ssl-connect-no-auth", keepalive=60)
 connack_packet = paho_test.gen_connack(rc=0)
 disconnect_packet = paho_test.gen_disconnect()
 
 
-def test_08_ssl_connect_crt_auth_pw(ssl_server_socket, start_client):
-    start_client("08-ssl-connect-cert-auth-pw.py")
+def test_08_ssl_connect_no_auth(ssl_server_socket, start_client):
+    start_client("08-ssl-connect-no-auth.py")
 
     (conn, address) = ssl_server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/test_08_ssl_connect_no_auth.py` & `paho_mqtt-2.1.0/tests/lib/test_03_publish_b2c_qos1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-# Test whether a client produces a correct connect and subsequent disconnect when using SSL.
-#
-# The client should connect with keepalive=60, clean session set,# and client id 08-ssl-connect-no-auth
-# It should use the CA certificate ssl/all-ca.crt for verifying the server.
+# Test whether a client responds correctly to a PUBLISH with QoS 1.
+
+# The client should connect with keepalive=60, clean session set,
+# and client id publish-qos1-test
 # The test will send a CONNACK message to the client with rc=0. Upon receiving
-# the CONNACK and verifying that rc=0, the client should send a DISCONNECT
-# message. If rc!=0, the client should exit with an error.
+# the CONNACK the client should verify that rc==0.
+# The test will send the client a PUBLISH message with topic
+# "pub/qos1/receive", payload of "message", QoS=1 and mid=123. The client
+# should handle this as per the spec by sending a PUBACK message.
+# The client should then exit with return code==0.
 import tests.paho_test as paho_test
 
-connect_packet = paho_test.gen_connect("08-ssl-connect-no-auth", keepalive=60)
+connect_packet = paho_test.gen_connect("publish-qos1-test", keepalive=60)
 connack_packet = paho_test.gen_connack(rc=0)
+
 disconnect_packet = paho_test.gen_disconnect()
 
+mid = 123
+publish_packet = paho_test.gen_publish(
+    "pub/qos1/receive", qos=1, mid=mid, payload="message")
+puback_packet = paho_test.gen_puback(mid)
+
 
-def test_08_ssl_connect_no_auth(ssl_server_socket, start_client):
-    start_client("08-ssl-connect-no-auth.py")
+def test_03_publish_b2c_qos1(server_socket, start_client):
+    start_client("03-publish-b2c-qos1.py")
 
-    (conn, address) = ssl_server_socket.accept()
+    (conn, address) = server_socket.accept()
     conn.settimeout(10)
 
     paho_test.expect_packet(conn, "connect", connect_packet)
     conn.send(connack_packet)
+    conn.send(publish_packet)
 
-    paho_test.expect_packet(conn, "disconnect", disconnect_packet)
+    paho_test.expect_packet(conn, "puback", puback_packet)
 
     conn.close()
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/01-asyncio.py` & `paho_mqtt-2.1.0/tests/lib/clients/01-asyncio.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/01-decorators.py` & `paho_mqtt-2.1.0/tests/lib/clients/01-decorators.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/01-zero-length-clientid.py` & `paho_mqtt-2.1.0/tests/lib/clients/01-zero-length-clientid.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos0.py` & `paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos0.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos1.py` & `paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos1.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/02-subscribe-qos2.py` & `paho_mqtt-2.1.0/tests/lib/clients/02-subscribe-qos2.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/02-unsubscribe.py` & `paho_mqtt-2.1.0/tests/lib/clients/02-unsubscribe.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-b2c-qos1.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-b2c-qos1.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def on_message(mqttc, obj, msg):
     assert msg.mid == 123, f"Invalid mid: ({msg.mid})"
     assert msg.topic == "pub/qos1/receive", f"Invalid topic: ({msg.topic})"
     assert msg.payload == expected_payload, f"Invalid payload: ({msg.payload})"
     assert msg.qos == 1, f"Invalid qos: ({msg.qos})"
-    assert msg.retain is not False, f"Invalid retain: ({msg.retain})"
+    assert not msg.retain, f"Invalid retain: ({msg.retain})"
 
 
 def on_connect(mqttc, obj, flags, rc):
     assert rc == 0, f"Connect failed ({rc})"
 
 
 mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION1, "publish-qos1-test")
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-b2c-qos2.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-b2c-qos2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+import logging
+
 import paho.mqtt.client as mqtt
 
-from tests.paho_test import get_test_server_port, wait_for_keyboard_interrupt
+from tests.paho_test import get_test_server_port, loop_until_keyboard_interrupt
 
 expected_payload = b"message"
 
 
 def on_message(mqttc, obj, msg):
     assert msg.mid == 13423, f"Invalid mid: ({msg.mid})"
     assert msg.topic == "pub/qos2/receive", f"Invalid topic: ({msg.topic})"
     assert msg.payload == expected_payload, f"Invalid payload: ({msg.payload})"
     assert msg.qos == 2, f"Invalid qos: ({msg.qos})"
-    assert msg.retain is not False, f"Invalid retain: ({msg.retain})"
+    assert not msg.retain, f"Invalid retain: ({msg.retain})"
 
 
 def on_connect(mqttc, obj, flags, rc):
     assert rc == 0, f"Connect failed ({rc})"
 
-
+logging.basicConfig(level=logging.DEBUG)
 mqttc = mqtt.Client(mqtt.CallbackAPIVersion.VERSION1, "publish-qos2-test", clean_session=True)
+mqttc.enable_logger()
 mqttc.on_connect = on_connect
 mqttc.on_message = on_message
 
 mqttc.connect("localhost", get_test_server_port())
-
-with wait_for_keyboard_interrupt():
-    while True:
-        if mqttc.loop(0.3):
-            break
+loop_until_keyboard_interrupt(mqttc)
```

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-c2b-qos1-disconnect.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-c2b-qos1-disconnect.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-c2b-qos2-disconnect.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-c2b-qos2-disconnect.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-fill-inflight.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-fill-inflight.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-qos0-no-payload.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-qos0-no-payload.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/03-publish-qos0.py` & `paho_mqtt-2.1.0/tests/lib/clients/03-publish-qos0.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-alpn.py` & `paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-alpn.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-cert-auth-pw.py` & `paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-cert-auth-pw.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-connect-cert-auth.py` & `paho_mqtt-2.1.0/tests/lib/clients/08-ssl-connect-cert-auth.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/lib/clients/08-ssl-fake-cacert.py` & `paho_mqtt-2.1.0/tests/lib/clients/08-ssl-fake-cacert.py`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/all-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/all-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client-expired.crt` & `paho_mqtt-2.1.0/tests/ssl/client-expired.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client-pw.crt` & `paho_mqtt-2.1.0/tests/ssl/client-pw.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client-pw.key` & `paho_mqtt-2.1.0/tests/ssl/client-pw.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client-revoked.crt` & `paho_mqtt-2.1.0/tests/ssl/client-revoked.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client-revoked.key` & `paho_mqtt-2.1.0/tests/ssl/client-revoked.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client.crt` & `paho_mqtt-2.1.0/tests/ssl/client.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/client.key` & `paho_mqtt-2.1.0/tests/ssl/client.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/crl.pem` & `paho_mqtt-2.1.0/tests/ssl/crl.pem`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/gen.sh` & `paho_mqtt-2.1.0/tests/ssl/gen.sh`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/openssl.cnf` & `paho_mqtt-2.1.0/tests/ssl/openssl.cnf`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/server-expired.crt` & `paho_mqtt-2.1.0/tests/ssl/server-expired.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/server.crt` & `paho_mqtt-2.1.0/tests/ssl/server.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/server.key` & `paho_mqtt-2.1.0/tests/ssl/server.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-alt-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/test-alt-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-alt-ca.key` & `paho_mqtt-2.1.0/tests/ssl/test-alt-ca.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-bad-root-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/test-bad-root-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-bad-root-ca.key` & `paho_mqtt-2.1.0/tests/ssl/test-bad-root-ca.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-fake-root-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/test-fake-root-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-fake-root-ca.key` & `paho_mqtt-2.1.0/tests/ssl/test-fake-root-ca.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-root-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/test-root-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-root-ca.key` & `paho_mqtt-2.1.0/tests/ssl/test-root-ca.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-signing-ca.crt` & `paho_mqtt-2.1.0/tests/ssl/test-signing-ca.crt`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/ssl/test-signing-ca.key` & `paho_mqtt-2.1.0/tests/ssl/test-signing-ca.key`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/tests/testsupport/broker.py` & `paho_mqtt-2.1.0/tests/testsupport/broker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import contextlib
+import os
 import socket
 import socketserver
 import threading
 
 import pytest
 
 from tests import paho_test
 
 
 class FakeBroker:
-    def __init__(self):
-        # Bind to "localhost" for maximum performance, as described in:
-        # http://docs.python.org/howto/sockets.html#ipc
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+    def __init__(self, transport):
+        if transport == "tcp":
+            # Bind to "localhost" for maximum performance, as described in:
+            # http://docs.python.org/howto/sockets.html#ipc
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            sock.bind(("localhost", 0))
+            self.port = sock.getsockname()[1]
+        elif transport == "unix":
+            sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
+            sock.bind("localhost")
+            self.port = 1883
+        else:
+            raise ValueError(f"unsupported transport {transport}")
+
         sock.settimeout(5)
-        sock.bind(("localhost", 0))
-        self.port = sock.getsockname()[1]
         sock.listen(1)
 
         self._sock = sock
         self._conn = None
+        self.transport = transport
 
     def start(self):
         if self._sock is None:
             raise ValueError('Socket is not open')
 
         (conn, address) = self._sock.accept()
         conn.settimeout(5)
@@ -35,14 +45,20 @@
             self._conn.close()
             self._conn = None
 
         if self._sock is not None:
             self._sock.close()
             self._sock = None
 
+        if self.transport == 'unix':
+            try:
+              os.unlink('localhost')
+            except OSError:
+              pass
+
     def receive_packet(self, num_bytes):
         if self._conn is None:
             raise ValueError('Connection is not open')
 
         packet_in = self._conn.recv(num_bytes)
         return packet_in
 
@@ -56,18 +72,18 @@
     def expect_packet(self, name, packet):
         if self._conn is None:
             raise ValueError('Connection is not open')
 
         paho_test.expect_packet(self._conn, name, packet)
 
 
-@pytest.fixture
-def fake_broker():
+@pytest.fixture(params=["tcp"] + (["unix"] if hasattr(socket, 'AF_UNIX') else []))
+def fake_broker(request):
     # print('Setup broker')
-    broker = FakeBroker()
+    broker = FakeBroker(request.param)
 
     yield broker
 
     # print('Teardown broker')
     broker.finish()
```

### Comparing `paho_mqtt-2.0.0rc2/.gitignore` & `paho_mqtt-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `paho_mqtt-2.0.0rc2/pyproject.toml` & `paho_mqtt-2.1.0/pyproject.toml`

 * *Files identical despite different names*

